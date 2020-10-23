
Links are the defining feature of the web
because they allow you to move from
one web page to another
Links are created using the a element. Users can click on anything
between the opening a tag and the closing a tag. You specify
which page you want to link to using the href attribute.
The text between the opening
<a> tag and closing </a> tag
is known as link text. Where
possible, your link text should
explain where visitors will be
taken if they click on it
Clear link text can help visitors
find what they want.
To write good link text, you can
think of words people might
use when searching for the
page that you are linking to. 
URL stands for Uniform
Resource Locator. Every web
page has its own URL. This is the
web address that you would type
into a browser if you wanted to
visit that specific page.

Relative URLs
When linking to other pages
within the same site, you can
use relative URLs. These are like
a shorthand version of absolute
URLs because you do not need
to specify the domain name.



On larger websites it's a good idea to organize your code by placing the
pages for each different section of the site into a new folder. Folders on a
website are sometimes referred to as directories.

The root folder contains:
● A file called index.html which
is the homepage for the
entire site
● Individual folders
Each sub-directory contains:
● A file called index.html which
is the homepage for that
section
● A reviews page called reviews
.html
● A listings page called listings.html
Every page and every image on
a website has a URL (or Uniform
Resource Locator). The URL is
made up of the domain name
followed by the path to that page
or image.

Relative URLs can be used when linking to pages within your own
website. They provide a shorthand way of telling the browser where to
find your files.
mailto: chapter-04/email-links.html HTML
To create a link that starts up
the user's email program and
addresses an email to a specified
email address, you use the a
element. However, this time the
value of the href attribute starts
with mailto: and is followed by
the email address you want the
email to be sent to.
If you want a link to open in a
new window, you can use the
target attribute on the opening
a tag. The value of this
attribute should be _blank.
Linking to a Specific
Part of the Same Page
Before you can link to a specific
part of a page, you need to
identify the points in the page
that the link will go to. You do
this using the id attribute (which
can be used on every HTML
element). 
To link to an element that uses
an id attribute you use the <a>
element again, but the value of
the href attribute starts with
the # symbol, followed by the
value of the id attribute of the
element you want to link to. 


CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.
If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.

CSS has the following positioning schemes that allow you to control
the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property


To indicate where a box should be positioned, you may also need to use
box offset properties to tell the browser how far from the top or bottom
and left or right it should be placed. (You will meet these when we
introduce the positioning schemes on the following pages.)


Fixed Positioning 
When you move
any element from
normal flow, boxes
can overlap. The
z-index property
allows you to control
which box appears
on top. 

Relative positioning moves an
element in relation to where it
would have been in normal flow

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

When you use relative, fixed, or
absolute positioning, boxes can
overlap. If boxes do overlap, the
elements that appear later in the
HTML code sit on top of those
that are earlier in the page.
If you want to control which
element sits on top, you can use
the z-index property. Its value
is a number, and the higher the
number the closer that element
is to the front. For example, an
element with a z-index of 10
will appear over the top of one
with a z-index of 5.



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

When designing for print, you
always know the size of the
piece of paper that your design
will be printed on. However,
when it comes to designing for
the web, you are faced with the
unique challenge that different
users will have different sized
screens.
Since computers have been sold
to the public, the size of screens
has been steadily increasing.
This means that some people
viewing your site might have 13
inch monitors while others may
have 27+ inch monitors.
Resolution refers to the number of dots a screen shows per inch. Some
devices have a higher resolution than desktop computers and most
operating systems allow users to adjust the resolution of their screens.

Plugins are scripts that extend the functionality of the jQuery library.
Hundreds have been written and are available for you to use. 
jQuery is an example of what programmers call a JavaScript library.
It is a JavaScript file that you include in your page, which then lets you
use the functions, objects, methods, and properties it contains. 

Ajax is a technique for loading data into part of a page
without having to refresh the entire page. The data is often
sent in a format called JavaScript Object Notation (or JSON). 
Ajax uses an asynchronous processing model. This means the user can
do other things while the web browser is waiting for the data to load,
speeding up the user experience. 


Data can be formatted using JSON (pronounced "Jason").
It looks very similar to object literal syntax, but it is not an object. 

JavaScript's JSON object can turn JSON data into a JavaScript object.
It can also convert a JavaScript object into a string. 
HTML is the easiest type of data to add into a page using Ajax.
The browser renders it just like any other HTML.
The CSS rules for the rest of the page are applied to the new content. 
Requesting XML data is very similar to requesting HTML. However,
processing the data that is returned is more complicated because the
XML must be converted into HTML to be shown on the page
jQuery provides several methods that handle Ajax requests.
Just like other examples in this chapter, the process involves two steps:
making a request and handling the response. 
Ajax refers to a group of technologies that allow you to
update just one part of the page (rather than reload a
whole page).
You can incorporate HTML, XML, or JSON data into
your pages. (JSON is becoming increasingly popular.)
To load JSON from a different domain, you can use
JSONP but only if the code is from a trusted source.
jQuery has methods that make it easier to use Ajax .
. load() is the simplest way to load HTML into your
pages and allows you to update just a part of the page .
. aj ax () is more powerful and more complex. (Several
shorthand methods are also offered.)
It is important to consider how the site will work if the
user does not have JavaScript enabled, or if the page is
not able to access the data from a server. 
