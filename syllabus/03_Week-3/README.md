# Week 02: JavaScript

#### Outline
* [Introduction](#intro)
* [Import your own JavaScript](#import)
* 

****
<a name="intro"></a>
## Introduction

JavaScript is one of the most popular programming language in the world. 
JavaScript is essential in constructing an interactive & engaging website. Where elements and animations reacts to a user's interaction.

Basically JS is used to store, manipulate values, and there are a number of **types** of values. It is also used to manipulate elements in your HTML by altering their property values for eg, background-color, position, size etc. 

### Javascript Value Types

[JavaScript's value types](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript) are:

* Number
* String
* Boolean
* Function
* Object
	* Function
	* Array
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
	
	
<a name="import"></a>
## Import your own JavaScript
##### Lets get started.

1. Open your **index.html** [file](https://github.com/intositeme/ts2016/blob/master/syllabus/01_Week-1/base.template.html) that was created previously. 
2. Add the line to [import your new external javascript](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/script#Examples) to the *index.html* file. *Inside the `<body>` tag, just before the `</body>`*

`<script src="javascript.js"></script>`

3. Go to your `css` folder and create a new file named `style.css`
4. This will be your base style sheet where you can use to define your styles, or override Bootstrap's base styles to start making your webpage look unique.



****

