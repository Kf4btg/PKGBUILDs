Note on installation order for idevice-software:

Install order: 
	libplist -> libusbmuxd -> libimobiledevice -> usbmuxd, ifuse, ideviceinstaller, ...

Clean-chroot-manager-manjaro has been patched to work with the "mkmanjaroroot" command in the Manjaro devtools. I've also included a version of arch-nspawn (renamed to "manjaro-nspawn", natch) that has received the same treatment. This little tool makes compiling for other architectures (or just making sure you've really got a pure compiling-environment) so much easier! All kudos to GraySky with Arch.

Andromeda-git has been updated (compared to the PKGBUILD currently on the AUR) to use QBS rather than cmake due the corresponding upstream switch.

For wine-d3dstream-git, I included a patch to fix for a game-breaking (literally) bug that only shows up when the package is compiled with gcc>=4.9 . The bug has been fixed upstream in main wine, so newer versions of wine-d3dstream (should there be any before 1.8 is released) will not need the patch.