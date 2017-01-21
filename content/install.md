+++
date = "2016-10-16T19:28:41+02:00"
draft = false
title = "getting started"

[sitemap]
  changefreq = "weekly"
  priority = 1.0
  filename = "sitemap.xml"
  
+++

#  getting started with gohugo-amp

This Hugo theme is supposed to be a starter theme to make it easy to adapt to [Google's AMP-Project](https://www.ampproject.org/). Included in the theme are [**40+ shortcodes and partials**](/shortcodes/) making it a pleasure to embed AMP-Elements within your content files or your template.

## Installation

Go to the directory where you have your Hugo site and run:

```
$ mkdir themes
$ cd themes
$ git clone https://github.com/wildhaber/gohugo-amp.git
$ rm -rf gohugo-amp/.git
```

---

## [Configuration](/config/)

After installing the theme successfully, we recommend you to take a look at the [kitchen sink](/kitchen-sink/). You find extensive documentation and a demonstration of all shortcodes and partials there.

Read more about the `config.toml` in the [configuration example](/config/). You will find explanations how to setup [General AMP Configuration](/config/amp/), [Theme Appearance](/config/appearance/), using [AdSense](/config/adsense/), [Configure Analytics with custom Triggers](/config/analytics/) and [many things more](/config/).

---

## [Styling](/styling/)

AMP does not allow you to include CSS styles with the regular `link rel='stylesheet'`-tag we need to embed the CSS in the header section.

For this case add a file in your regular `layouts/partials/`-folder called `stylesheet.html`. In this file you can write pure CSS (no `<styles>`-Tags required) 

Since its not a cool idea have to write your stylesheets in an HTML-File we provide an automated process rendering your Sass output directly in this file. You can read more in our [Guide about Styling](https://gohugo-amp.gohugohq.com/styling/) in the documentation.

Why we had to do this process you can read in the [official amp-project documentation](https://www.ampproject.org/docs/guides/responsive_amp).
