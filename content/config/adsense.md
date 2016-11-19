+++
date = "2016-11-18T19:28:41+02:00"
draft = false
title = "adsense configuration"

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
  
+++

# AdSense configuration

From the base configuration the following attributes are relevant if you are using [adSense](https://www.google.com/adsense/start/) on your website. All the configuration parameters living in the `[params]` section of your [`config.toml`](/config/) in the root folder of your HUGO project.

### AdSense

#### adsensePublisher

```toml
adsensePublisher = "ca-pub-123456789"
```

>  your adsense publisher id. Here you will find a guide how to [find your adsense publisher id](https://support.google.com/adsense/answer/105516).

We recommend reading more in the guide about [how to use `amp-adsense` partial and shortcodes in gohugo amp theme](/shortcodes/amp-adsense/).