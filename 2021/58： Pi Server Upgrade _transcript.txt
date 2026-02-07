[0.00 --> 5.38]  Well, given that we only record every two weeks, it's not often that I get the chance to say,
[5.76 --> 15.38]  breaking news! I have some exciting news about the Prusa XL, a 3D printer that is enormous.
[16.30 --> 20.82]  Okay. Wait, when you say enormous, how enormous are we talking about?
[21.46 --> 28.14]  So, the standard size for a 3D printer has kind of been dictated by the Prusa Mark III now for
[28.14 --> 35.94]  several years. Similar size to like the Ender 3 and the Creality CR10, all these guys, they've had a
[35.94 --> 43.28]  build volume that's been in the region of 10 inches by 8 by 8, something like that, which is 25 by 21
[43.28 --> 52.08]  by 21 centimeters. This new one from Prusa, 14 inches square. Ah, okay. So, it's a big boy.
[52.08 --> 59.42]  Okay. That's adequate, at least. Yeah. Now, what's really interesting is the Prusa Mark III
[59.42 --> 64.64]  has a bed that moves back and forwards and the extruder moves left and right and that kind of
[64.64 --> 71.04]  stuff. So, there's a lot of moving parts. The Prusa XL is so big that they couldn't really figure out a
[71.04 --> 76.50]  way to make the bed move properly and smoothly. So, they're doing what's called a Core XY 3D printer
[76.50 --> 83.02]  for this. So, essentially what that means is the extruder does all the movement and the bed moves
[83.02 --> 90.96]  up and down. Aha. Which is pretty cool. It sounds like my place. Now, this thing has five interchangeable
[90.96 --> 97.10]  or up to five interchangeable tool heads. That's great. So, you put your order in, I assume.
[97.10 --> 103.96]  Oh, no, no, no. Because this thing, wait for it, starts at $2,000.
[105.02 --> 107.18]  Oh. And that's before you've tricked it out.
[107.66 --> 113.52]  Yeah. I mean, that's beyond even Alex Impulse purchase territory at two grand. You know what I
[113.52 --> 118.76]  mean? Here's what we do is we launch a merch store that's filled with stuff that we've 3D printed. It
[118.76 --> 125.44]  pays for itself. Yeah. Yeah. So, it's not that easy, you know. I've had a few things up on Etsy that
[125.44 --> 130.10]  I've been 3D printing for a while, like workshop accessories, that kind of thing. And I've sold
[130.10 --> 134.88]  a few, but I mean, I've come nowhere close to even paying for a couple of spools of filament,
[135.02 --> 141.38]  you know? So. Yeah, there is that. I guess you got to deduct the cost of the machine,
[141.62 --> 145.66]  the materials, and God forbid your time. And the electricity. Don't forget that.
[146.26 --> 151.00]  Right. All that's valuable. So, that's why you should probably go learn it at cloudguru.com,
[151.04 --> 154.94]  the leader in learning for cloud, Linux, and other modern tech skills. Hundreds of courses,
[154.94 --> 161.02]  and thousands of hands-on labs. Get certified, get hired, get learning at a cloudguru.com.
[162.78 --> 166.32]  I've been thinking about talking a bit more about 3D printing on the show. If you're interested
[166.32 --> 172.82]  in a segment on 3D printing, let me know, selfhosted.show slash contact. Now, something
[172.82 --> 176.96]  else I found on the internet this week, well, I guess it was a couple of weeks ago now, was-
[176.96 --> 178.52]  It was like just after the last episode.
[178.76 --> 183.08]  Yeah, literally a day or two after the last episode. It was a new toy for you, Chris, a Raspberry
[183.08 --> 185.22]  Pi compute module powered router.
[186.16 --> 188.32]  Ah, you're spending my money again, Alex.
[188.34 --> 188.54]  Yeah.
[188.86 --> 190.46]  It's easier when it's someone else's.
[191.08 --> 196.34]  Yeah. Well, this is perfect timing because we have a project to replace the router here
[196.34 --> 201.06]  at the studio and we want something that does WireGuard. I've decided after the last road trip
[201.06 --> 208.82]  that I wanted to divorce my VPN and server because guess what? My server was down and I couldn't
[208.82 --> 213.28]  VPN into troubleshoot. I want to put it on the router. I've wanted it that way for a long time,
[213.40 --> 215.18]  but I got a confession.
[215.58 --> 218.74]  Dear listener, Alex is nodding very, very strongly right now.
[220.04 --> 226.40]  I've been using the Comcast router that came with my Comcast business internet since they
[226.40 --> 230.72]  gave it to me. I just, it worked. Can we have a sad tuba sound effect, please, editor?
[230.72 --> 239.52]  I know. The only excuse really is truly just I didn't feel like Googling. That's barely an excuse.
[239.88 --> 246.92]  So this is obviously something that needs to be fixed. And you found this fantastic dual gigabit
[246.92 --> 254.78]  ethernet carrier board for the Raspberry Pi 4 compute module. It's a pretty small board, smaller than the
[254.78 --> 260.20]  original size of the Raspberry Pi, not quite, but around that size that you snap the compute module
[260.20 --> 268.78]  onto and you get USB ports, you get ethernet, you get HDMI. And I should make it clear, you get two
[268.78 --> 273.04]  ethernet, which wouldn't that be great? You know, you can have one interface connected to your LAN,
[273.12 --> 277.70]  you have one interface connected to your network, to your ISP or whatever it might be. And you know,
[277.78 --> 280.14]  you can build yourself a firewall.
[280.14 --> 288.28]  Are they both on the PCI bus? Because only one of them is like on the Raspberry Pi 4 at least is PCI,
[288.34 --> 288.46]  right?
[289.90 --> 294.44]  Sadly, I would say you have cut right to what the core issue is.
[294.50 --> 295.34]  Oh no.
[296.28 --> 304.26]  Interface 0 is on the PCI bus. So like that would be a great LAN interface, right? But interface 1
[304.26 --> 309.14]  connects via USB, which is then connected to the PCI bus. And...
[310.14 --> 318.24]  This is also a challenge because stock OpenWrt does not have a driver for that. So you, if you install
[318.24 --> 322.96]  just regular old Linux or Raspberry Pi OS, you're good to go. I mean, it's like there's been a driver
[322.96 --> 330.94]  since like kernel 4. But OpenWrt has decided not to ship that. And a friend of the show, Jeff Gerling,
[331.04 --> 336.26]  you know, he posted a poll request saying, hey, how about adding this support for this? And it doesn't
[336.26 --> 337.16]  seem like it's going anywhere.
[337.36 --> 337.54]  Yeah.
[339.28 --> 344.62]  It was actually funny. Speaking of Jeff, I was doing some research on this very thing and I came across
[344.62 --> 348.64]  this whole GitHub thread that he had created on this very issue. And it was actually really useful
[348.64 --> 355.08]  to know, don't go with stock OpenWrt with this router board because of this issue. And if you look
[355.08 --> 360.36]  at the documentation from the folks over at, what is it? Seed Studios? Is that what it is?
[360.36 --> 361.76]  Yeah. Link in the show notes.
[362.28 --> 371.76]  Yeah. On their wiki, they link to their own build of OpenWrt, which has the driver. So if you get the
[371.76 --> 377.70]  image from them, you're pretty much good to go. But I'd like to back up and talk about why I wanted
[377.70 --> 384.00]  this because the compute module has interested me for a while because I think that the critical flaw
[384.00 --> 392.14]  in the Raspberry Pi 4 as a server for me was the SD card. Just sucks. It's fine for booting the
[392.14 --> 398.54]  random OS here and there, but you don't want to run your server on that. And you can get the compute
[398.54 --> 408.20]  module with a built-in eMMC, up to 32 gigs of eMMC. And that's pretty appealing. So I thought that would
[408.20 --> 412.56]  be the way to go, or, you know, maybe an external USB drive. But I really wanted to try the eMMC
[412.56 --> 418.72]  and see how that works. And I got this device pretty quickly. I was shocked because I've tried
[418.72 --> 423.76]  to get the compute module on its own in some cases, and I've seen prices as high as $130 right now.
[424.40 --> 428.88]  And I think this whole thing all in was like $80. Then depending on the price of the compute
[428.88 --> 434.10]  module, it goes up from there. So you get it, and it's really small. One thing I didn't like about it
[434.10 --> 439.94]  is they put the SD card on the bottom of the board, and it's right under the HDMI port. So when you're
[439.94 --> 443.78]  plugging in the HDMI port, you're thumbing the SD card, which is a trigger to eject.
[444.48 --> 449.68]  And it's really frustrating. And then the USB-C port's also in the same area. And so when you're
[449.68 --> 453.76]  like kind of using your thumb to brace on the board so you can pull the power out,
[454.66 --> 460.40]  well, guess what you're doing? You're ejecting the SD card. It's kind of annoying. So if you can
[460.40 --> 463.58]  avoid it, just don't use the SD card. I don't like the way they've designed that at all.
[463.58 --> 472.44]  But the tricky thing is flashing eMMC. I didn't really appreciate this. But if you want to flash
[472.44 --> 479.46]  the eMMC with an image, a pre-built image directly, you got to move some jumpers on this little board
[479.46 --> 484.62]  to put it in a specific kind of boot mode. So it shows up as an external storage on your OS.
[484.84 --> 488.14]  Then you got to install a driver, and you got to actually flash it that way.
[488.14 --> 495.62]  Well, I wasn't down for that. I said, no, thank you. Thanks anyways. And I went and got myself
[495.62 --> 499.70]  OpenSUSE at Tumbleweed, because I've been diving deep into Tumbleweed recently,
[500.36 --> 507.24]  downloaded their Arch 64 image, just their generic ISO, not a Raspberry Pi image, not an image file,
[507.32 --> 513.78]  but an ISO, which is also an image file, downloaded that to my machine, and I flashed it to a Samsung
[513.78 --> 522.44]  SSD, a USB-C SSD, the ISO image, plugged it into the USB port on this little board,
[522.72 --> 529.66]  booted it up like a regular old PC. It booted off the SSD, because there's no OS on the thing.
[530.94 --> 535.38]  I booted up the SUS installer, which was crazy-ass slow, like ridiculously stupid slow.
[535.84 --> 540.18]  They're taking every opportunity to check your packages, scan your hardware, double-check this.
[540.18 --> 544.82]  I mean, I'm not exaggerating when I say maybe it was nearly a 30-minute boot process,
[545.32 --> 547.08]  just to get to the installer.
[547.12 --> 547.42]  Oh my god.
[548.02 --> 552.24]  Yeah. But then you get a full graphical Yast installer and all that kind of stuff,
[552.30 --> 554.78]  which is, you know, that's nice. That's nice to see.
[554.98 --> 555.66]  30 minutes.
[556.82 --> 558.96]  Yeah, and it took quite a while to install it, too.
[560.08 --> 564.76]  I noticed on the console that it was like checking repositories,
[564.76 --> 568.68]  and every single thing it was checking was 404ing on the console.
[568.68 --> 571.80]  But I could ping, right?
[571.88 --> 575.10]  Like, I had no problem getting out and routing to the internet.
[575.28 --> 577.08]  So I don't know what exactly was going on there,
[577.12 --> 579.22]  but it seemed to just really slow stuff down.
[580.96 --> 586.00]  But goodness, if my name isn't Chris, I'll tell you what.
[587.18 --> 590.88]  The SUSE installer just saw the EMMC like it was a hard drive.
[592.12 --> 593.38]  No big deal at all.
[593.38 --> 598.02]  It just auto, the whole auto partition, auto install the bootloader, it all worked.
[598.08 --> 603.94]  It just, it installed to the EMMC on this Raspberry Pi compute module as if it was an x86 PCI.
[604.02 --> 607.38]  Just booted off a thumb drive and was installing to the internal disk.
[607.74 --> 609.32]  It felt like a real computer.
[609.52 --> 613.76]  And then it rebooted, and sure enough, I'm in OpenSUSE Tumbleweed, and it's good to go.
[613.96 --> 615.22]  And it worked great.
[615.22 --> 619.26]  I did do a little bit of benchmarking on the old EMMC because I was curious.
[620.20 --> 626.62]  And, you know, I saw anywhere between 80 to 200 megabytes a second.
[627.54 --> 629.52]  I don't really think it's very high.
[629.56 --> 632.26]  I don't think it's very good performance in terms of, like, overall.
[632.44 --> 634.76]  Like, if you want this thing to be faster, it's not going to be that.
[634.92 --> 636.60]  But it's way better than the SD.
[637.26 --> 640.66]  That's the same kind of level of performance as a spinning hard drive.
[640.66 --> 641.10]  Yeah.
[642.42 --> 644.04]  Yeah, it kind of performs like a, yeah.
[644.22 --> 647.38]  Yeah, that's a good way to think of it, Alex, is it kind of performs like a spinning hard drive.
[648.40 --> 650.64]  Yeah, that's a no from me, dog.
[651.28 --> 651.52]  Yeah.
[653.22 --> 658.22]  Well, you know, some of these compute module boards have NVMe slots and stuff.
[658.90 --> 660.46]  Or PCI Express slots.
[661.24 --> 665.32]  It's still an order of magnitude better than the SD card.
[665.94 --> 666.60]  Yeah, oh, for sure.
[666.98 --> 667.50]  Yeah, for sure.
[667.50 --> 671.44]  At what point do we sit back and think we're flogging a dead horse here, you know?
[671.96 --> 676.66]  Everything you've just told me, there wasn't a single thing that made me think, oh, I need this now.
[677.04 --> 682.32]  Like, when I first saw the link, I was like, huh, okay, now I'm going to take this seriously.
[682.44 --> 684.20]  But hearing what you've just said, I'm like, oh.
[685.28 --> 685.56]  Yeah.
[686.20 --> 687.46]  Reality doesn't match.
[687.46 --> 700.36]  I mean, you could use, like I do on my Pi 4 servers in the RV, you could use an external USB 3 SSD, which I never would have done until I was in this situation.
[700.60 --> 702.38]  And I can't believe how well it's worked.
[702.58 --> 703.62]  It's embarrassing.
[704.42 --> 708.16]  Like, what am I, two years now into using these things with SSDs that are over USB?
[708.38 --> 708.82]  It's stupid.
[708.94 --> 710.16]  It shouldn't be working, but it is.
[710.16 --> 711.52]  So you could go that route.
[711.66 --> 718.08]  Or, you know, I'm going to get the IO board that I think has a PCI-1X express slot on it.
[718.32 --> 719.30]  And I want to get an MV.
[719.36 --> 722.98]  I already have an MVME adapter for that, that I'm going to try that.
[725.10 --> 730.22]  The other area that's a bit of a limit in terms of performance is thermals.
[730.94 --> 732.58]  So this thing runs hot.
[732.58 --> 738.02]  I think there's not a lot of room between the router board and the compute module.
[738.46 --> 739.56]  So it runs warm.
[740.30 --> 743.28]  And I was throwing different jobs at it.
[743.34 --> 746.42]  Like, I thought, let's, this is a great opportunity to try out Jellyfin again.
[746.52 --> 747.60]  It's been a couple of years.
[748.16 --> 751.30]  And so I tossed Jellyfin on there and had it scan my library.
[751.38 --> 754.48]  And the CPU got up to like 181 degrees Fahrenheit, which is pretty hot.
[755.12 --> 758.90]  Then I started a build of net data while the library scan was going on.
[758.98 --> 760.92]  And it got up to 186 degrees.
[760.92 --> 764.92]  Sorry, in real numbers, that's 82 Celsius.
[765.50 --> 765.78]  Right.
[766.02 --> 768.06]  I ain't dealing in your freedom units, dude.
[768.12 --> 769.46]  I know I live here, but still.
[769.98 --> 773.76]  I think I saw it got up to 85 Celsius is the highest I saw it get somewhere out there.
[773.80 --> 774.54]  I mean, that's warm.
[774.68 --> 775.78]  I mean, you know, Intel.
[775.78 --> 777.14]  That's where it starts to thermal throttle, though.
[777.54 --> 781.32]  You know, real CPUs, air quotes, real CPUs get up to, what, 100?
[781.70 --> 783.42]  And then they start throttling.
[783.70 --> 785.16]  So 85 is okay.
[785.28 --> 785.74]  It's warm.
[786.42 --> 786.56]  Yeah.
[786.56 --> 787.64]  No, it's fine.
[787.76 --> 789.26]  And it'll handle it all.
[789.26 --> 794.34]  It's literally been going now for more than 24 hours.
[794.68 --> 799.18]  And I'm still getting like 1.5 gigahertz out of most of the cores most of the time.
[799.40 --> 801.42]  It's going as we record right now.
[801.42 --> 812.98]  So if you put a heat sink or you put it in a case with a fan, I think you'd get a little bit less thermal throttling out of this thing is kind of what my takeaway was, because this is just naked.
[813.78 --> 814.86]  You know, it's just absolutely naked.
[815.44 --> 817.80]  I saw decent performance on the network transfer.
[817.80 --> 823.94]  I will have a better take on how it works as a router after I've, you know, gone through all of the paces there.
[824.10 --> 828.38]  But I don't have a super fast connection to deal with.
[828.72 --> 837.96]  So I was getting around 600 megabits out of the interface that's connected to USB, which is the ETH1.
[838.80 --> 840.56]  600 megabits is doable for me.
[840.56 --> 843.72]  I have a 300 megabit Comcast connection, right?
[844.24 --> 845.64]  I have a gigabit LAN.
[846.02 --> 849.02]  So the LAN interface, that's on the PCI bus.
[849.30 --> 849.96]  That'll be full.
[850.06 --> 852.68]  That's like you get nearly 900 megabits a second out of that thing.
[853.46 --> 862.74]  And because the interface connected to USB is still twice as fast as my internet connection, I don't really think it's going to be a problem.
[862.74 --> 868.92]  The only other downside I could foresee is that stuff on the USB bus also takes more CPU.
[869.38 --> 872.20]  So I could see it putting more load on the box.
[872.28 --> 874.78]  So I won't know until I put this thing into production in that regard.
[875.16 --> 885.04]  But as far as like this, could this work as I can no longer wait for the Home Assistant Amber to arrive because of part delays or something.
[885.12 --> 886.28]  So I'm going to deploy this.
[886.36 --> 887.20]  Could it work as that?
[887.26 --> 887.50]  Yes.
[887.50 --> 893.64]  I think this would be a pretty good upgrade from my current Pi setup as servers.
[893.76 --> 901.52]  I think this compute module on a board, especially maybe the IO board, which is arriving tonight after we record, funny enough.
[901.64 --> 904.04]  If it just would have showed up a little earlier, I could have told you.
[904.22 --> 906.32]  But I bought it like two days later.
[906.44 --> 908.10]  And so, of course, it's showing up a little late.
[908.52 --> 912.38]  But I think that has real potential for me to build a server platform around.
[912.84 --> 915.92]  And when I look at this and what do I get out of it?
[915.92 --> 920.82]  What I get out of it is two to three watts of power draw, even when it's being slammed.
[921.32 --> 922.68]  That's massive for me.
[923.12 --> 932.68]  And to get dual network ports and to have additional IO, depending on which board you put the compute module into, while having access to the Raspberry Pi ecosystem of support.
[932.68 --> 949.06]  And at this point, you can pull down Arch, Fedora, Alma Linux, and, of course, CentOS, and RHEL, and Ubuntu that all just work out of the box using the generic ARM64 ISO image now.
[949.20 --> 950.62]  And they work with this stuff.
[950.62 --> 956.72]  And so we've gotten past the point where you've got to go find this very specific image to get it all to work.
[957.14 --> 963.32]  And that opens the door up to a lot more people, in my opinion, and a lot more standard server-type operating systems.
[963.66 --> 970.32]  Just in time for the Raspberry Pi 5 to come in and require a whole new bunch of esoteric builds.
[970.60 --> 971.32]  I wonder.
[971.76 --> 972.68]  Yeah, you're probably right.
[972.68 --> 972.72]  All right.
[973.08 --> 973.80]  We'll see.
[974.66 --> 983.86]  I also, after I was reading through the thread that Jeff had started, I found another board that he's talked about before in the past that has both NICs on the PCI bus.
[985.30 --> 986.74]  Yeah, so I ordered that one.
[987.02 --> 987.84]  Of course you did.
[987.96 --> 988.32]  Of course you did.
[988.32 --> 989.44]  It was like 30 bucks.
[989.58 --> 990.14]  So, like, why not?
[990.26 --> 990.40]  Right?
[990.74 --> 995.22]  Once you've got the compute module, this is where this is actually quite a powerful little thing.
[995.96 --> 996.04]  Right.
[996.04 --> 999.98]  For those that aren't familiar, the compute module is slightly smaller than the Pi 4 itself.
[999.98 --> 1004.04]  And it just sort of pops into a daughter board, if you like.
[1004.92 --> 1012.32]  And then lots of different people make different breakout boards, I suppose, that expose different interfaces for the Pi and stuff like that.
[1012.48 --> 1016.06]  So the one that Chris has been talking about, obviously, is focused at being a router.
[1017.26 --> 1023.22]  But this I.O. board, for example, exposes, like, it's got an NVMe slot on it and all sorts of other stuff.
[1023.22 --> 1023.70]  Yeah.
[1025.06 --> 1030.66]  And a battery for the real-time clock, which is something that the Pi has traditionally been missing.
[1031.06 --> 1031.32]  Huge.
[1031.32 --> 1033.60]  Which is another nice little, yeah, nice thing for a server.
[1033.96 --> 1034.60]  Yeah, very cool.
[1034.94 --> 1038.40]  Well, I put a link in the show notes to that Seed Studio website.
[1039.28 --> 1042.32]  It's spelt a little bit funny, so you will need to go and look it up how it's spelt.
[1042.32 --> 1048.36]  And they do still have, if you can believe it, the compute module 4s in stock shipping today.
[1048.70 --> 1050.92]  So take it for what it's worth.
[1051.16 --> 1051.70]  Chris bought one.
[1051.74 --> 1052.20]  It showed up.
[1052.28 --> 1053.58]  So hopefully it does the same for you.
[1053.64 --> 1055.02]  We're not affiliated in any way.
[1055.52 --> 1056.44]  I wish you luck.
[1058.10 --> 1060.28]  Leno.com slash SSH.
[1060.36 --> 1064.54]  Go there to get $100 in 60-day credit on a new account, and you go there to support the show.
[1064.82 --> 1069.78]  It's like the next best thing to being jacked into the matrix and having information downloaded to your brain.
[1069.78 --> 1077.32]  I mean it, because you can go on there and you can just learn and play and investigate and test.
[1077.96 --> 1079.98]  I mean, that's a huge part of what I use Linode for.
[1080.40 --> 1085.70]  When I think about how it's changed my game over the years, doing just a little bit of research here and there,
[1085.80 --> 1089.60]  trying something out every now and then, and when you add it all up, man,
[1090.16 --> 1095.62]  that's been one of the keys to getting things done on time for these shows and being able to get things figured out.
[1096.26 --> 1099.20]  But, you know, Linode really is just super fast, too.
[1099.20 --> 1101.02]  And I think that's a big part of why I've stuck with it.
[1101.38 --> 1103.26]  They just rolled out new MVME disks.
[1104.08 --> 1106.46]  They've got 40 gigabit connections coming to the hypervisors.
[1106.92 --> 1108.20]  They are their own ISP.
[1109.08 --> 1111.58]  That's the level of control they have over their connectivity.
[1112.22 --> 1114.34]  They've got 11 data centers to choose from.
[1115.28 --> 1120.50]  And I feel like it is a bit of a superpower because it's how we've hosted everything for the last couple of years.
[1120.50 --> 1125.18]  And, you know, frankly, our audience would tell us if something wasn't up to snuff.
[1125.68 --> 1131.54]  There's a higher expectation with Jupyter Broadcasting that our technology stack is going to respect your privacy,
[1131.54 --> 1138.06]  that's going to perform well, that it's going to be up when you want to download a show right before you hit the road or something like that.
[1138.06 --> 1142.20]  And, you know, you're all kind of picky, as I am.
[1142.74 --> 1148.28]  And if things didn't work right, if the infrastructure wasn't up to snuff, you'd tell us.
[1148.88 --> 1153.56]  And we literally get zero complaints because Linode is just screaming fast.
[1153.66 --> 1159.22]  And it's 30 to 50 percent cheaper than the major hyperscalers out there that just want to lock you into their platforms anyways.
[1159.22 --> 1161.74]  And that's one of the nice things about Linode.
[1163.14 --> 1167.70]  I strike that balance with Linode where I feel like I'm in control.
[1168.26 --> 1170.28]  I have the power in this relationship.
[1170.96 --> 1174.36]  And I think that's also really important for just the type of business person that I am.
[1175.16 --> 1178.54]  But like I said earlier, like there's so much you could learn and try with Linode, too.
[1178.56 --> 1180.50]  And that's where that $100 is really special.
[1180.64 --> 1187.82]  That is actually a unique opportunity because with $100, you can really try out the platform, see what you can do with it.
[1187.82 --> 1196.30]  And then, you know, if you ever have any problems, they've got the best customer support in the business by phone or ticket or even on social.
[1196.44 --> 1200.22]  If you're a customer, they're going to help you out and they're going to I think they're going to impress you.
[1201.04 --> 1204.46]  They also have just a bunch of great tutorials and how to guides.
[1204.62 --> 1209.06]  They have S3 compatible object storage that I use just the crap out of.
[1209.78 --> 1215.90]  So from the best customer support, super fast rig, super fast networking and a Linux culture that runs deep.
[1215.90 --> 1221.62]  There's just like a lot of these types of reasons to choose Linode, but you'll find your own.
[1221.88 --> 1222.68]  So go try it out.
[1223.26 --> 1225.54]  Linode.com slash SSH.
[1227.48 --> 1227.92]  Right.
[1228.12 --> 1231.64]  So we're not really going to be talking about self-hosting for the next few minutes.
[1231.64 --> 1242.28]  I want to have a bit of a rambling gripe grudge airing fest about Android 12 and everything that I think is wrong with the state of the mobile ecosystem these days.
[1242.28 --> 1246.68]  I'm actually up for it because how do you get how do you access all these things you're hosting?
[1246.80 --> 1250.44]  A lot of times it's through a mobile device or a tablet on the wall or something like that.
[1250.84 --> 1257.28]  You know, it was interesting as well as I posted a tweet last night or the night before about saying, you know, Pixel 6 isn't for me.
[1258.20 --> 1261.46]  I can't stand Android 12 UI, which I'll come on to shortly.
[1261.46 --> 1267.96]  And the fingerprint reader sucks and the phone is too slippery and, you know, all these different reasons.
[1268.58 --> 1272.72]  And then a couple of people reminded me why I was excited about buying it in the first place.
[1273.02 --> 1277.70]  The stuff that the Pixel does that is genuinely pretty cool.
[1277.80 --> 1289.02]  So they've got this call screening thing built in for scammers, which if you don't live in the US, like in the UK, that you can just register with some telephone preference service.
[1289.02 --> 1290.92]  But in the US, there's no such thing.
[1291.56 --> 1297.12]  And I get, you know, it's a brand new phone number to me that I've obviously only ever given out to a few people.
[1297.94 --> 1303.50]  And I get four or five spam calls a day that just love to call me and just say nothing.
[1304.40 --> 1305.46]  Does that happen to you?
[1306.54 --> 1308.40]  Oh, well, it did for a long time.
[1308.50 --> 1308.64]  Yeah.
[1308.98 --> 1309.32]  Yeah.
[1309.40 --> 1313.84]  I've got a couple of apps that screen calls on the iPhone because they did open up an API for that.
[1314.20 --> 1316.64]  But it's not built into the OS like it is with Google Assistant.
[1316.64 --> 1324.34]  My mom got a call recently saying that she owed AT&T $1,200 for an iPhone, but the whole call was a scam.
[1324.78 --> 1326.46]  But she was very convinced.
[1326.56 --> 1327.94]  So she calls me up.
[1328.32 --> 1329.40]  She's like, I owe somebody money.
[1329.50 --> 1330.34]  Like, what's going on?
[1331.14 --> 1332.26]  Like, mom, it's a scam.
[1332.60 --> 1332.74]  Yeah.
[1332.82 --> 1333.78]  It's absolutely a scam.
[1333.94 --> 1334.06]  Yeah.
[1334.06 --> 1341.62]  And that kind of stuff is really nice just to, when you're at work and your phone, you know, maybe you're in a meeting, it's nice to have something catch that kind of thing.
[1341.64 --> 1343.08]  So it doesn't interrupt your day.
[1343.08 --> 1343.36]  Yeah.
[1343.42 --> 1343.94]  Yeah.
[1343.98 --> 1347.14]  Not only do they have call screening, so that's inbound.
[1347.66 --> 1359.10]  They've also added with the Pixel 6 a new outbound kind of on hold Google Assistant will be on hold for you type mode, which is legitimately very, very cool.
[1359.38 --> 1363.58]  It uses all of the text to speech stuff to listen to what the phone is saying.
[1363.78 --> 1364.86]  The person on the phone is saying.
[1364.86 --> 1367.64]  And it will print it out in text for you on the screen.
[1368.16 --> 1370.88]  So, you know, press 1 to talk to sales.
[1371.04 --> 1372.18]  Press 2 to talk to.
[1372.26 --> 1375.38]  And by the time you got to option 7, you're like, what was option 1 again?
[1376.22 --> 1377.56]  It's on the screen in front of you.
[1377.58 --> 1379.68]  So I found that quite helpful a couple of times.
[1381.44 --> 1386.50]  But yeah, in general, I just couldn't deal with Android 12.
[1386.96 --> 1387.32]  You know?
[1387.32 --> 1389.96]  It's just I think they've ruined it.
[1391.28 --> 1399.86]  There's also in the background like the slow and continued effort to de-Google different services over different, you know, like different chunks.
[1400.00 --> 1402.02]  Like I still haven't gone back to Google Maps.
[1402.18 --> 1404.98]  Like that was a successful de-Googlefication.
[1405.24 --> 1407.84]  It was rough because I did it on the road trip.
[1407.98 --> 1414.76]  But I think because I did it on the road trip, I had to do it like in anger, under pressure, and it stuck.
[1414.76 --> 1415.50]  Like great.
[1415.78 --> 1420.86]  So I wonder too, like, does this play into that at all for you?
[1421.54 --> 1422.20]  A little bit.
[1422.34 --> 1422.50]  Yeah.
[1422.54 --> 1436.48]  I mean, when I saw the news this week that Apple have somehow made a U-turn on right to repair and made some parts available, previously only available to authorized service centers and stuff like that,
[1436.48 --> 1443.76]  I think to myself, okay, that's another pin down on the Apple domino board of stuff that I care about.
[1443.76 --> 1448.24]  So, you know, right to repair, I can get parts for my phone and my laptop shortly.
[1448.52 --> 1448.66]  Okay.
[1448.66 --> 1462.80]  Right now it's only a very small program, but I'm excited for what that means over the next five, ten years of how they're going to expand that program and hopefully start designing the devices with a bit more modularity in mind so that people can just pop out the logic board and pop out a battery.
[1462.80 --> 1467.66]  And that kind of basic stuff that after two or three years, the phone still functions fine.
[1467.98 --> 1470.80]  You think, oh, I wish I could just have a new battery.
[1471.24 --> 1472.94]  I don't want to buy a whole new phone.
[1473.54 --> 1477.14]  Well, that's hopefully going to be the reality moving forward.
[1477.14 --> 1487.60]  The other thing that Apple are doing pretty well, and I was really suspicious of this at first, but I think their privacy stance is actually really solid.
[1487.96 --> 1499.96]  You know, a lot of the stuff that they're doing with the ask to track stuff in iOS, you know, particularly I've seen articles talking about how much that's hurt Facebook and specifically their targeted advertising.
[1500.96 --> 1502.56]  Okay, you've got me.
[1502.66 --> 1504.06]  I am really impressed by that.
[1504.16 --> 1505.32]  Google could never do that.
[1505.32 --> 1505.48]  Right.
[1506.38 --> 1507.28]  Well, that's true.
[1507.38 --> 1507.56]  Yeah.
[1507.94 --> 1509.00]  You know, it's funny.
[1509.18 --> 1520.38]  It is good to see them make these right to repair moves, and I do like to see them make anti-track moves on the platform, even if they're, in some cases, just asking apps not to do it.
[1520.82 --> 1527.58]  But then I see them doing, like, the library scanning stuff, and I'm like, boy, you got to, with Apple, there's a lot of good with the bad you have to take.
[1527.62 --> 1529.18]  And that's the thing that I've been struggling with.
[1529.18 --> 1534.52]  So, for me, I have to ask myself, how important is customizing my device?
[1534.52 --> 1540.24]  Like changing out the launcher, maybe even just putting an entirely different OS on there or a different image.
[1540.84 --> 1544.26]  And for different devices, I have different answers to that question.
[1544.26 --> 1554.06]  If you were to ask me about the fire tablets that I have littered throughout my homes now, the studio, or at least the studio in the RV, I would say extremely.
[1554.46 --> 1556.36]  I want to always be able to reflash that.
[1556.44 --> 1557.92]  I always want to be able to replace the launcher.
[1558.14 --> 1563.48]  That is probably the two top features of those devices for me, right?
[1563.48 --> 1567.04]  Mostly because the fire launchers are just garbage.
[1567.38 --> 1568.36]  And so unstable.
[1568.50 --> 1570.24]  Very slow and unstable, yeah.
[1570.48 --> 1570.82]  Yeah.
[1571.60 --> 1576.28]  And it's like, okay, maybe a decade ago, but what are we doing today?
[1576.34 --> 1576.98]  What's going on here?
[1577.50 --> 1578.98]  It's just unacceptable.
[1579.70 --> 1584.70]  So, you know, but I've never wanted that from my phone.
[1584.70 --> 1591.60]  And I think maybe I'm just an old enough of a guy where I've never totally wanted that.
[1591.86 --> 1598.04]  I wanted that early on in the early days of Android when there was like things I was getting from it.
[1598.10 --> 1604.10]  Maybe improved battery life, improved performance, getting the OS on a device that didn't get that OS because the vendors bailed so quickly.
[1604.24 --> 1605.88]  Or maybe the camera app was better.
[1606.16 --> 1607.52]  The same reason that you're into Linux.
[1607.94 --> 1608.14]  Yeah.
[1608.34 --> 1609.72]  You like to tinker under the hood.
[1609.84 --> 1610.10]  I mean.
[1610.66 --> 1611.06]  Right.
[1611.06 --> 1612.02]  That's just you.
[1612.56 --> 1612.80]  Yeah.
[1612.92 --> 1619.04]  And I want my phone to always take a picture and I want it to always make a call.
[1620.40 --> 1623.88]  So I didn't really have that same requirement for that device.
[1623.92 --> 1626.32]  And I think those things shift for us too over time.
[1626.44 --> 1631.34]  You may really, for example, like the launchers, maybe replacing the launchers with something you did all the time.
[1631.96 --> 1634.28]  And then the vendor started to get it right after a while.
[1634.42 --> 1636.94]  So the need to replace it stopped becoming as necessary.
[1637.24 --> 1641.04]  It's funny you should say that because I've been running a OnePlus 7T for the last two years.
[1641.78 --> 1641.98]  Yeah.
[1641.98 --> 1645.80]  I think that's actually the last good device that OnePlus made.
[1646.04 --> 1648.22]  But I still replaced the launcher.
[1648.46 --> 1649.56]  So it's running Android 10.
[1650.12 --> 1659.14]  It did run Android 11, but I wiped and downgraded it because the update that OnePlus shipped for Android 11 was, it was just so buggy.
[1659.24 --> 1660.90]  Like it just kept dropping the frame rate.
[1661.02 --> 1662.50]  It's a 90 hertz display.
[1663.12 --> 1666.66]  And it kept dropping the frame rate to like 20 or 30 frames a second.
[1666.98 --> 1668.54]  And I noticed that kind of thing.
[1668.76 --> 1673.64]  So I had to go into the settings and toggle it to 60 hertz and then back to 90 and it was fine again.
[1673.64 --> 1679.30]  I also have the Google work profile installed on my phone.
[1679.30 --> 1682.04]  So it has like, I love the way Android does this, by the way.
[1682.12 --> 1685.50]  It has like two separate profiles, like modes on the phone.
[1686.06 --> 1686.28]  Yeah.
[1686.66 --> 1687.30]  That's nice.
[1687.30 --> 1690.54]  All my work apps are completely separate from my personal apps.
[1690.64 --> 1693.04]  So like I've got two Gmail apps installed on my phone.
[1693.28 --> 1697.22]  So it's very obvious for me when I'm context switching, two calendar apps, you know.
[1697.22 --> 1704.94]  You could achieve that in iOS as far as customizing alerts and icons.
[1705.20 --> 1707.16]  Like you could have a focus mode that is work.
[1707.34 --> 1713.28]  And so you'd have work launchers and you'd have work alerts, but you would not be able to have two versions of Gmail.
[1713.48 --> 1715.76]  You'd have to have essentially two mail apps.
[1715.84 --> 1717.80]  One's a personal mail app and one's your work mail app.
[1718.04 --> 1721.94]  I'll tell you what's also awesome is there's an app I've got called Quiet for Gmail.
[1721.94 --> 1726.94]  And I have it set on a timer and it turns my email on and off at 8am.
[1727.08 --> 1728.42]  It turns it on at 6pm.
[1728.54 --> 1729.16]  It turns it off.
[1729.44 --> 1739.96]  And then for the rest of the time, I can just go into the app and swipe to refresh and it will, you know, load my emails if I really want to at, you know, midnight check, you know, a Sunday night before work or whatever.
[1740.70 --> 1748.70]  But, you know, on the whole, it's a very easy way to separate concerns between the two contexts of my life.
[1748.70 --> 1762.28]  And there was some really awful bugs in the way the underscreen fingerprint reader on the 7T and Android 11 just kept not working very well.
[1762.70 --> 1766.04]  And, you know, I use it dozens of times a day and it was very frustrating.
[1766.04 --> 1772.98]  So I've gone back to Android 10 on the 7T and forever there it shall stay until I find a replacement, you know.
[1773.16 --> 1773.72]  What could go wrong?
[1774.08 --> 1774.66]  That'll be fine.
[1774.96 --> 1776.94]  But that brings me back to the Pixel 6, I think.
[1776.94 --> 1780.66]  And the in-screen fingerprint reader.
[1781.94 --> 1783.26]  Oh, God, is it bad.
[1783.94 --> 1785.06]  It's really bad.
[1785.32 --> 1787.58]  You know, I've had one for two years in my OnePlus device.
[1788.22 --> 1796.58]  And sure, you know, when I'm, you know, baking bread or doing something and my hands are a little bit greasy or sweaty or whatever, it doesn't work all the time.
[1796.58 --> 1798.46]  But I have the pattern to unlock.
[1798.58 --> 1801.00]  And on OnePlus devices, I have face unlock as well.
[1801.84 --> 1803.24]  Don't have face unlock on a Pixel.
[1804.10 --> 1805.86]  It seems like something they would have ripped off by now.
[1805.86 --> 1806.90]  Yeah.
[1807.18 --> 1810.16]  Well, I mean, all the OnePlus are doing is using the selfie camera.
[1810.28 --> 1815.18]  It's not like a Face ID system like Apple with fancy 3D dot matrix scanners.
[1815.42 --> 1815.86]  It's just...
[1816.50 --> 1817.94]  Does that look vaguely like Alex?
[1818.16 --> 1819.10]  Yeah, that'll do.
[1820.18 --> 1821.02]  Is that a picture?
[1821.12 --> 1821.64]  Who cares?
[1822.42 --> 1822.82]  Right.
[1822.92 --> 1823.34]  Exactly.
[1823.34 --> 1830.48]  And for the most part, I mean, if you physically got my phone, I'm probably going to notice, you know, unless you're my kid.
[1830.66 --> 1831.96]  And then maybe.
[1832.38 --> 1834.12]  But she's not quite old enough for that yet.
[1835.08 --> 1836.32]  She'll be coming for it soon.
[1836.38 --> 1836.62]  Yeah.
[1836.78 --> 1837.02]  Yeah.
[1837.02 --> 1838.14]  She started crawling this week.
[1838.20 --> 1839.16]  So that's been fun.
[1840.18 --> 1845.66]  I remember early on when I was in a grocery store and I figured out, wait a minute, are there rattle apps?
[1845.98 --> 1847.54]  There is rattle apps.
[1847.84 --> 1848.16]  Perfect.
[1848.38 --> 1849.46]  Here, hold this.
[1849.52 --> 1853.68]  And this is like, I'm going to let you hold this, you little monster, while I pay for these groceries.
[1853.94 --> 1855.86]  This $1,000 baby rattle.
[1858.16 --> 1858.52]  Yeah.
[1858.52 --> 1860.60]  Really kind of ridiculous, actually.
[1861.26 --> 1865.64]  So fingerprint readers aside, because, you know, you can kind of just about learn to deal with that.
[1866.58 --> 1871.56]  We've got to talk about Android 12 and this Material U interface redesign.
[1871.98 --> 1873.84]  Have you seen much in the way of screenshots?
[1874.04 --> 1875.18]  You've got a Pixel 3, right?
[1875.64 --> 1876.00]  I do.
[1876.24 --> 1876.54]  I do.
[1877.26 --> 1879.64]  It's up to date as far as the Pixel 3 will go.
[1879.78 --> 1881.02]  So I don't know.
[1881.30 --> 1884.56]  But I have not immersed myself in it.
[1884.56 --> 1886.96]  I have heard a lot of different takes on it, though.
[1887.00 --> 1888.08]  So I'm curious to know what you think.
[1888.08 --> 1891.24]  Because I've actually heard people that like it, and it doesn't sound like you do.
[1891.68 --> 1892.14]  Well, they're wrong.
[1892.28 --> 1892.78]  I'll tell you.
[1894.34 --> 1895.44]  Do you like padding?
[1896.58 --> 1897.68]  I mean, not really.
[1897.80 --> 1899.48]  I generally find it to be kind of gross.
[1899.80 --> 1905.66]  Because if you like lots of wasted white space on a beautiful big display, then Android 12 is for you.
[1906.34 --> 1911.10]  It makes it feel like the whole UI just isn't designed for your screen size.
[1911.38 --> 1911.70]  No.
[1911.70 --> 1913.22]  You know, so there's a couple of things.
[1913.22 --> 1919.20]  And they're almost all to do with how the notification center toggle swipe down thing operates.
[1919.64 --> 1930.96]  So on my OnePlus device, which is running, like I say, Android 10, I have 12 toggles that I can customize to be practically anything on my phone that are just a tap.
[1930.96 --> 1932.16]  You know, want to turn Wi-Fi off?
[1932.48 --> 1933.24]  Swipe tap.
[1933.50 --> 1933.96]  That's it.
[1934.00 --> 1934.92]  It's all in one place.
[1934.98 --> 1936.04]  It's all at the top of the screen.
[1936.28 --> 1937.34]  It doesn't move around.
[1937.76 --> 1939.38]  It's just in one place.
[1939.44 --> 1940.70]  And there are 12 different things.
[1940.76 --> 1944.52]  And I can long press to get to the settings of Wi-Fi or Bluetooth or whatever it is.
[1944.92 --> 1945.28]  Right.
[1945.28 --> 1947.96]  It's a really elegant system.
[1948.72 --> 1950.52]  Android 12, there are four.
[1951.78 --> 1953.00]  That's just crazy.
[1953.56 --> 1953.88]  Mm-hmm.
[1954.28 --> 1960.08]  And not only that, one of those options now is a new internet toggle.
[1960.08 --> 1975.22]  So rather than it being a simple single tap to turn off Wi-Fi, I have to swipe, tap, and then do this hand kind of gymnastic gesture all the way down to the bottom of the screen, then toggle off Wi-Fi.
[1978.28 --> 1988.32]  You know, that's so funny because it seems like even iOS, right, it's going in the direction of like control center where there's just way more things you can do just by sliding down the screen.
[1988.32 --> 1990.48]  Like even Apple has added a whole bunch of buttons there.
[1991.04 --> 1992.54]  Why go back?
[1992.72 --> 1994.04]  Why reduce functionality?
[1994.18 --> 1995.60]  Why make you take more tabs?
[1995.72 --> 1996.80]  Yeah, that kind of stuff is frustrating.
[1996.80 --> 1997.34]  I don't know.
[1997.78 --> 1999.02]  It was too complicated, Alex.
[1999.08 --> 2003.34]  The problem was it was too complicated of a UI, and it was intimidating to new users.
[2003.44 --> 2004.50]  They needed to make it simpler.
[2005.24 --> 2010.74]  You're sounding like the comment section on one of Linus Tech Tips Linux Challenge videos at this point.
[2011.48 --> 2013.10]  We hear this all the time.
[2013.18 --> 2015.42]  Who are these mythical new users?
[2015.70 --> 2016.40]  Who are they?
[2016.40 --> 2028.30]  I don't know because it's funny because Google changes it all the time with every single release, and so it causes users, these new users, to actually lose their footing.
[2028.44 --> 2037.20]  It's the geeks who can adapt, and people criticize the iOS launcher for being very slow to change and the notifications, which got a huge change in the last OS.
[2037.60 --> 2038.42]  It still sucked there.
[2038.42 --> 2050.26]  Yeah, but at the same time, the reality is all of my family members that got an iPhone or an iPad a decade ago are more competent today.
[2050.38 --> 2051.64]  Like they know how to get to settings.
[2051.76 --> 2052.80]  They know how to change stuff.
[2052.88 --> 2053.76]  They know how to launch apps.
[2053.94 --> 2060.08]  They have evolved their skill set, and my family members that have Android devices are still lost as hell.
[2060.08 --> 2063.76]  Every time they get an Android device, the buttons are all in a different place.
[2064.10 --> 2070.02]  The setting screen is reorganized, renamed, and they start at zero every single time.
[2070.06 --> 2077.22]  And every time Google reorganizes these drop-down screens, they're making it harder for these very new users that they're trying to design this stuff for.
[2077.22 --> 2079.18]  You know what it feels like?
[2079.24 --> 2083.42]  And I think it was Tyler on Twitter that said it most succinctly to me.
[2083.76 --> 2088.80]  It feels like someone has slapped a cheap skin on top of my stock Android.
[2089.78 --> 2092.86]  And it just doesn't work.
[2092.94 --> 2093.88]  It doesn't fit for me.
[2094.00 --> 2100.74]  And, you know, they tout all these features like it picks up colors from your wallpaper and changes the theme throughout.
[2100.86 --> 2102.30]  I don't want that.
[2102.70 --> 2104.54]  I want to set it and forget it.
[2104.54 --> 2110.26]  It is a production device that should just always be exactly as I left it.
[2110.34 --> 2110.66]  That's it.
[2110.72 --> 2111.30]  That's its job.
[2113.58 --> 2114.26]  It's funny.
[2114.34 --> 2123.48]  That has been a trend recently of, like, we will automatically detect a primary color in your website or in your background, and we'll completely recolor the UI so that way it matches.
[2123.78 --> 2128.40]  And users' response is always, no, don't really want that.
[2129.18 --> 2131.62]  I think Big Sur might have started this trend, actually.
[2131.80 --> 2132.28]  You know, Apple.
[2132.34 --> 2132.58]  Right.
[2132.58 --> 2142.16]  Maybe even going back to, was it, iOS 7 when they introduced, like, the new Crayola-style, you know, cartoonish kind of vibe to it.
[2142.30 --> 2143.10]  It was a big redesign.
[2143.34 --> 2144.48]  It was a while ago now.
[2145.06 --> 2145.20]  Yeah.
[2145.26 --> 2149.42]  Well, wasn't there just a big upset about Safari, like, changing colors and stuff?
[2149.70 --> 2150.84]  New tab design or something.
[2151.02 --> 2151.18]  Yeah.
[2151.28 --> 2152.66]  And taking colors from websites.
[2152.66 --> 2153.44]  And people hate it.
[2153.76 --> 2155.08]  People don't like change.
[2155.66 --> 2156.54]  Why change it?
[2156.76 --> 2157.64]  It's not broken.
[2157.64 --> 2161.14]  Radical change for just change sake, I think, is what people don't like.
[2161.60 --> 2168.70]  I mean, I'm the type of guy that installs Bartender on my Mac so that I can condense the icons in Big Sur back together again.
[2168.90 --> 2169.18]  You know?
[2169.18 --> 2172.54]  I don't need things spacing out more and more.
[2172.62 --> 2177.22]  Like, I have a very fine cursor on a laptop or, you know, a computer.
[2177.34 --> 2179.50]  I don't need finger-sized buttons.
[2181.50 --> 2181.94]  Yeah.
[2182.04 --> 2190.68]  And on a phone, I tell you, you know, you give me a six and a half inch display or whatever, and you reduce my options by an order of magnitude.
[2190.68 --> 2191.68]  I just...
[2191.68 --> 2193.86]  Can I tell you what my lesson is from this?
[2194.58 --> 2202.08]  Is that if you're building an app or you're hosting something or whatever it is, web apps are still the best way to go.
[2202.88 --> 2206.36]  Because all of these OS platforms disappoint in some other way.
[2206.62 --> 2209.84]  And, like, you can be an Android fan for a while, and then you get burned out.
[2209.90 --> 2211.62]  You can be an iOS fan for a while, you get burned out.
[2211.66 --> 2216.42]  And it's not like you can go out and buy some other phone at any scale, at any practicality right now.
[2216.42 --> 2221.56]  But as long as it's a web app, well, you can get to it from any phone OS.
[2221.70 --> 2223.24]  You can get it from any desktop OS.
[2223.90 --> 2225.26]  Ultimately, it is the neutralizer.
[2226.06 --> 2232.28]  Which brings me to my final nail in the coffin for iOS for now.
[2232.50 --> 2235.84]  And I do hope the courts kind of change how this is going to go.
[2236.66 --> 2243.16]  I was listening to Craig Federighi passionately defend against sideloading.
[2243.16 --> 2246.24]  And I could not believe some of the trash.
[2247.08 --> 2248.90]  It's so embarrassing to listen to him.
[2249.42 --> 2249.82]  Cringy.
[2250.32 --> 2254.50]  And for me, on Android, you know, I discovered Sponsor Block this week for YouTube.
[2254.90 --> 2260.74]  By the way, if you've not come across this thing, it will cut out the intros of YouTube videos.
[2261.00 --> 2264.68]  And this video is brought to you about, like, all that stuff is just gone.
[2265.10 --> 2266.68]  You know, like and subscribe is gone.
[2266.88 --> 2267.34]  Just gone.
[2267.86 --> 2268.44]  It's amazing.
[2268.44 --> 2271.90]  And I wanted to sideload this on my Android TV device.
[2272.28 --> 2273.46]  And I can do that.
[2273.76 --> 2276.94]  If I wanted to do this on an Apple TV, I mean, I don't have one.
[2277.08 --> 2278.42]  But I assume it would be more difficult.
[2278.60 --> 2281.96]  Because why would Apple approve something like that through the App Store, you know?
[2282.56 --> 2282.74]  Yeah.
[2284.08 --> 2291.50]  So, for now at least, I think I'll stick with my 7T until something better comes along.
[2291.50 --> 2299.84]  Although the grass over on the iOS side is looking ever more slightly verdant and greener.
[2300.08 --> 2304.54]  I'll probably buy one at some point and then regret it and return it like I always do.
[2305.24 --> 2309.06]  Well, since we'll probably never have this chat again on the show, or we will have it very infrequently,
[2309.50 --> 2313.66]  I just want to add, because I don't get an opportunity to do this very often,
[2313.66 --> 2316.78]  and it holds true now about two years in.
[2317.26 --> 2322.08]  I think something we do not give iOS enough credit for on this show in particular is that
[2322.08 --> 2330.58]  if you are a Home Assistant user, you can use HomeKit to integrate with the iOS HomeKit system.
[2331.68 --> 2336.60]  And every device you have in Home Assistant, every light, every fan, every thermostat,
[2336.60 --> 2343.74]  shows up as a HomeKit device to your iPhone, which means it shows up as a device to Siri.
[2343.96 --> 2346.32]  It shows up as a device to your watch.
[2346.58 --> 2348.82]  It shows up when I pull down the control panel.
[2349.34 --> 2351.28]  And it changes location, too, by the way.
[2351.66 --> 2355.04]  So, when I'm at the studio, it updates to devices that are here.
[2355.12 --> 2357.76]  And when I go home, it updates to devices and jupes.
[2358.24 --> 2359.22]  And as I'm here right now...
[2359.22 --> 2362.64]  Is that what you've been telling me about this HomeKit Bridge for ages?
[2362.82 --> 2364.20]  No, HomeKit Bridge is a little different.
[2365.08 --> 2365.92]  That's a little different.
[2365.92 --> 2369.76]  And that HomeKit Bridge allows you to talk to devices that don't natively speak HomeKit.
[2370.16 --> 2372.88]  It'll, like, talk whatever they speak and bridge it to HomeKit.
[2373.06 --> 2373.76]  Oh, okay.
[2373.76 --> 2377.60]  But this, this actually, like, you connect the HomeKit to...
[2377.60 --> 2380.76]  You connect the HomeKit on the iOS to Home Assistant,
[2381.00 --> 2383.34]  and Home Assistant actually speaks native HomeKit now.
[2383.60 --> 2389.60]  And it means every device is in here, and I can use voice prompts on HomePods, on the phone,
[2389.60 --> 2391.76]  but also in Control Center, in the Home app.
[2391.76 --> 2399.46]  And it also means if you want, if you have a family iOS setup, so, like, my wife and kids, we're all family in iOS,
[2399.98 --> 2402.62]  they also get access to devices through the Home app.
[2402.72 --> 2404.56]  I don't even have to give them the Home Assistant app.
[2404.78 --> 2406.96]  And it works remotely because we have a HomePod.
[2406.96 --> 2414.48]  So, and it really is, it's very special, and there's nothing quite close to that integration on Android without going all in on Google Assistant.
[2415.20 --> 2423.92]  And additionally, what I love about it is the Home Assistant app for iOS is a particularly great piece of software.
[2423.92 --> 2430.88]  And the developer who makes the iOS Home Assistant app deserves a few beers, just for me personally,
[2431.00 --> 2432.42]  because it is such a great app.
[2432.74 --> 2438.10]  And they've recently added focus mode support as a sensor to Home Assistant.
[2438.56 --> 2440.56]  So I want you to think about what that means for a second.
[2440.66 --> 2442.22]  I have an NFC tag on my mixer.
[2442.60 --> 2443.52]  I sit down.
[2443.84 --> 2445.46]  I set my phone on this tag.
[2445.70 --> 2447.48]  It goes into recording focus mode.
[2448.64 --> 2450.68]  Now Home Assistant knows I'm in recording mode.
[2451.04 --> 2452.16]  So lights change.
[2452.16 --> 2455.50]  I can do all kinds of automations based around that.
[2455.72 --> 2458.56]  And it all happens without me having to do hardly anything.
[2459.12 --> 2461.10]  And last part, and then I'm totally done.
[2461.38 --> 2464.28]  Because all of the devices show up in HomeKit,
[2464.66 --> 2469.78]  I can actually just use the built-in shortcut app on iOS.
[2470.16 --> 2474.60]  So if I never wanted to write a Home Assistant automation because I felt it was too complicated or whatever,
[2474.94 --> 2478.50]  I could do all my automations with shortcuts on iOS and on the Mac
[2478.50 --> 2481.40]  and just have it talk to the devices like HomeKit devices.
[2481.40 --> 2483.04]  And you could just do that.
[2483.26 --> 2484.16]  And it's fantastic.
[2484.58 --> 2489.22]  And it's something that I think is five notches above anything you can do on Android with Home Assistant.
[2489.66 --> 2490.84]  And I think it's fantastic.
[2491.08 --> 2494.16]  But other than that, you know, I agree there's nice things about both platforms.
[2494.26 --> 2499.54]  But I just think that's an area where iOS perhaps has a leg up for us Home Assistant users.
[2499.54 --> 2503.60]  Yeah, and this rant, it wasn't too much of a rant, I don't think.
[2503.68 --> 2509.28]  But this segment for me isn't necessarily a, I think iOS stinks and Android is better.
[2509.44 --> 2519.66]  I just think in general, they've both got significant issues that I don't know what the next few years holds in the mobile OS space.
[2519.66 --> 2526.08]  There's room for a third player, honestly, to come along and disrupt, I think.
[2527.32 --> 2529.44]  But I'm tempted by an iPhone.
[2529.54 --> 2534.72]  I must admit, you know, those cameras in particular, the camera on the Pixel 6 is good,
[2534.72 --> 2537.76]  but it's not earth-shatteringly good.
[2537.84 --> 2540.22]  Everybody else has caught up to what Google are doing, you know.
[2541.06 --> 2544.72]  Their de-blurring a face feature is just marketing.
[2545.04 --> 2549.16]  Their erase thing that they love to tout on the adverts is just that.
[2549.24 --> 2550.30]  It's just marketing as well.
[2550.48 --> 2554.24]  So, I mean, it's a perfectly fine device, but it's $700.
[2555.18 --> 2558.90]  And my 7T is just about as good, to be honest.
[2559.06 --> 2561.44]  So, I think I'm going to stick with that.
[2561.44 --> 2565.96]  Backblaze.com slash SSH.
[2566.06 --> 2569.62]  Get peace of mind knowing your files are backed up securely with Backblaze.
[2569.82 --> 2575.84]  You can get a free trial, no credit card required, by going to Backblaze.com slash SSH.
[2576.82 --> 2581.14]  Unlimited backup for your Mac or your PC for just $7 a month.
[2581.22 --> 2584.22]  Your documents, your music, your photos, your videos, your drawings, your projects.
[2584.74 --> 2591.08]  All of your data on your PC, backed up to the cloud, and restored anywhere you want.
[2591.08 --> 2596.14]  I mean, you could just directly download them back to your machine or restore them via the app.
[2596.20 --> 2600.72]  Or if it's a lot of data, heaven forbid, you need to restore like a lot of data.
[2601.72 --> 2604.70]  Backblaze will work with you to restore by mail as well.
[2605.04 --> 2606.08]  It's a neat system.
[2606.96 --> 2611.66]  And, you know, the nice thing about the mobile apps is that even when you're out on the go,
[2611.82 --> 2616.92]  if you really need to get something, you don't have to expose your network to remote access or something like that.
[2617.22 --> 2620.12]  You can log into that Backblaze app and grab the file there.
[2621.08 --> 2621.84]  That's really nice.
[2622.88 --> 2627.68]  And these kinds of reasons are why 50 billion files have been restored for Backblaze customers.
[2627.82 --> 2629.40]  I mean, you guys know it's Backblaze.
[2629.70 --> 2630.74]  It's Backblaze.
[2630.86 --> 2638.76]  And now you can get a fully featured, no credit card required trial and support the show by going to Backblaze.com slash SSH.
[2639.28 --> 2641.86]  Go there so that way they know you heard about it here on the show.
[2641.96 --> 2643.00]  And that way you can support the show.
[2643.08 --> 2644.78]  But you get that 15-day free trial too.
[2644.78 --> 2649.62]  You go there, play with it, start protecting your data, and start backing up today.
[2650.68 --> 2660.66]  Backblaze started 14 years ago as a bold idea to create a business that was fair and good for its customers, its partners, its employees, and of course your data, and now the greater community.
[2660.66 --> 2667.26]  And I love how they've contributed over the years with not only their drive reports, which we've cited on the air lots of times.
[2667.78 --> 2673.76]  They've got their storage pods, over 500,000 customers in 175 countries.
[2674.56 --> 2675.42]  It's Backblaze.
[2675.42 --> 2677.98]  And you can try it out 15 days for free.
[2678.26 --> 2682.72]  And then it's only $7 a month after that for unlimited backup for your Mac and your PC.
[2683.62 --> 2685.76]  Backblaze.com slash SSH.
[2687.78 --> 2694.58]  Now, if you have any thoughts on whether Chris and I should talk a little bit more about the world of technology and the art of smart...
[2694.58 --> 2695.52]  No, wait, that's the wrong show.
[2696.44 --> 2698.08]  You should talk about this stuff a bit more.
[2698.20 --> 2700.66]  Do let us know at selfhosted.show slash contact.
[2700.88 --> 2702.46]  And, you know, we'd love to hear from you.
[2702.46 --> 2707.32]  Speaking of which, we have a bit of feedback about Home Assistant.
[2707.90 --> 2709.52]  Yeah, listener Chris writes in.
[2709.58 --> 2711.30]  He says, hello, Chris and the Badger.
[2711.94 --> 2717.30]  Home Assistant hit a milestone recently with 100,000 users participating in their analytics.
[2718.12 --> 2721.72]  This is a great way for users to contribute to the project and help shape the development.
[2722.20 --> 2725.04]  And the best part is it's an opt-in implementation.
[2725.42 --> 2731.30]  The downside to an opt-in is that it can get overlooked by some users who maybe wouldn't mind contributing.
[2731.30 --> 2739.78]  So I thought maybe a shout-out to this feature and its location in the UI would be an excellent way for the self-hosted community to give back to an incredible project.
[2740.20 --> 2742.60]  Thanks for all you do and happy hosting.
[2742.60 --> 2751.28]  If you go into Home Assistant, and this can just be Home Assistant Core, and you go into Configuration, and then in the Configuration screen, you go to General.
[2751.74 --> 2755.42]  And then in General, at the bottom of that, there's an Analytics section.
[2755.42 --> 2761.42]  And I have opted on my systems to check all those boxes and hit save.
[2761.64 --> 2763.64]  I trust the Nebukasa guys.
[2763.72 --> 2764.90]  I also pay for the service.
[2765.24 --> 2771.16]  And I want them to know that I'm running this thing on a Pi, and I'm running on an x86 box, and I'm not always using their OS.
[2771.32 --> 2775.06]  I actually want it to represent my usage, and I feel like that's the best way for me to do it.
[2776.06 --> 2779.90]  Brandon writes in with some feedback about Frigate from a couple of episodes ago.
[2779.90 --> 2782.74]  Hey guys, I just listened to episode 56.
[2783.00 --> 2784.10]  I really enjoyed the show.
[2784.28 --> 2787.32]  I've been using Frigate for a while now, and I think it's pretty great.
[2787.70 --> 2790.34]  I have not upgraded to 0.9 yet.
[2790.50 --> 2793.48]  I'm still on the version of 0.8.
[2794.22 --> 2800.58]  I'm contacting you guys because one thing Frigate's very good for is improving a camera system that you might already have.
[2801.10 --> 2804.00]  As Chris mentioned, Frigate just needs an RTSP feed.
[2804.00 --> 2812.72]  And I had a Lorex Dahua, I hope I said that right, camera system set up on my network with a standalone NVR.
[2813.62 --> 2815.80]  Frigate's integration with Home Assistant is pretty great.
[2815.94 --> 2819.50]  I've got a WISE camera in the basement which detects if the kids are playing down there.
[2820.22 --> 2824.00]  If they leave and don't turn the lights off, brackets, they never do,
[2824.46 --> 2828.28]  then it will turn the lights off after 10 minutes of not recognising any people.
[2828.90 --> 2829.72]  That's nice.
[2829.72 --> 2834.92]  When an object is detected, I get a snapshot and a notification through Home Assistant.
[2835.58 --> 2838.70]  One thing I'm curious about is updating the models in Frigate, though.
[2838.78 --> 2846.26]  I'd love to have a custom model that could detect our two vehicles versus, say, a DoorDash delivery vehicle or a UPS truck.
[2847.00 --> 2849.24]  Wow, that's a great idea.
[2849.70 --> 2850.94]  Have you seen anything about that?
[2851.24 --> 2853.38]  I wonder if that's possible right now.
[2853.98 --> 2856.48]  Well, we might have something in this space.
[2856.48 --> 2865.84]  We're planning fairly soon a site reliability engineers only live stream with Chris and I to hang out with the supporters and patrons of the show.
[2866.40 --> 2871.62]  And I've been doing some background sleuthing with the author of an app called Double Take.
[2872.10 --> 2876.88]  And essentially what this does is it's facial recognition for Home Assistant.
[2876.88 --> 2881.08]  So it will sort of plug into DeepStack and Frigate and Double Take.
[2881.18 --> 2889.66]  It's all this kind of machine object detection learning type melange of stuff that all sort of kind of works together.
[2890.02 --> 2894.62]  I could see adding a vehicle detection model in one of these programs being quite viable.
[2894.74 --> 2898.50]  And perhaps we'll pick the Double Take author's brain on that on that live stream.
[2898.50 --> 2898.94]  Interesting.
[2900.48 --> 2901.38]  I look forward to that.
[2901.38 --> 2908.22]  I could see, like, the next thing I might want, right, is detecting Levi versus any other animal.
[2908.76 --> 2909.92]  Don't worry about Levi.
[2910.18 --> 2911.98]  Dog, not hot dog, right?
[2912.28 --> 2912.72]  Right.
[2914.06 --> 2914.70]  All right.
[2915.10 --> 2916.62]  This will probably be our last one today.
[2916.74 --> 2918.98]  IA writes in with some network jargon questions.
[2919.16 --> 2919.44]  He says,
[2919.44 --> 2923.82]  I recently graduated and discovered this podcast a few days ago.
[2923.98 --> 2932.34]  So since I've been listening, I've heard the term doubly natted and the term punching a hole through a firewall on the podcast at least a couple of times.
[2932.56 --> 2934.54]  I think TeamViewer was cited as an example.
[2934.76 --> 2937.98]  I'm wondering if you could explain what this is in a bit of detail.
[2938.38 --> 2942.50]  I'd like to know about ways to overcome DoubleNet and the pros and cons of that.
[2942.68 --> 2944.52]  You mentioned Wireguards and VPNs.
[2944.80 --> 2945.88]  Maybe they fit into this picture.
[2946.14 --> 2946.48]  Thanks.
[2946.48 --> 2950.92]  Well, Mr. Carrier Grade, Nat, why don't you start by explaining that one?
[2951.12 --> 2952.84]  I thought you were giving me a hard time.
[2953.36 --> 2953.78]  Right.
[2954.08 --> 2963.98]  So what has just unfortunately become way more common than we'd like is a situation where you have somebody that runs a private network.
[2964.44 --> 2969.68]  So a private network is generally a way of saying a network that doesn't route outside itself.
[2970.34 --> 2972.96]  So if you're on that network, you're not routing.
[2973.32 --> 2974.48]  You're not publicly available.
[2974.64 --> 2976.10]  People can't find you on the internet.
[2976.10 --> 2977.26]  You're a private network.
[2977.26 --> 2982.66]  The most typical example of that would be, say, like an intranet at a school or even just your LAN at home.
[2983.26 --> 2983.44]  Right.
[2983.56 --> 2985.12]  Those are all private networks.
[2985.12 --> 2992.34]  Now imagine that private network set up a network for another set of machines.
[2992.34 --> 2994.78]  And it was essentially networkception.
[2995.48 --> 2997.62]  And it was also a private network.
[2997.78 --> 3002.86]  So you have a private network that is connected to a private network that is then connected to the public internet.
[3002.86 --> 3011.24]  And that, in a really loose way, is what double-nated is, is you were behind two network address translated networks.
[3011.24 --> 3015.54]  You can actually set this up for yourself if you're curious to kind of play around with it.
[3016.02 --> 3020.44]  Spin up OpenSense or PFSense in a VM behind your existing router.
[3021.14 --> 3025.66]  And that would create a network within a network, which is essentially what Chris is talking about here.
[3025.66 --> 3030.32]  So he has a wireless ISP that's, you know, got a mast up on a hill somewhere.
[3030.54 --> 3033.18]  And that thing has a router behind it.
[3033.50 --> 3036.84]  So that router has a public-facing IP address.
[3037.18 --> 3041.26]  Now you know that there are only a certain number of IPv4 addresses available.
[3041.80 --> 3044.80]  They're expensive as a consequence, relatively speaking.
[3044.80 --> 3048.82]  And so what a lot of these wireless ISP guys do is to save a bit of money.
[3049.60 --> 3059.66]  They will just give you a private IP and essentially translate your local devices on your local network in Chris's RV, for example.
[3060.78 --> 3065.14]  They won't know, you know, everything he's got behind their little router that they've given him.
[3065.68 --> 3070.72]  But his router will have an IP address on their network, not the public internet.
[3070.72 --> 3070.90]  Yeah.
[3071.36 --> 3081.22]  And because of this, software like VPNs or other types of software that want to, quote unquote, punch a hole through a firewall,
[3081.52 --> 3086.96]  they can't just open up a port on the firewall through something like Universal Plug and Play and start receiving connections.
[3086.96 --> 3095.00]  Because even if they open up a port on that firewall, there's just a private network on the other side of that that can't talk to the internet.
[3095.00 --> 3105.34]  And so when you're double-natted, you need something that is sort of like a proxy between whatever is on the private network and whatever is on the public network.
[3105.64 --> 3109.64]  And that's usually what you hear us talking about ways around double-natting or something like that.
[3109.64 --> 3117.20]  And really what it just means is that if you want to host something on a double-natted network, you're going to have to work to make it happen.
[3117.32 --> 3119.80]  And it's not going to be the most efficient way to do it.
[3120.46 --> 3128.88]  And they probably don't want you doing it because another place you'll often see this is on cell networks and mobile networks and some satellite internet.
[3129.28 --> 3132.86]  And so they probably don't want you hosting anything either.
[3132.98 --> 3133.66]  That's very common.
[3133.72 --> 3137.16]  And that's where something like our sponsor, Linode, could be useful.
[3137.16 --> 3150.24]  Yeah, and this is one of the reasons why I found Tailscale so useful is they host a lighthouse, a third-party kind of witness node somewhere that does all that natraversal stuff for you.
[3150.58 --> 3154.20]  So then you end up with a peer-to-peer connection to the remote host.
[3154.32 --> 3163.52]  And I'm very pleased to say that I've been using Tailscale now for, what, a couple of months and doing all my backups to England on my Synology box over Tailscale.
[3163.80 --> 3165.50]  And it's just working.
[3165.50 --> 3167.12]  I really like it too.
[3167.16 --> 3167.40]  Yeah.
[3167.78 --> 3169.40]  Higher phrase you cannot find.
[3169.50 --> 3170.18]  It just works.
[3170.48 --> 3174.40]  It is so simple to get up and get going and have a mesh network.
[3175.24 --> 3184.80]  The only thing about Tailscale that I'm not a huge fan of is you are placing a lot of trust in them because they are doing the key exchange and managing all of that stuff for you.
[3184.80 --> 3194.56]  And if you want something like Tailscale but you want full control and you want to be completely trustworthy setup, I still think Nebula is better in that regard.
[3194.56 --> 3199.38]  Especially in a server-to-server-to-server scenario, I might be more comfortable with Nebula.
[3199.74 --> 3203.54]  But if it's like phone workstation server, that might be where I are.
[3203.80 --> 3206.44]  Or workstation, workstation, workstation among friends.
[3206.60 --> 3207.68]  I'd probably go Tailscale.
[3207.68 --> 3212.90]  But when it's server-server-server, I might be more inclined to go Nebula just because you have complete control.
[3213.10 --> 3217.00]  It is also exceedingly good at punching through double nat.
[3217.46 --> 3221.32]  And you have complete control over the keys in that scenario.
[3221.32 --> 3223.48]  You know what I'd equate that to?
[3223.84 --> 3225.36]  Tailscale is a bit like Plex.
[3225.78 --> 3231.08]  Like I'm not totally 100% on board with what they're doing, but it's very slick.
[3231.66 --> 3233.26]  And Nebula is kind of like Cody.
[3233.68 --> 3234.16]  Jellyfin.
[3234.48 --> 3235.06]  Nice, Jellyfin.
[3235.06 --> 3235.64]  Or Jellyfin.
[3235.88 --> 3236.84]  Jellyfin, you know what?
[3236.88 --> 3242.04]  I didn't say it during the compute module review, or at least first look.
[3242.72 --> 3247.48]  But Jellyfin, in a way, is a lot more appealing now.
[3247.48 --> 3251.78]  Because, you know, Plex has added a lot of stuff, and Jellyfin remains kind of lean and mean.
[3252.42 --> 3259.30]  And it has a pretty good metadata manager, and it will write the information to the folders and NFO files.
[3259.68 --> 3264.14]  And it'll go through and scan for chapter images so you can get chapters for all your stuff.
[3264.70 --> 3265.10]  That's fine.
[3265.24 --> 3265.70]  That's fine.
[3265.80 --> 3266.88]  How are the clients?
[3267.48 --> 3268.66]  Yeah, you're right.
[3268.86 --> 3269.70]  That's the problem.
[3269.90 --> 3270.36]  You see what I mean?
[3270.50 --> 3272.26]  Like Tailscale has that figured out.
[3272.36 --> 3275.96]  They have all the clients for iOS, for Android, for everything.
[3275.96 --> 3278.04]  Whereas Nebula, you're on your own.
[3278.78 --> 3279.74]  That's kind of what I mean.
[3280.34 --> 3281.52]  Yeah, it is a similar.
[3282.26 --> 3284.58]  And I think there is a place for both of them.
[3284.90 --> 3287.72]  But when you want simplicity and ease of use, Tailscale wins.
[3287.80 --> 3288.06]  You're right.
[3288.28 --> 3288.76]  It is that.
[3289.36 --> 3289.50]  Yeah.
[3289.76 --> 3291.36]  They should totally sponsor.
[3291.58 --> 3296.50]  If anybody at Tailscale is listening, hook us up with a deal, and we'll start getting people signed up.
[3296.86 --> 3298.42]  We're all pretty happy users here.
[3299.42 --> 3300.58]  You know we like some of them.
[3300.60 --> 3301.88]  We start asking them to sponsor us.
[3301.90 --> 3303.92]  And by that point, we've already given away the milk.
[3303.92 --> 3312.62]  We'd love to hear your feedback, your ideas, your projects you're working on, things you're using a compute module for.
[3313.08 --> 3313.94]  Let me know.
[3314.14 --> 3314.82]  Let us all know.
[3315.12 --> 3316.56]  Selfhost.show slash contact.
[3317.20 --> 3320.84]  And also, find our sponsor, A Cloud Guru, on social media.
[3321.26 --> 3325.40]  They're just slash A Cloud Guru at anything that's like a social media platform.
[3325.70 --> 3325.94]  You know?
[3326.16 --> 3328.62]  Like the YouTubes, the Facebooks, the Twitters, slash A Cloud Guru.
[3328.62 --> 3341.24]  Now, you heard me mention it a little bit earlier in the show, but for our site reliability engineers at selfhosted.show slash SRE, we're going to be doing a secret super special live stream over the next few weeks.
[3341.42 --> 3346.44]  Chris and I, we're going to hang out with you guys, and we'll just have like a video call where we can all talk.
[3346.52 --> 3350.40]  But we have a few special guests on the show as well at that point.
[3350.40 --> 3354.40]  And it'll be basically like a pseudo episode, I guess, except you're part of it.
[3354.90 --> 3356.28]  Like a hypervised episode.
[3356.42 --> 3358.88]  It's not like a, it's not a, or a para-virtualized episode.
[3359.02 --> 3359.64]  That's what it is.
[3359.86 --> 3364.80]  I just wanted to say, too, I also, I bought a new microphone for it, because I'm going to do it up from my office, I think.
[3365.26 --> 3366.76]  And so I needed a microphone in my office.
[3366.82 --> 3371.52]  I'm going to be trying out a brand new microphone for these, for this, for this whole live stream stuff.
[3371.86 --> 3373.56]  Selfhost.show slash SRE.
[3373.56 --> 3376.58]  And don't forget, you'll also get the post-show every episode.
[3377.34 --> 3381.68]  So, you know, by now, selfhosted.show slash contact is the place to go to get in touch with us.
[3381.86 --> 3384.00]  You can find me on Twitter at Ironic Badger.
[3384.44 --> 3387.62]  I'm over there at Chris Ellis, and the show is at selfhosted.show.
[3388.12 --> 3390.16]  Don't forget the network at Jupiter Signal.
[3390.46 --> 3391.52]  And thanks for listening, everyone.
[3391.86 --> 3394.16]  That was selfhosted.show slash 58.
