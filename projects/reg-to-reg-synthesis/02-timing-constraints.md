# Timing Constraints

## Tool

Synopsys Design Compiler

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

![Create clock command](../images/09-create-clock.jpg)

![Report clock output](../images/10-report-clock.jpg)

## Input and Output Delays

Input delays were used to represent the timing contribution of external logic at the input ports.

Output delays were used to specify the timing requirements associated with output paths.

![Set input delay command](../images/11-set-input-delay.jpg)

![Set output delay command](../images/12-set-output-delay.jpg)

## Clock Uncertainty

Clock uncertainty was applied to account for expected timing variation in the clock network.

The project considered both:

* Setup uncertainty
* Hold uncertainty

![Setup uncertainty command](../images/13-setup-uncertainty.jpg)

![Hold uncertainty command](../images/14-hold-uncertainty.jpg)

## Driving Cell and Load

Input driving-cell constraints were used to specify the external drive strength of input ports.

Load constraints were used to represent the capacitance that output drivers must drive.

![Driving cell command](../images/16-set-driving-cell.jpg)

![Load command](../images/17-set-load.jpg)

## Path Grouping

Path groups were used to organize specific timing paths for targeted timing analysis and optimization.

![Path grouping command](../images/15-group-path.jpg)

## Outcome

The required timing constraints were applied to the design to support subsequent timing analysis and optimization.
