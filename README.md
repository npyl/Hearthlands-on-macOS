# Hearthlands on macOS
Automator script to run Hearthlands game on macOS with one click.

# Requirements
Wine 2.0.3 (has been tested only on this version)

# How it works
Uses spotlight to find location of Hearthlands.exe executable and passes it as argument into this SHELL script:

`
EXECUTABLE=$1
/usr/local/bin/wine start /unix $EXECUTABLE
`

This ensures that wherever you put the game it will start. (Unless Spotlight can't index the drive/place the game is stored)
