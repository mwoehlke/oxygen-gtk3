=======================
 Oxygen style for GTK3
=======================

Are you a KDE user that is fed up with ugly GTK3 applications that don't match your Qt/KDE color scheme? Do you dislike the other available GTK3 widget styles? Does the excessive padding of other GTK3 themes cramp your style? Are you in love with the Oxygen widget style (quite possibly the best widget style ever designed)?

Have you been searching high and low for a port of Oxygen to GTK3?

Well, look no further! This is a pure CSS port of the excellent Oxygen style to a GTK3 pure-CSS theme.

Usage
-----

Using this theme couldn't be easier. Just clone the repository to ~/.themes/Oxygen/gtk-3.0, or create a symlink with that name to wherever you clone this repositry. Then go to System Settings → Application Style → GNOME Application Style and change the GTK3 Theme to Oxygen.

At this time, GTK3 is unable to inherit the KDE color scheme, so you will have to manually select or set up your color scheme. The default is Zion Dark. Available color schemes may be found in the ``colors`` subdirectory. Edit ``gtk.css`` and change the line that imports the color scheme CSS to import your selected scheme.

In the future, I hope to create a tool that will create a new color scheme CSS from the current color scheme. Perhaps at some point I will modify this theme to support user-adjustable colors, and modify KDE's color configuration module to automatically export the KDE color scheme.

Known Bugs
----------

The GTK3 Oxygen theme attempts to replicate Oxygen's gradient window backgrounds, but KWin expects non-Qt applications to have a solid background. The title bars of GTK3 applications will not match the rest of the window as a result. Also, GTK3 does not support multiple or radial gradients, so the background gradient has only the main linear-vertical component.
