[0.26 → 8.32] Somehow, it's 2024. Welcome in to Self-Hosted for the Year, everybody. How are you doing? I hope you had a good holiday break. Hi, Chris. How are you?
[8.98 → 16.54] Hello, Alex. I'm all right. I had a very productive holiday break. Extremely productive holiday break. Got a lot done.
[16.54 → 33.26] A bit of chaos, also. There was, I'm not going to lie, a few moments where things seemed like maybe we had some sort of burglar or some sort of water leak, and we just turned out to be, well, chaos monkeys in the system.
[34.04 → 36.88] And my TV died, but other than those things...
[36.88 → 38.56] You've been watching too much Home Alone, haven't you?
[39.22 → 42.70] No, we watched Gremlins. Got me thinking.
[42.70 → 49.44] Now, you know, so fantastic new feature. I used to come... First, let me back up. Sorry. But let me back up real quick.
[50.46 → 55.48] I used to strongly recommend the HomePods here on this podcast as a weird in-between.
[55.92 → 67.34] Now, this is really before the year of voice, but as a weird in-between to have somewhat of a voice assistant that had very simple integration with Home Assistant that didn't require an always-on connection all the time.
[67.34 → 70.48] Well, that's not really true, but didn't require all the levels of internet integration.
[70.48 → 75.70] They do it for the transcription, but all the actual execution of Home commands is done over the LAN.
[75.98 → 81.48] It's a nice compromise, and it integrates into Home Assistant with no cloud account required on the Home Assistant side.
[82.80 → 87.82] However, in iOS 17, they dropped the requirement to say, hey, before you invoke the assistant.
[89.06 → 92.78] And as you can imagine, the assistant gets invoked more often now.
[92.78 → 99.04] And it maybe has had an adjustment to its logic, and it kind of defaults to two modes now.
[99.74 → 105.80] The first mode is if it can't really figure out what you're saying, it just plays music, because they just want you to play as much Apple Music as possible.
[106.80 → 116.34] And the second mode, which is the real problem, it appears it just toggles everything.
[116.34 → 120.86] Anything in Home Assistant that can be toggled, it will toggle.
[121.80 → 133.76] So thermostats, alarms, lights, heaters, switches, anything that you could imagine that could be toggled, Siri will toggle it.
[134.38 → 139.24] And all of it, all at once, as fast as your Home Assistant can process.
[139.24 → 145.22] And this happened to me not once, but twice over the holiday break.
[145.52 → 149.70] Once, while I was out in the woods, trying to consume as little power as possible.
[150.40 → 161.02] And as you can imagine, flipping absolutely everything on, including all of our heat and all our water bay heater, flipping everything on at once, not conducive to saving power.
[161.56 → 164.04] Also, I have alarms.
[164.04 → 169.56] So my family's inside, and the siren starts going off.
[169.76 → 173.06] The 95 decibel siren starts going off.
[173.30 → 174.90] Thankfully, that is outside, not inside.
[175.26 → 176.92] But it's still very loud, even inside.
[177.50 → 179.22] Freaking everyone out.
[179.94 → 182.46] So don't recommend HomePods anymore.
[182.80 → 184.16] You're a voice for the win.
[184.68 → 185.76] Yeah, it's a really strange one.
[185.80 → 188.48] I mean, I've heard the phrase, if in doubt, throw it out before.
[188.48 → 192.50] But never, if in doubt, turn everything you possibly can the opposite way.
[192.50 → 193.46] Crazy craziness.
[193.68 → 194.90] It's absolutely crazy.
[195.08 → 195.94] That is insane.
[196.72 → 202.40] Basically, you're giving voice commands almost root access to your physical space, aren't you, if you think about it like that?
[202.62 → 205.54] It's a very insecure way of exposing an interface.
[205.74 → 208.12] And it's things that get changed outside your control.
[208.24 → 211.12] Like, it's been fine for the entire run of the show.
[211.32 → 214.50] And then with iOS 17, it's totally gone sideways.
[215.00 → 215.94] Yeah, rut row.
[215.94 → 220.42] You know what we need to do is integrate more technology into this stuff and more voice recognition.
[220.42 → 228.60] No, actually, really, what I'm looking forward to is getting rid of the HomePods one day and then just building my own voice system that uses all local.
[228.90 → 235.08] But I don't know if you've seen the project that lets you turn one of the old Google Home or, you know, like the Nest Minis.
[235.22 → 235.60] Yes.
[235.60 → 240.72] Into a Home Assistant compatible, like ESP based microphone array.
[241.22 → 242.16] We're going to get there.
[242.34 → 243.12] We're going to get there.
[243.28 → 252.52] Well, you know what I have to wonder is if one couldn't just have one very powerful computer that just had multiple remote devices that listen.
[253.58 → 254.10] I mean, I don't know.
[254.20 → 259.00] I'm just thinking about different ways maybe I could do it with Home Assistant, even with the current tech, because it's very close.
[259.00 → 263.06] It's just not quite there with, like, the ESP based stuff.
[263.74 → 265.32] More experimentation needs to be had.
[266.12 → 266.74] Yes, indeed.
[267.44 → 272.88] Well, I think over the Christmas period, we both did a lot of tinkering and stuff like that.
[273.24 → 279.70] You were busy, it looks like, in the dock anyway, playing the Nextcloud multi-hop game of shame upgrade.
[280.10 → 281.92] Have you done this before where you get behind?
[282.36 → 282.80] Yes.
[283.30 → 283.74] Yes.
[283.74 → 289.94] I'm still not thrilled with the overall process of managing Nextcloud through Docker.
[290.86 → 295.26] So I'd like to hear if people have simple, successful configurations with Nix.
[295.88 → 298.52] Because right now I have to upgrade the Docker container, which is fine.
[298.70 → 299.32] You know, do that.
[299.74 → 308.04] But then I have to go inside the Docker container and then do a bunch of other different upgrades using the classic OCC command.
[308.36 → 308.62] Yeah.
[308.62 → 314.80] And I always find that to be not rickety, but brittle.
[315.64 → 319.78] And I'm always worried I'm going to break something, and then I'm going to lose my entire Nextcloud instance.
[319.96 → 327.30] And I don't know, I just would feel so much, I don't know why it feels safer to me, just if I could do it with a Docker Compose poll, and it just updates.
[327.56 → 329.12] But I would feel much better about it.
[329.66 → 330.34] Snapshots, baby.
[330.34 → 332.50] That's probably going to be my answer to you.
[332.74 → 337.08] But for the OCC stuff, yeah, you're absolutely right.
[337.20 → 339.36] It does feel really rickety.
[339.58 → 346.36] You have to Docker exec inside a container and then PHP, OCC, Admin, blah, blah, blah, blah.
[346.60 → 349.38] And I had to go through three different versions, right?
[349.44 → 351.04] Because you can't just go from...
[351.04 → 355.12] So I was three versions behind because this process I find to be somewhat intimidating.
[355.84 → 357.14] So I always wait.
[357.14 → 360.22] And also it's a very high use, very high value system.
[360.72 → 363.04] So I also just kind of usually wait a couple releases.
[363.70 → 366.08] But then, you know, I end up having to go pin to as very...
[366.08 → 368.74] I have to basically pin to each release in between.
[369.14 → 371.24] Go through and do all the OCC upgrade stuff.
[371.36 → 376.14] Then go bring it down, update my Docker Compose, pin to the next version, which means I got to go look up on Hub.
[376.22 → 377.22] Okay, which one is the next one?
[377.26 → 377.82] What's it called?
[378.28 → 378.96] You know, all this.
[380.30 → 381.30] It's just rickety.
[381.80 → 382.46] I'm sorry.
[382.60 → 383.04] It's rickety.
[383.04 → 394.12] And it means like, okay, so my other option is I have to be like Johnny on the spot every four months or three months, whatever it is, and upgrade my Nextcloud instance to avoid this?
[394.38 → 395.84] Well, how often is Brent going to Berlin?
[395.98 → 397.54] I think that's their release cadence, right?
[397.78 → 398.50] Yeah, once a quarter.
[399.00 → 399.20] Yeah.
[399.54 → 409.56] So for those that don't know, Nextcloud originally forked from a project called OwnCloud, which is why the sort of admin binary is called OCC.
[409.56 → 415.58] I mean, it makes perfect sense when you know the history, but it seemed so weird to me the very first time.
[415.92 → 416.64] Yeah, what is this?
[416.72 → 417.22] What is this?
[417.32 → 419.42] And to be fair, it all worked.
[420.06 → 425.06] But it felt sort of like, oh, this is – it's 100% on me for getting that far behind.
[425.74 → 430.38] But, you know, so yes, it is on you a little bit.
[430.38 → 435.62] And it is good that the upgrade path works most of the time.
[436.02 → 441.84] There's been a couple of instances where I've had to get pretty deep into the OCC magic to unbank something.
[442.46 → 449.60] But typically the only way I know that it's balked is if I go to the Nextcloud web interface, and it says system under maintenance.
[449.60 → 455.02] And I'm like, oh, so that's why my phone hasn't been backing up for the last week.
[455.64 → 461.50] I hate to say it, but that's my general experience as well is, oh, oh, right.
[461.58 → 467.20] And then you have to make time, you know, in your busy schedule to go and fix it.
[467.20 → 479.68] So that's why I have to wonder if there isn't a way to just have a very simple Nix config for Nextcloud that that's how it gets updated is through Nix packages.
[479.82 → 481.08] Of course, it all have to be packaged there.
[481.60 → 489.24] I think the issue you'll run into is that because Nextcloud is very database dependent, they upgrade the schemas a lot between releases.
[489.24 → 502.34] And so unless you've got a fully, you know, atomic snapshot or some kind of way of saying the database looked like this at this moment in history and rolling back those schemas can be really challenging.
[502.50 → 508.50] And it's a problem that plagues enterprises across the world, you know, banking and all that kind of stuff.
[508.50 → 519.80] I spent huge amounts of time listening to DBA's in London at the bank talking about release risk and why they couldn't upgrade their Oracle database schemas this way and that way and, you know, convert columns.
[519.96 → 522.98] And I think that's a lot of what Nix Cloud is doing under the hood too.
[523.36 → 524.92] So that makes sense.
[525.30 → 537.34] And I guess really the most practical thing, instead of ripping out my entire setup, which has been working great for a couple of years, would be just when Nix Cloud announces a new release, set a reminder in 30 days to do an upgrade.
[537.34 → 538.92] Speed dial Brent.
[539.02 → 539.58] That's what you got to do.
[540.28 → 541.78] Hey, do you think anything to know about in this release?
[541.86 → 548.76] No, but, you know, like give it like 30 days to cook or whatever and then just have a reminder pop up that says, okay, man, it's time to go do your upgrade.
[549.02 → 550.06] Don't fall too far behind.
[551.76 → 560.88] Over the holiday period, my iPad Pro met an untimely demise at the hands of a glass of red wine of my wife while she was playing video games at my computer.
[561.20 → 562.24] Oh, you outed her.
[563.74 → 564.10] Yeah.
[564.10 → 571.46] I mean, look, earlier in the year, full, well, last year, I spilt water over a brand new 16-inch MacBook Pro.
[572.02 → 577.32] So I didn't want to be the guy that ruined a MacBook Pro and an iPad Pro in the same year.
[577.44 → 578.96] Now, is this a 2018?
[579.34 → 579.90] That's what I have.
[579.94 → 580.88] Is I have a 2018 Pro.
[581.10 → 581.34] Yeah.
[581.78 → 582.60] It's quite an old one.
[582.72 → 582.98] Yeah.
[583.28 → 583.86] They've hung on.
[584.06 → 590.12] I was kind of waiting for the spring anyway to, you know, like, cause there's supposed to be a bunch of new display technology coming.
[590.12 → 593.14] And there was not a new iPad at all last year.
[593.42 → 594.26] No, no, no.
[594.36 → 597.14] So I've kind of been just patiently waiting.
[597.24 → 599.68] I don't use the iPad that much.
[599.88 → 602.86] If I'm honest, I use it as an auto cue on my cameras.
[602.86 → 609.76] I use the sidecar display mode to do the Teleprompter app and have it controlled through the keyboard and mouse on my desk in front of me.
[610.30 → 615.40] Actually, sometimes I put the keyboard on the floor and use the space bar to control the Teleprompter, which is a fun little trick.
[616.12 → 626.08] But I decided, because this happened a couple of days before I had to take a business trip to Phoenix, and it coincided with my dumping Plex completely as well for videos.
[626.08 → 632.14] I haven't really got a good way to do offline media downloads to an iPad now.
[632.46 → 636.24] Now, I'm not an Android Jellyfin app user, so you'll have to excuse my ignorance here.
[636.38 → 642.16] But could you not just swap in the Jellyfin app and download in there or whatever, sync, whatever they might call it?
[642.42 → 645.86] I can, but it only downloads at full quality.
[646.50 → 652.72] One of the nice things about Plex downloads was you could set, okay, it used to be per file or per series, a certain quality.
[652.72 → 654.80] And they removed that and made it a global setting.
[655.18 → 660.08] But you could say, hey, Plex, go and transcode all this media to 720p.
[660.22 → 664.82] I don't need the highest fidelity codex on the airplane, right?
[665.68 → 675.86] Well, unfortunately, Jellyfin just has, it does have a download button, but downloading 40 gig rips of things can take quite a long time.
[675.86 → 684.32] And also, with the Apple tax on storage, you know, I don't, I think I've only got, only got 256 gigs in my iPad.
[684.52 → 690.08] Oh, that'll go quick, though, when you're trying to do a couple of series or a movie or two that are high-res, and you already have stuff on there.
[690.34 → 697.04] The thing I like to do for plane rides is I like to completely over-subscribe the amount of media I've got available,
[697.14 → 700.22] because I never know what kind of mood I'm actually going to be in when I sit in that seat.
[700.22 → 700.66] Yeah.
[700.96 → 706.52] I put John Wick on the iPad, and I sat down to watch 10 minutes of it, and I was like, nah.
[707.00 → 709.60] And I just went back to Top Gear, because that was the kind of mood I was in.
[709.64 → 711.84] I just was in a silly mood, you know?
[711.90 → 717.02] And I like to have 10 series of Top Gear, 10 series of South Park, some Rick and Morty,
[717.22 → 724.10] just some complete asinine, silly brain food that just is, you know, I'm on a plane, I can't go anywhere,
[724.34 → 727.20] I'm just going to half-watch this and read a book or something.
[727.20 → 734.24] I'm very similar, or another kind of adjacent strategy that I have is here's season one,
[734.38 → 738.78] or maybe half of season one or whatever, depends on the flight, of a show I've been meaning to watch,
[738.82 → 739.94] and I'll do two or three of them.
[740.56 → 743.72] And then, like, depending on if the wife's with me or not, we'll see how we're both feeling,
[743.82 → 745.22] and maybe we'll pick one of those.
[745.32 → 745.60] Mm-hmm.
[746.18 → 747.14] And you just don't know.
[747.26 → 752.48] So you do want to have multiple choice, and that's why, absolutely, if you can, you want to –
[752.48 → 757.26] and you don't need – like you said, the iPad might be a nice screen, but it's tiny,
[757.46 → 761.04] and it's – you're on an airplane, 720p will do the job.
[761.94 → 765.24] Did you think about just – I mean, this is horrible or something,
[765.34 → 772.02] but you could set up, like, a small library and just use something like Handbrake and re-encode stuff.
[772.38 → 773.80] Well, I did do that last year.
[773.80 → 779.54] I actually, it turns out, in my tech pouch, had a one terabyte SSD that I'd pre-encoded a bunch of media to
[779.54 → 784.80] when Play did what they did last year for different qualities, different movies, et cetera, et cetera.
[785.34 → 790.52] But the iPad still turned on, so I could charge it through the Magic Keyboard case
[790.52 → 795.32] with the three POGO pins on the back, but I couldn't charge it through the USB-C port.
[795.40 → 800.68] So I've got this iPad in front of me and this USB SSD in front of me,
[800.68 → 805.70] and the two will not talk to each other. I cannot connect the two together, and it's really annoying.
[806.48 → 811.46] So it got me thinking, why don't iPads support micros cards?
[811.58 → 817.96] Wouldn't it just be the correct solution to the problem to have a device that supports micros cards?
[818.68 → 822.86] Which, of course, means looking across the fence at the Android side of the pond.
[823.48 → 827.08] And I got looking at different tablets. There's the OnePlus tablet, which looks great.
[827.08 → 831.30] Honestly, I was going to buy that one until I realized it didn't have a micros card slot.
[832.02 → 836.00] Looked at a few others. Samsung has a huge, huge range of different tablets.
[836.60 → 845.28] I ended up going with the S9 Plus, which is a 12.4-inch tablet with an AMOLED screen, I think.
[845.36 → 849.72] It's 120Hz, something like that, so it feels really nice under the fingers.
[849.86 → 853.08] You know, I'm a bit of a refresh rate snob these days.
[853.08 → 856.00] 60Hz on a tablet feels kind of gross.
[856.70 → 863.56] And it seems it also offers at least the stock one I'm looking at is either 256 or a 512GB option.
[863.74 → 865.36] I'm guessing you went 512?
[865.68 → 867.52] No, I went for the cheaper one.
[867.82 → 870.10] You did. Look at your restraint. I'm impressed.
[870.62 → 877.26] Mostly because I figured if I just get a couple of 1TB USB drives and load them up with Peppa Pig and stuff like that for Ella,
[877.26 → 879.20] when we're on airplanes and things.
[879.40 → 883.70] Oh, right. The SD card slot means you don't have to go crazy with the internal storage.
[883.84 → 884.20] Exactly.
[884.46 → 886.02] Oh, I'm still thinking iPad terms.
[886.22 → 891.94] Right. Yeah, so just, I mean, I can just use VLC or the Files app on Android.
[892.30 → 892.98] That's great.
[893.18 → 895.06] It's been a while since I've used Android.
[895.38 → 901.40] I'm still an iOS phone guy, and I think I will be for the foreseeable, but man, do I love Nova Launcher.
[902.08 → 902.58] Oh, really?
[902.58 → 904.28] It's so good.
[904.74 → 904.88] Yeah.
[904.88 → 912.70] Yeah, isn't it funny when you haven't been on a platform for a while, the things that are really have improved or just better than the one you're used to really stand out.
[913.48 → 920.40] I agree. I have always felt that Android is a better tablet OS than it is a phone OS.
[920.92 → 925.80] Since it first launched, that's been my commentary is this is okay, but it'd be great on a tablet.
[925.80 → 933.50] And then like they've never really super executed on the tablets, but I mean, it sounds like you've got a use case.
[934.00 → 936.58] Well, Samsung haven't been sleeping on it like a lot of people have.
[936.94 → 940.66] They've been keeping a lot of things revving at the low end of the market.
[940.66 → 945.32] And they released a couple of years ago, I think it was the S7 or the S8 was the first one.
[945.50 → 946.80] I have the S9 here.
[947.06 → 953.10] They released an ultra tablet, which is like a 15-inch tablet, which is just honestly, it's like a laptop.
[953.10 → 967.54] It's obscene to fit into an airplane seat, which is honestly, with the amount of travelling I'm doing for work these days, my primary use case for a tablet is something because the American Airlines planes have started removing the screens in the back of the seats in front of you.
[967.54 → 979.46] And they give you these little plastic clips that you can kind of like pull apart and then clamp a tablet or a phone into, which I love because I'm like, yes, finally, my tablet's not on my tray table or whatever.
[979.58 → 980.18] It's eye level.
[980.28 → 981.34] And that that's fantastic.
[981.34 → 992.36] And the really nice thing about the S9 tablets is their 16 by 10 aspect ratio compared to the iPad sort of four by three is, more rectangular better for videos.
[992.84 → 993.04] Right.
[993.16 → 993.78] For videos.
[993.96 → 996.26] This is where it's at, man.
[996.26 → 997.62] So it comes with the keyboard.
[997.74 → 1010.18] It comes with the pen, 12.4 inches, Wi-Fi 6E, AMOLED screen, and it's multiple hundreds of dollars cheaper than the iPad Pro.
[1010.28 → 1010.56] Yep.
[1011.14 → 1013.32] Before you even get the keyboard or the pencil.
[1013.88 → 1014.12] Yeah.
[1014.44 → 1018.30] And I can run emulation games on it, too, which, I mean, I haven't gotten there yet.
[1018.30 → 1018.62] Yes.
[1018.70 → 1021.16] Because I only got it last week and I had a trip to do, but.
[1021.26 → 1024.60] I mean, you could even sideload apps as crazy as that sounds, but you could if you wanted to.
[1024.60 → 1024.64] Yeah.
[1024.98 → 1025.20] Yeah.
[1025.20 → 1026.74] That smart tube's pretty great, huh?
[1026.82 → 1036.34] How is the Samsung, you know, overall influence on the interface, on the I don't know, just the experience.
[1036.42 → 1038.20] Is it very Samsung-y?
[1038.32 → 1039.22] Is it minimal?
[1039.44 → 1039.92] How is that?
[1040.16 → 1040.70] It's fine.
[1040.70 → 1045.58] It reminds me of what OnePlus were doing a couple of years ago when I switched away from OnePlus.
[1045.90 → 1047.74] I mean, it's definitely not stock Android.
[1048.56 → 1050.38] It's definitely got a Samsung flavour to it.
[1050.44 → 1052.38] I mean, there are a bunch of apps pre-installed and stuff.
[1052.58 → 1054.62] Do you happen to know which version of Android it is off the top of your head?
[1054.94 → 1055.72] I can check.
[1055.86 → 1057.58] I have it on the table right here next to me.
[1057.60 → 1058.04] Oh, well, okay.
[1058.16 → 1058.92] Let's find out.
[1059.60 → 1063.56] That's always like a weird benchmark for me is like, can Samsung ship a current version of Android?
[1064.34 → 1065.74] If they can, then they've got my attention.
[1066.82 → 1067.92] Seems like a really nice device.
[1067.92 → 1072.20] So the version of Android that this tablet has right now is Android 14.
[1072.64 → 1073.44] That's not bad.
[1073.50 → 1073.74] Okay.
[1074.74 → 1075.36] All right.
[1075.48 → 1076.24] Hey, look at that.
[1076.52 → 1076.74] Yeah.
[1077.46 → 1078.96] Oh, I'm very impressed.
[1079.42 → 1079.98] All right.
[1080.02 → 1081.28] Well, it passes the Chris Fisher test.
[1081.56 → 1082.94] And you're satisfied with it.
[1082.98 → 1083.52] You like it.
[1083.90 → 1085.72] Well, I've had it for a week.
[1085.96 → 1088.88] I've taken a trip with it, and it did everything I needed to do.
[1088.94 → 1090.10] The battery life was fabulous.
[1090.94 → 1095.96] It made it through a five-hour flight, Raleigh to Phoenix, no problem.
[1095.96 → 1097.94] Have you put the Home Assistant app on it?
[1098.46 → 1098.66] Yes.
[1099.08 → 1102.42] Have you looked at all the freaking sensors that are in Home Assistant now?
[1103.14 → 1103.54] No.
[1103.98 → 1104.86] Oh, it's bonkers.
[1105.10 → 1106.90] It's bonkers with the Android app.
[1107.18 → 1115.98] Well, so you could, you start looking at that, you could really set some really great travel automations, those types of things, just based on where your tablet's at and what the sensor's reading.
[1115.98 → 1117.24] Well, that's interesting.
[1117.44 → 1118.76] Maybe I'll take a look at that.
[1119.38 → 1129.80] Now, one other thing that really piqued my interest about this tablet was the fact that I can basically turn it into almost Chromebook using Samsung DEX.
[1130.24 → 1131.90] Single cable, USB-C.
[1132.06 → 1135.28] I plug it in, and it basically turns it into a desktop computer.
[1135.82 → 1140.36] There's none of this iPad nonsense of stage manager and trying to manage multiple windows.
[1140.36 → 1146.30] Apple are trying to reinvent the wheel when it comes to a tablet and I just don't think they're executing.
[1146.46 → 1149.28] They're just not doing a good job with the software side of the iPad.
[1149.64 → 1153.22] The hardware is years ahead of where the software is on the iPad.
[1153.98 → 1161.42] Whereas on the Samsung with DEX, I've basically got a full-on window manager as if it was just a normal Chromebook.
[1161.58 → 1162.66] I can drag and drop windows.
[1162.78 → 1163.76] I can resize them.
[1163.88 → 1164.64] I can use a keyboard.
[1164.74 → 1165.46] I can use a mouse.
[1165.46 → 1168.96] It's fabulous to have that flexibility.
[1170.40 → 1173.36] Yeah, really, especially when you're in a pinch.
[1173.70 → 1181.74] That's always when I really feel like a tablet falls down is when there's something that's kind of critical happening and I need a lot of input or whatever it might be.
[1181.82 → 1183.00] That's super great, Alex.
[1183.54 → 1187.28] I guess my standard questions don't really apply for these types of things, but battery life must have been decent.
[1187.40 → 1188.50] You haven't mentioned anything about that.
[1189.06 → 1190.06] Yeah, it was fine.
[1190.30 → 1192.90] It was fully charged when I left the house.
[1193.30 → 1194.12] Does it get hot?
[1194.12 → 1194.56] No.
[1195.46 → 1200.20] 50% by the time I got home and I used it for the entire five-hour flight, so it's fine.
[1200.36 → 1202.24] It sounds like they finally have figured it out.
[1202.66 → 1202.84] Yeah.
[1203.24 → 1203.74] That's nice.
[1204.68 → 1205.40] All right, you sold me.
[1205.46 → 1205.90] I want one.
[1206.78 → 1207.96] Putting that on the birthday list.
[1208.24 → 1209.08] Well, they do make a couple.
[1209.28 → 1215.28] I got the S9 full-on version, which has the high refresh rate and a Snapdragon processor.
[1215.66 → 1224.00] They do make one that's half the price that has an LCD screen and an Enos chip, slightly lower refresh rate, that kind of stuff, for half the price.
[1224.00 → 1228.54] So if your super price sensitive, then the FE edition is the one you want.
[1228.54 → 1237.66] Also, the S8 Plus, low latency S Pen as well, 128 gigs, 120 hertz refresh, 12.4-inch AMOLED screen, $499.
[1237.66 → 1240.46] So also pretty price competitive.
[1240.52 → 1241.12] Yeah.
[1241.12 → 1249.94] I didn't really anticipate dropping Plex was going to cost me a few hundred bucks in terms of syncing videos, but here we are.
[1249.94 → 1257.02] It really is just a downstream series of, what do you call it, ramifications that I hadn't foreseen.
[1257.66 → 1265.96] But I think in the long run, you know, if Jellyfin can add a feature where I can set when I press download, what quality do you want this to be at?
[1266.90 → 1269.30] Oh, that would just be chef's kiss.
[1269.72 → 1270.34] Maybe one day.
[1270.34 → 1275.58] Speaking of Jellyfin, the Jellyfin transition sounds like it's complete for you.
[1275.70 → 1278.44] I have a – it's interesting.
[1278.54 → 1283.64] I have all my personal watching happening on Jellyfin, but I still have a Plex instance going for family.
[1284.06 → 1287.84] And I don't – I'm going to have to, like, go to their house and replace devices.
[1288.16 → 1289.24] So it's going to be a process.
[1289.24 → 1298.90] But I've been really enjoying just sort of having that decision finalized, moved on, everything's working.
[1299.68 → 1302.24] And so now it looks like it's time to pull some data out of there.
[1302.82 → 1304.62] It looks like you found a project called Jelly stat.
[1305.20 → 1307.38] And I'm going to guess what this one does, Alex.
[1307.44 → 1309.80] I'm going to guess this is for Jellyfin statistics.
[1310.78 → 1313.46] Well, you're familiar with Tautly on the Plex side of the fence.
[1313.68 → 1314.48] Indeed, yeah.
[1314.76 → 1317.00] This is basically Tautly for Jellyfin.
[1317.00 → 1317.96] It's called Jelly stat.
[1318.44 → 1321.78] Pulls in a bunch of statistics from your Jellyfin server.
[1322.46 → 1322.86] Jelly stat.
[1323.28 → 1328.02] How many movies I have in my library, how many TV shows, how many episodes, et cetera, et cetera.
[1328.48 → 1335.90] Who's watched what, when they were last seen, their watch time in minutes, the number of plays they've had, et cetera, et cetera.
[1336.62 → 1337.12] That's it.
[1337.32 → 1337.72] Jelly stat.
[1337.92 → 1338.50] It's pretty awesome.
[1338.68 → 1340.42] It works exactly as you would hope.
[1341.08 → 1345.86] You know what's interesting about it, though, is it does show you that – because there's some irony here, right?
[1345.86 → 1354.56] Because, like, what made you move to Jellyfin was that Plex was sharing data kind of similar, only vaguely, just partially with these displays.
[1354.92 → 1356.22] But Plex was showing that data.
[1356.42 → 1362.08] And both of us were so offended, we left, even though we still have lifetime subs.
[1362.72 → 1365.12] But then once we get a Jellyfin server set up, what do we do?
[1365.56 → 1369.76] Set up Jelly stat where it tells us all of this and way, way more data.
[1369.86 → 1371.42] It's like we definitely want the data.
[1371.96 → 1373.78] We just want to have control over that data.
[1374.28 → 1376.62] Yeah, it's the cloud authentication piece, really, isn't it?
[1377.00 → 1381.76] And the fact that we don't know – I mean, we had this discussion at length in a previous episode.
[1382.00 → 1385.08] But it's just we don't know what Plex are doing with that data.
[1385.20 → 1394.36] We don't know when they have data breaches, who has taken that information, and at what point it's going to be turned around and used as a foot gun against ourselves.
[1394.36 → 1402.20] So for me, the main reason I want to know this stuff is just how many transcodes are happening.
[1403.12 → 1406.26] Because I gave Brent access through Tail scale.
[1406.40 → 1410.36] I did a shared node and shared this server with him over Tail scale.
[1411.22 → 1420.12] And it would just be good for me to know how many files are direct play and how many are transcoded so that I know these – I don't share media with many people anymore like I used to.
[1420.12 → 1425.04] And for me, the hardware requirements to do so with Quick Sync became a lot easier.
[1425.14 → 1426.48] But I'd still like to know this stuff.
[1426.64 → 1428.94] I'm like, how much am I transcoding without even realizing?
[1429.14 → 1430.14] Like, just trends.
[1430.26 → 1431.24] I'm using it for trends.
[1432.40 → 1435.10] Open SSH 9.5 is out.
[1435.88 → 1439.76] There are a couple of rather significant bugs in there that get fixed.
[1440.58 → 1442.70] But I don't think that's probably why you want to talk about it.
[1443.26 → 1446.04] No, I'm a big fan of SSH keys.
[1446.04 → 1448.92] It's a bit of a problem, honestly.
[1449.94 → 1459.10] The 9.5 release of Open SSH makes ED25519 SSH keys now the default.
[1460.12 → 1463.66] These are elliptic curve Diffie-Hellman keys.
[1464.06 → 1471.78] And they are very short, very easy to copy and paste around compared to, dare I say, the old school RSA keys.
[1471.78 → 1475.44] Which were, I think, four or five lines worth of characters typically.
[1475.64 → 1483.40] Whereas an ED25519 key is maybe 50 or 60 characters at most.
[1484.12 → 1485.96] It just becomes a lot easier to handle.
[1486.22 → 1491.66] And they're more secure with the elliptic curve cryptography that's used to sign them and stuff like that.
[1491.82 → 1493.98] So, great to see that come out.
[1494.06 → 1497.14] They were originally added in January 2014.
[1497.14 → 1503.28] So, this should give you an idea of the pace of Open SSH as a project and cryptography in general.
[1503.70 → 1504.76] Moves very slowly.
[1504.90 → 1506.00] These things have been well tested.
[1506.72 → 1509.40] And so, to see them as the default now, I just think is great.
[1511.28 → 1513.92] Talescale.com slash self-hosted.
[1514.16 → 1515.72] Oh, what a game changer for me.
[1515.82 → 1516.70] Go over there right now.
[1516.78 → 1517.60] Support the show.
[1518.12 → 1521.62] And create an account for up to 100 devices and three users.
[1521.74 → 1523.62] That's Talescale.com slash self-hosted.
[1524.14 → 1524.74] So, what is it?
[1524.74 → 1529.26] Well, it's the easiest way to connect devices and services directly to each other, wherever they are.
[1529.30 → 1530.70] I'll get to that more in a moment.
[1531.14 → 1531.92] It's fast.
[1532.26 → 1533.58] Like, really, really fast.
[1533.64 → 1534.12] It's private.
[1534.12 → 1537.40] It's built on top of WireGuard's noise encryption.
[1538.22 → 1540.14] And it's really programmable networking.
[1540.98 → 1542.82] It's private and secure by default.
[1543.46 → 1546.80] Zero-trust networking that's easy to deploy, easy to use.
[1547.32 → 1549.46] And so, I'm using it for more and more now.
[1549.46 → 1552.74] What's really been a game changer for me is these service containers.
[1553.38 → 1556.16] And just putting services directly on my Tail net.
[1556.44 → 1560.38] So, when somebody wants to go to Jellyfin, you just go to the name of the Jellyfin server.
[1560.82 → 1561.88] One of them is called Hollywood.
[1562.46 → 1569.36] When you want to go watch the Hollywood server, you know, when you open up the Jellyfin app, you just put HTTP colon slash Hollywood in there.
[1569.86 → 1572.26] And I have the search domain all set for the Tail net.
[1572.26 → 1574.14] You don't even have to put the domain in there.
[1574.84 → 1576.74] It's so smooth, and it's so instant.
[1576.84 → 1579.14] It also means easy access to buy containers.
[1579.82 → 1583.64] As the longer I use Tail scale, I'm loving the new ways that I deploy it.
[1584.48 → 1586.22] I mean, yes, I started using it as a VPN.
[1586.90 → 1589.68] Now, I'm fundamentally re-architecting the way I use networking.
[1589.80 → 1591.34] I'm not using reverse proxies anymore.
[1591.94 → 1593.52] I don't have inbound ports.
[1594.08 → 1595.84] I don't have anything on the public internet.
[1596.28 → 1599.38] I'm spread across multiple homes and multiple businesses now.
[1599.44 → 1601.48] And I'm using ACLs to keep it all separated.
[1601.48 → 1604.30] I mean, it is beyond VPN.
[1604.96 → 1606.96] It is literally programmable networking.
[1607.74 → 1611.80] And the more I wrap my head around it, the more I realize it's going to fundamentally change the way I do things.
[1611.98 → 1613.12] And for the better, too.
[1613.78 → 1615.44] Secure by default, private by default.
[1615.86 → 1616.84] It's really great stuff.
[1617.38 → 1617.90] Go try it out.
[1617.96 → 1618.48] Support the show.
[1618.86 → 1620.86] Get it on all your devices up and running in just minutes.
[1621.16 → 1621.78] I'll say this.
[1622.28 → 1623.74] Even 32-bit devices.
[1624.62 → 1627.54] Yeah, I had it recently running on the Debian 32-bit system.
[1627.64 → 1629.40] They still package it for 32-bit.
[1629.46 → 1630.22] Can you believe it?
[1630.22 → 1631.92] I mean, really, they have it for just about everything.
[1632.44 → 1633.10] All right, go try it.
[1633.18 → 1633.56] Support the show.
[1633.62 → 1635.82] Talescale.com slash self-hosted.
[1637.76 → 1643.08] You mentioned over the holiday period you've been doing a bunch of generation on your home infrastructure.
[1643.86 → 1645.66] Audio bookshelf is in the dock.
[1645.76 → 1646.66] What have you been doing with that?
[1646.66 → 1654.20] Well, speaking of ramifications of leaving Plex, this is also how the wife was doing audiobooks, and I was doing audiobooks.
[1654.36 → 1654.90] Ruhr.
[1655.14 → 1656.28] Yep, yep, yep, yep.
[1657.02 → 1661.48] And, you know, over the years you and I have seen recommendations to check out audio bookshelf come in.
[1661.54 → 1663.50] And I figured now is my chance to do it.
[1663.52 → 1665.36] I've got to come up with a solution for this.
[1665.42 → 1666.66] I've got these audiobooks.
[1666.66 → 1667.36] I've got to do something.
[1667.36 → 1678.44] So I installed audio bookshelf, which generally works best if you have an already organized directory structure, and they give you some documentation on how to do that.
[1678.50 → 1679.92] So I'll link that in there.
[1680.08 → 1690.22] But I got lucky because I've done one flat directory with all of my audiobooks just in there as a file, always assuming I'd have a front end to all the metadata information.
[1690.22 → 1691.50] And that also works.
[1691.50 → 1694.48] It's a very simple Docker container to get set up.
[1694.58 → 1702.70] What I did slightly different with mine is I took out all of their networking that comes with their Docker Compose example.
[1703.04 → 1710.34] And I added a tail scale service container above it that does a connection to my tail net.
[1710.68 → 1719.08] And then I set the audio bookshelf application container network mode to use the tail scale services container.
[1719.08 → 1724.84] So the audio bookshelf container isn't actually on the network at all anymore.
[1725.20 → 1739.28] It's speaking directly to the tail scale services container, which I then Docker exec in, do an up, authorize, and then boom, it's now on my tail net as whatever host name I put in the Docker Compose.
[1739.62 → 1741.24] In this case, it was books.
[1741.24 → 1753.56] And so the wife gets home a few minutes after I've done this, Alex, and it was, you know, like I remember I shared the story about we were watching a movie, and it died at the end, and we couldn't get it to work.
[1753.62 → 1755.46] And that's why we went back to Plex for a bit.
[1755.78 → 1756.92] This is the reverse moment.
[1757.38 → 1760.72] This is the moment where you haven't tested it, but it works.
[1760.76 → 1762.82] And it's so amazing.
[1762.82 → 1764.06] So the wife gets home.
[1764.12 → 1764.66] She's like, what are you doing?
[1764.92 → 1770.22] And I'm like, oh, I was just getting our new audiobook server going, which she's a big, big audiobook user.
[1770.46 → 1772.48] She's immediately, she tunes in.
[1772.90 → 1773.44] Oh, really?
[1773.50 → 1773.92] She says.
[1774.80 → 1777.82] I say, yep, they have an Android app and they have an iOS app.
[1777.86 → 1779.64] So go ahead and install it, and I'll show you how to connect.
[1779.72 → 1783.06] So she installs the audio bookshelf app, opens it up.
[1783.16 → 1784.48] First thing it wants, right, is a URL.
[1785.02 → 1788.52] I tell her, put in HTTP books.
[1789.26 → 1792.12] And she says, well, I mean, I have to have like a .com or something.
[1792.12 → 1794.88] I'm like, no, HTTP books.
[1795.42 → 1798.34] And I'm like, oh, God, please work because I hadn't tested it yet.
[1799.42 → 1805.80] But I know she has Tail scale on her phone, and it's usually always on because I have it like a couple of different shortcuts to keep it connected.
[1806.68 → 1809.06] And sure enough, she hits the login button.
[1809.12 → 1811.28] She puts her name, hits the login button and it connects.
[1811.86 → 1815.04] And there is all her books right there.
[1815.12 → 1818.34] And it was a glorious self-hosting moment.
[1818.34 → 1824.20] And it's really nice because at the top of Audio bookshelf, you can switch through everybody's book library.
[1825.30 → 1831.24] And Audio bookshelf does a fantastic job of organizing books in collections and series.
[1831.24 → 1836.04] So I have a lot of series of books, like the Expanse series, for example.
[1836.60 → 1839.54] And you can put them all in there and then play them chronologically.
[1839.90 → 1841.54] And I can also create collections.
[1841.92 → 1847.46] So I have like Star Trek collections and Bitcoin collections and all these different kind of collections that I can link out.
[1847.66 → 1849.28] And the family can play if they want.
[1849.28 → 1858.92] So talk me through that DNS situation because just typing the word books shouldn't work.
[1859.18 → 1860.44] How did you figure that out?
[1860.44 → 1860.82] Ha ha!
[1861.52 → 1865.38] Well, it's magic, magic DNS a bit.
[1865.62 → 1873.28] So magic DNS essentially just turns on a DNS resolver for your local Tail net land name, domain name.
[1873.38 → 1876.26] So like mines whatever.whatever.net or whatever.
[1876.26 → 1881.26] And so it just makes that the default search domain for Tail net clients.
[1882.24 → 1890.28] And then after that, I have a DNS server that I'm running in the Tail net running.
[1890.46 → 1896.18] It's actually Spyhole that also is acting as a DNS server that I've put some custom host names in.
[1896.28 → 1901.12] And it also is in that same domain as the Tail net.
[1901.42 → 1904.46] So it's the same local search domain as well.
[1904.54 → 1905.14] Does that make sense?
[1905.14 → 1914.16] So it's just like if I was outside of that, I would have to put the – if like you tried to connect to my Tail net,
[1914.40 → 1922.68] you would have to use the full Tail net host name because your local search domain would be your Tail net if you had magic DNS turned on.
[1923.20 → 1924.22] Yeah, makes perfect sense.
[1924.76 → 1927.18] So just a magic DNS entry is all you need.
[1927.18 → 1934.16] I've done some fancy stuff with split DNS in the past to achieve not quite as nice as what you have here.
[1934.36 → 1939.78] But there's also an internal Tail scale project called Go Slash Links, which I'll put a link to in the show notes,
[1940.16 → 1945.36] which we use internally to share, you know, like who owns which particular part of the product.
[1945.62 → 1948.36] We just have a Go Slash Which or Go Slash Who.
[1948.36 → 1949.46] I forget which one it is.
[1950.10 → 1953.48] And this just opens up a document with everything that's in there.
[1953.58 → 1958.98] And so, you know, you can build out internal directory link shortening structures with this kind of stuff too.
[1959.12 → 1967.84] I mean, when you start adding individual containers to the Tail net as individually resolvable machines, nodes,
[1968.22 → 1973.26] whatever you want to call them, you can do some fun stuff like Chris has just found out.
[1973.26 → 1976.78] I didn't explain it very well because I was just explaining how I have it structured,
[1976.92 → 1980.16] but I'd like to now explain the end result because that might be more understandable.
[1980.46 → 1988.82] The end result is I now have Audio Bookshelf and VS Code Studio and Jellyfin and several other applications,
[1989.26 → 1991.66] including a notes' application.
[1992.58 → 1994.76] None of them are using a reverse proxy.
[1995.16 → 1996.36] I don't have any Nginx.
[1996.52 → 1997.28] I don't have traffic.
[1997.28 → 2004.30] I'm not doing anything to route traffic to them because they are coming onto the Tail net directly.
[2004.70 → 2010.24] Whatever host name I configure in that Docker Compose, they show up as on the Tail net directly.
[2010.74 → 2017.54] And so everything is communicating over the Tail net and nothing has to be like routed through Nginx or anything like that.
[2017.64 → 2021.52] So it actually, I know this, when I explain it, it sounds very complicated.
[2021.52 → 2032.22] But when you understand it, it's actually easier to implement than typical because you don't have any kind of reverse proxy to set up at all.
[2032.56 → 2034.68] And everything is secured by the Tail net.
[2034.84 → 2042.90] And if you need to do SSL, there's actually an integration with Let's Encrypt to get an SSL cert for objects on your Tail net.
[2043.04 → 2045.06] So it's like even that's easier.
[2046.10 → 2050.56] I mean, I tell you, Alex, when I figured this out, I was just like, well, I'm redoing this machine.
[2050.56 → 2051.40] I'm redoing this machine.
[2051.48 → 2054.80] I'm redoing this machine because the family's all spread out.
[2055.28 → 2058.14] Sometimes the kids are with their mom and, you know, Aaliyah's at the RV.
[2058.28 → 2060.58] I'm here at the studio or whatever's going on.
[2060.88 → 2063.40] We're all spread out, but we want to access the same resources.
[2064.18 → 2065.86] And sometimes those resources are at the RV.
[2066.00 → 2066.90] Sometimes they're at the studio.
[2067.12 → 2068.14] Sometimes they're at Age's house.
[2068.26 → 2069.28] They literally move.
[2070.72 → 2075.86] It doesn't hit you until you are sat in a for me at least, you know,
[2075.86 → 2081.74] I have all the services across this house, my mom's house, my mother-in-law's house,
[2081.84 → 2085.22] all completely unified on my Tail net.
[2085.70 → 2089.76] It doesn't really hit me until I'm in a hotel in Phoenix and then try and access something in this house
[2089.76 → 2091.12] and then something in my mom's house.
[2091.20 → 2094.24] And it's like, oh yeah, I've just got a flat network.
[2094.34 → 2095.94] It doesn't matter where in the world I am.
[2096.10 → 2097.50] Like, you know, it's sorry.
[2097.60 → 2099.26] This sounds like a Tail scale commercial.
[2099.38 → 2100.88] It really, this isn't the read.
[2100.88 → 2102.70] It's just, it's just a cool project.
[2103.10 → 2107.32] And what was great is Dylan was also very big on audiobooks for going to sleep.
[2107.50 → 2109.44] And so I could just tell him the same thing.
[2109.98 → 2114.42] Open up your app, go to this URL, and now you're on there.
[2114.52 → 2119.64] And it's like, I could just roll this out to my kids, even though they weren't with me that night.
[2120.26 → 2122.44] Because we're all, we all have access to that resource.
[2122.50 → 2124.84] And I just think that's, oh, I love it.
[2124.88 → 2125.60] I love that mesh.
[2125.66 → 2127.66] I love that mesh one flat network thing.
[2127.66 → 2133.52] And then to get them on that, to get the container applications on that network
[2133.52 → 2137.52] without having to do any kind of reverse proxy setup,
[2138.34 → 2141.08] it's like, I feel like it's just even faster now to get started.
[2141.46 → 2144.26] Like, because once it's connected, it's got a name.
[2144.70 → 2145.14] It's DNS.
[2145.78 → 2146.96] It's just, I'm good to go.
[2147.08 → 2147.76] It's like, wow.
[2148.60 → 2149.64] Ah, it was great.
[2149.76 → 2151.88] It was a really productive holiday break.
[2152.52 → 2156.86] I feel like the cloud opened, and we had angelic, oh, music playing.
[2156.86 → 2157.26] Yeah.
[2157.44 → 2158.46] Oh, it was so nice.
[2158.48 → 2159.24] I can picture it now.
[2160.82 → 2164.32] Well, I'm glad that you keep your lady friend happy with audiobooks.
[2164.46 → 2169.62] I had to keep mine happy with a PDF editor or PDF tool the other week.
[2169.68 → 2171.02] She was signing a contract for something.
[2171.80 → 2175.78] And there's always that whole dance of, have we got Acrobat installed?
[2176.00 → 2177.72] Has my Adobe subscription lapsed?
[2178.36 → 2179.28] Blah, blah, blah, blah, blah.
[2179.28 → 2188.76] Well, I'm very pleased to tell you about your locally hosted one-stop shop for all of your PDF needs, Sterling PDF.
[2189.26 → 2190.96] You know, at first I was like, what?
[2191.28 → 2194.40] And then I started looking into it, and I'm like, hmm, okay.
[2194.42 → 2195.98] So I'm setting this up after the show.
[2196.36 → 2198.06] It does a lot of basic stuff.
[2198.18 → 2200.36] Like it can rotate PDFs.
[2200.36 → 2202.76] It can convert an image to a PDF and that kind of stuff.
[2202.76 → 2204.62] But it can also add watermark.
[2204.72 → 2205.02] That's cool.
[2205.14 → 2209.94] But then I see in here some really serious things like change and edit metadata.
[2210.10 → 2210.86] That could be massive.
[2211.60 → 2213.86] And then OCR and cleanup.
[2214.60 → 2216.08] That's an option in here.
[2216.46 → 2228.74] All the basic stuff you might want to do with a PDF, like split pages, add pages, put a signature on it, put a password on it, compress it, you know, turn it into an image, turn an image into a PDF, rotate it.
[2228.74 → 2233.32] Of course, view a PDF as well if you want to view a PDF.
[2233.86 → 2233.94] Yeah.
[2234.44 → 2238.48] Extract certain pages, split the PDF up, you know, like goes on and on.
[2238.84 → 2244.68] It really is just killed Adobe Acrobat in one fell swoop, this application.
[2245.36 → 2248.18] So we used it for a couple of contracts, like I said, that we signed recently.
[2249.02 → 2250.92] Works fantastically well.
[2251.00 → 2256.72] So if you need to edit PDFs in any capacity, Sterling PDF is a web service.
[2256.72 → 2260.84] So you would host this, I'm using, of course, a container on my primary server.
[2261.72 → 2263.32] And then it's just a web app.
[2263.32 → 2272.38] So I don't even need any software installed on my computer anymore, which is like, oh, it's just, that's the way every piece of software should be like this.
[2272.64 → 2276.26] It's always agnostic that way too, which is, it's a checkbox for me.
[2276.26 → 2278.22] And that's one I'm installing after the show.
[2278.28 → 2280.08] I think I'm going to install this next one, I suspect.
[2280.92 → 2284.34] But before you tell me about this, I just want you to be aware.
[2284.42 → 2287.54] You kind of take, you may be taking away like my top use for Obsidian.
[2288.12 → 2288.60] Oh, no.
[2289.36 → 2291.18] Well, I will be honest.
[2291.24 → 2293.82] I got this one from, I think it was a self-hosted Subreddit.
[2293.82 → 2298.00] And I had to double-check which Subreddit I was actually looking at when I saw the name of it.
[2298.32 → 2300.88] Because this application is called Lube Log.
[2301.56 → 2301.96] Oh.
[2303.40 → 2305.30] Well, you want to keep track of that too, I suppose.
[2305.54 → 2306.28] It's a vehicle.
[2306.60 → 2308.54] Where is your mind at, sir?
[2308.54 → 2309.30] Oh, for the car.
[2309.70 → 2310.64] Yes, yes.
[2311.06 → 2313.96] Vehicle Service Record and Maintenance Tracker.
[2315.06 → 2315.90] I don't know what you were thinking.
[2316.70 → 2320.08] This is honestly an embarrassment of mine.
[2320.18 → 2324.44] Because I have like logs that I have handwritten before I got Obsidian.
[2324.64 → 2325.50] And then I have Obsidian.
[2325.66 → 2330.36] But then, of course, I have various different iterations on the format of how I logged things over time.
[2330.96 → 2333.00] It is actually, I'm not kidding, it's embarrassing.
[2333.38 → 2336.76] So, God, I love the idea of something that's just a standardized application.
[2336.92 → 2338.38] They don't have any screenshots though, Alex.
[2338.40 → 2339.20] That concerns me.
[2339.98 → 2341.44] Tell me it's not awful to use.
[2342.02 → 2342.84] It's just a web app.
[2342.84 → 2348.02] If you look in there, in the GitHub repo, which will be linked in the show notes, there is a docs' folder.
[2348.28 → 2350.14] And you can have a look at a couple of screenshots in there.
[2350.52 → 2350.72] Okay.
[2351.08 → 2353.40] So, you add, you know, specific vehicles.
[2353.76 → 2359.20] And then, you know, every time you fill the car up with fuel, you can say, right, my odometer said this.
[2359.32 → 2362.54] And it will give you an average consumption of miles per gallon.
[2362.98 → 2364.90] And, you know, how much.
[2364.92 → 2365.04] Do you do that?
[2365.64 → 2366.50] Do I do that?
[2366.56 → 2366.74] No.
[2366.74 → 2367.12] No.
[2367.12 → 2367.28] No.
[2367.56 → 2373.62] This application pick is one of those podcaster public service announcements.
[2373.84 → 2376.34] It's not an application I actually want or need.
[2376.66 → 2380.26] Oh, I do if I could actually log oil changes and maintenance on my car.
[2380.76 → 2380.98] Yeah.
[2381.02 → 2382.90] Well, I think you could absolutely do that with this one.
[2383.06 → 2384.44] I'm looking at the service record right now.
[2384.46 → 2385.12] You absolutely can.
[2385.50 → 2387.08] That I genuinely am going to use.
[2387.40 → 2388.70] Fuel, not so much.
[2388.98 → 2393.10] As you say, I have discovered the joys of Obsidian for such tasks.
[2393.10 → 2395.16] And I just keep it all in Obsidian these days.
[2395.80 → 2396.06] Yeah.
[2397.00 → 2399.70] But it looks like it's a pretty easy stand-up either way.
[2400.52 → 2402.76] And the name, you know, not hard to forget at all.
[2402.86 → 2403.20] Lu blog.
[2405.36 → 2407.50] Self-hosted. Show slash SRE.
[2407.64 → 2411.08] Please consider becoming a member and supporting the production directly over there.
[2411.58 → 2413.04] We'll also give you a little bonus content.
[2413.16 → 2416.32] You get a new feed, which will have some upgrades in the not-too-distant future.
[2416.64 → 2418.84] But you get a new feed with a post-show.
[2419.24 → 2423.08] As a way of saying thank you for supporting us, we give you a little extra content.
[2423.08 → 2427.02] And something else you might consider doing is boosting each production individually.
[2427.52 → 2431.04] I like this because automatically there's a split system in there.
[2431.44 → 2432.88] So a portion of your boost goes to me.
[2433.18 → 2435.74] A portion of your boost goes to the show production, which also covers Alex.
[2436.34 → 2440.02] And a portion of it goes to Editor Drew and the Pod verse development team,
[2440.14 → 2442.98] who are building an open-source podcasting app that we really like.
[2443.00 → 2444.44] And we use their player on our website.
[2445.20 → 2449.78] So when you boost the show, you're kind of immediately boosting the entire ecosystem around the show as well.
[2449.78 → 2451.04] And the splits all do that.
[2451.12 → 2453.48] Everybody gets their piece automatically, instantly.
[2453.94 → 2459.14] And I think it's a nice option for this show because the entire infrastructure can be self-hosted to do that.
[2459.44 → 2460.72] And it is a lot of fun.
[2460.76 → 2461.46] It is challenging.
[2461.80 → 2462.68] It is not easy.
[2463.42 → 2468.96] It is definitely one of the more endurance hikes in Home lab.
[2468.96 → 2474.28] But there's versions and sizes and different ways to go for all types.
[2474.90 → 2481.66] And so you can really build something neat that is self-hosted, programmable money that you can shoot around over TCP IP.
[2482.12 → 2485.08] And one of the things you can do with it is support the production here.
[2485.86 → 2487.86] You go get a new podcast app if you want to do it that way.
[2488.12 → 2489.10] PodcastApps.com.
[2489.60 → 2492.86] Fountain1.0 is just chef's kiss.
[2492.96 → 2493.28] Great.
[2493.82 → 2494.52] So good.
[2494.52 → 2495.70] I mentioned Pod verse.
[2495.86 → 2496.86] Absolutely fantastic.
[2497.02 → 2497.50] GPL.
[2497.86 → 2499.42] And cross-platform as well.
[2499.50 → 2502.86] It's available on mobile, iOS, Android, and the web.
[2503.64 → 2508.74] I like to mention that because a use case for me when I was commuting is I would sometimes want to finish the podcast at my desk.
[2508.78 → 2509.76] And it's great for that.
[2511.00 → 2512.50] Automatic is fantastic on iOS.
[2512.62 → 2513.94] They all support boosting.
[2514.46 → 2518.90] And some of the other features the network is rolling out, like livestream, right there in the podcast app.
[2519.46 → 2524.08] When, say, Linux Unplugged or Code Radio or a special event down at scale with Alex and me,
[2524.52 → 2529.82] when that is happening, it'll be in the Jupyter Station live feed, which is in the Podcasting 2.0 apps.
[2530.16 → 2532.38] And you get to listen right there in your podcasting app.
[2532.50 → 2536.48] You don't have to go to a different app to catch our livestream, which just never made sense anyway.
[2537.14 → 2538.80] Podcasting has needed that for a long time.
[2539.26 → 2544.34] So it's worth jumping on that because Podcasting 2.0 is all an open standard, lots of great features in there,
[2544.40 → 2549.34] like transcriptions, chapters, the live tag, like I mentioned, and, of course, boosting.
[2549.34 → 2558.04] And all of that, all of it, all of that technology, all open source, all self-hostable, all sovereign tech, all of it,
[2558.08 → 2559.54] none of it owned by a big company.
[2559.96 → 2561.54] So it's a pretty cool initiative to support.
[2562.52 → 2564.70] It's, you know, I mean, I say my piece.
[2565.14 → 2566.40] You also get to support the show, too.
[2566.92 → 2567.94] So there are a couple options in there.
[2568.32 → 2572.30] You can support us directly with your Fiat Fund coupons and invest in the ongoing production, essentially,
[2573.02 → 2574.72] at self-hosted.show.SRE.
[2574.72 → 2578.60] Or boost a production, send a message in and send support to that individual production,
[2578.96 → 2581.60] and then immediately split it out into the ecosystem around the show.
[2582.70 → 2583.62] They're both really appreciated.
[2584.16 → 2586.02] They both mean a lot during the Apocalypse.
[2586.82 → 2592.72] Self-hosted.show.SRE and newpodcastapps.com or just podcastapps.com.
[2595.12 → 2601.00] Speaking of notes, whilst we're on the topic of Obsidian and maintenance logs and all that kind of stuff,
[2601.00 → 2606.28] you found a new app that does note-taking called Memos.
[2607.06 → 2610.72] And it, you know, it's sort of aiming at that Apple Notes crowd.
[2611.08 → 2612.82] And this was sent in by an audience member.
[2612.88 → 2614.50] And I'm sorry, I forgot who at this point.
[2614.98 → 2618.42] But they had heard me kind of complain that, boy, I just wish I could have Apple Notes.
[2618.82 → 2619.96] This tries to get there.
[2619.96 → 2624.00] It bills itself as a privacy-first, lightweight note-taking service.
[2624.96 → 2627.26] And it's marked down.
[2627.96 → 2630.86] And it does look a little bit like something like Apple Notes.
[2630.86 → 2631.62] It's a web app.
[2631.86 → 2632.98] It is open source.
[2633.06 → 2634.06] It is very self-hosted.
[2634.20 → 2635.44] It's very simple to get going.
[2636.04 → 2640.06] And it works pretty well either on the phone or in your web browser.
[2640.80 → 2647.00] And it, I mean, it's probably great for somebody who just wants a simple feed of notes.
[2647.20 → 2652.34] And then you can do a quick search against them either based on date or title or hashtag.
[2652.34 → 2656.32] And if that sounds like you, it is really great for that.
[2656.54 → 2664.10] And I think where I may see this get some uses with the wife because she's a big Apple Notes user.
[2664.10 → 2667.94] And I'm beginning the very slow process over 2024.
[2667.94 → 2671.30] Therefore, I'm beginning to move her off of an iPhone.
[2671.88 → 2674.26] And I'm going to move her on to Graphene OS.
[2675.06 → 2677.34] And Apple Notes is my first target.
[2678.16 → 2680.80] And I think Memos is going to be perfect for that.
[2681.38 → 2690.94] The one area that I wish it did a little better is it doesn't really do great with pictures and getting text out of pictures.
[2690.94 → 2693.24] And that's an area where the Apple Notes just kills it.
[2693.32 → 2694.60] It does have a brilliant UI.
[2694.96 → 2696.08] It's really simple to understand.
[2696.18 → 2700.42] You can attach pictures and, like, you know, to-do checkboxes.
[2700.58 → 2703.08] And it has a nice sharing system, multi-user system.
[2703.08 → 2704.96] And you can mark notes private.
[2705.28 → 2707.46] Or you can mark them for anybody on the instance.
[2707.92 → 2710.84] Or you can make them public and link to them if you have that set up.
[2711.86 → 2714.00] And it is actually, you know, it's got an API.
[2714.22 → 2716.62] So you could probably integrate it with a lot of stuff if you knew how to do that.
[2717.26 → 2718.30] I like it a lot.
[2718.30 → 2721.76] I feel bad that I found, I sound like I'm negative on it.
[2721.84 → 2723.18] But it's just not quite it for me.
[2723.18 → 2724.56] It does look nice.
[2724.64 → 2728.92] Like, the user interface looks pretty polished in a way that Obsidian's isn't.
[2729.56 → 2733.96] It's almost like someone took Tiddly Wiki and made it pretty.
[2734.54 → 2734.72] Yeah.
[2735.40 → 2735.84] Yeah.
[2735.84 → 2739.28] And in a feed style, like a news feed style.
[2739.38 → 2739.66] Yeah.
[2740.26 → 2743.12] Which works for me for my first 20 or 30 notes.
[2743.12 → 2745.22] But I think would kind of get old after a while.
[2745.30 → 2748.62] And then I would be down into the hashtags and in the searching all the time.
[2749.36 → 2753.12] Maybe this would be good if you're into something like journaling or something like that.
[2753.22 → 2753.40] Definitely.
[2753.82 → 2756.34] And you just want that daily or even hour by hour.
[2756.46 → 2757.68] Like, I'm at the bus stop.
[2757.72 → 2759.58] I want to capture this random thought or something.
[2759.58 → 2763.92] Or like, I've noticed the way my wife uses notes is she's generally using three or four
[2763.92 → 2766.42] or five notes at a time for different things.
[2766.42 → 2767.98] But then they kind of age out.
[2768.36 → 2768.44] Yeah.
[2768.54 → 2770.84] And so this, I think, system will work for her.
[2770.92 → 2771.86] So I have it running.
[2771.86 → 2778.38] And with my new way I have containers set up, she just goes to memos in her web browser.
[2779.08 → 2781.14] And then it comes up as a quick little web app.
[2781.82 → 2782.92] Well, it's nice that it's open source.
[2783.14 → 2785.82] You can find a link to the GitHub repo in the show notes.
[2785.90 → 2787.26] It's written in React and Go.
[2787.98 → 2791.24] So, yeah, nothing terrible to say about it from that perspective.
[2791.72 → 2791.88] No.
[2792.14 → 2792.40] No problem.
[2793.06 → 2796.00] Well, let's get to some boost before we get out of here.
[2796.68 → 2798.04] ZZ Bra has boosted in.
[2798.14 → 2799.30] I think I'm getting that right.
[2799.30 → 2805.42] I'm feeling like I got that right with 20,000 SATs using Cast-O-Magic, which is a fantastic app.
[2805.90 → 2807.48] It's like something I miss on Android.
[2808.00 → 2808.66] Long-time listener.
[2808.78 → 2809.68] Appreciate all the content.
[2809.94 → 2816.62] Alex, for my Medea mini split unit, I've tried both, I think it's Mesa and Sensing.
[2817.20 → 2817.60] I don't know.
[2817.86 → 2818.32] Air Pro.
[2818.96 → 2822.04] I ended up keeping the Mesa as it has HomeKit support.
[2822.12 → 2822.86] That sounds nice.
[2823.24 → 2825.60] It ties right into Home Assistant with that HomeKit support.
[2825.94 → 2827.70] Provides physical local control.
[2828.14 → 2828.56] Nice.
[2828.56 → 2831.32] Shows the temperature physically on the screen as well.
[2831.92 → 2833.46] It's been rock solid for a year now.
[2833.90 → 2836.22] Did not require me to open up the mini split unit.
[2836.52 → 2837.28] Oh, that's nice.
[2838.04 → 2840.26] My new LG TV has HomeKit support.
[2840.94 → 2843.92] You can turn it off, but you can't turn it on.
[2844.20 → 2844.92] That doesn't make sense.
[2845.28 → 2846.04] How lame is that?
[2846.34 → 2846.90] It's lame.
[2847.22 → 2848.70] Well, because it's off, I guess.
[2849.20 → 2851.32] Maybe it burns a fuse on the circuit board.
[2851.38 → 2851.70] Do you remember?
[2851.90 → 2852.78] Like certain things.
[2853.28 → 2855.18] Voids the warranty if you disable HomeKit.
[2855.18 → 2860.18] Also, my LG TV came with a big Matter logo on it, but I installed the Matter integration on Home Assistant.
[2860.36 → 2861.14] Nothing shows up.
[2861.22 → 2862.32] So I don't know.
[2863.00 → 2864.84] It's the year of Matter again.
[2865.58 → 2865.72] Yeah.
[2865.72 → 2867.02] I just watched their live stream today.
[2867.38 → 2871.96] He also wants to recommend, and we had some other folks boost in with this, Obsidian Live Sync.
[2872.54 → 2873.86] A bevy of features, he writes.
[2874.38 → 2875.78] Instant sync between devices.
[2875.94 → 2879.06] It gives the ability to merge conflicts before overriding in case you have issues.
[2879.20 → 2880.48] Oh, I hate that kind of stuff.
[2881.06 → 2882.70] And it works between all my devices.
[2882.80 → 2884.66] iOS, Android, Windows, and even Mac.
[2884.66 → 2888.96] I have a separate Couch DB for the wife and myself, and I have multiple vaults on each.
[2889.18 → 2889.82] Ah, I see.
[2889.88 → 2891.10] So it's got a Couch DB back in.
[2891.30 → 2892.76] Been using it for almost six months now.
[2892.98 → 2893.42] No issue.
[2893.80 → 2894.94] Strong recommend.
[2895.18 → 2895.42] Okay.
[2895.52 → 2896.18] Very good to know.
[2896.66 → 2900.98] Yeah, we've had lots of recommendations for this Couch DB-based live sync situation.
[2901.28 → 2907.14] So whenever my subscription is up for Obsidian, which I think is in the summer, I will definitely take a look at this.
[2907.48 → 2907.80] Interesting.
[2907.90 → 2908.78] We'll put a link in the show notes.
[2909.46 → 2911.90] I appreciate the signal on this one.
[2911.90 → 2912.38] Yeah.
[2912.38 → 2920.22] You know, when you see, like, that's finally what pushed me over to try Audio Bookshelf, was that people just kept coming in and saying, you got to try it.
[2921.14 → 2922.50] And they were right.
[2922.96 → 2923.78] They were right.
[2923.86 → 2926.14] So Obsidian Live Sync, you're probably right there, too.
[2926.58 → 2933.88] What I really, really, really, really appreciate about Obsidian Sync so far is that I've never once had to resolve a conflict.
[2933.88 → 2943.54] And it's funny because I'm constantly resolving conflicts with Nextcloud Sync for my Obsidian Library folder.
[2943.90 → 2949.00] Because on a couple of machines, I guess I put it in my Nextcloud folder thinking that was smart.
[2949.46 → 2955.58] And now I'm just inundated every day with Nextcloud Sync errors because of that.
[2955.58 → 2958.86] But yet Obsidian Sync continues on.
[2959.76 → 2961.78] Bola Par comes in with 5,000 SATs.
[2962.66 → 2963.88] This is about your mini split, too.
[2963.92 → 2965.12] I had a Mitsubishi mini split.
[2965.18 → 2969.40] It was in my office, and it got connected nicely to Home Assistant.
[2969.66 → 2973.46] Oh, I used an ESP01 with ESP Home and it works well.
[2973.62 → 2977.30] Links to the project, a little ESP Mitsubishi heat pump project.
[2978.32 → 2979.20] That's pretty nice.
[2979.20 → 2986.86] Yeah, I mentioned in the last episode, I ended up using Broad link RM4 infrared to control it.
[2986.94 → 2988.18] And honestly, that's been working fine.
[2988.30 → 2988.46] Is it working?
[2989.12 → 2989.36] Yeah.
[2989.48 → 2995.10] The main thing I wanted to do is just turn it off at midnight and turn it on at like 8 a.m. or something.
[2995.40 → 2997.78] And does that RF controller talk to Home Assistant?
[2998.10 → 2999.00] Yeah, it's infrared.
[2999.48 → 3001.88] But yeah, the Broad link talks to Home Assistant.
[3002.06 → 3005.68] I think it's a cloud integration, so it's not perfect, but it does the job.
[3005.68 → 3011.22] And I didn't have to open up anything, particularly with that CN105 connector that I talked about a little bit.
[3011.34 → 3016.78] I'm just nervous to plug into a new $5,000, $6,000 air conditioning unit.
[3017.06 → 3020.16] And yeah, I want to.
[3020.62 → 3020.92] That's good.
[3021.02 → 3022.04] Sounds like you've got a working solution.
[3023.42 → 3024.00] That's nice.
[3024.10 → 3026.34] MountBudDude comes in with 5,000 SATs.
[3026.60 → 3031.58] This is going to sound stupid, but I finally figured out Docker Compose, and now I'm spinning up all the stuff on my home server.
[3031.68 → 3032.26] Hey, right on.
[3032.48 → 3032.92] Congratulations.
[3032.92 → 3036.58] Always had trouble with the environment variables and now those have been worked.
[3037.02 → 3039.96] I'm setting them up now, and I'm so happy to be self-hosting stuff.
[3040.48 → 3042.98] So now I have to figure out remote backups with duplicating.
[3043.26 → 3044.14] Well, good job.
[3045.00 → 3057.26] I remember, you know, when I got Docker Compose working, I think the big breakthrough for me was when I realized I could stack multiple, you know, different services and apps in one Docker Compose.
[3057.26 → 3063.38] And have liked my media centre, my, you know, my editing, you know, and just have them all updated.
[3063.60 → 3064.62] So have fun with it.
[3064.84 → 3064.98] Yeah.
[3065.64 → 3066.86] Do make sure you pack it up.
[3067.46 → 3069.32] Grumpy Linux admin comes in with some space balls.
[3069.42 → 3070.68] One, two, three, four, five SATs.
[3070.82 → 3076.02] In episode 113, you mentioned that you guys are running a reverse proxy in your home labs.
[3076.02 → 3081.26] What's the purpose of running a reverse proxy, and how would you use it in a home lab?
[3081.70 → 3082.32] Love the show.
[3082.56 → 3083.76] I always look forward to new episodes.
[3084.38 → 3085.14] Great question.
[3085.46 → 3090.48] I have written about this topic quite a few times over the years, originally on the Linux server blog.
[3090.60 → 3094.68] Let me see if I can find that blog post and put a link to it in the show notes.
[3094.68 → 3099.06] But the basic gist is remembering IP addresses and port numbers stinks.
[3099.80 → 3105.42] Not having TLS certificates or HTTPS, SSL certificates, whatever you want to call them, stinks.
[3106.06 → 3113.28] And the idea behind a reverse proxy is you have one service exposed to the internet listening for web requests.
[3113.28 → 3124.66] And when you type a URL into your web browser, let's say homeassistant.alexishouse.com, that reverse proxy is listing for that web request.
[3125.14 → 3133.48] Now in that request is a bunch of headers and a bunch of information identifying your client, your source IP address, the destination, all that kind of stuff.
[3133.48 → 3144.70] And the reverse proxy has the knowledge and the permissions to actually proxy that traffic in your internal network from wherever your reverse proxy is hosted.
[3144.86 → 3147.36] In the old days, this was hanging out on the public internet.
[3147.72 → 3152.78] Although with these days, with Tail scale and things like that, I just have everything behind the firewall.
[3153.46 → 3157.62] But reverse proxies will work whether they're on the internet or in a private network or anything like that.
[3157.62 → 3163.34] So the general idea is you type in a URL rather than an IP address and port number.
[3164.00 → 3165.42] And it's really just become common.
[3166.24 → 3175.22] I mean, our infrastructure, just about every infrastructure you're going to go to, you're going to have one machine that's sort of on the edge that's going to receive the connections.
[3175.22 → 3177.94] It'll be the termination point for the TLS certification.
[3178.34 → 3182.78] And then it'll send the traffic to the correct box internally and then bring it back forward.
[3183.54 → 3187.16] And you can see on a system with containers why this would be useful.
[3187.50 → 3190.94] Because you could have Nextcloud on there, and you could have VS Code Studio on there.
[3190.94 → 3194.28] And you could have some of the apps like Audio bookshelf we talked about.
[3194.36 → 3196.50] They're all on their own ports.
[3197.12 → 3203.92] But you could all have them just be at your domain without the port number with something like Nginx or Traffic.
[3204.10 → 3211.76] And they're doing a reverse proxy for you that knows that when you go to that domain name, I'm actually sending it to this application, this service, this machine, whatever it is.
[3211.76 → 3212.68] And it's at this port number.
[3212.84 → 3214.72] And it just handles all of that for the user.
[3214.72 → 3217.38] So that's another reason to do it even for yourself.
[3217.80 → 3230.84] And then another reason that reverse proxies became really popular, we talked a little bit about TLS a few minutes ago, is Let's Encrypt came along probably when 2017, 18-ish, I think.
[3231.26 → 3232.98] You used to have to pay for SSL certificates.
[3233.08 → 3234.22] Remember that back in the day?
[3234.40 → 3235.40] You used to have to actually pay.
[3235.48 → 3238.52] It was hundreds of dollars for a TLS certificate for a domain.
[3238.68 → 3242.70] And depending on the web server, treacherous to install sometimes.
[3242.70 → 3243.30] Yeah.
[3243.68 → 3247.12] And the purpose of a TLS certificate is to verify ownership.
[3247.46 → 3255.58] So when you make a web request, you want to know that the server answering that request is the server that you actually requested the content from.
[3256.28 → 3264.42] So if you click on the little padlock or these days the little menu item in your browser, you can actually go in and view the certificate.
[3264.42 → 3277.44] But the reason that reverse proxies in self-hosting are really popular is because a lot of them have cert bot built in or some kind of Let's Encrypt Acme-based kind of certificate automation built in.
[3277.44 → 3291.50] So you can type in to your reverse proxy configuration, homeassistant.alexishouse.com, verify ownership through whoever your registrar is through some kind of DNS validation or HTTP validation.
[3292.16 → 3305.54] I appreciate some of that might be a little advanced, but I have a tutorial, which again I'll link to in the show notes on perfectmediaserver.com, walking you through the entire process of TLS validation with traffic, Namecheap and Cloudflare.
[3305.54 → 3319.68] Yeah, and the upshot is you end up with a TLS certificate verifying that Alex's home assistant, or was it home assistant at alexishouse.com, is actually my version of home assistant and not Chris's, for example.
[3320.42 → 3324.12] Or it's not got some kind of man-in-the-middle injection that's going on.
[3324.18 → 3327.58] Somebody hasn't intercepted an iframe or done some weird injection somewhere.
[3327.58 → 3337.02] Like, you can verify the content that's actually reaching your device and your eyeballs is cryptographically, a bit for bit, what was sent from the origin server.
[3337.52 → 3349.24] I think Home Lab is more and more going to probably have to learn some sort of reverse proxy solution because, just in my experience, more and more mobile apps just fundamentally don't work if you don't have SSL or TLS.
[3349.46 → 3351.22] Like, it just, they won't connect.
[3351.36 → 3352.36] They'll just refuse to connect.
[3352.36 → 3354.48] And that, I think, will become more and more common.
[3354.68 → 3359.42] And then people will have to have more and more applications they're hosting on their own homeland that need TLS.
[3359.82 → 3361.82] And that's where reverse proxy will be really useful.
[3363.10 → 3366.64] Noobs comes in with a total of 2,322 SATs.
[3366.88 → 3368.48] And I know.
[3368.76 → 3372.48] He says, the rage when I fire up Jellyfin for the kids, and it just throws up an air.
[3372.98 → 3376.44] It's hard to put into words, so I'll turn it into SATs.
[3376.78 → 3378.24] Glad no, it's not just me.
[3378.24 → 3379.82] I like this.
[3380.20 → 3385.90] When your home lab fails you, turn that rage into support for the self-hosted podcast.
[3386.82 → 3388.88] Gene Bean comes in with 2048 SATs.
[3388.98 → 3394.56] Regarding Zigbee plugs that make overall mesh better, that's the key, I've been impressed with the Zen geld.
[3395.26 → 3398.04] That's S-E-N-G-L-E-D.
[3398.54 → 3400.56] And he says, I've replaced others with them.
[3400.82 → 3403.16] They make the mesh better, but they also do energy monitoring.
[3403.66 → 3404.58] Yeah, I'll plus one that.
[3404.58 → 3408.88] They pop right up on Home Assistant three out of four times.
[3409.34 → 3415.64] I will say, having deployed like a dozen of them, the fourth sometimes just never connects.
[3416.02 → 3421.56] So like, I'm not kidding you, one out of every four I kind of just end up tossing.
[3422.20 → 3426.80] However, I still like them a lot, and they will improve your Zigbee reliability because they are repeaters.
[3427.04 → 3428.64] And the energy monitoring is great.
[3428.64 → 3435.56] Okay, rounding it out, I'm Root, a row of ducks, and this is really brilliant.
[3436.04 → 3438.22] Take this advice, take this sage wisdom.
[3439.22 → 3443.34] Dashboards are like cable management, all nice and tidy for like three days.
[3443.82 → 3445.82] Then you change something, and it's a mess again.
[3446.28 → 3446.96] Yes, sir.
[3447.30 → 3447.56] Yep.
[3448.28 → 3448.70] That's it.
[3448.70 → 3452.96] I saw that one when it came in, and it made me laugh.
[3453.48 → 3459.84] Do you ever see these productivity gurus on YouTube that make a living out of making videos telling other people how to be productive?
[3460.16 → 3460.46] Oh, yeah.
[3461.02 → 3467.74] And they always have these perfectly cable managed desks, and they're talking about aesthetics, and they're talking about this and that.
[3468.26 → 3472.84] I'm sure it's a lovely place to be in a life that nothing ever changes.
[3472.84 → 3476.68] But how are they getting any actual work done?
[3477.22 → 3478.66] That is their work, I think.
[3478.92 → 3479.18] Yeah.
[3479.18 → 3479.70] I think that's it.
[3479.98 → 3480.60] I think that's it.
[3480.68 → 3481.32] That's the hack.
[3481.68 → 3485.78] Because just before this show, I mean, we haven't sat down and recorded for three weeks.
[3485.98 → 3496.60] I don't change much on this desk, but for whatever reason, I had to get underneath and unplug my audio interface because it had dropped off my Thunderbolt dock for whatever reason.
[3497.06 → 3497.20] Yeah.
[3497.30 → 3499.80] And I had to, you know, unpick the cable.
[3500.02 → 3500.76] Oh, is it this one?
[3500.80 → 3501.28] Is it that one?
[3501.28 → 3504.28] And like, do these guys not have these issues?
[3504.74 → 3508.82] Like, no, I think they don't have, they don't live real lives.
[3508.92 → 3509.42] I tell you what.
[3509.80 → 3513.36] What perplexes me is I have an automation that fires up one of my computers in here.
[3514.04 → 3516.18] Same exact process to boot it every single time.
[3516.26 → 3516.82] Nothing changes.
[3516.94 → 3518.44] No state changes on the computer.
[3519.30 → 3520.94] Sometimes you launch your launches.
[3521.30 → 3523.44] Sometimes it crashes at boot.
[3523.90 → 3524.58] Nothing changes.
[3524.68 → 3525.62] Nothing changes in the state.
[3525.70 → 3526.92] Nothing changes in the process.
[3526.92 → 3531.24] And our last boost comes from Southern Fried Sassafras.
[3531.52 → 3532.42] 2,000 sets.
[3532.60 → 3537.84] This is a thanks for keeping my to-do and research list for my home lab and setup tech ever-growing.
[3538.46 → 3539.46] We do have a few more boosts.
[3539.50 → 3542.56] I had to kind of cut it down for time because we're running long, but I put them in the boost barn.
[3542.82 → 3543.92] It is linked in the show notes.
[3544.00 → 3544.74] You can go find that.
[3545.08 → 3547.08] There are some good ones in there, and I read all of them.
[3547.08 → 3551.02] We had 12 boosters total, 63,136 sets.
[3551.18 → 3554.70] I think that's maybe one of our lowest ever, but it has been the holidays.
[3555.56 → 3558.10] But with the ad winter continuing, we'd love your support.
[3558.22 → 3559.60] Go get a new podcast app.
[3559.76 → 3562.78] Fountain1.0 is out, and it is fantastic.
[3563.80 → 3564.76] It's fabulous.
[3565.82 → 3571.76] Pod verse continues to build one of the best GPL podcast apps out there as well, and Automatic is a real choice on iOS.
[3572.28 → 3573.06] Three great apps.
[3573.54 → 3575.98] Newpodcastapps.com to pick and then boost in.
[3575.98 → 3582.06] I will say as well, I know that Chris did a bunch of stuff promoting the network and stuff already in the show,
[3582.14 → 3587.46] but I will say if you work for a company or know of someone that works for a company that is in this space
[3587.46 → 3591.48] and has been thinking, oh, it'd be cool if we could advertise on a network like JB,
[3592.38 → 3595.86] we're not swimming in sponsorships these days.
[3597.08 → 3600.78] Like Chris says, it's a bit of a winter when it comes to that kind of thing.
[3600.78 → 3607.36] And it's tricky for us too because we say no, and the sponsors a lot,
[3607.42 → 3610.30] and the sponsors that are available tend to be at lower and lower quality right now.
[3610.36 → 3612.96] So it's like the ones that are high quality we'd love to work with.
[3613.24 → 3617.06] And folks that are sourced from our community tend to be of some of the highest quality.
[3617.28 → 3618.20] So, yeah, do reach out.
[3618.54 → 3619.14] Get a good deal.
[3619.68 → 3620.50] Yeah, reach out.
[3620.86 → 3621.22] Reach out.
[3621.22 → 3624.40] Speaking of community support and stuff like that,
[3624.50 → 3629.82] we are going to be having a very, very busy first half of the year conference-wise, aren't we?
[3630.26 → 3630.42] Yeah.
[3630.68 → 3637.14] We have Nixon and Scale coming up March 14th through like the whatever.
[3637.84 → 3640.80] Then shortly after that, it is Texas Linux Fest.
[3641.00 → 3642.18] You mean Barbecue Fest.
[3642.46 → 3642.82] Yes.
[3643.36 → 3643.72] Yes.
[3643.80 → 3648.28] And then we'll round it out with Linux Fest at the end of April.
[3648.50 → 3650.12] It's boom, boom, boom.
[3650.12 → 3650.84] Boom, boom, boom.
[3650.84 → 3658.84] I legitimately am concerned about how I'm going to get my butt from Texas back up to Seattle area in time for Linux Fest Northwest.
[3659.64 → 3664.82] Because when I do the shows, it takes me like six, seven days to drive from Texas when I stop to do the shows.
[3665.46 → 3666.06] Well, it's going to be tricky.
[3666.06 → 3674.92] You know if only they had invented these things that you could sit in that do hundreds of miles per hour in the sky.
[3674.92 → 3677.16] If man was meant to fly, he'd have wings, Alex.
[3677.16 → 3677.24] Thanks.
[3679.08 → 3681.56] Chris, I've got three words for you.
[3682.00 → 3683.10] Make it so.
[3685.34 → 3685.94] All right.
[3685.98 → 3687.30] You can find me on Weapon X.
[3687.44 → 3688.84] I'm at Chris LAS.
[3689.12 → 3692.84] The podcast is over there as well at Self Hosted Show.
[3693.20 → 3695.76] You can find me at alex.ktz.me.
[3695.84 → 3700.98] I've got a sort of like little link tree situation going on over there for all the different places you can find me.
[3701.56 → 3703.32] And as usual, thanks for listening, everybody.
[3703.50 → 3706.38] That was self-hosted. Show slash 114.
[3706.38 → 3707.28] And I'll see you later.
[3707.42 → 3707.76] All right.
[3707.76 → 3708.40] Beautiful.
[3708.40 → 3708.66] Weapon X 4.
[3708.66 → 3709.52] Nice 힘 for you.
[3710.78 → 3710.92] Folks are nice for you.
[3710.92 → 3711.20] Blackjack, you too.
[3711.20 → 3714.20] The video of Google in baseball a hearts will likely 15 to 16.
