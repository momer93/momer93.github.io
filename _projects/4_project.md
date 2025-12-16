---
layout: page
title: Incremental Forming
description: Incremental forming of PVC
img: assets/img/spif/spif1.png
importance: 8
category: work
---

## Overview

This was a **3-month Master’s project** at TU Dortmund (Manufacturing Technology) investigating the **formability of PVC sheets using Single Point Incremental Forming (SPIF)**. SPIF is a dieless forming process where a smooth, rounded tool incrementally forms a sheet along a CNC toolpath, shaping the part layer-by-layer.

The project combined **experiments, optical metrology, and finite element simulation** to understand why PVC fails at steep wall angles and how toolpath strategy can improve thickness distribution.

---

## Problem & Motivation

In SPIF, polymer sheets tend to experience **severe thinning** in the wall region. For PVC, this thinning leads to tearing before steep walls can be achieved.

The central question was:

> How can toolpath strategy be improved to reduce thinning and push the forming limit beyond the conventional wall-angle ceiling?

---

## Experimental Setup

The forming trials were carried out on a **3-axis CNC milling machine** equipped with a custom clamping fixture and a rounded forming tool.

<div class="row">
  <div class="col-sm-6 mt-3 mt-md-0">
    {% include figure.html path="assets/img/spif/sheet_in_fixture.jpg" title="PVC sheet clamped in SPIF fixture on CNC machine" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-6 mt-3 mt-md-0">
    {% include figure.html path="assets/img/spif/spif1.png" title="Single Point Incremental Forming (SPIF) schematic" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Experimental SPIF setup: PVC sheet clamped in a dedicated fixture and incrementally formed on a CNC machine.
</div>

Toolpaths for conical test geometries were generated programmatically (Excel-based NC generation), enabling controlled variation of key parameters such as wall angle, depth, and vertical step-down. A structured **Design of Experiments (DoE)** approach was used to explore parameter effects on failure and thickness evolution.

---

## Failure Mode: Thinning and Tearing

At higher wall angles, the sheet exhibited localized thinning followed by tearing—defining the practical forming limit.

<div class="row justify-content-sm-center">
  <div class="col-sm-5 mt-3 mt-md-0">
    {% include figure.html path="assets/img/spif/spif_tearing_defect.jpg" title="Localized thinning and tearing during SPIF of PVC" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Typical failure: localized thinning leading to tearing during SPIF of PVC.
</div>

---

## Measurement & Validation with Optical Scanning

When a test completed without fracture, the formed geometry was digitized using an optical 3D scanning system. The scan data enabled:

- reconstruction of the formed geometry  
- extraction of section cuts through the part  
- thickness evaluation along the wall to locate critical thinning zones

<div class="row">
  <div class="col-sm-6 mt-3 mt-md-0">
    {% include figure.html path="assets/img/spif/spif_scanning_part.jpg" title="Optical 3D scanning of formed sheet" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-6 mt-3 mt-md-0">
    {% include figure.html path="assets/img/spif/spif_scanning_part_1.jpg" title="Stereo camera setup for measurement" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Optical metrology workflow used to capture the formed geometry and evaluate thickness distribution.
</div>

<div class="row justify-content-sm-center">
  <div class="col-sm-6 mt-3 mt-md-0">
    {% include figure.html path="assets/img/spif/deformed_part_scan.jpg" title="Reconstructed scan of the deformed part" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Example of a reconstructed scan used for sectioning and thickness analysis.
</div>

---

## Numerical Simulation (Abaqus Explicit)

To analyze thickness evolution and deformation patterns, SPIF was modeled using **Abaqus Explicit**. The simulation helped identify:

- where thinning accumulates along the wall  
- how toolpath strategy influences material flow  
- qualitative agreement with experimentally observed thinning zones

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/spif/abaqus_STH_visual.jpg" title="Thickness distribution (STH) from Abaqus Explicit simulation" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Thickness distribution (STH) from Abaqus Explicit simulation during incremental forming.
</div>

---

## Toolpath Strategy Development (MATLAB)

Conventional multi-pass strategies can unintentionally re-stretch the same material, increasing thinning. To counter this, a modified multi-stage concept was developed and visualized in MATLAB, aiming to pull additional material from the flange region to improve thickness distribution.

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/spif/3D_NTP_30mm_4s.jpg" title="MATLAB visualization of a multi-stage SPIF toolpath" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  MATLAB visualization of the multi-stage toolpath strategy used to study material flow and thinning behavior.
</div>

---

## Key Outcomes

- Established an experimental baseline for **PVC SPIF forming limits** under the tested conditions  
- Identified thinning-driven tearing as the dominant failure mode  
- Implemented a repeatable workflow combining:
  - CNC-based experiments  
  - optical scanning for geometry/thickness evaluation  
  - Abaqus Explicit simulation for thickness evolution  
  - MATLAB toolpath visualization to reason about strategy effects  

This project strengthened my interest in **process-aware manufacturing**, where toolpath design, measurement, and simulation are used together to improve real production outcomes.

---

## Gallery

(Additional part photos and plots can be added here as the project archive grows.)
