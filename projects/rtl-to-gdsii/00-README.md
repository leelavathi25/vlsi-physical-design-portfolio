# RTL-to-GDSII Physical Design — `iguana_soc`

## Project Overview

Hands-on ASIC Physical Design implementation of the `iguana_soc` block through the RTL-to-GDSII flow using Cadence Genus and Innovus.

The project covers synthesis, floorplanning, placement, Clock Tree Synthesis, routing, post-route analysis, and physical verification.

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

## Design Flow

**Synthesis → Floorplanning → Placement → CTS → Routing → Post-Route Analysis → GDSII**

## Design Information

| Parameter    | Value |
| ------------ | ----: |
| Ports        |   240 |
| Input Ports  |    44 |
| Output Ports |    76 |
| Inout Ports  |   120 |
| Macros       |    32 |
| Clocks       |     8 |

## Physical Design Stages

### 1. Synthesis

RTL synthesis and timing analysis were performed using Cadence Genus.

Key activities included:

* RTL elaboration
* SDC constraint application
* Gate-level synthesis
* Timing analysis
* Area analysis
* Timing optimization

[View Synthesis](01-synthesis.md)

### 2. Floorplanning

The physical floorplan was created in Cadence Innovus with macro placement, IO planning, and power planning.

[View Floorplanning](02-floorplan.md)

### 3. Placement

Standard-cell placement and optimization were performed with analysis of density, congestion, timing, and design-rule constraints.

[View Placement](03-placement.md)

### 4. Clock Tree Synthesis

Clock trees were synthesized and analyzed for skew, latency, transition, fanout, and clock-related timing.

[View CTS](04-CTS.md)

### 5. Routing

Global and detailed routing were performed, followed by routing congestion and DRC analysis.

[View Routing](05-Route.md)

### 6. Post-Route Analysis

Post-route timing and physical verification were performed, including setup/hold analysis, DRC, legality, and final design checks.

[View Post-Route Analysis](06-Post-route.md)

## Final Deliverables

The physical implementation flow generated:

* GDSII
* DEF
* Final netlist
* Signoff reports

## Project Documentation

| Stage         | Documentation                        |
| ------------- | ------------------------------------ |
| Synthesis     | [01-synthesis.md](01-synthesis.md)   |
| Floorplanning | [02-floorplan.md](02-floorplan.md)   |
| Placement     | [03-placement.md](03-placement.md)   |
| CTS           | [04-CTS.md](04-CTS.md)               |
| Routing       | [05-Route.md](05-Route.md)           |
| Post-Route    | [06-Post-route.md](06-Post-route.md) |
