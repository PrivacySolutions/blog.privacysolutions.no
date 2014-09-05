---
layout: post
title: "Weekly news #2"
description: "Second weekly news!"
category: weekly-news
tags: [weekly,news]
---
```written by Mikal Villa (aka Meeh)```



General PS News
----------

It seems like we have gotten a deal with a bulk of PurpleI2P shirts which we can send to people donating above a sum, and bring to <a href="http://www.ccc.de/">CCC</a> this year to share! We're just awaiting final answers from one of a million sites that can do this. But we would prefer current partner because of price, and we know other people that are happy with their service. We will then give away some free shirts at <a href="http://www.ccc.de/">CCC</a>, and send to our best sponsors! (People who donate, and/or codes, and contributes in a way or another)

At this writing moment it seems like at least I (Meeh) and Marielle are going to <a href="http://www.ccc.de/">CCC</a>, and hopefully Torkel, orignal and K1773R as well. The last three haven't confirmed yet, but they all wish to go if possible in their life situation. From I2P, as far as I know zzz, psi and zab at least are joining. We will team up with them at the start of <a href="http://www.ccc.de/">CCC</a>!

On the other hand we have started looking into if PurpleI2P can take over for I2P real soon in the Abscond bundle, which will ultimate remove the need of JRE. And we can introduce new interesting features. I and orignal has had some really interesting discussions lately about what, and how we're going to continue and which projects we will take care of and develop future.

When that said, if you're an experienced C++ / <a href="http://qt-project.org/" target="_blank">Qt</a> developer we would be happy to talk with you. Please send us an mail or join us at IRC for a chat! We always need more good C++ / <a href="http://qt-project.org/" target="_blank">Qt</a> people!



PurpleI2P
----------

In the past time we have worked with getting PurpleI2P to run on Windows, so we can provide test binaries for Windows users. However we haven't decided what compiler to use, and is researching it now. As some of you might know, mingw-w64 doesn't support threading in C++11, so we need to either use a older mingw32 or the VS2013 compiler. Ether way, if you're on Windows the next week will be interesting! Also a lot of time condition bugs have been fixed and people running PurpleI2P for fun and testing have noticed a far much better uptime without any segment fault or other crashes. Another topic not yet decided is if we're going to make PurpleI2P to could use <a href="http://qt-project.org/" target="_blank">Qt</a> instead of boost, making boost optional for regular users. But of course don't remove the boost support to make dependency hell as small as possible for server users. Rewriting a lot of the PurpleI2P code into <a href="http://qt-project.org/" target="_blank">Qt</a> does not mean it will be more graphical, it just enables less dependencies in some cases, and would suit a lot of other projects we have. But as said, this is early discussion and should not be taken as a final decision. It's nearly a little discussion still, and I won't dare to even guess what we end up with here. But you will be updated!



The metrics system
----------

In the past days I've been working with setting up multiple <a href="http://cassandra.apache.org/" target="_blank">Cassandra</a> systems around on different geolocated servers I have for storing the data of the old BigBrother system I made long ago. Since a lot of this data is valuable when put into graphs. We also discuss a fully anonymous way (of course always set to off per default) to report  this data to the BigBrother system. Also, we're going to change the name on BigBrother since it might scare or offend people. Codename on the code will still be BigBrother, but as  a "service name" it will be mentioned as something else. We might just keep a keep it simple stupid approach with just naming it metrics.

The reason we choosed <a href="http://cassandra.apache.org/" target="_blank">Cassandra</a> for this is because of it's unique <a href="http://en.wikipedia.org/wiki/Single_point_of_failure" target="_blank">no-single-point-of-failure</a> way of working where you got none master database server. It's a flat structured system. Almost reminds me more of a <a href="http://en.wikipedia.org/wiki/Distributed_hash_table" target="_blank">DHT</a> sytem than a database. But the other interesting thing here is <a href="http://en.wikipedia.org/wiki/RRDtool" target="_blank">RRD</a> emulation on top of <a href="http://cassandra.apache.org/" target="_blank">Cassandra</a>. So we can use the <a href="http://en.wikipedia.org/wiki/RRDtool" target="_blank">RRD</a> databases to make new graphs in frontend applications like <a href="http://graphite.wikidot.com/" target="_blank">Graphite</a>, which hopefully is ready soon. At writing time I'm at the testimport stage against <a href="http://cassandra.apache.org/" target="_blank">Cassandra</a> from the old <a href="http://www.mysql.com/" target="_blank">MySQL</a> structure. Lately I haven't had time to much because of some big projects we're trying to complete, which ultimate will give me more time when completed!



