### HTML Interview Questions and Answers — Complete Technical Notes

Questions 1–79 · Simplified technical answers · Based on your reference article

### Questions 1–20

### 1. What are HTML tags?

HTML tags are keywords enclosed in angle brackets that define elements on a webpage. For example, `<h1>` defines a heading and `<p>` defines a paragraph.

### 2. What is the difference between HTML and HTML5?

HTML5 introduced modern web features, including semantic elements, multimedia, graphics, and new form input types. Examples include `<video>`, `<canvas>`, `<header>`, and `<input type="email">`.

### 3. What is the basic structure of an HTML document?

An HTML document contains a doctype declaration, root element, head, and body. The head stores metadata and resource links, while the body contains the webpage content.

### 4. What is the difference between a tag and an element?

A tag is the markup inside angle brackets, such as `<p>`. An element is the complete structure, including its tags and content, such as `<p>Hello</p>`.

### 5. What are attributes in HTML?

Attributes provide additional information about an element. They are usually written in the opening tag as name-value pairs.

Example: `<img src="photo.jpg" alt="Photo">`

Here, `src` specifies the image location and `alt` provides alternative text.

### 6. What is the difference between `<section>`, `<article>`, and `<div>`?

* `<section>` groups related content under a common topic.

* `<article>` represents independent content, such as a blog post.

* `<div>` is a generic container without specific semantic meaning.

### 7. How do you create hyperlinks? What are absolute and relative URLs?

Use the `<a>` tag with the `href` attribute to create a hyperlink.

* Absolute URL: Contains the complete address, such as `https://example.com/about.html`.

* Relative URL: Specifies a path relative to the current website or document, such as `about.html`.

### 8. What is the purpose of the `<img>` tag?

The `<img>` tag embeds an image into a webpage. Its `src` attribute specifies the image path, while `alt` provides alternative text for accessibility and when an image cannot load.

### 9. What is the difference between block-level and inline elements?

Block-level elements generally start on a new line and occupy the available width. Inline elements remain within the current line and take up the space their content needs.

Examples: `<div>` and `<p>` are block-level by default; `<span>` and `<a>` are inline by default.

### 10. What types of lists are available in HTML?

HTML supports three main list types:

* `<ol>` — ordered list, usually numbered.

* `<ul>` — unordered list, usually bulleted.

* `<dl>` — description list containing terms and descriptions, using `<dt>` and `<dd>`.

### 11. What is the `<form>` tag, and what do `action` and `method` do?

The `<form>` element collects user input and submits it for processing.

* `action` specifies where the form data is sent.

* `method` specifies how the request is sent.

`GET` usually places submitted data in the URL. `POST` sends data in the request body. POST does not automatically encrypt data; HTTPS is needed for secure transmission.

### 12. What does the `<br>` tag do, and when should you avoid it?

The `<br>` tag inserts a line break without creating a new paragraph. It is suitable for addresses or poetry, but CSS should be used for layout spacing.

### 13. How do you make a link open in a new tab safely?

Use `target="_blank"` to open the link in a new tab. The `rel="noopener"` attribute prevents the new page from accessing the original page through `window.opener`.

```html
<a href="https://example.com"
   target="_blank"
   rel="noopener">Open Website</a>
```

### 14. What does the `<title>` tag do, and why is it important for SEO?

The `<title>` tag defines the webpage title shown in the browser tab. A clear, relevant title also helps search engines and users understand the page topic.

### 15. What is the `<meta>` tag?

The `<meta>` tag defines metadata about an HTML document. It is placed inside `<head>` and can specify character encoding, viewport settings, and page descriptions.

Example:

```html
<meta charset="UTF-8">
<meta name="viewport"
      content="width=device-width, initial-scale=1.0">
```

### 16. How do you create a table in HTML?

Use `<table>` to create the table, `<tr>` for rows, `<th>` for header cells, and `<td>` for data cells. `<thead>`, `<tbody>`, and `<caption>` can improve organization and accessibility.

### 17. How do you create an email link?

Use the `<a>` tag with the `mailto:` scheme in the `href` attribute. Clicking the link can open the user's default email application.

Example: `<a href="mailto:hello@example.com">Send Email</a>`

### 18. What is the `<em>` tag?

