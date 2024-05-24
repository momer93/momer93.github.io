---
layout: page
title: A frugal CNC Oxyfuel Cutter
description: An open source CNC gas cutter for resource constrained settings
img: assets/img/gcp/gc1.JPG
importance: 1
category: work
related_publications: 10.1007/978-3-031-28839-5_97, https://doi.org/10.15488/12154
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gas_cutter_cad.png" title="CNC gas cutter in action" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Cad model of the CNC oxyfuel cutter
</div>

A frugal [CNC oxyfuel cutter](https://momer93.github.io/cnc-gas-cutter/) was designed for metal fabrication microenterprises. Such microenterprises often fabricate metal structural and non-structural goods such as warehouses, car park shades, furniture, signage and custom parts. An oxyfuel cutter is one of the oldest cutting processes used in the steel industry and is used to cut metal plates ranging from 4 mm up to 50+ mm thick. Parts cut out are often simple shapes such as circles, triangles and rectangles. Even though oxyfuel cutting has been mechanized in industry, such machines are usually much too expensive, locally unavailable and often overengineered for the needs of small microenterprises.

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
    Pictures of some steel fabrication microenterprises in Oman
</div>

When repetitive parts were required that were not simple rectangles, such as circles or more complex shapes such as stiffeners. The workers went through a tedious process of drawing a shape on a thin metal sheet, cutting it out, laying the template onto the metal plate to be cut and marking it with chalk, followed by manual gas cutting using a hand held oxyfuel cutter and finally post-processing.

The part edges were often uneven with excessive dross. This had to be corrected by extensive grinding using a hand held grinder. Therefore, the entire cutting process was inefficient, often tedious, time-consuming and mundane, specially for large batches of repititive shapes. With some workers revealing stories of gas explosions while cutting, the process was also dangerous. In terms of increased efficiency and reducing manual labour, the gas cutting process was determined to benefit significantly from process automation.

The project was started by carrying our a field visit to manufacturing microenterprises in the industrial cluster of Wadi Kabir Sanaya in the city of Muscat. The cluster has a pre-dominantly dense population of migrant run manufacturing microenterprises. Due to limited online and telecommunication opportunities of the microenterprises, interviews with the respondents were carried out face to face at their sites of business. The respondents were all male migrants from the South Asian countries of Pakistan, India, and Bangladesh. Semi-structured interviews and field observations were carried out to gain an understanding of the technology needs and readiness levels of the target group. Talking with the shop owners revealed insights into their available resources, educational backgrounds and day to day lives. Most had small workshop spaces which were not more than 15-20 square meters. They were all open air workshops with no climate control and dust being everywhere. They seldom had the time to work on such projects due to working 6 days a week, 12 hours each day. This mean't they rarely had free time and therefore it was imperative to find a company that would be willing to help with the build during their work hours.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc2.jpg" title="Interviews_1" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc3.jpg" title="Interviews_2" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc4.jpg" title="Interviews_3" class="img-fluid rounded z-depth-1" %}
</div>
</div>
<div class="caption">
    Interviewing owners and workers from various steel fabrication microenterprises in Oman.
</div>

Next interviews were carried out with the end users to determine key design requirements. The requirements for smaller shops compared to bigger shops were slightly different. Smaller shops often had very little space in the shop and did not often have production runs that needed the cutting of multiple plates. Such shops often wanted just the cheapest possible machine (max budget 500 euros), with portability or the function of stowing away to be important. Slightly bigger shops were willing to spend more for reliability and quality (max budget upto 3000 euros). 

**Key points learned from the interviews were:**
1. Plate thicknesses they normally cut with a gas cutter range from 3 to 40 mm.
2. They sometimes cut scrap cut pieces which are much smaller than a full sheet and sometimes also a full sheet
3. Due to the weight of full sheets, they are unable to carry them, so cut them where they are unloaded by a vendor often outside the shop.
4. They do not having cutting jobs all the time, so it is preferable for smaller shops to be able to stow the machine away to make more space when not needed
5. For small jobs they would prefer to cut with the hand torch and so the torch should be removable from the CNC machine
6. They preferred to purchase as little as possible and would like to use as much locally available material in the workshop than to buy exotic profiles or parts

Such findings allowed me to determine the right strategy for the design. Next a survey was made of all available local raw material sizes and listed in an indexable spreadsheet along with pricing, such that only locally available material would be used in the design, atleast for the machine structure. 

Next several concepts were generated for the machine by sketching on paper, making basic calculations on excel sheets etc. Next the chosen profiles and design was modelled in CAD. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc10.png" title="Materials list" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    List of locally available raw materials
</div>

Through qualitative interviews, it was determined how they would normally use such a machine, what sizes and thicknesses of plate would they be normally cutting etc. 



The first proof of concept that was built in Oman was a low fidelity prototype. This was done to keep costs low and figure out the viability of the design quickly. The machine frame was designed from 2" (50mm) square steel profiles with a thickness of 2mm. These profiles were usually in surplus in such workshops, therefore even if there were leftovers, they could be reused in other projects.

When asked about the need for more automated machines, they often complained about the lack of space because they imagined CNC or automated machine tools must be really big as industrial machines normally are. Most small shops had 2-3 workers and none of the workshops observed had any CNC machine tools. Those that did possess machine tools, these were usually manual lathes that were often purchased used. None of them carried out precision work, so they usually produced structural (car park shades, warehouses etc) and non-structural items (gates, staircases, railings, furniture etc.) None of them had access to CNC machine tools and had no idea about CAD or CAM. A few pictures of such open air workshops below.

As a next step various manufacturing processes within such workshops were observed to determine possible processes that could be automated. Gas cutting was chosen due to its potential for increased efficiency and productivity for the users. From the interviews it was revealed that due to the lack of space, users would prefer something that could be easily stowed away when not needed and most importantly they needed the machine to be as cheap as possible. Many estimated that they would be able to afford the machine if it were to cost between 500 and 800 USD. Bigger shops that had more employees and access to bigger jobs had a higher budget of about 2000-3000 USD. Next functional requirements were derived depending on the surveyed local resources from local shops such as available raw materials and other mechanical and electronic components.

The biggest constraints for this project were the materials and components availability. Starting with the frame, the cheapest materials available was mild steel hollow sections, rolled profiles and plates. Aluminum was almost impossible to find. Oman doesn't really have marketplaces for hobby components like electronics, motors or other components required for machine building. Online stores do exist but they are mainly selling consumer appliances.

This means it is almost impossible to find parts for building smaller machines such as M3 and smaller screws or other standard machine elements. There are new stores coming up to cater to the needs of spare parts for chinese machine tools that many are importing from China. However, these are more for industrial scale machines. The only way was to visit several local shops and make a list of commonly available materials. I listed these on an excel sheet along with their prices. This list constrained my available materials for use in the design. Next on discussions with the workshop workers and owner, we found there were a select few profiles, plates or bars that were often in surplus in the workshops since they used these often for fabrication jobs. They would prefer to use these than to have to buy one off exotic profiles. These field searches and discussions with the end user helped inform the choice of materials and parts for the design.

The design started with paper sketches, internet searches and some rough calculations on paper before progressing onto CAD. The linear guides were the defining machine element that decided the final machine design since most conventional linear bearings such as linear rails, profile linear guides, rack and pinion etc were not locally available. These would also be expensive to source on international B2C ecommerce platforms like aliexpress due to the excessive shipping costs owing to their weight. There were some local shops selling linear profile guides but these were for larger industrial machines and were far too expensive to stay within the budget requirements. Therefore a simple linear bearing concept made of radial roller bearings mounted on bolts as axles was used for the X and Y cartesian motion. The bearing setup can be preloaded by simply tightening the bolts and this way can also account for profiles with varying dimensional tolerances.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/x2.png" title="Linear carriage model" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Cad model of the linear carriage design
</div>

The Z axis setup was responsible for raising and lowering the torch and actuating the oxygen lance lever. Conventionally, one uses a machine torch for such automation applications since they are vertical and easy to mount and fasten onto a CNC Z axis carriage, however these were not locally available and would have to be imported which had high shipping costs due to its weight and the end users said in interviews that they preferred to not buy another torch and it would be optimal if they could just use the torch the had on hand. Also in case someone had to buy the machine, the hand actuated torch could be sourced locally.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/x3.png" title="Z axis model" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Cad model of the Z-axis
</div>

The machine was completely fabricated and assembled in the microenterprise in Oman. The fabrication of the individual components faced several challenges. The workers could not dimension parts accurately by just reading them off a drawing and so templates of holes or cut outs were printed to scale on paper. The shapes were then cut out and glued onto the metal. A center punch was used to hammer the center points of the holes and these were then drilled on a drill press.

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

For the design to be as affordable as possible, a frugal design approach with a participatory design approach was chosen. A frugal design is one that focuses on the essential and core components for the machine to be functional. A participatory approach of the Co-design type, involves the end user during the design and/or prototyping phase. The workers gave several inputs during the design phase (user centered approach). Since the machine was built with the end users in the microenteprise, they were directly involved in the prototyping phase (participatory co-design approach), whereby they often helped solved some challenges in fabrication and assembly. The level of user participation was progressively increased as the design progressed from the sketching and CAD model to the prototyping phase.


Below is a FRDPARRC table from Professor Slocum's book on Precision Design.


 | Functional Requirements (FR) | Design Parameters (DP) | Analysis | References | Risk | Countermeasures |
 | ---------------------------- | ----------------------|-----------|------------|------|-----------------|
 | Affordable design (<800USD) | use locally available materials, choose components with minimum required performance, don't overengineer | Most shop owners want cheap machines (interviews), Excel list of locally available raw materials | Interviews | Cheap parts might be unreliable and break |  Test parts before use in design |
 | Easy to fabricate | Use simple 2D shapes for parts to be manufactured, consider local manufacturing capabilities, print out to scale drawings and stick on flat parts for drilling or cutting operation, avoid bending | Users aren't used to precision manufacturing and so local capabilities need to be considered | Interviews, observations | Limited fabrication choice may reduce precision of parts and so machine final accuracy | Compromise between precision required and simplicity of fabrication process |  
 | Robust | Use materials not affected by harsh workshop environment (high temperatures in summer and open air workshops) | Avoid 3d printed plastic parts or wood in design, enclose electronics to safeguard from dust and iron particles | observations, experience | Might be difficult to get robust electronics in the required price range | Test suitability of electronics and build safety measures in design |


 The mechanical components (like belts, pulleys, leadscrews etc) and the electrical components (motors, microcontroller, endstops etc) were typical 3D printer components, which meant they were affordable and easily available. Moreover such microcontrollers could also use freely available open source software.