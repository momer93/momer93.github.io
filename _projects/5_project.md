---
layout: page
title: Incremental Forming
description: Incremental forming of PVC
img: assets/img/1.jpg
importance: 3
category: fun
---

The aim of this project was to experimentally and numerically investigate the formability of PVC with single point incremental forming (SPIF). SPIF is a forming process whereby a flat sheet is gradually formed with a smooth rounded tool that forms a shape layer by layer.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/spif/spif1.png" title="Incremental forming" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    Single point incremental forming setup. <a href="#" class="https://robodk.com/blog/robotic-incremental-forming-savings/">source</a>  
</div>

This was done by trying to achieve a 90 degree wall angle for a cup. The maximum wall angle that could have been achieved till then was 65degrees. Therefore the goal of the project was set to trying different toolpath strategies to achieve a 90 degree wall angle.

For the experimental setup a 3 axis CNC machine was fitted with a special sheet clamping setup and the a 8mm round nose tipped smooth tool was used for the forming process. The gcode for the cone formation was generated with an excel sheet, with formulas to change the wall angle, depth of cone and the tool increment. A DOI was performed to test various parameter combinations. 

Incase the part did not fracture or break during the forming process, a 3D scan of the formed sheet was made with a 3D stereoscopic camera system known as aramis. For the process, the formed sheets were cleaned of lubricaiton oil. Special locating stickers were stuck on various points of the sheet and 3D model of the scanned sheet was made up. Next, a section was made through the centre of the sheet in the 3D model. The thickness values were extracted for each scanned point on the sheet. These thickness values were extracted in a CSV file and plotted. These values


Every project has a beautiful feature showcase page.
It's easy to include images in a flexible 3-column grid format.
Make your photos 1/3, 2/3, or full width.

To give your project a background in the portfolio page, just add the img tag to the front matter like so:

---
layout: page
title: project
description: a project with a background image
img: /assets/img/12.jpg

---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
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
