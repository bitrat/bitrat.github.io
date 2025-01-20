---
title: Basic HTML Elements
description: Example test article that contains basic HTML elements for text formatting on the Web.
date: 2018-04-16
categories:
  - "Development"
tags:
  - "Access Support"
  - "Android Tips"
  - "Apple Tips"
  - "Automation"
  - "Cloud"
  - "AWS"
  - "Azure"
  - "Databases"
  - "Amazon Aurora"
  - "Amazon RDS"
  - "MSSQL Server"
  - "PostGreSQL"
  - "Dynamo DB"
  - "Networking"
  - "Small Business - NZ"
  - "Software Development"
  - "Git"
  - "C#"
  - "Python"
categories:
  - "Consulting"
  - "Technical"
#menu: main # Optional, add page to a menu. Options: main, side, footer
draft: true
---

The main purpose of this article is to make sure that all basic HTML Elements are decorated with CSS so as to not miss any possible elements when creating new themes for Hugo.
<!--more-->

## Headings

Let's start with all possible headings. The HTML `<h1>`—`<h6>` elements represent six levels of section headings. `<h1>` is the highest section level and `<h6>` is the lowest.

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

***

## Paragraph

According to the [HTML5 specification](https://www.w3.org/TR/html5/dom.html#elements) by [W3C](https://www.w3.org/), **HTML documents consist of a tree of elements and text**. Each element is denoted in the source by a [start tag](https://www.w3.org/TR/html5/syntax.html#syntax-start-tags), such as `<body>`, and an [end tag](https://www.w3.org/TR/html5/syntax.html#syntax-end-tags), such as `</body>`. (*Certain start tags and end tags can in certain cases be omitted and are implied by other tags.*)

Elements can have attributes, which control how the elements work. For example, hyperlink are formed using the `a` element and its `href` attribute.

## List Types

### Ordered List

1. First item
2. Second item
3. Third item

### Unordered List

* List item
* Another item
* And another item

### Nested list
* First item - alright!
* Second item
    * Second item First subitem
    * Second item second subitem
        * Second item Second subitem First sub-subitem
        * Second item Second subitem Second sub-subitem
        * Second item Second subitem Third sub-subitem
    * Second item Third subitem
        * Second item Third subitem First sub-subitem
        * Second item Third subitem Second sub-subitem
* Third item

### Definition List

HTML also supports definition lists.

Blanco tequila
: The purest form of the blue agave spirit...
Reposado tequila
: Typically aged in wooden barrels for between two and eleven months...

## Blockquotes

The blockquote element represents content that is quoted from another source, optionally with a citation which must be within a `footer` or `cite` element, and optionally with in-line changes such as annotations and abbreviations.

> Quoted text.
> This line is part of the same quote.
> Also you can *put* **Markdown** into a blockquote.

Blockquote with a citation.

> My goal wasn't to make a ton of money. It was to build good computers. I only started the company when I realized I could be an engineer forever.
> -- <cite>Steve Wozniak[1]</cite>
[1]: https://www.brainyquote.com/quotes/steve_wozniak_589494

> According to Mozilla's website, <cite>"Firefox 1.0 was released in 2004 and became a big success".[2]</cite>
[2]: https://www.mozilla.org/en-US/about/history/details/

## Tables

Tables aren't part of the core Markdown spec, but Hugo supports them.

| ID  | Make      | Model   | Year |
| --- | --------- | ------- | ---- |
| 1   | Honda     | Accord  | 2009 |
| 2   | Toyota    | Camry   | 2012 |
| 3   | Hyundai   | Elantra | 2010 |

Colons can be used to align columns.

| Tables      | Are           | Cool         |
|:----------- |:-------------:| ------------:|
| align: left | align: center | align: right |
| align: left | align: center | align: right |
| align: left | align: center | align: right |

You can also use inline Markdown.

| Inline     | Markdown  | In                | Table      |
| ---------- | --------- | ----------------- | ---------- |
| *italics*  | **bold**  | ~~strikethrough~~ | `code`     |

## Code

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```

{{< highlight html >}}
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

## Other stuff doesn't work as expected — abbr, sub, sup, kbd, etc.

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

Subscripts  
H<sub>2</sub>O

C~6~H~12~O~6~

Superscript  
X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd>X</kbd> to win. Or press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>F</kbd></kbd> to show FPS counter.

<mark>As a unit of information in information theory, the bit has alternatively been called a shannon</mark>, named after Claude Shannon, the founder of field of information theory.
