# HTML Interview Questions & Answers — Complete Revision Guide

A complete, structured collection of HTML interview questions — from fundamentals to accessibility, performance, and SEO — with clear answers and code examples where they help. Built to be your one-stop revision resource the night before an interview or test.

## 📚 Table of Contents

- [🔥 Most Asked / Tricky Questions](#most-asked-tricky-questions)
  - [What is the difference between HTML elements and HTML tags?](#what-is-the-difference-between-html-elements-and-html-tags)
  - [What does the DOCTYPE declaration do, and why is it needed?](#what-does-the-doctype-declaration-do-and-why-is-it-needed)
  - [What is the difference between block-level and inline elements?](#what-is-the-difference-between-block-level-and-inline-elements)
  - [What's the difference between the id and class attributes?](#whats-the-difference-between-the-id-and-class-attributes)
  - [What is semantic HTML, and why does it matter?](#what-is-semantic-html-and-why-does-it-matter)
  - [What is the difference between `<div>` and `<span>`?](#what-is-the-difference-between-div-and-span)
  - [What is the difference between async and defer on a `<script>` tag?](#what-is-the-difference-between-async-and-defer-on-a-script-tag)
  - [What is the difference between localStorage, sessionStorage, and cookies?](#what-is-the-difference-between-localstorage-sessionstorage-and-cookies)
  - [What is the purpose of the alt attribute on `<img>`, and when should it be left empty?](#what-is-the-purpose-of-the-alt-attribute-on-img-and-when-should-it-be-left-empty)
  - [What is the difference between `<link>` and `<a>` tags?](#what-is-the-difference-between-link-and-a-tags)
  - [What is the viewport meta tag, and why is it essential for responsive design?](#what-is-the-viewport-meta-tag-and-why-is-it-essential-for-responsive-design)
  - [What's the difference between an HTML entity like &nbsp; and a regular space?](#whats-the-difference-between-an-html-entity-like-nbsp-and-a-regular-space)
  - [Why is it recommended to place `<script>` tags at the end of `<body>` (or use defer)?](#why-is-it-recommended-to-place-script-tags-at-the-end-of-body-or-use-defer)
  - [What is the difference between `<b>`/`<i>` and `<strong>`/`<em>`?](#what-is-the-difference-between-bi-and-strongem)
  - [What happens if you nest a block-level element inside an inline element?](#what-happens-if-you-nest-a-block-level-element-inside-an-inline-element)
- [HTML Basics](#html-basics)
  - [What is HTML and what is its role in web development?](#what-is-html-and-what-is-its-role-in-web-development)
  - [What is the basic structure of an HTML document?](#what-is-the-basic-structure-of-an-html-document)
  - [What is the difference between HTML and XHTML?](#what-is-the-difference-between-html-and-xhtml)
  - [What are void (self-closing) elements? Give examples.](#what-are-void-self-closing-elements-give-examples)
  - [What is the difference between an HTML attribute and a DOM property?](#what-is-the-difference-between-an-html-attribute-and-a-dom-property)
  - [What is the purpose of the `<meta charset="UTF-8">` tag?](#what-is-the-purpose-of-the-meta-charsetutf-8-tag)
  - [What are data attributes (data-*), and what are they used for?](#what-are-data-attributes-data--and-what-are-they-used-for)
  - [What is the difference between HTML4 and HTML5?](#what-is-the-difference-between-html4-and-html5)
  - [What is the difference between `<ol>`, `<ul>`, and `<dl>`?](#what-is-the-difference-between-ol-ul-and-dl)
  - [What is the difference between the `<head>` and `<body>` sections?](#what-is-the-difference-between-the-head-and-body-sections)
  - [How do you include CSS and JavaScript in an HTML document?](#how-do-you-include-css-and-javascript-in-an-html-document)
- [Semantic HTML & Document Structure](#semantic-html-document-structure)
  - [What are semantic HTML5 elements? Name several.](#what-are-semantic-html5-elements-name-several)
  - [What is the difference between `<section>` and `<div>`?](#what-is-the-difference-between-section-and-div)
  - [What is the difference between `<article>` and `<section>`?](#what-is-the-difference-between-article-and-section)
  - [What is the purpose of the `<main>` element, and how many can a page have?](#what-is-the-purpose-of-the-main-element-and-how-many-can-a-page-have)
  - [What is the difference between `<header>`/`<footer>` and `<head>`/`<body>`?](#what-is-the-difference-between-headerfooter-and-headbody)
  - [What is the `<nav>` element used for?](#what-is-the-nav-element-used-for)
  - [What is the `<figure>` and `<figcaption>` pairing used for?](#what-is-the-figure-and-figcaption-pairing-used-for)
  - [What is the purpose of heading tags (`<h1>`–`<h6>`), and how should they be structured?](#what-is-the-purpose-of-heading-tags-h1h6-and-how-should-they-be-structured)
  - [What is the difference between `<aside>` and a regular `<div>` used for a sidebar?](#what-is-the-difference-between-aside-and-a-regular-div-used-for-a-sidebar)
  - [How does using semantic HTML affect SEO?](#how-does-using-semantic-html-affect-seo)
- [Forms & Input Elements](#forms-input-elements)
  - [What is the purpose of the `<form>` element, and what are its key attributes?](#what-is-the-purpose-of-the-form-element-and-what-are-its-key-attributes)
  - [What is the difference between GET and POST as form submission methods?](#what-is-the-difference-between-get-and-post-as-form-submission-methods)
  - [What are some common HTML5 input types, and why do they matter?](#what-are-some-common-html5-input-types-and-why-do-they-matter)
  - [What is the difference between the placeholder and value attributes on an input?](#what-is-the-difference-between-the-placeholder-and-value-attributes-on-an-input)
  - [What is the purpose of the `<label>` element, and why is it important?](#what-is-the-purpose-of-the-label-element-and-why-is-it-important)
  - [What is the difference between disabled and readonly on a form input?](#what-is-the-difference-between-disabled-and-readonly-on-a-form-input)
  - [How does built-in HTML form validation work, and how do you customize it?](#how-does-built-in-html-form-validation-work-and-how-do-you-customize-it)
  - [What is the difference between a `<select>` dropdown and a set of `<input type="radio">` buttons?](#what-is-the-difference-between-a-select-dropdown-and-a-set-of-input-typeradio-buttons)
  - [What is the purpose of the `<fieldset>` and `<legend>` elements?](#what-is-the-purpose-of-the-fieldset-and-legend-elements)
  - [How do you handle file uploads in an HTML form?](#how-do-you-handle-file-uploads-in-an-html-form)
  - [What is the difference between `<button type="submit">`, type="button", and type="reset"?](#what-is-the-difference-between-button-typesubmit-typebutton-and-typereset)
  - [What is the autocomplete attribute, and why does it matter?](#what-is-the-autocomplete-attribute-and-why-does-it-matter)
- [Tables](#tables)
  - [What are the basic building blocks of an HTML table?](#what-are-the-basic-building-blocks-of-an-html-table)
  - [What is the purpose of `<thead>`, `<tbody>`, and `<tfoot>`?](#what-is-the-purpose-of-thead-tbody-and-tfoot)
  - [What do the colspan and rowspan attributes do?](#what-do-the-colspan-and-rowspan-attributes-do)
  - [How do you properly associate header cells with data cells for accessibility?](#how-do-you-properly-associate-header-cells-with-data-cells-for-accessibility)
  - [Should tables be used for page layout?](#should-tables-be-used-for-page-layout)
  - [What is the `<caption>` element used for in a table?](#what-is-the-caption-element-used-for-in-a-table)
  - [How would you make a large table responsive on mobile?](#how-would-you-make-a-large-table-responsive-on-mobile)
  - [What is the difference between border-collapse: collapse and default table borders?](#what-is-the-difference-between-border-collapse-collapse-and-default-table-borders)
- [Media & Graphics](#media-graphics)
  - [How do you embed an image in HTML, and what are the important attributes?](#how-do-you-embed-an-image-in-html-and-what-are-the-important-attributes)
  - [What is the purpose of the `<picture>` element?](#what-is-the-purpose-of-the-picture-element)
  - [What is the srcset attribute used for, and how does it differ from `<picture>`?](#what-is-the-srcset-attribute-used-for-and-how-does-it-differ-from-picture)
  - [How do you embed video and audio natively in HTML5?](#how-do-you-embed-video-and-audio-natively-in-html5)
  - [What is the purpose of the loading="lazy" attribute on images?](#what-is-the-purpose-of-the-loadinglazy-attribute-on-images)
  - [What is the `<canvas>` element used for?](#what-is-the-canvas-element-used-for)
  - [What is the difference between `<canvas>` and SVG for graphics?](#what-is-the-difference-between-canvas-and-svg-for-graphics)
  - [What are common video/audio formats, and why do multiple `<source>` tags matter?](#what-are-common-videoaudio-formats-and-why-do-multiple-source-tags-matter)
  - [How would you make an image accessible when it's purely decorative?](#how-would-you-make-an-image-accessible-when-its-purely-decorative)
  - [What is the object-fit CSS property, and why is it commonly used with images/video?](#what-is-the-object-fit-css-property-and-why-is-it-commonly-used-with-imagesvideo)
- [Links, Navigation & Metadata](#links-navigation-metadata)
  - [What is the difference between absolute and relative URLs in an `<a>` href?](#what-is-the-difference-between-absolute-and-relative-urls-in-an-a-href)
  - [What does target="_blank" do, and what security consideration comes with it?](#what-does-targetblank-do-and-what-security-consideration-comes-with-it)
  - [How do you create an in-page anchor link (jump to a section)?](#how-do-you-create-an-in-page-anchor-link-jump-to-a-section)
  - [What is the purpose of the rel attribute on a link, and what are some common values?](#what-is-the-purpose-of-the-rel-attribute-on-a-link-and-what-are-some-common-values)
  - [What is a canonical URL, and why is it important for SEO?](#what-is-a-canonical-url-and-why-is-it-important-for-seo)
  - [What are Open Graph meta tags, and what are they used for?](#what-are-open-graph-meta-tags-and-what-are-they-used-for)
  - [What is the purpose of the `<meta name="description">` tag?](#what-is-the-purpose-of-the-meta-namedescription-tag)
  - [How do you create a favicon, and where does it go in the HTML?](#how-do-you-create-a-favicon-and-where-does-it-go-in-the-html)
  - [What is the difference between a link's default, visited, hover, and active states?](#what-is-the-difference-between-a-links-default-visited-hover-and-active-states)
  - [What is a breadcrumb, and how would you mark it up semantically?](#what-is-a-breadcrumb-and-how-would-you-mark-it-up-semantically)
- [Accessibility (ARIA)](#accessibility-aria)
  - [What is web accessibility, and why does it matter?](#what-is-web-accessibility-and-why-does-it-matter)
  - [What is ARIA, and when should you use it?](#what-is-aria-and-when-should-you-use-it)
  - [What is the difference between aria-label and aria-labelledby?](#what-is-the-difference-between-aria-label-and-aria-labelledby)
  - [What is the purpose of the alt attribute vs. aria-label for accessibility?](#what-is-the-purpose-of-the-alt-attribute-vs-aria-label-for-accessibility)
  - [What are ARIA landmark roles, and why are they useful?](#what-are-aria-landmark-roles-and-why-are-they-useful)
  - [What is keyboard accessibility, and what should you test for?](#what-is-keyboard-accessibility-and-what-should-you-test-for)
  - [What is the tabindex attribute, and what do its different values mean?](#what-is-the-tabindex-attribute-and-what-do-its-different-values-mean)
  - [What is a "skip to content" link, and why is it important?](#what-is-a-skip-to-content-link-and-why-is-it-important)
  - [How do you make a custom dropdown or modal accessible?](#how-do-you-make-a-custom-dropdown-or-modal-accessible)
  - [What is the difference between aria-hidden="true" and the hidden HTML attribute?](#what-is-the-difference-between-aria-hiddentrue-and-the-hidden-html-attribute)
  - [What are common color-contrast accessibility requirements?](#what-are-common-color-contrast-accessibility-requirements)
  - [What is the difference between an accessible name and an accessible description in ARIA?](#what-is-the-difference-between-an-accessible-name-and-an-accessible-description-in-aria)
- [HTML5 APIs & Storage](#html5-apis-storage)
  - [What is the localStorage API, and how do you use it?](#what-is-the-localstorage-api-and-how-do-you-use-it)
  - [What is the Geolocation API used for?](#what-is-the-geolocation-api-used-for)
  - [What is the Drag and Drop API?](#what-is-the-drag-and-drop-api)
  - [What is the difference between Web Workers and the main JavaScript thread?](#what-is-the-difference-between-web-workers-and-the-main-javascript-thread)
  - [What is the History API, and what problem does it solve?](#what-is-the-history-api-and-what-problem-does-it-solve)
  - [What is the Fetch API, and how does it compare to XMLHttpRequest?](#what-is-the-fetch-api-and-how-does-it-compare-to-xmlhttprequest)
  - [What is IndexedDB, and how does it differ from localStorage?](#what-is-indexeddb-and-how-does-it-differ-from-localstorage)
  - [What is a Service Worker, and what enables it to power offline functionality?](#what-is-a-service-worker-and-what-enables-it-to-power-offline-functionality)
  - [What is the contenteditable attribute?](#what-is-the-contenteditable-attribute)
  - [What is the difference between the DOM and the HTML source code?](#what-is-the-difference-between-the-dom-and-the-html-source-code)
- [SEO & Meta Tags](#seo-meta-tags)
  - [What are the most important meta tags for basic on-page SEO?](#what-are-the-most-important-meta-tags-for-basic-on-page-seo)
  - [What is a sitemap.xml, and how does it help SEO?](#what-is-a-sitemapxml-and-how-does-it-help-seo)
  - [What is a robots.txt file, and what does it control?](#what-is-a-robotstxt-file-and-what-does-it-control)
  - [How does semantic HTML and heading structure impact SEO?](#how-does-semantic-html-and-heading-structure-impact-seo)
  - [What is structured data / Schema.org markup, and why is it used?](#what-is-structured-data-schemaorg-markup-and-why-is-it-used)
  - [What is the difference between "nofollow" and "noindex"?](#what-is-the-difference-between-nofollow-and-noindex)
  - [Why does page load speed matter for SEO?](#why-does-page-load-speed-matter-for-seo)
  - [What is the significance of using descriptive, keyword-relevant URLs?](#what-is-the-significance-of-using-descriptive-keyword-relevant-urls)
- [Performance & Best Practices](#performance-best-practices)
  - [How do image width/height attributes affect performance?](#how-do-image-widthheight-attributes-affect-performance)
  - [What is render-blocking content, and how do you minimize it?](#what-is-render-blocking-content-and-how-do-you-minimize-it)
  - [What is the purpose of preload, prefetch, and preconnect resource hints?](#what-is-the-purpose-of-preload-prefetch-and-preconnect-resource-hints)
  - [How does minifying HTML/CSS/JS improve performance?](#how-does-minifying-htmlcssjs-improve-performance)
  - [Why is it best practice to avoid deeply nested or excessive DOM elements?](#why-is-it-best-practice-to-avoid-deeply-nested-or-excessive-dom-elements)
  - [What is the difference between critical rendering path optimization and lazy loading?](#what-is-the-difference-between-critical-rendering-path-optimization-and-lazy-loading)
  - [How do web fonts impact performance, and how do you mitigate the impact?](#how-do-web-fonts-impact-performance-and-how-do-you-mitigate-the-impact)
  - [What is the impact of HTTP/2 on HTML/asset delivery compared to HTTP/1.1?](#what-is-the-impact-of-http2-on-htmlasset-delivery-compared-to-http11)
  - [What is accessibility's relationship to good HTML practices overall?](#what-is-accessibilitys-relationship-to-good-html-practices-overall)
  - [What tools would you use to audit an HTML page's performance and accessibility?](#what-tools-would-you-use-to-audit-an-html-pages-performance-and-accessibility)
- [Behavioral / Scenario-Based Questions](#behavioral-scenario-based-questions)
  - [How would you make an existing non-semantic HTML page more accessible without a full rewrite?](#how-would-you-make-an-existing-non-semantic-html-page-more-accessible-without-a-full-rewrite)
  - [How would you debug a page that looks broken only in one specific browser?](#how-would-you-debug-a-page-that-looks-broken-only-in-one-specific-browser)
  - [How would you decide whether to use a semantic element or ARIA roles for a custom widget?](#how-would-you-decide-whether-to-use-a-semantic-element-or-aria-roles-for-a-custom-widget)
  - [A page's Largest Contentful Paint (LCP) is slow — where would you look first in the HTML?](#a-pages-largest-contentful-paint-lcp-is-slow-where-would-you-look-first-in-the-html)
  - [How would you structure a form's HTML to work well for both sighted and screen-reader users?](#how-would-you-structure-a-forms-html-to-work-well-for-both-sighted-and-screen-reader-users)
  - [How would you handle serving different images for different device sizes and pixel densities?](#how-would-you-handle-serving-different-images-for-different-device-sizes-and-pixel-densities)
  - [What would you check first if a form isn't submitting data correctly to the server?](#what-would-you-check-first-if-a-form-isnt-submitting-data-correctly-to-the-server)
  - [How would you approach reviewing a teammate's HTML in a pull request?](#how-would-you-approach-reviewing-a-teammates-html-in-a-pull-request)
- [How to Use This Guide](#how-to-use-this-guide)

---

<a id="most-asked-tricky-questions"></a>
## 🔥 Most Asked / Tricky Questions

These come up in almost every HTML interview. If you're short on time, start here.

<a id="what-is-the-difference-between-html-elements-and-html-tags"></a>
### Q: What is the difference between HTML elements and HTML tags?
**Answer:** A tag is the markup syntax itself — the opening `<p>` or closing `</p>`. An element is the tag together with its content and attributes, e.g. `<p class="intro">Hello</p>` is the full element. People often use the terms interchangeably in conversation, but technically the tag is just the delimiter.

<a id="what-does-the-doctype-declaration-do-and-why-is-it-needed"></a>
### Q: What does the DOCTYPE declaration do, and why is it needed?
**Answer:** `<!DOCTYPE html>` tells the browser which rendering mode to use, triggering "standards mode" instead of the older, inconsistent "quirks mode" kept around for legacy pre-standards pages. Without it, browsers may render CSS and layout differently across each other.

<a id="what-is-the-difference-between-block-level-and-inline-elements"></a>
### Q: What is the difference between block-level and inline elements?
**Answer:** Block-level elements (`<div>`, `<p>`, `<h1>`) start on a new line and take the full available width by default. Inline elements (`<span>`, `<a>`, `<strong>`) only take up as much width as their content and sit inline with surrounding text, without forcing a line break.

<a id="whats-the-difference-between-the-id-and-class-attributes"></a>
### Q: What's the difference between the id and class attributes?
**Answer:** `id` must be unique within a page and targets one specific element (for CSS, JS, or in-page anchor links). `class` can be applied to multiple elements and is used for shared styling or behavior across a group of elements.

<a id="what-is-semantic-html-and-why-does-it-matter"></a>
### Q: What is semantic HTML, and why does it matter?
**Answer:** Semantic HTML uses elements that describe their meaning (`<header>`, `<article>`, `<nav>`) instead of generic containers (`<div>`, `<span>`) for everything. It improves accessibility (screen readers rely on semantic structure to navigate), SEO (search engines weigh it), and overall code readability.

<a id="what-is-the-difference-between-div-and-span"></a>
### Q: What is the difference between `<div>` and `<span>`?
**Answer:** Both are generic, non-semantic containers, but `<div>` is block-level (used to group larger sections of content) while `<span>` is inline (used to wrap a small piece of text within a sentence or line).

<a id="what-is-the-difference-between-async-and-defer-on-a-script-tag"></a>
### Q: What is the difference between async and defer on a `<script>` tag?
**Answer:** Both let a script download without blocking HTML parsing. `async` executes the script as soon as it finishes downloading — order isn't guaranteed relative to other scripts, and it can interrupt parsing mid-way. `defer` waits until HTML parsing is fully complete before executing, and multiple deferred scripts always run in the order they appear in the document.

<a id="what-is-the-difference-between-localstorage-sessionstorage-and-cookies"></a>
### Q: What is the difference between localStorage, sessionStorage, and cookies?
**Answer:** `localStorage` persists with no expiration until explicitly cleared, scoped per origin. `sessionStorage` persists only for the page session and is cleared when the tab closes, scoped per tab. Cookies are much smaller (~4KB), can have an expiration date, and — unlike the other two — are automatically sent to the server with every HTTP request, which matters for both performance and security.

<a id="what-is-the-purpose-of-the-alt-attribute-on-img-and-when-should-it-be-left-empty"></a>
### Q: What is the purpose of the alt attribute on `<img>`, and when should it be left empty?
**Answer:** `alt` provides alternative text describing an image for screen readers and for when the image fails to load. It should meaningfully describe the image's content or purpose — not just say "image of...". Purely decorative images that add no informational value should use an empty `alt=""` so screen readers skip them, rather than omitting the attribute entirely (which some screen readers announce as "unlabeled image").

<a id="what-is-the-difference-between-link-and-a-tags"></a>
### Q: What is the difference between `<link>` and `<a>` tags?
**Answer:** `<a>` creates a clickable hyperlink for navigation. `<link>` lives inside `<head>` and defines relationships between the document and external resources — most commonly stylesheets (`rel="stylesheet"`), but also favicons, preconnect hints, or canonical URLs. `<link>` has no visible content of its own.

<a id="what-is-the-viewport-meta-tag-and-why-is-it-essential-for-responsive-design"></a>
### Q: What is the viewport meta tag, and why is it essential for responsive design?
**Answer:** `<meta name="viewport" content="width=device-width, initial-scale=1">` tells mobile browsers to render the page at the device's actual width instead of a default desktop-width viewport (often 980px) that gets zoomed out. Without it, responsive CSS media queries won't behave as expected on mobile devices.

<a id="whats-the-difference-between-an-html-entity-like-nbsp-and-a-regular-space"></a>
### Q: What's the difference between an HTML entity like &nbsp; and a regular space?
**Answer:** `&nbsp;` (non-breaking space) prevents a line break at that point — keeping two words together, e.g. "10 mph" — and, unlike regular whitespace, multiple consecutive `&nbsp;` won't be collapsed into a single space by the browser.

<a id="why-is-it-recommended-to-place-script-tags-at-the-end-of-body-or-use-defer"></a>
### Q: Why is it recommended to place `<script>` tags at the end of `<body>` (or use defer)?
**Answer:** Script tags block HTML parsing by default while they download and execute. Placing them at the end of `<body>`, or using `defer`, lets the browser parse and render the visible page first, improving perceived load time since the script no longer holds up rendering everything below it.

<a id="what-is-the-difference-between-bi-and-strongem"></a>
### Q: What is the difference between `<b>`/`<i>` and `<strong>`/`<em>`?
**Answer:** `<b>` and `<i>` are purely presentational (bold/italic with no semantic meaning). `<strong>` conveys strong importance and `<em>` conveys emphasis — both are semantic and are announced differently by screen readers, even though visually they typically render the same as `<b>`/`<i>`.

<a id="what-happens-if-you-nest-a-block-level-element-inside-an-inline-element"></a>
### Q: What happens if you nest a block-level element inside an inline element?
**Answer:** Inline elements can generally contain other inline elements or text, and block elements can contain both block and inline children — but putting a block-level element inside an inline one (e.g. a `<div>` inside a `<span>`) is invalid HTML. Browsers typically "fix" it through error-correction parsing, producing unexpected DOM structure, so it's best avoided.

---

<a id="html-basics"></a>
## HTML Basics

<a id="what-is-html-and-what-is-its-role-in-web-development"></a>
### Q: What is HTML and what is its role in web development?
**Answer:** HTML (HyperText Markup Language) is the standard markup language used to structure content on the web — defining headings, paragraphs, links, images, and forms. It works alongside CSS (styling) and JavaScript (behavior) to build complete web pages.

<a id="what-is-the-basic-structure-of-an-html-document"></a>
### Q: What is the basic structure of an HTML document?
**Answer:** A `<head>` section holds metadata not directly visible on the page, and a `<body>` section holds everything that actually renders.

**Example:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Page Title</title>
</head>
<body>
  <h1>Hello, world!</h1>
</body>
</html>
```

<a id="what-is-the-difference-between-html-and-xhtml"></a>
### Q: What is the difference between HTML and XHTML?
**Answer:** XHTML is a stricter, XML-based reformulation of HTML requiring well-formed markup — every tag properly closed and lowercase, all attributes quoted, and only one root element. HTML5 is more forgiving and doesn't enforce strict XML syntax rules.

<a id="what-are-void-self-closing-elements-give-examples"></a>
### Q: What are void (self-closing) elements? Give examples.
**Answer:** Void elements have no closing tag and can't contain content, since they represent a single, standalone piece of content. Examples: `<img>`, `<br>`, `<hr>`, `<input>`, `<meta>`, `<link>`.

<a id="what-is-the-difference-between-an-html-attribute-and-a-dom-property"></a>
### Q: What is the difference between an HTML attribute and a DOM property?
**Answer:** An attribute is defined in the markup itself (e.g. `value="hello"` in the source) and represents the initial state. A property is the corresponding value on the live DOM object in JavaScript, which can change independently after the page loads — typing into an input changes its `value` property, but not the original `value` attribute in the source markup.

<a id="what-is-the-purpose-of-the-meta-charsetutf-8-tag"></a>
### Q: What is the purpose of the `<meta charset="UTF-8">` tag?
**Answer:** It declares the character encoding used for the document, ensuring special characters, accented letters, and symbols display correctly across browsers. UTF-8 is the near-universal standard recommended for virtually all web pages.

<a id="what-are-data-attributes-data--and-what-are-they-used-for"></a>
### Q: What are data attributes (data-*), and what are they used for?
**Answer:** Custom attributes prefixed with `data-` let you attach extra information to an HTML element without inventing non-standard attributes. They're commonly read and written through JavaScript's `element.dataset` API.

**Example:**
```html
<div data-user-id="42"></div>
```
```js
element.dataset.userId; // "42"
```

<a id="what-is-the-difference-between-html4-and-html5"></a>
### Q: What is the difference between HTML4 and HTML5?
**Answer:** HTML5 introduced semantic elements (`<header>`, `<footer>`, `<article>`, `<section>`), native multimedia support (`<audio>`, `<video>`) without plugins like Flash, new form input types (`email`, `date`, `range`), the `<canvas>` element, and APIs like localStorage, geolocation, and drag-and-drop. It also simplified the doctype down to just `<!DOCTYPE html>`.

<a id="what-is-the-difference-between-ol-ul-and-dl"></a>
### Q: What is the difference between `<ol>`, `<ul>`, and `<dl>`?
**Answer:** `<ul>` is an unordered (bulleted) list and `<ol>` is an ordered (numbered) list — both hold `<li>` items. `<dl>` is a description list, pairing terms (`<dt>`) with descriptions (`<dd>`), useful for glossaries or key-value content.

<a id="what-is-the-difference-between-the-head-and-body-sections"></a>
### Q: What is the difference between the `<head>` and `<body>` sections?
**Answer:** `<head>` contains metadata not directly rendered — title, character encoding, linked stylesheets/scripts, and meta tags for SEO/social sharing. `<body>` contains everything actually visible and rendered to the user.

<a id="how-do-you-include-css-and-javascript-in-an-html-document"></a>
### Q: How do you include CSS and JavaScript in an HTML document?
**Answer:** CSS: a `<link rel="stylesheet" href="styles.css">` in `<head>`, an inline `<style>` block, or the `style` attribute directly on an element. JavaScript: a `<script src="app.js"></script>` tag (with `defer`, or placed at the end of `<body>`), or an inline `<script>...</script>` block.

---

<a id="semantic-html-document-structure"></a>
## Semantic HTML & Document Structure

<a id="what-are-semantic-html5-elements-name-several"></a>
### Q: What are semantic HTML5 elements? Name several.
**Answer:** Semantic elements clearly describe their meaning to both the browser and developers. Common ones: `<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, `<aside>`, `<footer>`, `<figure>`/`<figcaption>`, `<time>`, `<mark>`.

<a id="what-is-the-difference-between-section-and-div"></a>
### Q: What is the difference between `<section>` and `<div>`?
**Answer:** `<section>` is a semantic element representing a thematic grouping of content, typically with its own heading — it conveys meaning to assistive technology and helps outline document structure. `<div>` is a purely generic container used only for styling/scripting hooks, with no inherent meaning.

<a id="what-is-the-difference-between-article-and-section"></a>
### Q: What is the difference between `<article>` and `<section>`?
**Answer:** `<article>` represents self-contained content that could be distributed or reused independently — a blog post, a news story, a forum comment. `<section>` groups related content within a page or article, often with a heading, but doesn't imply that same standalone reusability.

<a id="what-is-the-purpose-of-the-main-element-and-how-many-can-a-page-have"></a>
### Q: What is the purpose of the `<main>` element, and how many can a page have?
**Answer:** `<main>` wraps a page's dominant, unique content, excluding repeated elements like headers, nav, and footers. There should be only one visible `<main>` per page — it helps assistive technology and "skip to content" links jump straight to the primary content.

<a id="what-is-the-difference-between-headerfooter-and-headbody"></a>
### Q: What is the difference between `<header>`/`<footer>` and `<head>`/`<body>`?
**Answer:** `<head>`/`<body>` are top-level document structure — metadata vs. rendered content. `<header>`/`<footer>` are semantic content elements that live inside `<body>` (and can appear multiple times, e.g. a header for each `<article>`) representing introductory or closing content for a page or a section.

<a id="what-is-the-nav-element-used-for"></a>
### Q: What is the `<nav>` element used for?
**Answer:** `<nav>` wraps a major block of navigation links — the main site menu, a table of contents, breadcrumbs. Not every group of links needs `<nav>` — it's meant for significant, page-level navigation blocks, not every link on the page.

<a id="what-is-the-figure-and-figcaption-pairing-used-for"></a>
### Q: What is the `<figure>` and `<figcaption>` pairing used for?
**Answer:** `<figure>` groups self-contained content — typically an image, diagram, or code snippet — that could be moved elsewhere without affecting the main flow, and `<figcaption>` provides its caption, semantically linked to the figure.

<a id="what-is-the-purpose-of-heading-tags-h1h6-and-how-should-they-be-structured"></a>
### Q: What is the purpose of heading tags (`<h1>`–`<h6>`), and how should they be structured?
**Answer:** Heading tags build a hierarchical outline of a page's content, used by screen readers to navigate and by search engines to understand structure. Best practice: one `<h1>` per page, and don't skip heading levels (e.g. `<h2>` straight to `<h4>`) purely for visual sizing — use CSS for that instead.

<a id="what-is-the-difference-between-aside-and-a-regular-div-used-for-a-sidebar"></a>
### Q: What is the difference between `<aside>` and a regular `<div>` used for a sidebar?
**Answer:** `<aside>` semantically marks content tangentially related to the surrounding content — a sidebar, a pull quote, related links — which assistive technology can identify and optionally skip. A generic `<div>` conveys none of that meaning even if it looks like a sidebar visually.

<a id="how-does-using-semantic-html-affect-seo"></a>
### Q: How does using semantic HTML affect SEO?
**Answer:** Search engines use semantic structure (headings, `<article>`, `<nav>`, etc.) as signals for understanding page hierarchy and content importance, which can influence how content is indexed and displayed — e.g., in featured snippets. It's not the only SEO factor, but it's a meaningful, low-cost one to get right.

---

<a id="forms-input-elements"></a>
## Forms & Input Elements

<a id="what-is-the-purpose-of-the-form-element-and-what-are-its-key-attributes"></a>
### Q: What is the purpose of the `<form>` element, and what are its key attributes?
**Answer:** `<form>` wraps a set of interactive controls for submitting data. Key attributes: `action` (the URL data is sent to), `method` (`GET` or `POST`), and `enctype` (how data is encoded, e.g. `multipart/form-data` for file uploads).

<a id="what-is-the-difference-between-get-and-post-as-form-submission-methods"></a>
### Q: What is the difference between GET and POST as form submission methods?
**Answer:** `GET` appends form data as URL query parameters — visible in the URL, bookmarkable, cacheable, but limited in length and unsuitable for sensitive data. `POST` sends data in the request body — not visible in the URL, no practical length limit, and appropriate for sensitive data or larger payloads (though HTTPS is what actually encrypts it in transit).

<a id="what-are-some-common-html5-input-types-and-why-do-they-matter"></a>
### Q: What are some common HTML5 input types, and why do they matter?
**Answer:** `email`, `number`, `date`, `tel`, `url`, `range`, `color`, `search`, among others. They trigger the appropriate mobile keyboard, enable built-in browser validation (e.g. rejecting a malformed email), and improve UX without extra JavaScript.

**Example:**
```html
<input type="email" required>
```

<a id="what-is-the-difference-between-the-placeholder-and-value-attributes-on-an-input"></a>
### Q: What is the difference between the placeholder and value attributes on an input?
**Answer:** `placeholder` shows greyed-out hint text inside an empty input that disappears once the user types — it's never submitted as data and shouldn't replace a proper `<label>`. `value` sets (or holds) the input's actual current content, which is submitted with the form.

<a id="what-is-the-purpose-of-the-label-element-and-why-is-it-important"></a>
### Q: What is the purpose of the `<label>` element, and why is it important?
**Answer:** `<label>` associates descriptive text with a form control, improving accessibility (screen readers announce the label when the input is focused) and usability (clicking the label focuses or toggles the associated input). Association is done via `for` matching the input's `id`, or by wrapping the input inside the label.

**Example:**
```html
<label for="email">Email</label>
<input id="email" type="email">
```

<a id="what-is-the-difference-between-disabled-and-readonly-on-a-form-input"></a>
### Q: What is the difference between disabled and readonly on a form input?
**Answer:** A `disabled` input can't be focused, edited, or interacted with, and its value is **not** submitted with the form. A `readonly` input can be focused and its text selected, but not edited — and its value **is** still submitted.

<a id="how-does-built-in-html-form-validation-work-and-how-do-you-customize-it"></a>
### Q: How does built-in HTML form validation work, and how do you customize it?
**Answer:** Attributes like `required`, `pattern`, `minlength`/`maxlength`, and `min`/`max` trigger the browser's native validation before submission, showing default error messages and applying `:valid`/`:invalid` CSS pseudo-classes. Customize the message via the Constraint Validation API — `input.setCustomValidity('message')` in JavaScript.

<a id="what-is-the-difference-between-a-select-dropdown-and-a-set-of-input-typeradio-buttons"></a>
### Q: What is the difference between a `<select>` dropdown and a set of `<input type="radio">` buttons?
**Answer:** Both let a user pick one option from a set, but `<select>` is more compact and better for many options (hidden until clicked), while radio buttons show every option at once — better for a small number of choices where seeing everything at a glance matters.

<a id="what-is-the-purpose-of-the-fieldset-and-legend-elements"></a>
### Q: What is the purpose of the `<fieldset>` and `<legend>` elements?
**Answer:** `<fieldset>` groups related form controls together (with a border by default), and `<legend>` provides a caption for that group — useful for accessibility, e.g. grouping a set of radio buttons under a meaningful label like "Preferred contact method."

<a id="how-do-you-handle-file-uploads-in-an-html-form"></a>
### Q: How do you handle file uploads in an HTML form?
**Answer:** Use `<input type="file">`, and set the form's `enctype="multipart/form-data"` (required for binary file data to be sent correctly) with `method="post"`. The `accept` attribute can restrict allowed file types (e.g. `accept="image/*"`), and `multiple` allows selecting more than one file.

<a id="what-is-the-difference-between-button-typesubmit-typebutton-and-typereset"></a>
### Q: What is the difference between `<button type="submit">`, type="button", and type="reset"?
**Answer:** `type="submit"` (the default inside a form) submits the form. `type="button"` does nothing on its own — meant for custom JavaScript-driven behavior. `type="reset"` clears all fields back to their initial values — rarely used today since it can accidentally wipe user input.

<a id="what-is-the-autocomplete-attribute-and-why-does-it-matter"></a>
### Q: What is the autocomplete attribute, and why does it matter?
**Answer:** `autocomplete` hints to the browser whether and how to offer to fill in a field from previously saved data (e.g. `autocomplete="email"`, `autocomplete="new-password"`). Setting it correctly speeds up form completion significantly and is especially important for accessibility, since browsers and password managers rely on it to autofill accurately.

---

<a id="tables"></a>
## Tables

<a id="what-are-the-basic-building-blocks-of-an-html-table"></a>
### Q: What are the basic building blocks of an HTML table?
**Answer:** `<table>` is the container, `<tr>` defines a row, `<td>` defines a standard data cell, and `<th>` defines a header cell — bold and centered by default, and semantically marked as a header for accessibility.

<a id="what-is-the-purpose-of-thead-tbody-and-tfoot"></a>
### Q: What is the purpose of `<thead>`, `<tbody>`, and `<tfoot>`?
**Answer:** They group a table's rows into header, body, and footer sections respectively. This isn't just cosmetic — it helps assistive technology understand table structure, and can let `<tbody>` scroll independently of a fixed `<thead>` in some layouts.

<a id="what-do-the-colspan-and-rowspan-attributes-do"></a>
### Q: What do the colspan and rowspan attributes do?
**Answer:** `colspan` makes a cell span multiple columns; `rowspan` makes it span multiple rows — used for merged cells, like a header spanning several sub-columns.

**Example:**
```html
<th colspan="2">Contact Info</th>
```

<a id="how-do-you-properly-associate-header-cells-with-data-cells-for-accessibility"></a>
### Q: How do you properly associate header cells with data cells for accessibility?
**Answer:** Use `<th scope="col">` or `<th scope="row">` to indicate whether a header applies to a column or a row — screen readers use this to announce the right header as a user navigates through data cells. For complex tables, the `headers`/`id` attribute pairing gives even more precise association.

<a id="should-tables-be-used-for-page-layout"></a>
### Q: Should tables be used for page layout?
**Answer:** No — using tables purely for visual layout instead of tabular data is an outdated, pre-CSS-era practice. It creates accessibility problems (screen readers announce layout tables as if they held data, confusing users) and produces inflexible, hard-to-maintain markup. Modern layout should use CSS Flexbox or Grid.

<a id="what-is-the-caption-element-used-for-in-a-table"></a>
### Q: What is the `<caption>` element used for in a table?
**Answer:** `<caption>` provides a title or description for the whole table, placed as the first child inside `<table>`. Screen readers announce it before the table content, giving context about what the data represents.

<a id="how-would-you-make-a-large-table-responsive-on-mobile"></a>
### Q: How would you make a large table responsive on mobile?
**Answer:** Common approaches: wrap the table in a scrollable container (`overflow-x: auto`) so it scrolls horizontally on small screens, or reflow it into a stacked, card-like layout on narrow viewports (hiding `<thead>` and labeling each cell with a `data-label` via CSS) — a well-known responsive-table pattern.

<a id="what-is-the-difference-between-border-collapse-collapse-and-default-table-borders"></a>
### Q: What is the difference between border-collapse: collapse and default table borders?
**Answer:** By default, adjacent table cell borders are separate, creating a double-border look with spacing between them. `border-collapse: collapse` (a CSS property) merges adjacent borders into a single shared line, producing the clean, single-line grid look most designs want.

---

<a id="media-graphics"></a>
## Media & Graphics

<a id="how-do-you-embed-an-image-in-html-and-what-are-the-important-attributes"></a>
### Q: How do you embed an image in HTML, and what are the important attributes?
**Answer:** `<img src="photo.jpg" alt="Description" width="600" height="400">`. `src` is the image path, `alt` is required alternative text for accessibility and fallback, and `width`/`height` help the browser reserve space before the image loads, reducing layout shift.

<a id="what-is-the-purpose-of-the-picture-element"></a>
### Q: What is the purpose of the `<picture>` element?
**Answer:** `<picture>` lets you serve different image sources based on conditions like viewport width or supported formats, using nested `<source>` elements with an `<img>` fallback — useful for art direction (different crops for mobile vs. desktop) or serving modern formats like WebP/AVIF with a fallback.

**Example:**
```html
<picture>
  <source srcset="photo.webp" type="image/webp">
  <img src="photo.jpg" alt="A description">
</picture>
```

<a id="what-is-the-srcset-attribute-used-for-and-how-does-it-differ-from-picture"></a>
### Q: What is the srcset attribute used for, and how does it differ from `<picture>`?
**Answer:** `srcset` (on `<img>` directly) lets the browser choose the best resolution of the *same* image from a list of candidates based on screen density/size — resolution switching. `<picture>` handles more complex cases, like serving genuinely different images or formats, not just different resolutions of the same one.

**Example:**
```html
<img srcset="small.jpg 480w, large.jpg 1080w" sizes="(max-width: 600px) 480px, 1080px" src="large.jpg" alt="...">
```

<a id="how-do-you-embed-video-and-audio-natively-in-html5"></a>
### Q: How do you embed video and audio natively in HTML5?
**Answer:** `<video>` and `<audio>` support native playback without plugins, with a `controls` attribute for the built-in UI, `<source>` children for format fallbacks, and attributes like `autoplay`, `loop`, and `muted`.

**Example:**
```html
<video controls width="600">
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.webm" type="video/webm">
  Your browser doesn't support video.
</video>
```

<a id="what-is-the-purpose-of-the-loadinglazy-attribute-on-images"></a>
### Q: What is the purpose of the loading="lazy" attribute on images?
**Answer:** It tells the browser to defer loading an offscreen image until the user scrolls near it, reducing initial page load time and bandwidth usage for images below the fold — a native alternative to JavaScript-based lazy-loading libraries.

<a id="what-is-the-canvas-element-used-for"></a>
### Q: What is the `<canvas>` element used for?
**Answer:** `<canvas>` provides a blank, scriptable drawing surface for rendering graphics, animations, or game visuals pixel-by-pixel via JavaScript (typically the Canvas 2D API or WebGL) — unlike SVG, canvas content isn't part of the DOM and can't be styled per shape with CSS selectors.

<a id="what-is-the-difference-between-canvas-and-svg-for-graphics"></a>
### Q: What is the difference between `<canvas>` and SVG for graphics?
**Answer:** Canvas is raster-based and imperative — you draw shapes via JS calls and the browser doesn't track individual shapes afterward, making it well suited to complex, frequently-redrawn scenes like games. SVG is vector-based and declarative — each shape is an actual DOM element you can style with CSS and attach event listeners to, better suited to icons, diagrams, and graphics that need to scale without quality loss.

<a id="what-are-common-videoaudio-formats-and-why-do-multiple-source-tags-matter"></a>
### Q: What are common video/audio formats, and why do multiple `<source>` tags matter?
**Answer:** Common formats: MP4 (H.264) and WebM for video; MP3 and OGG for audio. Different browsers have historically supported different formats, so providing multiple `<source>` elements lets the browser pick the first one it supports, improving cross-browser compatibility.

<a id="how-would-you-make-an-image-accessible-when-its-purely-decorative"></a>
### Q: How would you make an image accessible when it's purely decorative?
**Answer:** Give it an empty `alt=""` attribute (not omitted entirely) so screen readers skip it rather than reading a meaningless or auto-generated description, and consider whether it should be a CSS `background-image` instead if it carries no content meaning at all.

<a id="what-is-the-object-fit-css-property-and-why-is-it-commonly-used-with-imagesvideo"></a>
### Q: What is the object-fit CSS property, and why is it commonly used with images/video?
**Answer:** `object-fit` (e.g. `cover`, `contain`) controls how a replaced element like `<img>` or `<video>` is resized to fit its box. `cover` crops to fill the box while preserving aspect ratio; `contain` fits the whole element inside the box, letterboxing if needed. Widely used for consistent image galleries and thumbnails without distortion.

---

<a id="links-navigation-metadata"></a>
## Links, Navigation & Metadata

<a id="what-is-the-difference-between-absolute-and-relative-urls-in-an-a-href"></a>
### Q: What is the difference between absolute and relative URLs in an `<a>` href?
**Answer:** An absolute URL includes the full address (`https://example.com/page`) and works regardless of the current page's location. A relative URL (`/page`, `../page`, `page.html`) is resolved relative to the current document's location, and breaks if the file structure changes without updating the link.

<a id="what-does-targetblank-do-and-what-security-consideration-comes-with-it"></a>
### Q: What does target="_blank" do, and what security consideration comes with it?
**Answer:** It opens the link in a new tab or window. Best practice is to also add `rel="noopener noreferrer"` — without it, the newly opened page can access `window.opener` and potentially redirect the original tab to a malicious page ("tabnabbing"), and `noreferrer` additionally prevents leaking the referring URL.

<a id="how-do-you-create-an-in-page-anchor-link-jump-to-a-section"></a>
### Q: How do you create an in-page anchor link (jump to a section)?
**Answer:** Give the target element an `id`, then link to it with a hash fragment.

**Example:**
```html
<a href="#section2">Jump to Section 2</a>
<h2 id="section2">Section 2</h2>
```

<a id="what-is-the-purpose-of-the-rel-attribute-on-a-link-and-what-are-some-common-values"></a>
### Q: What is the purpose of the rel attribute on a link, and what are some common values?
**Answer:** `rel` describes the relationship between the current document and the linked resource. Common values: `nofollow` (tells search engines not to pass ranking credit through the link), `noopener`/`noreferrer` (security, as above), `canonical` (indicates the preferred URL for duplicate content), and `stylesheet` (for CSS).

<a id="what-is-a-canonical-url-and-why-is-it-important-for-seo"></a>
### Q: What is a canonical URL, and why is it important for SEO?
**Answer:** `<link rel="canonical" href="https://example.com/preferred-url">` tells search engines which URL is authoritative when the same or similar content is reachable via multiple URLs (with/without a trailing slash, or tracking parameters) — preventing duplicate-content penalties and consolidating ranking signals to one URL.

<a id="what-are-open-graph-meta-tags-and-what-are-they-used-for"></a>
### Q: What are Open Graph meta tags, and what are they used for?
**Answer:** Open Graph tags (`og:title`, `og:description`, `og:image`, `og:url`, etc.) are meta tags controlling how a page's link preview appears when shared on social platforms like Facebook, LinkedIn, or Slack.

**Example:**
```html
<meta property="og:title" content="Page Title">
<meta property="og:image" content="https://example.com/preview.jpg">
```

<a id="what-is-the-purpose-of-the-meta-namedescription-tag"></a>
### Q: What is the purpose of the `<meta name="description">` tag?
**Answer:** It provides a short summary of the page's content, which search engines often display as the snippet text under the page title in results. It doesn't directly affect ranking but strongly influences click-through rate.

<a id="how-do-you-create-a-favicon-and-where-does-it-go-in-the-html"></a>
### Q: How do you create a favicon, and where does it go in the HTML?
**Answer:** Add `<link rel="icon" href="/favicon.ico">` (or a `.png`/`.svg` variant) inside `<head>` — browsers display it in the tab, bookmarks, and history.

<a id="what-is-the-difference-between-a-links-default-visited-hover-and-active-states"></a>
### Q: What is the difference between a link's default, visited, hover, and active states?
**Answer:** These correspond to CSS pseudo-classes: `:link` (unvisited), `:visited` (already clicked before), `:hover` (mouse over), `:active` (being clicked). Styling them in that order — remembered by the mnemonic "LoVe HAte" — gives users visual feedback about link state and interaction.

<a id="what-is-a-breadcrumb-and-how-would-you-mark-it-up-semantically"></a>
### Q: What is a breadcrumb, and how would you mark it up semantically?
**Answer:** A breadcrumb shows the user's location within a site's hierarchy (Home > Category > Page). It's typically marked up as an ordered list inside `<nav aria-label="breadcrumb">`, often with `aria-current="page"` on the final, current item for accessibility.

---

<a id="accessibility-aria"></a>
## Accessibility (ARIA)

<a id="what-is-web-accessibility-and-why-does-it-matter"></a>
### Q: What is web accessibility, and why does it matter?
**Answer:** Accessibility (a11y) means designing and building sites usable by people with disabilities — visual, auditory, motor, or cognitive — often relying on assistive technology like screen readers or keyboard-only navigation. It matters for inclusivity, is frequently a legal requirement (e.g. ADA, WCAG compliance), and generally improves usability for everyone.

<a id="what-is-aria-and-when-should-you-use-it"></a>
### Q: What is ARIA, and when should you use it?
**Answer:** ARIA (Accessible Rich Internet Applications) is a set of attributes that add accessibility information to HTML, especially for custom widgets built from generic elements that lack built-in semantics. The first rule of ARIA is: don't use it if a native HTML element already provides the needed semantics and behavior — prefer `<button>` over `<div role="button">`.

<a id="what-is-the-difference-between-aria-label-and-aria-labelledby"></a>
### Q: What is the difference between aria-label and aria-labelledby?
**Answer:** `aria-label` provides a text string directly as the accessible name for an element (e.g. an icon-only button: `<button aria-label="Close">×</button>`). `aria-labelledby` instead references the `id` of another element on the page whose text content becomes the accessible name — useful when visible label text already exists elsewhere.

<a id="what-is-the-purpose-of-the-alt-attribute-vs-aria-label-for-accessibility"></a>
### Q: What is the purpose of the alt attribute vs. aria-label for accessibility?
**Answer:** `alt` is specifically for images and is part of core HTML, required by spec on `<img>`. `aria-label` is a broader ARIA attribute that can apply an accessible name to nearly any element, commonly used for interactive controls that lack visible text, like icon buttons or custom widgets.

<a id="what-are-aria-landmark-roles-and-why-are-they-useful"></a>
### Q: What are ARIA landmark roles, and why are they useful?
**Answer:** Landmark roles (`role="navigation"`, `role="main"`, `role="banner"`, etc.) mark major regions of a page, letting screen reader users jump directly between them instead of tabbing through everything. Modern semantic HTML elements (`<nav>`, `<main>`, `<header>`) already carry these landmark roles implicitly, so explicit ARIA roles are mostly needed only when semantic HTML isn't used.

<a id="what-is-keyboard-accessibility-and-what-should-you-test-for"></a>
### Q: What is keyboard accessibility, and what should you test for?
**Answer:** It means every interactive element — links, buttons, form controls, custom widgets — can be reached and operated using only the keyboard, typically Tab to move focus and Enter/Space to activate. Test that focus order is logical, nothing traps keyboard focus, and there's always a visible focus indicator.

<a id="what-is-the-tabindex-attribute-and-what-do-its-different-values-mean"></a>
### Q: What is the tabindex attribute, and what do its different values mean?
**Answer:** `tabindex="0"` adds an element to the natural tab order — useful for making a custom element like a `<div>` focusable. `tabindex="-1"` removes it from the tab order but still allows programmatic focus via JavaScript's `.focus()`. A positive `tabindex` forces a custom tab order — generally discouraged since it's easy to create a confusing focus sequence.

<a id="what-is-a-skip-to-content-link-and-why-is-it-important"></a>
### Q: What is a "skip to content" link, and why is it important?
**Answer:** Typically the very first focusable element on a page — a visually hidden link (revealed on focus) that jumps keyboard/screen-reader users straight past repetitive navigation to the main content, saving them from tabbing through the entire header/nav on every single page.

<a id="how-do-you-make-a-custom-dropdown-or-modal-accessible"></a>
### Q: How do you make a custom dropdown or modal accessible?
**Answer:** Use appropriate ARIA roles and states (`role="dialog"`, `aria-modal="true"`, `aria-expanded` for dropdown triggers), manage focus explicitly (move it into the modal when opened, trap it while open, return it to the triggering element when closed), and ensure it can be closed with the Escape key.

<a id="what-is-the-difference-between-aria-hiddentrue-and-the-hidden-html-attribute"></a>
### Q: What is the difference between aria-hidden="true" and the hidden HTML attribute?
**Answer:** The `hidden` attribute removes an element from both the visual layout and the accessibility tree entirely, similar to `display: none`. `aria-hidden="true"` hides an element only from assistive technology while it may still be visually present — useful for hiding purely decorative icons from screen readers without hiding them visually.

<a id="what-are-common-color-contrast-accessibility-requirements"></a>
### Q: What are common color-contrast accessibility requirements?
**Answer:** WCAG guidelines specify minimum contrast ratios between text and background — commonly 4.5:1 for normal text and 3:1 for large text at the AA compliance level — to ensure readability for users with low vision or color blindness.

<a id="what-is-the-difference-between-an-accessible-name-and-an-accessible-description-in-aria"></a>
### Q: What is the difference between an accessible name and an accessible description in ARIA?
**Answer:** The accessible name is the primary label announced for an element (from visible text, `aria-label`, or `aria-labelledby`) — it identifies *what* the element is. The accessible description (via `aria-describedby`) provides supplementary detail announced after the name — like a hint or extra instructions — without being the primary identifier.

---

<a id="html5-apis-storage"></a>
## HTML5 APIs & Storage

<a id="what-is-the-localstorage-api-and-how-do-you-use-it"></a>
### Q: What is the localStorage API, and how do you use it?
**Answer:** `localStorage` stores key-value string data in the browser that persists indefinitely until explicitly cleared, scoped to the page's origin.

**Example:**
```js
localStorage.setItem('theme', 'dark');
const theme = localStorage.getItem('theme');
localStorage.removeItem('theme');
```

<a id="what-is-the-geolocation-api-used-for"></a>
### Q: What is the Geolocation API used for?
**Answer:** It lets a web page — with the user's explicit permission — access the device's current geographic location via `navigator.geolocation.getCurrentPosition()`, useful for maps, location-based recommendations, or delivery services.

<a id="what-is-the-drag-and-drop-api"></a>
### Q: What is the Drag and Drop API?
**Answer:** A native HTML5 API that makes elements draggable (`draggable="true"`) and defines drop targets, firing events like `dragstart`, `dragover`, and `drop` that you handle in JavaScript — used for drag-and-drop file uploads or reorderable lists.

<a id="what-is-the-difference-between-web-workers-and-the-main-javascript-thread"></a>
### Q: What is the difference between Web Workers and the main JavaScript thread?
**Answer:** Web Workers run JavaScript in a background thread separate from the main UI thread, allowing CPU-intensive tasks to run without freezing the page or blocking user interaction. Workers communicate with the main thread via message passing (`postMessage`) and have no direct DOM access.

<a id="what-is-the-history-api-and-what-problem-does-it-solve"></a>
### Q: What is the History API, and what problem does it solve?
**Answer:** The History API (`pushState`, `replaceState`, the `popstate` event) lets JavaScript change the browser's URL and history without a full page reload — the foundation client-side routing libraries build on for single-page applications.

<a id="what-is-the-fetch-api-and-how-does-it-compare-to-xmlhttprequest"></a>
### Q: What is the Fetch API, and how does it compare to XMLHttpRequest?
**Answer:** `fetch()` is a modern, Promise-based API for HTTP requests, replacing the older, callback-based `XMLHttpRequest`. It has cleaner syntax and integrates naturally with `async`/`await`, though it requires an extra step (`response.json()`) to parse JSON and doesn't reject on HTTP error statuses like 404 by default — you have to check `response.ok` yourself.

<a id="what-is-indexeddb-and-how-does-it-differ-from-localstorage"></a>
### Q: What is IndexedDB, and how does it differ from localStorage?
**Answer:** IndexedDB is a low-level, transactional, NoSQL-style database built into the browser, supporting structured data, indexes, and much larger storage limits than `localStorage`. `localStorage` is synchronous and string-only, which blocks the main thread and is unsuitable for large or complex data; IndexedDB is asynchronous and better suited to offline apps or larger structured datasets.

<a id="what-is-a-service-worker-and-what-enables-it-to-power-offline-functionality"></a>
### Q: What is a Service Worker, and what enables it to power offline functionality?
**Answer:** A Service Worker is a script that runs in the background, separate from the page, acting as a programmable network proxy — it can intercept network requests and serve cached responses, enabling offline support, push notifications, and background sync for Progressive Web Apps.

<a id="what-is-the-contenteditable-attribute"></a>
### Q: What is the contenteditable attribute?
**Answer:** Setting `contenteditable="true"` on any element makes its content directly editable by the user in the browser, without needing a `<textarea>` or `<input>` — commonly used to build custom rich-text editors.

<a id="what-is-the-difference-between-the-dom-and-the-html-source-code"></a>
### Q: What is the difference between the DOM and the HTML source code?
**Answer:** The HTML source is the static markup as originally written or downloaded. The DOM is the live, in-memory tree the browser builds from that HTML — JavaScript can modify the DOM at runtime (adding/removing elements, changing attributes) without those changes ever appearing in the original HTML source or view-source.

---

<a id="seo-meta-tags"></a>
## SEO & Meta Tags

<a id="what-are-the-most-important-meta-tags-for-basic-on-page-seo"></a>
### Q: What are the most important meta tags for basic on-page SEO?
**Answer:** `<title>` (arguably the single most important on-page SEO element), `<meta name="description">` (influences click-through rate from search results), and `<meta name="viewport">` (mobile-friendliness is a ranking factor). `<link rel="canonical">` also matters to avoid duplicate-content issues.

<a id="what-is-a-sitemapxml-and-how-does-it-help-seo"></a>
### Q: What is a sitemap.xml, and how does it help SEO?
**Answer:** A sitemap is an XML file listing a site's important URLs, often with metadata like last-modified date and priority, helping search engine crawlers discover and index pages more efficiently — especially useful for large sites or pages that aren't well linked internally.

<a id="what-is-a-robotstxt-file-and-what-does-it-control"></a>
### Q: What is a robots.txt file, and what does it control?
**Answer:** A plain-text file at a site's root that instructs well-behaved crawlers which paths they're allowed or disallowed from crawling. It's a convention, not an enforced restriction — it doesn't prevent access, just requests that compliant crawlers respect it, and should never be relied on to hide sensitive content.

<a id="how-does-semantic-html-and-heading-structure-impact-seo"></a>
### Q: How does semantic HTML and heading structure impact SEO?
**Answer:** Search engines use heading hierarchy (`<h1>`–`<h6>`) and semantic elements to understand a page's topic and structure, which can influence ranking and how content is featured — e.g. in rich snippets. A single, descriptive `<h1>` and a logical heading order are considered SEO best practice.

<a id="what-is-structured-data-schemaorg-markup-and-why-is-it-used"></a>
### Q: What is structured data / Schema.org markup, and why is it used?
**Answer:** Structured data — often added as JSON-LD in a `<script type="application/ld+json">` block — explicitly labels page content (recipes, products, reviews, events) using a shared vocabulary (Schema.org) that search engines can parse to generate rich results, like star ratings or recipe times shown directly in search listings.

<a id="what-is-the-difference-between-nofollow-and-noindex"></a>
### Q: What is the difference between "nofollow" and "noindex"?
**Answer:** `rel="nofollow"` on a link tells search engines not to pass ranking credit through that specific link. `<meta name="robots" content="noindex">` on a page tells search engines not to include that page in search results at all — different scopes, a link vs. an entire page.

<a id="why-does-page-load-speed-matter-for-seo"></a>
### Q: Why does page load speed matter for SEO?
**Answer:** Search engines factor page speed and user experience metrics (Core Web Vitals) into ranking, since slow pages correlate with poor user experience and higher bounce rates. This ties back to HTML-level practices like lazy-loading images, minimizing render-blocking scripts, and reserving image dimensions to reduce layout shift.

<a id="what-is-the-significance-of-using-descriptive-keyword-relevant-urls"></a>
### Q: What is the significance of using descriptive, keyword-relevant URLs?
**Answer:** Clean, readable URLs (e.g. `/blog/html-interview-questions` rather than `/page?id=1234`) are easier for both users and search engines to understand at a glance, and offer a modest ranking benefit — though content quality and relevance matter far more than URL structure alone.

---

<a id="performance-best-practices"></a>
## Performance & Best Practices

<a id="how-do-image-widthheight-attributes-affect-performance"></a>
### Q: How do image width/height attributes affect performance?
**Answer:** Specifying `width` and `height` on `<img>` lets the browser reserve the correct space in the layout before the image finishes loading, preventing content from jumping around as images load in — directly improving the Cumulative Layout Shift (CLS) Core Web Vital.

<a id="what-is-render-blocking-content-and-how-do-you-minimize-it"></a>
### Q: What is render-blocking content, and how do you minimize it?
**Answer:** Resources like synchronous `<script>` tags or `<link rel="stylesheet">` in `<head>` can block the browser from rendering the page until they're downloaded and processed. Minimize this by deferring non-critical scripts (`defer`/`async`), inlining critical CSS, and loading non-critical CSS asynchronously.

<a id="what-is-the-purpose-of-preload-prefetch-and-preconnect-resource-hints"></a>
### Q: What is the purpose of preload, prefetch, and preconnect resource hints?
**Answer:** `<link rel="preload">` fetches a critical resource (a font, a key image) early with high priority since it'll be needed soon. `<link rel="prefetch">` fetches a lower-priority resource likely needed for a future navigation. `<link rel="preconnect">` establishes an early connection to a third-party origin before an actual request to it is made, shaving off connection setup time.

<a id="how-does-minifying-htmlcssjs-improve-performance"></a>
### Q: How does minifying HTML/CSS/JS improve performance?
**Answer:** Minification strips whitespace, comments, and unnecessary characters (and can shorten variable names in JS/CSS) without changing functionality, reducing file size and download time — a simple, safe optimization typically automated by a build tool.

<a id="why-is-it-best-practice-to-avoid-deeply-nested-or-excessive-dom-elements"></a>
### Q: Why is it best practice to avoid deeply nested or excessive DOM elements?
**Answer:** A large, deeply nested DOM tree takes longer for the browser to parse, style, and lay out, and can slow down JavaScript operations that traverse or query it. Simpler, flatter markup generally renders and updates faster, and is easier for developers and assistive technology to reason about too.

<a id="what-is-the-difference-between-critical-rendering-path-optimization-and-lazy-loading"></a>
### Q: What is the difference between critical rendering path optimization and lazy loading?
**Answer:** Critical rendering path optimization focuses on getting the *initially visible* content to render as fast as possible — inlining critical CSS, deferring non-essential scripts. Lazy loading defers content that *isn't* immediately visible — below-the-fold images, off-screen components — until it's actually needed. They're complementary strategies targeting different parts of the page.

<a id="how-do-web-fonts-impact-performance-and-how-do-you-mitigate-the-impact"></a>
### Q: How do web fonts impact performance, and how do you mitigate the impact?
**Answer:** Custom web fonts (via `@font-face`) require an extra network request and, if not handled carefully, can cause a "flash of invisible text" while the font loads, or a "flash of unstyled text" when it swaps in. Mitigate this with `font-display: swap`, preloading the font file, and limiting the number of font weights/styles used.

<a id="what-is-the-impact-of-http2-on-htmlasset-delivery-compared-to-http11"></a>
### Q: What is the impact of HTTP/2 on HTML/asset delivery compared to HTTP/1.1?
**Answer:** HTTP/2 supports multiplexing — multiple requests and responses over a single connection simultaneously — removing the old practice of concatenating or bundling assets purely to reduce the number of HTTP requests, a common HTTP/1.1 workaround. It generally improves load performance for pages with many small assets.

<a id="what-is-accessibilitys-relationship-to-good-html-practices-overall"></a>
### Q: What is accessibility's relationship to good HTML practices overall?
**Answer:** Writing clean, semantic HTML — proper headings, labeled forms, meaningful alt text, keyboard-operable interactive elements — tends to naturally satisfy most core accessibility requirements. Accessibility isn't a separate add-on step so much as a natural consequence of following HTML best practices correctly in the first place.

<a id="what-tools-would-you-use-to-audit-an-html-pages-performance-and-accessibility"></a>
### Q: What tools would you use to audit an HTML page's performance and accessibility?
**Answer:** Browser DevTools' Lighthouse panel audits performance, accessibility, SEO, and best practices in one report. Other common tools: WebPageTest for detailed performance waterfalls, axe DevTools or WAVE specifically for accessibility issues, and the browser's Network/Performance tabs for granular loading analysis.

---

<a id="behavioral-scenario-based-questions"></a>
## Behavioral / Scenario-Based Questions

<a id="how-would-you-make-an-existing-non-semantic-html-page-more-accessible-without-a-full-rewrite"></a>
### Q: How would you make an existing non-semantic HTML page more accessible without a full rewrite?
**Answer:** Start with the highest-impact, lowest-effort fixes: add missing `alt` text to images, ensure form inputs have associated `<label>`s, fix heading hierarchy, add a "skip to content" link, and verify keyboard navigation works. Swap the most structurally important generic `<div>`s (main content, nav, header/footer) for their semantic equivalents where it's safe to do so without breaking existing CSS/JS selectors.

<a id="how-would-you-debug-a-page-that-looks-broken-only-in-one-specific-browser"></a>
### Q: How would you debug a page that looks broken only in one specific browser?
**Answer:** Check for browser-specific rendering quirks (vendor-prefixed CSS, quirks mode from a missing DOCTYPE), inspect the DOM in that browser's DevTools to see how it actually parsed the markup, check for unsupported HTML5 features in that browser version, and validate the markup (e.g. with the W3C Markup Validator) to catch invalid HTML a more forgiving browser might silently "fix" differently.

<a id="how-would-you-decide-whether-to-use-a-semantic-element-or-aria-roles-for-a-custom-widget"></a>
### Q: How would you decide whether to use a semantic element or ARIA roles for a custom widget?
**Answer:** Always prefer a native semantic HTML element first (e.g. `<button>` over a styled `<div>`) since it comes with built-in keyboard support, focus handling, and accessible semantics for free. Reach for ARIA only when you genuinely need a custom widget with no native HTML equivalent — and even then, you must still manually replicate all the keyboard/focus behavior ARIA alone doesn't provide.

<a id="a-pages-largest-contentful-paint-lcp-is-slow-where-would-you-look-first-in-the-html"></a>
### Q: A page's Largest Contentful Paint (LCP) is slow — where would you look first in the HTML?
**Answer:** Check whether the LCP element (often a hero image or heading) is being lazy-loaded when it shouldn't be (it should load eagerly since it's above the fold), whether its dimensions are specified to avoid layout shift, whether render-blocking scripts or styles are delaying it, and whether a `preload` hint could fetch it earlier.

<a id="how-would-you-structure-a-forms-html-to-work-well-for-both-sighted-and-screen-reader-users"></a>
### Q: How would you structure a form's HTML to work well for both sighted and screen-reader users?
**Answer:** Use a real `<label>` for every input (not just a placeholder), group related fields with `<fieldset>`/`<legend>`, mark required fields with the `required` attribute rather than only a visual asterisk, and use `aria-describedby` to associate validation error messages directly with their input so screen readers announce them.

<a id="how-would-you-handle-serving-different-images-for-different-device-sizes-and-pixel-densities"></a>
### Q: How would you handle serving different images for different device sizes and pixel densities?
**Answer:** Use `srcset`/`sizes` on `<img>` for resolution switching — same image, different sizes based on viewport or density — and `<picture>` with multiple `<source>` elements when you need genuinely different crops (art direction) or modern formats like WebP/AVIF with a fallback.

<a id="what-would-you-check-first-if-a-form-isnt-submitting-data-correctly-to-the-server"></a>
### Q: What would you check first if a form isn't submitting data correctly to the server?
**Answer:** Verify each input has a `name` attribute (data without a `name` isn't included in the submission), check the form's `method`/`action` match what the server expects, confirm `enctype="multipart/form-data"` is set if uploading files, and check whether a submit button's `type` was left as the default `submit` where it shouldn't have been.

<a id="how-would-you-approach-reviewing-a-teammates-html-in-a-pull-request"></a>
### Q: How would you approach reviewing a teammate's HTML in a pull request?
**Answer:** Check for semantic correctness (right element for the right purpose), a logical, unskipped heading hierarchy, meaningful `alt` text on images, properly labeled form controls, valid nesting (no block elements inside inline ones), and whether interactive elements are actually reachable and operable via keyboard.

---

<a id="how-to-use-this-guide"></a>
## How to Use This Guide

- **A few days before an interview?** Go section by section, top to bottom — each one builds on the last, from basics to performance/SEO.
- **Revising the night before?** Jump straight to 🔥 Most Asked / Tricky Questions, then skim section headers for anything you're unsure about.
- **During quick revision:** Use `Ctrl+F` (or `Cmd+F`) to jump straight to a keyword or topic instead of scrolling.
- **After every interview:** Come back and add any question you got asked that isn't already here — this file is meant to grow with you.

Good luck — you've got this. 🚀
