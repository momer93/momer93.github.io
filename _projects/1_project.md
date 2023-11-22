---
layout: page
title: CNC Oxyfuel Cutter
description: An open source CNC gas cutter for resource constrained settings
img: assets/img/GC1.jpg
importance: 1
category: work
related_publications: <
---

An automated oxyfuel cutter was designed for a migrant run steel fabrication microenterprise in Oman. The aim of the design is to automate the hand held oxyfuel cutter as seen in figure below. The machine was designed to be as affordable as possible while being reliable enough to function in the harsh environments seen in Oman. The design is focused on being ultra affordable while being able to be built from the local resouces available to the microenterprises. Therefore this isn't a design for everyone but really tailored to be reproduced in Oman with simple tools and components. The machine frame is made from standard square steel profiles which are locally available. The Motors, belt drive components and electronics are typical 3d printer components and were chosen due to their affordability and availability.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/GC1.jpg" title="Working Gas Cutter" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Working proof of concept of the CNC Oxyfuel Cutter
</div>

The project was started by carrying our a field visit to manufacturing microenterprises in the industrial cluster of Wadi Kabir Sanaya in the city of Muscat. The cluster has a pre-dominantly dense population of migrant run manufacturing microenterprises. Due to limited online and telecommunication opportunities of the microenterprises, interviews with the respondents were carried out face to face at their sites of business. The respondents were all male migrants from the South Asian countries of Pakistan, India, and Bangladesh. Semi-structured interviews and field observations were carried out to gain an understanding of the technology needs and readiness levels of the target group. Talking with the shop owners revealed insights into their available resources, educational backgrounds and day to day lives. Most had small workshop spaces which were not more than 15-20 square meters. They were all open air workshops with no climate control and dust being everywhere. When asked about the need for more automated machines, they often complained about the lack of space because they imagined CNC or automated machine tools must be really big as industrial machines normally are. Most small shops had 2-3 workers and none of the workshops observed had any CNC machine tools. Those that did possess machine tools, these were usually manual lathes that were often purchased used. None of them carried out precision work, so they usually produced structural (car park shades, warehouses etc) and non structural items (gates, staircases, railings, furniture etc.) None of them had access to CNC machine tools and had no idea about CAD or CAM. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/GC2.jpg" title="Interviews" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/GC3.jpg" title="Interviews" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/GC4.jpg" title="Interviews" class="img-fluid rounded z-depth-1" %}
</div>
</div>
<div class="caption">
    Interviewing owners and workers from various steel fabrication microenterprises in Oman.
</div>

As a next step various manufacturing processes within such workshops were observed to determine possible processes that could be automated. Gas cutting was chosen due to its potential for increased efficiency and productivity for the users. From the interviews it was revealed that due to the lack of space, users would prefer something that could be easily stowed away when not needed and most importantly they needed their the machine to be as cheap as possible. Many estimated that they would be able to afford the machine if it were to cost between 500 and 800 USD. Bigger shops that had more employees and access to bigger jobs had a higher budget of about 1500-2000 USD.Next functional requirements were derived depending on the surveyed local resources from local shops such as available raw materials and other mechanical and electronic components. Below is a FRDPARRC table from Professor Slocum's book on Precision Design.

| Functional Requirements (FR) | Design Parameters (DP) | Analysis | References | Risk | Countermeasures |
| ---------------------------- | ----------------------|-----------|------------|------|-----------------|
| Affordable design (<800USD) | use locally available materials, choose components with minimum required performance, don't overengineer | Most shop owners want cheap machines (interviews), Excel list of locally available raw materials | Cheap parts might be unreliable and break |  Test parts before use in design |
| Easy to fabricate | Use simple 2D shapes for parts to be manufactured, consider local manufacturing capabilities, print out to scale drawings and stick on flat parts for drilling or cutting operation, avoid bending | Users aren't used to precision manufacturing and so local capabilities need to be considered | Interviews, observations | Limited fabrication choice may reduce precision of parts and so machine final accuracy | Compromise between precision required and simplicity of fabrication process |  
| Robust | Use materials not affected by harsh workshop environment | | | | |

