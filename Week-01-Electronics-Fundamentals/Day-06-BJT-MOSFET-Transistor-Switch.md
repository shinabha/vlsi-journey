# Day 6 — BJT, MOSFET and Transistor as a Digital Switch

## Date
22 November 2026

## Topics Studied
- BJT: current controlled switch, terminals = Base, Collector, Emitter
- MOSFET: voltage controlled switch, terminals = Gate, Drain, Source, Body
- NMOS: turns ON when Gate voltage > V_th
- PMOS: turns ON when Gate voltage < V_th
- CMOS: NMOS + PMOS complementary pair, almost zero static power
- CMOS Inverter: one PMOS + one NMOS = NOT gate

## Key Concepts

### BJT vs MOSFET
- BJT: current controlled, base current needed, older technology
- MOSFET: voltage controlled, no gate current, used in all modern chips

### NMOS Switch
- Gate HIGH → ON → current flows Drain to Source
- Gate LOW → OFF → no current flows

### PMOS Switch
- Gate LOW → ON → current flows Source to Drain
- Gate HIGH → OFF → no current flows

### CMOS Inverter
- Input HIGH → NMOS ON, PMOS OFF → Output LOW
- Input LOW → PMOS ON, NMOS OFF → Output HIGH
- Same behaviour as NOT gate in Verilog: assign out = ~in

## Quiz Results

| Question | Answer | Result |
|----------|--------|--------|
| Q1. BJT terminals? | Base, Collector, Emitter | ✅ |
| Q1. MOSFET terminals? | Gate, Source, Drain, Channel (Channel is wrong, correct = Body) | ❌ |
| Q2. BJT vs MOSFET control? | BJT current controlled, MOSFET voltage controlled | ✅ |
| Q3. NMOS V_th=1V, Gate=0.5V → ON or OFF? | OFF (used wrong V_th=0.7V in reasoning) | ✅ |
| Q4. CMOS inverter, input LOW → which ON, output? | PMOS ON (forgot to state output = HIGH) | ½ |
| Q5. Why CMOS low static power? | Only one transistor ON at any time | ✅ |

Score: 3.5 / 5

## Mistakes to Fix
1. MOSFET fourth terminal is Body, not Channel
2. Always state complete answer — if question asks two things, give both
3. Always use V_th value given in the question, not 0.7V (that is diode voltage)

## VLSI Connection
- Every Verilog logic gate physically maps to CMOS transistor pairs
- assign out = ~in → one PMOS + one NMOS on the actual chip
- Understanding CMOS explains why chips are power efficient

## Next Session
Day 7 — Week 1 Mini Project: Transistor Switching Circuit
