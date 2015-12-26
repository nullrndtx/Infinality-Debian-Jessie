# Infinality For Debian Jessie

i've been building Infinality for debian jessie! 

# So, what is infinality? 

[Infinality](https://infinality.net) is a set of Freetype patches that try to provide an improved font rendering for Linux and also, to allow easy customization so the users can adjust the settings to their taste. Using it, you can easily set the font style to emulate OSX, OSX2, Windows 98, WIndows XP or Windows 7 or you can use the "Linux" or "Infinality" (default) styles.

# How to install?

Download 3 deb files from this repository , create new folder and move it. Open terminal , and type

> dpkg -i *.deb

# Set your infinality styles

> bash /etc/fonts/infinality/infctl.sh setstyle

And select the style you want to use. Available options are: debug, infinality, linux, osx, osx2, win7, win98 and winxp (I recommend using the "linux" style, obviously, but you can try any style, then remember to log out and log back in - you can easily select a different style later on by using the same command). To use the Windows or OSX style you'll also need to use the Windows or OSX fonts.

# Optional 

Open /etc/profile.d/infinality-settings.sh with a text editor as root.

And in this file, search for USE_STYLE (it should be USE_STYLE="DEFAULT" by default) and change it to one of the following styles (I recommend using "UBUNTU" here but you should also try the default to see which one you like better):

+ DEFAULT - A compromise that should please most people
+ OSX - Simulate OSX rendering
+ IPAD - Simulate iPad rendering
+ UBUNTU - Simulate Ubuntu rendering
+ LINUX - Generic "Linux" style - no snapping or certain other tweaks
+ WINDOWS - Simulate Windows rendering
+ WINDOWS7 - Simulate Windows rendering with normal glyphs
+ WINDOWS7LIGHT- Simulate Windows 7 rendering with lighter glyphs
+ WINDOWS - Simulate Windows rendering
+ VANILLA - Just subpixel hinting
+ CUSTOM - Your own choice
+ Infinality styles
- CLASSIC - Infinality rendering circa 2010. No snapping
- NUDGE - CLASSIC with lightly stem snapping and tweaks
- PUSH - CLASSIC with medium stem snapping and tweaks
- SHOVE - Full stem snapping and tweaks without sharpening
- SHARPENED - Full stem snapping, tweaks, and Windows-style sharpening
- INFINALITY - Settings used by the Infinality developer
- DISABLED - Act as though running without the extra infinality enhancements (just subpixel hinting).

In this file you can change many other settings but if you don't know what they do, only change the style. Then, save the file, log out and log back in to see the changes.

# SCREENSHIT!