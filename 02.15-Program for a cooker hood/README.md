# 02.15 — Program for a Cooker Hood

**Book:** Collection of Exercises for PLC Programming — Tom Mejer Antonsen (2024)

---

## Exercise Description

Write a PLC program for a kitchen cooker hood. The cooker hood has a fan that operates at three speeds and built-in lighting. There are six control buttons on the front panel:

| Button | Function |
|--------|----------|
| Turn off light | Turns the light off |
| Turn on light | Turns the light on |
| Turn off fan | Turns the fan off |
| Turn on fan, low speed | Sets fan to low speed |
| Turn on fan, medium speed | Sets fan to medium speed |
| Turn on fan, high speed | Sets fan to high speed |

**Important rules:**
- Only **one** fan speed signal may be TRUE at any given time
- It is **not necessary** to turn the fan off before changing speed — pressing a new speed button switches directly
- If all three speed signals are FALSE, the fan is off

---

## Inputs & Outputs

| Tag | Type | Description |
|-----|------|-------------|
| S1 | DI | Fan low speed button |
| S2 | DI | Fan medium speed button |
| S3 | DI | Fan high speed button |
| Switch_Fan_on  | DI | Fan on button |
| Switch_Fan_off | DI | Fan off button |
| Switch_Light_On  | DI | Light on button |
| Switch_Light_Off | DI | Light off button |
| Fan_Low_Speed  | DO | Fan — low speed output |
| Fan_Mid_Speed  | DO | Fan — medium speed output |
| Fan_High_Speed | DO | Fan — high speed output |
| Light_on | DO | Cooker hood light |

---

## Status

- [x] Studio 5000 — Complete
- [ ] TIA Portal — Not started