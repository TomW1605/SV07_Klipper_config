### SV07 Klipper Config
I recently got an SV07 and immediately proceeded to mess up my config (accidentally changed a pin). I then had an incredibly hard time getting a stock copy of the config from Sovol and could not find it anywhere online.

So to help others that may run into the same issue (and myself when I inevitably need it again) I am uploading my config here including some changes I have made.

## Changes
This is not the stock config but the changes I have made I feel improve the UX of the printer.

These changes include:
- Changing the hot end LED to be a toggle not a brightness slider. The stock config had the PWM frequency set to a 5 second cycle so you couldn't control brightness anyway.
- Added a macro for toggling the hot end LED.
- Added an override for M106 and M107 to also use the large fan on the back.
- Added a toggle that enables and disables the large fan (this requires the [Virtual Pins klipper module](https://github.com/pedrolamas/klipper-virtual-pins)). When switched off it will turn the fan off and when switched on it will set the fan to the same speed as the normal extruder fan.
