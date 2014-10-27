---
layout: post
title: "PurpleI2P/i2pd's first release, v0.1.0 is here!"
description: "The i2pd daemon has finally reached v0.1"
category: releases
tags: [release,info]
---
```written by Mikal Villa (aka Meeh)```

17th October was the first tag for i2pd/purplei2p tagged. Meaning our first release is v0.1.0, and is available on github to be compiled. This is the first C++ implementation of I2P which has gotten so far as i2pd is today. On our first release we can offer;<br>

* Simple router functionality.<br>
* SAMv3 (Simple Anonymous Messaging) bridge with streaming.<br>
* HTTP proxy which can be used to browse I2P webpages.<br>
* I2P Tunnel interface to host a service like an eepsite or a IRC server.<br>

It also has server functionality for one service, meaning you can use your old tunnel keyfile from the java version to run your service from i2pd instead. But we're currently limited to one service per instance of i2pd in writing moment.


We would also like to thank ArchAssault for becomming the first Linux distro with i2pd in it's official repository. If you're an Arch Linux fan, or you liked BackTrack(Kali Linux) we would recommend that you check them out!<br>Visit them at <a href="https://archassault.org/" target="_blank">https://archassault.org/</a>.

We're also mirroring ArchAssault, so if you're near Norway it might be worth checking out. We also provide this over I2P/Tor, but more on that for a later post.
For those of you running a Linux distro based on Debian, like for example Ubuntu or Linux Mint, or even FreeBSD (with dpkg support) you can already download deb builds at <a href="http://deb.i2p2.no/" target="_blank">http://deb.i2p2.no/</a> and even add the repository to your system for updates as well. Thanks to KillYourTV for his builds and work on the repository. The repository itself is hosted by Sigterm, our sponsor ISP.


We plan to release and provide downloads for Windows Vista, 7, 8, and maybe even Windows XP. As well as a bundle for Mac OS X 10.6 and newer releases. Linux/FreeBSD will have static builds for download as well. All platforms mentioned will have support for x64 and x86 architecture when possible.<br>
All which will be built by us will also have nightly builds or builds per commit available for download, provided by jenkins. We will also start to sign builds for Windows and Mac OS X from the next release on, since Sigterm has applied and got a Apple developer license, and a Windows developer license in validation processing by the certificate provider at writing moment.
