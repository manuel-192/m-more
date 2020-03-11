# mirrorlist-m

Installs file /etc/pacman.d/mirrorlist-m that contains
repository definitions for packages in
https://github.com/manuel-192/m-more and https://github.com/manuel-192/m-m.

You may add a references to this file in the end of your /etc/pacman.conf, e.g.:
<pre>
[m-m]
Include = /etc/pacman.d/mirrorlist-m
SigLevel = Required

[m-more]
Include = /etc/pacman.d/mirrorlist-m
SigLevel = Required
</pre>
Note: there's a small script *install-mirrorlist* that adds Manuel's repositories to your system. You may use it with these commands:
<pre>
wget -q https://github.com/manuel-192/m-more/raw/master/PKGBUILDs/mirrorlist-m/install-mirrorlist
bash install-mirrorlist
</pre>
