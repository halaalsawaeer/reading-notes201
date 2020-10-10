

What is the hardest thing about writing code?
There are many common answers to this question:
•	Learning a new technology
•	Naming things
•	Testing your code
•	Debugging
•	Fixing bugs
•	Making software maintainable



If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:
1.	Make the problem domain easier
2.	Get better at understanding the problem domain

 it is often beneficial to take a part of the problem and fully understand that part before expanding the problem domain.


IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES
IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS

literal notation is a way to create an object.
the object is stored in a variable
you can access the properties or methods using dot notation.
you can also access properties using square brackets

THE DOM TREE IS A
MODEL OF A WEB PAGE 

Accessing and updating the DOM tree involves two steps:
1: Locate the node that represents the element you want to work with.
2: Use its text content, child elements, and attributes. 

Each node is an object with methods and properties.
Scripts access and update this DOM tree (not the source HTML file).
Any changes made to the DOM tree are reflected in the browser. 
The terms elements and element nodes are used interchangeably
but when people say the DOM is working with an element,
it is actually working with a node that represents that element. 


methods that find elements in the dom tree are called dom queries


DOM queries may return one element, or they may return a Nodelist,
which is a collection of nodes. 

getElementByid () allows you
to select a single element node
by specifying the value of its
id attribute. 

There are two ways to select an element from a Nodelist:
The item() method and array syntax.
Both require the index number of the element you want. 

The getElementsByClass Name()
method allows you to select
elements whose c 1 ass attribute
contains a specific value. 

The getElementsByTagName ()
method allows you to select
elements using their tag name.

When you have an element node, you can select
another element in relation to it using these five
properties. This is known as traversing the DOM. 

parentNode
This property finds the element
node for the containing (or
parent) element in the HTML. 

previousSibling
nextSibling
These properties find the
previous or next sibling of a node
if there are siblings. 

firstChild
lastChild
These properties find the first or
last child of the current element. 


Traversing the DOM can be difficult because
some browsers add a text node whenever they
come across whitespace between elements. 

When you select a text node, you can retrieve or amend the content of it
using the node Value property. 

The textContent property allows you to
collect or update just the text that is in the
containing element (and its children).

Using the innerHTML property, you can access
and amend the contents of an element,
including any child elements. 


DOM manipulation can be used to remove
elements from the DOM tree. 

If you add HTML to a page using i nnerHTML (or several jQuery methods),
you need to be aware of Cross-Site Scripting Attacks or XSS; otherwise,
an attacker could gain access to your users' accounts. 

Make sure that your users can only input characters they need to use
and limit where this content will be shown on the page. 

To remove an attribute from an
element, first select the element,
then call removeAtt r i bute () .
It has one parameter: the name
of the attribute to remove. 

Modern browsers come with tools that help
you inspect the page loaded in the browser
and understand the structure of the DOM tree. 

An element node can contain multiple text nodes and
child elements that are siblings of each other

Whenever a DOM query can return more than one
node, it will always return a Nadelist. 

DOM trees have four types of nodes: document nodes,
element nodes, attribute nodes, and text nodes. 
