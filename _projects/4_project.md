---
layout: page
title: Incremental Forming
description: Incremental forming of PVC
img: assets/img/spif/spif1.png
importance: 8
category: work
---

The aim of this project was to experimentally and numerically investigate the formability of PVC with single point incremental forming (SPIF). SPIF is a forming process whereby a flat sheet is gradually formed with a smooth rounded tool that forms a shape layer by layer.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/spif/spif1.png" title="Incremental forming" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The limitation with forming PVC sheets was the thinning that occured during the material flow while forming. This thinning caused the material to tear before a right angled wall could be achieved. The achievable angle was 65 degrees. This result was derived theoretically as well as experimentally. The aim of our work was therefore to determine an optimal tool path strategy to increase the theoretical forming limit of the current multipass toolpath strategy

<div class="caption">
    Single point incremental forming setup. <a href="#" class="https://robodk.com/blog/robotic-incremental-forming-savings/">source</a>  
</div>

For the experimental setup a 3 axis CNC machine was fitted with a special sheet clamping setup and a 8mm round nose tipped smooth tool was used for the forming process. The machine toolpath for the cone formation was generated using a simple excel program, with user input parameters to change the wall angle, depth of cone and tool increment. A design of experiments (DOI) experimental procedure was performed to test various parameter combinations.

In case, the part did not fracture or break during the forming process, a 3D scan of the formed sheet was made with a 3D stereoscopic camera system from the company Aramis. For the process, the formed sheets were cleaned of lubricaiton oil. Special locating stickers were stuck on various points of the sheet and 3D model of the scanned sheet was created.

Next, a section was made through the centre of the sheet in the 3D model. The thickness values were extracted for each scanned point on the sheet. These thickness values were extracted in a CSV file and plotted against the cut profile, to show the points with the most thinning.

