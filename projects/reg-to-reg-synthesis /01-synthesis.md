# Synthesis

## Tool

Synopsys Design Compiler

## Objective

Convert the RTL design into an optimized gate-level netlist while applying the required technology libraries and timing constraints.

## Synthesis Flow

| Synthesis Stage                | Key Commands                                                   |
| ------------------------------ | -------------------------------------------------------------- |
| Library Setup                  | `link_library`, `target_library`                               |
| RTL Analysis                   | `analyze`                                                      |
| RTL Elaboration                | `elaborate`                                                    |
| Logic Synthesis & Optimization | `compile`                                                      |
| Design Checking                | `check_design`                                                 |
| Timing Checking                | `check_timing`                                                 |
| Clock Definition               | `create_clock`                                                 |
| Clock Reporting                | `report_clock`                                                 |
| Timing Constraints             | `set_input_delay`, `set_output_delay`, `set_clock_uncertainty` |
| Path Grouping                  | `group_path`                                                   |
| Timing Analysis                | `report_timing`                                                |
| QoR Analysis                   | `report_qor`                                                   |

## Work Performed

* Technology library setup using link and target libraries
* RTL analysis and elaboration
* Logic synthesis and optimization
* Design and timing checks
* Clock definition and reporting
* Timing constraint application
* Timing analysis
* QoR analysis

## Outcome

The RTL design was synthesized using Synopsys Design Compiler, producing an optimized gate-level representation for subsequent timing and QoR analysis.
