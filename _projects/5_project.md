---
layout: page
title: Incremental Forming
description: Incremental forming of PVC
img: assets/img/spif/spif1.png
importance: 3
category: work
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

This was done by trying to achieve a 90 degree wall angle for a cup. The maximum wall angle that could have been achieved till then was 65 degrees. Therefore the goal of the project was set to trying different toolpath strategies to achieve a 90 degree wall angle.

For the experimental setup a 3 axis CNC machine was fitted with a special sheet clamping setup and the a 8mm round nose tipped smooth tool was used for the forming process. The gcode for the cone formation was generated with an excel sheet, with formulas to change the wall angle, depth of cone and the tool increment. A DOI was performed to test various parameter combinations. 

Incase the part did not fracture or break during the forming process, a 3D scan of the formed sheet was made with a 3D stereoscopic camera system known as aramis. For the process, the formed sheets were cleaned of lubricaiton oil. Special locating stickers were stuck on various points of the sheet and 3D model of the scanned sheet was made up. Next, a section was made through the centre of the sheet in the 3D model. The thickness values were extracted for each scanned point on the sheet. These thickness values were extracted in a CSV file and plotted. These values


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