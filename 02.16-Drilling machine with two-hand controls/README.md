# 02.16 — Drilling Machine with Two-Hand Controls

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

Write a PLC program for a drilling machine with two-hand safety controls. The machine consists of a drilling motor **M1** driven by an electric cylinder (actuator), two push buttons **S1** and **S2**, and a workpiece sensor **B3**.

**How it works:**

**Workpiece placement:**
- A workpiece must be placed in the fixture under the drilling machine
- Sensor **B3** activates (TRUE) when the workpiece is correctly positioned
- A small LED lamp (**B3_Lamp**) turns on when B3 is active, indicating the machine is ready

**Starting the drill:**
- Both push buttons **S1** and **S2** must be pressed simultaneously to start — this is a two-hand safety control to keep the operator's hands away from the drill
- The machine can only start if B3 is TRUE (workpiece in place)

**Cylinder direction:**
- The cylinder moves **down** when **M1_K2** is TRUE
- The cylinder moves **up** when **M1_K1** is TRUE
- M1_K1 and M1_K2 must never be TRUE at the same time

**Limit sensors:**
- **M1_B2** gives TRUE when drilling is deep enough — cylinder must return upward
- **M1_B1** gives TRUE when the cylinder has returned to the top — machine stops

**Safety:** If the operator releases either button at any point, the machine stops immediately.

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| S1  | DI | Two-hand push button 1 |
| S2  | DI | Two-hand push button 2 |
| B3  | DI | Workpiece presence sensor |
| M1_K1 | DI | Up direction signal |
| M1_K2 | DI | Down direction signal |
| M1_B1 | DI | Upper stop sensor |
| M1_B2 | DI | Lower stop sensor |
| M1_Downward | DO | Motor — downward direction |
| M1_Upward   | DO | Motor — upward direction |
| B3_Lamp | DO | Workpiece indicator LED |

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started