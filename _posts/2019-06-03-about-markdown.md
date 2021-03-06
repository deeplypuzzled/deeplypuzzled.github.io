---
layout: post
title: "About Markdown"
author: "JSG"
date: 2019-06-03
underconstruction: 'no'
---
Markdown is a simple set of markup (ho-ho) codes. Added to plain text, these codes cue processing to implement HTML formatting of the text. The codes are designed to be easy to write, and to read. Processing is handled by Markdown's Perl software.

This post describes the features of [Markdown](https://daringfireball.net/projects/markdown/) *that I use*, including on this website. For full details, see sources, below. I have left out obscure and little-used (by me) features, and other ways of doing the same thing -- that's what the docs are for! Examples are included.

**NOTE:** The look of this page and its examples will change, depending on the template and/or CSS used to display it.

## Basics

Separate paragraphs with a blank line. For a line break within a paragraph, use two spaces or two backslashes at the end of a line. *No spaces/backslashes: no line break.*

HTML can be used freely alongside Markdown and plain text.

## Headers

Simple: use hashes (`#`) -- one `#` for a top-level `<H1>` header, to six `######` for `<H6>`. Headers *must* be preceded by a blank line, except at the top of the page.

###### Example: this is a lowest-level, H6 header; more examples below

## Emphasis

For italics (light emphasis), use a single asterisk or underscore at start and end; for bold (strong emphasis), use two asterisks or underscores.

Examples:
* `*italic*` &#8594; *italic*
* `**bold**` &#8594; **bold**
* `***bold italics***` &#8594; ***bold italics***

(BTW, underlining isn't part of Markdown, but can be implemented using inline CSS:\\`<span style="text-decoration:underline">underlined</span>`  &#8594; <span style="text-decoration:underline">underlined</span>.)

## Links

*Code:* `[A link to my website](https://www.gibbs.at)` &#8594; [A link to my website](https://www.gibbs.at)

## Pictures

*Code:* `![Kitten](/assets/images/kitten-550x825.jpg "A kitten")` *(alt text in square brackets, title after URL)*
![Kitten](/assets/images/kitten-550x825.jpg "A kitten")

kramdown allows attributes to be appended:

![Kitten](/assets/images/kitten-550x825.jpg "A kitten"){: width="100" height="150" style="float:right; padding:16px"}
*Code:* `![Kitten](/assets/images/kitten-550x825.jpg "A kitten"){: width="100" height="150" style="float:right; padding:16px"}`

<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>

## Blockquotes (and code blocks)

Start a line with `>` (and optional space). Every following line that starts with `>` is included in that blockquote. Multiple `>`s are nested.

*Code:*
~~~~
> A sample blockquote.
>
> >Nested blockquotes are
> >also possible.
>
> #### Headers work too
> This is the outer quote again.
~~~~

(That was a code block, BTW, with a row of a few tildes (`~~~`) above and below it. Highlighted code is also possible, by specifying a language abbreviation at the end of the first row of tildes, e.g. `~~~ html`.)

> A sample blockquote.
>
> >Nested blockquotes are
> >also possible.
>
> #### Headers work too
> This is the outer quote again.

### Inline code

You can also have `inline code` within normal text. Enclose code in \` (backticks/left single inverted commas).

## Horizontal rules

Use three or more asterisks, dashes or underscores (on their own). Formatting of the rule depends on the CSS for the page. \\
*Code:* \\
`***`

***

## Lists

Either number each line, with a period after the number, or (for bullets) use an asterisk and a space. Lists can be nested by indenting with spaces or tabs.

1. One
2. Two
3. Three

* Alpha
* Bravo
* Charlie

## Footnotes

*Code:*
~~~~
Here is some text with a footnote.[^1]

[^1]: This is the footnote, with a link back to the text.
~~~~

Here is some text with a footnote.[^1]

[^1]: This is the footnote, with a link back to the text.

## Simple tables

*Code:*
~~~~
| Header1 | Header2 | Header3 |
|:--------|:-------:|--------:|
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|----
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|=====
| Foot1   | Foot2   | Foot3
{: rules="groups"}
~~~~

| Header1 | Header2 | Header3 |
|:--------|:-------:|--------:|
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|----
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|=====
| Foot1   | Foot2   | Foot3
{: rules="groups"}

# More examples

## Headers

(The two headings above are H1 and H2, respectively.)

### Header 3

#### Header 4

##### Header 5

###### Header 6

## Crib sheets and sources

* [Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* [*Learning Markdown*](https://www.markdownguide.org/)
* [Markdown home page](https://daringfireball.net/projects/markdown/).
