# Description

A couple of months ago a firmware update for my Fritz!box 7340 prevented the bridge-mode hack I had been using for a couple of years.
The changes via telnet were no longer persistent so I had to find a new way of putting the modem in bridge-mode.

Through some searching on several forums I found the fake "firmware" update provided in this repository which I've modified a little.

# Usage

- Put the "var" directory containing the "install" file in a tar file
- Go to the web-interface of your Fritz!box and initiate a firmware update 
- Supply the .tar file you've just created
- The modem will complain it's not a valid firmware-update
- Ignore this message and continue
- Your modem is now in bridge-mode and you can set-up a PPPoE session on VLAN6 (this is the case for xs4all)
- Do not reboot

# Notes

Sadly this "firmware" update is not persistent, so you have to do this everytime you reboot your Fritz!box.

# Disclaimer

Use this "firmware" at your own risk!
