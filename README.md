Note on installation order for idevice-software:

Install order: 
	libplist -> libusbmuxd -> libimobiledevice -> usbmuxd, ifuse, ideviceinstaller, ...
	
About owlman PKGBUILD:
	I simply removed the "abs" dependency so it will install on Manjaro; no actual code was changed. The ABS-related functions remain in the program and using them will fail.