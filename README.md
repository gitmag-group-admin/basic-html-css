

# HTML

Hyper Text Markup Language

**Code Editor**
Visual Studio Code
Download: *https://code.visualstudio.com/*

**Tag**
\<tag-name> **content** \</tag-name>
*\<html> HTML document content \</html>*

\<tag-name />
*\<img />*

**Introduction HTML document**
All HTML documents must start with a `<!DOCTYPE>` declaration.
```html
<!doctype html>
```
## HTML Document structure

Simple HTML document
```html
<!doctype html>
<html>
    <head>
    </head>
	    
    <body>
    </body>
</html>
```
head: *Search engine information structure*
body: *User information structure*

## HTML document title

The `<title>` tag defines the title of the document. The title must be text-only, and it is shown in the browser's title bar or in the page's tab.
```html
<!doctype html>
<html>
    <head>
	<title> GitMag website </title>
    </head>
    <body>
    </body>
</html>
```
## HTML content
The `<body>` tag defines the document's body.
There can only be one `<body>` element in an HTML document.
```html
<!doctype html>
<html>
    <head>
	<title> GitMag website </title>
    </head>
    <body>
	This is my website
    </body>
</html>
```
## Break line tag
The `<br>` tag inserts a single line break.
```html
My name is Sohrab <br> I am Programmer
```
## Horizontal tag
The `<hr>` tag defines a thematic break in an HTML page
```html
My name is Sohrab <hr> I am Programmer
```
## Paragraph tag
The HTML `<p>` element defines a paragraph.
```html
<p>This is first paragraph</p>
<p>This is second paragraph</p>
<p>This is third paragraph</p>
```
## Formatting tags
Formatting elements were designed to display special types of text:

`<b>` - Bold text
`<strong>` - Important text
`<i>` - Italic text
`<small>` - Smaller text
...
```html
   <p>
    In publishing and <b>graphic design</b>, Lorem ipsum is a placeholder text commonly used to demonstrate the visual form of a document or a typeface without relying on <strong>meaningful content</strong>. 
   </p>
   <p>
    Lorem ipsum may be used as a placeholder before <i>final copy is available</i>.
   </p>
```
## Heading tags
The `<h1>` to `<h6>` tags are used to define HTML headings.
```html
<h1>heading1</h1>
<h2>heading2</h2>
<h3>heading3</h3>
<h4>heading4</h4>
<h5>heading5</h5>
<h6>heading6</h6>
```
## HTML tag Attributes
\<html lang="en"> *HTML document content* \</html>
\<html lang='en'> *HTML document content* \</html>
```html
<!doctype html>
<html lang="en">
    <head>
	<title> GitMag website </title>
    </head>
    
    <body>
	This is my website
    </body>
</html>
```
## Anchor tag

The `<a>` tag defines a hyperlink, which is used to link from one page to another.
```html
<a href="http://google.com"> Go to Google</a>
```
A linked page is normally displayed in the current browser window, unless you specify another target.
```html
<a href="http://google.com" target="_parent"> Go to Google</a>
```
> Target attribute values:
> _self: *Opens the linked document in the same frame as it was clicked (**this is default**)*
> _blank: *Opens the linked document in a new window or tab*
> _parent: *Opens the linked document in the parent frame*
> _top: *Opens the linked document in the full body of the window*

