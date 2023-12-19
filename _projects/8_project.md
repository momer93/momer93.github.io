---
layout: page
title: The Frugal 3D printer
description: Replicating an open source 3D printer in Oman
img: assets/img/f3dp/f3dp2.png
importance: 3
category: work
giscus_comments: true
---

This project was a result of a comparative research project whereby I was exploring the concept of replicability of open source machine tools using the case study of the peviously used 3D printer design. The project was carried out to empirically determine the challenges to replicating a fully open source design in a resource constrained context.

Even though the design was affordable in Germany at about 650 Euros for the whole kit and was relatively easy to replicate. When exploring its replicaiton in Oman, it turned out to be really difficult to source most of the components locally. The electronics and small hardware components could be imported from China via aliexpress. However, to import heavier parts such as the slotted aluminium profiles was prohibitively expensive whereby shipping alone costed 2 times the parts price.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/f3dp/buying_profiles_china.png" title="Buying alu profiles from china" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Cost of importing aluminium slotted profiles for the 3d printer from china
</div>

Therefore, the design had to be slightly adapted in order for the machine to be replicated in Oman. The only available local alternative was to use steel square hollow sections. The problem here was assembling firstly the frame together and then mounting the various components on the frame. For the slotted aluminium profile this was rather easy, since any part could be mounted along any of the profile faces by simply inserting a so-called hammer nut. Moreover the frame could be completely put together without drilling any holes. With the lack of this slot on the steel profiles, a new method of mounting everything would have to be derived.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/f3dp/frame_004.png" title="frame" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/f3dp/View54.png" title="Mounting part on frame" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: T slotted profiles assembly of frame, Right: Mounting components on frame with hammer nuts
</div>

The first iteration of the frame fabrication involved welding the frame together using the same dimensions as the original slotted profile design. Even though warping is normally a concern with welding, done with the right jigs, tools and technique, warping can be avoided. On asking the microenterprise workers if they could weld the frame together according to the dimensions without any warp, they said they could since they welded frames all day long.

The welded frame cost about 10 euros and took about an hour. This was significantly cheaper than importing the slotted profiles from China, which would have cost about 450 euros just for the frame. This is price difference of atleast 45! However, on measuring the warp on the steel frame, it was noticed that there was sigificant dimensional errors in the frame. This would not work for a 3D printer design due to the high precision required in the process.

Therefore next, it was decided to use a bolting strategy instead of welding the frame together. This was much more labour and time intensive, however the frame could be assembled with much better accuracy and tolerances. The new design required 31 brackets and about 372 holes to be drilled. The holes were made slightly bigger than the bolt size, so for M6 bolts, the holes were 7mm in diameter. This would allow the frame profiles to be adjusted during assembly incase the holes were not accurately spaced.  As one can imagine this was highly time intensive and not the ideal solution. However, once the frame was built, the remaining parts could be mounted by similarly drilling further holes for each mounting point.

Even the bolting method was fraught with difficulties in accurately drilling the holes. This was because the microenterprise workers possessed no jigs or flat surfaces to work on. Moreover, they did not use vernier calipers but just a tape measure for all their work. Therefore, for accurately marking the holes, paper templates were printed which could be placed on the profiles and the hole centers marked with a center punch.

Most functional parts and brackets on the 3d printer were designed to be 3d printed in the original design. 3D printing services could not be found locally and only a few relatively new startups offered 3d printing as a service, but their prices were too high to realistically build the printer within budget. There were also no local makerspaces or places where 3d printing could be carried out. Moreover, no shops sold 3d printers either. A local university was then approached to print the parts as part of a research project and the parts could be printed. 3D printing is not really an ideal process for such economies where 3d printing is not as ubiquitous as in the global north. Moreover, it is counterintuitive to have to 3d print parts to build a 3d printer.

- Use case of the broken electrical connector clip
- Redesign of the 3d printer to be built locally with co-design with local potential end users.