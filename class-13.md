
Persistent local storage is one of the areas where native client applications have held an advantage over web applications.
If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions.
 Cookies were invented early in the web’s history,and indeed they can be used for persistent local storage of small amounts of data.But they have three potentially dealbreaking downsides:

Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful

userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure. (Trusted domains, such as intranet sites, can store 10 times that amount. And hey, 640 KB ought to be enough for anybody.) IE does not present any form of permissions dialog, and there is no allowance for increasing the amount of storage available.
Flash cookies  allows Flash objects to store up to 100 KB of data per domain.

In 2007, Google launched Gears, an open source browser plugin aimed at providing additional capabilities in browsers
Gears can store unlimited amounts of data per domain in SQL database tables.

“HTML5 Storage” is a specification named Web Storage
Certain browser vendors also refer to it as “Local Storage” or “DOM Storage.”
So what is HTML5 Storage? Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser. 
You store data based on a named key,then you can retrieve that data with the same key.
Calling setItem() with a named key that already exists will silently overwrite the previous value. Calling getItem() with a non-existent key will return null rather than throw an exception.
 there is a property to get the total number of values in the storage area, and to iterate through all of the keys by index (to get the name of each key).
 If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something.
 The storage event is supported everywhere the localStorage object is supported, which includes Internet Explorer 8. IE 8 does not support the W3C standard addEventListener (although that will finally be added in IE 9). Therefore, to hook the storage event, you’ll need to check which event mechanism the browser supports.

 HTML5 Storage are “5 megabytes,”

 Let’s see HTML5 Storage in action. Recall the Halma game we constructed in the canvas chapter. There’s a small problem with the game: if you close the browser window mid-game, you’ll lose your progress. But with HTML5 Storage, we can save the progress locally, within the browser itself.

 most of the action resides in the string 

 his string can be any supported SQL statement, including SELECT, UPDATE, INSERT, and DELETE statements. It’s just like backend database programming, except you’re doing it from JavaScript
 The Indexed Database API exposes what’s called an object store.
 An object store shares many concepts with a SQL database.
 There are “databases” with “records,” and each record has a set number of “fields.”
 Each field has a specific datatype, which is defined when the database is created.
 You can select a subset of records, then enumerate them with a “cursor.” Changes to the object store are handled within “transactions.”
 the records, filter out records for inactive users, and use accessor methods to get the values of each field in the remaining records  --
