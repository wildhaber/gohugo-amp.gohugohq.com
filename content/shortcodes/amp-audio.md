{
    "date" : "2016-10-16T19:28:41+02:00",
    "draft" : false,
    "title" : "amp-audio",
    "amp" : {
        "elements" : ["amp-audio"]
    },
    "documentation" : {
        "category" : "Media",
        "element" : "amp-audio",
        "examples" : {
            "default" : {
              "description" : "usage as shortcode",
              "code" : ["{{< amp-audio ", "   width=\"300\"", "   height=\"35\"", "   src=\"https://ia801402.us.archive.org/16/items/EDIS-SRP-0197-06/EDIS-SRP-0197-06.mp3\"", "   mp3=\"https://ia801402.us.archive.org/16/items/EDIS-SRP-0197-06/EDIS-SRP-0197-06.mp3\"", "   ogg=\"//sample.ogg.fallback.ogg\"", "   autoplay=\"true\"","   loop=\"true\"","   muted=\"true\"", ">}}"]
            },
            "partial" : {
              "description" : "usage as partial",
              "code" : ["{{ partial \"amp/audio\" (dict \"width\" \"300\" \"height\" \"35\" \"src\" \"https://ia801402.us.archive.org/16/items/EDIS-SRP-0197-06/EDIS-SRP-0197-06.mp3\" \"mp3\" \"https://ia801402.us.archive.org/16/items/EDIS-SRP-0197-06/EDIS-SRP-0197-06.mp3\" \"ogg\" \"//sample.ogg.fallback.ogg\" \"autoplay\" \"true\" \"loop\" \"true\" \"muted\" \"true\") }}"]
            }
        },
        "references" : [{
            "title" : "AMP documentation amp-audio",
            "url" : "https://www.ampproject.org/docs/reference/components/amp-audio"
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
            "mp3" : {
                "name" : "mp3",
                "type" : "string"
            },
            "ogg" : {
                "name" : "ogg",
                "type" : "string"
            },
            "autoplay" : {
                "name" : "autoplay",
                "type" : "string",
                "description" : "There is a currently a `true` value just as placeholder. The code only checks for existence of this parameter not to the value."
            },
            "loop" : {
                "name" : "loop",
                "type" : "string",
                "description" : "There is a currently a `true` value just as placeholder. The code only checks for existence of this parameter not to the value."
            },
            "muted" : {
                "name" : "muted",
                "type" : "string",
                "description" : "There is a currently a `true` value just as placeholder. The code only checks for existence of this parameter not to the value."
            }
        }
    },
    "sitemap" : {
      "changefreq" : "monthly",
      "priority" : 0.5,
      "filename" : "sitemap.xml"
    }
}

{{% amp-audio width="300" height="35" src="https://ia801402.us.archive.org/16/items/EDIS-SRP-0197-06/EDIS-SRP-0197-06.mp3" mp3="https://ia801402.us.archive.org/16/items/EDIS-SRP-0197-06/EDIS-SRP-0197-06.mp3" ogg="//sample.ogg.fallback.ogg" autoplay="true" loop="true" muted="true" %}}
