# Week 02: CSS

#### Outline
* [Introduction](#intro)
* [Import your own stylesheet](#import)
* [CSS Basics](#basics)
* [Bootstrap Extended](#bootstrap)
* 

****
<a name="intro"></a>
## Introduction

Cascading Style Sheets, most of the time abbreviated as CSS, is a stylesheet language used to describe the presentation of a document written in HTML or XML (including various XML languages like SVG or XHTML). CSS describes how the structured element must be rendered on screen, on paper, in speech, or on other media. - [Read More](https://developer.mozilla.org/en-US/docs/Web/CSS)

![html tag](https://mdn.mozillademos.org/files/8573/anatomy-of-an-html-element.png "HTML Tag struture")

*CSS styles is an Attribute of a HTML Tag/Element.*

You can view a whole list of of CSS properties which you can use to style your elements [here](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference).

Here's a [quick cheatsheet](https://media-mediatemple.netdna-ssl.com/wp-content/uploads/images/css3-cheat-sheet/css3-cheat-sheet.pdf), which has a quick summary of the most used, and the accepted values.

****


<a name="import"></a>
## Import your own stylesheet
##### Lets get started.

1. Open your **index.html** [file](https://github.com/intositeme/ts2016/blob/master/syllabus/01_Week-1/base.template.html) that was created last week. 
2. Add the line to [import your new external stylesheet](https://developer.mozilla.org/en-US/Learn/CSS/Using_CSS_in_a_web_page#The_%3Clink%3E_tag) to the *index.html* file. *Inside the <head> tag, after all the other <link> tags*
`<link href="css/style.css" rel="stylesheet">`

3. Go to your `css` folder and create a new file named `style.css`
4. This will be your base style sheet where you can use to define your styles, or override Bootstrap's base styles to start making your webpage look unique.



****


<a name="basics"></a>
## CSS Basics

### Selectors
You can apply styling to elements selectively using [**Selectors**](https://developer.mozilla.org/en/docs/Web/Guide/CSS/Getting_started/Selectors).

**What are selectors?**

There are few selectors

Live Samples on [CodePen](http://codepen.io/intosite/pen/eJGPGv?editors=110)


1. [**Elements**](https://developer.mozilla.org/en/docs/Web/HTML/Element) for eg. `div`, `img`, `p` 
2. [**Class selectors**](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/class) `<div class="my-class"></div>` the class selector is `my-class`
3. [**ID selectors**](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/id) `<div id="special-item"></div>` the ID for this element is `special-item`. Generally we do not use IDs to style elements, but it's not a hard and fast rule.
4. [**Pseudo-classes selectors**](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes) Pseudo class is a keyword added to selectors that specifies a special state of the element to be selected. For example :hover will apply a style when the user hovers over the element specified by the selector.
 


### Fonts

To use your own fonts, would require you to import your font into the HTML. Try not to use fonts installed on your system, as people who view your website on systems without the fonts will not show up properly.

There are many online font libraries which allow you to import fonts to use with your website, some are paid or free. 

Some of the font foundaries

* [fonts.com](http://www.fonts.com/web-fonts)
* [TypeKit](https://typekit.com/)
* [Google Fonts](https://www.google.com/fonts)

[Google Fonts](https://www.google.com/fonts) is free and popular choice though limited to the less popular fonts.

Live Samples on [CodePen](http://codepen.io/intosite/pen/mVBzxo?editors=110)

Lets select and import a font!

1.	Go to [google.com/fonts](https://www.google.com/fonts)
2.	Find a font you'll like to use.
3.	Add the font to your **collection** by clicking on the `Add to Collection` button.
4.	Repeat step 3 and add any other fonts you'll like to use. *Recommened to keep fonts to a minimum as it will affect the loading times of your website.*
5.	Click on `Use` under the **Collection** at the bottom of the screen.
6.	By default only the **Normal** weight of the font will be included. You can select the different styles you'll be using. *Note: The more styles you use the large the filesize of the font will be.*
7.	In `Step 3` of Google Fonts, under the **Standard** tab, copy the `<link>` tag code that you'll need to insert into your `index.html` file.
	`<link href='https://fonts.googleapis.com/css?family=Raleway:400,900' rel='stylesheet' type='text/css'> `
8.	Open your `index.html` file and paste the code you copied. It should be placed before your `style.css` import code.
9.	Use it in your `style.css` file. Under the **selector** which you like to change the font of, use the `font-family` property and set it to the name of the font you've use imported. Google Fonts `Step 4` `font-family: 'Raleway', sans-serif;`


### CSS Trasitions

Instead of having property changes take effect immediately, you can cause the changes in a property to take place over a period of time. [CSS transitions](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions), provide a way to control animation speed when changing CSS properties.

	transition: all 1s ease;

Live Samples on [CodePen](http://codepen.io/intosite/pen/jWGoab?editors=110)

In the Live Sample, I'm using the `:hover` pseudo class to trigger changes to the class properties, and using css transitions to animate the changes smoothly.

Transitions have [timing-functions](https://developer.mozilla.org/en-US/docs/Web/CSS/timing-function#Keywords_for_common_timing-functions), also known as 'easing'. This determines how fast the animation starts or slow down towards the end.

There are a few preset easings you can use, for more advance or custom easings, you can find them [here](http://easings.net/).

**Open up the Live Sample and play around. Try creating your own animation for the last box .my-own-transition**

Some properties you can animate

* width
* height
* colors
* padding/margin
* positions

**Advance**

You can make use of [CSS animations](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations/Using_CSS_animations) to create more complex animations. Not needing to use the :hover pseudo class.



****

<a name="bootstrap"></a>
## Bootstrap Extended

### Responsive elements
