[0.00 --> 5.60]  A dream of mine came true yesterday. We had a mini split installed in the garage.
[6.26 --> 7.72]  Air conditioning and heating?
[8.20 --> 11.70]  Hot and cold running air in the garage, yes.
[11.82 --> 15.90]  That's so fancy. I feel fancy when I put a space heater out in the garage.
[16.68 --> 22.08]  Yeah, you know, the temperatures in Raleigh the last couple of weeks, it was 2 or 3 Celsius one week,
[22.12 --> 25.46]  and then it was 20 Celsius the next week, and then back down to 2 or 3 again.
[25.46 --> 30.76]  And I just got tired of it being either too hot or too cold or too muggy.
[30.98 --> 34.06]  And, you know, we've got a window unit in there and all the rest of it,
[34.18 --> 38.90]  but we had a crew come out and split the upstairs HVAC system into two.
[39.00 --> 41.72]  So the room above the garage is where I record all these shows.
[41.98 --> 43.44]  We call that a bonus room in America.
[44.54 --> 49.20]  And this room was always too hot or too cold compared to the rest of the upstairs
[49.20 --> 52.08]  because it wasn't as insulated as well and all that kind of stuff.
[52.44 --> 55.08]  So our upstairs system is split into two.
[55.46 --> 61.70]  So I bought an Ecobee for this room and paired that up with Home Assistant using HomeKit.
[62.10 --> 63.80]  It was totally uneventful.
[63.96 --> 67.70]  I was hoping for some content out of it, but honestly, the fact it just works is,
[68.60 --> 70.06]  as a content man, it's kind of boring.
[70.82 --> 76.46]  And so now your Home Assistant system is using HomeKit to communicate with the Ecobee?
[76.66 --> 76.98]  Yeah.
[77.26 --> 77.76]  All locally?
[77.76 --> 85.54]  I nearly didn't buy the Ecobee because I was under the misconception that they are a cloud-based integration.
[85.70 --> 89.64]  Now, there is a cloud-based integration that you can use with an Ecobee,
[89.96 --> 93.76]  but also the Ecobee support HomeKit.
[93.98 --> 99.88]  And if you're running Home Assistant, you can talk locally to the smart thermostat over HomeKit protocol.
[99.88 --> 101.88]  And it's all local.
[102.06 --> 106.64]  I have not actually signed this particular thermostat into any cloud account whatsoever.
[106.80 --> 109.12]  I had to connect it to my Wi-Fi, but that was it.
[109.78 --> 110.68]  That is so great.
[110.76 --> 116.62]  Now are you going to start playing around with automations for cooling and not cooling when you're not there and that kind of stuff?
[116.68 --> 118.00]  Or are you just going to leave it kind of vanilla?
[118.00 --> 120.34]  I mean, I've got an Everything Presence 1 on the way.
[120.96 --> 122.38]  I don't know when that's going to show up.
[122.44 --> 123.38]  I did it a couple of weeks ago.
[123.56 --> 129.02]  So when that arrives, I will have a millimeter wave at this desk or pointed at the sofa or something,
[129.24 --> 134.36]  because this is our lounge slash my Tinker office drum room.
[135.10 --> 140.78]  But yeah, it means I've now got two extra zones to worry about from a climate perspective in Home Assistant.
[140.94 --> 142.50]  So we've got the main upstairs.
[142.70 --> 146.68]  We've got all of downstairs, because they're on two completely separate four-stair systems.
[146.68 --> 152.54]  And then the bonus room is splitting the top half of the house in half.
[152.66 --> 158.42]  And it's got this kind of like valve system in the attic now that turns a baffle in the ducting on or off,
[158.48 --> 160.86]  depending on which zone is calling for heat.
[161.02 --> 161.50]  It's cool.
[162.78 --> 168.30]  But the one I don't quite fully have an answer for yet is the mini split in the garage.
[168.46 --> 175.50]  That is a infrared-based, you know, you point a little remote control at the unit on the wall.
[175.50 --> 181.66]  It bleeps and says, right, you're going to set this to 70 Fahrenheit, so about 20 Celsius-ish.
[182.68 --> 183.98]  And that's it.
[184.44 --> 190.80]  Now, I did a bit of research, and it turns out that these Mitsubishi units have a, I think it's a CN105 port.
[190.80 --> 197.92]  And some people have reverse-engineered it, of course, and made it so you can control these things using an ESP device.
[198.66 --> 204.60]  So you can basically retrofit Wi-Fi control through Home Assistant and ESPHome into these devices.
[204.60 --> 211.16]  But I'm a little nervous about pulling apart a brand new several thousand dollar air conditioning unit.
[211.32 --> 217.02]  So if you're in the Raleigh area and would love to come and help me pull this thing apart, I would appreciate the help, honestly.
[217.12 --> 223.10]  Or if you've done anything similar, step-by-step instructions or, you know, walking me through it on a video call, I would love that.
[223.10 --> 224.30]  I know your feel.
[224.82 --> 228.26]  You know, I got these new, they're called Max Air fans in the RV.
[228.44 --> 230.26]  Brand new, wonderful fans.
[231.10 --> 235.52]  But they're those, not capacitive, but it's like a plastic laminate.
[235.52 --> 241.34]  And there's like a button underneath and you push through the plastic and then it triggers the button and then it beeps.
[241.38 --> 245.16]  And you can step the motor up or step the motor down or put it in reverse mode.
[245.80 --> 247.68]  And it just screams for going in Home Assistant.
[247.82 --> 252.66]  It screams for it because they're up high on the roof, which is kind of difficult for my wife to reach.
[253.36 --> 256.16]  And, of course, you want to be able to schedule them and automate them and whatnot.
[256.42 --> 257.40]  So I know what you mean.
[257.40 --> 262.86]  But at the same time, I was like, well, I just spent combined nearly a grand for these fans.
[263.00 --> 265.30]  I don't really want to tear them apart right away.
[265.76 --> 271.34]  Maybe in a year when I'm like doing service on them and I have them taken apart, maybe then I'll do it.
[271.40 --> 272.04]  I'm not sure.
[272.72 --> 277.00]  But if, you know, again, if somebody has done this and has steps, I would try it.
[277.64 --> 282.54]  It reminds me how spoiled I am with having everything just in one single app.
[282.54 --> 288.50]  Not, you know, not juggling the Ecobee app and the Venstar app and the Mitsubishi doesn't have an app.
[288.60 --> 290.22]  But if it did, you know what I mean?
[290.34 --> 294.46]  Like it just reminds you why you put all the effort into something like Home Assistant now.
[294.46 --> 294.76]  Yeah.
[295.12 --> 295.40]  Yeah.
[295.96 --> 302.64]  I have felt that way, you know, forever is one of the ways I kind of begin to explain it is it's sort of like the universal unifier app.
[302.88 --> 304.50]  You know, bring all your vendors in one spot.
[304.72 --> 308.44]  And Zigbee and Z-Wave are great for that.
[308.52 --> 310.00]  You know, a lot of that stuff just works.
[310.00 --> 318.42]  I just recently installed a sensor that I'm going to give the stamp of approval for the in the fridge or in the freezer sensor.
[318.74 --> 321.06]  Can we get a sound effect for the stamp of approval, please?
[321.60 --> 321.84]  Editor.
[321.84 --> 326.52]  It's funny, too, because right now it's the holidays.
[326.52 --> 335.58]  So on Amazon, the product description is, quote, keep prying eyes out of Santa's closet with a Zigbee door window sensor.
[336.62 --> 346.18]  It's it's it's really just a standard magnet sensor, but it's got a good magnet in there with a really approachable way to replace the battery that just has a little slide out.
[346.28 --> 349.76]  One of those little sort of coin batteries, one of the thicker ones just pops right out.
[349.76 --> 350.58]  But you can put it in there.
[351.04 --> 353.70]  And I had a listener tell me theirs has been lasting a year.
[354.22 --> 357.54]  Amazon has it for 19 percent off right now as we record.
[357.78 --> 359.00]  I'll put a link in the show notes.
[359.08 --> 361.00]  It's twenty five dollars U.S.
[361.36 --> 370.98]  And I all I did is I put the magnet part on the door that opens and I put the sensor brick inside the fridge.
[371.24 --> 376.72]  And the brilliant thing about it, and this is what sold me on it, is it also has a temperature sensor.
[376.72 --> 391.32]  So not only does it stay functional inside the fridge and remains connected inside your apparently nuke proof fridge, if I'm supposed to believe the movies, but it also acts as a very frequently updated temperature sensor.
[391.60 --> 395.46]  So I can really hone the temperature of my fridge in and I can see immediately the results.
[395.70 --> 399.88]  So I'm giving it the good old Chris stamp of approval if you want a sensor in your fridge.
[399.94 --> 403.66]  And I I recommend it because it's a good way to keep an eye on how your fridge is doing.
[403.66 --> 406.68]  Yeah, it's funny. We had a talking of the garage.
[406.82 --> 409.56]  We had a we have a freezer in there had.
[409.92 --> 412.68]  And on Black Friday, we picked up a new fridge freezer combo.
[412.96 --> 418.20]  And I the reason I knew that the freezer was dying was because of my Aqara temperature sensor that I have in the freezer.
[418.52 --> 428.64]  And I could see that over the summer it was frequently struggling to stay below zero Celsius, which obviously for a freezer, it's pretty terminal.
[428.64 --> 432.44]  So I think anyone in a van or an RV should have one of these.
[432.56 --> 432.74]  Yeah.
[432.78 --> 437.04]  Because you don't think about it, but you travel and you go somewhere where the ambient temperature is quite a bit different.
[437.46 --> 438.66]  Your fridge needs to be adjusted.
[439.70 --> 442.94]  And if you go somewhere where it's hot, you got to turn that fridge up and vice versa.
[443.12 --> 444.04]  One other thing I got.
[444.46 --> 447.70]  So that was a Zigbee sensor on the Z-Wave side of accessories.
[447.70 --> 454.28]  I picked up another set of these Zeus 700 series water leak sensors.
[454.60 --> 455.38]  They're tiny.
[455.88 --> 458.66]  They're about the size of a quarter and just a little bit longer.
[459.84 --> 462.44]  I've had three of them for over a year already.
[462.56 --> 463.70]  They've never lost connection.
[463.86 --> 464.74]  They're all still kicking.
[465.66 --> 466.64]  I've just lost them.
[466.94 --> 468.20]  Unfortunately, I lost a couple of them.
[468.36 --> 469.02]  That's another story.
[469.44 --> 470.02]  But they're great.
[470.34 --> 472.70]  I have read that if they get really soaked, they get destroyed.
[473.12 --> 474.04]  That's fine by me.
[474.08 --> 475.06]  They're like 25 bucks.
[475.06 --> 477.76]  You should stick an air tag on your water leak sensor.
[480.04 --> 484.34]  But just really simple, solid, and not bulky, you guys.
[484.48 --> 487.96]  I was surprised how many of these water leak sensors are very bulky.
[488.52 --> 490.10]  This has four points of contact.
[490.24 --> 491.72]  You put it down on the ground or wherever.
[492.58 --> 496.06]  There are other ones that have more sophisticated sensors, but I really like this one.
[496.12 --> 497.14]  And it's cheap.
[497.50 --> 502.44]  And I'm giving it, again, the stamp of approval because I've had these in production for over a year and I just bought another batch.
[503.20 --> 503.74]  I'm liking it.
[503.90 --> 504.64]  What about you?
[504.64 --> 507.16]  You got any new hardware that you're giving the stamp of approval to these days?
[507.50 --> 507.70]  Yeah.
[507.74 --> 514.44]  If you're paying attention on my YouTube channel, I just did a video about the framework that arrived on my doorstep this week.
[514.68 --> 515.52]  Ooh, new laptop.
[515.80 --> 516.06]  Yeah.
[516.16 --> 520.08]  I got one of the Ryzen frameworks, one of the Ryzen, and it's pretty nice.
[520.38 --> 523.64]  It's sort of all metal feeling construction.
[523.64 --> 525.64]  It's like a DIY MacBook.
[526.06 --> 534.76]  If the MacBook wasn't proprietary and didn't respect your freedoms in all those kind of ways, this is the equivalent.
[534.76 --> 537.16]  So far, I've been pretty impressed.
[537.16 --> 544.72]  I put Fedora on it to start with after the initial build, which was really only half an hour at tops because I was filming.
[544.96 --> 546.70]  You know, it would have been 10 minutes if I wasn't filming.
[546.70 --> 551.46]  And then after I'd done Fedora, I thought, right, it's time to do it properly.
[551.62 --> 554.16]  And I wiped it and I put Nix OS on that bad boy.
[554.50 --> 554.70]  Ah.
[555.28 --> 556.70]  I imagine that's probably running great.
[556.94 --> 557.72]  It's running pretty well.
[557.90 --> 558.10]  Yeah.
[558.10 --> 562.20]  The fan noise is a bit of an issue.
[562.38 --> 571.20]  So when I'm just browsing the web or something or, you know, just, you know, Telegram or just boring terminal stuff, it's totally fine.
[571.74 --> 573.34]  Normal usage is total fine.
[573.48 --> 576.84]  Like I can sit with it on a pillow, on the sofa, on my lap, and it's fine.
[577.30 --> 583.74]  But the minute I do like a Nix OS rebuild switch where it might have to compile something like a GTK library or something like that,
[583.74 --> 594.70]  the fans, you can hear them, and it reminds me just how impressive the Apple Silicon situation is with regards to how they dissipate heat and things like that.
[594.82 --> 598.20]  So, you know, overall, I've got nothing to really knock this thing about.
[598.62 --> 604.90]  Maybe the removal of their little dongles that go into the ports is a bit too difficult.
[605.10 --> 606.04]  They're a bit too stiff.
[606.20 --> 607.72]  Like the tolerances are a bit too tight.
[607.86 --> 610.40]  But I'm really splitting hairs with that.
[610.40 --> 615.98]  It's everything I want in a thin and light Linux laptop.
[616.14 --> 617.84]  The battery life has been great.
[618.04 --> 620.64]  Plenty of computing power to run virtual machines.
[620.84 --> 626.68]  Like I was just at the racetrack this weekend and I needed to do something with my VCDS cable to connect into my Golf.
[627.20 --> 633.86]  I had a Windows VM on the framework, spanned that up, did a USB redirect for the USB OBD2 cable,
[634.50 --> 639.44]  flashed some brake parameter that someone in the paddock told me was good to go and it actually worked a treat.
[640.40 --> 645.28]  And so, yeah, I don't need to take two laptops to the track anymore.
[645.40 --> 651.68]  I was taking an old ThinkPad running Windows and my MacBook Pro because it didn't have a USB-A port for the VCDS cable.
[651.80 --> 653.72]  And I'm like, well, I don't want to have to take a dongle.
[654.86 --> 657.58]  Because the framework, I can put whatever ports I want in it.
[658.14 --> 660.02]  It just works perfectly for my use case.
[660.02 --> 667.64]  Do you think there will be third-party fans or something you could install into that thing to make it quieter,
[667.80 --> 670.20]  maybe with better acoustics of some type?
[670.26 --> 671.42]  I don't know if it's even possible, but...
[671.98 --> 673.28]  I think it's just a matter of physics.
[673.52 --> 679.12]  Like if you feel the chassis, before you hear the fans, you feel the heat spreading.
[679.12 --> 685.80]  You remember in laptops of old, I say this having been an Apple wanker for the last few years,
[686.90 --> 690.28]  you know, you feel the heat spreading under your fingers on the keyboard and you're like,
[690.40 --> 691.18]  oh, here we go.
[691.48 --> 695.28]  And then sure enough, a minute or two later, up go the fans.
[695.64 --> 698.28]  So, you know, that Ryzen CPU is no joke.
[698.36 --> 701.50]  I mean, it's DDR5-based memory, NVMe SSD.
[701.50 --> 705.54]  So the performance of this thing is really good, honestly.
[705.78 --> 710.26]  It's by far and away the fastest Linux desktop experience I've had on a laptop.
[711.12 --> 716.44]  But yeah, I think they're just, you know, up against it with the architectural decisions of x86
[716.44 --> 721.40]  and all the history and all good and bad that comes with that.
[722.40 --> 725.48]  I wonder, and perhaps this is something that listeners could reach out,
[726.36 --> 729.52]  I wonder if taking the Jeff approach here might work,
[729.52 --> 731.12]  depending on what you want to use the machine for.
[731.50 --> 735.20]  And what kind of performance, it does sort of stink to get a brand new machine
[735.20 --> 736.44]  and have really crappy performance.
[736.70 --> 739.32]  But one of the things you can do with those AMD systems
[739.32 --> 743.80]  is you can kind of really lock in and say, hey, don't go above this wattage.
[743.90 --> 745.02]  Don't go above this.
[745.06 --> 747.04]  And you can kind of find the sweet spot for heat there.
[747.36 --> 748.94]  And you could say, say it's 15 watts.
[749.02 --> 749.70]  Don't go above whatever.
[749.86 --> 750.94]  I'm making that number up.
[751.06 --> 752.20]  Don't go above 15 watts.
[752.28 --> 753.78]  Don't go above 10 watts, whatever it is.
[754.36 --> 757.82]  And yeah, you would be governing your performance,
[757.82 --> 762.78]  but you would be sort of also preventing the CPU and chipsets from getting hot enough
[762.78 --> 764.14]  that the fan needs to kick in.
[764.40 --> 766.42]  And it also would extend battery life, of course.
[766.76 --> 769.72]  There probably is a way to do that if it's something you'd be interested in.
[770.04 --> 770.92]  I'll have to give that a go.
[771.02 --> 772.46]  I am definitely interested in that.
[772.98 --> 775.56]  You know, just having this laptop to replace that.
[775.56 --> 777.82]  I had a T480S before this.
[779.00 --> 779.72]  Dual core.
[780.14 --> 781.20]  It was plastic.
[781.52 --> 783.08]  It was a bad keyboard.
[783.30 --> 783.98]  Keyboard's nice.
[784.56 --> 785.84]  I know it's important to some people.
[786.86 --> 788.20]  Objectively, the keyboard's really nice.
[788.28 --> 789.80]  The trackpad is really good, too.
[790.12 --> 794.12]  Like, it's, yeah, I wouldn't say it's quite MacBook good, but it's pretty close.
[795.30 --> 796.30]  Okay, well, let me ask you this, then.
[797.82 --> 800.66]  Say, for whatever reason, in the future, you need to buy another PC laptop.
[801.08 --> 802.80]  Is this your go-to brand now, do you think?
[802.94 --> 803.16]  Yeah.
[803.16 --> 808.92]  Yeah, you know, this chassis, I am anticipating being with me for the next decade or so.
[809.14 --> 810.16]  I'll replace the motherboard.
[810.56 --> 813.56]  You know, obviously, if you're not aware, the reason I'm so excited about a framework
[813.56 --> 816.58]  is that you can upgrade the motherboard.
[817.48 --> 822.66]  So with that comes a longevity that laptops typically haven't had before.
[823.56 --> 826.78]  And so for me, I'm hoping that this chassis will be one that lasts for a decade.
[827.14 --> 830.00]  Maybe I'll upgrade the screen as technology improves.
[830.14 --> 831.56]  And I didn't talk about the screen.
[831.56 --> 833.48]  It's a 4x3 aspect ratio.
[833.82 --> 834.80]  Yeah, that seems nice.
[834.88 --> 837.16]  I'd really like a machine with 4x3 again.
[837.82 --> 841.42]  It reminds me of almost like War Games situation.
[841.66 --> 842.88]  I feel like I've gone back in time.
[843.00 --> 843.50]  And it's like...
[843.50 --> 843.78]  Retro.
[844.00 --> 844.16]  Yeah.
[844.22 --> 847.50]  When I went back to my MacBook, I was like, where's the height gone?
[847.74 --> 849.96]  I want a tall screen again.
[849.96 --> 856.78]  45Homelab.com.
[857.12 --> 859.38]  Premium storage servers for the Home Lab.
[859.52 --> 860.72]  They're finally here.
[860.78 --> 865.18]  If you're looking for an open Home Lab server that's strong, it's big, it's fast,
[865.28 --> 868.54]  and it doesn't compromise in any way on build quality,
[869.12 --> 872.02]  45 Home Lab, that's a new division from 45 Drives.
[872.02 --> 877.24]  They've taken their enterprise design and philosophy, and they've scaled it down to the Home Lab,
[877.64 --> 879.20]  and it is here.
[879.62 --> 884.84]  The HL15, the premium Home Lab storage server, it's beautifully designed, beautifully built.
[885.10 --> 887.02]  It's got 15 bays for TIS.
[887.48 --> 889.98]  I suppose that's where the 15 comes in the HL name.
[890.24 --> 893.24]  And it's designed and manufactured and assembled in North America.
[893.24 --> 898.58]  It's built with steel and with screws, not rivets, so you can take it apart if you need to.
[899.36 --> 901.04]  It may have multiple design options.
[901.64 --> 903.86]  So you can get it with a fully built, ready-to-go system.
[904.34 --> 907.90]  You can get just the chassis and the backplane, or probably the route I might go,
[908.30 --> 912.68]  the chassis, the backplane, and the PSU, and then you bring your own MOBO and CPU and memory and stuff.
[913.10 --> 914.18]  But however you like it.
[914.20 --> 916.04]  Perhaps you'd just rather have it come out of the box ready to go.
[916.10 --> 917.08]  They got that for you, too.
[917.32 --> 919.22]  So go to 45Homelab.com.
[919.22 --> 923.10]  This has been inspired and designed by the feedback from our self-hosted community.
[923.24 --> 927.54]  And now it is here as a product, and it is a sweet-looking rig.
[928.44 --> 929.78]  45Homelab.com.
[931.70 --> 934.04]  Well, in the last episode, we had ESP Corner.
[934.44 --> 936.92]  It was probably a sign that I was in tinker mode.
[937.26 --> 940.14]  So this week, we've got WLED Corner.
[940.62 --> 941.64]  Do-do-do-do.
[942.08 --> 942.70]  We have a theme tune.
[942.70 --> 944.22]  This is something we really should have had sooner.
[944.36 --> 946.08]  I mean, WLED is such a great project.
[946.88 --> 948.78]  It's really been underserved by our podcast.
[949.68 --> 950.34]  It has.
[950.42 --> 952.24]  I was really into it a few years ago.
[952.24 --> 954.78]  It was kind of one of my gateway drugs into Home Assistant.
[954.96 --> 964.72]  We did a self-hosted live hack where I flashed an ESP board on camera using the Arduino software and custom sketches and all that kind of stuff.
[964.98 --> 968.42]  And I thought, right, I've got this ESP just in a drawer right here.
[968.50 --> 970.66]  I haven't turned this on for like four years.
[970.66 --> 972.94]  I'm not even going to try and boot it up.
[973.36 --> 974.08]  Actually, no, I am.
[974.14 --> 975.56]  I'm going to try and boot it up.
[975.68 --> 976.14]  Plugged it in.
[976.60 --> 978.18]  Picked up the Wi-Fi instantly.
[979.02 --> 983.32]  It was still running the Arduino sketch, though, that I flashed four years ago.
[983.72 --> 986.08]  And so I thought, right, let's just put WLED on this.
[986.08 --> 997.40]  And I remember in the old days, you used to have to have a specific driver installed and then you used to have to press the boot button in the correct order and then hope it showed up and then fart around with drivers for like 20 minutes.
[997.72 --> 1000.24]  And you won't believe how easy it is these days.
[1000.24 --> 1001.78]  You can do it through the web now, Alex.
[1001.86 --> 1002.30]  Exactly.
[1002.66 --> 1003.62]  You open a browser.
[1004.66 --> 1012.00]  The WLED website walks you through the installation process and it brings it up in Chrome as a device that you select.
[1012.74 --> 1014.96]  You don't have to press boot buttons or anything like that.
[1015.06 --> 1016.90]  And it just flashes it to the device.
[1017.72 --> 1026.18]  And maybe one minute later, you've got a device booted that has started to broadcast a wireless access point, you know, SSID.
[1026.18 --> 1030.66]  You connect to that with your phone, type in your real Wi-Fi credentials.
[1031.04 --> 1031.28]  Boom.
[1031.46 --> 1031.80]  You're done.
[1032.66 --> 1032.78]  Yeah.
[1033.38 --> 1043.00]  So for those of you out there that aren't familiar, this is WLED is a very feature rich project that you can flash on to an ESP like Alex is just saying.
[1043.46 --> 1050.12]  You get a little web server and then it'll control those NeoPixel LED light strips you can get on Amazon for like nothing.
[1050.76 --> 1054.26]  And it's full of fun stuff and it's kind of great for the holidays.
[1054.26 --> 1056.96]  I'm using this to like light everything up green and red.
[1057.50 --> 1062.90]  Well, we're at the point where Ella can leave the bedroom by her own motive power.
[1063.00 --> 1063.96]  She can reach door handles.
[1064.18 --> 1068.86]  She has, you know, free thought as a three-year-old or nearly three anyway.
[1069.50 --> 1070.22]  There it goes.
[1070.38 --> 1070.72]  Yeah.
[1070.96 --> 1072.44]  It was good while it lasted.
[1073.10 --> 1078.68]  And so I thought I've heard of people that have nightlights that change colors almost a bit like a traffic light.
[1078.68 --> 1083.68]  Based on the time of day and, you know, different circumstances.
[1084.30 --> 1094.72]  And so I thought, wouldn't it be great if I just use some of these old five volt LEDs that I have sat in a drawer doing nothing and 3D printed her a little dinosaur, little dino nightlight.
[1094.72 --> 1097.50]  She loves this thing.
[1097.98 --> 1107.78]  And when it's nap time in the afternoon, I just put it into rainbow mode and I caught her on the camera the other day pointing at it going, rainbow dino, rainbow dino.
[1109.20 --> 1110.10]  That's adorable.
[1110.72 --> 1111.90]  Yeah, it really is.
[1111.90 --> 1117.18]  And then at bedtime, 7 p.m. or whenever, we have a button that we push on the wall outside.
[1117.80 --> 1124.16]  It turns the dino red, which we've told her means that when the dino's red, you stay in your bedroom.
[1124.30 --> 1128.54]  If you need a potty or anything like that, you know, that's allowed.
[1128.64 --> 1130.64]  You can leave the room for potty and stuff.
[1131.32 --> 1137.42]  And then at about 7 a.m., depending on where the sun is and stuff, we have it changed to green.
[1137.42 --> 1139.74]  And they say, right, when it's green, you're allowed out of your room.
[1139.74 --> 1142.86]  You can come wake us up if you need it, need to or anything like that.
[1143.50 --> 1145.62]  And then it turns off at 9 a.m. or something like that.
[1145.68 --> 1147.12]  And then nap time, there's a button.
[1147.66 --> 1151.22]  I'm using that four-way scene switcher that you recommended, by the way, for that.
[1151.84 --> 1152.12]  Oh, great.
[1152.54 --> 1154.74]  That is such a great use for WLED.
[1155.58 --> 1156.92]  Man, that's really clever.
[1157.26 --> 1163.84]  Just kind of, it's interesting how our family can kind of help build routines with automation.
[1164.42 --> 1165.96]  We do this with the kids, too.
[1165.96 --> 1171.86]  We have a bedtime routine that kind of winds down the whole house and starts up noisemakers.
[1172.16 --> 1175.52]  And it's just now, you know, years into it, it's just natural.
[1175.60 --> 1177.04]  When that stuff starts, okay, yeah, we're good.
[1177.12 --> 1178.18]  We'll go brush my teeth.
[1178.30 --> 1179.56]  I don't even have to say anything anymore.
[1181.16 --> 1183.24]  And WLED is a nice little part of that.
[1183.36 --> 1186.50]  It's such a, we'll put a link to your Mastodon post.
[1186.58 --> 1187.34]  It's really adorable.
[1187.88 --> 1189.60]  It's such a great idea.
[1189.70 --> 1191.98]  Some dads out there should totally nab that.
[1191.98 --> 1195.78]  Now, WLED is really great.
[1196.82 --> 1206.60]  I know, though, that for some people, it is a little too advanced because while the software is now easy to load and configure and it integrates with Home Assistant in a snap,
[1207.56 --> 1214.10]  you'll have to either get some sort of clamps or you'll do some soldering or some kind of wiring to be able to get all the connectors in.
[1214.10 --> 1221.80]  And the ESPs are pretty good, but they're not maybe purpose-built for driving a nice, you know, light strip.
[1222.16 --> 1236.70]  So I've been digging for about a year to try to find a product that is cheap, that comes with WLED preloaded, that is really like has a clamp or something where you just take the wires from the LED strip and just connect them in.
[1236.70 --> 1245.88]  And I've experimented with a couple off of Amazon and haven't really liked what I found until I found the domestic automation product.
[1246.36 --> 1250.66]  I think they have a, like the Shafoos, I believe is the one I got.
[1250.74 --> 1251.64]  It's something like that.
[1252.10 --> 1255.88]  This is, it's a little board about the size, a little bit smaller than a Raspberry Pi.
[1255.88 --> 1260.50]  And it has a few things on here I like a lot.
[1260.62 --> 1269.42]  First of all, it comes pre-wired with the three-pin JSTSM connector that you need for the WS2812 LEDs.
[1269.66 --> 1272.22]  So it comes with that connector.
[1272.82 --> 1273.88]  You just plug it in.
[1273.96 --> 1275.50]  It also comes with a mounting bracket.
[1275.72 --> 1279.76]  So if you want to put it like on the wall or under a table, it comes with all the stuff you need to mount it.
[1279.76 --> 1288.86]  But the thing that I think is really sharp and why I might just end up using this, even though it's a little bit more than an ESP, is it comes with an onboard 10 amp fuse.
[1289.74 --> 1293.12]  And the other thing I really like is it comes with an onboard relay.
[1293.92 --> 1298.82]  And if you really, really, really care about vampire power draw, you know why that matters.
[1298.82 --> 1301.68]  Because those LED light strips will take a little teeny tiny bit of power.
[1301.84 --> 1305.74]  When you turn them off, they're still taking a little teeny tiny bit of power.
[1305.74 --> 1316.00]  But with this relay, as soon as you tell, like Home Assistant, you say turn off the light strip, I guess the board must detect the drop in voltage.
[1316.32 --> 1319.40]  And the relay kicks in and physically turns off the light strip.
[1320.46 --> 1321.60]  That's really nice.
[1323.08 --> 1331.44]  And then there's one more aspect to it that I just feel like I probably wouldn't have built had I done this with an ESP myself.
[1331.44 --> 1335.16]  And that is they include an onboard sacrificial pixel.
[1335.62 --> 1346.72]  So if you're not familiar with this, the idea is it essentially allows you to put the LED light strip actually further down away from the controller and not have a signal degrade.
[1347.54 --> 1352.72]  Because that first light there, basically, once it hits that first LED at the full voltage, it converts it to a data signal.
[1352.78 --> 1354.08]  And you can send that a lot further.
[1354.08 --> 1359.46]  So there's a sacrificial LED that's really useful that's just built into the board.
[1359.64 --> 1364.30]  And if you don't want it to light up, you just go to the WLED preferences and you say turn off light one.
[1364.52 --> 1367.76]  There's a little option in the preferences actually just to say don't turn on light one.
[1368.58 --> 1370.82]  Because I guess other people do the sacrificial pixel thing as well.
[1371.74 --> 1372.64]  I think it's fantastic.
[1372.80 --> 1377.64]  And last but not least, it has a little power injection block on it.
[1377.96 --> 1382.62]  So if you want to do a longer light strip, you can inject power into it.
[1382.90 --> 1383.58]  That's really nice.
[1383.58 --> 1390.42]  I've spent a good number of hours explaining to friends and family even that voltage drop is a thing.
[1390.98 --> 1391.46]  Yes.
[1391.90 --> 1395.28]  You know, it's really hard to explain the circuit required.
[1395.40 --> 1401.16]  And if you just have a black hole and a red hole, like plug in these wires into this spot, so much easier.
[1401.36 --> 1401.92]  This is great.
[1402.58 --> 1403.84]  Now they have several different models.
[1404.00 --> 1405.18]  This one is off Amazon.
[1405.28 --> 1406.04]  I got it for $39.
[1406.40 --> 1410.68]  Now I know, again, if you're comparing it to like a pack of ESPs, that's not cheap.
[1410.68 --> 1413.46]  But they have a couple of different models.
[1413.66 --> 1417.82]  They have one that has an external Wi-Fi antenna if you need better signal, which I think is really clever.
[1417.82 --> 1420.68]  They also have a fuse block if you need to do a breakout.
[1420.88 --> 1429.90]  They have a couple of additional accessories that connect over like a serial RJ11 type connection and including a physical momentary button switch.
[1429.90 --> 1436.98]  So if you want to have a physical switch that's physically wired to the controller to control your WLED strip, you can.
[1437.18 --> 1438.04]  I think that's kind of nice.
[1438.84 --> 1442.08]  $40 isn't cheap, but it's a family-run business.
[1442.08 --> 1446.46]  This entire idea was created by a high school kid as he was getting out of high school.
[1447.06 --> 1449.62]  His mom, his dad, his sister, he's the youngest of the group.
[1449.70 --> 1453.30]  They're all running this business with him, this domestic automation.
[1454.64 --> 1456.52]  And he's using the sales of this.
[1456.56 --> 1456.96]  I don't know.
[1457.04 --> 1458.96]  I just did some investigation before the show.
[1459.36 --> 1460.18]  I don't know them personally.
[1460.18 --> 1465.96]  And he says he's using the funds that they're raising from the business to help fund his college.
[1466.98 --> 1474.82]  Which is, I mean, think about this kid, and I say that with all respect, came up with a product that I have been looking for for a year.
[1475.14 --> 1476.68]  And it's really well done.
[1476.74 --> 1477.60]  It's a solid piece.
[1477.66 --> 1478.24]  I have it upstairs.
[1478.38 --> 1479.62]  It's a really well-built thing.
[1480.20 --> 1482.16]  And then they made a family business out of it.
[1482.74 --> 1485.98]  And I just don't know why bigger companies out there didn't see this opportunity.
[1485.98 --> 1491.66]  But this clever kid is quite the entrepreneur, and I think it's pretty great.
[1491.74 --> 1492.70]  So I'll put a link to it in the notes.
[1493.34 --> 1494.66]  They got several different models on Amazon.
[1495.62 --> 1498.88]  And it really is nice because it makes WLED plug and play.
[1499.28 --> 1503.06]  And if you order it right around when this show comes out, you can probably still get it in time for Christmas.
[1504.02 --> 1506.52]  And you can just, boom, plug in one of those LED light strips.
[1507.02 --> 1509.48]  It doesn't come with the 5-volt barrel adapter.
[1509.62 --> 1513.64]  You will need to buy the power adapter separately.
[1513.64 --> 1517.90]  It's one of those 2.5 by 5.5 millimeter barrel connectors.
[1518.16 --> 1519.78]  Got to get that on your own, 5 volts.
[1520.70 --> 1524.20]  Mine that I got, I think, is 5 volts, 15 amps, something like that.
[1524.84 --> 1525.96]  Plug it all in, and you're good to go.
[1526.20 --> 1527.32]  Plug in the light strip, good to go.
[1527.76 --> 1528.70]  Get it on the Wi-Fi, done.
[1529.50 --> 1530.90]  Very, very neat little product.
[1531.62 --> 1535.82]  You pay a little bit extra for all that stuff built in, you know, versus a $5 ESP.
[1537.14 --> 1541.88]  But, I don't know, for something you're going to be running for 5, 10 years potentially, I think it's worth it.
[1541.88 --> 1546.02]  And then you have the warm fuzzies of sending little Jimmy through college, too.
[1547.16 --> 1548.14]  I think it's Michael.
[1548.22 --> 1549.12]  I do love that.
[1549.14 --> 1549.64]  It's not Jimmy, it's Michael.
[1549.64 --> 1549.84]  It is great.
[1550.66 --> 1551.62]  Michael, sorry.
[1552.20 --> 1552.94]  It is, sir.
[1552.96 --> 1559.40]  We also had on the show, back in episode 9, if you remember, in January 2020, in the before times.
[1559.72 --> 1559.96]  Wow.
[1559.96 --> 1566.12]  The maker of Quinn LED, which is a, you know, he's based out of Europe, I think, in the Netherlands.
[1567.32 --> 1571.02]  So, if shipping from America to Europe, if you're listening to this in Europe, is an option.
[1571.58 --> 1574.62]  The Quinn LED boards, I've used a couple of the Digunos.
[1574.96 --> 1577.76]  They have fuses built in and a bunch of other stuff, too.
[1578.12 --> 1579.34]  That's another great option for you.
[1579.34 --> 1584.00]  Linode.com slash SSH.
[1584.10 --> 1589.14]  Man, Linode is the hosting provider because now they're part of Akamai.
[1589.34 --> 1595.48]  All the tools and the infrastructure that we like and the interfaces, even the API, that's all staying the same.
[1595.56 --> 1601.18]  The stuff we use to build and deploy at scale quickly is still there, but now they're backed by the Akamai.
[1601.58 --> 1603.80]  This is really the only choice now.
[1603.80 --> 1611.36]  If you want a high-quality hosting provider with great pricing, it's Linode now, especially when they're now part of Akamai.
[1611.88 --> 1616.36]  And there's more resources that Akamai is adding to Linode, so they're expanding their data centers worldwide.
[1616.52 --> 1621.04]  We just took advantage of one of those new ones, like the week it went online, and it was smooth.
[1621.34 --> 1622.46]  It's been working flawlessly.
[1623.36 --> 1627.96]  They have solutions that are great for individuals, but they'll scale up to an enterprise of any size.
[1628.06 --> 1630.54]  I mean, they have massive enterprises running on Linode.
[1630.54 --> 1635.06]  And as part of Akamai's global network of offerings, you're going to see more resources.
[1635.20 --> 1636.30]  You're going to see more data centers.
[1636.40 --> 1637.82]  You're going to see better network connectivity.
[1638.48 --> 1639.12]  So why wait?
[1639.72 --> 1642.20]  Go see why we love Linode, why we've been using it for years.
[1642.30 --> 1643.74]  It's how JB hosts everything.
[1644.44 --> 1646.10]  It's the only hosting provider I would use.
[1647.04 --> 1648.92]  Go to linode.com slash SSH.
[1649.18 --> 1654.26]  Go see how Linode, now Akamai, will help scale your applications from the cloud way out to the edge.
[1654.78 --> 1656.00]  Probably even Brent's place.
[1656.56 --> 1657.32]  In fact, I'm pretty sure.
[1658.32 --> 1660.32]  Linode.com slash SSH.
[1660.54 --> 1671.94]  As if we needed yet another thing to worry about, our push notifications are now under threat, are being watched by Big Brother.
[1673.04 --> 1674.18]  You hate to see it.
[1674.30 --> 1675.88]  I'm not surprised at all.
[1675.96 --> 1677.24]  In fact, I've speculated on air.
[1677.94 --> 1679.36]  This is very likely the case.
[1680.02 --> 1681.74]  But, God, you just hate to see it.
[1681.76 --> 1685.74]  And the part that I really, really don't like is there's this silent rule.
[1686.42 --> 1691.20]  Apple and Google have been forbidden by the Justice Department here in the U.S. at disclosing details.
[1691.34 --> 1692.92]  So they couldn't tell us this was happening.
[1693.56 --> 1695.02]  So, Alex, I'm not kidding you.
[1695.84 --> 1698.14]  They have this transparency report they put out.
[1698.60 --> 1700.78]  But they couldn't put this in the transparency report.
[1700.88 --> 1705.48]  But now that we know, now that we know, Apple has said they can now put it in the transparency report.
[1706.18 --> 1706.54]  Hmm.
[1707.48 --> 1708.36]  Color me skeptical.
[1708.36 --> 1712.90]  But then what is the purpose of a transparency report that isn't fully transparent?
[1714.28 --> 1714.40]  Yeah.
[1714.82 --> 1715.38]  Yeah, I know.
[1715.44 --> 1717.04]  It's like, okay, guys.
[1717.38 --> 1720.94]  And also not so great for iPhone users.
[1721.26 --> 1724.76]  With Apple, law enforcement agents can just issue subpoenas on their own.
[1725.42 --> 1726.36]  There is no oversight.
[1726.36 --> 1732.96]  But on Google's side of the house, Google requires a court order before they hand over the push notification data.
[1733.78 --> 1734.58]  Yeah, this is gross.
[1734.74 --> 1743.48]  I mean, the push notification token basically gives you access as law enforcement to any push notification that was sent to your device.
[1743.48 --> 1751.64]  So that contains every text message pretty much that you get from any app on your phone and the text that's in that message.
[1751.82 --> 1757.72]  So even if they can't break the encryption on WhatsApp or Telegram or whatever else, Signal or whatever.
[1757.84 --> 1761.30]  Well, actually, Signal is probably a good example of what to do.
[1761.54 --> 1764.80]  Because I saw a tweet earlier saying, or was it a toot?
[1764.90 --> 1771.82]  I forget where I saw it earlier, saying Signal actually don't send anything sensitive through the push notification system.
[1771.82 --> 1775.20]  So they're actually not vulnerable to being eavesdropped through Signal.
[1775.34 --> 1778.76]  So if you care about this, actually, Signal might be a good way to go.
[1779.20 --> 1783.44]  I also will give a plug here on the self-hosting side for SimpleX or SimpleX.
[1783.84 --> 1784.68]  Same sort of setup.
[1785.58 --> 1787.04]  No phone number required.
[1787.18 --> 1787.68]  No email.
[1788.16 --> 1789.90]  And you can control the push notifications.
[1790.44 --> 1797.16]  But this has got me thinking about a project to bring more of my push notifications into my own infrastructure.
[1797.16 --> 1805.38]  When I first set up my current NextCloud system a while ago now, I really considered it.
[1805.74 --> 1806.80]  I really considered it.
[1806.92 --> 1810.28]  And then when I switched to Android, I don't know if you know this, but I have Android now.
[1810.34 --> 1812.36]  I'm an Android user, by the way.
[1812.60 --> 1814.44]  You've been doing that joke for a year now, dude.
[1814.66 --> 1814.90]  Yeah.
[1815.10 --> 1815.64]  I know.
[1815.68 --> 1816.30]  Just over a year.
[1816.90 --> 1818.16]  Then at that, again, I reassessed.
[1818.88 --> 1821.08]  And I thought, well, you know, this would really be the time.
[1821.16 --> 1822.44]  I'm not going to have Google services.
[1822.44 --> 1824.80]  This would really be the time to do it.
[1825.48 --> 1829.92]  And I punted because it just seemed like one more thing to bite off at that moment.
[1830.92 --> 1832.22]  Now I'm looking back at that decision.
[1832.32 --> 1833.34]  I'm thinking maybe I made a mistake.
[1833.40 --> 1834.48]  I think my instincts were right.
[1835.46 --> 1836.32]  No, I don't think so.
[1836.54 --> 1840.26]  Like most things, I'm going to take the pragmatic standpoint on this.
[1841.32 --> 1843.30]  Push notifications are a bit like email.
[1843.56 --> 1846.04]  Like they need to just work.
[1846.04 --> 1852.90]  And there is so much plumbing involved in replacing the OS level skullduggery that goes on.
[1852.98 --> 1856.68]  Because you know that Apple and Google have special APIs they reserve for just themselves.
[1857.22 --> 1861.96]  And you're going to have to have apps that support any kind of custom notification system, I imagine.
[1862.00 --> 1862.98]  They're going to have to support that API.
[1863.18 --> 1866.62]  It's going to be on each developer, which means it's going to be not very often they're going to support it.
[1866.62 --> 1879.84]  The reality is it's basically impossible unless you go the graphene route, honestly, and just turn off all these things or just simply don't use apps that leak data this way.
[1879.84 --> 1891.64]  I do think it's a little easier on Android because Android is such a fragmented landscape that a lot of application developers, at least the large ones, can't depend on Google Play API and push notifications.
[1892.06 --> 1895.92]  So they've kind of developed like this fallback where like they'll use the Play API.
[1896.32 --> 1901.52]  But if it's not there, we'll just run the app in the background all day long and just receive notifications that way.
[1901.58 --> 1903.86]  That's what Element and Telegram do on Android.
[1904.04 --> 1905.10]  Here's the thing, though.
[1905.16 --> 1908.36]  At what point is self-hosting not self-hosting anymore?
[1908.36 --> 1914.02]  Is running all of your stuff on a VPS self-hosting because someone else is running the server?
[1914.92 --> 1920.24]  What about your ISP that you trust to run the internet from your house to the exchange?
[1920.88 --> 1922.50]  What about, what about, what about?
[1922.88 --> 1928.04]  So there comes a point where you're like, I just can't possibly do it all.
[1928.24 --> 1929.54]  There's only so many hours in the day.
[1929.60 --> 1932.14]  There's only so many things I can control.
[1932.40 --> 1935.42]  And it's a sad position to take.
[1935.42 --> 1943.08]  But I think that for push notifications in particular, it's just impossible not to fall victim to some of this stuff.
[1944.10 --> 1950.56]  Yeah, and I guess it reminds us that if you're really sensitive about what's in those push notifications, use an app that lets you turn that off.
[1951.00 --> 1954.18]  I wonder if they'll be able to remind me where I parked my car because I always seem to forget that.
[1954.18 --> 1959.92]  How are you going to know if it's actually not sending the data versus just not showing it?
[1960.28 --> 1963.52]  Right, because on iOS, there's that setting to just not show the preview.
[1963.70 --> 1965.62]  But that doesn't mean that the app didn't send it in the background.
[1965.74 --> 1967.10]  The OS is just hiding it.
[1967.78 --> 1971.02]  Well, it's hiding it until you unlock your phone.
[1971.22 --> 1971.24]  Unlock.
[1971.30 --> 1972.20]  And then it shows up, right?
[1972.26 --> 1973.38]  So it must have come through somehow.
[1973.38 --> 1974.00]  Unlocking it, yeah.
[1975.76 --> 1980.74]  How are users ever going to, regular users are never going to be able to manage all this?
[1980.88 --> 1988.20]  What happens on your iPhone stays on your iPhone, except unless it's a push message and it didn't actually originate from your iPhone.
[1988.20 --> 1992.82]  And then it came through iCloud and actually through the NSA and, you know.
[1994.14 --> 1997.02]  The year of voice chapter five was today.
[1997.20 --> 1998.38]  I watched the live stream.
[1999.20 --> 2000.90]  And this is really remarkable.
[2000.90 --> 2002.96]  I can't believe we got five chapters this year.
[2003.24 --> 2007.28]  And I think they're transitioning now into just a continuous improvement mode.
[2007.92 --> 2009.28]  Some big stuff came out today.
[2010.30 --> 2021.38]  And if you were listening carefully last episode and you heard me say, hey, that ESP Box 3 is available and this is going to be the new Home Assistant voice thingy.
[2021.40 --> 2022.86]  You should go grab one while they're in stock.
[2022.96 --> 2028.38]  Well, hopefully you did because today they announced official support for the S3 Box 3.
[2028.56 --> 2029.78]  And I got mine right here.
[2029.78 --> 2032.98]  And it's a lot smaller than I thought, but it's got a little screen on it.
[2033.42 --> 2035.72]  It's got two microphones and a better speaker.
[2035.72 --> 2046.70]  And then depending on the one you get, it comes with like this PC, a mini PCI Express connector and then three different docks.
[2047.44 --> 2055.86]  This one has an IR sensor, a temperature sensor, and apparently takes a big old lithium battery that I can put in the bottom of this thing.
[2055.86 --> 2060.42]  Another one came with like a bunch of pins to like wire stuff to it.
[2060.52 --> 2063.96]  And then another one came with just some basic dongle connectors for like USB.
[2064.70 --> 2067.14]  But the device itself fits in the palm of the hand.
[2067.14 --> 2077.82]  And the screen displays, once you flash it, a little Home Assistant logo that's giving you feedback on when it's processing or when it's connected or disconnected or when it's giving you an answer.
[2077.82 --> 2082.48]  And of course, you can replace it with your own images if you like.
[2082.48 --> 2088.78]  In fact, the Home Assistant team teased a little template that you can give to your kids.
[2089.72 --> 2091.38]  It's got boxes on there.
[2091.64 --> 2095.52]  And each box is supposed to be one of the state faces of the Assistant.
[2095.64 --> 2099.80]  And you can have your kids draw and then turn that into one of the images on here.
[2099.80 --> 2108.50]  And they said that when they were developing this at home, their kids started interacting with the Assistant a lot more once their drawings were on the screen.
[2109.54 --> 2112.90]  And this setup is much like it is for anything else these days.
[2113.00 --> 2118.18]  You plug it in over USB, go to the web page, flash it, and then connect it to Home Assistant.
[2118.74 --> 2123.94]  And you're up and running with something that's got much better microphones and supports the wake word.
[2123.94 --> 2138.98]  So I can say, OK, Naboo, and it wakes up and I can give it a command and it will execute that command all locally using my local whisper, my local piper, and my local open wake word instance running on a different box than my Home Assistant blue.
[2140.02 --> 2141.62]  What a time to be alive, huh?
[2141.82 --> 2148.16]  You know, so all of the installation stuff we talked about for WLED, this is using an ESP device underneath.
[2148.48 --> 2150.26]  That's exactly what this is doing, too.
[2150.34 --> 2152.64]  It's using that same magic from Chrome.
[2152.64 --> 2160.84]  It's using that same magic just to connect to these devices and install whatever firmware binary that you're trying to flash onto them from your web browser.
[2161.28 --> 2163.10]  It's genuinely quite amazing.
[2163.10 --> 2164.18]  It's mind-blowing, Alex.
[2164.24 --> 2164.82]  It's mind-blowing.
[2165.46 --> 2167.86]  And then just one last little other thing that's really nice to see.
[2169.56 --> 2173.64]  They have greatly improved the Raspberry Pi satellites.
[2174.22 --> 2176.56]  If you go on Amazon, and I'm sorry I don't have the name of it,
[2176.56 --> 2185.06]  but there is an Anker circular speakerphone that's got like three or more microphones built into it and a speaker, and it's USB.
[2186.06 --> 2190.14]  And it makes for a perfect voice assistant speaker.
[2190.76 --> 2196.46]  And you can plug that in over USB to a Raspberry Pi 4 or 3 or whatever, or 0 even.
[2196.46 --> 2198.56]  And you can turn that into a satellite.
[2198.80 --> 2207.34]  And with this new release that came out today as we record, they've solved some of the limitations with Raspberry Pi satellites and made them really first-class listening devices.
[2207.34 --> 2217.16]  And now the Raspberry Pis have been integrated directly into their Wyoming protocol and will communicate to the backend instances,
[2217.32 --> 2221.74]  and the backend instances can communicate directly to them without having to go through any extra steps.
[2222.40 --> 2223.36]  And it's faster.
[2223.54 --> 2223.92]  It's smoother.
[2224.50 --> 2225.40]  And it's really nice to see.
[2225.50 --> 2229.16]  So both from like the DIY standpoint and from the stuff you can buy, they're coming along.
[2229.58 --> 2234.88]  And the nice thing about the Raspberry Pi satellites, obviously, Alex, is that you could go as geeky as you want.
[2234.88 --> 2240.82]  Like if you want to set it up to a huge set of speakers with an amp and a receiver, you could, right?
[2240.86 --> 2241.72]  With a big old microphone.
[2241.72 --> 2244.06]  You could put your podcast microphone hooked up to that thing if you want.
[2244.10 --> 2249.08]  You could have perfect, crystal clear audio when you're telling your home assistant to turn on your lights or whatever.
[2249.46 --> 2252.06]  Or, you know, you could use something that's just built into a little box.
[2252.22 --> 2260.22]  But because it's an open system using open source software and open protocols, we as tinkerers can go as far or not as we want with this.
[2260.26 --> 2261.70]  And that's what I'm really excited about.
[2262.14 --> 2264.38]  I wonder where home assistant is going to go next year.
[2264.38 --> 2266.66]  You know, so this year, the voice stuff.
[2266.80 --> 2271.48]  I mean, it's nothing short of amazing what they've done with this year of the voice.
[2271.82 --> 2275.70]  You know, all the wait word stuff actually working on a fully open source platform.
[2276.06 --> 2282.36]  You know, you think how much money Amazon and Google must have spent on those departments to make that happen with their hardware.
[2283.08 --> 2288.70]  And home assistant, the little scrappy open source startup has gone ahead and done it with a skeleton crew.
[2288.88 --> 2291.20]  And amazing, amazing stuff.
[2291.28 --> 2292.58]  So I wonder what they're going to do next year.
[2292.58 --> 2298.52]  My personal wish list would be some UI improvements and just overall UX improvements, hopefully.
[2299.16 --> 2300.04]  Yeah, I'd like to see more of that.
[2300.38 --> 2300.50]  Yeah.
[2301.02 --> 2303.52]  The thermostat card just got a nice UI overhaul.
[2304.04 --> 2309.12]  I think, Alex, they have a year's worth of work updating home assistant to actually be used by voice.
[2309.22 --> 2309.90]  I'll give you an example.
[2309.90 --> 2312.08]  If you say, what is the temperature?
[2313.54 --> 2314.54]  Well, what does it know?
[2314.70 --> 2316.06]  How does it even know what you're talking about?
[2316.10 --> 2319.44]  Because you can have a temperature sensor, you know, in my fridge.
[2319.46 --> 2320.84]  I can have a temperature sensor outside.
[2321.04 --> 2322.64]  I have a temperature sensor in the room I'm in.
[2323.22 --> 2326.34]  You know, you can have a temperature sensor in your water heater.
[2326.34 --> 2332.30]  Like, when you think about it, they really have so much work to do to make it really clear.
[2332.70 --> 2333.88]  Okay, he's in this room.
[2334.18 --> 2335.44]  He's asking these questions.
[2335.54 --> 2336.48]  It's in this context.
[2336.90 --> 2337.88]  And they've started to solve that.
[2337.98 --> 2339.24]  Like, they've added area support.
[2339.74 --> 2348.88]  So now when you say, turn on the lights, and you don't give any specifics, and you just leave it, like, just empty like that, it'll assume the room you're in.
[2348.88 --> 2351.86]  It'll know what room you're in, and it'll turn off the lights in that room.
[2351.90 --> 2352.70]  So they've gotten there.
[2352.84 --> 2359.84]  But there's so much more you really have to do to make it a speakable interface where everything gets recognized and you get the right things.
[2359.84 --> 2367.94]  Like, everything from basics to, like, you know, task lists and timers, which they're starting to get, to more advanced stuff.
[2368.08 --> 2376.34]  Like, I think, ultimately, when they're done on this journey, my prediction is you're going to see an overhaul of the automations.
[2376.34 --> 2380.40]  Because you're going to have the ability to create automations using natural language.
[2380.58 --> 2387.38]  And you're going to be able to use the technology they're using for all of this voice recognition to use natural language to create automations.
[2387.82 --> 2389.78]  And I think that's where this eventually goes.
[2389.96 --> 2391.00]  But I don't know how long it takes.
[2393.18 --> 2395.54]  Talescale.com slash self-hosted.
[2395.62 --> 2398.76]  Go on over there to get a free personal account for up to 100 devices.
[2398.88 --> 2399.62]  That's my account.
[2400.08 --> 2403.42]  All of my HomeLab stuff, it's on my free personal account.
[2403.56 --> 2405.10]  And it's a great way to support the show.
[2405.10 --> 2409.14]  100 devices really, really lets you get an idea of what Talescale can do.
[2409.56 --> 2417.72]  Now, if you're not familiar, it's a zero-config VPN built on WireGuard that you can get up and running in just minutes.
[2418.16 --> 2425.28]  Not only do you not have to worry about, like, these weird problems of trying to get DNS between two different subnets when you have a WireGuard VPN between them.
[2425.32 --> 2427.10]  And for some reason, it's not working today.
[2427.50 --> 2431.40]  You don't have to worry about how to try to make it all work through Network Manager or the command line or not.
[2431.40 --> 2435.72]  You don't have to run a WireGuard server on one box that everything connects into.
[2436.36 --> 2439.42]  Talescale builds out a mesh VPN in just minutes.
[2439.70 --> 2440.44]  It's a flat network.
[2440.60 --> 2442.02]  All your devices get a static IP.
[2442.66 --> 2450.28]  And then you can start doing things like magic DNS or throw a pie hole in there and have DNS on your tail net and start resolving things by name wherever you go.
[2450.28 --> 2454.58]  So pretty soon you start realizing you don't need to have anything external.
[2455.06 --> 2457.60]  You essentially can build your own private internet.
[2458.18 --> 2462.44]  And the beautiful thing is, is you can have it on multiple different cloud providers.
[2462.68 --> 2463.72]  You can have it on your LAN.
[2463.82 --> 2464.54]  You can have it in a VM.
[2464.96 --> 2466.80]  There's even plugins for, like, VS Code.
[2467.24 --> 2475.70]  There's all kinds of different ways to install and use Talescale and build out a flat mesh network between instances that are spread out all over the world.
[2475.70 --> 2480.28]  Man, did it just totally come in handy when I was traveling in El Salvador.
[2480.76 --> 2481.92]  Talk about peace of mind.
[2482.24 --> 2487.38]  And it's perfect for businesses or developers who want to set up ad hoc networking, maybe do some demos.
[2487.56 --> 2494.24]  And, man, for the enterprise space, not to have to manage all those traditional VPN systems, but still to get that superior protection of WireGuard.
[2494.46 --> 2498.22]  And it integrates with your existing authentication system and two-factor for you to use that.
[2498.22 --> 2501.86]  And there are so, so many tools built around Talescale as well.
[2502.28 --> 2505.64]  It's truly one of the best, I think, benchmark tools out there.
[2506.04 --> 2507.42]  They're showing the industry how it's done right.
[2507.94 --> 2513.54]  Support the show and try it for free on 100 devices when you go to talescale.com slash self-hosted.
[2513.92 --> 2515.00]  Head on over there and try it.
[2515.30 --> 2516.86]  I think you're really going to be impressed.
[2517.32 --> 2523.02]  And it just solves a connectivity problem and just totally changes the way you can do networking for the better.
[2523.52 --> 2526.12]  Talescale.com slash self-hosted.
[2528.22 --> 2534.58]  Last episode, I talked a little bit about hardwired ESP32s and the listeners wrote in in their droves.
[2534.70 --> 2536.98]  We got literally an email about it.
[2537.80 --> 2542.00]  Yeah, listener, Mike sent in a cheaper PoE option for the ESP32.
[2542.00 --> 2543.44]  This is the ESP32 episode.
[2544.10 --> 2545.02]  And here's the nice thing.
[2545.08 --> 2547.34]  Not only is it 20 bucks, totally open source.
[2547.82 --> 2548.58]  That's neat.
[2549.12 --> 2549.84]  Hard to beat that.
[2550.56 --> 2550.74]  Yeah.
[2550.90 --> 2554.58]  I mean, the one you talked about last episode was 50 and it looked really robust.
[2554.58 --> 2560.04]  Again, you guys, if this is something like I'm putting in my wall for 10 years, I'll spend the 20 bucks.
[2560.10 --> 2561.02]  I'll spend the 50 bucks.
[2561.14 --> 2563.00]  But if I can spend a little bit less, I will.
[2563.16 --> 2564.16]  So I like that option.
[2564.40 --> 2564.90]  Thank you, Mike.
[2565.44 --> 2568.80]  Alex, are you excited about the first ever NixCon North America?
[2568.96 --> 2570.14]  NixCon North America.
[2570.30 --> 2570.88]  North America.
[2571.42 --> 2572.52]  I think so.
[2572.52 --> 2578.20]  You know, I'm reluctantly a Nix convert at this point.
[2578.48 --> 2581.48]  Like, I really enjoy messing around with it.
[2581.62 --> 2584.68]  But also, like, sometimes I just want to get work done.
[2585.26 --> 2587.72]  And, you know, it's balancing the two.
[2588.28 --> 2595.08]  So NixCon should be really good because there'll be a bunch of people there who know way more about Nix than anybody has any right to know.
[2595.74 --> 2596.14]  Definitely.
[2596.14 --> 2596.26]  Definitely.
[2598.10 --> 2598.46]  Yeah.
[2598.54 --> 2599.94]  We'll, like, absorb it, right?
[2600.00 --> 2602.44]  And get all, get, like, the Nix hype and the Nix tips.
[2603.00 --> 2605.00]  Maybe people will be there just sharing their configs.
[2605.00 --> 2605.40]  I don't know.
[2606.00 --> 2613.06]  I like the fact that it's co-located alongside Scale, Southern California Linux Expo, number 19, I think.
[2613.42 --> 2616.44]  It's good to see that conference come back because I had a bit of a dip after COVID.
[2617.40 --> 2617.62]  Yeah.
[2617.92 --> 2619.60]  So you will need a Scale Pass.
[2619.78 --> 2620.98]  Those are, like, 20 bucks or something.
[2621.02 --> 2621.52]  Not very much.
[2621.52 --> 2626.58]  You will need a Scale Pass to get in there and we'll be there.
[2627.10 --> 2628.44]  So, you know, come say hi to us.
[2628.50 --> 2636.70]  Do a little self-hosted hangout and maybe enjoy NixCon if you like or enjoy Scale otherwise, which has got a wide range of topics.
[2637.50 --> 2642.30]  Pretty much anything open source is going to be talked about there and stuff that can be absolutely applicable to your day job.
[2642.58 --> 2643.86]  We're going to put a link in the show notes.
[2644.00 --> 2647.90]  They've got their call for proposals open right now, as does Scale, I believe.
[2647.90 --> 2653.14]  So if you've ever wanted to submit a talk about Nix, now's the chance.
[2653.78 --> 2656.58]  Now, we did get some great boosts into this episode.
[2656.78 --> 2660.34]  Thank you, everybody who supports this here individual production with a boost.
[2660.62 --> 2664.06]  And Devator came in with 29,000 sats using Podverse.
[2664.64 --> 2665.82]  And he agrees with you, Alex.
[2665.90 --> 2669.42]  He says, this was my Google Photos moment with Plex.
[2670.12 --> 2674.08]  I've had a lifetime pass for years and it was my gateway to self-hosting.
[2674.08 --> 2677.88]  And they've also just added auto intro skipping with a watch button.
[2679.48 --> 2683.62]  It's really still the best possible user experience, but alas, it's all gone.
[2683.92 --> 2686.30]  I spun up Jellyfin and I deleted my Plex account.
[2686.78 --> 2691.34]  The Jellyfin clients are a huge barrier for me, but I deployed Jellyfin Tizen to my TV.
[2691.98 --> 2695.16]  It's working great, though it did take a while because of the cert signing.
[2695.32 --> 2696.00]  That kind of sucked.
[2696.00 --> 2707.50]  Well, yeah, running it through a non-encrypted reverse proxy or not putting it through a reverse proxy with a certificate is going to be tricky with clients.
[2707.64 --> 2712.52]  So my suggestion there would be just put Caddy in front of it or something and just do a DNS challenge.
[2712.66 --> 2719.34]  Put your DNS in any provider that's supported by the Lego library that is used underneath to get those certificates.
[2719.98 --> 2724.56]  But the Android TV client had an update this week as well, which is pretty nice.
[2724.56 --> 2729.86]  I still get a bunch of crashes with this thing when I'm loading into the library itself.
[2730.18 --> 2732.32]  But apart from that, the performance is great.
[2732.48 --> 2734.36]  The library loads a lot faster now.
[2734.76 --> 2736.96]  The screensaver is quite nice too.
[2737.52 --> 2744.98]  I am still using Infuse as my primary interface, but I too have switched back over to Jellyfin on the back end.
[2745.06 --> 2749.42]  So I had to do the browser of shame approach.
[2749.42 --> 2755.86]  This is what I do is I open up the Plex web browser and I open up the Jellyfin web browser and I bring them both up.
[2756.04 --> 2758.84]  And I go into each TV show and I mark as red whatever.
[2759.02 --> 2765.46]  OK, so whichever one I'm switching, if I'm going from Plex to Jellyfin or Jellyfin to Plex, I just I have to like go in there and manually mark them all red.
[2766.18 --> 2769.54]  And maybe there's a project that syncs between Jellyfin and Plex your watch status.
[2769.54 --> 2772.30]  But hopefully this is the last time I've ever had to do it.
[2772.62 --> 2778.88]  I think probably what you're looking for is tracked TV sync and that will sync via tracked between the two different projects.
[2779.10 --> 2781.04]  Oh, yes, of course.
[2781.24 --> 2783.98]  I do have one request for the listeners.
[2783.98 --> 2799.58]  If you are a Plex Meta Manager user and you know of an equivalent that's as good for Jellyfin, I would love to hear you because building handcrafted holiday collections is not something I've got any interest in doing.
[2799.78 --> 2805.24]  And when wife goes, I want to watch a Christmas movie with the kid, I'm like, well, OK.
[2805.58 --> 2807.02]  Yes, I hear you.
[2807.30 --> 2809.12]  I also agree.
[2809.12 --> 2815.12]  I had a very frustrating I had a very frustrating moment, too, with that this week last weekend.
[2815.36 --> 2818.04]  I was like, well, we've got these ones and we're just sitting here scrolling through the list.
[2818.12 --> 2818.66]  It's embarrassing.
[2819.70 --> 2823.44]  Fuzzy Mistborn comes in with one, two, three, four, five sats.
[2823.54 --> 2825.40]  That is a Spaceballs boost from the index.
[2825.50 --> 2833.44]  He says regarding Chromecast and IoT networks, I subscribe to the Tom Lawrence school of thought that your phone isn't a trusted device.
[2833.44 --> 2835.86]  It goes out into the world, connects to public Wi-Fi, et cetera.
[2835.86 --> 2842.32]  Therefore, mine lives on the same network as my IoT devices, so casting isn't an issue.
[2842.82 --> 2846.78]  If I need something on my secure network, I either create a firewall rule or I use Tailscale.
[2847.26 --> 2847.44]  Yeah.
[2848.32 --> 2852.00]  Now, that's a pretty strict rule there, Fuzzy.
[2852.24 --> 2857.10]  So, Alex, do you think you could survive by never putting your phone on your main Wi-Fi network?
[2858.10 --> 2859.08]  It's an interesting thought.
[2859.24 --> 2863.68]  And until I read Fuzzy's feedback, I hadn't really thought about it.
[2863.68 --> 2872.00]  I mean, so I've got Blink as an SSH client that connects into my server via SSH using Tailscale for the authentication these days.
[2872.26 --> 2873.92]  So that wouldn't be a problem.
[2874.62 --> 2880.38]  My 3D printers are Bamboo Lab printers now, not Octoprint running behind me on a Pi anymore.
[2880.56 --> 2883.32]  So they are a cloud-based situation.
[2883.64 --> 2885.66]  So that would be fine.
[2885.98 --> 2887.14]  Maybe Blue Iris.
[2887.40 --> 2888.74]  But then I guess I could put that on.
[2888.96 --> 2890.66]  Well, I wouldn't want that on the IoT.
[2890.66 --> 2902.08]  I think it's hard for an iPhone, Alex, because if you're in the Apple ecosystem, they use Wi-Fi to do a lot of the handoff between HomePods, Apple TV, Apple Watch.
[2902.82 --> 2904.44]  A lot of that is all done over.
[2904.68 --> 2910.56]  It's assumed that your Wi-Fi is that your phone is on the Wi-Fi of all the same devices.
[2910.86 --> 2912.22]  I think it's tricky.
[2912.36 --> 2916.14]  And then, you know, for not about you, but I use my phone to control a lot of my devices.
[2916.14 --> 2916.86]  Oh, yeah.
[2917.26 --> 2918.62]  Yeah, my NVIDIA Shield, actually.
[2918.76 --> 2921.08]  I've just got the Shield app on my phone that I use all the time.
[2921.50 --> 2921.60]  Yeah.
[2921.76 --> 2922.84]  Yeah, that might be a problem.
[2923.76 --> 2924.50]  Should try it, though.
[2924.72 --> 2924.90]  Hey.
[2925.12 --> 2926.72]  Yeah, I would be interested to experiment with it.
[2926.78 --> 2927.64]  I actually do think fuzzy.
[2927.76 --> 2939.40]  I also think it's worth going the other direction, fuzzy, is could you come up with a system that you were happy enough with that you could then, you know, feel safe about putting your phone on your home Wi-Fi?
[2939.54 --> 2941.92]  Like, if you only used a VPN remotely?
[2941.92 --> 2942.04]  Absolutely.
[2942.34 --> 2943.50]  Here's the baller solution.
[2944.12 --> 2949.00]  One phone for the house, one phone for the world that's literally wrapped in tin foil.
[2949.70 --> 2950.52]  I love it.
[2950.98 --> 2951.34]  Yep.
[2951.52 --> 2953.64]  You got your going-to-town phone and you got your home phone.
[2953.80 --> 2954.10]  Yes.
[2954.30 --> 2955.30]  One is a flip phone.
[2955.44 --> 2955.98]  How about that?
[2957.42 --> 2959.60]  Eric sent in a row of ducks from the index.
[2959.70 --> 2965.14]  He says, hey, I've been using Obsidian over the past year, or about when you guys first started talking about it, and I've been enjoying it.
[2965.14 --> 2971.28]  I needed it to sync with iOS, and I had to have Wive Approval Factor, and I found the LiveSync plugin.
[2971.68 --> 2976.54]  It's just a plugin in Obsidian that syncs your notes across your devices using CouchDB as the backend.
[2976.80 --> 2978.86]  It also encrypts your data at rest.
[2979.20 --> 2985.84]  So if someone is on the fence about using the official sync and paying $8 a month, this can be a really good alternative.
[2986.14 --> 2987.44]  Again, it's called the LiveSync plugin.
[2987.88 --> 2992.56]  To offset this, though, I did make a contribution to Obsidian to continue supporting them on their development.
[2992.56 --> 3003.82]  You know, it's funny, I was just talking to a co-worker about Obsidian this week, and the $8, I think, you know, if they drop that price to $4 or $5 a month, they would have so many more users.
[3004.20 --> 3006.54]  But it is a little bit much for what it does.
[3006.82 --> 3007.36]  It is.
[3007.74 --> 3015.08]  And, you know, for those of us that are in the self-hosting mindset, you know, you think, oh, I can sync files between devices.
[3015.08 --> 3016.00]  It's easy.
[3016.54 --> 3025.44]  But then if you have every OS going, like in this house, I've got iOS, iPadOS, a Linux laptop, a MacBook, a Windows machine.
[3026.26 --> 3030.40]  Like, there's always some gotcha, and it's almost always an Apple gotcha.
[3031.18 --> 3034.52]  Like, the iOS backgrounding APIs are just crap.
[3034.92 --> 3038.24]  You know, I know they do it for battery life reasons compared to Android.
[3038.24 --> 3048.88]  I know why they do it, but the only solution that has worked 100% reliably for me with Obsidian, unfortunately, is their proprietary sync service.
[3049.34 --> 3056.10]  I would like to give this live sync plugin a go, though, because $8 a month, I'd prefer not to spend $8.
[3056.40 --> 3056.68]  Yeah, really.
[3057.06 --> 3057.20]  Yeah.
[3057.42 --> 3061.42]  Let us know, dear listener, if you've been using alternative sync solutions for Obsidian.
[3061.58 --> 3062.92]  How's that working out for you?
[3062.92 --> 3067.08]  How long have you been using it, and which OSs do you use it on?
[3067.72 --> 3070.02]  I'd love to get info on that, start collecting that information.
[3070.20 --> 3076.24]  Because, yeah, you know, the tricky thing, too, is my wife was like, maybe I want to get my own Obsidian going.
[3076.34 --> 3079.84]  It's like, well, do we pay $8 for her, too, now?
[3080.14 --> 3080.72]  Like, I don't know.
[3080.86 --> 3082.98]  So, I'd like to know what people are doing.
[3083.00 --> 3085.26]  You might get away with just a different vault each.
[3085.88 --> 3086.96]  Yeah, that's what we are doing now.
[3087.10 --> 3091.92]  And then encrypt that with a password that you each, well, probably husband and wife will share.
[3091.92 --> 3093.92]  Yeah, said passwords, but.
[3094.92 --> 3098.30]  Yeah, we're doing that now, but it's all under my account, because I didn't think about that initially.
[3098.46 --> 3100.16]  And so, she's like, well, what if I wanted my own account?
[3100.34 --> 3102.08]  I'm like, well, okay.
[3102.72 --> 3103.90]  Thank you, everybody, who boosted in.
[3103.92 --> 3104.88]  We had 10 boosters.
[3104.98 --> 3108.64]  Now, not all the boosts make it in every episode for runtime, but we do put those in the boost barn.
[3108.80 --> 3111.04]  And that's linked in the show notes, if you'd like to read through those.
[3111.08 --> 3112.22]  We also read through all of those.
[3112.26 --> 3115.66]  And we appreciate everybody who does take a moment to boost in.
[3115.66 --> 3116.46]  We had 10 boosters.
[3116.62 --> 3120.00]  58,346 sats were stacked.
[3120.00 --> 3124.46]  And if you'd like to boost in, go get a new podcast app at podcastapps.com.
[3125.00 --> 3126.46]  Fountain is just about to hit 1-0.
[3126.80 --> 3127.82]  Podverse is rocking.
[3128.00 --> 3130.88]  And if you're on iOS, Cast-O-Matic just keeps going from strength to strength.
[3131.26 --> 3131.76]  They're really great.
[3131.82 --> 3134.68]  Or you can boost from the index with something like Albie in your browser.
[3134.78 --> 3135.74]  Just get albie.com.
[3136.10 --> 3137.10]  We'll have links in the notes.
[3137.90 --> 3140.20]  And you know what else we should mention while we're talking about events?
[3140.20 --> 3145.72]  The original, the OG where you and I met, Texas Linux Fest, is coming up too.
[3146.32 --> 3147.66]  April 12th and the 13th.
[3147.72 --> 3148.40]  It's coming up fast.
[3149.02 --> 3149.24]  Yeah.
[3149.38 --> 3149.64]  Oh, boy.
[3149.66 --> 3150.52]  It's even less than what I put.
[3150.56 --> 3152.86]  Because I put this in there on Sunday, these numbers in there.
[3152.90 --> 3156.04]  So it's like 120 days away from when we were.
[3156.16 --> 3159.98]  It's going to be like 118 days or something like when this episode comes out.
[3160.14 --> 3160.90]  That's really soon.
[3160.90 --> 3165.90]  Austin in April, do you remember that first time we met was I think it was June or July?
[3166.14 --> 3166.76]  So hot.
[3166.76 --> 3168.42]  And we were in the conference center.
[3169.04 --> 3172.88]  And I didn't know you hardly at all, apart from listening to you for several years.
[3174.06 --> 3176.98]  And we were like, how far away is the barbecue joint?
[3177.18 --> 3178.82]  And someone was like, oh, it's a 10-minute walk.
[3178.84 --> 3181.44]  And we both looked at each other and were like, yeah, that'd be fine.
[3181.56 --> 3181.90]  Yeah, that's fine.
[3182.20 --> 3186.20]  Five minutes into this walk, both of our shirts are soaked with sweat.
[3186.44 --> 3189.36]  And we both looked at each other and went, that was a mistake.
[3189.94 --> 3190.10]  Yeah.
[3190.10 --> 3192.46]  We definitely didn't walk back, did we?
[3192.50 --> 3193.66]  We wrote with a listener, I think.
[3194.44 --> 3195.88]  I think that might have been my first time in Austin.
[3196.40 --> 3197.20]  I learned my lesson.
[3197.58 --> 3198.26]  I'll tell you what.
[3198.44 --> 3198.62]  Yeah.
[3199.50 --> 3201.72]  And now in April, it's going to be wonderful.
[3201.90 --> 3204.62]  It's going to be perfect, especially coming from here in the Pacific Northwest,
[3204.74 --> 3207.30]  where I won't have seen sunlight for four months by that point.
[3207.88 --> 3208.80]  It's going to be wonderful.
[3208.80 --> 3214.96]  And then LinuxFest Northwest, everybody's favorite conference, is officially back again.
[3216.10 --> 3216.30]  Yep.
[3216.34 --> 3219.28]  And this one will be in April, April 26th through the 28th,
[3219.28 --> 3220.70]  when it is starting to get nice here.
[3220.84 --> 3223.52]  And they have the call for sessions going over there as well.
[3223.74 --> 3230.36]  And Alex, I would really like to see the self-hosted community fill up some of those sessions.
[3230.90 --> 3235.62]  Because there's just not enough self-hosting and sovereignty and cool things you can do
[3235.62 --> 3237.30]  in your home lab talks at these events.
[3237.30 --> 3238.00]  We need more.
[3238.72 --> 3242.08]  If you're on the fence about what you want to talk about, please reach out to me on the Discord,
[3242.24 --> 3243.44]  AlexKTZ over there.
[3243.54 --> 3250.78]  I'd happily help you craft a submission or a topic or, you know, even just work out what the idea,
[3251.04 --> 3252.56]  you know, the nugget of an idea might be.
[3253.00 --> 3253.48]  That's all been nice.
[3253.52 --> 3254.30]  I think that'd be great.
[3254.40 --> 3257.82]  Gosh, I'd love to see some serious self-hosted sessions there.
[3258.32 --> 3260.68]  I will have links to those in the notes as well.
[3260.68 --> 3266.26]  And I just want to take a moment before we get out of here and say thank you very, very much to our members.
[3266.52 --> 3272.36]  We have our self-hosted reliability engineers over at selfhosted.show.sre.
[3272.90 --> 3277.78]  And it's a great way to support the show directly, keep the show independent and honest,
[3277.84 --> 3278.86]  making you our biggest customer.
[3279.00 --> 3284.08]  And we give you an ad-free version of the show with some bonus content as a thank you.
[3284.46 --> 3287.16]  That's at selfhosted.show.sre.
[3287.16 --> 3292.76]  You can become one of our sites, Reliability Engineers, and keep the show on the road.
[3293.32 --> 3294.30]  We do truly mean it.
[3294.52 --> 3301.40]  You know, next year, the adpocalypse that Chris has been talking about for a long time is really starting to bite.
[3301.54 --> 3304.86]  I mean, we were just looking at Leo Laporte over at twit.tv.
[3305.20 --> 3305.54]  Sad.
[3305.66 --> 3309.42]  Talking about, yeah, talking about some serious financial issues over there potentially.
[3309.86 --> 3313.48]  So the market's not looking good for any podcast, I think, in 2024, Alex.
[3313.50 --> 3314.08]  It's pretty sad.
[3314.44 --> 3316.28]  It's going to be a bumpy year, probably.
[3316.28 --> 3323.94]  So, you know, if you like independent media and want to keep shirt on Chris's back, you know.
[3324.56 --> 3330.38]  You know, I think, too, it's like the thing we're getting at with podcasts is they're kind of a unique beast when you look at the media landscape.
[3330.52 --> 3332.28]  They're nothing like TV or radio anymore.
[3332.90 --> 3337.86]  YouTube is independent in a way, but it's also there's a lot of commercial influence and interest over there.
[3337.86 --> 3340.60]  And it's just a really different kind of dynamic.
[3341.34 --> 3345.34]  Podcasting is this truly unique, decentralized beast.
[3345.82 --> 3349.38]  We don't really have anything where there's no company that owns podcasting, right?
[3349.40 --> 3355.26]  There's no central platform that manages and controls and moderates podcasting.
[3355.38 --> 3356.50]  That is so unique.
[3356.76 --> 3358.56]  If you have tried, I mean, Spotify.
[3358.90 --> 3358.96]  Yeah.
[3359.42 --> 3359.54]  Yeah.
[3359.54 --> 3360.06]  Blimey.
[3360.20 --> 3361.26]  They tried and failed.
[3361.48 --> 3364.52]  It's just you'd hate to see something like that go away.
[3365.06 --> 3365.40]  Indeed.
[3365.60 --> 3365.96]  Indeed.
[3366.54 --> 3372.90]  So, you know, I'm in such a privileged position because I have a jobby job, which, you know, pays the bills and stuff like that.
[3373.04 --> 3376.40]  But, you know, JB is a small independent business.
[3376.66 --> 3383.66]  And if you are feeling a little extra generous this Christmas, we'd love to see a bit of your extra support come our way.
[3383.66 --> 3383.94]  Yeah.
[3384.66 --> 3389.56]  And we'd be happy to give you a extra little bonus content at the end of the show as a thank you.
[3389.88 --> 3391.16]  Self-hosted.show slash SRE.
[3391.60 --> 3392.20]  Thank you, everybody.
[3392.68 --> 3394.64]  And don't forget about our upcoming meetups.
[3394.76 --> 3398.32]  I think our good buddy Brent is in Berlin again right now.
[3398.72 --> 3400.74]  Meetup.com slash Jupiter Broadcasting.
[3400.92 --> 3401.88]  Keep an eye on that page.
[3402.28 --> 3403.16]  He's at Seabase.
[3403.28 --> 3406.86]  I think it was a couple of days ago with a little impromptu meetup.
[3407.00 --> 3408.30]  So just keep it on that page.
[3408.34 --> 3411.82]  It's always updating and you might get to meet one of us.
[3411.82 --> 3412.18]  Yeah.
[3412.56 --> 3416.68]  You know, with Scale and Linux Fest coming up and Texas Linux Fest, there's probably going to be some activity on there.
[3417.10 --> 3425.94]  I think I might just move to the West Coast for the spring because I'm going to be in L.A. for a couple of weeks and then Austin for a few days and then Seattle, you know.
[3426.44 --> 3427.32]  I got a couch for you.
[3427.38 --> 3429.56]  It's hardly worth flying back to Raleigh for, right?
[3430.62 --> 3431.68]  Just bring the fam out.
[3432.96 --> 3434.34]  We'll put them all up on a couch.
[3434.36 --> 3434.82]  You joke.
[3434.82 --> 3441.06]  I am seriously thinking about just renting an Airbnb in L.A. for Scale and just bring Edna and Catherine with me.
[3441.06 --> 3441.18]  Yeah.
[3441.60 --> 3441.88]  Yeah.
[3442.12 --> 3442.36]  Yeah.
[3443.00 --> 3443.80]  It's kind of fun.
[3444.32 --> 3446.60]  I mean, it's kind of, if you can, it's kind of neat to be able to take family.
[3447.26 --> 3447.56]  All right.
[3447.88 --> 3452.56]  Well, if you'd like to get links to what we talked about today, head over to selfhosted.show slash 112.
[3453.76 --> 3457.40]  And, of course, you'll find our contact page, RSS feed and all that good stuff over there as well.
[3457.76 --> 3460.72]  Selfhosted.show slash contact is the place to go to get in touch with us.
[3461.12 --> 3464.18]  You can find me at alex.kdz.me.
[3464.18 --> 3465.00]  Oh, yeah.
[3465.08 --> 3465.32]  Okay.
[3465.44 --> 3465.76]  All right.
[3465.82 --> 3466.98]  I'll be at chrisles.
[3467.24 --> 3467.74]  How about that?
[3468.12 --> 3472.68]  You still on the Twitter ex-fire train dumpster fire bomb, are you?
[3473.20 --> 3473.70]  Kind of.
[3473.88 --> 3474.94]  I mean, I'm kind of everywhere.
[3476.16 --> 3477.04]  Sort of a ghost.
[3477.40 --> 3478.38]  Thanks for listening, everybody.
[3478.54 --> 3480.76]  That was selfhosted.show slash 112.
[3480.76 --> 3481.06] 怎麼one02.
[3482.94 --> 3483.86] andelion.
