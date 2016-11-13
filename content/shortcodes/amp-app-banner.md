{
    "date" : "2016-10-16T19:28:41+02:00",
    "draft" : false,
    "title" : "amp-app-banner",
    "amp" : {
        "elements" : ["amp-app-banner"]
    },
    "documentation" : {
        "category" : "Advertising",
        "element" : "amp-app-banner",
        "examples" : {
            "default" : {
                "code" : ["{{ with $.Site.Data.app.banner }}{{ partial \"amp/app-banner\" . }}{{ end }}"]
            }
        },
        "references" : [{
            "title" : "AMP documentation amp-app-banner",
            "url" : "https://www.ampproject.org/docs/reference/components/amp-app-banner"
        }],
        "attributes" : {
            "id" : {
               "name" : "id",
               "type" : "string",
               "example" : "app-banner-id"
            },
            "src" : {
               "name" : "src",
               "type" : "string",
               "description" : "used for the amp-image element and app-icon"
            },
             "name" : {
                "name" : "name",
                "type" : "string",
                "description" : "name of the app"
             },
              "description" : {
                 "name" : "description",
                 "type" : "string",
                 "description" : "Very short description of the app."
              },
              "openText" : {
                   "name" : "openText",
                   "type" : "string",
                   "description" : "Text for the call-to-action button",
                   "example" : "Get the app"
              }
        }
    },
    "sitemap" : {
      "changefreq" : "monthly",
      "priority" : 0.5,
      "filename" : "sitemap.xml"
    }
}

> to run amp-app-banner, please set all the below configuration correctly.

#### Example `data/app/banner.json`

```json
{
  "id" : "app-banner-id",
  "src" : "https://placehold.it/60x51/ff3300/cccccc",
  "name" : "My Apps Name",
  "description" : "Short app description. Really short.",
  "openText" : "get the app"
}
```

#### Example `static/amp-manifest.json`

```json
{
  "prefer_related_applications": true,
  "related_applications": [
    {
      "platform": "play",
      "id": "com.app.path",
      "url": "android-app://com.app.path/https/host.com/path/to/app-content"
    }
  ]
}
```

#### Example `config.toml` with defined `appleItunesApp` and `ampManifest`

```toml
[params]
    appleItunesApp = "app-id=123456789, app-argument=app-name://link/to/app-content"
    ampManifest = "/amp-manifest.json"
```
