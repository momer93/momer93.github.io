---
layout: page
title: Custom GCODE generator
description: An easy to use GCODE generator for a CNC gas cutter
img: assets/img/gcodegen/GUI_1.png
importance: 5
category: work
giscus_comments: true
---

A GCODE Generator GUI was created using python that could generate gcodes for specific shapes like a square, circle, triangle and a stiffener along with nesting the shapes for optimum space utilization. This GUI was created as a response to feedback recieved from the first user testing of the open source CNC gas cutter with the microenterprise end users. The users could not read or understand english and did not have any CAD or CAM knowledge. Therefore a simple user interface was required that would allow the users to skip the complex CAD and CAM processes for the most commonly cut shapes in the shop.

The end user is asked to input the following variables
1. Dimensions of the specific shape they want to cut
2. Thickness of the sheetmaterialNext they have to enter t
3. Size of the sheet
4. Quantity of parts to be cut
5. The system automatically nests the parts in the best possible configuration.