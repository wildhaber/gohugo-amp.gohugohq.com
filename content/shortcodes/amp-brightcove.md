{
    "date" : "2016-11-20T00:30:41+02:00",
    "draft" : false,
    "title" : "amp-brightcove",
    "amp" : {
        "elements" : ["amp-brightcove"]
    },
    "documentation" : {
        "category" : "Media",
        "element" : "amp-brightcove",
        "examples" : {
            "shortcode" : {
              "description" : "run a video",
              "code" : ["{{% amp-brightcove account=\"906043040001\" video=\"1401169490001\" player=\"180a5658-8be8-4f33-8eba-d562ab41b40c\" width=\"480\" height=\"270\" layout=\"responsive\" %}}"]
            },
              "partial" : {
                "description" : "usage as partial",
                "code" : ["{{ partial \"amp/brightcove\" (dict \"account\" \"906043040001\" \"video\" \"1401169490001\" \"player\" \"180a5658-8be8-4f33-8eba-d562ab41b40c\" \"width\" \"480\" \"height\" \"270\" \"layout\" \"responsive\") }} "]
              }
        },
        "references" : [{
            "title" : "AMP documentation amp-brightcove",
            "url" : "https://www.ampproject.org/docs/reference/components/amp-brightcove"
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
            "account" : {
                "name" : "account",
                "description" : "becomes data-account",
                "type" : "string"
            },
            "video" : {
                "name" : "video",
                "description" : "becomes data-video-id",
                "type" : "string"
            },
            "player" : {
                "name" : "player",
                "description" : "becomes data-player-id",
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

> No demo available because we have no certain account-id