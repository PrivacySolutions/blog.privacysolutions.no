---
layout: post
title: "The birth of the privacy solutions project"
description: "the foundation"
tags: [information,general]
---
```written by Mikal Villa (aka Meeh)```

Hello all,

Today we announce the Privacy Solutions project, a new organization that develops and maintains I2P software. Privacy Solutions includes several new development efforts designed to enhance the privacy, security, and anonymity for users, based on I2P protocols and technology.

These efforts include:

- The Abscond browser bundle.
- The i2pd C++ router project.
- The "BigBrother" I2P network monitoring project.
- The Anoncoin crypto-coin project.
- The Monero crypto-coin project.

Privacy Solutions' initial funding was provided by the supporters of the Anoncoin and Monero projects. Privacy Solutions is a Norway-based non-profit type of organization registered within the Norwegian government registers. ( Kind of like US 501(c)3. )

Privacy Solutions plans to apply for funding from the Norwegian goverment for network research, because of BigBrother (We'll get back to what that is) and the coins that are planned to use low-latency networks as primary transport layer. Our research will support advances in software technology for anonymity, security, and privacy.

There is probably no easy way to explain what this is if you're not familiar with I2P or other mix-networks like The Tor project. If you got no clue what this is, we suggest you take a trip on wikipedia before continue reading. <a href="http://en.wikipedia.org/wiki/Mix_network" target="_blank">http://en.wikipedia.org/wiki/Mix_network</a>.

We're going to try illustrate a mix-network with the image bellow.
<img src="/public/gallery/intro/how_it_works.png" width="500" height="320" />

First a little bit about the Abscond Browser Bundle. This was first a one-man project by Meeh but later on friends started sending patches, the project is now trying to create the same easy access to I2P as Tor has with their browser bundle. Our first release isn't far away, it's just some gitian script tasks left, including setup of the Apple toolchain. But again we will add monitoring with PROCESS_INFORMATION (A C struct keeping vital proces information about an process) from the Java instance to check on I2P before I declare it stable. I2pd will also switch with the Java version once it's ready, and there is no point in shipping a JRE in the bundle anymore. You can read more about the Abscond Browser Bundle at

<a href="https://hideme.today/dev" target="_blank">https://hideme.today/dev</a>.

For windows users, we have already released some pre-releases and a alpha version of the bundle. Much because windows is still the most common used operating system unfortunaly, and the one with most common runtime errors. In other words need most testing.

We would also like to inform of the current status of i2pd. I2pd supports bi-directional streaming now, that allows to use not only HTTP but long-lived communication channels. Instant IRC support has been added. I2pd users are able to use it same way as Java I2P for access to I2P IRC network. I2PTunnel is one of key features of I2P network, allowing non-I2P applications communicate transparently. That's why it's vital feature for i2pd and one of key milestones.

As you might have understood, the I2P network wasn't made to be exited like Tor is, but still it's one shared exit node in the default installation, Privacy Solutions will now take over this, since Meeh already hosts it. The exit node of ours has a multi-homing setup for better performance, as well as it should resolve .onion links as well. In other words it can act as a gateway to Tor. The service is used by many people on I2P. In case we get donations (since it's a free service) for the outproxy setup, we can setup more for better performance and speed.

At last, if you are familiar with I2P you probably know about Bigbrother.i2p, which is a metrics system Meeh made over a year back. Recently we noticed that Meeh actually have 100Gb of non-duplicated data from nodes reporting in since initial launch. This will also be moved to Privacy Solutions and be rewritten with a NSPOF backend. With this we will aslo start using the Graphite ( http://graphite.wikidot.com/screen-shots ). This will give us a great overview over the network without privacy issues for our end users. The clients filter all data except country, router hash and success rate on tunnel buildings. The name of this service is as always a little joke from Meeh.

Here are some random selected screendumps of the old bigbrother.i2p running at the old home computer of Meeh's;

<img src="/public/gallery/old-bb/old-bb01.png" alt="old bb" /><br>
<img src="/public/gallery/old-bb/old-bb02.png" alt="old bb" /><br>
<img src="/public/gallery/old-bb/old-bb03.png" alt="old bb" /><br>
<img src="/public/gallery/old-bb/old-bb04.png" alt="old bb" /><br>




For further information contact: press@privacysolutions.no.


As you might see we also got a discussion/comment system here, we had a talk about that. Honestly it would be quite naive of us to use a service like disqus or something since we stand for privacy. The system is an external one, but still hosted by the project itself. Since we doen't prefer to give away marketing data (your traffic).




Best regards,<br>
Mikal Meeh Villa


