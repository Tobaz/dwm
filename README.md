# dwm - dynamic window manager
dwm is an extremely fast, small, and dynamic window manager for X.
This is my customized configuration of DWM, based of off rudyghill's build
(https://github.com/rudyghill/dwm)

## Requirements
In order to build dwm you need the Xlib header files.


## Installation
Edit config.mk to match your local setup (dwm is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dwm (if
necessary as root):

```
make clean install
```


## Running dwm
There are two scripts included, scripts/dwmstatus and scripts/startdwm. Add the
following into your .xinitrc

~/script/path/here/dwmstatus &
~/script/path/here/startdwm

This will start the statusbar update script in the background, and then start
the actual DWM instance. This is run in a while loop, so closing DWM will
instantly restart it, allowing you to quickly see your applied configurations
without requiring logging out and back in, restarting your X server etc

## Configuration
The configuration of dwm is done by creating a custom config.h
and (re)compiling the source code.

## Patches Applied
- attachbottom
- autostart
- horizontal grid mode
- three column mode
- cycle layouts
- useless gaps
