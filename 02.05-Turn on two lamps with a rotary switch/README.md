# 02.05 — Turn on Two Lamps with a Rotary Switch

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

A rotary switch **S1** is connected to a digital input, and two lamps **P1** and **P2** are connected to separate digital outputs.

Write a PLC program that operates as follows:
- If the rotary switch **S1** is in position **"1" (on)**, both lamps P1 and P2 should be turned on
- If the rotary switch **S1** is in position **"0" (off)**, both lamps P1 and P2 should be turned off

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| S1  | DI | Rotary switch (2-position) |
| P1  | DO | Lamp 1 |
| P2  | DO | Lamp 2 |

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started