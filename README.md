# qipdisp

QIPDISP is a tiny little program that displays the computer's
current LAN IP address in a window. QIPDISP is primarily intended
to run on computers that do not have a keyboard or mouse attached,
as is common in systems used inside a visual neuroscience setup.

QIPDISP is smart enough not to display 127.0.0.1 when the computer
is attached to a LAN, but not smart enough to punch through a
router and determine the computer's WAN address.

QIPDISP accepts window manager command line argument, so you can
run it, for example, as

    qipdisp --geometry -0+0

to place the window in the top-right corner of the screen.

The normal way to terminate QIPDISP is by way of the "kill" command
from an (ssh) terminal. (That is because QIPDISP will typically run
on systems without a keyboard or mouse.) However, mouse clicks
inside QIPDISP's window also terminate it.
