# 02.06 — Turn on and off Lamps with a Push Button

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

A push button **S1** and two lamps **P1** and **P2** are connected to a PLC. The push button is a **Normally Open (NO)** contact. One of the lamps is turned on by default.

Write a program that operates as follows:
- When push button **S1** is pressed: lamp **P1** turns off, lamp **P2** turns on
- When push button **S1** is not pressed: lamp **P1** is on, lamp **P2** is off

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| S1  | DI (NO) | Push button switch |
| P1  | DO | Lamp 1 (on by default) |
| P2  | DO | Lamp 2 |

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started