# Day 11 — Boolean Algebra and De Morgan's Laws

## Date
27 November 2026

## Topics Studied
- Boolean algebra laws: Identity, Null, Idempotent, Complement, Commutative, Associative, Distributive, Absorption
- De Morgan's Law 1: (A·B)' = A' + B'
- De Morgan's Law 2: (A+B)' = A' · B'
- Boolean simplification to reduce gate count

## Key Laws

### De Morgan's Laws
- (A·B)' = A' + B'  → break bar, AND becomes OR
- (A+B)' = A' · B'  → break bar, OR becomes AND

### Important Laws
- A + A·B = A  (absorption)
- A + 1 = 1   (null)
- A·A' = 0    (complement)
- A + A' = 1  (complement)
- (A')' = A   (double complement)

## Quiz Results

| Question | Answer | Result |
|----------|--------|--------|
| Q1. Y = A + A·B | A (Null law: 1+B=1) | ✅ |
| Q2. Y = A·B + A·B' + A'·B | A+B | ✅ |
| Q3. (A·B·C)' | A'+B'+C' | ✅ |
| Q4. (A'+B')' | A·B | ✅ |
| Q5. (A+B)·(A'+B) | Got A, correct = B (A·A'=0 error) | ❌ |
| Q6. ~(~A & ~B) → Verilog | assign Y = A\|B | ✅ |

Score: 5 / 6

## Q5 Correct Solution
(A+B)·(A'+B)
= A·A' + A·B + B·A' + B·B
= 0 + A·B + A'·B + B
= B·(A + A' + 1)
= B·1 = B

## Mistake to Fix
- A·A' = 0 always (complement law)
- Never write A·A' = A

## VLSI Connection
- Synthesis tools apply Boolean algebra automatically to reduce gate count
- Fewer gates = smaller chip area = lower power consumption
- De Morgan's Law used to convert between NAND/NOR implementations

## Next Session
Day 12 — Karnaugh Maps (K-Maps)
