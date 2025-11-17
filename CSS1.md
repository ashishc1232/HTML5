
# **00:00 – 01:30 — Opening**

**You say:**

“Welcome everyone.
In this session, you will learn the fundamentals of CSS, how to target elements using selectors, and how to work with colors in a modern way.
Even though this is a recorded class, follow along by coding on your side and pausing whenever needed.”

---

# **01:30 – 05:00 — What is CSS? (Modern Explanation)**

**You say:**

“CSS stands for Cascading Style Sheets.
While HTML gives the structure, CSS controls the visual presentation — spacing, colors, layout, responsiveness.

The word *Cascading* means:

* If multiple rules apply to the same element, CSS decides which rule wins based on **specificity**, **source order**, and **importance**.

Today, we’ll focus on the absolute basics:

1. How to write CSS
2. How to use selectors to target elements
3. How to apply colors in different formats”

---

# **05:00 – 09:00 — How to Apply CSS (3 Modern Ways)**

**You say:**

“There are three standard ways to apply CSS:

### 1. External CSS (Modern Best Practice)

```html
<link rel="stylesheet" href="styles.css">
```

Use this in real projects — clean, maintainable, scalable.

---

### 2. Internal CSS

```html
<style>
  h1 { color: blue; }
</style>
```

Placed in the `<head>` section — useful for small demos.

---

### 3. Inline CSS (Not recommended)

```html
<h1 style="color: red;">Hello</h1>
```

Avoid using inline style — bad for maintainability and hard to override.

We’ll focus on **external and internal CSS** in this class.”

---

# **09:00 – 17:00 — CSS Selectors (Core Topic)**

**You say:**

“To style anything, you must correctly select elements.
Selectors tell CSS *what* to style.

Let’s go through the essential ones.”

---

### **1. Element Selector**

Targets all elements of a given type.

```css
p {
  font-size: 16px;
}
```

---

### **2. Class Selector (Most Common)**

Used for reusable styles.

```css
.box {
  padding: 20px;
}
```

HTML:

```html
<div class="box"></div>
```

---

### **3. ID Selector**

Unique style for a single element. Use rarely.

```css
#header {
  background: black;
}
```

---

### **4. Universal Selector**

Targets everything.

```css
* {
  margin: 0;
  padding: 0;
}
```

---

### **5. Descendant Selector**

Targets elements inside another element.

```css
nav a {
  text-decoration: none;
}
```

---

### **6. Child Selector**

Direct children only.

```css
ul > li {
  font-weight: bold;
}
```

---

### **7. Attribute Selector (Modern and Useful)**

```css
input[type="email"] {
  border-color: blue;
}
```

---

### **8. Pseudo-class Selector**

React to states.

```css
button:hover {
  background: black;
  color: white;
}
```

---

### **9. Pseudo-element Selector**

Targets a part of an element.

```css
p::first-line {
  font-weight: bold;
}
```

**You say:**
“These are the selectors used in real projects.
Avoid relying only on classes — mix semantic HTML with appropriate selectors.”

---

# **17:00 – 26:00 — Working With Colors (Modern CSS)**

**You say:**

“CSS gives several color formats.
Understanding them is essential for UI work.”

---

### **1. Named Colors (Basic)**

```css
color: red;
```

Limited and rarely used in production.

---

### **2. Hex Colors (Most Common)**

```css
color: #3498db;
```

Hex decides the exact color based on red, green, blue values.

---

### **3. RGB / RGBA**

```css
color: rgb(255, 0, 0);
color: rgba(255, 0, 0, 0.5);
```

RGBA adds transparency (0 to 1).

---

### **4. HSL / HSLA (Modern & UI-Friendly)**

```css
color: hsl(200, 80%, 50%);
```

This is the most intuitive for designers:

* H = Hue (color wheel)
* S = Saturation
* L = Lightness

---

### **5. CSS Color Variables (Modern Must-Have)**

Define in root:

```css
:root {
  --primary-color: #4a90e2;
}
```

Use anywhere:

```css
h1 {
  color: var(--primary-color);
}
```

**You say:**
“Always use CSS variables in medium or large projects.
This makes themes, dark mode, and maintainability extremely easy.”

---

# **26:00 – 31:00 — Quick Practical Demo (Small Live Example)**

**You say:**

“Let’s now combine selectors and colors into a mini example.”

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>CSS Demo</title>
  <style>
    :root {
      --primary: #2c3e50;
      --accent: #e67e22;
    }

    body {
      font-family: Arial;
      background: #f5f5f5;
    }

    h1 {
      color: var(--primary);
    }

    p.intro {
      color: var(--accent);
    }

    button:hover {
      background: var(--accent);
      color: white;
    }
  </style>
</head>
<body>
  <h1>Welcome to CSS</h1>
  <p class="intro">Understanding selectors and colors is the foundation of styling.</p>
  <button>Hover Me</button>
</body>
</html>
```

**You say:**
“This small example already uses semantic selectors, a class, pseudo-classes, and CSS variables.”

---

# **31:00 – 35:00 — Conclusion + What’s Next**

**You say:**

“Today, we learned the fundamentals of CSS:

* What CSS is
* How to write and apply it
* Essential selectors
* Modern color systems and CSS variables

These basics are the foundation for all UI development.

In the next session, we’ll go deeper into:

* Box Model
* Margin, Padding, Border
* Display types (block, inline, inline-block)
* Flexbox introduction

Make sure to revise everything shown today.
Thank you for watching.”




Just tell me.
