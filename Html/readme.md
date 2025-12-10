# HTML Interview Questions

------------------------------------------------------------------------

## 1️⃣ What is HTML?

**HTML (HyperText Markup Language)** is the standard language used to
create webpages.\
It defines the structure of a webpage using tags like `<div>`, `<h1>`,
`<p>`, etc.

------------------------------------------------------------------------

## 2️⃣ Difference between `<div>` and `<span>`

  -----------------------------------------------------------------------
  Tag             Type                  Behavior
  --------------- --------------------- ---------------------------------
  `<div>`         Block-level           Starts on a new line, takes full
                                        width

  `<span>`        Inline                Stays in the same line, takes
                                        only required width
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## 3️⃣ What is Semantic HTML?

Semantic HTML uses meaningful tags that describe the purpose of content.

**Examples:**\
`<header>`, `<footer>`, `<article>`, `<nav>`, `<section>`

**Benefits:** - Better SEO\
- Improved accessibility\
- Cleaner code

------------------------------------------------------------------------

## 4️⃣ Difference between `<script>` and `<link>`

  Tag          Purpose
  ------------ --------------------
  `<script>`   Embeds JavaScript
  `<link>`     Links external CSS

------------------------------------------------------------------------

## 5️⃣ What is DOCTYPE?

`<!DOCTYPE html>` tells the browser to use HTML5 standards.

------------------------------------------------------------------------

## 6️⃣ HTML vs HTML5

  Feature         HTML         HTML5
  --------------- ------------ ------------------------------------
  Audio/Video     ❌ No        ✔ Supported
  Storage         ❌ No        ✔ `localStorage`, `sessionStorage`
  Graphics        ❌ Limited   ✔ `<canvas>` & SVG
  Semantic Tags   ❌ No        ✔ Yes

------------------------------------------------------------------------

## 7️⃣ Use of `<meta>` Tag

Provides metadata for search engines & browsers.

**Example:**

``` html
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

------------------------------------------------------------------------

## 8️⃣ What are HTML Attributes?

Additional info added to HTML elements.

**Example:**

``` html
<img src="logo.png" alt="Company Logo" />
```

------------------------------------------------------------------------

## 9️⃣ Block vs Inline Elements

### Block Elements:

-   Start on a new line\
-   Take full width\
-   Examples: `<div>`, `<h1>`, `<p>`

### Inline Elements:

-   Do not start a new line\
-   Take only required width\
-   Examples: `<span>`, `<a>`, `<img>`

------------------------------------------------------------------------

## 🔟 Use of `<canvas>` Tag

Used to draw graphics, charts, animations via JavaScript.

------------------------------------------------------------------------

## 1️⃣1️⃣ localStorage vs sessionStorage

  Feature       localStorage            sessionStorage
  ------------- ----------------------- ------------------
  Persistence   Permanent               Until tab closes
  Capacity      \~10MB                  \~5MB
  Use           Save user preferences   Temporary data

------------------------------------------------------------------------

## 1️⃣2️⃣ Difference Between `<img>` and `<picture>`

### `<img>`

-   Loads a single image.

### `<picture>`

-   Useful for responsive and multiple image formats.

**Example:**

``` html
<picture>
  <source srcset="img.webp" type="image/webp">
  <img src="img.jpg" alt="Image">
