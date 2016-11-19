+++
date = "2016-11-06T21:05:25+01:00"
draft = false
publishdate = "2016-11-06T21:05:25+01:00"
tags = ["kitchen-sink","elements","shortcodes"]
title = "kitchen sink"

[amp]
    elements = ["amp-accordion","amp-ad","amp-anim","amp-analytics","amp-carousel","amp-iframe","amp-audio","amp-brid-player","amp-brightcove","amp-dailymotion","amp-dynamic-css-classes","amp-facebook","amp-fit-text","amp-form","amp-fx-flying-carpet", "amp-gfycat", "amp-image-lightbox", "amp-instagram","amp-jwplayer","amp-kaltura-player","amp-lightbox","amp-o2-player", "amp-pinterest", "amp-reddit", "amp-sidebar", "amp-social-share", "amp-soundcloud", "amp-springboard-player", "amp-sticky-ad", "amp-twitter", "amp-user-notification", "amp-vimeo", "amp-vine", "amp-youtube"]
    
[sitemap]
  changefreq = "monthly"
  filename = "sitemap.xml"
  priority = 0.5

+++

# Kitchen sink
A kitchen-sink is a showcase and test-page for all available elements.

## Second Header
Lorem ipsum dolor sit amet, [Kitchen Sink with AMP Elements](/kitchen-sink) consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

### Third Header
Lorem ipsum dolor sit amet, consetetur sadipscing elitr,  sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

### Fourth Header
Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

#### Fifth Header
Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

##### Sixt Header
Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

### FX-Flying-Carpet
{{% amp-fx-flying-carpet height="250" imgSrc="http://lorempixel.com/1600/900/sports/5/" imgWidth="800" imgHeight="450" %}}

```markdown
{\{% amp-fx-flying-carpet height="250" imgSrc="http://lorempixel.com/1600/900/sports/5/" imgWidth="800" imgHeight="450" %}\}
```

### Lists

 - Unordered
 - List
 - Example
 
 1. Ordered
 2. List
 3. Example
 
### Include (partial)
{{% partial "test/lipsum" %}}

```markdown
{\{% partial "test/lipsum" %}\}
```
 
### Images
{{% amp-image src="//placehold.it/350x350" srcset="//placehold.it/600x600 640w, //placehold.it/150x150 320w" height="300" width="300" layout="responsive" alt="Alternative Text" attribution="CC courtesy of placehold.it" %}}

```markdown
{\{%
    amp-image src="//placehold.it/350x350"
    srcset="//placehold.it/600x600 640w, //placehold.it/150x150 320w"
    height="300"
    width="300"
    layout="responsive"
    alt="Alternative Text"
    attribution="CC courtesy of placehold.it"
%}\}
```

### Lightbox
{{% amp-button onTap="my-custom-lightbox" text="Open my custom lightbox" %}}

```markdown
{\{% amp-button onTap="my-custom-lightbox" text="Open my custom lightbox" %}\}
```

{{% amp-lightbox id="my-custom-lightbox" %}}
# Hello Lightbox
Wow this is amazing.
{{% /amp-lightbox %}}

Lightbox content:

```markdown
{\{% amp-lightbox id="my-custom-lightbox" %}\}
# Hello Lightbox
Wow this is amazing.
{\{% /amp-lightbox %}\}
```

### Image Lightbox 
{{% amp-image-lightbox id="test-image-lightbox"  %}}
{{% amp-image src="https://placehold.it/300x150/cceeff/000000" onTap="test-image-lightbox" role="button" tabindex="0" layout="responsive" height="150" width="300" %}}
{{% amp-image src="https://placehold.it/600x300/cc00ff/000000" onTap="test-image-lightbox" role="button" tabindex="0" layout="responsive" height="300" width="600" %}}
{{% amp-image src="https://placehold.it/400x200/ccccff/000000" onTap="test-image-lightbox" role="button" tabindex="0" layout="responsive" height="200" width="400" %}}

```markdown
{\{% amp-image-lightbox id="test-image-lightbox"  %}\}
{\{% amp-image src="https://placehold.it/300x150/cceeff/000000" onTap="test-image-lightbox" role="button" tabindex="0" layout="responsive" height="150" width="300" %}\}
{\{% amp-image src="https://placehold.it/600x300/cc00ff/000000" onTap="test-image-lightbox" role="button" tabindex="0" layout="responsive" height="300" width="600" %}\}
{\{% amp-image src="https://placehold.it/400x200/ccccff/000000" onTap="test-image-lightbox" role="button" tabindex="0" layout="responsive" height="200" width="400" %}\}
```

### Fit-Text
{{% amp-fit-text layout="responsive" max="150" min="5" height="150" width="600" %}}The amp-fit-text component expects its content to be text or other inline content, but it can also contain non-inline content. For the given content the amp-fit-text will try to find the best font size to fit all of the content within the available space.{{% /amp-fit-text %}}

```markdown
{\{% amp-fit-text layout="responsive" max="150" min="5" height="150" width="600" %}\}
The amp-fit-text component expects its content to be text or other inline content, but it can also contain non-inline content. For the given content the amp-fit-text will try to find the best font size to fit all of the content within the available space.
{\{% /amp-fit-text %}\}
```

