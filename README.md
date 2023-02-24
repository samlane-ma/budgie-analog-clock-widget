# Budgie Analog Clock Widget

### This project was merged into the analogue-clock-applet

### The updated project can be found at:
### https://github.com/samlane-ma/analogue-clock-applet

### It will still be able to be used separately if so desired.

![Screenshot](./images/analog-clock.png)

An analog syle clock for the Budgie Desktop Raven panel
This widget will evenually be a part of the Analogue Clock Applet.

However, though it is a work in progress, it is 100% fully funtcional in its current form.

Dependencies

* gtk+-3.0
* budgie-raven-plugin-1.0
* libpeas-gtk-1.0

To install (for Debian/Ubuntu):

    mkdir build
    cd build
    meson setup --prefix=/usr --libdir=/usr/lib
    ninja
    sudo ninja install
