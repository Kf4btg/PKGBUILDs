**Clean-chroot-manager-manjaro** has been patched to work with the "mkmanjaroroot" command in the Manjaro devtools. I've also included a version of arch-nspawn (renamed to "manjaro-nspawn", natch) that has received the same treatment. **NOTE**: _Probably Obsolete._

**Andromeda-git** has been updated (compared to the PKGBUILD currently on the AUR) to use QBS rather than cmake due the corresponding upstream switch. **NOTE**: _QBS seems to be included in the default QT5 install now, so this PKGBUILD needs updating._

**Qlipper2** now pulls from pvanek's GitHub repo (only real difference is a larger icon), has a proper pkgver(), and fixes compilation by disabling the use of system qxt and QTsingleapp, neither of which are in the arch/Manjaro repos anymore.

**Klook-git** includes a patch (just a quick hack, really) to enable the text-preview for various files (source code, configuration, etc.) that, for whatever reason, are not recognized as plain text.

  Currently includes:
  - json (mimetype recognized as *application/json* )
  - javascript
  - xml
  - ...more as they come up.
