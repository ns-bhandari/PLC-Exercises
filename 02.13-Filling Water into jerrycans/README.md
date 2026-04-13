# 02.13 — Filling Water into Jerrycans

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

A conveyor belt system fills water into jerrycans automatically. A motor **M1** drives the conveyor. An electric water valve **Q1** controls the water flow. Three sensors monitor can position and fill level.

**System behaviour:**

1. The conveyor moves jerrycans to the right when **M1** is TRUE
2. When sensor **B1** gives a **FALSE** signal and sensor **B2** gives a **TRUE** signal, the jerrycan is correctly positioned for filling
3. Valve **Q1** opens (TRUE) to fill the jerrycan when the can is in position and not yet full
4. Sensor **B5** gives a TRUE signal when the jerrycan is full — valve **Q1** must close
5. Once filled, **M1** runs again to move the full can away and bring in the next empty one

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| B1  | DI | Position sensor 1 — FALSE when can is in fill position |
| B2  | DI | Position sensor 2 — TRUE when can is in fill position |
| B5  | DI | Fill level sensor — TRUE when jerrycan is full |
| M1  | DO | Conveyor motor |
| Q1  | DO | Electric water valve |

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started