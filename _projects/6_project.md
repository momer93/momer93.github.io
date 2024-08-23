---
layout: page
title: Manufacturing process optimization
description: Simulation and optimization of a rapid hot forging process.
img: assets/img/amps/forming_simulation.gif
importance: 7
category: work
---

## Background and Motivation

The aim of this project was to characterize and optimize a rapid hot forging process that was used to manufacture a geared seat recliner component. Being a critical safety component, the part was required to deform with a certain ductility in order to decelerate the seat during a crash and as a result garantee the safety of the passenger. This mean't the part needed a tailored hardness and strength distribution, with the outer surface of the gear teeth being hard enough to withstand abrasion over an extended period of function and the root of the gear teeth to have sufficient ductility to deform during a crash instead of causing a sudden fracture.

The part was previously manufactured by fine blanking and later subjected to targeted heat treatment to achieve the required hardness and strength profile of the part. In order to make the process more efficient by including the heat treatment phase within the manufacturing phase, a new process was introduced, namely rapid plate forging. The process was still in its development phase and an accurate simulation model of the manufacturing process was required to better optimize the material flow and microstructure of the finished part. This is because, the process variables were difficult to observe or measure insitu, due to the high stresses and temperature during the forging process within the forming zone.

## Methodology

Forge NxT, a commercial forging process simulator was used to simulate the forging process. The CAD model of the forming tools were imported into Hypermesh, a mesh generating software, in order to simplify the design for simulation and perform a optimized meshing of the tool and workpiece to make the simulation efficient.

The meshed tools and billet were imported into Forge NXT to set up the simulation model.

## Simulation Model Setup

To measure the durations of the forming process, several experiments were carried out to measure the exact heating and forming phase durations. The process was recorded by video cameras and the footage observed to determine the exact durations.

## Simulation Validation

Thermal cameras were used to measure the billet temperature before and after forming. With post-processing software provided with the thermal camera, temperature probes were places on various regions of the teeth profile on the thermal image to create a basic heat map of the part. 

The gear shape profile on the final part was measured on a CMM machine, such that several profiles in step increments along the teeth height were measured to create point clouds. This point cloud was exported in a CAD friendly form (IGES) and exported to the CAD program CATIA.

The time durations within the process were entered into the simulation model and informed the process parameter input durations. The temperature profiles before and after forming along with the final formed part geometry were used to validate the simulation model results.
