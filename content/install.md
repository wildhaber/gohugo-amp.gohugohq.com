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

An extended [theme documentation](https://gohugo-amp.gohugohq.com) at [gohugo-amp.gohugohq.com](https://gohugo-amp.gohugohq.com). For more information about the theme installation read the official [setup guide](https://gohugo.io/overview/installing/) of Hugo.

## Configuration

After installing the theme successfully, we recommend you to take a look at the [demo website](https://gohugo-amp.gohugohq.com). You find extensive documentation and a demonstration of all shortcodes and partials there.

For some features, you need to add configuration to your base `config.toml` params section:

```toml
[params]
    amp = true # enables amp features
    ampCdnRoot = "https://cdn.ampproject.org/" # defined base cdn root of the amp projects files
    ampRelease = "v0" # define amp release you want to use
    ampElementsVersion = "0.1" # define amp-elements version you want to use
    
    # define which amp-elements you are using globally, these elements will be included in every page
    ampElements = ["amp-accordion","amp-ad","amp-analytics","amp-carousel","amp-iframe","amp-app-banner","amp-dynamic-css-classes","amp-form","amp-fx-flying-carpet","amp-image-lightbox","amp-lightbox","amp-sidebar","amp-social-share","amp-sticky-ad","amp-user-notification"]

    themeColor = "#112233" # define a theme color (this will colorize the android address-bar)

    adsensePublisher = "ca-pub-123456789" # required if you want to include google adsense
    googleAnalytics = "UA-123456-78" # required if you want to use google analytics
    appleItunesApp = "app-id=123456789, app-argument=app-name://link/to/app-content" # required if you want to add an app banner with iOS app
    ampManifest = "/amp-manifest.json" # required if you want to add the app-banner feature
```


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

### Google Analytics

Beside of adding the googleAnalytics in your base `config.toml` you also need to define triggers. Simply add a file in your base data section `/data/analytics/triggers.json`. For example:

```json
{
  "trackPageview": {
    "on": "visible",
    "request": "pageview"
  },
  "trackEvent" : {
    "selector": "body",
    "on": "click",
    "request": "event",
    "vars": {
      "eventCategory": "body-click",
      "eventAction": "click"
    }
  }
}
```

Further information about AMP Analytics you will find in the [official documentation of the amp-project](https://www.ampproject.org/docs/reference/components/amp-analytics).

## App-Banners

App-Banners are very popular and help you to win your regular website's visitor downloading your app. Simply add a file in your base data section `/data/app/banner.json` for the configuration to display it in a mobile browser:

```json
{
  "id" : "app-banner-id",
  "src" : "https://placehold.it/60x51/ff3300/cccccc",
  "name" : "My Apps Name",
  "description" : "Short app description. Really short.",
  "openText" : "get the app"
}
```

Further information about AMP App-Banners you will find in the [official documentation of the amp-project](https://www.ampproject.org/docs/reference/components/amp-app-banner).

## Contributing

Have you found a bug or got an idea for a new feature? Feel free to use the [issue tracker](https://github.com/wildhaber/gohugo-amp/issues) to let me know. Alternatively, make a [pull request](https://github.com/wildhaber/gohugo-amp/pulls) directly.

## License

gohugo-amp released under the [MIT License](https://github.com/wildhaber/gohugo-amp/blob/master/LICENSE).

## Thanks

Thanks to [Steve Francia](https://github.com/spf13) for creating Hugo and the awesome community around the project.