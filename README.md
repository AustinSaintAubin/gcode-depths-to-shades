# gcode-depths-to-shades
Convert 3-Axis CNC Router G-code generated from applications such as [Inventables Easel](https://www.inventables.com/technologies/easel), and turn it into G-code suitable for 2-Axis CNC Laser Engraving.

# Screenshot
![gcode-depths-to-shades](https://raw.githubusercontent.com/AustinSaintAubin/gcode-depths-to-shades/master/media/screenshot.png)

[GRBL](https://github.com/gnea/grbl) Spindle RPM Settings: (Used for Laser PWM)
```
$30=255 (rpm max)
$31=0 (rpm min)
```
