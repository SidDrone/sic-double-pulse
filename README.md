# SiC Half-Bridge Gate Driver and Double-Pulse Test

**Status: in progress.** This repository is being built; nothing here is a finished result yet.

## Goal

An LTspice model of a 400 V / 50 A SiC MOSFET half-bridge with vendor SPICE models, a gate driver and parasitic loop inductance. Double-pulse tests extract switching energy across gate resistance and junction temperature; gate-resistance tuning and an RC snubber control drain overshoot against switching loss.

## Layout

```
ltspice/models/           # Vendor SiC MOSFET and diode models (sources listed here).
ltspice/circuits/         # Half-bridge, gate driver and double-pulse test bench.
sweeps/                   # Python batch runner and .raw parser.
analysis/                 # Eon/Eoff extraction, overshoot, loss vs Rg and temperature.
results/                  # Plots and tables.
docs/                     # Setup and results.
```

## Plan

- [ ] Half-bridge + gate driver circuit
- [ ] Double-pulse test bench
- [ ] Batch sweep runner
- [ ] Switching-energy extraction
- [ ] Rg / temperature sweeps
- [ ] Snubber design and trade-off
- [ ] Write-up
