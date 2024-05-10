---
layout: page
title: A frugal CNC Oxyfuel Cutter
description: An open source CNC gas cutter for resource constrained settings
img: assets/img/gcp/gc1.JPG
importance: 1
category: work
related_publications: 10.1007/978-3-031-28839-5_97, https://doi.org/10.15488/12154
---

# CNC Oxyfuel Cutter #

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc1.JPG" title="CNC gas cutter in action" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Picture of the machine working
</div>

A frugal [CNC oxyfuel cutter](https://momer93.github.io/cnc-gas-cutter/) was designed for small fabrication microenterprises in Oman. The design objective was to automate the oxyfuel cutting process that is commonly used in steel fabrication workshops around the world. The main design constraints were the cost, spatial constraints, use of local materials and local manufacturing capability.

## insert picture of a hand held oxyfuel cutter ##

The machine was designed to be as affordable as possible while being reliable enough to function in the harsh environments seen in Oman. The design is focused on being ultra affordable while being able to be built from resouces locally available to the microenterprises. Therefore this isn't a design for everyone but really tailored to be reproduced in Oman with simple tools and components. The cnc gas cutter design was chosen to explore the potential of frugally designed open source machine for its impact potential on the one hand and on the other hand to shed light on how frugal design for such resource constrained settings can work and what challenges can be faced.

The first proof of concept that was built in Oman was a low fidelity prototype. This was done to keep costs low and figure out the viability of the design quickly. The machine frame is made from standard 2" (50mm) square steel profiles which are usually in surplus in such workshops. The mechanical and electronic components are typical 3d printer components and were chosen due to their affordability and availability. 

The project was started by carrying our a field visit to manufacturing microenterprises in the industrial cluster of Wadi Kabir Sanaya in the city of Muscat. The cluster has a pre-dominantly dense population of migrant run manufacturing microenterprises. Due to limited online and telecommunication opportunities of the microenterprises, interviews with the respondents were carried out face to face at their sites of business. The respondents were all male migrants from the South Asian countries of Pakistan, India, and Bangladesh. Semi-structured interviews and field observations were carried out to gain an understanding of the technology needs and readiness levels of the target group. Talking with the shop owners revealed insights into their available resources, educational backgrounds and day to day lives. Most had small workshop spaces which were not more than 15-20 square meters. They were all open air workshops with no climate control and dust being everywhere. They seldom had the time to work on such projects due to working 6 days a week, 12 hours each day. This mean't they rarely had free time and therefore it was imperative to find a company that would be willing to help with the build during their work hours.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc2.jpg" title="Interviews_1" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc3.jpg" title="Interviews_2" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc4.jpg" title="Interviews_2" class="img-fluid rounded z-depth-1" %}
</div>
</div>
<div class="caption">
    Interviewing owners and workers from various steel fabrication microenterprises in Oman.
</div>

When asked about the need for more automated machines, they often complained about the lack of space because they imagined CNC or automated machine tools must be really big as industrial machines normally are. Most small shops had 2-3 workers and none of the workshops observed had any CNC machine tools. Those that did possess machine tools, these were usually manual lathes that were often purchased used. None of them carried out precision work, so they usually produced structural (car park shades, warehouses etc) and non-structural items (gates, staircases, railings, furniture etc.) None of them had access to CNC machine tools and had no idea about CAD or CAM. A few pictures of such open air workshops below.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc14.jpg" title="Workshop_1" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc15.jpg" title="Workshop_2" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc16.jpg" title="Workshop_3" class="img-fluid rounded z-depth-1" %}
</div>
</div>
<div class="caption">
    Pictures of some steel fabrication workshops in Oman
</div>

As a next step various manufacturing processes within such workshops were observed to determine possible processes that could be automated. Gas cutting was chosen due to its potential for increased efficiency and productivity for the users. From the interviews it was revealed that due to the lack of space, users would prefer something that could be easily stowed away when not needed and most importantly they needed the machine to be as cheap as possible. Many estimated that they would be able to afford the machine if it were to cost between 500 and 800 USD. Bigger shops that had more employees and access to bigger jobs had a higher budget of about 1500-2000 USD. Next functional requirements were derived depending on the surveyed local resources from local shops such as available raw materials and other mechanical and electronic components.

The biggest constraints for this project were the materials and components availability. Starting with the frame, the cheapest materials available was mild steel hollow sections, rolled profiles and plates. Aluminum was almost impossible to find. Oman doesn't really have marketplaces for hobby components like electronics, motors or other components required for machine building. Online stores do exist but they are mainly selling consumer appliances.

This means it is almost impossible to find parts for building smaller machines such as M3 and smaller screws or other standard machine elements. There are new stores coming up to cater to the needs of spare parts for chinese machine tools that many are importing from China. However, these are more for industrial scale machines. The only way was to visit several local shops and make a list of commonly available materials. I listed these on an excel sheet along with their prices. This list constrained my available materials for use in the design. Next on discussions with the workshop workers and owner, we found there were a select few profiles, plates or bars that were often in surplus in the workshops since they used these often for fabrication jobs. They would prefer to use these than to have to buy one off exotic profiles. These field searches and discussions with the end user helped inform the choice of materials and parts for the design.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc10.png" title="Materials list" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Snapshot of the materials excel sheet
</div>

The design started with paper sketches, internet searches and some rough calculations on paper before progressing onto CAD. The linear guides were the defining machine element that decided the final machine design since most conventional linear bearings such as linear rails, profile linear guides, rack and pinion etc were not locally available. These would also be expensive to source on international B2C ecommerce platforms like aliexpress due to the excessive shipping costs owing to their weight. There were some local shops selling linear profile guides but these were for larger industrial machines and were far too expensive to stay within the budget requirements. Therefore a simple linear bearing concept made of radial roller bearings mounted on bolts as axles was used for the X and Y cartesian motion. The bearing setup can be preloaded by simply tightening the bolts and this way can also account for profiles with varying dimensional tolerances.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/x2.png" title="Linear carriage model" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Cad model of the linear carriage design
</div>

The Z axis setup was the most complex part of the machine since a typical manual gas cutter torch had to be mounted and the lever actuated. Conventionally, one uses a machine torch for such applications since they are vertical and easy to mount and fasten onto a CNC Z axis carriage, however these were not locally available and would have to be imported which had high shipping costs due to its weight and the end users said in interviews that they preferred to not buy another torch and it would be optimal if they could just use the torch the had on hand. Also in case someone had to buy the machine, the hand actuated torch could be sourced locally.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/x3.png" title="Z axis model" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Cad model of the Z-axis
</div>

The machine was completely fabricated and assembled in the microenterprise in Oman. The fabrication of the individual components faced several challenges due to several reasons. The workers could not dimension parts accurately by just reading them off a drawing and so templates of holes or cut outs were printed to scale on a simple A4 printer. The shapes were then cut out and glued onto the metal. A center punch was used to hammer the center points of the holes and these were then drilled on a drill press.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc11.JPG" title="paper template" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc12.JPG" title="Sticking the template onto part" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc13.JPG" title="Drilling holes" class="img-fluid rounded z-depth-1" %}
</div>
</div>
<div class="caption">
    Drilling holes in components with paper drawing templates
</div>

The final machine prototype can be seen below with its square profile frame construction and custom linear bearing guides.

#insert Cad of final design#

Below is a FRDPARRC table from Professor Slocum's book on Precision Design.


 | Functional Requirements (FR) | Design Parameters (DP) | Analysis | References | Risk | Countermeasures |
 | ---------------------------- | ----------------------|-----------|------------|------|-----------------|
 | Affordable design (<800USD) | use locally available materials, choose components with minimum required performance, don't overengineer | Most shop owners want cheap machines (interviews), Excel list of locally available raw materials | Interviews | Cheap parts might be unreliable and break |  Test parts before use in design |
 | Easy to fabricate | Use simple 2D shapes for parts to be manufactured, consider local manufacturing capabilities, print out to scale drawings and stick on flat parts for drilling or cutting operation, avoid bending | Users aren't used to precision manufacturing and so local capabilities need to be considered | Interviews, observations | Limited fabrication choice may reduce precision of parts and so machine final accuracy | Compromise between precision required and simplicity of fabrication process |  
 | Robust | Use materials not affected by harsh workshop environment (high temperatures in summer and open air workshops) | Avoid 3d printed plastic parts or wood in design, enclose electronics to safeguard from dust and iron particles | observations, experience | Might be difficult to get robust electronics in the required price range | Test suitability of electronics and build safety measures in design |

