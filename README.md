# ffsnap2deb — Revert to using the Firefox .deb Package in Ubuntu 22.04+
## (instead of using that "§$%&/() Snap version)

Starting with it's 22.04 LTS version, Ubuntu dumped the traditional Debian packages for Firefox, replacing it with the home-grown Snap system. Many users do not like that decision. Luckily, there is a PPA available: https://launchpad.net/~mozillateam/+archive/ubuntu/ppa

So it is possible to ditch the Firefox Snap, and return to the Debian packages. At least for now.

When I decided to make the effort of doing so (right after realizing what Ubuntu had done, during upgrade of an Xubuntu machine to 22.04 LTS) I found a nice description on how to achieve this. But as I knew I would be upgrading a couple more machines soon, and being lazy, I decided to put the sample commands from that description into a script. And lo and behold, it worked like a charm the first time, and has done so ever since.

So may be you can use it, to. Let me know if anything fails or could be improved.
Of course, no guarantees. YMMV ;-)


## What it does

This small script does the following:

1. __uninstall__ the Firefox __Snap__
2. __add the Mozilla Team's PPA__ (package repository) for the Firefox Debian package for Ubuntu
3. __pin Firefox__ to the deb version (see apt pinning for details)
4. __create configuration__ to ensure Firefox __updates use the deb__, not the snap, even with automatic updates
5. __install Firefox from the deb__
6. __Enjoy.__

The script __requires__ you have __sudo__ rights and will ask for your credentials accordingly.

I have used this script on several machines by now, so far without any problems.

Feel free to use this script, but take heed it is just a quick hack. So, __no promises, no guarantees.__


## Resources

I found the snippets and info in __How to Install Firefox as a .Deb on Ubuntu 22.04 (Not a Snap)__ by __Joey Sneddon__ (Updated 28 April 2022) — 
URL: https://www.omgubuntu.co.uk/2022/04/how-to-install-firefox-deb-apt-ubuntu-22-04

