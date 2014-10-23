Continuity Activation Tool
==========================

This tool makes the necessary changes to enable OS X 10.10 Continuity on compatible hardware. Continuity features activated by this tool include Application Handoff, Instant Hotspot, and Airdrop iOS<->OSX.

## Features
* Activate continuity: Does a Continuity compatibility check, backups the original Systems kexts, disables a Mac-model blacklist in the Buetooth kext, whitelists the Mac board-id in the Wi-Fi kext.
* System diagnostic: Produces a report of the current system parameters influencing Continuity.

## Compatibility list
The tool should work with the following Mac models:

Mac Model | Hardware change required first
---|:---:
MacBook Air 2008-2010 | New wireless card: BCM94360CS2
MacBook Air mid-2011 | no
Mac mini 2009-2010 | New wireless card
Mac mini mid-2011 | no
MacBook Pro mid 2009 to late 2011 | New wireless card: BCM94331PCIEBT4CAX
iMac 2008-2011 | Wi-Fi + Bluetooth card upgrade
MacBook Pro late-2011 | New wireless card: BCM94331PCIEBT4CAX

Macs that are unlisted above have no use of this tool but might still need a hardware upgrade. Table source and more info: [UncleSchnitty's guide on MacRumors](http://forums.macrumors.com/showpost.php?p=20124161).
**The tool is not compatible with BT4 USB Dongles**, it only works with the right internal Apple wireless hardware.

## How to use it

**From Finder**

1. Download the zip (link on the right) and extract it.
2. Double-click on the app.
3. Follow instructions on the screen. Ignore or deny any "Access to accessibility features" prompt.

**From the command line**
The script can also be run right from the command line. It is located in Continuity Activation Tool.app/Contents/MacOS/contitool.sh

Usag example: "./contitool.sh activate"

Script arguments: 
* activate : Starts the activation procedure and does compatibility checks.
* diagnostic : Starts the system compatibility diagnostic.
* forceHack : Starts the activation procedure, and skips compatibility checks.

When using the script from the command line, make sure you have the strings binary in the same directory as the script OR, if you have Apple's Command Line Tools installed, edit contitool.sh and set stringsPath="strings".

### Sources
* [Full guide to enable Continuity manually (MacRumors Forum Thread)](http://forums.macrumors.com/showpost.php?p=20124161)
* [Get help using Continuity with iOS 8 and OS X (Apple Support KB)](http://support.apple.com/kb/TS5458)


### Thanks
* Lem3ssie
* UncleSchnitty
* Skvo
* TealShark
* Manic Harmonic
* rob3r7o

This tool took me many days and nights of research and coding. A small donation would be much appreciated to continue to keep the app maintained and evolving. Thanks!
<form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
<input type="hidden" name="cmd" value="_donations">
<input type="hidden" name="business" value="david@dudokdewit.net">
<input type="hidden" name="lc" value="US">
<input type="hidden" name="item_name" value="Continuity Activation Tool">
<input type="hidden" name="no_note" value="0">
<input type="hidden" name="currency_code" value="USD">
<input type="hidden" name="bn" value="PP-DonationsBF:btn_donate_LG.gif:NonHostedGuest">
<input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!">
<img alt="" border="0" src="https://www.paypalobjects.com/en_US/i/scr/pixel.gif" width="1" height="1">
</form>