# 02.07 — Turn on Lamp with Two Push Buttons (NO, NC)

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

Two push buttons and a lamp are connected to a PLC. One push button is a **Normally Open (NO)** contact and the other is a **Normally Closed (NC)** contact.

Write a PLC program where lamp **P1** is turned on when either push button is pressed — demonstrating how NO and NC contacts are handled differently in ladder logic.

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| S1  | DI (NO) | Normally Open push button |
| S2  | DI (NC) | Normally Closed push button |
| P1  | DO | Lamp |

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started