---
layout: post
title: "About kramdown"
date: 2019-05-18
---
This quick post covers the extras provided by [kramdown](https://kramdown.gettalong.org/) (*not* capitalised!), in addition to [Markdown](https://daringfireball.net/projects/markdown/).

**kramdown** is a superset of Markdown. It does everything that Markdown does, plus some extras. The extras that are useful to me include:

* Code blocks, begun and ended with a line of several tilde `~` characters on their own:

*Code:*
`~~~`
~~~
def what?
  42
end
~~~
`{: .language-ruby}`
`~~~`

~~~
def what?
  42
end
~~~
{: .language-ruby}
