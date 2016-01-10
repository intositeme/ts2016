# Week 01: Web Development

#### Outline
* Introduction
* HTML
* CSS
* Frameworks
* Bootstrap

****

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

****

## HTML

* What is HTML?
* Introduction to HTML elements <sup>[3](#footnote3)</sup> <sup>[4](#footnote4)</sup>


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

#### HTML Elements

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
 
<sup>_importing an external file containing the styles_</sup>

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

##### More on CSS in week 2.

#### JavaScript
JavaScript is a cross-platform, object-oriented scripting language. It is a small and lightweight language. Inside a host environment (for example, a web browser), JavaScript can be connected to the objects of its environment to provide programmatic control over them.<sup>[5](#footnote5)</sup>

If you're interested, you can try out a basic tutorial [here](https://developer.mozilla.org/en-US/Learn/Getting_started_with_the_web/JavaScript_basics).

##### More on JavaScript in week 3.

****

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

## Bootstrap
##### Lets get started. 

1. You will need to download BootStrap [here](https://github.com/twbs/bootstrap/releases/download/v3.3.6/bootstrap-3.3.6-dist.zip), we will be using v3.3.6.
2. Unzip the file. This will be your project folder. _(Use this folder and create a new repository and commit it to your [GitHub account](https://github.com/intositeme/ts2016/tree/master/syllabus/00_Week-0#github), as outlined in the [pre-requisites](https://github.com/intositeme/ts2016/tree/master/syllabus/00_Week-0#githubapp))_

##### Your first page.
1. Create a new file `index.html`.
2. Use the base template from [here](https://github.com/intositeme/ts2016/blob/master/syllabus/01_Week-1/base.template.html).

#### Essential Bootstrap Elements
Lots of Bootstrap basic examples [here](http://getbootstrap.com/getting-started/#examples). 

##### Grid System
Bootstrap is built on a 12 column [grid system](http://getbootstrap.com/css/#grid-example-basic).

##### Navigation
Bootstrap provides a variaty of different Navbars to start with. You should view them [here](http://getbootstrap.com/getting-started/#examples-navbars).

##### Containers
Fixed and Fluid containers

##### Rows
Use rows to create horizontal groups of columns.

##### Columns
Content should be placed within columns, and only columns may be immediate children of rows.

##### Buttons
http://getbootstrap.com/css/#buttons

##### Images
http://getbootstrap.com/css/#images


	<img src="..." alt="..." class="img-rounded">
	<img src="..." alt="..." class="img-circle">
	<img src="..." alt="..." class="img-thumbnail">



****
###### Footnotes

<a name="footnote1">1</a>: [Difference between UI & UX](http://blog.careerfoundry.com/the-difference-between-ux-and-ui-design-a-laymans-guide/)

<a name="footnote2">2</a>: [UX is not UI](http://www.helloerik.com/ux-is-not-ui)

<a name="footnote3">3</a>: [HTML Reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

<a name="footnote4">4</a>: [HTML cheatsheet](http://www.simplehtmlguide.com/cheatsheet.php)

<a name="footnote5">5</a>: [Introduction to JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Introduction)

<a name="footnote6">6</a>: [What are Frameworks?](http://www.awwwards.com/what-are-frameworks-22-best-responsive-css-frameworks-for-web-design.html)

