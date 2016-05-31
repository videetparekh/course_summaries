# JAVASCRIPT

JavaScript is the most popular language today. It's used in many different platforms, as back-end and front-end technology. It's primary goal is to make the static elements of HTML and CSS respond to user actions, i.e. make an application dynamic. 



### DOM

The Document Object Model is a tree of objects built when a webpage is first called. 

![](http://www.webstepbook.com/supplements/slides/images/dom_tree.gif)

With the object model JS gets all the capability it needs to access parts of the HTML and CSS and manipulate these objects to react in certain ways.



### JQuery

Jquery is a commonly used JavaScript library dedicated to simplifying the use of JS to manipulate the DOM. 

```javascript
var eleinstances = $('element');
```

The `$` selector is a function to which the function, id, class or tag name is passed. In case of the last three, it returns every instance of the specified element to the variable `eleinstances`. This can be further manipulated with various functions like `.append()`, `.addClass()`, `.remove()`, etc.

A complete list of JQuery references is found in the [Jquery API Documentation][http://www.webstepbook.com/supplements/slides/images/dom_tree.gif].



### Data Types

Javascript supports various data-types like string, num, int, float, boolean, etc. They are all encompassed within a single keyword, `var`. All JS libraries allow express manipulation of these variables. Numerical variables can undergo mathematical operations. Strings may undergo operations such as slicing, splitting, concatenation, etc. Boolean variables are subject to logical operations. 

In addition to these basic data types, JS supports more complex stuctures like arrays, and objects (JSON data structures with a dictionary-like key: value pair definition).



### Loops

Types:

- For(){}
- While(){}
- Do{}... While();
- For( ... in){}
- ForEach(){}




### Logical Conditions

- if(){} 
  - else if(){} 
  - else{}



### Event Listeners

Event listeners are functions used to monitor browser events and perform actions based on these events. 

```javascript
$('#my-button').on('click', function(){ //initiates a listener on my-button for a click
   $('#my-button').remove(); //removes the button
   $('body').addClass('success'); //adds a class called success to the body, that   								     //appends success message to the body
});
```

There are various types of events these can be configured for.

A list of events is available [here][https://api.jquery.com/category/events/].

Certain functions can also be represented as convenience methods. These methods are shorthand function calls made to achieve the same goal as their fullhand counterparts. The following code achieves the same goal as the code above.

```javascript
$('#my-button').click(	//initiates a listener on my-button for a click
function(){
   $('#my-button').remove(); //removes the button
   $('body').addClass('success'); //adds a class called success to the body, that   								     //appends success message to the body
});
```