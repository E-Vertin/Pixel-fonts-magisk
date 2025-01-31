# Pixel-fonts-magisk
A simple Magisk module to apply Google Sans family fonts extracted from a Pixel 9 running Android 15 QPR1 globally.

**ONLY VERIFIED ON LINEAGE OS 22.1 WITH APATCH**

## Disclaimer

* I am not responsible for bricked devices, dead SD cards, thermonuclear war, or you getting fired because the alarm app failed.

* Please do some research if you have any concerns about this module before flashing it!

* YOU are choosing to make these modifications; I AM NOT RESPONSIBLE for any consequences.

## Mechanism

- v1.1

The Roboto font family was mapped by the Android system to apply globally, `Roboto-Regular.ttf` and `RobotoFlex-Regular.ttf` to be exact.

This Magisk module adds Google Sans font to `/system/etc/fonts` and manipulates `/system/etc/fonts.xml` and `/system/etc/font_fallback.xml` to define the Google Sans family and make the family "sans-serif" and "roboto-flex" to use `GoogleSans-Regular.ttf` and `GoogleSansFlex-Regular.ttf` as source files. 

Applying custom font by editing the font mapping configuration rather than replacing font itself might be a better idea...


- v1.0

The Roboto font family was mapped by the Android system to apply globally, `Roboto-Regular.ttf` and `RobotoFlex-Regular.ttf` to be exact.

This Magisk module applies Google Sans globally by simply swapping two font files mentioned above to `GoogleSans-Regular.ttf` and `RobotoFlex-Regular.ttf` respectively.

## Known issues

### The transition from Always On Display to Lock Screen

If you take a close look to the transition animation of Pixel phones, from Android's AOD to Lock Screen, the clock face font, Google Sans Clock, will transform from Light to Bold which I believe was made possible via a technology called "Variable Font", but sadly, I do not know how to implement it into this Magisk module.

If you have any idea, please do not hesitate to fill a Pull request!

### You tell me.