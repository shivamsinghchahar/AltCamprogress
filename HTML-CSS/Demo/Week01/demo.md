# Week 1

### **Table of contents**

1. Intro to HTML & CSS
2. Getting to Know about Box-Model
3. Positioning

## Intro to HTML & CSS

*HTML*, or *Hypertext Markup Language* is used to give structure and meaning to the content with the help of headings, paragraphs or images. *CSS*, or *Cascading Style Sheets* is used to give style to appearance of our content by using fonts or colors.

*HTML* & *CSS* are independent of each other but they work together. CSS should never be written inside of HTML and vice versa.

### Common HTML Terms
#### Elements
Element is an Individual component that defines the structure and content of objects within a page. Some commonly used elements include headings, paragraphs, images and so on.

` HTML `
```html
	<h1>
	<a>
```
#### Tags
The use of less-than and greater-than surrounding an element creates what is known as a *tag*.

An *opening tag* marks the beginning of an element. 
for example

` HTML `
```html
	<a>
```
A *closing tag* marks the end of the element
for example

` HTML `
```html
	</a>
```

So the final tag will look like this

`HTML`
```html
	<a>...</a>
```

#### Attributes

*Attributes* are properties used to provide additional information about an element. The most common attributes are *id*, *class*, *src* and *href*.

Attributes are defined within an opening tag. An attribute has a *name* and a *value*. The format for the attribute includes the attribute name followed by an equals sign and then a quoted attribute value.

`HTML`
```html
	<a href="www.google.com">Google</a>
```
### HTML Document Structure

All HTML elements have a required structure that includes the following declaration and elements: `<!DOCTYPE html>`, `<html>`, `<head>`, and` <body>`.

The document type declaration, or  `<!DOCTYPE html>`, informs the web browser about the version of HTML being used. The `<html>` element signifies the beginning of html document.

The `<head>` element contains metadata and any content inside it is not displayed on the web page. It may include the document title, links to any external files, or any beneficial metadata.

All the visible content on the web page goes inside the `<body>` tag.

`HTML`
```html
	<!DOCTYPE html>
	<html lang="en">
	  <head>
	    <meta charset="utf-8">
	    <title>Hello World</title>
	  </head>
	  <body>
	    <h1>Hello World</h1>
	    <p>This is a web page.</p>
	  </body>
	</html>
```

### Common CSS Terms
#### Selectors

As the name suggests, *Selectors* help us select, or target the elements within our HTML on which we need to apply the styles. Selectors may include a combination of different qualifiers to select unique elements, all depending on how specific we wish to be. e.g., we may want to select all paragraphs on a page, or we may want to select only one paragraph on a page.

Selectors generally target an attribute value, such as an *id* or *class* value, or target the type of an element, such as `<h1>` or `<p>`. 

The below selector targets all the paragraphs.

`CSS`
```css
	p {
	 ...
	}
```

#### Properties

Once an element is selected , a property determines the style that will be applied to that element. There are numerous properties that we can use
*background*, *color*, *font-size*, *height*, and *width*.

In the following code we define *font-size* and *color*.

`CSS`
```css
	p {
		color: ...;
		font-size: ...;
	}
```
#### Values

Coupled with an appropriate property, a value can determine the behaviour of the selected element.

In the below example we select all the `<p>` elements and apply *color* property to be *red* and the value of *font-size* to be *16px*

`CSS`
```css
	p {
		color: red;
		font-size: 16px;
	}
```

### Types of Selectors

#### Type Selectors

*Type* selector targets the element by their type. For example, using *p* as selector targets all the paragraph elements in the web page.

`CSS`
```css
	p { ... }
```
`HTML`
```html
	<p>...</p>
	<p>...</p>
	<p>...</p>
```

#### Class Selectors

*Class* Selectors allows us to select an element based on its *'class'* attribute
value. Class selectors are a little more specific than the type selectors because they select a group of elements.

`CSS`
```css
	.my-class { ... }
```
`HTML`
```html
	<div class="my-class">...</div>
	<p class="my-class">...</p>
```

#### ID Selectors

*ID* selectors are even more precise than the class selectors, as they target only unique element at a time. 

*id* attribute can only be used once per page.

`CSS`
```css
	#my-id { ... }
```
`HTML`
```html
	<div id="my-id"> ... </div>
```

#### Additional Selectors

All the selectors that we discussed till now are common selectors, But there are many other [advanced selectors](https://learn.shayhowe.com/advanced-html-css/complex-selectors/) which are not in scope of this lesson.

### Referencing CSS
To link our CSS with our HTML, we need to reference our CSS file within our
HTML file.

Within the `<head>` element of the HTML document, the `<link>` element is used to define relationship between the HTML file and CSS file. We use the *rel* attribute with a value of *stylesheet* to specify the relationship and *href* attribute is used to identify the location, or path, of the CSS file.

`HTML`
```html
	<head>
		<link rel="stylesheet" href="main.css">
	</head>
``` 

### CSS Resets
Every browser has its default styles for different elements. So, to ensure cross-browser compatibility, CSS resets have become widely used.

CSS resets take every common HTML element with a predefined style and assigns one unified style for all browsers.

One of the most popular resets is [Eric Meyer's](https://meyerweb.com/eric/tools/css/reset/) reset, which has been adapted to include styles for the new HTML5 elements.

## HTML

After knowing the basics of HTML and CSS, it's time to dig a little deeper into HTML.

In order to start building websites, we need to understand which HTML elements are best to display different types of content. It's also important to understand how elements are visually displayed on a web page, as well as what different elements mean semantically.

It is very important to use an appropriate element for the content.

### Semantics

Semantics within HTML is a practice of giving content on the page meaning and structure by using a proper element.

We'll talk about semantic elements as we move forward. 

### Divisions & Spans

