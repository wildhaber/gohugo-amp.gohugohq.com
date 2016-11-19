+++
date = "2016-11-18T19:28:41+02:00"
draft = false
title = "Schema Organization configuration"

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
  
+++

# Schema Organization configuration

From the base configuration the following attributes are relevant for a proper Organization-Schema configuration. All the configuration parameters living in the `[params]` section of your [`config.toml`](/config/) in the root folder of your HUGO project.

### organization

#### organizationLogo

```toml
organizationLogo = "https://gohugohq.com/logo.png"
```

> set organization logo for structured data

#### organizationName

```toml
organizationName = "gohugohq.com"
```

> set organization name

#### organizationLogo

```toml
organizationAddress = "Some Street 123, 12345 City" # set organization address
```

> set organization address (optional)

#### socialProfiles

```toml
socialProfiles = ["http://www.facebook.com/your-profile","http://instagram.com/yourProfile","http://www.linkedin.com/in/yourprofile","http://plus.google.com/your_profile"]
```

> an array of your social profile URL's. Will be set as `sameAs` in organization's structured data

We recommend reading more about how [gohugo amp-theme is using structured data automatically](/schema/) in the schema Section.