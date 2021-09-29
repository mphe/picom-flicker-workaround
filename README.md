# Picom Flicker Workaround

Workaround to stop picom from flickering after waking up the screen.
See <https://github.com/yshui/picom/issues/578>

The tool listens for screen-wakeup-events and restarts picom when triggered.

It was forked from <https://github.com/unixdj/xssstart> and adapted to run a command when the screensaver gets turned off instead of on.


### Usage

Run `make` to compile, then start it using `./xssstart bash picom.sh` or just `./run.sh`.

Add it to your `.xinitrc` or session startup to run it automatically on boot.
