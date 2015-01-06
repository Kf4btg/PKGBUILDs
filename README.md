Clean-chroot-manager-manjaro has been patched to work with the "mkmanjaroroot" command in the Manjaro devtools. I've also included a version of arch-nspawn (renamed to "manjaro-nspawn", natch) that has received the same treatment. This little tool makes compiling for other architectures (or just making sure you've really got a pure compiling-environment) so much easier! All kudos to GraySky with Arch.

Andromeda-git has been updated (compared to the PKGBUILD currently on the AUR) to use QBS rather than cmake due the corresponding upstream switch.

Klook-git includes a patch (just a quick hack, really) to enable the text-preview for various files (source code, configuration, etc.) that, for whatever reason, are not recognized as plain text.

  Currently includes:
  - .json (mimetype recognized as *application/json* )
  - ...more as they come up.