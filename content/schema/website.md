+++
date = "2016-11-18T19:28:41+02:00"
draft = false
title = "Structured Data: WebSite"

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
  
+++

# WebSite

WebSite details can be defined in your [`config.toml`](/config/) in the [`website`-Section](/config/schema-website).

### WebSite data are automatically generated

Website data will be rendered automatically on all pages. For example:

```javsacript
<script type="application/ld+json">
{
    "@context": "http://schema.org",
    "@type": "WebSite",
    "name": "gohugo-amp starter theme",
    "alternateName": "HUGO AMP",
    "url": "http:\/\/gohugo-amp.gohugohq.com\/"
}
</script>
```