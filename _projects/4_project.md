---
layout: page
title: Incremental Forming
description: Incremental forming of PVC
img: assets/img/spif/spif1.png
importance: 8
category: work
---

## Overview

This project, completed during my master’s studies in Manufacturing Engineering at TU Dortmund, investigated the **formability of PVC sheets using Single Point Incremental Forming (SPIF)**—an emerging dieless forming process in which a sheet is shaped gradually by a smooth, rounded tool following a programmed toolpath.

SPIF is attractive for prototyping and low-volume production due to its flexibility, but polymeric materials such as PVC often suffer from excessive thinning during deformation. Understanding and improving this formability limit was the focus of the work.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/spif/spif1.png" title="Incremental forming setup" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Single point incremental forming of a PVC sheet.
</div>

---

## Problem & Motivation

PVC sheets exhibit significant **thinning during material flow** in SPIF, leading to early fracture before steep wall angles can be achieved.

- Theoretical and experimental tests showed a maximum achievable wall angle of **≈ 65°** for the chosen material and process parameters.  
- The goal of this project was therefore to explore **alternative toolpath strategies** that could increase the theoretical forming limit beyond this angle.

This required a combined **experimental + numerical** approach to understand how different parameters influence thinning, strain distribution, and failure.

---

## Experimental Setup

The forming trials were conducted on a **3-axis CNC milling machine** equipped with:

- A custom sheet clamping fixture  
- An **8 mm diameter rounded SPIF tool**  
- A programmable toolpath for conical geometries

Toolpaths were generated using a simple Excel-based script allowing user-defined inputs such as:

- Wall angle  
- Depth of the cone  
- Vertical step size / tool increment  

A **Design of Experiments (DoE)** methodology was used to evaluate multiple parameter combinations and observe their influence on fracture behavior and wall-angle capability.

---

## Measurement & Analysis

When a forming test completed without fracture, the resulting geometry was digitized using an **ARAMIS 3D stereoscopic camera system**.

Workflow:

1. The formed PVC sheet was cleaned of lubrication residues.  
2. Reference markers were applied to the surface for tracking.  
3. A 3D scan was generated and exported as a mesh model.  
4. A mid-section of the formed shape was extracted.  
5. Thickness values along this section were exported as CSV data.  
6. The values were plotted to identify **regions of critical thinning**.

This enabled a precise comparison between:

- Theoretical predictions  
- Experimental deformation patterns  
- The impact of different toolpath strategies on thinning behavior  

---

## Outcome

The work identified the **critical material limits** for SPIF of PVC under the tested conditions and demonstrated how toolpath adjustments can influence thinning distributions.  
The experiments confirmed the expected forming limit of around **65°**, providing a baseline for further optimization through multipass strategies or process modification.

More detailed numerical simulations and extended studies were developed as part of the broader research associated with this project.

---

## Gallery

(Additional images of the setup, 3D scans, and formed samples can be added here.)
