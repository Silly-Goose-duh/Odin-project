# Introduction

Most content on the web is text-based, so you will find yourself needing to work with HTML text elements quite a bit.

In this lesson, we will learn about the text-based elements you are likely to use the most.

## Lesson Overview

This section contains a general overview of topics that you will learn in this lesson.

- How to create paragraphs.
- How to create headings.
- How to create bold text.
- How to create italicized text.
- The relationships between nested elements.
- How to create HTML comments.

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

It looks like two paragraphs of text, so you might expect it to display in that way. However, that is not the case, as you can see in the output below:

When the browser encounters new lines like this in your HTML, it will compress them down into one single space. The result of this compression is that all of the text is clumped together into one long line.

If we want to create paragraphs in HTML, we need to use the paragraph element, which will add a new line after each of our paragraphs. A paragraph element is defined by wrapping text content with a `<p>` tag.

## Headings

Headings are different from other HTML text elements: they are displayed larger and bolder than other text to signify that they are headings.

There are 6 different levels of headings starting from `<h1>` to `<h6>`. The number within a heading tag represents that heading’s level. The largest and most important heading is `<h1>`, while `<h6>` is the tiniest heading at the lowest level.

Using the correct level of heading is important as levels provide a hierarchy to the content. An `<h1>` heading should always be used for the heading of the overall page, and the lower-level headings should be used as the headings for content in smaller sections of the page.

## Strong Element

The `<strong>` element makes text bold. It also semantically marks text as important, which affects tools like screen readers.

```html
<strong>Important text</strong>
```

Sometimes you will want to make text bold without giving it an important meaning. You’ll learn how to do that in the CSS lessons later in the curriculum.

## Em Element

The `<em>` element makes text italic. It also semantically places emphasis on the text.

```html
<em>Emphasized text</em>
```

Like the `<strong>` element, the `<em>` element is often used with other text elements.

## Nesting and Indentation

When we nest elements within other elements, we create a parent and child relationship between them. The nested elements are the children, and the element they are nested within is the parent.

For example:

```html
<body>
  <p>This is a paragraph.</p>
</body>
```

The `<body>` element is the parent, and the `<p>` is the child.

We use indentation to make the level of nesting clear and readable for ourselves and other developers.

## HTML Comments

HTML comments are not visible to the browser; they allow us to comment on our code.

```html
<!-- This is a comment -->
```

### VSCode Keyboard Shortcut

- **Mac Users:** Cmd + /
- **Windows and Linux Users:** Ctrl + /

# Lists in HTML

Whether it be IMDB’s top 250 movies or the FBI’s most wanted, lists are everywhere on the web.

## Lesson Overview

This section contains a general overview of topics that you will learn in this lesson.

- How to create an unordered list.
- How to create an ordered list.

## Unordered Lists

If you want to have a list of items where the order doesn’t matter, like a shopping list, then you can use an unordered list.

Unordered lists are created using the `<ul>` element, and each item within the list is created using the `<li>` element.

```html
<ul>
  <li>Milk</li>
  <li>Bread</li>
  <li>Eggs</li>
</ul>
```

Each list item in an unordered list begins with a bullet point.

## Ordered Lists

If the order does matter, like step-by-step instructions, then you can use an ordered list.

Ordered lists are created using the `<ol>` element.

```html
<ol>
  <li>Wake up</li>
  <li>Brush teeth</li>
  <li>Have breakfast</li>
</ol>
```

Each list item in an ordered list begins with a number.

# Assignment

To get some practice working with text and lists in HTML:

1. Create a plain blog article page using different headings, paragraphs, and formatted text (bold and italicized).
2. Create the following lists in a new HTML document:
   - An unordered shopping list of your favorite foods.
   - An ordered list of todo’s you need to get done today.
   - An unordered list of places you’d like to visit someday.
   - An ordered list of your all-time top 5 favorite video games or movies.

# Knowledge Check

The following questions are an opportunity to reflect on key topics in this lesson.

- How do you create a paragraph in HTML?
- How do you create a heading in HTML?
- How many different levels of headings are there, and what is the difference between them?
- What element should you use to make text bold and important?
- What element should you use to make text italicized to add emphasis to it?
- What relationship does an element have with any nested elements within it?
- What relationship do two elements have if they are at the same level of nesting?
- How do you create HTML comments?
- What HTML element is used to create an unordered list?
- What HTML element is used to create an ordered list?
- What HTML element is used to create list items within both unordered and ordered lists?

# Additional Resources

This section contains helpful links to related content. It isn’t required, so consider it supplemental.

- [The semantic difference between `<strong>` and `<b>` or `<em>` and `<i>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)
- [MDN documentation on the unordered list element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul)
- [MDN documentation on the ordered list element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol)
- [Shay Howe’s HTML lists tutorial](https://learn.shayhowe.com/html-css/working-with-lists/)

