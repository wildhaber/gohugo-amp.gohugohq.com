+++
date = "2016-11-18T19:28:41+02:00"
draft = false
title = "configuration - config.toml"

[sitemap]
  changefreq = "weekly"
  priority = 1.0
  filename = "sitemap.xml"
  
+++

# configuration

Configuration explained:

 - [AMP Configuration](/config/amp/) 

---
 
Example `config.toml`

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

    alternatePageName = "HUGO AMP" # alternative name for website structured data
    organisationLogo = "https://gohugohq.com/logo.png" # set organisation logo for structured data
    organisationName = "gohugohq.com" # set organisation name
    organisationAddress = "Some Street 123, 12345 City" # set organisation address

    socialProfiles = ["http://www.facebook.com/your-profile","http://instagram.com/yourProfile","http://www.linkedin.com/in/yourprofile","http://plus.google.com/your_profile"]  # for sameAs in organisation's structured data

    publisherName = "gohugohq.com" # publisher used in article schema
    publisherLogo = "https://gohugo-amp.gohugohq.com/logo-publisher.png" # https://developers.google.com/search/docs/data-types/articles#logo-guidelines
    publisherLogoWidth = 600 # logo width
    publisherLogoHeight = 60 # logo height
```