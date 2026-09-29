# Synthesis

## Tools

- Synopsys Design Compiler

## Objective

Synthesize the `Tile` RTL design using Synopsys Design Compiler and generate the gate-level netlist required for physical implementation.

## Synthesis Checks

The synthesis stage included:

- RTL files loaded successfully
- RTL elaboration completed without errors
- SDC file applied successfully
- Design and timing checks
- Technology library setup
- Gate-level netlist generation
- Synthesis report generation

## Design Information

| Metric | Value |
|---|---:|
| Technology | 28nm |
| Total Cell Area | 871688.081 µm² |
| Combinational Area | 130670.315 µm² |
| Sequential Area | 201834.609 µm² |
| Macro Area | 539183.15 µm² |
| Total Cells | 326035 |
| Sequential Cells | 102538 |
| Combinational Cells | 223497 |
| Buffer/Inverter Cells | 30585 |

## Timing & Power

| Metric | Value |
|---|---:|
| Worst Setup Slack (WNS) | 0.19 ns |
| Total Negative Slack (TNS) | 250.59 ns |
| Violating Paths | 5842 |
| Total Power | 265.6898 mW |

## Synthesis Configuration

The project applied specific cell-usage restrictions during synthesis, including restrictions on LVT, CK*, and high-drive-strength cells.

## Outcome

The `Tile` RTL design was successfully synthesized, with the required gate-level netlist and synthesis reports generated for subsequent physical implementation.
