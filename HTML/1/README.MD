## Section 1. The Absolute Beginner: Foundational Concepts 👶

### Chapter 1 - HTML Core

#### What is HTML?

HTML (HyperText Markup Language) is the standard markup language used to create web pages. 
It defines the structure and content of a webpage by using a series of elements (also known as tags) that tell the browser how to display the information.
HTML is not a programming language but a markup language, meaning it uses tags to define elements within a document.

HTML documents are made up of elements such as headings, paragraphs, links, images, and more. 
These elements can be nested inside one another to create complex layouts. 
Every webpage on the internet has an HTML file that serves as its foundation. 
Without HTML, there would be no way to structure content for display on the web.

HTML is often used in conjunction with CSS (Cascading Style Sheets) for styling and JavaScript for interactivity. 
Together, they form the core technologies of the web.

#### Syntax

In HTML, every element is composed of three main components:

1. Opening Tag: This is where an element begins, denoted by a less-than sign (`<`) followed by the element name and optional attributes, ending with a greater-than sign (`>`).

For example:
   ```html
   <p>
   ```
Here, <p> is the opening tag for a paragraph.

2. Content: This is the actual text or other elements that appear between the opening and closing tags.

`<p>This is the content of the paragraph.</p>`
3. Closing Tag: This marks the end of an element, with a forward slash (/) before the element name. For example:

`</p>`
Closing tags are required for most elements in HTML.

Some elements, known as self-closing or void elements, do not have content and do not require closing tags.
Examples include <img> and <br>.

#### Attributes
Attributes are properties that provide additional information about an element. 
They are always specified in the opening tag of an element, usually in the format attribute="value". 

For example:
`<a href="https://www.example.com">Visit Example</a>`
In this case, href is an attribute with the value "https://www.example.com", which tells the browser where to navigate when the link is clicked.

Other common attributes include:
* src: Used in <img> tags to specify the image source.
* alt: Provides alternative text for images if they fail to load.
* class: Assigns a class name for CSS styling or JavaScript manipulation.
* id: Assigns a unique identifier for an element.

Attributes can also be used to control how elements behave or look on a page, such as setting the width of an image or making a button disabled.

#### HTML Intro - Example
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Blog Post</title>
</head>
<body>

    <h1>Hello, HTML!</h1>

    <p>This is my first blog post where I'm practicing my HTML skills. Every web page is built on HTML, which provides the essential structure for all of the content you see.</p>

    <p>I'm learning so much! To read more about my journey, <a href="about.html">click here to visit the about page</a>.</p>

    <img src="https://via.placeholder.com/600x400" alt="A placeholder image for a blog post.">

    <p>You can also check out the official <a href="https://developer.mozilla.org/en-US/docs/Web/HTML" title="Visit the MDN Web Docs for HTML">MDN HTML documentation</a> for more information on the language.</p>

</body>
</html>
```

* The HTML code provided creates a single web page, likely for a blog post, by using fundamental HTML syntax and attributes.
It demonstrates how different elements are structured to form a complete, readable document.

* Document Structure
The code starts with <!DOCTYPE html>, which declares the document type as HTML5.
The entire page is contained within the <html> element, which has a lang="en" attribute to specify the language as English for accessibility and SEO.
The <head> section contains metadata not displayed on the page, such as the character set (<meta charset="UTF-8">) and the viewport settings (<meta name="viewport"...>) for responsive design.
The <title> tag sets the title that appears in the browser tab. The visible content of the page is all placed within the <body> element.

* Elements, Syntax, and Attributes

Within the body, the code uses various elements to structure content.
The `<h1>` tag defines the main heading of the page.
 This demonstrates the core HTML syntax of an opening tag (`<h1>`), content (Hello, HTML!), and a closing tag (`a`).
The <p> tags are used for paragraphs of text, further illustrating this fundamental syntax.

The code also effectively uses attributes to add properties to elements. 
The <a> (anchor) tag creates a hyperlink, and its href attribute specifies the URL of the destination page, in this case, a file named about.html within the same project. 
The <img> tag, a self-closing element, uses the src attribute to define the source of the image file and the alt attribute to provide a text description for screen readers or if the image fails to load. 
Finally, a title attribute on the second <a> tag provides extra information that appears as a tooltip when a user hovers over the link. 
The comments within the code (using ``) provide human-readable explanations of the purpose of each element.


#### HTML Core Questions
1. What does HTML stand for?
2. What are the three main parts of an HTML element?
3. Why are closing tags important in HTML?
4. Can all HTML elements be closed with a closing tag? Explain.
5. What is the purpose of attributes in HTML?
6. Give two examples of attributes and their usage.
7. How do you create a hyperlink in HTML using the <a> tag?
8. What is the difference between src and href attributes?
9. Why might you use an alt attribute in an image tag?
10. How do you define a paragraph in HTML?