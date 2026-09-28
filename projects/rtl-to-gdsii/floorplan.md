# Floorplanning

## Tool

Cadence Innovus

## Objective

Create the physical floorplan for the synthesized design, including core/die definition, macro placement, IO planning, and power planning.

## Design Information

* Technology: 28nm
* Number of macros: 32
* Initial core utilization: 70%

## Key Results

| Metric           |          Result |
| ---------------- | --------------: |
| Core Width       |         1169 µm |
| Core Height      |       1166.4 µm |
| Core Area        |   1366521.6 µm² |
| Die Width        |      1189.16 µm |
| Die Height       |       1186.4 µm |
| Die Area         | 1410839.424 µm² |
| Core Utilization |             79% |
| Macro Area       |   629020.74 µm² |

## Work Performed

* Core and die definition
* Macro placement and orientation
* Macro channel planning
* Placement halo and routing blockage planning
* IO placement
* Power-ring and power-stripe planning
* Congestion analysis

## Timing Check

* Pre-placement WNS: -0.064 ns
* Pre-placement TNS: -0.101 ns
* Violating paths: 3

## Outcome

The physical floorplan was established for the `iguana_soc` design and prepared for standard-cell placement.
