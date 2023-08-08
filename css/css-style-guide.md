# Html style guide
## 1. Background
_**This document defines formatting and style rules. It aims at improving collaboration, code quality, and enabling supporting infrastructure. It applies to raw working files that use HTML and CSS. Tools are free to obfuscate, minify, and compile as long as the general code quality is maintained.**_

## 2. Protocol
_**Always use HTTPS (https:) for images and other media files, style sheets, and scripts, unless the respective files are not available over HTTPS.**_
```css
/* Not recommended: uses HTTP */
@import 'http://fonts.googleapis.com/css?family=Open+Sans';

/* Not recommended: omits the protocol */
@import '//fonts.googleapis.com/css?family=Open+Sans';

/* Recommended */
@import 'https://fonts.googleapis.com/css?family=Open+Sans';
```

## 3. General Formatting Rules
_**Indentation: Indent by 2 spaces at a time, Don’t use tabs or mix tabs and spaces for indentation.**_
```css
.example {
  color: yellow;
}
```