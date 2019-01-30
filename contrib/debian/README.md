
Debian
====================
This directory contains files used to package lightpaycoind/lightpaycoin-qt
for Debian-based Linux systems. If you compile lightpaycoind/lightpaycoin-qt yourself, there are some useful files here.

## lightpaycoin: URI support ##


lightpaycoin-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install lightpaycoin-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your lightpaycoinqt binary to `/usr/bin`
and the `../../share/pixmaps/lightpaycoin128.png` to `/usr/share/pixmaps`

lightpaycoin-qt.protocol (KDE)

