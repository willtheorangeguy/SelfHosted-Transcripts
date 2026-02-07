[0.00 --> 4.10]  It's episode 85, and first and foremost, Alex is back.
[4.30 --> 4.96]  Welcome back, buddy.
[6.56 --> 7.76]  I'm still a little sick.
[7.92 --> 12.52]  I've got that annoying little tickle in my throat, but the rona finally got me.
[12.66 --> 16.82]  It wasn't too terribly awful, although there was one day that was pretty rough.
[17.00 --> 23.52]  My lungs didn't really feel like they fitted in my chest anymore, but after that one day
[23.52 --> 26.88]  and a whole bunch of cough syrup, I was all good.
[27.28 --> 28.86]  Yeah, I actually was really impressed.
[28.86 --> 29.72]  It was your first time.
[30.50 --> 32.34]  I think if I get it again, it's going to be my fourth.
[32.72 --> 35.88]  I have no idea how I avoided it so long with a two-year-old in daycare.
[36.22 --> 37.10]  Yeah, really, really.
[37.52 --> 38.06]  That's true.
[38.06 --> 42.66]  But I'm also really excited to say that I think all the way from episode one or two, our buddy
[42.66 --> 43.42]  Wendell is back.
[43.64 --> 44.26]  Hello, Wendell.
[44.34 --> 45.32]  Welcome back to Self-Hosted.
[45.42 --> 46.12]  How's it going?
[47.28 --> 48.40]  It's going great.
[49.24 --> 51.22]  There's a million things to talk about.
[51.34 --> 56.56]  There's so much exciting stuff in the self-hosting world because there's liquidation happening.
[56.56 --> 63.36]  You can get a 77.73 for like $4,000 if you're that crazy to run it in your home lab.
[63.50 --> 64.26]  I mean, that's a steal.
[64.66 --> 65.56]  Alex, you're that crazy.
[66.08 --> 68.10]  Never mind the power bill, though, these days.
[68.28 --> 70.68]  Hey, that thing sips the power when it's not doing anything.
[71.14 --> 71.32]  Okay.
[71.40 --> 72.28]  Define sips.
[73.22 --> 75.96]  Idling at about 68 watts.
[75.96 --> 76.86]  Oh, okay.
[76.96 --> 77.12]  Yeah.
[77.24 --> 78.96]  That's a healthy sip.
[79.04 --> 80.36]  That's my entire server.
[83.62 --> 85.18]  But yeah, that is nice to see.
[85.42 --> 89.24]  Should we maybe begin with low-powered hardware in the self-hosting area?
[89.36 --> 90.12]  There's so much.
[90.50 --> 95.90]  I think so, yeah, because Chris, you've recently got off the, if Linux Unplugged titles are to
[95.90 --> 102.46]  be believed, you've got off the Raspberry Pi train recently for the Odroid train, the x86
[102.46 --> 103.34]  train, should I say.
[103.76 --> 104.74]  And that's been going great.
[104.74 --> 107.56]  I've been doing more and more, more than I ever could before.
[107.88 --> 109.64]  It's great to have access to QuickSync.
[110.16 --> 115.84]  But, you know, the Odroid's power draw, when it's idle, it's not exactly 65 watts.
[115.98 --> 118.24]  It's more like 1.5 watts.
[118.84 --> 118.96]  Yeah.
[119.28 --> 120.62]  That is something.
[121.20 --> 121.44]  Yeah.
[122.04 --> 127.58]  It gets me thinking about these new Intel chips with their kind of weird architecture
[127.58 --> 128.26]  these days.
[128.32 --> 130.70]  They've got the performance cores and the e-cores.
[131.24 --> 133.56]  There's been a whole bunch of changes on the Intel side.
[133.64 --> 133.94]  Hey, Wendell?
[133.94 --> 140.74]  You can get a Linux-based operating system that will handle it really well.
[140.84 --> 141.24]  And that works.
[141.32 --> 142.34]  That works pretty well.
[142.70 --> 150.74]  My pause is the horror show that's going out of my head with VMware and Proxmox and XCPNG.
[150.74 --> 154.08]  It's not a lot of fun with any of those.
[154.08 --> 157.82]  Because XCPNG is, you know, it's an older kernel, but they do a lot of patches.
[157.82 --> 163.98]  But mixed cores with that, it's just, I don't like inconsistent performance.
[163.98 --> 171.72]  Honestly, I'm kind of annoyed with XCPNG because I have a separate thread going and they're basically
[171.72 --> 177.96]  okay with the performance not being as good as it could be in the hypervisor.
[178.68 --> 182.70]  And I'm not sure what it is, but like turbo is not working correctly on some high-end parts
[182.70 --> 183.88]  that will turbo like crazy.
[183.88 --> 185.76]  But that's not really super applicable for the home lab.
[186.00 --> 191.08]  But those issues are kind of bleed over when we're talking about mixed, small, and big cores.
[191.50 --> 196.02]  So Proxmox works a little better because you can run a newer Linux kernel and the Linux kernel
[196.02 --> 197.74]  will do the appropriate juggling for that.
[198.10 --> 203.64]  And so, yeah, like at 13900K, you can end up with a 24-core system if you want to go something
[203.64 --> 206.36]  crazy like that for your home setup.
[206.36 --> 211.80]  But really, it's like 64 gigabytes of memory is like the largest practical maximum, although
[211.80 --> 213.48]  you can do 128 gigabytes of memory.
[214.14 --> 219.64]  But the $100 processors, the $100-ish processors, I think are way more interesting in that LGA
[219.64 --> 225.20]  1700 socket because you can run 32 or 64 gigs of memory pretty inexpensively because you
[225.20 --> 225.94]  can get DDR4.
[226.62 --> 231.88]  And the motherboard for like your home server use case, there's not a lot of super interesting
[231.88 --> 233.48]  motherboards for LGA 1700.
[233.66 --> 234.72]  There's one from Gigabyte.
[234.80 --> 235.56]  They didn't make enough.
[235.56 --> 242.86]  I'm really tempted to do a group buy of those motherboards on level one, like buy 100 of
[242.86 --> 248.56]  them or 200 of them and then resell them because it's a W680 chipset and that motherboard works
[248.56 --> 248.98]  pretty well.
[249.06 --> 251.62]  I'd like to have more slots, but motherboard works pretty well.
[251.76 --> 256.88]  And that's what I'm, I've got a test system that I've been just, I'm blown away by how
[256.88 --> 258.02]  insanely fast it is.
[258.08 --> 263.84]  It's six Alder Lake P cores, no E cores on a processor that I got for around $100, the
[263.84 --> 264.48]  12400.
[264.48 --> 266.94]  And so it turbos like crazy.
[267.04 --> 268.84]  It turbos like there's nobody's business.
[269.04 --> 271.22]  And so those six cores are insanely fast.
[271.32 --> 274.44]  Even XCPNG, VMware, Proxmox, whatever you want to run on it.
[274.84 --> 276.06]  It's very, very fast.
[276.12 --> 278.68]  It puts all of the embedded processors to shame.
[278.78 --> 279.54]  It really is shocking.
[279.66 --> 280.80]  Like 2X is fast.
[280.80 --> 288.82]  Gigabyte made my first real, you know, foray into home server, you know, dual Xeon socket
[288.82 --> 289.16]  boards.
[289.26 --> 290.70]  It had two 10 gig NICs.
[290.76 --> 292.42]  It was the GA7 PESH2.
[292.84 --> 294.28]  That thing was awesome.
[294.40 --> 300.60]  It had an HBA built directly into the board and two 10 gig NICs plus a BMC NIC as well.
[300.60 --> 305.48]  What is it about this other gigabyte board that you mentioned, the 12th, 13th gen board
[305.48 --> 306.90]  that has got you interested?
[307.34 --> 308.26]  Because it's so disruptive.
[308.66 --> 314.30]  So like you go on eBay or you look at, you know, I need to find an appropriate home server
[314.30 --> 314.74]  system.
[314.84 --> 317.44]  And you look at the board and it's not, it's really kind of unremarkable.
[317.44 --> 322.26]  You've got two X8 slots that'll run, you know, to the CPU and then, you know, Alder
[322.26 --> 326.22]  Lake has got the extra lanes and then the DMI is eight lanes.
[326.42 --> 328.24]  So it's got a ton of M.2 slots.
[328.48 --> 332.34]  In my video, I converted the M.2 slots into two and a half gig NICs.
[332.40 --> 335.08]  So you can get M.2, two and a half gig or 10 gig NICs.
[335.14 --> 335.82]  Those are a lot of fun.
[336.00 --> 337.50]  So you add a bunch of NICs that way.
[337.56 --> 341.64]  And then you've got three PCIe slots that you can mix and match for peripherals, disk storage,
[341.76 --> 346.36]  whatever, which is pretty reasonable and 32 or 64 gigs of memory, which is pretty reasonable.
[346.36 --> 348.20]  And you could put an i5 in there.
[348.42 --> 350.36]  So is that the route you'd go these days?
[350.62 --> 352.74]  A 12th or 13th gen CPU?
[353.12 --> 357.46]  Or would you be tempted to look for, you know, four, five year old, eighth, ninth, 10th gen,
[357.54 --> 358.10]  something like that?
[358.24 --> 358.92]  No, no.
[359.02 --> 362.70]  Because the Alder Lake PCORs are so insanely fast.
[362.94 --> 365.74]  It is, Intel is not asleep at the wheel anymore.
[366.04 --> 370.30]  I mean, it is not incremental improvements over the course.
[370.38 --> 373.28]  So like, if you look at like 10th to 11th gen, total snooze fest.
[373.86 --> 375.34]  And yeah, I mean, they're really good.
[375.34 --> 379.66]  If you're rocking a ninth, 10th, 11th generation system, okay, that's fine.
[380.18 --> 387.92]  But the per core performance is almost a 2X in those configurations.
[388.64 --> 393.98]  And with the W680 chipset, they're not playing games with ECC anymore.
[394.10 --> 395.66]  So the Gigabyte board's DDR4.
[395.86 --> 397.72]  So you can get commodity DDR4.
[397.72 --> 403.38]  All the hyperscalers and everybody else is sucking up the DDR5 ECC and registered ECC.
[404.00 --> 404.94]  Like there's no tomorrow.
[405.20 --> 408.42]  And I'm not even really sure we've completely figured out DDR5 yet.
[408.50 --> 410.38]  So this Gigabyte board is DDR4.
[410.92 --> 414.86]  And so you can get cheap, cheap, cheap commodity DDR4 memory.
[414.86 --> 419.66]  And that 6P core system will run circles around anything that's older.
[419.78 --> 426.22]  It's like, oh, I've got this, you know, great, you know, Lenovo system that was a small form factor that has a two and a half week Nick.
[426.22 --> 428.02]  It's like, yeah, I don't care.
[428.14 --> 430.94]  This thing is twice as fast per core.
[430.94 --> 439.60]  And the kinds of things that you're running on a home server generally run better with fewer faster cores than more slower cores.
[439.98 --> 445.44]  You want SMB to, you know, run, rock your socks off and you're not willing to set up multi-channel.
[445.82 --> 448.46]  Having insanely fast cores is nice.
[449.04 --> 450.50]  What about the AMD side of things?
[450.52 --> 453.90]  Because they've had a pretty big launch with the Ryzen 7000 stuff lately.
[454.34 --> 457.14]  Those are going to cost more, but those are also really nice.
[457.14 --> 466.00]  So I set up a system around Linux, you know, just vanilla Linux, but running services on vanilla Linux based on the 7950X.
[466.00 --> 473.34]  But I used the, you know, the 7950X, it'll consume north of 150 watts happily.
[473.66 --> 476.50]  But you can configure it to not do that.
[476.82 --> 481.26]  And so if you're willing to let it run, it's not quite 65 watts.
[481.60 --> 485.06]  The happy medium, I think, is probably around 80 or 85 watts.
[485.08 --> 486.24]  You can tell it to run at that.
[486.24 --> 487.26]  It runs cooler.
[487.40 --> 488.56]  It uses way less power.
[488.68 --> 491.94]  And you lose like maybe 5 or 6% overall performance.
[492.46 --> 494.66]  And you have 16 homogenous cores.
[495.02 --> 501.02]  And yeah, the processor is like $558, $600, something like that, because it's on sale right now.
[501.14 --> 502.24]  But it's 16 cores.
[502.34 --> 503.94]  And that is a really monstrous system.
[504.40 --> 508.68]  The only limitation is really the whole, the aforementioned 64 to 128 gigabytes of memory.
[508.68 --> 516.24]  Those cores are so awesome that in a home server scenario, for me, 128 gigs doesn't do it.
[516.38 --> 519.32]  And 64 gigs is insanely way faster than 128 gig.
[519.84 --> 523.70]  Do, in your opinion, the media encoding engines matter?
[523.84 --> 524.90]  With Intel, it's QuickSync.
[525.00 --> 531.42]  With AMD, the support, certainly for like Plex and Jellyfin and stuff like that, is a bit ropey.
[531.42 --> 532.34]  Yeah, yeah.
[532.40 --> 535.14]  QuickSync is still much more well supported.
[535.52 --> 538.36]  It is an option now on the AMD side.
[538.44 --> 540.62]  And the encoder, the hardware is there and it's very good.
[540.70 --> 545.22]  But I don't think the software has, the software enablement has happened yet.
[545.88 --> 551.62]  But, you know, PCIe hardware runs circles around both QuickSync and the CPU.
[552.00 --> 553.20]  But it uses a lot more power.
[553.44 --> 554.82]  So it just depends on what you're building.
[555.22 --> 555.86]  It's interesting.
[555.86 --> 560.32]  I was speaking to some people in our Discord today from England and their electricity prices.
[560.44 --> 567.54]  When I left, I think I was, you know, this is four or five years ago, I was paying about 14, 12, 14 pence a kilowatt hour.
[568.06 --> 570.56]  They're paying 40 to 50 pence now.
[570.64 --> 571.26]  It's lower.
[571.60 --> 572.44]  Per kilowatt hour.
[572.94 --> 578.04]  And through that lens, an energy efficient system pays for itself extremely quickly.
[578.50 --> 582.16]  Yeah, that six core Alder Lake system will give you QuickSync and everything else.
[582.16 --> 592.82]  And when it's idle, it will be very, like, honestly, the Gigabyte board, the ASP2500 uses, because it's, you know, the system on the IP mine, it's in a system in a system that's always on.
[593.32 --> 597.00]  We use more power than the CPU at idle.
[597.26 --> 597.56]  They do.
[597.84 --> 598.44]  It's crazy.
[598.62 --> 605.18]  Why do BMCs need to use so much, so much electricity just to sit there and provide an insecure web UI, you know?
[605.24 --> 606.40]  Maybe that's how they make their money.
[606.48 --> 609.40]  It's doing some sort of cryptocurrency mining in the background.
[609.40 --> 612.70]  It's owned by the power company.
[612.98 --> 613.64]  They have stock.
[613.96 --> 614.06]  Yeah.
[615.14 --> 620.74]  You can disable that and get, I was shocked when I was building the test system.
[621.22 --> 624.72]  The thing that's using the most power now is keeping the mechanical hard drives spinning.
[625.32 --> 625.74]  Oh, yeah.
[626.22 --> 628.42]  Are you a spin down sort of gentleman or?
[628.42 --> 632.26]  I haven't historically been, but I'm becoming that.
[632.40 --> 633.80]  And it's just, it's like a.
[634.62 --> 635.06]  Yeah.
[635.18 --> 637.50]  With ZFS in particular, that can be a bit of a pain.
[637.70 --> 646.62]  If you have the metadata special device, it seems to help because then all the metadata is stored on the SSD or on a solid state.
[646.62 --> 650.04]  And you can also specify that smaller files are stored that way as well.
[650.24 --> 657.08]  So if you're careful with your data sets and everything else, then you're using your mechanical storage just for bulk storage.
[657.08 --> 659.22]  And then it ends up working pretty well.
[659.72 --> 660.60]  Well, that's a great tip.
[660.76 --> 664.22]  You're going to spend a lot of time chasing down some rabbit holes, but you can do it.
[664.22 --> 669.06]  While we're talking storage, what are you looking at for local storage these days?
[669.18 --> 674.28]  Personally, I think we should delineate and maybe also for if you want to disclose for workside.
[674.36 --> 677.20]  But we always like to ask our guests what they're doing storage wise.
[677.24 --> 679.30]  And I think you've ranked pretty highly on that list.
[679.48 --> 680.32]  Yeah, you're on our leaderboard.
[680.40 --> 680.94]  You're at the top.
[681.02 --> 683.64]  You've got a petabyte, which nobody's come close to.
[683.64 --> 687.24]  Yeah, I just, a few, it was like a month and a half, two months ago.
[687.32 --> 688.64]  I was like, all right, I'll just bite the bullet.
[689.30 --> 693.92]  So I got to, there's, we have, it's about 1.2 petabytes locally.
[693.92 --> 698.36]  There's one system that has, that has a usable, it has a petabyte usable.
[698.36 --> 702.88]  And then the other system is 180 or 100.
[702.98 --> 706.10]  I think it's, it's 180 ish terabytes, give or take.
[706.56 --> 716.30]  At home, I have six, 14 or 16 terabyte hard drives in a RAID Z2 and eight, two terabyte
[716.30 --> 719.26]  NVMe that are enterprise cast off drives that are just completely shredded.
[719.26 --> 722.90]  Like they were in production use for three or four years.
[722.90 --> 728.10]  And they've, they've, they've had, you know, their, their drive, drive lifetime is, is let's
[728.10 --> 729.10]  say five petabytes.
[729.24 --> 733.38]  I don't remember what the numbers are, but if you look at the, like how much those drives
[733.38 --> 736.76]  have been used, they've been used like 2.1 petabytes.
[737.22 --> 741.60]  And so it's like, I'll just, I'll put eight of them in and we'll RAID Z2 those as well.
[741.68 --> 746.98]  So I have a, I have a, an SSD pool and I have a, I have a mechanical storage pool and the
[746.98 --> 749.34]  mechanical storage pool has all the media and everything on it.
[749.34 --> 750.34]  And it's pretty full.
[751.20 --> 753.60]  I did the, uh, it's, what is it?
[753.62 --> 757.82]  It's like the ultimate ripping machine or fully, fully automatic ripping machine.
[757.90 --> 758.84]  There's a GitHub project.
[759.32 --> 763.68]  And, uh, Jeff Geerling did a video on, um, the Blu-ray side of it.
[763.74 --> 767.46]  I'm scared to death to do that because YouTube will just, you know, Disney or somebody will
[767.46 --> 769.32]  watch it and just blah, blah, blah.
[769.42 --> 770.62]  And then I don't have a channel anymore.
[771.04 --> 773.04]  So I got a pretty extensive DVD collection.
[773.04 --> 776.00]  And so I ripped, I re-ripped all that for a while.
[776.04 --> 777.00]  It was like, I'll just stream it.
[777.02 --> 777.76]  I don't need to do this.
[777.82 --> 778.80]  I don't need to store this.
[779.08 --> 781.22]  And so I didn't really do a good job maintaining that.
[781.62 --> 783.32]  I'd already ripped all my DVDs once.
[783.66 --> 785.26]  And so now I've redone that.
[785.60 --> 788.36]  And we have left the golden age of streaming.
[788.50 --> 789.40]  It has left the building.
[789.62 --> 789.86]  Yeah.
[789.96 --> 790.26]  Yeah.
[790.36 --> 790.62]  Yeah.
[791.46 --> 792.00]  Yeah, definitely.
[792.50 --> 797.86]  I definitely have that kind of now sort of thought process of, well, I better have a local
[797.86 --> 801.48]  copy of this because who knows when they might pull it and it won't be available.
[801.48 --> 805.32]  And if my kids love this show, I don't want it to become unavailable.
[805.78 --> 806.50]  Final Space, man.
[806.74 --> 808.20]  That's the perfect example.
[808.36 --> 809.04]  Final Space.
[809.28 --> 809.48]  Yeah.
[809.76 --> 810.42]  Never forget.
[810.76 --> 811.86]  Never forget Final Space.
[812.48 --> 812.66]  Yeah.
[812.66 --> 815.24]  I don't think anybody's going to beat over a petabyte of storage.
[815.42 --> 817.84]  So I think they'll remain high on the chart for a while.
[817.92 --> 818.48]  Congrats, Wendell.
[818.58 --> 819.68]  It's like, this is like Top Gear.
[819.80 --> 822.18]  It's like Lewis Hamilton going on and going a second faster.
[822.30 --> 824.24]  It's like, okay, you're already in the lead.
[824.36 --> 824.84]  Well done.
[826.66 --> 828.08]  More petabytes now.
[828.08 --> 828.36]  Oh yeah.
[829.02 --> 833.32]  So last time we spoke to you, I think you were doing some cool stuff around your mailbox
[833.32 --> 836.32]  and Bluetooth low energy sensors, that kind of stuff.
[836.58 --> 839.98]  What have you got going in the home automation side of things these days?
[840.12 --> 844.54]  So I just did, I don't know if it's out yet or not.
[844.76 --> 847.08]  I got, I was, the seed studio reached out.
[847.08 --> 852.86]  And so I talked to them and they filled in some gaps on some stuff.
[852.86 --> 853.58]  That's really exciting.
[853.68 --> 857.32]  One of the things is they have the re-server.
[857.48 --> 861.14]  They have the re-terminal, re-server and some sensors.
[861.40 --> 863.12]  And so re-server, I'll mention first.
[863.18 --> 864.62]  You can get it in a bunch of different configurations.
[864.80 --> 865.72]  One of them has Thunderbolt.
[865.92 --> 866.80]  It's very low powered.
[866.88 --> 870.68]  It has two mechanical three and two, three and a half inch drive bays you can use with
[870.68 --> 871.90]  mechanical drives or anything else.
[872.04 --> 873.34]  That's a very low power system.
[873.44 --> 874.64]  It's shockingly powerful.
[874.64 --> 878.52]  It has three M.2 internally, B key, E key, and M key.
[879.20 --> 886.90]  And I set up that with ZFS, a mirror and metadata on the M.2.
[887.14 --> 889.04]  Also with Optane, because Optane's on fire sale.
[889.14 --> 890.54]  We should talk about the Optane fire sale.
[890.76 --> 890.86]  Woo!
[891.24 --> 891.64]  All right.
[891.68 --> 892.74]  There's so much going on.
[893.08 --> 894.24]  And so I love that little thing.
[894.30 --> 894.86]  It's low power.
[894.98 --> 896.44]  It's Intel, four core.
[896.88 --> 897.42]  It's older.
[897.96 --> 902.10]  It's not, you know, going to burn your house down with fire power, like the older Lake CPUs,
[902.28 --> 903.30]  but it's pretty good.
[903.30 --> 905.36]  And it's a nice, it's an attractive aluminum enclosure.
[906.10 --> 908.10]  The specs are all online.
[908.18 --> 909.82]  You can 3D print accessories for it.
[910.14 --> 912.80]  And it's a fan in the bottom vent from the top.
[912.88 --> 914.46]  The re-server is, it's really, really cool.
[914.54 --> 915.46]  I'm having a lot of fun with it.
[916.18 --> 920.54]  And then they sent me, I showed them the setup that I had with my, I don't think I have one
[920.54 --> 921.36]  of those sensors handy.
[921.48 --> 925.38]  I've got the O2 sensors there, the O2 CO2 sensors for my house.
[925.38 --> 928.34]  And I sort of showed some of the setup that I did with that.
[928.66 --> 934.00]  And so I've got a re-terminal tied into Home Assistant now, because it's a Raspberry Pi
[934.00 --> 937.14]  compute module in a thing, in like an enclosure.
[937.24 --> 939.48]  And the enclosure is pretty attractive, although it's not power over ethernet.
[939.52 --> 940.16]  It's not perfect.
[940.26 --> 943.26]  It's got some rough edges, some obvious things that could have done better.
[943.26 --> 945.02]  Uh, PoE would be so nice.
[945.16 --> 948.88]  Yeah, but it's a, it's a touchscreen and I got it tied in with Home Assistant now.
[948.96 --> 950.06]  It's all my Home Assistant stuff.
[950.16 --> 956.46]  And so where the, uh, one of the thermostats was for one of the middle-aged heating and
[956.46 --> 958.48]  cooling systems that was in my house, it's no longer there.
[958.58 --> 961.90]  I put, I put it there and I, I'm powering it that way.
[961.92 --> 965.30]  And I'm, I've, I used the old thermostat wire to pull Cat6.
[965.68 --> 967.58]  And so it's got power and everything else.
[967.92 --> 969.62]  And that has gone really well.
[969.62 --> 974.02]  And so in a Home Assistant, I can see what it's doing as far as air quality.
[974.02 --> 979.40]  And if the, the heat exchanger is on and if it, it'll, it'll override the air conditioning
[979.40 --> 982.78]  system and turn the fan on to just move air around the house.
[983.00 --> 987.72]  But the existing HVAC system continues to work without Home Assistant.
[988.04 --> 992.82]  So everything that I have ever done with sensors and everything else could be on fire and broken.
[993.16 --> 997.22]  And I will still have at least basic temperature control and environmental controls.
[997.22 --> 1002.84]  I kind of seem to recall you were semi-skeptical of Home Assistant a couple of years ago.
[1003.00 --> 1005.98]  Has that, are you still a little skeptical that it could fail?
[1006.04 --> 1007.18]  Is that why you designed it that way?
[1007.56 --> 1007.86]  Yes.
[1008.00 --> 1009.82]  And it's actually worked out really well.
[1009.94 --> 1014.94]  And Home Assistant has added the high availability features that I was looking for since then.
[1015.16 --> 1018.62]  So you can run a cluster of Home Assistant, which is...
[1019.24 --> 1019.98]  There you go.
[1019.98 --> 1026.28]  They don't have a mechanism for shooting the other node in the head though.
[1026.36 --> 1027.62]  So you could get split brain.
[1028.14 --> 1030.00]  At least I'm pretty sure you can get split brain.
[1030.40 --> 1034.82]  But you know, if that's the worst that we're dealing with on thermostat controls, it's not bad.
[1035.24 --> 1038.24]  I hadn't seen this re-terminal thing before from Siege Studio.
[1038.82 --> 1043.32]  This is a, for those that aren't familiar as well, it's an all-in-one Raspberry Pi board,
[1043.32 --> 1049.14]  which takes a CM4 module and it can connect over Wi-Fi, Bluetooth, all the rest of it.
[1049.82 --> 1051.88]  I think it looks, it looks pretty cool.
[1052.02 --> 1057.02]  There's an HDMI or, sorry, a micro HDMI, a micro SD card slot, all the rest of it that's on there.
[1057.74 --> 1059.68]  This thing looks pretty, pretty interesting.
[1059.80 --> 1061.58]  Have you got it mounted on the wall, I presume?
[1061.90 --> 1065.48]  Whenever I've been dealing with the modules, the compute modules for Raspberry Pi,
[1065.56 --> 1068.02]  I tend to run my Raspberry Pis pretty hard and they get hot.
[1068.34 --> 1072.96]  This thing has a really huge mechanical heat sink that's connected to the outside of the enclosure.
[1073.32 --> 1075.78]  And it seems like they started with that for the design.
[1075.90 --> 1077.90]  And that is the best feature of this design.
[1078.02 --> 1081.80]  The touchscreen is very high quality and so far, no issues with it.
[1081.98 --> 1087.32]  And it's very, very accurate, I guess, is probably the way to describe it.
[1087.56 --> 1091.66]  And it's been a lot of fun, you know, sort of hacking on that and making it a little more accessible.
[1092.22 --> 1092.56]  Yeah, no kidding.
[1092.64 --> 1095.56]  I could see, well, I don't know if I could see Chris doing this in the RV,
[1095.82 --> 1097.60]  putting some nice on the wall, but definitely in the studio.
[1098.18 --> 1098.38]  Yeah.
[1098.60 --> 1099.62]  You know, it's funny.
[1099.62 --> 1104.94]  For me, I have been thinking more and more instead of doing tablets that run wall panel
[1104.94 --> 1107.46]  or something like that or some kiosk mode.
[1108.04 --> 1112.76]  But maybe I should just Raspberry Pi that or really CM4 it and a touchscreen.
[1113.32 --> 1117.16]  And this is kind of like the next version of that that I didn't even really,
[1117.24 --> 1119.16]  I hadn't really even thought of as all in one device.
[1119.26 --> 1123.42]  It'd be great if you could embed it into the wall so it was flush with the wall.
[1123.54 --> 1124.62]  How slick would that be?
[1125.04 --> 1126.66]  You just need to get Brent to come around again.
[1126.66 --> 1128.10]  Do a little drywall work.
[1130.04 --> 1131.52]  It would probably breathe better.
[1132.72 --> 1136.48]  There's a backpack you can get for it that will give it proper power over Ethernet.
[1136.92 --> 1141.70]  But I ended up just running a DC, an extra little DC cable for now.
[1142.32 --> 1143.26]  I don't long term.
[1143.40 --> 1148.52]  I'm sort of torn because I could actually run a DC cable through the wall and have the power
[1148.52 --> 1150.08]  over Ethernet thing in the basement.
[1150.08 --> 1155.22]  So like just a long extension for the wires needed for PoE.
[1156.66 --> 1158.90]  I guess, but I don't know.
[1158.98 --> 1160.18]  It's just, it's.
[1162.04 --> 1164.08]  Yeah, that's my strugs as well.
[1164.66 --> 1164.80]  Yeah.
[1164.84 --> 1168.14]  And the other issue is, is what if I want to replace it with something else that's totally
[1168.14 --> 1169.08]  different down the road?
[1169.26 --> 1172.30]  And then I've done all this work for something that I only use for like two years.
[1172.92 --> 1173.98]  You know, there's that as well.
[1174.38 --> 1175.16]  That's where I ended up.
[1175.18 --> 1175.62]  It's like power.
[1175.78 --> 1178.64]  I'm going to have an Ethernet cable and then a little something else.
[1178.64 --> 1182.10]  And then maybe down the road, I'll have something that's just power over Ethernet and I won't
[1182.10 --> 1182.84]  use the other wire.
[1182.92 --> 1183.48]  And that's fine.
[1183.48 --> 1186.00]  All right.
[1186.04 --> 1189.12]  So the read terminal, we'll put a link to that in the show notes at self-hosted.show
[1189.12 --> 1190.54]  slash 85.
[1191.02 --> 1191.20]  Right.
[1191.64 --> 1194.68]  Cause you know, seed is all about the whole electronic projects.
[1194.82 --> 1199.28]  They have a CO2 sensor module and they have adapters for that kind of stuff.
[1199.30 --> 1205.82]  So you can DIY that sort of stuff together using that as a basis and then really build
[1205.82 --> 1208.78]  something that's you, but that was sort of Lego together.
[1209.12 --> 1209.32]  Yeah.
[1209.66 --> 1209.86]  Yeah.
[1209.86 --> 1212.34]  And would last as long as you want to, you know.
[1213.48 --> 1213.82]  Keep it.
[1214.18 --> 1215.26]  Did you, is that what you used?
[1215.34 --> 1217.64]  I noticed you did mention you have some sensors.
[1217.92 --> 1220.60]  Are those the sensors you're using or did you go a different route?
[1220.70 --> 1220.82]  Yeah.
[1220.88 --> 1228.04]  Well, so I, I have preexisting, I have the co-pilot sensors, which have a USB output you
[1228.04 --> 1230.94]  can use, but I tried theirs and theirs is very good as well.
[1230.94 --> 1236.82]  I have been probably spending the last two weeks experimenting with water leak sensors, temperature
[1236.82 --> 1244.48]  sensors, humidity sensors, motion sensors, door sensors, window sensors, present sensors.
[1245.10 --> 1248.24]  And, uh, I really still haven't found like the perfect combination of it.
[1248.30 --> 1252.16]  So I, I like, I kind of like what you're suggesting because it kind of feels like it's a little more
[1252.16 --> 1252.54]  permanent.
[1252.54 --> 1253.70]  It's a little more infrastructure.
[1254.00 --> 1255.80]  It's kind of like you build it once and then you leave it.
[1255.80 --> 1256.28]  Yeah.
[1256.38 --> 1262.90]  And I still have, um, you know, my home alarm system has the, uh, PIR motion sensors and
[1262.90 --> 1270.20]  mechanical door sensors and mechanical, it's the home, the home alarm sensors for, uh, water
[1270.20 --> 1271.90]  where it's not supposed to be.
[1272.40 --> 1277.44]  And that sort of stuff are all tied into the alarm panel, but the alarm panel is also tied
[1277.44 --> 1278.16]  into home assistant.
[1278.52 --> 1281.06]  And that has been working fabulously well.
[1281.06 --> 1282.82]  100% reliability.
[1283.34 --> 1287.42]  That's a pretty high number, pretty high level, pretty high level of reliability there.
[1287.78 --> 1291.24]  So far it hasn't gone down and it has its own lead acid battery.
[1291.44 --> 1295.06]  So even when the power has been off the lead, the separate lead acid battery for the alarm
[1295.06 --> 1296.80]  system has kept it going.
[1297.38 --> 1300.92]  So it's like, Oh, there's no power at my house, but the alarm system will still blare
[1300.92 --> 1301.98]  if somebody breaks in.
[1302.62 --> 1307.64]  Speaking of power, I think I, uh, tripped across a video of yours, uh, a few weeks ago about
[1307.64 --> 1308.94]  UPSs and stuff like that.
[1308.94 --> 1310.76]  I just thought it was an excellent video.
[1311.34 --> 1315.44]  Uh, and if anybody's curious about, you know, which UPS should I buy?
[1315.52 --> 1316.68]  How big should it be?
[1316.68 --> 1321.78]  And we want to hear, you know, 20 minutes of, uh, Wendell talking about UPSs.
[1322.04 --> 1325.40]  Almost all UPSs are just absolute trash.
[1325.66 --> 1329.54]  And it's just, it's just, it's all down here.
[1329.62 --> 1330.86]  We want UPSs to be up here.
[1330.96 --> 1332.00]  They're all just down here.
[1332.58 --> 1338.80]  There's no reason that we shouldn't be able to buy UPS and get a UPS that lasts 10
[1338.80 --> 1339.30]  years.
[1339.62 --> 1343.78]  And it would only be marginally more expensive than the UPSs we have now.
[1344.30 --> 1344.60]  Yes.
[1344.74 --> 1348.52]  I was wondering about using something like, you know, the Jackeries that you can buy these,
[1348.52 --> 1353.64]  uh, lithium ion based portable battery packs as a UPS in some, some places.
[1353.76 --> 1354.84]  Interesting idea, Alex.
[1355.04 --> 1357.56]  I don't know what the switch time is on off the top of my head.
[1357.66 --> 1359.52]  You need a really fast switch time.
[1360.10 --> 1360.32]  Yeah.
[1360.80 --> 1361.08]  Yeah.
[1361.08 --> 1361.98]  I suppose it would depend.
[1362.04 --> 1363.20]  Are they generating the power?
[1363.20 --> 1367.48]  The power for those plugs, is that coming from the inverter and the battery all the time?
[1367.60 --> 1370.72]  Or does it only switch over once it's done charging?
[1370.82 --> 1375.48]  Because in theory, in your setup, Alex, the Jackery would be in charge mode, right?
[1375.58 --> 1377.02]  Plugged into source power.
[1377.24 --> 1377.30]  Yeah.
[1377.30 --> 1382.46]  And so I guess the question is, is what happens when the batteries are fully charged?
[1382.80 --> 1385.18]  The outlets on the Jackery, where does that power come from?
[1385.22 --> 1386.08]  Is it just pass through?
[1387.52 --> 1388.16]  Who knows?
[1389.06 --> 1391.72]  But they're, you know, they're lithium ion, decent inverters.
[1391.82 --> 1392.98]  They give you the load information.
[1392.98 --> 1395.80]  They give you a nice digital display with the percentage of the battery.
[1395.80 --> 1399.06]  And they cost about as much as a high-end UPS.
[1399.48 --> 1400.34]  It's not a bad idea.
[1400.52 --> 1403.92]  It may be possible to override, if it's got a fast switch time, it may be possible to override
[1403.92 --> 1404.72]  things in software.
[1404.86 --> 1410.60]  Because if you want a lithium ion battery to last 10 years, don't charge it past 70 or 72%,
[1410.60 --> 1411.48]  something like that.
[1411.56 --> 1411.84]  Yeah.
[1412.04 --> 1413.50]  I don't remember what it is off the top of my head.
[1413.56 --> 1417.18]  I'm sure that there's a battery expert in the chat or in the comments that'll be like,
[1417.22 --> 1419.44]  this is the power curve for lithium.
[1419.44 --> 1421.02]  And this is what you want it to be.
[1421.96 --> 1422.94]  Yeah, for sure.
[1423.34 --> 1424.98]  That's what I try to go for.
[1424.98 --> 1433.84]  So in my RV, I have six lithium ion batteries and I'm aiming for about 70% just float charge
[1433.84 --> 1435.90]  when we're hooked up all the time for months at a time.
[1436.14 --> 1438.58]  But I have to remember to remove that.
[1438.64 --> 1442.40]  And it's a manual thing because when we're on the road, I want to have them up at 100%
[1442.40 --> 1445.54]  so that I have the full range of the batteries.
[1445.86 --> 1449.86]  And, you know, it's one of those things where there's no automation for that because I have
[1449.86 --> 1454.72]  not really been able to automate the battery system and definitely has screwed me.
[1454.98 --> 1457.40]  So I got to be careful.
[1458.20 --> 1460.42]  I've run into the same thing with lead acid batteries.
[1460.54 --> 1462.34]  It's like, oh, these lead acid batteries will last forever.
[1462.48 --> 1466.64]  And it's like, I got to remember to, I can't remember what model it is.
[1466.68 --> 1471.60]  There's a model of UPS where you can actually get an FTDI controller and plug in and just
[1471.60 --> 1479.14]  reprogram the UPS to not have the charge voltage be dumping 14.8 volts into the batteries all
[1479.14 --> 1479.76]  the time.
[1479.76 --> 1482.84]  And then, boom, the lead acid batteries last two more years.
[1482.84 --> 1487.28]  CrowdStrike.com slash LCE.
[1487.46 --> 1491.08]  That's where you go to ingest and view all of your logs in one place.
[1491.86 --> 1497.14]  CrowdStrike Falcon LogScale is CrowdStrike's new centralized log management and observability
[1497.14 --> 1497.46]  tool.
[1497.82 --> 1498.84]  It's formerly known as Humio.
[1499.30 --> 1503.70]  LogScale was developed as an alternative to legacy logging solutions that make it cost
[1503.70 --> 1507.74]  prohibitive to ingest and search the data volumes you see in today's IT infrastructures.
[1507.74 --> 1513.62]  And the real beauty of LogScale is that it can take logs from any source and make them
[1513.62 --> 1514.42]  usable.
[1515.08 --> 1517.26]  You don't need to constantly massage the format.
[1517.62 --> 1518.58]  It doesn't need a schema.
[1518.94 --> 1522.10]  You just pump them all in there and you have what you need when you need them.
[1522.18 --> 1524.36]  And of course, the dashboard is great.
[1524.76 --> 1526.04]  The platform is crazy, too.
[1526.54 --> 1531.00]  LogScale's index-free architecture means you can ingest over a petabyte of data per day.
[1531.16 --> 1533.46]  And then you could search that with sub-second latency.
[1534.08 --> 1534.70]  Not hours.
[1535.52 --> 1536.04]  Seconds.
[1536.04 --> 1540.82]  And LogScale is up to 80% cheaper than the competing platforms like Splunk and Elastic
[1540.82 --> 1542.50]  thanks to its reduced hardware footprint.
[1543.12 --> 1547.68]  I was fighting a machine in the studio today and I realized, aha, I should put the studio
[1547.68 --> 1549.42]  machines into LogScale.
[1549.60 --> 1553.04]  So that way I discover the problem before I arrive at the studio.
[1553.48 --> 1557.50]  I think the best way to get going with LogScale is the LogScale Community Edition.
[1558.08 --> 1561.28]  It's the largest no-cost data ingestion offering on the market.
[1561.28 --> 1565.94]  And LogScale Community Edition allows you to ingest up to 16 gigabytes.
[1566.04 --> 1568.74]  Per day with seven days of retention.
[1569.22 --> 1570.24]  No credit card required.
[1570.78 --> 1571.26]  No trial.
[1571.66 --> 1573.00]  You've got that for the long haul.
[1573.40 --> 1577.56]  This is perfect for self-hosters who want to ingest their home logs and get a single
[1577.56 --> 1579.54]  view of everything happening in their environment.
[1580.50 --> 1582.56]  Why have all separate places you have to go look?
[1582.72 --> 1583.46]  Why do it that way?
[1583.52 --> 1584.42]  That's just making it hard.
[1584.50 --> 1586.26]  And when it's your hobby, you want it easy.
[1586.50 --> 1587.06]  You want it quick.
[1587.14 --> 1587.70]  You want it usable.
[1588.08 --> 1589.52]  And you don't want it to be a big old job.
[1589.52 --> 1594.50]  So go get started with LogScale Community Edition for free over at CrowdStrike.com slash
[1594.50 --> 1595.46]  LCE.
[1595.66 --> 1599.54]  That's CrowdStrike.com slash LCE.
[1601.82 --> 1605.32]  Last week, I talked about some issues I was having with Zigbee.
[1605.32 --> 1605.40]  Zigbee.
[1605.80 --> 1609.26]  And we've gotten a lot of feedback.
[1609.68 --> 1611.34]  A lot of feedback that was very helpful.
[1611.50 --> 1614.66]  I spent the last week sorting my Zigbee issues out.
[1614.72 --> 1616.68]  And I'm curious, Wendell, if you've ever had this issue.
[1617.04 --> 1621.18]  I really wanted to like Zigbee because I know it's involved with the Matter standard.
[1621.84 --> 1623.72]  And so I thought, okay, this is the direction to go.
[1624.10 --> 1626.96]  But I have to say a lot of my devices have been dropping off the network.
[1627.38 --> 1628.38]  What are your experiences?
[1629.18 --> 1630.82]  Yeah, I got a bunch of Zigbee stuff.
[1630.82 --> 1634.42]  I set it up and then three days later, there was two things missing.
[1634.50 --> 1635.36]  And it's like, you know what?
[1635.68 --> 1636.80]  Nope, I'm out.
[1637.14 --> 1637.68]  Yeah, exactly.
[1639.26 --> 1639.66]  Yeah.
[1640.08 --> 1640.48]  Yeah.
[1640.52 --> 1643.64]  You know how many times a PIR sensor has dropped out of the alarm panel?
[1644.16 --> 1644.48]  Zero.
[1645.68 --> 1646.66]  It's like that kind of stuff.
[1646.72 --> 1647.40]  It's too critical.
[1647.54 --> 1650.96]  I have a water sensor for a very specific spot that I need to watch very closely.
[1651.10 --> 1654.50]  And I don't want the sensor just dropping off the network and not alerting me.
[1654.58 --> 1654.70]  Yeah.
[1655.20 --> 1660.14]  I've even had that problem with Z-Wave, the Z-Wave devices, where like occasionally,
[1660.14 --> 1662.00]  it seems more reliable.
[1662.12 --> 1664.12]  The Z-Wave stuff seems a little more reliable than Zigbee.
[1664.60 --> 1668.58]  But, you know, after a power outage or something weird like that, it's like, oh, look at that.
[1668.66 --> 1671.42]  All the garage Zigbee sensors and stuff.
[1672.04 --> 1674.78]  And then it's like, okay, let me go flip some breakers on and off.
[1674.82 --> 1676.54]  And then I do that and then everything comes back okay.
[1677.44 --> 1677.66]  Yeah.
[1678.02 --> 1682.92]  I have had a Z-Wave device as well drop off where it was like, okay, I don't know what happened.
[1683.06 --> 1683.92]  I'll go reboot it.
[1684.14 --> 1686.42]  And when I do restart it, it tends to bounce back.
[1686.42 --> 1690.86]  But if I don't notice it's offline, the system's not very good about telling me, right?
[1690.94 --> 1694.88]  Home Assistant doesn't make it obvious that something critical has gone offline.
[1695.14 --> 1695.26]  Yeah.
[1695.46 --> 1696.06]  Yeah, exactly.
[1696.60 --> 1701.46]  Meanwhile, the way that the alarm panel is integrated, all of the motion sensors are like,
[1701.52 --> 1703.86]  I last saw motion this time.
[1703.96 --> 1705.46]  I last saw motion this time.
[1705.64 --> 1710.60]  You get constant reassurance that, oh, yeah, everything is connected and working fine and
[1710.60 --> 1711.12]  it's good.
[1711.12 --> 1715.80]  And you could do that kind of thing with other sensors, but, you know, come on.
[1716.30 --> 1716.38]  Yeah.
[1716.66 --> 1720.92]  I have these little IKEA, a listener sent me the correct pronunciation.
[1721.74 --> 1722.10]  Trodfri.
[1722.64 --> 1726.92]  So please, please tell me, Mr. Listener, if I got that right.
[1727.00 --> 1727.92]  The Swedish, you know, the trad.
[1727.94 --> 1728.70]  Could you say it again?
[1729.12 --> 1729.52]  Trodfri.
[1729.94 --> 1730.80]  Something like that.
[1730.90 --> 1731.82]  I think that's what it is.
[1732.44 --> 1733.42]  You know what I mean.
[1733.46 --> 1734.56]  The tradfri buttons, right?
[1734.96 --> 1735.62]  Trodfri, whatever.
[1736.34 --> 1736.70]  Trodfri.
[1736.98 --> 1737.94]  That's what I'm going with.
[1737.94 --> 1740.42]  I've got a bunch of those.
[1740.48 --> 1743.30]  In fact, there's one right here next to me to turn these lights above my head on.
[1743.64 --> 1751.62]  They're all Zigbee and they work 92% of the time, which is just enough to be really frustrating
[1751.62 --> 1755.48]  because you push it and you're like, why didn't that work?
[1755.82 --> 1757.28]  And you push it again and it works.
[1757.34 --> 1758.12]  You're like, God damn it.
[1758.18 --> 1758.42]  Why?
[1758.70 --> 1759.10]  Why?
[1759.62 --> 1761.48]  Why didn't you work the first time?
[1762.60 --> 1763.78]  It's very frustrating.
[1763.98 --> 1767.32]  It's even more embarrassing when a friend or a family member hits the button and nothing
[1767.32 --> 1767.84]  happens.
[1768.30 --> 1769.98]  That's the worst.
[1770.30 --> 1771.12]  I hate that.
[1771.42 --> 1775.26]  So now I thought I'd try and solve it with NFC tags through iOS and you can do the shortcut
[1775.26 --> 1776.64]  automation kind of nonsense.
[1776.92 --> 1778.58]  And they're even worse.
[1778.70 --> 1780.28]  They're even less reliable for some reason.
[1780.42 --> 1782.40]  I can't seem to get the reliable scan.
[1782.72 --> 1789.42]  I don't know if it's just iOS NFC APIs are really finicky or whatever, but there isn't
[1789.42 --> 1797.12]  a good solution really for an always on kind of low megahertz protocol like Zigbee or Z-Wave
[1797.12 --> 1797.66]  should be.
[1797.74 --> 1798.88]  They should be the answer.
[1799.02 --> 1801.78]  They should work, but they just don't.
[1801.84 --> 1803.46]  Where's my quality of service?
[1804.08 --> 1806.50]  Where's my assurance that this is working?
[1806.50 --> 1809.24]  Can I have a button over Ethernet?
[1809.84 --> 1813.64]  But I suppose the other thing you've got to consider is, you know, with a little battery
[1813.64 --> 1816.90]  powered button or something like that, you can't be constantly pinging to say, are you
[1816.90 --> 1817.30]  okay?
[1817.38 --> 1818.02]  Are you okay?
[1818.06 --> 1819.96]  Because that would just, that's the problem.
[1820.58 --> 1821.30]  That is it.
[1821.70 --> 1823.96]  And the always powered stuff does do better.
[1823.96 --> 1829.60]  As a matter of the protocol though, when you hit the button, it should be a two-way thing.
[1829.70 --> 1832.74]  The button sends the thing and gets the acknowledgement back.
[1832.78 --> 1833.26]  I heard you.
[1833.34 --> 1835.28]  Otherwise the button just keeps buttoning.
[1835.48 --> 1835.92]  Yeah.
[1836.32 --> 1836.72]  Yeah.
[1837.32 --> 1837.72]  Yeah.
[1837.72 --> 1839.42]  And same with the sensors like temperature drop.
[1839.54 --> 1844.62]  I wake up and I send notification about temperature drop, but there's also an issue in Home Assistant
[1844.62 --> 1849.20]  where these devices are essentially offline until they wake up to do their job.
[1849.20 --> 1854.52]  And Home Assistant seems to be getting better about that, but it's not fantastic.
[1854.86 --> 1860.82]  And one of the things that can happen is it can say the temperature is 72 degrees Fahrenheit.
[1861.16 --> 1863.96]  And that's the last number that got into Home Assistant.
[1864.16 --> 1868.54]  And if it doesn't wake up and transmit another number for eight hours, Home Assistant just
[1868.54 --> 1872.84]  happily reports 72 degrees and here's your little bar graph and everything's just fine.
[1873.00 --> 1876.12]  And really the reality was the thing dropped off the network for eight hours.
[1876.28 --> 1877.88]  And I'm using mine to monitor my freezer.
[1877.88 --> 1880.88]  And in eight hours you can spoil a freezer, you know?
[1881.10 --> 1881.54]  Yes.
[1882.02 --> 1889.46]  See, it's funny because all of these are things that engineers solved in like the 1970s or 1980s
[1889.46 --> 1890.98]  with these alarm sensors.
[1891.34 --> 1896.72]  And the alarm sensors, like the ones that I'm using are encrypted, but the ones just before
[1896.72 --> 1899.54]  the ones that I'm using were not encrypted.
[1899.92 --> 1904.34]  And you can use software defined radio with those and you don't even have to have the alarm
[1904.34 --> 1905.54]  panel or anything like that.
[1905.54 --> 1907.82]  They actually do periodically check in.
[1907.90 --> 1913.24]  So like the batteries, like the little, the weird little, I don't even, I forget what their
[1913.24 --> 1916.48]  lithium cells, but they're tiny, but they're really thick.
[1917.02 --> 1921.02]  And those last like five years with these sensors.
[1921.02 --> 1925.00]  And it'll send a ping like every 15 minutes or so.
[1925.80 --> 1932.10]  And that the alarm panels will report, you know, a jam or RF interference.
[1932.10 --> 1938.80]  If the sensors don't check in every 15 minutes and same with the water sensors, like it'll set
[1938.80 --> 1940.56]  the, you'll get a trouble light on the panel.
[1940.56 --> 1947.28]  That's like, this is maybe alarm worthy, maybe not, but there is RF interference, or I haven't
[1947.28 --> 1948.82]  heard from this sensor in a while.
[1949.36 --> 1955.92]  And we were doing that when we had like 6502 levels of compute power for these kinds of
[1955.92 --> 1959.40]  things, which shows you how much garbage all of this stuff is.
[1960.32 --> 1961.04]  Yeah, you're right.
[1961.30 --> 1965.98]  Do we assume too much is going to work just because of how reliable TCP IP is?
[1965.98 --> 1971.66]  You know, we, uh, as a generation of engineers haven't grown up with just not working.
[1972.60 --> 1980.28]  We assume too much is, is, should work because TTL Motorola and the TTL, TTL logic was too
[1980.28 --> 1981.08]  damn good.
[1981.60 --> 1983.68]  Yeah, I can see it.
[1984.42 --> 1985.94]  TTL logic was so good.
[1986.00 --> 1987.96]  We could build an entire computer out of it.
[1988.00 --> 1988.62]  The Apple two.
[1989.36 --> 1990.04]  I'm sorry.
[1990.10 --> 1990.84]  The original Apple.
[1991.04 --> 1994.30]  The problem was that we wouldn't put everything on 2.4 gigahertz.
[1994.30 --> 2001.06]  So now everything has to communicate on the same exact channel on the same exact radio
[2001.06 --> 2001.56]  frequency.
[2002.28 --> 2003.78]  Oh, you know, it's crazy though.
[2004.28 --> 2009.22]  Like when you, cause I went down the rabbit hole in this whole IOT thing with radio frequencies
[2009.22 --> 2012.48]  and stuff, and I had no idea, but it really is the case.
[2012.48 --> 2014.52]  Like the physics of it with spread spectrum.
[2015.16 --> 2021.34]  If you have a really well implemented spread spectrum algorithm, the radio frequency bandwidth
[2021.34 --> 2031.72]  is, uh, very high shockingly high for these kinds of, of things, because it's, there's
[2031.72 --> 2036.58]  even a relatively small amount of frequency, the random, random hopping and rapidly random,
[2036.86 --> 2042.30]  randomly hopping at a relatively high frequency, doing those kinds of things on 2.4 gigahertz
[2042.30 --> 2043.58]  absent everything else.
[2043.58 --> 2047.38]  You could almost say that the FCC is getting to the point where it's obsolete.
[2047.76 --> 2051.26]  When our radio technology is a little bit more advanced, the whole spectrum allocation,
[2051.66 --> 2052.18]  blah, blah, blah.
[2052.28 --> 2058.26]  If everything, everything is, is implementing their radio circuit that way, it is a, it is,
[2058.34 --> 2059.00]  it's crazy.
[2059.10 --> 2064.58]  Nothing will interfere with anything else because it's, they're all using a different key to
[2064.58 --> 2066.96]  pick which thing is next for the thing that it's doing.
[2066.96 --> 2068.18]  Ah, I see.
[2068.38 --> 2069.36]  Boy, I hope that happens.
[2069.50 --> 2076.18]  In the meantime, I actually had to physically separate my wifi AP from my, my Zigbee stick
[2076.18 --> 2078.50]  because they were just colliding with each other too much.
[2078.54 --> 2083.62]  And so now I've physically separated the two and my Zigbee network has become more reliable.
[2083.98 --> 2088.86]  It's not solid, solid, not a hundred percent, but it's better now that I've just moved those
[2088.86 --> 2089.64]  two devices apart.
[2089.92 --> 2090.02]  Yeah.
[2090.08 --> 2093.02]  See, having to do that is just, we failed.
[2093.22 --> 2095.94]  Like whatever that technology is, has failed.
[2095.94 --> 2097.26]  That's what it felt like.
[2097.34 --> 2099.28]  It felt like I was doing a stupid, okay.
[2099.36 --> 2099.64]  All right.
[2099.66 --> 2101.12]  Well, all right.
[2101.12 --> 2103.18]  I'll do a layer one fix for this, I guess.
[2103.78 --> 2107.70]  That's like, well, you know, we've got running water, but in order for it to be potable, I
[2107.70 --> 2108.46]  have to boil it.
[2108.54 --> 2110.40]  And it's like, that's not a first world problem.
[2114.34 --> 2116.64]  Linode.com slash SSH.
[2116.72 --> 2120.46]  Go there to get a hundred dollars in 60 day credit on a new account and go there to support
[2120.46 --> 2124.74]  the show while you're checking out Linode, which I think is the best place to host your
[2124.74 --> 2129.48]  stuff, fast, reliable, great support data centers all over the world.
[2129.60 --> 2130.56]  It's what we use.
[2130.62 --> 2131.78]  It's the only thing I'll use there.
[2132.30 --> 2137.40]  There very well may be a way I could save a few bucks for a short period of time by going
[2137.40 --> 2142.38]  to a more fly by the night kind of hosting provider, but that's not what I'm here for.
[2142.42 --> 2144.40]  And I don't, I don't want that hassle.
[2144.96 --> 2146.02]  I want to deploy it.
[2146.06 --> 2146.26]  Right.
[2146.46 --> 2147.52]  I want it to be fast.
[2147.58 --> 2148.80]  I want it to be well supported.
[2149.12 --> 2150.54]  That is Linode.
[2150.54 --> 2152.40]  You can try it with that hundred dollars.
[2152.52 --> 2154.74]  You can really actually try it.
[2154.98 --> 2155.90]  Go see how fast it is.
[2155.96 --> 2161.00]  Try out one of their MVME rigs with a 40 gigabit connection to the internet or one of their dedicated
[2161.00 --> 2163.18]  CPU rigs with AMD epic processors.
[2163.56 --> 2167.38]  And I finally recently had a choice to try out one of their GPU rigs.
[2167.50 --> 2170.06]  I've been satisfied every single time.
[2170.32 --> 2173.40]  That's because they've been doing this for 19 years and they've just been getting better
[2173.40 --> 2174.02]  and better.
[2174.24 --> 2177.06]  Go see the results of that hard work and try it out for yourself.
[2177.28 --> 2179.02]  Support the show and get a hundred dollars.
[2179.02 --> 2182.14]  Go to linode.com slash SSH.
[2182.40 --> 2185.94]  That's linode.com slash SSH.
[2187.72 --> 2190.46]  All right, Alex, do you want to set me straight about notes?
[2190.56 --> 2192.04]  Because we've got, this is the other area.
[2192.12 --> 2192.94]  We got a ton of feedback.
[2193.16 --> 2194.02]  This is my bad.
[2194.54 --> 2198.92]  Evernote got acquired and I set off the alarm bells on the show that I need a note system
[2198.92 --> 2205.42]  that'll be at least something the spouse can use for note capture and OCR of text and
[2205.42 --> 2206.70]  pictures and PDFs.
[2206.70 --> 2210.76]  And I got a lot of feedback and a lot of them, I think are going to tell me what you're going
[2210.76 --> 2211.18]  to tell me.
[2211.88 --> 2215.68]  Well, it's your own damn fault for just dropping it in there and just saying, yeah, I know
[2215.68 --> 2217.02]  Obsidian isn't the solution.
[2217.48 --> 2221.62]  Just casually like one liner with you and Joe last week.
[2221.68 --> 2222.58]  That's your own damn fault.
[2222.92 --> 2223.50]  Yeah, it is.
[2223.62 --> 2224.76]  What about Obsidian with plugins?
[2225.88 --> 2226.66]  There you go.
[2226.66 --> 2228.46]  Exactly, Wendell.
[2228.56 --> 2228.90]  Exactly.
[2229.06 --> 2231.04]  Obsidian is just a plugin engine.
[2231.20 --> 2233.68]  It's like a modern Emacs in a lot of ways.
[2234.40 --> 2242.16]  It's a portal into a whole, dare I say, different dimension of productivity stuff.
[2242.38 --> 2247.12]  You can honestly lose weeks on YouTube just to productivity improvement channels.
[2247.72 --> 2249.52]  Would you have Catherine use it though?
[2249.52 --> 2251.12]  Yeah, I would.
[2251.68 --> 2257.02]  There is a, for example, she currently uses Calibre to manage all of the books that she's
[2257.02 --> 2257.62]  ever read.
[2257.76 --> 2261.90]  She used to use it before that Delicious Library, but that was a Mac only app and then they stopped
[2261.90 --> 2262.52]  supporting it.
[2262.58 --> 2266.94]  So we migrated her over to Calibre and she literally just uses it like a checklist to
[2266.94 --> 2267.98]  say, yes, I've read this book.
[2268.06 --> 2268.64]  No, I haven't.
[2268.72 --> 2269.44]  I own this book.
[2269.54 --> 2271.04]  It's that kind of stuff.
[2271.04 --> 2276.88]  Turns out someone has written a plugin for Obsidian to go to the Google Books API, pull
[2276.88 --> 2280.34]  down the covers, pull down all the information about that particular book, the publishers,
[2280.48 --> 2281.10]  all the rest of it.
[2281.48 --> 2285.78]  And then just with a couple of lines of text, she can, you know, write whether she's, whether
[2285.78 --> 2288.54]  it's in her to read pile or whether she's read it.
[2288.64 --> 2293.96]  And then because it's just plain text, you can do what you like with the rest of the note.
[2294.20 --> 2295.72]  You know, it's just a plain text file.
[2295.80 --> 2296.66]  You can write a review.
[2296.84 --> 2297.86]  You could write spoilers.
[2298.04 --> 2299.76]  You could do whatever you want in there.
[2299.76 --> 2305.44]  And that's just one example of how flexible just having a plain text system that is somewhat
[2305.44 --> 2311.56]  kind of self-aware can do with the plugin ecosystem that it has.
[2312.24 --> 2316.34]  And the other thing that really grabbed my attention, I heard you mention was talking
[2316.34 --> 2318.66]  about PDFs and OCR and that kind of thing.
[2319.18 --> 2321.18]  It can do that obviously via a plugin, of course.
[2321.72 --> 2325.54]  There are different ways you can do this and you can do it all locally.
[2325.92 --> 2327.54]  I forget the name of the framework, unfortunately.
[2327.84 --> 2329.34]  If I find it, I'll put it in the show notes.
[2329.76 --> 2335.24]  But there are some people who swear by the Microsoft Azure cloud OCR stuff.
[2336.14 --> 2340.42]  And you can actually, if you're doing, I think, 300 documents or less a month or something
[2340.42 --> 2342.66]  like that, it might even be something like 4,000.
[2342.74 --> 2343.72]  I forget the exact number.
[2344.12 --> 2344.52]  Okay.
[2344.86 --> 2345.56]  Quite a difference.
[2345.70 --> 2345.92]  I know.
[2345.92 --> 2346.12]  Yeah.
[2346.12 --> 2346.14]  Yeah.
[2346.34 --> 2348.76]  But easily, it wouldn't even be more than a dozen.
[2349.18 --> 2349.50]  Right.
[2350.02 --> 2356.34]  So essentially, you can use the Azure OCR stuff and not even have to do any local processing.
[2356.34 --> 2361.30]  Although modern devices are so good, particularly with the neural engines and that kind of stuff,
[2361.78 --> 2363.76]  that it shouldn't really be too much of an issue.
[2363.76 --> 2370.46]  I use Office Lens and OneNote and then paste from that into the other thing because you can do the,
[2370.46 --> 2372.44]  just got the document camera and everything else.
[2372.44 --> 2376.22]  And then you're just, you know, and then you're good to go.
[2376.56 --> 2380.74]  There's also a, there's a plugin for Obsidian or NextCloud.
[2380.98 --> 2384.80]  There's a way to get the NextCloud's note-taking document management thing.
[2384.80 --> 2387.08]  And also talking to Obsidian.
[2387.42 --> 2388.22]  Oh, really?
[2388.74 --> 2389.66]  That sounds perfect.
[2389.72 --> 2392.76]  I haven't done that yet, but there's a thread about it on the forum because we had a,
[2392.82 --> 2393.44]  I did a video.
[2393.72 --> 2396.00]  It's the magic words are Zettelkasten.
[2396.18 --> 2396.46]  Yes.
[2396.58 --> 2403.88]  It was like, use like, so this is Zettelkasten is probably the closest way to describe what I do
[2403.88 --> 2404.88]  for knowledge capture.
[2405.24 --> 2410.50]  And it, it, it, it originates from a guy that literally used index cards, like a card catalog
[2410.50 --> 2412.22]  to make notes.
[2412.22 --> 2415.36]  And it's not note notes.
[2415.40 --> 2416.74]  It's really index notes.
[2416.88 --> 2423.16]  So when you read a book and you know, you're making notes in, in, in, in the margins or
[2423.16 --> 2428.92]  whatever, and if it's a dead tree book, you also make those notes on a, on a card or you
[2428.92 --> 2433.46]  just say, Hey, this page in this book is about this thing that I've encountered before that
[2433.46 --> 2434.36]  I'm probably going to need.
[2434.52 --> 2439.18]  If I were reading, say one of Michael Lucas's book about books about ZFS and it's like, Oh,
[2439.18 --> 2444.76]  this is something that I've encountered in the past that, uh, I needed reference information
[2444.76 --> 2445.20]  for.
[2445.38 --> 2451.64]  So then I would write the words that I know that I'll search later and a link to where
[2451.64 --> 2454.94]  that is or a note of what page that is in the dead tree book.
[2454.94 --> 2457.94]  And it's like, Oh, this is in advanced ZFS page 37.
[2457.94 --> 2460.70]  And this is the keywords that go with that.
[2461.04 --> 2464.86]  And then when I'm in obsidian or anything and I'm searching, it's like, boom, here's all
[2464.86 --> 2467.24]  the, here's all the things that match that.
[2467.30 --> 2471.14]  And it's like, okay, here are my own personal notes of the times that I've encountered these
[2471.14 --> 2476.06]  things and links to them either in document format or even in dead tree format.
[2476.06 --> 2482.38]  And if you're willing to put your notes in a specific directory format, you can actually
[2482.38 --> 2488.92]  link all of this kind of backlinking, Zettelcast and style stuff, link it together with MK docs.
[2489.08 --> 2492.76]  And so this is what I do for all of my personal home documentation at the moment.
[2492.98 --> 2500.10]  It goes through a drone CI, a Docker container, and then spits out just a simple, um, static
[2500.10 --> 2504.08]  website, which then an NGINX container takes care of the actual hosting for me.
[2504.08 --> 2510.26]  And the nice thing about that is obsidian has a sync service, which they charge, I think,
[2510.30 --> 2512.74]  $8 a month for it used to be four.
[2512.96 --> 2514.56]  And that was already in my mind expensive.
[2514.56 --> 2518.54]  And then they doubled it to eight same for their published service as well.
[2518.68 --> 2526.36]  So they provide all the tools you would need as a non self hosting geek to go out and publish
[2526.36 --> 2531.30]  your notes and to sync your notes between iOS and Mac and Linux and blah, blah, blah.
[2531.30 --> 2537.62]  But the nice thing about doing it with MK docs and keeping it all local is it's free.
[2538.00 --> 2542.84]  And the plugin that I use is self-aware of all the backlinks that are going on.
[2542.96 --> 2545.58]  So even in the webpage, it generates in the static site.
[2545.90 --> 2552.30]  It has all the kind of clever backlinks to all the different subtopics about XYZ.
[2553.44 --> 2553.52]  Yeah.
[2553.52 --> 2558.46]  I think obsidian is one of those things you can, you can just use it like a dumb plain text
[2558.46 --> 2561.16]  folder structure if you want to, just to get started.
[2561.48 --> 2564.96]  You could also then jump in and start adding tags to things.
[2565.10 --> 2570.58]  So you could have it appear in multiple places at once, which long time listeners might remember.
[2570.74 --> 2576.48]  That's why I really liked Tiddlywiki is because I could have one note appear in multiple places
[2576.48 --> 2580.72]  when actually the right thing to do is what Wendell was saying is have an index card for
[2580.72 --> 2586.32]  that topic and then have like a list of all the places that that topic should appear or
[2586.32 --> 2588.78]  whatever, like a cheat sheet for that topic.
[2589.48 --> 2593.82]  But that's my point about obsidian really is you can start super simple and then you can
[2593.82 --> 2598.40]  just add and iterate and everybody's note taking process and everybody's thinking processes
[2598.40 --> 2598.98]  are different.
[2599.58 --> 2603.90]  And I think that's what makes obsidian in particular different from all the rest.
[2603.90 --> 2606.16]  It's, it's not really opinionated.
[2606.80 --> 2607.20]  Okay.
[2607.30 --> 2612.68]  The, the initial simple text editor is a little opinionated, tiny, tiny little bit.
[2612.92 --> 2613.32]  Okay.
[2613.46 --> 2618.06]  But you know, if you want to take it further, you know, for Hadir or whatever, you know,
[2618.06 --> 2620.38]  that's, it's the only game in town.
[2620.42 --> 2624.02]  I mean, I know there's log sec and some people really, really like that one, but yeah.
[2624.20 --> 2624.48]  Yep.
[2624.86 --> 2630.28]  For me, obsidian is the, the first mover advantage in the, uh, in the plugin space.
[2630.46 --> 2631.74]  I like that you can build up.
[2631.74 --> 2635.40]  I had a good luck with the, the get plugin also for synchronization.
[2635.80 --> 2636.66]  Oh yes.
[2636.90 --> 2637.04]  Yeah.
[2637.08 --> 2637.16]  Yeah.
[2637.16 --> 2638.26]  Oh, that does sound nice.
[2638.38 --> 2640.66]  So that's how I trigger the drone CI container.
[2640.80 --> 2646.72]  I've got a keyboard shortcut bound to command shift G that does get that pushes it to get
[2646.72 --> 2647.72]  and then drone picks it up.
[2647.76 --> 2650.72]  It also syncs every five minutes automatically when it's open as well.
[2651.06 --> 2651.50]  All right.
[2651.52 --> 2657.54]  Well, we did get a lot of mentions for notion, uh, L re or L re 741 boosted in with a row of
[2657.54 --> 2660.70]  ducks and said, I personally use notion right now.
[2660.70 --> 2662.06]  And it's so versatile.
[2662.56 --> 2665.62]  I've been using it for daily work diary entries.
[2665.86 --> 2668.16]  As I learned to do different programming.
[2668.34 --> 2671.14]  I haven't tried its OCR, but they have an API.
[2671.52 --> 2673.52]  So maybe somebody has built something for it.
[2673.60 --> 2678.50]  I don't remember where I heard about it from, but also app flowy.io is supposed to be an open
[2678.50 --> 2681.68]  source alternative to notion might be worth checking out.
[2682.04 --> 2685.82]  Now, Alex, I know you gave a real serious look at notion, even though it wasn't necessarily
[2685.82 --> 2686.76]  self-hosted.
[2686.76 --> 2688.12]  Notion is fantastic.
[2688.90 --> 2693.34]  I don't really have very many things to say about it, apart from the fact that I don't
[2693.34 --> 2693.98]  own the data.
[2694.38 --> 2695.64]  What do you think about app flowy then?
[2695.72 --> 2700.50]  If it's an open source self-hosted notion, is that worth my time?
[2700.56 --> 2702.58]  Do you think, or should I just not bother with this stuff?
[2702.86 --> 2704.66]  You should take a look at it and report back.
[2704.78 --> 2705.86]  That's your homework, sir.
[2706.20 --> 2706.92]  All right.
[2708.20 --> 2708.88]  All right.
[2708.92 --> 2709.32]  I will.
[2709.50 --> 2711.38]  That's the stuff that I get sucked into too.
[2711.38 --> 2716.54]  It's like, okay, because I had a media wiki for some things set up and it was like, this
[2716.54 --> 2716.98]  is great.
[2717.08 --> 2719.90]  And then it got just large and complicated enough.
[2719.98 --> 2722.58]  It's like, okay, now how do I merge this back in?
[2722.86 --> 2727.08]  And so I still have a media wiki thing, which is like, oh, what was that thing?
[2727.14 --> 2727.84]  It was like, oh, right.
[2727.86 --> 2729.06]  It's in the media wiki instance.
[2729.14 --> 2733.12]  And then it's like, I was like, I really, it's on the to-do list to fix that someday.
[2733.38 --> 2734.20]  But I don't know.
[2734.20 --> 2740.54]  So yeah, I think over the years I've accumulated a bunch of, you know, when I was on iOS the
[2740.54 --> 2744.52]  first time in 2012, I've got some Apple notes from 2012.
[2744.84 --> 2747.86]  I then got some simple notes that I used to use for a long time.
[2748.10 --> 2751.00]  And then I moved to notational velocity for a little while.
[2751.00 --> 2756.52]  And then I moved to something out and I've got stuff scattered everywhere.
[2756.52 --> 2760.10]  And it's just, it's not, it's not nice.
[2760.18 --> 2760.80]  It's not manageable.
[2760.80 --> 2764.70]  Whenever I think, oh, where, where did I write down the serial number for that motherboard?
[2764.98 --> 2767.16]  I think, oh God, which app did I put that into?
[2767.28 --> 2768.66]  Because when, when did I buy it?
[2769.62 --> 2770.60]  Yeah, I know.
[2770.64 --> 2772.06]  Or, and in my case, Evernote too.
[2772.62 --> 2776.62]  Nomadic Coder sent 1,555 sats to say on an Evernote replacement.
[2776.62 --> 2778.70]  And this is probably the number one I heard.
[2779.16 --> 2780.64]  So I'm curious to know what you think about this.
[2781.30 --> 2783.80]  Try Joplin with Nextcloud.
[2783.94 --> 2786.40]  I moved from Evernote and was happy with that.
[2786.66 --> 2788.12]  It syncs using Nextcloud.
[2788.12 --> 2794.60]  What Nomadic Coder has here is probably what I've heard the most is Joplin with Nextcloud.
[2795.40 --> 2801.86]  I'm tempted to try that, but I'd have to rely on Nextcloud to do some of the optical character recognition stuff it looks like.
[2802.32 --> 2804.92]  So I'd be going even deeper into Nextcloud land.
[2805.50 --> 2806.72]  Yeah, Joplin's fine.
[2806.72 --> 2812.38]  I mean, it's, um, it's sync has lost me data in the past, which I think we covered on this show even.
[2812.94 --> 2818.70]  And that was what I, what kind of forced me towards the notion angle is whilst I was writing some articles for Ars Technica.
[2818.86 --> 2822.44]  So I was quite cheesed off when all that work disappeared on me.
[2823.24 --> 2823.60]  I recall.
[2824.14 --> 2824.46]  All right.
[2824.46 --> 2825.44]  That was Joplin, huh?
[2825.70 --> 2825.94]  All right.
[2825.94 --> 2826.64]  That was Joplin.
[2826.64 --> 2833.04]  I mean, it only happened one time, but much like Zigbee, one time is one time too many.
[2833.62 --> 2837.52]  I don't feel like I live in a first world country when these things happen.
[2837.70 --> 2838.60]  I know, right?
[2839.06 --> 2840.62]  Data loss is not acceptable.
[2841.42 --> 2842.44]  Well, here's the last note.
[2842.68 --> 2845.64]  DJ boosted in with 69,420 sats.
[2845.70 --> 2847.60]  Hey, I wonder if there was a message there.
[2847.78 --> 2848.12]  Nice.
[2848.62 --> 2851.10]  Hot boost coming in from an OG SRE.
[2851.28 --> 2852.92]  Glad to hear that Joe was on the show.
[2853.12 --> 2853.56]  Yeah, yeah.
[2853.56 --> 2862.08]  Joe and I had, by the way, a good ZFS versus ButterFS discussion in the members post show, which was spicy.
[2862.26 --> 2863.32]  What is there to discuss?
[2866.14 --> 2868.04]  ButterFS is better, isn't it?
[2868.16 --> 2868.50]  Oh, yeah.
[2868.62 --> 2868.80]  I know.
[2869.70 --> 2872.00]  Why can't we have both is my version.
[2872.16 --> 2876.10]  Why can't I put ButterFS on my root and ZFS on my data?
[2876.38 --> 2877.98]  That's my position.
[2878.68 --> 2881.58]  I feel like maybe ButterFS for a Raspberry Pi.
[2881.58 --> 2890.10]  But then, of course, after I said that, I saw somebody release an article about how well ZFS seems to work on the Raspberry Pi 4.
[2890.10 --> 2892.02]  So I got to try it.
[2892.08 --> 2897.44]  I really do have to try it because I've only ever tried ButterFS on the Raspberry Pi and I've never tried ZFS on the Raspberry Pi.
[2897.58 --> 2900.72]  I just wish we could get over this licensing bollocks, don't you?
[2901.02 --> 2901.20]  Yeah.
[2901.20 --> 2901.38]  Yeah.
[2901.66 --> 2902.46]  That would solve it.
[2902.94 --> 2904.86]  That certainly would be nice, wouldn't it?
[2905.72 --> 2906.12]  Maybe.
[2906.32 --> 2907.34]  Maybe in 2035.
[2907.74 --> 2914.70]  I just think anytime anybody asks me about something at work and I've got my corporate hats on, I'm like, oh, just use ZFS.
[2914.70 --> 2917.36]  Oh, no, no, you can't recommend that today, Alex.
[2917.46 --> 2917.64]  Nope.
[2917.82 --> 2918.02]  Nope.
[2918.08 --> 2919.44]  Have to do the company thing.
[2919.92 --> 2920.28]  That's true.
[2920.34 --> 2922.72]  You're working for the company that's trying to come up with Stratus.
[2922.82 --> 2923.82]  I mean, that's never going to.
[2924.10 --> 2925.28]  Well, that's IBM now.
[2925.34 --> 2926.58]  All the storage stuff has moved.
[2927.00 --> 2928.24]  I'm sure you saw that news.
[2928.48 --> 2928.82]  Yeah, yeah.
[2928.82 --> 2929.08]  Okay.
[2930.00 --> 2931.74]  I've actually been having a lot of fun.
[2931.94 --> 2935.90]  I've been, you know, the whole home setup, re-architecting some things.
[2936.36 --> 2938.40]  And it's like Proxmox versus XCPNG.
[2938.40 --> 2941.22]  And I'm just over here like, you know, OpenShift is a thing.
[2941.66 --> 2943.40]  We can do a lot with OpenShift.
[2944.28 --> 2945.42]  OpenShift is pretty cool.
[2946.24 --> 2947.68]  Ceph is a pretty easy setup.
[2947.82 --> 2949.24]  Like, let's go hyperconverge.
[2949.30 --> 2950.06]  This is fine.
[2950.28 --> 2952.28]  I can run it on 16 servers for free.
[2952.38 --> 2953.06]  Let's just do it.
[2953.58 --> 2959.22]  I think you would need your head examining if you wanted to run OpenShift at home just for a home workload, to be honest.
[2959.38 --> 2960.90]  Don't you have OpenShift at home?
[2961.00 --> 2961.62]  Come on.
[2961.86 --> 2963.14]  No, I mean, I used to.
[2963.34 --> 2966.34]  But then, I don't know, I just, I like my stuff working.
[2966.48 --> 2966.94]  You know what I mean?
[2966.94 --> 2970.66]  That says something about my abilities as an admin more than OpenShift.
[2972.72 --> 2979.48]  Yeah, and probably my preference to have ButterFS on my Raspberry Pis than ZFS.
[2979.70 --> 2985.66]  I've managed to make a career out of telling people how to install OpenShift and architect all the various different NCD nonsense.
[2986.22 --> 2989.72]  As soon as the cluster's up and running, I'm kind of like, all right, that's your thing now.
[2990.48 --> 2992.56]  Somebody else's problem at that point, right?
[2992.96 --> 2993.20]  Yeah.
[2993.50 --> 2993.94]  Exactly.
[2994.10 --> 2994.50]  How do I get that gig?
[2994.58 --> 2995.80]  That's what the SREs are for.
[2996.04 --> 2996.52]  Yeah.
[2996.94 --> 2999.88]  Thank you to our SREs, too.
[3000.40 --> 3004.16]  You can become a member over at selfhosted.show slash SRE.
[3004.26 --> 3007.16]  You do get that post show and an ad-free version of the show.
[3007.34 --> 3008.80]  And thank you to everybody who boosts in.
[3008.86 --> 3009.78]  There was more boosts.
[3009.96 --> 3012.20]  But, of course, we're trying to keep it nice and tight these days.
[3012.40 --> 3017.52]  But you can grab a new podcasting app at newpodcastapps.com to send a boost into the show as well.
[3017.74 --> 3020.32]  And we'll have some more there in the future.
[3020.32 --> 3024.62]  And last but not least, a big thank you to Wendell for joining us this week.
[3024.66 --> 3026.16]  Wendell, it was great to catch up with you.
[3026.16 --> 3027.10]  It was great.
[3027.50 --> 3030.18]  And so much exciting hardware stuff happening.
[3030.32 --> 3031.04]  It's magical.
[3031.44 --> 3031.98]  It is great.
[3031.98 --> 3035.22]  I feel like, I mean, we didn't even touch on Intel Arc at all.
[3035.34 --> 3037.52]  Maybe we'll save that for the post show for our members.
[3037.74 --> 3038.30]  Oh, right.
[3039.58 --> 3040.56]  Let's do that.
[3040.74 --> 3042.12]  I do definitely want to talk about that.
[3042.16 --> 3044.08]  There's just so much stuff going on at the minute.
[3044.08 --> 3051.92]  It's after the last couple of years of hardware just being jacked because of crypto and COVID supply chain stuff.
[3052.28 --> 3057.80]  It's so amazing that I am seriously considering building a desktop computer for the first time in five years.
[3058.12 --> 3059.22]  It's very exciting.
[3059.86 --> 3060.30]  That's nice.
[3060.54 --> 3061.10]  That is nice.
[3061.24 --> 3061.92]  Good for you, Alex.
[3061.96 --> 3062.86]  I'd love to hear about that.
[3063.14 --> 3063.74]  And you know what?
[3063.78 --> 3066.18]  I also love to hear from everybody out there listening to the show.
[3066.28 --> 3068.26]  They can go to selfhosted.show slash contact.
[3068.56 --> 3070.30]  That's the way to get a hold of us.
[3070.82 --> 3072.60]  And we usually point people towards Twitter.
[3072.60 --> 3074.68]  But I have no idea if it's going to be around next week.
[3074.84 --> 3076.68]  So, you know, who knows?
[3076.86 --> 3079.80]  But if it's still there, I'm there at ironicbadger.
[3079.94 --> 3083.06]  Where's the Go-based open source clone of Twitter?
[3083.38 --> 3084.10]  Go or Rust?
[3084.34 --> 3085.22]  I'll take either.
[3086.00 --> 3086.26]  Yeah.
[3086.82 --> 3089.22]  Something I can just run as a single binary on my server.
[3089.36 --> 3089.96]  That'd be great.
[3090.70 --> 3093.34]  I guess in the meantime, find me on the Matrix Fediverse.
[3094.24 --> 3095.70]  jupiterbroadcasting.com slash matrix.
[3096.18 --> 3098.74]  I have also signed up for that Mastodon thing.
[3098.74 --> 3104.02]  So if that's of interest to you, there'll be a link in the show notes of where to find me.
[3104.14 --> 3109.12]  I'm still not fully sure how to tell people how to find me on Mastodon yet.
[3109.48 --> 3110.72]  So go to it, Alex.
[3110.76 --> 3111.48]  You got to go to it.
[3111.54 --> 3112.38]  I've got to go to it.
[3112.44 --> 3112.60]  Have I?
[3112.70 --> 3113.78]  Is that not truth social?
[3114.02 --> 3114.34]  Is that not?
[3114.54 --> 3114.88]  No, no.
[3115.02 --> 3115.88]  No, those are truths.
[3116.04 --> 3117.00]  I've got to re-truth.
[3117.22 --> 3117.50]  Okay.
[3117.62 --> 3118.58]  That's on truth social.
[3118.66 --> 3120.78]  Then you got toots on Mastodon, which...
[3120.78 --> 3121.68]  What a load of nonsense.
[3121.94 --> 3122.64]  Isn't that adorable?
[3122.96 --> 3126.56]  I mean, tweets was already silly enough, but that's just a word now, isn't it?
[3126.56 --> 3126.76]  Yeah.
[3127.54 --> 3128.16]  All right, everybody.
[3128.28 --> 3130.58]  Thanks so much for joining us on this episode of Self Hosted.
[3130.82 --> 3133.94]  This has been selfhosted.show slash 85.
