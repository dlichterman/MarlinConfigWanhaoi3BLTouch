# MarlinConfigWanhaoi3BLTouch

This is a sample config to add BLTouch to the WanHao i3 or similar. Most is copied from [Matthieu Heimer on his blog](http://blog.osdev.org/3d/printing/2019/10/13/wanhao-duplicator-i3-bltouch.html) but there were some tweaks I needed for the specific mount, and also my printer. Mine is one of the early Wanhao models with the "wrong" resistor for the thermistors, so I copied the code from Marlin 2.0/TH3D unified and added it to Marlin 1.1.x.

This config allows LCD, SD, and BL Touch, all barely fitting into the space available.

Specific changes I have made:
- Thermistor resistor fix - thermistor table change
- Reversing scroll direction to match original
- Tweaking thermal protection variables
- FAN_SOFT_PWM so the damn thing doesn't make noise when running the part fan
