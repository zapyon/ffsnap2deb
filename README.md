# ffsnap2deb
For [X]Ubuntu, replace the Firefox snap installation by a classic Debian package

Annoyingly, Ubuntu decided to use the snap format for several packages and dropped the Debian packages. One affected program is Firefox, my current web browser of choice. As I was annoyed to have to revert from snap to Debian package manually after upgrading the system, I looked for options.

This is the result, a small script that does the following:

1. uninstall the Firefox snap
2. add the repository for the Firefox debian package for Ubuntu
3. pin Firefox to the deb version (see apt pinning for details)
4. create configuration to ensure Firefox updates are performed usidn the deb, with automatic updates
5. install Firefox from the deb.

Source: https://www.omgubuntu.co.uk/2022/04/how-to-install-firefox-deb-apt-ubuntu-22-04

I have used this script on several machines by now, without any problems.

Feel free to use it, but take heed it is just a quick hack.

