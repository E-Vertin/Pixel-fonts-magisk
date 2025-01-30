# Pixel-fonts-magisk
A simple Magisk module to apply Google Sans family fonts extracted from a Pixel 9 running Android 15 QPR1 globally.

## Mechanism
The Roboto font family was mapped by the Android system to apply globally, `Roboto-Regular.ttf` and `RobotoFlex-Regular.ttf` to be exact.

This Magisk module applies Google Sans globally by simply swapping two font files mentioned above to `GoogleSans-Regular.ttf` and `RobotoFlex-Regular.ttf` respectively.

## Known issues

### The transition from Always On Display to Lock Screen

If you take a close look to the transition animation of Pixel phones, from Android's AOD to Lock Screen, the clock face font will transform from Google Sans Light to Google Sans Bold which I believe was made possible via a technology called "Variable Font", but sadly, I do not know how to implement it into this Magisk module.

If you have any idea, please do not hesitate to fill a Pull request!

### You tell me.