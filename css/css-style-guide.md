# CSS style guide

## 1. Background

_**This document defines formatting and style rules. It aims at improving collaboration, code quality, and enabling supporting infrastructure. It applies to raw working files that use HTML and CSS. Tools are free to obfuscate, minify, and compile as long as the general code quality is maintained.**_

## 2. CSS Formatting Rules

- ## Protocol
  _**Always use HTTPS (https:) for images and other media files, style sheets, and scripts, unless the respective files are not available over HTTPS.**_

```css
/* Not recommended: uses HTTP */
@import 'http://fonts.googleapis.com/css?family=Open+Sans';

/* Not recommended: omits the protocol */
@import '//fonts.googleapis.com/css?family=Open+Sans';

/* Recommended */
@import 'https://fonts.googleapis.com/css?family=Open+Sans';
```

- ## Indentation
  _**Indentation: Indent by 2 spaces at a time, Don’t use tabs or mix tabs and spaces for indentation.**_

```css
.example {
  color: yellow;
}
```

- ## Capitalization
  _**All code has to be lowercase: this applies to CSS selectors, properties, and property values**_

```css
/* Not recommended */
color: #e5e5e5;

/* Recommended */
color: #e5e5e5;
```

- ## Class Name separator
  _**Separate words in class names by a hyphen,Do not concatenate words and abbreviations in selectors by any characters other than hyphens**_

```css
/* Not recommended*/
.studentimage {
}

/* Not recommended: uses underscore instead of hyphen */
.student_icon {
}

/* Recommended */
.student-image {
}
.student-icon {
}
```

- ## Shorthand Properties
  _**Use shorthand properties where possible,CSS offers a variety of shorthand properties (like font) that should be used whenever possible, even in cases where only one value is explicitly set.Using shorthand properties is useful for code efficiency and understandability.**_

```css
/* Not recommended*/
border-top-style: none;
font-family: palatino, georgia, serif;
font-size: 100%;
line-height: 1.6;
padding-bottom: 4px;
padding-left: 2px;
padding-right: 2px;
padding-top: 0;

/* Recommended */
border-top: 0;
font:
  100%/1.6 palatino,
  georgia,
  serif;
padding: 0 2px 4px;
```

- ## 0 and Units
  _**Omit unit specification after “0” values, unless required.**_

```css
/* Not recommended*/
padding: 0px;
margin: 0em;

/* Recommended */
padding: 0;
margin: 0;
```

- ## Declaration Stop
  _**Use a semicolon after every declaration for consistency and extensibility reasons.**_

```css
/* Not recommended */
.male {
  width: 50px;
  height: 50px;
}

/* Recommended */
.male {
  width: 50px;
  height: 50px;
}
```

- ## Property Name Stops
  _**Use a space after a property name’s colon (but no space between property and colon) for consistency reasons**_

```css
/* Not recommended */
.male {
  width: 50px;
  height: 50px;
}

/* Recommended */
.male {
  width: 50px;
  height: 50px;
}
```

- ## Block Separation
  _**Always use a single space between the last selector and the opening brace that begins the declaration block,The opening brace should be on the same line as the last selector in a given rule**_

```css
/* Not recommended: missing space */
.gender {
  margin: 1em;
}

/* Not recommended: unnecessary line break */
.gender {
  margin: 1em;
}

/* Recommended */
.gender {
  margin: 1em;
}
```

- ## Selector and Declaration Separation
  _**Separate selectors and declarations by new lines.**_

```css
/* Not recommended */
h1,
h2,
h3 {
  font-weight: small;
}

/* Recommended */
h1,
h2,
h3 {
  font-weight: small;
  line-height: 1.2;
}
```

- ## Comments (optional)
  _**Use comments to explain code: What does it cover, what purpose does it serve, why is respective solution used or preferred?**_
