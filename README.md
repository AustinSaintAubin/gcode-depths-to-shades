# gcode-depths-to-shades
Convert 3-Axis CNC Router G-code generated from applications such as [Inventables Easel](https://www.inventables.com/technologies/easel), and turn it into G-code suitable for 2-Axis CNC Laser Engraving.

[GRBL](https://github.com/gnea/grbl) Settings:
```
Grbl 1.0c ['$' for help]
$0=10 (step pulse, usec)
$1=255 (step idle delay, msec)
$2=0 (step port invert mask:00000000)
$3=4 (dir port invert mask:00000100)
$4=0 (step enable invert, bool)
$5=0 (limit pins invert, bool)
$6=0 (probe pin invert, bool)
$10=15 (status report mask:00001111)
$11=0.020 (junction deviation, mm)
$12=0.002 (arc tolerance, mm)
$13=0 (report inches, bool)
$20=1 (soft limits, bool)
$21=1 (hard limits, bool)
$22=1 (homing cycle, bool)
$23=3 (homing dir invert mask:00000011)
$24=25.000 (homing feed, mm/min)
$25=750.000 (homing seek, mm/min)
$26=250 (homing debounce, msec)
$27=1.000 (homing pull-off, mm)
$30=1. (rpm max)
$31=0. (rpm min)
$100=40.000 (x, step/mm)
$101=40.000 (y, step/mm)
$102=188.976 (z, step/mm)
$110=8000.000 (x max rate, mm/min)
$111=8000.000 (y max rate, mm/min)
$112=500.000 (z max rate, mm/min)
$120=500.000 (x accel, mm/sec^2)
$121=500.000 (y accel, mm/sec^2)
$122=50.000 (z accel, mm/sec^2)
$130=740.000 (x max travel, mm)
$131=740.000 (y max travel, mm)
$132=100.000 (z max travel, mm)
```

```
Compiled with settings:
#define HOMING_FORCE_SET_ORIGIN // Enabled
//#define PARKING_ENABLE  // Default disabled.
```
