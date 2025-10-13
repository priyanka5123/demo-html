✅ Task 1: Flexbox Property Definitions
Property	Definition/Explanation
display: flex:	Defines the element as a flex container, enabling flexbox layout for its children.
justify-content: center:	Horizontally centers flex items along the main axis.
flex-direction: row-reverse	Changes the direction of the main axis to row but in reverse (right-to-left).
flex-wrap: wrap:	Allows flex items to wrap onto multiple lines if they can’t fit in one row or column.
align-items: center:	Vertically aligns flex items to the center of the cross axis.
flex-grow:	Defines how much a flex item should grow relative to others in the container.
flex-shrink: Controls how much a flex item should shrink when there’s not enough space.
align-content:	Aligns multiple rows of flex items along the cross axis when there's extra space.

✅ Task 2: Flexbox Property Matching
Flexbox Property	Function/Description
justify-content: space-between	e) Space is distributed evenly between and around items in a flex container.
align-items: flex-end	a) Defines how items are aligned along the main axis.
flex-direction: column	b) Defines whether the flex container is a row or a column.
flex-wrap: nowrap	d) Items will not wrap, and overflow the container.
flex-grow: 1	c) Allows items to shrink or grow to fit the container.

✅ Task 3: Reflection Questions

Q1: What is the primary advantage of using flexbox for layouts compared to traditional methods like floats?
Answer:
Flexbox provides a more efficient and responsive way to lay out items in a container. Unlike floats, Flexbox allows for easy vertical and horizontal alignment, dynamic resizing, spacing, and ordering of elements without needing extra CSS hacks or clearfixes.

Q2: What does the flex-direction property control in a flex container, and how does it affect item alignment?
Answer:
The flex-direction property controls the main axis direction of the container — whether items are laid out in a row (horizontally) or a column (vertically), and whether in normal or reverse order. It affects how items are aligned and in which direction they flow.

Q3: What happens when you set flex-wrap to wrap in a flex container with many items?
Answer:
When flex-wrap: wrap is set, the flex items will move to the next line if there isn’t enough space in one row or column. This prevents overflow and allows items to be displayed more neatly across multiple lines.
