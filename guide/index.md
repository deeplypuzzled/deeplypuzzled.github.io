---
layout: default
title: Guide to Markdown and kramdown
---
# Guide to Markdown and kramdown

This page is a quick reference to Markdown and kramdown. I have put *my* most-used features at the top, with more-complex elements lower down. I have left out obscure and little-used (by me) features, and other ways of doing the same thing -- that's what the docs are for! Examples are included.

**NOTE:** The look of this page and its examples will change, depending on the template and/or CSS used to display it.

## Basics

Separate paragraphs with a blank line. For a line break within a paragraph, use two spaces or two backslashes at the end of a line. No spaces/backslashes, no line break.

## Headings

Simple: use hashes (\#) -- one \# for a top-level H1 heading, to six \###### for H6. Headings *must* be preceded by a blank line, except at the top of the page.

###### Example: this is a lowest-level, H6 heading

## Emphasis

For italics (light emphasis), use a single asterisk or underscore at start and end; for bold (strong emphasis), use two asterisks or underscores. 

Example: \*italic\* &#8594; *italic*; \*\*bold\*\* &#8594; **bold**; \*\*\*bold italics\*\*\* &#8594; ***bold italics***
(BTW, underlining isn't part of Markdown, but can be implemented using inline CSS: `<span style="text-decoration:underline">underlined</span>`  &#8594; <span style="text-decoration:underline">underlined</span>.)

# More examples

## Headings

(The two headings above are H1 and H2, respectively.)

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6
