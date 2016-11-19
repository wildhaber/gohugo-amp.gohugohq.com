+++
date = "2016-11-18T19:28:41+02:00"
draft = false
title = "Structured Data: Recipe"

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
  
+++

# Recipe

Mark up your recipe content with structured data to provide rich cards and host-specific lists for your recipes, such as reviewer ratings, cooking and preparation times, and nutrition information.

### Recipe-Front-Matters

Recipe structured data are rendered and defined by the front-matters of your content. Following you will find an [example recipe](/examples/recipes/first-recipe/) with and its output in the structured data:

```toml
date = "2016-11-18T19:28:41+02:00"
publishdate = "2016-11-18T19:28:41+02:00"
draft = false
title = "course example one"
description = "Short description of the course."

[amp]
    elements = []
    
[structured]
    type = "Recipe"

[author]
    name = "John Doe"

[recipe]
    category = "appetizer"
    prepTime = "PT30M"
    totalTime = "PT3H"
    recipeYield = "8"
    ingredients = ["1 box Pillsbury™ refrigerated pie crusts, softened as directed on box","6 cups thinly sliced, peeled apples (6 medium)","3/4 cup sugar","2 tablespoons all-purpose flour","3/4 teaspoon ground cinnamon","1/4 teaspoon salt","1/8 teaspoon ground nutmeg","1 tablespoon lemon juice"]
    instructions = ["1 Heat oven to 425°F. Place 1 pie crust in ungreased 9-inch glass pie plate. Press firmly against side and bottom.","2 In large bowl, gently mix filling ingredients; spoon into crust-lined pie plate. Top with second crust. Wrap excess top crust under bottom crust edge, pressing edges together to seal; flute. Cut slits or shapes in several places in top crust.","3 Bake 40 to 45 minutes or until apples are tender and crust is golden brown. Cover edge of crust with 2- to 3-inch wide strips of foil after first 15 to 20 minutes of baking to prevent excessive browning. Cool on cooling rack at least 2 hours before serving."]
    
[rating]
    value = "4.0"
    reviewCount = "12"
    best = "4.5"
    worst = "2.5"

[nutrition]
    "servingSize" = "1 medium slice"
    "calories" = "230 calories"
    "fatContent" = "1 g"
    "carbohydrateContent" = "43 g"
    "cholesterolContent" = "0 mg"
    "fiberContent" = "1 g"
    "proteinContent" = "1 g"
    "saturatedFatContent" = "2 ½ g"
    "sodiumContent" = "200 mg"
    "sugarContent" = "27 g"
    "transFatContent" = "0 g"

[image]
    src = "https://gohugo-amp.gohugohq.com/example-square.jpg"
    width = 900
    height = 900
    title = "Example Square image"
    author = "gohugohq"
    link = "https://gohugohq.com"
    license = "CC BY 2.0"
    license_link = "https://creativecommons.org/licenses/by/2.0/"

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
```

This will generate the following **valid structured data** in the head-section:

```javsacript
<script type="application/ld+json">
{
  "@context": "http://schema.org",
  "@type": "Recipe",
  "name": "course example one",
  "description": "Short description of the course.",
  "recipeCategory": "appetizer",
  "author": {
    "name" : "John Doe"
  },
  "description": "Short description of the course.",
  "datePublished" : "2016-11-18T19:28:41",
  "dateModified" : "2016-11-18T19:28:41",
  "prepTime": "PT30M",
  "totalTime": "PT3H",
  "recipeYield": "8",
  "recipeIngredient": ["1 box Pillsbury™ refrigerated pie crusts, softened as directed on box","6 cups thinly sliced, peeled apples (6 medium)","3/4 cup sugar","2 tablespoons all-purpose flour","3/4 teaspoon ground cinnamon","1/4 teaspoon salt","1/8 teaspoon ground nutmeg","1 tablespoon lemon juice"],
  "recipeInstructions": ["1 Heat oven to 425°F. Place 1 pie crust in ungreased 9-inch glass pie plate. Press firmly against side and bottom.","2 In large bowl, gently mix filling ingredients; spoon into crust-lined pie plate. Top with second crust. Wrap excess top crust under bottom crust edge, pressing edges together to seal; flute. Cut slits or shapes in several places in top crust.","3 Bake 40 to 45 minutes or until apples are tender and crust is golden brown. Cover edge of crust with 2- to 3-inch wide strips of foil after first 15 to 20 minutes of baking to prevent excessive browning. Cool on cooling rack at least 2 hours before serving."],
  "aggregateRating" : {
      "@context": "http://schema.org",
      "@type": "AggregateRating",
      "ratingValue": "4.0",
      "reviewCount": "12",
      "bestRating": "4.5",
      "worstRating": "2.5"
  },
  "image" : {
      "@context": "http://schema.org",
      "@type": "ImageObject",
      "author": "gohugohq",
      "url": "https:\/\/gohugo-amp.gohugohq.com\/example-square.jpg",
      "datePublished": "2016-11-18T19:28:41",
      "name": "Example Square image",
      "height" :  900 ,
      "width" :  900 ,
      "license" : "https:\/\/creativecommons.org\/licenses\/by\/2.0\/",
      "isBasedOn" : "https:\/\/gohugohq.com"
    },
  "nutrition": {
    "@type": "NutritionInformation",
    "servingSize": "1 medium slice",
    "calories": "230 calories",
    "fatContent": "1 g",
    "carbohydrateContent": "43 g",
    "cholesterolContent": "0 mg",
    "fiberContent": "1 g",
    "proteinContent": "1 g",
    "saturatedFatContent": "2 ½ g",
    "sodiumContent": "200 mg",
    "sugarContent": "27 g",
    "transFatContent": "0 g"
  }
}
</script>
```