# Day 8 — Number Systems: Binary, Decimal, Octal and Hexadecimal

## Date
24 November 2026

## Topics Studied
- Decimal: base 10, digits 0-9, powers of 10
- Binary: base 2, digits 0-1, powers of 2
- Octal: base 8, digits 0-7, powers of 8
- Hexadecimal: base 16, digits 0-9 and A-F, powers of 16

## Key Conversion Methods

### Binary to Decimal
- Multiply each bit by its power of 2, add all results

### Decimal to Binary
- Divide by 2 repeatedly, read remainders bottom to top

### Binary to Octal
- Group bits in 3s from right, convert each group directly
- Never go through decimal as middle step

### Binary to Hexadecimal
- Group bits in 4s from right, convert each group directly

### Hex/Octal to Decimal
- Multiply each digit by its power of base, add all results

## Powers of 2 (Memorized)
2⁰=1, 2¹=2, 2²=4, 2³=8, 2⁴=16, 2⁵=32, 2⁶=64, 2⁷=128

## Quiz Results

| Question | Answer | Result |
|----------|--------|--------|
| Q1. 1101 binary → decimal | 13 | ✅ |
| Q2. 25 decimal → binary | 11001 | ✅ |
| Q3. 101110 binary → octal | 56 | ✅ |
| Q4. 53 octal → decimal | 43 (wrong subscript ₂ instead of ₁₀) | ½ |
| Q5. 11001010 binary → hex | CA | ✅ |
| Q6. 3B hex → decimal | 59 | ✅ |

Score: 5.5 / 6

## Mistakes to Fix
1. Always write correct base subscript: ₁₀ decimal, ₂ binary, ₈ octal, ₁₆ hex
2. Binary to octal: always use grouping method, never go through decimal

## VLSI Connection
- Chips use binary internally for all data
- Hex used in Verilog: 8'hFF, 4'hA
- Memory addresses written in hex in all VLSI tools

## Next Session
Day 9 — Binary Arithmetic and 1's and 2's Complement
