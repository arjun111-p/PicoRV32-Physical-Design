# PicoRV32-Physical-Design
Physical design implementation and analysis of the PicoRV32 RISC-V processor using OpenLane, OpenROAD, and the SKY130A technology stack.
# PicoRV32 Physical Design

## Project Overview

This project presents the physical design implementation and analysis of the PicoRV32 RISC-V processor using the OpenLane RTL-to-GDSII flow and OpenROAD-based physical design tools with the SKY130A process design kit.

The project covers the major stages of the digital physical design flow, including synthesis, static timing analysis, floorplanning, placement, power distribution network generation, clock tree synthesis, routing, and post-route physical design analysis.

## Design Information

| Parameter                | Value           |
| ------------------------ | --------------- |
| Design                   | PicoRV32        |
| Architecture             | RISC-V          |
| PDK                      | SKY130A         |
| Standard Cell Library    | sky130_fd_sc_hd |
| Clock Port               | clk             |
| Clock Period             | 6 ns            |
| Physical Design Flow     | OpenLane        |
| Physical Design Analysis | OpenROAD        |

## Physical Design Flow

The project follows the standard RTL-to-GDSII physical design flow:

1. Design preparation and configuration
2. Logic synthesis
3. Static timing analysis
4. Floorplanning
5. I/O pin placement
6. Placement
7. Tap and decap cell insertion
8. Power distribution network generation
9. Clock tree synthesis
10. Routing
11. Timing and physical verification
12. Post-route design analysis

## Timing and Constraint Analysis

The design was analyzed using clock constraints and timing parameters including:

* 6 ns clock period
* Clock uncertainty
* Input and output delays
* Timing derating
* Static timing analysis

The project also includes analysis of timing uncertainty and early/late timing derates during the physical design flow.

## Floorplanning

The physical design experiments include analysis of:

* Core utilization
* Core aspect ratio
* Core dimensions
* Die dimensions
* I/O pin placement
* Power planning
* Core ring generation

An example analyzed configuration produced a core size of approximately:

* Core Width: 488.52 µm
* Core Height: 340.0 µm

The corresponding die dimensions were approximately:

* Die Width: 499.895 µm
* Die Height: 363.96 µm

## Clock Tree Synthesis

Clock tree synthesis was analyzed using OpenROAD.

The project used a target clock skew of 0.3 ns and the analyzed design achieved an actual clock skew of approximately 0.1 ns.

The CTS analysis also includes clock buffers and inverters inserted into the clock network.

## Routing Analysis

Post-routing analysis was performed using the OpenROAD database and routed DEF data.

The project includes analysis of:

* Signal routing metal layers
* Routing buffers
* Routing inverters
* Standard-cell instances
* Flip-flops
* Physical-only cells
* Technology layers and routing resources

## OpenROAD Design Exploration

The OpenROAD analysis includes extraction of physical design information such as:

* Core and die dimensions
* Buffer count
* Inverter count
* Flip-flop count
* CTS buffer count
* CTS inverter count
* Site dimensions
* Physical-only cells

## Tools and Technologies

* OpenLane
* OpenROAD
* SKY130A PDK
* sky130_fd_sc_hd standard-cell library
* Tcl
* SDC
* RISC-V
* PicoRV32

## Project Structure

```text
PicoRV32-Physical-Design/
│
├── README.md
│
├── report/
│   └── PicoRV32_Physical_Design_Report.pdf
│
├── scripts/
│   ├── derate.tcl
│   ├── floorplan.tcl
│   ├── port.tcl
│   ├── core_ring.tcl
│   ├── skew.tcl
│   ├── clk.tcl
│   └── other analysis scripts
│
├── config/
│   ├── config.json
│   └── base.sdc
│
└── screenshots/
    ├── floorplan.png
    ├── placement.png
    ├── cts.png
    └── routing.png
```

> Note: The repository structure should contain only files and scripts that are actually available from the project environment.

## Results Summary

The project demonstrates the physical implementation and analysis of the PicoRV32 RISC-V processor through the OpenLane flow, followed by detailed inspection using OpenROAD.

The analysis covers timing constraints, floorplanning, placement, power planning, CTS, routing, and post-route physical characteristics.

## Author

Bodugam Naga Sai Kiran

Physical Design / VLSI Project

## Report

The complete project report is available in the `report/` directory.
