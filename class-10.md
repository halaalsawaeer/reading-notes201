To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run

The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope. 

In the interpreter, each execution context has its own va ri ables object.
It holds the variables, functions, and parameters available within it.
Each execution context can also access its parent's variables object

Error objects can help you find where your mistakes are
and browsers have tools to help you read them. 

 DEBUG THE SCRIPT TO FIX ERRORS
If you come across an error while writing a script
(or when someone reports a bug), you will need to
debug the code, track down the source of the error,
and fix it. 

Debugging is about deduction: eliminating potential causes of an error. 

The JavaScript console will tell you when there is a problem with a script,
where to look for the problem, and what kind of issue it seems to be

HOW TO LOOK AT ERRORS
IN FIREFOX

1. The Console option is selected.
2. Only the JavaScript and
Logging options need to be
turned on. The Net, CSS, and
Security options show other
information. 

2. Only the JavaScript and
Logging options need to be
turned on. The Net, CSS, and
Security options show other
information.
+
Find the area of a wall:
+-+ width
! height
Calculate area ...
3. The type of error and the error
message are shown on the left.
4. On the right-hand side of the
console, you can see the name
of the JavaScript file and the line
number of the error


Browsers that have a console have a console object, which has several
methods that your script can use to display data in the console.
The object is documented in the Console API. 

You can pause the execution of a script on any
line using breakpoints. Then you can check the
values stored in variables at that point in time. 

If you know that you may get an error, you can handle
it gracefully using the try, catch, finally statements.
Use them to give your users helpful feedback.

Here are a selection of practical tips that you
can try to use when debugging your scripts. 
1.ANOTHER BROWSER 
2.SEARCH 
3.STRIP IT BACK 
4.EXPLAINING THE CODE
