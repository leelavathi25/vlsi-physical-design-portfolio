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

The clock was defined using `create_clock` and verified using `report_clock`.

```tcl
create_clock -name gg -period 1 [get_ports clk]
```

The clock definition establishes the timing reference used for subsequent timing analysis.

---

## Input Delay

Input delay constraints were used to represent the timing contribution of external logic at the input ports.

```tcl
set_input_delay 0.2 -clock gg [get_ports data_in]
```

This allows the input path to be analyzed relative to the defined clock.

---

## Output Delay

Output delay constraints were used to specify the timing requirement associated with output paths.

```tcl
set_output_delay 0.2 -clock gg [get_ports data_out]
```

This represents the timing requirement at the output interface.

---

## Clock Uncertainty

Clock uncertainty was applied to account for timing variation associated with the clock.

The project considered both:

* Setup uncertainty
* Hold uncertainty

```tcl
set_clock_uncertainty -setup 0.1 [get_clocks gg]
set_clock_uncertainty -hold 0.05 [get_clocks gg]
```

Clock uncertainty is included in timing analysis to provide the required timing margin.

---

## Driving Cell

The input driving cell was specified to model the characteristics of the external logic driving the design inputs.

```tcl
set_driving_cell -lib_cell <cell_name> [get_ports data_in]
```

This provides the synthesis and timing analysis flow with a representation of the input drive characteristics.

---

## Output Load

Output load constraints were used to represent the capacitance driven by output ports.

```tcl
set_load <load_value> [get_ports data_out]
```

The load information is used during synthesis and timing analysis to evaluate output-path behavior.

---

## Path Grouping

Path grouping was used to organize timing paths for targeted timing analysis and optimization.

```tcl
group_path -name REG2REG -from [all_registers] -to [all_registers]
```

This allows related timing paths to be analyzed as a defined group.

---

## Timing Check

After applying the constraints, timing consistency was checked using:

```tcl
check_timing
```

Detailed timing analysis was then performed using:

```tcl
report_timing
```

## Outcome

The required timing constraints were applied to the REG-to-REG synthesis flow, enabling subsequent timing analysis and QoR evaluation.
