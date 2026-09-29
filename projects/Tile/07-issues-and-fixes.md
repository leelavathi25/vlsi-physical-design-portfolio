# Issues and Fixes

## Issue 1 — M4 Spacing DRC

### Issue Details

- **Stage:** Floorplan
- **Category:** DRC
- **Tool:** ICC2_shell
- **Severity:** High

### Problem

Metal spacing DRC violations were observed over macro regions on the M4 layer.

### Root Cause

The issue was attributed to a mismatch in metal pitch values and larger via dimensions, which resulted in spacing violations.

### Debugging

The affected macro regions were identified and the metal blockage and via configuration were reviewed.

### Fix

- Disabled treatment of fat blockages as fat metal.
- Reduced the VIA45 row configuration from 3 to 2.

### Result

The DRC violations were cleared successfully.

---

## Issue 2 — Open Locations

### Issue Details

- **Stage:** Post-Route
- **Category:** LVS
- **Tool:** ICC2
- **Severity:** Critical

### Problem

Missing VDD rail connectivity was observed on the M1 layer, resulting in open connections.

### Root Cause

A routing blockage/keepout around macros prevented proper VDD rail connectivity.

### Debugging

Cells without M1 power-rail connectivity were identified and the affected regions were analyzed.

### Fix

The missing VDD rail was added to the M1 layer to restore connectivity.

### Result

All open violations were cleared successfully.

---

## Issue 3 — Setup Violations

### Issue Details

- **Stage:** Post-Route
- **Category:** Timing
- **Tool:** ICC2
- **Severity:** Critical

### Problem

Negative setup slack was observed on multiple timing paths after routing.

### Root Cause

The documented root causes included:

- Use of HVT cells resulting in higher delay
- Aggressive external input and output delays set to 70%

### Debugging

Timing reports were analyzed to identify critical paths, cell types, and delay contributions.

### Fix

- Replaced HVT cells with LVT cells where required.
- Reassigned external input and output delays from 70% to 60%.
- Applied higher weights to reg-to-reg paths to prioritize critical timing paths during optimization.

### Result

Setup violations were resolved and timing closure was achieved.