</picture>
```

------------------------------------------------------------------------

## 1️⃣3️⃣ What is the `alt` Attribute?

Describes an image if it fails to load.

**Importance:** - Accessibility\
- SEO\
- Screen readers support

------------------------------------------------------------------------

## 1️⃣4️⃣ Explain `<iframe>`

Used to embed another webpage inside your webpage.

``` html
<iframe src="https://google.com"></iframe>
```

------------------------------------------------------------------------

## 1️⃣5️⃣ GET vs POST (Forms)

  Method            GET              POST
  ----------------- ---------------- -------------
  Data Visibility   Visible in URL   Hidden
  Data Size         Small            Large
  Security          Less secure      More secure
  Use Case          Fetch            Submit

------------------------------------------------------------------------

## 1️⃣6️⃣ Purpose of `required` Attribute

Ensures the user must fill the form field.

``` html
<input type="email" required>
```

------------------------------------------------------------------------

## 1️⃣7️⃣ What is ARIA?

**ARIA = Accessible Rich Internet Applications**

Improves accessibility for assistive tools.

Example:

``` html
<button aria-label="Close popup"></button>
```

------------------------------------------------------------------------

## 1️⃣8️⃣ Difference: `<ul>`, `<ol>`, `<dl>`

  Tag      Meaning
  -------- ---------------------------------------
  `<ul>`   Unordered list (bullets)
  `<ol>`   Ordered list (numbers)
  `<dl>`   Definition list (terms + description)

------------------------------------------------------------------------

## 1️⃣9️⃣ Purpose of `data-*` Attributes

Stores custom data in elements.

``` html
<div data-userid="102">Amisha</div>
```

------------------------------------------------------------------------

## 2️⃣0️⃣ What is Responsive Design?

Design that adapts to all screen sizes.

**Techniques:** - Media queries\
- Flexible grids\
- Responsive images

------------------------------------------------------------------------
## 2️⃣1️⃣ Difference Between Inline, Block, and Inline-Block Elements

### **Block Elements**

-   Start on a new line\
-   Take full width\
-   Width/height can be set\
-   Used for layout\
    **Examples:** `<div>`, `<p>`, `<h1>`, `<section>`

**Example Code:**

``` html
<div style="width:200px; height:50px; background:lightblue;">
  I am a block element
</div>
```

------------------------------------------------------------------------

### **Inline Elements**

-   Do not start on a new line\
-   Take only required width\
-   Width/height cannot be set properly\
-   Used for styling small text portions\
    **Examples:** `<span>`, `<a>`, `<strong>`, `<em>`

**Example Code:**

``` html
<span style="background:yellow;">I am inline</span>
```

------------------------------------------------------------------------

### **Inline-Block Elements**

-   Do not start on new line (like inline)\
-   Width/height can be set (like block)\
-   Used for buttons & UI elements\
    **Examples:** `<button>`, `<input>`, `<select>`

**Example Code:**

``` html
<button style="width:100px; height:40px;">Click</button>
```

------------------------------------------------------------------------

## 2️⃣2️⃣ Difference Between `<meta charset="UTF-8">` and `<meta name="viewport">`

### **`<meta charset="UTF-8">`**

-   Defines character encoding\
-   Ensures correct display of emojis, symbols, Indian languages\
-   UTF‑8 supports almost all characters

**Example:**

``` html
<meta charset="UTF-8">
```

------------------------------------------------------------------------

### **`<meta name="viewport">`**

-   Makes webpage responsive on mobile\
-   Scales layout to device width\
-   Prevents zoomed-out look on phones

**Example:**

``` html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

------------------------------------------------------------------------

### 🎉 Memory Trick

-   **charset → characters**\
-   **viewport → mobile scaling**

------------------------------------------------------------------------

## 2️⃣3️⃣ Difference Between `<script>` in `<head>` vs `<body>`

### **Script in `<head>`**

-   JS loads *before* page content\
-   Can delay rendering\
-   Used for must-load-early scripts (e.g., analytics)

### **Script at end of `<body>`**

-   HTML loads first, then JS\
-   Faster page load\
-   Recommended for most websites

### ✅ Why scripts are placed at the bottom?

-   Faster performance\
-   DOM is fully loaded\
-   Prevents render-blocking

------------------------------------------------------------------------

## 2️⃣4️⃣ Difference Between HTML Tags and Attributes

### **HTML Tags**

Define structure/elements of webpage.\
Tell browser what the content *is*.

**Examples:**

``` html
<p>Paragraph</p>
<div>Container</div>
<img>
```

------------------------------------------------------------------------

### **HTML Attributes**

Give *extra information* about tags.\
Always in the opening tag.

**Examples:**

``` html
<img src="logo.png" alt="Company Logo">
<a href="https://google.com">Click</a>
<input type="text" placeholder="Enter name">
```

------------------------------------------------------------------------

### 🎉 One-line Summary

-   **Tags = what the element is**\
-   **Attributes = extra details about the element**

------------------------------------------------------------------------

## 2️⃣5️⃣ What is the `<link>` Tag?

The `<link>` tag connects **external resources** to an HTML page.

### **Where is it used?**

Inside the `<head>` section.

### **Common Uses**

-   Linking CSS\
-   Google fonts\
-   Favicons

### **Example:**

``` html
<link rel="stylesheet" href="styles.css">
<link rel="icon" href="logo.png">
```

### 🎯 One-line Summary

**`<link>` connects external files (mostly CSS) to your page.**

------------------------------------------------------------------------