## Table tag
The `<table>` tag defines an HTML table.
An HTML table consists of one `<table>` element and one or more `<tr>` `<th>` and `<td>` elements.
 ```html
<table>  
    <tr>  
        <th>Name</th>  
        <th>Family</th> 
        <th>Age</th>  
    </tr>  
    <tr>  
        <td>Sohrab</td>  
        <td>Azin far</td>  
        <td>30</td>
    </tr>
    <tr>  
        <td>Hussein</td>  
        <td>Mohammadi</td>  
        <td>25</td>
    </tr>  
 </table>
```
How to add collapsed borders to a table:
```html
<table border="1">
   
</table>
```
How to create a table with a caption:
```html
<table>
    <caption> Table caption </caption>
</table>
```
An HTML table with a `<thead>` and `<tbody>` element:
```html
<table>
   <thead>
	   ...
   </thead>
   <tbody>
	   ...
   </tbody>
</table>
```    
How to define table cells that span more than one row or one column:
```html
<table>  
    <thead>
	<tr>  
	    <th>Name</th>  
	    <th>Family</th> 
	    <th>Age</th>
	    <th colspan="2">Phone</th>  
	</tr>  
    </thead>
    <tbody>
        <tr>  
	    <td>Sohrab</td>  
	    <td>Azin far</td>  
	    <td>30</td>
	    <td>0912-1111111</td>
	    <td>021-22222222</td>
	</tr>
        <tr>  
	    <td>Hussein</td>  
	    <td>Mohammadi</td>  
	    <td>25</td>
	    <td>0912-2222222</td>
	    <td>021-66666666</td>
	</tr>  
    </tbody>
</table>
```
## Image tag

The `<img>` tag is used to embed an image in an HTML page.
```html
<img src="logo.png" alt="GitMag.png" width="200" height="50" />
```
>src: *Specifies the path to the image*
> alt: *Specifies an alternate text for an image*
> width: *Specifies the width of an image*
> height: *Specifies the height of an image*

## List tag

**Order lists**
An ordered list starts with the `<ol>` tag. Each list item starts with the `<li>` tag.
```html
<ol>
    <li>Home</li>
    <li>About Us</li>
    <li>News</li>
    <li>Contact Us</li>
</ol>
```
**Unorder list**
An unordered list starts with the `<ul>` tag. Each list item starts with the `<li>` tag.
```html
<ul>
    <li>Home</li>
    <li>About Us</li>
    <li>News</li>
    <li>Contact Us</li>
</ul>
```    
## Divider tag
The `<div>` tag defines a division or a section in an HTML document.
```html
<div id="header"> Website Header </div>
<div id="navbar"> Website Navbar </div>
<div id="main">
    <div id="sidbar"> Website Sidebar </div>
    <div id="content"> Website Content </div>
</div>
<div id="footer"> Website Footer </div>
```
## Semantic tags
*Semantic elements = elements with a meaning.*
```html
<header> Website Header </header>
<nav> Website navbar </nav>
<main>
    <aside>Website Sidebar</aside>
    <sction>
    	<article>Article 1</article>
    	<article>Article 2</article>
    	<article>Article 3</article>
    	<article>Article 4</article>
    </sction>
</main>
<footer>Website Footer</footer>
```
## Forms
An HTML form is used to collect user input. The user input is most often sent to a server for processing.
```html
<form action="http://gitmag.ir" method="GET">
    ...
</form>
```
**Input tag**
One of the most used form element is the `<input>` element.
The `<input>` element can be displayed in several ways, depending on the `type` attribute.
```html
<label for="fname">First name:</label>  
<input type="text" id="fname" name="fname">
```
> text: *Displays a single-line text input field*
> radio: *Displays a radio button (for selecting one of many choices)*
> checkbox: *Displays a checkbox (for selecting zero or more of many choices)*
> submit: *Displays a submit button (for submitting the form)*
> button: *Displays a clickable button*
> color: *Displays a color picker*
> file: *Display a "Browse" button for file uploads.*

**Textarea tag**
The `<textarea>` element defines a multi-line input field (a text area):
```html
<textarea name="message" rows="10" cols="30">  
    The cat was playing in the garden.  
</textarea>
```
**Select tag**
The `<select>` element defines a drop-down list:
```html
<select name="cars">  
    <option value="volvo">Volvo</option>  
    <option value="benz">Benz</option>  
    <option value="fiat">Fiat</option>  
    <option value="audi">Audi</option>  
</select>
``` 
## Meta tags
The `<meta>` tag defines metadata about an HTML document. Metadata is data (information) about data.
```html
<head>  
    <meta charset="UTF-8">  
    <meta name="description" content="Free Web tutorials">  
    <meta name="keywords" content="HTML, CSS, JavaScript">  
    <meta name="author" content="John Doe">  
</head>
```
> keywords: *Define keywords for search engines*
> description: *Define a description of your web page*
> author: *Define the author of a page*

