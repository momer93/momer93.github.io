---
layout: page
title: A frugal 3D Printer Design
description: A 3d printer design for low resource settings
img: assets/img/3dp1.png
importance: 2
category: work
giscus_comments: true
---

This 3D printer is a remix of the thingiverse user Scott_3D's hypercube evolution design. The project started out with the intention of carrying out machine build workshops in Hamburg, Germany. The initial 3D printer design was not enclosed and the electronics were outdated. I modified it to be fully enclosed, revamped the electronics and changed the dual z axis drives to a single motor driven Z axis. Moreover, I made a lego like instruction manual such that the printer could be replicated by laypersons in a 2 day build workshop. 10 such workshops were carried out in various institutions throughout hamburg. I personally prepared all the printer build kits that means procuring all the components, printing all the parts and packing them all in labelled packets.

---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3dp2.png" title="original 3d printer" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3dp3.png" title="modified 3d printer" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Original 3d printer design - Right: Modified 3d printer design
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal its glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


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
