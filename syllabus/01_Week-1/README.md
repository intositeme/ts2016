# Week 01: Web Development

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
* `<footer>` - Use to define content for [footer](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/footer)
* `<link>` - Specifies relationship between your page and an external resource, mainly CSS used for files. 
 
<sup>_importing an external file containing the styles_</sup>

```
<link rel="stylesheet" href="css/main.css">
```


* `<script>` - used to embed or reference an executable [script](https://developer.mozilla.org/en/docs/Web/HTML/Element/script)

<sup>_importing an external file containing JavaScript_</sup>

```
<script src="javascript.js"></script>
```
	

#### CSS
Casscading Style Sheets. CSS styles can be included both [inline](https://developer.mozilla.org/en/docs/Web/HTML/Element/style) and by importing it with the `<link>` tag.


## Frameworks




****
###### Footnotes

<a name="footnote1">1</a>: [Difference between UI & UX](http://blog.careerfoundry.com/the-difference-between-ux-and-ui-design-a-laymans-guide/)

<a name="footnote2">2</a>: [UX is not UI](http://www.helloerik.com/ux-is-not-ui)

<a name="footnote3">3</a>: [HTML Reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

<a name="footnote4">4</a>: [HTML cheatsheet](http://www.simplehtmlguide.com/cheatsheet.php)
