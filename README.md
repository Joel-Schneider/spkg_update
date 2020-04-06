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

Download the source as an archive, and download the SlackBuild file to the same folder, change to the folder with the compressed source file, then run (as root):
<pre>$ ./spkg_update.SlackBuild</pre>
You can then install it as above.

Code
---- 
https://www.github.com/Joel-Schneider/spkg_update
