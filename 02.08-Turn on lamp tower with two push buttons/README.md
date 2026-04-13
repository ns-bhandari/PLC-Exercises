# 02.08 — Turn on Lamp Tower with Two Push Buttons

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

Two push buttons and a 3-lamp tower (P1, P2, P3) are connected to a PLC. Write a PLC program that lights the correct lamp based on which button(s) are pressed:

- Only **S1** pressed → **P1** on
- Only **S2** pressed → **P2** on
- Both **S1 and S2** pressed → **P3** on
- Neither pressed → all lamps off

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| S1  | DI | Push button 1 |
| S2  | DI | Push button 2 |
| P1  | DO | Lamp tower — light 1 |
| P2  | DO | Lamp tower — light 2 |
| P3  | DO | Lamp tower — light 3 |

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started