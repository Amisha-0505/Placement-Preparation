# CSS Interview Questions & Answers

## 1. What is CSS?

**Answer:**
CSS (Cascading Style Sheets) is a stylesheet language used to control the presentation of HTML elements.
It defines how web pages look — layout, colors, fonts, spacing, animations, etc.

---

## 2. What are the advantages of using CSS?

**Answer:**

* Separation of content and design → HTML handles structure, CSS handles styling
* Reusability → One CSS file can be used for multiple pages
* Faster page loading → Less inline code, better maintainability
* Better consistency → Uniform styling across the website
* Responsive design → Media queries help adapt UI to all screen sizes
* Cleaner code → Reduces duplication

---

## 3. How do you specify units in CSS? What are different types?

**Answer:**
You specify units for dimensions like width, height, margin, font-size, etc.

### Absolute Units

* `px` (pixels)
* `cm` (centimeters)
* `mm`
* `in` (inches)

### Relative Units

* `em` → relative to parent font-size
* `rem` → relative to root font-size
* `%` → relative to parent
* `vw` → viewport width
* `vh` → viewport height

---

## 4. What is the Box Model in CSS? Which properties belong to it?

**Answer:**
The CSS Box Model describes how every element on a webpage is structured like a box.

**Structure:**
Content → Padding → Border → Margin

**Properties:**

* `width`, `height`
* `padding`
* `border`
* `margin`
* `box-sizing`

---

## 5. What are the limitations of CSS?

**Answer:**

* No advanced programming capabilities (loops, conditions)
* Limited logic handling
* Browser compatibility issues
* Global scope causes naming conflicts
* Hard to manage large projects without structure

---

## 6. How to include CSS in a webpage?

**Answer:**

### Inline CSS

```html
<p style="color: blue;">Hello</p>
```

### Internal CSS

```html
<style>
  p { color: blue; }
</style>
```

### External CSS (Recommended)

```html
<link rel="stylesheet" href="styles.css">
```

---

## 7. What are the different types of selectors in CSS?

**Answer:**

* Universal → `*`
* Element → `p`, `div`
* Class → `.container`
* ID → `#header`
* Attribute → `input[type="text"]`
* Descendant → `div p`
* Child → `div > p`
* Adjacent sibling → `h1 + p`
* General sibling → `h1 ~ p`
* Pseudo-class → `:hover`, `:focus`
* Pseudo-element → `::before`, `::after`

---

## 8. What is a CSS Preprocessor? Why are Sass, Less, and Stylus used?

**Answer:**
A CSS preprocessor extends CSS with programming-like features and compiles into standard CSS.

**Examples:**

* Sass (SCSS)
* Less
* Stylus

**Benefits:**

* Variables
* Nesting
* Mixins & functions
* Code reusability
* Better maintainability

---

## 9. What is VH and VW in CSS?

**Answer:**

* `1vh` = 1% of viewport height
* `1vw` = 1% of viewport width

```css
height: 100vh;
width: 50vw;
```

---

## 10. Difference between Reset CSS and Normalize CSS?

**Answer:**

| Reset CSS                  | Normalize CSS             |
| -------------------------- | ------------------------- |
| Removes all default styles | Makes styles consistent   |
| Aggressive                 | Safer & modern            |
| No defaults preserved      | Preserves useful defaults |

---

## 11. Difference between inline, inline-block, and block?

| Property       | Inline  | Inline-block | Block |
| -------------- | ------- | ------------ | ----- |
| New line       | ❌       | ❌            | ✅     |
| Width/Height   | ❌       | ✅            | ✅     |
| Margin/Padding | Limited | Full         | Full  |

---

## 12. Is it important to test webpages in different browsers?

**Answer:**
Yes. It ensures cross-browser compatibility, consistent UI, and better user experience.

---

## 13. What are Pseudo-classes and Pseudo-elements?

**Answer:**

* **Pseudo-class:** Styles an element in a specific state (`:hover`, `:focus`)
* **Pseudo-element:** Styles a specific part (`::before`, `::after`)

---

## 14. What is cascading in CSS?

**Answer:**
Cascading decides which CSS rule applies based on:

1. `!important`
2. Specificity
3. Source order

---

## 15. What property is used to change the font face?

**Answer:**

```css
font-family: "Roboto", sans-serif;
```

---

## 16. Difference between Adaptive Design and Responsive Design?

| Adaptive         | Responsive    |
| ---------------- | ------------- |
| Fixed layouts    | Fluid layouts |
| Predefined sizes | Media queries |
| Less flexible    | More flexible |

---

## 17. How are CSS selectors matched by the browser?

**Answer:**
Browsers match selectors from right to left for better performance.

```css
div p span { }
```

---

## 18. Difference between border-box and content-box?

| content-box            | border-box                |
| ---------------------- | ------------------------- |
| Default                | Includes padding & border |
| Width excludes padding | Width includes padding    |

```css
box-sizing: border-box;
```

---

## 19. How is opacity specified in CSS3?

**Answer:**

```css
opacity: 0.5;
```

Range: `0` to `1`

---

## 20. Why use the float property in CSS?

**Answer:**

* Position elements left or right
* Wrap text around images

```css
img { float: left; }
```

---

## 21. What is z-index and how does it function?

**Answer:**
Controls stacking order of positioned elements.

* Works only on positioned elements
* Higher value appears on top
* Depends on stacking context

```css
.box1 { position: absolute; z-index: 10; }
.box2 { position: absolute; z-index: 5; }
```

---

## 22. What do common CSS selectors mean?

* `*` → Universal selector
* `div p` → Descendant
* `div > p` → Child
* `h1 + p` → Adjacent sibling
* `h1 ~ p` → General sibling
* `.className` → Class
* `#idName` → ID
* `input[type="text"]` → Attribute

---

## 23. What are the properties of Flexbox?

### Flex Container Properties

* `display: flex`
* `flex-direction`
* `flex-wrap`
* `justify-content`
* `align-items`
* `align-content`
* `gap`

### Flex Item Properties

* `flex-grow`
* `flex-shrink`
* `flex-basis`
* `flex`
* `align-self`
* `order`

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}

.item {
  flex: 1;
}
```
