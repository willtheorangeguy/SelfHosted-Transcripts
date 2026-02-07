[0.00 → 4.46] Well, Alex, we're gathered together for episode 117 of the self-hosted podcast.
[4.70 → 9.40] We've got a lot to get into this week, so we should probably right off the bat here,
[9.48 → 10.52] introduce our guest.
[11.30 → 13.40] I'm delighted to welcome to the podcast, Brett.
[13.58 → 16.60] You might know him better as Raid Owl from YouTube.
[17.02 → 21.56] Describes himself as just a nerdy dude who's passionate about home lab stuff,
[21.82 → 24.26] networking, PC builds, and tech in general.
[24.48 → 25.22] Welcome to the show, Brett.
[25.50 → 26.98] Thank you so much for having me.
[26.98 → 33.70] Yeah, that sounds like a pretty decent description I wrote for myself, so I'll take it.
[34.34 → 37.26] We didn't even involve ChatGPT in that one, so yeah.
[37.26 → 37.72] Not right.
[37.96 → 38.90] Not yet, yeah.
[39.08 → 41.76] Although one of us may be ChatGPT, but we won't say who.
[41.80 → 43.20] Yeah, that's for you guys to find out.
[43.60 → 48.06] So we thought we'd talk to you today about a few things home lab related.
[48.20 → 50.82] Obviously, there's the VMware news, which we'll get into in a little bit.
[50.82 → 57.32] But before we go there, I've noticed on Twitter that you're talking about 30 days of Linux
[57.32 → 58.06] challenge.
[58.36 → 59.48] What's that all about?
[60.20 → 62.20] I don't even know where to start with this.
[62.24 → 68.62] So last year, I did a, I'm going to switch to Linux challenge because I hate myself.
[68.62 → 79.16] And I did it for a week when I got rid of my MacBook and my main Windows machine and used,
[79.46 → 88.20] or I, for that one, I installed, I think I used Ubuntu on my desktop and did it for a week.
[88.30 → 93.06] And at the end, I came out the other end hating Linux as a desktop.
[93.06 → 96.72] And of course, you know, everyone loved that.
[97.42 → 103.48] So I said that next year I would try again and do it a little differently.
[104.18 → 106.52] So that's what I'm doing this year.
[106.62 → 108.96] I've extended the duration.
[108.96 → 112.44] It's now 30 days instead of a week.
[112.44 → 120.90] And I'm running it on a laptop instead of a desktop because if I'm doing it for a month,
[120.98 → 124.38] I can't be tied down to my desktop the entire month.
[124.66 → 129.90] So here I am on a Dell XPS 15 running Linux Mint.
[130.66 → 135.36] I am about three weeks in now.
[135.88 → 137.14] I'm just under three weeks.
[137.78 → 138.98] And it's been something.
[138.98 → 142.80] You sound like a man who has aged in the process, if I'm honest.
[142.80 → 143.14] I have.
[143.30 → 146.78] I used to have a lot of hair and no gray in my beard.
[147.88 → 152.46] And I have no hair and lots of gray in my beard now.
[152.76 → 155.34] So not to spoil the conclusion of the challenge,
[155.42 → 157.84] because obviously you're only three out of the four weeks into it.
[157.84 → 158.08] Yeah.
[158.20 → 161.14] But I'm curious, like, as a YouTuber,
[161.24 → 163.80] obviously you're doing video workflows a lot of the time.
[163.88 → 165.12] So I don't know.
[165.18 → 166.58] Are you a Mac guy typically?
[166.58 → 173.66] I use a MacBook, an M1 Pro MacBook Pro as my main laptop.
[173.94 → 179.38] And then I have a Windows desktop that I use as my main workstation.
[180.50 → 180.80] All right.
[180.96 → 181.26] Yeah.
[181.60 → 185.38] And typically your workflow is, I'm assuming, then probably Adobe based?
[185.64 → 186.44] It used to be.
[186.62 → 189.08] I'm on da Vinci Resolve now.
[189.32 → 189.82] Oh, nice.
[189.90 → 191.12] And of course, that's on Linux too.
[191.12 → 195.92] Yes, that was, I guess, convenient.
[196.42 → 202.78] I switched from Adobe to Resolve last year, not because of anything Linux related,
[203.22 → 205.68] but because Adobe has been pissing me off.
[206.48 → 206.56] So...
[206.56 → 208.20] And it's expensive these days.
[208.22 → 208.92] It's expensive.
[208.92 → 216.46] And just the quality of their upgrades to Premiere have just been so mediocre.
[217.00 → 220.70] And I noticed I was getting better performance testing on da Vinci.
[221.28 → 224.34] So I said, why not just pay 300 bucks one time?
[225.26 → 225.78] Use da Vinci.
[225.98 → 231.50] It's compatible on my Windows machine, my MacBook, and my Linux machine.
[231.50 → 235.68] So that part's been decent, I will say.
[235.92 → 241.70] Being able to use my pretty much same workflow for editing.
[242.00 → 245.26] Whereas last year I was still on Premiere Pro when I switched.
[245.68 → 252.00] So I ended up using Caden Live, which is a free Linux-based video editor.
[252.64 → 254.50] And that was...
[255.44 → 256.50] I don't...
[256.50 → 257.96] It wasn't terrible.
[257.96 → 261.76] But compared to something like Premiere Pro, it was difficult.
[262.70 → 265.74] I just tweeted that it hasn't gone as expected.
[266.12 → 270.48] Not so much because it's more difficult than I expected.
[270.78 → 271.96] It's more of...
[272.50 → 277.24] I went into this time thinking, okay, I have 30 days.
[277.34 → 279.98] I'm going to learn a lot about Linux in these 30 days.
[280.20 → 281.56] I'm going to come out the other side.
[282.24 → 286.02] Being, you know, up on my high horse, ready to, you know,
[286.16 → 287.88] talk down to the Linux clubs.
[288.12 → 288.78] I'm joking.
[289.10 → 293.98] But that hasn't been the case with other videos in the works
[293.98 → 296.96] because I can't just stop making videos for 30 days.
[297.00 → 297.64] I mean, I can.
[298.12 → 299.94] This isn't my real job, but I don't want to.
[300.38 → 303.60] Other videos happening, real life things happening.
[303.96 → 306.78] And I found myself like in this last week,
[306.78 → 310.34] I hadn't really learned much that I had planned.
[310.58 → 313.92] So I don't know what this video is going to look like at the end, honestly.
[314.08 → 314.68] So we'll see.
[314.80 → 315.62] We've got a week left.
[315.62 → 318.18] I have found that one of the trickier things to do
[318.18 → 321.72] is to try to make a transition like that when you're really busy
[321.72 → 325.72] because it's everything is a new learning process.
[325.92 → 327.52] But see, it's been about a year.
[328.34 → 330.82] What's better since the last time you tried it?
[330.90 → 332.10] Has anything gotten a little bit better?
[332.10 → 336.10] So last year I tried, I used Ubuntu.
[337.44 → 338.54] This year I'm on Mint.
[338.64 → 342.20] I was debating between Pop! OS and Mint.
[342.20 → 345.50] I'm just more comfortable with Debian-based stuff.
[345.70 → 350.12] I know everyone out there, like it was a joke when people would ask me,
[350.26 → 352.80] you know, which district you go with, I would just tell them the wrong one
[352.80 → 354.66] because no matter who you ask.
[354.80 → 356.08] There's never a right answer, is there?
[356.26 → 359.48] You grow a thick skin in this business after a while on that question.
[359.56 → 360.16] I'll tell you what.
[360.52 → 361.12] I went with Mint.
[361.38 → 363.56] It felt decent.
[363.82 → 366.16] I was debating between, like I said, Pop! OS and Mint.
[366.16 → 367.66] Eventually chose Mint.
[368.40 → 372.84] Compared to last year, having everything working right out of the box,
[372.92 → 378.20] especially on a laptop, because I've tried Linux installed on a laptop,
[378.62 → 380.20] you know, years and years ago.
[380.42 → 383.98] Probably, you know, maybe once a year since then.
[384.68 → 388.60] And I've always run into issues with, like, touchpad not working,
[388.90 → 392.64] Wi-Fi drivers not automatically loaded, you know, random stuff like that.
[392.66 → 394.34] There's always something.
[394.34 → 399.90] So I was fully prepared to, day one, just be like, okay, guys,
[400.04 → 403.48] the screen only shows every other pixel.
[403.78 → 404.94] I don't know what to do.
[405.12 → 405.60] Please help.
[406.30 → 410.42] But out of the box, I mean, everything worked great.
[410.56 → 415.24] I mean, it's a relatively recent kernel that Mint 21's on.
[415.80 → 422.28] So it's, you know, in that aspect, I'd say it's much improved.
[422.28 → 426.24] Maybe not so much since last year, but I'd say over the last few years.
[426.76 → 428.00] How has the stability of apps been?
[428.16 → 432.40] Just as one quick follow-up question, have you had application crashes?
[432.56 → 433.24] Has that been okay?
[433.56 → 434.28] Oh, yeah, 100%.
[434.80 → 437.48] That's what I live for, application crashes.
[437.94 → 438.52] You've had those?
[439.38 → 440.98] OBS likes to.
[441.28 → 441.50] So.
[442.36 → 443.14] NVIDIA system?
[443.28 → 444.06] It's an NVIDIA card?
[444.06 → 444.78] Oh, yeah.
[444.86 → 450.50] So it's just, it's a Dell XPS, Dell XPS 15 9530 or something.
[450.72 → 451.68] It's got a.
[451.68 → 451.90] Right.
[451.96 → 452.74] With the NVIDIA.
[452.94 → 455.40] Yeah, with the RTX 3050.
[455.68 → 456.48] That's a nice laptop.
[457.18 → 462.76] I wanted to make sure that I gave it the best chance to impress me.
[462.96 → 465.20] Yeah, the NVIDIA card is really tricky right now.
[465.44 → 466.88] We're in an awkward period there.
[466.88 → 474.14] So I noticed one thing that I, I don't know if it's a mint thing, or you can choose between
[474.14 → 484.28] like power profiles and it, you can pick between only use Intel, only use NVIDIA or this on demand
[484.28 → 488.78] where, you know, when you launch an app, it has some way of determining if it's a graphic
[488.78 → 491.64] intensive app, and it'll use a GPU for it.
[491.64 → 497.40] I had some issues with it in the beginning, but now it's working pretty well.
[497.80 → 504.34] I'm honestly surprised because one of the main issue or main fears I had going into this was that,
[504.42 → 509.58] you know, I'm used to running a MacBook and then one MacBook that I can get freaking like
[509.58 → 513.58] two whole days of battery life, not even think about plugging it in.
[514.00 → 519.62] This one, I was so nervous about, you know, battery dying instantly.
[519.62 → 528.86] And man, I am impressed with this, you know, on demand, you know, run Intel on pretty much
[528.86 → 531.72] everything desktop and then all using NVIDIA for the stuff you need it for.
[532.44 → 533.34] Battery life has been awesome.
[533.94 → 536.84] So that's another thing that's impressed me, I will say.
[537.56 → 539.38] But yeah, crashes, OBS.
[540.12 → 544.94] I don't know if it's docking it with a Thunderbolt dock and then unplugging it.
[544.94 → 551.12] But anytime I undock it or dock it in, I have to like to cross my fingers, do a little dance,
[551.56 → 558.60] pray to the Linux gods that my NVIDIA card doesn't just disappear or give me errors.
[559.18 → 560.18] So, yeah.
[560.64 → 565.54] Now we've been chatting behind the scenes a lot about changes that are happening with VMware.
[565.84 → 570.44] One of the ways that I really got my hands on VMware was through their free programs.
[570.44 → 573.90] They had ESXi free, they had player that was free.
[574.96 → 581.54] And through that, I kind of learned a lot about the basics and then was able to go to my company
[581.54 → 584.88] and say, I think I'm actually comfortable recommending we deploy this at scale.
[585.66 → 595.44] And we ended up having a very large offsite data centre with about 115 servers that were all using VMware ESXi
[595.44 → 598.42] or whatever it is, whatever the expensive one was.
[598.42 → 602.02] And it all really kind of got started, though, because I was able to get my hands on the free one
[602.02 → 603.66] and experiment in my home lab.
[604.20 → 607.80] And, Brett, I'm curious if you've been following the VMware news that happened recently,
[607.90 → 614.70] but VMware's been pulling a bunch of products, including their free ESXi product, I think it is.
[614.96 → 615.56] ESXi, yep.
[615.60 → 615.82] Yeah.
[616.22 → 622.36] As a consumer, as a home lubber, you know, the home lab space is very, I'd say, finicky
[622.36 → 625.80] when it comes to anything that requires money.
[625.80 → 630.52] Anytime you see something, because, you know, it's built upon, like, you know, open source
[630.52 → 635.90] and FOSS, you know, just free software, building a community around that, you know, it's a big
[635.90 → 636.78] part of home jabbing.
[636.98 → 641.70] So when you see any, like, bigger corporations come in and make these changes, especially with
[641.70 → 647.94] something that was, you know, free and readily available, and then paywall it, you know,
[647.96 → 650.72] that's not going to make anybody happy, especially the home lab community.
[650.72 → 657.76] I never used ESXi in an extensive, you know, environment.
[657.90 → 659.48] I've tested it a couple of times.
[660.12 → 667.82] So my direct impact is minimal, but I know people who are extremely upset about this because,
[668.22 → 670.32] you know, this is something that they deploy in their home lab.
[670.40 → 672.58] This is something they have quite a few servers running.
[672.58 → 676.02] And to just all of a sudden be like, oh, yeah, guess what?
[676.72 → 678.78] That's, you have to pay for that now.
[679.56 → 680.66] It's huge.
[680.96 → 688.34] And one of my buddies, Rich from Two Guys Tech, did a pretty good video on that about the changes
[688.34 → 694.58] to VMware and about how the switch to something like XCPNG would be.
[694.96 → 698.54] It's hard for me to sit here and say, like, you know, as a business, it's not the right
[698.54 → 698.80] call.
[698.80 → 699.60] What's the right call?
[699.68 → 705.76] I'm not a business guy, but as a home lab user, I know a lot of people are not happy.
[706.26 → 708.44] Well, I'm sure they've done the calculations, right?
[709.08 → 714.58] They're following a similar model to many other big corporate mergers.
[714.76 → 722.56] You know, the prevailing wisdom is that VMware makes 90% of their money from 10% of their customers.
[722.56 → 728.06] And so they're just going to double down and focus on that big 10%, those big customers
[728.06 → 732.84] that spend hundreds of millions of dollars with them every year.
[733.48 → 736.94] And the little guys actually are a rounding error.
[737.12 → 742.06] And I guess maybe those rounding errors to you and I seem like big numbers.
[742.20 → 746.14] But when you're dealing at VMware's scale, perhaps they don't.
[746.14 → 754.24] And what really, I think, for me, the most tragic part of this is that it's killing the pipeline.
[755.10 → 759.38] I'm not, you know, I'm not going to sit here and say that VMware have been great open source
[759.38 → 762.66] advocates and stalwarts or anything like that because they haven't.
[763.44 → 768.88] But the reality is, in the business world, they were one of, if not the de facto method
[768.88 → 770.46] of running things on premise.
[770.46 → 775.34] And it was a standardized tool that you could learn and change between different companies
[775.34 → 778.42] and say, right, I know VMware inside out and backwards.
[779.02 → 784.30] At the bank in London I used to work at, for example, there was a guy whose entire job
[784.30 → 790.06] was talking to VMware all day, figuring out what was coming down the pipeline, implementing
[790.06 → 790.72] it at the bank.
[790.84 → 794.84] And, you know, if I said to him, right, I need to deploy X number of OpenShift nodes next
[794.84 → 797.94] week, he'd be like, right, well, I need to call this guy for hardware and I need to get
[797.94 → 802.50] this license in, and it was this whole-complicated thing that he'd built his career around.
[802.76 → 806.34] And now I'm sort of sat here thinking, well, what's he going to do?
[806.56 → 810.56] What are all the MSPs who've been reselling VMware for the last decade plus?
[810.88 → 812.10] What are they going to do?
[812.20 → 813.10] Never mind the home labels.
[813.18 → 814.96] I mean, they'll be all right, I think.
[815.56 → 822.20] You know, there's Proxmox, there's XCPNG, there's Beehive, there's Flipping Lib Vert.
[822.36 → 826.36] You know, there's a million different ways to run VMs in a home lab, but it's the people
[826.36 → 828.80] that have built businesses around it that I really feel for.
[829.28 → 829.70] Yeah, for sure.
[829.82 → 835.36] And those people, obviously, you know, they didn't have a say in this, you know, that's,
[836.08 → 840.00] you know, like you said, resellers, people who, this is their business.
[841.30 → 847.72] I'm 99% sure that the executives over there didn't personally go up to them and ask them
[847.72 → 849.68] for permission to do this.
[850.30 → 852.32] So that's got to be...
[852.32 → 853.76] So what's your home lab situation?
[853.88 → 855.00] What's your hypervisor look like?
[855.00 → 857.14] Uh, I'm a Proxmox boy.
[857.78 → 866.18] I got a main Proxmox server, then I have a three-node Proxmox cluster for like my super-duper
[866.18 → 868.46] important high-availability stuff.
[868.96 → 871.78] That's not actually that important, but...
[871.78 → 873.42] Am I detecting sarcasm there?
[873.48 → 874.34] Oh, yeah, absolutely.
[874.90 → 878.04] I hope my sarcasm came through because it's...
[878.04 → 879.24] None of it's super important.
[879.56 → 884.04] The world will still go around if my cluster goes down, but it's fun.
[884.04 → 885.88] Hey, look, dude, I'm British.
[885.98 → 888.24] We practically invented sarcasm, so I think we'll be all right.
[888.24 → 888.42] Perfect.
[890.00 → 894.60] Okay, so then we have to ask, how much storage is attached to all of this?
[894.64 → 899.02] Like if you were to just do a rough back-of-the-napkin kind of math calculation,
[899.42 → 902.30] how much storage would you roughly say is in your home network there?
[902.36 → 904.56] We just try to keep track when we have people on the show.
[904.56 → 907.72] I don't think it's anything impressive compared to what...
[907.72 → 914.78] Even people on my Discord have a crazy amount of storage, but my main server...
[914.78 → 915.24] There's no shame.
[915.24 → 917.30] Yeah, my main server, so it's a Proxmox server.
[917.42 → 919.14] It's running True NAS on a VM.
[920.18 → 924.34] And I have all my drives passed through to theirs, and it's 12 terabyte drives.
[924.56 → 926.40] So 144 terabytes.
[926.40 → 929.06] That's a solid entry in our leaderboard.
[929.52 → 930.14] I think so.
[930.30 → 932.36] That puts you above Jeff Deerling.
[932.54 → 936.54] Oh, man, I'll have to hit him up and say I'm ahead of him on something.
[936.86 → 939.32] Although Jeff didn't include the petabyte pie in his...
[939.32 → 940.02] Oh, yeah, that's...
[940.02 → 944.68] We still hold Wendell in first place with a petabyte, so I think...
[944.68 → 946.10] Yeah, I'm not close to that.
[946.20 → 955.38] I mean, if you count my backup server too, then you're looking at, like, maybe another 60 terabytes, so...
[955.38 → 956.90] All right, that's a solid entry.
[957.06 → 959.40] I'm going to give you 200 terabytes.
[959.50 → 959.90] How about that?
[959.96 → 962.18] Yeah, let's just round it and say 200.
[962.30 → 962.90] That's a fair...
[962.90 → 963.84] All right, the board approves.
[963.86 → 967.58] Somebody from the audience will open a pull request on our wiki and put you on our leaderboard.
[967.66 → 968.68] So that's pretty cool.
[968.68 → 970.68] Now, I noticed in the...
[971.34 → 973.96] I see you on my YouTube feed all the time these days, I think.
[974.58 → 982.00] You and Hardware Haven and Two Guys Tech, some up-and-coming Home lab YouTubers to watch there for sure.
[982.12 → 989.82] But one thing that really caught my eye was your $200 Home lab challenge series that you did with Hardware Haven.
[990.50 → 991.92] I thought that was fascinating.
[992.04 → 993.28] Do you want to talk about that briefly?
[993.74 → 998.06] Yeah, so Colton from Hardware Haven came to me, and he was like,
[998.06 → 1007.02] Hey, what do you think about something like a Scrapyard Wars type thing like LTT did back in the day?
[1007.82 → 1008.70] I was like, yeah, I'm down.
[1008.70 → 1014.88] So we went back and forth deciding how we want to do this and eventually settled on, you know, we have $200.
[1015.70 → 1020.70] Let's create the ultimate...
[1020.70 → 1024.70] I say ultimate, it's a little bit of sarcasm, but the ultimate Home lab.
[1024.82 → 1026.00] So what can you do with $200?
[1027.00 → 1033.98] Went back and forth on how to make it, you know, interesting rather than just saying here's $200, you know, go build, whatever.
[1033.98 → 1037.46] So we incorporated, we had this little wheel to spin.
[1037.58 → 1041.12] So every week we'd check in, and we'd have to spin this wheel to give ourselves a challenge.
[1041.78 → 1047.12] He got hit with like, he had to build his own case.
[1047.92 → 1051.06] He had, I think he had some ones that were actually good.
[1051.84 → 1055.62] He got like $10 added to his budget like straight off the bat.
[1056.06 → 1057.16] I got hit with that.
[1057.16 → 1059.12] I had to use an off-the-shelf NAS.
[1059.62 → 1062.68] I had to use ZFS in my build.
[1063.68 → 1070.10] What I thought was interesting was you guys bought parts and then some other piece of the jigsaw didn't quite land as you expected.
[1070.22 → 1072.80] So then you resold the part and bought something else.
[1073.36 → 1073.76] Yeah.
[1074.22 → 1075.24] That was fascinating.
[1075.62 → 1075.82] Yeah.
[1075.88 → 1084.58] I think me and Colton both ran into something similar to that where I also, my math was butt cheeks.
[1084.58 → 1089.36] And I somehow couldn't do basic math.
[1089.94 → 1094.10] So while I'm editing, I'm like saying, this is how much I have left.
[1094.12 → 1095.26] And I'm like doing the math.
[1095.78 → 1098.58] And I'm like, wait, that's not how much you have.
[1098.88 → 1105.74] So at the end I was like, I had, I went over too much, and then I had to sell the part and go back and buy the cheaper version.
[1105.74 → 1108.06] And it was just, it was fun.
[1108.86 → 1112.36] Me and Colton have talked about if we do it again, there are some changes we'd like to do.
[1112.36 → 1116.50] I think the wheel was a fun thing, but we do it all at the beginning.
[1117.02 → 1117.10] So.
[1117.58 → 1117.66] Yeah.
[1117.68 → 1119.00] The wheel was really fun.
[1119.64 → 1121.88] We're talking like a wheel of fortune style.
[1122.44 → 1123.74] Must use ZFS.
[1123.94 → 1124.06] Yeah.
[1124.06 → 1127.34] Like land, spin the wheel, land on certain things you must do as part of it.
[1127.36 → 1127.56] Yeah.
[1127.82 → 1129.10] I think we just do it all at the beginning.
[1129.10 → 1135.52] So we'd have kind of like a handful of challenges to work with over the course of, you know, two weeks instead of.
[1136.16 → 1145.04] Cause there were certain things like, you know, if you're on the last week of the challenge, and you get hit with like must use off the shelf mass, and you already have your stuff built.
[1145.34 → 1146.48] You can't really do it.
[1146.58 → 1148.02] So we'll see.
[1148.02 → 1148.42] Yeah.
[1148.50 → 1161.44] Well, I'd say what, what would be fun is just to do something like that at a convention or something where people have got transportation, and you're in a big city and there's a few Linux nerds around and like, what can you build for 200 bucks in a weekend?
[1161.64 → 1164.84] And there are five teams, and you know, that could be really fun.
[1164.84 → 1167.22] I was thinking, yeah, funny you say that.
[1167.24 → 1179.10] Because I was thinking I was at CES this year, and I was like, man, the challenge would be very comical if it happened during CES where I was out there with thousands and thousands of others.
[1179.16 → 1182.02] Who could you, who could you sweet talk at a booth to give you free stuff?
[1182.02 → 1182.08] Yeah.
[1182.44 → 1182.70] Yeah.
[1182.80 → 1183.50] That's it.
[1183.68 → 1184.42] That would have been funny.
[1184.72 → 1186.28] I've arrived with a Lamborghini.
[1186.40 → 1186.70] Yeah.
[1186.70 → 1196.78] I turned 200 bucks into this Lamborghini home server that's sponsored by Lamborghini.
[1197.48 → 1197.94] Well, very good.
[1198.06 → 1199.66] Thank you very much for joining us, Brett.
[1199.74 → 1201.10] It was an absolute pleasure to have you.
[1201.44 → 1203.48] Is there anywhere in particular you'd like to send folks?
[1204.40 → 1215.22] Just if you want to watch some Home lab content, some networking, hardware, just general Home lab stuff, go check me out.
[1215.22 → 1217.06] Raid Owl on YouTube.
[1217.40 → 1224.64] And if you're on Twitter or X these days at Raid Owl tweets, I'm over there as well posting.
[1225.00 → 1228.02] So if you like that, check it out.
[1228.62 → 1231.48] But I appreciate you guys for, appreciate you guys for, for having me on.
[1231.80 → 1232.40] It's super fun.
[1232.60 → 1234.70] I love nerd out with Home lab stuff.
[1234.84 → 1236.04] So this was awesome.
[1236.48 → 1236.56] Yeah.
[1236.58 → 1237.26] Thanks for coming on.
[1237.54 → 1237.92] Thank you, sir.
[1237.92 → 1242.96] Tailscale.com slash self-hosted.
[1243.04 → 1248.16] Head on over to Tailscale.com slash self-hosted and get 100 devices for free while you're supporting the show.
[1248.70 → 1253.98] Tail scale is the easiest way to connect your devices and your services directly to each other wherever they are.
[1254.04 → 1260.08] Even if you have a complex network with some things behind NAT, some things up on a VPS, maybe you have a mobile device in the mix.
[1260.18 → 1264.66] Tail scale brings it all together, protected by WireGuard's noise protocol.
[1264.66 → 1265.98] It's easy to deploy.
[1266.36 → 1270.54] It's essentially zero config, and you can get up and running in just minutes.
[1270.68 → 1274.16] Try it out for 100 devices and just see what I'm talking about.
[1274.22 → 1276.60] Put it on a couple devices and see why I love it so much.
[1276.80 → 1280.84] You can build simple networks, even if you have devices all over the world.
[1281.12 → 1284.88] You can save time with a proven security solution that just works.
[1285.28 → 1292.12] So if you're in an enterprise environment, and you're struggling with VPN solutions right now or remote access solutions,
[1292.12 → 1295.00] I have seen every kind of incarnation in enterprise.
[1295.92 → 1297.88] Tail scale can dramatically simplify that.
[1298.40 → 1302.72] There's also nice little aspects of Tail scale that make it really slick to use once you start to learn it.
[1303.00 → 1309.62] What you realize after using Tail scale for a while is it's really just a way for devices to communicate securely directly to each other.
[1310.06 → 1313.56] Something the internet should have done for us a long time ago, but has never done right.
[1313.98 → 1318.04] And Tail scale will punch through all the different places to make it happen and make it smooth.
[1318.04 → 1325.38] For example, if you have two Tail scale devices on the same LAN, they know that, and they just talk directly to each other.
[1325.44 → 1328.62] So you're going to get line speed there essentially because the Tail scale overhead is minimal.
[1329.44 → 1333.94] But if you've got a device that moves like a laptop and maybe now it's at your work, it'll still connect.
[1334.10 → 1336.56] And they'll still talk to each other like they're still on the same local LAN.
[1336.96 → 1338.26] It's secure. It's fast.
[1338.80 → 1343.04] And one of the benefits is they have it for so many different platforms.
[1343.04 → 1352.78] So if you're a Linux user, a Mac user, Windows user, ARM, Intel, if you're on a mobile device, if you have an appliance, you'd be amazed what there's Tail scale apps for and where there isn't an app.
[1353.34 → 1356.32] They have the ability to do subnet routing and things like that.
[1356.88 → 1360.72] Listeners use things like the Apple TV or Raspberry Pi just as a dedicated subnet router.
[1361.02 → 1362.42] It's really handy.
[1362.90 → 1364.72] So go try it out for free on 100 devices.
[1364.96 → 1368.92] Support the show and go to tailscale.com slash self-hosted.
[1368.92 → 1373.10] Simple secure networks for teams of any scale built on top of WireGuard.
[1373.46 → 1378.78] A zero config VPN that you'll get up and running in just minutes and will change the way you network.
[1379.10 → 1380.26] It definitely has for us.
[1380.72 → 1383.68] Tailscale.com slash self-hosted.
[1385.62 → 1393.74] So listener Joe writes, I wanted to bring to your attention that the Unpaid CEO and now his daughter also has joined in.
[1393.74 → 1403.90] I know Alex is a former Unpaid user, but frankly, since they've added ZFS and have added several other new staff, it's rapidly becoming a different and much more mature product.
[1404.46 → 1408.94] They're making a transition to be a proper grown up company, not just for hobbyists.
[1409.48 → 1412.00] They've also acquired a bunch of staff from iX Systems.
[1412.48 → 1415.60] It's evolving into a truly different tier product, in my opinion.
[1416.02 → 1421.68] And especially as version seven will be coming out soon, I think it deserves basically fresh eyes.
[1421.68 → 1427.66] Tom the founder has an interesting Linux story in general that's told here if you want to watch and listen to the full session.
[1428.42 → 1432.74] I'll put a link to the interview referenced in this comment, by the way, in the show notes down below.
[1432.88 → 1433.94] It's an Unpaid podcast.
[1434.18 → 1435.44] It's actually pretty good.
[1436.50 → 1444.38] At the 45-minute mark, they are talking about this bigger pivot in, and I'm talking about here, the licensing changes that we'll get into in just a second.
[1444.94 → 1447.78] They're going along the lines of elementary OS.
[1447.78 → 1453.78] Lower entry price and then pay for updates and enhancements when and if you want to stay current.
[1454.24 → 1458.56] And with the highbrow grandfathering option for all existing license holders.
[1459.42 → 1472.56] Then they get into new features for version seven, rounding out the full suite of ZFS support and several very new and interesting options that I think you will both find interesting, especially, Alex, with your cross-continental needs.
[1472.56 → 1479.80] We're talking an API for things like Home Assistant, multiserver options, porting shares across different servers and users.
[1480.02 → 1484.86] It feels to me like a Linux company done right, sustainable in the right way.
[1485.46 → 1492.16] As I'm sure they could wave a finger and have venture capital money anytime they wanted, but specifically have issued that option.
[1492.16 → 1502.38] So we are, of course, talking about the licensing changes to Unpaid that happened this week, essentially moving to a subscription model for updates.
[1503.22 → 1507.70] And it seems they're going to have a starter, unleashed, and lifetime license type.
[1507.86 → 1509.08] So three different types there.
[1509.08 → 1517.12] But I think I do have to acknowledge the move to grandfathering existing license holders so they have a lifetime update guarantee.
[1517.82 → 1520.00] That bodes well for this transition.
[1520.18 → 1528.28] And I think it's a smart, savvy move because it creates a loyal, passionate base that could go advocate the product to other people instead of starting on a bad note.
[1528.82 → 1530.10] We've seen it many, many times.
[1530.30 → 1537.10] I mean, Plex is the perfect example of a lifetime pass that isn't really a sustainable model.
[1537.10 → 1543.50] I mean, if you bought an Unpaid license, I mean, you could legitimately have bought one 15 years ago at this point.
[1544.24 → 1548.72] Tom and Lime Tech haven't seen another penny from you since.
[1548.96 → 1558.78] And they've still been working, adding stuff, as we've seen adding new features, pretty impressive ones, like dual parity support, ZFS, a bunch of other stuff.
[1559.18 → 1563.48] And it's really quite a good product these days for most people.
[1563.48 → 1567.92] There are still some things that I find a bit peculiar, but maybe Joe has a point.
[1568.26 → 1572.14] I haven't actually used Unpaid now, getting on for seven or eight years.
[1572.24 → 1575.28] So it probably is worth some more attention from us moving forward.
[1575.68 → 1582.02] And I think for me, just the way in which this whole thing has been handled has actually been pretty good, pretty classy.
[1582.02 → 1586.68] Grandfathering in all existing customers for lifetime updates.
[1587.74 → 1599.00] I mean, you're losing out on a huge chunk of what could be potential revenue there if you wanted to, you know, play the asshole and say, right, if you want updates, we're going to give you three more years or something.
[1599.18 → 1599.56] I don't know.
[1599.90 → 1603.26] And then after that, we're going to start charging you the same as everybody else.
[1603.34 → 1604.68] But no, this is a lifetime thing.
[1604.68 → 1609.98] And it's a really nice way of rewarding the people that put Unpaid in the position that they're in now.
[1610.28 → 1615.74] And I would think if it's true that they have some IX staff working for them, perhaps they have enterprise ambitions.
[1616.16 → 1619.04] And that's a much, much larger, much more lucrative market.
[1619.28 → 1621.80] So if they're playing the long game here, it would make sense.
[1622.32 → 1623.56] I've been quite surprised, actually.
[1623.64 → 1625.18] Now I've left the red hat umbrella.
[1625.72 → 1627.40] Just how many folks are running Unpaid?
[1627.66 → 1630.16] I'm speaking to engineers all the time from different companies.
[1630.16 → 1631.52] And they're like, oh, does it run on Unpaid?
[1631.66 → 1633.08] You know, talking about Tail scale, of course.
[1633.08 → 1642.36] And it's a really popular product amongst not just home libbers, but developers and people that just want to store stuff in their house.
[1642.50 → 1648.96] You know, it's kind of my ESXi argument that, you know, you start with deploying it in your home lab.
[1649.16 → 1650.04] You use it.
[1650.20 → 1652.40] You create your own network effect with it.
[1652.52 → 1658.80] And then it's sort of like the bring your own device effect at work when the workplace starts looking for a solution.
[1658.80 → 1665.38] Well, if you've got something employees are already familiar with, does the job and meets your requirements, that's a pretty big win.
[1665.44 → 1667.62] And I suppose Unpaid fell into that category.
[1668.34 → 1678.04] Isn't it weird that in the same episode, we've got VMware pulling the rug and Unpaid almost doubling the thickness of it.
[1678.40 → 1683.18] You know, like they're making the company guaranteed sustainable by doing this.
[1683.18 → 1695.34] So those people that have the grandfathered licenses should be, in my opinion, probably pretty happy about this because all the new people that come along are going to be supporting the development of features for them.
[1695.82 → 1700.88] You know, so it doesn't really affect them in the long run other than making the product more sustainable.
[1700.88 → 1704.60] And I think there is a market fit.
[1704.88 → 1712.18] When I was in IT, the small business that had 50 employees or so, you know, they needed centralized storage.
[1712.30 → 1714.18] They wanted to run a couple of applications.
[1714.98 → 1717.54] There wasn't a great solution.
[1717.70 → 1720.36] And Free NAS was one of the good alternatives out there.
[1720.90 → 1722.64] But I think Free NAS could use a competitor.
[1722.96 → 1726.88] I think the market's right for a good competitor to a True NAS, Free NAS category.
[1726.88 → 1730.88] And Synology's have been pretty successful in this category, too, in small business.
[1731.82 → 1733.94] So, yeah, we could see it.
[1733.98 → 1739.60] I think, you know, maybe our friends over at 45 Drives are trying to kind of get there with that kind of stuff, too.
[1739.64 → 1745.18] But I think Unpaid, with the network they already have, probably has one of the best shots.
[1745.66 → 1749.06] I don't know why more people aren't going after this market segment, to be honest with you.
[1749.34 → 1750.20] Maybe we should.
[1751.00 → 1752.32] Maybe we should start a company.
[1752.32 → 1767.48] But there honestly must be quite a lot of people that want to store data without having to learn the inner workings of how you grow a neck beard, you know, and do ZFS properly, dare I say.
[1767.72 → 1769.92] Air quotes from gatekeeping when I say properly.
[1770.60 → 1775.00] Or learn Cash FS or Butters or whatever the latest hotness is.
[1775.20 → 1781.76] They just want to click a button, click some shares, and forget about it for three years until they add a new disk or something pops, you know.
[1782.62 → 1784.24] And Unpaid fits that bill perfectly.
[1784.34 → 1790.64] Well, what I find interesting as well is that this licensing model actually follows that of Blue Iris pretty closely.
[1791.48 → 1795.98] I think I end up paying about $35-ish per year to Blue Iris now.
[1796.50 → 1802.74] And every time I sort of think about it when the renewal comes up, I'm like, oh, yeah, I've been running Blue Iris for another year.
[1802.88 → 1804.04] I haven't really thought about it.
[1804.06 → 1804.76] I haven't touched it.
[1805.00 → 1808.38] And that, for a lot of people, is exactly what they want from an appliance.
[1808.76 → 1811.06] And for a lot of people, that's what Unpaid is.
[1811.06 → 1819.04] Yeah, I heard from a lot of listeners who adopted Unpaid, too, because they made it really easy to do VM hardware pass-through for certain setups.
[1819.36 → 1820.54] And that was really attractive to them.
[1820.78 → 1820.96] Yeah.
[1821.20 → 1825.88] Yeah, back in the day, that was actually one of the things that got me into Linux in the first place.
[1825.92 → 1827.30] I was running an Unpaid box.
[1827.56 → 1828.96] I mean, I've told this story on the show before.
[1829.06 → 1829.88] I'm certain of it.
[1829.88 → 1835.52] But I was running an Unpaid box, and I wanted, because I was a poor student at the time, I couldn't afford a desktop.
[1836.00 → 1838.12] I could afford a GPU on its own, but not both.
[1838.86 → 1846.08] So I shoved the GPU into my server and started compiling Unpaid on top of Ubuntu kernels and stuff.
[1846.08 → 1858.60] And eventually, sort of, in that whole mess, helped push the envelope forward a little bit, in some small way anyway, to adding that feature into Unpaid.
[1858.64 → 1861.54] I'm not going to claim credit for doing all the work, because Lime Tech did that.
[1861.68 → 1866.16] But it was definitely something that got me into Linux in the first place.
[1866.16 → 1877.22] I just find it such a fascinating idea that you can take a piece of hardware and make the virtual machine think that it's not a virtual machine, and it's a real, I'm a real boy, you know?
[1877.84 → 1878.06] Yeah.
[1878.38 → 1880.42] That's just so cool to me.
[1880.56 → 1880.82] It is.
[1881.18 → 1882.06] No, it totally is.
[1882.58 → 1882.94] Well, okay.
[1883.04 → 1888.40] Well, seems like maybe there is some rug pulling going on over at F5, potentially.
[1888.40 → 1898.70] The core NGINX developer has forked the project into free NGINX, claiming that there's been shenanigans going on over there at F5, and they're not really taking his advice anymore.
[1898.78 → 1911.32] Now, this is an interesting situation, because, see, F5 closed, F5, who's got an office here, where I live, closed their Moscow office in 2022, and severed their relationship with the core developer of NGINX,
[1911.32 → 1918.68] but then kept him on kind of as some kind of contractor with an agreement that he'd have oversight of the project and certain development things.
[1919.26 → 1926.00] But it seems like F5 has started to proceed and make changes that he hasn't approved and doesn't agree with.
[1926.50 → 1927.02] And he writes,
[1927.02 → 1930.44] As such, starting from today, I'll no longer participate in NGINX development.
[1930.56 → 1944.68] As run by F5, instead, I'm starting an alternative project, which is going to be run by developers and not corporate entities, at freeginx.org.
[1944.82 → 1945.88] We'll put a link in the notes.
[1946.08 → 1947.84] But what's your reaction, Alex?
[1948.28 → 1951.06] To some degree, it was inevitable, wasn't it?
[1951.80 → 1954.94] Big corporate entity buys free and open source project.
[1954.94 → 1958.94] The goals of those two entities are at odds with one another.
[1959.36 → 1970.68] And so at some point in the future, unless they have some unicorn leadership that fully understands both the corporate world and the open source world,
[1970.78 → 1979.82] as someone who gave up part of their life to create a project like NGINX does, there's going to be some disagreement at some point.
[1980.60 → 1981.68] It's just reality.
[1981.68 → 1985.10] Yeah, I'm just not clear how and where things go now.
[1985.22 → 1987.08] Does the community start using this?
[1988.06 → 1993.86] Amazon and the other big cloud providers that have all of their code based on NGINX rebase?
[1993.94 → 1995.54] Or do they keep using the F5 version?
[1996.34 → 1998.04] Where does the innovation happen at now?
[1998.84 → 2002.12] What does this mean for home libbers that use it for reverse proxy long term?
[2002.60 → 2004.84] I think it means nothing for a short term.
[2005.04 → 2006.48] It really doesn't mean anything short term.
[2006.62 → 2008.42] And it is consequential long term.
[2008.64 → 2009.42] It's fascinating.
[2009.42 → 2015.54] You wonder about the tectonic plates underneath acquisitions like this all the time, don't you?
[2015.58 → 2019.86] The things that bubble away really slowly in the background that nobody pays attention to.
[2019.96 → 2022.70] So the slow undercurrents of change.
[2023.42 → 2026.88] And eventually there's an earthquake and all hell breaks loose for a little bit.
[2026.96 → 2027.86] And then it settles down again.
[2028.06 → 2031.64] So yeah, it'll be interesting to see where this one settles.
[2032.60 → 2035.66] Zach wrote in with an audiobook pick.
[2035.66 → 2041.98] This is one that's of particular interest to me because my wife, actually we ended up going to our local library this week.
[2042.06 → 2044.24] There was a kid's craft corner.
[2044.38 → 2051.52] So we took Ella to the library, and she was cutting out shapes and sticking them on paper and having a wonderful old time.
[2051.62 → 2055.84] But while she was doing that, I sort of wandered around the library and had a look at various sections.
[2055.84 → 2062.04] And it turns out there are audiobooks on CDs in the corner of my local library.
[2062.04 → 2069.86] So I whipped out my library card and rented, borrowed, rented, borrowed, checked out.
[2070.10 → 2070.92] Yeah, checked out.
[2071.14 → 2077.10] Margaret Atwood Testaments audiobook, which is on like 14 CDs.
[2077.62 → 2078.74] 14 CDs?
[2079.26 → 2082.58] I'd forgotten how tedious ripping 14 CDs was.
[2083.22 → 2084.04] Oh my gosh, yeah.
[2084.12 → 2084.52] One CD.
[2084.58 → 2085.82] I'm like, not so bad, right?
[2085.86 → 2086.14] Yeah.
[2086.28 → 2088.34] Why don't they just put it on a DVD for goodness’s sake?
[2089.06 → 2090.20] I guess it's for cars, maybe.
[2090.30 → 2091.28] But yeah, so you ripped it.
[2091.28 → 2093.84] I'm not an expert at ripping audiobooks, okay?
[2094.14 → 2099.16] I'm good at stripping DRM from Audible books, but I haven't actually ripped a CD in a very long time.
[2099.72 → 2099.98] Yeah.
[2100.30 → 2109.46] So I fired up my Windows desktop and opened up Windows Media Player and clicked the Rip CD button like it was 2005 all over again.
[2109.62 → 2110.68] That's how you did it?
[2110.76 → 2111.76] Oh my goodness.
[2112.72 → 2117.42] So what, did it put them in WMA files or anything funky like that?
[2117.44 → 2118.66] Oh, you can select the codex.
[2118.78 → 2120.62] You know, it's pretty advanced stuff, Chris.
[2120.62 → 2124.26] It's like I could select my bit rate up to 320K and MP3.
[2125.00 → 2125.60] Oh yeah.
[2126.34 → 2130.64] Even the encoders even support flack in Windows Media Player these days.
[2130.90 → 2131.20] Wow.
[2131.40 → 2132.00] Credit to them.
[2132.12 → 2132.36] Okay.
[2133.36 → 2134.40] So, wow.
[2134.60 → 2136.78] What a solid husband move on your part.
[2136.90 → 2137.60] 14 disses.
[2137.60 → 2138.92] Well, I thought so too.
[2139.06 → 2141.34] I'm actually waiting my Nobel Prize in the mail.
[2141.68 → 2143.14] I think it'll be here any day now.
[2144.34 → 2146.94] But coming back to the actual topic, audiobooks.
[2146.94 → 2153.68] I thought it was pretty interesting because, you know, I've mentioned on the show that I still run Plex only for music.
[2154.18 → 2158.12] Preamp, by the way, I think might be the greatest music app ever made.
[2158.24 → 2161.10] I am absolutely falling in love with Preamp.
[2161.16 → 2170.38] I've done a bunch of work to my home office and put my Keels 50s up, and I'm listening to music again, not just sort of passively in the same.
[2170.38 → 2172.86] I'm listening and my flack farts.
[2172.96 → 2173.82] Anyway, I digress.
[2174.30 → 2175.14] Audiobooks again.
[2177.58 → 2180.32] Zach wrote in with a pic called Plasma.
[2180.56 → 2182.16] P-L-A-P-P-A.
[2182.72 → 2185.24] And he says, I've got a find here that may be interesting.
[2185.24 → 2193.92] It's an early test flight version of an iOS app for audiobooks which uses Jellyfin as the back-end server.
[2194.42 → 2194.82] All right.
[2194.92 → 2198.50] So, this would be similar to like a prologue is to Plex.
[2199.22 → 2199.70] Correct.
[2199.70 → 2208.80] Now, what's particularly interesting is if you look at the roadmap on the GitHub page, first, it says the first option is an iOS app with all the basic features.
[2209.06 → 2209.32] Check.
[2209.90 → 2211.64] Next up is CarPlay support.
[2212.04 → 2213.38] Not checked, but coming.
[2213.82 → 2215.00] Then an Apple Watch app.
[2215.14 → 2215.86] Then a Mac app.
[2215.96 → 2216.98] Then an Apple TV app.
[2217.54 → 2219.44] How many people listen to audiobooks on their Apple TV?
[2219.98 → 2224.86] I don't know, but it's written in Swift, so I assume the lift of putting it on those different platforms.
[2225.50 → 2228.22] When I saw that, I thought, you know, chores, right?
[2228.22 → 2229.06] And if it's synced.
[2229.34 → 2229.66] Maybe.
[2229.76 → 2233.56] If it uses iCloud, which it looks like it syncs playback status via iCloud, it says.
[2234.00 → 2237.62] So, you could listen on your car and then say you want to do some charging.
[2237.62 → 2240.20] And you bring it up on your old Apple TV.
[2240.32 → 2242.66] Since you're all in on the Apple ecosystem, you've got the HomePods.
[2243.22 → 2245.74] So, then you long press on the button on the Apple TV remote.
[2245.84 → 2252.90] You send it to all your HomePods throughout your whole house, synchronized audio playback, controlled by your Apple TV that you can play and pause from your Apple Watch as you move about.
[2253.14 → 2253.42] Boom.
[2253.66 → 2254.16] There you go.
[2254.24 → 2254.88] Living the dream.
[2254.88 → 2257.28] Now, the Apple ecosystem dream.
[2257.62 → 2258.22] Clapper.
[2258.58 → 2259.66] Is it Clapper?
[2259.78 → 2260.32] I think it is.
[2260.66 → 2267.38] Is currently in closed test flight beta and its public release is set for early 2024.
[2267.86 → 2269.42] So, any day now.
[2269.94 → 2274.76] But what excites me the most on this roadmap is the last item.
[2275.08 → 2275.76] Do you see that?
[2276.18 → 2280.26] It says support for audio bookshelf servers.
[2280.76 → 2282.06] Oh, now we are talking.
[2282.06 → 2283.34] Now we're talking, right?
[2283.34 → 2284.06] Now we're talking.
[2284.88 → 2286.16] That's the box I want checked.
[2286.80 → 2288.10] Oh, an Apple Watch app too.
[2288.34 → 2291.14] You know, there is something really sweet.
[2292.00 → 2296.02] You know, it is actually kind of nice to see the Apple ecosystem get some self-hosting love.
[2296.08 → 2299.06] Because it feels like, really, it's all the funds for the Android users.
[2299.14 → 2299.92] But this is really neat.
[2300.02 → 2301.76] This is like the screenshots alone.
[2302.54 → 2304.20] I'm blown away by the design of the app.
[2305.30 → 2307.92] I could immediately see spousal approval with this app.
[2308.18 → 2309.16] It looks beautiful, doesn't it?
[2309.40 → 2309.62] Yeah.
[2309.86 → 2310.04] Yeah.
[2310.04 → 2311.08] It's really well done.
[2311.08 → 2318.54] If Leo Klaus, the developer, is listening and wants to have us do a test flight test, I think Chris and I will be game.
[2318.78 → 2319.08] Absolutely.
[2319.08 → 2319.16] Absolutely.
[2319.64 → 2329.80] And also, if you would like very, very, very enthusiastic audiobook listeners who are average users, but still quite sharp, the wife's.
[2330.26 → 2331.30] They could do a bug report.
[2331.52 → 2335.88] They'll listen to five books in a week, and they'll tell you how it's working.
[2336.02 → 2336.18] I mean.
[2336.42 → 2337.02] You know it.
[2337.02 → 2339.46] Now, my wife, actually, just a quick plug for her thing.
[2339.62 → 2342.58] It's just like her version of journaling.
[2342.74 → 2346.28] She's actually started writing a blog at Perfect Prose.
[2346.40 → 2347.90] There'll be a link to that in the show notes.
[2348.50 → 2350.64] She wants to read at least one book a month.
[2351.32 → 2355.86] And she's, for the whole time I've known her, has been an absolutely ferocious reader.
[2356.52 → 2360.10] But since Ella came along, obviously finding time for that kind of thing has been more tricky.
[2360.10 → 2364.50] So she's going to try and read a book a month, write a little review on the blog.
[2364.88 → 2369.90] And if that kind of thing floats your boat, there's an RSS feed and there'll be a link in the show notes.
[2372.48 → 2375.24] Trustebook.com slash self-hosted.
[2375.80 → 2377.94] Trustebook.com slash self-hosted.
[2378.28 → 2386.48] This is a simple, easy to use workbook that lets you take your digital records, your digital legacy, all of your important digital stuff, take it offline.
[2386.48 → 2390.20] And it's really simple to get started with a great interface.
[2390.30 → 2395.68] And if you go to trustebook.com slash self-hosted, you'll take $10 off while you're supporting the show.
[2395.88 → 2400.26] Yeah, you can now create hard copies of your most important online information.
[2400.58 → 2404.58] This is just great for continuity planning for a family or a business.
[2405.04 → 2406.94] But I think it's also peace of mind.
[2407.10 → 2411.08] Once you have this stuff documented, you're not quite as dependent on that cloud service.
[2411.08 → 2414.98] And we'd all love to self-host absolutely 100% everything.
[2414.98 → 2417.34] But you have bank account information.
[2417.46 → 2420.70] There's just accounts you're going to have online that you need to have documented somewhere.
[2420.80 → 2424.16] So the idea with Rulebook is you download and use it offline.
[2424.24 → 2427.34] So that way you feel confident that your information is staying private.
[2427.92 → 2428.72] It's all on your system.
[2429.34 → 2433.98] The user-friendly design makes it super easy to pick out what you need and prepare for potential disaster
[2433.98 → 2438.58] just to be absolutely ready to go in case maybe you're travelling, and you want hard copies of your stuff.
[2438.70 → 2444.08] There are so many different reasons to get this information documented, but there hasn't been a great way to do it.
[2444.08 → 2447.14] Now Rulebook is stepping in to fill that.
[2447.52 → 2455.62] So try it out while you support the show and use the promo code self-hosted or go to trustebook.com slash self-hosted and get $10 off when you purchase it.
[2455.90 → 2459.94] Simple, easy-to-use workbook that helps you take control of your digital legacy.
[2460.46 → 2461.24] Go get started today.
[2461.66 → 2462.54] Take the $10 off.
[2462.94 → 2463.54] Support the show.
[2464.04 → 2465.10] Trustebook.com.
[2465.34 → 2468.82] That's trustebook.com slash self-hosted.
[2468.82 → 2475.20] This is perhaps the least surprising news story of 2024.
[2476.04 → 2488.70] Waze have confirmed, and I'm talking about Waze cameras here, have confirmed at least 13,000 owners' video was able to be viewed through an unauthenticated or unintended viewer.
[2488.70 → 2488.78] Yeah.
[2490.14 → 2495.50] 13,000 Waze camera owners saw thumbnails from other users' video feeds.
[2496.16 → 2500.50] 1,504 users tapped on those and actually viewed the feeds.
[2500.66 → 2500.84] Yeah.
[2501.62 → 2508.12] Waze writes, the incident was caused by a third-party caching client library that was recently integrated into our systems.
[2508.12 → 2516.46] This client library received an unprecedented load condition caused by devices coming back online all at once because there was a data centre outage, I guess, or something.
[2516.84 → 2524.92] As a result of the increased demand, it mixed up device ID and user ID mapping and connected some data to incorrect accounts.
[2525.86 → 2527.80] I'm struggling to even understand how that happens.
[2527.92 → 2534.88] I could understand something getting DDoSed, but how it starts mixing and matching device and user IDs?
[2534.88 → 2538.22] I struggle to understand how that's possible, but...
[2538.22 → 2541.18] Yeah, it must just be a really poorly written back end, honestly.
[2541.42 → 2550.00] Yeah, they say they've written their systems about bypass caching checks on user devices and certain client libraries until it's been stress-tested for extreme events like we experienced.
[2550.62 → 2560.18] Yeah, Waze are in the fool me once stage of companies now, and I think if they're not on your do not buy list, if you already have some, it might be a bit different.
[2560.18 → 2565.64] But if you're thinking about buying some new ones, it might be prudent to look at some other options.
[2566.12 → 2568.84] If your account was affected by this, they do email you.
[2568.92 → 2573.06] There's like a sentence in there that tells you if your account was impacted or not.
[2573.26 → 2574.26] So you don't have to worry.
[2574.38 → 2578.84] They are particularly specific, but you just have to read all the email.
[2579.68 → 2580.34] Not ideal.
[2581.10 → 2581.64] Hey, look at that.
[2581.68 → 2584.62] We made it all the way to the boosts without mentioning Tail scale once.
[2585.24 → 2585.82] Go us.
[2586.00 → 2586.98] Hey, look at that.
[2587.06 → 2587.92] Hey, look at that.
[2587.92 → 2593.02] Now we got a baller boost from A.A. Ron, and he mentions Tail scale.
[2593.26 → 2594.08] Yeah, I know.
[2595.60 → 2601.52] He says, I recently dove into Tail scale, and now I will never do networking the same again.
[2601.62 → 2603.02] It's unbelievably simple to use.
[2603.10 → 2606.04] I was curious about how Chris got his Jellyfin domain name working, though.
[2606.52 → 2612.76] When I use HTTP colon slash Jellyfin, it fails randomly when loading content, but using the IP succeeds every time.
[2613.34 → 2615.02] P.S. I'm curious to see how you pronounce the city.
[2615.50 → 2617.22] The name of my zip code, hint, it is German.
[2617.22 → 2618.40] Oh, no.
[2618.58 → 2618.94] Great.
[2619.38 → 2624.32] Well, the thing with Jellyfin in particular is that the clients do not like plain HTTP.
[2624.88 → 2625.00] Yeah.
[2625.28 → 2628.46] They really, really want you to have a TLS certificate.
[2628.76 → 2632.16] So I would put money on that being the issue here.
[2632.36 → 2633.78] You know, and of course, that means you need DNS.
[2634.00 → 2635.42] There are a couple of ways you could do that.
[2635.42 → 2641.70] But the really kind of clunky way is you can point a public DNS name at a private Tail net IP.
[2642.02 → 2644.38] It will never resolve unless you're on your Tail net.
[2644.88 → 2648.38] But if something's checking its name, well, that might work.
[2648.60 → 2648.80] All right.
[2648.80 → 2650.80] So you gave me your zip code here.
[2651.40 → 2651.92] It's funny.
[2652.48 → 2654.96] According to Google, it does not exist in Germany.
[2655.12 → 2656.96] You gave me the zip code for Born, Texas.
[2657.76 → 2659.98] That's what it says.
[2660.06 → 2661.02] I don't think that's probably true.
[2661.02 → 2669.90] But yeah, it says it's the city of Born, Texas, which has an eclectic menu of international
[2669.90 → 2674.72] and local favourites, including European and German restaurants, according to Google.
[2675.16 → 2677.76] I'm rereading the feedback here, the boost.
[2677.92 → 2682.86] And if you can pronounce the city name of my zip code, hint, it's German.
[2683.30 → 2685.02] I think that the name of...
[2685.66 → 2686.20] Oh, it's Burin.
[2686.42 → 2686.86] Burin.
[2686.86 → 2687.14] Burin?
[2687.44 → 2689.22] I think that's the challenge.
[2689.94 → 2690.54] All right.
[2690.92 → 2693.28] Well, it's B-O-R-N-E.
[2693.70 → 2694.14] No, it's not.
[2694.24 → 2696.34] It's B-O-E-R-N-E.
[2696.72 → 2696.98] Yes.
[2697.64 → 2698.50] How would you say it?
[2698.88 → 2699.26] Burr.
[2699.96 → 2701.64] I'd say Antares.
[2702.04 → 2702.78] That's how I'd say it.
[2703.22 → 2703.58] Burr.
[2703.78 → 2705.04] I remember back in the day.
[2705.90 → 2707.80] That's a tricky one, actually.
[2707.96 → 2707.98] Burr.
[2709.00 → 2710.46] How would a German say it?
[2710.92 → 2711.24] Burr.
[2711.32 → 2712.16] I was trying to...
[2712.16 → 2712.42] Yeah.
[2712.58 → 2712.84] Burr.
[2712.98 → 2713.58] I don't know.
[2714.04 → 2714.76] I don't know.
[2715.30 → 2716.18] I was just trying to...
[2716.18 → 2718.22] If you know, please write in.
[2718.30 → 2718.98] That one's hilarious.
[2719.40 → 2719.68] Yeah.
[2719.84 → 2722.02] That's not my best work.
[2722.14 → 2723.26] I'm going to be honest with you.
[2723.84 → 2725.80] I'm trying, but it's just not my best work.
[2725.80 → 2726.60] That is a tricky one.
[2727.20 → 2727.64] It is.
[2727.68 → 2727.82] Yeah.
[2727.88 → 2730.48] And I like that it has eclectic menu, including...
[2730.48 → 2734.12] It is on here, too, which I never believe this, by the way, if it's anything in Texas.
[2734.68 → 2735.88] Good Thai food restaurants.
[2737.02 → 2740.94] I have never had good Thai food in Texas.
[2741.18 → 2742.06] I've had great barbecue.
[2742.54 → 2743.78] Never had good Thai food in Texas.
[2743.78 → 2745.94] According to Wikipedia, it's Burr.
[2745.94 → 2745.96] Burr.
[2745.96 → 2746.40] Burr.
[2746.40 → 2746.64] Burr.
[2747.64 → 2748.04] Apparently.
[2748.44 → 2749.12] I don't know.
[2749.30 → 2749.68] We'll see.
[2750.12 → 2750.24] All right.
[2750.24 → 2751.02] Let's see how we do with here.
[2751.14 → 2756.58] IRU comes in with two boosts coming in with 51,931 SATs.
[2756.66 → 2758.20] And the first one's a zip code boost.
[2758.38 → 2758.70] All right.
[2759.34 → 2760.66] It's from the land of Paraguay.
[2761.04 → 2761.82] I love the podcast.
[2762.08 → 2765.42] And I'm also a great fan of some show darlings like NixOS and Tail scale.
[2765.62 → 2766.68] Also Bitcoin and Lightning.
[2766.84 → 2767.92] I love you, too, Edna Mole.
[2767.92 → 2772.32] Don't you all have impressions that file sharing has stagnated?
[2772.98 → 2774.28] We have NFS and Samba.
[2774.92 → 2776.26] They're trusty, and they are old.
[2776.80 → 2778.54] And they don't really work well over the internet.
[2778.72 → 2780.02] On the other hand, there's web dev.
[2780.12 → 2782.16] It's slow, and it doesn't respect ACLs.
[2782.20 → 2784.22] And all files are owned by the web root user.
[2784.64 → 2787.76] It seems the world is perfectly happy with this.
[2787.80 → 2789.24] And no one has tried something new.
[2789.62 → 2790.90] I wouldn't say they're perfectly happy.
[2790.90 → 2800.50] I mean, stuff like InfiniBand and S3 has come along as well as a bunch of other cloud-related storage protocols.
[2801.08 → 2807.64] Because NFS and Samba didn't support ACLs, like you say, and are kind of old and a bit crusty.
[2808.02 → 2818.40] I do wish that there was like a Samba version 7 or 8, you know, that had come along with Windows 11 and gave me a real reason to upgrade things.
[2818.40 → 2824.50] But, you know, Samba being a single core is sometimes a bit of a pain.
[2825.36 → 2830.58] But, I mean, the reality is, for me and my performance here, like I've got a 10 gig network.
[2830.88 → 2833.32] I can easily saturate a 10 gig network over Samba.
[2834.16 → 2840.98] Maybe you're running a data centre where you need 100 gigs, and you need, you know, direct PCIe connections between nodes and stuff like that.
[2841.20 → 2841.38] Yeah.
[2841.72 → 2847.22] I mean, I take his point, though, just like sharing files over the internet definitely stinks.
[2847.22 → 2849.84] Like you're always using some sort of way to link.
[2850.78 → 2854.00] Like Synching solves it on a smaller scale for individuals.
[2854.30 → 2857.62] I have my own little Synching empire that I really like.
[2858.54 → 2862.92] But, yeah, if people – this is an area I'd like to experiment with more, too.
[2862.98 → 2866.96] So people have suggestions, Boosted, and for ways to share files and sync files over the internet.
[2867.40 → 2869.42] I really have it solved for myself individually.
[2869.42 → 2875.32] You know, I'd love to see – and this is an Alex feature request to Tail scale.
[2876.14 → 2883.06] Wouldn't it be cool if you could use your own node storage as like a Tail scale file system and then just –
[2883.06 → 2883.54] Like a bin.
[2883.88 → 2884.10] Yeah.
[2884.62 → 2884.88] Yeah.
[2884.98 → 2885.64] That'd be pretty nice.
[2885.64 → 2887.20] I do use Tail scale send.
[2887.86 → 2892.60] And the thing that is nice about that, which is – it's an odd thing, but I find it very handy.
[2893.04 → 2894.64] And I don't know how it works exactly.
[2895.30 → 2896.10] I mean, I can guess.
[2896.58 → 2901.72] But I can start a transfer before I go to the box receiving it and tell that box where to save it.
[2902.30 → 2903.38] And I just love that.
[2903.96 → 2910.06] I don't have – like, you know, I can just – it'll start sending, and then I can log into the remote host when I get to it, assuming it's a long file transfer.
[2910.54 → 2912.52] And then I can just say, hey, save that file out to here.
[2912.56 → 2914.18] And it could be like halfway through the file transfer.
[2914.54 → 2915.94] It still goes to the right spot.
[2916.40 → 2916.92] I love that.
[2917.72 → 2919.50] Mc Zip comes in with 25,000.
[2919.62 → 2921.00] Sat says, I got to boost the show.
[2921.14 → 2923.86] They got me through the train rides across a rainy northern England.
[2924.66 → 2925.34] Keep it up, gents.
[2925.84 → 2927.02] Oh, you should probably read that one.
[2927.10 → 2928.84] He probably has it with an accent.
[2928.84 → 2931.12] I kind of did a half-walking with that one.
[2931.32 → 2933.72] Whenever I think of northern England, I go to one or two places.
[2933.90 → 2937.14] I either go to, like, Lancashire, like Dickie Bird, like a proper –
[2937.14 → 2937.34] Uh-huh.
[2937.54 → 2938.32] Manchurian.
[2938.44 → 2939.88] I was going to say that's not even a word.
[2940.38 → 2944.24] Like, I think of, like, a Lancashire accent or a Bradford accent.
[2944.54 → 2945.18] I'm going to need a map.
[2945.64 → 2946.24] Like, you got a map?
[2946.32 → 2947.20] I'm going to need a map of this.
[2947.52 → 2948.40] You got a dialect map?
[2948.86 → 2950.60] These places – this is the thing about England, right?
[2950.60 → 2953.20] These places are, like, 50 miles apart.
[2953.20 → 2959.34] And yet the accents could not be more different between Liverpool, Manchester, Leeds, and Grimsby.
[2959.78 → 2962.52] They're all in, like, a horizontal line across the middle of England.
[2962.64 → 2965.04] And they all sound completely different.
[2965.80 → 2969.08] You know, Clarkson sometimes drops into a northern accent in the show.
[2969.08 → 2972.58] So I'm not going to try and do one because I'm very bad at them.
[2972.70 → 2976.92] But have they got rid of the Pacers yet if you're riding trains in northern England?
[2976.92 → 2988.66] Are they still – there was this whole thing in – I think it was the 90s where they took old buses or, like, bus bodies and literally threw them on top of a train chassis.
[2988.66 → 2989.58] Yeah, sure.
[2989.72 → 2990.76] And they were called Pacers.
[2991.06 → 2997.02] And they were supposed to be temporary, but then they ended up being in service for, like, 40 years or something stupid.
[2997.16 → 2998.88] I think they were being phased out.
[2998.96 → 3000.32] I'm not sure if they have yet or not.
[3000.54 → 3001.32] Oh, I'd like to see that.
[3001.40 → 3004.50] Trains in northern England can be a little grim sometimes.
[3005.96 → 3008.06] Well, then I appreciate the boost even more.
[3008.28 → 3008.54] Thanks.
[3008.96 → 3009.38] Makes sense.
[3009.38 → 3013.62] Network Rob comes in with 20,573 SATs.
[3013.72 → 3018.04] He says, I wanted to send some value back to you guys in addition to my streams, which I always appreciate.
[3018.46 → 3022.72] I've been listening to you guys for over four years, mainly with the built-in iOS podcast app.
[3023.12 → 3028.10] I made the switch to Fountain, which 1.0 is awesome, about eight months ago once I got my Walt build up.
[3028.58 → 3031.72] The experience has been great, especially knowing that I can support you directly.
[3032.10 → 3034.80] I love self-hosting, and I always enjoyed listening to hear about new projects.
[3034.88 → 3035.64] Keep up the great work.
[3035.64 → 3041.50] I think I got the value correct for a Sega boost, 7,680.
[3042.42 → 3046.26] So together it's 19,571, but I'm not getting the Sega connection there.
[3046.54 → 3047.08] What am I missing?
[3047.50 → 3047.84] I don't know.
[3047.94 → 3051.54] What does 7,860, is that a like, Sega?
[3052.80 → 3053.66] I'll do that for you.
[3054.24 → 3054.44] Sorry.
[3054.58 → 3059.86] I do have a classic nostalgia spot for that when I hear the old Sega go off.
[3059.86 → 3066.80] We're going to talk in the post-show a little bit about a handheld gaming device that I bought about three weeks ago, just on a whim.
[3067.26 → 3070.26] It was like $38, and it's called the R36S.
[3070.96 → 3075.70] And I loaded up Sonic the Hedgehog, and as soon as I did, I heard the Sega.
[3076.18 → 3079.94] I was like, suddenly I was nine years old all over again.
[3080.04 → 3080.58] It was incredible.
[3080.58 → 3080.94] Cool.
[3081.18 → 3082.04] I love that.
[3082.30 → 3086.22] I'm done messed up, and I cut off the name for this next one, so I apologize.
[3086.46 → 3087.12] That's my bad.
[3087.22 → 3089.92] They came in, though, with two boosts.
[3090.00 → 3092.28] They had a question about Unify replacement gear.
[3092.64 → 3097.08] They're not totally dishappy with it, but they're looking for some replacement, something that can incorporate multiple brands.
[3097.80 → 3102.10] Do we have a go-to suggestion for Unify alternatives?
[3102.64 → 3105.06] Probably TP-Link Omaha is the one I see the most.
[3105.26 → 3105.52] Yeah.
[3105.66 → 3111.24] They have a similar kind of hosted control panel, control centre type deal.
[3111.50 → 3113.12] I don't think they're quite equivalent.
[3113.28 → 3115.22] I mean, it is good, though, if you don't need – yeah.
[3115.62 → 3116.62] I just don't think they're quite equivalent.
[3116.82 → 3118.34] No, I haven't used them.
[3118.34 → 3122.64] I bought fully into, about this time last year, the Unify ecosystem.
[3123.46 → 3125.64] I've honestly been very happy since I did.
[3125.64 → 3132.16] My network, since I did that whole fibre thing, has just been better than I could have ever hoped for, honestly.
[3132.46 → 3135.12] I also – I include the boost because I love this admission right here.
[3135.20 → 3137.54] It says, I boosted before bragging about my Zigbee networks.
[3137.60 → 3138.92] I'm really sorry I dropped your name off.
[3139.46 → 3144.70] It's been rock solid, but recently I had issues with two-thirds of my devices dropping off the network.
[3145.12 → 3146.36] It's happened a few times now.
[3147.14 → 3153.62] I have found that the best way to recover is just reboot my coordinator, which is Raspberry Pi, so it's just an SSH away.
[3153.62 → 3155.56] And then it all comes back in about 10 minutes.
[3155.98 → 3157.04] How do you normally recover?
[3157.54 → 3159.24] Well, I try turning it off and on again.
[3159.56 → 3160.40] Yeah, yeah.
[3160.56 → 3161.94] That's exactly what I do.
[3162.24 → 3165.02] I'll tell you what I eventually did is I just swapped them out to Z.
[3165.02 → 3167.68] The ones that really matter, I swapped them out to Z-Wave devices.
[3168.06 → 3172.60] Because I've got some that are triggering heaters, and if the heaters don't fire, my water freezes.
[3173.10 → 3173.30] Right?
[3173.34 → 3174.18] My pipes freeze.
[3174.48 → 3176.12] My batteries go below freezing.
[3176.32 → 3177.98] Like, it's just non-optional.
[3179.00 → 3181.44] So I had to go back to Z-Wave on those devices.
[3181.44 → 3188.38] But if you look at the Z-Wave, if you go into the Zigbee integration on Home Assistant, there's a visualizer where you can visualize the network layout.
[3188.90 → 3193.12] And that is handy for figuring out what devices are meshing off of each other.
[3193.26 → 3198.36] And you can usually track it down to one of the repeaters is what's giving you an issue.
[3199.04 → 3203.06] And you either need to add another repeater in the area or replace that repeater.
[3203.18 → 3208.54] Or sometimes, instead of rebooting your entire Zigbee network, you could just power cycle that one repeater.
[3208.54 → 3214.06] So any Zigbee device that is permanently powered, not always, but is generally a Zigbee repeater.
[3214.42 → 3215.58] So look at that visual map.
[3215.98 → 3217.46] See if that can help you track it down.
[3217.96 → 3223.46] Eric D boosted with 50,000 SATs with an update on his image server with Back blaze B2 storage via R clone.
[3224.12 → 3225.18] So far, he says, good results.
[3225.26 → 3231.18] I've uploaded my entire 400 gig Google Photos takeout to Image using the Image Go CLI tool.
[3231.18 → 3237.72] And it's cost me about $2 a month so far with B2 and 18 years of photos and videos, which is about 30,000 files.
[3237.84 → 3239.28] The performance has been great.
[3239.64 → 3245.16] I cached thumbnails on the local SSD, but the raw files and the transcoded videos are all on Back blaze.
[3245.54 → 3247.86] I've had zero delay opening any files, including videos.
[3247.98 → 3248.58] You can do that?
[3248.66 → 3249.82] The next step is my wife account.
[3250.28 → 3251.04] That's great.
[3251.34 → 3252.80] Well, so he must be doing it with R clone?
[3253.16 → 3253.52] Yeah.
[3253.78 → 3255.66] I mean, R clone SO.
[3256.18 → 3258.00] But the caching, that's great.
[3258.04 → 3259.24] Having local images cached.
[3259.24 → 3263.78] That's one of those moments where someone writes in, and you're like, hey, thank you for writing in.
[3263.82 → 3267.46] I've actually learned something from what you just said to us.
[3267.56 → 3275.54] I've actually got some ideas around doing some stuff with Obama, which is a self-hosted LLM, like, you know, local language model.
[3276.26 → 3278.68] Sort of like a local self-hosted ChatGPT.
[3278.94 → 3285.24] And I had an NVIDIA A4000 delivered this week, a nice, beefy machine learning GPU.
[3285.96 → 3286.70] Yeah, buddy.
[3286.70 → 3294.64] And I'm actually hoping to be able to throw my image library at this thing and see what CUBA acceleration I can do over there as well.
[3295.06 → 3297.58] Boy, if you get a chance to do that, I'd be really curious to hear how it goes.
[3297.94 → 3298.44] Yeah, me too.
[3298.72 → 3299.94] Well, thank you, everybody who boosted in.
[3299.96 → 3301.66] We're going to cut it right there just for runtime.
[3302.26 → 3306.26] We try to squeeze as many as we can in, but we do read them all, and we'll put the extras in the boost barn.
[3306.26 → 3311.66] We had 15 total boosters, and we stacked 300,970 SATs.
[3311.90 → 3314.76] If you'd like to boost in, go grab the Fountain or Pod verse app.
[3315.18 → 3321.96] We're taking in feedback for Fountain and I have a weekly meeting with the devs right now to give JB community members feedback.
[3322.20 → 3325.50] So it's a great time to try it out as we make improvements on the road to scale.
[3326.20 → 3327.54] Fountain.fm to get that.
[3327.76 → 3330.04] And then you can integrate it with the Strike app and boost away.
[3330.38 → 3331.44] We really appreciate it.
[3331.44 → 3336.26] And also don't forget, speaking of scale, meetup.com slash Jupyter Broadcasting.
[3336.48 → 3343.40] We do have lunch planned for Saturday while we are at Pasadena for the scale conference and Nixon.
[3344.04 → 3345.22] It's going to be a good event.
[3345.50 → 3346.60] I can't wait for Nixon.
[3346.82 → 3349.42] Something for me has clicked about Nix.
[3350.08 → 3361.02] Maybe, honestly, it was that episode of UP that I did with you and Was and Brent recently where we just spent the entire two hours talking about Nix basically end to end.
[3362.22 → 3363.52] Something has clicked for me.
[3363.84 → 3369.66] Like, I can actually, I feel maybe a bit like Tank in the Matrix.
[3369.80 → 3371.14] Like, I don't even see the girl.
[3371.20 → 3372.10] I don't even see the code.
[3372.16 → 3373.96] I just see a girl in a red dress or whatever.
[3374.64 → 3375.84] I'm not there yet.
[3375.92 → 3380.84] But honestly, like, I'm looking at Flakes now, and I'm like, oh, so that's what that means.
[3380.96 → 3382.98] Oh, why did you do that?
[3383.26 → 3383.82] Oh, yeah.
[3384.20 → 3386.54] And there's been a few things that have kind of coalesced.
[3386.54 → 3388.90] I was reading Mitchell Hashimoto's.
[3389.00 → 3390.60] Got a pretty good Nix config.
[3390.74 → 3393.10] He's the HashiCorp guy or was.
[3393.22 → 3394.20] I don't think he's there anymore.
[3394.88 → 3404.08] John Seeger, who I think might be coming on a future episode to talk about his contributions of packaging an app for Nix packages as well.
[3404.18 → 3405.44] He might be coming on a future episode.
[3405.44 → 3413.00] But there's just been this onslaught of, besides JB, there's been this onslaught of Nix stuff happening.
[3413.50 → 3415.96] When I go out and talk to people, too, it's amazing.
[3416.10 → 3419.88] Like, regular old people just working in the industry are talking Nix to me now and stuff.
[3420.06 → 3420.36] It's wild.
[3420.36 → 3423.98] I thought you meant, like, you know, Jill at Kroger or something.
[3424.58 → 3425.26] No, no, no.
[3425.58 → 3427.54] Regular people in the normal are talking about Nix.
[3428.30 → 3434.12] I've had a couple of, like, IRL moments recently where I've just been like, wait, wait, you're running Nix here?
[3434.26 → 3435.54] Oh, yeah, no, it's a whole Nix shop.
[3435.84 → 3440.56] I was talking to a guy making a piece of hardware that I can't talk about yet on air, and he's, the whole thing's built on Nix.
[3440.72 → 3443.90] And, yeah, it's a phenomenon happening, I think, Alex.
[3443.90 → 3450.40] We are rewriting all the Jupyter broadcasting infrastructure now that Linde have stopped supporting the shows directly.
[3451.20 → 3458.90] So we're going to be rebuilding everything on top of Nix and a mixture of a few cloud things that have to be in the cloud.
[3459.02 → 3463.10] And then we're going to bring a bunch of stuff back on premise to save costs and stuff like that.
[3463.24 → 3467.48] So we don't have any concrete plans exactly on what that's going to look like.
[3467.48 → 3477.96] But at some point, we will probably want contributors to help with, you know, clarifying certain things and, you know, modifying certain pieces of infrastructure.
[3478.22 → 3482.30] So if that floats your boat, join our Nix nerds Element channel.
[3482.62 → 3484.84] I got some really sage advice in there this week.
[3484.90 → 3486.98] It's a really fantastic resource.
[3487.74 → 3490.96] So, yeah, head over to Element with a bunch of JB channels over there.
[3491.66 → 3497.28] Thank you also to all our Sees, our site reliability engineers who subscribe to the show directly through our membership program.
[3497.98 → 3500.58] Self-hosted. Show slash SRE if you'd like to sign up.
[3500.70 → 3504.46] You get an ad-free version of the show with extra content.
[3505.14 → 3505.86] A little post-show.
[3506.02 → 3509.64] And Alex teased earlier he's going to be talking about a cool little piece of hardware for our members.
[3510.34 → 3511.72] Thank you to our Sees out there.
[3511.74 → 3515.36] And thank you, everybody, who just listens to the gosh darn show and shares it with somebody.
[3515.52 → 3516.52] We really appreciate all of that.
[3517.18 → 3522.26] As usual, you can go to alex.ktz.me to find the various different things I do on the Internet.
[3522.76 → 3524.90] I'm playing around with Foster a little bit.
[3525.18 → 3527.00] ChrisLass.com if you want to find me over there.
[3527.00 → 3527.86] Thanks for listening.
[3528.08 → 3530.56] That was self-hosted. Show slash 117.
