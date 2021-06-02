---
title: "Sandbox"
date: 2021-06-02T13:53:44+09:00
draft: true
pager: false
sidebar: false
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

<ul>
  <li>First item</li>
  <li>Second item
    <ul>
      <li>Second item First subitem</li>
      <li>Second item second subitem
        <ul>
          <li>Second item Second subitem First sub-subitem</li>
          <li>Second item Second subitem Second sub-subitem</li>
          <li>Second item Second subitem Third sub-subitem</li>
        </ul>
      </li>
      <li>Second item Third subitem
        <ol>
          <li>Second item Third subitem First sub-subitem</li>
          <li>Second item Third subitem Second sub-subitem</li>
          <li>Second item Third subitem Third sub-subitem</li>
        </ol>
    </ul>
  </li>
  <li>Third item</li>
</ul>

### Definition List

HTML also supports definition lists.

<dl>
  <dt>Blanco tequila</dt>
  <dd>The purest form of the blue agave spirit...</dd>
  <dt>Reposado tequila</dt>
  <dd>Typically aged in wooden barrels for between two and eleven months...</dd>
</dl>

## Blockquotes

The blockquote element represents content that is quoted from another source, optionally with a citation which must be within a `footer` or `cite` element, and optionally with in-line changes such as annotations and abbreviations.

> Quoted text.
> This line is part of the same quote.
> Also you can *put* **Markdown** into a blockquote.

Blockquote with a citation.

<blockquote>
  <p>My goal wasn't to make a ton of money. It was to build good computers. I only started the company when I realized I could be an engineer forever.</p>
  <footer>— <cite>Steve Wozniak</cite></footer>
</blockquote>

According to Mozilla's website, <q cite="https://www.mozilla.org/en-US/about/history/details/">Firefox 1.0 was released in 2004 and became a big success.</q>

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

