**bpython-git** wouldn't even run when I first installed it; I added the missing required dependencies to the PKGBUILD.

**gtk-theme-mona** was added as I feel it matches nicely with my dark-breeze-style QtCurve setup (and QtCurve only provides an engine for gtk2-based applications, not gtk3). PKGBUILD tweaks the gtk3 theme slightly and also enables the dark gtk2 scheme for good measure.

**qps-git** pulls from the [QtDesktop][1] version of qps which has been been updated to Qt5 and received a few other small fixes.

**Qlipper2** is now based off of pvanek's GitHub repo (only real difference is a larger icon), has a proper pkgver(), and fixes compilation by disabling the use of system qxt and QTsingleapp, neither of which are in the Arch/Manjaro repos anymore.

**Klook-git** includes patches (read: hacks) to **1)** make the text-preview use the system fixed-width font and **2)** enable the text-preview for various files (source code, configuration, etc.) that, for whatever reason, are not recognized as plain text.

  Currently includes:
  - json (mimetype recognized as *application/json* )
  - javascript
  - xml
  - perl
  - .desktop files
  - ...more as they come up.

[1]: https://github.com/QtDesktop/qps
