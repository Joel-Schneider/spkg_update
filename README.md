spkg_update
===========
Update list of updates available for Slackware Linux.

Also updates sbopkg queue files. This script will check for slackpkg and sbopkg updates daily.

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
<pre>$ installpkg spkg_update-VERSION-noarch-TAG.tgz</pre>
The current version on github is 1.1, and default tag is SBo

Usage (run once)
----------------
Must be run as root:
<pre>$ spkg_update &</pre>
It will automatically re-run itself every 24 hours, using the 'at' processor, so the exact time may vary. Even if the device is off, it will try to re-run again once restarted.

Compiling from source
---------------------
Just use the package!

Follow the instructions for the SlackBuild package at https://www.github.com/Joel-Schneider/spkg_update.SlackBuild

Code
---- 
https://www.github.com/Joel-Schneider/spkg_update
