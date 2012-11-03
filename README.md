Allow.app : unlock quarantined mac apps
=======================================

Execute, select the app / document you want to be unlocked.

Unfortunately Drag & drop is prevented if the app is locked.

Problem
-------

Mountain Lion's security model is great, it protects you from
unadvertently executing rogue applications. You know it's coming, there
is a but: developers need to pay Apple $99 to get a certificate, which
is fine unless you develop free apps.

![Example](quarantined.png)

Allow.app gives you a way to selectively unlock quarantined apps, the
ones coming from people you trust.

Installation
------------

Chicken and egg issue right ? Download the archive, unpack and
right-click on the Allow app. Drag to your application folder.

About
-----

Made with Automator.

The heart of the script boils down to
`find $INPUT -exec xattr -d com.apple.quarantine {} \;`

Copyright
---------

MIT 2012 Jonas Pfenniger

Lock icon comes from
http://www.iconspedia.com/icon/silver-lock-18598.html
Copytight NewIdols, CC Attribution Non-Commercial
