+++
date = "2016-11-18T19:28:41+02:00"
draft = false
title = "analytics configuration"

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
  
+++

# Analytics configuration

From the base configuration the following attributes are relevant if you are using google analytics to measure your websites traffic. All the configuration parameters living in the `[params]` section of your [`config.toml`](/config/) in the root folder of your HUGO project.

### analytics

#### googleAnalytics

```toml
googleAnalytics = "UA-123456-78"
```

>  your UA-Tracking code. Here you will find a guide how to [find your UA-Code](https://support.google.com/analytics/answer/1032385).

---

## Event Triggers

Its recommended to use custom event triggers. You can define them in a custom JSON-File `/data/analytics/triggers.json`. A simple example you find below:

```toml
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

For further possible triggers please head to the official [AMP Analytics Documentation](https://www.ampproject.org/docs/reference/components/amp-analytics) with some [advanced examples](https://ampbyexample.com/components/amp-analytics/).