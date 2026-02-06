[0.00 → 7.46] Coming up on Self-Hosted 13, Alan Pope from Canonical joins us, and Alex crashes a drone
[7.46 → 9.44] into a tree. I'm Chris.
[9.88 → 13.40] And I'm Alex, and this is Self-Hosted episode 13.
[14.58 → 20.40] Welcome back to Self-Hosted, everyone. We start today with a special guest, Mr. Alan
[20.40 → 21.20] Pope. Hey, Pope.
[21.44 → 22.86] Hey, how are you doing, guys?
[23.36 → 28.84] Great. I appreciate you coming on, and honestly, I think our topic today?
[28.84 → 34.92] I think you're going to make me put my words in my emotes when you have to eat what you
[34.92 → 39.44] said, because today, Pope's going to join us and convince us why IRC is not dead. When
[39.44 → 44.72] I went on air and said IRC is totally dead, but I was actually just being a little click
[44.72 → 46.42] bait, so I appreciate you being here.
[46.96 → 48.64] You triggered me, Chris. You triggered me.
[49.98 → 53.50] Alex, before we started the show, you and I were talking drones, and I discovered this
[53.50 → 55.56] week that you managed to crash a drone into a tree.
[55.56 → 62.20] And a car park, and a building, and so to be clear, it's not one of the DJI balloon
[62.20 → 67.36] simulator drones. It's a racing drone made of carbon fibre that does 70 miles an hour.
[68.36 → 73.68] And yeah, this thing ended up in a tree. And there's a video in the show notes one of my
[73.68 → 79.78] buddies made where we have to fly another drone with a rope tied to it over the tree
[79.78 → 84.84] I'd crashed into to actually shake the damn thing out of it. So yeah, that was a lot of
[84.84 → 85.64] fun. That was my Sunday.
[86.26 → 88.26] So you threw another drone at that drone?
[88.66 → 94.20] We tied a piece of string or a rope to the bottom of another drone that I have, flew it
[94.20 → 99.22] over the tree that it was stuck in, did a sort of loop-DE-loop to try and tie it in some
[99.22 → 105.90] kind of like a maypole style situation around the tree, and then used the quad that had just
[105.90 → 111.22] flown over with the rope as like an anchor, like a barb fishing hook or whatever, shipped the tree.
[112.86 → 117.22] And it all came down, and I didn't lose any drones. The only thing that happened was I snapped
[117.22 → 122.10] an arm off the drone, which sounds like a big deal, except for the fact the frames that I use
[122.10 → 127.02] have a lifetime warranty. So I just email them a picture, and they send me a new one for five bucks
[127.02 → 128.86] every time I have to cover shipping.
[129.28 → 133.96] Do you send them a picture of the drone in the tree, or just the drone that's broken?
[133.96 → 140.26] You have to send them a picture of the carnage. I posted it on Twitter about how I cracked the
[140.26 → 144.74] arm of this thing, but you can maybe see how I can bend this thing.
[145.46 → 147.20] That doesn't look like it should do that.
[148.10 → 153.54] No, that's pretty bad. We will put a video to this in the show notes. Were you trying to
[153.54 → 155.56] use toilet paper at first to recover this thing?
[155.64 → 161.98] It looks like toilet paper, but it's actually a piece of AT&T, I don't know, rope that they use.
[161.98 → 163.20] Yeah. Okay.
[163.42 → 167.80] Like fishing string through cable, like it can hold like 2,000 pounds or something crazy.
[168.12 → 171.68] So you were being a fancy flyby, and you were flying too close to the trees. What happened?
[172.32 → 174.98] Yeah, or I just ran out of talent and...
[174.98 → 180.80] Well, I have no excuse because I flew my drone into the side of a barn the other day.
[182.06 → 185.96] Can I say the tree leapt out at me? I think barns are inanimate, aren't they?
[185.96 → 191.68] Yeah. Yeah, totally. Totally. Well, now, before we prove why I was wrong about IRC,
[191.98 → 196.70] you have been writing recently, and I have been sneaking into your computer at night,
[196.88 → 198.62] checking your documents and following along.
[198.94 → 203.88] I don't know if I should be creeped out about this, or... I think I'm creeped out.
[204.26 → 206.34] Well, you did give me pseudo-access after all.
[206.62 → 208.48] Oh, yeah. Yeah, maybe I should revoke that.
[208.48 → 214.50] But Docker Compose Workflows has been on your mind. And so it's funny that this came up in the show,
[214.58 → 218.38] because this week, I've been told by a couple of individuals that Docker is dead,
[218.92 → 222.94] and I asked them if they've met my friend Docker Compose, because I think it sort of breathed
[222.94 → 227.00] new life into people using Docker online. Every project you see now,
[227.44 → 230.10] somebody drops some Docker Compose example along with it.
[230.34 → 233.36] Why do they think Docker is dead, though? That's what I want to know.
[233.44 → 237.42] I am the worst person to ask about Docker, because I never use it for anything.
[237.42 → 239.74] Well, that's the way. Hold on. That's a good perspective.
[240.28 → 245.76] I think there's one service that I installed, two services that I installed via Docker,
[245.98 → 249.80] and that's only because that's the upstream-supported way of doing it, and I couldn't
[249.80 → 257.98] find a better way, and that's Mastodon and Discourse. And they were both upstream-supported
[257.98 → 262.92] ways, so that's what I used. I don't feel part of a Docker ecosystem, or I don't feel like a
[262.92 → 267.28] power user or anything. I just pasted a command in a terminal, and the service started.
[267.42 → 268.46] And I was like, okay, I'm done.
[269.06 → 272.72] But that's how it goes the first few times, right? With anything, not just Docker.
[273.26 → 279.90] And that's really what it's supposed to be like. If you're consuming some software and
[279.90 → 284.10] you want to start a service, you just want to run a command. You want to run whatever
[284.10 → 288.28] the right command is to get the thing working, and then walk away and leave it, and then come
[288.28 → 291.90] back to it three months later and think, how did I set this thing up? I've got to do some
[291.90 → 297.38] software updates on this, and I don't know. I had to relearn how to do it all, and that
[297.38 → 300.34] was a learning curve. But once you get over that, it's fine.
[300.94 → 305.54] Yeah, that's a very fair assessment of it. That's really true. I just recently went back
[305.54 → 309.28] to a system I set up a couple of months ago and went, oh, oh, right, okay, yes, okay.
[309.32 → 314.54] I have this URL, I go to admin it. I have this URL where I go to use it. Okay, yeah, right.
[314.54 → 318.94] I can remember all of this. And maybe that's part of what appeals to me about some of these
[318.94 → 324.54] newer install techniques. Like using Docker Compose, I can go read a compose file, and
[324.54 → 328.30] it's all in YAML, and I can have a pretty good understanding of what it's doing. But Alex,
[328.34 → 333.92] to answer your question, I think it's a combination of answers. Fundamentally, Docker isn't doing
[333.92 → 337.94] anything that other technologies can't do, because it's relying on underpinning technologies
[337.94 → 342.78] that are built into the operating system. So a lot of different vendors have different takes
[342.78 → 347.38] on how to solve this problem. And a lot of times they are better integrated into their
[347.38 → 353.36] overall product than Docker itself is. And when you combine the technical aspects of what
[353.36 → 357.50] a container actually is, and how any Linux host operating system or many other OSes now
[357.50 → 362.10] can run them, and the fact that many distributions have a preferred container technology that tends
[362.10 → 369.32] to work better on their distribution and ecosystem, I think it's understandable that people kind of see
[369.32 → 375.58] Docker as sort of being pointless, not necessary. And then you have the VM crowd as well, who is maybe
[375.58 → 379.70] not even totally bought off on the idea of running applications in containers when they could just
[379.70 → 380.78] run it in a VM system.
[381.48 → 386.90] I was about to argue with you that various different people didn't have their own versions of container
[386.90 → 392.32] runtimes, and then I realized that Red Hat have their own, Docker have their own, VMware have bought
[392.32 → 397.94] Pivotal, so they're going to have their own. So yeah, you're totally right. I can see why people might
[397.94 → 403.00] come to that conclusion. And if I was on the Red Hat platform, I might use Rodman. And I could be
[403.00 → 408.90] wrong, but if I'm on Ubuntu, I'd probably use LXD. Yep, I use LXD for everything. Right. And there's
[408.90 → 415.24] even nice scripts or applications built around those tools to make setting up environments super quick
[415.24 → 421.38] and fast, and kind of no-brainer when you're on those platforms. So my thrust for bringing this up
[421.38 → 428.80] really was that one of the first questions I see and hear from people getting into containers for
[428.80 → 435.08] the first time is, is there a UI? Is there a GUI? Is there a web app that I can run that exposes this
[435.08 → 443.44] stuff to me? And my general answer is you don't need one. What do you think? Do noobs need a UI?
[444.12 → 446.40] What are noobs doing running containers?
[446.40 → 451.74] They're running Unpaid boxes or Free NAS boxes or... Which have web UIs, don't they?
[452.04 → 458.20] Or Raspberry Pis. Running what though? You don't... Nobody goes out to install a Raspberry Pi.
[458.50 → 464.24] You go out because there's an appliance that you want to put on a Raspberry Pi, or there's some
[464.24 → 470.88] device you want to build around a Raspberry Pi. Or you just think, hmm, that's $25, I'm going to buy one.
[471.66 → 473.66] And then what should I do with it when it arrives?
[473.86 → 476.32] And put it in a drawer with all the others.
[476.40 → 485.86] Yeah. I have got a couple of Raspberry Pis here in service. One is my DNS, so it does Pi hole and
[485.86 → 490.50] blocks adverts and stuff. That has a web UI. I almost never use it because I just don't care.
[490.56 → 495.14] It just works. Like if I have to whitelist something, then yeah, I could use, you know,
[495.16 → 501.96] I consider myself expert, so I could use the command line, but the web UI is nicer. And
[501.96 → 509.42] for other things that I run on a Pi, they have web UIs as well. So I don't know. I think it's just a
[509.42 → 514.22] nicer experience. I could see the argument for being hardcore and doing it on the command line
[514.22 → 521.54] because it's, you know, you have total control and power. But I also quite like a pretty graph now
[521.54 → 521.86] and then.
[521.86 → 528.38] I don't necessarily disagree in a couple of ways. And I recently got a note from a listener who said,
[528.44 → 534.84] Chris, you're always advocating people just use the command line. And I have kind of in the last
[534.84 → 540.56] year and a half sort of transitioned to just learn the command line because it's sort of a universal
[540.56 → 547.98] tool that will always work. But working with team members that learn in different ways than I learn
[547.98 → 554.02] here on our podcast team, I realized that for some of them, they want to see what the end result is
[554.02 → 559.26] that they could achieve if they invest the time to learn the whole stack. So if they can do something
[559.26 → 565.08] that gets them deploying software and turning on things and actually using the end product
[565.08 → 572.72] that gets them excited and motivated, it's worth it. So they'll use a GUI to sort of skip learning how to
[572.72 → 577.06] get on the command line, learning how to run Docker and end up running the application. And they'll go
[577.06 → 581.46] right to using the application. They go from zero to using the application. They go, okay, this is
[581.46 → 587.20] great. This is worth it. And then they kind of walk it back. So in that way, I kind of think, yes,
[587.22 → 592.12] it is important to have a GUI tool because different people learn differently, and some people are extremely
[592.12 → 597.40] visual learners. But I want to just sort of caveat all of that with, I just want to remind us that
[597.40 → 604.54] sometimes some groups do actually put some form of design into their tools. I remember,
[604.54 → 611.74] I think I might've been having a conversation with you, Pope, about having folks at Canonical look
[611.74 → 616.90] at the syntax of the snap commands or the Docker folks, they look at the syntax of the Docker
[616.90 → 620.80] commands to actually see if it logically makes sense. There is some design that goes into command
[620.80 → 626.20] line tools to make them more usable. So some tools are more usable than others on the command line.
[626.70 → 630.14] I think for me, it's not necessarily about being a hardcore elite super hacker.
[630.14 → 636.68] It's about having some way to repeatedly rebuild my system when it goes tits up.
[637.28 → 643.76] I love committing text files to Get and just being able to copy and paste whatever that Docker
[643.76 → 649.10] run command. I mean, this is how I started. I used to run one Docker run command after another and just
[649.10 → 655.34] keep that in a GitHub repo in a text file. I used fig when that was new and Docker compose was new.
[655.34 → 660.40] And as, as it's gone on, Docker compose has matured. And now I manage something like 30,
[660.52 → 669.08] 35 containers on a single host with one interface to it. And for me, I have a single text file. Now
[669.08 → 675.48] it's a YAML file, admittedly, not a text file. I have a single file, which defines what every single
[675.48 → 681.48] container on my system looks like. And if I want to add a new container, I have to add maybe eight lines
[681.48 → 686.36] of code because I figured out what the syntax of that YAML is. Now that's investment I've made to
[686.36 → 691.72] learn that. And I will fully admit that for a completely new user, that's not realistic.
[692.54 → 698.90] However, I think simply asking, is there a UI like Container or something like that, you know,
[698.92 → 704.52] using that as your crutch rather than actually investing in learning how the underlying stuff
[704.52 → 712.32] works over time will bite you in the bum because it's just that question of when you want to redeploy
[712.32 → 717.62] something, how do you do it? I mean, taking a few steps to address that, I've started writing a wiki
[717.62 → 723.50] at home, as we discussed last episode, keeping notes as Chris is doing now, you know, all these
[723.50 → 729.58] things, but nothing beats the source of truth, which is the file that you use to deploy the application
[729.58 → 736.96] itself. And for me, compose.yaml is the one. I think you're two steps ahead of me. I've just
[736.96 → 742.78] started a wiki at home to keep track of some of these things because I've now been bitten in the
[742.78 → 748.30] butt where I, like I said, didn't remember how I set up the Mastodon instance. And now I have to
[748.30 → 753.46] revisit the thing because I've got to clean it up or upgrade it or something. And I think we're in a
[753.46 → 760.22] similar state along that course. But I think what a lot of people are doing is they want to get to
[760.22 → 763.86] the goal. As Chris says, they just want to have that appliance working. They want to have that
[763.86 → 771.44] thing installed, and they want the fast track to get it in. And what they don't have is the blessing
[771.44 → 778.64] of experience that you've had of things going tits up over and again, and you're learning from that
[778.64 → 784.20] experience and deciding to write stuff down so that the next time it does, or hopefully it doesn't,
[784.54 → 791.50] you've got a document that you can refer to get your system back in order. And, you know, my pie
[791.50 → 800.52] hole has never broken, but it is a Raspberry Pi sat in a warm room, and it's using an SD card for its
[800.52 → 807.68] storage. So inevitably it's going to fail at some point, right? And I couldn't tell you off the top of
[807.68 → 812.64] my head how I installed that thing. I probably just did curl pipe to bash or something like that.
[813.08 → 817.16] I think appliances are a different use case altogether though. I'm more talking about those
[817.16 → 823.52] people on Friends, on Unpaid, or maybe people like Open Media Vault users or people like me that just
[823.52 → 830.34] run Debian with some stuff, actually Ubuntu these days, that'll make you happy as my server OS. And I
[830.34 → 835.36] just run a bunch of containers on top of that. The other thing to think about, of course, is discoverability.
[835.36 → 840.72] You know, app stores have shown us that people like to browse through a list of stuff and click
[840.72 → 846.40] on buttons and install things to try them out. There are some good resources that I use to kind
[846.40 → 852.44] of counteract the GUI discoverability versus the command line stuff. One of those is the awesome
[852.44 → 858.32] self-hosted list, which we'll link to in the show notes. And the other is a list of containers published
[858.32 → 864.56] by the linuxserver.io team. That's at fleet.linuxserver.io. And you can actually just look through the list and it
[864.56 → 869.76] could take you through to the project page and show you how to deploy each one and all that kind
[869.76 → 876.74] of stuff. And even when I was actively involved in that project, which I'm not anymore, I used to
[876.74 → 879.90] find containers on there all the time. I didn't even know they would have been working on. So
[879.90 → 883.68] there are ways to find this stuff, even if you don't have a UI.
[883.68 → 891.18] I think that's a good point is now the Linux ecosystem has matured to the point where we have
[891.18 → 897.56] these different app stores and places people can go and browse a list of applications, whether they're
[897.56 → 904.44] containerized or not. Is light years ahead of where we were going and finding all the individual
[904.44 → 911.84] components and compiling them from scratch like animals. Now it is a point and click user interface,
[911.84 → 918.40] and you can stand up a service or a bunch of services really super easily these days.
[919.06 → 920.46] Too easily maybe sometimes.
[921.32 → 924.24] Well, yes, I'm a danger to myself.
[924.96 → 929.34] I mean, what I mean by that is that if it's, if the barrier to entry is so low that you set
[929.34 → 934.28] something up, and you have no idea how you did it in six months time, maybe you set Nextcloud up
[934.28 → 940.58] using a snap or a container or whatever it is. And you go, where's my actual data live? And you
[940.58 → 946.18] don't really understand how you did it, and you wipe the wrong drive and oops, it's easily done.
[947.00 → 951.16] Yeah. And the bigger worry is if other people depend on that service, like if you set up a
[951.16 → 958.04] public service, like a Mastodon instance, and other people are using it, and you haven't kept up with
[958.04 → 965.68] your security updates, or you haven't, you know, set it up using the best practices, then people might
[965.68 → 972.36] come knocking on your door because their data is compromised or, you know, their features are
[972.36 → 973.26] not available anymore.
[973.78 → 975.18] And of course, it's going to happen on a weekend.
[975.50 → 980.72] When you're away from a keyboard and your only interface to your, your Docker containers are SSH on
[980.72 → 981.52] your mobile phone.
[981.82 → 987.44] This is why you need an IRC room filled with community members. And of course, everyone knows
[987.44 → 991.08] that IRC is exploding with popularity in 2020.
[992.16 → 993.42] Oh, Chris.
[994.08 → 999.48] So I made the bodacious claim, although I was a little out there, that IRC was dead. And that
[999.48 → 1005.10] actually came from a FOSDEM talk where a member at FOSDEM said, I'm not joining your open source
[1005.10 → 1010.60] community because it's on IRC. I'm of the GitHub generation and I want to use Discord. I want to
[1010.60 → 1016.70] use Twitter. I want to use discourse, but I don't want to use IRC. Oh, my friends, we all chat on Slack.
[1016.70 → 1022.64] We don't, we don't chat on IRC. And he threw up some numbers like 13 million Slack users versus
[1022.64 → 1029.52] 400,000 IRC users. But there is a tinge of sadness when I talk about this because obviously
[1029.52 → 1033.58] you can self-host IRC and you can run other things in IRC as well.
[1034.32 → 1039.30] How many of those Slack users actually want to be there versus the IRC users though?
[1039.70 → 1040.44] Yeah, fair enough.
[1040.74 → 1045.22] I'd say a decent percentage are there simply because their employer mandates it.
[1045.22 → 1049.68] Yeah. I mean, there are some definite communities that use Slack, but you're probably right. Same
[1049.68 → 1051.36] with Teams. It was a big number for Teams.
[1051.84 → 1057.16] Yeah. I've been in Slacks where it was the network effect. There was one individual who
[1057.16 → 1062.96] pushed everyone towards a Slack. And the second they left the company, everyone left that Slack
[1062.96 → 1069.40] completely. So nobody is in that Slack anymore as a result of it being actually not what anyone
[1069.40 → 1077.50] wanted to use. And I realize, I appreciate that there are youngling who are using new modern tools,
[1077.58 → 1084.56] like you say, like Slack and Twitter and discourse. And that's fine. But it turns out there are still
[1084.56 → 1091.20] existing communities that have been around for a long time who do still have a presence on IRC.
[1091.20 → 1100.46] And it's actually not that painful to use IRC. Yeah. Okay. If you're advocating for the use of
[1100.46 → 1109.54] IRC or Bit Checks or one of the more quirky IRC clients, then for a new user, it's a bit frosty.
[1109.82 → 1117.68] But there are plenty of other ways to access IRC that are not quite as comparable with Slack,
[1117.68 → 1124.88] but nowhere near as frosty as it used to be. IRC Cloud is a great example of a very modern IRC client
[1124.88 → 1131.90] that I like to use. It does a lot of the things that Slack does, like image previews, URL previews,
[1132.10 → 1139.24] avatars, all just based on IRC. And the thing that pains me the most, and obviously our live stream
[1139.24 → 1143.94] for Jupyter Broadcasting is still IRC. The community is going right now. It's just over my shoulder.
[1143.94 → 1152.90] Um, is its all text. At the end of the day, it's all beautiful, wonderful, gorgeous text. And I,
[1153.04 → 1156.88] I would think that would be extremely appealing to the community at large.
[1157.60 → 1166.66] I think there's certainly a compelling argument for getting down to raw ASCII. There are times when
[1166.66 → 1173.70] I sometimes want to paste an animated GIF or, you know, something richer in an IRC channel,
[1173.70 → 1178.98] but really you've got to think about all the other people in the room. Like what is the purpose of
[1178.98 → 1184.02] this channel? Why does it exist? It exists to discuss the development of a piece of software.
[1184.76 → 1190.08] And you've got a bunch of people from different, uh, cultures, perhaps different,
[1190.08 → 1198.90] you know, um, connectivity. And if you're respectful of those and just use text, then it's accessible to
[1198.90 → 1204.38] everyone. Absolutely. And you could layer on client richness on top of that. So if you're someone that
[1204.38 → 1209.24] wants to see that animated GIF get a preview, then you could elect to use a client that shows that.
[1209.68 → 1214.24] Right. I mean, if I'm using IRC cloud, which I have done for a couple of years now,
[1214.24 → 1223.26] it feels very much like the more modern, richer, uh, clients. Actually, I think Slack have not really
[1223.26 → 1229.62] done an awful lot in, in the last couple of years. And that's given an opportunity for some of the
[1229.62 → 1237.66] other clients to catch up, whether it is the newer IRC clients or things like Mattermost, uh, and
[1237.66 → 1244.06] Discourse and Rocket Chat. A lot of them are catching up with the richness that Slack has.
[1244.24 → 1250.14] So they're getting to be mostly on a part and yeah, I will concede IRC is a bit behind all the
[1250.14 → 1257.52] others, but there are still, like I say, a bunch of projects that are still on IRC. And so sometimes
[1257.52 → 1263.76] if you're working in the open source world, as we do, it's useful to maintain a presence on IRC.
[1263.76 → 1268.76] So you can talk to these people. It does one thing. Um, it does one thing really, really well.
[1268.76 → 1274.54] And, uh, there is the saying that there'll be a few things left after a nuclear Holocaust,
[1274.74 → 1276.02] cockroaches and IRC.
[1276.52 → 1277.36] And maybe ham radio.
[1279.14 → 1283.52] I mean, I look at IRC, it's, it's a it's almost like it's the communications protocol. And then the
[1283.52 → 1288.06] client can add the richness. I know I've just said that, but I mean, think about it. One of the
[1288.06 → 1293.06] traditional complaints about IRC is that while I'm on mobile, and I have varying connectivity, so it's hard
[1293.06 → 1298.76] for me to follow a conversation. Slack handles that really well. Well, no, an IRC client that has a
[1298.76 → 1303.78] server log that is keeping track of the conversation and logging it to a SQL database and then disseminates
[1303.78 → 1308.98] it to a client when it reconnects works perfectly well. Quasar can do that. You can host it yourself.
[1309.42 → 1310.58] It's doable today.
[1310.76 → 1317.34] I've used Quasar for many years and, uh, the, the app that makes it the best IRC experience in my
[1317.34 → 1322.98] opinion is Quasar Droid. Red Hat use it for most of their internal communications. So I'm
[1322.98 → 1328.58] on eight, 10 hours a day and I get all the notifications through to my phone and it just
[1328.58 → 1335.96] works. It's just great. I went for an alternative approach and I used to use IRC or IRSSI if you
[1335.96 → 1342.02] want to spell it out. And I used to run that on my VPS and I would miss notifications when smart,
[1342.10 → 1347.42] I've been using it since before smartphones were a thing. And when smartphones became a thing,
[1347.54 → 1352.42] I quite liked the idea of having that connectivity to IRC on the phone.
[1352.98 → 1359.00] And I didn't get the notifications. Uh, and there's an app in the Android app store called
[1359.00 → 1367.32] IRC Notifier and you load a plugin into IRC and then authenticate it with your, with your Android
[1367.32 → 1371.86] device. And from that point onwards, you get push notifications through to your phone when people
[1371.86 → 1380.10] mention your name or highlight you in some way or, uh, PM you on IRC. So I, I started to get that
[1380.10 → 1385.02] availability of, you know, the, the messages people were sending me and the conversations people were
[1385.02 → 1391.60] having. I didn't feel left out of the conversations, but the problem was I couldn't then reply because
[1391.60 → 1398.92] they were just notifications. And so I did find myself leveraging that SSH client on my phone and I
[1398.92 → 1405.52] would SSH into the VPS and use IRC inside a screen session so that I could bash out a quick reply to
[1405.52 → 1410.28] someone if it was urgent and then disconnect from SSH, uh, when I'm done.
[1410.76 → 1413.00] Okay. When you say all that, I know why people are switching to discord.
[1413.94 → 1420.00] Right. And that's quite brutal. I mean, that is between 10 and 15 years ago, I was doing that.
[1420.14 → 1425.64] You know, I remember being on holiday 15 years ago with my daughter in a pram and getting a push
[1425.64 → 1431.64] notification on IRC, but something was going on. And while I'm pushing my daughter along with one hand,
[1431.64 → 1437.56] I'm typing in my SSH password on my phone with the other and getting into IRC, but it's possible,
[1437.56 → 1443.32] but things have moved on a bit now. And we now have better ways of being on, on IRC.
[1443.86 → 1450.22] The juxtaposition of you, Pope, on one hand, you're advocating for UIs to make things simpler.
[1450.22 → 1454.28] And on the other hand, we're talking about SSH passwords on IRC from our phone.
[1454.28 → 1458.96] Yeah. I'm not complaining. I, I love the fact that I could SSH to my VPS from,
[1458.96 → 1463.66] you know, walking along, having a stroll around, around the Isle of Wight with my daughter. That
[1463.66 → 1464.10] was great.
[1465.36 → 1470.52] So what do you use for IRC on iOS, Chris? Cause that was one of the major pain points I had. I
[1470.52 → 1477.82] tried out iOS in the fall last year in autumn, and I just couldn't get away with any clients that
[1477.82 → 1480.66] really were as good as Quasar Droid.
[1480.66 → 1485.00] Quasar Droid does look perfect. So I, I, I don't know if this is as good,
[1485.06 → 1490.84] but I just use the IRC cloud client for iOS, which is just a native IRC app.
[1490.96 → 1496.20] I think I might have some unique requirements in that the Red Hat IRC stuff, I have to be on a VPN
[1496.20 → 1500.74] to connect to it. So IRC cloud wouldn't really work for that use case.
[1501.12 → 1506.06] That's sort of the tricky thing is you can both roll your own solution, and you have to roll your
[1506.06 → 1510.50] own solution with IRC in that regard. So I'm not going to sit here and try to say,
[1510.50 → 1515.16] it's as easy as all the other alternatives. It might even honestly be easier to set up a
[1515.16 → 1522.72] Mattermost server than an IRC server these days, but there are other aspects of IRC that I, I don't
[1522.72 → 1528.68] know what we would do if say we switched to discord, I guess we would rewrite Bot. I, I guess,
[1528.78 → 1534.36] I don't know. Like the, the bot aspect is a very nice thing about IRC, and it feels like it's a wild
[1534.36 → 1538.20] west. You can do whatever you want. Whereas with these other platforms, you have to get an
[1538.20 → 1543.34] integration. And I think that's one of the reasons why Slack took off so well with open source
[1543.34 → 1549.10] developers is you could press a couple of buttons, and you'd have an integration that told you whether
[1549.10 → 1553.00] your Jenkins was operating correctly and whether your code was landing. And if someone had reviewed
[1553.00 → 1559.20] your code. And so for developers Slack with a few integrations was a very compelling argument
[1559.20 → 1565.22] against, Oh, well, IRC and I have to write some Python to make my own bot or go and find a bot that
[1565.22 → 1570.44] someone's made and create a new IRC account and all that nonsense. I could totally see why,
[1570.56 → 1576.14] why that's more compelling. So the whole reason we're really talking about IRC and the reason that
[1576.14 → 1581.56] Pope's on the show today is he reached out to me a few days ago about something he's just put into
[1581.56 → 1585.76] a snap. Is that right? Yeah, it's actually been a snap for a while, but we've improved it.
[1586.36 → 1593.16] It's an IRC client, shall we say, but it's a web front end. So you can effectively think of it as
[1593.16 → 1601.66] self-hosted IRC cloud. So you install it. It's called the lounge. And it's a fork of a previous
[1601.66 → 1609.92] project that was called shout IRC. You install the lounge on your own machine. You create an account
[1609.92 → 1617.64] for every user who's going to use it. So multiple users can use that IRC client. And then you just
[1617.64 → 1622.74] point your web browser at it and log in. Once you've logged in, you can then sign in to all your
[1622.74 → 1629.96] different IRC networks. And the connection is then maintained from that, the lounge server to all
[1629.96 → 1637.20] of those IRC networks. And so you don't have to run any client anywhere because the lounge is the client.
[1637.50 → 1643.90] And all you need to do is point a web browser at it, and you're an IRC. And you can point a web browser
[1643.90 → 1652.72] at it from anywhere, like from your desktop or from your phone. So I have a Chrome window.
[1652.74 → 1658.96] on my desktop, but it could just as easily be Firefox or any other browser. And that window points to
[1658.96 → 1665.68] my lounge server, which is connected to all my IRC. But then I also have a similar browser window
[1665.68 → 1674.90] on my phone, which points to exactly the same URL and connects to all the same IRC channels. So I can
[1674.90 → 1681.72] be on exactly the same IRC channels on my phone in a browser with the rich content that you see with,
[1681.72 → 1686.58] you know, images showing up and stuff like that, that you would see in something like IRC cloud
[1686.58 → 1692.94] or, you know, other modern chat systems. It's made a real change to me because I'm now self-hosting my
[1692.94 → 1699.68] own IRC client again, instead of relying on IRC cloud. But also I can access it from anywhere on
[1699.68 → 1707.18] the phone and the desktop. That's great. I like that a lot. And it's something that the Linux server
[1707.18 → 1711.92] team containerized quite some time ago. So you can get it in a container as well. If that's more
[1711.92 → 1717.08] up your street. It looks like the UI is really sharp too. It probably is, I would even say
[1717.08 → 1721.96] competitive with IRC cloud. Do, would you agree having used it? Yeah. I went through a process last
[1721.96 → 1728.42] week of disconnecting from all my IRC networks in IRC cloud and closing it. And now I only use the
[1728.42 → 1735.76] lounge. The thing that I love about it is because it's self-hosted, I feel a lot more safe. It's logging
[1735.76 → 1742.02] everything on my own server and a change that we made last week to the snap because we've got it
[1742.02 → 1749.46] published in the snap store. Uh, we integrated cert bot into the snap. So now once you've installed
[1749.46 → 1755.64] the lounge, you can then put an SSL cert on it with one line, and then it puts a cron job on your
[1755.64 → 1763.54] system automatically, and it will just keep refreshing that SSL cert. So I've now got SSL between me and my
[1763.54 → 1769.30] lounge server, whether I'm on my phone or I'm on the desktop. And then from my lounge server to my
[1769.30 → 1775.02] IRC networks, I've got an SSL connection there as well. So I feel, I feel a lot happier. I always
[1775.02 → 1779.12] had this nagging thing in the back of my head that I was, there's nothing wrong with IRC cloud. It's
[1779.12 → 1786.16] great, but all my IRC logs are hosted on IRC cloud. And there was that little twinge in the back
[1786.16 → 1791.60] that I just thought, I don't like this. You're kind of losing one of the best things about IRC by doing
[1791.60 → 1796.58] it on IRC cloud. And I do it out of convenience, but I think of this weekend, I'm going to make
[1796.58 → 1801.22] the switch to this. This looks so, so nice. Do you happen to recall what the database back in,
[1801.26 → 1805.36] that it's storing all of this in? The logs are free texts stored on your file system.
[1805.64 → 1811.40] I love that. It also does push notifications because it's in a browser. I just pressed the
[1811.40 → 1816.74] button to say enable push notifications. And now on my phone, I get notifications when people
[1816.74 → 1821.50] mention me on IRC, I click on them, and it takes me straight into the browser window. It feels like
[1821.50 → 1826.26] an app. You know, it's, it's just a browser window, just like all the cool kids use these days.
[1827.94 → 1830.68] It's so nice to see something like this that you can host yourself.
[1831.04 → 1835.34] Ah, I love this kind of stuff, Pope. I love it. The lounge. We'll have a link in the show notes.
[1835.46 → 1841.90] Of course. I don't know if I'll switch from my beloved Quasi Droid, but we'll see. I'm going to,
[1841.90 → 1847.66] I'm going to try it and spin it up. At least people who use IRC, who have used it for years,
[1847.66 → 1856.28] are often totally wedded to the solution they've got. Like, IRC, for me, I don't care what IRC client
[1856.28 → 1862.68] anyone else uses. This is God's own IRC client, and you will never make me move from it, right? But
[1862.68 → 1869.20] you'll hear people just as passionate about Quasi or any of the others. The guys in France at
[1869.20 → 1874.02] Canonical have their favourite IRC client and all the guys in France seem to use the same one.
[1874.02 → 1878.76] And all the guys in the UK all seems to use IRC. I don't know why, whether the translations are
[1878.76 → 1883.30] better or different or what, I don't know. But people are super passionate about their IRC client,
[1883.52 → 1889.72] which is a thing you never get with Slack because there are no really first class alternative
[1889.72 → 1894.14] clients for it. It's just not a thing. You just don't have that choice.
[1894.64 → 1897.34] Right. Yeah, that's very true. That's a good point.
[1897.86 → 1900.34] So Chris, I have a question for you. Yes, sir.
[1900.62 → 1901.84] Why are you in your dressing gown?
[1901.84 → 1910.18] Oh, outing me like this on the show. The furnace is broken in the studio, and I'm doing a podcast
[1910.18 → 1915.36] when it's 30 degrees outside. So I figured, you know, I'd get comfortable and put my robe on.
[1915.86 → 1920.28] So the furnace broke in your RV and the studio in the same week.
[1920.60 → 1924.90] Well, the furnace in the studio has been going out for the last couple of years, and it was just
[1924.90 → 1929.28] this winter that it kind of gave the ghost out, you know, just like some sort of like final
[1929.28 → 1935.10] thing happened, and it's just falling apart. It works, but it only heats the upstairs.
[1935.34 → 1937.52] So like 50% of the studio is liable.
[1937.62 → 1939.28] Good job. Heat rises, hey?
[1939.86 → 1945.26] Yeah, I know. But when I do get it fixed, I'm going to need somewhere to document the fix.
[1945.26 → 1949.54] Alex, do we have perhaps a wiki?
[1949.94 → 1956.06] The self-hosted wiki is in full flow. We have a group now with about 15 or 16 people already
[1956.06 → 1963.30] since the last episode who have started contributing their free time, chatting all day,
[1963.40 → 1968.54] every day about what, you know, different technology stacks to use. For now, we're using MK Docs,
[1968.54 → 1973.98] but we are trying to decide whether to use that platform or another one called Hugo, which is a
[1973.98 → 1979.66] static site generator that might have some more customization when it comes to theming.
[1980.12 → 1985.96] But we're early enough in the process that what we're really looking for right now is good,
[1986.24 → 1991.96] solid content. And we're not trying to reproduce stuff that's already out there on the internet.
[1992.14 → 1996.88] You know, we don't want to provide a list of self-hosted apps because the awesome self-hosted
[1996.88 → 2002.68] list already does that. What we're looking to do is actually provide, you know, code snippets,
[2002.98 → 2008.18] Docker Compose, for example, snippets of maybe the Lounge or Quasar, like we talked about on this
[2008.18 → 2014.36] episode, just to help people break down that barrier of entry of self-hosting some of this stuff.
[2015.16 → 2020.20] You know, I flashed some Taste devices the other week, so I'm in the middle of writing up a little
[2020.20 → 2026.38] page to go on there about Taste and what it is and why you might like it. But also we'll link back
[2026.38 → 2031.50] to the particular episodes in which we talk about certain stuff as well. So one of the things I
[2031.50 → 2035.74] quite often get is, oh, which episode did you talk about cameras? I don't want to go through the show
[2035.74 → 2042.46] notes one by one, but if I can search it in the wiki and find the episode that way, that's one of
[2042.46 → 2046.24] the problems we're trying to solve with this wiki. But I've been delighted with the response. I must
[2046.24 → 2051.50] have had 30 or 40 different emails or telegram messages from people just in this last few days
[2051.50 → 2057.88] alone. So if you want to be part of it, you can go to wiki.self-hosted.show, which will take you to
[2057.88 → 2064.12] the GitHub Pages hosted site. We are going to host it ourselves, but for now it's on GitHub Pages.
[2065.02 → 2072.20] And be part of it. Help us choose the tech stack, choose what content goes in there and what the
[2072.20 → 2076.68] different directory structures and layout and all that kind of stuff looks like. It's going to be a
[2076.68 → 2082.46] crowdsourced thing. So if you want to have input, now's the time. I'm really happy to see people
[2082.46 → 2087.20] that are getting involved with this. It's like really that telegram group's almost too much at
[2087.20 → 2094.20] this point for me. This is completely thrown me. I've got my own wiki on like popi.com. It's just a
[2094.20 → 2100.38] Dou wiki that I use for keeping some notes, but I've also been using Hugo for another project.
[2100.82 → 2105.50] And now you've mentioned it, I'm thinking, why don't I just replace my wiki with
[2105.50 → 2111.44] a Hugo instance? And then I could do it all nicely in Markdown. I can just use standard
[2111.44 → 2117.02] Git tools to commit my changes and then automate pushing it live. It's such a good idea.
[2117.34 → 2120.60] Use GitHub issues and pull requests and all that kind of stuff.
[2120.94 → 2125.32] No, I just commit to master because it's my wiki. I can do what the hell I want.
[2126.04 → 2130.22] What was it you called me earlier? Elite hacker? Hardcore elite hacker? Yeah, that must be you now.
[2130.22 → 2138.10] So you're loving Hugo, huh? Oh, yeah. There's a theme I'm using on one of my sites. I think it's
[2138.10 → 2145.10] called paper, and it automatically changes light to dark throughout the day. So when I refresh the
[2145.10 → 2150.52] browser, if it's in the evening, I know it's the evening because the browser just all dims nicely.
[2150.66 → 2155.56] It's really, really nice. That is slick. Don't look out the window and see what the light level is.
[2155.56 → 2160.40] No, just look at your browser. Yeah. Who needs it? We can automate that.
[2160.68 → 2164.68] My blind is closed. I can't see outside. I never do that.
[2166.84 → 2172.66] So how will the self-hosted podcast end up self-hosting its self-hosted wiki? Stay tuned
[2172.66 → 2176.78] and find out. But in the meantime, wiki.self-hosted.show if you want to get involved.
[2177.28 → 2181.48] I guess we kind of need to get a sense of what the interest is to kind of get an idea of what the
[2181.48 → 2185.72] traffic's going to be to then decide how we're going to host it. So that's the phase we're in
[2185.72 → 2190.68] right now. It's looking really great though. So that's super neat. That's really cool.
[2191.46 → 2194.86] So Pope, where should people go to find more of you throughout the week?
[2195.26 → 2201.46] Oh gosh. Well, they can go to my wiki. I have a contact page, but that might be moving.
[2201.68 → 2203.48] Can they find your last will and testament there?
[2203.48 → 2210.78] I had a very funny email actually from a gentleman who was it? No, it was on Twitter.
[2211.04 → 2212.80] Honey, I need to set up a wiki.
[2213.94 → 2215.18] Yep. That was great.
[2215.38 → 2217.80] That was very funny Twitter exchange, but yes.
[2218.04 → 2221.62] We need to have a morbid conversation in case something ever happens to me. We need a wiki,
[2221.76 → 2221.98] darling.
[2222.56 → 2227.18] Yes. Of course, Pope, you're on user error, which is one of my favourite podcasts.
[2227.64 → 2228.54] Yes, absolutely.
[2228.54 → 2234.90] Oh, thank you. Yes. It's lovely having an argument with Dan and Joe about all kinds
[2234.90 → 2242.54] of random stuff. We enjoy hearing the audience questions and trying to answer them. So if people
[2242.54 → 2249.32] have questions for us, just ping us in the JB telegram with hashtag ask error or on Twitter
[2249.32 → 2250.96] or anywhere, we'll probably spot it.
[2251.38 → 2255.58] I am delighted by how often you are voicing exactly what is in my head. Even you are all
[2255.58 → 2257.20] the way across the pond, all the way over there.
[2257.20 → 2257.86] That's worrying.
[2257.86 → 2264.96] It is a bit actually, isn't it? It's really quite something. You really often echo my thoughts
[2264.96 → 2269.08] on very many topics, but you deliver them better than I would. So it really, it is one of my
[2269.08 → 2273.04] favourite shows as well. And of course, rumour has it the Ubuntu podcast may be coming back
[2273.04 → 2274.64] soon. So of course, Ubuntu podcasts.
[2275.18 → 2281.70] It's more than a rumour. We're recording first episode of season 13 next week as we record
[2281.70 → 2282.06] this.
[2282.40 → 2282.72] Boom.
[2282.94 → 2286.30] Oh, announcing season 13 on SSH 13. I like it.
[2286.30 → 2287.80] Right there. Yes.
[2287.86 → 2290.24] Very nice. Very nice. Well, thank you, Pope, for making it.
[2290.42 → 2291.36] Thanks for having me on.
