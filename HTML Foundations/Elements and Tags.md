**Introduction**

HTML (HyperText Markup Language) defines the structure and content of webpages. We use HTML elements to create all of the paragraphs, headings, lists, images, and links that make up a typical webpage. In this lesson, we will explore how HTML elements work.

**Lesson Overview**
This section contains a general overview of topics that you will learn in this lesson.

- Explain what HTML tags are.
- Explain what HTML elements are.

**Elements and Tags**
Almost all elements on an HTML page are just pieces of content wrapped in opening and closing HTML tags.

- **Opening tags** tell the browser that this is the start of an HTML element. They are comprised of a keyword enclosed in angle brackets <>. For example, an opening paragraph tag looks like this: `<p>`.
- **Closing tags** tell the browser where an element ends. They are almost the same as opening tags; the only difference is that they have a forward slash before the keyword. For example, a closing paragraph tag looks like this: `</p>`.

A full paragraph element looks like this:

```html
<p>some text content</p>
```

Let’s break this down:

- `<p>` is the opening tag.
- `some text content` represents content wrapped within the opening and closing tags.
- `</p>` is the closing tag.

You can think of elements as containers for content. The opening and closing tags tell the browser what content the element contains. The browser can then use that information to determine how it should interpret and format the content.

HTML has a vast list of predefined tags that you can use to create all kinds of different elements. It is important to use the correct tags for content. Using the correct tags can have a big impact on two aspects of your sites: how they are ranked in search engines; and how accessible they are to users who rely on assistive technologies, like screen readers, to use the internet.

Using the correct elements for content is called **semantic HTML**. We will explore this in much more depth later on in the curriculum.

**Void Elements**
Some HTML elements do not have a closing tag. These elements just have a single tag, like: `<br>` or `<img>`. They are known as **void elements** because they are void of any content, there is nothing inside of them. No closing tag means they can’t wrap content like other tags do.

You might also see these referred to as **self-closing tags**. But those are just void elements with a forward slash(`/`) at the end like: `<br />` or `<img />`. You’re likely to see self-closing tags used often for historical reasons. Browsers will be able to render them just fine, but the latest version of the HTML specification discourages their use and considers them invalid.

**Assignment**
- Watch *Kevin Powell’s HTML & CSS for Absolute Beginners: What is HTML?*

**Knowledge Check**
The following questions are an opportunity to reflect on key topics in this lesson. If you can’t answer a question, click on it to review the material, but keep in mind you are not expected to memorize or master this knowledge.

- What is an HTML tag?
- What are the three parts of an HTML element?

**Additional Resources**
This section contains helpful links to related content. It isn’t required, so consider it supplemental.

- *Don’t Fear the Internet’s video about HTML*

