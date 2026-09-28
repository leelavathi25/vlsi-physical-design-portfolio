# Synthesis

## Tool

Synopsys Design Compiler

## Objective

Convert the RTL design into an optimized gate-level netlist while applying the required technology libraries and timing constraints.

## Synthesis Flow

The synthesis flow covered the following steps:

1. Link library setup
2. Target library setup
3. RTL analysis
4. RTL elaboration
5. Design compilation
6. Design checking
7. Timing checking
8. Clock definition
9. Clock reporting
10. Timing constraint application
11. Timing analysis
12. QoR analysis

## Work Performed

* Technology library setup using link and target libraries
* RTL analysis and syntax checking
* RTL elaboration
* Logic synthesis and optimization
* Design consistency checking
* Timing constraint definition
* Clock definition and reporting
* Timing analysis
* QoR analysis

## Key Commands

* `analyze`
* `elaborate`
* `compile`
* `check_design`
* `check_timing`
* `create_clock`
* `report_clock`
* `set_input_delay`
* `set_output_delay`
* `set_clock_uncertainty`
* `group_path`
* `report_timing`
* `report_qor`

## Outcome

The RTL design was synthesized using Synopsys Design Compiler, producing an optimized gate-level representation for subsequent timing and QoR analysis.
