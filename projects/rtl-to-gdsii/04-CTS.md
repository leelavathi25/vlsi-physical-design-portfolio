# Clock Tree Synthesis

## Tool

Cadence Innovus

## Objective

Build and optimize the clock tree to distribute clock signals with controlled skew, latency, transition, and fanout.

## Design Information

* Technology: 28nm
* Number of clocks: 8

## Key Results

| Metric                 |     Result |
| ---------------------- | ---------: |
| Clock Buffers          |        787 |
| Clock Inverters        |          2 |
| Total Clock Tree Cells |       3357 |
| Clock Tree Area        | 89.712 µm² |
| Global Skew            |     198 ps |
| Maximum Latency        |     186 ps |
| Fanout Limit           |         35 |
| Clock Net DRCs         |          0 |

## Timing Check

* Reg-to-Reg Setup WNS: -0.064 ns
* Reg-to-Reg Setup TNS: -0.101 ns
* Setup Violating Paths: 3
* Reg-to-Reg Hold WNS: -0.170 ns
* Hold Violating Paths: 0

## Work Performed

* Clock tree synthesis
* Clock buffer insertion
* Clock tree balancing
* Clock skew analysis
* Clock latency analysis
* Transition and fanout analysis
* Clock DRC analysis
* Timing optimization

## Outcome

The clock tree was synthesized and analyzed for skew, latency, transition, fanout, and timing before proceeding to routing.
