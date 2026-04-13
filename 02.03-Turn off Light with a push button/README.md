# 02.03 — Turn off Light with a Push Button

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

A push button **S2** and a lamp **P2** are connected to a PLC. The push button is a **Normally Open (NO)** contact. The lamp is already turned on by default.

Write a PLC program that meets the following requirements:
- When button **S2** is pressed, the lamp **P2** should be turned off
- When button **S2** is not pressed, the lamp **P2** should remain on

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| S2  | DI (NO) | Push button switch |
| P2  | DO | Lamp |

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started