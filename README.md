**qps-git** pulls from the [QtDesktop][1] version of qps which has been been updated to Qt5 and received a few other small fixes.

**Qlipper2** is now based off of pvanek's GitHub repo (only real difference is a larger icon), has a proper pkgver(), and fixes compilation by disabling the use of system qxt and QTsingleapp, neither of which are in the Arch/Manjaro repos anymore.

**Klook-git** includes a patch (just a quick hack, really) to enable the text-preview for various files (source code, configuration, etc.) that, for whatever reason, are not recognized as plain text.

  Currently includes:
  - json (mimetype recognized as *application/json* )
  - javascript
  - xml
  - ...more as they come up.

[1]: https://github.com/QtDesktop/qps
