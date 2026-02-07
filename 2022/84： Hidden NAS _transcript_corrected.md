[0.00 → 4.64] Well, unfortunately, Alex is out sick this week, but the show must go on.
[4.70 → 6.20] We send him our best wishes.
[6.80 → 11.00] But our buddy Joe Remington's here from Late Night Linux and Two and a Half Admins.
[11.38 → 13.38] Joe, welcome to Self-Hosted.
[13.78 → 16.58] Hey, Chris. Good to be here. I've never been on this show before.
[16.96 → 19.62] I was just thinking that when I was introducing you.
[19.68 → 20.88] I was thinking this must be his first time.
[20.98 → 25.88] It's good timing because I know you're kind of thinking about building a new NAS.
[26.16 → 28.00] So I think that's one of the things we'll get into.
[28.00 → 32.14] It is, but we should address a weird situation that's come up.
[32.38 → 34.90] Alex helped me out by coming on Two and a Half Admins.
[35.00 → 36.98] We recorded that weeks ago now.
[37.30 → 41.80] So as you're listening to this, that came out yesterday with Alex, even though he's sick now.
[41.94 → 44.48] It's crazy time math. Don't worry about it.
[44.54 → 48.28] But that explains why he's on Two and a Half Admins, but not this show.
[48.48 → 50.76] And I'm kind of paying him back by coming here.
[51.20 → 52.52] It worked out, you know.
[52.72 → 56.74] And when you record ahead, it means you have time to get sick, apparently.
[56.74 → 57.66] I should think about that.
[58.00 → 58.30] Hmm.
[58.66 → 60.76] So I've been rebuilding my home setup.
[61.06 → 61.88] It's been crazy.
[61.88 → 66.42] The short version is, is like weeks ago during my road trip, my Raspberry Pi 4 died.
[67.00 → 67.96] Totally unplanned.
[68.06 → 71.48] I had backups, but didn't have any replacement hardware.
[71.60 → 75.00] I tried doing like a swap where I swapped everything over to my backup Pi.
[75.22 → 77.28] It still didn't boot.
[77.28 → 83.28] And so I had to make the trip home in the last couple of weeks while I was waiting for hardware without any of my gear.
[83.62 → 84.48] And it was horrible.
[84.86 → 85.96] It was absolutely horrible.
[85.96 → 89.54] But I've been steadily rebuilding, and it's at a pretty good spot now.
[89.66 → 92.98] So I feel like I'm on the end of a journey, and you're just at the beginning of a journey.
[92.98 → 95.98] I know you need a new NAS box, but it sounds like you got some hardware.
[96.20 → 98.02] So tell us what your quandary is.
[98.60 → 98.72] Right.
[98.88 → 106.24] So I have currently got a Cameron J1800 box, passively cooled, totally silent, apart from the disks that's been in it.
[106.24 → 112.00] And that has been doing the job for me for a couple of years at this point.
[112.38 → 115.36] It was actually kindly donated to me by a late night Linux listener.
[115.88 → 117.60] So that was really appreciated.
[118.02 → 123.24] It's got only four gigabytes of RAM in it, just a few disks, ZFS with a bit of replication.
[124.06 → 127.18] And it's working totally fine, except when I have to reboot it.
[127.56 → 128.26] So get this.
[128.48 → 133.72] I have no idea why, but the only way I can reboot that box is by hooking a monitor up,
[133.72 → 136.04] turning the monitor on, rebooting it.
[136.38 → 138.16] I can reboot it via SSH, no problem.
[138.30 → 141.06] But the monitor has to be there, plugged in and on.
[141.60 → 146.14] I have to wait for the AMI BIOS thing to come up, and then it boots and no problem.
[146.68 → 153.68] Oh man, there is like a dummy video adapter you can get that make it look like a monitor signal is there.
[154.12 → 157.74] And that will sometimes let them boot without actually having a monitor connected.
[158.02 → 160.50] But that must not be the only reason you want to replace it.
[160.52 → 162.14] I mean, it's probably getting a little long in the tooth.
[162.14 → 167.84] Well, yeah, and it makes me wonder, well, should I replace it with something a bit more powerful?
[168.04 → 170.62] It doesn't use much power in terms of electricity.
[171.38 → 180.36] We're talking about 30 something watts, I think, idle and only a couple more under load because it's so underpowered that it's basically always under load, I think.
[180.36 → 189.30] I've got an i5 9600K box, which is kind of my backup workstation box because my main workstation is the i9 9900K.
[189.72 → 191.34] And so it's almost a hot spare for me.
[191.40 → 197.14] I can just take the SSD out, stick it in the i5 box and just get going again if anything goes wrong.
[197.14 → 203.54] And it also means that I've got a relatively powerful box to do just testing of distros and software.
[203.92 → 207.30] And, you know, I can just do anything I want on that and just not worry about it.
[208.00 → 208.74] That is nice.
[208.74 → 214.40] I miss having a perfect test system because I've ended up putting all of my machines into some kind of use now.
[214.50 → 218.06] And I just don't have a machine to just throw a random distro on and play around.
[218.46 → 228.64] I think my question would be, because you've been living with this Cameron box for so long, do you plan to run applications, like server-side applications on that machine?
[228.90 → 230.52] Do you want it to do more than it's currently doing?
[230.52 → 232.56] Well, maybe, maybe.
[232.92 → 233.68] That's what I'm thinking.
[233.84 → 236.64] At the moment, it's not really that feasible to do it.
[236.72 → 241.44] But if I had more power, then maybe I could start thinking about stuff that I want to do with it.
[241.74 → 244.38] And so this ties into the next situation, right?
[244.96 → 247.44] So I'm going to be moving, and I'm going to have more space.
[247.54 → 253.26] So I'm going to actually have a TV finally, instead of just a 27-inch monitor, which is effectively my TV at the moment.
[253.58 → 254.46] That's just 1080p.
[254.46 → 261.18] So I bought a dirt-cheap 4K TV that's 58 inches, £400 from Costco in the UK.
[261.96 → 264.04] I don't know how they make it so cheap.
[264.08 → 267.96] Well, I do know how they make it so cheap, by selling your data, because it's a smart TV.
[268.22 → 271.00] But this thing is not getting connected to my network.
[271.34 → 272.98] Not even a VLAN, no way.
[273.68 → 274.04] There you go.
[274.24 → 276.62] I'm thinking I can kind of kill two birds with one stone.
[276.62 → 286.04] There's no reason why I can't install a GUI XFCE, let's say, on top of my server and have an as-come TV box.
[286.92 → 294.02] But I've been testing the i5 box, and it's kind of okay for most stuff at 4K.
[294.34 → 300.38] But trying to play actual 4K content, it kind of skips a few ways.
[300.44 → 301.88] It's just a bit laggy here and there.
[301.94 → 304.60] And I think it's too annoying to play 4K content.
[304.60 → 308.52] And so do I double them up and use that one?
[308.74 → 313.02] Or do I just have a separate NAS and a separate TV box?
[313.12 → 316.08] I know you have got way more experience with TV stuff.
[316.38 → 318.06] Are you still using the shields for TV?
[318.78 → 319.60] I do have one left.
[319.90 → 324.20] Yeah, they're getting a little long in the tooth because I have a second-gen shield.
[324.70 → 328.66] And to NVIDIA's credit, they continue to update that thing.
[329.20 → 329.24] Really?
[329.72 → 331.96] I want to say it's been like four or five years, maybe.
[332.28 → 332.72] Wow.
[332.88 → 333.10] Yeah.
[333.10 → 339.08] The only issue is that it's now running multiple versions of Android since it shipped.
[339.72 → 341.14] And so it's slow now.
[341.26 → 341.56] Yeah.
[341.80 → 345.94] It used to be my fastest set-top box, and now it feels kind of slow.
[346.46 → 350.38] But it is really overall been a solid device.
[350.52 → 355.46] The latest updates added ads to the Android UI, which I'm not a fan of.
[355.46 → 359.18] So it's sort of like you're saying, you disable the smart TV tracking.
[360.12 → 363.18] But is the situation much better on Android?
[363.18 → 363.70] Yeah.
[363.80 → 367.94] Whereas a good old GNU slash Linux box, I know I'm in complete control of it.
[368.14 → 368.46] Yeah.
[368.60 → 370.66] I mean, Cody is a good solution too.
[370.96 → 373.58] You know, you could do something like that, and you don't have to worry about it.
[373.64 → 376.54] That where it really is nice is if you have multiple televisions.
[376.94 → 380.96] Because then all of a sudden, you know, you're into some kind of show with your significant other.
[380.96 → 384.48] You're into episode seven in season three or whatever.
[384.48 → 385.90] And you watch in the one room.
[386.10 → 388.74] And then you want to pick up some other night in another room.
[388.74 → 390.54] And you want to be right where you left off.
[390.82 → 391.82] You want the metadata.
[391.96 → 393.58] You want it all organized by season.
[393.70 → 397.86] That's where it just becomes really nice to just do a jelly fit or a Plex.
[397.96 → 399.54] And then, you know, you just throw it all on the server.
[399.74 → 402.52] You load the app on the Nvidia Shield or whatever.
[403.26 → 404.98] And it really works pretty well.
[404.98 → 408.72] So that's the direction I chose to go in this latest build.
[408.80 → 410.78] I actually ended up with Plex again.
[411.46 → 414.82] Just because it's just a little bit smoother.
[415.38 → 416.50] The intro skipping is better.
[417.06 → 419.16] The hardware decoding works better for me.
[419.34 → 420.90] It's simpler to get the hardware decoding to work.
[420.96 → 422.56] I just could not get it working with Jellyfin.
[423.44 → 427.74] And if you have Intel Quick Sync, it makes a big difference on the performance.
[427.86 → 429.26] It takes the load off of the CPU.
[429.74 → 430.14] I don't know.
[430.18 → 431.90] I didn't check to see if your CPU has that.
[431.90 → 434.90] I think it does because it's a ninth gen i5.
[435.80 → 437.10] Yeah, there's probably a good chance it does then.
[437.34 → 437.46] Yeah.
[437.88 → 439.60] Can I get that to work locally, though?
[440.62 → 440.82] Yeah.
[441.00 → 441.38] Oh, sure.
[441.62 → 441.94] Yeah, yeah.
[442.34 → 442.54] Yeah.
[442.58 → 447.12] So it would run either like just with an installed application or through a container.
[447.32 → 448.74] And then it would do the Quick Sync.
[449.00 → 452.22] It would re-encode the video and send it to wherever you're watching it.
[452.42 → 452.62] Right.
[452.66 → 457.16] Because I don't have multiple TVs and multiple rooms where I want a TV.
[458.12 → 460.96] I just kind of want to do it all in one box if possible.
[461.16 → 463.18] You could have, you know, one setup.
[463.44 → 464.50] I definitely have seen this.
[464.50 → 465.94] One box, it's a NAS.
[466.12 → 467.40] It's also the Jodi box.
[467.54 → 469.10] It's connected directly to the television.
[469.48 → 470.66] And you just have a keyboard.
[471.08 → 474.46] And, you know, one of those like RF keyboards that also has a built-in trackpad.
[474.96 → 475.58] I've seen it.
[475.68 → 476.16] It works.
[476.50 → 479.26] And there's plenty of machines there because there's no...
[479.26 → 483.76] Like if you have a whole i5 sitting there doing your NAS, you might as well have it also doing
[483.76 → 484.28] other things.
[484.36 → 486.66] It just seems like, yeah, you totally could.
[486.74 → 488.76] And the only problem is, do you want a PC next to your television?
[488.76 → 492.90] Well, it's going to go on a sideboard thing, the TV.
[492.90 → 497.78] And there's room in this IKEA sideboard that we've bought to put the PC.
[498.42 → 503.38] And what I was thinking is I can drill out the back of it and put a fan there and one in the
[503.38 → 507.44] bottom of it, one in the back of it and get enough airflow to keep it cool.
[507.44 → 509.54] And it's otherwise just closed into a cupboard.
[509.90 → 510.84] So you won't even see it.
[511.54 → 513.72] Yeah, that now you're talking.
[514.00 → 514.92] Now I'm on board.
[515.02 → 515.86] I like that idea.
[516.22 → 520.06] If it was me, I'd throw a little Droid H3 in there because I love that Droid.
[520.44 → 522.28] I think that thing's the ultimate home PC.
[522.64 → 523.94] And it's got HDMI out.
[524.20 → 526.38] It's got a pretty good little processor on there.
[526.96 → 527.72] Make a good NAS.
[528.16 → 532.04] Yeah, but I've got this box already that is kind of a luxury because I've got a ton of
[532.04 → 532.88] laptops as well.
[532.96 → 536.38] I've got an Intraware Apollo, which is kind of my secondary laptop.
[536.38 → 538.06] You could use that as a test machine.
[538.46 → 539.30] Well, yeah, that's what I'm thinking.
[539.44 → 539.52] Yeah.
[539.98 → 541.24] Yeah, then I would do it.
[541.40 → 548.22] You know, listener Jeff, who let us very graciously stay at his place in Sacramento, he has that
[548.22 → 548.54] set up.
[549.00 → 553.92] He's using Plasma Desktop if he needs to drop to the desktop.
[554.62 → 556.86] You could fire up Cody directly on it.
[557.08 → 563.32] It's running Samba file services and NFS and running a couple of containers for him and works
[563.32 → 563.60] great.
[563.60 → 564.42] And it's got a disk.
[564.42 → 566.52] You've got a couple of disks in there to act as the NAS.
[567.14 → 568.78] So it's one PC doing all those things.
[568.92 → 572.70] And I think that's pretty easy to justify a power draw for in utility.
[573.14 → 574.38] Yeah, that's exactly what I'm thinking.
[574.64 → 576.84] The only thing is smooth 4K playback.
[577.38 → 583.26] So if anyone out there has got a suggestion for software I can run on top of Ubuntu, the
[583.26 → 584.62] LTS, then let me know.
[584.74 → 588.16] Either email the show or you can just tweet at me at Joe Islington.
[588.16 → 592.18] Linode.com slash SSH.
[592.26 → 595.50] That's where you go to get $100 in 60-day credit on a new account.
[595.64 → 600.12] And it's a great way to support the show while you're checking out some fast, reliable cloud
[600.12 → 600.50] hosting.
[600.94 → 602.14] Linde's the best and the best.
[602.52 → 605.46] That's why we pick them for everything we've deployed in like the last three years.
[605.72 → 606.78] All of our new projects.
[607.40 → 609.18] Backend infrastructure we use for our tooling.
[609.50 → 610.96] The stuff that's facing towards the audience.
[611.50 → 611.84] It's Linde.
[611.84 → 613.66] They got the best support in the business.
[613.76 → 614.26] Real humans.
[614.54 → 614.92] All day.
[615.28 → 616.70] Every single day.
[616.98 → 619.38] So you'll get the help you need if you ever get stuck.
[619.76 → 623.30] They've built up some great tooling and a great support department because they've been
[623.30 → 624.74] doing this for nearly 19 years.
[625.02 → 627.14] And they've had to just survive on the merits of the product.
[627.28 → 628.36] Nobody has a match.
[628.66 → 629.06] Nobody.
[629.58 → 634.00] And they're 30 to 50% cheaper than the hyperscalers out there that you really don't want.
[634.30 → 639.02] That don't let you have the full control and customizability and access to the system
[639.02 → 640.16] that you really want.
[640.16 → 642.34] And Linde is going to give you that.
[642.58 → 643.62] They got a great dashboard.
[643.90 → 644.78] A slick API.
[644.98 → 649.08] And lots of ways like Ansible and Terraform and Kubernetes to interact with the overall
[649.08 → 649.50] system.
[649.96 → 653.24] And on top of that, they got 11 data centres you can choose from today.
[653.56 → 655.32] A dozen more coming online next year.
[655.48 → 659.38] And features like object storage, cloud firewall, backups, Kubernetes support.
[659.94 → 660.92] You know, all that stuff.
[661.92 → 662.68] So I don't know.
[663.06 → 666.58] You can either like start from the very first principles and just do a bare box and build
[666.58 → 667.02] up from there.
[667.26 → 669.02] You could deploy one of their one clicks.
[669.02 → 670.88] Or you could use some infrastructure management tools.
[671.08 → 672.92] Maybe it's a great chance to learn some of that stuff.
[673.04 → 673.50] I mean, I don't know.
[674.02 → 674.80] I don't know you.
[675.36 → 677.26] But I have a suspicion that might be true.
[677.88 → 678.76] So go build something.
[679.24 → 680.10] Go learn something.
[680.44 → 685.82] Try for yourself and support the show and get that $100 by going to linode.com slash SSH.
[685.82 → 688.94] That's linode.com slash SSH.
[690.84 → 696.64] Well, Joe, I've been re-gearing a lot of sensors and small little edge devices for my home network.
[697.46 → 699.06] Had to throw some of the old ones out.
[699.46 → 700.46] Wanted to replace a few.
[700.88 → 704.36] And I decided this time around, I'm going to give Zigbee a try.
[704.46 → 707.94] Because Zigbee is an open source, wireless, and communication standard.
[708.60 → 709.96] It's pretty popular, actually.
[710.24 → 712.66] And it's going to be part of the new Matter standard as well.
[712.66 → 714.56] So I thought, all right, let's get on the Zigbee train.
[715.78 → 717.22] And I deployed sensors.
[717.50 → 719.52] You know, I probably spent a little more than I should.
[720.04 → 721.18] I do this sometimes.
[721.66 → 723.06] And I got everything all set up.
[723.14 → 724.50] Got it all connected into Home Assistant.
[725.36 → 729.22] And now I've discovered about once every couple of days,
[729.90 → 732.28] several of the devices just drop off my Zigbee network.
[732.54 → 733.18] They just disappear.
[733.82 → 734.16] Right.
[734.30 → 735.12] Any idea why?
[735.84 → 736.76] I have a couple of theories.
[736.94 → 739.44] I think in part, a couple of them are pretty low power devices.
[740.00 → 744.74] And what I've learned is Zigbee uses 2.4 gigahertz.
[745.66 → 748.00] And, you know, there's a lot of stuff in the thing.
[748.68 → 749.98] Microwaves, Wi-Fi.
[750.22 → 753.52] Yeah, I was going to say, does it drop out when you turn the microwave on it by any chance?
[753.94 → 754.34] I don't know.
[754.42 → 755.32] Maybe that is it.
[755.56 → 759.70] Because actually one of them going out is an LED light strip in the kitchen.
[760.02 → 761.20] Now that I think about it.
[761.20 → 764.52] The audience has kind of warned me about this.
[764.58 → 768.16] Because I've gotten hints that, like, you've got to get the right Zigbee adapter
[768.16 → 772.52] that has a perfect antenna that is, like, sticking out from the box or something.
[772.58 → 773.98] Like, I've seen some hints about that.
[774.06 → 775.26] And I just ignored all that.
[775.82 → 779.40] And I have a Zigbee antenna that hangs off of a USB hub
[779.40 → 784.18] that is actually mounted away from the Home Assistant Yellow.
[784.32 → 786.38] But it seems to be not strong enough.
[786.38 → 791.46] And I think I, you know, now I think about it, it's in the cabinet with my Wi-Fi router.
[793.08 → 795.38] And I didn't even expect this problem.
[795.58 → 797.78] Because previously I've been using Z-Wave.
[798.24 → 800.68] Z-Wave is a proprietary standard.
[801.52 → 806.50] But Z-Wave operates at 915 megahertz in the United States.
[806.50 → 813.72] And while it is lower bitrate, I think anybody that's familiar with the old wireless phones
[813.72 → 819.22] knows that 900 megahertz just goes farther and goes through walls more.
[819.56 → 822.12] And 900 megahertz is just less crowded.
[822.40 → 824.66] There's less going on at 900 megahertz these days.
[825.18 → 829.00] And so I just took for granted how well my Z-Wave network worked.
[829.06 → 829.70] I mean, rock solid.
[829.76 → 832.12] I'm talking devices way outside.
[832.60 → 833.74] You know, 100 feet outside.
[834.48 → 836.16] Still connected and still reporting in.
[837.10 → 838.46] Run for a year off a battery.
[838.88 → 840.86] I kind of expected the same thing for Zigbee.
[841.62 → 844.92] And that has not been my experience.
[845.04 → 845.90] And man, it sucks.
[846.18 → 847.48] Because it's several devices.
[847.70 → 849.32] So it's a temperature sensor that's failing.
[849.46 → 850.92] It's supposed to be monitored in my water bay.
[851.34 → 853.04] And it's the light strip that's failing.
[853.18 → 856.82] So sometimes we do the like, nighttime shutdown stuff.
[857.36 → 859.28] And I go to check on the kids and I realize,
[859.52 → 860.98] oh, crap, this light strip's still on.
[861.06 → 862.10] Like, the lights didn't turn off.
[862.10 → 863.28] Oh, it's disconnected.
[863.90 → 864.72] It's embarrassing.
[864.72 → 867.48] It destroys the family acceptance factor.
[868.36 → 868.80] Yeah.
[868.80 → 873.14] So what I ended up kind of piecing together, and I'm still kind of figuring it out,
[873.32 → 881.42] is if you get, this is true with Z-Wave too, if you get, like, a smart plug that's constantly powered,
[881.42 → 884.80] they will most often act as a network repeater.
[885.38 → 889.68] And they will rebroadcast the network and kind of make up for these gaps.
[890.06 → 892.40] But I think you have to have a fair amount of them.
[892.46 → 893.84] Like, quite a bit.
[893.90 → 896.28] It has to be a pretty dense network of these.
[896.40 → 898.32] In Z-Wave, that also wasn't the case.
[898.42 → 902.74] But I think it's because the transmitters and some of these low-powered devices are just really weak.
[902.74 → 907.16] And so you have to compensate by having a lot of mesh coverage.
[907.16 → 912.32] But your house for a bus or an RV is big.
[912.38 → 915.04] But for a home, it's pretty small, right?
[915.58 → 917.18] So you shouldn't be having this problem with it.
[917.74 → 920.18] I mean, we do have a lot of Wi-Fi in the area.
[920.30 → 923.22] So maybe it's just a lot of radio noise.
[923.30 → 926.64] Maybe it's because it's in the booth with my Wi-Fi access point.
[927.02 → 927.32] Yeah.
[927.60 → 928.60] Do you have 2.4?
[929.00 → 933.30] I have a lot of my IoT devices that are on Wi-Fi on the 2.4 network.
[933.46 → 934.00] Ah, right.
[934.80 → 935.10] Hmm.
[935.76 → 938.58] But Zigbee can use another frequency, right?
[939.10 → 939.82] Yeah, I think there is.
[939.90 → 944.14] And I think there's also something with Thread that is going to be part of the new Matter Standard that's going to help.
[944.14 → 951.02] So I feel like there are solutions coming, but nothing that's here right now that I can use.
[951.06 → 953.30] So I'm just kind of going back to Z-Wave devices for now.
[953.78 → 955.76] For the most part, the Z-Wave stuff just works.
[956.32 → 958.20] It's just there's more Zigbee things than ever.
[958.20 → 960.50] I've been noticing just an increase in Zigbee devices.
[960.64 → 961.96] I think it's probably because of Matter.
[962.16 → 964.04] So I just picked up a new multi-sensor.
[964.16 → 966.16] I love these Z-Wave multi-sensors.
[966.52 → 967.58] And they have a brand-new version.
[968.04 → 973.30] And here's something else I've noticed is you really get what you pay for with these little edge IoT sensor devices.
[973.30 → 977.30] And I'll admit, this Aztec Multi-Sensor 7, it's $70.
[978.12 → 980.26] And if you really think about it, you want one for every room.
[980.50 → 981.36] And this is expensive.
[981.36 → 989.98] But I have also been comparing these to $19 sensors and $30 sensors, $40 sensors, and none of them are as good.
[990.70 → 992.00] And none of them are as flexible.
[992.62 → 993.66] So it's just a solid.
[993.76 → 995.82] Aztec just made some solid Z-Wave devices.
[996.06 → 999.26] Are you sure that if you crack them all open, they're not going to look exactly the same?
[999.62 → 1000.02] They do.
[1000.20 → 1000.40] Yeah.
[1000.58 → 1001.56] They probably do.
[1001.80 → 1002.56] Except for this one.
[1002.56 → 1004.10] I have cracked a couple of them open.
[1004.56 → 1006.64] And this one is actually pretty neat.
[1007.76 → 1013.60] It's just the problem is I feel like Z-Wave's going away because matter's becoming more and more of a thing.
[1014.26 → 1015.06] It uses Zigbee.
[1015.84 → 1017.18] I feel like Z-Wave's just getting abandoned.
[1017.52 → 1021.50] But I think it's 900 MHz, I think, is the superior radio for this kind of stuff.
[1021.86 → 1023.78] Because you want it to be reliable like a rock, right?
[1023.78 → 1027.82] You flip a switch, and you want it to immediately turn that light on.
[1028.88 → 1030.02] That's what you get with Z-Wave.
[1030.02 → 1030.38] Hmm.
[1030.78 → 1031.30] You get real.
[1031.38 → 1037.80] Because it takes it off your TCP IP network, takes it off of the Wi-Fi, moves it off of 2.4 GHz,
[1038.00 → 1042.12] and puts it down on this super efficient 915 MHz radio network.
[1042.64 → 1044.12] Just a gosh darn thing of beauty.
[1045.06 → 1048.58] So anyway, I'll put a link to my multi-sensor that I really like in the show notes.
[1049.26 → 1051.80] Now, you weren't ever an Evernote user by any chance, were you?
[1052.28 → 1052.64] No.
[1053.18 → 1053.74] You lucked out.
[1054.08 → 1060.00] I'm more of a kind of SSH into my server and just NATO a text file kind of guy, to be honest.
[1060.62 → 1065.30] I started using Evernote way a long time ago when, like, the iPhone was new.
[1065.56 → 1066.78] And then kind of faded on it.
[1067.42 → 1071.46] Because they just did all these different permutations of UI and technology.
[1071.84 → 1073.64] But my wife stuck with it.
[1073.68 → 1074.80] She really likes it.
[1075.22 → 1079.62] It's one of the few apps where you can throw a bunch of different kinds of data,
[1079.72 → 1083.60] from pictures to PDFs to website clippings to notes.
[1083.84 → 1086.98] And it will index and OCR and tag it for you.
[1087.44 → 1091.54] And then years later, you can search for, like, RV exhaust, right?
[1091.58 → 1095.24] It'll show the PDF from the manufacturer that we put in there that talks about our exhaust system.
[1096.16 → 1097.84] It's really handy for that kind of stuff.
[1097.86 → 1101.76] Or you could take a picture of a business card and search that person's name.
[1102.24 → 1103.26] And it'll find it, right?
[1103.28 → 1106.00] Because it does the optical character recognition stuff.
[1106.00 → 1110.52] But they've been sold to a company called Bending Spoons.
[1111.48 → 1114.68] And Evernote says the acquisition should be completed in early 2023.
[1115.04 → 1116.44] And you'll love this one, Joe.
[1117.22 → 1118.80] They say nothing's going to change.
[1119.18 → 1120.16] It's going to be a good investment.
[1120.16 → 1122.22] That's always what happens with acquisitions, right?
[1122.80 → 1123.00] Yeah.
[1123.28 → 1126.08] Yeah, it's usually actually a warning sign these days when they say that.
[1126.44 → 1127.08] I start to worry.
[1129.00 → 1129.50] Uh-oh.
[1129.98 → 1131.36] They say nothing's going to change.
[1131.68 → 1131.96] Uh-oh.
[1133.16 → 1137.42] Yeah, so I feel like this is probably something we should look into on the show.
[1137.50 → 1138.90] So I kind of wanted to put a call out there.
[1138.90 → 1145.92] I'm curious if anybody has a self-hosted solution for something that kind of worked like Evernote.
[1146.02 → 1147.40] You know, a textual data store.
[1147.54 → 1148.30] You can index it.
[1148.38 → 1149.10] You can search it.
[1149.16 → 1152.34] It'll do the OCR of a PDF or a picture you throw in there.
[1152.70 → 1156.46] You know, maybe it'll even have an app on the phone that takes a picture of something and throws it in there.
[1156.56 → 1158.70] Ideally, it has a phone app and a desktop app.
[1158.74 → 1160.80] And ideally, it has sync and offline support.
[1161.66 → 1164.52] Also, ideally, multi-user or some kind of sharing.
[1164.78 → 1168.08] So the wife could create a note and then share it with me and vice versa.
[1168.08 → 1170.52] And I know I hear Obsidian already.
[1170.72 → 1171.48] People are writing Obsidian.
[1172.04 → 1176.48] But I just don't think that's going to have high wife approval factor.
[1176.88 → 1178.56] It sounds like you're looking for a unicorn here.
[1178.70 → 1185.42] That does not sound like it's even possible without a huge company behind it to have all those features.
[1186.02 → 1186.26] Yeah.
[1186.42 → 1189.28] I know Notion's an idea that, you know, it's again, but you're right.
[1189.58 → 1190.50] Company behind that.
[1190.66 → 1192.44] There are a couple of other ones I've looked at recently.
[1192.88 → 1193.12] But yeah.
[1193.44 → 1194.60] Now, what you want to do is, right,
[1194.60 → 1211.80] you want to have a horrible mess of Telegram messages that you send to yourself and some Google Docs and some, like I said, just text files on a server somewhere, maybe on your NAS that you can't even remember which directory you put it in.
[1211.80 → 1213.30] And that's the best way to do it.
[1213.30 → 1217.26] And then you just force yourself to remember things the hard way.
[1217.52 → 1218.00] And it's more fun.
[1218.00 → 1218.02] Yeah.
[1218.88 → 1221.22] There's a little bit of that approach currently for myself.
[1221.74 → 1227.56] The random documents on my server thing kind of hits home because I haven't restored.
[1227.56 → 1233.32] Like I had this little web UI that would render the markdown files into like this web browser thing so I could view my notes.
[1233.76 → 1237.72] But I haven't reinstalled that since my new server setup because I just don't use it that much.
[1238.08 → 1240.76] But when I do need the notes, I got SSH in.
[1241.20 → 1242.56] I got to look it up in NATO.
[1244.00 → 1244.40] Yeah.
[1244.44 → 1248.58] And then you can really top it off with some LibreOffice docs and some text files.
[1248.78 → 1252.58] So depending on whether you're actually at your desktop or SSH in to somewhere.
[1252.96 → 1254.62] Well, maybe somebody out there can save me.
[1254.62 → 1257.08] I do not want to do OneNote.
[1257.56 → 1259.52] I have heard that one quite a bit as well.
[1259.74 → 1262.82] But just not particularly interested in that ecosystem.
[1263.08 → 1266.66] And it would really be nice if it's something that I could self-host.
[1266.90 → 1268.34] I actually kind of feel like that's a requirement.
[1268.52 → 1271.98] Because otherwise, why not just stick with Evernote for a little bit longer until they really crash that ship.
[1272.68 → 1273.64] So let us know.
[1274.16 → 1275.54] Self-hosted. Show slash contact.
[1277.66 → 1283.64] Visit CrowdStrike.com slash LCE to ingest and view all of your logs in one place.
[1283.64 → 1289.48] Yeah, CrowdStrike Falcon Log Scale is CrowdStrike's new centralized log management and observability tool.
[1289.92 → 1299.38] Formerly known as Humid, Log Scale was developed as an alternative to legacy logging solutions that made it cost prohibitive to ingest and search the data that you just see in today's IT infrastructures.
[1299.80 → 1303.98] And the real beauty of Log Scale is that it can take logs from any source and make them usable.
[1304.30 → 1307.30] You don't need to constantly massage the formats and tweak it.
[1307.48 → 1308.40] It doesn't need a schema.
[1308.76 → 1311.14] You just pump it all in there, and you have it when you need it.
[1311.22 → 1311.82] And the dashboard?
[1311.82 → 1312.80] It's great.
[1314.16 → 1315.78] This platform is crazy.
[1316.00 → 1322.02] Log Scale's index-free architecture means you can ingest over a petabyte of data per day and then search that with sub-second latency.
[1322.20 → 1323.58] Not hours, not seconds.
[1324.14 → 1331.16] And Log Scale is up to 80% cheaper than competing platforms like Splunk or Elastic thanks to its reduced hardware and computational footprint.
[1331.16 → 1337.48] I realized I probably could have used Log Scale to get an alert and analyze when my original Home Assistant incident went down.
[1338.00 → 1343.08] So now I think I'm going to hook up my current Home Assistant yellow box to it, and then I can help troubleshoot when these Zigbee errors occur.
[1343.08 → 1346.88] I think probably the best way to get going is with Log Scale's Community Edition.
[1347.26 → 1350.56] It is the largest no-cost data ingestion offering on the market.
[1351.14 → 1356.08] And Log Scale Community Edition allows you to ingest up to 16 gigabytes per day with seven-day retention.
[1356.52 → 1357.74] No credit card required.
[1358.24 → 1359.46] No trial period.
[1359.46 → 1361.68] You've got it for the long haul.
[1362.54 → 1367.56] This is perfect for self-hosted who just want to ingest some home logs and get a single view of everything going on in your environment.
[1368.08 → 1370.78] It's way better than having separate places to go look at everything.
[1371.36 → 1375.34] Log Scale gives you the ability to bring it all together and correlate it in one place for easier troubleshooting.
[1375.90 → 1377.10] And that's nice when it's your hobby.
[1377.56 → 1378.16] You want it easy.
[1378.70 → 1380.00] You want it usable and quick.
[1380.42 → 1381.42] You don't want it to be a job.
[1381.94 → 1388.36] So go get started with Log Scale Community Edition for free at CrowdStrike.com slash L-C-E.
[1388.36 → 1392.16] That's CrowdStrike.com slash L-C-E.
[1394.44 → 1397.10] All right, Joe, how about we wrap it up with some feedback?
[1397.60 → 1400.08] I want to give a shout-out for our Matrix rooms out there.
[1400.18 → 1402.52] We've been seeing some growth in the meetup rooms.
[1402.62 → 1406.80] We have some dedicated rooms like a London Colony meetup room in honour of Joe being here.
[1407.18 → 1408.38] There's a Mumble Colony in there.
[1408.44 → 1412.14] There's one for Ohio, for folks going to Ohio Linux Fest.
[1412.90 → 1414.56] Matrix lets us create all kinds of rooms, so we do it.
[1415.02 → 1415.78] And you can find them all.
[1416.06 → 1418.18] Just go to jupiterbroadcasting.com slash Matrix.
[1419.02 → 1422.28] For the meets on that, sometimes you'll see a wild Joe in there, too.
[1423.50 → 1424.94] Rumour has it he's in the Metaverse.
[1425.28 → 1427.00] Rumour has it, yeah, if you look carefully.
[1428.62 → 1430.90] We got an email into the show from Belgium.
[1431.72 → 1432.96] Brain Damage writes in,
[1433.52 → 1435.04] Dear Chris and Alex, and also Joe,
[1435.62 → 1437.66] I've been listening to Self-Hosted since the start.
[1437.80 → 1439.30] Looking forward to it every release day.
[1439.66 → 1444.16] So I monitor my stuff, and I've tried monitoring software like Nagios, Prometheus,
[1444.36 → 1447.94] currently trying out Rabbi, but none of them seem to just click with me.
[1448.94 → 1450.88] I'm wondering what you're using and why,
[1451.00 → 1453.60] and if you've ever considered switching to another option.
[1454.28 → 1457.14] And also for your European listeners, the German website,
[1458.24 → 1462.74] itsco.de, most of the time has secondhand small form factor systems on sale.
[1462.74 → 1464.86] Yeah, I took a look, and there's a bunch on there.
[1464.96 → 1466.40] We'll put a link to that in the show notes, too.
[1466.80 → 1470.02] This is a good option for people just starting their self-hosted journey.
[1470.30 → 1471.70] Greetings from Belgium.
[1472.32 → 1473.94] So my answer is boring.
[1474.00 → 1474.94] It's just Uptime Kumar.
[1475.08 → 1477.00] And I wonder, do you have a favourite Uptime tool, Joe?
[1477.00 → 1483.72] Yeah, I use Uptime Robot, which is free for as many domains as I've ever thrown at it.
[1483.86 → 1486.76] And I think it monitors every five minutes and emails you,
[1486.96 → 1490.34] and then emails you when it's back up and tells you how long it was down for.
[1490.72 → 1493.76] It is very handy sometimes for my own sites,
[1493.88 → 1497.56] but really it's more handy for just watching some other sites
[1497.56 → 1501.70] and laughing at people who can't keep them up for very long a time.
[1501.70 → 1502.98] So that's good.
[1503.04 → 1505.80] So it gives you a report of their downtime.
[1506.50 → 1506.88] Yeah, yeah.
[1506.90 → 1509.56] And you can see the percentage uptime that each domain has,
[1509.58 → 1511.62] and you can just stick any domain you want into it.
[1511.78 → 1512.10] Nice.
[1512.50 → 1516.42] All right, we'll put a link to Uptime Robot in the show notes as well.
[1516.42 → 1520.26] And I'll give a shout-out to Uptime Kumar, which we have running here.
[1520.46 → 1522.26] And there's a few other good ones out there,
[1522.36 → 1525.04] but those are just simple enough that they're easy to set up.
[1525.20 → 1526.58] They're kind of nice for the hobby level.
[1527.28 → 1529.26] Yeah, and Uptime Robot does have a paid tier.
[1529.36 → 1531.42] I've never needed to try it, but presumably.
[1531.70 → 1532.08] It's better.
[1532.16 → 1532.46] I don't know.
[1533.02 → 1535.02] We got some big boosts this week, and we got a bunch,
[1535.06 → 1536.98] so we're going to read just a few on the show this week.
[1537.04 → 1539.10] The first one comes in from The Helpful Idiot.
[1540.08 → 1542.06] 320,001 sat, says,
[1542.16 → 1544.24] Long-time listener, first-time caller.
[1544.24 → 1545.40] Well, thank you, Helpful Idiot.
[1545.98 → 1546.92] Very generous boost.
[1547.00 → 1548.00] He says, Love the shows.
[1548.44 → 1551.14] I want to share my blog with you guys, thehelpfulidiot.com.
[1551.40 → 1553.24] It's nothing special, but it has a few examples,
[1553.34 → 1556.48] some of my home lab projects which were inspired by your shows.
[1556.92 → 1558.48] My day job is an eye doctor,
[1558.48 → 1563.08] and he sent a video behind his wire guard,
[1563.58 → 1565.26] like an cloud VM box,
[1565.74 → 1568.64] which might be in this picture on his website at helpfulidiot.com.
[1569.20 → 1570.18] There's some good stuff on here,
[1570.24 → 1571.92] including one that actually was very,
[1572.18 → 1573.88] which was actually kind of really up my alley,
[1573.98 → 1577.02] which are these big outdoor decoration lights
[1577.02 → 1578.34] that he's integrated with Home Assistant.
[1578.52 → 1580.02] It's funny that he's an eye doctor,
[1580.26 → 1582.04] and his cable management is an eyesore.
[1582.04 → 1584.28] Oh, calling him out.
[1584.88 → 1585.22] Calling him out.
[1585.22 → 1587.00] Well, at least it makes me feel better about mine.
[1589.22 → 1593.56] C-dubs boosted him with 40,404 SATs using Boost CLI.
[1593.74 → 1595.06] So that was a series of boosts.
[1595.10 → 1598.16] I think I put it all in one big baller boost.
[1598.26 → 1600.58] He says, I put together a little 1U NixOS router.
[1600.92 → 1605.04] It's got multiple LAN's and Wi-Fi set up with DHCP and NF tables.
[1605.74 → 1606.92] The Wi-Fi is wonky.
[1607.34 → 1609.68] Client connections just stop randomly.
[1609.68 → 1611.94] I wire guard proxy all of my traffic,
[1612.12 → 1614.58] but when I turn it on, nothing routes.
[1614.98 → 1615.76] It's probably my firewall.
[1615.88 → 1616.64] Not sure how to debug.
[1617.26 → 1618.62] I could use some tips.
[1619.00 → 1623.12] Well, C-dubs, you got a lot going on that one box, you know?
[1623.30 → 1626.28] And so I feel like Wi-Fi wonky.
[1626.50 → 1627.32] That's one issue.
[1628.14 → 1630.92] Client connections stopping randomly could be related to the Wi-Fi.
[1631.00 → 1633.56] That could be a third, or I'm sorry, a second issue.
[1633.90 → 1637.12] And then wire guard not properly routing your traffic.
[1637.12 → 1640.56] That's at least your third issue, if not your fourth issue.
[1641.06 → 1645.62] I feel like where I would start is I would probably try to break down each one of those
[1645.62 → 1648.04] into its own separate problem.
[1648.42 → 1649.50] Like, I'd start with the Wi-Fi.
[1649.62 → 1656.16] Like, what's the point of even fixing the routing and the firewall issue if your Wi-Fi isn't working?
[1656.16 → 1658.14] So I'd probably start with the Wi-Fi.
[1658.78 → 1660.10] Figure out what's going on there.
[1660.30 → 1661.28] You know, check D-message.
[1661.58 → 1663.08] Run journalctl-f.
[1663.28 → 1664.38] Watch your log for a bit.
[1664.76 → 1665.88] See if you can catch it happening.
[1666.94 → 1667.36] I don't know.
[1667.38 → 1668.06] You got any thoughts, Joe?
[1668.34 → 1669.50] I think just what you said, really.
[1669.62 → 1674.56] Try and break it down into systematic chunks that you can work on.
[1674.68 → 1676.94] Don't try and work on the whole thing at once,
[1676.96 → 1679.20] because there's too much going on to do that.
[1679.24 → 1680.50] There are too many moving parts.
[1680.50 → 1685.02] Let's try one of the moving parts at a time and just work through it logically
[1685.02 → 1688.20] until you solve each problem, and then the whole thing will work.
[1688.68 → 1695.52] I wonder, too, C-dubs, if you're on a later Linux kernel, like a 602 or later,
[1696.20 → 1699.66] because I swear, man, I've been having wonky Wi-Fi issues
[1699.66 → 1702.54] on the latter, more recent 6-series kernels.
[1702.98 → 1704.74] I don't know how long you've had that NIC system installed,
[1704.74 → 1708.40] but if you could roll back to, like, 5.18,
[1708.40 → 1712.92] I would give that a try and see what happens, too, for your Wi-Fi issues,
[1712.98 → 1717.80] because I have a machine that actually have two laptops
[1717.80 → 1720.64] that are having really wonky Wi-Fi.
[1720.74 → 1721.92] One's not connecting reliably,
[1722.80 → 1726.36] and the other is experiencing really long latency
[1726.36 → 1729.44] at different parts of the network that just doesn't really make sense.
[1729.52 → 1731.82] Like, sometimes several hops outside my direct land,
[1732.52 → 1735.76] one laptop that's having Wi-Fi issues will have four, five,
[1735.82 → 1737.30] 600 milliseconds on a route,
[1737.30 → 1739.32] and all the other machines on the LAN
[1739.32 → 1742.16] have no problem with that one hop.
[1742.48 → 1743.64] I'm having the weirdest problems,
[1744.02 → 1745.86] and it's been since the later 6-series kernels.
[1746.36 → 1748.14] Yeah, or you could just try Ubuntu or something,
[1748.30 → 1750.06] rather than a fancy OS like NixOS.
[1750.62 → 1751.78] Could always try a live session.
[1751.86 → 1752.92] That's actually a pretty good tip.
[1753.72 → 1754.60] Try a live session.
[1755.38 → 1758.40] See if you have some of the same Wi-Fi issues
[1758.40 → 1759.86] in the live session.
[1760.22 → 1762.28] With a different OS, maybe an older kernel.
[1762.82 → 1764.68] Yeah, or dig out an old SSD or something,
[1764.84 → 1766.70] install it on that, and just boot off that temporarily.
[1767.70 → 1769.70] Optimum Gray boosted in with some grandpa ducks,
[1769.78 → 1771.72] 22,222 SATs.
[1771.80 → 1772.92] He says, I need your help.
[1773.54 → 1774.50] I'm an anti-Google.
[1775.08 → 1777.32] I just don't like being the product of a company
[1777.32 → 1779.04] that's like the thing that's being sold.
[1779.14 → 1781.36] So when I hear this great tool is free to use,
[1781.80 → 1783.02] and it makes everyone's life better,
[1783.02 → 1784.52] my radar gets lit up.
[1785.06 → 1786.18] Tail scale, a great tool,
[1786.86 → 1788.48] but a company that's not looking to make money,
[1788.66 → 1789.36] I don't understand.
[1789.48 → 1791.74] P2P connects are very cheap, so they don't need much.
[1792.08 → 1794.66] But my radar is up for something am I not seeing.
[1794.66 → 1797.56] I just don't like connections to everything on my network,
[1797.64 → 1799.18] so my radar is going off.
[1799.50 → 1802.54] I know they sponsor JB, but I wanted your input.
[1802.92 → 1803.86] That's a fair question,
[1803.92 → 1806.52] and I think it's one that Tail scale gets enough
[1806.52 → 1810.08] that they did a blog post about how they make money
[1810.08 → 1813.06] and how they built their network
[1813.06 → 1814.88] to make it sustainable,
[1815.04 → 1816.44] because I think that's a common question.
[1816.96 → 1818.90] So the short version is where they make money
[1818.90 → 1821.06] is if you want to have more than 20 devices
[1821.06 → 1823.20] that get connected to that LAN, you got to pay.
[1823.58 → 1825.44] Yeah, which is a pretty good business model.
[1825.56 → 1826.98] I mean, they sponsor my shows as well,
[1827.46 → 1828.84] so I'm somewhat biased here,
[1828.90 → 1832.14] but it seems like your classic business model,
[1832.26 → 1834.38] give away just enough to get people hooked,
[1834.52 → 1836.14] and then, you know, you're using it
[1836.14 → 1838.62] on five, six, ten devices on your LAN,
[1839.14 → 1840.24] and then you go into work
[1840.24 → 1841.48] and talk about how great it is,
[1841.48 → 1844.64] and then suddenly you're on two or three hundred devices.
[1845.16 → 1847.04] Yeah, it's kind of the Dropbox idea too, right?
[1847.12 → 1849.08] Dropbox used to give away like five gigs for free,
[1849.08 → 1850.62] so everybody could just start sharing files
[1850.62 → 1851.54] with up to five gigs,
[1851.56 → 1852.72] and they would spread it around.
[1853.18 → 1854.40] Yeah, but the advantage here is
[1854.40 → 1856.06] that if you are just a hobbyist,
[1856.24 → 1857.92] you can just take advantage of it for free
[1857.92 → 1860.30] and let all the corporate customers pay for you.
[1860.56 → 1861.60] Yeah, and he really nailed it there.
[1861.68 → 1864.14] The reason for that is because they are peer-to-peer,
[1864.26 → 1866.82] so when you're communicating with another machine
[1866.82 → 1867.68] on the Tail scale network,
[1867.74 → 1868.88] you're talking directly through it.
[1868.98 → 1872.14] You're not routing through the Tail scale servers.
[1872.32 → 1873.74] The Tail scale servers come in
[1873.74 → 1875.06] for the authentication backplate
[1875.06 → 1876.34] that kind of authorizes
[1876.34 → 1878.32] your single sign-on provider
[1878.32 → 1879.96] to get access to that network,
[1880.80 → 1883.76] and then basically then authorizes the machine
[1883.76 → 1884.36] to have a key,
[1884.70 → 1885.98] and then it gets access to the network.
[1886.34 → 1887.70] That key expires from time to time,
[1887.72 → 1888.66] and you have to re-authenticate,
[1889.38 → 1890.98] or you can set some not to expire as well.
[1891.06 → 1891.86] And if you ever have to do that
[1891.86 → 1892.84] with more than 20 machines,
[1893.26 → 1897.12] then you end up becoming a paid Tail scale user.
[1898.26 → 1899.76] Rapid Mustang also boosted in
[1899.76 → 1901.80] with a Mc Duck row of Grandpa Ducks,
[1901.86 → 1903.68] 22,222 SATs.
[1903.68 → 1905.04] I learned about you guys
[1905.04 → 1906.60] from when you were on Level 1 Techs.
[1907.10 → 1908.60] Started listening and really enjoyed it.
[1908.92 → 1910.14] Now I listen to all the JB shows.
[1910.76 → 1911.68] Glad to give back now.
[1911.80 → 1912.72] Keep up the great work.
[1912.98 → 1913.38] Well, thank you.
[1913.44 → 1915.28] You know, I think we've got to have Wendell on again.
[1916.26 → 1917.48] I've gotten a few notes about that.
[1917.96 → 1919.62] Check in with Wendell and see what he's been up to.
[1919.72 → 1921.32] See how his self-hosting setup is going.
[1921.42 → 1922.42] See what's changed about it.
[1923.06 → 1924.98] Maybe find out what he's doing differently in 2023.
[1926.46 → 1927.36] Thank you, Rapid Mustang.
[1927.54 → 1928.26] And thank you also.
[1928.36 → 1929.68] We got a lot more boosts in.
[1930.38 → 1931.84] So just a couple of random call-outs.
[1931.84 → 1937.14] We got 67,000 SATs from Moutons Corral.
[1938.28 → 1940.86] I think I put that in there just to see if I think I put that in there.
[1940.96 → 1941.42] I remember now.
[1941.74 → 1942.86] See if I could pronounce it.
[1942.96 → 1944.66] Now I'm realizing I could not.
[1945.22 → 1945.94] They just say hi.
[1946.66 → 1947.84] 911 SATs from Noob.
[1948.70 → 1950.76] He says this is his very first boost ever.
[1951.28 → 1952.44] We got a couple of double boosts.
[1952.48 → 1953.00] Came together.
[1953.54 → 1954.26] Double elite SATs.
[1954.40 → 1956.82] 2,674 SATs from Sir Lurksalot.
[1957.28 → 1960.48] Was listening live last week and wanted to send some support in.
[1960.48 → 1963.56] We got 9,709 SATs from Zero.
[1963.84 → 1965.20] Just trying out Breeze for the first time.
[1965.30 → 1966.60] 50,000 SATs from ENTEC.
[1966.84 → 1967.96] Throwing some love our way.
[1968.32 → 1970.52] He's a 14-year self-hosting Vetted as well.
[1970.98 → 1971.64] Thank you, ENTEC.
[1971.68 → 1973.64] Your support across the shows has been appreciated.
[1974.36 → 1977.60] And we got 119,999 SATs from WE.
[1978.22 → 1980.44] He was on a series of boosts across all the shows.
[1981.22 → 1982.20] Spraying some SATs.
[1982.64 → 1983.84] And he wanted to spray some love.
[1984.26 → 1985.38] Over at Self-Hosted.
[1985.76 → 1987.58] Thank you, everybody else who boosted in.
[1987.96 → 1989.60] We'll read some of those in the post-show, I suspect.
[1989.60 → 1992.96] If you'd like to boost into the show, go get a new podcast app.
[1993.40 → 1994.80] A newpodcastapps.com.
[1995.18 → 1997.66] And special geek cred if you figure out how to do it with Boost CLI.
[1997.78 → 1999.68] That is a freaking setup.
[2000.24 → 2004.02] Joe, tell people where they can find you after they get done listening to this here show.
[2004.54 → 2008.64] So either latenightlinux.com or 2.5admins.com.
[2009.20 → 2009.82] There you go.
[2009.90 → 2012.56] And you can catch Alex on 2.5 Admins.
[2012.56 → 2015.48] And then get all caught up.
[2015.66 → 2019.12] Then join us over in our Discord at self-hosted. Show slash Discord.
[2019.52 → 2022.18] You can become a member and support the ongoing production.
[2022.42 → 2023.64] You get an ad-free version.
[2023.84 → 2030.98] And you get the post-show by becoming one of our site reliability engineers at self-hosted. Show slash S-R-E.
[2030.98 → 2035.26] with some hinted at but yet to be fully disclosed features coming to the members feed.
[2036.08 → 2037.32] Hopefully in early 2023.
[2038.34 → 2038.64] I don't know.
[2038.68 → 2043.42] It depends on when Santa, Was, and I are done working on things.
[2044.62 → 2045.90] Joe, it's good to catch up with you.
[2046.14 → 2046.70] Good to hear from you.
[2046.74 → 2047.68] Thanks for filling in for Alex.
[2048.44 → 2049.02] Yeah, it's been great.
[2049.96 → 2051.28] And thank you everybody for listening.
[2051.28 → 2053.82] That was self-hosted. Show slash 84.
