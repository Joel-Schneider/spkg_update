spkg_update
===========
Update list of updates available for Slackware. Also updates sbopkg queue files. This script will check for slackpkg and sbopkg updates daily.
(C) 2016-2020 Joel Schneider.

License
-------
ISC

Requires
--------
* at
* sbopkg
* slackpkg

Installation
------------
Download source, change to source directory, then run:
$ ./create_package.sh
$ installpkg spkg_update-1.0-noarch-JS.tgz

Usage (run once)
----------------
Must be run as root:
$ spkg_update &
It will automatically re-run itself every 24 hours, using
the 'at' processor, so the exact time may vary. Even if the 
device is off, it will try to re-run again once restarted.

Compiling from source
---------------------
Just use the package!
If you must, extract source to a temporary folder, then run:
$ makepkg -l y -c n ../spkg_update-VERSION-noarch-TAG.tgz
in the source directory. You can then install as above.
The current version on github is 1.0, and tag is JS

Code
---- 
https://www.github.com/Joel-Schneider/spkg_update
