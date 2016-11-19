+++
date = "2016-11-18T19:28:41+02:00"
draft = false
title = "Structured Data: Article"

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
  
+++

# Article

Proper structured data in your news, blog, and sports article page can enhance your appearance in Google Search results. Enhanced features include entry in a top stories carousel and rich result features such as headline text and larger-than-thumbnail images.

### Article-Front-Matters

Article structured data are rendered and defined by the front-matters of your content. Following you will find an [example article](/examples/articles/first-article/) with and its output in the structured data:

```toml
date = "2016-11-18T19:28:41+02:00"
publishdate = "2016-11-18T19:28:41+02:00"
draft = false
title = "article example one"
description = "Short description of the article."

[amp]
    elements = []
    
[structured]
    type = "Article"

[author]
    name = "John Doe"

[image]
    src = "https://gohugo-amp.gohugohq.com/example-image.jpg"
    width = 1600
    height = 900
    title = "Example Article image"
    author = "gohugohq"
    link = "https://gohugohq.com"
    license = "CC BY 2.0"
    license_link = "https://creativecommons.org/licenses/by/2.0/"

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
```

This will generate the following **valid structured data** in the head-section:

```javsacript
<script type="application/ld+json">
{
  "@context": "http://schema.org",
  "@type": "Article",
  "author": {
    "name" : "John Doe"
  },
  "headline": "article example one",
  "description": "Short description of the article.",
  "wordCount":  357 ,
  "datePublished" : "2016-11-18T19:28:41",
  "dateModified" : "2016-11-18T19:28:41",
  "image" : {
      "@context": "http://schema.org",
      "@type": "ImageObject",
      "author": "gohugohq",
      "url": "https:\/\/gohugo-amp.gohugohq.com\/example-image.jpg",
      "datePublished": "2016-11-18T19:28:41",
      "name": "Example Article image",
      "height" :  900 ,
      "width" :  1600 ,
      "license" : "https:\/\/creativecommons.org\/licenses\/by\/2.0\/",
      "isBasedOn" : "https:\/\/gohugohq.com"
    },
  "mainEntityOfPage" : "http:\/\/localhost:1313\/examples\/articles\/first-article\/",
  "publisher" : {
    "@type": "Organization",
    "name" : "gohugohq.com",
    "logo" : {
        "@type" : "ImageObject",
        "url" : "https:\/\/gohugo-amp.gohugohq.com\/logo-publisher.png",
        "height" :  60 ,
        "width" :  600 
    }
  }
}
</script>
```

> Please not that the `publisher`-Data are rendered from the [`config.toml`](/config/) in the [`publisher`-Section](/config/schema-article).