---

### Adsense
{{% amp-adsense width="300" height="250" slot="2195367133" %}}

```markdown
{\{% amp-adsense width="300" height="250" slot="2195367133" %}\}
{\{% amp-adsense width="320" height="50" slot="2195367133" sticky="true" %}\}
```

### User Notification
{{% amp-user-notification message="This is a custom message. For user notifications." dismiss="Oh, I see" %}}
```markdown
{\{% amp-user-notification message="This is a custom message. For user notifications." dismiss="Oh, I see" %}\}
```

### Iframe
{{% amp-iframe src="https://example.com" layout="responsive" width="450" height="300" resizable="true" sandbox="allow-scripts allow-same-origin" overflow="Read more!!!"  %}}
```markdown
{\{% amp-iframe src="https://example.com" layout="responsive" width="450" height="300" resizable="true" sandbox="allow-scripts allow-same-origin" overflow="Read more!!!"  %}\}
```

### Pixel
{{% amp-pixel src="//placehold.it/1x1" %}}
```markdown
{\{% amp-pixel src="//placehold.it/1x1" %}\}
```


---

### Twitter
{{% amp-twitter width="486" height="657" layout="responsive" tweet="585110598171631616" cards="hidden" %}}
```markdown
{\{% amp-twitter width="486" height="657" layout="responsive" tweet="585110598171631616" cards="hidden" %}\}
```

### Facebook
{{% amp-facebook width="300" height="400" href="https://www.facebook.com/zuck/posts/10102593740125791" layout="responsive" %}}
{{% amp-facebook-video width="680" height="400" href="https://www.facebook.com/zuck/videos/10102509264909801/" layout="responsive" %}}
```markdown
{\{% amp-facebook width="300" height="400" href="https://www.facebook.com/zuck/posts/10102593740125791" layout="responsive" %}\}
{\{% amp-facebook-video width="680" height="400" href="https://www.facebook.com/zuck/videos/10102509264909801/" layout="responsive" %}\}
```

### Instagram
{{% amp-instagram shortcode="fBwFP" width="400" height="400" layout="responsive" %}}
```markdown
{\{% amp-instagram shortcode="fBwFP" width="400" height="400" layout="responsive" %}\}
```

### Reddit
Post: {{% amp-reddit src="https://www.reddit.com/r/me_irl/comments/52rmir/me_irl/?ref=share&amp;ref_source=embed" layout="responsive" width="200" height="200" %}}
Comment: {{% amp-reddit-comment uuid="b1246282-bd7b-4778-8c5b-5b08ac0e175e" created="2016-09-26T21:26:17.823Z" parent="true" live="true" src="https://www.reddit.com/r/sports/comments/54loj1/50_cents_awful_1st_pitch_given_a_historical/d8306kw" layout="responsive" width="400" height="400" %}} 
```markdown
{\{% amp-reddit src="https://www.reddit.com/r/me_irl/comments/52rmir/me_irl/?ref=share&amp;ref_source=embed" layout="responsive" width="200" height="200" %}\}
{\{% amp-reddit-comment uuid="b1246282-bd7b-4778-8c5b-5b08ac0e175e" created="2016-09-26T21:26:17.823Z" parent="true" live="true" src="https://www.reddit.com/r/sports/comments/54loj1/50_cents_awful_1st_pitch_given_a_historical/d8306kw" layout="responsive" width="400" height="400" %}\} 
```

### Pinterest
Embed: {{% amp-pinterest url="https://www.pinterest.com/pin/99360735500167749/" layout="responsive" width="200" height="90" %}}
```markdown
{\{% amp-pinterest url="https://www.pinterest.com/pin/99360735500167749/" layout="responsive" width="200" height="90" %}\}
```
Pinit: {{% amp-pinterest-pin url="https://www.pinterest.com/pin/99360735500167749/" media="https://s-media-cache-ak0.pinimg.com/237x/a7/66/56/a76656e966b1958f568d63c3f1c05aec.jpg" description="this is a example description." width="40" height="20" %}} 
```markdown
{\{% amp-pinterest-pin url="https://www.pinterest.com/pin/99360735500167749/" media="https://s-media-cache-ak0.pinimg.com/237x/a7/66/56/a76656e966b1958f568d63c3f1c05aec.jpg" description="this is a example description." width="40" height="20" %}\} 
```
Follow: {{% amp-pinterest-follow profile="https://www.pinterest.com/kentbrew/" label="Folllowing me!" width="150" height="20" %}} 
```markdown
{\{% amp-pinterest-follow profile="https://www.pinterest.com/kentbrew/" label="Folllowing me!" width="150" height="20" %}\} 
```

### Social Share
{{% amp-social-share facebook="true" twitter="true" pinterest="true" linkedin="true" gplus="true" email="true" %}}
```markdown
{\{% amp-social-share facebook="true" twitter="true" pinterest="true" linkedin="true" gplus="true" email="true" %}\}
```

---

