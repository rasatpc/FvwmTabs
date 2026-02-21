# FvwmTabs
An upgraded generic tabbing module for Fvwm3, included in Fvwm2.

# Description
The FvwmTabs module is capable of swallowing any fvwm window & treating it as a tab in a tab-manager window. A tab-manager is sometimes called a tabber. Each tab-manager can store any number of windows, each in its own tab.

# Invocation
FvwmTabs is invoked by inserting the lines:

ModulePath ${HOME}/.fvwm/modules:+
Module FvwmTabs
in your .fvwmrc or config file.

# Installing Dependencies
FvwmTabs requires 2 CPAN modules (that are NOT distributed with fvwm) to be installed on your system. They are Tk and X11::Protocol.

Debian: perl-tk and libx11-protocol-perl
Arch Linux: perl-tk and perl-x11-protocol

FvwmTabs will tell you if you do not have these packages installed when you (try to) start it.
