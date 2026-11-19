# Day 3 — KCL, Series and Parallel Circuits

## Date
19 November 2026

## Topics Studied
- KCL: total current entering a junction = total current leaving
- Series circuits: same current, resistances add, voltage divides
- Parallel circuits: same voltage, currents add, resistance decreases

## Key Formulas

### KCL
- I_in = I_out

### Series Circuit
- R_total = R1 + R2 + R3
- I is same through all components
- V_total = V_R1 + V_R2 + V_R3

### Parallel Circuit
- 1/R_total = 1/R1 + 1/R2
- V is same across all branches
- I_total = I_R1 + I_R2

## Quiz Results

| Question | Answer | Result |
|----------|--------|--------|
| Q1. 7A + 4A enter → I_out = ? | 11A | ✅ |
| Q2. 15A in, 6A+5A out → Branch 3 = ? | 4A | ✅ |
| Q3. R1=5Ω, R2=10Ω, R3=15Ω series, 30V → R_total and I? | 30Ω, 1A (missed current) | ✅/❌ |
| Q4. R1=6Ω, R2=12Ω parallel, 12V → I1, I2, I_total? | 2A, 1A, 3A | ✅ |
| Q5. Parallel circuit → voltage or current same? | Voltage | ✅ |

Score: 4.5 / 5

## Bonus Problem — Full Circuit Analysis
V=24V, R1=8Ω, R2=4Ω in series

1. R_total = 12Ω ✅
2. I = 2A ✅
3. V_R1 = 16V ✅
4. V_R2 = 8V ✅
5. KVL: 24 - 16 - 8 = 0 ✅

Bonus Score: 5/5

## VLSI Connection
- Series paths cause signal delay on chips
- Parallel paths used in power delivery networks
- KCL used to analyze current distribution across transistors

## Next Session
Day 4 — Capacitors, Diodes and AC/DC Basics
