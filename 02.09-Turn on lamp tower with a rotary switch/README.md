# 02.09 — Turn on Lamp Tower with a Rotary Switch

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

A rotary switch with 4 positions and a 3-lamp tower are connected to a PLC. Write a PLC program that lights the lamp tower progressively based on the rotary switch position:

- Position **S0** → all lamps off
- Position **S1** → **P1** on only
- Position **S2** → **P2** on only
- Position **S3** → **P1, P2 and P3** all on

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| S0  | DI | Rotary switch — position 0 (off) |
| S1  | DI | Rotary switch — position 1 |
| S2  | DI | Rotary switch — position 2 |
| S3  | DI | Rotary switch — position 3 |
| P1  | DO | Lamp tower — light 1 |
| P2  | DO | Lamp tower — light 2 |
| P3  | DO | Lamp tower — light 3 |

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started