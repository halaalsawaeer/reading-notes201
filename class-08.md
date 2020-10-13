
CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.

If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.

CSS has the following positioning schemes that allow you to control
the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.

To indicate where a box should be positioned, you may also need to use
box offset properties to tell the browser how far from the top or bottom
and left or right it should be placed. 

In normal flow, each block-level
element sits on top of the next
one
Relative positioning moves an
element in relation to where it
would have been in normal flow.
When the position property
is given a value of absolute,
the box is taken out of normal
flow and no longer affects the
position of other elements on
the page

Fixed positioning is a type
of absolute positioning that
requires the position property
to have a value of fixed.
It positions the element in
relation to the browser window.
Therefore, when a user scrolls
down the page, it stays in the
exact same place. 

The float property allows you
to take an element in normal
flow and place it as far to the
left or right of the containing
element as possible.

The clear property allows you
to say that no element (within
the same containing element)
should touch the left or righthand sides of a box. It can take
the following values:
left
The left-hand side of the box
should not touch any other
elements appearing in the same
containing element.
right
The right-hand side of the
box will not touch elements
appearing in the same containing
element.
both
Neither the left nor right-hand
sides of the box will touch
elements appearing in the same
containing element.
none
Elements can touch either side.

Different visitors to your site will have different sized screens that show
different amounts of information, so your design needs to be able to
work on a range of different sized screens.

Resolution refers to the number of dots a screen shows per inch. Some
devices have a higher resolution than desktop computers and most
operating systems allow users to adjust the resolution of their screens.

Because screen sizes and display resolutions vary so much, web
designers often try to create pages of around 960-1000 pixels wide

Fixed width layout
designs do not
change size as the
user increases
or decreases
the size of their
browser window.
Measurements tend
to be given in pixels.

Liquid layout designs
stretch and contract
as the user increases
or decreases the
size of their browser
window. They tend to
use percentages.

CSS frameworks aim to make your life easier by providing the code for
common tasks, such as creating layout grids, styling forms, creating
printer-friendly versions of pages and so on. You can include the CSS
framework code in your projects rather than writing the CSS from scratch.


There are two ways to add
multiple style sheets to a page:
1: Your HTML page can link
to one style sheet and that
stylesheet can use the @import
rule to import other style sheets.
2: In the HTML you can use a
separate <link> element for
each style sheet.

You can include multiple CSS files in one page.

Grids help create professional and flexible designs.

div elements are often used as containing elements
to group together sections of a page.
