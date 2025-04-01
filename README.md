# PicoVector Fonts / Alright Fonts

A collection of sample Alright Fonts for using with PicoVector on Pimoroni RP2040
and RP2350-based microcontroller boards.

These fonts are all taken from Google Fonts: https://fonts.google.com/

They are converted on the fly with Alright Fonts: https://github.com/Gadgetoid/alright-fonts/tree/feature/16bit-afinate

:warning: Note this currently uses my 16bit-afinate branch for much more detailed contours where necessary.

You will find converted fonts available for download in the latest release: https://github.com/Gadgetoid/alright-fonts/releases/latest

To add your own:

1. Grab a zipped otf/ttf font from https://fonts.google.com/
2. Unzip it
3. Copy the directory and *all files* into google-fonts/
4. Run `pip install -r requirements.txt` (you may need a virtual env)
5. Run `./convert` and test your font!
6. Raise a PR with your addition!