{
    "date" : "2016-10-16T19:28:41+02:00",
    "draft" : false,
    "title" : "amp-adsense",
    "amp" : {
        "elements" : ["amp-ad"]
    },
    "documentation" : {
        "category" : "Advertising",
        "element" : "amp-ad",
        "examples" : {
            "default" : {
                "description" : "Regular adsense display",
                "code" : ["{{< amp-adsense width=\"300\" height=\"250\" slot=\"2195367133\" >}}"]
            },
             "sticky" : {
                 "description" : "Make a sticky adsense to the bottom",
                 "code" : ["{{< amp-adsense width=\"320\" height=\"50\" slot=\"2195367133\" sticky=\"true\" >}}"]
             },
              "partial" : {
                  "description" : "Usage example as partial",
                  "code" : ["{{ partial \"amp/adsense\" (dict \"context\" $ \"width\" \"320\" \"height\" \"50\" \"slot\" \"2195367133\" \"sticky\" \"true\") }}"]
              }
        },
        "references" : [{
            "title" : "AMP documentation amp-ad",
            "url" : "https://www.ampproject.org/docs/reference/components/amp-ad"
        }],
        "attributes" : {
            "width" : {
               "name" : "width",
               "type" : "number",
               "example" : "300"
            },
            "height" : {
               "name" : "height",
               "type" : "number",
               "example" : "250"
            },
            "slot" : {
               "name" : "slot",
               "type" : "number",
               "example" : "123456789",
               "description" : "set as data-ad-slot attribute"
            }
        }
    },
    "sitemap" : {
      "changefreq" : "monthly",
      "priority" : 0.5,
      "filename" : "sitemap.xml"
    }
}

{{% amp-adsense width="300" height="250" slot="2195367133" %}}

> Make sure you have set your **adsensePublisher** parameter in the `config.toml` file
```toml
[params]
    adsensePublisher = "ca-pub-123456789"
```