Anoncoin updates
----------

As already told, KGW, the system calculating the difficutly had some backdraws we didn't notice in the start, but for example now, you can see the blockchain has been joked with earlier, making the difficutly float as a wave, making blocks a little unpredictable. I (Meeh), K1773R and Gnosis startet at once drawing and discussing new design ideas. Not all of them was accepted by the community, so we started a discussion which lead to a lot of interesting people comming with really good ideas on our IRC channels. And how we could patch this part the best as possible. It now seems we found our own simple way, which don't have attack vectors like KGW. (It's not like darkcoin's solution, but not as simple as digishield either). We will post that patch as soon as we decide what date to set on the hardfork.

Some changes are needed, and some others comes when the needed patch is in place anyway. It looks like we're ending up with a multiple <a href="https://en.bitcoin.it/wiki/Merged_mining_specification" target="_blank">AuXPoW</a> chain, where we both support <a href="https://litecoin.info/scrypt" target="_blank">Scrypt</a>, <a href="https://en.bitcoin.it/wiki/CryptoNight" target="_blank">CryptoNight</a>, maybe the primes of <a href="http://primecoin.io/" target="_blank">XPM</a>, and some others. This is still under discussion. Please comment here or visit our bitcointalk.org forum to say youtr opinion if you feel you got useful information. Also, Gnosis has mentioned that we might be able to do a own hash as well, based on the <a href="https://wiki.anoncoin.net/RSA_UFO" target="_blank">RSA UFOs</a> concept. But I doubt that will be introduced.

Gnosis is adding support to libzerocoin for <a href="https://wiki.anoncoin.net/RSA_UFO" target="_blank">RSA UFOs</a>, and will be done in a few days; also to avoid copycat coins, development is being done in a private repo hosted on a git server by Meeh. Commits 2 weeks old will be pushed to github (in the 'zc' branch) which is the current Gnosis works in for ZC related.

K1773R has also solved a problem with Anoncoin and p2pool. He will probably announce this on bitcointalk in near future if not already done!

We also started nightly builds for Anoncoin. I haven't yet had time to test how the win32 build works, but I know that the linux builds would probably not work on other machines than Ubuntu because we're still building the static toolchain for making anoncoin on linux fully static, so we don't need to depend on other libraries. While speaking, it's worth mentioning that I'm also working on a Windows and FreeBSD environment for such type of builds.

You find nightly builds at: 
<a href="https://nightly.privacysolutions.no/" target="_blank">https://nightly.privacysolutions.no/</a>

This link will also serve other software we decides to build at least once a day! 

Also, all this talk about about <a href="http://www.ccc.de/">CCC</a> made me wonder, and I've decided to ask if Gnosis wants to join as well. Hopefully PS(we) can pay for his trip!

Update!
( - Actually copied from a draft from Gnosis, but newsworthy so I'm posting it. /Meeh)
Lastly, I wanted to give an update on the UFO project: it is ongoing and will  finish on September 15, when ANC rewards will be issued and the server source will be published to our Github. The largest factor found so far is 143551628346878317311308640667091515671003679, which is 45 digits (147 bits). For some perspective, the world record for factors found using this method is 78 digits (though for all we know, the NSA/GCHQ/$spook_agency have factored larger ones...). I'd like to thank all the participants for contributing their CPU core-months (core-years, in some cases) to this project -- this effort was essential for creating a trustless Zerocoin implementation using RSA UFOs.

