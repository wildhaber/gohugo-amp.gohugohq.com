{
    "date" : "2016-11-26T00:30:41+02:00",
    "draft" : false,
    "title" : "amp-facebook-video",
    "amp" : {
        "elements" : ["amp-facebook"]
    },
    "documentation" : {
        "category" : "Social",
        "element" : "amp-facebook-video",
        "examples" : {
            "shortcode" : {
              "description" : "run as shortcode",
              "code" : ["{{< amp-facebook-video width=\"680\" height=\"400\" href=\"https://www.facebook.com/zuck/videos/10102509264909801/\" layout=\"responsive\" >}}"]
            },
              "partial" : {
                "description" : "usage as partial",
                "code" : ["{{ partial \"amp/facebook-video\" (dict \"href\" \"https://www.facebook.com/zuck/videos/10102509264909801\" \"width\" \"680\" \"height\" \"400\" \"layout\" \"responsive\") }} "]
              }
        },
        "references" : [{
            "title" : "AMP documentation amp-facebook",
            "url" : "https://www.ampproject.org/docs/reference/components/amp-facebook"
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
            "href" : {
                "name" : "href",
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

{{< amp-facebook-video width="680" height="400" href="https://www.facebook.com/zuck/videos/10102509264909801/" layout="responsive" >}}