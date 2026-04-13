# 02.02 — Turn on Lamp with Two Push Buttons

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

Two push buttons **S1** and **S2**, and a lamp **P1** are connected to a PLC. Both push buttons are **Normally Open (NO)** contacts, connected to separate digital inputs.

Write a PLC program where lamp **P1** is turned on when **both** push buttons S1 and S2 are pressed simultaneously. If both push buttons are not pressed at the same time, the lamp should remain off.

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| S1  | DI (NO) | Push button 1 |
| S2  | DI (NO) | Push button 2 |
| P1  | DO | Lamp |

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started