[0.00 → 2.32] Well, I'm pretty excited because I get to geek out this week.
[2.46 → 6.98] Matt from Adventurous Way, a YouTube channel that Alex and I watch, is joining us.
[7.14 → 11.02] And Matt, you've got a ton of videos about RV travel, automation, self-hosting.
[11.16 → 17.16] And just recently, you and the wife bought 40 acres of raw land in central Vermont
[17.16 → 22.56] and are starting the long work of building a smart home from the ground up.
[22.64 → 23.54] Matt, welcome to the show.
[23.94 → 24.86] Thank you so much for having me.
[25.32 → 26.12] Are you crazy?
[26.12 → 30.94] I watch your videos, and it looks like years of work ahead of you.
[31.96 → 32.56] It really is.
[32.62 → 35.70] Yeah, this is the start of a pretty long journey.
[35.84 → 38.62] I think we are just at the very beginning of it.
[38.86 → 42.12] And yeah, I think we are probably a little bit crazy.
[42.96 → 46.10] I'm sure you've noticed, Chris, that I've managed to coerce another Brit onto the shows.
[46.22 → 50.20] I wanted to bring the average, you know, raise the standard a bit.
[50.54 → 51.56] Yeah, it wasn't lost on me.
[51.68 → 53.28] It wasn't lost on me at all.
[53.28 → 57.06] But, you know, Alex, there's like a ton of stuff we could talk to Matt about.
[57.18 → 59.76] But I thought maybe we'd start with what he and I have in common.
[60.18 → 65.14] When I first started watching your channel, you were doing a smart RV system similar to mine.
[65.26 → 67.60] Home Assistant, Victory, the whole work.
[67.74 → 69.94] So can you walk us through a little bit of what you built?
[70.46 → 74.54] Yeah, so we've been living full-time in our RV now for about three years.
[74.54 → 83.58] We moved out of a perfectly good four bedroom home in the Bay Area, California, and into a 180 square foot box on wheels.
[84.36 → 89.30] So imagine about half the size of the average like master bedroom in the US.
[89.56 → 92.10] And that's been our entire home for the last three years.
[92.10 → 96.28] And so pretty quickly, we realized that we're both technologists.
[96.48 → 100.98] My partner and I are both former software engineers and tech people.
[101.58 → 107.20] We kind of realized there's an opportunity here to use technology to make ourselves more comfortable.
[107.66 → 110.52] And that was really where this whole journey began.
[110.52 → 117.32] And so what started off as just like a hobby, it's pretty hard to have hobbies when you live in such a small space.
[117.32 → 121.30] If they're physical, we obviously don't have a backyard to go and do gardening.
[121.30 → 123.50] And I've given up my woodworking shop and things.
[123.72 → 126.64] So we really focused on digital hobbies.
[127.24 → 133.18] And so although I've been into some elements of self-hosting and tech for many, many years,
[133.84 → 139.06] this for me really was an opportunity to go deep into tech.
[139.06 → 141.82] And the home automation side of things.
[142.46 → 148.58] So starting almost three years ago, I had a Raspberry Pi and I loaded Home Assistant onto it.
[148.80 → 150.40] And that was kind of where I started.
[151.20 → 157.46] And within a matter of weeks, I was already overwhelming the Raspberry Pi.
[157.76 → 160.18] It must have been a Model 3, I guess, back then.
[161.34 → 163.44] Completely overwhelming what it was able to do.
[164.20 → 167.60] And I was like, I think it's time for an upgrade.
[167.60 → 172.04] Again, space, big concern for us here, as you know, living in an RV.
[172.68 → 173.96] And power draw as well, right?
[174.02 → 175.08] And that's the nice thing about the Pi.
[175.48 → 175.84] Yeah.
[175.98 → 179.14] And so the Pi was great because it could run off the DC voltage.
[179.42 → 181.90] And that was something that I wanted to stick with.
[182.16 → 185.92] So we upgraded to an 8th gen Intel NUC.
[185.92 → 188.12] It runs an i3 processor.
[189.02 → 201.40] And because it runs, I think it's like 19 volts that it actually runs on, I was able to avoid using the normal AC power brick and instead run it straight off DC using a DC boost converter.
[201.40 → 206.50] That has been running flawlessly now for almost three years, 24-7.
[206.88 → 207.50] Ah, nice.
[208.24 → 209.96] It's interesting you say that, Matt.
[210.12 → 217.02] I think a few years ago, maybe five plus, Plex was the gateway drug for a lot of people that got them into self-hosting.
[217.54 → 219.10] I know you're a proponent of that as well.
[219.90 → 221.98] Home Assistant is the new gateway drug, don't you think?
[221.98 → 223.56] I think it is.
[223.80 → 228.60] And it's literally the hub of the entire experience in our RV.
[229.26 → 232.82] It is even when we're consuming media, I've got Plex plugged into Home Assistant.
[233.26 → 237.02] And so it really is that kind of entrance point for me.
[237.40 → 247.44] But I think it's becoming so accessible and so easy to get up and running with that it's just attracting more and more people to this kind of lifestyle and this hobby.
[248.04 → 249.64] Well, I have a ton of questions for you, Matt.
[249.64 → 252.58] And in fact, I want to get into some of the details about your system.
[252.66 → 255.22] But I want to mention this episode is brought to you by a Cloud Guru.
[255.34 → 258.32] They are the leader in learning for Cloud, Linux, and other modern tech skills.
[258.76 → 261.00] Hundreds of courses and thousands of hands-on labs.
[261.32 → 261.74] Get certified.
[262.04 → 262.36] Get hired.
[262.58 → 265.08] Get learning at a CloudGuru.com.
[265.56 → 274.80] Matt, something you said there was that it was what struck you was, well, we could use some of this technology to make life more comfortable in our tiny home.
[275.36 → 276.92] That's kind of how I got into it, too.
[276.92 → 279.60] And I'm curious, what was some of your very first automations?
[279.76 → 281.74] Was it around enabling boon docking?
[281.94 → 282.64] Was it around heating?
[282.78 → 283.40] Where did you start?
[283.84 → 283.98] Yeah.
[284.06 → 288.04] So for us, the scarcity of resources was one of our biggest challenges.
[288.94 → 291.80] Much like you, we have battle-borne lithium batteries.
[292.10 → 292.96] We have solar.
[293.66 → 294.82] But they're still finite.
[295.38 → 298.90] In three years on the road, we do not and have never owned a generator.
[299.52 → 302.74] So one of my big first priorities was how do I get power?
[302.74 → 306.82] We prefer to boondock rather than stay in RV parks.
[307.46 → 310.82] I think start of last year, we did 100 days in a row of boon docking.
[311.18 → 312.26] Just totally off-grid.
[312.64 → 312.96] Wow.
[313.24 → 313.90] 100 days.
[313.96 → 314.70] That's impressive.
[314.86 → 315.52] Very nice.
[315.60 → 315.70] Yeah.
[315.76 → 316.00] Wow.
[316.08 → 322.60] So when the pandemic first hit, we were just every 10 to 14 days, we would run into town to go and dump our tanks and fill up again.
[322.60 → 325.86] And then back out into the middle of nowhere and carry on.
[326.16 → 326.72] Oh, look at you.
[326.78 → 327.52] You big show off.
[327.52 → 334.24] So one of the priorities with the home automation was how do I make this more achievable?
[335.28 → 343.62] And for me, I've never got into the scripts so much, just the trigger a thing and then things happen all at once.
[343.84 → 350.78] I was always into how can I make the RV smarter in the first place, so I don't have to interact with it at all.
[350.78 → 357.28] So one of my favourites, I call it the auto dump feature and has nothing to do with dumping tanks.
[358.06 → 359.54] This is all about electricity.
[360.14 → 364.28] And the idea is to say, let's say it's a sunny day outside.
[365.12 → 366.16] It's spring.
[366.42 → 367.02] I'm in the desert.
[367.28 → 369.32] I've got plenty of solar coming in.
[370.04 → 371.78] At some point, my battery is going to fill up.
[372.22 → 374.02] So what do I do with that excess?
[374.28 → 375.28] How can I use it?
[375.28 → 385.80] So I set up an automation that as the batteries reached higher and higher voltage levels and higher and higher percent charge, it would begin to turn on or enable certain devices.
[386.72 → 392.04] So as you've probably noticed, the Victory inverter has a fairly high background power draw.
[392.30 → 394.96] And so we keep it turned off most of the time.
[395.62 → 399.52] Once the batteries reach 80%, I would turn the inverter on automatically.
[399.52 → 406.20] Once the batteries reach 90%, it would switch the fridge over from propane to AC electric.
[407.10 → 412.24] And once the batteries reach 95%, it would switch the electric water heater on.
[412.86 → 423.18] So on a good sunny day, without us doing anything at all, we would end the day with full batteries, a full tank of hot water, and having saved some propane from the fridge.
[423.72 → 424.40] I love that.
[424.58 → 425.36] That's so great.
[425.48 → 426.38] And that's really cool.
[426.38 → 432.58] You must be then going through and replacing those basic DC switches that came with the RV with something smarter.
[432.98 → 437.48] One of the challenges in the RV is nothing is designed for RVs in the smart world.
[438.02 → 440.66] So we don't use a lot of 110 volts.
[441.10 → 442.48] DC is king.
[443.04 → 448.42] And so the Son off SV has been my choice for a lot of this and a couple of the other Son off devices.
[448.70 → 451.26] The 4chan Pro has been another one I've used.
[451.26 → 456.58] And then a couple of things are running on Son off.
[456.72 → 462.00] I think it's the POW R2, the energy monitoring hardwired one, or the Son off S31.
[462.92 → 465.08] And those have really been the heart of it.
[465.32 → 471.60] I started off with TRIMOTOR running on those and then switched over to ESP Home a little while later.
[471.94 → 473.62] I actually use one of those Son off SVs.
[473.70 → 475.28] I'm holding it up to the camera for you both.
[475.28 → 477.50] For my garage doors.
[477.78 → 479.82] And yeah, it's worked absolutely flawlessly.
[479.92 → 481.00] It's got a little relay on it.
[481.24 → 483.26] It runs on low voltage, like you said, Matt.
[484.02 → 484.96] I really like it.
[485.00 → 486.84] I put TRIMOTOR on mine, of course.
[487.98 → 488.94] Fantastic little board.
[488.94 → 498.52] And then it sounds like another key piece of insight that's coming into Home Assistant is you are making Home Assistant aware of your electrical system.
[498.62 → 502.10] Sounds like battery state, power generation from solar.
[502.84 → 506.36] So Home Assistant must be getting a lot of information off of your Victory setup.
[506.52 → 508.72] How are you supplying that to Home Assistant?
[509.08 → 509.62] Yeah, you're right.
[509.62 → 519.36] So we are using the Victory CCGX, the Colour Control GO, which is one of their family of products that has a built-in MQTT broker.
[520.08 → 529.76] So this is actually one of the original reasons, I guess, that we chose Victory versus some of the other vendors out there that do solar for RVs.
[530.26 → 538.62] We basically slurp up all of that MQTT data, throw it into Home Assistant, and also then collect it all in InfluxDB as well.
[538.62 → 544.20] And for me, it was actually the data collection side of things that was really why I started this in the first place.
[544.60 → 551.10] We wanted to see the long-term trends of our batteries, of our solar, all these sorts of things.
[551.84 → 562.66] And we've now got, I think, almost three years' worth of data at about a one to ten second resolution across dozens and dozens and dozens of data points on the electrical system.
[562.66 → 567.88] So you're getting real insights to how the health of your batteries are, if they're still delivering the same way.
[568.04 → 573.36] And probably even, like, you could start to see maybe something's wrong with one of our solar panels because of this data.
[573.76 → 574.16] Exactly.
[574.16 → 582.36] So we've used it ourselves to answer questions like, if we added 200 more watts of solar, what would that do to our system?
[582.98 → 586.86] Or how many watts of solar do we need to get through winter at a given latitude?
[586.86 → 593.80] Because we can graph the location of the RV versus the amount of power that we bring in during the day.
[594.44 → 594.92] I love this.
[594.98 → 599.72] You've got to come on board as a road trip consultant for me, you know, running operations.
[599.72 → 600.20] Yeah.
[600.84 → 603.86] So a lot of the stuff that we've done in that sense has been quite selfish.
[604.12 → 607.30] It's informed decisions that we've made ourselves.
[608.40 → 613.38] But I think one of the things that's really excited me the most is being able to share this data with others.
[613.78 → 620.08] So we've actually shared all of our electrical data with Battle born, who make our batteries, with Dennis, the CEO.
[620.08 → 627.52] And he's then able to look at that data and from that get real-world insight into how their batteries actually perform in the wild.
[627.52 → 637.52] Because no lab can recreate an RV in temperature fluctuations and casually turning on the AC and then boon docking for...
[638.16 → 638.86] A hundred days.
[639.32 → 639.70] Exactly.
[640.10 → 642.18] So we've been able to share all that data with them.
[642.40 → 649.20] And that really helps them to then understand how their batteries perform in different conditions and hopefully then improve their products.
[649.20 → 653.66] Yeah, I could show them how their batteries perform while they're cooking because it's so dang hot here.
[653.78 → 662.34] But something else that strikes me is that you could do is you could watch for the total draw of the RV and prevent tripping a breaker when you're set up to shore power.
[662.44 → 665.88] And you're actually maybe not boon docking, but you're at an RV park or something like that.
[665.92 → 668.36] So there are utilities for when you're not off-grid as well, I would imagine.
[668.82 → 672.74] We actually added that exact automation about 10 months ago.
[673.00 → 674.32] We arrived here in Vermont.
[674.32 → 677.72] We had full hookups, and we knew we were going to be here during the winter.
[678.32 → 688.60] And we're only in a 30-amp RV, which means that our main breaker in the RV can only handle 30 amps, which means it's really, really easy for us to trip that breaker.
[688.76 → 698.72] If we ran an electric water heater, an electric space heater, if we then happened to turn on the microwave or electric kettle or something else, that would trip the breaker.
[698.72 → 713.70] So I was able to use a home assistant automation to look at what I'd set the Victory system to allow as the input current, so 30 amps usually, and then deduct from that whatever the current total power draw was.
[713.70 → 735.68] And then if I was exceeding the 30 amps, it would then automatically pause either the electric water heater or the electric space heater so that I can run the microwave or run the electric kettle, because I need my cup of tea, and pause those things until the microwave or the kettle has shut off and then take them back to their original state.
[735.86 → 738.90] And thanks to that, we didn't trip a breaker all winter long.
[738.90 → 750.86] So, Matt, are you telling me that my Colour Control GO is collecting all the information I need, and I just need to go into the settings and tell it an MQTT endpoint or something?
[751.06 → 752.50] Do I already have it?
[752.62 → 753.64] It's even simpler than that.
[753.72 → 756.18] It actually has a built-in MQTT broker.
[756.34 → 756.64] No!
[757.18 → 763.82] So you can just connect to it on port 1883 and pull the data straight off.
[764.02 → 765.36] You're doing it right now, aren't you, Chris?
[765.40 → 765.80] Be honest.
[765.80 → 771.54] I just don't understand why nobody's built a Victory integration for Home Assistant.
[771.86 → 773.26] Like, get on it, somebody.
[773.44 → 774.68] So I actually looked at doing it.
[774.80 → 781.44] I posted on the Victory forums late last year and said I'd be really interested in making a Victory integration.
[781.78 → 783.32] That was probably your forum post I read.
[783.94 → 785.40] I just, I don't know Python.
[785.98 → 794.90] And so for me, like, there's a decent barrier to entry to go straight from, like, not knowing a language to writing an integration with this massive kind of project.
[794.90 → 797.48] But yeah, I mean, all the data's there on MQTT.
[797.92 → 808.06] It feels like this is a great example of if you had somebody who was a Python developer and had a Victory system, it would be pretty, it wouldn't take long until we had an integration.
[808.26 → 811.40] But it's just those two paths have not yet crossed.
[811.64 → 817.90] But these Victory systems are crazy popular in van builds, bus builds, modern RVs.
[817.90 → 821.24] RVs, like, this is going to be, these things are going everywhere.
[821.52 → 822.96] And Victory makes some great stuff.
[823.32 → 823.78] They really do.
[823.92 → 829.34] And one of the things that I like the most about Victory is they are open sourcing nearly all of their software.
[829.90 → 834.32] So all the APIs they use are all completely publicly documented.
[834.54 → 836.76] But all the source code is also there as well.
[836.88 → 837.30] Hell yeah.
[837.30 → 838.68] And you'll like this one.
[839.24 → 848.80] They've even got a literal how-to guide on GitHub along with all the software you need to run the CCGX software on a Raspberry Pi.
[849.16 → 850.20] Yeah, I really like that.
[850.22 → 853.62] I know some of their boxes internally are running Linux, too, which I think is just great.
[854.18 → 855.58] I'm a huge fan of that as well.
[855.86 → 859.16] We should reach out to Victory and have them on the show.
[859.62 → 860.04] We should.
[860.14 → 860.42] You're right.
[860.42 → 864.42] I should give them enough publicity on there for heck's sake.
[865.32 → 866.02] But yeah.
[866.36 → 866.68] All right.
[866.72 → 867.06] Well, yeah.
[867.12 → 871.66] So I am setting up MQTT and pointing it at my Clorox right now.
[872.02 → 875.88] So I'm going to get that going.
[876.46 → 881.38] Top tip, if you want to, my favourite MQTT kind of tool is something called MQTT Explorer.
[881.72 → 882.38] Ah, OK.
[882.58 → 886.64] This thing lets you log into a broker and see all the messages that it's getting in real time.
[886.98 → 889.34] Oh, and is, I see, it's a Mac app.
[889.34 → 890.28] Is that a Mac app?
[890.96 → 894.22] Brew install MQTT-explorer, I think.
[894.58 → 895.16] No kidding.
[895.46 → 895.72] Really?
[895.88 → 896.08] OK.
[896.32 → 900.60] You can actually, so you can use Brew to install practically everything these days.
[901.08 → 904.12] When I set this, I got an M1 Mac about a month ago.
[904.84 → 914.50] And I've religiously used Brew for absolutely everything, including Chrome, VS Code, Audacity, everything.
[914.80 → 914.92] Yeah.
[915.12 → 916.58] I legitimately had no idea.
[916.72 → 917.10] No, I know.
[917.10 → 920.36] It's come a really, really long way in the last five years or so.
[920.92 → 921.06] Yeah.
[921.16 → 926.54] You know, I have to say, you know, my Mac experiment here on the road trip has been, it's been good.
[926.54 → 936.72] I mean, once I got, and Matt, I don't know if you've ever run into this, but I had this problem where like NS URL session D just would consume all of my bandwidth.
[936.72 → 939.22] Because I was in a pretty crappy signal area.
[939.22 → 942.22] And I had like hardly any signal.
[942.22 → 948.22] And I'd fire up the Mac, and it would just sit there and run and run and run in part because the download speeds were slow.
[948.30 → 948.98] So it took longer.
[948.98 → 950.82] And I'm sitting there trying to do a live show.
[952.90 → 953.72] It's just horrible.
[953.98 → 959.28] So once everybody yelled at me to try Little Snitch out again, which I had tried out a hundred years ago.
[959.70 → 966.84] I gave Little Snitch a go and set up an outbound firewall for, you know, and blocked basically everything except for the apps I'm using to do the shows.
[966.84 → 968.60] It's been pretty solid since then.
[969.10 → 971.30] Seemed a little hacky, but sure works.
[971.62 → 971.70] Yeah.
[971.70 → 983.04] There's a load of little tricks like that you can use when you're on a really constrained bandwidth situation just to make sure that your devices are only doing the things you really, really want them to do.
[983.14 → 985.94] And not just those like background tasks that can wait.
[986.22 → 989.24] Are you doing any of that at the firewall level now?
[989.24 → 992.20] The big one for us is actually just the ad blocker.
[992.28 → 995.72] Just having AdGuard Home on there just cuts out so much stuff.
[995.88 → 1003.34] I will say we are completely spoiled having been running on like bonded cellular connections for the past kind of a couple of years.
[1003.78 → 1008.38] We actually have cable internet plugged into the side of our RV.
[1008.68 → 1011.46] So we're sitting on 400 Meg cable internet right now.
[1012.02 → 1012.16] Nice.
[1012.30 → 1013.10] Yeah, that's a treat.
[1013.42 → 1013.56] Yeah.
[1013.56 → 1019.48] Yeah, the one nice thing about this spot we are in Tucson right now is we have pretty dang good signal.
[1019.64 → 1023.56] It's not like that good, but you know, it's not wired good, but it's been pretty good.
[1023.80 → 1028.50] So that's been nice because some points on this trip I have just had horrendously bad signal.
[1029.48 → 1031.60] It's amazing what you can actually still get done.
[1032.00 → 1041.52] We actually found that in all our time kind of boon docking around the southwest, I think it was only one spot we ended up in where we didn't have usable cellular internet.
[1041.52 → 1043.34] And we sort of knew that going into it.
[1043.38 → 1046.80] So we just made sure that all the work we had to do, we didn't need anything online.
[1047.56 → 1057.50] But a big part of living in the RV is you find all of these challenges, I think, a lot quicker than when you live in a house.
[1057.72 → 1058.10] No kidding.
[1058.46 → 1058.60] Yeah.
[1058.78 → 1063.86] And a good one for us is when I want to update our website, let's say I've got a new Docker container I want to push.
[1064.68 → 1070.04] If you're sitting in an office, you think nothing of going Docker push and uploading that image.
[1070.04 → 1071.02] Of course, right.
[1071.02 → 1079.46] I spent a long time optimizing hours so that it was pushing just the tiniest little delta of that layer at the top that had to change.
[1079.86 → 1082.18] And it was otherwise as static as possible.
[1082.56 → 1084.14] And all these little things you find.
[1084.52 → 1085.20] That's a great point.
[1085.38 → 1089.68] It's like, boy, sometimes updating Docker images takes freaking forever over cellular.
[1089.96 → 1092.00] Like, it's clearly not many people doing that.
[1092.80 → 1095.22] Hey, Alex, hot, hot update here.
[1095.22 → 1100.88] It looks like MQTT Explorer is available for Linux as an app image and a snap.
[1101.24 → 1105.40] So you can get it on GNU slash Linux and a Mac and the App Store and a DMG.
[1105.56 → 1106.38] And, of course, on Windows.
[1106.38 → 1115.40] I think I've spent more time nodding and smiling and looking impressed in the last 20 minutes than I have in the last 20 months.
[1115.76 → 1118.04] Some seriously, seriously cool stuff.
[1118.12 → 1126.38] I wonder how much we could apply to people's houses and make people more cognizant of the energy they're using and maybe make that into some kind of sustainable movement.
[1126.38 → 1126.98] Movement.
[1127.88 → 1128.88] Fascinating.
[1129.04 → 1131.98] So what's your favourite automation that you've done?
[1132.76 → 1137.70] The unrippable breaker has probably been the most impactful day to day.
[1138.06 → 1147.94] One of the ones that was so simple yet made a huge difference to our quality of life was we have a GPS dongle that we have plugged into the Victory CCGX,
[1148.18 → 1152.18] which means the Victory system is aware of the trailer's location at any point in time.
[1152.18 → 1158.62] It can use that for some geo-fencing and things through the Victory software, through their dashboard.
[1159.72 → 1165.30] But once you then plug that GPS dongle in, it's then also exposing its data on the NQTT broker,
[1165.56 → 1173.94] which means I can then collect that data with Node. RED and Home Assistant, about maybe 18 months or so ago, I guess,
[1174.52 → 1180.08] added a new service allowing you to set the home location through the Home Assistant API.
[1180.08 → 1185.94] So then as we're driving down the road, every 60 seconds, Node. RED will ping Home Assistant and say,
[1186.38 → 1187.50] oh, by the way, we're now here.
[1188.04 → 1191.76] And that way, as we cross time zones or state borders or whatever,
[1192.52 → 1194.70] Home Assistant always has our latest information.
[1195.70 → 1197.90] Schedules based on time all continue to work.
[1198.62 → 1201.06] Yeah, that was a real simple one, but really worked well.
[1201.64 → 1204.36] I know that's a problem you've been trying to solve, Chris, for some time now.
[1204.74 → 1205.56] Yeah, it's so silly.
[1205.56 → 1212.64] Here I am in Tucson right now, and my evening automation for lighting is based on the sunset in the Pacific Northwest.
[1213.22 → 1216.22] And I used to go in there and update it, but I just kind of stopped.
[1216.28 → 1217.52] I just kind of said, ah, screw it.
[1217.54 → 1218.56] I'm done updating it.
[1218.62 → 1219.34] It's close enough.
[1219.42 → 1220.58] It's about an hour off.
[1222.78 → 1224.24] So I should totally look into that.
[1225.94 → 1227.82] Linode.com slash SSH.
[1227.90 → 1232.56] Go there to get $100 in 60-day credit on your account and go there to support this show.
[1232.56 → 1234.72] You know, Linde started in 2003.
[1234.84 → 1238.98] It's one of the very first companies in cloud computing before we called it cloud computing.
[1239.18 → 1242.70] And now, 18 years later, they haven't launched a trillion different services.
[1242.86 → 1245.68] They've remained focused on building out their core service.
[1245.96 → 1251.50] Not only do they have the best servers in the business with incredible performance, fast networking, 11 data centres around the world,
[1251.50 → 1260.42] but they've added services that matter, things that impact the quality of your life, like DDoS protection, VLAN support, a powerful DNS manager,
[1260.82 → 1266.00] and, of course, block storage and S3-compatible object storage, which I absolutely love.
[1266.36 → 1270.92] But I know there's people, you know, like Alex, who like things like the Terraform support and the Kubernetes support.
[1271.74 → 1272.42] Yeah, yeah, yeah.
[1272.44 → 1274.16] I'm sure that's great for some of you out there.
[1274.34 → 1275.12] So shoot me.
[1275.12 → 1284.70] But what I like about Linde is they have really just remained focused on building something really great for those of us who want something fast and reliable.
[1285.02 → 1289.92] And then they back that with the best customer support in the business, phone, ticket, email, even social.
[1290.02 → 1291.06] They're going to take care of you.
[1291.44 → 1293.02] And there are tons of one-click deployments.
[1293.12 → 1296.22] If you just want to get started with something, that can be a great way to learn.
[1296.60 → 1299.96] You can also just DIY, which is often the way I prefer to go.
[1299.96 → 1306.78] Or sometimes they'll do something in the middle where I'll deploy a base system that has just the runtime for the container information.
[1306.94 → 1309.48] I'll install all that junk that you'd normally have to set up.
[1309.58 → 1311.06] And it has the right repos.
[1311.16 → 1313.62] You're getting the right versions of the packages and the GPG keys.
[1313.92 → 1315.34] And then we'll just build on top of that.
[1315.58 → 1318.14] And that takes like, I don't know, eight seconds to deploy.
[1318.26 → 1319.10] It's pretty fast.
[1319.14 → 1319.76] It's pretty amazing.
[1320.20 → 1322.48] So go over to linode.com slash SSH.
[1322.56 → 1323.64] Get that $100.
[1324.10 → 1326.36] Support the show and see what we've been talking about.
[1326.36 → 1330.12] Every time we're working on a project, we'll try something out on Linde real quick.
[1330.82 → 1332.38] It's a great way to R&D stuff.
[1332.60 → 1334.78] And, you know, that $100 can help you do that as well.
[1335.16 → 1336.48] So you've got to go check it out for yourself.
[1336.60 → 1340.70] Take advantage of that $100 and see why Linde is better than the rest.
[1340.78 → 1343.62] There are a lot of choices out there, but nobody does it like Linde.
[1344.00 → 1346.12] Linode.com slash SSH.
[1348.66 → 1349.28] Right then.
[1349.38 → 1356.08] So the ultimate conclusion of self-hosting, at least in my opinion, is probably to self-build, you know, a house.
[1356.36 → 1358.00] Or somewhere you're going to live, right?
[1358.84 → 1364.08] Tell us a little bit about your plans, Matt, for the 40 acres in Vermont that you've just bought.
[1364.70 → 1364.98] Yes.
[1365.14 → 1369.96] So I am, like you, sort of Brit here in the US.
[1370.28 → 1374.56] And as we've been travelling around the US, we've been looking for where we might want to live one day.
[1375.14 → 1380.40] We don't have family in the US, so we're really free to kind of choose wherever it is we want to live.
[1380.40 → 1383.74] And we have spent a lot of time in a lot of different places.
[1383.84 → 1386.60] We've eventually settled on Vermont as a place.
[1387.52 → 1396.98] So about two or three months ago, we closed our sale or our purchase on 40 acres of completely raw land in central Vermont.
[1397.86 → 1401.88] And when I say raw land, this is literally like trees and dirt.
[1402.14 → 1403.30] There really is nothing there.
[1403.30 → 1404.66] It's a hill with some trees on it.
[1404.84 → 1405.90] You know, you can say it.
[1405.90 → 1406.86] You can be honest.
[1407.30 → 1408.70] It's a hill with some trees on it.
[1409.74 → 1410.70] It really is.
[1410.90 → 1412.34] And there is not a lot there.
[1412.64 → 1416.14] But when we went into this, we had some very specific requirements of what we wanted.
[1416.74 → 1418.58] We didn't want to be in a city or a town.
[1418.66 → 1419.92] We wanted to be somewhere more rural.
[1419.92 → 1426.52] And one of the things that made that requirement a little bit more challenging is we said a must-have is fibre internet.
[1427.12 → 1433.54] So even though we're in the middle of nowhere in central Vermont, we will have 800 Meg symmetric fibre to the property.
[1434.08 → 1434.48] You bastard.
[1434.92 → 1436.02] Good for you, man.
[1436.20 → 1436.90] Nicely done.
[1438.06 → 1439.48] In the woods with fibre?
[1439.62 → 1440.26] Yes, please.
[1440.76 → 1441.08] Yeah.
[1441.24 → 1443.68] So we are now at the start of this journey.
[1443.98 → 1446.24] Last week, we had our driveway put in.
[1446.24 → 1453.40] We're building the house site about 1,000 feet back from the road, and building that driveway was just beyond what Diana and I could possibly take on.
[1453.84 → 1454.10] I don't know.
[1454.16 → 1455.46] I've been watching your videos, dude.
[1455.56 → 1459.12] You have been felling trees like a proper lumberjack.
[1459.42 → 1460.74] It's really impressive.
[1461.36 → 1463.18] There are a lot of new skills that we're picking up.
[1463.52 → 1475.88] It's kind of surreal to, like today, I was out there with a chainsaw working on the property and then came home writing a blog post, compiling some stuff and working on some programming and some automations and things.
[1475.88 → 1480.38] It's a very surreal kind of contrast, I guess, between the two things.
[1480.74 → 1482.16] What a cool existence there, huh?
[1482.50 → 1483.60] Yeah, we have a lot of fun doing it.
[1483.96 → 1490.82] And how great that you have the RV there with you with all this stuff kind of done and now taking care of itself so you can focus on other stuff.
[1491.10 → 1491.74] Yeah, exactly.
[1491.96 → 1502.38] And in many ways, this house that we want to build, it should probably go without saying that we want to have a load of smart technology in there and things and obviously self-host a lot of things inside there.
[1502.38 → 1508.38] The RV in many ways has been our test lab and still continues to be our test lab for a lot of those things.
[1508.88 → 1520.48] So even though we're running with just like one little Intel NUC and could serve that all with like a little travel router and would probably be fine in here, we sort of push the boundaries to learn some of the things we might need for the house.
[1521.06 → 1521.90] The RV is staging.
[1522.32 → 1523.34] It basically is, yeah.
[1523.34 → 1529.22] I'm sure you're already daydreaming of ideas for the new house, but this is something you get to build from scratch.
[1529.34 → 1532.32] So I imagine you're thinking Ethernet throughout.
[1532.54 → 1535.04] You're already picturing a spot where you'll probably run a server.
[1535.18 → 1540.90] Walk us through a little bit of what you're now considering that you got a crack to build something from scratch, even if it is a bit off.
[1541.34 → 1542.40] I'm learning so much.
[1542.46 → 1547.24] And I think the community around the self-hosted Discord and things has been a fantastic resource already.
[1547.24 → 1551.20] As I learn more, I keep evolving my plans.
[1551.44 → 1564.40] But some of the things that I've picked up so far are things like if you want to run your own hardware, there's usually a tradeoff of like heat and noise and cost and power efficiency in these things.
[1565.06 → 1568.12] We've learned so much about resource management in the RV.
[1568.28 → 1570.20] We want to have a completely net-zero house.
[1570.20 → 1581.64] We're trying to build a passive house and hit the living building challenge, which are a set of requirements that basically mean a very, very high quality, sustainable, comfortable home.
[1582.08 → 1586.10] How do I now then host servers and things within that is kind of the challenge.
[1586.84 → 1593.54] So one of the things that we're going to do because we're self-building, the priority is to get utilities onto the property.
[1593.54 → 1603.96] So electricity and fibre, bring those up the driveway, make sure we've got our solar and our batteries installed, bring the well truck up and dig a well, all those sorts of things.
[1604.28 → 1606.16] I love that water came after internet.
[1606.50 → 1607.46] I noticed that too.
[1608.04 → 1612.92] Someone asked us a few days ago if we had a phone line at the property, and I'm like, I have no idea.
[1613.12 → 1613.98] I have never checked.
[1614.94 → 1616.50] No, why would you?
[1616.64 → 1618.36] Yeah, it's gone now.
[1618.36 → 1625.54] But no, so because we need to bring those things on and get them done quickly, most people would put those in a basement.
[1626.28 → 1629.12] But to have a basement implies you already got a house and we don't.
[1629.66 → 1645.24] So we're actually going to build a separate standalone mechanical building, bring all the utilities into there, which gives us this big advantage that we've then got a separate building where noise and environmental controls can be tailored to whatever we want inside.
[1645.24 → 1649.12] And that's where we're going to run all of our servers and switches and all that kind of stuff.
[1649.26 → 1651.20] And it can be as loud as it wants to be.
[1651.84 → 1652.52] It doesn't matter.
[1652.90 → 1654.96] We can then have a separate building for that.
[1655.58 → 1655.60] Right.
[1655.64 → 1657.14] With an Ethernet cable going to the house.
[1657.66 → 1664.40] So that's where you're going to put all your solar batteries and inverters and electric grid tie off points.
[1665.22 → 1665.66] Exactly.
[1666.26 → 1668.28] So it'll have as much power as it needs.
[1668.28 → 1675.78] We're thinking because the property is quite large, the distances between some of the buildings could also therefore be quite large.
[1676.08 → 1679.02] For example, we want to run cameras along the driveway.
[1679.56 → 1682.34] We're sort of pushing the limits of what Ethernet can do.
[1682.58 → 1693.90] So we're then probably going to run fibre as a backbone between the buildings and run fibre from the road to the house site and then our own fibres back down to the road and then tap in there.
[1694.46 → 1694.94] Might as well.
[1694.94 → 1700.90] And at this stage, and if you're building this property in 2021, actually fibre does seem like a pretty smart way to go.
[1700.98 → 1702.12] It sort of future proofs it a bit.
[1702.54 → 1703.06] Yeah, exactly.
[1703.34 → 1706.58] And it's one of those things where we have a YouTube channel.
[1706.92 → 1709.54] We're moving around big media files all the time.
[1710.52 → 1716.60] And so having an ability to do that at greater than one gig speed is something that we would actually really find valuable.
[1717.26 → 1718.94] Can I rent some space in your mech room?
[1720.88 → 1721.06] Yeah.
[1721.34 → 1722.92] Forest data centre, Colo hosting.
[1723.02 → 1723.80] I can see it now.
[1723.80 → 1725.76] Vermont Rural, yeah.
[1726.00 → 1726.22] Yeah.
[1726.32 → 1727.64] What did we coin it on Discord?
[1727.84 → 1729.80] VT Rural, like AWS do.
[1731.76 → 1732.72] That's pretty great.
[1733.30 → 1738.76] That sounds like almost exactly, although at a larger scale and distance than what I had vision.
[1738.76 → 1749.12] My ultimate goal for RV Lady Joop's would be to park her on a piece of property that we've bought with a shed that has solar.
[1749.32 → 1749.98] It has the inverter.
[1750.10 → 1750.80] It has the batteries.
[1751.64 → 1753.04] Maybe it has a washer and dryer in it.
[1753.04 → 1761.28] And it has some on-premises servers that have been, you know, theoretically syncing over Starlink or something with media ready to go or whatever.
[1761.60 → 1766.16] And I love the idea of separating out the noisy stuff into its own building.
[1766.38 → 1767.52] I mean, why not?
[1767.60 → 1769.84] That's such a great way to go.
[1769.84 → 1774.22] And so I imagine you're considering a whole new generation of home assistant build.
[1774.30 → 1775.82] You're not going to take the one out of the RV.
[1775.96 → 1776.80] You're going to leave that.
[1776.92 → 1778.62] And I would imagine a whole new build.
[1779.02 → 1779.18] Yeah.
[1779.40 → 1782.30] And this is an area now that I'm learning so much about.
[1782.40 → 1786.90] The hardware side of running servers is pretty new to me.
[1786.90 → 1798.14] And so although I'm comfortable, like, with the concepts, the specifics of exactly what to run is all new, but you actually touch on something there that's a real challenge that I'm battling with.
[1798.42 → 1802.72] The concept of self-hosting is that you have your own little private island of stuff.
[1803.42 → 1807.52] It doesn't matter what goes on elsewhere, out in the cloud or whatever.
[1808.12 → 1811.60] You are insulated from that because you have your own little private island.
[1812.26 → 1816.26] Well, when we have a house, we sort of then have two islands.
[1816.26 → 1817.00] Mm-hmm.
[1817.36 → 1819.36] You have things like take Plex as an example.
[1819.82 → 1824.70] Do I run Plex in the house, in the RV, both?
[1825.02 → 1827.22] Like, how do I sort of manage those things?
[1827.54 → 1827.74] Right.
[1828.02 → 1828.38] In there.
[1828.56 → 1828.86] Yes.
[1829.16 → 1829.40] Yeah.
[1829.70 → 1832.58] So that's an area for me that's, I think, really exciting.
[1833.00 → 1835.36] There are some places where it's a huge asset, like backups.
[1835.64 → 1835.84] Great.
[1836.06 → 1837.92] I've now got a really easy way to do that.
[1838.22 → 1841.46] But for things like media sharing, do I have two copies?
[1841.90 → 1843.06] It becomes tricky.
[1843.06 → 1867.24] And then there's the angle as well of, for you in particular, I think this will be a unique challenge, is when you are driving around in your RV for potentially six months, and you're leaving the rural pad empty for six months, you want to make sure that that stuff is reliable and has decent redundancy and all that kind of stuff.
[1867.24 → 1873.70] And I think one of the things that I've heard you struggling with, you sort of brought up on the Discord, is how good is good enough?
[1873.82 → 1875.80] And do I need to have dual power supplies?
[1876.18 → 1883.38] And, you know, how many SSDs do I need to put in RAID to make sure that that doesn't, you know, kick things over and that kind of thing?
[1883.38 → 1885.16] So there's a lot to consider.
[1885.72 → 1889.70] And I'll add to that, Alex, you know, lesson learned here.
[1889.78 → 1891.46] I thought I had a fairly good setup.
[1891.88 → 1903.16] And as I'm on the road at this point, my main server at the studio is offline, which does a ton of lifting for me and then syncs the results to the RV.
[1903.16 → 1909.22] And I feel like I'm, like, operating with one hand tied behind my back while that server's down.
[1909.28 → 1912.82] And now I'm running through my head of, like, what am I going to do to rebuild that?
[1912.86 → 1914.62] Because it really, it is a tricky problem.
[1914.62 → 1919.52] And this is on, you know, a pretty nice actual server box.
[1920.24 → 1921.70] It's a nice little box.
[1922.14 → 1930.50] See, the thing is, I don't think we really fully admit to ourselves just how much light tinkering we do on the average week to these servers to keep them tended,
[1930.50 → 1937.14] to keep the, you know, the leaves in the correct space, you know, to coin a gardening kind of analogy, you know?
[1937.68 → 1942.10] I probably SSH into my server just out of habit, well, at least once or twice a day.
[1942.20 → 1943.62] I don't really know why sometimes.
[1943.68 → 1944.20] I just do.
[1945.90 → 1948.54] Yeah, I mean, you touched on it there with the dual Plus.
[1948.54 → 1954.38] And I would just say, imagine the situation where you don't have physical access to your server,
[1954.62 → 1958.14] nor would anybody else have physical access to your server for three months.
[1958.14 → 1963.46] How do you give yourself the best chance of being okay and everything working?
[1963.82 → 1969.44] I've gone through exactly this week, because as you both know, I'm going back to England at the weekend.
[1970.14 → 1972.46] It will be probably the day after this airs, actually.
[1972.88 → 1981.78] And the server that lives in England, for me, has been running on an old super micro board with a Java-based PMI KVM built in.
[1982.32 → 1985.88] Works okay, but I prefer it was a little more modern, that kind of stuff.
[1985.88 → 1991.84] And I thought to myself, could I just make do by taking in a Raspberry Pi 4 over there and put Pi KVM on it?
[1991.96 → 1999.68] And I'm like, no, actually, I need this to be 100% as close as is possible, reliable.
[2000.16 → 2007.20] Because the last thing I want to do is have to call my dad up and say, hey, can you go and push this widget into this particular orifice?
[2007.20 → 2012.82] And, you know, wave your hands at three o'clock on Sunday, you know, and make it work.
[2013.64 → 2019.72] So I've bought a new AS Rock board, which I've written a blog post about, which I'll put a link to in the show notes.
[2020.08 → 2023.46] I think that might be the perfect media server motherboard for me moving forward.
[2023.78 → 2024.30] We'll see.
[2024.88 → 2027.42] But there's just so much to consider.
[2027.42 → 2034.82] And I think you have to get to a point where you're like, okay, I'm willing to risk a single power supply in this system.
[2034.94 → 2038.90] If that goes boom, okay, what's my plan B?
[2039.24 → 2046.66] You know, my plan B might be Linde, something like that, with some ZFS datasets replicated or something like that.
[2047.20 → 2053.10] It's too bad about the Pi KVM, though, because that was one of my thoughts, was if I had Pi KVM at the studio,
[2053.10 → 2055.48] I could at least see what's going on the console right now.
[2056.10 → 2058.22] But really, an PMI system would be better.
[2058.80 → 2066.30] I was actually thinking, although I don't really know how to pull it off, is like a redundant Pi KVM system or a redundant Pi system for WireGuard.
[2067.22 → 2073.06] When I'm back, when I do get back to Washington, addressing that redundancy is one of my to-do items.
[2073.24 → 2075.10] Because I know exactly what you mean, Matt.
[2075.14 → 2079.20] It's like I'm sort of helpless down here in Tucson when the server's up in Seattle.
[2079.20 → 2084.48] Yeah, I mean, one of the technologies I've been researching and playing with some more recently is Karp.
[2085.28 → 2093.50] So this gives you essentially the ability to have two devices that can fight between themselves, let's say, for an IP address on the network.
[2094.20 → 2096.16] So Open Sense supports this out of the box.
[2096.26 → 2098.96] You can run two separate machines with Open Sense on.
[2099.64 → 2104.00] And if one of them dies, the other will automatically kind of pickup and run with that.
[2104.68 → 2108.34] And maybe there's a similar thing you can do with Raspberry Pis with other services.
[2108.34 → 2112.36] So you can have essentially a redundant Raspberry Pi sitting there idle.
[2112.86 → 2118.86] And if the first one drops off the network for any reason or just doesn't respond, the second one would pick up.
[2119.18 → 2122.54] But you've got this vision of two fish flopping around on the deck fighting each other.
[2125.22 → 2125.66] Right?
[2126.88 → 2127.74] It might be fun.
[2127.86 → 2128.76] That could be good to watch.
[2129.44 → 2135.62] Well, Matt, there are so many things we could talk about, but we should probably leave some of it for your YouTube channel.
[2135.62 → 2139.12] But thank you for coming on the show today and chatting with us about some of this.
[2139.24 → 2143.92] And best of luck to you and the wife building your new home.
[2144.08 → 2145.62] I think it's going to be quite the project to watch.
[2145.74 → 2146.20] Thank you so much.
[2146.28 → 2146.42] Yeah.
[2146.46 → 2148.48] And I'm looking forward to learning a lot more.
[2148.62 → 2152.22] And I've been binging all the podcasts recently.
[2152.34 → 2156.12] So over the last three and a half weeks, I've just got through all 50-something episodes.
[2156.12 → 2160.24] I'm looking forward to learning a lot more from the group and the Discord as well.
[2160.58 → 2160.80] Yes.
[2160.88 → 2161.94] Good plug for the Discord there.
[2162.04 → 2163.68] Self-hosted. Show slash Discord.
[2164.04 → 2164.64] You can go over there.
[2164.70 → 2167.62] Also, if you want to give us an email, there's self-hosted. Show slash contact.
[2168.04 → 2172.52] And if you want to find more of Matt, you can go and search on YouTube for Adventurous Way.
[2173.00 → 2179.50] And we'll have a link to Matt's YouTube channel in the show notes as well as Instagram and other things like that.
[2179.50 → 2181.10] Big thanks for listening, everybody.
[2181.58 → 2187.46] Huge thanks, actually, to our site reliability engineers over at self-hosted. Show slash SRE.
[2188.36 → 2190.48] Loads of you have been buying the Chris and the Badger t-shirts.
[2190.62 → 2192.32] I think we're going to be taking those down soon.
[2192.70 → 2194.12] Uh-oh, better go get them soon.
[2194.48 → 2199.08] Do feel free to go over there and give those a quick once-over before they've gone for good.
[2199.38 → 2201.44] Yep, that's at jupytergarage.com.
[2201.54 → 2204.28] And also, go check out our friends at A Cloud Guru.
[2204.28 → 2210.12] They have a course on setting up, learning, configuring, and managing Linux web services.
[2210.60 → 2212.46] Apache, Nginx, and Squid.
[2212.60 → 2217.94] Yeah, reverse proxy servers as well as HTTPS, SSL stuff, load balancing, all of that goodness.
[2218.50 → 2219.92] Linux web services with the Cloud Guru.
[2220.08 → 2223.00] We'll have a link in the show notes, or you can find them at a cloudguru.com.
[2223.14 → 2224.52] You can find Alex on Twitter.
[2224.62 → 2225.76] He's at Ironic Badger.
[2225.86 → 2226.90] I'm at Chris LES.
[2227.02 → 2229.54] And the show, the whole show, it's at Self Hosted Show.
[2229.84 → 2230.94] A big thanks for listening, everybody.
[2230.94 → 2233.56] That was self-hosted. Show slash 53.
[2234.28 → 2236.04] 중纸
