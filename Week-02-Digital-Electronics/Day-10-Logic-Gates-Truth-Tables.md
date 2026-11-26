# Day 10 — Logic Gates and Truth Tables

## Date
26 November 2026

## Topics Studied
- AND, OR, NOT, NAND, NOR, XOR, XNOR gates
- Truth tables for all 7 gates
- Universal gates: NAND and NOR
- Verilog operators for each gate
- Number of truth table rows = 2^n (n = number of inputs)

## Gate Summary

| Gate | Expression | Key Rule |
|------|------------|----------|
| AND | Y = A·B | Output 1 only when ALL inputs 1 |
| OR | Y = A+B | Output 1 when ANY input 1 |
| NOT | Y = A' | Output opposite of input |
| NAND | Y = (A·B)' | Opposite of AND |
| NOR | Y = (A+B)' | Opposite of OR |
| XOR | Y = A⊕B | Output 1 when inputs DIFFERENT |
| XNOR | Y = (A⊕B)' | Output 1 when inputs SAME |

## Verilog Operators

| Gate | Operator | Example |
|------|----------|---------|
| AND | & | assign y = a & b; |
| OR | \| | assign y = a \| b; |
| NOT | ~ | assign y = ~a; |
| NAND | ~& | assign y = ~(a & b); |
| NOR | ~\| | assign y = ~(a \| b); |
| XOR | ^ | assign y = a ^ b; |
| XNOR | ~^ | assign y = ~(a ^ b); |

## Universal Gates
- NAND and NOR are universal gates
- Any logic circuit can be built using only NAND or only NOR gates
- NAND preferred in chip design — fewer transistors than AND

## Quiz Results

| Question | Answer | Result |
|----------|--------|--------|
| Q1. 3-input AND truth table, rows? | Correct table, 8 rows (2³) | ✅ |
| Q2. XNOR truth table | Correct — 1,0,0,1 | ✅ |
| Q3. NAND A=1,B=1 → output? | 0 | ✅ |
| Q4. NOR A=0,B=0 → output? | 1 | ✅ |
| Q5. Universal gates and why? | NAND and NOR, any gate implementable | ✅ |
| Q6. XOR same/different inputs? | Same=0, Different=1 | ✅ |
| Q7. Verilog: Y=(A OR B) AND (NOT C) | assign y = (A\|B) & (~C); | ✅ |

Score: 7 / 7

## Notes to Remember
1. n inputs → 2^n rows in truth table
2. Verilog is case sensitive — A and a are different signals

## VLSI Connection
- Every Verilog gate maps to physical CMOS transistors on chip
- NAND gate needs fewer transistors than AND — preferred in synthesis
- XOR is core of adder circuits — used in ALU design

## Next Session
Day 11 — Boolean Algebra and De Morgan's Laws
