+++
date = "2016-11-18T19:28:41+02:00"
draft = false
title = "Structured Data: Breadcrumbs"

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
  
+++

# Breadcrumbs

A breadcrumb trail on a page indicates the page's position in the site hierarchy. A user can navigate all the way up in the site hierarchy, one level at a time, by starting from the last breadcrumb in the breadcrumb trail.

### Breadcrumbs are automatically generated

Breadcrumbs will be rendered automatically according to the page you are currently in. For example:

```javsacript
<script type="application/ld+json">
{
  "@context": "http://schema.org",
  "@type": "BreadcrumbList",
  "itemListElement": [{
        "@type": "ListItem",
        "position":  1 ,
        "item": {
          "@id": "http:\/\/gohugo-amp.gohugohq.com\/",
          "name": "home"
        }
    },{
        "@type": "ListItem",
        "position":  2 ,
        "item": {
          "@id": "http:\/\/gohugo-amp.gohugohq.com\/schema\/",
          "name": "schema"
        }
    },{
        "@type": "ListItem",
        "position":  3 ,
        "item": {
          "@id": "http:\/\/gohugo-amp.gohugohq.com\/schema\/breadcrumb\/",
          "name": "breadcrumb"
        }
    }]
}
</script>
```