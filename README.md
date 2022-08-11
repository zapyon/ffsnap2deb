# ffsnap2deb
For [X]Ubuntu, replace the Firefox snap installation by a classic Debian package

Annoyingly, Ubuntu decided to use the snap format for several packages and dropped the Debian packages. One affected program is Firefox, my current web browser of choice. As I was annoyed to have to revert from snap to Debian package manually after upgrading the system, I looked for options.

This is the result, a small script that simply uninstalls the Firefox snap, adds the repository for the Firefox debian package for Ubuntu (or, in my case, Xubuntu), and installs Firefox from the deb. I have used it on several machines by now, without any problems.

Feel free to use it, but take heed it is just a quick hack.
