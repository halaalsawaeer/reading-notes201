Traditionally, the term 'form' has referred
to a printed document that contains
spaces for you to fill in information.

HTML borrows the concept of a form to refer to different
elements that allow you to collect information from visitors to
your site.

There are several types of form controls that
you can use to collect information from visitors
to your site.

ADDING TEXT:
Making Choices:
Submitting Forms: Uploading Files:
Password input
Like a single line text box but it
masks the characters entered.
Text input (single-line)
Used for a single line of text such
as email addresses and names.
Text area (multi-line)
For longer areas of text, such as
messages and comments.
Checkboxes
When a user can select and
unselect one or more options.
Radio buttons
For use when a user must select
one of a number of options.
Drop-down boxes
When a user must pick one of a
number of options from a list.
Image buttons
Similar to submit buttons but
they allow you to use an image.
Submit buttons
To submit data from your form
to another web page.
File upload
Allows users to upload files
(e.g. images) to a website.

A form may have several form controls, each
gathering different information. The server
needs to know which piece of inputted data
corresponds with which form element.

form
Form controls live inside a
form element. This element
should always carry the action
attribute and will usually have a
method and id attribute too.
input
The input element is used
to create several different form
controls. The value of the type
attribute determines what kind
of input they will be creating
textarea
The textarea element
is used to create a mutli-line
text input. Unlike other input
elements this is not an empty
element. It should therefore have
an opening and a closing tag. 

input
type="radio"
Radio buttons allow users to pick
just one of a number of options.

input
type="checkbox"
Checkboxes allow users to select
(and unselect) one or more
options in answer to a question.

select
A drop down list box (also
known as a select box) allows
users to select one option from a
drop down list. 

option
The option element is used
to specify the options that the
user can select from. The words
between the opening option
and closing option tags will
be shown to the user in the drop
down box.

input
If you want to allow users to
upload a file (for example an
image, video, mp3, or a PDF),
you will need to use a file input
box.
type="file"
This type of input creates a
box that looks like a text input
followed by a browse button. 

<button>
The <button> element was
introduced to allow users more
control over how their buttons
appear, and to allow other
elements to appear inside the
button.

fieldset
You can group related form
controls together inside the
fieldset element. This is
particularly helpful for longer
forms.
legend
The legend element can
come directly after the opening
fieldset tag and contains a
caption which helps identify the
purpose of that group of form
controls.
You have probably seen forms
on the web that give users
messages if the form control has
not been filled in correctly; this is
known as form validation.


type="date"
If you are asking the user for a
date, you can use an <input>
element and give the type
attribute a value of date.
This will create a date input in
browsers that support the new
HMTL5 input types. 
type="email"
If you ask a user for an email
address, you can use the email
input. 
type="search"
If you want to create a single
line text box for search queries,
HTML5 provides a special
search input

The list-style-type property
allows you to control the shape
or style of a bullet point (also
known as a marker). 
It can be used on rules that
apply to the <ol>, <ul>, and <li>
elements.
You can specify an image to act
as a bullet point using the
list-style-image property.
The value starts with the letters
url and is followed by a pair
of parentheses. Inside the
parentheses, the path to the
image is given inside double
quotes.
This property can be used on
rules that apply to the ul and
li elements.

You have already met several
properties that are commonly
used with tables. Here we will
put them together in a single
example using the following:
width to set the width of the
table
padding to set the space
between the border of each table
cell and its content
text-transform to convert the
content of the table headers to
uppercase
letter-spacing, font-size
to add additional styling to the
content of the table headers
border-top, border-bottom
to set borders above and below
the table headers
text-align to align the writing
to the left of some table cells and
to the right of the others
background-color to change
the background color of the
alternating table rows
:hover to highlight a table row
when a user's mouse goes over it

If you have empty cells in
your table, then you can use
the empty-cells property to
specify whether or not their
borders should be shown.
Since browsers treat empty cells
in different ways, if you want to
explicitly show or hide borders
on any empty cells then you
should use this property.
It can take one of three values:
show
This shows the borders of any
empty cells.
hide
This hides the borders of any
empty cells.

The border-spacing property
allows you to control the
distance between adjacent cells.
By default, browsers often leave
a small gap between each table
cell, so if you want to increase
or decrease this space then
the border-spacing property
allows you to control the gap.

separate
Borders are detached from each
other. (border-spacing and
empty-cells will be obeyed.)

Here are some properties that
can be used to style submit
buttons.
color is used to change the
color of the text on the button.
text-shadow can give a 3D
look to the text in browsers that
support this property.
border-bottom has been used
to make the bottom border of
the button slightly thicker, which
gives it a more 3D feel.
background-color can make
the submit button stand out
from other items around it. 

The :hover pseudo-class
has been used to change the
appearance of the button when
the user hovers over it.

The cursor property allows
you to control the type of mouse
cursor that should be displayed
to users.

Once you have included the Google Maps script in your page, you can
use their maps object. It lets you display Google maps in your pages. 

 Starting at the bottom of the script, when the
page has loaded, the on load event will call the
l oadScri pt () function.
2. l oadScri pt() creates a <script> element to load
the Google Maps API. W hen it has loaded, it calls
i nit (), to initialize the map.
3. i nit() loads the map into the HTML page. First it
creates a mapOpti ons object with three properties.
4. Then it uses the Map () constructor to create
a map and draw the map into the page. The
constructor takes two parameters:
• The element that the map will appear inside
• The mapOpt ions object 

APPEARANCE OF CONTROLS POSITION OF TH E CONTROL
To alter the appearance and position of map
controls, you add to the mapOpt ions object.
1. To show or hide a control, the key is the name of
the control, and the value is a Boolean (true will
show the control; fa 1 se will hide it).
2. Each control has its own options object used to
control its style and position. The word Options
follows the control name, e.g., zoomControlOptions.
Styles are discussed below. The diagram on the lefth

 style the map you need to specify three things:
• feature Types: the map feature you want to style:
e.g., roads, parks, waterways, public transport.
The first sty 1 ers property alters the colors of the
map as a whole. It, too, contains an array of objects.
• hue property adjusts color, its value is a hex code
• e 1 ementTypes: the part of that feature you want
to style, such as its geometry (shapes) or labels.
• stylers: properties that allow you to adjust the
color or visibility of items on the map.
The st yles property in the mapOptions object sets
the map style. It's value is an array of objects.
Each object affects a different feature fo the map. 


-----------------------------------------------------
When an event has occurred, it is often described as having fired or
been raised. In the diagram on the right, if the user is tapping on a link, a
cl ick event would fire in the browser. 

Event listeners are a more recent approach to handling events.
They can deal with more than one function at a time
but they are not supported in older browsers. 

Because you cannot have parentheses after the
function names in event handlers or listeners,
passing arguments requires a workaround. 

User interface CUI) events occur as a result of interaction with the
browser window rather than the HTML page contained within it,
e.g., a page having loaded or the browser window being resized. 

he mouse events are fired when the mouse is moved and also when its
buttons are clicked. 
The keyboard events are fired when a user interacts with the keyboard
(they fire on any kind of device with a keyboard). 

Binding is the process of stating which event you are
waiting to happen, and which element you are waiting
for that event to happen upon. 

When an event occurs on an element, it can trigger a
JavaScript function. When this function then changes
the web page in some way, it feels interactive because
it has responded to the user. 
You can use event delegation to monitor for events
that happen on all of the children of an element. 

The most commonly used events are W3C DOM
events, although there are others in the HTMLS
specification as well as browser-specific events. 
