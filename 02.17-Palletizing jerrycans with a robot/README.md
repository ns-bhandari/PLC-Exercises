# 02.17 — Palletizing Jerrycans with a Robot

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

Write a PLC program for a small robotic palletizing system that places two jerrycans onto a pallet. A robot arm picks jerrycans from an upper conveyor belt and places them on a pallet carried by a lower conveyor belt (motor **M1**).

**System behaviour:**

1. The robot is only allowed to start working when sensors **B1**, **B2**, and **B3** all give a TRUE signal
2. The PLC signals the robot by setting **M3_DI** to TRUE
3. While the robot is working, the robot controller output **M3_DO** is TRUE
4. When the robot is working, lamp **P1** must be turned on
5. When the robot finishes (M3_DO goes FALSE), the PLC must move the filled pallet away by setting motor **M1** to TRUE
6. A new empty pallet is moved in by M1 until sensor **B1** gives a TRUE signal (pallet in position)

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| B1  | DI | Pallet position sensor |
| B2  | DI | Sensor 2 |
| B3  | DI | Sensor 3 |
| M3_DO | DI | Robot controller output — TRUE when robot is working |
| M1    | DO | Conveyor motor |
| M3_DI | DO | Robot controller input — TRUE to start robot |
| P1    | DO | Lamp — on when robot is working |

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started