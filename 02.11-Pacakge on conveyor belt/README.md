# 02.11 — Package on Conveyor Belt

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

A conveyor belt system with a motor **M1**, a rotary start switch **S1**, and a package detection sensor **B1** are connected to a PLC.

Write a PLC program that operates as follows:
- When **S1** is turned on and no package is detected, the conveyor motor **M1** starts
- The motor continues running (self-hold) until sensor **B1** detects a package at the end of the belt
- When **B1** detects a package, the conveyor stops

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| S1  | DI | Rotary start switch |
| B1  | DI | Package detection sensor |
| M1  | DO | Conveyor motor |

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started