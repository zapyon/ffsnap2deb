# ffsnap2deb
For [X]Ubuntu, replace the Firefox snap installation with the classic Debian package

Annoyingly, Ubuntu decided to use the snap format for several packages and dropped the Debian packages. One affected program is Firefox, my current web browser of choice. As I was annoyed to have to revert from snap to Debian package manually after upgrading the system, I looked for options.


## What it does

This is the result, a small script that does the following:

1. uninstall the Firefox snap
2. add the repository for the Firefox debian package for Ubuntu
3. pin Firefox to the deb version (see apt pinning for details)
4. create configuration to ensure Firefox updates are performed usidn the deb, with automatic updates
5. install Firefox from the deb

The script requires you have sudo rights and will ask for your credentials accordingly.

I have used this script on several machines by now, and without any problems.

Feel free to use this script, but take heed it is just a quick hack. So, no promises, no guarantees.


## Resources

I found the snippets and info in __How to Install Firefox as a .Deb on Ubuntu 22.04 (Not a Snap)__ by __Joey Sneddon__ (Updated 28 April 2022) — 
URL: https://www.omgubuntu.co.uk/2022/04/how-to-install-firefox-deb-apt-ubuntu-22-04

