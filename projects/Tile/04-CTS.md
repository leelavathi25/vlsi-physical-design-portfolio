# Clock Tree Synthesis

## Tool

Synopsys ICC2

## Objective

Implement the clock tree for the `Tile` block and analyze clock skew, latency, fanout, transition, and timing after CTS.

## CTS Metrics

| Metric | Value |
|---|---:|
| Clock Buffers Inserted | 8507 |
| Clock Inverters Inserted | 0 |
| Total Clock Tree Cells | 8507 |
| Clock Tree Area | 8250.35 µm² |
| Clock Fanout Limit | 16 |
| Clock Transition Limit | 0.2833 ns |
| Clock Net DRCs | 0 |
| Core Utilization | 79.93% |
| Congestion | 0.18 H% / V% |

Only CK*LVT cells were used in the clock tree.

## Clock Tree Analysis

Clock tree reports were generated to analyze:

- Global clock skew
- Maximum clock latency
- Clock transition
- Clock fanout
- Clock-tree DRCs

Reported global skew values were:

- RC Best: 0.53 ps
- C Best: 0.49 ps
- RC Worst: 0.82 ps
- C Worst: 0.9 ps

Reported maximum clock latency values were:

- RC Best: 0.7 ps
- C Best: 0.65 ps
- RC Worst: 1.08 ps
- C Worst: 1.2 ps

## Timing After CTS

### Setup Timing

| Path Group | WNS (ns) | TNS (ns) | FEP |
|---|---:|---:|---:|
| REG-to-REG | -0.32 | -106.74 | 5172 |
| IN-to-REG | -0.23 | -21.65 | 359 |
| REG-to-OUT | -0.45 | -225.39 | 786 |
| IN-to-OUT | 0 | 0 | 0 |

### Hold Timing

| Path Group | WNS (ns) | TNS (ns) | FEP |
|---|---:|---:|---:|
| REG-to-REG | -0.17 | -23.69 | 2208 |

## Clock Uncertainty

- Setup uncertainty: 0.15 × 1.7 = 0.255 ns
- Hold uncertainty: 0.05 ns

## CTS Checks

- Clock tree reports generated
- Clock net DRCs: 0
- Maximum capacitance violations: 0
- Placement/legalization check: Clean

## Outcome

The CTS stage was completed with the clock tree implemented and clock-tree reports generated. Post-CTS timing, skew, latency, congestion, and clock DRCs were analyzed.
