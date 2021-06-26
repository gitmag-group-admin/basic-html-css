
## HTML

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

    <!doctype html>

## HTML Document structure

Simple HTML document

    <!doctype html>
    <html>
	    <head>
	    </head>
	    
	    <body>
	    </body>
    </html>

head: *Search engine information structure*
body: *User information structure*

## HTML document title

The `<title>` tag defines the title of the document. The title must be text-only, and it is shown in the browser's title bar or in the page's tab.

    <!doctype html>
    <html>
	    <head>
		    <title> GitMag website </title>
	    </head>
	    <body>
	    </body>
    </html>

## HTML content
The `<body>` tag defines the document's body.
There can only be one `<body>` element in an HTML document.

    <!doctype html>
    <html>
	    <head>
		    <title> GitMag website </title>
	    </head>
	    <body>
		   This is my website
	    </body>
    </html>

## Break line tag
The `<br>` tag inserts a single line break.

    My name is Sohrab <br> I am Programmer

## Horizontal tag
The `<hr>` tag defines a thematic break in an HTML page

    My name is Sohrab <hr> I am Programmer
    
## Paragraph tag
The HTML `<p>` element defines a paragraph.

    <p>This is first paragraph</p>
    <p>This is second paragraph</p>
    <p>This is third paragraph</p>

## Formatting tags
Formatting elements were designed to display special types of text:

`<b>` - Bold text
`<strong>` - Important text
`<i>` - Italic text
`<small>` - Smaller text
...

       <p>
        In publishing and <b>graphic design</b>, Lorem ipsum is a placeholder text commonly used to demonstrate the visual form of a document or a typeface without relying on <strong>meaningful content</strong>. 
       </p>
       <p>
        Lorem ipsum may be used as a placeholder before <i>final copy is available</i>.
       </p>

## Heading tags
The `<h1>` to `<h6>` tags are used to define HTML headings.

       <h1>heading1</h1>
       <h2>heading2</h2>
       <h3>heading3</h3>
       <h4>heading4</h4>
       <h5>heading5</h5>
       <h6>heading6</h6>

## HTML tag Attributes
\<html lang="en"> *HTML document content* \</html>
\<html lang='en'> *HTML document content* \</html>

    <!doctype html>
    <html lang="en">
	    <head>
		    <title> GitMag website </title>
	    </head>
	    
	    <body>
		   This is my website
	    </body>
    </html>

## Anchor tag

The `<a>` tag defines a hyperlink, which is used to link from one page to another.

    <a href="http://google.com"> Go to Google</a>

A linked page is normally displayed in the current browser window, unless you specify another target.

    <a href="http://google.com" target="_parent"> Go to Google</a>

> Target attribute values:
> _self: *Opens the linked document in the same frame as it was clicked (**this is default**)*
> _blank: *Opens the linked document in a new window or tab*
> _parent: *Opens the linked document in the parent frame*
> _top: *Opens the linked document in the full body of the window*

## Table tag
The `<table>` tag defines an HTML table.
An HTML table consists of one `<table>` element and one or more `<tr>` `<th>` and `<td>` elements.
 

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

How to add collapsed borders to a table:
	
      <table border="1">
       
      </table>

How to create a table with a caption:

    <table>
	    <caption> Table caption </caption>
    </table>
    
An HTML table with a `<thead>` and `<tbody>` element:

    <table>
	   <thead>
		   ...
	   </thead>
	   <tbody>
		   ...
	   </tbody>
    </table>
    
How to define table cells that span more than one row or one column:

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

## Image tag

The `<img>` tag is used to embed an image in an HTML page.

    <img src="logo.png" alt="GitMag.png" width="200" height="50" />

>src: *Specifies the path to the image*
> alt: *Specifies an alternate text for an image*
> width: *Specifies the width of an image*
> height: *Specifies the height of an image*

## List tag

**Order lists**
An ordered list starts with the `<ol>` tag. Each list item starts with the `<li>` tag.

    <ol>
        <li>Home</li>
        <li>About Us</li>
        <li>News</li>
        <li>Contact Us</li>
    </ol>
    
**Unorder list**
An unordered list starts with the `<ul>` tag. Each list item starts with the `<li>` tag.

    <ul>
	    <li>Home</li>
	    <li>About Us</li>
	    <li>News</li>
	    <li>Contact Us</li>
    </ul>
    
## Divider tag
The `<div>` tag defines a division or a section in an HTML document.
    
    <div id="header"> Website Header </div>
    <div id="navbar"> Website Navbar </div>
    <div id="main">
	    <div id="sidbar"> Website Sidebar </div>
	    <div id="content"> Website Content </div>
    </div>
    <div id="footer"> Website Footer </div>
    

## Semantic tags
*Semantic elements = elements with a meaning.*

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

## Forms
An HTML form is used to collect user input. The user input is most often sent to a server for processing.

    <form action="http://gitmag.ir" method="GET">
	    ...
    </form>

**Input tag**
One of the most used form element is the `<input>` element.
The `<input>` element can be displayed in several ways, depending on the `type` attribute.

    <label for="fname">First name:</label>  
    <input type="text" id="fname" name="fname">

> text: *Displays a single-line text input field*
> radio: *Displays a radio button (for selecting one of many choices)*
> checkbox: *Displays a checkbox (for selecting zero or more of many choices)*
> submit: *Displays a submit button (for submitting the form)*
> button: *Displays a clickable button*
> color: *Displays a color picker*
> file: *Display a "Browse" button for file uploads.*

**Textarea tag**
The `<textarea>` element defines a multi-line input field (a text area):

    <textarea name="message" rows="10" cols="30">  
	    The cat was playing in the garden.  
    </textarea>

**Select tag**
The `<select>` element defines a drop-down list:

    <select name="cars">  
        <option value="volvo">Volvo</option>  
        <option value="benz">Benz</option>  
        <option value="fiat">Fiat</option>  
        <option value="audi">Audi</option>  
    </select>
    

## Meta tags
The `<meta>` tag defines metadata about an HTML document. Metadata is data (information) about data.

    <head>  
	    <meta charset="UTF-8">  
	    <meta name="description" content="Free Web tutorials">  
	    <meta name="keywords" content="HTML, CSS, JavaScript">  
	    <meta name="author" content="John Doe">  
    </head>

> keywords: *Define keywords for search engines*
> description: *Define a description of your web page*
> author: *Define the author of a page*

## Comment in HTML
You can add comments to your HTML source by using the following syntax:

    <!-- This is a comment -->  
	    <p>This is a paragraph.</p>  
    <!-- Remember to add more information here -->
