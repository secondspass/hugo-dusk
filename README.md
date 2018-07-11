Simple minimalistic dark theme for [Hugo](https://gohugo.io/). Modified to my preference.

![screenshot](https://github.com/secondspass/hugo-dusk/blob/master/images/tn.png "screenshot")

## Features

* Responsive minimalistic design
* Configurable theme colors
* Syntax highlight with builtin [Chroma](http://gohugo.io/content-management/syntax-highlighting/)
* [OpenGraph](http://ogp.me/), [Twitter cards](https://dev.twitter.com/cards/overview) support
* Configurable pagination for posts
* KaTeX included (for use with mmark)
* Lazy menu
* Custom 404 page

## Installation

~~~sh
$ mkdir themes
$ cd themes
$ git clone https://github.com/secondspass/hugo-dusk
~~~

## Configuration

Example configuration:

~~~~toml
baseurl = "/"
title = "My site."
copyright = "Copyright (c) 2017, all rights reserved."
canonifyurls = true
languageCode = "en-US"
paginate = 3
theme = "hugo-dusk"

# use Chroma for syntax highlight
pygmentsStyle = "native" # other dark style options: vim, fruity, monokai
# enable syntax highlight for code blocks
pygmentsCodeFences = true

[author]
  name = ""


[[menu.main]]
  name = "Posts"
  weight = -120
  identifier = "posts"
  url = "/posts/"

[[menu.main]]
  name = "Tags"
  weight = -110
  identifier = "tag"
  url = "/tags/"

[params.meta]
  keywords = "blog, tech"
  description = "Personal blog."

[params]
  github = "github id"
  twitter = "twitter id"

[params.colors]
  # hugo-dusk colors
  background = "#101010" # background color for the site
  main = "#99cc66"
  text = "#dbdbdb"
  code-quote-bg = "#1D1F21" # background color for quotes and code blocks
  copyright = "#404040" # copyright text color
~~~~
