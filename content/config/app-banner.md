+++
date = "2016-11-18T19:28:41+02:00"
draft = false
title = "app-banner configuration"

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
  
+++

# app-banner configuration

From the base configuration the following attributes are relevant if you wish to show an app-banner on top of your website. All the configuration parameters living in the `[params]` section of your [`config.toml`](/config/) in the root folder of your HUGO project.

### app-banner

#### appleItunesApp

```toml
appleItunesApp = "app-id=123456789, app-argument=app-name://link/to/app-content"
```

>  required if you want to add an app banner with iOS app.

#### ampManifest

```toml
ampManifest = "/amp-manifest.json"
```

>  required if you want to add the app-banner feature. This file should be in the `static` folder of your root HUGO project.

---

### Example amp-manifest.json

```json
{
  "prefer_related_applications": true,
  "related_applications": [
    {
      "platform": "play",
      "id": "com.app.path",
      "url": "android-app://com.app.path/https/host.com/path/to/app-content"
    }
  ]
}
```

We recommend reading more in the guide about [how to use `amp-app-banner` partial and shortcode in gohugo amp theme](/shortcodes/amp-app-banner/).
