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
```

Next, you need to build the theme's styling once: 

```
$ cd gohugo-amp
$ npm install
```

## Configuration

After installing the theme successfully, we recommend you to take a look at the [kitchen sink](/ktichen-sink/). You find extensive documentation and a demonstration of all shortcodes and partials there.

Read more about the `config.toml` in the [configuration example](/config/). You will find explanations how to setup [General AMP Configuration](/config/amp/), [Theme Appearance](/config/appearance/), using [AdSense](/config/adsense/), [Configure Analytics with custom Triggers](/config/analytics/) and [many things more](/config/).

### Styling

Because amp does not allow you to include CSS styles with the regular `link rel='stylesheet'`-tag we need to embed the CSS in the header section. Helping in this case, we provided a workflow that injects the output from `/src/styles.scss` in the header automatically for you. From this entry point, you can import your custom styling as you like.

Building the styles `gohugo-amp` provides the following `npm scripts` in the [package.json](build-process):

**building the styles once** (perfect for automatic deployments) - also included in the postinstall hook
```
$ npm run build
```

**generates the styles once**
```
$ npm run styles
```

**watching changes** - recommended while development
```
$ npm run styles:watch
```

Why we had to do this process you can read in the [official amp-project documentation](https://www.ampproject.org/docs/guides/responsive_amp).

Further information about AMP Analytics you will find in the [official documentation of the amp-project](https://www.ampproject.org/docs/reference/components/amp-analytics).

## Contributing

Have you found a bug or got an idea for a new feature? Feel free to use the [issue tracker](https://github.com/wildhaber/gohugo-amp/issues) to let me know. Alternatively, make a [pull request](https://github.com/wildhaber/gohugo-amp/pulls) directly.

## License

gohugo-amp released under the [MIT License](https://github.com/wildhaber/gohugo-amp/blob/master/LICENSE).

## Thanks

Thanks to [Steve Francia](https://github.com/spf13) for creating Hugo and the awesome community around the project.