# 02.10 — Programming of Self-Hold

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

A start button **S1**, a stop button **S2**, and a lamp **P1** are connected to a PLC. Write a PLC program using a **self-hold (seal-in) circuit**:

- Pressing **S1** turns on lamp **P1** and the lamp stays on even after S1 is released
- Pressing **S2** turns off lamp **P1**

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| S1  | DI | Start push button |
| S2  | DI | Stop push button |
| P1  | DO | Lamp |

---

## Key Concept

The self-hold circuit is one of the most fundamental patterns in PLC programming. The output coil (P1) is used as a contact in parallel with the start button, so the output latches itself on after the start button is released.

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started