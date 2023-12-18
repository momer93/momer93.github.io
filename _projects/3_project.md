---
layout: page
title: Semi-automatic watering system
description: another without an image
img: /assets/img/hobby/xxx
importance: 3
category: fun
---

The watering setup uses an esp32 microcontroller board which is connected to a 8 channel relay board. The relays switch on 5V water pumps via buttons on a smartphone app. Soil moisture sensors are also connected to the plants that measure the soil moisture at regular intervals and show it as a percentage on the app. The ESP32 is connected to the home wifi and also added to the software homeassisstant which is installed on a raspberry pi central hub. The raspberry pi acts like a central hub and the esp32 as a node.

The reason I built this was becaue I found it really cumbersome begging my neighbour to water my plants, every time I was away from home for over a month. So i decided to build one with really cheap off the shelf components. I didn't want a system that would water my plants completely automatically, I actually wanted to water them myself depending on which plant actually needed it. Depending on the soil moisture readings, I pressed a button on the app and this switched on the pumps for a set duration of time and so I had full control and also enjoyed watering my plants, as I was in another country.

I designed the setup in Onshape. The esp32 casing was designed to be 3d printed, since it had to be a little complex. The rest of the parts were designed to be laser cut. I cut out the casing out of balsa wood and then painted it so it had some form of water resistance. Connectors were attached on one side to attach the 3 wire capacitive soil moisture sensors and the other side had the female connectors for the 5V pumps.

TailVPN was used to connect to my home internet when I was outside my home WiFi.

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}
```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %}
