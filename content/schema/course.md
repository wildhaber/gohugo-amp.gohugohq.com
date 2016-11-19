+++
date = "2016-11-18T19:28:41+02:00"
draft = false
title = "Structured Data: Course"

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
  
+++

# Course

Mark up your course lists with structured data so prospective students find you through Google Search. You can provide details including the course name, who's offering it, and a short description.

### Course-Front-Matters

Course structured data are rendered and defined by the front-matters of your content. Following you will find an [example course page](/examples/courses/first-course/) with and its output in the structured data:

```toml
date = "2016-11-18T19:28:41+02:00"
publishdate = "2016-11-18T19:28:41+02:00"
draft = false
title = "course example one"
description = "Short description of the course."

[amp]
    elements = []
    
[structured]
    type = "Course"

[provider]
    name = "University of Example"
    url = "https://gohugohq.com"

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
  "@type": "Course",
  "name" : "course example one",
  "description": "Short description of the course.",
  "provider" : {
    "@type": "Organization",
    "name" : "University of Example",
    "sameAs" : "https:\/\/gohugohq.com"
  }
}
</script>
```