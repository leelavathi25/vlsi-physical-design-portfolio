# RTL-to-GDSII Physical Design — iguana_soc

## Project Overview

Hands-on ASIC Physical Design project implementing the `iguana_soc` block through the RTL-to-GDSII flow using Cadence Genus and Innovus.

## Technology

* 28nm
* 9T standard-cell technology
* HVT / SVT / LVT cells
* 32 macros
* 8 clocks

## Tools

* Cadence Genus
* Cadence Innovus
* Tcl
* SDC

## Physical Design Flow

**Synthesis → Floorplanning → Placement → CTS → Routing → Post-Route Analysis → GDSII**

## Key Areas

* Floorplanning and macro placement
* Power planning
* Standard-cell placement
* Clock Tree Synthesis
* Routing and congestion analysis
* Static Timing Analysis
* Timing optimization
* DRC and physical verification
* Post-route analysis

## Project Documentation

- [Synthesis](01-synthesis.md)
- [Floorplanning](02-floorplan.md)
- [Placement](03-placement.md)
- [Clock Tree Synthesis](04-CTS.md)
- [Routing](05-Route.md)
- [Post-Route Analysis](06-Post-route.md)
