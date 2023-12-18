---
layout: page
title: The Remocube 3D printer
description: Redesigning a 3D printer for replication
img: assets/img/3dp/printer_lit.JPG
importance: 2
category: work
giscus_comments: true
---

The aim of this project was to carry out build workshops with the citizens of hamburg whereby an open source machine could be built from scratch over two days. The machine had to be a safe one and something that could be done with schools, libraries, makerspaces and other institutions. The safest personal production machine was chosen to be a 3d printer for its widescale adoption as almost a household appliance lately.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3dp/printer_printing.jpg" title="Working printer" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Printer printing
</div>

## Design ##

Since there were already several good open source 3d printer designs on the internet, it was decided to use one and further develop it, than to start from scratch. The 3D printer design chosen was the thingiverse user [Scott_3D's hypercube evolution](https://www.thingiverse.com/thing:2254103) design which is an open source design with several community groups.
 
<div class="row justify-content-sm-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/3dp/original_hypercube.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/3dp/new_printer.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Original printer design - Hypercube Evolution, Right: My modified design - Remocube
</div>

 The selection of this design was based on its track record of successful replications, signifying its functionality and widespread popularity. In terms of function, its coreXY configuration enables swift movement of the print head along the X-Y plane. Moreover it uses a healthy combination of stiff aluminium slotted profiles to create a torsionally rigid box frame design, while the moving parts and brackets are from 3D printed PETG parts. 
 
 With PETG used for the pd printed parts, it offers a higher stiffness and temperature resistance compared to more conventional PLA. The use of off the shelf aluminium profiles and 3d printing for the complex parts, meant parts could be easily sourced as well as manufactured at home or at a nearby makerspace. The rigid design mean't the frame could withstand high accelerations and decelerations without flexing.

The oiginal design had some problems that needed to be rectified before it could be used. The design was not enclosed, which mean't high temperature plastics like ABS that required a closed build chamber could not be printed without warping. Moreover, the open design meant, it posed a hazard for children since the printer would be used in schools. The bowden drive extruder did not allow the printing of flexible filaments since the extruder motor was mounted further away from the printhead, this mean't flexible filament would get compressed in the bowden tube and not be pushed through the hot end. 

The electronics were also outdated i.e. it used an 8-bit microcontroller, that could not process coreXY kinematics quick enough and also was limited to a 12V power supply, which would not be able to run the motors efficiently enough. Moreover the elctronics needed to be made safe i.e. any mains wiring had to completely sealed such that children could not by accident touch mains wiring.

# insert my design pictures

To enhance it, I fully enclosed the structure with a temperature controlled build chamber. I modernized the electronics in that a 32 bit microcontroller was used, which mean't a 24V power supply could be used, which would allow the motors to run more efficiently. The print head was redesigned and a lightweight direct drive extruder with a small Nema14 pancake motor was mounted. This allowed the printhead to be as light as possible so that faster motion could be achieved by the coreXY setup. Since the design was enclosed, for a shorter printer height, a cable chain was required to route the cables from the printhead to the electronics compartment. It also gave the printer a more refined look.

Shielded cables were used on the endstop cables, so that no interference would occur, which was a case with the previous optical endstops. In the original design 2 motors were used with the Z axis, with each motor shaft directly coupled to each lead screw with a flex coupler. The direct coupling of the motors to the Z-axis leadscrews meant, vibrations were transmitted directly to the build plate, introducing wave like patterns on the 3d printed parts surface. This was replaced with a single Z motor that transmitted the motion by a closed belt to both the Z lead screws simultaneously. This allowed the Z axis lead screws to move in sync and also removed the vibrations to the bed by the belt drive.

# Insert picture of current design from front, dual Z axis design and view of back electronics #

Furthermore, I developed an instruction manual resembling LEGO manuals, facilitating easy replication by laypersons during a concise two-day build workshop. I also created a user guide to make the software and firmware setup easy.

# insert picture of new printer and a build manual snapshot  side by side #

Conducting ten such workshops across multiple institutions in Hamburg, I personally prepared all the printer build kits. This encompassed sourcing components, 3d printing parts, and meticulously packaging them into labeled sets, ensuring a seamless experience for workshop participants. This was challenging since during corona we were stuck to working from home, so i literally transformed my room into a small production facility.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3dp/printer_parts.JPG" title="3d printer kit" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    3D printer build kit
</div>

Several workshops were offered in schools, libraries, museums and other institutions. The participants ranged from school teachers, students, to engineers and architects. Using the build manual and some tips from me during the build workshops, the participants were able to build the 3d printers from scratch within 2 days and also start printing on the second day. This shows machine building, even though a complex endeavour, with the right build instructions and appropriately intuitive design, is doable and can be plenty of fun. Along the way, participants learn several aspects of machine building, electronics, mechanics etc.

# Insert pictures of the printer being built in build workshops #

 
