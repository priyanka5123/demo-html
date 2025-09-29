Theory: CSS Concepts

1.What is CSS and why do we use it?
CSS stands for Cascading Style Sheets.
It’s a language used to describe the style and appearance of HTML elements on a webpage.

2.What is the difference between an HTML element, a class selector and an ID selector?
An HTML element selector styles all instances of a tag (e.g., p {} for all paragraphs), a class selector (.classname {}) styles multiple elements sharing the same class, and an ID selector (#idname {}) styles a single unique element with that ID.


3. Explain the difference between inline styles, internal CSS, and external CSS. Which one are we using in our demo and why?
Inline styles apply CSS directly inside an element’s style attribute, internal CSS is written inside a <style> tag in the HTML file, and external CSS is placed in a separate .css file linked to the HTML; in our demo, we’re using external CSS because it keeps code cleaner, reusable, and easier to maintain.



4. In the CSS rule below, identify the selector, property, and value:
.first-article {
  background-color: purple;
}


Selector: .first-article
Property: background-color
Value: purple

5. What does border-radius: 20px; do to an element?
A 20px radius means each corner of the element will be curved like a quarter of a circle with a radius of 20 pixels.Example: A rectangular button with border-radius: 20px; will have soft, rounded corners instead of sharp edges.

6. Why do we use the font-family property? What happens if the browser doesn’t have the first font listed?
We use the font-family property to define the text’s typeface, and if the browser doesn’t have the first font listed, it automatically falls back to the next available font in the list.


7. Explain what happens if two CSS rules target the same element with different styles (CSS specificity).
When two CSS rules target the same element, the rule with higher specificity (ID > class > element) or the one declared later in the CSS overrides the other.

8. Look at this HTML snippet from the demo and explain what will be styled by .second-h2 in the CSS file:
<div class="second-article">
  <h2 class="second-h2">I am another div</h2>
</div>

The CSS selector .second-h2 will style the <h2> element inside the <div> because the <h2> has the class second-h2. 

So, any CSS rules under .second-h2 { ... } will apply only to that <h2> element, not the <div> or other elements.

The browser really creates a box for every element under the hood. It doesn't know the meaning of your element. It only knows that those elements are boxes and they have certain sizes and different dimensions, it does some calculations to render things on your screen.

1.What is the Box Model in CSS?
Describe the Box Model and how it helps determine the size of an element on a webpage.
Answer: The Box Model represents every HTML element as a box made up of content, padding, border, and margin. It helps determine the element's total size and spacing on a webpage.


2.Explain the difference between padding and margin.
How does padding affect an element differently from the margin?
Answer:Padding is the space inside the element, between content and border; margin is the space outside the border, separating elements.


3.How does the browser calculate the total size of an element?
Consider the content size, padding, border, and margin. Write a formula that represents the total width and height of an element.
Answer:Total Width = content width + padding (left + right) + border (left + right) + margin(left + right)
Total Height = content height + padding (top + bottom) + border (top + bottom) + margin (top + bottom).


4.Where can you find the Box Model in the browser’s developer tools?
Describe how to access the Box Model in the dev tools to inspect an element's size and spacing.
Answer:Right-click an element, select Inspect, and scroll to the "Computed" tab in dev tools; the Box Model diagram shows size, padding, border, and margin.


5.Why is it important to understand the Box Model when designing a webpage?
Explain how understanding the Box Model can help you control the layout and spacing of elements on a webpage.
Answer:It helps you control spacing and layout accurately, avoiding unexpected element sizes and overlaps.

1. Which parts of your layout were most affected by changes in padding?
Ans: The internal spacing of .box and .card elements was most affected — content moved inward, increasing the overall element size.

2. How did changing the margin affect the spacing between cards?
Ans: Larger margins increased the space between the cards, pushing them further apart vertically and horizontally.

3. Did increasing the border thickness impact the layout? How?
Ans: Yes — it added to the total box size, slightly shifting elements by increasing the space they occupy on the page.

4. How does the Box Model help you design balanced, readable components?
Ans: It helps control spacing (inside and outside elements), ensuring consistent alignment, padding for readability, and margins for clean separation.