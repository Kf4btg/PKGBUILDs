Note on installation order for idevice-software:

Install order: 
	libplist -> libusbmuxd -> libimobiledevice -> usbmuxd, ifuse, ideviceinstaller, ...
	
About owlman PKGBUILD:
	I simply removed the "abs" dependency so it will install on Manjaro; no actual code was changed. The ABS-related functions remain in the program and using them will fail.  On my system, I created a dummy "abs" file and placed it in my path to mitigate any errors, but I'm not sure if that's really necessary or not.
	
Clean-chroot-manager-manjaro has been patched to work with the "mkmanjaroroot" command in the Manjaro devtools. I've also included a version of arch-nspawn (renamed to "manjaro-nspawn", natch) that has received the same treatment. This little tool makes compiling for other architectures (or just making sure you've really got a pure compiling-environment) so much easier! All kudos to GraySky with Arch.

Andromeda-git has been (compared to the PKGBUILD currently on the AUR) updated to use QBS rather than cmake due the corresponding upstream switch.

Wine-d3d-git has been patched with a fix for a game-breaking (literally, and pun intended) bug that only showed up when the package was compiled with gcc>=4.9 . The fix has been committed upstream in main wine, so it shouldn't be long before the d3dstream fork gets it, too.