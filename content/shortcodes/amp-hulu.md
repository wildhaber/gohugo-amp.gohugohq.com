{
    "date" : "2016-10-16T19:28:41+02:00",
    "draft" : false,
    "title" : "amp-hulu",
    "amp" : {
        "elements" : ["amp-hulu"]
    },
    "type" : "shortcode",
    "documentation" : {
        "category" : "Media",
        "element" : "amp-hulu",
        "examples" : {
            "default" : {
              "description" : "usage as shortcode",
              "code" : ["{{< amp-hulu id=\"Bx6H30RBVFNpOe-iiOxp3A\" layout=\"responsive\" width=\"412\" height=\"213\" >}}"]
            },
            "partial" : {
              "description" : "usage as partial",
              "code" : ["{{ partial \"amp/hulu\" (dict \"width\" \"412\" \"height\" \"213\" \"id\" \"Bx6H30RBVFNpOe-iiOxp3A\" }}"]
            }
        },
        "references" : [{
            "title" : "AMP documentation amp-hulu",
            "url" : "https://www.ampproject.org/docs/reference/components/amp-hulu"
        }],
        "attributes" : {
            "width" : {
               "name" : "width",
               "type" : "number"
            },
            "height" : {
               "name" : "height",
               "type" : "number"
            },
            "layout" : {
               "name" : "layout",
               "type" : "string"
            },
            "id" : {
                "name" : "id",
                "description" : "becomes data-eid",
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

> Demo is disabled since it throws an error like `The tag 'amp-hulu' is disallowed`.