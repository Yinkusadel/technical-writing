# Html style guide

## 1. Background

_**This document defines formatting and style rules. It aims at improving collaboration, code quality, and enabling supporting infrastructure. It applies to raw, working files that use HTML and CSS. Tools are free to obfuscate, minify, and compile as long as the general code quality is maintained.**_

## 2. HTML Formatting Rules

- ## Indentation
  _**Indent by 2 spaces at a time, Don’t use tabs or mix tabs and spaces for indentation.**_

```html
<ul>
  <li>Adeleye</li>
  <li>Ibrohim</li>
</ul>
```

- ## Capitalization
  _**Use only lowercase: All code has to be lowercase this applies to HTML element names, attributes, attribute values (unless text/CDATA)**_

```html
<!-- Not recommended -->
<a href="/">Home</a>

<!-- recommended -->
<a href="/">Home</a>
```

- ## Trailing Whitespace
  _**Remove trailing white spaces:Trailing white spaces are unnecessary and can complicate diffs.**_

```html
<!-- Not recommended -->
<p>want?_</p>

<!-- Recommended -->
<p>Yes thanks.</p>
```

- ## Encoding

  _**Make sure your editor uses UTF-8 as character encoding,Specify the encoding in HTML templates and documents via `<meta charset="utf-8">`**_

- ## Comments (optional)

  _**Use comments to explain code: What does it cover, what purpose does it serve, why is respective solution used or preferred?**_

- ## Semantics
  _**Use elements for what they have been created for. For example, use heading elements for headings, p elements for paragraphs, a elements for anchors, etc**_

```html
<!-- Not recommended -->
<div>1. orange</div>
<div>2. apple</div>

<!-- Recommended -->
<ol>
  <li>orange</li>
  <li>apple</li>
</ol>
```

- ## Multimedia
  _**Provide alternative contents for multimedia such as images, videos, animated objects.Providing alternative contents is important for accessibility reasons: A blind user has few cues to tell what an image is about without alt, and other users may have no way of understanding what video or audio contents are about either.**_

```html
<!-- Not recommended -->
<img src="chairs.png" />

<!-- Recommended -->
<img src="spreadsheet.png" alt="chairs screenshot." />
```

- ## New line
  _**Use a new line for every block, list, or table element, and indent every such child element.**_

```html
<table>
  <tr>
    <th>Company</th>
    <th>sensei</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>mini techcypher</td>
    <td>my uncle</td>
    <td>Anime world</td>
  </tr>
</table>
```

- ## Quotation Marks
  _**When quoting attributes values, use double quotation ( "" ) marks rather than single quotation marks ( '' )**_

```html
<!-- Not recommended -->
<div class="gender">male</div>

<!-- Recommended -->
<div class="gender">male</div>
```

- ## Comments (optional)

  _**Use comments to explain code: What does it cover, what purpose does it serve, why is respective solution used or preferred?**_

### Credit and Acknowledgement to [google style guide](https://google.github.io/styleguide/htmlcssguide.html)
