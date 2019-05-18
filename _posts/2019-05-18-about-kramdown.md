---
layout: post
title: "About kramdown"
date: 2019-05-18
---
This quick post covers the extras provided by [kramdown](https://kramdown.gettalong.org/) (*not* capitalised!), in addition to [Markdown](https://daringfireball.net/projects/markdown/).

**kramdown** is a superset of Markdown. It does everything that Markdown does, plus some extras. The extras that are useful to me include:

* Code blocks, begun and ended with a line of several tilde `~` characters on their own:

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

* Improved tables

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
