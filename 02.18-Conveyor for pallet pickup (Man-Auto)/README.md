# 02.18 — Conveyor for Pallet Pickup (Manual/Auto)

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

Write a PLC program for a conveyor belt that moves pallets loaded with goods to a pickup point where a forklift can collect them.

**User interface — 3 switches:**
- **S1** — On/Off turn switch (enables the conveyor system)
- **S2** — Auto/Manual mode selector switch
- **S3** — Manual run push button (only active in manual mode)

**Light tower — 2 lamps:**
- **P1** — Conveyor is running (moving next pallet into position)
- **P2** — Pallet is ready for pickup at the end of the belt

**Program requirements:**

- In **AUTO mode**: the conveyor motor M1 runs automatically when S1 is on
- In **MANUAL mode**: the motor M1 only runs while push button S3 is held down
- In **both modes**: the conveyor must stop when sensor **B1** gives a TRUE signal (pallet has reached the pickup point — prevents it from falling off the belt)

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| S1  | DI | On/Off turn switch |
| S2  | DI | Auto/Manual mode selector |
| S3  | DI | Manual run push button |
| B1  | DI | Pallet at end sensor |
| M1  | DO | Conveyor motor |
| P1  | DO | Lamp — conveyor running |
| P2  | DO | Lamp — pallet ready for pickup |

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started