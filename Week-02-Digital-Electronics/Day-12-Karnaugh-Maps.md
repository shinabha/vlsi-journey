# Day 12 — Karnaugh Maps (K-Maps)

## Date
28 November 2026

## Topics Studied
- K-Map: visual Boolean simplification method
- 2-variable K-Map: 4 cells
- 3-variable K-Map: 8 cells, Gray code column order
- 4-variable K-Map: 16 cells
- Grouping rules: powers of 2, rectangular, wrap-around allowed
- Don't care conditions: marked X, treated as 0 or 1 for larger groups

## Critical Rules

### Column Order (Gray Code)
- Always: 00 → 01 → 11 → 10
- Never: 00 → 01 → 10 → 11

### Group Size and Variables
| Group Size | Variables Eliminated |
|------------|---------------------|
| 2 cells | 1 variable |
| 4 cells | 2 variables |
| 8 cells | 3 variables |
| 16 cells | 4 variables |

### Reading a Group
- Find variables that are CONSTANT across all cells in the group
- Those constant variables form the term
- Changing variables are eliminated

## Worked Examples
- Q1: Y = A'B' + A'B + AB → K-Map → Y = A' + B
- Q2: Truth table with C'=1 pattern → Y = C'
- Q5: 4-var map, group of 8 → 3 variables eliminated, 1 remains

## Quiz Results

| Question | Answer | Result |
|----------|--------|--------|
| Q1. 2-var K-Map simplification | A'+B | ✅ |
| Q2. 3-var K-Map from truth table | C' (wrap-around group) | ✅ |
| Q3. Column order for 3-var K-Map | 00→01→11→10 | ✅ |
| Q4. Group of 4 eliminates how many? | Said 3, correct = 2 | ❌ |
| Q5. Group of 8, variables remaining? | 3 eliminated correct, remaining=1 | ½ |

Score: 4 / 5

## Mistake to Fix
- Group of 4 always eliminates 2 variables in any K-Map size
- Always answer exactly what the question asks (eliminated vs remaining)

## VLSI Connection
- Synthesis tools use K-Map equivalent algorithms internally
- Fewer product terms = fewer gates = smaller chip area
- Don't cares used heavily in control logic to minimize gate count

## Next Session
Day 13 — Combinational Circuits: Half Adder, Full Adder, MUX, Decoder
