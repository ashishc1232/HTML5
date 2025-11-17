
**Topic:** HTML5 Hands-On Practice
**Audience:** Beginner/Intermediate
**Goal:** Teach students how to approach HTML questions **effectively** using modern semantic structure, accessibility, and real-world examples.

---

# **00:00 – 02:00 — Introduction**

**You say:**

“Welcome everyone.
In this session, we’re going to practice HTML the right way — not old school tags, not outdated patterns — but clean, modern HTML5 that companies expect today.

We will solve practical questions that reflect real interview tasks: semantic structure, forms, accessibility, and proper layout foundations.

Even though this is a recording, follow along on your end. Pause whenever needed and try the questions before I show the solution idea.”

---

# **02:00 – 05:00 — Core Rules Before Starting**

**You say:**

“Before solving anything, remember these four rules for writing modern HTML:

1. **Always start with semantic tags** — `<header>`, `<main>`, `<section>`, `<article>`, `<footer>`.
2. **Avoid div-only layout** — use meaningful tags.
3. **Make content accessible** — proper labels, alt text, headings order.
4. **Keep structure separate from styling** — no inline styling.

We’ll keep these rules applied in all practice tasks.”

---

# **05:00 – 15:00 — Practice Question 1: Create a Modern Blog Layout**

**You say:**

“Question 1:
Create a clean blog page with the following requirements:

* A header with a site title
* A navigation bar with 3 links
* A main section containing two blog posts
* Each blog post must have a title, date, and short paragraph
* Add a footer with copyright text
* Use only semantic HTML5 tags
* Avoid any CSS — focus purely on structure

Pause now and try. Then continue to see the best approach.”

**Show Solution Approach (not full code yet):**

“When you approach this, think:
Header → Nav → Main → Articles → Footer.
Never start using only `<div>` tags — interviews expect semantic flow.”

**Then show full example code (modern):**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Practice Blog</title>
</head>
<body>
  <header>
    <h1>My Blog</h1>
    <nav>
      <a href="#">Home</a>
      <a href="#">Posts</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <main>
    <article>
      <h2>First Post</h2>
      <time datetime="2025-01-10">January 10, 2025</time>
      <p>This is a short introduction to modern HTML practice.</p>
    </article>

    <article>
      <h2>Second Post</h2>
      <time datetime="2025-01-15">January 15, 2025</time>
      <p>HTML5 semantic tags improve accessibility and SEO.</p>
    </article>
  </main>

  <footer>
    <p>© 2025 MyBlog</p>
  </footer>
</body>
</html>
```

**You say:**
“This is the simplest and most professional structure for a blog in HTML5.”

---

# **15:00 – 25:00 — Practice Question 2: Build a Modern Registration Form**

**You say:**

“Question 2:
Create a clean registration form with the following fields:

* Full Name
* Email
* Password
* A checkbox for agreeing to terms
* A submit button

Rules:

* Use `<label>` for every input
* Use the correct input types
* Structure should be inside `<form>` with a meaningful sectioning tag
* Include required validation attributes
* Keep accessibility in mind

Pause the video and attempt it.”

**Solution Explanation:**

“Most students fail because they forget label-for pairing, placeholder vs label differences, and required attributes. This version is clean and modern.”

**Full solution:**

```html
<section>
  <h2>Create Your Account</h2>

  <form>
    <label for="name">Full Name</label>
    <input id="name" name="name" type="text" required>

    <label for="email">Email Address</label>
    <input id="email" name="email" type="email" required>

    <label for="password">Password</label>
    <input id="password" name="password" type="password" minlength="6" required>

    <label>
      <input type="checkbox" required>
      I agree to the terms and conditions
    </label>

    <button type="submit">Register</button>
  </form>
</section>
```

**You say:**
“This follows proper accessibility and modern form practices.”

---

# **25:00 – 32:00 — Practice Question 3: Create an Image Gallery (No CSS)**

**You say:**

“Question 3:
Create a simple image gallery using modern HTML rules:

* Use a `<section>` for the gallery
* Add 4 images
* Each image must have descriptive alt text
* Wrap each image and caption using `<figure>` and `<figcaption>`
* No CSS allowed — pure HTML structure

Pause and try.”

**Solution:**

```html
<section>
  <h2>Gallery</h2>

  <figure>
    <img src="img1.jpg" alt="Mountain landscape">
    <figcaption>Mountain View</figcaption>
  </figure>

  <figure>
    <img src="img2.jpg" alt="Forest trail">
    <figcaption>Forest Trail</figcaption>
  </figure>

  <figure>
    <img src="img3.jpg" alt="City skyline">
    <figcaption>City Skyline</figcaption>
  </figure>

  <figure>
    <img src="img4.jpg" alt="Beach sunset">
    <figcaption>Beach Sunset</figcaption>
  </figure>
</section>
```

**You say:**
“This is the modern HTML5 way to present images with meaning.”

---

# **32:00 – 40:00 — Practice Question 4: Create a Product Card (Real Interview Style)**

**You say:**

“Question 4:
Create a product card layout using HTML only:

* Product image
* Product name
* Price
* Short description
* ‘Add to Cart’ button
* Use semantic tags where possible

Pause here and attempt.”

**Solution:**

```html
<article>
  <img src="phone.jpg" alt="Smartphone model X">
  <h3>Smartphone X</h3>
  <p class="price">$699</p>
  <p>A modern smartphone with advanced camera and battery.</p>
  <button>Add to Cart</button>
</article>
```

**You say:**
“Keep the structure minimal and accessible. This is how product cards are built in real front-end components.”

---

# **40:00 – 45:00 — Final Practical Question + Thoughts**

**You say:**

“Final Question:
Create a simple landing page structure with:

* Header
* Hero section with one headline and one paragraph
* Features section with 3 short feature points
* Footer

This tests your overall structure skills.
Pause here, build it, and compare your attempt with the previous patterns.”

**You end with:**

“Modern HTML is not about memorizing tags. It’s about building meaningful structure.
Review these questions again, repeat them, and practice rewriting them in your own style.”



