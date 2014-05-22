Note on installation order for idevice-software:

Install order: 
	libplist -> libusbmuxd -> libimobiledevice -> usbmuxd, ifuse, ideviceinstaller, ...
	
About owlman PKGBUILD:
	I simply removed the "abs" dependency so it will install on Manjaro; no actual code was changed. The ABS-related functions remain in the program and using them will fail.  On my system, I created a dummy "abs" file and placed it in my path to mitigate any errors, but I'm not sure if that's really necessary or not.
	
Clean-chroot-manager-manjaro has been patched to work with the "mkmanjaroroot" command in the Manjaro devtools. I've also included a version of arch-nspawn (renamed to "manjaro-nspawn", natch) that has received the same treatment. This little tool makes compiling for other architectures (or just making sure you've really got a pure compiling-environment) so much easier! All kudos to GraySky with Arch.