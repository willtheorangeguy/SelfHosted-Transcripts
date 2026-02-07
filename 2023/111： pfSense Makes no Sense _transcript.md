[0.00 --> 3.38]  We've made it episode 111, which feels like a special number.
[3.56 --> 8.20]  I don't know why, but I do know, Alex, that we have a special guest for episode 111.
[8.54 --> 8.94]  Yes, we do.
[9.00 --> 13.40]  I'm delighted to welcome Wolfgang of Wolfgang's Channel fame from YouTube to the show.
[13.46 --> 13.88]  Hi, Wolfgang.
[13.94 --> 14.38]  How are you?
[14.60 --> 14.82]  Hello.
[14.90 --> 15.40]  I'm doing great.
[15.44 --> 15.82]  How are you?
[16.14 --> 17.74]  Yeah, I'm feeling the Christmas spirit.
[17.88 --> 18.48]  I'll tell you what.
[18.60 --> 21.48]  It's well, as this airs, it's December somehow.
[21.80 --> 24.08]  I don't know how that's possible, but time flies.
[24.18 --> 24.38]  Yes.
[24.92 --> 25.98]  Oh, it's definitely time travel.
[25.98 --> 30.92]  Did you manage to stop in the middle of the time travel and get any sweet Black Friday deals?
[31.28 --> 31.86]  There were a few.
[32.00 --> 34.14]  Yeah, I got a standing desk frame.
[34.52 --> 41.36]  So a couple of years ago, I bought a fully Jarvis bamboo desktop for like 50 bucks on Facebook Marketplace.
[41.80 --> 45.98]  And I've been keeping my eye out for a decent deal on a standing desk frame basically since then.
[46.16 --> 53.22]  And I built a wooden frame out of two by fours, which has been serving our guest room for the last three years.
[53.22 --> 57.62]  Anyway, I found a FlexiSpot desk for 150 bucks, which is a sit-stand desk.
[57.70 --> 58.94]  And I was like, yep, that's the one.
[59.02 --> 59.52]  That's the ticket.
[60.18 --> 62.56]  And then I thought, right, I'm pretty much all done with Black Friday.
[62.80 --> 74.36]  The deals this year weren't, I don't know, they didn't feel like they were anything spectacular outside of the 18 terabyte Best Buy hard drives for 200 bucks a pop, which was pretty good.
[74.64 --> 77.66]  But there were some crucial SSDs went on sale.
[78.62 --> 81.30]  $165 for a four terabyte SATA SSD.
[81.80 --> 82.06]  Nice.
[82.06 --> 83.64]  I was looking at that one.
[84.00 --> 93.06]  So I picked up three of those to throw them into a RAID Z1 just to try and see if I could actually do video editing over that fancy new 10 gig network I built in the spring.
[93.56 --> 95.30]  So that'll be interesting to see.
[95.52 --> 100.64]  I ran into, I was doing some speed tests using FIO and stuff like that locally on the box.
[100.64 --> 106.90]  And I ran into some issues where I exhausted the cache on those drives after about 30 or 40 seconds.
[106.90 --> 112.96]  So I'm able to max, basically max out my 10 gig line for about 30 or 40 seconds.
[112.96 --> 118.00]  And then it drops between those three drives to only about, only about 300 or 400 megs a second.
[118.36 --> 124.48]  So I guess that would work if say you're in the scenario you're editing, you might burst while you're scrubbing.
[124.94 --> 125.18]  Right.
[125.22 --> 127.10]  You could see it might work for that scenario.
[127.28 --> 127.44]  Right.
[127.44 --> 133.24]  And then when you're normally just playing back and editing and stop, make an edit, play, play, stop, make an edit.
[133.40 --> 134.68]  That sounds like it's going to be plenty of bandwidth.
[135.10 --> 135.26]  Yeah.
[135.50 --> 136.98]  I mean, Wolfgang, you'll know.
[137.30 --> 144.08]  Whenever you're ingesting a bunch of footage after you've shot a video, that can easily be 100 gigs worth of footage out of a decent camera.
[144.50 --> 144.90]  Absolutely.
[144.90 --> 151.58]  So throwing that kind of data around a network, you know, it didn't used to be a problem for me, but now I'm a small time YouTuber.
[154.18 --> 154.70]  Yeah.
[154.86 --> 159.74]  I actually record in, I have an Atomos Ninja 5 recorder, so I record in ProRes.
[160.28 --> 162.76]  So my videos, the folders do get pretty big.
[162.84 --> 163.00]  Yeah.
[163.56 --> 171.28]  But I've actually discovered that a RAID Z array of SATA SSDs is actually enough for me, like two edits in DaVinci Resolve at least.
[171.28 --> 176.40]  I also have a 10 gig setup with SFV plus, I think, in my case.
[177.30 --> 188.42]  And I don't know if it's the DaVinci Resolve cache that, you know, that's built like locally or if the SATA SSDs are just enough for that kind of workflow, but I've never had any issues really.
[188.72 --> 190.52]  I think that you're using ZFS, right?
[190.74 --> 190.96]  Right.
[191.06 --> 191.20]  Yeah.
[191.40 --> 192.10]  For SSDs, yes.
[192.40 --> 194.04]  And so there'll be a bunch of caching going on.
[194.04 --> 201.12]  And, you know, when you're editing a specific project, ZFS is pretty good about caching those specific things.
[201.70 --> 203.46]  So I think there's probably some of that going on.
[203.78 --> 208.72]  And I'll be curious to know if you've ever exhausted the RAM cache on that kind of thing.
[209.42 --> 214.92]  Because one of the things I'm tempted to do is throw an NVMe in front of these SATA SSDs as like a ZIL or something.
[215.46 --> 216.20]  Or maybe not a ZIL.
[216.30 --> 217.44]  What am I thinking of?
[217.52 --> 218.02]  A ZIL, right?
[218.08 --> 218.98]  Slog, right?
[219.30 --> 219.90]  Yeah, maybe.
[220.02 --> 220.14]  Yeah.
[220.14 --> 221.68]  Like the front end cache, basically.
[222.58 --> 224.18]  So, you know, that's an option.
[224.82 --> 227.20]  So, yeah, we're talking about ZFS and servers and stuff like that.
[227.20 --> 229.68]  So let's not beat around the bush any longer.
[230.00 --> 234.72]  I thought I'd bring you on today to talk about basically the stuff you talk about on your YouTube channel.
[234.72 --> 236.32]  Because I find it absolutely fascinating.
[236.92 --> 241.10]  All the low power server stuff, hardware transcoding, all that kind of stuff.
[241.10 --> 254.92]  So I think one of the first videos of yours that I saw was one where you were going deep, deep, deep down into like sleep states of CPUs to try and get the absolute lowest power drawer of a CPU that you could.
[255.66 --> 255.76]  Right.
[255.76 --> 259.86]  I've heard that that's a gateway drug video for a lot of people, actually.
[260.66 --> 261.80]  So what are you running right now?
[261.86 --> 263.14]  What's your primary home server today?
[264.00 --> 271.72]  I actually kind of have a scuff setup because for me, my home server is sort of a playground where I test a lot of the stuff that comes in the next videos.
[272.20 --> 279.40]  I found that basically this is kind of, this gives me a better chance to test hardware than just some kind of a test bench setup.
[279.40 --> 285.76]  So my home server setup changes pretty much every couple of months.
[286.28 --> 290.74]  But currently I have an Azzerok C236 motherboard.
[291.26 --> 301.60]  It's a Kaby Lake, Skylake slash Kaby Lake motherboard with eight SATA ports, which is pretty crazy considering it's a mini ITX board with eight SATA ports.
[301.92 --> 302.48]  No, I'm dead to you.
[302.78 --> 305.58]  But I mean, eight SATA ports more than compensate for that, I find.
[305.58 --> 318.86]  And I also have a Pentium, I'm forgetting the exact name right now, but it's basically the Kaby Lake Pentium, like dual core, four threads, and 32 gigs of SDC RAM.
[319.50 --> 320.68]  So that's basically my setup right now.
[321.38 --> 323.26]  There's a name I didn't hear in a while, Pentium.
[323.66 --> 324.48]  Yeah, I know, right?
[325.52 --> 327.74]  So what's the energy draw like on that kind of thing?
[328.18 --> 333.16]  Right now, I actually checked before the podcast, I think it's around 14 watts at idle.
[333.16 --> 343.82]  So that also has a Bly KVM, which is sort of like this Pi KVM thing that sort of plugs into PCIe, but not really.
[344.00 --> 345.80]  It's just, it's all a lie.
[346.10 --> 347.68]  There is no PCIe connectivity in this thing.
[348.72 --> 352.42]  And it's powered by CM4, so Raspberry Pi Compute Module 4.
[352.42 --> 366.08]  Yeah, so obviously with this as a USB HID and HDMI, it does consume 14 watts, plus three Seagate XS drives, 7200 RPM, four WD-Rate SSDs.
[366.16 --> 368.18]  How did you get all that into 14 watts?
[368.24 --> 369.38]  They must be spun down, right?
[369.46 --> 370.70]  Of course, of course, yes.
[370.76 --> 371.02]  Okay.
[371.02 --> 373.04]  So that's kind of the catch here, right?
[374.52 --> 382.56]  And an Intel X710 DA2, so that's a 10 gigabit SFP Plus networking card.
[382.94 --> 394.84]  It's one of the few SFP Plus cards that do support those lower power efficient PCIe states, which turns out it's kind of not very common, I guess, in the server space.
[394.84 --> 400.06]  Yeah, because I threw a bunch of Mellanox cards in mine, because I think they were like $40 each.
[400.22 --> 401.38]  I mean, that's another thing, right?
[401.44 --> 403.08]  So how expensive was the Intel card?
[403.56 --> 406.54]  I think I got it for around 100 euros used.
[406.70 --> 406.96]  Okay.
[407.18 --> 408.22]  It's not too bad, I guess.
[408.54 --> 409.72]  So it's definitely not 40 euros, yes.
[409.72 --> 415.58]  I wonder what the ROI is, because I know electric prices are a bit higher in Europe these days than over here.
[415.58 --> 426.42]  I wonder what the ROI is on a Mellanox card at $40 versus an Intel card at, what's that, $110, $120-ish, something like that.
[427.02 --> 433.28]  So for most of the stuff that I cover, at least for me, the ROI is just terrible.
[433.28 --> 447.50]  I would not recommend, you know, just hopping from, like, one setup to another and, like, buying stuff, you know, buying 100 euros, like, networking cards in hope that maybe, maybe you'll be able to shave off, like, 2, 3 watts or something.
[449.26 --> 462.92]  But in terms of an ROI for an actual person who's deciding between the Mellanox, well, let's say Mellanox Connect X3 and the Intel X710, I think it would, like you said, it would definitely depend on the power and the energy prices.
[462.92 --> 469.48]  So in Germany right now, we pay around 30 cents per kilowatt, which it's not too great, not too terrible.
[470.76 --> 477.80]  But I guess you would actually be able to reimburse that within five years, I want to say, five, six years.
[478.32 --> 487.08]  Yeah, and, you know, our co-host, Chris, loves him some Raspberry Pis, particularly in his RV, because they're all low power stuff, you know, running off battery, all that kind of stuff.
[487.08 --> 496.94]  And I'm always badgering him to say that the small form factor, like one liter PCs, you know, the x86 is still a better value proposition.
[497.54 --> 501.28]  Because, you know, the ROI on just, you know, even three, four, five watts, something like that.
[501.72 --> 504.84]  But obviously, Chris has the constraint of being on battery power.
[505.16 --> 507.34]  Yeah, maybe I should just add more batteries, I suppose.
[508.62 --> 510.26]  That's such an American answer.
[510.26 --> 517.94]  No, it's actually one of the reasons why I've been closely watching what my options are for media encoding that are low power.
[518.16 --> 523.20]  And I saw that, Wolfgang, you did a video on the Intel Arc for a media server.
[523.28 --> 529.90]  And I don't know if that, I'm curious to A, to know what you, where you think the Arc compares in terms of PowerDraw to other GPUs of a similar class.
[529.90 --> 536.48]  And I'd be interested to know if you experimented with the Arc with Jellyfin and maybe hardware encoding with Jellyfin.
[536.94 --> 537.34]  Right.
[537.42 --> 551.74]  So that's actually a great question, because I was actually very excited seeing that one post on Reddit that claimed that basically the person who made that post claimed that they were able to get their Intel Arc card to one watt power consumption.
[552.16 --> 553.94]  So I was like, that's a smoking gun.
[554.04 --> 557.76]  You know, if that's, if that's true, I'm buying a bifurcating riser I'm putting into an Arc.
[558.56 --> 559.38]  Right, exactly.
[559.38 --> 559.72]  Yeah.
[559.90 --> 560.70]  Is it true, though?
[560.94 --> 561.60]  Unfortunately, no.
[561.60 --> 567.26]  Unfortunately, that turned out to be, I guess, a software power metering issue.
[567.48 --> 569.98]  So they didn't use a hardware power meter.
[570.10 --> 571.88]  They used like some, some kind of software setup.
[572.14 --> 579.58]  They basically mistook the core power consumption with like the, the whole thing power consumption.
[579.74 --> 580.46]  The entire card.
[580.76 --> 580.84]  Right.
[581.06 --> 582.16]  Common, common mistake.
[582.38 --> 583.42]  Rookie mistake, I would say.
[583.84 --> 587.14]  Yeah, it's pretty, it's pretty easy to do if you look in Intel GPU top or whatever.
[587.14 --> 589.12]  Like it gives you a little wattage number at the top.
[589.12 --> 593.82]  But that doesn't take into the entire, that doesn't take the entire package into consideration.
[594.08 --> 594.10]  Yeah.
[594.10 --> 594.38]  Let alone.
[594.38 --> 597.74]  There's a lot of chips and fans and everything else on that motherboard.
[597.88 --> 598.06]  Yeah.
[598.14 --> 598.94]  And fans.
[599.12 --> 599.50]  Absolutely.
[599.70 --> 600.64]  All that kind of stuff too.
[600.64 --> 613.16]  So when it comes to performance, I would say it's somewhere in between older Intel, like integrated Intel GPUs, like Kaby Lake or Coffee Lake and older Lake.
[613.28 --> 617.04]  So older Lake is actually a bit better than the Intel Arc in terms of power consumption.
[617.04 --> 619.30]  I get so confused about all these different lakes.
[619.42 --> 621.10]  Can you just put that into like numbers?
[621.34 --> 622.32]  7th gen or like?
[622.42 --> 626.72]  Yeah, I would say it's between 9th gen and 12th gen.
[627.14 --> 627.40]  Okay.
[627.40 --> 631.56]  So as far as I know, the GPU didn't change for a while.
[631.80 --> 635.56]  So Kaby Lake, Coffee Lake CPUs, they had Intel Graphics 630.
[636.18 --> 642.40]  And so for 12th gen, 13th gen and 14th gen, I'm putting air quotes right here because...
[642.96 --> 646.36]  14th gen was very much a tick on the tick tock, wasn't it?
[646.44 --> 646.70]  Yeah.
[647.02 --> 647.50]  Or a tock.
[647.64 --> 648.96]  It was a small one anyway.
[649.12 --> 650.40]  It was a very minor upgrade.
[650.62 --> 651.24]  Right, exactly.
[652.24 --> 655.54]  And so with 12th gen, I think we got 730.
[655.68 --> 660.38]  So I'm not sure if there was anything in between 630 and 730 for the 10th and 11th gen.
[661.02 --> 661.58]  Maybe not.
[661.74 --> 662.26]  Maybe yes.
[662.72 --> 668.06]  So for single transcode, I found that the performance is somewhere in between those two internal GPUs.
[668.92 --> 671.60]  What I didn't test, however, is multiple transcodes.
[671.90 --> 675.50]  So that's something I'm still planning to test in one of the next videos.
[675.50 --> 682.26]  And that also applies for kind of like comparison between the Intel Arc and some of the other GPUs.
[682.28 --> 686.74]  So I actually did buy a couple of the new GPUs to test them out.
[686.90 --> 688.42]  So, you know, subscribe.
[688.72 --> 689.04]  Wink, wink.
[689.16 --> 689.54]  Nudge, nudge.
[690.20 --> 691.58]  You went to the dark side, huh?
[692.12 --> 692.48]  Yeah.
[693.02 --> 693.74]  I'm curious.
[693.94 --> 696.22]  So how was the software support side of things?
[696.26 --> 700.10]  Because when Arc first launched, particularly on the Linux desktop side of things,
[700.68 --> 704.92]  the Linux driver support was not so good.
[704.92 --> 705.72]  It was rough.
[705.94 --> 706.08]  Yeah.
[706.54 --> 707.58]  How was it these days?
[708.50 --> 713.10]  So I guess my experience only applies to hardware transcoding, really,
[713.28 --> 717.40]  and moreover hardware transcoding in Jellifin because I didn't try Plex.
[717.74 --> 719.60]  I've heard that it's not supported yet.
[720.36 --> 723.54]  Like, I don't know whether that's even possible because as far as I know, Plex,
[724.22 --> 727.70]  does Plex use FFmpeg like Jellifin or did they have like their own thing going on?
[728.18 --> 732.58]  We'll get on to Plex a little bit later in the show with some of the shenanigans they did this week.
[732.58 --> 735.06]  I was talking to a former Plex employee.
[735.36 --> 738.36]  Apparently, they used to have one of the FFmpeg developers on staff.
[738.62 --> 743.24]  But as part of their restructuring earlier this year, Plex this is, they let them go.
[743.60 --> 747.52]  So, yeah, I think it's safe to say that Plex uses FFmpeg under the hood.
[748.04 --> 751.78]  That's interesting because now that I'm thinking about it,
[751.88 --> 755.14]  Jellifin folks do maintain their own fork of FFmpeg, right?
[755.46 --> 756.08]  Yes, they do.
[756.08 --> 761.20]  So it could be that a certain component or certain drivers are included in a Jellifin fork,
[761.28 --> 766.54]  but not in the Plex because I've heard a lot of folks saying that Plex doesn't support our GPUs, period.
[767.18 --> 769.52]  When Morgan and I were coming up with that benchmarking script,
[769.64 --> 772.12]  which, by the way, I love the fact you used that in the video.
[772.22 --> 772.92]  I thought it was super cool.
[773.32 --> 776.66]  We really ran into some issues using just vanilla FFmpeg,
[776.76 --> 780.00]  trying to get it to pick up the right codex for what we were trying to do.
[780.10 --> 782.76]  And then the Jellifin fork just worked.
[782.82 --> 784.50]  And we were like, well, let's just use that.
[784.50 --> 786.26]  So yeah, there might be something to that.
[786.92 --> 788.64]  Yeah, it would definitely make sense.
[789.18 --> 792.30]  So to kind of come back to your question,
[793.16 --> 796.26]  the support in Jellifin when it comes to hardware transcoding is phenomenal.
[796.54 --> 800.54]  So it's basically, it was as easy to set up as the integrated graphics.
[801.14 --> 808.70]  So absolutely nothing to write home about in terms of problems, issues, hiccups, nothing.
[809.18 --> 810.50]  That's what you want, right?
[810.50 --> 812.32]  You just check a box and it just works, right?
[812.40 --> 813.38]  That's the dream.
[813.38 --> 814.28]  That's boring, right?
[814.28 --> 816.98]  I mean, you want to tinker with it.
[817.08 --> 819.22]  We've been doing this long enough that boring is great.
[819.40 --> 820.42]  I'm a fan of boring.
[820.44 --> 822.74]  Yeah, or at least I want one brand that's the boring brand.
[822.84 --> 823.58]  Can I just have that?
[825.88 --> 828.20]  Talescale.com slash self-hosted.
[828.26 --> 831.40]  Go on over there to get a free personal account for up to 100 devices.
[831.54 --> 832.26]  That's my account.
[832.78 --> 836.06]  All of my Homelab stuff, it's on my free personal account.
[836.22 --> 837.76]  And it's a great way to support the show.
[837.84 --> 841.80]  100 devices really, really lets you get an idea what Talescale can do.
[841.80 --> 850.38]  Now, if you're not familiar, it's a zero config VPN built on WireGuard that you can get up and running in just minutes.
[850.38 --> 857.94]  Not only do you not have to worry about like these weird problems of trying to get DNS between two different subnets when you have a WireGuard VPN between them.
[858.00 --> 859.76]  And for some reason, it's not working today.
[860.14 --> 864.06]  You don't have to worry about how to try to make it all work through network manager at the command line or not.
[864.06 --> 868.38]  You don't have to run a WireGuard server on one box that everything connects into.
[869.04 --> 872.06]  Talescale builds out a mesh VPN in just minutes.
[872.36 --> 873.10]  It's a flat network.
[873.26 --> 874.66]  All your devices get a static IP.
[875.32 --> 882.94]  And then you can start doing things like magic DNS or throw a pie hole in there and have DNS on your tail net and start resolving things by name wherever you go.
[883.58 --> 887.22]  Pretty soon you start realizing you don't need to have anything external.
[887.70 --> 890.24]  You essentially can build your own private internet.
[890.24 --> 895.10]  And the beautiful thing is, is you can have it on multiple different cloud providers.
[895.28 --> 896.36]  You can have it on your LAN.
[896.46 --> 897.20]  You can have it in a VM.
[897.62 --> 899.46]  There's even plugins for like VS Code.
[899.66 --> 908.36]  There's all kinds of different ways to install and use Talescale and build out a flat mesh network between instances that are spread out all over the world.
[908.72 --> 912.90]  Man, did it just totally come in handy when I was traveling in El Salvador.
[913.40 --> 914.56]  Talk about peace of mind.
[914.88 --> 920.02]  And it's perfect for businesses or developers who want to set up ad hoc networking, maybe do some demos.
[920.24 --> 926.90]  And man, for the enterprise space, not to have to manage all those traditional VPN systems, but still to get that superior protection of WireGuard.
[927.10 --> 930.88]  And it integrates with your existing authentication system and two-factor for you use that.
[931.02 --> 934.52]  And there are so, so many tools built around Talescale as well.
[934.94 --> 938.28]  It's truly one of the best, I think, benchmark tools out there.
[938.68 --> 940.06]  They're showing the industry how it's done right.
[940.56 --> 942.78]  Support the show and try it for free on 100 devices.
[942.78 --> 946.20]  When you go to talescale.com slash self-hosted.
[946.54 --> 947.66]  Head on over there and try it.
[947.66 --> 949.54]  I think you're really going to be impressed.
[949.72 --> 955.70]  And it just solves a connectivity problem and just totally changes the way you can do networking for the better.
[956.20 --> 958.82]  Talescale.com slash self-hosted.
[960.60 --> 966.02]  So, I mean, Plex for me, and we mentioned it briefly there, Plex for me was a huge gateway drug into self-hosting.
[966.42 --> 967.36]  What was yours?
[967.48 --> 968.38]  What was your first?
[968.38 --> 970.46]  I want to say Plex too, actually.
[971.20 --> 987.56]  And I don't know if you guys discuss these kind of very, very illegal and dark things in this podcast, but actually sort of trying to avoid having, you know, 75 streaming services all at once, you know, paying for them.
[987.56 --> 992.34]  I guess that was one of the things that sort of acted as a gateway drug for me.
[992.70 --> 1000.78]  And also considering the fact that even if you wanted to pay for certain streaming services to watch certain movies or series, you can't, right?
[1000.78 --> 1009.16]  Because they're like geo-restricted or maybe certain movies not even on any streaming service at all.
[1009.16 --> 1023.34]  So, Netflix kind of started out strong, you know, they were having a lot of series, a lot of movies, but like now that they sort of have to, you know, sort of make the shareholders happy, they've been kind of dropping rights for a lot of IPs.
[1024.28 --> 1025.56]  There's too much money at stake.
[1025.76 --> 1029.90]  I mean, so I don't know the last time I pirated any music material.
[1030.28 --> 1038.46]  I couldn't tell you genuinely because Spotify largely solved that problem and then Apple Music and, you know, all the rest of it and everything else is on YouTube.
[1039.16 --> 1041.84]  But video is for some reason been a special beast.
[1041.92 --> 1053.52]  I think it's because it's so expensive to make versus a record, you know, to make a high quality video production, you need tens of millions, if not hundreds of millions of currency units to make that happen.
[1053.76 --> 1053.96]  Right.
[1054.00 --> 1056.54]  And it's just there is too much money at stake.
[1056.54 --> 1065.82]  And I think because of that ubiquity of availability of music content, like on Spotify or whatever, like music piracy kind of just died there and then.
[1067.02 --> 1068.24]  But you and you were right.
[1068.24 --> 1068.80]  You mentioned it.
[1068.86 --> 1070.94]  Netflix were the first movers.
[1071.12 --> 1076.08]  And for a while, a Netflix subscription got me pretty much everything I cared about.
[1076.30 --> 1077.94]  And then I just rented the rest or whatever.
[1078.54 --> 1083.32]  But then over the last 10 years or so, that pool has become more and more diluted.
[1083.42 --> 1087.18]  And I couldn't even tell you half of the streaming services services that exist these days.
[1087.18 --> 1089.10]  It's just it's just ridiculous.
[1089.28 --> 1091.98]  I mean, the catch always used to be live sports.
[1091.98 --> 1092.20]  Right.
[1092.20 --> 1095.28]  And now I can the only live sport I actually care about is Formula One.
[1095.46 --> 1101.66]  So I just stream that now using the F1 TV app and cable is dead and all the rest of it.
[1101.78 --> 1102.20]  You know, so this.
[1102.76 --> 1102.98]  Yeah.
[1103.50 --> 1110.18]  Does this lead to more and more storage sprawl over time, which then leads you down further into the self hosting rabbit hole?
[1110.18 --> 1111.32]  Yes, absolutely.
[1111.96 --> 1118.72]  But I think whereas like with movies and series, you know, you can basically say, OK, I've watched this one.
[1118.82 --> 1119.66]  I don't need this anymore.
[1119.88 --> 1120.80]  So I can delete it.
[1120.90 --> 1128.12]  Obviously, there are people who who are definitely have these data hoarder sort of.
[1129.12 --> 1129.48]  Yeah.
[1129.48 --> 1130.84]  They have a data hoarder in them.
[1131.04 --> 1135.04]  So they say, no, I have to keep everything just in case the apocalypse comes.
[1135.20 --> 1137.12]  You know, I will be the guy with all the movies.
[1137.26 --> 1137.40]  Right.
[1137.70 --> 1139.44]  No electricity, but you've got the movies.
[1139.70 --> 1139.88]  Yeah.
[1139.94 --> 1141.06]  I mean, at least you got that, you know.
[1142.10 --> 1144.64]  So what's your we have a bit of a tradition around here.
[1144.70 --> 1149.06]  We try and ask guests what the number of raw terabytes on their LAN is.
[1149.48 --> 1152.12]  Wendell, I think, is currently the winner with like a petabyte or something.
[1152.66 --> 1153.92]  I mean, of course, it's got to be Wendell, right?
[1154.40 --> 1155.18]  Yeah, of course.
[1155.50 --> 1157.76]  I'm curious what your number might be.
[1157.76 --> 1158.76]  Oh, I actually.
[1158.76 --> 1159.44]  Hmm.
[1159.70 --> 1160.82]  I'm going to have to think about it.
[1160.98 --> 1162.30]  So the nearest hundred is fine.
[1163.20 --> 1164.84]  Well, that would be a hundred then.
[1165.30 --> 1166.38]  But let me think.
[1166.48 --> 1169.94]  I got three 16 terabyte access drives.
[1170.92 --> 1173.42]  I got so that would be 48.
[1173.78 --> 1177.90]  And I got four two terabytes SSDs.
[1177.98 --> 1179.04]  So that would be 16.
[1180.90 --> 1184.68]  Yeah, let's say 65, around 65 terabytes, I guess.
[1185.12 --> 1185.46]  Great.
[1185.46 --> 1191.84]  And one of our lovely listeners I know will update the SSH wiki with Wolfgang's entry into the leaderboard.
[1192.10 --> 1192.54]  Not bad.
[1192.62 --> 1194.14]  65 terabytes is not bad.
[1195.36 --> 1196.40]  That's pretty good.
[1196.68 --> 1197.10]  I got it.
[1197.14 --> 1198.00]  I got up my game.
[1198.00 --> 1201.12]  And that's without keeping absolutely all your media on top of that.
[1201.18 --> 1204.62]  Are you keeping all of the raw footage for your YouTube channel?
[1204.72 --> 1205.02]  Right.
[1205.22 --> 1205.42]  So.
[1205.82 --> 1206.58]  Oh, boy.
[1206.82 --> 1207.78]  I was getting to that.
[1208.26 --> 1210.06]  But yeah, I absolutely do.
[1210.14 --> 1210.32]  Yeah.
[1210.32 --> 1214.44]  And it has gotten more and more difficult as I moved to ProRes.
[1215.26 --> 1215.52]  Right.
[1215.58 --> 1218.48]  Because I used to film in just H264.
[1218.92 --> 1227.06]  But once you kind of try ProRes, you know, you never really go back because the performance when it comes to editing is just much, much better.
[1227.38 --> 1228.46]  It's just so much better.
[1228.56 --> 1230.02]  It's not even a comparison.
[1230.36 --> 1232.34]  ProRes is an incredible bit of work.
[1232.34 --> 1236.06]  Like Apple at its finest when they created that lossless video codec.
[1236.42 --> 1238.36]  Even on Linux, I want to use ProRes.
[1239.18 --> 1239.54]  Right.
[1239.96 --> 1242.62]  So I'm curious if you were starting from scratch today.
[1243.24 --> 1245.04]  And I don't want to say money's no object.
[1245.12 --> 1247.58]  So let's give you a budget of $1,000 just for the hardware.
[1247.68 --> 1248.66]  I'm not talking about hard drives.
[1250.02 --> 1252.90]  What would you build in terms of a media server?
[1253.88 --> 1254.68]  Intel or AMD?
[1255.34 --> 1261.68]  I would want to say Intel because you can use AMD as a home server.
[1261.68 --> 1268.34]  And the AMD internal graphics are supported in Jalefin when it comes to video transcoding.
[1268.54 --> 1268.60]  Right.
[1268.66 --> 1271.00]  So they have, they don't have AMF or Linux.
[1271.16 --> 1272.60]  That's the Windows only thing is for now.
[1273.06 --> 1275.24]  But it is supported by VA API.
[1276.80 --> 1280.64]  And in my experience, the performance when it comes to single file.
[1280.76 --> 1283.44]  So 4K, HEVC, HDR, all that jazz.
[1284.26 --> 1285.52]  Is around 30 FPS.
[1285.86 --> 1289.50]  So it is enough to watch a movie, watch a single 4K movie.
[1289.50 --> 1294.28]  So if you don't need anything more than that, then I think AMD is great.
[1294.48 --> 1294.62]  Right.
[1294.74 --> 1302.38]  So even just for the fact that you also get ECC support on pretty much any consumer grade motherboard.
[1302.94 --> 1303.84]  Yeah, that's a nice thing.
[1303.96 --> 1308.16]  So that's something that Intel has kind of gatekept for a while.
[1308.20 --> 1311.00]  And they kind of keep gatekeeping it.
[1311.00 --> 1317.26]  But then for some reason, they gave it to the i3 CPUs and said, hey, i3, you can do ECC.
[1317.46 --> 1318.12]  That's totally cool.
[1318.52 --> 1323.96]  It's funny that you mention that because they actually went, they completely reversed that with the 12th and 13th gen, right?
[1324.22 --> 1328.86]  So now Pentium, Celerons and i3s do not get ECC support.
[1329.04 --> 1331.40]  But everything higher than that, you get ECC.
[1331.74 --> 1334.98]  Whereas like before Coffee Lake, it was the opposite.
[1334.98 --> 1341.28]  So I don't know what kind of game Intel was playing, but it's probably some kind of 4D, 5D chess, right?
[1341.90 --> 1343.74]  I'm not sure Intel knows half the time either.
[1343.82 --> 1345.04]  That's probably half the problem.
[1345.34 --> 1345.58]  Right.
[1345.82 --> 1346.02]  All right.
[1346.06 --> 1347.72]  So do you have any motherboard picks for us?
[1349.10 --> 1353.84]  I would have to say something from ASRock or ASUS, right?
[1353.88 --> 1362.52]  Because motherboards, I think, unless you're going with some kind of, I don't know, very obscure kind of stuff, I think it's hard to go wrong these days.
[1362.52 --> 1369.62]  Because like there are anecdotal experience when it comes to, oh, I think MSI has like bad QA or ASRock or ASUS.
[1369.82 --> 1372.96]  So it's all going to depend on the exact unit.
[1373.64 --> 1380.74]  But personally, I have actually, I think right now in all the x86 systems in my house, I have ASRock, right?
[1380.82 --> 1383.80]  And I haven't had any issues with it so far.
[1384.46 --> 1385.84]  Yeah, the ASRock rack stuff is okay.
[1385.84 --> 1398.48]  There's a couple of weird things with some of the PCI switching layouts on a couple of boards I've got and some of their choices around like BMC being exposed to the WAN interface.
[1398.80 --> 1399.46]  Oh, that's amazing.
[1399.72 --> 1399.92]  It's a bit odd.
[1400.92 --> 1403.44]  I wrote a blog post about it a while ago, which I'll link in the show notes.
[1403.74 --> 1404.42]  But yeah.
[1405.00 --> 1406.98]  But when it comes to BMC, this is actually a good point.
[1406.98 --> 1414.98]  But like if you do want to use hardware transcoding, right, on a media server, I would actually recommend going for something without a BMC.
[1415.94 --> 1425.48]  Because a lot of motherboards, they don't give you a choice when it comes to video output between the BMC, quote unquote, GPU and the integrated Intel card.
[1426.04 --> 1434.62]  So what you have is basically a system that is not capable of not just monitor output through the Intel GPU, but also the rendering capabilities.
[1434.62 --> 1442.38]  So even though you might have a processor with its greater GPU, your BMC will not let you use it.
[1442.88 --> 1450.74]  And unfortunately, there's just kind of like no way to know beforehand whether there is a bias option that like, you know, lets you change it.
[1450.94 --> 1455.50]  And it's the same thing with bifurcation, like the number of PCIe lanes on the consumer chips is quite low.
[1455.50 --> 1465.68]  So you end up like you can get these cards where you split one card into four NVMe drives, for example, with 4X, you know, you take a 16X slot and split it into 4X slots.
[1466.50 --> 1473.24]  But there is just genuinely no way of knowing whether the motherboard BIOS has got a bug in it or is even going to support that until you get the thing in your hands.
[1473.24 --> 1479.72]  And then if you enable the wrong M.2 slot, it can switch half of the slot into an 8 slot.
[1479.82 --> 1481.26]  And it's just a mess.
[1481.72 --> 1482.42]  So, yeah.
[1482.68 --> 1483.46]  Yeah, exactly.
[1484.26 --> 1492.78]  And also like a big, my biggest pet peeve when it comes to M4 motherboards is that they, almost all of them do have PCIe bifurcation, right?
[1492.92 --> 1493.20]  Great.
[1493.20 --> 1496.40]  But they have exactly three options, I think.
[1496.54 --> 1500.96]  So X16, X8, X8, and then X8, X4, X4.
[1501.20 --> 1508.32]  They don't have X4, X4, X4, X4, which is like what a lot of people would want for these like ASUS Hyper M.2 adapters.
[1508.64 --> 1519.98]  That's one of the good things I will say about the HL15 I've got in for review at the minute is because it's a Xeon, it's got 48 lanes of PCIe compared to my i5 8500 that's got 16.
[1519.98 --> 1524.60]  So I've got four M.2 SSDs in there in one card.
[1524.76 --> 1526.62]  And it's, mwah, chef's kiss.
[1526.74 --> 1527.26]  It's wonderful.
[1527.74 --> 1528.20]  That's great.
[1528.30 --> 1528.70]  That's great.
[1529.58 --> 1530.92]  Well, thanks for joining us, Wolfgang.
[1531.04 --> 1532.72]  I think you're going to stick around for the rest of the show.
[1533.40 --> 1533.94]  Thank you.
[1534.04 --> 1535.16]  It's a pleasure to be here.
[1535.92 --> 1538.62]  Alex, will you break down the NetGate situation?
[1538.86 --> 1542.62]  Because we've been sitting on this story watching it evolve over about a month now.
[1543.18 --> 1545.54]  And it's gotten pretty confusing at this point.
[1545.56 --> 1548.00]  But I think you've gotten some clarity.
[1548.36 --> 1549.36]  I'm not sure I do.
[1549.36 --> 1550.88]  I think you and I were doing some research.
[1550.88 --> 1551.60]  As close as we've gotten.
[1552.08 --> 1556.78]  You and I were doing the research for this episode before the show talking on chat.
[1556.92 --> 1562.38]  And we were both saying, like, the more we read about this NetGate drama, the more confused that we got.
[1562.54 --> 1568.00]  So for those of you that aren't familiar, NetGate is the commercial entity behind PFSense.
[1568.86 --> 1574.94]  And PFSense is a firewall distribution built on top of FreeBSD, the operating system.
[1574.94 --> 1580.84]  And they've got a bunch of different tiers of licensing that they operate in different, like, I guess, distros.
[1581.12 --> 1581.92]  What do we call it?
[1581.94 --> 1582.28]  Distros?
[1582.96 --> 1583.62]  I don't know.
[1583.72 --> 1587.76]  They're really just kind of, I mean, they're kind of like products.
[1587.88 --> 1589.46]  They're just product, different products.
[1589.96 --> 1594.02]  It's one of those market differentiators where they try to create a different product for different size groups.
[1594.02 --> 1600.60]  Just like Intel and Microsoft and tier, I guess.
[1600.88 --> 1601.04]  Yeah.
[1601.12 --> 1601.26]  Yeah.
[1601.26 --> 1601.98]  Different tiers.
[1602.24 --> 1602.40]  Yeah.
[1602.76 --> 1602.94]  Yeah.
[1602.94 --> 1604.32]  OK, so let's go with different tiers.
[1604.50 --> 1613.20]  So the idea is that they have a PFSense CE community edition available, which is free of charge and always will be in air quotes.
[1613.20 --> 1619.74]  And they have a PFSense Plus option, which has a bunch of different tiers where you can basically buy support.
[1619.84 --> 1624.28]  And we've seen that model quite a few times with Red Hat and a bunch of other open source companies over the years.
[1625.14 --> 1628.78]  And so you'd think there isn't much room for drama in a model like that.
[1628.94 --> 1635.72]  But NetGate seemed to be a company that go out of their way to attract detractors and drama.
[1636.18 --> 1638.38]  And I think we're going to break some of that down for you today.
[1638.38 --> 1646.96]  When I first heard about this, what I essentially heard getting kicked around online is that you can't get PFSense for free anymore.
[1647.92 --> 1651.06]  And I don't think that's actually the net result of this.
[1651.20 --> 1657.38]  But there are now new restrictions on how you can deploy it or, I guess, redistribute it in their verbiage.
[1658.46 --> 1658.56]  Yeah.
[1658.62 --> 1666.32]  So a year ago, NetGate made a version of the PFSense Plus license, their commercial fork of PFSense Community Edition, remember.
[1666.32 --> 1676.24]  They made a HomeLab version available for free and said, we will continue to support this and make it free for the foreseeable future.
[1676.88 --> 1682.36]  And they also encouraged folks to upgrade from the Community Edition to the Plus Edition.
[1683.00 --> 1688.64]  On top of that, the Plus Edition has a bunch of features, rollbacks and other configuration niceties,
[1688.64 --> 1698.10]  which if you're deploying this into a whole bunch of remote sites, you know, it's very nice, useful to be able to pick up the phone and call NetGate and actually have some support.
[1698.76 --> 1701.90]  The HomeLab option didn't come with any of that support side of things.
[1702.20 --> 1703.52]  And for me, that's fine.
[1703.62 --> 1705.32]  You know, it's like we've seen this model a hundred times.
[1705.38 --> 1712.36]  It's the gateway drug to get people, you know, that want to run commercial grade software at home and then take it to work.
[1712.36 --> 1713.94]  We've seen this model a hundred times.
[1714.88 --> 1722.18]  The issue is a year after introducing this HomeLab license, without really communicating it properly,
[1722.62 --> 1727.88]  and this is a theme for NetGate, unfortunately, they just revoked this license and said,
[1728.16 --> 1732.14]  yeah, we're not going to offer this HomeLab license anymore pay up.
[1732.14 --> 1743.58]  And at the time of the original press release, the only option was to buy what they call a TAC support contract for $399 per year.
[1744.14 --> 1745.04]  Yeah, that was pretty shocking.
[1745.34 --> 1751.80]  And the initial communication wasn't even like a blog post or a Twitter update or anything like that.
[1751.82 --> 1756.38]  It was just kind of updates to the website when you went to go download what used to be free.
[1756.38 --> 1762.30]  Now, a couple of days elapsed and, you know, all the folks in the community, like Tom Lawrence, made a video, for example,
[1762.40 --> 1767.34]  showing you how to downgrade from PFSense Plus to PFSense CE.
[1767.50 --> 1771.82]  And the very fact I'm using the word downgrade should give you an idea of the general sentiment in the community.
[1772.32 --> 1776.32]  Because the CE version is the free version and the release cycle is slower.
[1776.58 --> 1778.72]  It doesn't get the updates as quickly as Plus.
[1778.86 --> 1786.20]  And that was part of the sales pitch that NetGate themselves made over the previous year to get folks to switch from CE to Plus in the first place.
[1786.78 --> 1790.36]  Then they do the bait and switch and pull the rug out from under people's feet and say,
[1790.70 --> 1791.70]  hey, actually, it's not so bad.
[1791.76 --> 1793.32]  You can go back to CE if you don't want to pay.
[1793.40 --> 1794.18]  That's totally cool.
[1795.28 --> 1799.12]  So the original announcement happened on October 26th.
[1799.42 --> 1803.38]  By October 30th, another blog post was released saying,
[1803.58 --> 1809.08]  hey, yeah, we've seen that many of our community members are, how should we put this, unhappy.
[1810.48 --> 1814.64]  And so we want to make a TAC Lite subscription available for individuals.
[1814.64 --> 1816.36]  And we'll do this over the next few days.
[1816.48 --> 1824.40]  So this takes the entry cost of some kind of supported option from $399 down to $129 per year.
[1825.16 --> 1829.98]  There's another aspect to this too, which I think was probably part of their calculation.
[1829.98 --> 1834.30]  And in their explanation blog post, they kind of infer to this.
[1834.30 --> 1838.02]  And that is that they're not very happy.
[1838.90 --> 1843.66]  And they've continuously tried to go after third-party hardware people.
[1843.66 --> 1850.86]  Like somebody buys a low-power one-liter PC, throws PFSense on there, and puts it on eBay for $600.
[1851.42 --> 1854.06]  I think that drives them crazy.
[1854.06 --> 1856.64]  And they've gone after them on trademark grounds.
[1856.74 --> 1859.30]  And I think they're trying to go after them with this licensing restructuring.
[1859.70 --> 1866.44]  And in their blog post, where they kind of go into all of this, they also imply that some of them have been susceptible to supply chain attacks.
[1866.82 --> 1868.68]  And they say, be careful and be wary.
[1868.82 --> 1872.04]  But they never go into detail about those supply chain attacks.
[1872.58 --> 1875.80]  And either that's a true statement or they're exaggerating.
[1875.80 --> 1880.16]  And if it's a true statement, then we need to be notifying users.
[1880.16 --> 1883.10]  And anything they know, they need to be making public immediately.
[1883.10 --> 1884.58]  Because these are people's firewalls.
[1884.76 --> 1890.18]  And if it's not a true statement, then they're exaggerating, which would make me think they're being emotional still.
[1890.32 --> 1891.52]  So I'm not sure which one it is.
[1891.64 --> 1893.50]  But either way, I don't like their actions so far.
[1893.66 --> 1896.24]  It could also be kind of a fear-mongering thing, right?
[1896.90 --> 1902.08]  So if they don't like people kind of preloading PFSense on those firewalls or like one-liter PCs.
[1902.08 --> 1906.44]  And they're also saying that they've been having those supply chain attacks.
[1906.90 --> 1915.70]  What they could be implying is that, you know, some people who are selling those PCs might have sort of maybe malicious intentions.
[1916.02 --> 1922.44]  Maybe they're preloading, I don't know, hardware botnets or hardware exploits onto the PFSense boxes.
[1922.74 --> 1924.96]  Which is obviously like a lot of rubbish, in my opinion.
[1925.84 --> 1929.42]  Yeah, we have no way of knowing because those claims aren't really substantiated anywhere.
[1929.42 --> 1935.44]  But Chris, you made a point that NetGate might be reacting emotionally here.
[1935.48 --> 1942.22]  And I want to just fill our listeners in on some of the history here of what NetGate has done previously, acting emotionally.
[1942.56 --> 1952.92]  So back in 2017, Jamie Thompson, who is the founder and CEO of NetGate, created a website dedicated to, air quotes, taking down OpenSense.
[1952.92 --> 1956.28]  They purchased OpenSense.com.
[1956.40 --> 1962.56]  Remember the actual project, OpenSense, which is a fork of PFSense, an open source fork of PFSense.
[1962.78 --> 1965.56]  I can't imagine why the community might want a fork of PFSense.
[1965.82 --> 1966.46]  I just can't imagine.
[1966.64 --> 1966.82]  No idea.
[1966.82 --> 1972.12]  The open source website, the open source version website is OpenSense.org.
[1972.80 --> 1980.84]  And so for some reason, NetGate registered, or somebody that worked for NetGate, I shouldn't say NetGate the company.
[1981.34 --> 1984.92]  Some person registered OpenSense.com.
[1984.92 --> 1992.22]  Some folks referred to this as a parody site, but in my opinion, it was designed to just be outright slanderous.
[1992.72 --> 1996.44]  So if you actually go and look at web.archive, we'll put a link to this in the show notes.
[1996.60 --> 2005.20]  The site included very sarcastic slogans and accusations of poor quality code, plagiarism.
[2005.62 --> 2010.74]  And there was even a video, you know, the famous Adolf Hitler movie that people put all sorts of memes on.
[2010.74 --> 2021.24]  They actually edited that video to be inside the OpenSense development bunker, naming and shaming OpenSense contributors that dared fork the PFSense code base.
[2022.14 --> 2026.04]  Now you might expect that kind of behavior from an angry teenager who just broke up from their girlfriend.
[2026.50 --> 2035.48]  And you'd think that once whoever registered that website sobered up in the morning and realized what they'd done, they'd agree that that was perhaps going a bit too far.
[2035.48 --> 2044.60]  Unfortunately, OpenSense, the project, had to go and take this to WIPO, the World Intellectual Property Organization.
[2044.94 --> 2052.08]  And they actually had to have that organization arbitrate a case and a ruling to take OpenSense.com down.
[2052.52 --> 2060.08]  It boggles my mind that lawyers and all that had to get involved in something that is just so clearly,
[2060.08 --> 2064.88]  it should be so far beneath a commercial company to do something like this to an open source project.
[2064.88 --> 2076.88]  When you read that site, which the archive site, you know, again, one of the themes in there is they say that they take enterprise code and they steal it and then they strip out the stuff that makes it great.
[2076.96 --> 2078.66]  So that way it's quote unquote clean.
[2078.94 --> 2090.10]  But that theme of somebody is stealing our code and using it in a way we don't want them to use it is coming up over and over again back then in 2017 and today in 2023.
[2090.10 --> 2093.10]  Sort of reminds me of the Red Hat statement, right?
[2093.24 --> 2105.40]  Because I think this common theme of, you know, people are freeloading our code, which we spend so much time and we kind of invested so much effort into,
[2105.40 --> 2115.40]  which I don't know, I guess, I guess this is not really the case, but in terms of common themes between these two topics,
[2116.06 --> 2122.08]  I think this theme of like people are searing our code is very prevalent.
[2122.08 --> 2130.76]  We see it time and time again with Prusa 3D, you know, the 3D printer manufacturer talking about inventing a new open source license,
[2131.14 --> 2135.08]  despite having built a company on top of open source for the last decade plus.
[2135.70 --> 2137.02]  HashiCorp is another one.
[2137.36 --> 2138.44]  Red Hat is another one.
[2138.56 --> 2141.22]  I mean, OK, Red Hat maybe have invested more money than most.
[2141.76 --> 2147.12]  PFSense itself is built on top of FreeBSD, which is maybe 85, 90 percent of the lift.
[2147.12 --> 2147.56]  Absolutely.
[2148.56 --> 2154.38]  So you'd think at this point, isolated incident 2017, the website opensense.com, right?
[2154.40 --> 2155.28]  You think, OK, it's a one off.
[2155.34 --> 2155.84]  We'll let them off.
[2157.14 --> 2167.88]  However, March 2021 came around and there was, if you remember, there was a whole bunch of hoopla about putting WireGuard into the BSD kernel back then.
[2167.88 --> 2178.36]  Linux had it at that point, and it was, in my opinion, a glaring deficiency in BSD at the time that it didn't have WireGuard in the kernel.
[2178.80 --> 2182.82]  So you were relying on user space implementations, which were a lot slower, et cetera, et cetera.
[2184.00 --> 2189.10]  NetGate tried to do a good thing and sponsor some work to get WireGuard brought into the BSD kernel tree.
[2190.16 --> 2194.78]  The code was upstreamed into BSD itself, FreeBSD itself, I should say, in November 2020.
[2194.78 --> 2202.82]  And unfortunately, issues were found with the implementation of WireGuard, which caused huge ripples throughout the BSD community.
[2202.98 --> 2209.70]  I actually remember our good friend Alan Jude commenting on this and getting involved in this whole debacle over on two and a half admins as well.
[2210.52 --> 2218.78]  A NetGate, true to form, rather than taking a step back and admitting fault in this endeavor about trying to rush through code that wasn't properly audited
[2218.78 --> 2224.90]  and trying to get things merged because it was in their commercial interest to do so, they went on the offensive.
[2225.08 --> 2227.06]  So we'll put another link to this in the show notes.
[2227.10 --> 2232.50]  But there was a blog post talking about PFSense Plus and the dev insights and the direction.
[2233.24 --> 2238.48]  And Scott Long, who was NetGate's director of software and engineering, put out several blog posts relating to this,
[2238.56 --> 2244.64]  which were later found to be, how should we say, economical with the truth, if we're being kind.
[2244.64 --> 2250.08]  And maybe if we're in our pitchfork grabbing mood, we might say he was lying.
[2250.50 --> 2251.34]  But, you know.
[2252.02 --> 2253.50]  I like economical with the truth.
[2255.64 --> 2263.06]  And then just to complete the trifecta of the pattern of behavior that makes me really find it very difficult to trust anything NetGate ever does,
[2263.06 --> 2266.00]  is the AES-NI flip-flop.
[2266.12 --> 2277.24]  So this is a set of instructions for encryption built into CPUs that NetGate told us in September 2017 would be required on CPUs to run PFSense going forward.
[2278.00 --> 2283.20]  It was this that actually pushed me to switch away from PFSense to OpenSense several years ago,
[2283.26 --> 2287.38]  because I was, like, running this on an APU2, I think, at the time.
[2287.38 --> 2291.90]  And that didn't have AES-NI, and I was like, well, I don't want to upgrade this firewall box.
[2291.96 --> 2292.82]  It does everything I need.
[2292.86 --> 2295.42]  So I'm just going to go and switch to something that means I don't have to.
[2296.32 --> 2302.32]  Anyway, many folks, myself included, scrambled to upgrade their firewalls and switch to other operating systems and stuff like that.
[2303.36 --> 2305.84]  So September 2017, they tell us they're going to need this.
[2305.94 --> 2306.86]  We're going to need this thing.
[2307.36 --> 2312.18]  March 2019, they go out and buy a pair of flip-flops and tell us, actually, no, we were just kidding.
[2312.34 --> 2315.22]  You don't actually need AES-NI.
[2315.22 --> 2321.42]  Yeah, for me, the red flag moment was the WireGuard situation with FreeBSD.
[2321.76 --> 2329.16]  The whole way it went down was massively embarrassing, in my opinion, for NetGate and those involved.
[2329.30 --> 2337.10]  And it was just barely caught at the last minute with a massively insecure implementation, if I recall correctly.
[2337.10 --> 2349.32]  And then what you touched on, the refusal to actually acknowledge the mistake and just fix it and resubmit, but instead hunker down and battle with the developers for something that was clearly flawed.
[2349.32 --> 2363.50]  You know, they said that NetGate accused the BSD developers of having a, quote, irrational bias against NetGate, even though their issue, their patch had a number of zero-day flaws, if I recall.
[2363.66 --> 2367.18]  I mean, it would have been a massive disaster for the FreeBSD project.
[2367.18 --> 2377.80]  So that was the big red flag for me, is it's clearly there wasn't clear thinking, there wasn't rational thinking, and there wasn't rational interaction with the upstream project in which they are dependent on.
[2378.62 --> 2383.08]  And then, yeah, it's just been a series of things every year or so since then.
[2383.08 --> 2388.22]  It's funny, we're going to talk about patterns with Plex after the break as well, you know.
[2388.44 --> 2401.32]  It's funny when money starts to get involved, it really muddies the waters of people's scruples of their understanding of open source and how different contributions are, you know, given away for free.
[2401.58 --> 2404.42]  And, you know, it's just money ruins everything.
[2404.60 --> 2405.46]  Can we just agree on that?
[2405.90 --> 2411.34]  Yeah, especially when the money is a little more expensive and there's less VC money going around.
[2411.34 --> 2416.12]  And so profits get a little tighter, things just start to get, you know, people start looking at their APIs.
[2416.36 --> 2417.68]  Gosh, that's costing us a lot of money.
[2417.74 --> 2420.28]  They start looking at their users going, hmm, we could monetize that.
[2420.62 --> 2426.82]  And PFSense starts looking at people selling clones of their stuff on hardware and thinking, that's sales that we could be having right now, boys.
[2426.86 --> 2427.88]  We've got to knock that off.
[2428.32 --> 2429.84]  I mean, it's all kind of a similar trend, isn't it?
[2432.26 --> 2434.84]  Linode.com slash SSH.
[2434.98 --> 2440.02]  Man, Linode is the hosting provider because now they're part of Akamai.
[2440.02 --> 2446.34]  All the tools and the infrastructure that we like and the interfaces, even the API, that's all staying the same.
[2446.42 --> 2452.04]  The stuff we use to build and deploy at scale quickly is still there, but now they're backed by the Akamai.
[2452.38 --> 2454.66]  This is really the only choice now.
[2454.82 --> 2462.22]  If you want a high-quality hosting provider with great pricing, it's Linode now, especially when they're now part of Akamai.
[2462.22 --> 2467.20]  And there's more resources that Akamai is adding to Linode, so they're expanding their data centers worldwide.
[2467.40 --> 2470.72]  We just took advantage of one of those new ones, like the week it went online.
[2470.94 --> 2471.92]  And it was smooth.
[2472.12 --> 2473.32]  It's been working flawlessly.
[2474.04 --> 2478.84]  They have solutions that are great for individuals, but they'll scale up to an enterprise of any size.
[2478.92 --> 2481.40]  I mean, they have massive enterprises running on Linode.
[2481.40 --> 2485.92]  And as part of Akamai's global network of offerings, you're going to see more resources.
[2486.04 --> 2487.16]  You're going to see more data centers.
[2487.26 --> 2488.68]  You're going to see better network connectivity.
[2489.34 --> 2489.98]  So why wait?
[2490.58 --> 2493.08]  Go see why we love Linode, why we've been using it for years.
[2493.16 --> 2494.60]  It's how JB hosts everything.
[2495.30 --> 2496.98]  It's the only hosting provider I would use.
[2497.94 --> 2499.78]  Go to linode.com slash SSH.
[2500.04 --> 2505.14]  Go see how Linode, now Akamai, will help scale your applications from the cloud way out to the edge.
[2505.68 --> 2506.86]  Probably even Brent's place.
[2507.42 --> 2508.18]  In fact, I'm pretty sure.
[2508.18 --> 2511.66]  Linode.com slash SSH.
[2513.54 --> 2517.40]  So as you may have seen in your email inbox over the last week or two,
[2517.80 --> 2522.32]  Plex decided it was okay to send emails to everybody who's registered with Plex,
[2522.76 --> 2526.98]  showing them what their friends have been watching on their Plex servers.
[2527.28 --> 2527.82]  Do you see that?
[2528.38 --> 2529.12]  How about this?
[2529.52 --> 2530.80]  How about this?
[2530.92 --> 2534.88]  You sent me a screenshot because I hadn't seen it from my side, right?
[2534.88 --> 2538.16]  I've seen your side, what you've watched or what my friends have watched.
[2538.52 --> 2542.16]  But I hadn't seen what you see of my viewing behavior.
[2543.34 --> 2546.02]  And I'm really glad I wasn't doing anything embarrassing.
[2546.56 --> 2550.84]  You know, I would if I like, what if I had watched like 15 episodes of something?
[2550.92 --> 2552.62]  You'd be like, geez, is he doing anything?
[2552.82 --> 2554.50]  Like, how would you not pass judgment on me?
[2554.56 --> 2557.72]  If I had like slammed 15 episodes of MASH, you're like, what?
[2557.90 --> 2558.24]  MASH?
[2558.34 --> 2559.52]  15 episodes of MASH?
[2559.52 --> 2560.12]  What's he doing?
[2560.66 --> 2562.06]  Thankfully, it wasn't one of those weeks.
[2562.62 --> 2567.20]  But, you know, we saw examples out there of softcore porn getting a screen, you know,
[2567.24 --> 2572.58]  and it shows you like the thumbnail or the picture too from, it's just embarrassing.
[2572.58 --> 2574.86]  And I can't believe they're thinking this is a great idea.
[2574.86 --> 2575.30]  Yeah.
[2576.36 --> 2581.08]  I mean, to be clear, this is Plex telling other people what I've been watching on my
[2581.08 --> 2582.98]  server with my files.
[2582.98 --> 2589.94]  And I just think it's such an egregious overreach for this information to leave the Plex, like,
[2590.14 --> 2590.68]  interface.
[2591.18 --> 2592.38]  Like, email lives forever.
[2592.68 --> 2594.76]  It goes across the internet in clear text.
[2595.28 --> 2600.52]  Like, I know because I put a Reddit thread up, which has annoyingly been my most popular
[2600.52 --> 2603.12]  Reddit thread ever, like 1800 upvotes.
[2603.52 --> 2609.00]  I know that most people in the self-hosted community agree with us that it's not a surprise
[2609.00 --> 2610.10]  that Plex are doing this.
[2610.10 --> 2614.68]  We already knew that Plex were collecting a bunch of this data.
[2615.50 --> 2621.74]  It does confirm, though, that they have actual title information of what we're watching, right?
[2621.84 --> 2627.34]  So the nuance here is they don't know if you actually watched it or if you marked it watched,
[2627.80 --> 2631.50]  but they now know, presumably the file name, don't know for sure, but they definitely know
[2631.50 --> 2632.96]  the name and what you watched.
[2633.78 --> 2635.28]  That's uncomfortable.
[2635.98 --> 2637.04]  Yeah, it really is.
[2637.04 --> 2642.32]  I mean, they're one subpoena away from having a, well, I say a subpoena.
[2642.72 --> 2648.00]  You know, they were hacked earlier this year and the entire database behind app.plex.tv was taken.
[2649.24 --> 2651.40]  Plex themselves have absolutely no idea.
[2652.34 --> 2657.02]  And this is from a source who wished to remain nameless, who is a former employee at Plex I spoke to this week.
[2657.66 --> 2662.34]  Plex themselves have no idea what information was actually taken in that breach.
[2662.34 --> 2668.10]  I mean, they know what's in the database, so they can assume what was taken, but they don't know what's being done with that information,
[2668.34 --> 2674.88]  which includes all of the cross-referencing of the content IDs, usernames, who you've shared things with.
[2675.28 --> 2679.10]  And now we know for sure watch history is also in that list, too.
[2679.58 --> 2680.40]  Maybe some other things, too.
[2681.06 --> 2681.46]  Yeah.
[2682.10 --> 2685.32]  You're sitting pretty over there with Jellyfin, though, Wolfgang, huh?
[2685.32 --> 2690.06]  Yeah, I've actually switched from Plex to Jellyfin about a couple of months ago.
[2691.10 --> 2693.08]  And it's been great so far, really.
[2693.28 --> 2694.02]  It's been amazing.
[2694.40 --> 2701.80]  And my experience, I personally left Plex because you just kind of have to have an internet connection to use Plex, in my experience,
[2702.22 --> 2704.62]  especially if you do some weird stuff with VLANs or whatever.
[2705.30 --> 2707.62]  And Jellyfin kind of just works for me.
[2707.76 --> 2708.72]  I love it so far.
[2708.72 --> 2714.64]  Now, you can opt out of this data collection, shall we call it?
[2714.70 --> 2717.18]  Shall we be kind to just call it data collection?
[2717.60 --> 2724.98]  There are some settings in the privacy settings of Plex itself, which is all controlled on the server side, on the Plex server side,
[2725.36 --> 2729.68]  because these things are not local to you as a server admin.
[2729.84 --> 2736.60]  They are local to Plex as the, I guess, the glue service that connects everything together, right?
[2736.60 --> 2742.82]  So you can go into your app.plex.tv website and go under privacy settings and, you know,
[2743.32 --> 2745.52]  click through a bunch of settings and disable a bunch of stuff.
[2745.90 --> 2751.02]  There's a link to the Reddit thread where all this stuff is actually the top post now, which will be in the show notes.
[2751.78 --> 2756.22]  What I found was the most malicious part of this whole activity was it was opt-in by default.
[2756.34 --> 2763.08]  Like, I didn't knowingly select and say it was okay to share my watch history with my friends.
[2763.08 --> 2768.08]  I mean, I guess I kind of became aware that there was something in the corner, a bit like Spotify, that said,
[2768.18 --> 2771.64]  here's what, you know, Chris has been watching this week or whatever.
[2772.36 --> 2773.66]  I didn't mind that as much.
[2773.88 --> 2780.28]  Or, like, I just noticed, because, again, I don't use the Plex app a ton, but I noticed just recently when I started a show,
[2781.04 --> 2783.72]  it said, I'm the first among my friends to watch this.
[2783.84 --> 2790.92]  Just a little badge there that says, I'm the, I don't, that's, that kind of sharing with a few select people that I,
[2790.92 --> 2796.24]  which is just a small handful of people, that was the line I was okay with them walking up to.
[2796.72 --> 2799.26]  And it didn't make me think a lot about how they're doing it.
[2799.84 --> 2803.66]  And it seemed fine because you guys can connect to my Plex server if you want and see what's on there.
[2803.74 --> 2804.66]  So, like, that seemed fine.
[2806.04 --> 2808.22]  But they took what could be a decent little feature.
[2808.96 --> 2812.52]  Like, so, like, we could sit down on a call and be like, oh, Alex, I see, I see you started the,
[2812.70 --> 2813.98]  you watched the latest Rick and Morty.
[2814.06 --> 2815.06]  Like, you know, what'd you think, right?
[2815.06 --> 2819.84]  Like, it could, it took what could have been a water cooler conversation to now,
[2820.02 --> 2823.62]  now they've pissed off another huge portion of their user base.
[2823.76 --> 2828.20]  And you're right, it's ridiculous that when I wanted to, in order to get that feature
[2828.20 --> 2831.30]  and to just kind of take advantage of some of the social features with you guys,
[2831.36 --> 2835.24]  I ended up getting slapped with the sharing, oversharing of information.
[2835.46 --> 2838.54]  And now I've had to rip all those settings out and turn all that stuff off.
[2839.12 --> 2839.22]  Yeah.
[2839.22 --> 2843.46]  And, you know, some folks, you know, play devil's advocate for a second,
[2843.92 --> 2848.98]  were saying, oh, it's okay because they had this full screen pop-up about these discover features,
[2849.04 --> 2852.94]  these sharing features that came up and I clicked past it and I said it was okay.
[2853.44 --> 2854.08]  I disagree.
[2854.26 --> 2857.54]  I find that such an unhealthy UX pattern.
[2857.64 --> 2858.68]  I really hate it.
[2859.24 --> 2862.58]  Wolfgang, you and I were just talking about this on Mastodon this week,
[2863.32 --> 2868.64]  about how when, there's two things about UX patterns in this that annoy me.
[2868.64 --> 2874.18]  One is when you have that kind of wizard of different options on a badly designed UI that says,
[2874.60 --> 2878.14]  well, first you have to click here to add something and then you click here to close something.
[2878.26 --> 2882.72]  And then you, like there's 15 options they make you go through with no skip button.
[2882.96 --> 2884.08]  That's one that I really hate.
[2884.14 --> 2890.76]  The second one is when I'm loading up Notion for work in the morning or Plex to watch,
[2891.08 --> 2894.00]  like I am in the middle of accomplishing a task.
[2894.64 --> 2898.58]  The last thing I want to do is have that flow interrupted by stopping and going,
[2898.98 --> 2899.94]  oh, hang on a minute.
[2900.06 --> 2905.38]  I'm not going to start doing my work until I've read all of this information that's been presented in front of me.
[2905.64 --> 2906.56]  Would you like to write a review?
[2906.86 --> 2907.84]  Would you like to rate this out?
[2908.36 --> 2909.70]  That one pisses me off as well.
[2909.74 --> 2910.40]  So that's three things.
[2910.40 --> 2918.42]  So I just click the X like most people I assume or OK, just whatever it is to get it out of my way and get on with the task that I was trying to do.
[2918.42 --> 2929.22]  I would have preferred that to be some kind of a like a banner at the top of the screen said, hey, and it persists for the next month until I click OK.
[2929.68 --> 2935.32]  And if I don't click OK, it doesn't assume that it's OK to share my information with friends and family.
[2935.64 --> 2939.10]  What planet was the person who came up with this on?
[2939.32 --> 2939.84]  I'm sorry.
[2939.92 --> 2942.48]  It's just got me all fired up, Chris.
[2942.48 --> 2945.34]  They must not have self-hosters working there anymore.
[2945.98 --> 2946.84]  Maybe they've all quit.
[2947.72 --> 2950.70]  Maybe they've all left and gone and started businesses or something.
[2950.96 --> 2960.98]  But because they have got to get in the head of their customer and understand that some of the people that are using Plex don't want to be on the grid.
[2961.42 --> 2963.70]  They want to be off the grid with their media stash.
[2963.70 --> 2980.42]  And so if you're going to do these social features with the hope to expand user base and become like a single plane of glass for all media content and reach out there and take advantage of everybody's social connections, then you have got to baby step this thing with privacy being your first priority every single time.
[2980.76 --> 2981.88]  And here's how you could have done it.
[2982.42 --> 2985.54]  You send out the email that we all saw that freaked us all out.
[2985.82 --> 2990.42]  But you send it just to me and you say, hey, next week we're starting to send these out.
[2990.76 --> 2992.26]  Would you like to opt out of this feature?
[2992.26 --> 2995.76]  And maybe 60% of us would have opted out.
[2995.88 --> 2997.88]  Maybe you would have had a massive opt-out amount.
[2998.86 --> 3002.82]  But that would have been better than, well, now we're leaving Plex entirely, right?
[3003.66 --> 3013.26]  It would have been better than we all just turned this feature off and we just ripped these features out in the settings and now it's all over Reddit and it's all over everywhere how to turn this stuff off, which we weren't even thinking about turning off before.
[3013.44 --> 3014.78]  You would have prevented all of that.
[3014.92 --> 3021.94]  You would have prevented all the miscommunication around what this actually sharing with the misunderstanding of people didn't realize that their titles were in your database.
[3022.26 --> 3029.88]  Like all of that could have been preemptively caught by just shooting me an email a week before saying, hey, starting next week, we're going to be sending these emails out to your friends.
[3030.20 --> 3032.28]  Here's an example of what one of these emails look like.
[3032.54 --> 3034.68]  Here's a link to opt out of the settings if you don't like it.
[3034.88 --> 3036.46]  Here's a little bit about our privacy policy.
[3036.46 --> 3043.14]  This feels not too far away from that Google Photos moment that we had a year ago.
[3043.44 --> 3044.18]  Was it a year ago?
[3044.34 --> 3045.22]  A while ago.
[3045.70 --> 3046.08]  Wait, wait.
[3046.14 --> 3057.00]  Something happens and it just confirms the absolute worst case scenario or the suspicions that we've had for a long time about the various different things that you can.
[3057.62 --> 3058.64]  Metadata is powerful.
[3058.78 --> 3060.60]  We should know this from Cambridge Analytica, right?
[3060.60 --> 3075.66]  We should know this, but it's only once all these things actually get connected together and presented to you in an easy to digest format, such as this week in Plex Review emails, that your brain goes, oh, well, now I've got to turn it off.
[3075.70 --> 3077.30]  I can't just ignore this any longer.
[3077.30 --> 3085.54]  You know what it is too is it confirms that just by passively using the thing, you are at risk.
[3086.34 --> 3091.54]  Just by passively using it in the day-to-day use, you're being exposed and you're at risk.
[3091.86 --> 3093.00]  And that's the problem.
[3093.36 --> 3101.18]  As soon as that has been confirmed, you're like, well, then I have to get off because just using this, my privacy is being encroached upon.
[3101.48 --> 3102.98]  This information is being put out there.
[3103.06 --> 3104.26]  Some people are going to get embarrassed.
[3104.26 --> 3108.92]  Like the whole thing is just – it's a sliding situation that just seems to be getting worse.
[3109.04 --> 3114.88]  And this is the point on the slide where we're like, oh, oh, it's a little bit worse than we realized.
[3115.06 --> 3115.42]  Okay.
[3115.86 --> 3116.38]  All right.
[3116.42 --> 3119.76]  I mean I know I like intro skipping and I like it a lot.
[3120.68 --> 3127.98]  And anybody who doesn't think intro skipping is a quintessential feature can go pound sand because it is a fantastic quintessential feature.
[3128.84 --> 3129.72]  Absolutely necessary.
[3129.72 --> 3133.34]  But I'm – if I can't have perfect intro skipping, so be it, Alex.
[3133.74 --> 3134.52]  So be it.
[3135.16 --> 3137.06]  I'm firing my jellyfin container back up.
[3137.36 --> 3140.82]  I'm getting that 10.8.13 release in that just came out this week.
[3141.36 --> 3142.40]  And we're doing this thing.
[3142.44 --> 3145.74]  And by the way, I never got any modal pop-up because I use Infuse.
[3146.74 --> 3148.88]  So I never even knew it was going on.
[3149.10 --> 3149.84]  Take that, Reddit.
[3149.84 --> 3150.26]  I'm getting it.
[3151.34 --> 3151.86]  Huh.
[3154.38 --> 3156.02]  45homelab.com.
[3156.22 --> 3158.60]  Premium storage servers for the HomeLab.
[3158.74 --> 3159.94]  They're finally here.
[3160.02 --> 3167.78]  If you're looking for an open HomeLab server that's strong, it's big, it's fast, and it doesn't compromise in any way on build quality,
[3168.36 --> 3171.26]  45 HomeLab, that's a new division from 45 Drives.
[3171.26 --> 3178.44]  They've taken their enterprise design and philosophy, and they've scaled it down to the HomeLab, and it is here.
[3178.86 --> 3184.08]  The HL15, the premium HomeLab storage server, it's beautifully designed, beautifully built.
[3184.30 --> 3186.26]  It's got 15 bays for disks.
[3186.78 --> 3189.22]  I suppose that's where the 15 comes in the HL name.
[3189.52 --> 3192.48]  And it's designed and manufactured and assembled in North America.
[3192.74 --> 3197.82]  It's built with steel and with screws, not rivets, so you can take it apart if you need to.
[3197.82 --> 3200.28]  And they have multiple design options.
[3200.68 --> 3203.10]  So you can get it with a fully built, ready-to-go system.
[3203.58 --> 3209.22]  You can get just the chassis and the backplane, or probably the route I might go, the chassis, the backplane, and the PSU,
[3209.28 --> 3211.92]  and then you bring your own MOBO and CPU and memory and stuff.
[3212.28 --> 3213.40]  But however you like it.
[3213.44 --> 3215.28]  Perhaps you'd just rather have it come out of the box ready to go.
[3215.32 --> 3216.30]  They got that for you, too.
[3216.56 --> 3218.46]  So go to 45homelab.com.
[3218.62 --> 3222.30]  This has been inspired and designed by the feedback from our self-hosted community,
[3222.46 --> 3226.76]  and now it is here as a product, and it is a sweet-looking rig.
[3226.76 --> 3229.02]  45homelab.com.
[3231.36 --> 3233.38]  Welcome into ESP Corner, everybody.
[3233.66 --> 3237.80]  I have been doing some really fun projects with the ESP8266 this week.
[3238.58 --> 3241.82]  Recently, I got a new 3D printer, the Bamboo Labs X1 Carbon.
[3242.16 --> 3248.68]  And so, like any new 3D printer nerd, I mean, I'm not new to 3D printing, but with a new toy to play with,
[3248.68 --> 3258.54]  I went browsing printables.com and Thingiverse and all the rest of it and found that somebody has finally made a 3D printed blast gate for woodworking dust collection.
[3259.20 --> 3262.84]  Not only that, they've also made one where you can attach a servo to it.
[3262.86 --> 3266.24]  And this is a project I've been wanting to tackle for years.
[3266.24 --> 3270.36]  So what I want to do is put a current sensor on a particular outlet.
[3270.56 --> 3275.40]  So one for my table saw, one for my planer, one for my drum sander.
[3275.40 --> 3283.88]  And when those tools turn on, it opens the correct blast gate in the piping to allow the sawdust from that tool into the dustbin, right?
[3284.10 --> 3284.98]  That's the idea.
[3285.62 --> 3292.56]  But using ESP Home and ESP8266s, I've been able to actually control these RC servos.
[3292.62 --> 3296.74]  So I'm just using servo motors from remote control cars to open these blast gates.
[3297.18 --> 3298.70]  It's amazing.
[3299.08 --> 3300.52]  It's so cool.
[3301.00 --> 3304.68]  Wolfgang, have you had a chance to play around with these little tiny little ESP devices?
[3305.40 --> 3306.14]  I have, actually.
[3306.36 --> 3315.18]  I think one of the earliest things in my channel is running a Wi-Fi D author on an ESP8266.
[3315.70 --> 3316.98]  So that was a lot of fun, actually.
[3318.08 --> 3319.20]  I'll have to check that out.
[3319.54 --> 3321.90]  It's like a precursor to the Flipper Zero, that kind of thing.
[3321.94 --> 3322.48]  Yeah, absolutely.
[3322.88 --> 3328.14]  I am very excited to see that the ESP32 S3 box is shipping.
[3328.44 --> 3332.64]  This is the little tiny unit that has a touchscreen on it.
[3332.64 --> 3334.94]  It's got two microphones built in.
[3335.10 --> 3343.44]  It has onboard voice processing with, like, up to 200 different customizable keywords and command words that you can set.
[3343.74 --> 3345.52]  It's got USB-C for charging.
[3345.52 --> 3349.68]  In fact, it even has, like, a high-density PCI connector on the bottom of the thing.
[3349.74 --> 3353.74]  So you can put it into docks via a PCI connection and then expand it from there.
[3354.10 --> 3364.50]  And this ESP32 S3 box 3 is the device and kit that I think is the one to get for the next phase of home assistance here at Voice.
[3364.50 --> 3373.24]  This, I believe, will be the, like, go-to recommended by this box if you want to set up a home assistant voice assistant.
[3373.56 --> 3375.44]  And it's got a little screen on there, too.
[3375.66 --> 3380.82]  And it's a lot nicer than that $13 dime-sized ESP, which is – that little Echo is a great device.
[3381.52 --> 3383.88]  Really handy for developing and testing.
[3384.70 --> 3389.16]  But this ESP32 S3 is going to be, like, build it into products.
[3389.16 --> 3392.16]  It's designed specifically to work as a voice assistant.
[3392.88 --> 3395.76]  And I think home assistant developers already have their eyes on this.
[3395.90 --> 3397.86]  And it's – nobody said anything.
[3398.24 --> 3399.58]  They haven't said a word yet.
[3400.04 --> 3403.54]  But I already ordered mine this morning, and I'm probably going to order another one after the show.
[3404.54 --> 3405.38]  You know it's coming.
[3406.14 --> 3406.40]  Yeah.
[3406.84 --> 3407.04]  Yeah.
[3407.12 --> 3412.04]  It's coming, I think, mid-December, I think, is when it was going to be shipping.
[3412.14 --> 3412.64]  We'll see, though.
[3413.40 --> 3415.02]  Mid to early December, but I don't know.
[3415.10 --> 3415.98]  I'm not getting my hopes up.
[3415.98 --> 3420.54]  What would an episode of the Self-Oasted Podcast be without some kind of a mention of home assistant, huh?
[3420.94 --> 3421.78]  Yeah, there you go.
[3421.96 --> 3424.40]  I also found – now, this might be interesting to you in the RV.
[3424.98 --> 3429.64]  With living in a tin can, Wi-Fi can be problematic sometimes.
[3430.34 --> 3435.00]  And I've heard you say before, it would be great if I could just have hardwired ESP devices.
[3435.30 --> 3437.44]  Well, I have good news for you, sir.
[3437.44 --> 3442.72]  The WESP32 is a wired ESP32 with PoE.
[3443.38 --> 3444.94]  That's awesome.
[3444.94 --> 3445.14]  Awesome.
[3445.74 --> 3454.34]  That takes the ESP32 devices from borderline hobbyist, which I have run in production, to, I think, production.
[3455.06 --> 3455.92]  That's incredible.
[3456.78 --> 3460.70]  I mean, to be able to power them off of PoE, too, would be so easy.
[3460.80 --> 3462.10]  I mean, we'd solve so many problems.
[3462.62 --> 3465.32]  The downside is they are 50 bucks a pop.
[3465.32 --> 3472.52]  I mean, one of the original draws of an ESP device was it was five or ten at most dollars.
[3473.84 --> 3478.58]  PoE makes things a little more complicated because it's a custom circuit board and all the rest of it.
[3478.74 --> 3488.80]  But, you know, if you're building home automation for the next 10 years into your RV, then actually you won't find any commercial products for less than 50 bucks a pop.
[3488.80 --> 3493.10]  Well, right. And right now I've built some into my wall that are on Wi-Fi.
[3493.46 --> 3497.10]  And so I'm kind of now stuck to that SSID forever.
[3497.10 --> 3508.22]  Or I've got to do some sort of thing where I update their config, push the config to the devices, and they would go offline when they would come back online.
[3508.34 --> 3509.82]  And then I would stand up the new one.
[3509.90 --> 3514.16]  I mean, it's just like I've really done myself a solid here for the future.
[3514.26 --> 3517.40]  Like I'm going to have a – I'm going to look back and think, what was I thinking?
[3517.52 --> 3519.04]  So, you know, you could wire that.
[3519.04 --> 3522.76]  If you could wire that, then you just don't even have to worry about that kind of stuff.
[3522.82 --> 3524.40]  And it just makes it a little bit more stable, too.
[3524.88 --> 3527.80]  Well, that actually leads us nicely into our first piece of feedback.
[3528.06 --> 3536.04]  Noel asks via Matrix, I often hear that you should set up a guest network for all of your IoT devices to keep them separate from your primary network.
[3536.52 --> 3537.66]  You did do that, right, Chris?
[3538.38 --> 3538.72]  Yeah.
[3539.28 --> 3539.74]  Sort of.
[3540.30 --> 3540.96]  I used to.
[3541.44 --> 3547.38]  Noel says, if I do that with, say, my Chromecast, then won't that mean I can't cast to it from my phone anymore?
[3547.38 --> 3549.30]  How do people typically work around that?
[3550.10 --> 3550.20]  Yeah.
[3550.38 --> 3554.70]  And I saw some people in the Matrix say, yeah, I just put the Chromecast in my main VLAN.
[3554.94 --> 3555.92]  You know, screw it.
[3555.94 --> 3556.58]  It's fine.
[3556.92 --> 3559.38]  But there are ways of solving this problem.
[3559.42 --> 3561.60]  Did you have any that you would employ?
[3562.26 --> 3564.64]  Well, it's all because the Chromecast works on MDNS.
[3564.84 --> 3566.42]  So you just need to handle that.
[3566.66 --> 3566.92]  Yes.
[3567.30 --> 3571.10]  And create whatever rules you need to for that traffic to traverse VLANs.
[3571.46 --> 3574.56]  And once you do that, then, you know, jobs are good.
[3575.06 --> 3575.46]  Yeah.
[3575.46 --> 3576.98]  We'll put a couple of links in the show notes.
[3577.38 --> 3579.46]  One way to do it was some unified network gear.
[3579.96 --> 3585.08]  Another way to just do it, you know, like Alex was saying, just the classic kind of just make sure it's getting to the right network.
[3585.22 --> 3589.56]  And we'll put one in there also for inter-VLAN casting with Chromecast.
[3590.20 --> 3592.58]  Fun fact about MDNS that I learned this week.
[3592.74 --> 3594.20]  This might be common knowledge.
[3594.30 --> 3594.66]  I don't know.
[3594.76 --> 3600.02]  But if you've been using Macs for a while, I'm sure you've seen the Bonjour protocol.
[3600.90 --> 3601.10]  Yeah.
[3601.10 --> 3602.80]  That is just MDNS.
[3603.06 --> 3603.24]  Yeah.
[3603.32 --> 3604.52]  Which is what Apple decided to call it.
[3604.62 --> 3608.04]  And when I read that this week, I was like, oh, well, now I feel stupid.
[3608.44 --> 3610.38]  I thought they weren't allowed to call it Bonjour anymore.
[3610.58 --> 3612.76]  I thought they, maybe they changed it from something else.
[3612.92 --> 3613.12]  But yeah.
[3613.18 --> 3614.48]  I thought they invented it, actually.
[3614.82 --> 3615.90]  But maybe that's wrong.
[3616.38 --> 3616.66]  Yeah.
[3616.70 --> 3617.02]  Who knows?
[3618.08 --> 3618.32]  Yeah.
[3618.32 --> 3620.00]  It's kind of nice.
[3620.10 --> 3621.68]  It's how your devices all discover each other.
[3621.82 --> 3629.90]  But it is also, when you ever do a line cap, if you ever run Wireshark and just look at your Ethernet traffic, there's a lot of MDNS traffic on there.
[3629.94 --> 3630.32]  Just stuff.
[3630.58 --> 3630.96]  I'm here.
[3631.10 --> 3631.50]  I'm here.
[3631.82 --> 3632.24]  I'm here.
[3632.70 --> 3633.56]  Is this guy here?
[3633.62 --> 3634.10]  Yep, I'm here.
[3634.20 --> 3635.46]  A lot of that on the network.
[3636.40 --> 3638.08]  We got some boosts into the show, too.
[3638.14 --> 3639.96]  That came in over the network as well.
[3640.10 --> 3643.12]  And Shaft and Spanner is our Pollard boost.
[3643.22 --> 3643.84]  That's good.
[3644.06 --> 3644.64]  That's good.
[3645.20 --> 3646.50]  33,000 sats.
[3646.50 --> 3648.40]  It's first time boost, too.
[3648.48 --> 3655.26]  He says, Alex and Brent's chat about hard drives finally convinced me to take the plunge and subscribe to the show as I really want to hear the second half of that discussion.
[3655.76 --> 3661.40]  I'd be interested to know if Alex's views on new hard drive rituals have changed as drive sizes have increased.
[3661.90 --> 3666.46]  I bought a 16-terabyte drive over the summer, and I've been running burn-ins.
[3666.54 --> 3667.80]  It took well over a month.
[3668.00 --> 3668.84]  Keep up the great work.
[3668.84 --> 3672.30]  I love listening to the show during my commute, which is an hour and a half each way.
[3672.60 --> 3674.40]  But thankfully, it's only two days per week.
[3674.40 --> 3676.72]  Well, thank you, Shaft and Spanner, for the boost.
[3676.94 --> 3684.32]  For those that aren't familiar, my burning ritual is to basically bad blocks the drive basically four times with different data.
[3684.92 --> 3685.70]  And yes, you are right.
[3685.80 --> 3694.72]  That was born out of, I think, originally doing an Unraid pre-clear, like, ritual on, like, one or two or three terabyte drives, which took a day or two.
[3694.72 --> 3696.34]  Whereas now you're right.
[3696.52 --> 3702.90]  I did a bag block scan on the 18 terabyte drives that I bought as part of that chat with Brent.
[3703.34 --> 3707.98]  It took, I think, 13 days of solid effort on the drive.
[3708.20 --> 3721.58]  But I stand by the logic behind it of trying to weed out the weaklings early on, whilst they're still in the retailer return period and exchange period, rather than having to go through an RMA process with Seagate or Western Digital or whatever.
[3721.58 --> 3729.18]  And also before I've committed any actual data to them, because once you start filling up a drive like that, it's like once you fill your house up with sofas.
[3729.90 --> 3734.42]  Like, you've got to put them somewhere if you want to paint the room or RMA the hard drive, right?
[3734.42 --> 3739.24]  It's, but there is a school of thought to say that how long is long enough to stress the drive?
[3739.32 --> 3740.20]  Is a week long enough?
[3740.32 --> 3742.42]  Is two weeks too long?
[3742.72 --> 3744.66]  Because it is incredibly stressful on the drive.
[3744.74 --> 3749.38]  And maybe they aren't designed to be constantly thrashed for two weeks solid.
[3749.48 --> 3749.82]  I don't know.
[3750.12 --> 3750.92]  But this could be.
[3751.08 --> 3754.34]  I've been doing it religiously for the last decade.
[3754.44 --> 3756.74]  So I don't see any reason to change now.
[3756.94 --> 3758.38]  Maybe that makes me a Luddite.
[3758.38 --> 3763.08]  I put them through a couple of weeks of testing, but nothing really super dramatic.
[3763.24 --> 3765.08]  I just sort of put some workloads on there.
[3765.18 --> 3769.34]  I have just checked using smart data on one of our servers.
[3769.64 --> 3778.24]  And in this one server, I've got one, two, three drives that are nine years old that have been powered on for nine years.
[3778.76 --> 3782.18]  And one drive that's been powered on for 10 years.
[3782.48 --> 3784.74]  The rest have all been powered on for either seven or five years.
[3785.08 --> 3785.84]  Ten years.
[3785.84 --> 3789.38]  And there's nothing younger than four years in this server.
[3790.16 --> 3792.02]  And most of them are like around five or seven.
[3792.32 --> 3794.46]  It was just Black Friday, my friend.
[3794.50 --> 3794.82]  I know.
[3795.14 --> 3795.64]  I know.
[3795.78 --> 3796.12]  I know.
[3796.16 --> 3799.32]  I look at that and think, I wish I would have checked that a couple of weeks ago or so.
[3799.68 --> 3800.58]  What about you, Wolfgang?
[3800.66 --> 3802.20]  What's your theory on hard drives?
[3802.62 --> 3805.98]  I mean, for me, I try and keep everything under about five years old if I can.
[3806.36 --> 3806.58]  Yeah.
[3807.42 --> 3808.32]  Don't do what I do.
[3808.50 --> 3808.68]  Right.
[3808.76 --> 3810.70]  So my drives are actually fairly new.
[3810.70 --> 3814.64]  I actually replaced my WD Reds with Seagates for a video.
[3814.64 --> 3818.18]  I don't have any drives that are older than a year right now in my system.
[3818.30 --> 3820.32]  But it's only three drives, so it's easy, I guess.
[3820.82 --> 3823.80]  I will say those 10-year drives and nine-year drives are Western Digitals.
[3823.98 --> 3824.90]  Yeah, they're solid drives.
[3825.02 --> 3825.30]  I agree.
[3825.42 --> 3825.88]  I agree with that.
[3826.60 --> 3832.26]  MCZP, or MixZip as I call them, came in with 25,000 sats and just was really appreciative on the image discussion.
[3833.08 --> 3835.68]  And he says self-hosted has really impacted his home lab.
[3835.90 --> 3836.82]  Well, thank you.
[3836.88 --> 3838.30]  And his wallet in a negative way.
[3838.30 --> 3842.46]  Yeah, we have that effect on people, and I'm not going to apologize for that one.
[3843.12 --> 3844.76]  It's all investing in your education.
[3844.92 --> 3846.30]  You're a better person now, right?
[3846.58 --> 3846.92]  Right.
[3848.12 --> 3853.02]  Bolipara comes in with a row of McDucks, 22,222 sats, first-time booster.
[3853.56 --> 3855.68]  It wanted to pass along Git Annex.
[3855.80 --> 3856.08]  They write,
[3856.08 --> 3861.78]  It provides deduplication, location tracking, bit rot protection, redundancy, and custom metadata.
[3862.24 --> 3866.90]  You can create a repo and then clone at multiple locations, either online machines or external media.
[3867.20 --> 3871.92]  You can add your own data repo and set policies, which repo should get copies of that data.
[3872.46 --> 3875.38]  I'll put a link to Git Annex in the notes.
[3875.44 --> 3876.14]  That's a great heads up.
[3876.36 --> 3881.86]  It's nice because once you get over the hump of learning Git and the various concepts required,
[3881.86 --> 3887.12]  a lot of people think Git and GitHub are synonymous with one another, but they're not.
[3887.28 --> 3891.46]  GitHub is just like a hosted cloud service that has Git in the name.
[3892.02 --> 3898.40]  Git is the version tool that lets you add things and remove things and version control things from a local repository.
[3898.98 --> 3906.34]  The fact that you have a remote thing that you push it to called GitHub, it's totally irrelevant, really, to Git itself.
[3906.34 --> 3912.70]  So I'm always interested in seeing these kinds of tools, particularly to use Git with use cases where it may not have been originally designed for,
[3912.84 --> 3917.28]  because it was developed by Linus Torvalds as part of the Linux kernel development process.
[3917.46 --> 3921.64]  So ostensibly, it's just a very good tool at managing text changes.
[3922.30 --> 3922.32]  Yeah.
[3922.66 --> 3926.42]  My goal for next year is to get my Nix config for my different machines onto Git.
[3926.94 --> 3927.50]  Just got to do it.
[3927.84 --> 3929.52]  I had so much fun with Nix this week.
[3929.62 --> 3931.04]  Perhaps we should talk about that in the post show.
[3931.26 --> 3931.88]  Oh, yes.
[3931.88 --> 3936.18]  I could install an entire server from a flake in like three minutes.
[3936.40 --> 3937.20]  It's amazing.
[3937.40 --> 3937.54]  Oh.
[3938.44 --> 3941.66]  Meditak comes in with a Spaceballs boost, one, two, three, four, five sets.
[3942.18 --> 3946.44]  And he wanted to give the booster who was asking about Nixifying the deck some information.
[3946.60 --> 3949.18]  It's called, I guess, maybe Jovian Nix OS.
[3949.36 --> 3950.28]  We'll put a link in the notes.
[3951.04 --> 3956.38]  It is drivers and all the stuff you need pre-configured for the deck hardware functioning in game mode.
[3956.66 --> 3958.62]  You can also change to the desktop mode.
[3958.80 --> 3959.94]  And of course, it's based on Nix.
[3959.94 --> 3961.36]  He says he can't recommend it enough.
[3962.06 --> 3962.32]  Wow.
[3962.54 --> 3966.66]  There is a few things you have to do to get your deck to accept that.
[3966.72 --> 3968.12]  But they have it all in the documentation.
[3969.36 --> 3970.24]  Well, there you go, Alex.
[3970.32 --> 3971.22]  Nixify your deck, huh?
[3971.96 --> 3972.66]  I don't know, though.
[3972.66 --> 3975.78]  The whole thing about the deck is that it's just a working piece of hardware, right?
[3976.32 --> 3977.78]  It just works.
[3978.62 --> 3981.56]  Greeno comes in with 5,000 SATs using the podcast index.
[3981.64 --> 3982.08]  Hey, guys.
[3982.52 --> 3983.20]  With all this talk.
[3983.24 --> 3983.92]  Oh, this is great.
[3984.18 --> 3991.30]  With all this talk around this Plex stuff recently, I felt I needed to chime in with my two cents with a prediction I think Plex is heading in and hopefully get your thoughts.
[3991.88 --> 4021.88] 
[4021.88 --> 4025.64]  They kind of whittle down the sharing program over time, he says.
[4026.52 --> 4032.44]  And essentially, inevitably, step 10 is Plex Media Server is abandoned.
[4032.60 --> 4034.38]  And then there's just Plex the service.
[4035.08 --> 4035.48]  What do you think?
[4035.48 --> 4047.30]  I mean, if you think about Plex as just basically being a bunch of clients, that's always the thing that people give Plex the most credit for is the fact that they are on every smart TV made in the last decade.
[4047.58 --> 4049.16]  They're on every game console.
[4049.36 --> 4050.22]  They're on every smart.
[4051.24 --> 4055.18]  That's probably Plex's biggest strength is they're everywhere.
[4055.18 --> 4059.32]  And you just send an update to those clients that says default to the Plex streaming service.
[4059.48 --> 4061.94]  And then over time, you just remove the feature to connect to home servers.
[4062.44 --> 4063.84]  Softly, softly, catchy monkey, I guess.
[4064.30 --> 4064.78]  Oh, man.
[4064.80 --> 4066.42]  I hope that's not the way it goes.
[4066.94 --> 4068.72]  Oh, but you know it's going to be.
[4068.96 --> 4070.32]  The writing is on the wall.
[4071.04 --> 4072.26]  Thank you for scaring me, Greeno.
[4074.42 --> 4075.08]  All right.
[4075.70 --> 4079.08]  Yevz comes in, said to finally set up Albie, been a listener since episode nine.
[4079.24 --> 4080.40]  Thanks for the inspiring discussion.
[4080.40 --> 4086.82]  And I wanted to also give a shout out to Gene Bean, who wanted to just send us a little love for the storage chat.
[4086.92 --> 4091.40]  We had a couple of folks that wrote in that really liked the chat you and Brent had about his storage setup.
[4091.88 --> 4093.04]  Well, we'll have to do a part three then.
[4093.12 --> 4095.94]  I think his hard drives are burning in right now as we speak.
[4096.00 --> 4098.64]  And he's about to get on a plane to go to Berlin again.
[4098.96 --> 4100.76]  So by the time he gets back, they might be finished.
[4101.14 --> 4102.66]  Yeah, maybe we'll have him on when he gets back.
[4103.06 --> 4103.74]  That'd be really great.
[4103.90 --> 4105.62]  Thank you, everybody who boosted in.
[4105.92 --> 4109.36]  We just did a small selection of the boosts, but we read all of them.
[4109.36 --> 4111.56]  And we put them in our boost barn, which is linked in the notes.
[4112.18 --> 4117.34]  And we do appreciate that we had nine folks boost in and we stacked 115,933 sats.
[4118.10 --> 4118.78]  Thank you, everybody.
[4119.04 --> 4120.86]  We appreciate you and our members.
[4121.08 --> 4127.66]  If you'd like to become a self-hosted site reliability engineer, you can become an SRE at selfhosted.show.sre.
[4128.14 --> 4129.78]  You get to sponsor the show yourself.
[4130.12 --> 4135.66]  So as a result, you get an ad-free version of the show that we put in a little special post show just for our members.
[4136.24 --> 4138.28]  That Black Friday sale goes on for one more week.
[4138.28 --> 4142.26]  Use the promo code Black Friday and you take $2 off the cost per month for a year.
[4142.98 --> 4145.02]  Selfhosted.show.sre.
[4145.02 --> 4148.46]  I wanted to say thank you to Wolfgang for joining us.
[4148.50 --> 4149.96]  Is there any way you'd like to send people?
[4150.30 --> 4150.96]  Thank you for having me.
[4151.06 --> 4154.34]  I guess just youtube.com slash at Wolfgang's channel.
[4154.72 --> 4155.24]  Easy, easy.
[4155.32 --> 4156.50]  We'll put a link in the notes for that too.
[4156.56 --> 4156.94]  You know it.
[4157.30 --> 4158.46]  There's some great stuff over there.
[4158.56 --> 4163.32]  Now, you all know by now selfhosted.show slash contact is the place to go to get in touch with us.
[4163.40 --> 4166.30]  And you can find me at alex.ktz.me.
[4166.30 --> 4168.18]  You can find me in the Matrix.
[4168.50 --> 4169.54]  I'm at Chris Elias in there.
[4169.64 --> 4173.14]  Details at jupiterbroadcasting.com slash Matrix.
[4173.40 --> 4176.82]  And you can find the show on Weapon X at Self Hosted Show.
[4177.34 --> 4178.16]  Weapon X.
[4178.64 --> 4180.64]  Yeah, that Matrix is really hopping these days.
[4180.76 --> 4183.60]  I am joining the element chat more and more often.
[4183.92 --> 4186.26]  You know, it's really moving along.
[4186.44 --> 4188.22]  So thank you very much for listening, everybody.
[4188.42 --> 4190.76]  That was selfhosted.show slash 111.
[4190.76 --> 4220.74]  Thank you very much for listening.
