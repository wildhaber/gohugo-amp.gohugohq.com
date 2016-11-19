+++
date = "2016-11-18T19:28:41+02:00"
draft = false
title = "amp configuration"

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
  
+++

# amp configuration

From the base configuration the following attributes are relevant for a successful configuration of AMP. All the configuration parameters living in the `[params]` section of your [`config.toml`](/config/) in the root folder of your HUGO project.

### enable amp

```toml
amp = true # enables amp features
```

> Enabling AMP features is easy. Simply put `amp = true`. Please be aware that it does not matter what value you put in, the logic only checks on the existence of an amp parameter.

### CDN for autoload

#### ampCdnRoot

```toml
ampCdnRoot = "https://cdn.ampproject.org/"
```

>  This parameter defines the root of the AMP CDN.

#### ampCdnRoot

```toml
ampCdnRoot = "https://cdn.ampproject.org/"
```

#### ampRelease

```toml
ampRelease = "v0"
```

>  This parameter defines the amp release you want to use. It will concat the script paths from `ampCdnRoot + ampRelease + '.js'` for the base AMP JavaScript file.

#### ampElementsVersion

```toml
ampElementsVersion = "0.1" # 
```

>  This parameter defines amp-elements version you want to use. It will concat the script paths from `ampCdnRoot + ampRelease + 'ELEMENT-NAME-' + ampElementsVersion + '.js'` for the AMP elements.


#### ampElements

```toml
ampElements = ["amp-accordion","amp-ad","amp-analytics","amp-carousel","amp-iframe","amp-app-banner","amp-dynamic-css-classes","amp-form","amp-fx-flying-carpet","amp-image-lightbox","amp-lightbox","amp-sidebar","amp-social-share","amp-sticky-ad","amp-user-notification"]
```

>  This parameter defines which amp-elements you are using globally, these elements will be included in every page. Please note that you can autoload additional amp-elements in the front-matters of each particular site separately if you need it. You should use this only for elements you use on every page.