The `<em>` tag adds semantic emphasis to text. Browsers usually display it in italics, and assistive technologies can interpret its emphasis.

### 19. How do you create a checkbox?

Use `<input type="checkbox">` to allow users to select an option. Multiple checkboxes can be selected independently, and associated `<label>` elements improve usability.

### 20. What is the `<label>` tag, and how do `for` and `id` improve accessibility?

The `<label>` tag provides a description for a form control. The label's `for` value should match the input's `id`, connecting the text to the control and helping screen readers identify it.

```html
<label for="email">Email:</label>
<input type="email" id="email" name="email">
```

### Questions 21–40

### 21. How do you create a dropdown list?

Use `<select>` to create the dropdown and `<option>` to define its choices. The `name` attribute identifies the field when form data is submitted.

```html
<select name="course">
  <option value="bca">BCA</option>
  <option value="btech">B.Tech</option>
</select>
```

### 22. What is the `<blockquote>` tag, and when should you use `cite`?

The `<blockquote>` element represents an extended quotation from another source. Its optional `cite` attribute can specify the source URL, although the URL is not displayed automatically.

### 23. How is HTML different from CSS?

HTML defines webpage structure and content, while CSS controls presentation, including colors, fonts, spacing, and layout.

### 24. What are semantic HTML elements?

Semantic elements communicate the meaning and purpose of webpage content. Examples include `<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, and `<footer>`. They improve code clarity and support accessibility.

### 25. How do you add a video in HTML5?

Use the `<video>` element and a nested `<source>` element to specify the video file. The `controls` attribute displays playback controls.

```html
<video controls>
  <source src="movie.mp4" type="video/mp4">
</video>
```

### 26. Why is the `alt` attribute important in `<img>`?

The `alt` attribute provides a text alternative for an image. It supports screen-reader users and provides useful information if the image cannot load. Decorative images should generally use `alt=""`.

### 27. What is the `<fieldset>` tag?

The `<fieldset>` element groups related form controls. The `<legend>` element provides a title for the group, improving form organization and accessibility.

### 28. What does `<noscript>` do, and why is it relevant?

The `<noscript>` element provides fallback content when JavaScript is disabled or unavailable. It can display instructions or alternative information to users who cannot run scripts.

### 29. How do you add an external JavaScript file?

Use the `<script>` tag with the `src` attribute to reference the JavaScript file.

Example: `<script src="app.js" defer></script>`

The `defer` attribute allows the script to download while HTML is being parsed and execute after parsing finishes.

### 30. How do you add CSS to an HTML document?

There are three common methods:

* Inline CSS: Uses the `style` attribute on an element.

* Internal CSS: Uses a `<style>` element inside `<head>`.

* External CSS: Uses `<link rel="stylesheet" href="style.css">`.

External CSS is often preferred for maintainability and reuse across pages.

### 31. When should you use `<strong>` and `<em>` instead of `<b>` and `<i>`?

`<strong>` indicates strong importance, and `<em>` indicates emphasis. `<b>` draws attention without adding strong importance, while `<i>` represents text in an alternate voice or mood.

Choose the element based on meaning, not only its visual appearance.

### 32. How do you create a multiline text input?

Use the `<textarea>` element for longer user input, such as comments or messages. The `rows` and `cols` attributes provide initial dimensions.

```html
<textarea name="comment" rows="4" cols="30"></textarea>
```

### 33. What is the `action` attribute in a form?

The `action` attribute specifies the URL that receives the form submission. If it is omitted or empty, the form generally submits to the current document URL.

### 34. What is the `<base>` tag?

The `<base>` element specifies a base URL for relative URLs in the document. It belongs inside `<head>` and can affect links and other URL-based resources throughout the page.

### 35. What is `enctype` in forms? When is `multipart/form-data` used?

The `enctype` attribute specifies how form data is encoded when submitted using POST.

* `application/x-www-form-urlencoded` — the default encoding.

* `multipart/form-data` — used for file uploads.

* `text/plain` — sends data as plain text and is rarely used.

### 36. How do you create a hidden input field?

Use `<input type="hidden">` to submit a value that is not displayed as a normal form control.

Example: `<input type="hidden" name="userId" value="123">`

Hidden fields are not secure storage; users can inspect or modify their values.

### 37. What is the `<address>` tag?

The `<address>` element represents contact information for the author or owner of a document or article. It can contain an email address, website link, or other relevant contact details.

### 38. What is the `lang` attribute in `<html>`?

The `lang` attribute identifies the primary language of the document. It helps browsers, search engines, and screen readers interpret the content correctly.

Example: `<html lang="en">`

### 39. What is the `contenteditable` attribute?

The `contenteditable` attribute allows users to edit an element's content directly in the browser when set to `true`.

Example: `<div contenteditable="true">Editable text</div>`

JavaScript or another application mechanism is needed if those changes must be saved.

### 40. Are `<div>` and `<span>` similar?

Yes. Both are generic containers, but they have different default display behavior.

* `<div>` — block-level container.

* `<span>` — inline container.

They are commonly used for grouping content when a more meaningful semantic element is not suitable.

### Questions 41–58

### 41. What is the difference between `<div>` and `<span>`?

`<div>` groups larger sections and normally starts on a new line. `<span>` groups smaller portions of inline content without normally starting a new line.

Both can use attributes such as `class` and `id`. CSS controls their styling.

### 42. Are `<div>` and `<span>` tags similar?

Yes. They are both generic HTML containers used for grouping content, applying CSS, or targeting elements with JavaScript. The main difference is that `<div>` is block-level by default, whereas `<span>` is inline by default.

### 43. What is the difference between `class` and `id`?

* `id` identifies a specific element and should be unique within a document.

* `class` groups elements and can be reused across multiple elements.

In CSS, `#intro` selects an ID, while `.highlight` selects a class.

