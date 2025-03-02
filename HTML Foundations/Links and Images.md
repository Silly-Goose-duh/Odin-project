# Introduction
Links are one of the key features of HTML. They allow us to link to other HTML pages on the web. In fact, this is why it’s called the web.

In this lesson, we will learn how to create links and add some visual flair to our websites by embedding images.

## Lesson Overview
This section contains a general overview of topics that you will learn in this lesson:

- How to create links to pages on other websites on the internet.
- How to create links to other pages on your own websites.
- The difference between absolute and relative links.
- How to display an image on a webpage using HTML.

## Preparation
To get some practice using links and images throughout this lesson, we need an HTML project to work with.

1. Create a new directory named `odin-links-and-images`.
2. Within that directory, create a new file named `index.html`.
3. Open the file in VS Code and fill in the usual HTML boilerplate.
4. Finally, add the following `<h1>` to the body:

```html
<h1>Homepage</h1>
```

---

## Anchor Elements
To create a link in HTML, we use the **anchor (`<a>`) element**. An anchor element is defined by wrapping the text or another HTML element we want to be a link with an `<a>` tag.

Add the following to the body of the `index.html` page we created and open it in the browser:

```html
<a>About The Odin Project</a>
```

You may have noticed that clicking this link doesn’t do anything. This is because an anchor tag on its own won’t know where we want to link to. We have to specify a **destination** using the `href` (hypertext reference) attribute.

### Adding an `href` Attribute
Modify the anchor element to include an `href`:

```html
<a href="https://www.theodinproject.com/about">About The Odin Project</a>
```

By default, any text wrapped with an anchor tag **without an `href`** will look like plain text. If the `href` is present, the browser will style it as a **blue, underlined link**.

### Opening Links in a New Tab
To open a link in a new tab, add the `target="_blank"` attribute:

```html
<a href="https://www.theodinproject.com/about" target="_blank" rel="noopener noreferrer">About The Odin Project</a>
```

- `target="_blank"`: Opens the link in a new tab.
- `rel="noopener noreferrer"`:
  - `noopener`: Prevents the new tab from accessing the original page (security measure).
  - `noreferrer`: Hides the referrer information from the new page.

It is **recommended** to always include `rel="noopener noreferrer"` when using `target="_blank"` for security reasons.

---

## Absolute and Relative Links
Generally, there are two kinds of links:

1. **Absolute links** – Links to pages on other websites on the internet.
2. **Relative links** – Links to pages within our own website.

### Absolute Links
An **absolute link** includes the full URL, such as:

```html
<a href="https://www.theodinproject.com/about">About The Odin Project</a>
```

### Relative Links
A **relative link** links to another page within the same website without specifying the domain.

#### Example: Linking to Another Page
1. Create a file named `about.html` in the same directory (`odin-links-and-images`).
2. Add the following content:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Odin Links and Images</title>
</head>
<body>
    <h1>About Page</h1>
</body>
</html>
```

3. Modify `index.html` to include the relative link:

```html
<body>
    <h1>Homepage</h1>
    <a href="about.html">About</a>
</body>
```

Clicking "About" will now take you to `about.html`.

#### Organizing with Subdirectories
1. Create a `pages/` directory inside `odin-links-and-images`.
2. Move `about.html` into the `pages/` directory.
3. Update the link in `index.html`:

```html
<a href="pages/about.html">About</a>
```

4. To avoid potential issues, prepend `./`:

```html
<a href="./pages/about.html">About</a>
```

### Metaphor: Absolute vs. Relative Links
- **Absolute links**: Full directions including protocol, domain, and path.
- **Relative links**: Directions from the current page to another page within the same website.

---

## Images in HTML
To display an image in HTML, use the `<img>` element. This is a **void element**, meaning it does not require a closing tag.

### Example: Displaying an Image
```html
<img src="https://www.theodinproject.com/logo.png" alt="Odin Project Logo">
```

- `src` (source): Specifies the image URL or file path.
- `alt` (alternative text): Describes the image (useful for accessibility and when the image cannot load).

### Using Relative Paths for Images
If the image is stored in the project directory, use a relative path:

```html
<img src="images/logo.png" alt="Website Logo">
```

If the image is inside a subdirectory (e.g., `assets/images`):

```html
<img src="assets/images/logo.png" alt="Website Logo">
```

---

## Summary
- Use `<a>` tags to create links.
- `href` specifies the destination URL.
- `target="_blank"` opens links in a new tab.
- `rel="noopener noreferrer"` enhances security.
- **Absolute links** include full URLs.
- **Relative links** reference files within the project.
- The `<img>` element embeds images using the `src` attribute.

By mastering links and images, we can make our websites more interactive and visually engaging!