```html
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

## FontAwesome

- {{< fa fas exclamation>}} `< fa fas exclamation >`
- {{< fa fas exclamation-circle>}} `< fa fas exclamation-circle >`
- {{< fa fas exclamation-triangle>}} `< fa fas exclamation-triangle >`
- {{< fa fas times>}} `< fa fas times >`
- {{< fa fas times-circle>}} `< fa fas times-circle >`
- {{< fa fas check>}} `< fa fas check >`
- {{< fa fas check-square>}} `< fa fas check-square >`
- {{< fa far check-square>}} `< fa far check-square >`
- {{< fa fas check-circle>}} `< fa fas check-circle >`
- {{< fa far check-circle>}} `< fa far check-circle >`
- {{< fa fas user>}} `< fa fas user >`
- {{< fa fas users>}} `< fa fas users >`
- {{< fa fas users-cog>}} `< fa fas users-cog >`
- {{< fa fas user-tag>}} `< fa fas user-tag >`
- {{< fa fas user-plus>}} `< fa fas user-plus >`
- {{< fa fas user-minus>}} `< fa fas user-minus >`
- {{< fa fas user-edit>}} `< fa fas user-edit >`
- {{< fa fas user-cog>}} `< fa fas user-cog >`
- {{< fa fas user-check>}} `< fa fas user-check >`
- {{< fa fas user-clock>}} `< fa fas user-clock >`
- {{< fa fas user-circle>}} `< fa fas user-circle >`
- {{< fa far user-circle>}} `< fa far user-circle >`
- {{< fa fas angle-down>}} `< fa fas angle-down >`
- {{< fa fas angle-left>}} `< fa fas angle-left >`
- {{< fa fas angle-right>}} `< fa fas angle-right >`
- {{< fa fas angle-up>}} `< fa fas angle-up >`
- {{< fa fas arrow-circle-down>}} `< fa fas arrow-circle-down >`
- {{< fa fas arrow-circle-left>}} `< fa fas arrow-circle-left >`
- {{< fa fas arrow-circle-right>}} `< fa fas arrow-circle-right >`
- {{< fa fas arrow-circle-up>}} `< fa fas arrow-circle-up >`
- {{< fa fas arrow-down>}} `< fa fas arrow-down >`
- {{< fa fas arrow-left>}} `< fa fas arrow-left >`
- {{< fa fas arrow-right>}} `< fa fas arrow-right >`
- {{< fa fas arrow-up>}} `< fa fas arrow-up >`
- {{< fa fas arrows-alt-h>}} `< fa fas arrows-alt-h >`
- {{< fa fas arrows-alt-v>}} `< fa fas arrows-alt-v >`
- {{< fa fas bolt>}} `< fa fas bolt >`
- {{< fa fas bomb>}} `< fa fas bomb >`
- {{< fa fas bookmark>}} `< fa fas bookmark >`
- {{< fa far bookmark>}} `< fa far bookmark >`
- {{< fa fas calendar>}} `< fa fas calendar >`
- {{< fa fas calendar-alt>}} `< fa fas calendar-alt >`
- {{< fa fas calendar-check>}} `< fa fas calendar-check >`
- {{< fa fas circle>}} `< fa fas circle >`
- {{< fa far circle>}} `< fa far circle >`
- {{< fa fas cloud>}} `< fa fas cloud >`
- {{< fa fas code>}} `< fa far code >`
- {{< fa fas cog>}} `< fa fas cog >`
- {{< fa fas cogs>}} `< fa fas cogs >`
- {{< fa fas comment>}} `< fa fas comment >`
- {{< fa far comment>}} `< fa far comment >`
- {{< fa fas comment-alt>}} `< fa fas comment-alt >`
- {{< fa far comment-alt>}} `< fa far comment-alt >`
- {{< fa fas comment-dots>}} `< fa fas comment-dots >`
- {{< fa far comment-dots>}} `< fa far comment-dots >`
- {{< fa fas comments>}} `< fa fas comments >`
- {{< fa far comments>}} `< fa far comments >`
- {{< fa fas edit>}} `< fa fas edit >`
- {{< fa fas envelope>}} `< fa fas envelope >`
- {{< fa fas envelope-open>}} `< fa fas envelope-open >`
- {{< fa fas external-link-alt>}} `< fa fas external-link-alt >`
- {{< fa fas file>}} `< fa fas file >`
- {{< fa fas file-alt>}} `< fa fas file-alt >`
- {{< fa fas folder>}} `< fa fas folder >`
- {{< fa fas folder-open>}} `< fa fas folder-open >`
- {{< fa fas heart>}} `< fa fas heart >`
- {{< fa fas home>}} `< fa fas home >`
- {{< fa fas inbox>}} `< fa fas inbox >`
- {{< fa fas info>}} `< fa fas info >`
- {{< fa fas info-circle>}} `< fa fas info-circle >`
- {{< fa fas lightbulb>}} `< fa fas lightbulb >`
- {{< fa fas lock>}} `< fa fas lock >`
- {{< fa fab mastodon>}} `< fa fas mastodon >`
- {{< fa fas mobile>}} `< fa fas mobile >`
- {{< fa fas mobile-alt>}} `< fa fas mobile-alt >`
- {{< fa fas pen>}} `< fa fas pen >`
- {{< fa fas pen-fancy>}} `< fa fas pen-fancy >`
- {{< fa fas pencil-alt>}} `< fa fas pencil-alt >`
- {{< fa fas pen-square>}} `< fa fas pen-square >`
- {{< fa fas question-circle>}} `< fa fas question-circle >`
- {{< fa fas quote-left>}} `< fa fas quote-left >`
- {{< fa fas quote-right>}} `< fa fas quote-right >`
- {{< fa fas rss-square>}} `< fa fas rss-square >`
- {{< fa fas server>}} `< fa fas server >`
- {{< fa fas skull>}} `< fa fas skull >`
- {{< fa fas skull-crossbones>}} `< fa fas skull-crossbones >`
- {{< fa fas square>}} `< fa fas square >`
- {{< fa fas star>}} `< fa fas star >`
- {{< fa fas sticky-note>}} `< fa fas sticky-note >`
- {{< fa fas tablet>}} `< fa fas tablet >`
- {{< fa fas tag>}} `< fa fas tag >`
- {{< fa fas tags>}} `< fa fas tags >`
- {{< fa fas terminal>}} `< fa fas terminal >`
- {{< fa fas trash>}} `< fa fas trash >`
- {{< fa fab twitter>}} `< fa fas twitter >`
- {{< fa fab twitter-square>}} `< fa fas twitter-square >`
- {{< fa fas book>}} `< fa fas book >`
- {{< fa fas book-open>}} `< fa fas book-open >`


## Notice

{{% notice note %}}
{{< fa fas exclamation-circle co-note NOTE >}} Note
A notice disclaimer
{{% /notice %}}
  
{{% notice ok %}}
{{< fa fas exclamation-circle co-ok OK >}} OK
A notice disclaimer
{{% /notice %}}
  
{{% notice warn %}}
{{< fa fas exclamation-circle co-warn WARN >}} WARN
A notice disclaimer
{{% /notice %}}
  
{{% notice danger %}}
{{< fa fas exclamation-circle co-danger DANGER>}} DANGER
A notice disclaimer
{{% /notice %}}

## Other stuff — abbr, sub, sup, kbd, etc.

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

C<sub>6</sub>H<sub>12</sub>O<sub>6</sub>

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd>X</kbd> to win. Or press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>F</kbd></kbd> to show FPS counter.

<mark>As a unit of information in information theory, the bit has alternatively been called a shannon</mark>, named after Claude Shannon, the founder of field of information theory.
