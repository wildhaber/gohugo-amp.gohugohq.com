+++
date = "2016-11-18T19:28:41+02:00"
draft = false
title = "schema WebSite configuration"

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
  
+++

# Schema WebSite configuration

From the base configuration the following attributes are relevant for a proper WebSite-Schema configuration. All the configuration parameters living in the `[params]` section of your [`config.toml`](/config/) in the root folder of your HUGO project.

### page name

#### alternatePageName

```toml
alternatePageName = "My Website"
```

>  This parameter defines a alternative name for website name in [structured data](/schema/). If this property is missing only the title will be shown in the structured data.