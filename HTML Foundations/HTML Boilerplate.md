**Introduction**
All HTML documents have a basic structure or boilerplate that serves as the foundation before adding any content. This lesson explores the different components of this boilerplate and their roles.

---

**Lesson Overview**
In this lesson, you will learn:
- How to write the basic boilerplate for an HTML document.
- How to open HTML documents in a browser.

---

**Creating an HTML File**
1. Create a new folder on your computer named `html-boilerplate`.
2. Inside this folder, create a new file named `index.html`.
3. The `.html` extension is necessary for the file to be recognized as an HTML document.
4. Naming the homepage file `index.html` is crucial, as web servers look for this file by default.

---

**The DOCTYPE Declaration**
- The first line in an HTML document is the doctype declaration: `<!DOCTYPE html>`.
- This informs the browser to use HTML5.
- Older versions of HTML had more complex doctype declarations, but HTML5 simplifies this.

**HTML Element**
- The `<html>` element is the root of an HTML document.
- Every other element is nested inside it.
- Example:
  ```html
  <!DOCTYPE html>
  <html lang="en">
  </html>
  ```
- The `lang` attribute specifies the document’s language for accessibility purposes.

---

**Head Element**
- The `<head>` element contains metadata and configurations for the webpage.
- It does not display content on the webpage.
- Example:
  ```html
  <head>
    <meta charset="UTF-8">
    <title>My First Webpage</title>
  </head>
  ```
- The `<meta charset="UTF-8">` tag ensures correct character encoding.
- The `<title>` tag defines the title shown on the browser tab.

---

**Body Element**
- The `<body>` element contains the visible content of the webpage.
- Example:
  ```html
  <body>
    <h1>Hello World!</h1>
  </body>
  ```

---

**Viewing HTML Files in a Browser**
- Methods to open `index.html`:
  1. Drag and drop the file into a browser.
  2. Double-click the file to open it in the default browser.
  3. Use the terminal:
     - Ubuntu: `google-chrome index.html`
     - macOS: `open ./index.html`
     - WSL: `explorer.exe index.html`
- The page appears blank unless content is added inside `<body>`.

---

**VSCode Shortcut**
- In VSCode, type `!` and press `Enter` to generate the full HTML boilerplate automatically.
- The auto-generated template includes:
  ```html
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  ```
  - This is used for responsive design but can be ignored for now.
- Writing boilerplate manually helps reinforce learning.

---

**Assignment**
1. Watch Kevin Powell’s *Building Your First Web Page* video.
2. Practice writing the boilerplate from memory.
3. Validate your HTML using the W3 HTML validator to check for errors.

---

**Knowledge Check**
- What is the purpose of the doctype declaration?
- What is the `<html>` element?
- What is the purpose of the `<head>` element?
- What is the purpose of the `<body>` element?

---

**Additional Resources**
- Use VSCode’s *Live Preview* extension for real-time updates.
- The `lang` attribute can be applied to specific elements if needed.