## Comment in HTML
You can add comments to your HTML source by using the following syntax:
```html
<!-- This is a comment -->  
<p>This is a paragraph.</p>  
<!-- Remember to add more information here -->
```



# CSS

CSS stands for Cascading Style Sheets
CSS describes how HTML elements are to be displayed on screen, paper, or in other media
CSS saves a lot of work. It can control the layout of multiple web pages all at once

**CSS rule structure**
A CSS rule consists of a selector and a declaration block.

![enter image description here](https://www.w3schools.com/css/img_selector.gif)

The selector points to the HTML element you want to style.
The declaration block contains one or more declarations separated by semicolons.
Each declaration includes a CSS property name and a value, separated by a colon.
```css
p {  
    color: red;  
    text-align: center;  
}
```
> `p` is a selector in CSS (it points to the HTML element you want to style: `<p>`).
> `color` is a property, and `red` is the property value
> `text-align` is a property, and `center` is the property value

## Using CSS

CSS can be added to HTML documents in 3 ways:
 -   Inline: *by using the `style` attribute inside HTML elements*
 -   Internal: *by using a `<style>` element in the `<head>` section*
 -   External *by using a `<link>` element to link to an external CSS file*

**Inline CSS**
An inline CSS uses the `style` attribute of an HTML element.
```html
<h1 style="color:blue;">A Blue Heading</h1>  
<p style="color:red;">A red paragraph.</p>
```
**Internal CSS**
An internal CSS is defined in the `<head>` section of an HTML page, within a `<style>` element.
```html
<!DOCTYPE html>  
<html>  
<head>  
    <style>  
	body {background-color: powderblue;}  
	h1 {color: blue;}  
	p {color: red;}  
    </style>  
</head>  
<body>  
    <h1>This is a heading</h1>  
    <p>This is a paragraph.</p>  
</body>  
</html>
```
**External CSS**
To use an external style sheet, add a link to it in the `<head>` section of each HTML page:
```html
<!DOCTYPE html>  
<html>  
<head>  
    <link rel="stylesheet" href="styles.css">  
</head>  
<body>   
    <h1>This is a heading</h1>  
    <p>This is a paragraph.</p>  
</body>  
</html>
```
**Cascading Order**
What style will be used when there is more than one style specified for an HTML element?
All the styles in a page will "cascade" into a new "virtual" style sheet by the following rules, where number one has the highest priority:

1.  Inline style (inside an HTML element)
2.  External and internal style sheets (in the head section)
3.  Browser default

## CSS Selectors
CSS selectors are used to "find" (or select) the HTML elements you want to style.

**Simple Selector**
 - **class**: *Selects all elements with class attribute*
 - **element:** *Selects all elements by tag name*(**The CSS Grouping Selector**)
 - **element class**: Selects only elements with a class
 - **Id**: *Selects the element with id attribute*
 - **element, element, ...:** *Selects all elements together*
 - \* *Selects all elements* (**The CSS Universal Selector**)

## CSS comment

Comments are used to explain the code, and may help when you edit the source code at a later date.
A CSS comment is placed inside the `<style>` element, and starts with `/*` and ends with `*/`:
```css
/* This is a single-line comment */  
p {  
    color: red;  
}
```
## CSS Colors

Colors are specified using predefined color names, or RGB, HEX.

**CSS Color Names**
In CSS, a color can be specified by using a predefined color name:
```css
h1 {  
    color:  green;  
}
```
In CSS, a color can be specified by using a predefined color HEX:
```css
h1 {  
    color:  #00ffff;  
}
```
In CSS, a color can be specified by using a predefined color RGB:
```css
h1 {  
    color:  rgb(255, 99, 71);  
}
```
## CSS  Backgrounds

The CSS background properties are used to add background effects for elements.

-   `background-color`
-   `background-image`
-   `background-repeat`
-   `background-attachment`
-   `background-position`
-   `background`  (shorthand property)

**CSS background-color**
The  `background-color`  property specifies the background color of an element.
```css
body {  
    background-color:  lightblue;  
}
```
**CSS background-image**
The  `background-image`  property specifies an image to use as the background of an element.
```csss
body {  
    background-image:  url("gitmag.jpg");  
}
```
**CSS background-repeat**
By default, the  `background-image`  property repeats an image both horizontally and vertically.
```css
body {  
    background-image:  url("gradient_bg.png");  
    background-repeat:  repeat-x;  
}
```
**CSS background-position**
```css
body {  
    background-image:  url('w3css.gif');  
    background-repeat:  no-repeat;  
    background-position:  center;  
}
```
**CSS background-attachment**
```css
body {  
    background-image:  url("img_tree.png");  
    background-repeat:  no-repeat;  
    background-position:  right top;  
    background-attachment:  fixed;  
}
```
 **CSS background - Shorthand property**
 To shorten the code, it is also possible to specify all the background properties in one single property. This is called a shorthand property.
```css
body {  
    background-color:  #ffffff;  
    background-image:  url("img_tree.png");  
    background-repeat:  no-repeat;  
    background-position:  right top;  
}
```
You can use the shorthand property  `background`:
```css
body {  
    background:  #ffffff url("img_tree.png") no-repeat right top;  
}
```
## CSS  Borders

**CSS Border Style**
The  `border-style`  property specifies what kind of border to display.

The following values are allowed:

-   `dotted`  - Defines a dotted border
-   `dashed`  - Defines a dashed border
-   `solid`  - Defines a solid border
-   `double`  - Defines a double border
-   `groove`  - Defines a 3D grooved border. The effect depends on the border-color value
-   `ridge`  - Defines a 3D ridged border. The effect depends on the border-color value
-   `inset`  - Defines a 3D inset border. The effect depends on the border-color value
-   `outset`  - Defines a 3D outset border. The effect depends on the border-color value
-   `none`  - Defines no border
-   `hidden`  - Defines a hidden border

The  `border-style`  property can have from one to four values (for the top border, right border, bottom border, and the left border).
```css
p {
    border-style:  solid;
}
```
**CSS Border Width**
The  `border-width`  property specifies the width of the four borders.
```css
p {  
    border-style:  solid;  
    border-width:  5px;  
}
```
***Specific Side Widths***
The  `border-width`  property can have from one to four values (for the top border, right border, bottom border, and the left border):
```css
p {  
    border-style:  solid;  
    border-width:  5px 20px; 
}
```
**CSS Border Color**
The  `border-color`  property is used to set the color of the four borders.
```css
p {  
    border-style:  solid;  
    border-color:  red;  
}
```
***Specific Side Colors***
The  `border-color`  property can have from one to four values (for the top border, right border, bottom border, and the left border).
```css
p {  
    border-style:  solid;  
    border-color:  red green blue yellow;   
}
```
**CSS Border - Shorthand Property**
The  `border`  property is a shorthand property for the following individual border properties:

-   `border-width`
-   `border-style`  (required)
-   `border-color`

The shorthand border for `<div>` element:
```css
p {  
    border:  5px solid red;  
}
```
**CSS Rounded Borders**
The  `border-radius`  property is used to add rounded borders to an element:
```css
p {  
    border:  2px solid red;  
    border-radius:  5px;  
}
```
## CSS Margins

The CSS  `margin`  properties are used to create space around elements, outside of any defined borders.

**Margin - Individual Sides**
CSS has properties for specifying the margin for each side of an element:
-   `margin-top`
-   `margin-right`
-   `margin-bottom`
-   `margin-left`

Set different margins for all four sides of a `<p>` element:
```css
p {  
    margin-top:  100px;  
    margin-bottom:  100px;  
    margin-right:  150px;  
    margin-left:  80px;  
}
```
**Margin - Shorthand Property**
Use the margin shorthand property with four values:
```css
p {  
    margin:  25px 50px 75px 100px;  
}
```

**The auto Value**
You can set the margin property to  `auto`  to horizontally center the element within its container.
```css
div {  
    width:  300px;  
    margin:  auto;  
    border:  1px solid red;  
}
```
**Margin Collapse**
Top and bottom margins of elements are sometimes collapsed into a single margin that is equal to the largest of the two margins.
```css
h1 {  
    margin:  0 0 50px 0;  
}
```
## CSS Padding

The CSS  `padding`  properties are used to generate space around an element's content, inside of any defined borders.

**Padding - Individual Sides**
CSS has properties for specifying the padding for each side of an element:
-   `padding-top`
-   `padding-right`
-   `padding-bottom`
-   `padding-left`

Set different padding for all four sides of a `<div>` element:
```css
div {  
    padding-top:  50px;  
    padding-right:  30px;  
    padding-bottom:  50px;  
    padding-left:  80px;  
}
```
**Padding - Shorthand Property**
Use the padding shorthand property with four values:
```css
div {  
    padding:  25px 50px 75px 100px;  
}
```
## CSS Height and Width

The CSS  `height`  and  `width`  properties are used to set the height and width of an element.
-   `auto` : This is default. The browser calculates the height and width
-   `length` : Defines the height/width in px, cm etc.
-   `%` : Defines the height/width in percent of the containing block
-   `initial` : Sets the height/width to its default value
-   `inherit` : The height/width will be inherited from its parent value

Set the height and width of a `<div>` element:
```css
div {  
    height:  200px;  
    width:  50%;  
    background-color:  powderblue;  
}
```
Set the height and width of another `<div>` element:
```css
div {  
    height:  100px;  
    width:  500px;  
    background-color:  powderblue;  
}
```
## The CSS Box Model

In CSS, the term "box model" is used when talking about design and layout.
The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content.

-   **Content**  - The content of the box, where text and images appear
-   **Padding**  - Clears an area around the content. The padding is transparent
-   **Border**  - A border that goes around the padding and content
-   **Margin**  - Clears an area outside the border. The margin is transparent

Demonstration of the box model:
```css
div {  
    width:  300px;  
    border:  15px solid green;  
    padding:  50px;  
    margin:  20px;  
}
```
## CSS Text

**CSS Text Alignment**
The  `text-align`  property is used to set the horizontal alignment of a text.
```css
h1 {  
    text-align:  center;  
}
```
When the `text-align` property is set to "justify",
```css
div {  
    text-align:  justify;  
}
```
**Text Direction**
The  `direction`  properties can be used to change the text direction of an element:
```css
p {  
    direction:  rtl;  
}
```
 **Text Decoration**
 The  `text-decoration`  property is used to set or remove decorations from text.
```css
a {  
    text-decoration:  none;  
}
```
 **Text Transformation**
 The  `text-transform`  property is used to specify uppercase and lowercase letters in a text.
```css
p.uppercase {  
    text-transform:  uppercase;  
}
```
**Line Height**
The  `line-height`  property is used to specify the space between lines:
```css
p {  
    line-height:  0.8;  
}
```
**Word Spacing**
The  `word-spacing`  property is used to specify the space between the words in a text.
```css
h1 {  
    word-spacing:  10px;  
}  
  
h2 {  
    word-spacing:  -5px;  
}
```
**Text Shadow**
The  `text-shadow`  property adds shadow to text.
```css
h1 {  
    text-shadow:  2px 2px 5px red;  
}
```
## CSS Fonts

**font-family**
In CSS, we use the  `font-family`  property to specify the font of a text.
```css
.p {  
    font-family:  Times;  
}
```
**Fallback Fonts**
Here, there are three font types: Tahoma, Verdana, and sans-serif. The second and third fonts are backups, in case the first one is not found.
```css
p {  
    font-family:  Tahoma, Verdana, sans-serif;  
}
```
**Font Style**
The  `font-style`  property is mostly used to specify italic text.
```css
p {  
    font-style:  normal;  
}
```
 **Font Weight**
 The  `font-weight`  property specifies the weight of a font.
```css
p.thick {  
    font-weight:  bold;  
}
```
**Font Size**
The  `font-size`  property sets the size of the text.
```css
h1 {  
    font-size:  40px;  
}
```
**The CSS Font Property**
To shorten the code, it is also possible to specify all the individual font properties in one property.
The  `font`  property is a shorthand property for:

-   `font-style`
-   `font-variant`
-   `font-weight`
-   `font-size/line-height`
-   `font-family`

Use  `font`  to set several font properties in one declaration:
```css
p {  
    font:  20px Arial, sans-serif;  
}
```
## How To Add Icons

**Bootstrap Icons**
To use the Bootstrap glyphicons, add the following line inside the  `<head>`  section of your HTML page:
```html
<!DOCTYPE html>  
<html>  
<head>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.5.0/font/bootstrap-icons.css">
</head>  
<body>  
    <i class="bi bi-alarm"></i>
    <i class="bi bi-telegram"></i>
    <i class="bi bi-tools"></i>
    <i class="bi bi-tag"></i>
    <i class="bi bi-sun"></i> 
</body>  
</html>
```
**Google Icons**
To use the Google icons, add the following line inside the  `<head>`  section of your HTML page:
```html
<!DOCTYPE html>  
<html>  
<head>  
    <link rel="stylesheet"  href="https://fonts.googleapis.com/icon?family=Material+Icons">  
</head>  
<body>  
    <i class="material-icons">cloud</i>  
    <i class="material-icons">favorite</i>  
    <i class="material-icons">attachment</i>  
    <i class="material-icons">computer</i>  
    <i class="material-icons">traffic</i>  
</body>  
</html>
```
## CSS  Lists

In HTML, there are two main types of lists:
-   unordered lists (`<ul>`) - the list items are marked with bullets
-   ordered lists (`<ol>`) - the list items are marked with numbers or letters

**Different List Item Markers**
The  `list-style-type`  property specifies the type of list item marker.
```css
ul {  
    list-style-type:  circle;  
}
```
**Remove Default Settings**
The `list-style-type:none` property can also be used to remove the markers/bullets. Note that the list also has default margin and padding.
```css
ul {  
    list-style-type:  none;  
    margin:  0;  
    padding:  0;  
}
```
## CSS  Layout - The display  Property
The  `display`  property is the most important CSS property for controlling layout.

***Block-level Elements***
Examples of block-level elements:

-   `<div>`
-   `<h1> - <h6>`
-   `<p>`
-   `<form>`
-   `<header>`
-   `<footer>`
-   `<section>`

***Inline Elements***
Examples of inline elements:

-   `<span>`
-   `<a>`
-   `<b>`
-   `<img>`

**Display: none;**
`display: none;`  is commonly used with JavaScript to hide and show elements without deleting and recreating them. Take a look at our last example on this page if you want to know how this can be achieved.

**Override The Default Display Value**
  As mentioned, every element has a default display value. However, you can override this.
```css
li {  
    display:  inline;  
}

span {  
    display:  block;  
}
```
## CSS  Layout - The position  Property
The  `position`  property specifies the type of positioning method used for an element (static, relative, fixed, absolute or sticky).

**Position Property**
The  `position`  property specifies the type of positioning method used for an element.

There are five different position values:

-   `static`
-   `relative`
-   `fixed`
-   `absolute`
-   `sticky`

**position: static;**
HTML elements are positioned static by default.
Static positioned elements are not affected by the top, bottom, left, and right properties.
```css
div {  
    position:  static;  
    border:  3px solid #73AD21;  
}
```
**position: relative;**
An element with  `position: relative;`  is positioned relative to its normal position.
```css
div{  
    position:  relative;  
    left:  30px;  
    border:  3px solid #73AD21;  
}
```
**position: fixed;**
An element with  `position: fixed;`  is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used to position the element.
```css
div.fixed {  
    position:  fixed;  
    bottom:  0;  
    right:  0;  
    width:  300px;  
    border:  3px solid #73AD21;  
}
```
**position: absolute;**
An element with  `position: absolute;`  is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).
```css
div.relative {  
    position:  relative;  
    width:  400px;  
    height:  200px;  
    border:  3px solid #73AD21;  
}  

div.absolute {  
    position:  absolute;  
    top:  80px;  
    right:  0;  
    width:  200px;  
    height:  100px;  
    border:  3px solid #73AD21;  
}
```
**position: sticky;**
An element with  `position: sticky;`  is positioned based on the user's scroll position.
```css
div.sticky {  
    position:  -webkit-sticky;  /* Safari */  
    position:  sticky;  
    top:  0;  
    background-color:  green;  
    border:  2px solid #4CAF50;  
}
```
**Overlapping Elements**
When elements are positioned, they can overlap other elements.

