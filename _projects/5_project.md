---
layout: page
title: A frugal CNC Router
description: A low cost and frugal design of a large format CNC router
img: assets/img/cncrout/router.jpg
importance: 3
category: work
---

- This is a low cost design for a CNC router designed to be as minimalistic as possible and can mill standard full sized sheets of wood, dibond, plastics etc.
- The key constraints for the design were affordability, use of local materials and the other typical engineering constraints such as reliability, robustness etc.
- However, owing to the fact that the machine was to be easily replicated by microenterprises in resource constrained settings, design for manufacturing and assembly had to also be considered
- Large format CNC routers that can accomodate an entire standard sheet (2.4m x 1.2m) are typically used in carpentry and signboards making where a milling cutter is used to either cut out shapes from dibond or plastic or as well as engrave complex designs in wood
- For the microenterprise involved in the case study, their aim was to capture more of the value chain of signboards fabrication.
- Currently they only manufacture the steel frame of the signboards, with the problem being the job is at the base of the value chain and so the least profitable
- Also since many fabrication microenterprises can easily manufacture the frames, along with freelance workers who can do such jobs in the open with just a welding machine, the market rate for such jobs is very low and the majority of the value within such products is captured in later steps of the production process
- The idea was to capture more of the value chain by being able to manufacture the individual letters, which would be impossible without access to a CNC router due to the complexity of the shapes involved
- Moreover when they do get jobs for signboards where they would have to cut out oval shapes or shapes of arrows from dibond sheet (aluminium-ABS sandwich panel), the task of marking the sheet and cutting it out with hand tools is tedious and not aesthetic, whereby they have recieved complaints from the customer that the work is not presentable
- There are no local producers of CNC routers and locally available ones are imports from China which are much too expensive for themn to afford
- Moreover the machines are also overly bulky and rigid, which is impossible to accomodate in their small shops.
- Therefore they were looking for an affordable as well as a portable machine that they could stow away when not being used

- The design of the CNC router was essentially an adaptation of the frugal oxyfuel cutter (put hyperlink to the gas cutter page here) design, whereby the frame and linear motion setup is the same.
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
{% endraw %} -->
