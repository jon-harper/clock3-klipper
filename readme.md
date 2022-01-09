# Clock 3 Klipper Configuration Files

## About

This repository contains a ready-to-go Klipper configuration for the stock configuration of Clock 3:

- Dependencies: MainsailOS
- MCU: BIGTREETECH Octopus
- Drivers: TMC2209
- Hotend: GulfCoast Robotics Black Edition V6 (300C capable)
- Build Volume: 300x300x350mm
- Display: FYSETC 12864 Mini or BIGTREETECH 12864 Mini
- Lights: WS2813/WS2815
- A/B Steppers: Stepperonline 17HM19-2004S / 2A, 0.9 degree
- Z Steppers: Stepperonline 1-17HS15-1504S-X1 / 1.5A, 1.8 degree
- Extruder Stepper: Stepperonline 17HS10-0704S / 0.7A, 1.8 degree
- Fans:
  - Hotend fan (24V)
  - Part cooling fan (24V)
  - Chamber: 2 blowers (24V)
  - Electronics: 3-4 fans (12V)
  
The main repository for Clock 3, including documentation, can be found [here](https://github.com/jon-harper/clock3).

## Example Usage

From a shell on the Clock 3 Raspberry Pi:

```
cd ~/klipper_config
git clone https://github.com/jon-harper/clock3-klipper clock3
```

Modify your `printer.cfg` so that it looks like this:

```
[include mainsail.cfg]

# Any other initialization before declaring [mcu] here

[include clock3/main.cfg]

# Any final configuration declarations or inclusions
```