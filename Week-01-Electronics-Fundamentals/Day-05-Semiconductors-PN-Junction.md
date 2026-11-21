# Day 5 — Semiconductors, PN Junction and Diode Operation

## Date
21 November 2026

## Topics Studied
- Semiconductors: between conductor and insulator, silicon is most common
- Doping: adding impurities to control conductivity
- N-type: 5 valence electron element added, extra electrons, negative carriers
- P-type: 3 valence electron element added, holes formed, positive carriers
- PN Junction: P and N joined together
- Depletion region: no free carriers, acts as barrier, built-in voltage = 0.7V
- Forward bias: V > 0.7V → diode conducts
- Reverse bias: diode blocks, I ≈ 0A

## Key Concepts

### Doping
- N-type: add Phosphorus (5 valence electrons) → free electrons
- P-type: add Boron (3 valence electrons) → holes

### Depletion Region
- Forms at PN junction
- Holes and electrons combine → no free carriers
- Creates built-in electric field and 0.7V barrier

### Bias
- Forward: V_applied > 0.7V → conducts
- Reverse: blocks current

## Worked Example
- V=3V, R=50Ω, silicon diode forward biased
- V_resistor = 3 - 0.7 = 2.3V
- I = 2.3 / 50 = 0.046A

## Quiz Results

| Question | Answer | Result |
|----------|--------|--------|
| Q1. What is doping and why? | Adding impurity to increase free electrons or holes | ✅ |
| Q2. N-type valence electrons and example? | 5 valence electrons, Phosphorus | ✅ |
| Q3. What is depletion region and how does it form? | No free carriers region, holes+electrons combine | ✅ |
| Q4. V=3V, R=50Ω, silicon diode → I = ? | 0.06A (forgot to subtract 0.7V, correct = 0.046A) | ❌ |
| Q5. Why does silicon diode need 0.7V minimum? | Depletion region barrier must be overcome | ✅ |

Score: 4 / 5

## Mistake to Fix
- In diode circuits always subtract 0.7V first: V_resistor = V_supply - 0.7V

## VLSI Connection
- Every MOSFET contains PN junctions
- Source and drain are doped N or P regions
- Gate voltage overcomes junction barrier to allow current — same principle as forward bias

## Next Session
Day 6 — BJT and MOSFET Basics, Transistor as a Switch
