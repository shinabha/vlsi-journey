# Day 9 — Binary Arithmetic and 1's and 2's Complement

## Date
25 November 2026

## Topics Studied
- Binary addition: 4 rules, carry propagation
- Binary subtraction: borrow method
- 1's complement: flip all bits
- 2's complement: flip all bits then add 1
- Subtraction using 2's complement: A-B = A + 2's complement of B
- 8-bit 2's complement range: -128 to +127

## Key Rules

### Binary Addition
- 0+0=0, 0+1=1, 1+0=1, 1+1=0 carry 1

### 1's Complement
- Flip every bit

### 2's Complement
- 1's complement + 1
- Used for negative numbers and subtraction in hardware

### Subtraction Using 2's Complement
- A - B = A + (2's complement of B)
- Ignore final carry bit

## Worked Examples
- 1101 + 1010 = 10111 (13+10=23) ✅
- 1001 - 0101 = 0100 (9-5=4) ✅
- 2's complement of 10110100 = 01001100
- 12 - 5 using 2's complement = 0111 = 7 ✅

## Quiz Results

| Question | Answer | Result |
|----------|--------|--------|
| Q1. 1101+1010 | 10111 | ✅ |
| Q2. 1001-0101 | 0100 | ✅ |
| Q3. 1's complement of 10110100 | 01001011 | ✅ |
| Q4. 2's complement of 10110100 | 01001110 (correct=01001100, carry error) | ❌ |
| Q5. 12-5 using 2's complement | 0111=7 | ✅ |
| Q6. 8-bit 2's complement range | +127 to -128 | ✅ |

Score: 5 / 6

## Mistake to Fix
- 2's complement addition: always trace carry propagation column by column
- When carry is generated, it must be added to the next column before moving on

## VLSI Connection
- ALU in chips performs subtraction using 2's complement internally
- No dedicated subtraction hardware needed — saves chip area
- Overflow detection is a real hardware design problem

## Next Session
Day 10 — Logic Gates and Truth Tables
