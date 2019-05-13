---
layout: default
title: Guide to Markdown and kramdown
---
# Guide to Markdown and kramdown

This page is a quick reference to Markdown and kramdown. I have put *my* most-used features at the top, with more-complex elements lower down. I have left out obscure and little-used (by me) features, and other ways of doing the same thing -- that's what the docs are for! Examples are included.

**NOTE:** The look of this page and its examples will change, depending on the template and/or CSS used to display it.

## Basics

Separate paragraphs with a blank line. For a line break within a paragraph, use two spaces or two backslashes at the end of a line. No spaces/backslashes, no line break.

## Headers

Simple: use hashes (\#) -- one \# for a top-level H1 header, to six \###### for H6. Headers *must* be preceded by a blank line, except at the top of the page.

###### Example: this is a lowest-level, H6 header; more examples below

## Emphasis

For italics (light emphasis), use a single asterisk or underscore at start and end; for bold (strong emphasis), use two asterisks or underscores. 

Examples:
* `*italic*` &#8594; *italic* 
* `**bold**` &#8594; **bold**
* `***bold italics***` &#8594; ***bold italics***

(BTW, underlining isn't part of Markdown, but can be implemented using inline CSS: `<span style="text-decoration:underline">underlined</span>`  &#8594; <span style="text-decoration:underline">underlined</span>.)

## Links

`[A link to my website](https://www.gibbs.at)` &#8594; [A link to my website](https://www.gibbs.at)

## Blockquotes (and code blocks)

Start a line with `>` (and optional space). Every following line that starts with `>` is included in that blockquote. Multiple `>`s are nested.

~~~~
> A sample blockquote.
>
> >Nested blockquotes are
> >also possible.
>
> ## Headers work too
> This is the outer quote again.
~~~~

(That was a code block, BTW, with a row of a few tildes (~) above and below it. Highlighted code is also possible, by specifying a language abbreviation after the first row of tildes.)

> A sample blockquote.
>
> >Nested blockquotes are
> >also possible.
>
> ## Headers work too
> This is the outer quote again.

## Horizontal rules

Use three or more asterisks, dashes or underscores (on their own).

***

## Lists

Either number each line, with a period after the number, or use an asterisk and a space. Lists can be nested by indenting with spaces or tabs.

1. One
2. Two
3. Three

* Alpha
* Bravo
* Charlie

## Footnotes

~~~~
Here is some text with a footnote.[^1]

[^1]: This is the footnote, with a link back to the text.
~~~~

Here is some text with a footnote.[^1]

[^1]: This is the footnote, with a link back to the text.

## Abbreviations (a bit obscure?)

If abbreviations are defined once, they apply to all instances on the page, so the definitions can be done last. Possibly an \_include could be used to make tthem global?

`*[HTML]: Hyper Text Markup Language` The word HTML should have a dotted underline; now hover the cursor over it.
*[HTML]: Hyper Text Markup Language

## Tables (very simple)

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

## Variables

In each case, the variable is enclosed in double curly brackets, thus: \{\{ *variable_name* \}\}

* site &#8594; {{ site }}
* page &#8594; (the whole page)
* site.time &#8594; {{ site.time }}
* page.title &#8594; {{ page.title }}
* page.url &#8594; {{ page.url }}
* page.path &#8594; {{ page.path }}
* page.dir &#8594; {{ page.dir }}

### Variables used for blog pages

* paginator &#8594; {{ paginator }}
* site.pages &#8594; (404)
* site.related_posts &#8594; {{ site.related_posts }}
* site.static_files &#8594; {{ site.static_files }}
* page.date &#8594; {{ page.date }}
* page.id &#8594; {{ page.id }}
* page.next &#8594; {{ page.next }}

# More examples

## Headers

(The two headings above are H1 and H2, respectively.)

### Header 3

#### Header 4

##### Header 5

###### Header 6

v8.7
