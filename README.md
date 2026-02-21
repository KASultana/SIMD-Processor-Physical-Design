# SIMD-Processor-Physical-Design
16-bit SIMD Processor Physical Design using complete RTL-to-GDSII flow (Synthesis, Floorplanning, CTS, Routing, DRC &amp; STA closure)

# 16-bit SIMD Processor – Physical Design Implementation

## Project Overview

This project presents the complete physical design implementation of a 16-bit Simple SIMD Processor. 

The processor consists of:
- 16-bit SIMD ALU
- Multi-width computation support (4-bit, 8-bit, 16-bit)
- 5-stage architecture (IF, ID, EX, MEM, WB)
- 18-bit instruction format
- 6-bit opcode control

The focus of this project is full RTL-to-GDSII Physical Design Flow.

---

## Design Specifications

- Architecture: SIMD
- ALU width: 16-bit
- Instruction width: 18-bit
- Register types: 16-bit, 8-bit, 4-bit
- Total placed cells: 7895

---

## Physical Design Flow

### 1. Synthesis
- Gate-level netlist generation
- Timing-driven synthesis

### 2. Floorplanning
- Core utilization setup
- IO pin placement
- Power ring creation

### 3. Power Planning
- VDD/VSS grid implementation

### 4. Placement
- Standard cell placement
- Congestion optimization

### 5. Clock Tree Synthesis (CTS)
- Clock buffer insertion
- Skew optimization

### 6. Routing
- Global & detailed routing
- Routing optimization

### 7. Design Rule Check (DRC)
- Initial DRC violations: 1000
- Final DRC violations: 0

### 8. Static Timing Analysis (STA)
- Timing closure performed
- Setup and hold analysis completed

---

## Results Summary

| Metric | Before Optimization | After Optimization |
|--------|--------------------|-------------------|
| Final Density | 83.98% | 105.74% |
| Placed Cells | 7895 | 7895 |
| DRC Errors | 1000 | 0 |
| Connectivity Violations | 77 | 0 |
| Glitch Violations | 33 | 0 |

All DRC, connectivity, and glitch violations were successfully resolved.

---

## Key Learning Outcomes

- End-to-end Physical Design flow
- DRC debugging and violation fixing
- Timing closure techniques
- Clock tree optimization
- Congestion and density management

---

## Future Improvements

- Fanout violation reduction
- Further timing margin improvement
- Custom instruction extension