### Animation
{{% amp-anim width="300" height="250" attribution="The Go gopher was designed by Reneee French and is licensed under CC 3.0 attributions." src="https://ampbyexample.com/img/gopher.gif" placeholder="https://placehold.it/100x100/ff0000" %}}
```markdown
{\{% amp-anim width="300" height="250" attribution="The Go gopher was designed by Reneee French and is licensed under CC 3.0 attributions." src="https://ampbyexample.com/img/gopher.gif" placeholder="https://placehold.it/100x100/ff0000" %}\}
```

### Audio
{{% amp-audio width="300" height="35" src="https://ia801402.us.archive.org/16/items/EDIS-SRP-0197-06/EDIS-SRP-0197-06.mp3" mp3="https://ia801402.us.archive.org/16/items/EDIS-SRP-0197-06/EDIS-SRP-0197-06.mp3" ogg="//sample.ogg.fallback.ogg" autoplay="true" loop="true" muted="true" %}}
```markdown
{\{% amp-audio width="300" height="35" src="https://ia801402.us.archive.org/16/items/EDIS-SRP-0197-06/EDIS-SRP-0197-06.mp3" mp3="https://ia801402.us.archive.org/16/items/EDIS-SRP-0197-06/EDIS-SRP-0197-06.mp3" ogg="//sample.ogg.fallback.ogg" autoplay="true" loop="true" muted="true" %}\}
```

### Video

> to reduce loading time we have removed this live demonstration

```markdown
{\{% amp-video
    src="https://ampbyexample.com/video/tokyo.mp4"
    poster="https://ampbyexample.com/img/tokyo.jpg"
    width="480"
    height="270"
    layout="responsive"
    controls="true"
    autoplay="true"
    muted="true"
    loop="true"
    source="<source src='video/tokyo.mp4' type='video/mp4'><source src='video/tokyo.webm' type='video/webm'>"
 %}\}
```

---

### Soundcloud

> to reduce loading time we have removed this live demonstration

```markdown
{\{% amp-soundcloud height="300" track="243169232" visual="true" color="ff6600" %}\}
```

### Springboard-Player

> to reduce loading time we have removed this live demonstration

```markdown
{\{% amp-springboard-player height="320" width="180" layout="responsive" mode="video" site="261" content="1578473" player="test401" domain="test.com" items="10" %}\}
```

### O2P layer

> to reduce loading time we have removed this live demonstration

```markdown
{\{% amp-o2-player pid="579a115aa01b4d2db062aa85" bcid="545db032e4b0af1a81424b48" macros="m.playback=click" layout="responsive" width="320" height="180" %}\}
```

### Brid-Player

> to reduce loading time we have removed this live demonstration

```markdown
{\{% amp-brid-player partner="264" player="4144" video="13663" width="480" height="270" layout="responsive" %}\}
{\{% amp-brid-player partner="264" player="4144" playlist="1220" width="480" height="270" layout="responsive" %}\} 
```

### Brightcove

> to reduce loading time we have removed this live demonstration

```markdown
{\{% amp-brightcove account="906043040001" video="1401169490001" player="180a5658-8be8-4f33-8eba-d562ab41b40c" width="480" height="270" layout="responsive" %}\}
```

### Dailymotion

> to reduce loading time we have removed this live demonstration

```markdown
{\{% amp-dailymotion video="x2m8jpp" highlight="FF4081" logo="false" info="false" endscreen="false" sharing="false" start="44" width="480" height="270" layout="responsive"  %}\}
```

### JWPlayer

> to reduce loading time we have removed this live demonstration

```markdown
{\{% amp-jwplayer player="aBcD1234" media="5678WxYz" width="16" height="9" layout="responsive" %}\}
{\{% amp-jwplayer player="aBcD1234" playlist="5678WxYz" width="16" height="9" layout="responsive" %}\}
```

### Kaltura Player

> to reduce loading time we have removed this live demonstration

```markdown
{\{% amp-kaltura-player uiconf="33502051" partner="1281471" entry="1_3ts1ms9c" streamerType="auto" width="480" height="270" layout="responsive" %}\}
```

### Gfycat

> to reduce loading time we have removed this live demonstration

```markdown
{\{% amp-gfycat id="FeistyBiodegradableBlackfish" layout="responsive" width="150" height="150"  %}\}
```

### Hulu (disallowed) 

> to reduce loading time we have removed this live demonstration

```markdown
{\{% amp-hulu id="Bx6H30RBVFNpOe-iiOxp3A" layout="responsive" width="412" height="213" layout="responsive" %}\}
```

### Vimeo

> to reduce loading time we have removed this live demonstration

```markdown
{\{% amp-vimeo width="480" height="270" layout="responsive" video="27246366" %}\}
```

### Youtube

> to reduce loading time we have removed this live demonstration

```markdown
{\{% amp-youtube width="480" height="270" layout="responsive" video="9XIRDtQgVX4" %}\}
```

---

### Google-VRView-Image (experimental)

> to reduce loading time we have removed this live demonstration

```markdown
{\{% amp-google-vrview-image src="https://storage.googleapis.com/vrview/examples/coral.jpg" width="400" height="300" stereo="true" yaw="15" layout="responsive" %}\}
```
