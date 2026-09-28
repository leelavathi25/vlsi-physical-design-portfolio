# Timing Constraints

## Objective

Apply timing constraints to the synthesized design so that the design can be analyzed against the required timing conditions.

## Constraints Covered

* Clock definition
* Input delay constraints
* Output delay constraints
* Clock uncertainty
* Input driving-cell specification
* Output load specification
* Path grouping

## Clock Definition

The project included clock creation and clock reporting using Synopsys Design Compiler.

Example:

```tcl
create_clock -name gg -period 1 [get_ports clk]
```

## Input and Output Delays

Input delays were used to represent the timing contribution of external logic at the input ports.

Output delays were used to specify the timing requirements associated with output paths.

## Clock Uncertainty

Clock uncertainty was applied to account for expected timing variation in the clock network.

The project considered both:

* Setup uncertainty
* Hold uncertainty

## Driving Cell and Load

Input driving-cell constraints were used to specify the external drive strength of input ports.

Load constraints were used to represent the capacitance that output drivers must drive.

## Path Grouping

Path groups were used to organize specific timing paths for targeted timing analysis and optimization.

## Outcome

The required timing constraints were applied to the design to support subsequent timing analysis and optimization.