The  `z-index`  property specifies the stack order of an element (which element should be placed in front of, or behind, the others).
```css
img {  
    position:  absolute;  
    left:  0px;  
    top:  0px;  
    z-index:  -1;  
}
```
## CSS  Layout - Overflow

**Overflow**
The CSS  `overflow`  property controls what happens to content that is too big to fit into an area.

The  `overflow`  property has the following values:

-   `visible`  - Default. The overflow is not clipped. The content renders outside the element's box
-   `hidden`  - The overflow is clipped, and the rest of the content will be invisible
-   `scroll`  - The overflow is clipped, and a scrollbar is added to see the rest of the content
-   `auto`  - Similar to  `scroll`, but it adds scrollbars only when necessary

**overflow: visible**
By default, the overflow is  `visible`, meaning that it is not clipped and it renders outside the element's box:
```css
div {  
    width:  200px;  
    height:  50px;  
    background-color:  #eee;  
    overflow:  visible;  
}
```
**overflow: hidden**
With the  `hidden`  value, the overflow is clipped, and the rest of the content is hidden:
```css
div {  
    overflow:  hidden;  
}
```
**overflow: scroll**
Setting the value to  `scroll`, the overflow is clipped and a scrollbar is added to scroll inside the box. Note that this will add a scrollbar both horizontally and vertically (even if you do not need it):
```css
div {  
    overflow:  scroll;  
}
```
**overflow: auto**
The  `auto`  value is similar to  `scroll`, but it adds scrollbars only when necessary:
```css
div {  
    overflow:  auto;  
}
```
**overflow-x and overflow-y**
The  `overflow-x`  and  `overflow-y`  properties specifies whether to change the overflow of content just horizontally or vertically (or both):

