---
layout: post
title: "Weekly news #1"
description: "First weekly news!"
category: weekly-news
tags: [weekly,news]
---
```written by Mikal Villa (aka Meeh)```


PurpleI2P
----------

The PurpleI2P router, formerly only named i2pd was started on July, 19, 2013. Now, over a year after we can finally enjoy some alpha testing with the router. It's still highly unstable, and should not be used in production of any kind. Just for testing and fun!

i2pd support ECDSA signature for destinations now, that's will be default for the upcoming release of I2P, 0.9.15. i2pd was tested at both sides and is completely ready for upcoming I2P network change, in other words i2pd can communicate with eepsites, IRC and other services using ECDSA effictive now.

I also took the time to hack together a service, running behind i2pd. irc.meeh.i2p is a IRC server on I2P you can access, and it's all done by i2pd, Java isn't even installed!


I2P and Bote
-------------

I would first use some time to explain the situation here with regards to I2P and Bote launched under us at Google Play. The reason behind it is that we fund the account, and also deliver server hosting for some of I2P's official clearnet services. All donations for the donation edition of the Android I2P router will be sent back to Echelon in the I2P project.

I2P and Bote was launched on Google Play in Norway for about three days ago. This because we want to see how I2P scales with a lot of mobile devices connected. But still don't try it on a world basis. However it got perfect timed with PST's earlier statements this week which was just the same old brainwashing story about the scary terrorists.

With this beta testing we hope to awake some interest in privacy here in Norway, which we honestly lack. Also the awareness of the I2P network. On next run we will launch it globaly as far as I've understood it from str4d, lead developer for the Android version.

The I2P router APK package is available for download for all people living outside of Norway on <a href="https://geti2p.net" target="_blank">https://geti2p.net</a> under the downloads section as always!


And some Anoncoin at last
--------------------------

My earlier place to update you was on <a href="https://sigterm.no" target="_blank">https://sigterm.no</a>. We think however this will be a better place from now on, since we're getting organized. Sigterm will continue as it does, with my random posts about security, privacy, outrages after stupid statements from the state and so on! This blog will be clean and contain organization content, and not my own private opinions about world events.

As earlier told, Gnosis is back, however yet to give a sight of himself in the light. (We have spoken a lot on I2P lately, but he hasn't been active on clearnet as far as I know.) But there is also an update for the RSA UFO project. We approved to continue the project until implementation in MainNet for further strengthening and will use what we currently have for the TestNet process. He also got some statitstics about who has contributed, so the one who has will ofcourse recieve some earnings for the help! I'm awaiting the list before I'll start payments. Those payments will happen soonish.  Once we implement ZeroCoin into MainNet, we probably send another round of payments for those who continued to run ufo_client.

K1773R is currently investigating on some transaction issues that have happended as a result of exchanges sending the wallet dust, resulting in transactions over 100Kb. Seems he found a solution there, which also is great news.

As for myself, I've shocked myself by using a lot of time with math, and earlier mentioned as boring whitepapers. But more code should emerge the next days by me as well. However, I've started on the ZeroCoin implementation and collobrate with Gnosis with regards to design options. It's possible to implement it in different ways, and we would like to find the best way. As of now it seems we're going for a "temporary-2nd-blockchain" where the oldest proofs will be deleted based on a "still in discussion" method. I'm also currently wrapping my head around the Finite-state machine scripting that Anoncoin uses to send transactions at the moment.

I would also mention Skaia who has done a great job working on the anoncoinj, to port Anoncoin to Android devices!

We're preparing a release now before the first ZeroCoin enabled release, but it's most for preparing the network for the upcoming hardfork. And since we're hardforking anyway, we're going to introduce some more changes. KGW is trashed by the way. The other news can wait until we're researched more on it. But what it is can wait a bit longer :)

