{
    "date" : "2016-10-16T19:28:41+02:00",
    "draft" : false,
    "title" : "amp-image",
    "amp" : {
        "elements" : []
    },
    "documentation" : {
        "category" : "Media",
        "element" : "",
        "examples" : {
            "default" : {
              "description" : "usage as shortcode",
              "code" : ["{{< amp-image", "  src=\"//placehold.it/350x350\"", "  srcset=\"//placehold.it/600x600 640w, //placehold.it/150x150 320w\"", "  height=\"300\"", "  width=\"300\"", "  layout=\"responsive\"", "  alt=\"Alternative Text\"", "  attribution=\"CC courtesy of placehold.it\"", ">}}"]
            },
            "partial" : {
              "description" : "usage as partial",
              "code" : ["{{ partial \"amp/image\" (dict \"src\" \"//placehold.it/350x350\" \"srcset\" \"//placehold.it/600x600 640w, //placehold.it/150x150 320w\" \"alt\" \"Alternative Text\" \"attribution\" \"CC courtesy of placehold.it\" \"layout\" \"responsive\" \"width\" \"300\" \"height\" \"300\" }}"]
            }
        },
        "references" : [{
            "title" : "AMP documentation amp-image",
            "url" : "https://www.ampproject.org/docs/reference/components/amp-img"
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
            "alt" : {
            "name" : "alt",
            "type" : "string"
            },
            "attribution" : {
            "name" : "attribution",
            "type" : "string"
            },
            "srcset" : {
            "name" : "srcset",
            "type" : "string"
            },
            "tabindex" : {
            "name" : "tabindex",
            "type" : "number"
            },
            "onTap" : {
            "name" : "onTap",
            "type" : "string"
            },
            "role" : {
            "name" : "role",
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

> This is a built in element, there is no need to explicitly load this in your amp-elements part of the front-matters.

{{<
    amp-image src="//placehold.it/350x350"
    srcset="//placehold.it/600x600 640w, //placehold.it/150x150 320w"
    height="300"
    width="300"
    layout="responsive"
    alt="Alternative Text"
    attribution="CC courtesy of placehold.it"
>}}