`overflow-x`  specifies what to do with the left/right edges of the content.  
`overflow-y`  specifies what to do with the top/bottom edges of the content.
```css
div {  
    overflow-x:  hidden;  /* Hide horizontal scrollbar */  
    overflow-y:  scroll;  /* Add vertical scrollbar */  
}
```
## CSS  Layout - float and clear

The CSS  `float`  property specifies how an element should float.
The CSS  `clear`  property specifies what elements can float beside the cleared element and on which side.

**The Float Property**
The  `float`  property is used for positioning and formatting content e.g. let an image float left to the text in a container.

The  `float`  property can have one of the following values:

-   `left`  - The element floats to the left of its container
-   `right`  - The element floats to the right of its container
-   `none`  - The element does not float (will be displayed just where it occurs in the text). This is default
-   `inherit`  - The element inherits the float value of its parent


**float: right;**
The following example specifies that an image should float to the  **right**  in a text:
```css
img {  
    float:  right;  
}
```
**float: left;**
The following example specifies that an image should float to the  **left**  in a text:
```css
img {  
    float:  left;  
}
```
**No float**
In the following example the image will be displayed just where it occurs in the text (float: none;):
```css
img {  
    float:  none;  
}
```    
**Float Next To Each Other**
Normally div elements will be displayed on top of each other. However, if we use  `float: left`  we can let elements float next to each other:
```css
div {  
    float:  left;  
    padding:  15px;  
}  
.div1 {  
    background:  red;  
}  
.div2 {  
    background:  yellow;  
}  
.div3 {  
    background:  green;  
}
```
**Clear Property**
The  `clear`  property specifies what elements can float beside the cleared element and on which side.
```css
div {  
    clear:  both;  
}
```
## CSS  Layout - display: inline-block
Compared to  `display: inline`, the major difference is that  `display: inline-block`  allows to set a width and height on the element.
Also, with  `display: inline-block`, the top and bottom margins/paddings are respected, but with  `display: inline`  they are not.
```css
span.a {  
    display:  inline;  /* the default for span */  
    width:  100px;  
    height:  100px;  
    padding:  5px;  
    border:  1px solid blue;  
    background-color:  yellow;  
}  
span.b {  
    display:  inline-block;  
    width:  100px;  
    height:  100px;  
    padding:  5px;  
    border:  1px solid blue;  
    background-color:  yellow;  
}  
span.c {  
    display:  block;  
    width:  100px;  
    height:  100px;  
    padding:  5px;  
    border:  1px solid blue;  
    background-color:  yellow;  
}
```
## CSS  Combinators
A CSS selector can contain more than one simple selector. Between the simple selectors, we can include a combinator.
-   descendant selector (space)
-   child selector (>)
-   adjacent sibling selector (+)
-   general sibling selector (~)

