---
layout: post
title: "About kramdown"
date: 2019-05-18
---
This quick post covers the extras provided by [kramdown](https://kramdown.gettalong.org/) (*not* capitalised!), in addition to [Markdown](https://daringfireball.net/projects/markdown/).

**kramdown** is a superset of Markdown. It does everything that Markdown does, plus some extras. The extras that are useful to me include:

## Pretty text

* `""` → "" (curly quotes)
* `''` → '' (curly quotes)
* `---` → --- (em-dash)
* `--` → -- (en-dash)

## Footnotes

This is a great way of keeping core text clear, and details accessible.

*Code:*
~~~
This is some text.[^1] Other text.[^footnote]
[^1]: Some footnote definition.
[^footnote]: Another footnote
~~~

*Output:*
This is some text.[^1] Other text.[^footnote]

[^1]: Some footnote definition.
[^footnote]: Another footnote

*Numbering is sequential and doesn't depend on the labels used in the code. The footnotes can go anywhere in the document.*

## Code blocks

* ...begun and ended with a line of several tilde `~` characters on their own:

*Code (using inline attribute list):*
`~~~`
~~~
def what?
  42
end
~~~
`{: .language-ruby}`
`~~~`

*Output:*
~~~
def what?
  42
end
~~~
{: .language-ruby}


*Output (using* `ruby` *after the initial tildes):*
~~~ ruby
def what?
  42
end
~~~

*Output (using* `html` *after the initial tildes):*
~~~ html
<html>
  <p>Hello, world</p>
</html>  
~~~

*Output (using* `css` *after the initial tildes):*
~~~ css
.center {
  text-align: center;
  color: red;
}
~~~


## Improved tables

*Code: EITHER*
~~~
|-----------------+------------+-----------------+----------------|
| Default aligned |Left aligned| Center aligned  | Right aligned  |
|-----------------|:-----------|:---------------:|---------------:|
| First body part |Second cell | Third cell      | fourth cell    |
| Second line     |foo         | **strong**      | baz            |
| Third line      |quux        | baz             | bar            |
|-----------------+------------+-----------------+----------------|
| Second body     |            |                 |                |
| 2 line          |            |                 |                |
|=================+============+=================+================|
| Footer row      |            |                 |                |
|-----------------+------------+-----------------+----------------|
~~~
*OR*
~~~
|---
| Default aligned | Left aligned | Center aligned | Right aligned
|-|:-|:-:|-:
| First body part | Second cell | Third cell | fourth cell
| Second line |foo | **strong** | baz
| Third line |quux | baz | bar
|---
| Second body
| 2 line
|===
| Footer row
~~~
*Output:*

|---
| Default aligned | Left aligned | Center aligned | Right aligned
|-|:-|:-:|-:
| First body part | Second cell | Third cell | fourth cell
| Second line |foo | **strong** | baz
| Third line |quux | baz | bar
|---
| Second body
| 2 line
|===
| Footer row

## Math blocks

I don't use them, but they're rather wonderful!

It turns out that while kramdown supports Mathjax, you do need to [call the relevant Javascript](https://quuxplusone.github.io/blog/2018/08/05/mathjax-in-jekyll/). I don't want to bog down this website just for one demo.
