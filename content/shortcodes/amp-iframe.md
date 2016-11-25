{
    "date" : "2016-10-16T19:28:41+02:00",
    "draft" : false,
    "title" : "amp-iframe",
    "amp" : {
        "elements" : ["amp-iframe"]
    },
    "documentation" : {
        "category" : "Media",
        "element" : "amp-iframe",
        "examples" : {
            "default" : {
              "description" : "usage as shortcode",
              "code" : ["{{< amp-iframe ", "  src=\"https://example.com\"", "  width=\"450\"", "  height=\"300\"", "  layout=\"responsive\"", "  resizable=\"true\"", "  sandbox=\"allow-scripts allow-same-origin\"", "  overflow=\"Read more!!!\"", ">}}"]
            },
            "partial" : {
              "description" : "usage as partial",
              "code" : ["{{ partial \"amp/iframe\" (dict \"src\" \"https://example.com\" \"resizable\" \"true\" \"sandbox\" \"allow-scripts allow-same-origin\" \"overflow\" \"Read more!!!\" \"layout\" \"responsive\" \"width\" \"412\" \"height\" \"213\" }}"]
            }
        },
        "references" : [{
            "title" : "AMP documentation amp-iframe",
            "url" : "https://www.ampproject.org/docs/reference/components/amp-iframe"
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
            "src" : {
             "name" : "src",
             "type" : "string"
            },
            "frameborder" : {
            "name" : "frameborder",
            "type" : "number"
            },
            "resizable" : {
            "name" : "resizable",
            "type" : "boolean"
            },
            "sandbox" : {
            "name" : "sandbox",
            "type" : "string"
            },
            "overflow" : {
            "name" : "overflow",
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

{{< amp-iframe src="https://example.com" layout="responsive" width="450" height="300" resizable="true" sandbox="allow-scripts allow-same-origin" overflow="Read more!!!"  >}}
