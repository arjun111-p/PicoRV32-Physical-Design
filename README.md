# PicoRV32 RISC-V Processor — Physical Design

## Project Overview

This project presents the physical design implementation and analysis of the **PicoRV32 RISC-V processor** using the **OpenLane RTL-to-GDSII flow**, **OpenROAD**, and the **SKY130A technology stack**.

The work covers the major stages of the ASIC physical design flow, including synthesis, static timing analysis, floorplanning, placement, power planning, clock tree synthesis (CTS), routing, and post-route physical design analysis.

The project also includes timing constraint analysis, timing derating, clock uncertainty, floorplan configuration, pin placement, routing analysis, and clock-tree analysis.

## Design Information

| Parameter             | Details         |
| --------------------- | --------------- |
| Processor             | PicoRV32        |
| Architecture          | RISC-V          |
| PDK                   | SKY130A         |
| Standard Cell Library | sky130_fd_sc_hd |
| Physical Design Flow  | OpenLane        |
| Analysis Tool         | OpenROAD        |
| Clock Port            | clk             |
| Clock Period          | 6 ns            |
| Clock Uncertainty     | 0.9 ns          |

## Physical Design Flow

The project follows the standard RTL-to-GDSII physical design flow:

1. Design preparation
2. Logic synthesis
3. Static timing analysis
4. Floorplanning
5. I/O pin placement
6. Placement
7. Tap and decap cell insertion
8. Power distribution network generation
9. Clock tree synthesis
10. Routing
11. Timing analysis
12. Post-route physical design analysis

## Timing Analysis

Timing analysis was performed using clock constraints and timing parameters including:

* Clock period
* Clock uncertainty
* Input and output delays
* Early and late timing derates
* Static timing analysis

The project investigates the effect of timing constraints and derating on the physical design implementation.

## Floorplanning

The physical design analysis includes:

* Core utilization
* Core aspect ratio
* Core dimensions
* Die dimensions
* I/O pin placement
* Power planning
* Core ring generation

One of the analyzed configurations produced approximately:

* **Core Width:** 488.52 µm
* **Core Height:** 340.0 µm
* **Die Width:** 499.895 µm
* **Die Height:** 363.96 µm

## Clock Tree Synthesis

Clock Tree Synthesis (CTS) was analyzed using OpenROAD.

The analysis used a target clock skew of approximately **0.3 ns** and achieved an actual clock skew of approximately **0.1 ns** in the reported configuration.

The report also analyzes clock buffers, inverters, clock-network delay, and clock-tree characteristics.

## Placement and Routing Analysis

The project includes physical design analysis of:

* Standard-cell placement
* Routing resources
* Routing metal layers
* Routing buffers
* Routing inverters
* Flip-flops
* Physical-only cells
* Post-route design characteristics

The report contains OpenROAD-based analysis of the implemented PicoRV32 design.

## Tools and Technologies

* **PicoRV32**
* **RISC-V**
* **OpenLane**
* **OpenROAD**
* **SKY130A PDK**
* **sky130_fd_sc_hd**
* **Tcl**
* **SDC**
* **ASIC Physical Design**

## Project Documentation

The complete physical design work, experiments, configurations, analysis, and results are documented in the project report available in this repository.

### Report

**PicoRV32 Physical Design Report**

The report contains the detailed analysis and results of the PicoRV32 physical design implementation.

## Repository Contents

Currently, this repository contains the project documentation/report.

The original physical design work was performed in the OpenLane/OpenROAD environment, while the available project submission artifact is the documented report.

## Key Learning Outcomes

Through this project, the following physical design concepts were studied and analyzed:

* RTL-to-GDSII flow
* Logic synthesis
* Static timing analysis
* Floorplanning
* Placement
* Power distribution network
* Clock Tree Synthesis
* Routing
* Timing constraints
* Timing derating
* Clock uncertainty
* Physical design metrics
* OpenROAD design analysis

## Author

Bodugam Naga Sai Kiran

B.Tech — Electronics and Communication Engineering

## Project Type

**ASIC Physical Design / VLSI**

**PicoRV32 RISC-V Processor**
