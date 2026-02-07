[0.00 → 2.36] Welcome into lucky episode 113, everyone.
[2.72 → 6.70] Can we just take a minute, chaps, and appreciate the fact that Bitwarden
[6.70 → 10.20] haven't raised their prices in, as far as I can remember, forever?
[10.72 → 12.00] My renewal just came through today.
[12.10 → 13.72] Ten bucks for another year.
[14.64 → 15.50] Still money well spent.
[16.18 → 16.96] I feel like it.
[18.04 → 20.78] That's ten bucks I'd be happy to spend every year.
[21.50 → 22.12] You're right.
[22.62 → 22.82] Hmm.
[24.20 → 25.66] You know what would be a nightmare to Alex?
[25.66 → 30.52] If they had figured out some way to open up the password database on the back end
[30.52 → 35.12] and were monetizing it for ads or something, that would be the worst.
[35.32 → 37.58] But, of course, that's not the case.
[37.68 → 40.14] Brent still has refused to join.
[40.36 → 42.96] He almost did, but he's refused to join the Bitwarden cult.
[43.16 → 44.74] Oh, he's putting me out there.
[44.82 → 45.52] But you're back on the show.
[45.62 → 46.12] Welcome back, Brent.
[46.22 → 46.58] Hello.
[47.00 → 47.82] It's good to be back.
[47.98 → 48.48] Happy holidays.
[49.40 → 49.74] Okay.
[49.84 → 50.64] You just shocked me.
[50.90 → 53.28] I can hardly realize that it's the holidays.
[53.28 → 54.56] I think that means I'm way behind.
[54.98 → 55.30] Yeah, well.
[55.30 → 55.92] Oh, come on.
[56.02 → 60.58] You're just fresh back from Germany, straight off the fart tube, full of glue vine and candy
[60.58 → 61.12] apples, right?
[61.30 → 61.64] Right.
[62.20 → 63.64] He knows what he's talking about.
[64.02 → 64.26] Yeah.
[64.76 → 66.06] I'm sure it was beautiful over there.
[66.18 → 66.94] Yeah, it was really nice.
[67.02 → 71.28] I went to a couple of Christmas markets and, like, they have castles over there in Europe
[71.28 → 72.94] and one of them was at a castle.
[73.60 → 76.82] And these Christmas markets are, like, more fancy than you think.
[76.82 → 80.00] There's, like, tons of food and, like, celebrating.
[80.34 → 83.40] And glue vine is, yeah, like a muddled red wine thing.
[83.56 → 84.80] Just, like, people galore.
[84.80 → 86.22] It was an awesome experience.
[87.22 → 91.40] Glue vine makes the weather and the cold dark nights a little more bearable.
[91.56 → 92.14] Let's put it that way.
[92.26 → 92.82] I see.
[92.94 → 94.42] There's this other drink I had, too.
[94.62 → 95.68] Everybody's like, have the glue vine.
[95.74 → 96.22] So I had that.
[96.28 → 97.06] I was like, yeah, all right.
[97.10 → 97.60] That's pretty good.
[97.64 → 98.94] And then he was like, okay, have this.
[99.28 → 100.52] And they lit it on fire.
[100.90 → 103.22] And I was like, why didn't you offer me this one first?
[103.22 → 104.12] I forget what it was called.
[104.30 → 106.88] But it was a super awesome experience.
[107.14 → 109.36] Softly, softly catchy monkey, I think, with that.
[109.98 → 115.74] Well, it is a good episode to have you here because we're looking back at the state of our home labs for 2024.
[115.74 → 123.34] And it's been a huge year for you, both in hardware and connectivity and in just joining the next cloud crew.
[123.46 → 126.44] I have to imagine you're exposed to a lot more self-hosting over there.
[126.58 → 128.54] So we're going to get into all of that today, Alex.
[128.54 → 131.10] And I've added some categories.
[131.40 → 132.68] You've added some categories.
[133.14 → 135.46] We didn't discuss ahead of time.
[135.92 → 137.94] So we're going to get into it, into the show.
[138.24 → 144.84] And I kind of felt like we should start with the category that always is at the top of Reddit for self-hosted, which is dashboards.
[145.50 → 148.58] Yeah, people love pea cocking on Reddit with their dashboards.
[150.12 → 151.10] Dashboard for days.
[151.10 → 156.10] How many services can I fit into a one gigabyte Raspberry Pi or something, you know?
[156.10 → 159.12] And their screenshots often make me a little envious.
[159.52 → 161.20] I have dashboard envy very often.
[161.40 → 162.14] Is it the theming?
[163.02 → 176.96] I think it's often the – it's like the idea of I open up my browser and the vital information I need to know about my tasks, my calendar, the state of my system, whatever new media is available, whatever it might be.
[177.02 → 178.08] It's all on one screen, right?
[178.44 → 182.26] It's like my own version of msn.com or whatever, right?
[182.36 → 185.80] Like I launch the browser and boom, there it all is and it's fantastic.
[185.80 → 187.40] And boom, look at all this information and pow.
[187.96 → 189.88] I've seen everything and I don't need to worry about it.
[189.88 → 190.78] I can go about my day.
[191.34 → 193.16] That's the beautiful idea, I think, of the dashboard.
[193.60 → 197.70] But you gents have played with dashboards for years now, I feel like.
[197.84 → 198.24] Many years.
[198.24 → 203.22] So you must have a bunch of choices that you've been happy with in the past or found new ones.
[203.72 → 206.70] I mean, I don't even have – I haven't even started this journey.
[206.80 → 208.28] So I'm curious where I should launch in here.
[208.28 → 219.02] The trouble with dashboards is in this household at least, I'm always adding or removing stuff, which means there's yet another thing to keep on top of and keep maintained.
[219.26 → 223.62] And so, you know, I build a dashboard and I spend a few weeks perfecting it and tweaking it.
[223.62 → 225.14] You know, I've tried all sorts.
[225.22 → 226.12] I've tried Heimdall.
[226.32 → 227.62] I've tried Flame.
[227.94 → 228.38] There are dozens.
[228.52 → 228.78] Homer.
[229.24 → 229.76] Bunch of others.
[230.60 → 241.94] And then, you know, the entropy of maintaining my own self-hosted services and changing stuff means that I load up the dashboard one day, and it's just completely broken.
[241.94 → 246.10] And then I think, do I want to spend half an hour fixing this right now?
[246.26 → 247.12] No, I don't.
[247.22 → 248.42] And then I never come back to it.
[248.48 → 253.22] And inevitably, the dashboard just ends up like every other dashboard attempt I've ever tried before.
[253.84 → 255.52] And it just ends up in the trash.
[256.04 → 258.20] That's exactly why I don't stick with dashboards.
[258.38 → 259.74] I change things around.
[259.88 → 260.80] I try new things.
[260.90 → 263.42] Maybe I do that more than folks that don't do a podcast.
[263.96 → 264.36] I don't know.
[265.02 → 271.34] But I kind of go the direction of – not dashboards, but instead of having a dashboard,
[271.34 → 273.32] maybe I'll have net data on this machine.
[274.02 → 274.88] Yeah, I have Smoke Ping.
[274.94 → 275.98] I know Alex runs Smoke Ping.
[276.10 → 277.00] I have Smoke Ping running.
[277.10 → 279.54] I have, you know, I have information on my router.
[279.66 → 281.26] Like, I kind of have different spots.
[281.64 → 282.68] It's a little more siloed.
[282.74 → 288.22] But if I want to know how something in particular is doing, I generally have data on that particular machine.
[288.32 → 289.10] You know what I mean, Alex?
[289.52 → 296.56] Yeah, there is a difference between a dashboard, which is kind of like having a nicely laid out desk with drawers that are properly organized.
[296.56 → 303.18] And you can be like, right, this service lives on this machine over here is in this category of document management.
[303.46 → 308.64] And it's a very nice thing for the first few days when everything's all lined up perfectly.
[308.88 → 309.98] Yeah, when you get your screenshot.
[310.18 → 310.98] Yeah, exactly.
[311.42 → 316.66] But that's a different situation from going in and triaging stuff with, like, monitoring and stuff like that.
[316.66 → 325.92] So I put under this heading that my dashboard is actually Grafana, which I feed using Prometheus and InfluxDB underneath.
[326.64 → 330.00] And the reason I do that is just to get, you know, some basic trends.
[330.00 → 337.96] I can look at the last 90 days of what my hard drive temperatures have been or what all the, you know, various sensors that I want to check, you know, disk space.
[338.00 → 339.86] And I can spot any trends and stuff like that.
[340.16 → 341.58] I don't look at it every day.
[341.98 → 344.38] I typically only load it up if I've been having issues.
[344.38 → 351.06] But I do have some alerts set in healthchecks.io for things like if backup replications fail and stuff like that.
[351.14 → 355.08] So I'm aware we're crossing over from dashboards into monitoring as a category.
[355.30 → 358.86] But I think it's more relevant for most self-hosted, honestly.
[359.40 → 361.58] I could probably do with a bit more monitoring.
[362.00 → 363.20] I do have some basics.
[364.26 → 368.96] And I have not actually verified the alerting is working on those, but they should be emailing me if anything goes wrong.
[369.06 → 374.12] You know, there's no better monitoring system than trying to load up Jellyfin at 7 a.m. with your daughter in the bed.
[374.12 → 377.00] And trying to go to load Peppa Pig, and it doesn't work.
[377.06 → 380.46] And then you realize that one of the switches in your basement froze last night.
[380.62 → 383.40] And nothing pinged you to tell you that everything was down.
[383.78 → 390.72] Can I say that the media playback failures are my absolute most frustrating kinds of failures?
[390.98 → 394.62] Is when I get the dad, dad, it's not working.
[394.88 → 397.00] Or when I come in, I say, why are you streaming that on Netflix?
[397.84 → 400.04] Well, I tried to play it on Plex or Jellyfin.
[400.14 → 401.32] They don't know.
[401.32 → 402.28] Ella is three.
[402.28 → 402.48] It's not working.
[402.76 → 406.90] And she understands that the little buffering goes, daddy, it's not working.
[408.68 → 410.14] She's three, and she gets it.
[411.82 → 412.22] Yeah.
[412.64 → 415.38] Anyway, what do you do for a dashboard, Brent?
[415.48 → 417.54] I think you've sort of said not much, but.
[417.94 → 421.46] I didn't even realize that it would be useful for me.
[421.52 → 428.14] I mean, you guys know I've been building kind of a new storage system these days in the hopes of building a better home lab.
[428.14 → 430.10] It's been a disaster.
[430.56 → 430.72] Me.
[430.92 → 431.96] That's probably pretty accurate.
[432.26 → 438.94] A bit of a disaster the last few years with moving across the country and just like having bad Internets and not really putting effort into it and stuff.
[439.02 → 440.96] But all that feels like has changed.
[441.18 → 442.40] So I'm building from the ground up.
[442.44 → 448.08] So really, you can just assume I'm doing nothing and that I'll take all your tips and tricks and implement them soon.
[448.08 → 451.88] So keep me up to date when you have new ideas because I want to try those first.
[452.08 → 458.36] As you build it, Brent, just think about as you create different like services or applications, think about this is important to me.
[458.48 → 459.32] This isn't important to me.
[459.36 → 460.42] And keep a list of that.
[460.50 → 463.68] And then that could be where you build out a dashboard from just that list alone.
[463.92 → 464.04] Smart.
[464.04 → 468.52] That does sort of lead us nicely into the next category then, which is backups.
[468.64 → 476.70] And Brent, I will start with you because you and me in a very recent self-hosted had a nice long chat about hard drives and storage and that kind of thing.
[477.10 → 479.88] And as part of that, we talked a little bit about backups.
[480.00 → 481.88] So what have you got going on there?
[481.88 → 487.62] Well, I've recently dived into Borg as kind of backup situation.
[487.80 → 496.64] And I did because I couldn't get others like file system based backup solutions to work, which I was playing with, specifically Butters, like sending across the network.
[497.10 → 499.34] I am shocked that Butters caused you issues.
[499.52 → 500.94] Absolutely flawed.
[501.30 → 503.08] I still had a lot of fun doing it.
[503.20 → 504.12] So there's that.
[504.32 → 505.20] Oh, that's what matters.
[505.32 → 505.44] Yeah.
[505.56 → 507.40] So I was just like, I'm leaving on a trip.
[507.44 → 508.24] I got to install something.
[508.34 → 510.60] So I'll try Borg combined with Word.
[510.60 → 518.44] And that actually has been really nice for me in the last, I don't know, it's been like six or eight months since I've had that going.
[519.10 → 525.44] And I've tried it from many different terrestrial locations, and it's worked very well for me.
[525.92 → 535.78] The issue I had recently is that the backup system that we're building in the last one of the last self-hosted episodes, I had it burning disks, which was lovely.
[535.78 → 540.20] And, you know, that takes many days because those hard drives I got were 20 terabyte hard drives.
[540.60 → 541.98] And I planned it, Alex.
[542.06 → 543.22] I was so excited about this.
[543.28 → 544.58] I was ready to make you proud.
[545.24 → 547.90] They were going to be done burning as I, you know, went to Europe.
[548.28 → 549.74] Like two days later, they're going to be done.
[549.82 → 550.94] So I was like, oh, I'm going to travel.
[551.04 → 554.86] Then I could like late at night when I can't sleep, I could play with this new backup server.
[555.18 → 557.04] And, but I screwed it up.
[557.08 → 560.44] I didn't set up the keys properly, and I couldn't, I couldn't SSH to that.
[560.74 → 561.96] My hope was.
[562.10 → 563.84] Please just get tail scale already.
[563.84 → 564.72] It's on there.
[564.84 → 566.46] And I just like, I don't know.
[567.22 → 567.36] What?
[567.76 → 568.12] Yeah.
[568.94 → 571.76] I can ping it, but I can't actually SSH in.
[571.90 → 573.86] Tail scale set dash SSH.
[573.96 → 574.10] Yeah.
[574.10 → 574.42] I suspect.
[574.42 → 574.94] I'm learning.
[575.22 → 575.72] I'm learning.
[576.40 → 581.16] But because my hope was like to continue doing these, these Borg and Aorta backups.
[581.22 → 584.46] And I even like set them up locally so that they're in the right place.
[584.56 → 584.70] Okay.
[584.84 → 586.90] And so I screwed that up.
[586.98 → 588.50] So test before you leave.
[588.50 → 591.98] Talk me through a little bit, the architecture of what Borg is doing, because obviously you
[591.98 → 594.18] need an endpoint for the backups to land on.
[594.50 → 594.60] Yeah.
[594.66 → 597.44] Borg is really existing on the server.
[597.62 → 600.26] So it's kind of a server agent setup.
[600.50 → 602.00] So you need it in both places.
[602.00 → 602.30] Right.
[602.42 → 605.50] And I mean, I think I'm using it in the most simple of ways.
[605.50 → 609.02] So I create a Borg repo on the destination.
[609.54 → 610.12] Which is what?
[610.32 → 611.54] Ah, that's your question.
[611.96 → 613.60] It has been a few different things.
[613.60 → 618.78] Because previous to this new build, it was that X220 laptop that I was running.
[619.06 → 621.78] Just to get it on some other machine, just to physically separate it.
[621.80 → 622.78] Just to physically separate it.
[622.84 → 628.14] The finest manifestation of a server is just another computer right there.
[628.66 → 631.28] Somebody else's computer or maybe one of my computers.
[631.30 → 632.98] One of my old main computers.
[634.12 → 635.48] I love talking to you, Brent.
[635.58 → 636.22] I really do.
[636.36 → 638.70] Well, fortunately or unfortunately, I'm not too sure.
[638.70 → 642.52] Just around the time that you gave me that one litter PC, which is about the time I was
[642.52 → 648.70] building this new backup system, that X220 would just like randomly shut off.
[649.02 → 650.36] You know, like a hard shut-off.
[650.70 → 652.90] And that thing's been running for years and years now.
[653.44 → 656.34] It turns out that the fan in it stopped working.
[656.52 → 659.44] You have these problems, Chris, with your stove.
[659.68 → 661.18] One of your stoves, the fan problem.
[661.30 → 662.32] So I need to replace the fan on it.
[662.32 → 662.94] Could be cat hair.
[664.04 → 666.94] You know, because really, my fan, you know what?
[667.02 → 667.96] It's the funniest thing, right?
[667.96 → 668.62] It's sensors.
[669.18 → 672.62] The sensors detect the fan drops below a certain RPM threshold.
[672.76 → 675.56] So like the thermal management system kicks in and shuts the system down.
[676.00 → 677.24] That's what my toaster was doing.
[677.32 → 678.12] That's exactly what's happening.
[678.24 → 678.38] Yeah.
[678.58 → 682.48] And I thought that's what was happening the first few times it happened.
[682.58 → 684.90] But, you know, when you don't really have the time to look into it.
[685.20 → 686.44] Sure enough, that's exactly what's happening.
[686.54 → 689.74] So that, I mean, that fan's been running for way too long.
[689.78 → 691.18] So I probably just need to replace it.
[691.18 → 693.48] And this was one of the backup destinations?
[694.12 → 695.68] It was the primary backup destination.
[695.80 → 696.54] Oh, the primary.
[697.02 → 697.30] Yeah.
[697.30 → 698.64] And it's randomly turning off.
[699.06 → 699.62] Not good.
[699.70 → 700.32] Not good for drives.
[700.40 → 700.54] Yeah.
[700.60 → 701.22] Not good for backups.
[701.22 → 701.76] Not good for file systems.
[701.86 → 702.50] Not good for backups.
[702.54 → 702.70] No.
[702.70 → 706.70] So it's about fine time I move on to something a little bit more robust, I think.
[706.78 → 706.92] Yeah.
[707.30 → 708.38] I do like Borg, though.
[708.46 → 712.72] I think you've, you know, even if you go to like a totally different solution for where
[712.72 → 716.12] the data gets stored, you spent the time well learning Borg.
[716.12 → 722.08] I really hesitated, actually, because I wanted to do it more at the file system level, just
[722.08 → 724.32] for deduplication purposes.
[724.92 → 728.02] Like, file systems can do that these days, even across machines.
[728.46 → 730.22] So I had...
[730.22 → 732.60] I've never known anybody that's had the problems you've had with Butteriest.
[732.80 → 733.82] And like, literally nobody.
[733.82 → 734.60] I know it's me.
[734.60 → 735.82] I know it's me.
[735.94 → 736.34] It's fine.
[736.42 → 737.06] You don't have to...
[737.06 → 737.28] All right.
[738.00 → 739.92] That's why I'm like, oh, I'm just having fun with it.
[740.34 → 742.00] Everybody else will have more success.
[742.14 → 742.28] Okay.
[743.48 → 745.38] Or teach me, wise one.
[745.92 → 750.26] I did hesitate, though, because I thought, yeah, I want to use, I don't know, more native
[750.26 → 751.06] technologies.
[751.06 → 757.58] Like, Borg is battle-tested, but it comes from a bit of an older time when, you know,
[757.64 → 762.06] deduplication doing it within Borg itself made a lot of sense back then.
[762.60 → 768.90] But I got to say, like, since I dove into it, I'm seeing Borg implemented in tons of places.
[769.02 → 769.50] It's everywhere.
[769.70 → 770.52] The default backup.
[770.76 → 771.30] So I'm feeling...
[771.30 → 774.22] Resistance is useless or futile or something, I don't know.
[774.74 → 776.00] So maybe I made the right choice.
[776.06 → 776.42] I'm not sure.
[776.56 → 777.06] I think so.
[777.26 → 779.18] I think it's a good skill set to develop.
[779.68 → 780.60] What about you, Alex?
[780.60 → 782.70] What is your situation with that?
[782.70 → 784.82] Oh, it's not been a good year for Alex's backups.
[784.96 → 785.60] I'll tell you what.
[785.78 → 786.50] It's been...
[786.50 → 786.66] Uh-oh.
[786.90 → 790.50] I made a video about my backups being a complete disaster.
[791.18 → 795.00] So the Synology box, I should have a perfect system, right?
[795.02 → 796.94] Because I've talked about this on the show numerous times.
[797.20 → 801.74] I have my old UK server, which is in my mother-in-law's house.
[802.26 → 804.10] It has fibre internet in front of it.
[804.24 → 806.72] So it's got 500 down and 70 up or something.
[806.82 → 808.58] It's the perfect backup server.
[808.58 → 813.96] However, it's, you know, it's in another country and the hard drives slowly but surely got to
[813.96 → 815.66] six, seven, eight-year-old hard drives.
[816.22 → 820.26] They started failing, which then meant the ZFS array errored out and failed completely.
[820.52 → 826.00] So I had Gary from Joe Kensington's network, who lives only five minutes down the road from
[826.00 → 827.18] my mother-in-law, funnily enough.
[827.18 → 833.56] I had my sister take four 14 terabyte hard drives with her back from here when she visited
[833.56 → 839.94] us for Halloween, then mail them in England across the country in a parcel to my mother-in-law's
[839.94 → 840.28] house.
[840.46 → 841.80] I'm feeling better about my situation.
[841.82 → 842.02] I know.
[842.08 → 844.92] This is a network of volunteers that are making this possible.
[844.92 → 845.28] Yeah.
[845.62 → 850.10] And then, and then Gary went to my mother-in-law's house and actually swapped the drives out
[850.10 → 850.40] for me.
[850.44 → 850.92] So thank you.
[850.98 → 852.56] If you're listening, Gary, thank you so much for that.
[853.10 → 854.84] The guy was a true professional, by the way.
[854.96 → 856.82] He, I asked him, what do you want for payment?
[856.88 → 857.78] And he said, beer.
[857.78 → 857.86] Yeah.
[858.98 → 862.92] I mean, he was, he got a he, that was the final mile.
[863.14 → 865.30] Well, I guess it's the final kilometre over there.
[865.48 → 865.68] Yeah.
[865.88 → 866.96] Well, no, we use miles.
[867.46 → 867.88] I know.
[867.96 → 868.20] The UK.
[868.32 → 869.16] It makes no sense.
[869.24 → 870.22] I don't understand it at all.
[870.24 → 871.66] England makes little sense.
[871.86 → 874.26] But then we do have bigger pints than the US does.
[874.68 → 876.78] So, you know, we do have some things straight.
[877.18 → 878.00] That is an improvement.
[879.66 → 883.88] So, you know, the lesson I learned there is that really having a remote backup server that
[883.88 → 889.40] you completely self-host that's not in a Colo or some kind of data centre that relies on
[889.40 → 893.92] other people's just kindness maybe isn't the best long-term strategy, but I've doubled
[893.92 → 898.80] down and gone with it again anyway, because I preceded those four 14 terabyte drives with
[898.80 → 904.34] data in my house before I sent them across the ocean on a like a ZFS encrypted data set,
[904.48 → 904.84] of course.
[905.20 → 910.14] And then I just did a ZFS import on that server in the UK and the they just came straight up.
[910.18 → 911.42] It was actually kind of amazing.
[912.00 → 912.36] Beautiful.
[912.36 → 919.26] And then I just changed the ZFS send endpoint with Synod from the SSH host in my house
[919.26 → 922.72] that I did the replication over to the SSH endpoint over tail scale.
[923.30 → 927.54] And it was as if, apart from the speed was a lot slower, nothing changed.
[927.56 → 930.62] And it picked up the incremental backups, and it was actually kind of amazing.
[931.82 → 934.84] So that one actually is in a decent state again now.
[935.18 → 936.18] It's still syncing.
[936.40 → 937.96] There was about one point.
[938.12 → 939.26] Now I'm a video guy.
[940.28 → 941.64] Oh God, it's a nightmare.
[941.64 → 943.60] With 30 Meg upload, I tell you.
[944.22 → 948.58] But the other one was a Synology at my mum's house, which kind of completely
[948.58 → 951.20] the bed this year for numerous reasons.
[951.80 → 958.66] First, I was using Autoerotic with Mini as my S3 target backend running in a container.
[959.18 → 963.12] And to do that, I was doing Mac VLAN to doing some custom stuff on the Synology side,
[963.12 → 967.48] rather than just doing sort of traditional Synology GUI based container stuff.
[967.48 → 974.66] So first, Mini changed their schema for how they store data and didn't really give people a good migration path,
[974.70 → 979.72] other than spin up another Mini alongside it and just re-replicate the data.
[979.76 → 985.26] And I'm like, I'm sorry, I don't have a spare 10 terabytes just knocking about on the same system.
[985.26 → 993.48] So I ended up having to, after a balked DSM update, ended up having to completely wipe that box, like completely.
[993.70 → 996.52] I tried the paperclip trick in the back of it that one listener wrote in.
[997.34 → 997.54] Yeah.
[997.66 → 1002.30] So that box is actually completely empty right now, which is kind of alarming.
[1002.30 → 1012.44] And so frustrating because it kind of feels like it touches on this topic that we've been orbiting around recently about these devices that have this abstracted away management UI.
[1012.90 → 1022.04] And when it breaks and goes sideways, you're left troubleshooting and managing that environment and not the actual problem.
[1022.04 → 1028.98] Which I know it is not a good description, again, of why I didn't go with Proxmox, but why I didn't go with Proxmox.
[1029.14 → 1033.66] And why I didn't go with True and why I probably won't go with Open Sense.
[1033.84 → 1035.34] Yeah, Open Sense I agree with.
[1036.62 → 1040.94] I actually kind of, I mean, I like Open Sense as a project, but I actually kind of hate it too.
[1041.02 → 1046.12] Because it's, I always go on about how much I dislike GUIs and click point and squirt.
[1046.12 → 1046.34] I get it though.
[1046.56 → 1047.38] I get it though.
[1047.40 → 1051.16] I also really think it's a great project and totally understand why people would want to use it.
[1051.16 → 1052.28] Absolutely.
[1053.32 → 1059.26] So if this was a Facebook status, my relationship status with backups right now would be it's complicated.
[1059.96 → 1060.56] Yeah, okay.
[1060.84 → 1061.32] Nice.
[1062.18 → 1066.16] I'm not proud for some reason about my backup solution.
[1066.94 → 1069.74] But it's working, and it's solid.
[1070.02 → 1071.88] So that's what you need, right?
[1072.06 → 1073.02] How do you know it's solid?
[1073.26 → 1074.58] Well, I check on it.
[1074.64 → 1077.80] I don't do a lot of restores, but I do check on it.
[1077.80 → 1083.42] And what I'm honestly most impressed by is that it's keeping up with my photos, right?
[1083.46 → 1086.74] Because now that I'm using image, I need to back up my photos.
[1086.90 → 1089.46] And I'm doing all of this on Starlink with my Droid.
[1090.08 → 1093.34] So my Droid is responsible for all of this now.
[1093.34 → 1110.10] And I was a little worried that between backing up my application data, backing up the data in my Nextcloud, backing up my configs, backing up my pictures, I was just a little worried that Starlink wouldn't be able to get that all up before it was time for me to get up and start using the internet.
[1110.24 → 1111.14] But so far it has.
[1111.14 → 1113.34] And I've been using duplicate.
[1113.86 → 1116.70] I'm still using duplicate, and it's been working really well for me.
[1116.74 → 1118.76] And I'm not super proud of it, but it has been.
[1119.02 → 1126.54] And I've been using storage, S-T-O-R-J, for my photos because it's ridiculously cheap.
[1127.06 → 1131.04] I don't recommend it because it just feels like it's going to go away because cheap storage always does.
[1131.14 → 1133.38] But I've been using it for a year so far.
[1133.38 → 1141.34] And then my application configs, my Docker composes, you know, like your configuration files, home directory type stuff.
[1141.42 → 1144.58] That's been going up on Google Drive now for a couple of years.
[1144.98 → 1149.30] I do an AES-256 local encryption first before it goes up.
[1149.44 → 1151.22] And then it does a 50 Meg chunk.
[1151.70 → 1154.20] It 50 Meg chunks everything and sends it up on Google Drive.
[1155.14 → 1158.70] And it gets it up before I'm awake in the morning over Starlink.
[1158.82 → 1161.64] And it even worked back in the day when I was on LTE.
[1161.64 → 1165.38] So I'm still going the duplicate route.
[1165.52 → 1170.12] I would really like to solicit feedback from the audience if you've had good or bad.
[1170.24 → 1172.10] And I don't want just the horror stories.
[1172.60 → 1176.66] But I would like to get everybody's story on recovery because I keep hearing different stuff.
[1177.34 → 1178.96] Thumbs down for my behaviour, I'm afraid.
[1179.28 → 1179.48] Really?
[1179.66 → 1181.22] I had a bad experience with recovery.
[1181.56 → 1181.76] Yeah.
[1182.40 → 1183.06] Oh, God.
[1183.44 → 1187.70] You mentioned that you were kind of embarrassed for running a duplicate.
[1187.82 → 1189.04] Where does that feel come from?
[1189.04 → 1192.02] Well, because I've gotten stories like Alex.
[1193.50 → 1200.46] I've heard that I go to recover, and I couldn't recover, or I had to go through all of these hoops to even get to the data in the first place.
[1200.52 → 1201.42] And it was a ton of work.
[1201.88 → 1206.24] From my perspective, I would say that's pretty much what you hear of any backup system.
[1206.38 → 1210.94] Because when things go wrong, people are vocal about it, I guess.
[1211.06 → 1211.18] Yeah.
[1211.26 → 1211.70] That could be.
[1211.70 → 1215.38] That's what I'm, I mean, I don't know.
[1215.64 → 1220.12] Because you can't just like pull down the tar files, join them all together and extract them and get the data, right?
[1220.16 → 1221.78] It doesn't, I guess it doesn't work like that.
[1221.92 → 1228.78] That's part of my problem with all of these like, I don't know, more elegant backup systems, I'll call them.
[1228.82 → 1231.76] Or like they feel like database style backup systems.
[1231.90 → 1233.00] The file-based ones, yeah.
[1233.00 → 1237.48] Yeah, where they're chunking things, like you get a ton of nice features doing that.
[1237.96 → 1247.12] But you also get this abstraction that you're talking about where if the backup system itself breaks for some reason, then you're in a bad place for sure.
[1247.28 → 1252.42] Which is where the 2 in 3.2.1 probably comes in handy, two different types of media, huh?
[1252.42 → 1262.40] Honestly, if I had the means, this is sounds silly, but I can't get past the idea that the best solution would be identical tape drives.
[1262.68 → 1264.60] One here and one in the RV.
[1265.36 → 1271.72] And every morning when I come to the studio, I just swap tapes at different locations.
[1271.84 → 1274.88] It's like the president can't fly on the same plane as the vice president, though.
[1274.92 → 1276.80] You can't carry them both in the car at the same time.
[1276.80 → 1277.58] Yeah, that's true.
[1277.58 → 1287.98] But every time I go through this and I look at the amount of storage I really need to back up everything, we're talking 30 terabytes, I just keep coming back to tapes.
[1288.68 → 1294.74] I'm not going to spend the time to learn what tape drive is the right tape technology and then try to find some used tape drive.
[1295.74 → 1297.10] And then where do you put it in?
[1297.56 → 1298.72] Yeah, and how does it connect?
[1298.98 → 1302.60] This is coming from a guy with a dot matrix printer in his garage, ladies and gentlemen.
[1303.10 → 1304.22] Dot matrix is awesome.
[1305.84 → 1307.32] All right, document management.
[1308.20 → 1308.52] Nextcloud.
[1309.08 → 1309.78] Yeah, Nextcloud.
[1310.10 → 1311.18] Paperless NGX.
[1311.72 → 1312.58] Ah, yes.
[1312.58 → 1313.82] You've been on that for a while now.
[1313.82 → 1315.14] I do have to give that a go.
[1315.34 → 1317.78] That's my miss of the year, I think, is paperless engine.
[1317.88 → 1318.94] I'm going to write that down right now.
[1319.00 → 1319.70] Wait a second.
[1320.54 → 1325.68] I asked you about this about a month ago, and you said you had a hard time with it, and you weren't recommending it anymore.
[1325.80 → 1331.40] Oh, see, I've been doing just really quick recap when I say Nextcloud is I've got a scan bot on my phone.
[1331.62 → 1334.16] I scanned a PDF and I send a Nextcloud.
[1334.74 → 1335.58] That's my system.
[1335.58 → 1339.06] I still use Nextcloud for long-term cold storage.
[1339.66 → 1343.08] But NGX is for things like, so I have different categories, I guess.
[1343.24 → 1343.62] It's a comp.
[1343.86 → 1348.56] I'm trying to make this fast because I'm aware this is going to be like a four-hour-long episode if we don't.
[1348.82 → 1349.86] But I got to sleep soon.
[1349.86 → 1357.00] So the short version is paperless NGX is for bills and things that come through the door, typically in the mail, that I just want to quickly scan.
[1357.42 → 1369.22] And then I use Nextcloud as long-term cold storage that I actually want to curate and care about, like scans of passports and titles for vehicles and all that kind of stuff.
[1369.22 → 1370.26] All right.
[1370.34 → 1371.56] I will give that a go this year.
[1371.66 → 1372.40] I'm going to try that.
[1372.74 → 1372.96] All right.
[1372.96 → 1374.10] Let's keep moving quick, though.
[1375.00 → 1375.40] Contacts.
[1375.74 → 1376.04] Calendar.
[1376.40 → 1376.68] Alex.
[1377.04 → 1379.02] Can I just not answer this one?
[1379.14 → 1380.54] Because I use Google for everything.
[1382.16 → 1383.32] I'm embarrassed now.
[1383.34 → 1383.98] Oh, my gosh.
[1384.08 → 1384.42] Drama.
[1384.82 → 1385.22] Drama.
[1385.22 → 1387.58] Brent, Nextcloud.
[1387.92 → 1388.18] Yeah.
[1388.28 → 1390.16] I mean, for six years now.
[1390.24 → 1390.38] Yeah.
[1390.46 → 1392.02] Since last November.
[1392.30 → 1393.96] So I have passed a year.
[1394.10 → 1396.08] So I'm about 13 months as Nextcloud.
[1396.18 → 1397.24] And DAVE, of course.
[1397.32 → 1397.48] Yeah.
[1397.58 → 1398.60] They pair so well.
[1399.08 → 1399.38] All right.
[1399.42 → 1400.56] Now, I don't have an answer for this.
[1401.46 → 1402.84] I don't do this part.
[1403.32 → 1403.92] But invoicing.
[1404.38 → 1405.10] Invoice Ninja.
[1405.36 → 1406.58] It is fabulous.
[1407.70 → 1408.10] Fantastic.
[1408.46 → 1409.86] I'm a bit embarrassed about this one.
[1410.44 → 1414.04] Alex has tried to move me to Invoice Ninja three times now.
[1414.04 → 1419.56] He even sent me a database of an instance he set up at his place for me to use for a while.
[1419.72 → 1426.66] But I'm using something called Invoice Plane, which no one's heard of because, well, it's a just enough solution.
[1426.86 → 1428.38] It's not Ninja enough, is it not?
[1429.84 → 1432.14] Everybody keeps using the Ninja in the name.
[1432.40 → 1433.04] Yeah, because it's good.
[1433.04 → 1433.76] Everybody can use it.
[1434.38 → 1434.86] Yeah.
[1435.28 → 1437.16] But I've used this thing for 10 years.
[1437.36 → 1440.06] Like, it's changed iterations and names and stuff.
[1440.06 → 1440.08] Okay.
[1440.16 → 1440.34] All right.
[1440.34 → 1440.80] That's good.
[1440.80 → 1441.54] So it's got some longevity.
[1441.82 → 1442.06] Okay.
[1442.06 → 1443.20] Same database and everything.
[1443.20 → 1446.14] That's exactly what you want from an app like that.
[1446.70 → 1446.90] Okay.
[1447.38 → 1447.64] Yeah.
[1448.44 → 1449.40] Networking gear.
[1450.56 → 1451.94] Generic HP switches.
[1452.90 → 1455.64] They're old gigabit switches, but they get the verb done.
[1455.92 → 1457.76] And then we've been given a couple of quick switches.
[1458.16 → 1460.10] Quick switches, fibre switches.
[1460.44 → 1461.90] But they're not in production yet.
[1462.36 → 1462.60] Alex?
[1462.92 → 1472.54] Primary reason I added this one to the dock was because in the spring, I made the jump from completely unmanaged gigabit copper everywhere in the building.
[1472.54 → 1481.90] I ran fibre through the walls and switched to be basically a Unify fanboy in the spring this year.
[1482.24 → 1482.36] Yeah.
[1482.38 → 1483.16] And it does work good.
[1483.54 → 1484.00] I like it.
[1484.04 → 1485.28] I like the results you got.
[1485.28 → 1495.12] You say that, but the Peppa Pig incident that I referenced was because one of the POE switches in my basement locked up at 5 a.m. the other day.
[1495.18 → 1495.84] Oh, right.
[1495.84 → 1500.74] And so my favourite thing in the world is to wake up and then my network's just completely broken.
[1501.00 → 1502.88] Just get right into troubleshooting stuff not working.
[1503.08 → 1504.18] That's the best thing in the world.
[1504.24 → 1507.30] And when it's a switch issue, it's real obvious when it's a switch issue.
[1507.48 → 1507.70] Yeah.
[1507.86 → 1508.46] Super obvious.
[1508.46 → 1513.64] I stood in the basement in front of my comes rack, which you've probably all seen in a video now.
[1513.84 → 1519.02] And I'm like, okay, so I can't SSH to this box, but I can SSH to that one.
[1519.26 → 1523.36] And then the lights on the front of this switch are on, but hang on, they're not blinking.
[1523.52 → 1523.92] Why are they not?
[1524.20 → 1529.16] And it took me a good 20 minutes to figure out it was the switch because when is it ever the switch?
[1529.38 → 1530.46] Yeah, exactly.
[1530.80 → 1531.20] Exactly.
[1531.20 → 1536.42] On that kind of level, though, cameras, any changes there this year?
[1536.82 → 1540.80] Slowly, slowly, but surely weaning myself off of the Waze Cam sauce.
[1541.34 → 1541.54] Yeah.
[1541.66 → 1544.10] Going still Blue Iris, still going pretty strong.
[1544.28 → 1550.70] I flirted with the Fright a couple of times this year and then ended up sending the Coral device that I had to a buddy.
[1551.36 → 1553.04] So I'm still on the Blue Iris train.
[1553.18 → 1558.00] POE cams, I've replaced a couple of Waze cams just this week, actually, with some extra POE cams.
[1558.12 → 1559.80] And yeah, it works really well.
[1559.80 → 1566.52] I think 2024, I'm probably going to do something with my cameras, probably a pretty big change.
[1567.12 → 1577.34] What I do right now is I have Shinobi on a Pi that I fire up from time to time, and then I shut down when I want recordings.
[1577.62 → 1583.62] And I was weaning myself off the Waze cameras until they came out with the pan and tilt with auto tracking.
[1583.62 → 1591.24] So I have the pan and tilt on the dash, and I can auto track when people come up to the RV or deliver packages.
[1591.62 → 1593.38] And I've really liked that feature set.
[1593.48 → 1597.60] And of course, I'm still using the Docker Waze bridge, which has been pretty great.
[1598.10 → 1601.08] What about DNS and DHCP and all that kind of stuff, though?
[1601.12 → 1602.90] Have you made any changes there this year?
[1603.34 → 1604.86] Year three for Pinhole for me.
[1605.06 → 1606.16] Nothing too fancy there.
[1606.24 → 1608.82] Could see a Nix router in 2024, but not in a lock.
[1609.26 → 1610.10] Pinhole's just worked.
[1610.10 → 1611.06] Yeah, me too.
[1611.92 → 1618.62] Nix as a router seems like the most obvious perfect use case for Nix possible.
[1619.04 → 1620.72] So why have neither of us done it yet?
[1621.74 → 1622.12] Time?
[1622.88 → 1628.38] I agree because it's the perfect solution for everything that you want declared.
[1628.82 → 1635.24] And yeah, you want something that has nice cutting edge features you can update real quick and smooth and has pretty solid rollbacks.
[1635.78 → 1637.34] It does seem perfect, Alex.
[1637.34 → 1643.38] So it seems like a foregone conclusion that one of us will do it in 2024, but no plans currently.
[1643.92 → 1649.54] This year, I've sent Alex two different projects, Nix OS-based projects that do this, but he hasn't bitten yet.
[1649.80 → 1651.46] Oh, I have started.
[1652.24 → 1652.56] Ooh.
[1652.86 → 1655.64] In my lab, my home lab, I do have a VM somewhere.
[1655.80 → 1656.96] Oh, that's exciting.
[1657.16 → 1660.06] With packet forwarding and all that kind of stuff in mind.
[1660.06 → 1666.68] But it's really, I got distracted trying to flakily it, and that can be difficult.
[1667.60 → 1668.40] No, you don't say.
[1668.86 → 1670.68] I think I have the perfect hardware waiting upstairs.
[1670.92 → 1673.18] It's an ARM device, but it's got dual gigabit Nix.
[1673.90 → 1674.56] Ready to go.
[1674.62 → 1675.20] Oh, man.
[1675.42 → 1676.62] Yeah, that does sound pretty good.
[1676.62 → 1692.16] I got, actually, most of the way towards where I want to be with a declarative router anyway in the spring again when I did all that networking work by splitting out my DNS and DHCP into Spyhole on a separate system configured using Ansible.
[1692.16 → 1702.58] So when I add and remove hosts, I do the MAC address-based static IP reservations, and then everything else is just put into basically a Git repo, and then I never have to worry about it ever again.
[1702.66 → 1705.84] Whereas with Open Sense, I was clicking through a UI and Ada, Ada, Ada.
[1706.14 → 1707.04] You've heard the story.
[1707.44 → 1707.50] Yeah.
[1707.92 → 1708.96] That's the better way to go.
[1709.12 → 1709.30] All right.
[1709.36 → 1715.16] And then last but not least, while we're talking about networking, I don't think there's going to be any surprises here for VPNs.
[1716.68 → 1717.36] Tail scale.
[1717.36 → 1733.06] It really started in last November for me, but for the first couple of months of using Tail scale, I just used it like a VPN, and I didn't really think of it much beyond, hey, now I can get to my home stuff and my work stuff real easy, even though my home stuff's got double carrier grading that.
[1733.48 → 1734.44] Like, hey, this is great.
[1734.44 → 1751.98] And then it wasn't until probably about January that I started redoing the way I network and realizing that Tail scale was not just a VPN solution, but it was really now I had my own flat network that I could have services on that were available wherever I went on every device.
[1751.98 → 1762.16] And then I just started rethinking everything, and I eventually shut down all my inbound ports, a lot of my firewalls, and I kind of just live on my tail net now.
[1763.14 → 1769.68] This was a – I mean, 2023 was the year I really just was like, oh, oh, this is more than a VPN.
[1770.52 → 1771.56] This is a game changer.
[1771.84 → 1774.76] I have a question around that when it comes to stability.
[1774.92 → 1776.98] Have you seen any, like, downtime or anything?
[1777.10 → 1777.62] Not once.
[1777.84 → 1778.08] Really?
[1778.08 → 1778.78] Not once.
[1779.74 → 1780.14] Impressive.
[1780.14 → 1780.70] No.
[1781.04 → 1781.32] Okay.
[1781.32 → 1786.48] And, man, I have – I say this in the ad read, so sorry, but, like, it's true.
[1786.62 → 1795.34] Like, I have been on AT&T, and then three minutes later I'll move to Verizon, and then a minute later I'll move to Starlink, and then maybe, like, that's not working, so I'll try campground Wi-Fi.
[1795.90 → 1800.22] And I'm still staying connected to all my different Tail scale devices while I'm doing all that.
[1800.38 → 1802.52] It's just – I don't know.
[1802.74 → 1803.02] Magic.
[1803.92 → 1806.04] But, Alex, I imagine you're probably using something else.
[1808.26 → 1810.36] I liked it so much I got a job there.
[1810.36 → 1811.06] So, yeah.
[1811.06 → 1812.88] That probably tells you everything you need to know.
[1815.82 → 1817.92] Tailscale.com slash self-hosted.
[1817.98 → 1822.32] Head on over there to try it for free on 100 devices and three users.
[1822.46 → 1826.80] Yeah, I'm talking 100 devices and up to three users for as long as you want.
[1826.86 → 1828.22] It's not a limited time thing.
[1828.64 → 1830.96] And Tail scale is something that's really special.
[1831.12 → 1832.78] It's changed my networking game.
[1832.78 → 1845.28] You can think of it as programmable networking software that's private and secure by default, connecting your machines all over the world on one flat mesh network protected by WireGuard.
[1845.28 → 1850.48] It really is the easiest way I've ever come across to connect devices and services directly to each other.
[1850.54 → 1861.34] Even if you're, like, on an LTE connection or on some weird carrier-grade setup, or you have a really hostile ISP, it just does its best to connect machines directly to each other.
[1861.42 → 1864.04] And it's fast, like, really fast.
[1864.04 → 1865.80] And it's super simple and intuitive.
[1865.94 → 1867.76] You get started, like, okay, I get this.
[1868.36 → 1870.96] As you start to use it, you realize how powerful this is.
[1871.04 → 1873.56] I mean, it took me – I'm a little embarrassed to admit it.
[1873.60 → 1877.22] It took me about three months to really wrap my head around how it was going to change how I do networking.
[1877.72 → 1884.52] You can build simple networks across really complex infrastructure, so multiple data centres can be bridged on one flat LAN.
[1884.52 → 1894.78] ACL policies allow you to securely control and access devices and services so you can have controls for friends and family on permissioned network that you have control over.
[1895.04 → 1903.30] And if you're an enterprise, it will integrate right in with your authentication policies, your group infrastructure, your two-factor, all the stuff you need.
[1903.42 → 1906.78] And it saves you a ton of time and money on a VPN provider.
[1906.78 → 1913.40] And you can do kinds of crazy things like Tail scale Send where you get sort of, like, airdrop for all your machines.
[1913.48 → 1920.10] And you can send data between an Android device and a Mac, you know, like an iPad and a VPS.
[1921.02 → 1922.72] It's really, really cool.
[1923.24 → 1930.28] And Tail scale also integrates with things like VS Code so you can just connect to your Tail net directly from within VS Code.
[1930.52 → 1934.22] There are a lot of applications you can plug into directly onto your Tail net as well.
[1934.22 → 1936.76] It's pretty game-changing.
[1937.20 → 1941.66] It really has been a massive upgrade for my security, my networking, and I have it on everything now.
[1942.36 → 1948.26] So go try it out for free on 100 devices and up to three users for free at tailscale.com slash self-hosted.
[1948.62 → 1953.82] That lets them know you heard about it here, supports the show, and gets you up to 100 devices for free.
[1954.32 → 1956.92] tailscale.com slash self-hosted.
[1958.62 → 1963.28] Well, Plex made it pretty easy for us this year to have something to talk about in this next segment.
[1963.28 → 1965.38] media playback.
[1965.78 → 1967.70] What happened to your media stack this year?
[1967.70 → 1970.90] Well, you remember we started with the Jellyfin Challenge.
[1971.02 → 1971.50] Yes, we did.
[1971.92 → 1981.88] And I went through the work of moving everything to Jellyfin, and inevitably, like an idiot, gave up because I wanted decent intro skipping.
[1982.02 → 1983.90] But I was watching Star Trek Enterprise.
[1984.44 → 1985.50] Star Trek fans, you understand.
[1985.50 → 1987.74] And now I'm back on Jellyfin.
[1988.20 → 1989.50] So that's my problem.
[1990.62 → 1999.28] Although, one problem I have is during that time, more friends and family have started using my Plex server on the regular.
[1999.78 → 2000.58] Yeah, that's okay, though.
[2000.58 → 2004.32] So I'm actually going through this with a couple of people that you know, Brent.
[2004.92 → 2008.98] We want to share all of what was shared through my Plex server before.
[2009.44 → 2014.96] I'm going to share that now using Tail scale to let them come in through a shared node in my network.
[2014.96 → 2018.00] But then I have the public DNS record in Cloudflare.
[2018.20 → 2024.52] So if I share that node with them, Cloudflare tunnelling doesn't let you share video over the Cloudflare tunnel.
[2025.06 → 2029.32] Tail scale's Dirt nodes, if you haven't got a direct connection, the performance won't be good enough.
[2029.32 → 2043.46] But because Tail scale sharing lets you do a direct connection from their phone or their laptop or whatever into my shared node, I can then share my Jellyfin without opening any ports in my firewall, which, if you remember, in January was one of my huge sticking points.
[2044.08 → 2050.20] But just as Tail scale's matured and added features and stuff like that, it's let me solve that particular problem, which is really nice.
[2050.42 → 2057.60] Your ask for friends and family will be got on my Tail net or get on Tail scale, and then I'll share this with you and this will show up on your Tail net.
[2057.60 → 2063.92] Correct. I will share my media server node into their Tail net, and they will just see it as another device.
[2064.72 → 2073.14] So then, like, practically speaking, we're all going to, like, say we all have Jellyfin installed on our Android TV boxes or our iOS box.
[2073.52 → 2075.78] We're all going to add each other's Jellyfin servers?
[2076.36 → 2076.82] Yeah, you could do.
[2077.04 → 2082.76] Yeah. I would. Yeah, I would. You guys got good stuff. But it's so much nicer in Plex.
[2083.00 → 2085.48] Well, it is. But you sell your soul to the devil.
[2085.48 → 2087.30] And as we've seen, you know, it's...
[2087.30 → 2094.94] Well, and Alex, the problem is just having the server online with content on it is now the vulnerability.
[2095.30 → 2095.48] Yeah.
[2095.64 → 2102.66] So even just, yeah, that's the problem is having a Plex server that's connected to a Plex account that is indexing what's on there.
[2102.88 → 2107.34] To that end, I removed all video content from my Plex this week. It's gone.
[2107.58 → 2110.80] Like, I've actually pulled the cord. It's done.
[2111.28 → 2112.26] So just audiobooks?
[2112.50 → 2114.28] Just audiobooks and music. Yeah.
[2114.28 → 2116.34] Uh-huh. Yeah. Okay.
[2116.68 → 2123.64] Wife loves, if you want to listen to The Reasons Why, episode 89, my wife loves Prologue. And that speaks Plex.
[2124.28 → 2133.08] If the developer for Prologue is listening, it's a long shot, but if you were to add support for Jellyfin, that would make me a very happy husband indeed.
[2133.64 → 2136.04] I think I'd make a contribution or whatever. Like, yes.
[2136.14 → 2136.46] Yeah.
[2136.60 → 2137.74] A couple of users over here for sure.
[2137.98 → 2138.16] Yeah.
[2138.16 → 2145.06] Can I ask you, though, are you still using the NVIDIA Shield? I think as long as I've known you, maybe, you've been an NVIDIA Shield user.
[2145.30 → 2152.14] Yeah. We even did a dedicated episode on how we both ended up at the NVIDIA. I mean, you've diverged a little bit with the Apple TV.
[2152.14 → 2153.92] I still have one in production.
[2154.06 → 2172.96] But my original Shield, which I purchased in December 2015, eight years ago, is still in production. I still use it every single day. It still gets updates. And it just works every time. I cannot believe it still works, but I love it so much.
[2172.96 → 2178.06] You don't ever have the problem where it's just off, and you have to unplug it and plug it back in?
[2178.16 → 2182.40] I think that's happened three or four times in eight years. I can kind of cope with that.
[2182.50 → 2186.84] Okay. Okay. I have that every six months or so. It's not great.
[2187.06 → 2195.10] Well, the one thing that I did feel obliged to actually dig into and tinker with this year, in particular with the NVIDIA Shield, was the launcher situation.
[2195.32 → 2195.98] Yes. Yes.
[2196.00 → 2199.48] You remember they brought their Google TV ad-infested crap?
[2199.48 → 2202.78] Remember, I see it every time I turn my TV on in my bedroom. Yes.
[2203.26 → 2203.38] Yeah.
[2203.66 → 2217.82] Well, there is an app called Productivity Launcher. There'll be a link in the show notes, which allows you to completely remove all the ads and set it as your default launcher because it's Android. You can do whatever you like.
[2218.06 → 2221.58] That's wonderful. That's nice. Okay. Thank you.
[2221.58 → 2226.22] So I haven't seen a single ad in my NVIDIA Shield now for six months, and it's been glorious.
[2226.22 → 2237.92] I will say I do feel slightly vindicated in my choice to switch out to Apple TV in several locations. The Apple TV remains an extremely well-performing device.
[2238.68 → 2248.98] Apple TV OS has seen some fantastic updates, and in Apple TV OS 17, tail scale arrived, and now I have my Apple TV on my tail net.
[2248.98 → 2267.00] And Infuse, which has nothing to do with Apple but is an Apple TV app, has gone from strength to strength. I mean, just absolute fantastic Dolby Digital support for surround sound, playback that is just absolutely pristine, fast, excellent, local, beautiful.
[2267.00 → 2277.36] So I really like the Apple TV, and as much as I hate to give Apple that money, I still think it is, compared to the NVIDIA TV, a better box.
[2277.52 → 2286.64] You don't have to worry about launcher bull crap, and if you do subscribe to all the Apple crap, like I do because I got kids, then you get the arcade.
[2286.64 → 2292.76] And then there are a bunch of those games, like a bunch of those games that you can play on the Apple TV, like it's a console.
[2293.28 → 2296.06] And many of them are family-friendly.
[2296.48 → 2299.64] And so we have a controller now paired to the Apple TV.
[2300.44 → 2306.70] And, in fact, one of Brent's favourite games was discovered via the Apple TV.
[2306.94 → 2307.20] It's true.
[2307.52 → 2309.62] It still remains one of my favourites.
[2309.96 → 2314.76] Yeah. He messaged me the other night, like, hey, what's that game I was playing on the Apple TV at your house?
[2314.76 → 2315.54] Tell someone about it.
[2316.88 → 2322.18] You know, I just think it's a really nice, very competitive device, except for on press.
[2322.18 → 2324.78] What is the game? Are you going to keep me waiting? What's the game?
[2324.78 → 2326.36] Oh, Alto's Odyssey.
[2326.56 → 2332.34] And the beautiful thing about Alto's Odyssey, if you think you get the second one with the purple icon, you can put it in Zen mode.
[2332.68 → 2336.96] And so the crashes don't matter, and you can just keep on skating.
[2338.04 → 2338.20] Yeah.
[2338.60 → 2339.04] Okay.
[2339.42 → 2342.82] They do have a decent version for Android.
[2343.48 → 2344.46] So what about you, Brent?
[2344.46 → 2346.26] Brent, what's your media situation?
[2347.12 → 2349.12] Include your brother's laptop in that question.
[2349.60 → 2354.96] For me, personally, I think most of the media that I'm consuming is actually coming from each of you.
[2356.32 → 2360.90] So this whole, you know, Plex shake-up thing, I guess I'll have to learn a new skill or two.
[2361.74 → 2362.90] Brent's going to get tail scale.
[2365.96 → 2366.70] Which is fine.
[2366.78 → 2367.68] Like, all the pieces are there.
[2367.90 → 2368.30] Yeah, yeah.
[2368.30 → 2373.78] And, you know, we've used Jellyfin enough over the years that that's totally, actually, I think it's great.
[2373.96 → 2374.20] Yeah.
[2374.34 → 2376.16] Yeah, you've set up Jellyfin.
[2376.30 → 2377.90] We did a segment or two on it.
[2378.06 → 2379.14] Like, you've been there.
[2379.34 → 2381.72] For video, it is absolutely where it needs to be.
[2381.72 → 2384.80] I still end up using Plex Amp for music, though.
[2384.98 → 2386.48] But we talked about that last episode.
[2386.48 → 2387.28] Plex Amp is so good.
[2387.62 → 2388.02] So, yeah.
[2388.38 → 2392.50] So I do have a Jellyfin instance or two floating around my network.
[2392.70 → 2397.72] One of them is installed on this dear laptop that you love, Alex, that's at my brother's place.
[2398.16 → 2402.30] It's like an X440 old ThinkPad that's just been rock solid.
[2402.92 → 2404.74] So that holds a little bit of, like, local media.
[2404.86 → 2410.30] But really, I haven't done the ripping of all the DVDs.
[2410.32 → 2411.06] You know, that project?
[2411.08 → 2411.36] Oh, yeah.
[2411.36 → 2412.80] That just takes forever.
[2412.80 → 2417.34] You've got to just get a machine set up somewhere where you hang out and just let it go.
[2417.56 → 2419.72] And just, you know, as you're doing other stuff, you just want to...
[2419.72 → 2420.42] Yeah, that's logical.
[2420.42 → 2425.02] And as you do it, you've got to give it a name, like the Originator 5000 or something.
[2425.62 → 2426.68] Yeah, that's fun.
[2426.86 → 2427.12] Yeah.
[2427.72 → 2428.36] Jack the Ripper.
[2428.50 → 2429.08] There you go.
[2429.20 → 2429.86] That's a good one.
[2429.96 → 2430.62] Yeah, we have a winner.
[2432.24 → 2437.12] Yeah, so from that, I think laziness means that I'm just kind of...
[2437.12 → 2438.80] And improved internet this year for me.
[2439.08 → 2439.78] Yeah, it's a big one.
[2439.88 → 2440.60] Thanks to Starlink.
[2440.90 → 2444.24] I'm really just leaning heavily on streaming stuff from each of you.
[2444.70 → 2455.00] I think you're underplaying, Alex, the effort in switching to Jellyfin because, like, I'm thinking of, you know, like Angela's house with the kids.
[2455.00 → 2465.88] Like, the only way I'm going to get them to switch to Jellyfin is if I get in my vehicle and I drive over to her house and I reconfigure her ROK or whatever she's using to, like, have Jellyfin.
[2465.88 → 2467.58] And then, like, you know, like, this is...
[2467.58 → 2473.58] And, like, Mom, like, this, it's going to require I go to people's house and I do tech.
[2473.58 → 2479.88] Like, I've weaned a lot of my family off this stuff over the last few years because I love my family.
[2480.08 → 2482.46] But the texts of, why is this down?
[2482.54 → 2483.18] Why is that down?
[2483.32 → 2486.70] Like, at 3 a.m., they just, yeah, I don't need that.
[2486.94 → 2489.52] And I'm sorry, but it's a service running in my basement.
[2489.64 → 2490.88] It doesn't have five nines.
[2491.04 → 2492.50] It's just, if it's up, it's up.
[2492.56 → 2494.56] If it's not, sorry, you know.
[2495.26 → 2503.08] So I appreciate it might be different for you with kids because kids are just used to, I mean, like I told you, Ella with Peppa Pig the other morning.
[2503.24 → 2504.08] Learn from my mistake, though.
[2504.24 → 2507.14] Get them locked into the right stuff at the right time.
[2507.48 → 2507.74] Yeah.
[2508.28 → 2508.86] Like notes.
[2509.20 → 2510.58] I know for you, you're going to say Obsidian.
[2510.78 → 2511.12] I am.
[2511.20 → 2511.72] Do I even need to ask?
[2511.80 → 2511.94] Yeah.
[2512.02 → 2514.68] This year has been huge for me because of Obsidian.
[2514.68 → 2519.74] I actually, just this afternoon, I got a new guitar cabinet for some speakers.
[2520.30 → 2520.90] And I was like, what?
[2520.90 → 2528.42] Because I put a bunch of effort into my old guitar cabinet of looking at like Celestial Vintage 30s and that kind of stuff and some greenbacks and made in England.
[2528.70 → 2536.70] I put hours of research into this and I just went into my Obsidian Vault, Command Shift F, typed in Celestial and boom.
[2536.90 → 2550.48] All of my notes from the summer were there, including wiring diagrams, including how to look up date codes of specific speakers because different years sound different compared to where they were made, and the materials used of the speaker cones and that kind of stuff.
[2550.90 → 2553.62] And all of it was just in Obsidian waiting for me.
[2554.22 → 2558.02] The same was true of when I was doing my break job before the track day a couple of weeks ago.
[2558.12 → 2560.98] All the Golf R, you know, torque specs and stuff like that.
[2560.98 → 2573.16] Like, yes, I could go and look through the manual every time, or I could write myself a one-pager that this nut has this part code with this torque spec and I need this thin line 17 millimetre spanner to get on that nut just there.
[2573.98 → 2581.38] You know, for me, it's just settling on a single source of truth, which is Obsidian for me, has just been liberating.
[2581.82 → 2582.88] The app could be better.
[2582.88 → 2590.66] I feel like it's not quite as smooth and as performant and particularly on mobile, it could be just nicer to use.
[2590.96 → 2601.68] But the fact that it exists in the same form across all the different platforms I use, iOS, Android, macOS, Windows, Linux, I can use it on all of them.
[2602.44 → 2604.44] It's just been the holy grail for me.
[2604.54 → 2606.42] It has solved the note problem.
[2606.70 → 2609.82] I'm curious, Alex, you've been using it almost for a year now, I think, right?
[2609.82 → 2614.06] How many times have I sent you notes and said, Brent, you've got to switch to Obsidian, dude.
[2614.52 → 2615.22] You don't send me notes.
[2615.28 → 2617.62] You just send me screenshots of beautiful features.
[2618.02 → 2622.40] You've convinced me, but we shall see what the new year brings.
[2622.60 → 2631.16] But I'm curious if your workflow in Obsidian has changed, let's say, in the last three months compared to where you started with it maybe in the spring.
[2632.12 → 2633.42] I don't think it has.
[2633.42 → 2643.90] I mean, I've been using that kind of outlining style of bullet points, you know, indented for many years in different plain text editors and things like that.
[2644.28 → 2651.08] I think the big difference really is just the searchability and discoverability within Obsidian is better than anything else.
[2651.16 → 2654.46] There's a plugin called Omni search that I absolutely adore.
[2654.46 → 2662.48] It not only does OCR search, but it also does, you know, in-document text search as well, which a lot of search things don't.
[2662.52 → 2665.26] They only do like keywords and titles and tags and that kind of stuff.
[2665.70 → 2669.54] I haven't worried too much about the whole Zettelkasten thing.
[2669.78 → 2674.42] I've just put my notes into folders and a directory structure that makes sense for me.
[2675.12 → 2680.72] I do a little bit of backlinking, but I haven't actually found that much utility in the end,
[2680.72 → 2684.42] which I know is the whole big selling point of these tools to start with.
[2685.30 → 2691.94] But, yeah, I just write stuff down, and I've got folders where, you know, I just need to dump a thought quickly into something.
[2692.16 → 2696.66] And I've got a keyboard shortcut that brings up a blank, you know, like I'm on a phone call.
[2696.72 → 2699.70] I need to write down a contact number or something.
[2700.14 → 2704.46] I've got a keyboard shortcut that brings up a brand-new note in my inbox folder, I call it.
[2704.46 → 2707.16] And so it just works for me.
[2707.50 → 2714.90] And I know that note-taking is an incredibly personal experience, but Obsidian has been just a revelation this year.
[2715.42 → 2720.38] Well, Chris, I got to ask about your notes' year because you built a whole PC around your notes' infrastructure.
[2720.50 → 2721.52] I'm curious how all that went.
[2721.82 → 2722.76] I am using Obsidian.
[2723.04 → 2724.68] It's going pretty well.
[2724.94 → 2728.74] I feel like I'm still struggling to decide what needs to be in its own vault.
[2728.74 → 2740.12] And I kind of find that I spend more time opening the app and then making sure my vaults are synced and then going through and making sure that all the stupid, obviously default sync options that should be checked are checked.
[2740.26 → 2741.38] That's very true.
[2741.64 → 2747.20] I hate that when you log into a new node, you have to check 15 boxes to say, sync this, sync that.
[2747.20 → 2751.28] And by the time I get ready to go write the note, I've already lost like half my momentum.
[2751.60 → 2753.38] That's the problem I'm having over and over again.
[2753.38 → 2758.06] But it does work for me, and it supports Markdown.
[2758.68 → 2760.96] And it, you know, so, you know, that's where I'm at.
[2760.98 → 2761.94] Yeah, but they all support Markdown.
[2761.96 → 2762.36] I don't know.
[2763.40 → 2771.46] I honestly, what I, again, because the issue for me is because a huge, huge, huge part of my note workflow is visual.
[2771.62 → 2772.12] It's pictures.
[2772.58 → 2775.64] I take a picture of something and I want to make notes about it.
[2775.72 → 2782.46] Or I take a picture of a receipt, or I take a picture of a sign, or I take a picture of an order, whatever it is, a parts list.
[2782.46 → 2783.82] And then I want to be able to search it later.
[2784.56 → 2785.88] There's just nothing great for that.
[2786.22 → 2787.80] And that's what I miss.
[2787.88 → 2788.92] That's what Evernote does really well.
[2788.98 → 2790.52] And that's what Apple Notes does really well.
[2790.72 → 2793.40] And I don't, I refuse to use either one of those systems.
[2793.60 → 2796.70] So with that set aside, Obsidian's working for me.
[2796.96 → 2801.38] And I have Omni Search and the other thing that lets me suck stuff in and all that kind of stuff.
[2801.56 → 2806.46] I really wish that Obsidian was an open source solution.
[2806.46 → 2812.54] I still maintain sovereignty over my data with Obsidian, which is the really critical part for me.
[2812.64 → 2822.00] It's just plain text files on my disk compared to things like Joplin, which come close, but they obfuscate things like the file names and ruin my directory structures and all that kind of stuff.
[2822.06 → 2824.50] Whereas Obsidian is just plain text files on the disk.
[2824.50 → 2838.70] To which you may well say, well, Alex, why don't you just use Tools, like Synching or whatever it might be, and sync or use iCloud Drive to sync and then use Synching to bridge the gap to clients that don't support iCloud Drive and Ada, Ada, Ada.
[2838.82 → 2839.50] And so on it goes.
[2840.18 → 2841.20] It's mobile, man.
[2841.32 → 2842.40] I tell you, it's iOS.
[2842.40 → 2847.66] It's the backgrounding APIs on iOS that screw me every single time.
[2848.34 → 2858.38] And without that, I wouldn't be paying Obsidian the absurdly high $8 a month for their proprietary syncing service.
[2859.06 → 2861.08] But for now, I am.
[2861.22 → 2862.42] And it works.
[2862.78 → 2864.36] So I guess I'm happy with that.
[2864.36 → 2874.50] I did flirt with a Nextcloud-only Notes-based solution, and I used Quilled, which is an app that almost has like a Google Keep-style UI.
[2874.62 → 2876.10] You know what I mean when I say that, like a postcard?
[2876.82 → 2885.08] But I was having this problem where I would enter data into Quilled, and then I would go into Nextcloud into the Notes app, and that data wouldn't be there.
[2885.18 → 2886.48] Oh, that's unacceptable.
[2886.48 → 2889.22] Some of the data would be in the web app, but not all of it.
[2889.46 → 2889.96] And yeah.
[2890.50 → 2891.82] The trust breaks down.
[2892.58 → 2893.50] So I went back to Obsidian.
[2893.50 → 2901.28] And To-Do, task management, news, those are all kind of categories that kind of stayed pretty static for me, but I'm curious if you've got any updates there.
[2901.72 → 2905.02] I have some nice workflows with G Suite for my work.
[2905.14 → 2908.72] This started at my Red Hat days because they were a G Suite-based organization.
[2909.64 → 2918.52] Tail scale also used G Suite for their emails, so I've just been able to lift and shift a lot of those things over from that side of things with To-dos.
[2918.78 → 2920.84] So it works on every platform I need.
[2920.94 → 2922.46] It's not expensive, really.
[2922.46 → 2924.06] The UI is nice.
[2924.16 → 2929.12] The fact that I can categorize things into priorities as well as categories and tags and projects.
[2929.38 → 2931.24] And a bit like Obsidian, really.
[2931.38 → 2934.38] It kind of doesn't prescribe a certain way of working.
[2934.64 → 2940.72] It just lets the tool kind of gets out of the way and says, right, there are 25 different ways to organize this piece of information.
[2941.24 → 2943.84] Pick one and stick with it, and you'll have a good time.
[2943.84 → 2946.48] I was a To-dos user, and I liked that a lot.
[2946.56 → 2948.92] But I wanted to try something that was self-hosted.
[2949.14 → 2953.50] And when Jeff came out, I really gave a go at Nextcloud Tasks.
[2953.82 → 2956.94] And that worked well for him, and it worked well for me.
[2956.94 → 2965.34] And what I really liked about it is I was creating the tasks as I thought about them using tasks.org on my Pixel.
[2965.34 → 2969.28] But Jeff was going through it on the web interface, so we could use both.
[2969.94 → 2976.74] That combination of Nextcloud Tasks with Tasks.org, the Android app, was really powerful.
[2976.88 → 2979.68] And Tasks.org can do things like reoccurring tasks.
[2979.68 → 2987.78] So I've set myself every Saturday, I have a series of, like, chip maintenance tasks that have to happen on tubes.
[2988.08 → 2989.10] You know, I need to go check this.
[2989.16 → 2989.84] I need to check on this.
[2989.90 → 2991.02] I need to manage this.
[2991.74 → 2998.52] And I needed something just to automatically every Saturday when I open up my Tasks app, I want to see some things I have to check off.
[2998.86 → 2999.56] That's sweet.
[2999.70 → 2999.88] Right.
[3000.26 → 3003.84] Now, Nextcloud Tasks itself doesn't offer that functionality yet.
[3004.66 → 3007.78] But Tasks.org syncing does.
[3007.78 → 3014.92] So I use the web UI, the nice big with my big keyboard and all of that, to enter in all my tasks using the Nextcloud interface.
[3015.46 → 3017.20] And then I open up Tasks.org on the phone.
[3017.30 → 3018.26] It's all synced down.
[3018.50 → 3021.02] And then I can just change them to reoccurring right there on the phone.
[3021.60 → 3022.32] Works great for me.
[3022.40 → 3023.28] It's just a nice little combo.
[3023.82 → 3030.82] But if that wasn't my setup, Todoist, I think, would be my go-to just because of the API, the general integrations.
[3031.04 → 3032.02] All of that's really nice.
[3032.76 → 3035.98] But, Brent, what are you using for task management besides paper?
[3036.08 → 3037.22] I know you use a lot of paper.
[3037.22 → 3037.86] It's true.
[3038.02 → 3040.08] You've caught me doing the paper thing.
[3040.72 → 3042.54] Yeah, I think I need an upgrade in this area.
[3042.70 → 3046.28] I did flirt with exactly the solution you mentioned with Jeff.
[3046.40 → 3052.22] Because when I was here and Jeff was, like, just cruising through that task list, it looked really sexy, actually.
[3052.28 → 3053.08] I was looking over his shoulder.
[3053.22 → 3055.80] I was like, that looks really nice, especially dark mode and everything.
[3055.90 → 3056.06] I know.
[3056.10 → 3057.84] And he's adding notes and contacts.
[3057.84 → 3058.72] Colours, too.
[3058.72 → 3064.66] And so I think the problem for me is actually not the apps because it sounds like they're there.
[3064.78 → 3069.48] And certainly with Nextcloud being the centre of my ecosystem, like, everything's already in place.
[3069.48 → 3074.80] I think I just need an upgrade, you know, in my discipline matrix or something.
[3075.12 → 3076.72] Maybe an extra day in the week.
[3077.34 → 3077.90] Oh, can we?
[3078.08 → 3078.86] Please, please, please.
[3079.16 → 3079.46] Okay.
[3079.46 → 3081.12] I got to talk server OSes.
[3081.60 → 3083.02] Not a lot of surprise from me.
[3083.10 → 3083.90] So what about you, Alex?
[3083.90 → 3086.14] Anything interesting happen to you in server realms?
[3087.04 → 3088.10] No, not really.
[3088.10 → 3091.76] I still run Proxmox almost everywhere in my house.
[3092.30 → 3095.54] And VPS land, it's Ubuntu 2204.
[3095.54 → 3107.50] I do have designs on switching out some of the more appliance nodes, particularly the VPSs, to Nix and having, you know, remote builders and all that kind of stuff figured out.
[3107.70 → 3110.92] Still a bit of learning for me to do there before I can do that reliably.
[3111.82 → 3114.64] But that's what I'm hoping I'll do in 2024 anyway.
[3114.64 → 3122.84] I'm curious, Alex, when you say Nix, do you mean, like, using the Nix package manager on these, you know, like Ubuntu, for instance?
[3123.02 → 3126.98] Or do you mean more Nix OS completely as the entire operating system?
[3127.32 → 3131.90] I think if you're going to go Nix on Linux, you may as well just go all in.
[3132.54 → 3132.92] Yeah!
[3133.44 → 3133.88] Yeah.
[3134.12 → 3137.90] I am so happy with my O-directed home running Nix OS.
[3138.14 → 3139.82] We're going Nix OS everywhere as I can.
[3140.08 → 3142.72] I tell you what, the OBS machine this year, Nix OS.
[3143.10 → 3143.72] How's that been?
[3143.72 → 3144.16] Great.
[3145.00 → 3146.76] In fact, fun.
[3147.02 → 3151.34] For the first time ever, the OBS machine isn't this sacred cow that we can't touch.
[3151.90 → 3157.96] It's always been this delicate, precious thing that you don't change anything on.
[3158.22 → 3168.72] And now, after the show sometimes, after we shut everything down, and we've had some food, Was and I are like, you want to try switching XYZ out?
[3168.90 → 3169.50] You guys.
[3169.50 → 3174.46] Like, what if we just move the whole thing over to Wayland and Pipe wire and just see if it works?
[3175.22 → 3176.36] And Plasma 6.
[3176.42 → 3177.58] Let's try Plasma 6, too.
[3178.06 → 3181.30] And if it doesn't, it's just one entry and grub, and we go back and everything's fine.
[3181.52 → 3186.36] You can completely break your production system, one of your most critical systems.
[3186.72 → 3187.60] You can experiment.
[3187.82 → 3188.48] You can test.
[3188.58 → 3189.34] You can try.
[3190.06 → 3190.86] You can develop.
[3191.28 → 3192.10] You can destroy.
[3192.88 → 3194.88] And then you can be like, all right, good time.
[3195.02 → 3195.54] All right, roll back.
[3196.54 → 3197.60] That's so powerful.
[3197.78 → 3198.54] It is massive.
[3198.86 → 3199.84] It's massive for us.
[3200.18 → 3204.92] And so there was a moment where I was going on the road, and we had to switch from Wayland back to X11.
[3205.10 → 3206.72] And we're like, well, what if this breaks something?
[3207.46 → 3208.24] Oh, we'll just roll back.
[3208.28 → 3208.80] Yeah, no big deal.
[3208.80 → 3212.70] So, yeah, it's been huge for production systems.
[3212.82 → 3215.12] And so it's been the year of Nix for me.
[3215.68 → 3220.50] Well, and I feel like, at least in my own mind, and I think it's been true of each of you as well,
[3220.58 → 3224.84] that often in this conversation about Nix OS, Ansible comes up.
[3224.92 → 3227.52] It's like, well, you could just do many of these things in Ansible.
[3227.52 → 3233.56] But that's a good example of when you're running Nix OS, you know, going the whole thing.
[3234.18 → 3238.36] These are some of the nice little features that you do get out of it that are, yeah.
[3238.84 → 3239.60] Worth it.
[3240.04 → 3247.50] The thing about Ansible really is that it fits into the older, dare I say, style of thinking about Linux systems.
[3247.76 → 3255.60] And it got those, it bridged the gap between where Nix is now and where Linux was before.
[3256.38 → 3262.60] There is an issue that I don't think I've fully solved yet with switching to Nix in the cloud, though,
[3262.68 → 3266.98] which is trying to find a VPS provider that will let me run Nix OS natively.
[3266.98 → 3272.62] I did figure out that you can just boot custom images on Hetzner the other day, which was kind of nice.
[3273.12 → 3273.24] Yeah.
[3273.36 → 3278.66] Also, you could just basically take over any distro.
[3279.12 → 3280.40] You are the Borg now.
[3280.88 → 3284.48] And just, so, like, I think we even did it live on UP once.
[3284.72 → 3285.80] Yeah, with Nix anywhere.
[3285.80 → 3291.20] Yeah, I think we had Was just reunify a VPS from, like, Ubuntu to Nix OS Live.
[3291.80 → 3295.22] And it just switches, it kind of just goes in, its cheroots, and it just takes over.
[3296.28 → 3297.60] It's kind of magical, actually.
[3297.76 → 3299.76] And I think, Alex, you would really enjoy playing with that.
[3299.88 → 3300.24] Probably.
[3300.58 → 3300.86] Probably.
[3300.86 → 3304.72] Linode.com slash SSH.
[3304.78 → 3307.60] I don't always cloud, but when I do, it's Linde.
[3307.72 → 3309.68] And now Linde is part of Akamai.
[3310.12 → 3313.48] The Akamai that you've heard about and known about for a long time.
[3313.56 → 3314.68] The tops of the tops.
[3315.02 → 3320.24] But all the friendly tools, like the cloud manager, the API that's powerful, the command line client that's so handy,
[3320.32 → 3324.18] all the things that we've used to build and deploy and scale, that's still available.
[3324.18 → 3327.62] But now it's combined with Akamai's power and global reach.
[3328.10 → 3331.96] They're expanding their services to offer more resources and more tooling,
[3332.40 → 3336.90] but keeping the reliable, affordable, scalable solutions for individual home labours,
[3337.10 → 3340.38] small projects, or enterprises and businesses of all sizes.
[3340.98 → 3342.24] It's Akamai we're talking about here.
[3342.30 → 3345.32] And part of their global network offerings, data centres are getting bigger and better,
[3345.78 → 3350.90] expanding worldwide, giving you more access to more resources to help you grow your business
[3350.90 → 3354.60] and serve your customers, your friends, your project, or whatever it might be.
[3355.42 → 3355.98] So why wait?
[3356.66 → 3357.82] Go see what I'm talking about.
[3358.16 → 3360.20] Experience the power of Linde, now Akamai.
[3360.52 → 3363.96] Go to linode.com slash SSH, support the show,
[3364.26 → 3369.68] and learn how Linde, now Akamai, can help you scale your applications from the cloud to the edge.
[3370.24 → 3372.88] Linode.com slash SSH.
[3374.68 → 3377.56] So continuing the theme of Nix and everything like that,
[3377.56 → 3385.20] my primary workstations this year have seen quite the change in how I manage the configuration for those systems.
[3385.84 → 3391.10] I'm still using macOS as my daily driver because I'm doing an awful lot more video than I was a year ago.
[3391.80 → 3398.16] And, you know, Final Cut is pretty good and the M1 stuff and, you know, we all know this.
[3398.54 → 3401.82] Actually, I will just say, just to support what you're saying,
[3401.88 → 3406.84] for the first time in like six months I did video on a Mac again after doing it on my Linux box,
[3406.84 → 3408.12] just doing quick little cut stuff.
[3408.92 → 3412.20] Oh my God, Alex, it's so much better on the M1 platform than it is.
[3412.52 → 3414.70] Like the export stuff, it's like just saving a file.
[3415.20 → 3420.72] Like I'm exporting to an H.264 file, and it just goes so quick, it's like I just saved a JPEG.
[3420.98 → 3421.84] Oh man.
[3422.36 → 3424.12] So it really is very impressive.
[3424.80 → 3426.96] I actually did a render for one of my YouTube videos the other day
[3426.96 → 3430.42] and, you know, went through to play with Ella for a bit whilst it rendered.
[3430.42 → 3435.50] You've seen the programmer's code compiling XKCD comic, right?
[3435.58 → 3437.78] That's basically how I felt about video rendering.
[3438.50 → 3442.16] And I've got the Mac Studio in front of me with an M2 Macs in it and it just,
[3442.46 → 3444.26] it must have done it in like two minutes.
[3444.36 → 3445.04] It was unbelievable.
[3445.94 → 3449.52] But I've adopted on my Mac workstations,
[3449.82 → 3454.70] Nick's Darwin in a Flake setup, and it has just been wonderful.
[3455.16 → 3456.24] Absolutely wonderful.
[3456.24 → 3459.94] Yeah, I think the most impressive thing was that when you got your latest machine,
[3460.08 → 3463.64] it was, you took like a two-day setup process into like 30 minutes.
[3464.42 → 3467.36] I mean, I've still got to log into everything, which is still a pain in the ass.
[3467.54 → 3467.80] Yeah, yeah.
[3468.16 → 3471.22] Yeah, the installing of all the Brute apps and, you know,
[3471.26 → 3473.76] configuring system preferences just the way I liked them,
[3473.80 → 3477.24] putting the dock in the right place, changing the order of the icons in the dock,
[3477.94 → 3481.56] configuring my terminal to have the correct completions and history.
[3481.86 → 3484.72] And there's just so many little things that, you know,
[3484.72 → 3487.26] when you're moving into a new shell, a new Mac,
[3487.64 → 3489.46] it's like a hermit crab into a new shell.
[3490.10 → 3492.62] It takes you a good week or two typically to,
[3492.76 → 3494.94] and I think I've cut that down to maybe a day or two.
[3495.42 → 3496.10] That is impressive.
[3496.60 → 3497.84] You mentioned brew in there.
[3498.70 → 3502.48] Isn't there quite an overlap between those two package managers?
[3502.70 → 3504.72] I'm curious why you're sticking with brew for certain things.
[3505.16 → 3505.96] I don't know why.
[3506.10 → 3507.24] That's just how you do it, isn't it?
[3508.24 → 3510.46] Oh, Alex, you'll grow up one day.
[3510.48 → 3511.74] You can install more from Nix, yeah.
[3511.74 → 3515.28] I do install a lot of tools from Nix, but there are certain things like casks,
[3515.44 → 3520.22] I think, for like GUI applications on macOS that the brew side of things still makes sense.
[3520.56 → 3525.12] I don't have a ton of brew stuff, but please, if you're in the audience, and you care about such things,
[3525.56 → 3529.68] go and look at my Nix config repo on GitHub, ironic badger, Nix config,
[3530.20 → 3531.48] and tell me what I'm doing wrong.
[3532.32 → 3535.88] I'd love to know because I'm just in sponge mode with Nix right now.
[3536.18 → 3538.58] Nothing fascinating for me, workstation-wise.
[3538.58 → 3540.08] Nix OS everywhere.
[3540.60 → 3545.84] The only thing that's really changed for me is I went from Plasma last year to GNOME this year
[3545.84 → 3548.46] because 44 and 45 I was just really interested in.
[3549.00 → 3550.90] So that's kind of it for me.
[3551.38 → 3555.22] And then Asa hi Linux on the M1 Macs that is also GNOME.
[3555.50 → 3556.40] That's been pretty great.
[3556.98 → 3561.48] And then I got one Mac machine right here that's been really nice, too, for some Mac stuff.
[3561.88 → 3562.92] So nothing too strange there.
[3563.06 → 3565.26] So let's move on to more of the back-end stuff.
[3565.80 → 3567.30] What about reverse proxy?
[3567.30 → 3573.52] I wanted to put this one in specifically because I had a bit of a switcheroo this year.
[3573.88 → 3578.18] Started the year with traffic and actually ended up back on Nginx.
[3578.42 → 3579.08] How come?
[3579.66 → 3581.12] Nothing too dramatic there.
[3581.24 → 3584.54] When I switched to Nix OS and started working with We son it,
[3584.76 → 3592.00] we came across some ways to just easily use, just pull in Nginx and just define everything right there
[3592.00 → 3593.58] in a very simple to understand way.
[3593.68 → 3599.32] And I thought I could understand the entire setup, and it could fit in one terminal window.
[3599.64 → 3601.06] And I thought, well, let's just go with that.
[3601.16 → 3603.12] And it's worked for me and I haven't needed to change.
[3603.62 → 3604.50] That's just the thing, isn't it?
[3604.50 → 3605.88] If it's working, don't touch it.
[3605.88 → 3614.08] So traffic's really nice because you define it in the same place as you define the application's configuration,
[3614.42 → 3616.98] if you're using Docker anyway, in the compose file.
[3617.38 → 3623.90] But I, as part of that whole network reshuffle in the spring, threw up a CANDLES system.
[3623.90 → 3631.44] And I have been absolutely loving the simplicity of CADD LX files for the last six, eight, nine months,
[3631.50 → 3632.10] whatever it's been.
[3632.86 → 3636.06] Just a few lines, like three or four lines of config per service.
[3636.40 → 3641.36] Okay, it doesn't live alongside the service itself, but it does mean that non-Voucherized services,
[3641.50 → 3645.32] things like Blue Iris and my Proxmox front ends and Ada, Ada, Ada,
[3645.54 → 3650.78] all now go through this one CADD LX instance on the LAN, and it's great, honestly.
[3651.10 → 3653.78] Any interesting things changing in your containers?
[3653.90 → 3654.14] I had a lot of stuff.
[3654.76 → 3657.10] I'd begun the year playing around with Rodman.
[3657.36 → 3662.48] I also played around with the Rodman-Docker-Compose compatibility and ended up sticking with Docker.
[3663.12 → 3666.04] Well, we had a bit of a scare with Docker in the middle of the year, didn't we?
[3666.14 → 3666.36] Yep.
[3666.52 → 3667.26] If you remember.
[3667.52 → 3669.44] We did a special up on it, I think.
[3670.14 → 3675.24] Yeah, and remember the ridiculous with the whole, it was an account switcheroo with the payment stuff,
[3675.32 → 3678.32] but also there was some namespace potential poaching that was going to happen.
[3678.88 → 3679.10] Yeah.
[3679.24 → 3681.02] Docker kind of walked it back a bit.
[3681.02 → 3681.66] They did.
[3681.76 → 3684.64] So it was the whole rate limiting situation, I think, if I recall.
[3685.22 → 3691.16] But no, I'm still sticking at the moment with Docker Engine, whatever you call it, Docker and Docker Compose,
[3691.74 → 3694.22] running through my Ansible generator.
[3694.52 → 3698.04] I wrote that as I was emigrating, and I've been here five years now,
[3698.12 → 3700.72] so I guess I'm going strong into year six using that system.
[3701.84 → 3702.10] Good.
[3702.44 → 3705.70] You know, if it works, especially for that kind of stuff, keep it.
[3705.70 → 3714.34] I do want to, you and I spent some time with a friend of mine talking through some Nix containers with System Spawn
[3714.34 → 3721.68] and installing Tail Scale into each container itself effectively and then having each service as its own node on a tail net,
[3721.74 → 3722.40] that kind of thing.
[3723.04 → 3725.18] And that kind of stuff piqued my interest.
[3725.18 → 3731.98] It's going to be a lot of work, you know, cognitive to understand what's going on because it's all flakes and all that kind of stuff.
[3732.10 → 3736.04] But I feel like that's probably where I will end up this time next year.
[3736.60 → 3737.94] But we'll see, I guess.
[3738.46 → 3738.54] Yeah.
[3738.64 → 3744.22] Just to underscore what you're saying there, that setup eliminates the need for the reverse proxy.
[3744.88 → 3745.72] That's what I need.
[3746.30 → 3748.18] Because the reverse proxy for me has been...
[3748.72 → 3749.48] It's just a barrier.
[3749.68 → 3749.96] Yeah.
[3749.96 → 3752.94] It's like a whole thing you've got to figure out before you can do the other stuff.
[3753.06 → 3755.08] I've been stuck at that point for about three years now.
[3755.22 → 3755.38] I know.
[3755.40 → 3760.74] And I just haven't really had the time to, like, really dive in and feel confident about it.
[3760.78 → 3760.84] I hear that all the time.
[3760.84 → 3761.82] I hear that all the time.
[3762.08 → 3763.02] I hear that all the time.
[3763.14 → 3766.00] And it's like, but boy, once you just learned it, it's not a big deal.
[3766.08 → 3768.74] Like, I could show you my Nginx config and be like, oh, okay.
[3769.02 → 3770.56] You would literally be like, that's not a big deal.
[3771.42 → 3775.72] However, there is just a conceptual thing you've got to get around.
[3775.72 → 3782.92] And for me, it's easier because I was in the industry when reverse proxies became a thing.
[3783.22 → 3785.68] So I was deploying reverse proxies when they were first a thing.
[3785.74 → 3786.82] And so it just made sense initially.
[3787.30 → 3788.96] But I hear that all the time.
[3789.16 → 3796.24] And what this tail scale setup does is it takes out the reverse proxy, and it puts the actual individual application directly on the tail net.
[3796.96 → 3801.34] And then you just connect directly between the different applications as you need on the tail net.
[3801.34 → 3813.24] But you've got to learn Nix, which in and of itself, unless you enjoy rock climbing and the view from the top, the learning curve for that, I would argue, is a lot steeper than just learning reverse proxy.
[3814.76 → 3822.12] Well, one consideration I always have with network stuff, especially when I'm learning it as I'm implementing it, is just a security consideration.
[3822.12 → 3825.80] So that's a big part of, I think, why I've hesitated.
[3826.10 → 3832.94] It's like, I don't feel that comfortable with my own skill set at doing it well and right to protect myself.
[3833.46 → 3835.98] But let's talk about file systems for a moment.
[3836.90 → 3840.40] Because this, I think, is the area where we probably diverge the most.
[3840.66 → 3845.44] I don't disagree with you necessarily, but in terms of actual implementation, we probably just disagree the most.
[3845.44 → 3848.20] ZFS for anything important.
[3849.20 → 3853.78] And people in the audience give me a hard time for switching between Z and Z all the time.
[3854.30 → 3857.24] And my brain doesn't know what side of the ocean it's on.
[3857.48 → 3860.28] I just, oh yeah, Canadians say Z as well, don't they?
[3860.42 → 3860.72] Sure do.
[3861.06 → 3863.24] Yeah, I think we got more Zs and Zs on this one.
[3863.40 → 3865.80] Like my little abbreviation, Alex KTZ.
[3866.22 → 3867.38] That's what I say in my head.
[3867.38 → 3871.50] But then when I'm spelling it to someone at the post office, it could be KTZ, whatever.
[3871.82 → 3873.14] Anyway, I digress.
[3873.14 → 3875.50] ZFS for anything important.
[3876.00 → 3880.88] Mostly because of the checksumming and data protection features, of the snapshooting features,
[3881.16 → 3889.04] and the fact that I can do the replication really easily at the block level instead of worrying about some of the chunking stuff you were talking about earlier, Brent,
[3889.14 → 3891.40] with Borg and Rustic and all that kind of stuff.
[3891.90 → 3897.72] For media files, or the ahem, more ephemeral side of my storage needs,
[3897.72 → 3904.18] is each disk is just XFS with Mergers on top to merge it together into one single mount point.
[3904.18 → 3910.88] So what that allows me to do is to have, I don't know, five data disks in my media server of differing sizes.
[3911.46 → 3915.72] One could be USB, one could be SATA, one could be NVMe, for example.
[3915.88 → 3916.40] It doesn't matter.
[3916.50 → 3918.30] They don't have to be the same size as with RAID.
[3918.30 → 3926.94] So just any array of BOD disks I can bring into a Mergers, air quotes, array, if you like,
[3927.06 → 3932.44] and then I view all the files on those drives as if they were all on the same drive,
[3932.52 → 3934.10] all together with a bunch of policies underneath.
[3934.10 → 3939.68] I then use Snap RAID to calculate parity for the data on that BOD.
[3940.40 → 3942.56] But I'm considering dropping it altogether.
[3942.82 → 3948.64] In the last seven years since I first wrote Perfect Media Server over on edxserver.io,
[3948.94 → 3954.32] I think I've recovered files once or twice using Snap RAID.
[3954.62 → 3961.24] And since I've moved all of my critical data over to ZFS, I've used it precisely zero times.
[3962.14 → 3962.62] Hmm.
[3962.62 → 3962.74] Hmm.
[3963.48 → 3969.76] I have been reducing my XFS usage this year as the longtime maintainer stepped aside.
[3969.92 → 3971.56] New maintainers in there, they're doing a great job.
[3972.10 → 3976.08] But I just decided that maybe it was getting old enough.
[3976.26 → 3982.30] I was using XFS when probably most people in this listening probably weren't using computers.
[3982.44 → 3984.58] I mean, I've been using it for a very, very long time.
[3984.82 → 3987.80] And so to me, it just seems like maybe it's getting to the point where it's,
[3988.30 → 3990.62] well, it's going to go through kind of transitionary year.
[3990.62 → 3997.28] And what you just described, what you do with Mergers and your Bods,
[3997.76 → 3999.80] I actually do kind of the reverse with Butters.
[4000.00 → 4002.56] And this is why I continue to deploy more Butters.
[4002.78 → 4003.38] I agree with you.
[4003.38 → 4004.40] ZFS is fantastic.
[4004.72 → 4006.38] And everybody should use it.
[4006.52 → 4007.36] Don't use Butters.
[4007.36 → 4015.68] But what I do is I set up a very crappy RAID because I just have really crappy disk hanging off my Droid over a SAT or a USB.
[4016.28 → 4017.98] And I set up some mirrors with that.
[4018.42 → 4024.38] And, you know, maybe this is like a four terabyte mirror over here and like a one terabyte mirror over here and like a two terabyte mirror over here.
[4024.38 → 4028.82] And then I use Butters add volume and it just kind of creates.
[4028.92 → 4029.26] I'm not sure.
[4029.30 → 4030.18] I'm probably getting the command wrong.
[4030.52 → 4035.04] But it creates essentially a one giant virtual disk.
[4035.10 → 4037.92] And it doesn't matter if this one's two terabytes and this one's one terabyte.
[4038.16 → 4045.30] It'll create one kind of unified storage point that I can mount and then put all my media on that'll go across all those devices.
[4045.30 → 4047.78] And, you know, it's built into the Linux kernel.
[4048.00 → 4051.36] So it always works, just works every time, even on my root device.
[4051.46 → 4056.60] It's fantastic on like ARM devices and on like Droids where I'm talking like really low resources.
[4056.98 → 4060.76] And then to have kind of these advanced capabilities where I can do Butters send.
[4060.88 → 4062.30] I have compression capabilities.
[4062.38 → 4063.56] I have encryption capabilities.
[4063.94 → 4069.00] I can do this kind of add all these different disparate disks into one giant volume things.
[4069.16 → 4074.24] All kind of just built-in with tools that just kind of are really simple to understand and come pre-installed.
[4074.24 → 4076.52] I just can't turn that away.
[4076.58 → 4077.66] And I think that's a great thing.
[4077.74 → 4081.30] And I don't think people should discount Butters at all.
[4081.48 → 4094.22] But, you know, if I had a, you know, a Leon box that I was reusing with 128 gigs of RAM and, you know, 20 plus terabytes of storage, I'd probably be using ZFS on it myself.
[4094.36 → 4098.74] But for me, it's been less XFS, more Butters just because of the hardware I'm running.
[4098.74 → 4106.36] My primary server is just an i5-8500, and it's got 64 gigs of RAM in it.
[4106.36 → 4106.56] Yeah.
[4106.82 → 4107.00] Yeah.
[4107.00 → 4107.68] You don't need a lot.
[4108.08 → 4109.84] I'm just saying like if I was building a big box.
[4110.08 → 4110.56] Right.
[4110.74 → 4123.12] But then you're also speaking to the guy who was spending most of his afternoon looking at Epic Rome based CPUs and wanted to upgrade his HL15 CPU.
[4123.60 → 4124.22] So let's go.
[4124.22 → 4133.08] You know what I will say, though, is that one of the really nice things about Butter versus ZFS is that it's built into the Linux kernel.
[4133.44 → 4144.54] You know, I've kind of largely sidestepped that being an issue by running exclusively Proxmox everywhere because they baked that in thanks to Ubuntu having the courage to ship ZFS as part of their distribution.
[4145.36 → 4146.72] No more DKMS for me.
[4146.78 → 4150.32] I kind of swore off that a while ago because it's just a bad experience.
[4150.52 → 4150.64] Yeah.
[4150.74 → 4151.80] It's not so bad on Ubuntu.
[4151.80 → 4156.92] And then Nix OS also now it's just a couple of lines, and you've got it too.
[4157.24 → 4158.42] It's basically baked in.
[4159.28 → 4163.38] We have seen a couple of bugs in all of these file systems this year too, I think.
[4163.62 → 4163.86] Yeah.
[4164.16 → 4164.34] Yeah.
[4164.48 → 4168.50] Butters, Extended 4, ZFS, CFS.
[4169.32 → 4171.98] They all kind of had some bad bugs this year.
[4172.46 → 4177.02] I was looking back at the stories and ZFS almost made it, man.
[4177.08 → 4178.02] It almost made it.
[4178.02 → 4181.44] But then they had some data corruption there.
[4181.64 → 4184.22] Now, what are you doing home automation hardware-wise, Alex?
[4184.22 → 4186.44] I know you've moved things around a little bit.
[4186.90 → 4188.56] I'm imagining it's all Home Assistant still.
[4189.02 → 4189.84] Still Home Assistant.
[4190.14 → 4193.16] It'll be the surprise to absolutely nobody in the audience.
[4193.94 → 4194.80] Ding, ding, ding.
[4194.94 → 4198.56] Yes, the home automation category is Home Assistant for both of us.
[4199.70 → 4200.14] Surprise.
[4200.14 → 4205.60] I found this year real joy in switching my Zigbee controller.
[4205.98 → 4211.40] We've documented it in the show several times that I kind of wasn't super sold on Zigbee over the years.
[4211.90 → 4216.06] And I switched to one built by a chap called Tubes ZB.
[4216.66 → 4217.02] There you go.
[4217.14 → 4218.26] I used Z that time.
[4218.52 → 4220.70] See, it's interchangeable in my brain, audience.
[4220.88 → 4222.50] Stop giving me a hard time, please.
[4223.16 → 4227.96] The Tubes ZB Zigbee controller is powered over Ethernet.
[4227.96 → 4235.84] It has a little radio in it so it can live in the house where it makes the most sense for the device to physically live.
[4236.42 → 4241.20] And then it connects back to Home Assistant over Ethernet as a serial device over Ethernet.
[4241.42 → 4252.16] So I don't need a USB dongle hanging out the back of my box in the basement, zip tied to a cross member underneath my house in the basement with no antenna on it.
[4252.26 → 4256.06] So I was using the Combee 2 for a long time, and it was just not a good experience.
[4256.06 → 4261.56] And this Tubes ZB coordinator and router has been absolutely fabulous.
[4261.68 → 4269.78] First time every time on buttons, on the IKEA smart blinds I bought, on all the Ankara temperature sensors that I've kitted the house out with.
[4270.56 → 4271.06] It's great.
[4271.20 → 4271.94] It's just fabulous.
[4272.14 → 4274.56] I have no bad things to say about it whatsoever.
[4274.56 → 4279.16] If people ask me, hey, I only want to buy one, what should I get?
[4279.22 → 4280.78] And I want reliability as a top thing.
[4280.86 → 4285.82] I'm still recommending Z-Wave because it's 900 megahertz, and you just can't beat 900 megahertz.
[4286.04 → 4292.40] But what happened for me with Zigbee was the realization this year that it's all in the repeaters.
[4292.40 → 4300.42] If you're trying to cover some location, you need to get like smart plugs, and you need to strategically place them.
[4300.58 → 4305.82] And where you can really be taken out, man, and I am still gets me.
[4305.92 → 4307.10] It still gets me to this day.
[4307.38 → 4310.08] I got one just as an experiment.
[4310.30 → 4312.24] Zigbee LED light strip.
[4313.36 → 4314.36] Off of Amazon.
[4314.54 → 4315.64] How easy could this be?
[4315.70 → 4316.98] We had an LED light strip replaced.
[4317.08 → 4318.18] I just want one colour.
[4318.92 → 4319.90] I want it on Zigbee.
[4320.30 → 4321.12] I'll put it here.
[4321.94 → 4326.32] And of course, it drops off the Zigbee network about once a week.
[4327.34 → 4330.26] And the way the Zigbee network works is everything is mesh.
[4330.36 → 4331.32] Well, wouldn't you know it?
[4331.58 → 4340.56] A bunch of devices this year, like the Christmas tree, are connecting to this LED light strip as their node that they route through.
[4340.78 → 4343.20] And so when this guy drops off, they all die.
[4343.66 → 4349.14] So now like my Christmas lights and my Christmas tree aren't turning off on time or at the bedtime script.
[4349.14 → 4353.20] And you cannot control that.
[4353.36 → 4353.72] You cannot.
[4353.98 → 4361.94] All you can do is like turn a device off, unplug it, have stuff refit itself out, reconnect, and then plug the other device back in.
[4362.10 → 4363.12] Hope it doesn't reconfig.
[4363.72 → 4366.62] And I find that to be very frustrating with Zigbee.
[4366.62 → 4374.04] But getting powerful repeaters that are a good option for nodes to connect to, I think is the best, as far as I know.
[4374.28 → 4375.20] Let me know otherwise.
[4375.58 → 4378.40] As far as I know, it's the best solution to this.
[4379.12 → 4384.26] But Alex, I've never, ever in years had to do that with C-Wave devices.
[4384.84 → 4386.62] So there's still that.
[4386.82 → 4389.82] But Zigbee's, you know, I guess at least it's open source.
[4389.82 → 4391.08] What about you, Brent?
[4391.18 → 4397.16] Do you have any home automation desires for, well, do you have any changes over the last year or desires for next?
[4397.58 → 4399.98] No changes because there wasn't really much in place.
[4400.08 → 4402.66] But I think desires is a good category.
[4402.90 → 4412.80] As I get more adventurous with my own little home lab setup, I definitely think there are some opportunities to do some automations of certain things.
[4412.80 → 4417.04] I'm installing, like, new heaters and stuff in my cabin as backup source.
[4417.24 → 4417.62] There you go.
[4417.62 → 4418.10] And, yeah, you've been.
[4418.10 → 4418.96] That's how it starts.
[4419.28 → 4419.94] Solve a real problem.
[4419.94 → 4420.66] Lighting and heaters.
[4420.78 → 4424.00] I'm really hoping to just bait you, Chris, to come out.
[4424.24 → 4424.62] I know.
[4424.84 → 4428.44] And Alex, if you want to join, we could do a whole, like, project out of it.
[4428.44 → 4428.98] Oh, we could.
[4429.36 → 4430.80] Lighting for this guy, right?
[4430.88 → 4433.46] Because he lives in an area where it gets dark for a very long time.
[4433.48 → 4435.92] So some automated lighting to keep it nice.
[4436.02 → 4436.42] Some heating.
[4436.62 → 4438.30] I could see a pretty cool setup out there.
[4438.46 → 4440.56] Mostly, like, utility, but bring it on.
[4440.56 → 4446.24] Okay, so our final category, the honourable mentions' category, I just have a really quick one.
[4446.74 → 4447.78] This one just is obvious.
[4448.26 → 4450.56] It's the ESP32 platform.
[4451.12 → 4453.32] It has just been fantastically useful this year.
[4454.08 → 4459.88] We have sensors in every room in the studio measuring temperature and humidity, thanks to listener Jeff.
[4460.70 → 4466.70] They've been incorporated in multiple different ways into the RV to automate essential functions of my RV now.
[4467.40 → 4469.00] Like, absolutely essential functions.
[4469.02 → 4470.26] Built literally into the wall.
[4470.26 → 4472.48] Yep, built into the wall in a few cases.
[4472.82 → 4476.62] And also built into, like, some control boxes and whatnot out in, like, the water bay.
[4477.48 → 4482.80] And they're just, the potential with the ESP32 platform is remarkable.
[4482.90 → 4489.40] And then you combine it with the year of voice and the ESP32-powered little remote listening devices.
[4489.60 → 4495.20] It's just, for me, been like the Swiss army knife of self-hosting this year.
[4495.20 → 4499.12] You know, what's fascinating is my item on this list was 3D printers.
[4499.48 → 4513.74] In the last month, I have switched from a fully open Brusa i3 Mark III S Plus and Octobrist combo to a pair of Bamboo Lab printers, which I made a video about on YouTube if you're interested.
[4513.74 → 4518.48] But what I found was fascinating was their cheaper model that I bought, the P1S.
[4518.48 → 4522.56] That entire 3D printer runs off an ESP32.
[4523.14 → 4523.44] Ah!
[4524.38 → 4525.10] How about that?
[4525.42 → 4526.46] That's really impressive.
[4526.88 → 4528.20] Although also kind of concerning.
[4529.24 → 4530.30] It's kind of amazing.
[4530.42 → 4530.70] No, no, powerful.
[4530.92 → 4531.94] Yeah, yeah, yeah, it is.
[4531.94 → 4536.92] So off this thing, they're able to run not only the 3D printer itself, but also a webcam somehow.
[4537.14 → 4542.58] Okay, it's like 0.5 frames a second webcam, but the fact it works at all is kind of amazing.
[4542.98 → 4544.70] And the Wi-Fi and all the rest of it.
[4544.84 → 4554.00] So, you know, those ESP devices, they just enable so many applications that were just impossible at the price points that these things are shipping at now.
[4554.46 → 4555.60] And the accessories are endless.
[4555.60 → 4562.28] You can browse on Amazon and Alibaba and all these other places, just sensors, probes, all kinds of stuff.
[4564.86 → 4567.42] 45homelab.com, the HL15 is here.
[4567.56 → 4573.10] It's available for purchase now in three different configurations, depending on what you need.
[4573.22 → 4575.82] We're talking big, strong, and fast.
[4575.94 → 4578.40] And it is also beautiful.
[4578.98 → 4581.42] And one of my favourite things is powered by open source.
[4581.42 → 4586.12] They've got a great system on there where you can install applications, running Rocky Linux under the hood.
[4586.84 → 4588.38] And you know 45 drives, right?
[4588.44 → 4592.76] They're well-known for their direct wired approach, high-performance, enterprise-grade capacity.
[4593.12 → 4594.62] They're bringing that to the home lab.
[4595.12 → 4605.20] Their design ethos, their performance ethos, their enterprise stability ethos, all coming into a box that you can have that lives up to your ideals in your home lab.
[4605.20 → 4612.40] With applications, the staff have hand-picked, and a community forum, which is active in helping people get it all sorted out and really learn this box.
[4613.24 → 4615.30] And man, does this thing look like it can cook, too.
[4615.86 → 4621.24] Super fast, and you can build it up to your own particular configuration or buy one that's pretty much ready to go.
[4621.74 → 4622.64] Go check it out.
[4622.74 → 4623.34] It's beautiful.
[4623.50 → 4623.94] It's here.
[4624.12 → 4624.70] It's fast.
[4625.26 → 4626.26] It's the HL15.
[4627.00 → 4630.02] It's 45homelab.com from the folks at 45 drives.
[4630.14 → 4632.02] That's 45homelab.com.
[4632.02 → 4638.72] Well, given it's the last show of the year, we got our last boots batch of the year.
[4638.92 → 4641.42] I bet we've got some cookies in here.
[4641.54 → 4642.16] Look at that.
[4642.52 → 4644.98] Shafts and Spanner came in with 20,000 sets.
[4645.04 → 4645.40] Woo-hoo.
[4645.68 → 4647.72] Kicking some boots with some boots using Pod verse.
[4648.40 → 4653.08] He says, Chris, I share your pain about syncing watch status between Plex and Jellyfin.
[4653.52 → 4655.34] Then I found Plex Jellyfin Watched.
[4655.60 → 4656.56] It's a Docker container.
[4656.66 → 4657.70] He links it for us.
[4657.74 → 4658.80] We'll have a link in the show notes.
[4659.48 → 4661.36] And it has exactly what you want.
[4661.36 → 4664.96] Full sync between multiple Plex and Jellyfin and Envy servers.
[4665.70 → 4666.34] All local.
[4666.42 → 4670.12] No need to share your media library with the tracker sites.
[4670.60 → 4672.94] Now I've just got to go sort out the wife approval factor.
[4673.10 → 4674.04] Oh, you're on the right track.
[4674.14 → 4674.88] That's a great pick.
[4674.96 → 4675.82] Yeah, we had this sent in.
[4676.12 → 4676.34] Yeah.
[4676.50 → 4677.22] A couple of times.
[4677.36 → 4680.12] This is vindication, Alex.
[4680.34 → 4681.10] This is vindication.
[4681.76 → 4682.04] Absolutely.
[4682.04 → 4684.58] Multiple people are running Jellyfin and Plex at the same time.
[4685.12 → 4686.36] We're not alone.
[4686.36 → 4696.38] Do you ever feel like sometimes we mention things on air, and we're lucky enough that, I don't know, people go out and make it or that they have the same use cases, and we just get to discover these things over and over?
[4696.38 → 4701.82] But like, I honestly, I thought I was the only idiot trying to like to manage a Plex and a Jellyfin server on the same box at the same time.
[4701.82 → 4702.86] Why would you do that?
[4702.88 → 4704.36] It feels like chasing your own tail.
[4704.60 → 4705.38] But you know what?
[4705.64 → 4706.38] Shaft and Spanner.
[4706.52 → 4708.10] It's been chasing that tail plenty enough.
[4708.10 → 4716.48] It almost reminds me of running two or three different note systems all at the same time and knowing deep down that Evernote isn't the right long-term solution.
[4716.50 → 4716.78] Damn it, Alex.
[4716.78 → 4718.86] Sticking with it for years and years and years.
[4719.02 → 4719.74] God, it burns.
[4719.96 → 4720.28] It burns.
[4721.02 → 4721.90] Two fingers, though.
[4722.42 → 4726.82] It doesn't know about you two, but Plex was the gateway drug that got me into self-hosting in the first place.
[4727.20 → 4730.40] Plex is the reason that I'm sat here speaking to you right now.
[4730.48 → 4734.74] So I have a soft spot for it, despite their behaviour this year.
[4734.74 → 4737.90] So remaking Eden comes in with 20,000.
[4738.00 → 4742.20] That's just a quick keeping the shirt on Chris's back boost.
[4742.44 → 4743.42] Well, that's nice.
[4743.48 → 4743.80] It's true.
[4744.36 → 4751.52] Also, I wanted to quickly mention that the Music Assistant has come leaps and bounds in the last few months since I tried it.
[4751.86 → 4754.92] It really does seem like the Sonos killer I always wanted.
[4755.32 → 4759.72] I use whatever speakers I want with all the music services I could possibly want.
[4760.28 → 4763.96] And the piece of resistance is that it has a lovely UI.
[4763.96 → 4766.96] It's still in beta, but it is getting very close.
[4767.78 → 4769.36] What is this Music Assistant that he's talking about?
[4769.40 → 4770.58] Is this something built into Home Assistant?
[4771.00 → 4772.80] No, but it should be, right?
[4772.92 → 4774.58] When I heard that, I thought the same thing.
[4775.24 → 4776.20] Wouldn't that be great?
[4776.58 → 4779.64] But no, I don't think it's officially built in, but it is.
[4779.78 → 4784.86] It's just, you know, it's like a plugin or an add-on or whatever for Home Assistant, I believe.
[4785.20 → 4785.44] Cool.
[4785.66 → 4791.62] Yeah, I actually dug out an old Chromecast audio that I found in the bottom of a box to power my garage speakers this week.
[4791.62 → 4799.68] So I would love some better way from it because casting from iOS doesn't allow you to put it as part of an AirPlay group.
[4799.88 → 4800.86] And I just want the whole house.
[4800.92 → 4806.78] Sometimes when you're tidying out, like the whole house, you just want the whole house pumping with the same tune sometimes, you know?
[4807.00 → 4807.02] Yeah.
[4807.76 → 4808.00] Yeah.
[4808.00 → 4814.78] So if you have that integrated, like if you have your HomePods connected to your Home Assistant, you could potentially use this to send out media.
[4814.94 → 4815.64] This is great.
[4815.78 → 4816.36] A great idea.
[4816.52 → 4817.10] It's party mode.
[4817.18 → 4818.38] I want a party mode button.
[4818.50 → 4818.82] Yes.
[4819.52 → 4820.38] Party automation.
[4822.24 → 4823.30] Thank you, Remaking Eden.
[4823.36 → 4824.72] I will check that out in the downtime.
[4825.72 → 4827.68] Tom's dad comes in with a Space balls boost.
[4827.80 → 4830.24] One, two, three, four, five SATs using the index.
[4830.34 → 4832.20] I have that same combination on my luggage.
[4832.38 → 4833.20] Ah, genius.
[4833.20 → 4835.98] You put out a call for a thermostat solution.
[4836.26 → 4836.70] I did.
[4837.12 → 4839.48] He says, here's my thermostat Home Assistant setup.
[4840.00 → 4843.20] I have a four zone hot water baseboard system.
[4843.82 → 4847.18] Buying four smart thermostats was a non-starter.
[4847.82 → 4852.24] This was the use case that tipped me into home automation and using Home Assistant.
[4852.70 → 4859.12] The hardware consists of a single board Son off four channel pro, which is an ESP32 plus for relays.
[4859.12 → 4863.36] The relays control the zone values just as the traditional thermostats would.
[4863.92 → 4869.38] This runs four instances of ESP Home thermostat module, all connected to Home Assistant.
[4869.94 → 4876.16] The temperature sensing is done with a $4 Naomi temperature sensor with custom firmware scattered around the house.
[4876.66 → 4884.10] I then have another ESP32 that is picking up Bluetooth from Naomi's devices, sending back to Home Assistant over MQTT.
[4884.10 → 4888.20] I was originally worried about all the moving parts for such a critical function.
[4888.40 → 4894.38] However, after two years in service, I've only recently had problems with the Bluetooth bridge stopping.
[4894.94 → 4897.58] If I had an automation that just restarts it, things are better.
[4898.00 → 4898.88] Thanks for the great show.
[4899.22 → 4907.36] I've thought about doing this a few times because, you know, like $100 to $150 per thermostat, of which I've now somehow got three in my house.
[4907.36 → 4915.64] Because it's not an insignificant amount of money, but I just worry about the interlocks and how that would be handled in the ESP firmware.
[4916.10 → 4925.60] I'm sure it's very easily done with code, but it scares me that I could accidentally run the cool at the same time as the hot, for example,
[4925.76 → 4931.16] and cause damage to very expensive equipment in the attic for the sake of a $100 thermostat.
[4931.32 → 4931.34] Right.
[4931.48 → 4933.00] That's a great point.
[4933.00 → 4936.82] Yeah, I would be really keen to hear what people have done about that.
[4937.68 → 4945.08] I could absolutely see a situation where I'm accidentally running the furnace and the air conditioner at the same time if they both activated somehow.
[4945.64 → 4945.74] Right.
[4945.74 → 4956.50] I know for sure that my automations around just basic stuff like lighting and garage doors opening and stuff have certain edge cases every once in a while that I missed.
[4956.68 → 4959.76] And the last thing I want is for my heat to do the same thing.
[4960.00 → 4960.34] Oh, yeah.
[4960.52 → 4960.92] Absolutely.
[4961.52 → 4961.88] Yes.
[4962.54 → 4965.80] Although I blast the furnace and the AC very rarely.
[4966.46 → 4968.04] Well, I mean, it depends on the time of year.
[4968.68 → 4972.46] Also, Darwin came in with 3,200 SATs on his setup.
[4972.54 → 4973.50] We'll put that in the boost barn.
[4973.50 → 4982.28] And then we got 5,833 from Iraq on how he controls his Fujitsu mini splits with an IR blaster using Home Assistant.
[4982.80 → 4985.04] I had a lot of feedback about this one in particular.
[4985.46 → 4990.26] There is a project called Smart IR, and I've been able to hook it up using a Broad link.
[4990.62 → 4994.52] I think it's a RM4 mini or pro or something like that.
[4994.92 → 4996.92] I've been able to hook that up using Smart IR.
[4996.92 → 5002.78] And then it has a bunch of pre-configured IR codes for all the different remotes built into it.
[5002.96 → 5007.26] So in Home Assistant now, I've got a – it's not a two-way connection.
[5007.50 → 5010.94] So, like, the infrared system doesn't know the current state of the air conditioner.
[5010.94 → 5021.26] So if I change the temperature using the physical remote in the garage versus the Home Assistant front page, the two are out of sync and it causes a problem.
[5021.46 → 5029.58] Because when you send an infrared command with this thing, it sends the entire state of the remote through infrared every single time.
[5029.72 → 5031.38] So it says, fan at this speed.
[5031.38 → 5036.06] I want you to be this temperature in this mode with Vane in this particular mode.
[5036.42 → 5037.60] So there must be –
[5037.60 → 5038.04] Just blasting the IR.
[5038.36 → 5042.14] There must be thousands of codes in this remote for every single possible permutation.
[5042.38 → 5043.84] But that's how it goes.
[5044.42 → 5044.60] Hmm.
[5044.90 → 5045.18] Okay.
[5045.86 → 5047.76] Gene Bean comes in with a row of ducks.
[5048.06 → 5048.48] Hey, Alex.
[5048.52 → 5052.36] I really liked how you structured your Nix flake, and I'm glad you mentioned it here.
[5052.64 → 5054.68] I'm taking inspiration to improve mine.
[5054.92 → 5055.04] Oh.
[5055.48 → 5059.04] Gene Bean reached out to me this week and said this on – I think it was Discord.
[5059.04 → 5060.06] We were in a little chat.
[5060.06 → 5062.04] And such a nice chap.
[5062.24 → 5065.58] But I feel like such a noob when it comes to Nix.
[5065.62 → 5070.64] I was considering submitting a talk for Nixon USA because it's at the same time as Scale, and I'm going to be there.
[5070.72 → 5072.84] But I'm like, who am I to talk about Nix?
[5072.98 → 5073.52] I mean, I don't know.
[5073.66 → 5074.78] I don't know anything about Nix.
[5075.00 → 5075.52] I don't know.
[5075.88 → 5076.56] Keep going.
[5076.66 → 5077.16] Just roll it.
[5077.30 → 5079.28] I mean, next year you'll be even better.
[5079.44 → 5080.42] The year after that you'll be even better.
[5080.74 → 5081.88] Get that rolling.
[5082.10 → 5087.56] I'm going to very much encourage you to do that talk, Alex, because I think you come at it from a different angle than many folks.
[5087.56 → 5095.00] And if I learned anything at the last few NixOS meetups I've attended in Berlin, everybody has their own way.
[5095.28 → 5099.42] And there's not necessarily a perfectly right way or a perfectly wrong way.
[5099.84 → 5100.54] That's the problem.
[5100.66 → 5108.20] Because it's – when you try and look up for a specific solution to solve a specific problem, sometimes I just want the answer.
[5108.20 → 5114.40] I don't want the entire works of Chaucer explaining to me why eight people did it nine different ways, you know?
[5114.80 → 5115.54] Yeah, that's true.
[5115.90 → 5118.90] Although I still want you to do it because then maybe you could do it at Linux Fest too.
[5119.36 → 5121.04] And I think we need some Nix talks at Linux Fest.
[5121.08 → 5123.60] You know, the spring is filling up fast.
[5123.74 → 5125.88] We've got Scale and Nixon in March.
[5126.06 → 5128.46] Then we've got Texas Linux Fest and the solar eclipse.
[5128.64 → 5132.56] And there's also a track day in Austin that I'm considering driving the golf over for.
[5132.78 → 5133.64] Oh, yeah, yeah.
[5133.64 → 5135.90] Two weeks after that is Linux Fest Northwest.
[5136.26 → 5138.54] It's going to be a busy spring, I tell you.
[5139.00 → 5141.04] Yeah, but then you can rest for the rest of the year.
[5141.18 → 5143.94] I might hit my first FOSDEM to this year.
[5144.44 → 5145.46] Yeah, that would be pretty sweet.
[5145.54 → 5146.20] So that's February.
[5146.44 → 5148.24] We've also got JB meetups coming.
[5148.32 → 5154.08] So keep an eye on meetup.com slash Jupyter Broadcasting for where in the world Brent Nerva is going to be this week.
[5155.48 → 5156.54] Okay, here's the last one.
[5156.56 → 5157.12] It's a tough one.
[5157.20 → 5158.34] It's a tough one from Scuffed1.
[5158.88 → 5160.98] Scuffed writes in 10,000 SATs.
[5160.98 → 5164.28] It's all this talk about switching from Plex to Jellyfin.
[5164.62 → 5166.08] But what about old Envy, guys?
[5166.74 → 5169.16] I bought a Lifetime Pass, and then they did the rug pull.
[5169.44 → 5171.08] So F those guys.
[5171.56 → 5171.96] All right.
[5172.24 → 5172.74] All right.
[5172.84 → 5173.08] Wow.
[5173.72 → 5174.12] Okay.
[5174.74 → 5177.52] Yeah, I kind of just tapped in after the whole split.
[5177.82 → 5179.22] And I've always gone with the Jellyfin route.
[5179.58 → 5181.40] Thank you, everybody who boosted in.
[5181.54 → 5182.54] Really appreciate it.
[5182.58 → 5183.32] This was a whopper.
[5183.42 → 5184.60] And we hope you had a great holiday.
[5185.02 → 5186.64] We had eight boosters across 10 boosts.
[5186.64 → 5188.22] Not everything made into the show for time.
[5188.22 → 5191.10] But we do put that in the boost barn, which is linked in the show notes.
[5191.52 → 5193.20] We made 83,600 SATs.
[5193.26 → 5193.98] Thank you very much.
[5193.98 → 5199.36] Everybody who supports this production, either by a boost or by becoming an SRE.
[5199.82 → 5200.20] Yes.
[5200.48 → 5206.22] Site Reliability Engineer for this here show at self-hosted. Show slash SRE.
[5206.44 → 5209.76] You get the show directly, ad free, and a little bonus content.
[5209.90 → 5211.10] You get a post show as well.
[5211.78 → 5212.58] Really appreciate it.
[5212.68 → 5214.54] Thank you, everybody who does support the show directly.
[5215.34 → 5215.84] Stay tuned.
[5215.84 → 5218.10] Brent has a very special post show topic.
[5218.48 → 5218.86] I sure do.
[5219.00 → 5219.10] Yeah.
[5219.66 → 5222.84] If you're still listening at this point, it's a bumper holiday episode.
[5223.04 → 5224.40] Thank you very much for listening, everybody.
[5225.14 → 5227.16] You can go to self-hosted. Show slash contact.
[5227.30 → 5228.74] That's the place to go to get in touch with us.
[5228.90 → 5231.76] And you can find me at alex.ktz.me.
[5232.14 → 5234.56] I'll do it on Weapon X at Chris LAS.
[5235.04 → 5237.88] I think you could probably find me on that Linux Unplugged.
[5238.10 → 5238.54] There you go.
[5239.08 → 5239.86] LinuxUnplugged.com.
[5239.98 → 5241.34] As always, thanks for listening, everybody.
[5241.50 → 5244.06] That was self-hosted. Show slash 113.
[5245.84 → 5264.56] Thanks for listening.
