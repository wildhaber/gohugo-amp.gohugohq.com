{
    "date" : "2016-10-16T19:28:41+02:00",
    "draft" : false,
    "title" : "amp-anim",
    "amp" : {
        "elements" : ["amp-anim"]
    },
    "documentation" : {
        "category" : "Media",
        "element" : "amp-anim",
        "examples" : {
            "default" : {
                "description" : "usage as shortcode",
                "code" : ["{{% amp-anim ", "    width=\"300\"", "    height=\"250\"", "    attribution=\"The Go gopher was designed by Reneee French and is licensed under CC 3.0 attributions.\"", "    src=\"https://ampbyexample.com/img/gopher.gif\"", "    placeholder=\"https://placehold.it/100x100/ff0000\"", "%}}"]
            },
            "partial" : {
                "description" : "usage as partial",
                "code" : ["{{ partial \"amp/anim\" (dict \"width\" \"300\" \"height\" \"250\" \"attribution\" \"The Go gopher was designed by Reneee French and is licensed under CC 3.0 attributions.\" \"src\" \"https://ampbyexample.com/img/gopher.gif\" \"placeholder\" \"https://placehold.it/100x100/ff0000\") }}"]
            }
        },
        "references" : [{
            "title" : "AMP documentation amp-anim",
            "url" : "https://www.ampproject.org/docs/reference/components/amp-anim"
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
             "attribution" : {
                "name" : "attribution",
                "type" : "string",
                "example" : "The Go gopher was designed by Reneee French and is licensed under CC 3.0 attributions."
             },
              "src" : {
                 "name" : "src",
                 "type" : "string",
                 "example" : "https://ampbyexample.com/img/gopher.gif"
              },
              "placeholder" : {
                   "name" : "placeholder",
                   "type" : "string",
                   "example" : "https://placehold.it/100x100/ff0000"
              }
        }
    },
    "sitemap" : {
      "changefreq" : "monthly",
      "priority" : 0.5,
      "filename" : "sitemap.xml"
    }
}

{{% amp-anim width="300" height="250" attribution="The Go gopher was designed by Reneee French and is licensed under CC 3.0 attributions." src="https://ampbyexample.com/img/gopher.gif" placeholder="https://placehold.it/100x100/ff0000" %}}

