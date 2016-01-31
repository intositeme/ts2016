# Week 03: JavaScript

#### Outline
* [Introduction](#intro)
* [Import your own JavaScript](#import)
* [jQuery](#jquery)
* [Start Coding](#start)
* [Libraries](#libraries)

****
<a name="intro"></a>
## Introduction

JavaScript is one of the most popular programming language in the world. 
JavaScript is essential in constructing an interactive & engaging website. Where elements and animations reacts to a user's interaction.

Basically JS is used to store, manipulate values, and there are a number of **types** of values. It is also used to manipulate elements in your HTML by altering their property values for eg, background-color, position, size etc. 

### Javascript Value Types

[JavaScript's value types](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript) are:

* Number
* String *"your value here in quotes"*
* Boolean *true/false*
* Function *function funcName () {  }*
* Object *special holder than can contain any of the above*
	* Function
	* Array *able to hold multiple values*
	* Date

### Variables

A **Variable** is a symbolic name (an identifier) that you can use to store a value.

To declare a **variable** you'll use the `var` keyword preceding the variable name.

Live sample on [CodePen](http://codepen.io/intosite/pen/YwvVEX?editors=0011)
	
	// Declaring the variables you'll be using. 
	// It's good practice to define them at the top of your program.
	var noOfApples = 10 ;
	var noOfOranges; 
	var totalNoOfFruits;
	
	// You can set a variable's value any time 
	// from any where in your program, but do beware of "Scopes"
	noOfOranges = 5;
	
	// Mathematical operations.
	totalNoOfFruits = noOfApples + noOfOranges;
	console.log(totalNoOfFruits); // returns 15;
	
### Operators

In most if not all programming languages there are **operators** which is a special symbol that tells the computer what to do, which can be a mathematical, relational or logical operation.

List of [operators here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators#Arithmetic_operators).

**Arithmetic operators** *commonly used*

* Addition (+) 
* Subtraction (-)
* Division (/)
* Multiplication (*)

### Functions

A [function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions) is a JavaScript procedure—a set of statements that performs a task or calculates a value. 

	// Declare a function with the name "sayHello"
	function sayHello () {
		console.log('Hello World!');
	}
	// to execute/call the function
	sayHello ();
	
A function can be passed value/s as [parameters](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions#Function_parameters).

	// Declare a function with the name "sayHello"
	// Accepting a parameter "name"
	function sayHello (name) {
		console.log('Hello ' + name +'!');
	}
	// to execute/call the function
	sayHello ("John");

****

<a name="jquery"></a>
## jQuery
[jQuery](https://jquery.com/) is a library. The purpose of jQuery is to make it much easier to use JavaScript on your website.

jQuery takes a lot of common tasks that require many lines of JavaScript code to accomplish, and wraps them into methods that you can call with a single line of code.

jQuery also simplifies a lot of the complicated things from JavaScript, like AJAX calls and DOM manipulation.

### Start using jQuery
To start using jQuery, you'll need to import the jQuery library .js file into your html. For Bootstrap templates, *provided template previously*, jQuery is already included. Bootstrap makes use of jQuery for some of their components, for eg, navigation bar.

If jQuery is not imported, you can import it using the `<script>` tag as such, for different versions you can find them [here](https://developers.google.com/speed/libraries/#jquery).

`<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.0/jquery.min.js"></script>`

****

<a name="import"></a>
## Import your own JavaScript
##### Lets get started.

1. Open your **index.html** [file](https://github.com/intositeme/ts2016/blob/master/syllabus/01_Week-1/base.template.html) that was created previously. 
2. Add the line to [import your new external javascript](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/script#Examples) to the *index.html* file. *Inside the `<body>` tag, just before the `</body>`*

`<script src="js/app.js"></script>`

3. Go to your `css` folder and create a new file named `style.css`
4. This will be your base style sheet where you can use to define your styles, or override Bootstrap's base styles to start making your webpage look unique.

****

<a name="start"></a>
## Start Coding

### First Step

We start with a function that ensures your html [document has finish loading](https://learn.jquery.com/using-jquery-core/document-ready/) before it starts running your codes. This will prevent errors that happens on occassions when JavaScript is trying to target an element that has not been loaded yet.

	$( document ).ready(function() {
    	// Your code here.
	});

### Selectors & Adding Click Events
Live sample on [CodePen](http://codepen.io/intosite/pen/VedxXV?editors=1010)

To start using jQuery, you will start with the `$()` function. To target elements, you'll provide the **selector** parameter inside the `()`. The parameter is usually a **string** much like a **CSS Selector**, or at times it can be an **object**, one such object is the `document` or `window` object.

Here is an [list of selectors](http://www.w3schools.com/jquery/jquery_ref_selectors.asp) that is available to enable you to select the html elements you require.

An [live example](http://www.w3schools.com/jquery/trysel.asp) of the selectors for you to explore can be found here.


#### jQuery APIs
Also know as functions or methods that you can use. In the above example, we were using the `.click()` function, to assign what JavaScript should do when the element is **clicked**. There are many other methods which are available, one of the other commonly used is the `.css()` function to apply changes to the CSS properties of an element.

##### .addClass() & .removeClass()
In the next example we will be using the `.addClass()` & `.removeClass()`
Live sample on [CodePen](http://codepen.io/intosite/pen/MKXGJj)

##### .animate();

A useful jQuery API function is `.animate()`. 
http://codepen.io/intosite/pen/BjVxbN

****

<a name="libraries"></a>
## Libraries
There are many JavaScript libraries out there. Libraries are sets of codes that makes it easy to do repeated task or effects. We'll take a look at a particular scrolling effect library

#### ScrollReveal.js & AniJS

**[ScrollReveal.js](https://github.com/jlmakes/scrollreveal.js)** is a set of tools that triggers a specific animation when the user scrolls the element into view. 
Live Sample on [CodePen](http://codepen.io/intosite/pen/jWKpEv).

**[AniJS](anijs.github.io/)** was created to help make it easier to apply effects with minimal knowledge of JavaScript.
Live Sample on [CodePen](http://codepen.io/intosite/pen/dGKjdW?editors=1010). 

In our example, we will explore how to implement **ScrollReveal** to elements on a page. We will also explore how we can make use of **AniJS**  to apply the same effects, but in a much easier manner.


####

