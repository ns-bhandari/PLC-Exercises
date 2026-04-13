# 02.14 — Pump Well with One Pump and Two Float Switches

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

A pump well below ground level pumps wastewater away from a house. The pump motor **M1** is controlled based on two float switch contacts that monitor the water level.

**Float switch behaviour:**
- **LS1** (top float) is a **Normally Closed (NC)** contact — gives a FALSE signal when the water level activates it
- **LS2** (bottom float) is a **Normally Open (NO)** contact — gives a TRUE signal when the water level activates it

**Program requirements:**

1. **Low level:** LS2 is FALSE — pump stays off, no wastewater to pump
2. **Rising level:** As water rises, LS2 activates first (TRUE), then LS1 activates (FALSE). Only when LS1 gives a FALSE signal should the pump start
3. **Decreasing level:** Pump continues running even after the level drops below LS1. The pump only stops when the level falls below LS2 (LS2 = FALSE again)

This prevents short-cycling and ensures the well is fully drained each cycle.

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| LS1 | DI (NC) | Top float switch — FALSE when water level is high |
| LS2 | DI (NO) | Bottom float switch — TRUE when water level reached |
| M1  | DO | Pump motor |

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started