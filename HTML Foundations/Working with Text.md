# Introduction
Most content on the web is text-based, so you will find yourself needing to work with HTML text elements quite a bit.

In this lesson, we will learn about the text-based elements you are likely to use the most.

## Lesson Overview
This section contains a general overview of topics that you will learn in this lesson:

- How to create paragraphs.
- How to create headings.
- How to create bold text.
- How to create italicized text.
- The relationships between nested elements.
- How to create HTML comments.

---

## Paragraphs
What would you expect the following text to output on an HTML page?

```html
<body>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
  incididunt ut labore et dolore magna aliqua.

  Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
  nisi ut aliquip ex ea commodo consequat.
</body>
```

It looks like two paragraphs of text, so you might expect it to display in that way. However, that is not the case. When the browser encounters new lines in your HTML, it will compress them into a single space, resulting in one continuous line of text.

To create paragraphs in HTML, use the `<p>` tag:

```html
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit...</p>
<p>Ut enim ad minim veniam, quis nostrud exercitation ullamco...</p>
```

---

## Headings
Headings are different from other text elements as they are displayed larger and bolder to signify importance.

There are **6 different levels of headings** in HTML, ranging from `<h1>` to `<h6>`, with `<h1>` being the most important and `<h6>` being the smallest.

Example:

```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
<h3>Smaller Heading</h3>
```

### Importance of heading levels:
- `<h1>` is used for the main page title.
- Lower-level headings (`<h2>` - `<h6>`) structure content hierarchically.

---

## **Strong Element**
The `<strong>` element makes text **bold** and semantically marks it as important. Screen readers may emphasize its importance with a change in tone.

```html
<strong>This is important text.</strong>
```

You can also combine it with other text elements:

```html
<p>This is a <strong>very important</strong> message.</p>
```

If you want bold text without added importance, use CSS (covered in later lessons).

---

## **Emphasis Element**
The `<em>` element makes text *italicized* and adds **semantic emphasis**. Screen readers may change their tone for emphasized text.

```html
<em>This text is emphasized.</em>
```

Like `<strong>`, `<em>` is commonly used within paragraphs:

```html
<p>Make sure to <em>read the instructions carefully</em> before proceeding.</p>
```

---

## **Nesting and Indentation**
In HTML, elements can be **nested** inside one another. This creates **parent-child relationships**:

```html
<body>
  <p>This is a paragraph inside the body.</p>
</body>
```

- The `<body>` element is the **parent**.
- The `<p>` element is the **child**.

### **Sibling elements**
Elements at the same nesting level are **siblings**:

```html
<body>
  <p>First paragraph</p>
  <p>Second paragraph</p>
</body>
```
Here, both `<p>` elements are **siblings** since they share the same parent (`<body>`).

Indentation improves readability, typically using **two spaces per nesting level**.

---

## **HTML Comments**
Comments in HTML help explain code but do **not appear** in the browser.

To write a comment, use `<!-- -->`:

```html
<!-- This is a comment -->
<p>This is visible text.</p>
```

### **VS Code Keyboard Shortcut for Comments**
- **Mac:** `Cmd + /`
- **Windows/Linux:** `Ctrl + /`

---

## **Assignment**
1. Watch [Kevin Powell’s HTML Paragraph and Headings Video](#).
2. Watch [Kevin Powell’s HTML Bold and Italic Text Video](#).
3. **Practice:**  
   - Create a simple blog article page using:
     - Different headings (`<h1>` - `<h6>`)
     - Paragraphs (`<p>`)
     - Bold (`<strong>`) and italic (`<em>`) text  
   - Use **Lorem Ipsum** as placeholder text.  
   - In VS Code, type `lorem` and press `Enter` to generate dummy text.

---

## **Knowledge Check**
Reflect on these key topics:

- How do you create a paragraph in HTML?
- How do you create a heading in HTML?
- How many heading levels exist, and how do they differ?
- Which element makes text bold and important?
- Which element makes text italicized with emphasis?
- What is the relationship between a parent element and its nested elements?
- What is the relationship between elements at the same nesting level?
- How do you create an HTML comment?

---

## **Additional Resources**
- [The semantic difference between `<strong>` and `<b>`, and `<em>` and `<i>`](#).
- [Interactive HTML text formatting article](#).

