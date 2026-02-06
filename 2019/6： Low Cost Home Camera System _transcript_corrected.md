[0.00 → 3.60] We teased last week, Chris, that you've been doing some camera stuff, right?
[3.86 → 7.44] And I think I certainly, because I'm just about to buy a house,
[7.84 → 12.18] I certainly want to know more about your cameras, the good and the bad.
[12.76 → 14.86] But let's just address the elephant in the room.
[15.00 → 16.96] You were pretty hard on Shinobi last week.
[17.56 → 20.62] First, congratulations on the news on the new house.
[20.62 → 22.86] That's going to be epic project material for the show.
[23.04 → 24.06] That's amazing.
[24.92 → 28.26] Yeah, so last week we talked a little bit about Shinobi on my Raspberry Pi 4.
[28.76 → 29.64] It was going bad.
[30.00 → 32.78] I don't know if you remember, but I was like pegging out the CPUs
[32.78 → 34.78] and I hadn't even added all the cameras yet.
[35.06 → 36.22] Three cameras is what you said.
[36.60 → 43.16] Yeah, well, I'm happy to say I've got five cameras now and the CPU usage is high,
[43.30 → 47.14] but that's because I've also turned on motion detection and recording,
[47.46 → 49.30] which saves some storage space.
[49.30 → 55.24] So you're able to get five cameras with all of this kind of advanced features
[55.24 → 56.82] working through a Pi 4?
[56.82 → 62.48] Yeah, I suppose for full disclosure, the fifth camera is more of an on or off.
[62.64 → 67.74] I actually set up my dash cam as a camera feed that feeds into the Shinobi DVR system.
[68.10 → 68.80] Of course you did.
[69.98 → 71.74] So I just turned that one on or off.
[71.88 → 77.90] So that's not motion detection based because that's really where a lot of the processor goes,
[78.04 → 79.20] Alex, is the motion detection.
[79.20 → 85.50] It turns out last week I was trying this out on Ubuntu LTS and find distro, Alex,
[85.56 → 88.46] but not quite there for the Raspberry Pi 4 yet.
[89.30 → 94.76] And when I switched over to Raspbian, when I just nuked and paved and rebuilt it on Raspbian,
[95.34 → 99.50] when I selected the hardware acceleration options, and I could just choose auto,
[99.50 → 103.82] but when I just turned them on in Shinobi, works with Raspbian.
[104.04 → 107.18] And my CPU used to just completely drop to the floor.
[107.38 → 108.72] It was just, it was gone.
[109.04 → 109.70] So what is that then?
[109.84 → 112.02] It must be some hardware acceleration at play here.
[112.24 → 118.04] I think so because like sometimes the camera feeds just kind of stop recording.
[118.42 → 122.22] And I think it's like a GPU acceleration failure.
[122.22 → 125.82] So about every couple of days I've rebooted the box.
[126.18 → 129.96] Now that I've switched over to motion capture, that hasn't been an issue yet.
[130.12 → 136.10] But so maybe I should recap a little bit just to remind you, I have those Waze cameras,
[136.22 → 137.86] those little $25 Waze cameras.
[138.16 → 143.20] I've mounted them all around the inside of my RV, had to run like the USB cords and stuff,
[143.28 → 144.94] which is what it is.
[145.34 → 148.48] But I popped on a new firmware onto those Waze cams.
[148.54 → 149.20] It's pretty simple.
[149.20 → 152.72] You just download their official RTSP firmware file.
[153.28 → 158.58] The downside is, does I don't think it's really quite feature complete compared to the official
[158.58 → 159.30] official firmware.
[159.48 → 159.98] What do you think?
[160.40 → 162.86] As I understood it, it's like a fork in time.
[163.26 → 167.08] So they, it's not a build that they keep up to date with the modern features.
[167.32 → 172.14] I believe they fork it every couple of months, although there's no commitment to doing so.
[172.22 → 175.24] They just say, here's a snapshot in time with RTMP turned on.
[175.40 → 177.38] We'll release another one when we feel like it.
[177.38 → 180.28] This seems to be like a very highly demanded feature though.
[180.36 → 182.70] So it's unlikely they're going to abandon it.
[183.10 → 187.34] But quite frankly, my goal here is to cut these things off from the internet anyway.
[187.84 → 189.94] So I care less.
[190.82 → 193.26] Why do you need a dash cam into Shinobi?
[193.42 → 195.72] Like, are you using one of those Waze cams as a dash cam?
[196.18 → 196.42] Yeah.
[196.56 → 196.72] Yeah.
[196.72 → 200.22] I haven't actually gone down the road yet, but I have one set out looking the windshield.
[200.68 → 201.24] In your car?
[201.56 → 202.18] No, on the RV.
[202.56 → 203.06] Oh, okay.
[203.06 → 206.14] Well, I mean, if you're driving a flipping bus down the road, I can see.
[206.28 → 206.48] Yeah.
[207.08 → 208.66] I can see that little camera not being a thing.
[208.68 → 209.82] I was thinking in your Golf, man.
[209.86 → 212.42] I was trying to figure where that little thing fitted in your Golf.
[213.20 → 215.68] No, I put it up front there and we'll see.
[215.96 → 218.24] I haven't actually been on a road trip with it yet to test it.
[218.30 → 221.30] But anyway, I got this RTSP firmware, popped it on the file.
[221.38 → 224.02] You just rename it to like demo.bin, I think.
[224.68 → 227.22] Reboot the cameras holding down the setup button.
[227.22 → 230.88] And they'll detect the file and just ref lash themselves.
[231.74 → 240.54] And your real only immediate tell, unless you memorize the version numbers, is when you relaunch the Waze app, there'll now be an advanced RTSP section.
[240.82 → 241.90] You can turn that on.
[242.00 → 244.92] It'll give you the URL and you can plug that in anything.
[245.74 → 247.00] VLC, Shinobi.
[247.50 → 249.84] There are a few things, though, to make it work right.
[249.84 → 257.80] So if you want to try this, Alex, I put a link in the show notes on an article that tells you how to optimize Shinobi for RTSP capture.
[257.92 → 263.58] Because there are a couple of things that aren't necessarily obvious, especially if you want to grab the audio.
[264.36 → 272.54] And maybe the other disclaimer of using these Waze cams like this is they don't support that device standard that so many security cameras support.
[273.14 → 273.94] I think it's what?
[274.28 → 275.74] O-N-V-I-F or whatever.
[276.26 → 276.70] What's that for?
[276.70 → 276.82] O-N-V-I-F or whatever.
[277.18 → 293.06] It's like a standard control and features baseline that all cameras, if they're certified to support this, then you know you can plug them into whatever security software and control it remotely, make it pan or tilt or get certain time information off of it.
[293.52 → 294.34] So what is it like?
[295.06 → 296.10] Not UPnP.
[296.18 → 296.56] What's the other one?
[297.60 → 298.56] DLA or something?
[298.74 → 301.60] Is it a similar kind of universal protocol like that?
[302.04 → 303.04] Yeah, you could think of it.
[303.04 → 306.66] But in terms of like, this is how I control certain aspects of the camera.
[307.12 → 313.06] So then vendors of software can just make a general interface that works with any camera that meets the standard.
[313.54 → 314.60] The Waze don't have that.
[314.86 → 315.48] But they're $25.
[315.98 → 318.88] So you can forgive a lot for that price, can't you?
[319.10 → 319.70] The $25.
[320.02 → 327.34] And the other thing that surprised me, and I haven't pushed it beyond two, but I have a feed that's going into Shinobi on that Raspberry Pi 24-7.
[327.34 → 329.64] But I also can pull them up in Home Assistant.
[330.12 → 331.64] And I can pull them up in MPV.
[332.24 → 335.30] So I now have a tab in Home Assistant that's called my security tab.
[335.80 → 341.12] And in there, I have a tile for each camera and a tile for each motion sensor.
[341.12 → 344.32] And I've also integrated our Ring camera.
[344.46 → 346.04] Yes, I got one of those a long time ago.
[346.52 → 352.02] I no longer have an active subscription, but I do have an account still and I have an API key.
[352.08 → 354.18] So I can actually pull the Ring feed into Home Assistant.
[354.64 → 356.24] So that's kind of a neat real-time snapshot.
[356.24 → 357.50] That's really neat.
[357.68 → 357.88] Yeah.
[358.34 → 359.34] I wanted to ask you, actually.
[359.58 → 364.94] So remote access for Shinobi and I guess Home Assistant as well, I'm going to add to my question.
[365.56 → 369.04] Trying to use the Waze app is a bit rough remotely, I've found.
[369.64 → 374.26] I don't know if that's just the URLs I'm using or whatever, but I haven't had great success.
[374.34 → 377.26] Like my Nest Cam, which again, I bought a long time ago.
[378.08 → 381.54] I can just pull that up wherever I am in the world, and it just works.
[381.92 → 384.36] And the Waze Cam doesn't do that for you, the Waze app?
[384.36 → 388.02] For some reason, no reliably, I can't seem to use an error.
[388.14 → 389.18] I'm almost certain of that.
[391.88 → 395.40] I have not solved remote access yet.
[396.48 → 399.10] Theoretically, I would solve it with a WireGuard VPN.
[399.58 → 404.34] However, I am behind some enterprise-grade double NAT systems here.
[404.74 → 406.22] Carrier-grade, as they like to call it.
[406.52 → 413.48] So I have this super convoluted system that I'm working on where I WireGuard out to a remote system
[413.48 → 415.90] that establishes a two-way tunnel.
[416.24 → 418.40] And then I remote from my other systems into that.
[418.50 → 421.82] I have IP tables set up and some DNS and all of that.
[421.88 → 424.36] And it routes everything for me, but I haven't gone that far yet.
[424.66 → 429.64] So right now, I use the Waze app for remote access when I need it.
[429.64 → 430.92] But I don't generally.
[431.72 → 435.32] So I'm really kind of using this to go back in time if something were to happen.
[435.32 → 440.02] You know, maybe there was a mini fire or an accident with the kids or...
[440.02 → 440.66] A mini fire.
[440.90 → 442.16] Oof, that still sounds scary.
[442.54 → 444.00] Yeah, like a fridge fire, no big deal.
[444.08 → 446.02] Just burn up the whole side of the rig or something, you know.
[446.64 → 448.60] Maybe for insurance purposes, I want that.
[448.78 → 451.92] Or burglars comes in or some crazy listener.
[452.08 → 452.54] I don't know.
[453.54 → 454.52] It's all on camera.
[454.80 → 455.46] Crazy listeners.
[456.02 → 457.32] I have had them show up at campgrounds.
[457.88 → 459.74] I have had them knock on my door at rest stops.
[459.82 → 460.72] I love it, actually.
[461.12 → 462.98] Most of the time when we're on the road, I love it.
[462.98 → 466.94] One time, and I bet he's listening, somebody showed up.
[467.04 → 471.16] We were in Montana, and we were in a gravel lot.
[471.74 → 475.74] And somebody came, pound, pound, pound, police open up on my door.
[477.32 → 479.10] My heart just dropped.
[479.62 → 481.66] Like I just stopped breathing for a second.
[481.76 → 483.46] I opened up the door, and it was a listener.
[483.92 → 484.94] It's just screwing with me.
[485.66 → 486.36] Good job.
[486.48 → 490.40] You know if I ever get the chance to troll you like that, I would definitely do that.
[490.58 → 491.14] It's all right.
[491.18 → 491.56] It's okay.
[491.60 → 491.92] I'm good.
[491.92 → 492.34] I'm good.
[492.34 → 493.76] It just makes me jumpy.
[494.06 → 497.10] Luckily, I live far enough away that it's unlikely I'm just going to turn up at a random
[497.10 → 498.96] parking lot with dupes.
[499.74 → 500.68] Unless I come to you.
[501.08 → 502.28] We should clarify, by the way.
[502.32 → 505.62] We had a few people that didn't actually know that Chris lives full-time in an RV.
[506.10 → 507.50] Yeah, since what?
[507.64 → 509.52] I mean, it's been about five years now.
[509.60 → 511.22] I've upgraded once in there.
[511.28 → 512.88] So I've been in this one for about four years.
[513.46 → 513.84] Full-time.
[514.10 → 516.42] Yeah, with the wife and the kids and a dog.
[516.56 → 519.00] We affectionately call it Lady Dupes on the network.
[519.00 → 524.20] So we have JB1, which is the studio that we record most of the podcasts from in Seattle.
[524.32 → 525.04] Anyway, Chris and Was.
[525.52 → 529.84] And then Lady Dupes is Chris's home on wheels, I guess.
[529.94 → 530.06] Yeah.
[530.22 → 537.38] Remote studio set up with multiple cellular networks and a little recording spot.
[537.38 → 539.62] So I can do shows from the road.
[539.72 → 540.76] I can work from the road.
[541.02 → 542.68] But we also have offline media.
[543.02 → 547.04] Part of my, well, this is all part of my project off grid is to really, really make that thing
[547.04 → 549.14] a fully workable machine, even without internet connection.
[549.14 → 556.12] And that's why I wanted to get these cameras into Shinobi is I was slipping into the Logitech
[556.12 → 556.92] circle cameras.
[557.08 → 561.40] They're not great, but they're kind of the best cloud connected priced camera, in my opinion.
[561.40 → 566.70] And then you have things coming along like the Blink cameras that are really cheap.
[566.82 → 569.24] And then the Waze cameras came out at $25.
[569.88 → 570.96] Yeah, they cleaned up.
[571.26 → 576.62] So the fact that I could get something at that cloud connected or cloud subsidized price,
[576.62 → 579.70] but then I can use it for my own offline system.
[579.80 → 582.06] It makes me comfortable putting these throughout my house.
[582.44 → 586.56] Because before that, if you wanted to have a camera that was cheap, you pretty much,
[586.56 → 592.08] you know, at that $25 price point, it was, in fact, it was pretty impossible to beat that
[592.08 → 593.00] price, to be honest.
[593.54 → 597.34] But you could put, you know, a Raspberry Pi with a Raspberry Pi cam somewhere.
[597.56 → 597.88] Yes.
[598.12 → 598.28] Yeah.
[598.54 → 602.90] And that would get you in the sort of $40, $50 price point.
[602.98 → 607.88] But even so, at that point, like the other ones you mentioned, like the Logic stuff, the
[607.88 → 610.74] Blink, et cetera, like the Nest stuff.
[610.84 → 614.64] I mean, the Nest is expensive, but it's nice physical hardware.
[614.64 → 617.08] Like it's machined aluminum and all that kind of stuff.
[617.12 → 618.70] It looks nice.
[619.38 → 624.28] So the cameras that I've been looking at for my new house, which hopefully I'll move into
[624.28 → 628.08] in about six to eight weeks, I don't want Wi-Fi cameras.
[628.28 → 631.12] So this is, for me, the biggest downfall of the Waze cameras.
[631.38 → 638.02] I've got two or three here, and they're perfectly fine, but frames drop on occasion and, you
[638.02 → 643.08] know, it's chewing up Wi-Fi bandwidth where if I'm buying a house, I'm going to live there
[643.08 → 644.52] for the next 10 whatever years.
[644.72 → 645.34] You're going to wire them.
[645.64 → 646.58] I'm going to run a cable.
[647.30 → 649.02] You know, I'm not driving down the road like you are.
[649.02 → 649.86] I'm going to run a cable.
[650.08 → 651.32] I'm going to run POE.
[651.50 → 652.66] It's going to be a POE camera.
[653.10 → 653.76] Good for you.
[654.06 → 657.48] So I'm looking heavily at the Unify gear right now, but damn, it's expensive.
[657.88 → 658.16] Yes.
[658.46 → 661.18] And just one 1080p camera is about $130.
[661.18 → 667.88] I know my entire setup is probably under $300, including the Raspberry Pi to record it.
[667.96 → 672.38] Now, that does not include storage, which right now is still in flux.
[672.52 → 677.40] I'm cheating, and I'm using a big old thumb drive as I experiment, but I like what you're
[677.40 → 681.22] doing because you're investing in something that could last you a very long time.
[681.48 → 681.96] I hope so.
[682.12 → 687.00] I don't consider these Waze cameras probably more than like a three-year setup.
[687.38 → 688.30] They're disposable, right?
[688.34 → 690.16] They're like the little wind-up cameras you used to have.
[690.16 → 692.34] So you could do a full POE setup.
[692.60 → 696.16] You could do high resolution that could be swapped out to even higher resolution down
[696.16 → 696.66] the road.
[697.20 → 699.28] What are your minimum requirements, do you think?
[699.68 → 706.88] One for the driveway, one internally on the front and back doors, and the other in the
[706.88 → 708.44] garage too, because that's another ingress point.
[709.00 → 713.02] That's one of the last cameras I did here at the studio because I did a trial run of this
[713.02 → 714.06] camera setup here at the studio.
[714.18 → 718.16] So I have a similar Waze setup here at the studio, in fact, even larger.
[718.16 → 720.98] And my favourite camera is the one in the garage, surprisingly.
[721.56 → 721.64] Yeah?
[722.26 → 722.48] Yeah.
[722.58 → 726.56] I like to just, like if there's a noise or something, I like to check in and make sure
[726.56 → 728.68] that everything's okay and the car is okay.
[728.90 → 732.02] So where my desk is in this current house, I can't see the front door.
[732.02 → 737.62] So I have a monitor up top and I just throw my Nest driveway feed up there all the time.
[737.70 → 741.78] So when I'm just sat here working from home, I can just glance up and say, oh, that's what
[741.78 → 742.44] that noise was.
[742.96 → 747.36] But in terms of my requirements, self-hosting obviously is important.
[747.36 → 751.60] I don't want to have to pay a subscription for two reasons.
[751.86 → 756.66] One is it's a hidden cost effectively in the ticket price of the item.
[756.98 → 761.54] You know, you spend, let's say for a Nest cam, I know I keep coming back to those, but that's
[761.54 → 762.58] because that's the ones I have.
[762.66 → 763.72] I have two of those right now.
[763.72 → 770.42] You spend a hundred plus dollars, nearly 200, I think on the external one on a camera.
[770.68 → 775.96] And then you've got to spend another 50, 60 bucks a year for their cloud connected service.
[776.08 → 780.88] Now I appreciate for most people, that's a great solution because for most people, they
[780.88 → 783.46] don't want to have hard drives in their house.
[783.52 → 784.66] They don't want to have to think about it.
[784.70 → 785.66] It's just pressed a button done.
[785.76 → 786.18] Thank you.
[786.56 → 788.80] For me, I've already got a hundred terabytes in my basement.
[788.80 → 795.82] So I may as well use that with the Unify NVR stuff that they let you self-host.
[796.24 → 798.58] Would you put a Nest camera in your bedroom?
[799.00 → 800.78] Well, I've already got a Google Home in there, so.
[801.30 → 802.04] A camera though?
[802.32 → 805.28] That's doing person detection and object detection and sound?
[805.38 → 806.56] I don't need a camera in the bedroom.
[807.26 → 808.22] Nobody wants to see that.
[809.50 → 814.28] The very powerful object detection and person detection that comes with the Nest cameras
[814.28 → 816.34] is also, I think, what sleeves me out.
[816.34 → 818.66] And I'm not necessarily cloud bad guy.
[818.80 → 824.26] I do want to be comfortable walking around on camera just being myself.
[824.44 → 826.58] Maybe I'm in a robe or something like that.
[826.96 → 832.76] In the RV, because it's such a small space, I literally have nearly full camera coverage
[832.76 → 834.42] of everywhere in the entire RV.
[835.02 → 839.26] So there's really no way where you can be off camera unless you're in the bathroom.
[839.96 → 840.04] Yeah.
[840.44 → 845.10] And so I really wanted to be comfortable when I looked up and looked at that camera lens
[845.10 → 846.20] and saw that light was on.
[846.20 → 851.38] I didn't want to be thinking about where that could get processed or get stored.
[851.84 → 855.30] Well, there was that whole thing, wasn't there, with the was it Siri?
[855.52 → 858.20] I think where Apple employees were listening in to those recordings.
[858.68 → 863.66] Actually, I guess Nest also has had a significant rash of people compromising accounts and then
[863.66 → 867.84] like jumping on people's Nest cams and talking through the two-way microphone system.
[868.10 → 868.50] Have they?
[868.72 → 869.56] Ah, I didn't know that.
[869.56 → 870.04] Yeah.
[870.40 → 874.44] I heard some tech journalists ranting about it on a podcast recently, and then they looked
[874.44 → 878.10] into it and found that it's a fairly regular thing that they go out of their way to kind
[878.10 → 878.74] of keep quiet.
[879.14 → 880.70] Well, you would if you were them.
[881.64 → 886.88] So, you know, Black Friday's coming up soon in the States and Best Buy have started their
[886.88 → 887.76] shenanigans already.
[888.32 → 889.74] Are you deal shopping already?
[890.04 → 890.52] Well, I am.
[890.60 → 890.80] Yes.
[890.80 → 895.64] Obviously, I'm looking for appliances for the house, but couldn't help notice going in there
[895.64 → 897.26] looking at TVs and stuff like that.
[898.10 → 899.54] I mean, what's a guy to do, right?
[899.88 → 900.18] Oops.
[901.02 → 909.52] I haven't bought anything yet, but they have a 75-inch LED LG TV for like $900.
[910.18 → 910.88] Stop it.
[911.20 → 911.52] Uh-huh.
[911.74 → 916.80] You don't even want to know what I spent for my first 60-inch Pioneer Plasma.
[916.80 → 921.62] Well, I've got one of these TCL ROK jobs in my lounge right now, which I bought last
[921.62 → 921.88] year.
[921.96 → 925.12] I think it's 55 inches, and it was like $300.
[925.50 → 925.96] I like it.
[926.02 → 926.12] Yeah.
[926.18 → 926.54] I remember.
[926.82 → 928.04] For the price, it's great.
[928.28 → 932.96] The image quality, you know, dark scenes and stuff like that, like the episode of Game
[932.96 → 935.66] of Thrones a few months ago that was just dark.
[936.26 → 938.86] Like all I saw was like compression artifacts.
[939.18 → 940.54] I literally couldn't see anything.
[940.76 → 941.92] That's my TV right now too.
[942.24 → 945.98] And I really want to get an OLED, but damn, they're expensive.
[945.98 → 952.22] Yeah, I feel like I'm going to wait one more cycle of television so that the top of the
[952.22 → 958.40] line bumps down one notch because one of, I think, I don't know, this could be past Chris
[958.40 → 959.90] being an idiot, which happens a lot.
[960.02 → 961.18] So future Chris will determine.
[961.52 → 967.32] But current Chris is thinking that HomeKit integration could be a pretty big deal into
[967.32 → 971.54] televisions because I have had tremendous success working with HomeKit and Home Assistant
[971.54 → 974.06] and there's no cloud connectivity required.
[974.18 → 975.06] It's all over the LAN.
[975.06 → 982.62] And so integrating input control and power control and things of that nature into Home
[982.62 → 983.00] Assistant.
[983.48 → 987.48] Well, did you know those TCL TVs, the ROK TVs have an API?
[987.92 → 991.44] Oh, so I mean, if one was willing, you could probably do it yourself.
[991.70 → 994.32] Well, I turn my TV on and off using curl effectively.
[994.54 → 995.80] It's just a command from Home Assistant.
[996.36 → 996.98] Oh, no kidding.
[997.40 → 998.80] Yeah, I do it already and it works great.
[998.94 → 1000.22] Oh, that's wonderful.
[1000.22 → 1001.52] You can set inputs.
[1001.76 → 1003.02] You can turn the TV on and off.
[1003.24 → 1004.24] You can set the volume.
[1004.68 → 1005.00] All that.
[1005.18 → 1006.28] I'm legit jealous of that.
[1006.74 → 1011.68] Like, I think I'll tackle a full solar install and be completely off grid before I get my
[1011.68 → 1012.66] TV fully automated.
[1013.36 → 1014.16] Yeah, probably.
[1014.56 → 1016.24] See, I had a Harmony Hub before that.
[1016.30 → 1022.46] And again, that was a cloud connected device, which Logitech decided to switch the APIs off
[1022.46 → 1025.28] for in January or February this year.
[1026.20 → 1030.42] Right around the time I was getting into Home Assistant and writing that talk for Linux Fest
[1030.42 → 1036.64] Northwest that I was doing, you know, the DIY smart LEDs, which leads me very, very nicely
[1036.64 → 1042.36] into a little plug I wanted to do on the show today, which is that Linux Fest Northwest 2020
[1042.36 → 1045.14] is a call for papers is open.
[1046.20 → 1047.02] Are you going to submit?
[1047.42 → 1048.50] I am going to submit something.
[1048.60 → 1049.28] I don't know what yet.
[1049.28 → 1054.02] We've got about 60 days at the time of recording, so it closes like mid-January, I think.
[1054.96 → 1059.76] So yeah, if you've been thinking, oh, I'd like to talk at a conference, but I always
[1059.76 → 1060.82] miss the submission dates.
[1061.04 → 1062.24] You've got a couple of months.
[1062.58 → 1063.30] Give it some thought.
[1063.46 → 1067.44] Don't rush into submitting upfront because there's no benefit from doing that.
[1067.54 → 1068.06] Take your time.
[1068.18 → 1069.36] Put together a good proposal.
[1070.24 → 1072.76] Try and think of something that people want to listen to.
[1073.10 → 1074.04] I just got a great idea.
[1074.14 → 1075.06] I'd have to get clearance.
[1075.06 → 1081.42] What if I did a talk about the Lady Joop's automation, but at the start of my talk, everybody
[1081.42 → 1086.56] stands up, and they follow me out to the RV and I just give them a tour of it in person.
[1087.18 → 1087.64] Does that scale?
[1088.18 → 1091.80] Well, I'd have to do it in probably batches of like 10 people or something.
[1091.98 → 1092.16] Yeah.
[1092.24 → 1093.78] I mean, it's an RV, Chris.
[1093.96 → 1095.04] It's small.
[1095.56 → 1097.46] Did you see how many people were in there for the barbecue?
[1097.62 → 1099.08] We probably had 15 people in there.
[1099.34 → 1099.54] Yeah.
[1099.66 → 1099.88] Yeah.
[1099.88 → 1101.30] It was a whole thing.
[1102.32 → 1103.22] I'd love that though.
[1103.28 → 1106.00] Like if you've got some legit automations finished by then.
[1106.48 → 1106.70] Yeah.
[1107.04 → 1111.14] So far, this has been our most comfortable summer just due to the automations that I have
[1111.14 → 1111.38] got.
[1112.16 → 1113.98] When you can make your quality of life better.
[1114.32 → 1114.50] Yeah.
[1115.04 → 1117.68] You know, that's something I was thinking about talking to you about with these cameras.
[1118.24 → 1122.50] One of the things I noticed when I was taking my time and kind of doing it slowly and
[1122.50 → 1127.72] applying some craftsmanship to it, like we talked about with Wendell, I got a much deeper
[1127.72 → 1130.62] sense of satisfaction when the work was over.
[1131.04 → 1134.86] Like, and it struck me because I'd had a day when like a lot of things were thrown at
[1134.86 → 1137.82] me because I'm doing some travelling and all this stuff had come up, and it was like this
[1137.82 → 1139.36] crazy weekday.
[1139.64 → 1145.70] And I got home and I had a little bit of time in the evening and I had the energy.
[1145.70 → 1149.74] And so I banged out a few of these things and got the, you know, the Shinobi system reloaded
[1149.74 → 1153.04] and got the two additional cameras installed.
[1153.04 → 1158.92] And I had done a perfect job with the wiring and I, I, like I showed you, I Velcroed the
[1158.92 → 1161.48] components inside the, the, the dinette seat.
[1161.56 → 1164.26] So everything looks and is routed really clean and nice.
[1164.26 → 1167.64] And the power cables are all clean, and it's really proud of myself.
[1167.78 → 1172.34] And I had like this sense of accomplishment after having kind of a rough day when I was
[1172.34 → 1174.82] kind of like, I got knocked down all day long.
[1174.96 → 1178.28] I came home and, and like, I felt perfect about what I had done.
[1178.28 → 1182.58] And I realized that that's sort of like my dad used to talk about, he'd come home and
[1182.58 → 1187.78] he'd work on like part of the deck and fix that part of the deck in the evening and feel
[1187.78 → 1191.26] he'd have a rough day at work, but at least he got that damn deck fixed, you know?
[1192.02 → 1195.96] And that's, that's how this, even like working with home assistant and automating things has
[1195.96 → 1196.50] made me feel.
[1196.76 → 1202.94] Making stuff, whether it's a home automation or whether it's 3d printing or building something
[1202.94 → 1206.60] out of wood, I, I just, I need to do something.
[1207.02 → 1212.10] Uh, I know home assistant isn't analog technically, but a lot of the stuff it's controlling us.
[1212.22 → 1217.08] So for example, I had to, um, replace the this is a rental house I'm in right now.
[1217.16 → 1222.00] And I replaced the, uh, thermostat controller board thing on the wall that changes the
[1222.00 → 1224.62] the AC and the furnace.
[1225.48 → 1229.94] I replaced that with a nest thermostat that someone was selling cheap locally on Craigslist.
[1230.52 → 1231.62] They found it off the back of a car.
[1231.62 → 1234.00] No, I don't think so.
[1234.20 → 1235.04] In the boot, I should say.
[1235.42 → 1236.70] Uh, in the trunk.
[1237.44 → 1237.80] Yeah.
[1237.80 → 1241.16] I had to learn all about, you know, HVAC wiring over here.
[1241.26 → 1246.64] You know, there's five like wires that do different things and like you just trace one end to the
[1246.64 → 1250.46] control board down in the basement and then there are five wires at the top, the same colour
[1250.46 → 1252.26] and you just figure out which one goes where.
[1253.16 → 1258.44] Um, and for me, it was fascinating because the HVAC unit, like the wire that had been run
[1258.44 → 1262.82] was a five core wire, but only four wires were in use with the old one.
[1263.42 → 1265.92] And someone has just stuffed the fifth one back in the wall.
[1266.16 → 1267.12] And I, so I didn't know it was there.
[1267.18 → 1271.10] So I went to Home Depot and I bought a five core thing, and I was prepared to pull it all through.
[1271.16 → 1274.46] And then I went down to the basement to look at the other end of the wire.
[1274.46 → 1276.58] And I was like, there's a loose wire here.
[1276.94 → 1277.66] Oh shit.
[1277.66 → 1279.34] That's both great.
[1279.46 → 1281.02] And also a bit of a pain in your butt.
[1281.66 → 1281.84] Yeah.
[1281.94 → 1283.90] So I've now got a five core wire sat here.
[1284.02 → 1285.84] I've opened, but I don't know what to do with.
[1286.76 → 1289.04] Um, but I learned a bunch of stuff that, that weekend.
[1289.04 → 1294.34] Uh, like you say, it's, it's that sense of accomplishment that self-hosting and self-building
[1294.34 → 1299.16] and making and all that kind of stuff is, is really, you know, not to be underestimated.
[1299.68 → 1299.92] Yes.
[1300.04 → 1303.08] And I, I just didn't expect that.
[1303.86 → 1306.46] Um, I got into this for practical reasons.
[1306.46 → 1311.94] I wanted to, to really just sort of DE-cloudify the RV and be able to go offline completely.
[1311.94 → 1317.08] So I could go like kind of on a tech diet over a weekend somewhere with no connectivity.
[1317.68 → 1321.56] I guess I just didn't really expect that applying a little bit of craftsmanship to it and taking,
[1321.76 → 1325.54] making it take a little bit longer, but doing it right would give me that much more sense
[1325.54 → 1326.18] of satisfaction.
[1326.94 → 1331.74] Um, and I'm pretty, I'm proud of that system, and I'm really proud of the system we've built
[1331.74 → 1332.96] here at the studio as well.
[1332.96 → 1337.36] Not quite as much craftsmanship, but it's running really well.
[1338.16 → 1341.22] And yeah, we didn't expect like to get that sensation from this.
[1341.30 → 1343.64] I just thought it'd be a practical thing.
[1344.18 → 1348.98] It's, it speaks to the one of the key points of my, uh, Linux Fest Northwest talk this year,
[1349.04 → 1350.44] which is solved a real problem.
[1350.56 → 1350.76] Yeah.
[1350.76 → 1354.98] Because if you do that, you have the motivation to see the project through to the end.
[1355.34 → 1358.28] And then once you've done one, you're like, well, that actually wasn't as hard as I thought
[1358.28 → 1358.80] it would be.
[1359.16 → 1359.86] What else can I do?
[1360.26 → 1364.72] That has helped with Shinobi because to be honest, it's sometimes it's felt a little rickety.
[1364.92 → 1366.88] It feels sort of like it's tossed together.
[1366.96 → 1367.80] It's kind of awkward.
[1367.80 → 1374.54] It has, it has a bunch of different user levels and a super URL that's only used for really
[1374.54 → 1376.54] managing users and restarting services.
[1376.54 → 1383.08] And it's kind of an odd duck, and you need to really kind of follow docs and read community
[1383.08 → 1384.80] threads to, to put it all together.
[1384.80 → 1389.54] I'd run the wires, I'd set up the cameras, I invested all of that time and money.
[1390.16 → 1393.90] And so I just sort of kept plucking at it until I, you know, had whittled it into a setup
[1393.90 → 1395.10] that's mostly good.
[1395.18 → 1401.12] I'm, I'm now going down the route of experimenting with motion detection, which is interesting
[1401.12 → 1407.52] because you take the camera shot that comes in, the GPU processes it, then it sends it off
[1407.52 → 1413.12] at a lower frame rate to FFmpeg, which then analyzes it for motion using a series of NPM
[1413.12 → 1413.60] plugins.
[1414.04 → 1417.20] And then if it detects motion above a threshold that you set.
[1417.36 → 1419.48] So my case, I have them pretty low.
[1419.62 → 1425.88] So if there's 2% motion in the frame, so that's like 2% of the area changes, it triggers motion.
[1426.06 → 1427.72] You can change that to whatever you'd like.
[1427.76 → 1433.40] You can also say if, if it exceeds a certain level of motion, just don't bother, just drop
[1433.40 → 1433.54] it.
[1433.54 → 1439.44] That can be useful with an RTSP feed that has frame drops or like bars across the video
[1439.44 → 1441.62] feed that where you can see there's been some signal loss.
[1441.62 → 1443.78] That you could essentially say ignore.
[1444.14 → 1447.24] If it's just what, if it's essentially the whole frame's changing, something's going
[1447.24 → 1448.10] on, drop that.
[1448.64 → 1452.30] But if it's somewhere between 2% and 70%, record that.
[1452.82 → 1454.04] So that's what I'm doing right now.
[1454.42 → 1456.40] And that uses CPU.
[1456.40 → 1459.76] But I'm saving disk because I'm only recording when there's motion.
[1459.84 → 1462.72] And I have some cameras that see very little activity during the day.
[1463.20 → 1470.54] And getting that just right now is, is like a finessing process because each camera has
[1470.54 → 1474.14] different contents with different lighting and different areas.
[1474.14 → 1478.94] And I can go in Shinobi and I can highlight with boxes exactly the spots I want motion.
[1479.20 → 1483.94] So in some cameras, I have just the windows selected, and the couch is completely out of
[1483.94 → 1484.26] the shot.
[1484.32 → 1486.58] So we can sit there on the couch and not trigger recording.
[1487.22 → 1487.24] Yeah.
[1487.28 → 1488.80] Those zones make a big difference.
[1489.14 → 1489.32] Yeah.
[1489.42 → 1490.92] And saves a lot of disk.
[1491.44 → 1491.84] Yeah.
[1492.24 → 1494.98] Unless you get it too sensitive, and it's just recording all the time.
[1495.02 → 1497.88] Like I did it first and it just blasted my desk.
[1497.88 → 1503.74] I have in my Google photos, I have a period from about three years ago where I started
[1503.74 → 1507.56] messing about with my own cameras for the first time, where every single time my dog
[1507.56 → 1509.76] walks past the camera, I've got a snapshot of my lounge.
[1511.34 → 1512.72] There are thousands of them.
[1513.94 → 1518.58] Hey, so I just listened on my run this morning to last week's Linux Action News, where you
[1518.58 → 1525.84] and Joe talked about ProtonMail and Horde Mail and Squirrel Mail and self-hosting all the mails.
[1525.84 → 1529.84] And to that end, we have a relevant Ask SSH.
[1530.40 → 1530.88] Ah, great.
[1531.14 → 1532.22] Comes from Tom Crouton.
[1532.80 → 1537.70] One of the biggest questions I have is whether I should self-host my own email or use something
[1537.70 → 1539.08] like the mail in a box.
[1539.62 → 1541.38] I've been trying to get away from Google.
[1541.80 → 1542.36] Who hasn't?
[1543.08 → 1544.54] I write a lot of notes.
[1544.70 → 1549.16] I'm not convinced by ProtonMail or others that require you to have their client installed.
[1549.58 → 1551.94] It's quite a long one, so I'll abbreviate.
[1552.62 → 1555.30] Is self-hosting email robust and secure?
[1556.08 → 1557.46] What do you use?
[1558.00 → 1559.08] Is it worth the risk?
[1559.24 → 1563.76] Or would it be better to just pay or use a service that gives away your privacy?
[1565.28 → 1567.28] Why does it have to be this question?
[1568.06 → 1575.28] This is one that I debate in our Jupyter Broadcasting Telegram group frequently.
[1575.74 → 1579.58] Because I am of a dozen mindsets on this.
[1579.58 → 1581.92] Because part of me says, no, don't ever do it.
[1582.00 → 1582.94] It's way too much hassle.
[1582.94 → 1586.40] It's not so much the difficulty in setting up email.
[1586.60 → 1588.20] That can be relatively easy.
[1588.86 → 1592.36] It's that you get so frustrated when you get blacklisted.
[1592.58 → 1594.90] And then your family and friends are affected that are using the service.
[1595.00 → 1596.24] And you have to hunt this thing down.
[1596.48 → 1597.60] And it's so insulting.
[1598.14 → 1600.10] It's so irritating.
[1600.66 → 1601.48] Email's so basic.
[1601.60 → 1603.28] It should just eff work.
[1603.54 → 1603.74] Yeah.
[1603.88 → 1606.46] And what happens, it'll smack you when you least expect it.
[1606.50 → 1608.44] You'll be like seven months, a year into it.
[1608.44 → 1609.14] You'll be busy.
[1609.28 → 1609.92] You'll be travelling.
[1610.06 → 1611.42] You'll be on vacation or whatever.
[1612.02 → 1612.70] And it breaks.
[1613.40 → 1614.94] Eventually, it will happen.
[1615.24 → 1617.32] But that's true of self-hosting almost anything.
[1617.70 → 1621.26] You know, Home Assistant, trust me, will break when you the least want it to.
[1621.34 → 1624.22] When you're, you know, trying to do a demo to your mother-in-law.
[1624.22 → 1630.30] The ramifications, though, of not receiving email can be pretty broad depending on the individual.
[1631.00 → 1631.64] That's a fair point.
[1631.98 → 1634.36] Now, here's another take on it.
[1634.78 → 1640.24] The federated by its basic nature aspect of email is vitally important.
[1640.60 → 1646.10] And I think it's critical that hobbyists continue to self-host email.
[1646.24 → 1650.30] So that way it continues to be even a thing that's possible.
[1650.30 → 1654.90] Because you could see this get locked down so that certain agreements get set up by certain
[1654.90 → 1655.98] commercial carriers.
[1656.24 → 1660.76] And then they have like protected email that passes between their systems.
[1660.86 → 1662.78] And people outside that might have to qualify.
[1663.00 → 1664.66] So I mean, you never know where this could go.
[1665.08 → 1667.76] Don't we kind of have that with WhatsApp and Telegram?
[1667.96 → 1670.58] And aren't they miniature emails in a way?
[1671.00 → 1672.00] Or are they miniature IRS?
[1672.52 → 1674.26] Or are they all just miniature Usenet?
[1674.26 → 1674.66] Mm-hmm.
[1675.46 → 1676.72] They're not decentralized.
[1677.10 → 1682.46] At the core of email is it's a decentralized, anybody can do it protocol.
[1682.98 → 1687.24] Also, it's handy to have a quick way to bounce out emails from systems that do reporting.
[1687.92 → 1689.92] You know, like my Shinobi system.
[1690.20 → 1693.50] It'd be nice to just have a quick little easy way to send out some emails.
[1693.58 → 1694.78] There are several ways to do that.
[1695.00 → 1696.90] But so I've never self-hosted my email.
[1697.46 → 1699.76] It's something that's crossed my mind on more than one occasion.
[1699.76 → 1705.00] But I just, whenever you tap that phrase into Google, should I self-host my email?
[1705.38 → 1708.40] The almost unanimous answer is no.
[1709.52 → 1713.76] Yeah, well, that's because folks like me that set it up for themselves and for friends
[1713.76 → 1717.24] and for family and for companies over the years say, don't do it.
[1717.66 → 1718.10] Yeah.
[1718.28 → 1719.16] Don't do it, Alex.
[1719.42 → 1721.62] Because there's the whole spam blacklisting thing.
[1721.70 → 1725.80] If your server gets compromised, some ISPs don't open certain ports.
[1725.84 → 1727.38] Although these days that's less of an issue.
[1727.38 → 1732.68] Yeah, well, it's difficult to understand how valuable of a target an email server is until
[1732.68 → 1733.38] you run one.
[1733.56 → 1735.04] You don't even have to be a popular one.
[1735.10 → 1736.72] You could have one with a dozen users.
[1737.58 → 1741.62] One of those accounts gets compromised and that server is immediately used for spam.
[1742.12 → 1745.68] It's amazing its speed and efficiency at which these lists work.
[1746.06 → 1747.60] Just takes one weak point.
[1747.70 → 1748.86] Could be in your software stack.
[1749.30 → 1751.50] Could be in a user account.
[1752.02 → 1756.70] So one of the listeners actually replied, Matty McGraw, who I think was our Ask SSH last time.
[1756.70 → 1757.70] Oh, yeah.
[1758.04 → 1763.60] He replied to the Ask SSH, as did you, because this was a while ago, with a link from our
[1763.60 → 1764.80] self-hosted Reddit.
[1766.28 → 1772.48] And the title of the article is, you should not run your own mail server because mail is
[1772.48 → 1772.82] hard.
[1773.84 → 1775.06] You know, lots of stuff is hard.
[1775.12 → 1776.20] That doesn't mean you shouldn't do it.
[1776.40 → 1778.18] I don't actually agree mail is hard either.
[1778.68 → 1783.40] Setting up a basic IMAP server and an SMTP server, that's not hard.
[1783.74 → 1785.00] Think about the price of entry, right?
[1785.00 → 1789.74] So this article claims that he presupposes that you're a sysadmin with tech knowledge
[1789.74 → 1793.60] who knows basic networking, basic protocol knowledge, all that kind of stuff.
[1793.90 → 1794.18] I agree.
[1794.28 → 1795.44] You need to.
[1795.86 → 1801.06] Just to get to zero in this situation actually assumes a lot of basic knowledge.
[1801.84 → 1803.98] And you probably should be a fairly decent one at that.
[1804.44 → 1808.20] So the answer to the question, Tom, is probably not.
[1808.30 → 1812.46] For most people, I would say it's, in my opinion, at least, it's something I've never
[1812.46 → 1812.66] done.
[1812.66 → 1814.16] And I don't have any desire to do it.
[1814.58 → 1815.20] Oh, I kind of do.
[1815.88 → 1817.70] Oh, but Gmail is so easy.
[1817.92 → 1821.06] And I know that's a cop out, and they can mine my data and all that kind of stuff.
[1821.22 → 1825.60] But like you said, the ramifications of email not working, like I'm buying and selling a
[1825.60 → 1826.14] house right now.
[1826.20 → 1829.46] If those contracts can't come through, that's a problem for me.
[1829.68 → 1829.82] Yeah.
[1829.92 → 1830.94] Tax season, it's a problem.
[1830.98 → 1833.22] If I need to get email from the school about the kids, it's a problem.
[1833.32 → 1834.82] I mean, there are a lot of ways it's a problem.
[1834.82 → 1840.58] I would, if I was going to do it, look into what VPS people have had success doing it
[1840.58 → 1840.68] on.
[1840.74 → 1844.92] I don't think I would do it on my home connection unless I had a very kind of special home connection
[1844.92 → 1846.28] or a business connection.
[1846.66 → 1847.42] You raise a good point.
[1847.66 → 1852.44] My Gmail goes back to when I was in lower sixth in England.
[1852.44 → 1856.72] So I guess I was 16, 17 when Gmail was brand new and invite only.
[1857.48 → 1858.40] I think that's 2005.
[1859.14 → 1861.62] So I've got emails in there going way, way back.
[1861.66 → 1865.86] And I've quite often reconstructed portions of my life using my Gmail inbox.
[1866.38 → 1866.78] So has Google.
[1866.98 → 1867.84] Well, there you go.
[1869.16 → 1872.78] Every Amazon purchase, any receipt ever sent to your mailbox.
[1873.54 → 1874.16] Think about that.
[1874.64 → 1881.26] Saying that, I got an email, or it was a targeted Facebook ad the other day, actually, saying,
[1881.26 → 1883.22] Alex, are you missing home?
[1883.58 → 1884.36] British Airways.
[1885.56 → 1886.48] For Christmas.
[1886.92 → 1888.16] Oh, wow.
[1888.60 → 1889.74] I thought that was kind of interesting.
[1890.60 → 1891.98] That's pretty clever.
[1892.48 → 1892.72] Yeah.
[1893.56 → 1895.14] I mean, would you have, maybe you were actually.
[1895.30 → 1897.66] I mean, if you weren't trying to buy a house, you might be, right?
[1898.22 → 1898.50] Yeah.
[1898.74 → 1899.02] Yeah.
[1900.76 → 1905.90] To be honest with you, like targeted advertising is a bit of a double-edged sword, right?
[1905.96 → 1911.14] I mean, on the one side, I don't want to see any ads ever, but in reality, that's
[1911.14 → 1912.12] not the world we live in, is it?
[1912.14 → 1916.20] So I'd rather see an advert about something that's relevant to me than, I don't know,
[1916.44 → 1917.02] shoe polish.
[1917.84 → 1922.16] I don't mind if Amazon wants to review my purchase history with their own servers and then figure
[1922.16 → 1923.22] out what I might be into.
[1923.34 → 1924.86] That doesn't really bother me that much.
[1925.30 → 1930.80] It's more like the total surveillance to try to piece me up into many different markets
[1930.80 → 1931.94] for many different ad purposes.
[1932.12 → 1933.36] That's sort of what bothers me.
[1933.60 → 1933.86] Yeah.
[1933.86 → 1933.90] Yeah.
[1934.34 → 1936.10] I, I don't know.
[1936.16 → 1938.20] I feel like we should set ourselves a challenge.
[1938.66 → 1941.92] We're going to really regret something like this, but like some, something crazy, like
[1941.92 → 1943.08] I don't like where this is going.
[1943.54 → 1950.48] If we make it to 100 episodes to celebrate, we launch our own self-hosted mail server for
[1950.48 → 1951.38] our, for our email.
[1951.60 → 1954.92] We do something, you know, we get our own, like, you know, we could just use our self-hosted
[1954.92 → 1957.00] dot show domain, and we could just have like show at.
[1957.32 → 1959.34] And we'll throw it on the Raspberry Pi seven.
[1959.34 → 1966.04] I just say, maybe we should, someone should hold us accountable to that because we'll
[1966.04 → 1967.06] surely forget that.
[1967.42 → 1968.50] I hope we do forget that one.
[1968.78 → 1969.06] Me too.
[1969.12 → 1974.18] But anyway, I'd say, I'd say consider all of, all the things like do the research
[1974.18 → 1978.50] about where you'll be sending the mail from if it's had issues, because if you can just
[1978.50 → 1983.96] get on a list that an entire block of IPs, like an entire VPS provider can be blocked
[1983.96 → 1986.84] and maybe you've been a good citizen, you've never had a problem.
[1986.84 → 1990.58] But if anyone else in that IP block has, then you're pretty much screwed.
[1990.70 → 1992.86] So you really need to do some due diligence first.
[1993.20 → 1993.32] Yep.
[1993.68 → 1994.88] That's where email is hard now.
[1994.92 → 1996.46] It's not actually setting up the software.
[1997.06 → 1997.38] Totally agree.
[1997.98 → 2002.28] So before we go, I just remember the reason I even went, went to that Best Buy area of
[2002.28 → 2006.56] conversation was to bring up the 12 terabyte easy store hard drive situation.
[2007.26 → 2010.98] Oh, it wasn't to talk about beautiful 75 inch televisions.
[2011.98 → 2013.52] It wasn't to talk about TVs.
[2013.52 → 2020.28] It was to talk about hard drives, $179, I think, right now for a 12 terabyte hard drive
[2020.28 → 2020.92] in the US.
[2021.78 → 2025.94] So yeah, if you're in the market for that kind of thing, you can shuck those drives, do
[2025.94 → 2031.32] the 3.3 volt mod that we talked about last week and get yourselves a darn good hard drive
[2031.32 → 2032.88] for a pretty unbeatable price.
[2033.36 → 2033.52] Yeah.
[2033.66 → 2037.84] Or grab some of those and just set your family up with backups for the holidays.
[2038.14 → 2038.30] Yeah.
[2038.36 → 2040.22] USB hard drives with a Raspberry Pi.
[2040.60 → 2040.96] Why not?
[2041.40 → 2041.88] Why not?
[2041.88 → 2042.48] Right.
[2042.72 → 2044.32] I think it's probably about that time, don't you?
[2044.70 → 2045.56] Oh, all right.
[2046.04 → 2051.18] I really have had a lot of fun setting up these cameras and I can't wait to talk about some
[2051.18 → 2052.30] of the other things we've been working on.
[2052.42 → 2053.80] I know you've got some stuff coming up.
[2053.84 → 2054.28] Oh my gosh.
[2054.30 → 2057.20] Could you imagine the shows we're going to get out of you getting a new place?
[2057.70 → 2058.44] Oh, it's going to be good.
[2058.98 → 2064.64] I'm looking at running a CAT 6A cable so I can do 10 gig Ethernet and all this stuff,
[2064.72 → 2065.68] you know, it's going to be great.
[2065.68 → 2070.22] Oh, I think it might have to take multiple trips, just might have to come down there.
[2070.30 → 2074.28] And maybe the timing, once everything is settled, would be around the spring by coincidence.
[2075.48 → 2078.38] Gosh, I mean, the things I'll have to do for this show next year.
[2078.38 → 2083.44] All I can say is Raleigh in April is, well, actually that's Linux Fest Northwest.
[2083.76 → 2085.58] So March, Raleigh in March is lovely.
[2087.20 → 2088.12] Surprise, surprise.
[2088.52 → 2089.74] Thank you for listening, everybody.
[2090.12 → 2093.12] And you can find me on Twitter at Ironic Badger.
[2093.42 → 2094.60] I'm at Christmas.
[2094.60 → 2099.18] The show is at selfhostedshow along with the show notes at self-hosted.show.
[2099.80 → 2105.56] And you can find more of Jupyter Broadcasting on Twitter at Jupyter Signal.
[2105.96 → 2106.14] Yes.
[2106.42 → 2108.44] Maybe a quick plug for Jupyter Extras.
[2108.58 → 2112.04] We've done some recent extras with the Mergers developer,
[2112.30 → 2116.96] as well as some basics on containers and reverse proxy.
[2117.12 → 2120.78] So extras. Show for additional and supplemental content to this here show.
[2121.04 → 2122.00] So thanks for listening, everyone.
[2122.00 → 2124.90] That was self-hosted. Show slash six.