### 44. What are the different types of input elements in HTML?

The `<input>` element supports different input types for collecting data.

Examples include:

* `text` — text input.

* `password` — password input.

* `email` — email input.

* `number` — numeric input.

* `radio` — single selection from a group.

* `checkbox` — independent selection.

* `date` — date input.

* `file` — file selection.

* `submit` — form submission button.

### 45. Which tags can be used inside the `<head>` element?

Common elements inside `<head>` include:

* `<title>` — document title.

* `<meta>` — metadata.

* `<link>` — external resources, such as CSS.

* `<style>` — internal CSS.

* `<script>` — JavaScript.

* `<base>` — base URL for relative URLs.

### 46. What is the difference between HTML and XHTML?

HTML follows the HTML syntax rules defined by the relevant HTML specification. XHTML applies XML syntax rules to HTML-like markup.

XHTML requires well-formed XML, including properly nested elements, quoted attribute values, and correctly closed elements.

### 47. What is HTML layout?

HTML layout is the organization of webpage content into meaningful regions. Common regions include the header, navigation, main content, sidebar, and footer. Semantic HTML defines the structure, while CSS controls positioning and appearance.

### 48. What are semantic elements?

Semantic elements describe the meaning of the content they contain.

Examples:

* `<main>` — primary content.

* `<nav>` — navigation links.

* `<article>` — independent content.

* `<aside>` — related supplementary content.

* `<figure>` — self-contained content, such as an image or chart.

* `<figcaption>` — caption for a figure.

* `<mark>` — highlighted text.

### 49. What are HTML entities?

HTML entities represent reserved characters or special symbols in markup. They help display characters that could otherwise be interpreted as HTML syntax.

Examples: `&lt;` displays `<`, `&gt;` displays `>`, and `&amp;` displays `&`.

### 50. How can you add symbols in HTML?

You can use HTML named entities or numeric character references to display special symbols.

Examples:

* `&copy;` — ©

* `&reg;` — ®

* `&trade;` — ™

* `&euro;` — €

* `&#8377;` — ₹

### 51. What is HTML encoding?

In the context of URLs, URL encoding converts characters into a format suitable for use in a URL. Characters are often represented using `%` followed by hexadecimal digits.

For example, a space can be encoded as `%20`. This is useful when URL values contain spaces or reserved characters.

### 52. What is the difference between HTML and XML?

HTML is primarily used to structure and present webpage content. XML is designed to store and transport structured data using custom-defined tags.

HTML has predefined elements such as `<p>` and `<table>`, while XML allows developers to define their own element names.

### 53. What is the difference between HTML and DHTML?

