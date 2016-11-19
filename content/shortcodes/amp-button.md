{
    "date" : "2016-11-20T00:30:41+02:00",
    "draft" : false,
    "title" : "amp-button",
    "amp" : {
        "elements" : ["amp-lightbox"]
    },
    "documentation" : {
        "category" : "Media",
        "element" : "",
        "examples" : {
            "shortcode" : {
              "description" : "add a button",
              "code" : ["{{% amp-button onTap=\"my-custom-lightbox\" text=\"Open my custom lightbox\" %}}"]
            },
              "partial" : {
                "description" : "usage as partial",
                "code" : ["{{ partial \"amp/button\" (dict \"onTap\" \"my-custom-lightbox\" \"text\" \"Open my custom lightbox\") }}"]
              }
        },
        "attributes" : {
            "onTap" : {
               "name" : "onTap",
               "type" : "string"
            },
            "text" : {
               "name" : "text",
               "type" : "string"
            }
        }
    },
    "sitemap" : {
      "changefreq" : "monthly",
      "priority" : 0.5,
      "filename" : "sitemap.xml"
    }
}

{{% amp-button onTap="my-custom-lightbox" text="Open my custom lightbox" %}}
{{% amp-button onTap="my-custom-lightbox.close" text="Close my custom lightbox" %}}

{{% amp-lightbox id="my-custom-lightbox" %}}
# Hello Lightbox
Wow this is amazing.
{{% /amp-lightbox %}}