+++
date = "2016-11-18T19:28:41+02:00"
draft = false
title = "Schema Article configuration"

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
  
+++

# Schema Article configuration

From the base configuration the following attributes are relevant for a proper Article-Schema configuration. All the configuration parameters living in the `[params]` section of your [`config.toml`](/config/) in the root folder of your HUGO project.

### publisher

#### publisherName

```toml
publisherName = "gohugohq.com"
```

> publisher used in article schema

#### publisherLogo

```toml
publisherLogo = "https://gohugo-amp.gohugohq.com/logo-publisher.png"
```

> Read more about the logo in the [guidelines for a publisher logo](https://developers.google.com/search/docs/data-types/articles#logo-guidelines).

#### publisherLogoWidth

```toml
publisherLogoWidth = 600
```

> logo width

#### publisherLogoHeight

```toml
publisherLogoHeight = 60
```

> logo height

We recommend reading more about how [gohugo amp-theme is using structured data automatically](/schema/) in the schema Section.