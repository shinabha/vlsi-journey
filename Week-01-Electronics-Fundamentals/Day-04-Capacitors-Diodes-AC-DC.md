# Day 4 — Capacitors, Diodes and AC/DC Basics

## Date
20 November 2026

## Topics Studied
- AC vs DC: AC alternates direction, DC flows one way
- Capacitors: store charge temporarily, block DC, pass AC
- Diodes: allow current in one direction only (PN junction)

## Key Formulas

### AC
- T = 1 / f
- V_rms = V_peak / √2

### Capacitor
- Q = C × V
- Units: Farad (F), µF, nF, pF

### Diode
- Forward bias: conducts, 0.7V drop (silicon)
- Reverse bias: blocks current completely

## Worked Examples

### AC
- f = 50Hz → T = 1/50 = 0.02 seconds

### Capacitor
- C=10µF, V=5V → Q = 0.00005C = 50µC

### Diode
- V=5V, R=100Ω, silicon diode → I = (5-0.7)/100 = 0.043A

## Quiz Results

| Question | Answer | Result |
|----------|--------|--------|
| Q1. f=50Hz → T = ? | 0.02s (wrote without unit) | ✅ |
| Q2. C=10µF, V=5V → Q = ? | 0.00005C | ✅ |
| Q3. Capacitor blocks DC? | True, passes AC via charge/discharge | ✅ |
| Q4. V=9V, R=200Ω, silicon diode → I = ? | 0.041A | ✅ |
| Q5. Reverse bias → current? | Blocks current (0A) | ✅ |

Score: 5 / 5

## Mistake to Fix
- Always write units with every answer (seconds, Coulombs, Amperes)

## VLSI Connection
- Parasitic capacitance in chip wires causes signal delay
- Decoupling capacitors smooth power supply on chips
- PN junction is the foundation of MOSFETs and all chip transistors

## Next Session
Day 5 — Semiconductors, PN Junction and Diode Operation
