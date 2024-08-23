---
layout: page
title: Usability Design for Machine Tools
description: An easy to use GCODE generator along with a DIY Joystick for motion control
img: assets/img/gcodegen/GUI_1.png
importance: 5
category: work
giscus_comments: true
---

Open source machine tools and the associated open source tool chain often suffers from biases towards users of the global north. With open source software not getting as much development effort compared to commercial tools, the interfaces are usually not user friendly and much too complex for users with limited digital literacy.

During the testing of the CNC Oxyfuel cutter(LINK PROJECT PAGE here), it was observed that it was much too complicated for the microenterprise users to learn to use the existing software toolchain of sketching the required shape in a CAD software, followed by exporting the drawing as a DXF file to a seperate CAM software, followed by applying the CAM toolpath to the desired shape and exporting the GCODE to be uploaded to the machine controller.

** INSERT flowchart of current process **

Even though the above toolchain is necessary for complex shapes and designs, for simpler shapes such as basic polygons or circles

This 2D GCODE generator software outputs CNC machine code for the CNC Oxyfuel cutter documented in another page. The user has to input the dimensions of the shape to be cut, choose the material thickness and specify the quantity of the shapes. The software outputs a text file with the machine code that can be sent to the gas cutter to carry out the cutting process.

The graphical user interphase (GUI) is written in python and utilizes the TKinter library for the creation of the GUI. The software can generate machine code for specific shapes like a square, circle, triangle and a stiffener (a rib shape often used to stiffen beam to plate connections in steel fabrication). It also nests the shapes automatically to minimize along with nesting the shapes for optimum space utilization. 

The choice of shapes were derived from discussions with the microenterprise workers. GCODE is basically several lines of code that instruct the microcontroller to move the axes to specific positions in time. The software basically just spits out a text file with the GCODE commands that can then be inserted into the LCD controller of the CNC machine and it would run the job.

The GCODE generation algorithm uses simple trignometry to calculate the coordinates between straight lines and arcs. Since Marlin the firmware used on the gas cutter only supports linear movements **(G1)** and arc movements **(G3)**, all motion is derived as a function of these two commands.

This GUI was created as a response to feedback received from the first user testing of the open source CNC gas cutter with the microenterprise end users. The users could not read or understand english and did not have any CAD or CAM knowledge. Therefore, a simple user interface was required that would allow the users to skip the complex CAD and CAM processes for the most commonly cut shapes in the shop.

WIP: Some features are yet to be implemented within the code. Right now the code employs a more rudimentary approach of the user specifying the number of parts horizontally and vertically, so that the sheet to be cut is optimally used. This is however not easily intuitive and requires the user to calculate how many parts would fit within a sheet. Therefore, the software needs to be able to automatically position the parts depending on the user input of sheet size and number of parts to be cut.