{
    "date" : "2016-10-16T19:28:41+02:00",
    "draft" : false,
    "title" : "amp-gfycat",
    "amp" : {
        "elements" : ["amp-gfycat"]
    },
    "type" : "shortcode",
    "documentation" : {
        "category" : "Media",
        "element" : "amp-gfycat",
        "examples" : {
            "default" : {
              "description" : "usage as shortcode",
              "code" : ["{{< amp-gfycat id=\"FeistyBiodegradableBlackfish\" layout=\"responsive\" width=\"150\" height=\"150\" >}}"]
            },
            "partial" : {
              "description" : "usage as partial",
              "code" : ["{{ partial \"amp/gfycat\" (dict \"width\" \"150\" \"height\" \"150\" \"id\" \"FeistyBiodegradableBlackfish\" }}"]
            }
        },
        "references" : [{
            "title" : "AMP documentation amp-gfycat",
            "url" : "https://www.ampproject.org/docs/reference/components/amp-gfycat"
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
                "description" : "becomes data-gfyid",
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

{{< amp-gfycat id="FeistyBiodegradableBlackfish" layout="responsive" width="150" height="150"  >}}
