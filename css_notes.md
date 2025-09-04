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