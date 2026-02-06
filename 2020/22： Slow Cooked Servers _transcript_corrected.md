[0.00 → 3.02] Coming up on Self-Hosted, I'm slow cooking some servers.
[3.42 → 8.38] Alex has self-hosted some AI with a nasty gotcha and a damp basement.
[8.74 → 9.14] I'm Chris.
[9.56 → 10.08] And I'm Alex.
[10.26 → 11.82] And this is Self-Hosted 22.
[13.32 → 16.02] I've got a £13 brisket in my fridge.
[16.34 → 19.56] The only man I know who has hooked his barbecue up to Home Assistant.
[19.92 → 20.94] Almost, almost.
[21.08 → 23.74] So I bought a Signals billow or something.
[24.38 → 26.26] Now they make a couple of products.
[26.26 → 31.04] And I wanted to try and get this particular one hooked up to Home Assistant.
[31.38 → 35.18] They have another more expensive model, which does work with Home Assistant.
[35.78 → 42.88] And so this one, I tried to decompile the APK and reverse engineer the Firebase database calls that it's making.
[43.40 → 44.26] But no luck.
[44.42 → 45.32] I haven't been able to get it working.
[45.62 → 49.36] So I just have to cope with using their crappy app, which is fine.
[49.96 → 50.48] No, it's no good.
[50.52 → 52.66] But this needs to be an obvious priority, clearly.
[52.66 → 57.00] We need to have you set everything else aside and get this working.
[57.84 → 58.78] There's no other option.
[59.24 → 59.82] It's really nice.
[60.00 → 67.86] So when you want to cook a big piece of meat in this, in the Amado Joe, you have to, you know, temperature is everything when you're coming to barbecue.
[68.70 → 72.38] And keeping a nice stable temperature to get that lovely smoky flavour.
[72.54 → 73.48] That's really important.
[73.82 → 75.60] I had lessons from Carl, you know.
[75.88 → 77.10] So, you know, it's important.
[77.50 → 78.30] You know, we'll get to this.
[78.36 → 82.04] But that's what I'm doing is I'm just slow cooking my raspberry pies in the RV.
[82.04 → 82.48] I'm not.
[82.90 → 84.86] It's not a thermal getaway issue.
[85.00 → 87.16] It's a slow cooking plan.
[87.30 → 88.24] I don't know what you're talking about.
[88.70 → 90.38] Ooh, could you use them to do sous vide?
[91.56 → 92.84] You absolutely could.
[92.90 → 97.96] You just put some meat in a bag in my server booth and let it go.
[97.96 → 103.64] So that is unless I have to deploy my current fix, which I'll tell you about shortly.
[104.12 → 115.34] But one of the things I did for this road trip that I'm on down here in Texas, enjoying myself some barbecue myself, was shut down my Shinobi home camera system.
[115.34 → 117.58] So I have no recordings right now.
[117.62 → 121.14] Everything's just streaming into the wind, I guess.
[121.78 → 128.26] And before I fire things back up, I think you may be changing my mind on what software I go with.
[128.54 → 132.76] Because while Shinobi did the job, I kind of had issues with it over time.
[133.14 → 134.00] I'd have to reboot.
[134.00 → 139.80] And for those of you not familiar, Shinobi is a closed circuit capturing application.
[139.96 → 140.74] It's a web-based app.
[140.80 → 147.78] It's a little strange to use, but it gives you an ability to pull in all these RTSP feeds and camera feeds into a single application.
[148.28 → 149.52] I have a sense, Alex.
[149.72 → 150.48] I have a sense.
[150.66 → 151.68] You may have found something better.
[151.68 → 159.28] I was watching a video by The Hookup YouTube channel, and he really piqued my interest in Blue Iris.
[159.76 → 162.46] Now, Blue Iris is paid software.
[162.64 → 164.64] It's $75 for a proper license.
[165.28 → 167.48] So I'll just get that out the way up front.
[167.78 → 170.02] You know, it's not free like Shinobi in terms of cost.
[170.44 → 171.36] But it is self-hosted.
[171.74 → 173.98] It is self-hosted, but it's not open source either.
[174.10 → 175.68] So, you know, there are a couple of trade-offs to make.
[176.16 → 178.74] It's running fully offline, fully on my LAN.
[178.74 → 182.36] You know, it's a local NVR software.
[183.32 → 191.00] And what really piqued my interest was he set up artificial intelligence motion detection.
[191.76 → 191.78] Really?
[192.02 → 194.22] Now, this is super cool.
[194.58 → 195.50] AI motion detection.
[195.58 → 202.12] In other words, the software is aware of what's in the picture, and it's using image recognition to make that determination?
[202.70 → 203.08] Correct.
[203.38 → 207.32] So when I first watched the video, I thought, there's no way this is all local.
[207.32 → 216.68] He must be leveraging some kind of cloud API, sending these photos off, you know, to who knows where, and I'm not interested.
[216.94 → 220.58] But then I watched the video and realized that he was using Deep Stack AI.
[221.12 → 225.86] And Deep Stack, you can run in a container on your LAN.
[225.86 → 234.20] And so what this thing does is you submit a JPEG to it, and then it will apply its, what do you call it?
[234.26 → 235.42] I don't know what, uh...
[235.42 → 236.94] Object recognition?
[237.08 → 245.72] Because from what I could see in there, it seems like it can determine the difference between faces, dogs, all kinds of common objects that would be in a camera feed.
[245.72 → 256.18] There is a list of objects it can detect, and, you know, a short list of useful ones is stuff like car, truck, bus, person, dog, bear, that kind of thing.
[256.42 → 256.48] Bear.
[257.76 → 258.86] Bear is on the list.
[259.46 → 261.36] That's good up in the Pacific Northwest, trust me.
[261.44 → 262.12] It's just funny.
[262.76 → 265.00] And so I thought, oh, this is going to be really hard to get working.
[265.32 → 266.12] But I'll give it a stab.
[266.18 → 268.46] I'll set aside an evening, and I'll get going.
[268.46 → 278.46] So JDM, who was on the last episode, you know, the serverbuilds.net guy, he hooked me up with one of those HP Z...
[279.20 → 281.42] I can't remember the model name.
[281.80 → 282.74] A HP box, anyway.
[282.94 → 284.22] And it cost me about $100.
[285.12 → 287.42] And in this thing, it has a dual-core seller on.
[288.56 → 292.54] And most importantly, it supports Intel Quick Sync.
[292.54 → 303.84] So this $90 x86 system with 12 gigabytes of RAM, and I bought a very cheap NVMe SSD that's like 60 gigs to put in there,
[303.86 → 306.96] so it was not booting off the spinning rust drive it shipped with.
[307.76 → 312.54] I have an NVR system now that can support five cameras for $90.
[313.22 → 314.54] Whoa, and how much storage?
[315.18 → 317.22] Like, how long can you keep the footage with this?
[317.66 → 318.60] Did you have to add disk?
[318.66 → 319.84] Are you using the network storage?
[319.94 → 320.90] How is that part working?
[320.90 → 326.62] I have a USB 4 terabyte hard drive that's been sat in a drawer for about three years,
[326.84 → 329.28] and I thought, well, I may as well use it for something useful.
[329.56 → 332.74] So I've just literally plugged in a USB hard drive into this desktop system.
[333.06 → 335.70] There is room inside for a three and a half inch hard drive,
[335.82 → 341.28] so I was kind of tempted to go and buy an easy store and throw it in there, but use what you got, right?
[341.72 → 345.38] Yeah, especially for something like this, and then you could always build on it later.
[346.02 → 347.36] While we're talking about storage,
[347.36 → 352.52] one of the things that impressed me when I was digging around and learning a little bit about Blue Iris
[352.52 → 356.36] and the hookups videos, he also mentions this,
[356.90 → 361.96] it would seem that if your camera supports it, you can do two types of video storage.
[361.96 → 369.70] A low resolution, maybe 15 frames a second, 640 by, you know, 480 or whatever,
[369.78 → 373.46] some really low res video that you can store indefinitely forever.
[373.76 → 374.74] You have that.
[375.02 → 381.78] But then when the AI detection kicks in, and it notices something that is recognized,
[381.78 → 389.22] it will flip over and keep a 4K copy or whatever your cameras support of that particular moment in time.
[389.52 → 393.50] So your stuff that has the action is in full glorious resolution,
[393.50 → 398.76] and then your keep forever stuff is lower resolution and lower frame rate.
[399.12 → 401.10] Is that how you are using it with this box?
[401.60 → 402.26] Yeah, pretty much.
[402.32 → 403.52] They're called substreams.
[403.52 → 406.86] So, you know, I have a 4K camera pointing at my driveway.
[407.46 → 410.12] There's no reason to record 4K 24-7.
[410.24 → 413.04] That's just honestly stupid and a waste of energy.
[413.36 → 420.08] But these cameras have hardware chips in them which do the video encoding in real time.
[420.34 → 422.58] So you actually get two streams out of this camera.
[422.68 → 423.72] You get the 4K stream.
[423.88 → 429.44] It can be either H.264 or H.265, which is great for file size.
[429.44 → 434.58] And then you get a second substream as well, which again comes out in H.264 or H.265,
[435.04 → 436.40] depending on what you set up.
[436.76 → 441.52] And the resolution, as you say, of the substream, the second stream, is much, much lower.
[442.14 → 445.30] So the SD stream, which is what we'll call the low-res stream,
[445.80 → 448.40] the SD stream is running pretty much all the time.
[448.54 → 450.16] It has motion detection turned on.
[450.22 → 452.34] So that's what's looking for motion in the frame.
[453.16 → 455.16] So what happens is motion is detected.
[455.16 → 461.24] It takes a JPEG still of that frame, sends that to the AI detection software.
[462.04 → 463.60] There are three pieces of software at work here.
[463.64 → 468.44] You've got Blue Iris, you've got AI Motion, and then you've got Deep Stack.
[468.70 → 470.84] So Deep Stack is what does the image processing.
[471.74 → 478.56] AI Motion is what reacts to the JPEGs coming in and sends the images off to Deep Stack.
[479.24 → 483.72] And then obviously Blue Iris is the CCTV NVR software.
[483.72 → 491.56] So AI Motion, which is a small app, which was written by someone in the IP Cam Talk forums.
[491.66 → 493.56] I think his name is Gentle Pumpkin.
[494.68 → 499.68] This app, you configure what you want the Deep Stack AI to be looking for.
[499.76 → 501.86] So, you know, cars, bears, trucks, etc.
[501.86 → 513.68] And then once it detects a certain type of object in the frame, it will then, and only then, tell your cameras to record the HD feed.
[514.08 → 518.86] And you can set a pre-record buffer of 5, 10, 30 seconds if you want to.
[519.22 → 523.60] So if you were sat there thinking, oh, well, maybe it takes a bit of time for the images to process.
[523.60 → 526.96] Am I not going to lose in the time it takes for that to happen?
[527.10 → 529.12] Am I not going to lose the pizza guy coming down my driveway?
[529.84 → 533.80] No, you won't because you get the pre-record, and it's all fine, and it all just works.
[534.02 → 536.64] You know, that's the amazing thing about it is it just works.
[536.92 → 545.04] So one of the big things I missed after moving away from Nest when I moved into this house earlier this year was, you know,
[545.06 → 549.66] that really super simple interface of just swiping back through the timeline to see events and stuff like that.
[549.66 → 552.64] And with Blue Iris, I have that again now.
[552.92 → 553.88] And it's great.
[554.00 → 554.80] I've really missed it.
[555.18 → 563.56] Yeah, there are a couple of cool modes for capturing stuff, including what looks like a really nice UI for reviewing those motion events pretty efficiently.
[563.76 → 564.44] Have you found that?
[564.92 → 565.36] Okay.
[566.00 → 570.32] I downloaded an app on my iPad that has been the best way to do that kind of stuff.
[570.74 → 575.62] But one of the better bits of Blue Iris is that it has a web interface.
[575.62 → 583.34] So I can just log into, you know, IP address of HP server, colon, port, whatever, and bring up the web interface.
[583.48 → 589.20] And I have access through WireGuard to my LAN, of course, so I can just connect through a WireGuard tunnel and do it that way wherever I am.
[589.84 → 591.12] That works really nicely.
[591.60 → 595.30] But I do have a bit of a confession to make about Blue Iris, Chris.
[596.42 → 597.46] It only runs on Windows.
[598.20 → 598.78] Wait a minute.
[598.84 → 602.00] But doesn't the Deep Stack stuff run in a container on Linux?
[602.22 → 602.80] It does.
[603.26 → 604.60] It's a Windows-Linux mix?
[604.60 → 605.04] Yes.
[606.18 → 606.42] Yep.
[606.62 → 611.72] Boy, I don't know if I want to deploy Windows just for that, but at the same time, it does look significantly better than Shinobi.
[611.86 → 615.72] That's, would you say maybe its biggest downside for those that don't run it?
[615.84 → 616.92] I mean, I don't know.
[617.26 → 618.52] Some people, that it's not a big deal.
[619.00 → 620.98] For sure, I'd say it's the biggest downside, yeah.
[620.98 → 635.60] The reason I ended up going that route in the end was because you want direct hardware support for things like Quick Sync to make the video transcoding and stuff like that, you know, not too CPU intensive.
[635.60 → 638.62] You're going to have a dedicated box for it anyway.
[639.32 → 641.40] Let's say I wanted to put it on my server in the basement.
[641.76 → 651.08] I would have either needed to buy a dedicated graphics card and pass that through to the Windows VM so that that can do the transcoding using NVN call or whatever.
[651.08 → 658.62] Or I would need to buy a more modern CPU and put that in my server because I have some old Eons that don't have Quick Sync.
[659.00 → 662.68] Or I can spend 90 bucks, put Windows on this thing and just forget about it.
[662.96 → 663.18] Yeah.
[663.36 → 664.16] You did Windows 10?
[664.16 → 670.36] I have an old Windows 8 product key that I bought back in like 2013 or something.
[671.02 → 673.24] And I just typed that in thinking this ain't going to work.
[673.36 → 673.72] And it did.
[673.96 → 676.76] So, you know, I've got Windows 10 Pro for free.
[677.30 → 679.46] I was getting pretty hyped, but that is a bummer.
[679.88 → 680.06] Yeah.
[680.12 → 680.74] Sorry about that.
[681.02 → 682.54] Do you think Deep Stack would work with Shinobi?
[683.04 → 685.54] Deep Stack will work with anything that is a JPEG.
[685.76 → 689.32] So all you need to feed to Deep Stack is an image.
[690.10 → 691.18] Doesn't really matter what.
[691.54 → 692.94] The problem is the rest of Shinobi.
[692.94 → 694.58] I don't mean any disrespect.
[694.84 → 696.32] It's a good app.
[696.52 → 703.40] But I just, yeah, when it came time to reduce thermal load in the server booth, I thought, yeah, this is one that has to go.
[703.60 → 706.90] Well, there are a couple of others that perhaps you should try out, you know, in the interest of science.
[707.40 → 709.38] There's Motion Eye and Zone Minder.
[709.80 → 710.96] Yeah, I have looked at them.
[711.78 → 715.22] I definitely need to give Motion Eye another fair shake.
[716.08 → 721.04] Zone Minder, I'm less impressed with, but maybe it's improved recently.
[721.48 → 721.72] Yeah.
[721.72 → 728.22] I mean, the worst thing about running Windows is that it's Windows, and I don't really like running it anywhere.
[728.44 → 734.44] And I don't mean to come across as, you know, a typical Linux kind of, you know, four legs good, two legs bad sort of guy.
[734.68 → 739.08] But I just don't feel the need to run it anywhere.
[739.08 → 744.84] But that said, if I'm throwing it in a closet and forgetting about it the whole time, does it really matter?
[745.10 → 745.54] Probably not.
[745.90 → 746.42] Probably not.
[746.58 → 746.74] No.
[746.74 → 759.16] And if you were in the commercial space out in the, you know, real world at businesses running CCTV systems, if they weren't appliances running Linux, they would be applications running on Windows boxes.
[759.16 → 761.28] So you do see some of it out there in the real world.
[761.70 → 765.94] Yeah, there's nothing really better in the small to medium NVR space, in my opinion.
[765.94 → 767.84] And yes, there's the Unify thing.
[767.92 → 776.54] But again, that's a proprietary ecosystem that you need to have their cloud key dream machine, whatever they're calling it this week, that's super expensive.
[776.54 → 779.52] And the prices of their cameras are outrageous.
[780.30 → 783.14] They might be good quality, but they are super-duper expensive.
[783.14 → 787.58] So, you know, 70 bucks for Blue Iris supports up to 64 cameras.
[788.22 → 790.64] And for me, obviously, I'm, you know, I'm only in a house.
[790.72 → 794.54] I'm not going to get anywhere much, much above 10, you know, and that's pushing it really.
[795.18 → 801.50] You know, I bought one of those doorbells we had Morgan review a couple of weeks ago, but I bought the Easy Vis branded version of it.
[801.82 → 804.56] Must say, the picture quality is fantastic on this thing.
[804.88 → 808.46] And it plugged into Blue Iris, no problem with the RTSP feed.
[808.60 → 810.48] So another vote for that doorbell.
[811.00 → 811.28] Really?
[811.28 → 814.66] So who needs a ring when you can get an Easy Vis, huh?
[814.92 → 825.08] Well, an Easy Vis with a 24-7 Windows box talking to a 24-7 Linux box running an artificial intelligence model to decode your images.
[825.32 → 831.08] Apart from that, that's what we're all about here, right, is taking something that is a commercial offering and enrolling it yourself.
[831.22 → 839.42] And in this case, you bought a commercial app to do it, but you're still able to run it locally on premises, which I think is, when it comes to video camera footage, it's just so critical.
[839.42 → 843.66] So I'm trading my time and effort for my data and convenience.
[844.18 → 848.28] Yes, but this in particular is visual data of activities around your home.
[848.76 → 858.44] And that to me, I'll tell you, when I'm walking around in my house in the buck naked, it crosses my mind when I see a camera out of the corner of my mind.
[858.48 → 862.06] I think to myself, man, I'm really glad that's not cloud connected right now.
[864.10 → 865.60] Ain't no one got to see that.
[865.88 → 866.38] Yeah, right.
[866.38 → 866.78] Exactly.
[867.44 → 868.82] Just go ahead and delete that footage.
[869.54 → 873.28] So Easy Vis is the maker of the doorbell you got, and that does RTSP.
[873.38 → 879.50] So you could, in theory, pull that into Home Assistant as well if you just wanted a Lovelace card just showing you the front door.
[879.94 → 882.80] Yep, I can pull it into Lovelace, and I do.
[882.96 → 883.54] It works great.
[883.82 → 887.34] The camera is like a weird, like, fisheye lens thing.
[887.34 → 889.66] So that's kind of a trip getting used to that.
[889.78 → 891.38] But, I mean, that's no big deal.
[891.70 → 896.08] At least I can see whether there are packages on my porch now without actually having to go and physically look.
[896.48 → 896.54] Yeah.
[896.70 → 903.64] And it sounds silly, but when you're travelling like I am right now, I have a camera at the studio, on the door.
[903.64 → 907.44] And I love being able to just pull it up and check on it from time to time.
[907.58 → 913.14] That particular camera, too, I've intentionally made it possible for me to view when I'm away.
[913.62 → 914.64] I just love this at the studio.
[914.70 → 918.22] That way, when I get a package, I know it's there, and I can call up Was, and I can say,
[918.28 → 920.44] Hey, Was, will you go grab that package for me?
[920.44 → 928.18] Now, before you left, you were really quite worried about the heat down in Texas, you know, melting your pies.
[928.38 → 929.12] How has that been?
[929.58 → 931.68] It has been tricky.
[931.82 → 937.88] In fact, I'd say it's been trickier than I appreciated because it really starts with the solar system.
[938.16 → 941.70] I've gotten some good experience, and I've learned a few tricks.
[942.26 → 946.48] So I can run my air conditioning off of solar, which feels like a hack.
[946.62 → 948.58] It feels like a cheat code for nature.
[948.58 → 959.74] But what I discovered when I'm running my air conditioners off of solar is when you invert that much of a load, it generates a lot of heat.
[960.04 → 968.16] So I'm already dealing with a heat issue in my server seat, and now my electrical system is struggling to stay cool as well.
[968.22 → 971.88] So the very system that powers the entire RV, which I did not expect to be an issue,
[971.88 → 978.48] But when you start inverting a huge load, there are safety mechanisms that kick in when the gear reaches 110 Fahrenheit.
[978.90 → 986.08] And it starts an auto shutdown procedure where certain things, ironically, it wasn't the air conditioner, but certain things start shutting off.
[986.48 → 988.88] How much load does your AC unit pull then?
[989.14 → 993.46] When they're both going, it's about 2200 watts.
[993.90 → 994.78] It varies.
[994.78 → 997.82] That's the same as what my entire house uses for AC.
[999.16 → 1003.42] Well, when they're both going full bore, and I really mean, you know, like it's 100 degrees, it's hot.
[1003.54 → 1003.90] It's hot.
[1003.98 → 1005.50] Yeah, when it's Texas heat.
[1005.70 → 1006.50] Yeah, I get it.
[1006.98 → 1014.00] If I run just one, and I don't have it on high power mode, I think it's around 700 watts.
[1014.28 → 1014.58] Okay.
[1014.82 → 1018.40] Well, that's still a lot, but not, you know, 2000 plus.
[1018.40 → 1022.60] It generates quite a bit of heat, so I've come up with a human solution to this problem.
[1023.66 → 1029.08] I've trained the boy on which bays of the RV to go open to create some venting.
[1030.62 → 1035.86] So I say, hey, Dylan, ventilation bays, go open the ventilation bays, and he runs out.
[1035.92 → 1037.18] So you have to do it when you're stopped, obviously.
[1037.26 → 1038.18] You can't do it going down the road.
[1038.58 → 1041.76] So he runs out, he opens up the bays, and then I kick on the air conditioning.
[1042.10 → 1046.14] I had visions of some Keanu Reeves-style speed stuff of hanging out the window.
[1046.14 → 1048.68] Yeah, I'm holding on to his feet.
[1049.04 → 1051.42] He's hanging down the side of the RV as we're going down the road.
[1051.86 → 1052.64] It's tricky.
[1052.76 → 1055.96] It's trickier than I expected because the batteries are near the drivetrain.
[1056.46 → 1059.96] And so the drivetrain gets hot, plus it's 100 degrees outside.
[1060.36 → 1063.32] So there's just a lot of thermal pressure on everything.
[1063.54 → 1066.46] And the server seats, very warm.
[1067.10 → 1070.72] During the day, if I don't get ready for this, get ready for these numbers.
[1070.72 → 1077.12] If I don't implement a cooling solution for the server seat, I have seen the temperature
[1077.12 → 1082.06] in that booth get as high as 97 degrees Fahrenheit for the ambient air temperature for all the
[1082.06 → 1082.78] components in there.
[1083.20 → 1085.10] So I've been following this very closely.
[1085.30 → 1088.54] Of course, I'm bringing all this data into Home Assistant, and then I'm reviewing it each
[1088.54 → 1089.74] day to kind of see how bad it got.
[1090.22 → 1097.22] I now have like five of these six-in-one multi-sensor from Biotech.
[1097.54 → 1098.36] It's Biotech.
[1098.36 → 1099.72] They're kind of expensive.
[1099.84 → 1106.00] They're like almost 60 bucks each, but they track light, UV, motion, vibration, temperature,
[1106.28 → 1107.66] all that kind of stuff.
[1107.94 → 1112.64] And it has a cool temperature sensor where it's actually like scanning using infrared.
[1113.48 → 1116.62] So it actually, it gets, it's a really cool way to get ambient temperature.
[1117.22 → 1123.10] And the pies themselves start to throttle when they reach 80 degrees Celsius.
[1123.10 → 1128.96] And they don't really go above 85 degrees Celsius without shutting down.
[1129.78 → 1132.04] Amazingly, they continue to function.
[1132.40 → 1133.70] Everything continues to work.
[1133.78 → 1138.74] Even transcoding and watching video, all that stuff is still working.
[1138.94 → 1143.80] And I have implemented another human solution here where I have Dylan crack the booth.
[1143.92 → 1149.16] He just, he removes the cover on the top of the booth and creates a little bit of airflow
[1149.16 → 1150.34] and that cools it down.
[1150.38 → 1152.88] But then we have to seal it back up to turn it into a bed every single night.
[1152.96 → 1158.20] So then the temperature builds back up each day, and then we crack it to cool it.
[1158.52 → 1160.70] Have you thought about a vent in the side of the thing or something?
[1160.96 → 1162.76] Yeah, we're looking right now at ways to vent it.
[1162.84 → 1165.74] It's tricky because it's wrapped in cloth, and it would be really gaudy.
[1165.98 → 1167.90] And it's also right as you enter the RV.
[1168.06 → 1171.64] So if I put it right in the side of the booth, it'd just be right as you walk in, you'd see it.
[1171.88 → 1172.48] Very ugly.
[1172.90 → 1174.12] I am looking at other options.
[1174.12 → 1177.78] I've just got visions of Dylan going to sit down, and you'd be like, nope, sorry, son.
[1177.84 → 1178.78] You can't sit down today.
[1178.88 → 1179.88] The servers have got to breathe.
[1180.10 → 1180.88] It's a hot seat.
[1180.98 → 1181.16] Yeah.
[1181.46 → 1183.00] You got to let the servers breathe.
[1184.62 → 1185.78] Oh, it's so bad.
[1185.92 → 1192.30] So I ended up scouring the internet to find the various ways to take the temperature of a Raspberry Pi
[1192.30 → 1197.58] because a lot of the built-in things like LM sensors that you would normally use on a Linux box,
[1197.68 → 1198.84] they don't work on a Raspberry Pi.
[1199.42 → 1202.20] I got a little script, and I'll link the details in it.
[1202.20 → 1208.98] But essentially, if you just cat sysclassthermal, thermalzone0 slash temp, if you just cat that file,
[1209.26 → 1214.76] you'll get back a number, and it'll be like 54,530.
[1215.18 → 1218.60] And what that actually is, is the temperature of your CPU.
[1219.40 → 1224.20] So when I ran it, it was 54,530 was the number that came back.
[1224.70 → 1230.34] Well, that is 54 degrees Celsius, 54.5 degrees Celsius.
[1230.34 → 1236.94] And so I know that right now as we do this, my Pi is just a little under 60 degrees Celsius.
[1237.26 → 1239.78] So it's not in the dangerous throttling zone yet.
[1240.40 → 1241.82] And I just keep an eye on that.
[1242.74 → 1246.46] Basically, I'm running it on the red line during this entire trip.
[1246.50 → 1251.66] And I have a few ideas about relocating or using ventilation when I get back.
[1251.66 → 1253.74] I mean, this is production mode.
[1254.14 → 1257.06] You know, the real solution here is just don't go to Texas in June.
[1257.66 → 1258.20] No kidding.
[1258.54 → 1261.26] This was a non-problem in the Pacific Northwest.
[1261.92 → 1267.10] I'm only here for a few more days, and then I'm making my way north again, and it shouldn't be as much of an issue.
[1267.52 → 1271.78] And then I think when I do eventually make it back to the Pacific Northwest and get to my home base,
[1272.34 → 1277.22] I will probably retool this setup and move it to a different spot that has ventilation.
[1277.54 → 1280.46] Because you had a spare Raspberry Pi ready to go and everything like that.
[1280.46 → 1281.00] I did.
[1281.22 → 1281.42] Yep.
[1281.60 → 1284.26] I was going to be surprised if it was the Pi that went first.
[1284.54 → 1287.86] You know, not a power supply or, you know, a switch or something instead.
[1288.14 → 1290.18] But I think that's a very fair point.
[1290.26 → 1295.32] In fact, that was the realization I had as the temperature started to rise is I realized,
[1295.44 → 1301.32] oh, you know what's going to pop first will be the power bricks or my firewall or my Wi-Fi.
[1301.92 → 1303.80] That's what's going to go first, not the Raspberry Pi.
[1303.80 → 1309.02] I mean, if you look at, you know, any Intel system these days, you know, any Intel laptop,
[1309.02 → 1312.62] they'll go up to 100 Celsius, you know, almost instantly.
[1313.14 → 1314.80] And so, I mean, these things can cope.
[1314.88 → 1319.24] I mean, a Pi isn't probably built to the same tolerances as a high-end Intel chip.
[1319.48 → 1323.32] But, you know, these things can cope with some heat, the circuit boards and stuff like that.
[1323.36 → 1325.04] They're not going to melt or anything like that.
[1325.16 → 1328.54] But power supplies, they really, really don't like heat.
[1329.00 → 1330.84] Yeah, I'm a little nervous, to be honest.
[1330.84 → 1334.88] I have to give a hearty plug again for these Adtech multi-sensors.
[1335.26 → 1336.88] I've talked about them on the show before.
[1337.42 → 1341.06] They're not the cheapest Z-Wave temperature sensors you can find out there.
[1341.58 → 1343.34] But I have these now.
[1343.46 → 1344.58] I have one in my water bay.
[1344.72 → 1346.16] I have one in my electrical bay.
[1346.36 → 1348.56] I have one in the bedroom, one in the living room.
[1348.76 → 1350.34] I have one in the server booth.
[1350.54 → 1352.38] I have one up front where I drive.
[1352.38 → 1357.64] And all of them flawlessly report into Home Assistant.
[1358.34 → 1363.54] And what is fantastic about them is you can run them with continuous power with USB.
[1363.80 → 1366.24] It's just, you know, like super low voltage.
[1366.60 → 1370.58] And then you get continuous every second reporting, if you'd like.
[1371.38 → 1376.32] Or you can pop a like a Duracell lithium-ion battery, you know, those little removable lithium-ions.
[1376.78 → 1379.02] It has a spot for one of those you can pop in there.
[1379.08 → 1380.62] And you can adjust the update interval.
[1380.62 → 1382.60] By default, when you run off battery, it's much slower.
[1382.70 → 1384.76] It's like every 15 minutes to save battery life.
[1385.12 → 1388.18] And then the thing runs for like a year off one of those batteries.
[1389.02 → 1389.32] Nice.
[1389.86 → 1391.40] I really like these things.
[1391.72 → 1394.24] You do have to have Z-Wave, but they're just fantastic.
[1394.68 → 1399.80] What I'm thinking is I'd love to put one under my deck or something outside that's somewhere kind of vaguely sheltered.
[1400.04 → 1402.54] Just to get, you know, an outdoor weather station going or something.
[1403.18 → 1405.46] Are they suitable to go outside or are they indoor only?
[1405.80 → 1407.48] I mean, I wouldn't be surprised if you could.
[1407.48 → 1411.32] But on their box, now that I think about it, it does say indoor use only.
[1411.98 → 1412.62] I don't know, man.
[1412.74 → 1416.76] I mean, once you have the power in there, and you seal it up, they're pretty simple.
[1416.82 → 1420.68] And if you had it under your deck where it was out of the rain, I think you'd probably be fine.
[1420.70 → 1422.86] Because I have two of them in my outside bays.
[1423.16 → 1429.66] And one of them is my water bay, which is frequently exposed to the elements because I have incoming, you know, hoses and stuff.
[1429.66 → 1433.18] So you might be able to get away with it because I'm doing it basically.
[1433.48 → 1434.28] It's pretty great.
[1434.42 → 1435.64] And I just want to give them a hearty plug.
[1435.70 → 1436.78] So I'll put it in the show notes.
[1436.90 → 1439.38] No, you know, I get no affiliate or anything like that.
[1439.44 → 1441.86] But boy, have they just worked really solid for me.
[1442.38 → 1447.16] What I learned is you can use motion sensors for a lot of the things I was using cameras for.
[1447.58 → 1449.88] For presence awareness and automations.
[1450.02 → 1450.76] It's pretty great.
[1450.76 → 1455.48] Well, particularly in your world where, you know, one footstep probably shakes the entire house.
[1456.26 → 1458.02] Or at least I'm running kids, right?
[1458.12 → 1467.46] Like I see a future where when several of these sensors are reading a certain vibration level, I just automate something.
[1467.66 → 1477.90] I started playing with this for a brief period of time when if there has been motion or not motion but vibration, disable all the automatic lights and heater stuff.
[1477.90 → 1485.48] Because one of the tricks about Home Assistant going down the road, which I've been dealing with on this trip, it does not automatically update its location.
[1486.00 → 1486.90] In fact, nothing does.
[1487.30 → 1489.84] Nobody builds these home products for a home that moves.
[1490.26 → 1492.14] The Echo product doesn't update.
[1492.26 → 1494.16] Google stuff doesn't auto-update its location.
[1494.62 → 1500.50] You think you have a smart tube on your counter and it, for the life of it, still thinks I'm in Washington.
[1501.04 → 1504.12] But also Home Assistant doesn't update its location automatically.
[1504.12 → 1509.26] And heaven forbid you've ever specified it via the YAML file because then you can't even update it on the web UI.
[1509.90 → 1514.52] So I've had to go through and like every time zone change, I have to go through and fix that stuff.
[1514.60 → 1518.00] So my automations for sunrise and sunset, no, that still work right.
[1518.28 → 1519.80] That really is a first-world problem, bro.
[1521.02 → 1521.84] Who are you telling?
[1522.00 → 1522.36] I know.
[1523.10 → 1525.12] It doesn't mean I don't enjoy them.
[1525.68 → 1529.44] You know, it's these little challenges that kind of make this fun.
[1529.44 → 1534.52] I mean, I know you were kind of playing around with trying to get it right in your basement recently because you got a wet basement.
[1535.16 → 1535.24] Yeah.
[1535.50 → 1541.22] When we first moved in, actually, one of the first episodes where I was in this house around the turn of this year,
[1541.30 → 1545.92] we talked a little bit about how I was monitoring the temperature and humidity in my basement.
[1546.60 → 1551.58] Now, it's not a finished basement, but it's important to me because that's where my primary server, you know,
[1551.58 → 1557.78] with the 15 or whatever it is, 13 spinning hard drives in, is down there.
[1557.98 → 1564.10] So, you know, if it's, you know, sitting at 90 plus percent humidity for a month, I want to know about it.
[1564.64 → 1567.38] Well, the rainy season has started here in Raleigh.
[1567.68 → 1574.72] And unfortunately, the basement at Casa del Breccia Mar is getting a little bit humid.
[1575.86 → 1576.52] Got a wet basement.
[1577.62 → 1578.68] How bad is it?
[1578.68 → 1580.30] Like when you say a little humid, is it like...
[1580.30 → 1581.50] Yeah, 90 percent plus.
[1581.82 → 1586.20] Oh, so there could be even moisture like collecting in areas and maybe mould starting to develop?
[1586.52 → 1586.74] Yep.
[1587.24 → 1589.14] You can actually correlate in Grafana.
[1589.26 → 1594.96] When I put some of the six-month views into the Discord, I was talking with some of the guys in there about it.
[1595.58 → 1601.08] And you could correlate storms with spikes in humidity in my basement.
[1601.34 → 1604.68] Obviously, as the ground around the house gets wet, it's got to come up somewhere,
[1605.22 → 1606.86] which I just thought was fascinating.
[1606.86 → 1618.06] And so I went on Costco's website and bought a $150 dumb dehumidifier, as in dumb as in it doesn't have any Wi-Fi enable nonsense or anything like that.
[1618.80 → 1621.44] And I've just thrown it down in the basement, forgetting about it.
[1621.60 → 1625.64] But I didn't really want it running 24 hours a day because it's quite loud.
[1625.64 → 1628.02] It's directly underneath where my home office is.
[1628.12 → 1629.76] So I could hear it through the floor.
[1630.32 → 1630.88] Oh, that's annoying.
[1630.88 → 1631.48] Yeah.
[1631.78 → 1635.06] And so I just thought, hmm, I've got the technology to solve this, haven't I?
[1635.32 → 1637.82] I found one of my TRIMOTOR smart plugs I wasn't using.
[1638.36 → 1646.42] I threw the dehumidifier on there, and then I put a home assistant automation to run the dehumidifier between 7 p.m. and 7 a.m.
[1646.88 → 1648.26] And that's worked great.
[1648.78 → 1654.68] Have you thought about getting a sensor for humidity and then just running it when humidity is at a certain level?
[1654.68 → 1670.78] Well, that's how I know the basement was at 90 plus percent was because the temperature sensor I have is one of those ESP8266 D1 minis connected to, I think it's a DHT22, which just monitor temperature and humidity.
[1670.94 → 1671.56] That's all they do.
[1672.02 → 1674.00] And that just reports back into the home assistant API.
[1674.76 → 1681.52] I flashed that one using ESP home a little while ago, which it just works really, really reliably, really, really well.
[1681.52 → 1690.68] And so, yes, you know, in time, I will have the dehumidifier, I will have that only come on.
[1691.12 → 1694.00] I mean, it has its own sensors built in.
[1694.06 → 1699.18] Once it detects the basement is, you know, like 45 percent or whatever your target is, it will shut itself off.
[1699.68 → 1702.94] But I also only want it running overnight when I'm not anywhere near it.
[1703.74 → 1708.22] So, you know, for me, I think that's the best of both worlds.
[1708.22 → 1713.38] The dumb appliance has been made vaguely smart to fit my own personal requirements.
[1714.04 → 1717.68] And then it uses its own thing inside itself to turn itself on only when needed.
[1718.04 → 1718.72] So, hmm.
[1718.84 → 1719.86] Yeah, that is a nice combo.
[1720.26 → 1722.52] A way to use some of its built-in sensors.
[1722.86 → 1728.28] I really whenever I can now, and I'm buying something like a fan or a heater or a dehumidifier,
[1728.64 → 1736.64] I just look for something that just has a dumb switch on that I can just leave in the on position and then really power cycle it with a smart switch.
[1736.64 → 1737.36] Mm-hmm.
[1738.10 → 1742.70] Speaking of smart outlets, some of the designers at GitHub have obviously been a bit bored recently.
[1743.14 → 1743.54] Uh-oh.
[1744.00 → 1747.56] I got to admit, I didn't realize they'd done a design change.
[1747.94 → 1750.72] I mostly just interact with GitHub from the command line.
[1750.94 → 1755.62] So, and also, I don't think it's as bad on my screen because I'm on a laptop screen.
[1755.88 → 1757.04] It's quite a subtle change.
[1757.04 → 1768.02] But it was, I think, the same day as Apple's keynote where they announced the Big Sur, you know, the big design refresh with the rounded corners and the transparency and the magic that Apple have.
[1768.54 → 1768.64] Yeah.
[1768.76 → 1770.74] Then comes the GitHub theme change.
[1770.88 → 1773.54] And it's a very subtle change.
[1773.60 → 1775.98] But I use GitHub every single day.
[1776.06 → 1778.72] So, for me, it's like one of the most important websites on the internet.
[1778.72 → 1781.08] And I hate it.
[1781.26 → 1781.92] I just hate it.
[1782.00 → 1785.18] There are the issues and the projects and the wiki thing.
[1785.34 → 1787.72] The little bar above the repo is now over to the left.
[1787.82 → 1793.90] And the releases tab has moved from being a tab to being this weird micro sidebar on the right.
[1794.20 → 1795.00] And...
[1795.00 → 1795.86] Oh, you're right.
[1796.10 → 1798.18] It's a fully adaptive website now.
[1798.40 → 1801.00] And it, I mean, it's probably better in some ways.
[1801.42 → 1802.88] I'm just checking it out right now.
[1802.98 → 1803.88] Oh, my goodness.
[1804.06 → 1804.64] You're right.
[1805.84 → 1806.82] Oh, hmm.
[1806.88 → 1807.68] I kind of like it.
[1807.68 → 1812.38] You really are an apple sheep.
[1812.62 → 1814.58] Well, no, it's just I'm on a smaller screen.
[1814.70 → 1816.40] So, it feels like it's a little tighter.
[1816.48 → 1821.82] But I could see if I was on a ginormous 95-inch screen like you are, it would be a lot of wasted space.
[1822.12 → 1823.18] 95, darling.
[1823.30 → 1824.04] It's only 38.
[1825.58 → 1827.70] Well, it's bigger than my 14-inch ThinkPad.
[1828.10 → 1828.76] Yeah, yeah.
[1828.86 → 1831.80] So, I mean, I do generally work on an ultra-wide all day.
[1831.80 → 1835.78] So, I'm probably not the target market the designers had in mind.
[1836.78 → 1842.30] When you move GitHub to be, you know, a third of my screen width or anything like that, it looks like it always used to.
[1842.30 → 1847.08] And for the most part, the changes are largely fine and benign.
[1847.08 → 1853.70] But it's only when you start to get that wider screen where you've got elements all the way to the right and all the way to the left and in the middle.
[1853.86 → 1856.26] It's like, guys, it was fine before.
[1856.40 → 1857.40] You've just made it worse.
[1857.88 → 1860.14] You've taken a mouse road trip just to click on a UI element.
[1860.14 → 1861.14] Yeah, true.
[1861.64 → 1865.70] Now, the good news is that that pushed me.
[1865.88 → 1872.18] I mean, this is something I've been using kind of not super seriously for a while, but in the last couple of weeks, I've taken it a bit more seriously.
[1872.46 → 1873.78] And that's Gift.
[1873.94 → 1874.50] Gaya?
[1874.78 → 1875.30] Gift?
[1875.46 → 1876.18] I think Gift.
[1876.50 → 1877.52] I've always called it Gift.
[1877.78 → 1880.64] A self-hosted, I want to say GitHub clone.
[1880.82 → 1886.10] That's probably not necessarily fair, although it's a very similar feature set to GitHub.
[1886.10 → 1893.72] They call it a community-managed, lightweight code hosting solution written in Go, and it's published under the MIT license.
[1894.14 → 1894.56] It's really nice.
[1894.66 → 1897.70] It lets you mirror any public repositories that you want to.
[1897.82 → 1905.48] So if you want to mirror every single thing you push to GitHub locally, just automatically, Gift will do that for you.
[1905.90 → 1912.00] It supports multiple organizations, multiple users, pull requests, forks, all that kind of stuff.
[1912.12 → 1914.04] Everything you're used to really with GitHub.
[1914.04 → 1920.74] Obviously, the downside of self-hosting something like Git is that you don't have the community that's there.
[1921.30 → 1928.66] You know, I often think that when I see big projects moving to GitLab even, which is obviously a next level up from self-hosting your own Git server again.
[1928.88 → 1932.32] So, you know, just bear that in mind when you're making that choice.
[1932.86 → 1933.46] I think that's fair.
[1933.46 → 1941.66] I think if you're a project that's trying to draw in as many contributors as possible, you've really got to do the math on this.
[1942.12 → 1949.72] However, if it's for yourself and some friends or for a work project, I don't think there's any real downsides to it if you've got the storage and the means to keep it running.
[1950.22 → 1953.06] I assume you probably deployed the container version of Gift.
[1953.06 → 1954.40] I do, yes.
[1954.56 → 1963.84] And then it backs itself up to a ZFS dataset, which is now remotely replicated between my server and my other server in England.
[1964.18 → 1969.14] I finally finished a six terabyte upload to England, which took eight weeks.
[1969.86 → 1970.06] Whoa!
[1970.56 → 1972.32] How often were you checking in on that thing?
[1972.32 → 1978.68] The trouble was, whenever I was uploading and my dad wanted to watch player, it kept buffering.
[1979.62 → 1984.58] So I had to keep going in and turning it off, and then I'd lose a night because I'd forget to turn it back on again.
[1985.42 → 1988.66] Did he complain, Alex, my internet's just been so horrible.
[1988.90 → 1989.56] I don't know why.
[1989.80 → 1991.00] Yes, he did.
[1991.58 → 1992.24] Sorry, Dad.
[1992.52 → 1994.26] Did you say, oh, Dad, sorry about that.
[1994.84 → 1997.72] Well, I don't understand because, so here's what I'm doing.
[1997.84 → 2000.24] I'm running from ZFS in my basement.
[2000.24 → 2013.40] I'm doing a wire guard tunnel through my Open Sense router directly to the endpoint, which is an Ubuntu 2004 LTS, the box I did the remote reinstallation on a few episodes ago.
[2013.48 → 2017.52] So if you want to know how long this upload's been going for, go back to that episode.
[2017.92 → 2019.40] And that was when I started the upload.
[2019.58 → 2020.74] So it was a while ago.
[2021.82 → 2028.22] He was having stuttering downloading player, which is going to be a couple of megabits at most, I would have thought.
[2028.94 → 2029.80] Let's say 10.
[2030.24 → 2032.38] And he has 300 something down.
[2032.66 → 2035.76] And I have 35 Meg up here with Spectrum.
[2036.02 → 2039.64] And it's like, how can that possibly be causing buffering on his end?
[2040.26 → 2040.56] No kidding.
[2040.68 → 2050.84] You would think that your remote connection that's over a transcontinental link wouldn't be able to mess up a download that he's doing that's probably as near local as it gets.
[2050.84 → 2058.08] Now, the only thing I could think of, and this is just a pie in the sky theory, is that there were too many connections open or something.
[2058.08 → 2063.66] But then it's going into a pfSense box at the other end, which has, you know, a pretty large state table.
[2063.66 → 2066.84] So it's not a cheap ISP router or anything like that, you know.
[2067.58 → 2071.06] So I'm a bit stumped really as to what was causing it.
[2071.36 → 2073.62] So if you have any ideas, write in and let me know, please.
[2074.26 → 2074.76] Yeah, that's tricky.
[2074.90 → 2076.12] It may not be a bandwidth issue.
[2076.26 → 2078.88] It could be a device issue that was causing it.
[2078.88 → 2082.72] But six terabytes, I mean, that must feel good to have it all done now and backed up.
[2083.10 → 2083.16] Yeah.
[2083.30 → 2084.88] And now I just do the incremental backups.
[2085.06 → 2090.30] You know, I did my app data backup this morning, and it took about 20 minutes instead of six weeks.
[2090.44 → 2091.00] That was nice.
[2091.30 → 2095.78] When you're self-hosting, boy, have I learned this lesson recently, that kind of peace of mind is necessary.
[2095.92 → 2100.58] Because, you know, when you're deploying something like Git T yourself, you don't want to lose that data.
[2100.62 → 2101.56] That's going to be really embarrassing.
[2101.56 → 2109.04] And I am so grateful that the recent data loss I had, the vast, vast, the vast majority of it was all recovered, even though my backups had broken.
[2109.18 → 2113.44] Because I had that data stored on another system, which, like you're doing now too.
[2114.02 → 2117.56] And I just really, really got to double down on that.
[2117.62 → 2121.50] Like if you're going to do this, if you're going to host this stuff yourself, take the time.
[2121.66 → 2124.46] Because, boy, did I learn that one the hard way recently.
[2124.72 → 2128.70] And that's even knowing this, you know, even having said this and preach this stuff over and over again.
[2128.76 → 2129.82] Like it can still be an issue.
[2129.82 → 2131.28] So congratulations, sir.
[2131.36 → 2133.28] That must be a nice peace of mind.
[2133.38 → 2134.02] It must feel good.
[2134.40 → 2135.26] Yep, yep, yep, yep.
[2135.78 → 2148.28] My grand vision is I'll have the ZFS replication at his house, which will then itself replicate to the Pi 8 gigabyte I bought a couple of weeks ago at my sister's house.
[2148.46 → 2154.66] So I'll have three full copies of everything I care about in a ZFS reachable location.
[2154.66 → 2159.84] On top of that, I have everything backed up to Google Drive that I care about and also Glacier.
[2160.20 → 2164.36] So between those five different points, I think I have it covered.
[2164.86 → 2167.58] You're set unless it's a meteor strikes the earth.
[2168.66 → 2171.90] Yeah, unless something takes out North America and Europe at the same time.
[2172.14 → 2172.68] I'm fine.
[2173.96 → 2176.10] I think you probably have other problems at that point.
[2176.42 → 2177.24] Maybe, maybe.
[2177.54 → 2178.10] We'll see.
[2178.48 → 2179.18] If you're lucky.
[2179.18 → 2181.56] So thank you very much for listening.
[2181.86 → 2183.00] That was Self-Hosted 22.
[2183.36 → 2185.88] You can find the show at Self-Hosted Show on Twitter.
[2186.50 → 2189.08] And don't forget the Discord, self-hosted. Show slash Discord.
[2189.40 → 2190.62] Oh, yeah, it's really kicking up over there.
[2190.66 → 2192.28] We've got over a thousand users these days.
[2192.40 → 2193.82] It's a really great community.
[2194.28 → 2196.18] It is my social media platform now.
[2196.24 → 2200.72] I mean, I'm still on Twitter at Chris Lass, of course, but I've been really getting a lot out of Discord.
[2200.84 → 2201.48] So go check that out.
[2201.48 → 2206.54] We'd also like your emails, your feedback, your questions, your ideas, self-hosted. Show slash contact.
