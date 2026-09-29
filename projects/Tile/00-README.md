# Tile — Physical Design Implementation

## Project Overview

Hands-on ASIC Physical Design implementation of the `Tile` block using Synopsys Design Compiler and Synopsys ICC2.

The project covers synthesis, floorplanning, placement, clock tree synthesis, routing, post-route timing analysis, physical verification, and signoff.

## Design Specifications

- Technology: 28nm
- Block: Tile
- Ports: 1,635
  - Input: 838
  - Output: 797
- Macros: 18
- Clock: 1 master clock
- Standard Cell VT Types: HVT, LVT, SVT

## Tools

- Synopsys Design Compiler
- Synopsys ICC2

## Design Flow

**RTL → Synthesis → Floorplan → Placement → CTS → Routing → Post-Route → Signoff**

## Documentation

### Synthesis

Technology library setup, RTL synthesis, SDC application, timing checks, and synthesis metrics.

[View Synthesis Documentation →](01-synthesis.md)

### Floorplan

Core and die definition, macro placement, power-grid connectivity, and floorplan checks.

[View Floorplan Documentation →](02-floorplan.md)

### Placement

Standard-cell placement, utilization, congestion analysis, legalization, and spare-cell insertion.

[View Placement Documentation →](03-placement.md)

### Clock Tree Synthesis

Clock-tree implementation, clock buffers, skew, latency, timing analysis, and CTS checks.

[View CTS Documentation →](04-CTS.md)

### Routing

Detailed routing, DRC, shorts, opens, antenna checks, and routing analysis.

[View Routing Documentation →](05-route.md)

### Post-Route

Final timing, physical verification, signoff checks, and final database generation.

[View Post-Route Documentation →](06-post-route.md)

### Issues and Fixes

Documented debugging and resolution of DRC, LVS/open, and setup-timing issues encountered during implementation.

[View Issues & Fixes →](07-issues-and-fixes.md)