HTML defines the structure of a webpage. DHTML, or Dynamic HTML, is an older term for combining HTML, CSS, and JavaScript to change webpage content or appearance dynamically without necessarily reloading the page.

DHTML is not a separate programming language.

### 54. What is an iframe in HTML?

An `<iframe>` embeds another webpage or document within the current webpage.

Example:

```html
<iframe src="https://example.com"
        title="Example website"
        width="500"
        height="300"></iframe>
```

The `title` attribute helps users of assistive technologies understand the embedded content.

### 55. What is the difference between `<iframe>` and `<embed>`?

`<iframe>` embeds another browsing context, commonly another webpage. `<embed>` embeds external content that the browser can display or handle, depending on supported formats.

Use the element that matches the type of content being embedded.

### 56. What is the Geolocation API in HTML5?

The Geolocation API allows a website to request the user's geographic location through JavaScript. The browser generally asks for permission before sharing the location.

Example: `navigator.geolocation.getCurrentPosition(successCallback)`

It is commonly used for maps and location-based services and normally requires a secure context such as HTTPS.

### 57. What is the HTML Web Storage API?

The Web Storage API allows websites to store key-value data in the browser.

* `localStorage` keeps data across browser sessions until it is removed.

* `sessionStorage` keeps data for the current tab's page session.

Both are client-side storage mechanisms and should not be used to store sensitive information without appropriate security measures.

### 58. What are forms in HTML?

HTML forms collect user input using controls such as text fields, checkboxes, radio buttons, dropdowns, and buttons. The `<form>` element defines the form, and its `action` and `method` attributes control submission behavior.

### Questions 59–79

### 59. What is the `<canvas>` element?

The `<canvas>` element provides a drawing area for graphics created using JavaScript and the Canvas API. It is commonly used for charts, animations, image processing, and games.

Example: `<canvas id="myCanvas" width="300" height="150"></canvas>`

### 60. What is the `<dialog>` element, and how do `showModal()` and `close()` work?

The `<dialog>` element creates a native dialog box.

* `showModal()` opens it as a modal dialog, placing a backdrop behind it and restricting interaction with the rest of the page.

* `show()` opens it as a non-modal dialog.

* `close()` closes the dialog.

### 61. How do you add SVG to HTML?

SVG stands for Scalable Vector Graphics. It defines vector graphics using markup, so shapes remain sharp when resized.

```html
<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" fill="red"/>
</svg>
```

### 62. What are data attributes in HTML?

Custom data attributes store additional information on HTML elements. Their names begin with `data-`, and JavaScript can access them using the `dataset` property.

```html
<div id="user" data-user-id="123">User</div>
```

JavaScript can read the value using `element.dataset.userId`.

### 63. What is the `<template>` tag?

The `<template>` element stores HTML content that is not rendered immediately. JavaScript can later clone and insert the template content into the document, making it useful for reusable components.

### 64. What is the `rel` attribute in `<link>`?

The `rel` attribute specifies the relationship between the current document and a linked resource.

Examples:

* `rel="stylesheet"` — links a CSS stylesheet.

* `rel="icon"` — identifies a favicon.

* `rel="alternate"` — identifies an alternative version or representation of a resource.

### 65. How do you provide different language versions of a webpage?

Use `<link>` elements with `rel="alternate"` and the `hreflang` attribute to identify language-specific versions.

```html
<link rel="alternate"
      hreflang="fr"
      href="https://example.com/fr/">
```

This helps search engines understand which language version is intended for which audience.

### 66. What is the `<output>` tag?

The `<output>` element represents the result of a calculation or user action, often within a form. It can display a result that JavaScript updates when the input values change.

### 67. What is the difference between `localStorage` and `sessionStorage`?

Both store key-value data in the browser.

| localStorage                     | sessionStorage                                   |
| -------------------------------- | ------------------------------------------------ |
| Persists across browser sessions | Usually lasts for the current tab's page session |
| Remains until removed or cleared | Usually cleared when the tab's page session ends |
| Shared by same-origin pages      | Separate for each tab's page session             |

Both are subject to browser storage limits and same-origin rules.

### 68. What is the difference between `defer` and `async` in `<script>`?

Both allow an external script to download while HTML is being parsed.

* `defer` executes after HTML parsing finishes and preserves the order of deferred scripts.

* `async` exec
