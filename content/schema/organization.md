+++
date = "2016-11-18T19:28:41+02:00"
draft = false
title = "Structured Data: Organization"

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
  
+++

# Organization

Organization details can be defined in your [`config.toml`](/config/) in the [`organization`-Section](/config/schema-organization). And further contact details can be set in a file called `data/organization/contacts.json`, you will find an example below.

### Organization data are automatically generated

Organization data will be rendered automatically on all pages. For example:

```javsacript
<script type="application/ld+json">
{
  "@context": "http://schema.org",
  "@type": "Organization",
  "name": "gohugohq.com",
  "url": "http:\/\/localhost:1313\/",
  "sameAs": ["http://www.facebook.com/your-profile","http://instagram.com/yourProfile","http://www.linkedin.com/in/yourprofile","http://plus.google.com/your_profile"],
  "logo": "https:\/\/gohugohq.com\/logo.png",
  "address": "Some Street 123, 12345 City"
  
}
</script>
```

or including [contact details](https://developers.google.com/search/docs/data-types/corporate-contacts) here:

**Example contacts.json**
```
{
 "contactPoint": [{
   "@type": "ContactPoint",
   "telephone": "+1-123-456-789",
   "contactType": "customer service",
   "contactOption": "TollFree",
   "areaServed": "US"
 },{
   "@type": "ContactPoint",
   "telephone": "+1-456-789-101",
   "contactType": "customer service"
 },{
   "@type": "ContactPoint",
   "telephone": "+1-789-101-123",
   "contactType": "customer service",
   "contactOption": [
     "HearingImpairedSupported",
     "TollFree"
   ],
   "areaServed": "US"
 },{
   "@type": "ContactPoint",
   "telephone": "+1-456-789-333",
   "contactType": "technical support",
   "contactOption": "TollFree",
   "areaServed": [
     "US",
     "CA"
   ],
   "availableLanguage": [
     "English",
     "French"
   ]
 },{
   "@type": "ContactPoint",
   "telephone": "+1-234-567-891",
   "contactType": "bill payment",
   "contactOption": "TollFree",
   "areaServed": [
     "US",
     "CA"
   ]
 }]
}
```

will output the following data:

```javsacript
<script type="application/ld+json">
{
  "@context": "http://schema.org",
  "@type": "Organization",
  "name": "gohugohq.com",
  "url": "http:\/\/localhost:1313\/",
  "sameAs": ["http://www.facebook.com/your-profile","http://instagram.com/yourProfile","http://www.linkedin.com/in/yourprofile","http://plus.google.com/your_profile"],
  "logo": "https:\/\/gohugohq.com\/logo.png",
  "address": "Some Street 123, 12345 City",
  "contactPoint": [{"@type":"ContactPoint","areaServed":"US","contactOption":"TollFree","contactType":"customer service","telephone":"+1-877-746-0909"},{"@type":"ContactPoint","contactType":"customer service","telephone":"+1-505-998-3793"},{"@type":"ContactPoint","areaServed":"US","contactOption":["HearingImpairedSupported","TollFree"],"contactType":"customer service","telephone":"+1-877-296-1018"},{"@type":"ContactPoint","areaServed":["US","CA"],"availableLanguage":["English","French"],"contactOption":"TollFree","contactType":"technical support","telephone":"+1-877-453-1304"},{"@type":"ContactPoint","areaServed":["US","CA"],"contactOption":"TollFree","contactType":"bill payment","telephone":"+1-877-453-1304"}]
}
</script>
```