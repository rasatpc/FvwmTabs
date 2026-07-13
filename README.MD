# FvwmTabs
FvwmTabs is a Python/Tk rewrite of the old Perl FVWM tabbing module. It keeps the socket/Tk design, multiple tabbers, FVWM command functions, assigned tabber IDs, right-click menu, and autoSwallow behavior.

FvwmTabs is a single, self-contained executable file. FVWM functions communicate with FvwmTabs through the standard FvwmMFL module, and the FvwmMFL socket client is built into FvwmTabs itself.

# INSTALL and SETUP
# Requirements

- Python 3
- python3-tk
- FVWM3 on X11
- xdotool
- x11-utils, which provides xprop and xwininfo

On Debian, Ubuntu, and MX Linux:
   sudo apt install python3 python3-tk fvwm3 xdotool x11-utils

## FVWM
# .fvwm/config

DestroyFunc StartFunction
AddToFunc StartFunction
+ I Module FvwmMFL
+ I ModulePath ${HOME}/.fvwm/FvwmTabs:+
+ I Module FvwmTabs
