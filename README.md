There has been a high demand for a feature complete and fully capable Linux Desktop for the RockPro64 RK3399, so myself and Lukasz teamed up to build one based on my minimal Debian build.

DOWNLOAD:
The download is available on the GitHub release: 
https://github.com/mrfixit2001/debian_desktop/releases

VIDEO PREVIEW:
Lukasz recorded a quick demo / intro to the capabilities for this release which can be viewed here: https://vimeo.com/323328316
The video was taken prior to me correcting some of the MPV code so it doesn't showcase 4K, but that is now supported in the final release (30fps only).

INTRODUCTION:
This is a custom Debian Mate desktop build based on my minimal image. The great majority of hardware features of the RockPro64, such as WiFi/BT SDIO module and PCIe, work on this image!
Please reference the aforementioned minimal build thread to learn of the details for a minimal Debian install.

This build is meant to bring full fledged desktop functionality to the RockPro64 (and, in the future, to the Pinebook Pro) with an appreciation for end-user ease of use. We hope that the image manages to balance out-of-the-box usability, an aesthetic look and performance with sparsity of preinstalled applications, so that each user can tweak the experience to their individual liking and use-case. 

INCLUDED:
* Mate desktop at 1080p (with 4K as optional*) with Arc theme + icons, custom layout and background 
* Glamor accelerated Xorg with window compositing; running smooth as butter on default settings
* Accelerated Chromium browser, with WebGL and WebGL 2.0 as well as accelerated video playback in browser - including 1080p Youtube and similar services 
* SMPlayer: Accelerated playback of 1080p and 720p local media
* MPV Player: 4K @ 30fps playback of local media (right click 4k video -> select MPV Player)
* OpenGL 3D acceleration via GL4ES; so if you want to play games then you’re in luck!
* Set of common desktop utilities as well as some quality of life additions, including:  LibreOffice, caja-share (SMB GUI), Synaptic Package Manager, Puseaudio (for GUI audio output source selection), Mate Tweak (for desktop tweaks), GPARTED, handy applet to set CPU governor (non-scaling by default), etc.
* Endless number of tweaks for smooth desktop performance

LOGIN: 
User credentials: rock/rock
Root credentials root/root 

FIRST BOOT:
The first boot will take longer to boot and then immediately reboot once time, this is to auto-size your system to the full capacity of your SD card or eMMC

REPORTING ISSUES:
This is an initial release of the OS image and, as with any such release, some things may not work as intended or break. To help us fix the issues you’re experiencing, please provide any relevant information when reporting problems; we presently don’t have a crystal ball on hand, so we are heavily reliant on logs to deduce the nature of the issue you’re experiencing. The preinstalled Hexchat takes you directly to #Rock64 in the IRC (please immediately change your nick using /nick after you enter the channel). 

KNOWN ISSUES:
* Chromium cannot be updated (it has been removed from apt update list on purpose) as it is custom and updating will break it's functionality
* Installing Iceweasel (Firefox) via apt will not work - you need a custom deb (armhf) or compile from source
* Thunderbird doesn’t work, you probably need a deb (armhf) for it too, or a custom compilation.
* Some OpenGL 3D applications will either not work correctly with GL4ES OR will only work in full screen at native resolution of your monitor (e.g. Tux Racer Extreme) when downloaded via apt. For most of these, the fix is to compile from source with necessary flags, rather than installing via apt to get them working. 
* LCD eDP and DSI / TP panels do not work … yet

UNTESTED:
USB-C video output
Cameras from PINE64 store

APPRECIATION
Please remember this is a community build, and just something we have worked on in our free time. There's no pressure at all, but if you appreciate the work then feel free to send me a buck on Paypal: mrfixit2001 at gmail. 

While I have done a great deal of debugging and development from a programming standpoint, the credit for the way the desktop interface is setup goes completely to Lukasz. He spent a LOT of time configuring it and setting it up to look so great!

Lastly, thanks to all of YOU for being part of the community!
- Mr Fix IT

