---
layout: default
title: About
---
# About this website

This website was built using software and platforms provided by others. Here's a list of them, with the foundations at the bottom and the "higher" levels at the top. The aim is to demonstrate a 'clever' static HTML site.

At the time of writing, all these are open source and/or free versions of software and services. (Some of them offer paid versions with additional features.)
* [kramdown](https://kramdown.gettalong.org/), a superset of Markdown used for this website
* [Markdown](https://daringfireball.net/projects/markdown/), the simple coding for text to implement HTML formatting ([Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet); [*Learning Markdown*](https://www.markdownguide.org/))
* Some [HTML](https://www.w3schools.com/html) was required to create the basic structure...
* ...and so was some [CSS](https://www.w3schools.com/css/)
* (but most of the spadework was done by using a [Jekyll Theme](http://themes.jekyllrc.org); I cautiously chose to use one of the [GitHub Pages Supported Themes](https://pages.github.com/themes/))
* [Jekyll](https://jekyllrb.com]), which converts plain text (and Markdown/kramdown) to HTML ([cheatsheet](https://learn.cloudcannon.com/jekyll-cheat-sheet/)). This may be the most technical bit. _You can sorta-kinda get away with working in a browser, in the GitHub website, but you'll probably need to install the software and use the command line. GitHub appears to run a background process that updates .html/HTML from .md/Markdown in a minute or so after a commit._
* [Ruby](https://www.ruby-lang.org/en/), the software that drives Jekyll. Don't panic, there's no need to learn (in fact, almost no opportunity) to code.
* [GitHub Pages](https://pages.github.com/), the online documentation subset of GitHub
* [GitHub](https://github.com/), the online/cloud version of Git (acquired by [Microsoft](https://blogs.microsoft.com/blog/2018/10/26/microsoft-completes-github-acquisition/) in 2018); it now calls itself a "software development platform"
* [Git](https://git-scm.com/), the leading, unpretentious version control system

## *Not* all my own work...

I used these guides in setting this up:
* [*Creating and Hosting a Personal Site on GitHub*][creating], possibly the best one-page introduction to Jekyll-based website creation, by Jonathan McGlone
* [Jekyll's excellent documentation][jekyll]
* [A Jekyll "cheat sheet"][cheat]
* [*Get Started With GitHub Pages* by Anna Debenham][getstarted]
* [*A guide to using Github Pages* by Thinkful][guideghp]
* [GitHub's own help for GitHub Pages][ghphelp]
* [*Resources to learn Git*][ghpresources]
* I will be using images. GitHub Pages focuses on text, so I found this guide on [*How to Style Images With Markdown*][styleimages] particularly useful.

{::comment}
REFERENCE LINKS FOR "Not all my own work..."
{:/comment}
[creating]: http://jmcglone.com/guides/github-pages/
[jekyll]: https://jekyllrb.com/docs/
[cheat]: https://learn.cloudcannon.com/jekyll-cheat-sheet/
[getstarted]: https://24ways.org/2013/get-started-with-github-pages/
[guideghp]: https://www.thinkful.com/learn/a-guide-to-using-github-pages/
[ghphelp]: https://help.github.com/en/categories/github-pages-basics
[ghpresources]: https://try.github.io/
[styleimages]: https://www.xaprb.com/blog/how-to-style-images-with-markdown/

## Other moving parts

This is partly documented in the guides mentioned above, but the other components that make GitHub Pages and Jekyll work together include:
* The crucial `_layouts` folder and its `default.html`, which 'tops and tails' every web page; it is _included_ in/inherited by pretty much every page on the website...
* ...and the `post.html` file, which adds extras to the layout for blog posts (but keeps the `default.html` settings)
* There's also a `blog/index.html` file that lists all the blog posts...
* ...and a `blog/atom.xml`, which provides an RSS feed.
* Under the hood, `_config.yml` (with the core config options)...
* ...and `.gitignore` (which tells Git to ignore the `_site` folder, where the new pages are written every time Jekylll runs)
* The primary CSS in `css/main.css`
* The pages themselves, starting with `index.html` in the `master` branch, though most pages are .md/Markdown files, which Jekyll translates into .html/HTML
* I set up a custom domain at a very early stage.

In GitHub setup, there's a **gotcha**. As you will know if you have followed [Jonathan McGlone's (excellent) guide](creating), you can set up a custom domain name for your GitHub Pages site. I use [www.gibbs.at](https://www.gibbs.at) instead of (as well as) [deeplypuzzled.github.io](https://deeplypuzzled.github.io). You need some basic DNS for this, in your domain name setup. Start on the website of the domain registrar from which you bought (rented) the domain name. As I discovered by trial and error, [gibbs.at](https://gibbs.at) doesn't work. The `www` in front is not optional.

## TO-DO
* I haven't yet worked out whether there is any opportunity for (or point in) using Javascript...
* ...but I am [experimenting with Bootstrap](https://www.gibbs.at/bootstrap_test.html) with [Bootstrap](https://getbootstrap.com/) (**v4**) ([tutorial](https://www.w3schools.com/bootstrap4/default.asp)).
* I'm not using \_[includes](https://jekyllrb.com/docs/includes/) yet...
* CSS, though this might be overtaken by...
* ...setting up a non-default [theme](https://jekyllrb.com/docs/themes), not forgetting to [override](https://jekyllrb.com/docs/themes/#overriding-theme-defaults) defaults
* When/if the site is big enough, maybe I will add a `sitemap.xml` file, which would be autogenerated.
* Similarly, the `blog/index.html` file may need to be paginated later.
* Maybe I'll install Ruby and the Jekyll gem (etc) locally, later.
* Maybe I'll have a `development` branch later.

v5.1.1
