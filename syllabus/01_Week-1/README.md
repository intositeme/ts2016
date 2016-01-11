# Week 01: Web Development

#### Outline
* [Introduction](#intro)
* [HTML](#html)
* [Frameworks](#frameworks)
* [Bootstrap](#bootstrap)
* [Assignment](#assignment)

****
<a name="intro"></a>
## Introduction 

* What do you think makes a good Website?
* Do you think you're a good web/interactive/digital designer? Why?
* What qualities do you think is needed to be so?
* UI/UX - What are they? <sup>[1](#footnote1)</sup> <sup>[2](#footnote2)</sup>


#### Development Stages 
Developing a website has many stages & specialisations. 

1. Project Definition 
2. Project Scope / Content gathering
3. **Wireframes & Site architecture**
4. **Visual Design**
5. **Site Development**
6. Site Testing
7. Launch

#### Wireframes & Site architecture
A website wireframe, is a visual guide that represents the skeletal framework of a website. Wireframes are created for the purpose of arranging elements to best accomplish a particular purpose: business objective and a creative idea. 

The wireframe depicts the page layout or arrangement of the website’s content, including interface elements and navigational systems, and how they work together.

[More reading](http://webdesign.tutsplus.com/articles/a-beginners-guide-to-wireframing--webdesign-7399).

Online tool, [Wireframe.cc](https://wireframe.cc) you can choose to use. Sketching with pen and paper is fine too. A [sample here](https://wireframe.cc/oSR3Bx). _* note: Others can edit your sketch if they have the link._ 

#### Visual Design
After outlining and planning the content of your website requirements, this stage is where you will start to design how it will look.

Most of the time you will design your website based off the wireframes. As the wireframes determines the what will be needed in the website. You **should not** restrict your design layout to the wireframe's layout. Feel free to explore.

This process usually involves quite a bit of review approval cycles with your Creative/Art Director & Clients. 

#### Site Development
Once the Wireframes & Visual Design has been approved, you will start to code your website. This is where the workshop begins.

****

<a name="html"></a>

## HTML 

* What is HTML?
* Introduction to HTML elements <sup>[3](#footnote3)</sup> <sup>[4](#footnote4)</sup>

#### What is HTML



> HTML, which stands for HyperText Markup Language, is the most basic building block of a webpage and used for creating and visually representing a webpage. It determines the content of a webpage , but not its functionality. _[HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)_

![html tag](https://mdn.mozillademos.org/files/8573/anatomy-of-an-html-element.png "HTML Tag struture")


#### Simple HTML Document

```
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Hello world!</title>
</head>
<body>
  <h1>Main heading in my document</h1>
  <!-- Note that it is "h" + "1", not "h" + the letters "one" -->
  <p>Look Ma, I am coding <abbr title="Hyper Text Markup Language">HTML</abbr>.</p>
</body>
</html>
```

#### HTML Elements/Tags

* `<html>` - main HTML [document root](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/html) that everything should be inside
* `<head>` - contains [document information](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/head), CSS, JS, search keywords etc.
* `<body>` - [Document body](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/body). Where the content you want to display sits in
* `<div>` - [Document division](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/div). Used to contain and layout content. Pay attention to allow [attributes](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes).
* `<nav>` - Use to define content for the [site navigation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/nav)
* `<p>` - Used to segment [paragraph](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/p) of text. 
* `<a>` - [Link](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a) to part or different page.
* `<img>` - Insert an [image](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img). Pay attention to [attributes](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img#Attributes) for tag

```
<img src="logo.jpg" alt="Logo">
```

* `<footer>` - Use to define content for [footer](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/footer)
* `<link>` - Specifies relationship between your page and an external resource, mainly CSS used for files. 


```
<!-- importing an external file containing the styles -->
<link rel="stylesheet" href="css/main.css">
```

* `<script>` - used to embed or reference an executable [script](https://developer.mozilla.org/en/docs/Web/HTML/Element/script)


```
<!-- importing an external file containing JavaScript_ -->
<script src="javascript.js"></script>

<!-- Embedding JavaScript into the document -->
<script>console.log("hello world!");</script>
```

#### CSS
Casscading Style Sheets. CSS styles can be included both [inline](https://developer.mozilla.org/en/docs/Web/HTML/Element/style) and by importing it with the `<link>` tag.

```
<!-- importing an external file containing the styles -->
<link rel="stylesheet" href="css/main.css">

<!-- Embedding styles into the document -->
<style type="text/css">
body {
  color:red;
}
</style>
```

##### Classes
What are [CSS classes](https://developer.mozilla.org/en-US/docs/Web/CSS/Class_selectors)?

CSS classes are used to specify what CSS styles a specific element should use. In your inline CSS style or external .css file, you will use CSS class selectors to match an element based on the contents of the element's class attribute.

###### CSS
	span.classy {
	  background-color: red;
	}
###### HTML
	<span class="classy">Here's a span with some text.</span>
	<span>Here's another.</span
	
[Example on Codepen](http://codepen.io/intosite/pen/bERNJV)

##### More on CSS in week 2.

#### JavaScript
JavaScript is a cross-platform, object-oriented scripting language. It is a small and lightweight language. Inside a host environment (for example, a web browser), JavaScript can be connected to the objects of its environment to provide programmatic control over them.<sup>[5](#footnote5)</sup>

If you're interested, you can try out a basic tutorial [here](https://developer.mozilla.org/en-US/Learn/Getting_started_with_the_web/JavaScript_basics).

##### More on JavaScript in week 3.

****

<a name="frameworks"></a>

## Frameworks 

A framework is a standardized set of concepts, practices and criteria for dealing with a common type of problem, which can be used as a reference to help us approach and resolve new problems of a similar nature.<sup>[6](#footnote6)</sup>

Frameworks allow us to cut out much of the work and save a lot of time.<sup>[6](#footnote6)</sup>

#### Front-end Frameworks (or CSS Frameworks)
Frontend frameworks usually consist of a package made up of a structure of files and folders of standardized code (HTML, CSS, JS documents etc.)<sup>[6](#footnote6)</sup>

**The usual components are:**

* CSS source code to create a grid: this allows the developer to position the different elements that make up the site design in a simple and versatile fashion.<sup>[6](#footnote6)</sup>
* Typography style definitions for HTML elements.<sup>[6](#footnote6)</sup>
* Solutions for cases of browser incompatibility so the site displays correctly in all browsers.<sup>[6](#footnote6)</sup>
* Creation of standard CSS classes which can be used to style advanced components of the user interface.<sup>[6](#footnote6)</sup>

##### We will be using [Bootstrap v3.3.6](http://getbootstrap.com/) built by Twitter.

****

<a name="bootstrap"></a>

## Bootstrap 
##### Lets get started. 
Live Samples on [CodePen](http://codepen.io/collection/XLYZmz/)

1. You will need to download BootStrap [here](https://github.com/twbs/bootstrap/releases/download/v3.3.6/bootstrap-3.3.6-dist.zip), we will be using v3.3.6.
2. Unzip the file. This will be your project folder. Rename the folder to `your_name-ts2016` _(Use this folder and create a new repository and commit it to your [GitHub account](https://github.com/intositeme/ts2016/tree/master/syllabus/00_Week-0#github), as outlined in the [pre-requisites](https://github.com/intositeme/ts2016/tree/master/syllabus/00_Week-0#githubapp))_

##### Your first page.
1. Create a new file `index.html`.
2. Use the base template from [here](https://github.com/intositeme/ts2016/blob/master/syllabus/01_Week-1/base.template.html).

#### Essential Bootstrap Elements
Lots of Bootstrap basic examples [here](http://getbootstrap.com/getting-started/#examples). 

##### Grid System
Bootstrap is built on a 12 column [grid system](http://getbootstrap.com/css/#grid-example-basic).

##### Containers
Fixed and Fluid containers
Example - [Interactive CodePen](http://codepen.io/intosite/pen/NxgPQN)

```
<!-- Fixed width container -->
<div class="container"> </div>

<!-- Fixed width container -->
<div class="container-fluid"> </div>
```

##### Rows
Use rows to create horizontal groups of columns.

```
<div class="container-fluid">
  <div class="row">
    ...
  </div>
  <div class="row">
    ...
  </div>
</div>
```

##### Columns
Content should be placed within columns, and only columns may be immediate children of rows.

```
<!-- Put this style into the header of the document to preview the columns -->
<style>
	.row {
		background-color: rgba(86, 61, 124, 0.15);
		border: 1px solid rgba(86, 61, 124, 0.2);
	}
</style>
```


```
<div class="container-fluid">
  	<div class="row">
  		<div class="col-md-8">.col-md-8</div>
  		<div class="col-md-4">.col-md-4</div>
	</div>
	<div class="row">
  		<div class="col-md-4">.col-md-4</div>
  		<div class="col-md-4">.col-md-4</div>
  		<div class="col-md-4">.col-md-4</div>
	</div>
	<div class="row">
 		<div class="col-md-6">.col-md-6</div>
	  	<div class="col-md-6">.col-md-6</div>
	</div>
</div>
```

###### Responsive Columns
Columns resizes according to browser size.

```
<div class="container-fluid">
	<div class="row">
  		<div class="col-xs-12 col-sm-6 col-md-4">.col-xs-12 .col-sm-6 .col-md-4</div>
  		<div class="col-xs-12 col-sm-6 col-md-4">.col-xs-12 .col-sm-6 .col-md-4</div>
  		<div class="col-xs-12 col-sm-6 col-md-4">.col-xs-12 .col-sm-6 .col-md-4</div>
	</div>
</div>
```

##### Navigation
Bootstrap provides a variaty of different Navbars to start with. You should view them [here](http://getbootstrap.com/getting-started/#examples-navbars).

##### Navbar
The `nav.navbar` is it's own unique container, thus it is **not** required to sit with in a **container**.

###### Main Navbar Container
Example - [Preview](http://intositeme.github.io/static-bootstrap/example-nav.html) & [Code](https://github.com/intositeme/static-bootstrap/blob/master/example-nav.html) & [Interactive CodePen](http://codepen.io/intosite/pen/jWwEoM)

	<nav class="navbar navbar-default">
		<!-- The container class can be fluid or fixed, depending on requirements -->
  		<div class="container-fluid">
  		...
  		</div>
  	</nav>
  	
###### Navbar header
The nav header sits within the Navbar's container. This is where you would place your brand name or logo. 

Example - [Preview](http://intositeme.github.io/static-bootstrap/example-nav__links.html) & [Code](https://github.com/intositeme/static-bootstrap/blob/master/example-nav__links.html) & [Interactive CodePen](http://codepen.io/intosite/pen/xZrbNj)

	 	<div class="navbar-header">
	 		<!-- This is the Mobile nav icon that will only display when the browser size is 'sm' -->
      		<button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1" aria-expanded="false">
        		<span class="sr-only">Toggle navigation</span>
        		<span class="icon-bar"></span>
        		<span class="icon-bar"></span>
        		<span class="icon-bar"></span>
      		</button>
      		<!-- You can change the"Brand Name" text to insert an image of your logo -->
      		<a class="navbar-brand" href="#">Brand Name</a>
      		<!-- <a class="navbar-brand" href="#">Brand Name</a> -->
    	</div>
    	


##### Buttons
http://getbootstrap.com/css/#buttons

##### Images
http://getbootstrap.com/css/#images

	<img src="..." alt="..." class="img-rounded">
	<img src="..." alt="..." class="img-circle">
	<img src="..." alt="..." class="img-thumbnail">

****
<a name="assignment"></a>
## Assignment 
1. Think about the website you want to create
2. Think about the content & how you would want to display it.
3. Sketch a wireframe layout of your website (photoshop/illustrator jpgs is fine, but a rough sketch is more than sufficient), [reference here](http://www.kimbieler.com/wp-content/uploads/2012/03/athayde-homepage.jpg). Create a new folder `wireframes` and place scan/photo jpgs in. Commit the files to your repository.
4. Edit your index.html file and try to layout your wireframe with Bootstrap. Commit files to your repository.

****
###### Footnotes

<a name="footnote1">1</a>: [Difference between UI & UX](http://blog.careerfoundry.com/the-difference-between-ux-and-ui-design-a-laymans-guide/)

<a name="footnote2">2</a>: [UX is not UI](http://www.helloerik.com/ux-is-not-ui)

<a name="footnote3">3</a>: [HTML Reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

<a name="footnote4">4</a>: [HTML cheatsheet](http://www.simplehtmlguide.com/cheatsheet.php)

<a name="footnote5">5</a>: [Introduction to JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Introduction)

<a name="footnote6">6</a>: [What are Frameworks?](http://www.awwwards.com/what-are-frameworks-22-best-responsive-css-frameworks-for-web-design.html)

