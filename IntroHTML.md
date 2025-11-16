# Introduction to HTML

**HTML** stands for **HyperText Markup Language**. It is the standard markup language used to create and structure content on the web. HTML uses "tags" to define elements like headings, paragraphs, links, images, and more.

## What is HTML?

- **Markup Language**: HTML is not a programming language; it's a markup language that uses tags to annotate content
- **Building Blocks of Web**: Every website you visit is built using HTML as its foundation
- **Works with CSS and JavaScript**: HTML provides structure, CSS adds styling, and JavaScript adds interactivity

## History of HTML

**1991** - Tim Berners-Lee created the first version of HTML while working at CERN. It had only 18 tags.

**1995** - HTML 2.0 was released as the first standard HTML specification.

**1997** - HTML 3.2 became a W3C Recommendation, adding support for tables, applets, and text flow around images.

**1999** - HTML 4.01 was released with better support for stylesheets, scripting, and accessibility.

**2000** - XHTML 1.0 was introduced as a reformulation of HTML 4 as an XML application.

**2008** - First public draft of HTML5 was released.

**2014** - HTML5 became the official W3C Recommendation.

**Present** - HTML is now a "living standard" maintained by WHATWG (Web Hypertext Application Technology Working Group), meaning it's continuously updated.

## Structure of an HTML Document

Every HTML document follows a basic structure:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page Title</title>
</head>
<body>
    <h1>This is a Heading</h1>
    <p>This is a paragraph.</p>
</body>
</html>
```

### Breaking Down the Structure:

**`<!DOCTYPE html>`** - Declares the document type and HTML version (HTML5). It must be the first line.

**`<html>`** - The root element that contains all other HTML elements. The `lang` attribute specifies the language.

**`<head>`** - Contains metadata about the document (not visible on the page):
  - `<meta charset="UTF-8">` - Defines character encoding
  - `<meta name="viewport">` - Makes the page responsive on mobile devices
  - `<title>` - Sets the title shown in browser tabs

**`<body>`** - Contains all visible content that appears on the webpage (text, images, links, etc.)

## HTML vs HTML5: Key Differences

### HTML (HTML4)

- Released in 1999
- Limited semantic elements
- Required plugins (like Flash) for audio, video
- No native support for vector graphics
- Basic form elements only
- Less support for mobile devices
- Weaker error handling

### HTML5

**New Semantic Elements**: Better structure and meaning
- `<header>`, `<footer>`, `<nav>`, `<article>`, `<section>`, `<aside>`, `<main>`

**Multimedia Support**: Native audio and video without plugins
- `<audio>` and `<video>` tags
- No need for Flash Player

**Graphics**: Built-in drawing capabilities
- `<canvas>` for 2D graphics
- `<svg>` for scalable vector graphics

**Enhanced Forms**: More input types and attributes
- `email`, `url`, `date`, `time`, `number`, `range`, `color`
- Attributes like `placeholder`, `required`, `autofocus`

**APIs and Storage**: 
- Geolocation API
- Local Storage and Session Storage
- Drag and Drop API
- Web Workers for background processing

**Better Mobile Support**: Responsive design features built-in

**Improved Accessibility**: Better support for screen readers and assistive technologies

**Offline Capabilities**: Application cache for offline web apps

## Basic HTML Elements

**Headings**: `<h1>` to `<h6>` (h1 being the largest)

**Paragraph**: `<p>This is text</p>`

**Links**: `<a href="url">Link text</a>`

**Images**: `<img src="image.jpg" alt="Description">`

**Lists**: 
- Unordered: `<ul><li>Item</li></ul>`
- Ordered: `<ol><li>Item</li></ol>`

**Division**: `<div>` for grouping content

**Span**: `<span>` for inline styling

## Why HTML5 Matters

HTML5 represents a major evolution in web development. It simplified many complex tasks, eliminated the need for third-party plugins, improved performance, and made websites more accessible and mobile-friendly. Today, when people say "HTML," they typically mean HTML5, as it's the current standard used across the web.
