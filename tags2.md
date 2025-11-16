# Common HTML Tags

Let me explain the most frequently used HTML tags that form the foundation of web content.

---

## 1. Heading Tags (`<h1>` to `<h6>`)

Headings are used to define titles and subtitles on a webpage. There are six levels of headings, from most important to least important.

```html
<h1>Main Heading - Largest</h1>
<h2>Sub Heading</h2>
<h3>Sub-sub Heading</h3>
<h4>Smaller Heading</h4>
<h5>Even Smaller</h5>
<h6>Smallest Heading</h6>
```

### Key Points:
- **`<h1>`** should be used only once per page (for the main title)
- Headings help with SEO (Search Engine Optimization)
- They create a hierarchy and improve accessibility for screen readers
- Don't skip levels (e.g., don't jump from h1 to h4)

---

## 2. Paragraph Tag (`<p>`)

The paragraph tag is used to define blocks of text. Browsers automatically add space before and after paragraphs.

```html
<p>This is a paragraph of text. It can contain multiple sentences and will automatically wrap to the next line when needed.</p>

<p>This is another paragraph. Each paragraph tag creates a new block of text with spacing.</p>
```

### Key Points:
- Creates line breaks before and after
- Cannot contain block-level elements like div or other paragraphs
- Good for organizing text content

---

## 3. Anchor Tag (`<a>`) - Links

The anchor tag creates hyperlinks that allow users to navigate between pages or jump to different sections.

### External Links
```html
<a href="https://www.google.com">Visit Google</a>
```

### Internal Links (Same Website)
```html
<a href="about.html">About Us</a>
<a href="/contact">Contact Page</a>
```

### Open in New Tab
```html
<a href="https://www.example.com" target="_blank">Open in New Tab</a>
```

### Email Links
```html
<a href="mailto:someone@example.com">Send Email</a>
```

### Phone Links
```html
<a href="tel:+1234567890">Call Us</a>
```

### Jump to Section (Anchor Links)
```html
<!-- Link to section -->
<a href="#section1">Go to Section 1</a>

<!-- Target section -->
<h2 id="section1">Section 1</h2>
```

### Download Links
```html
<a href="document.pdf" download>Download PDF</a>
```

### Important Attributes:
- **`href`** - Specifies the destination URL (required)
- **`target`** - Where to open the link:
  - `_blank` - New tab/window
  - `_self` - Same frame (default)
  - `_parent` - Parent frame
  - `_top` - Full window
- **`title`** - Tooltip text when hovering
- **`rel`** - Relationship (e.g., `nofollow`, `noopener`)

```html
<a href="https://example.com" target="_blank" title="Visit Example" rel="noopener">
    Example Site
</a>
```

---

## 4. Image Tag (`<img>`)

The image tag is used to embed images in a webpage. It's a **self-closing tag** (no closing tag needed).

### Basic Syntax
```html
<img src="image.jpg" alt="Description of image">
```

### With Additional Attributes
```html
<img src="photo.jpg" 
     alt="A beautiful sunset" 
     width="500" 
     height="300"
     title="Sunset Photo">
```

### Responsive Images
```html
<img src="image.jpg" alt="Description" style="max-width: 100%; height: auto;">
```

### Image from URL
```html
<img src="https://www.example.com/images/photo.jpg" alt="Online image">
```

### Image as a Link
```html
<a href="https://www.example.com">
    <img src="logo.png" alt="Company Logo">
</a>
```

### Important Attributes:
- **`src`** - Source/path to the image (required)
- **`alt`** - Alternative text for accessibility and SEO (required)
- **`width`** - Width in pixels
- **`height`** - Height in pixels
- **`title`** - Tooltip text
- **`loading`** - Lazy loading: `loading="lazy"`

### Image Formats:
- **JPEG/JPG** - Photos, complex images
- **PNG** - Images with transparency
- **GIF** - Animations
- **SVG** - Vector graphics, logos
- **WebP** - Modern, efficient format

---

## 5. Line Break (`<br>`) and Horizontal Rule (`<hr>`)

### Line Break
Creates a single line break without starting a new paragraph.

```html
<p>This is line one<br>This is line two</p>
```

### Horizontal Rule
Creates a horizontal line to separate content.

```html
<p>Section 1</p>
<hr>
<p>Section 2</p>
```

---

## Practical Example: Combining Tags

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My Web Page</title>
</head>
<body>
    <h1>Welcome to My Website</h1>
    
    <p>This is an introduction paragraph about my website. It contains useful information for visitors.</p>
    
    <h2>About Me</h2>
    <img src="profile.jpg" alt="My profile picture" width="200">
    
    <p>Hello! I'm a web developer. Visit my <a href="portfolio.html">portfolio</a> to see my work.</p>
    
    <h2>Contact Information</h2>
    <p>
        Email: <a href="mailto:hello@example.com">hello@example.com</a><br>
        Phone: <a href="tel:+1234567890">+123-456-7890</a>
    </p>
    
    <hr>
    
    <h3>External Links</h3>
    <p>
        Follow me on <a href="https://github.com" target="_blank">GitHub</a> and 
        <a href="https://linkedin.com" target="_blank">LinkedIn</a>
    </p>
</body>
</html>
```

