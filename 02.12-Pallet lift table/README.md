# 02.12 — Pallet Lift Table

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

A pallet lift table raises and lowers pallets to working height, operated by a foot panel with two switches. An actuator **M1** (motor cylinder) moves the table up and down.

Write a PLC program with the following behaviour:

- The lift moves **up** when switch **S2** is held down (stops at upper limit **B2**)
- The lift moves **down** when switch **S1** is held down (stops at lower limit **B1**)
- The lift must **not move** if both S1 and S2 are pressed at the same time
- Sensor **B2** gives a TRUE signal when the lift should stop moving up
- Sensor **B1** gives a TRUE signal when the lift should stop moving down

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| S1  | DI | Foot switch — down |
| S2  | DI | Foot switch — up |
| B1  | DI | Lower limit sensor |
| B2  | DI | Upper limit sensor |
| M1_Downward | DO | Actuator — downward direction |
| M1_Upward   | DO | Actuator — upward direction |

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started