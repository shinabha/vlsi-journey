# Day 2 — Power, Energy and Kirchhoff's Voltage Law (KVL)

## Date
18 November 2026

## Topics Studied
- Power: rate at which electrical energy is consumed (unit: Watt)
- Energy: total amount of electrical work done (unit: Joule)
- Kirchhoff's Voltage Law (KVL): sum of all voltages in a closed loop = 0

## Formulas

### Power
- P = V × I
- P = I² × R
- P = V² / R

### Energy
- E = P × T

### KVL
- Sum of all voltage rises and drops in a closed loop = 0

## Worked Examples

### Power
1. V=12V, I=2A → P = 24W
2. I=3A, R=10Ω → P = 90W
3. V=20V, R=5Ω → P = 80W

### KVL
1. 12V battery, R1=4Ω, R2=8Ω, I=1A → V_R1=4V, V_R2=8V → 12-4-8=0 ✅
2. 9V battery, V_R1=3V → V_R2=6V

## Quiz Results

| Question | Answer | Result |
|----------|--------|--------|
| Q1. I=2A, R=6Ω → P = ? | 24W (wrote 12W, wrong formula used) | ❌ |
| Q2. V=10V, P=50W → I = ? | 5A | ✅ |
| Q3. V=8V, R=4Ω → P using V²/R = ? | 16W | ✅ |
| Q4. 15V, R1=4V, R2=6V → V_R3 = ? | 5V (wrote 5Ω, wrong unit) | ❌ |
| Q5. P=3W, T=10s → E = ? | 30J | ✅ |

Score: 3 / 5

## Mistakes to Fix
1. P = I × R is wrong. Correct formula is P = I² × R
2. Always write correct units with every answer (W for power, V for voltage, A for current)

## VLSI Connection
- Chips contain billions of transistors, each consuming power when switching
- Too much power causes overheating and chip failure
- KVL helps analyze voltage distribution across signal paths on a chip

## Next Session
Day 3 — Kirchhoff's Current Law (KCL) and Series/Parallel Circuits
