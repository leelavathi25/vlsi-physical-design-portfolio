# Post-Route

## Tool

Synopsys ICC2

## Objective

Perform final post-route analysis and verify the implemented `Tile` design for timing, physical violations, and signoff database generation.

## Final Metrics

| Metric | Result |
|---|---:|
| DRC Violations | 0 |
| Shorts | 0 |
| Opens | 0 |
| Setup WNS — REG-to-REG | 0 ns |
| Setup TNS — REG-to-REG | 0 ns |
| Setup Violating Paths — REG-to-REG | 0 |
| Hold WNS — REG-to-REG | 0 ns |
| Hold TNS — REG-to-REG | 0 ns |
| Hold Violating Paths — REG-to-REG | 0 |
| Max Transition Violations | 0 |
| Max Capacitance Violations | 0 |

## Signoff Checks

The final implementation achieved:

- Clean placement/legalization check
- Zero DRC violations
- Zero shorts
- Zero opens
- Zero setup violations
- Zero hold violations
- Zero maximum-transition violations
- Zero maximum-capacitance violations

## Final Design Outputs

The following implementation outputs were generated:

- Final GDSII
- Final DEF
- Final gate-level netlist
- Signoff reports

## Final Power

The documented final total power was:

**9.28 × 10⁷ mW**

The power breakdown included sequential, combinational, clock-network, and leakage components.

## Outcome

The `Tile` block completed the post-route stage with clean physical and timing checks and with the required final design databases and signoff reports generated.
