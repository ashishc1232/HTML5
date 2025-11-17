

# ⭐ **CSS POSITION: STICKY**

*(15–20+ minutes of rich content — perfect for trimming into your final lesson)*

---

# **00:00 – 01:30 — Introduction**

**You say:**

“Welcome back.
We have now covered static, relative, absolute, and fixed positioning.
Today we are learning one of the most interesting and slightly confusing behaviors in CSS: **position: sticky**.

Sticky acts like a hybrid between **relative** and **fixed**.
It behaves normally until a certain point, and then locks into position as the page scrolls.”

---

# **01:30 – 05:00 — What is position: sticky? (Concept)**

**You say:**

“Position sticky is unique in the CSS world.
It behaves like:

* `position: relative` **before scrolling**
* `position: fixed` **after you scroll past a threshold**

This threshold is controlled by **top**, **left**, **right**, or **bottom**.

The moment the scroll reaches the defined offset, the element becomes fixed — but only within its parent container.”

---

# **05:00 – 08:00 — Visual Explanation (Verbal Diagram)**

Imagine a header inside a long section:

```
BEFORE scrolling:
-------------------------
[Section Title]
Paragraph
Paragraph
Paragraph
-------------------------
```

While scrolling:

```
Scrolling...
[Section Title]  <-- hits top: 0, becomes sticky
Paragraph
Paragraph
```

When leaving its parent:

```
Parent ends, sticky stops:
(it cannot float beyond its container)
```

**You say:**
“This behavior is unlike fixed, which stays on the screen at all times.”

---

# **08:00 – 13:00 — Basic Example**

### **HTML**

```html
<div class="section">
  <h2 class="title">Sticky Title</h2>
  <p>Lots of content...</p>
</div>
```

### **CSS**

```css
.section {
  height: 800px;
}

.title {
  position: sticky;
  top: 0;
  background: #fff;
  padding: 15px;
  border-bottom: 1px solid #ccc;
}
```

**You say:**

“Here the title behaves like a normal heading.
But when you scroll and the title touches the top edge (top: 0), it becomes sticky and stays visible until the section ends.”

---

# **13:00 – 17:00 — Sticky Requires Top/Bottom/Left/Right**

**You say:**

“One important rule that many beginners miss:

Sticky works **only** if you specify an offset:

```css
top: 0;
```

(or bottom, left, right depending on direction)

Without this, the element will never stick.”

### Wrong (doesn’t work)

```css
.position {
  position: sticky;
}
```

### Correct

```css
.position {
  position: sticky;
  top: 0;
}
```

---

# **17:00 – 21:00 — Sticky Respecting Parent Boundaries**

**You say:**

“This is the most misunderstood rule of sticky:

A sticky element **cannot** leave its parent container.

If the section ends, the sticky element stops sticking.”

### Example:

```
<section>
  <h2 class="sticky"></h2>
  Content...
</section>

The sticky element will unstick when the section ends.
```

**You say:**
“This is different from fixed.
Fixed attaches to the viewport and has no boundaries.”

---

# **21:00 – 26:00 — Real-World Example: Sticky Table Header**

### HTML

```html
<table>
  <thead>
    <tr class="header-row">
      <th>Name</th>
      <th>Age</th>
      <th>City</th>
    </tr>
  </thead>

  <tbody>
    <tr><td>...</td></tr>
    <tr><td>...</td></tr>
    <tr><td>...</td></tr>
    <!-- many rows -->
  </tbody>
</table>
```

### CSS

```css
.header-row {
  position: sticky;
  top: 0;
  background: white;
}
```

**You say:**
“This keeps table headers visible as you scroll — very useful for large datasets.”

---

# **26:00 – 30:00 — Real-World Example: Sticky Sidebar**

### HTML

```html
<div class="main">
  <aside class="sidebar">Sidebar</aside>
  <section class="content">Main content...</section>
</div>
```

### CSS

```css
.sidebar {
  position: sticky;
  top: 20px;
  height: fit-content;
  background: #f7f7f7;
  padding: 20px;
}
```

**You say:**
“The sidebar stays visible as long as its parent has enough height.”

---

# **30:00 – 35:00 — Real-World Example: Section Labels / Index Scrollers**

You see this often in documentation or long forms.

### HTML

```html
<div class="section">
  <h3 class="label">Profile</h3>
  ...
</div>

<div class="section">
  <h3 class="label">Settings</h3>
  ...
</div>
```

### CSS

```css
.label {
  position: sticky;
  top: 10px;
  background: #fff;
}
```

**You say:**
“It creates a floating section label that guides users while scrolling.”

---

# **35:00 – 40:00 — Sticky with Z-index**

**You say:**

“When sticky elements overlap with other content, you may need a **z-index**.”

### Example

```css
.title {
  position: sticky;
  top: 0;
  background: white;
  z-index: 10;
}
```

**You say:**
“z-index ensures sticky elements stay above other overlapping content.”

---

# **40:00 – 44:00 — Common Mistakes Beginners Make**

**You say:**

### ❌ Mistake 1: Forgetting top offset

Without `top: 0`, sticky doesn’t work.

---

### ❌ Mistake 2: Sticky inside a container with `overflow: hidden`

Sticky will not work if any parent has:

```css
overflow: hidden;
overflow: auto;
overflow: scroll;
```

---

### ❌ Mistake 3: Expecting sticky to behave like fixed

Sticky is **relative within the parent**,
fixed is **global to the viewport**.

---

### ❌ Mistake 4: Using sticky on elements with small parent height

Sticky only activates when scrolling is possible.

---

# **44:00 – 47:00 — When to Use Sticky (Real-World Use Cases)**

**You say:**

Use sticky for:

✔ Section headers
✔ Table headers
✔ Floating sub-navigation
✔ Documentation sidebars
✔ Filters in product listings
✔ Form labels for long forms
✔ Category tags in blogs
✔ Page section index markers

**You say:**
“Sticky is one of the most user-friendly behaviors when used correctly.”

---

# **47:00 – 50:00 — Final Recap**

**You say:**

“To summarize:

* Sticky starts as relative
* Becomes fixed when scroll reaches its offset
* Works only with top/left/right/bottom
* Stays inside parent boundaries
* Doesn’t work with overflow parents
* Perfect for headers, labels, table heads, and sidebars
* A modern alternative to fixed in many cases

Sticky is a smart positioning behavior built for better UX.”




Just tell me what you want next.
