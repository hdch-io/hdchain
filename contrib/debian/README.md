
Debian
====================
This directory contains files used to package hdchd/hdch-qt
for Debian-based Linux systems. If you compile hdchd/hdch-qt yourself, there are some useful files here.

## hdch: URI support ##


hdch-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install hdch-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your hdch-qt binary to `/usr/bin`
and the `../../share/pixmaps/hdch128.png` to `/usr/share/pixmaps`

hdch-qt.protocol (KDE)

