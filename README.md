# PicoVector Fonts / Alright Fonts

A collection of sample Alright Fonts for using with PicoVector on Pimoroni RP2040
and RP2350-based microcontroller boards.

These fonts are all taken from Google Fonts: https://fonts.google.com/

They are converted on the fly with Alright Fonts: https://github.com/Gadgetoid/alright-fonts/tree/feature/16bit-afinate

:warning: Note this currently uses my 16bit-afinate branch for much more detailed contours where necessary.

You will find converted fonts available for download in the latest release: https://github.com/Gadgetoid/alright-fonts/releases/latest

To use this repository:

1. Clone this repository: `git clone https://github.com/pimoroni/picovector-fonts`
2. Grab submodules: `cd picovector-fonts` then `git submodule update --init`
3. Run `pip install -r requirements.txt` (you may need a virtual environment)
4. Run `./convert` to convert everything in `google-fonts/`

To add your own:

1. Grab a zipped otf/ttf font from https://fonts.google.com/
2. Unzip it
3. Copy the directory and *all files* into `google-fonts/`
4. Run `./convert` and test your font!
5. Raise a PR with your addition!

Your PR should include the fonts and their license files.

The contents of any `static` directories should be moved to the main font directory.

## Troubleshooting

- `error: externally-managed-environment` means you need to be installing your Python packages into a virtual environment. You can set one up with `python3 -m venv .venv` and activate it with `source .venv/bin/activate`.

- If you get a `zip: command not found` error, you might need to `sudo apt install zip` and run `./convert` again.
