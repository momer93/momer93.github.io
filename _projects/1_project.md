---
layout: page
title: A frugal CNC Oxyfuel Cutter
description: An open source CNC gas cutter for resource constrained settings
img: assets/img/gcp/gc1.JPG
importance: 1
category: work
related_publications: 10.1007/978-3-031-28839-5_97, https://doi.org/10.15488/12154
---

## Overview

A frugal, open-source CNC oxyfuel cutter designed for metal fabrication microenterprises in Oman.

Small workshops there routinely cut thick steel plates (3–50+ mm) for warehouses, car park shades, furniture, signage, and custom parts. Today this is done manually with handheld gas torches: slow, hazardous, and inconsistent. Industrial CNC gas cutters exist, but they are far too expensive, overdimensioned, and rarely available locally.

This project explores how a **compact, locally fabricable CNC oxyfuel cutter** can make automated cutting accessible in such resource-constrained contexts.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc14.jpg" title="Steel fabrication microenterprise" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc15.jpg" title="Workshop environment" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc16.jpg" title="Typical workspace layout" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Steel fabrication microenterprises in Oman – small, open-air, highly constrained spaces.
</div>

---

## Problem & Context

The work began with field visits to the industrial cluster of Wadi Kabir Sanaya in Muscat, Oman. These workshops:

- Are typically **15–20 m²**, open-air, dusty, and without climate control.  
- Are run by **2–3 migrant workers** from Pakistan, India, and Bangladesh.  
- Operate **6 days a week, ~12 hours per day**, leaving almost no time for side projects.  
- Rarely own any CNC machinery; some have used manual lathes bought second-hand.  
- Have **no experience with CAD/CAM** and limited access to precision components.

When asked about automation, owners often imagined huge, expensive “factory-scale” CNC machines that would not fit their shops or budgets. Yet their day-to-day work clearly includes **highly repetitive plate cutting tasks** that would benefit from automation.

Key findings from early interviews and observations:

1. Typical plate thicknesses range from **3 to 40 mm** and beyond.  
2. They cut both full sheets (e.g. 2.4 m × 1.2 m) and smaller scrap plates.  
3. Full sheets are too heavy to move; cutting often happens where the sheet is dropped, sometimes outside the workshop.  
4. Cutting repetitive shapes is **tedious, time-consuming, and dangerous**.  
5. Small shops need a machine that can be **stowed away** when not in use.  
6. Workers want to keep using **their existing handheld torches**, not import special machine torches.  
7. They prefer to use **surplus workshop stock** rather than “exotic” profiles and components.

Altogether, gas cutting emerged as a **high-impact candidate for frugal automation**.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc2.jpg" title="Interview with workshop owner" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc3.jpg" title="Discussing current cutting practices" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc4.jpg" title="Observing manual oxyfuel cutting" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Semi-structured interviews and field observations with microenterprise owners and workers.
</div>

---

## Design Goals

From the fieldwork and discussions, two main target groups emerged:

- **Smaller shops**  
  - Very limited space  
  - Irregular cutting jobs, small batches  
  - Budget: **≈ 500–800 USD**  
  - Priority: simple, cheap, and stowable

- **Larger shops**  
  - More employees, larger and more frequent cutting jobs  
  - Budget: **≈ 2000–3000 USD**  
  - Priority: robustness and reliability

Across both, the key functional goals were:

- **Affordable**: stay within local budget constraints  
- **Locally fabricable**: use materials and components obtainable in the local ecosystem  
- **Compact & stowable**: not permanently occupy precious floor space  
- **Safer & more consistent** than manual cutting  
- **Compatible with handheld torches** and local work practices  

---

## Frugal & Participatory Design Approach

The project follows a **frugal, participatory co-design** approach:

- **Frugal design**  
  - Focus on essential functions, avoiding overengineering  
  - Use surplus **mild steel profiles, plates and bars**  
  - Avoid reliance on aluminum, precision rails, or specialized machine elements that are expensive or unavailable locally  

- **Participatory co-design**  
  - Workers and owners are involved in shaping requirements, reviewing concepts, and suggesting fabrication methods.  
  - The prototype is **built inside a microenterprise**, using their tools, skills, and constraints as design inputs.  
  - Complex subassemblies (e.g. the Z-axis) are co-designed and prototyped together, leveraging the workers’ fabrication experience.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc10.png" title="Locally available materials" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Survey of locally available raw materials – design constrained to what can realistically be sourced and reused.
</div>

---

## Technical Direction (High-Level)

Without going into publication-level detail, the current prototype explores:

- A **steel-frame structure** based on common 2" (50 mm) square hollow sections.  
- **Simple roller-based linear guidance**, using radial bearings and profiles obtainable locally.  
- A Z-axis concept that can handle a **standard handheld torch** rather than a specialized machine torch.  
- Fabrication strategies that match local skills, such as:
  - Printing **1:1 paper templates** for drilling patterns  
  - Using center punching and drill presses rather than precision CNC machining  

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gas_cutter_cad.png" title="CNC gas cutter CAD model" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    CAD model of the frugal CNC oxyfuel cutter tailored to local materials and capabilities.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc11.JPG" title="Paper drilling template" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc12.JPG" title="Template applied to metal" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gcp/gc13.JPG" title="Drilling based on templates" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Using printed 1:1 templates to support precise drilling with available tools.
</div>

The electronics and motion components build on **widely available, low-cost modules** (e.g. from the 3D printer ecosystem), enabling affordable motion control and integration with open-source software.

---

## Current Status & Publication

A first functional prototype has been designed and built in collaboration with a local workshop in Oman. The machine is undergoing further refinement and evaluation.

More detailed technical analysis, design rationale and performance results are part of an ongoing journal submission.  
Once published, the corresponding article and open documentation will be linked here.

---

## Gallery

(Additional build photos, cutting tests, and workshop impressions can be added here.)

