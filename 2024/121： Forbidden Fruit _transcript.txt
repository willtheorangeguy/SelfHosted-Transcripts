[0.00 --> 8.72]  1.21 is a special edition of the self-hosted podcast because we're recording this before Alex and I get together at Texas Linux Fest, which is where it all began.
[9.16 --> 15.62]  Oh, yeah. Jeez. Yeah, it is. It's one of those time travel episodes where we're recording like a week and a half early.
[16.52 --> 21.12]  Yeah. Texas Linux Fest. When was that? Must have been 2018, I guess.
[21.32 --> 24.90]  Before times. Yeah. I can't really recall quite, but I was really what kicked it all off.
[24.96 --> 26.80]  I was still a full Brit back then.
[26.80 --> 31.60]  Yes, but I think it was the delicious barbecue that made you decide to really stay.
[31.78 --> 32.48]  Oh, no doubt.
[33.26 --> 42.70]  Now, before we get to our special guest this week, it looks like you got yourself a little piece of hardware, an HDMI extender, but it's an HDMI extender over Ethernet?
[43.38 --> 52.48]  Yes. Now, I've for many years been familiar with the balloon extenders, which let you extend HDMI over a single or a pair of Cat5e cables.
[52.48 --> 61.14]  In fact, when I was a student, I used to put my gaming desktop under the stairs in my student house and run a couple of Ethernet cables up the stairs to my display in my bedroom.
[61.76 --> 65.28]  And that worked fine. But, you know, I'm a little bit past that these days.
[65.28 --> 69.68]  And I want high speed input devices for my actual gaming machine, etc, etc, etc.
[69.68 --> 71.70]  So I ended up not going that route.
[71.90 --> 79.92]  But I have in front of me here the TES Smart or TE Smart, because there's one, two few S's for it to be TES Smart.
[80.46 --> 85.68]  The model number is the HKE12MMA20-RX.
[86.52 --> 87.86]  And there's a dash TX as well.
[87.86 --> 98.56]  And what this does is it broadcasts a 1080p 60 hertz HDMI signal just over your bog standard IP-based network.
[98.62 --> 103.28]  So I can plug this into any Ethernet switch in the house.
[103.66 --> 105.70]  So I've got the transmitter in the basement.
[106.32 --> 110.86]  And then up here in my bonus room, which is a good 300 feet away as the fiber flies,
[111.14 --> 116.32]  I have the receiver and it outputs 1080p as if I was sat in the same spot.
[116.32 --> 118.92]  So it must be encoding it and sending it over IP?
[119.16 --> 120.40]  Oh, yeah, you can definitely tell.
[120.52 --> 124.82]  Like when you look closely at text, you know, you can spot compression artifacts and things.
[125.34 --> 127.80]  Like YouTube videos work totally flawlessly.
[128.06 --> 129.54]  The frame rate's great, 60 hertz.
[129.64 --> 131.40]  Like there's no drop frames or anything like that.
[131.86 --> 134.88]  But if you look closely at static images like text and things,
[134.94 --> 137.32]  like you can definitely tell it's not quite as sharp.
[138.06 --> 139.80]  But I mean, for what this is doing,
[139.80 --> 147.34]  I've actually just put a splitter onto my HDMI KVM switch that I've got down in my server rack down in the basement.
[147.88 --> 150.66]  So I've got one output going to the Pi KVM.
[150.80 --> 155.48]  And then as a backup, I've got this going out to the monitor behind me on my desk,
[155.48 --> 157.02]  which doesn't need a web browser.
[157.16 --> 159.34]  It doesn't need Pi KVM to be up or whatever.
[159.34 --> 163.20]  And it does USB HID device pass-through.
[163.28 --> 165.32]  So I can connect a keyboard or mouse to this receiver.
[165.62 --> 169.10]  And it can tune into any one of up to 16 different channels.
[169.20 --> 171.42]  So I could actually have 16 different transmitters
[171.42 --> 176.52]  and up to, I think, 200 and something different receivers tuned into different channels.
[176.70 --> 180.40]  So, you know, in the old days, this would have been suitable for like a TiVo box.
[180.44 --> 183.18]  And then you tune it into multiple different rooms, that kind of thing.
[183.18 --> 184.64]  That is really cool.
[184.86 --> 196.20]  I, for a very brief period of time, one of my all-time best setups was I had a KVM console at my cubicle desk.
[196.42 --> 201.26]  So I could just turn around and actually work at the console of the server.
[201.80 --> 205.06]  And man, was that so great.
[205.28 --> 205.38]  Yeah.
[205.48 --> 207.60]  I love what you're putting down right now.
[207.60 --> 211.50]  Like I could put one of these on each one of the servers,
[211.50 --> 213.58]  although I don't think any of them do HDMI out.
[214.00 --> 217.12]  But in theory, if they did, I could put one of these on each one of the servers,
[217.58 --> 221.02]  have one receiver in my office, and then I could just toggle between them.
[221.50 --> 222.18]  Yeah, absolutely.
[222.42 --> 222.86]  That's cool.
[223.18 --> 226.30]  The only downside would be that each unit is about $60 or $70.
[226.78 --> 228.20]  That seems fair, though, for what it's doing.
[228.56 --> 228.86]  Yeah.
[229.20 --> 229.56]  Yeah.
[229.98 --> 231.90]  It feels about right to me, to be honest.
[232.30 --> 236.50]  If it was at the sort of $30, $40 price point, then it would just be total no-brainer.
[236.60 --> 241.00]  But with it being $70, it's kind of at that, I just need to think twice territory.
[241.00 --> 244.22]  But how does it handle the post-process when the machine's booting up
[244.22 --> 246.08]  and the resolution is flickering and changing?
[246.20 --> 248.00]  Any weirdness with any of that stuff so far?
[248.24 --> 251.64]  Well, I've only tested it with my Blue Iris box, which is running Windows,
[251.98 --> 254.06]  and it's in an HP 290 Slim.
[254.32 --> 256.28]  And it seems to handle that just fine.
[256.36 --> 260.78]  I haven't actually gone into the BIOS, so maybe I will try that.
[260.82 --> 262.36]  And if there's any issues, I'll report back.
[263.10 --> 265.14]  But so far, so good with this thing.
[265.14 --> 269.28]  You know, I left it on for 24 hours just as a test, the monitor behind me,
[269.40 --> 271.00]  and it worked perfectly.
[271.60 --> 273.28]  Well, I think you're spending my money again, Alex.
[273.38 --> 274.74]  I kind of want one of those.
[274.80 --> 275.92]  I'll just try to grab a link from you.
[277.80 --> 280.12]  Well, I'm delighted to welcome to the show Casey Liss.
[280.16 --> 285.08]  You may well know him from Accidental Tech Podcast, or ATP, if that's your preference.
[285.60 --> 286.38]  Welcome to the show, Casey.
[286.76 --> 287.38]  Well, hello.
[287.62 --> 288.28]  Thank you for having me.
[288.30 --> 289.22]  I'm so excited to be here.
[289.22 --> 295.66]  We're on video talking to you today, and this is one of those moments where I've listened to you for so many years,
[295.82 --> 297.38]  and now I see you talking.
[297.50 --> 298.44]  It's kind of weird.
[298.78 --> 300.26]  Yeah, it messes up your mind.
[300.36 --> 300.96]  I've been there.
[301.06 --> 304.02]  I've been on the other side of this, and it is very, very odd.
[304.28 --> 306.90]  I almost said awkward, but I don't know if awkward is the right word for it.
[306.92 --> 307.72]  That's also very negative.
[307.80 --> 308.88]  It's just unusual.
[309.34 --> 313.64]  And plus, in all likelihood, I probably sound drunk because I'm talking slower than, you know,
[313.64 --> 316.52]  the 3X that everyone seems to listen to podcasts in.
[316.52 --> 320.74]  And so I sound like, you know, I'm talking so incredibly slowly as compared to normal.
[320.88 --> 322.18]  So I totally understand.
[322.80 --> 323.92]  I'm a 1Xer myself.
[324.12 --> 325.40]  I just, I can't do it.
[325.70 --> 326.40]  I can't do it.
[326.46 --> 329.36]  It just, it feels like I'm on too many caffeine shots for the day.
[330.24 --> 331.36]  Gives you anxiety, right?
[331.54 --> 331.98]  Right, right.
[333.30 --> 336.44]  Casey, I knew what you looked like because I've been following you on social media for a bit.
[336.92 --> 339.82]  And so I also have been following that you got at Apple Vision Pro.
[339.90 --> 342.90]  So later on in the show, we'll be talking to you about that.
[342.90 --> 347.20]  But towards the beginning, we thought we should probably stay on topic and talk a little self-hosting.
[347.30 --> 354.10]  And if anybody's listened to ATP, they know that you are really our brother and kin there when it comes to self-hosting.
[354.14 --> 359.10]  Because I've heard you mention things like garage door sensor automations and Raspberry Pis.
[359.36 --> 361.50]  So I think that's probably where we should start, Alex.
[361.90 --> 362.44]  Yes, sir.
[362.52 --> 365.30]  So talk us through a little bit what you've got running in the house, Casey.
[365.30 --> 368.32]  I know that typically with ATP, it's Apple focused.
[368.32 --> 371.32]  But like Chris just said, you've got a bunch of stuff running locally.
[371.42 --> 373.30]  Are you a home assistant guy or?
[373.86 --> 375.32]  Oh, you're starting off tough.
[375.40 --> 375.98]  I see how it is.
[376.02 --> 377.04]  I thought this was going to be friendly.
[377.24 --> 377.62]  No.
[377.78 --> 381.66]  So I tried home assistant years ago.
[381.84 --> 385.84]  This was easily like three, maybe four or five years ago.
[385.84 --> 392.10]  And at the time, the way it thought and the way I thought were just polar opposites.
[392.16 --> 394.72]  It doesn't mean home assistant was bad or wrong or anything like that.
[394.92 --> 396.72]  It's just I could not wrap my head around it.
[396.72 --> 402.74]  And I think it's because what I went into home assistant wanting was I just want a bridge
[402.74 --> 405.84]  to get non-home kit stuff into home kit.
[406.10 --> 407.74]  And so you can guess where this is going.
[407.90 --> 409.64]  I quickly realized this was not for me.
[409.78 --> 411.60]  And so what I need is just home bridge.
[411.66 --> 412.94]  And I've been running home bridge for forever.
[413.02 --> 418.74]  And in fact, home bridge and pie hole were the two things that got me started on doing
[418.74 --> 420.50]  any sort of home lab sort of thing.
[420.66 --> 422.40]  I don't recall which came first.
[422.66 --> 426.66]  It was possibly home bridge, but I don't have a strong memory one way or the other.
[426.72 --> 430.04]  But I wanted to do, you know, I wanted to get stuff on home kit.
[430.10 --> 431.52]  And so I started running home bridge.
[431.74 --> 434.70]  And if memory serves, I've always run home bridge and Docker.
[434.88 --> 438.88]  So that was my first adventure into containerization and things of that nature.
[439.36 --> 443.12]  My professional background is I did a lot of web development for a long time.
[443.22 --> 448.00]  But I got out of that right around the time, like Docker and Kubernetes and all that sort
[448.00 --> 449.12]  of thing started coming up.
[449.16 --> 451.60]  And so I never really had an excuse to learn any of it.
[451.60 --> 454.56]  And then I moved to iOS development and podcasting and whatnot.
[454.78 --> 457.68]  And so, again, I haven't really had a lot of excuses to do that sort of thing.
[457.98 --> 461.32]  But I taught myself how to at least be dangerous with Docker.
[461.76 --> 465.62]  And I was running and I was and am running home bridge.
[465.98 --> 468.46]  And then pie hole, I started also in Docker.
[468.56 --> 470.66]  And we can talk about where this was all happening.
[470.74 --> 472.14]  But anyways, that started in Docker.
[472.62 --> 473.48]  Actually, that's a perfect segue.
[473.56 --> 477.64]  Come to think of it, because I was running all this on an old Synology DS 1813 plus.
[477.64 --> 479.10]  I'm a huge Synology super fan.
[479.60 --> 484.46]  And that machine very well could have been user error, but it did not cooperate well
[484.46 --> 485.32]  with IPv6.
[485.72 --> 487.20]  And this was right.
[487.28 --> 491.18]  This was four or five years ago now, three or four years ago, where IPv6 was really starting
[491.18 --> 493.72]  to become an actual thing rather than a hypothetical thing.
[494.28 --> 497.34]  And so I, well, maybe in theory.
[497.66 --> 504.88]  And so anyway, so I moved the pie hole onto a dedicated Raspberry Pi 3B, I think.
[504.94 --> 505.56]  I might have that wrong.
[505.56 --> 509.36]  But I got a Raspberry Pi right before nobody could get a Raspberry Pi, because this was
[509.36 --> 510.68]  like shortly pre-pandemic.
[511.16 --> 514.42]  And that's running raw on the metal there.
[514.60 --> 518.08]  And then over time, I started realizing, well, this Docker thing works out real well.
[518.40 --> 519.68]  I can put other stuff in there.
[519.78 --> 525.04]  Although I don't run Plex or Channels, which I'm a super fan of both of those in a container.
[525.18 --> 528.56]  I do run both of those on a Mac Mini that I have in the house.
[528.86 --> 531.20]  I have the Raspberry Pi running pie hole.
[531.40 --> 533.24]  And I was running Pi VPN.
[533.24 --> 536.88]  And then I found that I was having a little bit of problems with WireGuard.
[536.98 --> 539.38]  And I thought, man, if only there was a way to do WireGuard easily.
[539.98 --> 541.04]  And I discovered this thing.
[541.10 --> 542.18]  I don't know if either of you have heard of it.
[542.26 --> 543.30]  It's called TailScale.
[543.44 --> 544.48]  And it's really good.
[544.58 --> 545.54]  You should check it out sometime.
[546.02 --> 547.28]  Have you ever seen QI?
[547.92 --> 551.40]  Because I feel like at the moment, the klaxons would be going off behind us.
[551.40 --> 551.56]  I know, right?
[552.68 --> 553.98]  I was not put up for that.
[554.04 --> 555.26]  I was not put up to say any of that.
[555.44 --> 556.20]  That's just well done.
[556.92 --> 558.52]  It just comes up naturally sometimes.
[558.52 --> 561.30]  So the Pi still remains in service running pie hole?
[561.74 --> 562.06]  It does.
[562.14 --> 562.88]  It's running pie hole.
[563.12 --> 567.40]  And a couple, like when I need to do a cron job for something silly, that's typically where I'll do it.
[567.40 --> 568.36]  Because, you know, why not?
[568.94 --> 572.34]  I upgraded my Synology to, shoot, what is that?
[572.42 --> 576.10]  It's a six bay from 2021?
[577.20 --> 577.44]  2021?
[577.84 --> 578.28]  So what is that?
[578.38 --> 580.66]  A DS something 621?
[580.82 --> 582.40]  I forget the name or the model off the top of my head.
[582.44 --> 583.50]  I'm very embarrassed now.
[583.52 --> 585.48]  But anyways, it's a six bay instead of an eight bay.
[585.48 --> 588.98]  Because, you know, hard drives have gotten bigger and it's quite a bit more powerful.
[589.16 --> 594.50]  This is before Synology got real aggressive about using Synology branded hard drives, which I really don't love.
[594.70 --> 595.26]  Boo, hiss.
[595.40 --> 596.72]  Yeah, I don't like that at all.
[596.82 --> 601.50]  I'm a Synology super fan with an asterisk because I really don't love that whole thing.
[601.76 --> 603.92]  And so I'm running a bunch of containers on there.
[603.92 --> 609.18]  But to come back to Home Assistant, I feel like I need a Home Assistant like guide.
[609.48 --> 611.12]  Because like not in terms of text.
[611.18 --> 614.80]  I mean, I need someone to like hold my hand and show me this is the way.
[614.80 --> 618.26]  Because everyone I speak to who's ever run Home Assistant swears by it.
[618.44 --> 620.72]  I was actually just earlier today not in prep for the show.
[620.82 --> 621.62]  I swear this is organic.
[621.88 --> 627.92]  I was watching one of Alex's videos with regard to tail scale and reverse proxies and something else.
[628.04 --> 633.20]  But it involved Home Assistant doing things that Home Assistant, in my opinion, had no business doing.
[633.36 --> 634.88]  But yet it did it really, really well.
[635.24 --> 636.94]  It was something with reverse proxies and whatnot.
[637.10 --> 639.30]  I think it was the most recent video on YouTube as we speak.
[639.58 --> 644.16]  But one way or the other, I feel like Home Assistant would be my kind of crap.
[644.16 --> 646.10]  I just haven't had it click yet.
[646.28 --> 649.88]  So somebody needs to come and hold my hand and show me the way.
[650.38 --> 652.70]  Home Assistant's really interesting because it can be.
[653.12 --> 659.36]  So if you're running Home Assistant OS, you can use it like a platform to run other self-hosted applications.
[659.48 --> 660.52]  Like it has an app store.
[660.68 --> 660.94]  Oh, wow.
[661.00 --> 665.30]  There's lots of other things in this space that do a similar job like CUS OS.
[665.94 --> 666.98]  There's Umbral 2.
[666.98 --> 673.72]  Unraid, of course, is the MVP in the original sort of self-hosted app store NAS type situation.
[674.16 --> 675.70]  Synology, of course, does it too.
[676.28 --> 681.86]  But what's interesting about Home Assistant is that it's all open source and all the add-ons are community maintained and all the rest of it.
[681.92 --> 686.96]  Like even the tail scale add-on in Home Assistant is actually maintained by Frank, who's one of the core developers of Home Assistant.
[687.26 --> 687.86]  That's super cool.
[688.28 --> 690.16]  So tail scale doesn't actually touch it.
[690.16 --> 692.84]  Although we do work with Frank sometimes.
[693.26 --> 693.84]  Yeah, it's incredible.
[694.28 --> 702.92]  I'd also like to know, Casey, what you use HomeBridge for today because it feels like maybe that's solving 90% of your use cases right now.
[703.14 --> 703.46]  Yeah.
[703.58 --> 708.66]  I mean, like I said, I don't do a whole bunch of advanced stuff with HomeBridge specifically.
[709.18 --> 714.40]  And so generally speaking, HomeBridge is just get me something like a Wemo device onto HomeBridge.
[714.50 --> 716.34]  Actually, I have a physical bridge for that, come to think of it.
[716.36 --> 717.28]  But that's sort of a thing.
[717.28 --> 719.18]  Get me something that isn't on.
[719.18 --> 720.62]  So lights, audio.
[721.14 --> 722.82]  And actually, this is a good segue.
[723.00 --> 723.80]  I don't know if it was intentional.
[724.08 --> 725.04]  I'll believe it was.
[725.08 --> 729.32]  It's a good segue into my Bananas garage door setup, which is early in 2020.
[730.54 --> 731.50]  Everyone's locked at home.
[731.60 --> 732.66]  I needed a pandemic project.
[732.66 --> 734.14]  And I thought, you know what I can do?
[734.20 --> 737.22]  I can figure out a way to detect whether or not my garage door is open.
[737.30 --> 738.82]  So at bedtime, I won't leave it open.
[739.30 --> 744.16]  And any normal human would have done like a Chamberlain MyQ, which I had used at some point.
[744.16 --> 747.88]  And I forget why I stopped using it, but this was before it kind of got cruddy.
[747.88 --> 752.08]  Probably because whenever you want to close that door, it does that annoying like five
[752.08 --> 755.04]  second wait and then blinks at you eight million times.
[755.14 --> 755.86]  Like, are you sure you?
[756.10 --> 757.72]  Yeah, just close the damn door thing.
[757.80 --> 758.18]  Come on.
[758.26 --> 758.82]  Just close the door.
[758.94 --> 759.90]  I said close the door.
[759.98 --> 761.12]  Just close the door.
[761.22 --> 761.38]  Yes.
[761.48 --> 766.30]  So anyway, so I decided that the only reasonable way to detect whether or not your garage door
[766.30 --> 770.86]  was open, this clearly there's no simpler way to do this, is to get two Raspberry Pi
[770.86 --> 772.06]  zero W's.
[772.24 --> 774.20]  So Wi-Fi enabled Raspberry Pi's.
[774.26 --> 777.66]  Oh, WH's, strictly speaking, because it had the header pins already soldered to it.
[778.02 --> 784.06]  And I put one down above the garage door with, I forget the name of the thing, but a sensor
[784.06 --> 789.06]  where if there's two panels, like two little contacts next to each other, it's either open
[789.06 --> 790.74]  or closed, depending on how you buy it.
[791.04 --> 792.08]  Magnetic read switch?
[792.32 --> 793.70]  Yes, a read switch might be it.
[793.74 --> 794.38]  Yeah, yeah, I think you're right.
[794.72 --> 796.04]  I can never remember the darn name of it.
[796.08 --> 798.86]  But anyways, so you have these two things, and I have one at the top of the garage door
[798.86 --> 801.72]  and one, you know, right on the frame of the house.
[802.22 --> 806.58]  And when they're, you know, physically close to each other, then the circuit is either closed
[806.58 --> 806.86]  or open.
[806.94 --> 807.68]  I forget off the top of my head.
[808.00 --> 813.80]  And so this zero W is via, you know, the Raspberry Pi GPIO is reading the state of that
[813.80 --> 814.18]  switch.
[814.36 --> 816.80]  And then it's periodically broadcasting via UDP.
[817.18 --> 819.32]  Okay, the garage is open, the garage is closed, so on and so forth.
[819.70 --> 820.76]  And that was fine.
[820.76 --> 826.10]  And then I had a different Pi Zero W, even though they're separated literally by the
[826.10 --> 827.96]  floor of the primary bedroom and nothing else.
[828.08 --> 829.86]  I could have run a wire if I really felt like it.
[829.86 --> 831.30]  But why would you do that when UDP exists?
[831.74 --> 838.40]  And so I had a second Pi Zero W H up in the bedroom, and that is wired to an LED.
[838.92 --> 843.96]  And it slurps up these UDP broadcasts and says, oh, the garage door's open, light up the
[843.96 --> 844.24]  LED.
[844.78 --> 847.58]  And so the LED, the red LED is illuminated when the garage door's open.
[847.58 --> 849.62]  And then it is turned off when the garage door's closed.
[850.00 --> 854.34]  And then I thought, well, hell, if I've already got this in Home Assistant, why not run a web
[854.34 --> 854.66]  server?
[854.84 --> 857.96]  And a web server can ping that same garage door Raspberry Pi.
[858.14 --> 859.90]  And then you can run in HomeBridge.
[859.98 --> 860.84]  This is what made me think of it.
[861.06 --> 865.50]  In HomeBridge, you can have a accessory that acts as garage door and just makes HTTP requests.
[865.86 --> 867.78]  And I'm sure that Home Assistant could do the same thing.
[867.78 --> 871.92]  I don't think any of this is particularly advanced or novel, but I was using the tools in front
[871.92 --> 872.12]  of me.
[872.20 --> 877.20]  And so now I have this cockamamie setup where I have the garage door Raspberry Pi just
[877.20 --> 880.24]  detecting whether the garage door is open or not and broadcasting UDP signals and running
[880.24 --> 880.80]  a web server.
[880.98 --> 885.52]  Then I have the primary bedroom Raspberry Pi slurping up the UDP and illuminating an LED.
[886.26 --> 890.34]  And then I also have HomeBridge running in a Docker container on the Synology because it
[890.34 --> 891.44]  isn't confusing enough yet.
[891.44 --> 896.06]  And that's pinging away at the garage door Raspberry Pi constantly asking, is the garage
[896.06 --> 896.36]  door up?
[896.38 --> 896.96]  Is the garage door up?
[896.98 --> 897.58]  Is the garage door up?
[897.60 --> 901.54]  And then notifying HomeBridge, or I guess HomeBridge, strictly speaking, is doing the
[901.54 --> 905.42]  pinging and it is letting me know whether or not the garage door is open.
[905.42 --> 910.34]  Oh, and then just to really beat this horse completely into the afterlife, I decided, you
[910.34 --> 910.64]  know what?
[911.00 --> 915.34]  I really am concerned about the physical security of my garage door for reasons, even though I
[915.34 --> 918.04]  live in like a completely vanilla suburb of Richmond, Virginia.
[918.50 --> 918.76]  Nevertheless.
[918.76 --> 923.52]  And so there's this app on the Mac called Swift Bar, which is like a reincarnation of BitBar.
[923.94 --> 928.38]  What that lets you do is put stuff on the menu bar up on the top of the Mac screen.
[928.50 --> 930.80]  This is kind of like the, what was it, the bottom right of Windows?
[930.92 --> 931.52]  I can't remember the name.
[931.54 --> 932.04]  SysTray.
[932.46 --> 932.78]  SysTray.
[932.78 --> 933.02]  Yeah, yeah.
[933.02 --> 933.34]  Thank you.
[933.62 --> 935.56]  And so you can put custom stuff up there.
[935.64 --> 940.54]  And so now I have a little bespoke garage door icon sitting on the top of my screen, letting
[940.54 --> 942.30]  me know if the garage door is open or closed.
[942.30 --> 946.36]  Like it literally has like the frame of the garage door when it's open and it's empty.
[946.36 --> 950.10]  And then it has the frame of the garage door with the garage door in it when the garage
[950.10 --> 950.74]  door is closed.
[950.74 --> 956.20]  So I will always flip and know if my garage door is open one way or the other.
[956.24 --> 957.22]  It is bananas.
[957.46 --> 959.64]  I'd say that definitely makes you a home assistant guy.
[959.80 --> 960.46]  Yeah, I think that.
[960.82 --> 963.96]  That's the thing is I feel like this probably could have been accomplished way easier in
[963.96 --> 964.40]  home assistant.
[964.58 --> 969.42]  Now, no regrets because I needed something to do with my darn hands during the early days
[969.42 --> 969.96]  of the pandemic.
[969.96 --> 974.40]  But I will be the first to tell you this is a banana setup that is probably eight times
[974.40 --> 975.94]  more complicated than I needed it to be.
[976.36 --> 979.26]  I hope you filed a patent with Rube Goldberg before you set that up.
[979.66 --> 980.40]  I should have.
[980.46 --> 981.20]  I should have looked into that.
[981.28 --> 981.84]  You're exactly right.
[982.24 --> 986.06]  You know, what's interesting is there is a project in home assistant, which maybe if
[986.06 --> 990.24]  this Raspberry Pi thing ever, one of those many things ever go sideways, you might want
[990.24 --> 990.84]  to look into.
[991.80 --> 993.52]  ESPHome will do the trick for you as well.
[993.58 --> 996.28]  So you define in YAML a small piece of configuration.
[996.28 --> 1000.56]  It spits out an ESP8266 firmware bin file.
[1000.66 --> 1005.82]  You flash that onto the device and it will read the pinouts of read switches and all
[1005.82 --> 1006.38]  that's super cool.
[1006.62 --> 1007.32]  All sorts of stuff.
[1007.40 --> 1008.08]  So yeah, just take a look.
[1008.14 --> 1009.84]  ESPHome, you might find it useful.
[1010.10 --> 1010.70]  I should do that.
[1010.82 --> 1014.22]  That's the thing is I need you to just come, what are we, three, three and a half hours
[1014.22 --> 1014.46]  apart.
[1014.72 --> 1018.76]  I just need you to come visit and like hold my hand and show me the way when it comes
[1018.76 --> 1021.44]  to home assistant because I feel like I'm a stiff breeze away.
[1021.44 --> 1026.18]  GetGrist.com slash self-hosted.
[1026.40 --> 1031.50]  Grist is the open source alternative to Airtable and Google Sheets.
[1031.88 --> 1036.80]  It's fantastic and you Excel expats are going to appreciate the many Excel functions that
[1036.80 --> 1041.00]  are supported and the fact that Grist supports granular user access rules.
[1041.54 --> 1046.02]  You can limit read right to individual rows, columns and event tables.
[1046.26 --> 1048.18]  It's really something you've got to go see.
[1048.28 --> 1050.82]  So go to GetGrist.com slash self-hosted.
[1050.82 --> 1057.08]  They have full Python syntax supported and even an AI formula assistant to help you write
[1057.08 --> 1058.16]  those Python formulas.
[1058.68 --> 1063.04]  And I think one of the best things, it's portable, it's self-contained format is all based on SQL
[1063.04 --> 1065.14]  light and you can host Grist as well.
[1065.36 --> 1070.62]  It's easy to integrate as well because it has a REST API and there's a lot of popular integrations
[1070.62 --> 1072.52]  ready to go right now.
[1072.60 --> 1076.82]  You know, some of the popular ones out there, then they probably already have a Grist integration
[1076.82 --> 1080.26]  and it goes beyond just being open source, right?
[1080.26 --> 1082.02]  Because that's fantastic.
[1082.14 --> 1082.62]  That's good.
[1082.86 --> 1084.20]  But what does that mean contribution wise?
[1084.30 --> 1088.56]  Well, one of the contributors to the project is the French government who uses Grist for
[1088.56 --> 1090.02]  thousands of employees.
[1090.26 --> 1091.72]  They did try the others.
[1091.84 --> 1095.12]  They tried everything and Grist was the best.
[1095.86 --> 1098.52]  Grist is the open source alternative you can host.
[1098.82 --> 1102.24]  So go try it at GetGrist.com slash self-hosted.
[1102.24 --> 1106.84]  It's a much better approach and it's the open source alternative to the other big guys.
[1107.22 --> 1108.74]  Check it out and support the show.
[1109.20 --> 1113.10]  GetGrist.com slash self-hosted.
[1113.24 --> 1115.74]  GetGrist.com slash self-hosted.
[1115.74 --> 1120.58]  That just there was a beautiful moment for me as a Brit living in America.
[1120.58 --> 1124.96]  So the British audience right now will be appreciating that Casey just hand waved a three
[1124.96 --> 1126.98]  and a half hour drive away as if it's nothing.
[1128.74 --> 1129.60]  Yeah, it is nothing.
[1129.78 --> 1130.16]  In England.
[1130.48 --> 1131.98]  That's like a weekend trip.
[1132.06 --> 1134.30]  You've got to pack all sorts of snacks in the car.
[1134.56 --> 1134.64]  Right.
[1134.64 --> 1135.80]  Yeah, it's a big deal.
[1135.94 --> 1138.86]  So, well, it's funny you say that because I'm in the suburbs of Richmond, right?
[1138.96 --> 1144.34]  And downtown Richmond is on a bad day, half an hour away, maybe.
[1144.88 --> 1147.62]  And it's funny because I didn't grow up here.
[1147.70 --> 1149.42]  I moved here after college.
[1149.56 --> 1150.84]  I'm sorry, Alex, university.
[1151.34 --> 1156.84]  And so I came after college and I'm in like, you know, the yuppie area of Richmond.
[1157.26 --> 1160.24]  And Erin, my wife, makes merciless fun of me.
[1160.24 --> 1165.88]  She grew up here, makes merciless fun of me for how just beleaguered I am or aggrieved
[1165.88 --> 1168.22]  I am when she asks to do something downtown.
[1168.38 --> 1170.38]  Oh, do we have?
[1170.46 --> 1171.32]  It's so far.
[1171.34 --> 1172.26]  It's 20 minutes, y'all.
[1172.34 --> 1172.84]  20 minutes.
[1173.10 --> 1174.48]  It's so far.
[1174.56 --> 1175.98]  Why can't we just stay around here?
[1176.10 --> 1181.08]  I don't know what my issue is, but I will complain and moan for an hour about a 20 minute
[1181.08 --> 1181.36]  drive.
[1181.42 --> 1182.54]  And yes, you're exactly right.
[1182.58 --> 1185.88]  I will literally wave my hand and say three and a half hours is nothing.
[1185.88 --> 1190.88]  Well, when I lived in London, it was always, so I've got this theory that like cities have
[1190.88 --> 1191.78]  this time.
[1191.96 --> 1195.12]  So in Raleigh, everywhere is 15 or 20 minutes away from everywhere else.
[1195.78 --> 1196.86]  In London, it was an hour.
[1196.98 --> 1198.04]  It didn't matter where you went.
[1198.12 --> 1199.42]  It was always an hour.
[1199.74 --> 1201.68]  So Richmond's time is clearly 20 minutes.
[1202.06 --> 1202.42]  Yep.
[1202.50 --> 1204.70]  About roughly, unless you're going to an extreme end.
[1204.78 --> 1207.96]  But yes, your point is completely fair, completely noted and completely accurate.
[1208.48 --> 1211.78]  Now, on your rundown there, Casey, there was one thing you said that I wanted to kind of
[1211.78 --> 1213.22]  dig into a little bit more.
[1213.22 --> 1216.40]  And you mentioned, and I've heard you mentioned this on your show too, that you're running
[1216.40 --> 1218.58]  Plex on a Mac mini.
[1218.70 --> 1219.80]  Could you go into more detail there?
[1219.84 --> 1221.80]  Is this a headless Mac mini?
[1222.14 --> 1227.22]  Is it connecting to the Synology storage through a network storage share somehow?
[1227.54 --> 1230.44]  Yeah, everyone knows that person with like 85,000 movies in Plex, right?
[1230.72 --> 1232.62]  And so my media collection is not 85,000 movies.
[1232.74 --> 1237.08]  But actually, I can tell you by way of my fancy fancy get homepage, which is another package
[1237.08 --> 1238.80]  I run on Docker.
[1239.00 --> 1240.12]  I have, where is it?
[1240.56 --> 1244.44]  1,311 movies and 125 TV shows, which is not insignificant.
[1244.76 --> 1250.22]  But I mean, I am Plex pals, if you will, with people that have like literally 10 times the
[1250.22 --> 1251.00]  amount of media I have.
[1251.58 --> 1253.48]  So anyway, so I take it seriously enough.
[1253.56 --> 1258.62]  And I share with enough friends and family that I want to be able to transcode stuff and
[1258.62 --> 1260.58]  do that without having to stress about it.
[1260.94 --> 1263.86]  Not that I'm running, you know, my own personal private Netflix.
[1263.86 --> 1267.70]  It's just, if I'm somewhere else and I want to be able to transcode something, I want
[1267.70 --> 1268.80]  to be able to freaking transcode something.
[1268.88 --> 1269.56]  I have two small children.
[1270.06 --> 1274.16]  And although they are very good children and very patient, they do not love it when there's
[1274.16 --> 1276.58]  a media related problem with my infrastructure.
[1277.42 --> 1279.08]  It doesn't feel good as a dad either.
[1279.30 --> 1279.62]  Yeah, exactly.
[1279.74 --> 1281.10]  They're not happy as a dad.
[1281.18 --> 1281.82]  You're not happy.
[1281.82 --> 1282.54]  Yeah, I'm not happy.
[1283.14 --> 1285.12]  My wife's looking at me like, this is your thing.
[1285.42 --> 1286.64]  How did you get this wrong?
[1287.12 --> 1289.22]  But I'm painting her as though she's mean.
[1289.32 --> 1289.90]  She's wonderful.
[1290.78 --> 1293.68]  But anyway, so the point is, I wanted to be able to transcode well.
[1293.68 --> 1297.84]  And I started this journey, I believe I was running Plex as an app, to Alex's point earlier,
[1298.02 --> 1299.82]  as an app on the old Synology.
[1300.24 --> 1303.36]  And it was all well and good until transcoding was required.
[1303.54 --> 1304.90]  And then it just coughed all over itself.
[1305.22 --> 1307.16]  And that quickly became untenable.
[1307.34 --> 1311.14]  And so at this point, I was running an iMac Pro as my primary machine.
[1311.56 --> 1313.38]  And so I moved Plex to be on there.
[1313.64 --> 1317.66]  But I didn't absolutely love Plex living on my primary computer.
[1317.90 --> 1319.84]  And so then I thought, okay, well, what can I do here?
[1320.26 --> 1325.98]  At the same time, a friend of mine who works at Mac Stadium, they're a Mac Mini co-location
[1325.98 --> 1326.38]  place.
[1326.56 --> 1331.06]  And so you can literally grab a Mac Mini and either send it to them, or they can buy one
[1331.06 --> 1333.96]  on your behalf and load it into their, I think it's a Las Vegas data center.
[1334.40 --> 1337.90]  And they had an old Intel Mac Mini that they were literally just going to throw away.
[1337.98 --> 1339.22]  And he was like, hey, I'll send it to you if you want.
[1339.28 --> 1340.66]  And that became my Plex server for a while.
[1340.66 --> 1344.70]  And then the Apple Silicon transition happened.
[1344.80 --> 1347.66]  And I was like, well, I don't want this old and creaky Intel thing in my house.
[1347.72 --> 1348.42]  I'm too good for this.
[1348.52 --> 1348.88]  Excuse me.
[1348.96 --> 1349.52]  Thank you very much.
[1349.86 --> 1352.76]  And so I got a refurb M1 Mac Mini.
[1352.88 --> 1355.82]  And that's running Plex, which everyone is probably familiar with.
[1356.22 --> 1359.14]  And Channels, which I don't know how much you fellas know about this.
[1359.18 --> 1364.36]  But Channels is a really incredible app for a very specific set of problems.
[1364.58 --> 1367.56]  So I believe the website is getchannels.com, if I'm not mistaken.
[1367.56 --> 1374.18]  And Channels, it's basically a network or a replacement, a software DVR,
[1374.40 --> 1376.64]  which in and of itself doesn't sound that remarkable.
[1376.64 --> 1380.86]  But what's really great about Channels is that it has incredible support for HD Home Run,
[1381.00 --> 1385.54]  which is a physical device that you can either hook up to an antenna
[1385.54 --> 1387.02]  so you can get like over the air broadcast.
[1387.44 --> 1391.68]  Or what I've eventually graduated to is you can get a cable card,
[1391.80 --> 1393.94]  which is a thing still to this day.
[1394.02 --> 1394.80]  I swear it's a thing.
[1394.80 --> 1399.02]  And if they are PCMCIA cards, or if not literally, then they look just like them.
[1399.08 --> 1401.28]  And that's an acronym you haven't heard in 15, 20 years.
[1401.78 --> 1405.10]  But anyways, you can get a cable card and hook it up to a particular kind of HD Home Run.
[1405.46 --> 1410.62]  And Channels will slurp up and record TV shows right off of your cable connection.
[1410.98 --> 1411.98]  And that's what I do.
[1412.04 --> 1413.24]  You know, we have Verizon Files here in Richmond.
[1413.70 --> 1418.04]  And I have a coax line running to my left as I sit here in the office.
[1418.30 --> 1421.88]  I have a coax line running into the HD Home Run with a cable card in it.
[1421.88 --> 1423.28]  And that's how we record stuff.
[1423.52 --> 1426.46]  And Channels becomes my DVR.
[1426.66 --> 1429.38]  And then if things are something that I think is worth keeping,
[1429.86 --> 1432.92]  then I'll slurp that into Final Cut Pro, take out the commercials,
[1433.06 --> 1436.72]  and that'll eventually graduate to Plex as long-term, like forever storage.
[1437.36 --> 1439.08]  And so both of those things run on the Mac Mini.
[1439.16 --> 1441.58]  The Mac Mini is probably overkill for that purpose.
[1442.02 --> 1447.54]  But I find that, A, I don't particularly have the interest in maintaining anything but Linux or Mac OS.
[1447.80 --> 1449.52]  And so I don't really want a Windows box.
[1449.52 --> 1451.12]  That's not to say there's anything wrong with them.
[1451.14 --> 1454.10]  And I know, like, a NUC is probably the right answer here, to be honest.
[1454.44 --> 1455.60]  But I don't want it.
[1455.74 --> 1459.48]  And so I got the Mac Mini because it's the path of least resistance for me.
[1459.60 --> 1461.68]  And it's worked out really well, if a bit overkill.
[1462.22 --> 1463.94]  Well, you say a NUC is the right move.
[1464.04 --> 1469.46]  I mean, there are these little Dell small form factor things you can get that are actually just slightly smaller than a Mac Mini.
[1469.62 --> 1470.90]  Not much, granted.
[1471.52 --> 1472.74]  They've got an Intel chip in them.
[1472.74 --> 1475.52]  I'm sorry to deal with your sensitivities.
[1475.70 --> 1478.86]  But they have some hardware transcoding built into them called QuickSync.
[1479.02 --> 1484.54]  And it's a really powerful drug if you're running Plex or Jellyfin or any kind of DVR system.
[1484.54 --> 1488.60]  Because the hardware transcoder in these boxes sips power.
[1488.70 --> 1492.04]  We're talking sort of 4, 5, 6 watts to do a 4K transcode.
[1492.58 --> 1496.52]  One question I have for you, Casey, about running Plex on a Mac Mini particularly.
[1496.52 --> 1502.46]  Does it take advantage of any of the hardware acceleration in the M1 chip to do video decoding?
[1502.84 --> 1506.32]  You're asking a completely reasonable question to which I'm not 100% sure of the answer.
[1506.48 --> 1507.94]  I think it does.
[1508.22 --> 1511.66]  I very well may be lying to you accidentally, but I think it does.
[1511.80 --> 1515.12]  I don't know if it did early on, but I thought at some point that landed.
[1515.90 --> 1517.30]  Again, Plex superfan.
[1517.44 --> 1520.86]  I know that they're Jellyfin and what's the other one?
[1520.94 --> 1522.14]  Ember or something like that?
[1522.36 --> 1522.66]  Emby.
[1522.98 --> 1523.60]  Emby, thank you.
[1523.98 --> 1525.72]  I know that they're superfans of those as well.
[1525.72 --> 1527.90]  I'm not here to say that Plex is the one true way.
[1528.20 --> 1532.22]  But Plex can be a little slow on the uptake for some of these sorts of things.
[1532.28 --> 1534.28]  Like they were very slow on HDR support, for example.
[1534.52 --> 1536.84]  But I thought that they had it.
[1536.86 --> 1541.72]  And certainly, I've had like four and five simultaneous streams running on Plex on this Mac Mini.
[1541.98 --> 1543.84]  And it seemed fine.
[1543.88 --> 1545.16]  And some of those were direct for sure.
[1545.22 --> 1546.42]  And some of them were transcodes.
[1546.46 --> 1547.30]  And it's worked out okay.
[1548.00 --> 1550.08]  It's funny you bringing up like wattage and stuff.
[1550.14 --> 1552.48]  Because I never really cared about that in the past.
[1552.48 --> 1556.04]  But my new favorite toy is you can get these.
[1556.10 --> 1557.40]  And this isn't exactly what you're talking about.
[1557.44 --> 1562.04]  But you can get these USB-C cables that like have little watt meters in them.
[1562.16 --> 1564.10]  And I really wish I didn't know this existed.
[1564.10 --> 1566.38]  Because now I want them to have them like everywhere.
[1566.38 --> 1569.12]  And I'm like, oh, well, why is my iPad not charging fast enough?
[1569.12 --> 1570.48]  It's only using 15 watts instead of 20.
[1570.54 --> 1570.98]  What's going on?
[1570.98 --> 1575.44]  And it's like the same reason I don't put battery percentages on my devices.
[1575.44 --> 1576.50]  Because it just adds stress.
[1576.82 --> 1579.24]  And yet here I am constantly buying these damn things on Amazon.
[1579.24 --> 1581.84]  Because I'm addicted to knowing how much power I'm using.
[1582.28 --> 1583.36]  It's a problem.
[1583.48 --> 1584.32]  Those are pretty great.
[1584.56 --> 1586.16]  How do you remotely manage a Mac then?
[1586.38 --> 1588.68]  I mean, I know you can do like screen sharing and stuff like that.
[1588.76 --> 1591.04]  But is it a good SSH platform?
[1591.34 --> 1592.86]  Like talk us through that a bit.
[1593.04 --> 1594.66]  It's a great SSH platform.
[1595.12 --> 1597.62]  I can't remember if Tailscale SSH supports Mac.
[1597.62 --> 1600.66]  I know the Synology is wonky and that doesn't work.
[1600.84 --> 1602.20]  It does not, to my knowledge.
[1602.36 --> 1602.92]  Yeah, okay.
[1603.26 --> 1606.40]  So I should really talk to somebody that works at Tailscale, if only I knew anyone.
[1606.56 --> 1609.48]  And see if we could get that bumped right up the priority list.
[1609.90 --> 1611.14]  Got one word for you, Casey.
[1611.64 --> 1611.84]  Sandboxing.
[1612.18 --> 1613.04]  Yeah, I know.
[1613.14 --> 1614.20]  And that's completely fair.
[1614.52 --> 1615.36]  And you're not wrong.
[1615.72 --> 1618.42]  In all seriousness, it is a pretty good SSH platform.
[1619.14 --> 1622.36]  I don't have dramatic needs of the device.
[1622.58 --> 1624.10]  Generally speaking, if it's working, it's working.
[1624.18 --> 1624.88]  That's all I care about.
[1625.58 --> 1626.66]  But SSH into it.
[1626.66 --> 1632.74]  But Apple devices or the Mac devices have, they call it screen sharing, but ultimately
[1632.74 --> 1634.12]  it's just VNC under the hood.
[1634.30 --> 1635.20]  And that's all built in.
[1635.32 --> 1636.32]  And so you just have to flip it on.
[1636.76 --> 1638.00]  And you can VNC.
[1638.12 --> 1642.14]  And actually, as of just a few months before the Vision Pro landed, when they added this
[1642.14 --> 1648.28]  Mac virtual display thing, now you have like this super high quality version of VNC that
[1648.28 --> 1650.00]  I think is proprietary to Apple platforms.
[1650.40 --> 1655.34]  And you could, I wouldn't, but you could watch a video like on the remote screen through
[1655.34 --> 1655.68]  VNC.
[1655.76 --> 1658.56]  Like it's phenomenal how good it is if you really wanted to.
[1658.92 --> 1660.16]  So that's what I do.
[1660.26 --> 1665.22]  I've just thought that that's now the reason for you to buy a Vision Pro is so you can remotely
[1665.22 --> 1666.16]  administer your servers.
[1667.00 --> 1668.82]  That's definitely worth $3,500.
[1669.22 --> 1669.78]  That's what it is.
[1670.22 --> 1671.78]  But no, I mean, it does work.
[1671.88 --> 1673.60]  And it's surprising how well it works.
[1673.68 --> 1675.46]  I will say that it is running headless.
[1675.46 --> 1678.80]  And it used to be, and I just have always had this plugged in.
[1678.88 --> 1681.32]  I don't know if it's still the case, but it used to be that you needed to get one of those
[1681.32 --> 1684.72]  dumb HDMI little things that you stick in.
[1684.80 --> 1688.70]  So it feels like the machine thinks it has a monitor plugged in, even though it doesn't.
[1688.80 --> 1692.70]  There's a term for this that I also is escaping me, but it's like 10 or 15 bucks on Amazon.
[1692.98 --> 1693.96]  A dummy plug, I think.
[1694.30 --> 1694.46]  Yeah.
[1694.54 --> 1697.58]  And I plugged one of those in on the Intel Mac mini.
[1697.76 --> 1702.30]  And I genuinely don't know if it's required these days, but it was, I'm doing a thumbs up on
[1702.30 --> 1704.36]  the video here because Apple is so great.
[1704.78 --> 1709.40]  So anyways, I don't know if it's required today, but it certainly was back in the Intel
[1709.40 --> 1709.78]  days.
[1709.96 --> 1712.10]  And I've been running one of those and that's fine.
[1712.18 --> 1714.76]  And it's this way it always runs effectively a 4K display.
[1714.96 --> 1716.34]  And that's what I'm VNCing into.
[1716.54 --> 1720.66]  And again, as long as I'm on a moderately decent network connection, it's fine.
[1720.74 --> 1724.66]  And when I'm at home, it's as though I'm looking at the physical monitor.
[1724.88 --> 1725.58]  It's impressive.
[1727.66 --> 1730.26]  Unraid.net slash self-hosted.
[1730.40 --> 1730.72]  Unraid.
[1730.72 --> 1734.28]  It's a powerful, easy operating systems for servers in your storage.
[1734.46 --> 1737.94]  You can maximize your hardware with unmatched flexibility.
[1738.20 --> 1741.88]  It really is flexible because you can mix and match hard drive sizes.
[1742.06 --> 1746.24]  So if you're like me, you might have a closet full of discs right now.
[1746.54 --> 1748.38]  Drawers, closets stacked on the desk.
[1748.80 --> 1750.48]  I mean, what are you going to do when they're all different sizes?
[1750.66 --> 1752.94]  Well, say hello to Unraid.
[1753.30 --> 1755.94]  They have the most flexible system for this.
[1755.98 --> 1758.96]  It lets you use whatever you have and you can build what you want.
[1758.96 --> 1761.42]  And I think you're going to love the UI.
[1761.66 --> 1762.06]  It's simple.
[1762.18 --> 1762.68]  It's straightforward.
[1762.78 --> 1765.96]  It makes it easy to manage your entire stack of Docker applications.
[1765.96 --> 1775.68]  You can add new applications from their hundreds of user-created templates in the community apps like, you know, AdGuard, PyHole, Home Assistant, Sennhear, Plex, and Jellyfin, many more.
[1775.80 --> 1777.72]  Or, you know, you can deploy your own containers too.
[1777.72 --> 1793.02]  And you can manage your VMs because Unraid is the most flexible NAS OS around with built-in VPN support, thousands of apps and plugins, VM support, and an expandable dual parity protected array utilizing CFS, ButterFS, or XFS.
[1793.02 --> 1797.28]  It's file system agnostic, it's hardware agnostic, and it's disk agnostic.
[1797.60 --> 1807.94]  You can mix and match your hard drives of any size to build out your server and grow your storage capacity bit by bit with a flexible OS that lets you run your self-hosting stack.
[1808.34 --> 1809.34]  It's really slick.
[1809.76 --> 1810.20]  Check it out.
[1810.74 --> 1811.38]  Support the show.
[1811.66 --> 1812.10]  It's Unraid.
[1812.24 --> 1815.34]  Unraid.net slash self-hosted.
[1815.80 --> 1819.30]  Truly a powerful, easy-to-use operating system for your home lab.
[1819.30 --> 1822.32]  You can maximize your hardware with unmatched flexibility.
[1822.70 --> 1823.48]  Try it today.
[1823.96 --> 1826.36]  Unraid.net slash self-hosted.
[1827.94 --> 1837.12]  I don't know if this was in honor of Casey's pre-arrival this week or not, but something in my mind just went, Alex, you've got to do this and just try it out.
[1837.18 --> 1838.60]  Just in the name of science.
[1839.14 --> 1841.90]  I went and bought Vision Pro this week.
[1842.38 --> 1843.38]  In the name of science, of course.
[1843.40 --> 1844.24]  In the name of science.
[1844.28 --> 1845.16]  I mean, how could you not?
[1845.26 --> 1846.40]  It's so affordable.
[1846.82 --> 1848.88]  There's so many clear use cases for it.
[1848.88 --> 1849.50]  How could you not?
[1849.76 --> 1852.54]  As you know, Casey, he has to for his podcast job.
[1852.66 --> 1853.30]  He has to.
[1853.86 --> 1855.96]  I've heard that excuse works from time to time.
[1856.38 --> 1863.74]  And remote server administration, as we just established, Blink SSH in that thing is obviously the only use case that makes sense.
[1864.02 --> 1864.44]  Right, right.
[1864.44 --> 1869.70]  I mean, obviously, Chris and I, as you listen to this, we've already been in Texas, but we're about to go to Texas.
[1869.82 --> 1875.34]  So I've got a flight coming up and I'm like, well, I really want to try Vision Pro on a plane and see how that whole thing goes.
[1875.34 --> 1877.70]  You have to be that guy.
[1877.80 --> 1878.04]  You do.
[1878.12 --> 1878.98]  You just have to embrace it.
[1879.08 --> 1883.74]  So I have not been on a plane with it, although I literally two weeks from today as we record, I'm going to be traveling to Memphis.
[1884.40 --> 1887.50]  And I plan to be that guy, although I'm talking a big game.
[1887.58 --> 1889.28]  We'll see if I actually come through.
[1889.28 --> 1897.82]  But no, I did use it on the train when I visited a friend of mine, a co-host of mine, Mike Hurley, who happened to be in New York for his Vision Pro pickup because he's a Londoner.
[1898.16 --> 1899.02]  Can't get it in London yet.
[1899.08 --> 1901.42]  And so he flew into New York and picked his up there.
[1901.54 --> 1905.82]  And I thought, well, you know, it's not often that I can say that Mike is on the eastern seaboard.
[1905.82 --> 1911.14]  So I took the train, the Amtrak, up to New York City and I used it on the train.
[1911.58 --> 1916.24]  And I did get a couple of weird looks, but surprisingly, most people just did not care.
[1916.80 --> 1919.30]  And now, again, this is a train, which is a very different animal than a plane.
[1919.44 --> 1922.18]  It's a lot more space, a lot fewer people.
[1922.54 --> 1924.92]  But it was incredible.
[1924.92 --> 1935.64]  And to kind of jump right into the deep end with it, in a situation where I'm used to my normal operating procedures, I sit here right now, I have three 5K displays in front of me.
[1935.76 --> 1941.98]  I have an LG Ultrafine that was sent to me by one of my podcast co-hosts because he hates this thing and I like it.
[1942.08 --> 1943.66]  So he just wanted it out of his house.
[1943.72 --> 1944.76]  And I said, OK, sure, I'll take it.
[1944.88 --> 1946.84]  And so there's an LG Ultrafine to my left.
[1947.00 --> 1948.48]  There's a studio display in front of me.
[1948.50 --> 1952.58]  And then there's an LG Ultrafine that I bought secondhand a few years ago to my right.
[1952.58 --> 1956.22]  So I have 15Ks, if you will, of displays all around me.
[1956.30 --> 1959.04]  I probably am getting a suntan as we speak, even though it's nighttime.
[1959.68 --> 1962.00]  And so because of that, that's all well and good when you're at home.
[1962.00 --> 1967.06]  But when you travel, it's crappy because I'm used to infinite real estate.
[1967.16 --> 1968.28]  And now I have effectively none.
[1968.34 --> 1969.50]  I use a 13-inch MacBook Pro.
[1969.66 --> 1972.54]  I made that choice deliberately, but it's not great.
[1972.74 --> 1976.38]  And if you're trying to get anything productive done, you want to have more real estate.
[1976.38 --> 1984.26]  And I recently, like a year ago, I got a little, I think it's a 2K 13-inch portable display that runs on USB-C.
[1984.36 --> 1985.66]  It's like bus powered, the whole rigmarole.
[1985.90 --> 1986.96]  I love this thing.
[1987.36 --> 1989.98]  It's not great, but it was like $150 and I love it.
[1990.26 --> 1994.52]  But then the Vision Pro came and it turns out one of the things you can do with the Vision Pro is what they call Mac virtual display,
[1994.64 --> 1999.36]  which is you can suck your Mac screen into the Vision OS virtual world.
[1999.36 --> 2007.50]  And what's really trick about it is if you have your Mac laptop in front of you, and if it's open, as you would expect, you're not clamshelled or anything,
[2007.80 --> 2012.92]  you can literally just look at your laptop and then a little connect button floats up above it.
[2013.04 --> 2017.90]  And you just pinch on the connect button and then suddenly you're looking at your Mac screen in the virtual world.
[2018.04 --> 2019.58]  And your Mac screen is now black.
[2019.72 --> 2020.78]  So you could be doing bills.
[2021.06 --> 2024.24]  You could be doing top secret proprietary work stuff.
[2024.24 --> 2029.90]  And no one will know because the only people that can see it are your two eyeballs inside the Vision Pro.
[2030.08 --> 2031.50]  It is incredibly cool.
[2031.68 --> 2042.14]  And of all the things that I've used the Vision Pro for, I think that might be the, maybe not the coolest, but the most important to me.
[2042.22 --> 2046.08]  Because in the occasion I want it, I really want it.
[2046.08 --> 2050.96]  Like in a hotel room or something or on a plane or on a train, I really want that real estate.
[2050.96 --> 2054.96]  And there's no other way to get it when you're in a car, when you're in a moving vehicle.
[2055.38 --> 2058.00]  And even in a hotel room, you're not going to bring a 5K display to a hotel.
[2058.18 --> 2060.70]  Like this is, I'm not going to be that guy.
[2060.94 --> 2063.74]  You're not Marques Brownlee carrying an iMac across the country.
[2063.86 --> 2064.52]  Right, exactly.
[2065.18 --> 2067.42]  With my Pelican case and the whole rigmarole, exactly.
[2067.86 --> 2069.80]  So that in and of itself is so cool.
[2070.08 --> 2071.48]  But it is only one screen.
[2071.64 --> 2072.92]  Is that not a problem for you still?
[2073.04 --> 2075.98]  You know, I can't tell if you're snarking, but it is a reasonable question.
[2076.32 --> 2078.60]  And I don't love that aspect of it.
[2078.60 --> 2082.54]  But I mean, it was not that long ago that, like I said, I was rocking the iMac Pro.
[2082.90 --> 2083.98]  And that was one 5K display.
[2084.18 --> 2086.68]  And somehow I was able to work with that for like three years.
[2086.82 --> 2090.08]  So I feel like I can go back to that and be okay.
[2090.30 --> 2091.38]  Yeah, it's still better than a 13-inch screen.
[2091.48 --> 2091.80]  Exactly.
[2092.10 --> 2096.86]  So what I'll say in counter to that, Chris, is, well, first of all, there is an app that I think it's in TestFlight,
[2096.92 --> 2101.52]  or maybe it just came out, called Split Screen, which lets you do multiple displays.
[2102.46 --> 2104.68]  I found it a little buggy, a little rough around the edges.
[2104.68 --> 2105.96]  It kind of works.
[2106.10 --> 2111.00]  But you've got your Mac display, and then wherever your eyes look, the keyboard and mouse,
[2111.14 --> 2117.88]  you sort of realize using this Vision Pro, all of the little things Apple have added over the last five years to iOS,
[2118.30 --> 2123.94]  and like Handoff, and, you know, some of the MagSafe improvements, and all these other things, right?
[2124.32 --> 2129.44]  You realize that they have been sucked out of the Vision Pro and thrust upon the masses.
[2129.44 --> 2132.48]  So I've got my Mac display mirrored in front of me.
[2132.62 --> 2137.28]  I look up to my right, and I've got a YouTube window in Safari on Vision OS Safari playing,
[2137.48 --> 2139.92]  and suddenly my keyboard and mouse is in that window.
[2140.26 --> 2141.34]  I don't have to do anything.
[2141.44 --> 2142.64]  It's just where I'm looking.
[2142.82 --> 2148.88]  And there was an early ATP episode that you guys did where you were talking about how some of the UI paradigms,
[2149.46 --> 2155.44]  where you have to get used to looking and clicking at the same time, exactly what, you know, pinching on what you want.
[2155.44 --> 2156.36]  Yeah, yeah, yeah.
[2156.52 --> 2161.62]  Turns out you were spot on with that, because there's a number of times where my eyes,
[2161.72 --> 2165.48]  I realize using a real computer, I don't mean the Vision OS isn't a real computer.
[2165.48 --> 2166.26]  No, no, no, I'm with you.
[2166.62 --> 2170.96]  But like using an old computer, where I realize I'm clicking on stuff,
[2171.04 --> 2175.94]  and my eyes are already five seconds ahead on the next thing where that UI element is going to be.
[2176.48 --> 2178.94]  And in the Vision Pro, you can't do that.
[2178.94 --> 2186.20]  Right. And that's the thing is, you know, being a good typist, a good touch typer is amazing until it isn't.
[2186.46 --> 2193.62]  And this is one of those cases where like, I might be looking and typing like a search query in the Safari, you know, a search bar.
[2193.92 --> 2198.58]  But yet I'm also looking over to the other direction because I'm watching a YouTube video or what have you.
[2198.68 --> 2202.04]  And with the Vision Pro, your gaze is also your pointer.
[2202.04 --> 2207.82]  And that's both magical and freaking terrible, depending on the context, which is kind of funny.
[2207.82 --> 2210.54]  But so when did you pick yours up? Just this week, you said?
[2210.96 --> 2213.42]  Yeah, I went on Friday. And as we record, it's Tuesday.
[2213.68 --> 2217.26]  I had a demo on Friday and I told the guy in the store, I'm not going to buy it.
[2217.80 --> 2221.40]  Went home and I said to my wife, I didn't buy one.
[2221.50 --> 2225.58]  Look, aren't I a good boy? And she went, oh, I was looking forward to playing with that.
[2225.66 --> 2226.70]  So I was like, right, gotta go.
[2227.52 --> 2228.28]  No, really?
[2228.68 --> 2231.22]  Yeah, literally. And I booked her a demo for the next day.
[2231.22 --> 2232.90]  She had one and we picked one up.
[2232.90 --> 2239.94]  So I spent most of the weekend in it and I've got a 65 inch OLED TV on the wall behind me here.
[2240.18 --> 2247.44]  And it feels small now I'm out of the Vision Pro because I've suddenly got used to 120 inch video screens.
[2247.70 --> 2252.48]  The immersive videos, I want to talk to you a little bit about like content and stuff like that.
[2252.54 --> 2256.74]  Like I found a couple of apps that let you stream Plex into this thing.
[2256.74 --> 2271.24]  And there's still very early days, like the immersive mode is limited to certain streaming services like Apple TV and Disney Plus, for example, have what's called immersive mode where it puts you in like the seat of an actual theater, for example.
[2272.16 --> 2275.84]  I found one called Cinephile for Plex that lets you do a similar thing for Plex.
[2276.00 --> 2279.98]  It's not as polished as all the others, but it does the job.
[2280.56 --> 2283.28]  So I'm really looking forward to on the plane a bit of that.
[2283.28 --> 2292.32]  Yeah. And that's the thing is that the problem with the Vision Pro is that you really, really, really need to experience it.
[2292.56 --> 2300.40]  And if you live anywhere near an Apple store, which depending on your portion of the country or the world, that may or may not be an easy ask.
[2300.54 --> 2303.92]  But, you know, we have one Apple store in Richmond and that's it.
[2303.94 --> 2309.18]  And we're the nearest Apple store for like two to three hours drive in many different directions, which is kind of barbaric.
[2309.20 --> 2309.74]  But here we are.
[2310.06 --> 2312.34]  But thankfully, it's only like 20 minutes from my house.
[2312.34 --> 2313.20]  So there you go.
[2313.58 --> 2314.58]  Coming full circle now.
[2315.16 --> 2318.76]  But nonetheless, if you have the time, book yourself a Vision Pro demo.
[2318.90 --> 2330.02]  Even if you do not care about Apple, if you don't care about the Vision Pro, if you don't care about any of this, it is worth the, what is it, like half an hour of your time leaving aside the travel and whatnot.
[2330.34 --> 2337.64]  It's worth half an hour of your time just to experience it because there is no way for me to verbalize what this is like.
[2337.64 --> 2347.40]  And, you know, I was struggling on the most recent episode as we record of ATP because one of my co-hosts, John, who is annoyingly bright and annoyingly good at so many things.
[2347.66 --> 2354.54]  But I was trying to verbalize to him, like, look, there is a big difference between 3D, which is what we're used to, right?
[2354.54 --> 2357.70]  Where you have a rectangle, but that rectangle has depth to it.
[2358.06 --> 2362.02]  There is a big difference between 3D and what Apple calls immersive.
[2362.38 --> 2365.90]  Because with 3D, there's a rectangle and there's depth and that's cool.
[2366.38 --> 2371.20]  But with immersive, you can turn your head to look at something else.
[2371.32 --> 2376.00]  And that just completely changes everything.
[2376.00 --> 2378.46]  That Alicia Keys demo, right?
[2378.62 --> 2382.50]  Where you've got, so they've got this thing called Alicia Keys Rehearsal Room.
[2383.10 --> 2393.16]  And it basically, they've got four cameras dotted throughout the room and you're in a small, it can't be more than sort of a few hundred square feet little rehearsal room with Alicia Keys and her band.
[2393.76 --> 2397.36]  And you can sit there and as a musician and a drummer, like, I love just watching.
[2397.36 --> 2404.54]  If I could go for a Blu-ray that is literally just focused on Danny Carey in Tool the whole time, like, that's what I would do.
[2404.54 --> 2407.88]  But unfortunately, such things rarely exist.
[2408.56 --> 2412.14]  Until the immersive music concerts come out.
[2412.44 --> 2416.28]  And it's really something like, you think, oh, the bass player is doing something interesting.
[2416.36 --> 2417.64]  I'm going to watch the bass player for a second.
[2418.24 --> 2418.52]  Exactly.
[2418.76 --> 2421.16]  So I cannot play anything but a stereo.
[2421.30 --> 2423.50]  And even that, I can only play with some amount of efficiency.
[2423.78 --> 2425.26]  I have never been a musician.
[2425.38 --> 2426.02]  I wish I was.
[2426.10 --> 2427.26]  I wish so desperately I was.
[2427.32 --> 2427.88]  I am terrible.
[2428.24 --> 2429.82]  But I love music.
[2429.92 --> 2431.68]  I love watching concert films.
[2431.82 --> 2433.28]  I love NPR Tiny Desk.
[2433.28 --> 2434.70]  You know, I love MTV Unplugged.
[2434.78 --> 2435.76]  You didn't mention Phish.
[2435.84 --> 2436.40]  I'm surprised.
[2437.86 --> 2438.22]  Trigger.
[2438.32 --> 2439.16]  Trigger warning, please.
[2439.28 --> 2439.62]  Trigger warning.
[2440.10 --> 2442.94]  But nevertheless, I love so much.
[2442.98 --> 2446.96]  Like, I have an entire library on Plex dedicated to Dave Matthews Band concerts because I'm one of those.
[2447.10 --> 2449.58]  You know, I went to school and I went to college in the early 2000s.
[2449.60 --> 2450.24]  This is what we did.
[2450.38 --> 2455.16]  But anyways, I loved the Alicia Keys thing for exactly what you're describing.
[2455.16 --> 2459.02]  That I might be interested in the guitarist or the bassist or the drummer or what have you.
[2459.12 --> 2462.78]  But the director might be focused on Alicia Keys, which on the surface makes sense.
[2462.90 --> 2467.98]  But the great thing is, I can turn my head and look at what I want to look at.
[2468.08 --> 2473.02]  Now, granted, that bassist may be on the other side of the room from the particular camera that I'm looking through right now.
[2473.02 --> 2477.28]  Or the, I shouldn't say camera because that implies like a stationary static thing.
[2477.36 --> 2477.96]  But you know what I mean.
[2478.02 --> 2481.58]  Like, you know, the perspective that I have right now is from the other side of the room.
[2481.78 --> 2486.22]  But at least I can turn my head and watch that this bass player is freaking shredding over there.
[2486.44 --> 2492.28]  And, you know, in any normal scenario, I'd just be looking at Alicia Keys being Alicia Keys, which is phenomenal.
[2492.60 --> 2494.42]  But I wanted to see the bass player.
[2494.52 --> 2495.14]  Now I can.
[2495.20 --> 2497.44]  And actually, there's an app that I just got wind of.
[2497.96 --> 2500.66]  Shoot, I don't know if I'm going to be able to find what the name of it is offhand.
[2500.66 --> 2503.34]  But it's an app that's specifically for immersive concerts.
[2503.50 --> 2506.92]  And it's all of the concerts are, I think, $13 each.
[2506.96 --> 2508.54]  But they have a demo of somebody.
[2508.84 --> 2512.00]  I could be that guy and put this all on my head as we record and figure it out.
[2512.02 --> 2512.46]  But I won't.
[2512.84 --> 2517.64]  But they have a demo of somebody that I downloaded but haven't had a chance to watch as we record.
[2518.10 --> 2523.76]  But apparently, these are like short, like Alicia Keys length concerts where you can buy them.
[2523.84 --> 2524.52]  And they're immersive.
[2524.68 --> 2526.04]  You can look around and so on and so forth.
[2526.10 --> 2527.30]  I know T-Pain was on there.
[2527.70 --> 2529.96]  I think Megan Thee Stallion or whatever she's called.
[2529.96 --> 2530.48]  I'm so old.
[2530.58 --> 2532.94]  And I don't know what the correct pronunciation for any of these people are.
[2533.22 --> 2534.98]  But I think there was one of hers.
[2535.28 --> 2536.48]  And then there's the demo one.
[2536.52 --> 2537.96]  And like somebody else I was not aware of.
[2538.04 --> 2539.18]  And I haven't had a chance to watch it.
[2539.26 --> 2541.34]  And if I remember, or please, gentlemen, remind me.
[2541.38 --> 2543.72]  And I'm happy to send you a link to whatever it is this thing is called.
[2543.76 --> 2545.12]  Because again, I can't remember it offhand.
[2545.44 --> 2547.54]  But I would kill for this.
[2547.82 --> 2553.02]  Like for whatever your particular band is, I would pay all of the money to have an immersive concert.
[2553.18 --> 2555.74]  Like it's just, it's that much better than 3D.
[2555.74 --> 2562.14]  And 3D is arguably, especially when you have a good situation where you don't have it dimming each eyeball in order to fake 3D.
[2562.30 --> 2563.92]  Like in the Vision Pro, 3D is really good.
[2564.12 --> 2566.76]  But even still, immersive is just night and day better.
[2566.76 --> 2576.60]  So I feel like there is no, there has been no device come out since the iPhone has been so clearly the future of where computing, personal computing is going.
[2576.98 --> 2582.80]  And yet this is such a hilariously first generation device in so many ways.
[2583.04 --> 2583.60]  Yep.
[2584.22 --> 2591.86]  But in contrast to that, like with waxing lyrical about, like it's genuinely, you sort of put it on and you're like, this is it.
[2591.86 --> 2598.08]  They've solved it with the pinching, with the interfacing, with all of the, you know, Apple magic of handing off things to each other.
[2598.24 --> 2603.84]  And I don't know what you feel about like the next decade or so is going to look like with this device and this platform.
[2603.84 --> 2605.74]  But for me, I'm excited.
[2605.86 --> 2607.28]  Like my daughter's three right now.
[2607.88 --> 2612.64]  By the time she's 13, I think these are going to be as ubiquitous as laptops in coffee shops.
[2613.20 --> 2614.28]  You know, I think it's very possible.
[2614.28 --> 2622.46]  And the other interesting thing about having a three-year-old is that now is the time, assuming your daily driver is an iPhone, now is the time to start recording immersive video.
[2622.68 --> 2631.94]  Like I wouldn't do it always by any means, but iPhones, or at least iPhones Pro, the way they have their lenses on, maybe it's only the brand new ones, I forget now.
[2632.06 --> 2642.66]  But the way the lenses are situated is that it'll use the two lenses that are vertically if you're holding a portrait, but they make you turn it horizontally so that they're adjacent to each other when you record.
[2642.66 --> 2648.36]  And you can put the iPhone into this immersive video mode and you can record a 3D video.
[2648.56 --> 2653.26]  It's not stellar, but it is stunning.
[2653.62 --> 2659.12]  Like it's funny because I know that sounds contradictory, which it kind of is, but the fidelity is all right.
[2659.30 --> 2664.26]  You kind of have like just a square that you're looking at this through, but there's a depth to it.
[2664.26 --> 2675.44]  And the spatial audio, which sounds 3D or, you know, the surround sound, if you will, it just adds this unbelievable amount of figurative depth to what you're viewing.
[2675.92 --> 2677.12]  Similarly with like panoramas.
[2677.22 --> 2685.04]  Panoramas are one of my favorite things to look at in the Vision Pro because generally speaking, a panorama, you know, it's just, it looks wonky.
[2685.14 --> 2688.16]  No matter what you do, it looks wonky when you're looking at it on a flat screen.
[2688.16 --> 2698.92]  And the Vision Pro isn't the first thing to do this, but when you have it kind of unravel or unwrap the panorama, so it is panoramic, it's like standing there.
[2699.02 --> 2705.16]  We have a photo I took two, three years ago of my family at a beach called Cape Charles on the Eastern shore of Virginia.
[2705.16 --> 2713.36]  And, you know, I was standing probably 30 yards away from the family and there's my wife, my son and daughter and our dog over there to the side.
[2713.48 --> 2716.74]  And I look around at this panorama and nothing's moving.
[2717.02 --> 2718.48]  You know, it's dead still, no audio.
[2718.74 --> 2720.74]  And it's like, I'm freaking there.
[2721.60 --> 2725.56]  It's just unreal how cool some of this stuff is.
[2725.62 --> 2731.44]  And so to build on what you're saying, Alex, like today, the hardware is phenomenal, except it's heavy and clunky and hot.
[2731.44 --> 2739.30]  The software is phenomenal, except it's a little wonky in a lot of places and a lot of things don't work and not a lot of apps have been written for the device.
[2739.76 --> 2744.32]  But yet you can see so easily where the future could go.
[2744.64 --> 2749.78]  And it's funny because early on, I was one of the many people that said, this is definitely going to be glasses one day.
[2749.88 --> 2753.00]  It's going to be AR glasses and that's going to be the future.
[2753.00 --> 2757.10]  And the more time I spend in the Vision Pro, the less and less I think I was right about that.
[2757.16 --> 2761.78]  And the more I think that the immersion might be the thing that really sells it.
[2761.86 --> 2767.30]  And that's tough because then you're immersed in this other world and you're not in your surroundings.
[2767.30 --> 2768.54]  You're ignoring your family.
[2768.66 --> 2770.06]  You're ignoring everything around you.
[2770.46 --> 2773.76]  And that's why they have that goofy looking display on the front and so on and so forth.
[2773.76 --> 2782.60]  But if you can be selfish for a minute, which I'm uniquely talented at, if you can be selfish for a minute, it is unlike anything else I've experienced.
[2782.94 --> 2787.84]  And it is very easy if you're listening to this, particularly if you're not an Apple fan, it's very easy to listen to this.
[2787.90 --> 2797.34]  And me as an avowed Apple person, it's easy to be like, oh, yeah, it's another one of those buffoons or another one of those sheeple that's just been told to buy this ridiculously expensive product and did.
[2797.46 --> 2799.72]  And now this idiot won't shut up about it.
[2799.72 --> 2805.08]  And all of those things are mostly true, but I swear to you, go to an Apple store and try it.
[2805.14 --> 2814.42]  Even if it's not your cup of tea, if you're a nerd and if you're into technology, it's worth the half an hour just to experience what this is like.
[2814.42 --> 2823.06]  And they do a pretty good job in 30 minutes of giving you a sample of immersive stuff, a sample of 3D stuff, a sample of what it's like to just try to get work done on this thing, which was not great.
[2823.36 --> 2828.50]  But it's worth the 30 minutes just to see and to see the future today.
[2829.72 --> 2832.66]  Tailscale.com slash self-hosted.
[2832.76 --> 2835.80]  Tailscale is programmable networking that you know we love.
[2835.90 --> 2838.74]  It's private, secure, and fast by default.
[2838.98 --> 2843.90]  It is the easiest way to connect devices and services directly to each other wherever they are.
[2844.46 --> 2849.00]  Put simply, you can build a flat network across complex infrastructure.
[2849.00 --> 2855.62]  Different VPSs, different machine types, VMs, physical devices, mobile devices.
[2856.18 --> 2862.44]  Replace a legacy VPN infrastructure in just minutes with a mesh VPN that uses WireGuard.
[2862.44 --> 2864.72]  You can transform your network in security.
[2864.94 --> 2866.28]  No more inbound ports for me.
[2866.58 --> 2872.44]  And for enterprises, it is so much more straightforward and it'll snap into your existing authentication and auth infrastructure.
[2872.44 --> 2874.08]  It's easy to deploy.
[2874.20 --> 2876.18]  The client gets up and going in just minutes.
[2876.32 --> 2877.10]  It's intuitive.
[2877.38 --> 2881.56]  And you can start to program your network in a way that you've never had access to.
[2881.68 --> 2886.50]  And it gives you a flat network for yourself or your team or your family.
[2886.68 --> 2889.40]  I have my friends and my family on my Tailnet.
[2889.40 --> 2895.14]  And when you go to tailscale.com slash self-hosted, you can try it for free for up to 100 devices.
[2895.52 --> 2899.16]  And one of the things that I've started to take advantage of is Tailscale's ACLs.
[2899.24 --> 2903.54]  So I can have certain friends that can see some systems and other friends that can't see other boxes.
[2903.74 --> 2908.72]  I can share individual systems or even down to the application level if that's how I prefer to do it.
[2908.98 --> 2911.98]  It's privacy for everyone and every organization.
[2912.34 --> 2913.52]  And it's fast.
[2913.72 --> 2914.44]  We love it.
[2914.52 --> 2916.42]  And I think you're going to see why once you try it.
[2916.42 --> 2920.72]  So go support the show and get it for free for up to 100 devices.
[2920.88 --> 2922.48]  That's not a limited time deal.
[2923.16 --> 2926.98]  You can use it for free for as long as you like on 100 devices.
[2927.58 --> 2930.28]  They can do that because the traffic is going between all your machines.
[2930.94 --> 2932.86]  They have some magic authentication layer.
[2933.34 --> 2937.12]  But all of the traffic, all of the communication, that's machine to machine protected by WireGuard.
[2937.58 --> 2938.46]  It's so great.
[2938.54 --> 2940.84]  It will transform the way you do networking and security.
[2941.30 --> 2941.78]  Try it out.
[2942.12 --> 2942.86]  You know we love it.
[2942.96 --> 2943.72]  I think you will too.
[2943.72 --> 2946.84]  Tailscale.com slash self-hosted.
[2948.46 --> 2955.34]  Well, if my time travel math checks out, I think this episode airs about two weeks before LinuxFest Northwest.
[2956.24 --> 2960.60]  Goodness, how the conference season is whizzing along in front of us.
[2960.98 --> 2962.68]  Yeah, we might as well take it out with a bang.
[2962.84 --> 2966.12]  System76 and Jupyter Broadcasting are throwing a barbecue.
[2966.32 --> 2968.92]  At this point in time, it's very early days.
[2968.98 --> 2969.98]  We're just getting it planned.
[2969.98 --> 2975.88]  And hopefully, though, hopefully it'll be quite the shindig, the shebang, the grill fest.
[2975.98 --> 2977.84]  I don't know, Alex, but I hope people can make it.
[2978.18 --> 2980.48]  I'll link to a meetup page if you do think you could attend.
[2980.54 --> 2982.54]  You're going to be at LinuxFest and you want to join the barbecue.
[2983.54 --> 2983.78]  Shindiggananigans.
[2983.98 --> 2984.46]  How about that?
[2984.74 --> 2985.38]  Yeah, I like that.
[2985.76 --> 2986.20]  Shindiggananigans.
[2986.92 --> 2991.04]  Join the meetup page just so we have an idea of maybe how many burgers and hot dogs we need to buy.
[2991.66 --> 2995.42]  Which means maybe the episode after this, we might be able to record in studio.
[2995.72 --> 2996.76]  How weird would that be?
[2996.76 --> 2998.08]  Oh, that'd be fun.
[2998.26 --> 2999.18]  Yeah, imagine that.
[2999.32 --> 3003.98]  You know, Alex, we probably almost do it more in Airbnbs in person than we do it in the studio in person.
[3004.12 --> 3004.70]  I think so.
[3005.02 --> 3005.18]  Yeah.
[3005.22 --> 3007.64]  The last time I was in Seattle must have been pre-COVID.
[3008.08 --> 3008.36]  Wow.
[3008.58 --> 3009.62]  I want to say it was the sprint.
[3009.98 --> 3010.64]  Wow, Alex.
[3010.76 --> 3011.76]  That's well we got it.
[3011.78 --> 3013.04]  I'm glad we're finally fixing that.
[3013.42 --> 3014.48]  We should have fixed that sooner.
[3014.98 --> 3016.74]  Although there's only so many good months up here.
[3017.36 --> 3017.88]  Truth be told.
[3018.30 --> 3021.36]  I want to say a special thank you to our SREs, our members.
[3021.60 --> 3024.66]  You make the show possible and you get an ad-free version of the show.
[3024.66 --> 3026.42]  You also get a post show.
[3026.80 --> 3029.84]  We have a little more chat with Casey coming up in the post show.
[3030.04 --> 3033.22]  You can sign up at selfhosted.show slash SRE.
[3033.76 --> 3038.04]  As always, you can go to alex.ktz.me to find all of the various places I'm online.
[3038.26 --> 3039.28]  And thank you so much for listening.
[3039.48 --> 3041.86]  That was selfhosted.show slash 121.
[3041.86 --> 3044.02]  MBCOM News 51.
[3044.02 --> 3056.16] 、 ordon和宣品材 führt。
[3056.36 --> 3058.82]  Dow欸 school2.7ена ilgili。
[3059.18 --> 3060.64]  гр worship2.5 mār�� Bach Ra н jpb5 sqqxx3 mw 5sqy mw 5sqrt mw 1y'a d鷹 cuxmlN
[3060.64 --> 3062.50]  苗
[3062.78 --> 3063.82]  从101
[3063.82 --> 3064.34]  N PhDN
[3064.44 --> 3065.28]  从102
[3065.28 --> 3066.26]  重拆
[3066.26 --> 3066.96]  壱
