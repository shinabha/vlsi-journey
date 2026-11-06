## ✅ Project 1 — 2:1 MUX (Multiplexer)
**Date:** 05 Oct 2026

### What is a 2:1 MUX?
A selector circuit with 2 inputs (a, b), 1 select line (sel),
and 1 output (y).
- sel=0 → output follows a
- sel=1 → output follows b

### Verilog Code
```verilog
module mux2to1(
  input a, b, sel,
  output y
);
  assign y = sel ? b : a;
endmodule
```

### Terminal Output
![Terminal simulation result](images/mux2to1_terminal.png)

### GTKWave Waveform
![GTKWave waveform](images/mux2to1_waveform.png)

### Verification — All 4 test cases passed ✓
| Time | a | b | sel | y | Expected | Result |
|------|---|---|-----|---|----------|--------|
| 0s   | 0 | 0 |  0  | 0 |    0     | ✓ |
| 10s  | 0 | 1 |  0  | 0 |    0     | ✓ |
| 20s  | 1 | 0 |  1  | 0 |    0     | ✓ |
| 30s  | 1 | 1 |  1  | 1 |    1     | ✓ |

### What I learned
- `assign` = continuous hardware connection, not a software assignment
- Ternary operator `sel ? b : a` maps directly to MUX logic
- Difference between `wire` (combinational output) and `reg` (testbench inputs)
- How to dump `.vcd` file and read waveforms in GTKWave

---

## ✅ Project 2 — 4:1 MUX (Multiplexer)
**Date:** 06 Nov 2026

### What is a 4:1 MUX?
Extends the 2:1 MUX — 4 inputs (i0, i1, i2, i3),
2 select lines (s1, s0), and 1 output (y).
- s1=0, s0=0 → output = i0
- s1=0, s0=1 → output = i1
- s1=1, s0=0 → output = i2
- s1=1, s0=1 → output = i3

### Terminal Output
![4:1 MUX terminal](images/mux4to1_terminal.png)

### GTKWave Waveform
![4:1 MUX waveform](images/mux4to1_waveform.png)

### HDLBits Verification
![HDLBits success](images/mux2to1_hdlbits.png)

### Verification — All test cases passed ✓
| Time | s1 | s0 | i0 | i1 | i2 | i3 | y | Result |
|------|----|----|----|----|----|-----|---|--------|
| 0s   | 0  | 0  | 1  | x  | x  | x  | 1 | ✓ |
| 10s  | 0  | 1  | x  | 0  | x  | x  | 0 | ✓ |
| 20s  | 1  | 0  | x  | x  | 0  | x  | 0 | ✓ |
| 30s  | 1  | 1  | x  | x  | x  | 0  | 0 | ✓ |

### What I learned
- How to extend a 2:1 MUX to 4:1 using 2 select lines
- Two select lines can encode 4 states: 00, 01, 10, 11
- HDLBits runs your Verilog against hundreds of hidden test cases
- Mismatch = 0 means every single one passed

---

## 🏆 HDLBits Progress
| Problem | Status |
|---------|--------|
| 2:1 MUX (mux2to1) | ✅ Solved |
| 4:1 MUX (mux4to1) | ✅ Solved |
