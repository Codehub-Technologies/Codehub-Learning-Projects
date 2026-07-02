

---
# HTML Text Formatting

## Task 1: The "Online News Article" Structure (Hierarchy & Layout)

**Objective:** Learn how to use structural headings (`<h1>`, `<h2>`, `<h3>`) in the correct logical order alongside paragraphs and inline formatting.

### Instructions:

Imagine you are building a layout for a technology news website. You need to take the raw, unformatted text below and turn it into a beautiful, accessible web page using the correct HTML structural elements.

1. Wrap the main article title in an `<h1>` tag.
2. Separate the two main sections using `<h2>` tags for their headings.
3. Separate the sub-points under the second section using `<h3>` tags.
4. Wrap all body text in proper `<p>` elements.
5. Apply **bolding** (`<strong>`) to the words "Artificial Intelligence" and "Quantum Computing" when they first appear.

### Raw Text to Format:

```text
The Future of Technology

Next-Gen Innovation
We are living in an era of unprecedented digital acceleration. Innovations that seemed like science fiction a decade ago are now becoming part of our daily workflows.

Key Drivers of Change
Artificial Intelligence
Machine learning models are changing how we write code, analyze business data, and communicate.

Quantum Computing
Though still in its early stages, quantum mechanics will soon process complex calculations in seconds that modern supercomputers would take years to solve.

```

---

## Task 2: The "E-Commerce Discount & Product Page" (Formatting Mechanics)

**Objective:** Correctly apply inline presentation modifiers like strikethroughs, superscripts, subscripts, and underlines within paragraphs.

### Instructions:

You are coding a product detail page for an online tech store. Write the HTML from scratch to display a product description paragraph that meets these exact design requirements:

1. The main section header should be an `<h2>` tag containing the text: **Product Details**.
2. Create a paragraph showing a price discount: The old price was ~~`N1,200`~~ (apply a **strikethrough** effect), and the new price is **`N899`** (apply a **bold** effect).
3. Create a second paragraph describing the hardware specifications:
* The device has a footprint of only N15\text{ cm}^2$ (use the **superscript** tag for the number 2).
* It requires a specialized liquid cooling fluid containing pure $\text{H}_2\text{O}$ mixed with custom chemicals (use the **subscript** tag for the number 2).

4. Create a final note at the bottom where the words "Limited Stock Available" are explicitly **underlined**.

---

---
# HTML Links Exercises


## Task 3: The Website Navigation Bar & External Resources Challenge

**Objective:** Practice the difference between internal relative paths, external absolute URLs, and utilizing tab targets.

### Instructions:

You are building the header navigation bar and the footer resources section for a multi-page company website. Write the HTML structure based on these explicit requirements:

1. Create a navigation section (`<nav>`) containing three **internal relative links**:
* One linking to the homepage (`index.html`) with the clickable text "Home".
* One linking to the about page (`about.html`) with the clickable text "About Us".
* One linking to the contact page (`contact.html`) with the clickable text "Contact".


2. Create a paragraph below the navigation bar that links to an **external resource**:
* Link to `[https://www.wikipedia.org](https://www.wikipedia.org)` with the text "Search Wikipedia".
* Ensure that when a user clicks this specific link, it **opens automatically in a brand new browser tab**.



---

## Task 4: The Long-Form Article "Table of Contents" (Anchor Links)

**Objective:** Learn how to create smooth internal page navigation using HTML `id` attributes and bookmark hash symbols (`#`).

### Instructions:

When webpages have a massive amount of text, developers create a "Table of Contents" at the top so users can skip directly to sections. Build an internal navigation system using the code guidelines below:

1. Create an unordered list at the top of your page acting as a Table of Contents. Inside it, create two links:
* The first link should have an `href` pointing to an internal target called `#features`.
* The second link should have an `href` pointing to an internal target called `#pricing`.


2. Below your table of contents, create a heading element for your first section:
* Give this heading an `id` matching your first link exactly (`features`).


3. Add a few paragraphs of dummy text under it, then create your second section heading:
* Give this heading an `id` matching your second link exactly (`pricing`).

4. At the very bottom of the page, add a final link with the text "Back to Top" that targets an `id` placed on your main page title at the very top.


---
# HTML Images

## Task 5: The "Broken Profile Card" (Debugging & Accessibility)

**Objective:** Understand how to properly implement image source paths, dimension attributes, and accessible `alt` text descriptions.

### Instructions:

You have been handed a snippet of code for a user profile component, but it has several issues. Copy the code into your editor and complete the following fixes:

1. The profile picture is broken because the path attribute name is completely missing. Fix it so it loads the correct online image: `[https://picsum.photos/id/237/200/300](https://picsum.photos/id/237/200/300)`.
2. Screen readers for visually impaired users cannot read this card because the image is missing its fallback description text. Add an appropriate attribute describing the image content.
3. The image file is rendering way too large on the screen and breaking the card container structure. Use the correct HTML attributes to force the image to display at exactly **150 pixels wide** and **150 pixels high**.

### Starter Code:

```html
<!-- Fix the image tag inside this profile card -->
<div class="profile-card">
  <h2>User Profile: Rover</h2>
  
  <img "https://picsum.photos/id/237/200/300" >
  
  <p>Status: Active Account</p>
</div>

```

---

## Task 6: The "E-Commerce Thumbnail Gallery" (Layout & Setup)

**Objective:** Practice writing self-closing `<img>` tags from scratch with strict inline scaling rules.

### Instructions:

You are coding a clean product display grid for a retail smartphone mockup. Write the clean HTML code from scratch using the following specifications:

1. Create a primary structural container using a `<div>` element.
2. Inside that container, insert **two separate images side-by-side** representing a "Front View" and a "Side View" of a smartphone. You may use `[https://picsum.photos/200](https://picsum.photos/200)` as a placeholder URL for both images.
3. For the first image, give it a clear alternative description text, and force its size to **200 pixels wide** by **200 pixels high**.
4. For the second image, give it a unique alternative description text, and force its size to **100 pixels wide** by **100 pixels high** so it looks like a smaller thumbnail.
5. Remember: The `<img>` tag is a self-closing element! Ensure you do not add a closing `</img>` tag.