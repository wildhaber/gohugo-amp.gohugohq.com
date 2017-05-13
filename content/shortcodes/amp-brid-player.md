{
    "date" : "2016-11-20T00:30:41+02:00",
    "draft" : false,
    "title" : "amp-brid-player",
    "amp" : {
        "elements" : ["amp-brid-player"]
    },
    "type" : "shortcode",
    "documentation" : {
        "category" : "Media",
        "element" : "amp-brid-player",
        "examples" : {
            "video" : {
              "description" : "run as video",
              "code" : ["{{< amp-brid-player partner=\"264\" player=\"4144\" video=\"13663\" width=\"480\" height=\"270\" layout=\"responsive\" >}}"]
            },
             "playlist" : {
               "description" : "run a playlist",
               "code" : ["{{< amp-brid-player partner=\"264\" player=\"4144\" playlist=\"1220\" width=\"480\" height=\"270\" layout=\"responsive\" >}}"]
             },
              "partial" : {
                "description" : "usage as partial",
                "code" : ["{{ partial \"amp/brid-player.html\" (dict \"partner\" \"264\" \"player\" \"4144\" \"playlist\" \"1220\" \"width\" \"480\" \"height\" \"270\" \"layout\" \"responsive\") }} "]
              }
        },
        "references" : [{
            "title" : "AMP documentation amp-brid-player",
            "url" : "https://www.ampproject.org/docs/reference/components/amp-brid-player"
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
            "partner" : {
                "name" : "partner",
                "description" : "becomes data-partner",
                "type" : "string"
            },
            "video" : {
                "name" : "video",
                "description" : "becomes data-video",
                "type" : "string"
            },
            "player" : {
                "name" : "player",
                "description" : "becomes data-player",
                "type" : "string"
            },
            "playlist" : {
                "name" : "playlist",
                "description" : "becomes data-playlist",
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

> No demo available because we have no certain partner-id