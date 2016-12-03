{
    "date" : "2016-11-26T00:30:41+02:00",
    "draft" : false,
    "title" : "amp-dailymotion",
    "amp" : {
        "elements" : ["amp-dailymotion"]
    },
    "type" : "shortcode",
    "documentation" : {
        "category" : "Media",
        "element" : "amp-dailymotion",
        "examples" : {
            "shortcode" : {
              "description" : "run as shortcode",
              "code" : ["{{< amp-dailymotion video=\"x2m8jpp\" highlight=\"FF4081\" logo=\"false\" info=\"false\" endscreen=\"false\" sharing=\"false\" start=\"44\" width=\"480\" height=\"270\" layout=\"responsive\">}}"]
            },
              "partial" : {
                "description" : "usage as partial",
                "code" : ["{{ partial \"amp/dailymotion\" (dict \"video\" \"x2m8jpp\" \"highlight\" \"FF4081\" \"logo\" \"false\" \"endscreen\" \"false\" \"sharing\" \"false\" \"start\" \"44\" \"width\" \"480\" \"height\" \"270\" \"layout\" \"responsive\") }} "]
              }
        },
        "references" : [{
            "title" : "AMP documentation amp-dailymotion",
            "url" : "https://www.ampproject.org/docs/reference/components/amp-dailymotion"
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
            "video" : {
                "name" : "video",
                "description" : "becomes data-videoid",
                "type" : "string"
            },
            "logo" : {
                "name" : "logo",
                "description" : "becomes data-ui-logo",
                "type" : "string"
            },
            "info" : {
                "name" : "info",
                "description" : "becomes data-info",
                "type" : "string"
            },
            "highlight" : {
                "name" : "highlight",
                "description" : "becomes data-highlight",
                "type" : "string"
            },
            "mute" : {
                "name" : "mute",
                "description" : "becomes data-mute",
                "type" : "string"
            },
            "endscreen" : {
                "name" : "endscreen",
                "description" : "becomes data-endscreen-enable",
                "type" : "string"
            },
            "sharing" : {
                "name" : "sharing",
                "description" : "becomes data-sharing",
                "type" : "string"
            },
            "start" : {
                "name" : "start",
                "description" : "becomes data-start",
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

{{< amp-dailymotion video=\"x2m8jpp\" highlight=\"FF4081\" logo=\"false\" info=\"false\" endscreen=\"false\" sharing=\"false\" start=\"44\" width=\"480\" height=\"270\" layout=\"responsive\">}}