**Descendant Selector**
The descendant selector matches all elements that are descendants of a specified element.
```css
div p {  
    background-color:  yellow;  
}
```
**Child Selector (>)**
The child selector selects all elements that are the children of a specified element.
```css
div > p {  
    background-color:  yellow;  
}
```
**Adjacent Sibling Selector (+)**
The adjacent sibling selector is used to select an element that is directly after another specific element.
```css
div + p {  
    background-color:  yellow;  
}
```
**General Sibling Selector (~)**
The general sibling selector selects all elements that are siblings of a specified element.
```css
div ~ p {  
    background-color:  yellow;  
}
```
## CSS  Pseudo - Classes
A pseudo-class is used to define a special state of an element.

For example, it can be used to:

-   Style an element when a user mouses over it
-   Style visited and unvisited links differently
-   Style an element when it gets focus

**Syntax**
The syntax of pseudo-classes:
```css
a:hover {  
    color:  #FF00FF;  
}
```
**Anchor Pseudo-classes**
Links can be displayed in different ways:
```css
/* unvisited link */  
a:link {  
    color:  #FF0000;  
}  
/* visited link */  
a:visited {  
    color:  #00FF00;  
}  
/* mouse over link */  
a:hover {  
    color:  #FF00FF;  
}  
/* selected link */  
a:active {  
    color:  #0000FF;  
}
```
**Pseudo-classes and CSS Classes**
Pseudo-classes can be combined with CSS classes:
```css
a:hover {  
    color:  #ff0000;  
}
```
**Simple Tooltip Hover**
Hover over a <div> element to show a <p> element (like a tooltip):
```css
p {  
    display:  none;  
    background-color:  yellow;  
    padding:  20px;  
}  
  
div:hover p {  
    display:  block;  
}
```
**CSS - The :first-child Pseudo-class**
The  `:first-child`  pseudo-class matches a specified element that is the first child of another element.
```css
p:first-child {  
    color:  blue;  
}
```
**Match the first <i> element in all <p> elements**
In the following example, the selector matches the first `<i>` element in all `<p>` elements:
```css
p i:first-child {  
    color:  blue;  
}
```
**Match all <i> elements in all first child `<p>` elements**
In the following example, the selector matches all <i> elements in <p> elements that are the first child of another element:
```css
p:first-child i {  
    color:  blue;  
}
```
## CSS Opacity
The  `opacity`  property specifies the opacity/transparency of an element.
```css
img  {  
    opacity:  0.5;  
}
img:hover {  
    opacity:  1.0;  
}
```
## CSS  Attribute  Selectors
The  `[attribute]`  selector is used to select elements with a specified attribute.
```css
a[target] {  
    background-color:  yellow;  
}
```
The  `[attribute="value"]`  selector is used to select elements with a specified attribute and value.
```css
a[target="_blank"] {  
    background-color:  yellow;  
}
```
## CSS  The !important Rule
The  `!important`  rule in CSS is used to add more importance to a property/value than normal.
```css
#myid {  
    background-color:  blue  !important;  
}
```
