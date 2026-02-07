[0.00 --> 5.78]  Happy holidays, listener. We have a special episode for you this week. Some old friends
[5.78 --> 9.86]  join the show for a 3D printing special with Alex.
[11.72 --> 17.60]  Well, I'm joined today by a couple of special guests, long-time JB friends and former colleagues,
[18.02 --> 21.58]  I suppose. We've got Cheese on the line. Hey, Cheese, how you doing?
[22.06 --> 22.94]  Hey, hey, how's it going?
[23.24 --> 23.86]  And Drew.
[24.30 --> 24.70]  Hello.
[25.22 --> 29.50]  Both of you are now in Colorado. You're both in Denver, serendipitously, I suppose.
[29.50 --> 29.60]  Thank you.
[30.00 --> 33.40]  Cheese, you're working for System76 these days. And what about you, Drew?
[33.84 --> 41.96]  I am working for the Community College System. So we handle basically high-end IT and server
[41.96 --> 45.14]  needs for 13 different colleges across the state.
[45.70 --> 48.14]  And you do chew my ear off about OpenShift on occasion.
[48.46 --> 49.30]  Every now and then, yeah.
[49.54 --> 52.96]  It has been known. What about you, Cheese? What are you doing for System76?
[53.92 --> 58.56]  Right now, I'm working with the marketing department, doing videography, photography,
[58.56 --> 63.58]  some animation, graphic design stuff, all sorts of fun, cool things.
[64.02 --> 68.96]  I feel like breaking out into Troy McClure at this point, you may remember Cheese from shows
[68.96 --> 74.08]  such as the Friday Stream and all sorts of other. Linux Unplugged, all sorts of stuff.
[74.16 --> 77.24]  If you're a long-time JB listener, these two guys will be very familiar to you.
[77.24 --> 83.20]  So I've got these two today to talk to you all about 3D printing. This is a topic that we covered
[83.20 --> 89.30]  very briefly in an episode of Self-Hosted recently. And lots of feedback came my way that you'd like
[89.30 --> 95.08]  a bit more information. So I have two guys that are at different points in their 3D printing journey.
[95.08 --> 101.48]  So just very quickly, Drew, perhaps you could give us a very quick overview of where you're at in
[101.48 --> 108.68]  your journey and that kind of thing. Sure. So just a few months ago, I purchased my first 3D printer
[108.68 --> 117.58]  and have been kind of getting up to speed since then. It's a smaller unit. We'll talk more about
[117.58 --> 125.72]  the actual gear a little later, but it's a very much the beginner's entrance style unit that one
[125.72 --> 130.94]  might pick up. It's not super fancy. So you're looking at this discussion through the lens of
[130.94 --> 134.94]  someone that's been printing for a few months. And what about you, Cheese? Where are you at in your
[134.94 --> 141.22]  journey? Well, I've been printing now for a couple of years after encouragement. I believe it was from
[141.22 --> 146.48]  LinuxFest Northwest where we all met up and you had printed some things,
[146.48 --> 152.90]  which encouraged me just to bite the bullet and buy a printer. And so I've been using basically
[152.90 --> 158.42]  the same printer as Drew for quite some time and over the last couple of years and learned that I
[158.42 --> 163.40]  enjoyed the hobby. So I want to expand that and picked up a new printer recently. Yeah, I think I
[163.40 --> 169.38]  3D printed a carabiner clip to hold my luggage together or something. Yeah, I believe it was that.
[169.74 --> 176.04]  And you had also printed the on-air signs that were powered by the- That's right, yeah.
[176.04 --> 180.42]  The little Node MCUs. Those things are so cool. Yeah, I think that's what pushed me over the edge.
[181.54 --> 186.16]  Well, I'm glad you liked them. Of course, they're running WLED. So, you know, I hope you've been
[186.16 --> 190.78]  keeping them up to date. There's lots of new features on that stuff these days on the ESP side
[190.78 --> 198.68]  of things. I mean, so I've been 3D printing a little bit off and on for four, I guess, years.
[198.68 --> 205.98]  Quite a long time, I guess. I got into it through wanting to print little parts for my racing drones.
[206.30 --> 212.00]  You know, the perfect use case for me was to print custom holders for all the little tiny circuit
[212.00 --> 218.58]  boards that go into an FPV racing drone. And so I learned very basic CAD skills, computer-aided design
[218.58 --> 224.92]  skills, you know, through stuff like Tinkercad and Fusion 360. I am not very good, but, you know,
[224.92 --> 232.06]  I can print a 3D print a cube or a little square box I made for something easily enough. And so,
[232.18 --> 236.92]  you know, I've had a probably three or four prints. I think I'm on my fourth printer now.
[237.40 --> 242.50]  I've had some of the cheap Chinese ones and I've got Prusas these days, but we'll come on to that
[242.50 --> 247.72]  stuff a bit more later. But first of all, I thought it might be helpful to sort of talk about what is
[247.72 --> 252.02]  3D printing a little bit for those that aren't familiar with it. Would either of you two like to
[252.02 --> 260.40]  take that mantle? I feel like as the junior here that you as the senior printer should take that,
[260.62 --> 268.38]  but... All right, fine, fine, fine. Okay, so what we call 3D printing is actually technically probably
[268.38 --> 273.34]  referred to, it's a bit like calling a Docker container a container and Linux container, like
[273.34 --> 278.44]  it's that whole Kleenex debate, right? So what we're actually talking about is what's called FDM
[278.44 --> 284.48]  printing, fused deposition modeling. And essentially what that does is it takes a spool of plastic
[284.48 --> 289.94]  filament, it can be of different materials. So there's three main types that I print with,
[290.46 --> 296.66]  I'll come on to those in a moment. But essentially what FDM printing does is it takes in a spaghetti
[296.66 --> 305.18]  sized piece of plastic, forces it through what's called a hot end, melts that plastic at 220-ish
[305.18 --> 310.92]  Celsius. It varies on the different filament that you use, the chemical properties of that filament.
[311.86 --> 316.90]  So it takes that filament in through a drive gear, squishes it through the hot end, melts it,
[317.42 --> 323.80]  and then the pressure of the drive gears forcing that filament through forces it out of what's called
[323.80 --> 329.72]  a nozzle at the bottom of your hot end. And so the hot end is the thing that contains the thermistor
[329.72 --> 333.66]  and it's what contains the chamber where the melted plastic is and all that kind of stuff.
[334.42 --> 338.80]  And right at the very end of the process is the nozzle, which is what, you know, if you've ever
[338.80 --> 346.32]  watched a video of a 3D printer printing, it's that kind of nozzle shaped thing, funnel shaped thing
[346.32 --> 353.92]  on the bottom where the plastic actually gets extruded out of. And essentially the basic premise is
[353.92 --> 361.18]  you can use what's called G-code to move stepper motors left and right, up and down, forwards and
[361.18 --> 367.78]  backwards. You can use G-code to control the movement of that nozzle such that it will form layers of
[367.78 --> 375.64]  plastic. You know, we're talking an extruded line of plastic will be half a millimetre wide, a millimetre
[375.64 --> 382.34]  wide at most. And what it will do is it will build up layer upon layer upon layer of plastic to form models.
[382.34 --> 387.88]  It has some limitations. Obviously you can't print stuff with certain overhangs in certain shapes
[387.88 --> 395.14]  because the layer by layer construction of these things presupposes that there is a support underneath.
[395.34 --> 399.56]  So there's all sorts of different ways you can get around that by including supports in your models
[399.56 --> 404.48]  and things like that. But ultimately there are some shapes that just aren't very well suited to 3D
[404.48 --> 410.42]  printing. You know, a complete sphere would be quite tricky because it wouldn't be able to stick to
[410.42 --> 415.72]  what's called the print bed. And so one of the most difficult parts of 3D printing, which I'm sure
[415.72 --> 420.64]  both of you can attest to, is that first layer adhesion.
[422.20 --> 427.36]  Definitely. I know whenever I first started, layer adhesion was definitely a thing for me.
[427.80 --> 434.60]  I was using the inexpensive removable bed that came with my printer and quickly found out that that
[434.60 --> 439.80]  probably wasn't the best idea, especially after cracking off one print and then kind of putting a
[439.80 --> 442.00]  crease in part of the removable bed.
[442.52 --> 446.30]  Well, you're doing better than me. I had a Creality CR10 as my first printer.
[446.84 --> 451.92]  And I went to Ikea and purchased a mirror tile, which is I think about 12 inches square.
[452.58 --> 457.08]  And I actually had something stick to the glass so hard that when I was trying to unstick and
[457.08 --> 460.82]  unpeel this damn thing, that the print actually smashed the mirror when I was...
[461.46 --> 461.98]  Wow.
[462.28 --> 462.38]  Wow.
[462.38 --> 463.94]  Took a chunk of glass with it.
[464.60 --> 468.80]  That's impressive. Yeah. I mean, I was able to get mine leveled out pretty good,
[468.90 --> 470.96]  but I definitely had to go to a glass bed.
[471.54 --> 480.10]  So even with the original mat that came with my Ender 3, I honestly didn't have many adhesion
[480.10 --> 486.62]  problems with PLA, which, you know, we'll get into the types of plastics that you can use, but
[486.62 --> 493.90]  PLA I had no trouble with. It's when I started going on to more exotic filaments that I'm using now
[493.90 --> 499.20]  that I really started having adhesion problems. And fortunately, I was finally able to suss them
[499.20 --> 503.88]  out. But it's taken some time and a lot of experimentation to get there.
[503.88 --> 511.22]  It does. I think we should dispel the myth right now that 3D printing is out of the box, ready to go
[511.22 --> 515.22]  hobby. You know, it's not like you can go to Best Buy and buy a 3D printer like you could,
[515.74 --> 521.02]  you know, a paper printer, for want of a better word, and just press go and expect it to work
[521.02 --> 527.12]  first time every time. That's just not the reality. They are very finely toleranced machines. We're
[527.12 --> 532.56]  talking microns of a millimeter makes a big difference to how well a layer sticks or doesn't.
[532.66 --> 537.04]  You know, a few particles of dust can make the difference between a print sticking or not.
[537.56 --> 543.30]  Well, and it's not just that. There are so many different things that can really matter here, like
[543.30 --> 547.68]  the temperature that you have the filament coming out at, the temperature that you have the bed
[547.68 --> 553.52]  sitting at, whether or not it's in an enclosure, depending on what type of material it is.
[553.52 --> 559.60]  There are so many different variables that you can mess up and just totally throw off the whole thing.
[560.36 --> 565.32]  All right, so let's break down the filaments for a second. We mentioned PLA. That's probably the most
[565.32 --> 569.06]  beginner-friendly one that's available and probably the most popular, to be honest.
[569.96 --> 575.62]  PLA has a few interesting characteristics. First of all, it's very easy to work with. There's very
[575.62 --> 582.54]  little in the way of stringing. It doesn't require a particularly sticky bed in order to adhese properly.
[582.54 --> 587.56]  But it can be quite brittle. So for stuff like my racing drone parts, for example,
[588.08 --> 592.80]  when it got a bit cold outside, I'd slam my drone into a tree or something and the stuff would just
[592.80 --> 598.90]  snap. It would just crack. So it's good for sort of indoor stuff like plant pots or, you know,
[598.96 --> 603.44]  I've got a rocket lamp behind me that I 3D printed, for example. So a Saturn V rocket.
[603.76 --> 607.40]  It's good for that kind of stuff where there's very little load and very little stress
[607.40 --> 613.72]  on the print. But if you're wanting to do anything where heat is an issue, you know,
[613.82 --> 618.76]  let's say you're printing a bracket for your car, you know, another 3D print I've done,
[618.80 --> 626.56]  a functional print is a dash cam bracket for my car. And, you know, a car in the south of the
[626.56 --> 631.42]  United States gets pretty warm in the summer. I'm talking to a Texan. I'm well aware that you
[631.42 --> 636.36]  guys get warm too. But you know what I'm saying, right? If you were to try and use PLA in that
[636.36 --> 641.36]  environment, very quickly that plastic would get to what it's called its glass transition point
[641.36 --> 646.90]  and start softening drastically. And eventually, you know, if it's under any kind of load,
[647.08 --> 652.94]  even if it's just from a dash cam, you know, a few grams, it would start to warp and twist and
[652.94 --> 653.76]  eventually melt.
[653.76 --> 659.54]  Yeah. And I think that that depends on your print too, because a print that I had made for
[659.54 --> 664.98]  some friends, they had an above ground pool. And on that pool was a railing that, I don't know,
[665.36 --> 671.76]  you know, what the diameter of that railing, but they had no cup holders, right? So everyone was
[671.76 --> 676.80]  trying to figure out like, where do I set my drink down? So I made some cup holders and it just had
[676.80 --> 682.20]  these little hooks that hooked over the top of the ring on the pool and was able to, you know,
[682.20 --> 690.04]  put your drink there. And they probably sat out there for a little over a year before one of
[690.04 --> 694.88]  them finally failed. And one of the little arms had cracked. And I don't know if that's because
[694.88 --> 701.80]  somebody bumped it or how it happened, but it can hold up to some extent, but under a magnified
[701.80 --> 706.66]  windshield in the heat, direct heat, probably not the best.
[706.84 --> 711.22]  Yeah. There's no chances there. So for that kind of application, you want to be looking at
[711.22 --> 717.06]  something called PETG. There are a few other types that are suitable for sort of higher
[717.06 --> 722.64]  temperature environments, but PETG in particular is one of my go-tos. It's sort of chemically
[722.64 --> 729.38]  related to PLA. So it takes the best bits of PLA and another plastic called ABS, which is famously
[729.38 --> 735.60]  difficult to print and work with because of things like warping, which is where during a print,
[735.60 --> 741.88]  the corners of a print will lift. And then the entire model is put under intense stress and it
[741.88 --> 749.44]  can start to crack and all that kind of stuff. But PETG is probably the best of both worlds. It's got
[749.44 --> 757.58]  pretty much the same ease of printing as PLA and almost the same heat resistant characteristics as ABS.
[757.58 --> 765.36]  The downside to PETG is it can be a very sticky thing indeed. That was the filament that stuck to
[765.36 --> 770.74]  my glass bed and took a chunk of glass with it, for example. So chemically, it's very good at bonding
[770.74 --> 776.92]  with the build layer, the build surface on certain printers. So for my Prusa behind me, for example,
[776.92 --> 781.92]  I actually have two separate sheets. I have a texture sheet from Prusa, which is actually designed
[781.92 --> 788.56]  for PETG and a separate one for PLA, just so that I have that separation of concerns. I don't have to
[788.56 --> 792.70]  worry about glue sticks or any other kind of nonsense or tape or anything like that.
[793.16 --> 799.62]  It's worth mentioning too, that PETG is the slightly more exotic material I referenced earlier that I
[799.62 --> 806.30]  was moving towards and was having adhesion issues. It does require more heat than PLA to really get it
[806.30 --> 813.52]  to flow nicely. And you also can't print as fast because, you know, to get it to where it's flowing
[813.52 --> 819.16]  well, if you get it flowing too well, then it bubbles. And there's, you know, you need a hotter
[819.16 --> 824.70]  bed to really get it to stick well. And it's just, it's a lot more finicky, but not as finicky as
[824.70 --> 828.62]  something like ABS or anything like that. Yeah.
[828.62 --> 835.94]  So we're talking about with, with PLA, for example, that prints, the nozzle is around the hot end,
[836.04 --> 844.10]  sorry, is around 180 Celsius. And typically I run my bed at around 60 Celsius with PETG. I can run my
[844.10 --> 850.82]  hot end anywhere from 220 to 250, depending on the particular filament properties. And the bed is
[850.82 --> 856.38]  anywhere from 80 to 90 degrees Celsius. So there's a good step up there in the temperature and therefore
[856.38 --> 861.10]  energy required to use this filament. But that's why it performs better in, you know,
[861.16 --> 867.04]  heat sensitive environments. Speaking of, you know, different filaments from different
[867.04 --> 874.36]  manufacturers can have vastly different responses. Like I'm using various filaments from Micro Center
[874.36 --> 881.60]  and I have my bed turned up to about a hundred. I find it works a little better, but I can print with
[881.60 --> 888.80]  the PETG itself down at about 230, which is the low end of what Micro Center actually recommends for
[888.80 --> 895.26]  that filament. Really, it just depends. Yeah. Most manufacturers will print a recommended set of
[895.26 --> 900.92]  settings on the side, and that's generally a good place to start. But you will need to start printing
[900.92 --> 905.92]  things like calibration cubes and, you know, temperature towers and torture tests and all this
[905.92 --> 910.52]  kind of thing. If you're moving to a completely new supplier of filament and you're not seeing the
[910.52 --> 915.20]  results you would expect, there's all sorts of things on a website called Thingiverse that you
[915.20 --> 922.12]  can actually download for free to import into your printer's slicer software and send across to the
[922.12 --> 929.76]  printer. So speaking of slicers, Cheese, we haven't really touched on that much at all yet. Would you like to?
[930.12 --> 936.90]  Yeah. So a slicer is basically exactly what it sounds like. As Alex had mentioned earlier,
[936.90 --> 944.62]  with FDM, you're laying down layer by layer. So a slicer will take your 3D model and separate it
[944.62 --> 952.74]  layer by layer, drawing the path and or creating the G-code that allows the printer to know in X,
[952.80 --> 959.14]  Y, and Z in space where the nozzle needs to be at any given time. And then once you've taken your
[959.14 --> 963.92]  model and you've sliced it, then you can import that G-code directly into your printer and print your
[963.92 --> 969.72]  model. So there are a couple of different pieces of software. Cura, which is one that I'm a little
[969.72 --> 978.80]  more familiar with. That's C-U-R-A. It's really great. And then Prusa, the manufacturer of 3D printers
[978.80 --> 985.46]  actually has their own piece of software. I think they, it's a fork of slicer was the original name.
[985.64 --> 990.06]  And now it's just referred to as Prusa slicer. But it's kind of the de facto for them.
[990.06 --> 993.40]  It's spelt slick 3R if you're looking for it on the internet.
[993.42 --> 998.00]  Yeah, slick 3R. Yeah, that's it. It's LeetSpeak spelt, right? But yeah, it's, it's,
[998.10 --> 1003.58]  it's, it's a great one as well. And I'm, I'm learning more of that now that I've, I've purchased
[1003.58 --> 1011.66]  a Prusa printer, but Cura is also fantastic. And there are a lot of settings that you can take
[1011.66 --> 1018.68]  from other resources. So I know Chep is, is one of the guys I took, um, his, uh, his settings,
[1019.02 --> 1024.66]  uh, for Cura originally. And, you know, they worked really well for me better than the stock settings
[1024.66 --> 1027.82]  that were, that were suggested by Cura itself. So.
[1029.10 --> 1034.12]  So I'm pretty curious, uh, to, to know how the humidity has affected you. Cause I know you've just
[1034.12 --> 1039.86]  moved from Texas to Colorado, but obviously there's a drastic humidity difference between the Gulf
[1039.86 --> 1046.78]  coast and the Colorado air and, and PETG is famously hygroscopic. So what that means is it
[1046.78 --> 1050.66]  will absorb water from the air around it. So, you know, me and Raleigh, for example,
[1050.66 --> 1056.34]  with my relatively high humidity, I have to keep my filament in a dry box full of silica gel in order
[1056.34 --> 1061.84]  to try and keep it relatively usable. I was wondering, have you noticed any difference in how you store
[1061.84 --> 1067.90]  your filaments and how easily they print or not at the different altitudes and humidity levels?
[1067.90 --> 1075.16]  Well, for me, I haven't really experimented with much outside of PLA. So, um, I know the PETG,
[1075.34 --> 1082.08]  like you said, has, has a lot more, uh, is hydroscopic as you mentioned. Um, but I will say
[1082.08 --> 1089.02]  that with PLA, I have noticed that moving from Texas, uh, along the Gulf coast to here in Colorado,
[1089.02 --> 1099.68]  um, even the PLA, it gets more, it gets more brittle than normal. Um, so I, it's not like I
[1099.68 --> 1107.04]  keep it in a humidifier or something, but, uh, once I get through the batch of filament that I have
[1107.04 --> 1112.54]  now and I move over to PETG, I'll know a little bit more, but so far the humidity and the change in
[1112.54 --> 1118.02]  humidity has affected the PLA, but not significantly to the point where I can't print with what I have.
[1118.02 --> 1120.54]  So how about you, Drew, how's your experience been?
[1121.62 --> 1127.82]  So, you know, I've only been doing this a few months. I'm not sure how quickly PETG under
[1127.82 --> 1134.84]  circumstances like yours, Alex would, would really take on enough water to need to be dried before
[1134.84 --> 1136.12]  printing, but.
[1136.72 --> 1141.66]  Could be a month. It could be three or four months. I mean, it really depends. Like for example,
[1141.66 --> 1144.98]  you were, you were living in Georgia before and now you're in Colorado.
[1144.98 --> 1150.82]  Right. Similar thing as cheese, really, you know, an ocean level of Gulf humidity moving up to the
[1150.82 --> 1151.86]  mountains, you know, so.
[1151.94 --> 1161.40]  Right. So here I have had my PETG sitting out for a while and I've also, I keep it in a box most of
[1161.40 --> 1167.62]  the time, but I don't like after a print is finished, heat up the end and pull the filament
[1167.62 --> 1172.08]  and put it back in the box. I tend to just kind of leave it on the roll.
[1172.58 --> 1176.82]  You should be fine where you are now. I mean, I was wondering whether you'd noticed any difference
[1176.82 --> 1181.20]  in terms of how, because I know, for example, things like boiling a kettle takes longer altitude
[1181.20 --> 1183.78]  and, you know, baking recipes are slightly different.
[1184.12 --> 1192.48]  Yeah, exactly. So no, I haven't had any issues just leaving my PETG on the roll for weeks.
[1194.52 --> 1195.40]  Still prints fine.
[1196.60 --> 1197.20]  All right.
[1197.62 --> 1204.32]  Well, talking of software, we mentioned Prusa Slicer and Cura. Those are the two main slicers.
[1204.84 --> 1208.44]  There's another piece of software that I think everybody ought to know about called Octoprint.
[1209.12 --> 1210.32]  Wonderful piece of software.
[1210.68 --> 1211.82]  It's like the best thing.
[1212.14 --> 1212.58]  Wonderful.
[1213.18 --> 1219.50]  Seriously, if you are getting into 3D printing, just, yeah, do yourself a favor and Google Octoprint.
[1219.50 --> 1232.40]  It is something that you install on like a Raspberry Pi and you connect it to your printer via the USB slot and then you can control your printer remotely.
[1232.40 --> 1237.26]  It is damn near necessary for anybody who's really going to do this as a hobby.
[1237.26 --> 1242.34]  You really need a way to be able to touch your printer without having to walk to it.
[1243.00 --> 1243.36]  Absolutely.
[1243.36 --> 1244.40]  I totally agree.
[1244.74 --> 1248.40]  I have a Pi 4 running my Octopi instance.
[1248.84 --> 1257.52]  So the piece of software is called Octoprint, but the developer of Octoprint makes available a build for the Raspberry Pi called Octopi,
[1257.52 --> 1262.30]  making the Raspberry Pi ecosystem almost synonymous with 3D printing in my opinion.
[1262.98 --> 1266.68]  And I actually use that to run the Python application, which is Octoprint.
[1266.86 --> 1268.82]  There are a bunch of different plugins you can get.
[1268.90 --> 1278.18]  So for example, I have one that's called Spaghetti Detective, which looks at my webcam feed and tries to use machine learning to try and figure out if my print has come unstuck for any reason.
[1279.04 --> 1279.92]  That's a fun one.
[1279.92 --> 1281.80]  There's another one that does Telegram integration.
[1282.08 --> 1286.22]  So I get notifications and I can control my printer via Telegram bot.
[1286.22 --> 1288.46]  I can get GIFs as well, all that kind of stuff.
[1288.94 --> 1290.08]  There are hundreds of plugins.
[1290.20 --> 1291.40]  We couldn't possibly list them all.
[1291.92 --> 1293.48]  MQTT is another one.
[1294.14 --> 1295.82]  Yeah, MQTT is awesome.
[1296.10 --> 1297.54]  The timelapse plugins.
[1298.12 --> 1299.44]  Yes, that one is great.
[1299.52 --> 1303.26]  The webcam plugin, just in general, to let you monitor in real time.
[1303.88 --> 1305.70]  There's even cost estimation plugins.
[1306.48 --> 1314.92]  So based on the G code that you provided, it will estimate how many grams of filament and how much that filament costs and therefore how much a print's going to cost.
[1314.92 --> 1322.58]  So there are a lot of things in Octoprint that there's really nothing out there that compares to it that I've seen.
[1323.00 --> 1330.90]  And it's probably one of the best uses for a Raspberry Pi, especially if you have, well, specifically if you have a 3D printer.
[1331.72 --> 1332.62]  For sure.
[1333.02 --> 1335.36]  Now, I would probably suggest running it on a Pi 4.
[1335.36 --> 1344.36]  I've been running it on a Pi 3B Plus for a year or two, but I upgraded about six months ago to a Pi 4, and it's night and day difference.
[1344.48 --> 1350.00]  It's so much faster, and I would highly recommend a Pi 4 as a baseline if you're just getting into this.
[1350.48 --> 1357.26]  So a few months ago, everybody from JB came out to Denver, and we all had a jolly good time.
[1357.26 --> 1365.26]  But Linode was giving away Raspberry Pis at our little meetup, and I managed to win one, right?
[1365.84 --> 1366.70]  Yeah, you did.
[1366.92 --> 1369.44]  That's what my Raspberry Pi from Linode is doing.
[1370.54 --> 1371.06]  Awesome.
[1371.74 --> 1372.00]  Rad.
[1373.00 --> 1378.72]  So the final filament I think is worth talking about is TPU, which is a flexible filament.
[1378.88 --> 1381.10]  Have either of you experimented at all with flexes?
[1381.64 --> 1382.46]  Not yet.
[1382.60 --> 1385.22]  Looking forward to it, though, but not quite yet.
[1385.48 --> 1385.70]  Yeah.
[1385.70 --> 1386.80]  It's a world of pain.
[1387.12 --> 1387.86]  Not at all.
[1388.04 --> 1395.70]  I mean, I'm familiar with TPU in that I've purchased phone cases before, but as far as actually making it myself, no, I haven't.
[1396.54 --> 1404.54]  So with the Creality CR10 I used to have in London, I was printing a lot of drone parts, as I said, which included stuff like GoPro mounts.
[1404.54 --> 1410.52]  Like I say, when I smashed into a tree, I wanted some give in the part, so it didn't just smash into a thousand pieces.
[1410.52 --> 1427.24]  And with the CR10, it had what's called a Bowden tube extruder, which essentially means that the gearing which feeds the filament into the hot end is on the main body of the printer connected to the extruder via plastic or nylon tube.
[1427.24 --> 1430.58]  Whereas the Prusa has what's called a direct drive extruder.
[1430.58 --> 1447.32]  And I've had a lot of success 3D printing with the flexible filaments on the Prusa simply because there's a lot less chance for a flexible filament to kind of collapse on itself and start tying itself in knots like spaghetti on the direct drive printers.
[1447.32 --> 1458.06]  Yeah, I haven't had much experience, actually no experience with TPU yet, but from what I've heard, the direct drive is kind of the way to go for that.
[1459.10 --> 1467.50]  Because, and depending on the extruder itself, right, the extruder itself can have one gear or multiple gears in it.
[1467.50 --> 1478.56]  So with multiple gears, you're able to pull filaments that are maybe a little bit more difficult to pull through and through the hot end and out the nozzle.
[1478.82 --> 1480.56]  So I'm looking forward to it.
[1480.64 --> 1483.68]  I kind of want to print my own phone case, but we'll see.
[1484.18 --> 1488.56]  I don't want to buy a whole roll and then just be sad because I can't print with it.
[1488.66 --> 1490.46]  And now I have a whole roll of TPU.
[1490.84 --> 1494.86]  One thing I will say is TPU is incredibly hygroscopic.
[1495.12 --> 1496.70]  So just bear that in mind.
[1496.70 --> 1500.98]  There are some more exotic filaments, you know, there's carbon fiber based ones.
[1501.10 --> 1506.16]  But once you start getting out of those main three that we talked about, so PLA, PETG and TPU,
[1506.80 --> 1513.18]  once you go outside of those three mainstream ones, there are significant compromises to be made with all the different other plastics that are available.
[1513.56 --> 1515.46]  There are too many for us to get into today.
[1516.04 --> 1520.16]  But that's an overview of most entry level filaments for most beginners.
[1522.52 --> 1524.22]  Leno.com slash SSH.
[1524.22 --> 1527.34]  Go there to get $100 and 60 day credit on a new account.
[1527.54 --> 1529.12]  And you go there to support the show.
[1529.22 --> 1532.90]  What I love about Linode, straight up, it's fast, reliable cloud hosting.
[1533.16 --> 1534.78]  And you should really go try it for your next project.
[1535.10 --> 1539.30]  It also makes for great R&D if you want to learn something and spin it up super quick.
[1539.62 --> 1543.50]  I guess back in the day, I used to fuss a lot more with VMs on my workstation.
[1543.50 --> 1547.96]  But these days, I just jump on the Linode dashboard and I get it going in no time.
[1548.02 --> 1554.92]  And one of the things I love is when I'm setting up a system, you can actually get console access through an SSH session.
[1555.10 --> 1557.30]  They even just give you the command right there in the dashboard.
[1557.50 --> 1560.92]  You highlight that, copy that thing, post it into your terminal.
[1561.24 --> 1567.44]  You hit that sucker in and then you're actually like in an SSH session looking at the console of your Linode machine.
[1567.76 --> 1568.76]  It's awesome.
[1569.16 --> 1572.24]  It's just those kinds of things that make it fun for when you really want to get down deep.
[1572.24 --> 1575.08]  But they also have like the one-click deployments of stuff.
[1575.58 --> 1577.28]  You know, like maybe you want to do a GitLab.
[1578.38 --> 1579.58]  Maybe your own Jitsi server.
[1579.66 --> 1580.50]  Get rid of that Zoom.
[1580.80 --> 1582.46]  One-click deployments for that kind of stuff.
[1582.68 --> 1585.16]  And they've been rolling out PCIe MVME storage.
[1585.28 --> 1587.04]  So things are real nice and fast.
[1587.18 --> 1589.10]  And they have 11 data centers around the world.
[1589.16 --> 1593.44]  So you're going to find something close to you or your clients or whoever you want it to be close to.
[1593.48 --> 1594.86]  Because there's 11 of them.
[1596.08 --> 1598.16]  And Linode's been doing this for 18 years.
[1598.16 --> 1602.14]  And they just keep dialing it in and making it better and better.
[1602.24 --> 1603.40]  So go see it for yourself.
[1603.78 --> 1604.80]  Use it for your next project.
[1605.02 --> 1605.68]  Deploy something.
[1606.28 --> 1607.64]  Maybe run a game server up there.
[1608.02 --> 1610.08]  Go have fun and use our promo code and get $100.
[1610.54 --> 1612.94]  It's linode.com slash SSH.
[1612.94 --> 1621.20]  So then there's a question about do I need an enclosure to 3D print?
[1621.70 --> 1623.90]  And the answer is maybe.
[1624.90 --> 1629.30]  I mean, there are a lot of factors that kind of go into it.
[1629.38 --> 1634.82]  But the main one is do you need to really contain the heat for one?
[1634.82 --> 1644.78]  And two, are there environmental variables in the area that you're going to put your 3D printer that you might benefit from using an enclosure?
[1644.92 --> 1649.40]  And in my particular case, I have lots of pets with lots of loose fur.
[1650.14 --> 1653.12]  And that was the primary reason that I bought one.
[1653.12 --> 1656.88]  And I'm pretty sure it saved a number of my prints already.
[1657.88 --> 1658.32]  Yeah.
[1658.40 --> 1665.56]  I mean, there's lots of cases I've had where just, you know, a single corner has lifted on a print for no discernibly good reason.
[1665.66 --> 1668.66]  And then I realized that the air conditioning kicked on halfway through that print.
[1668.66 --> 1677.62]  And I'm like, huh, I wonder if that draft from that vent up there was just enough to cause that part to cool down just enough to lift or something.
[1677.88 --> 1681.18]  So, yeah, like you say, it's highly dependent on your environment.
[1681.48 --> 1684.14]  It's also highly dependent on the plastic that you're using.
[1684.34 --> 1688.10]  So some plastics give off odors and smells.
[1688.10 --> 1693.66]  And sometimes you might want to actually extract those fumes away from the printer from the enclosure.
[1693.66 --> 1705.12]  But generally speaking, most people run an enclosure to prevent, like you do, pet hair or dust or to maintain some kind of temperature for more finicky plastics like ABS.
[1705.66 --> 1721.84]  I could see it being really valuable to have your printer in an enclosure if, say, you had your printer in your garage and the ambient temperature of your garage may shoot down during the winter or, you know, different variables just in the area in which your printer is.
[1721.84 --> 1731.24]  So I could see there being, you know, some uses other than just to help maintain the dust and noise and fumes of a printer.
[1732.82 --> 1733.82]  Yeah, totally agree.
[1733.94 --> 1736.16]  Garage is a great shout, particularly in a garage as well.
[1736.22 --> 1742.00]  You're going to end up with a lot of environmental debris in there because they're not as well sealed as a house, for example.
[1742.36 --> 1749.58]  So, all right, should we take a few moments to discuss the various different printers that we all have and the gear that we've got?
[1749.64 --> 1750.16]  Yeah, let's do it.
[1750.16 --> 1751.28]  Drew, would you like to go first?
[1751.84 --> 1753.22]  Sure, as the newbie here.
[1753.80 --> 1761.82]  So I bought an Ender 3 Pro, which I then very quickly upgraded various parts of.
[1762.52 --> 1773.44]  One thing that I saw on the Ender 3 subreddit that I really, really enjoy is that when you buy an Ender, you're not buying a 3D printer.
[1773.62 --> 1775.96]  You're buying a do-it-yourself 3D printing kit.
[1776.36 --> 1776.90]  Yes, you are.
[1777.04 --> 1777.32]  Yes.
[1777.32 --> 1780.10]  And that is absolutely so true.
[1780.10 --> 1784.32]  I have replaced a number of things on my printer already.
[1784.32 --> 1788.40]  I went from the Bowden tube setup to a direct drive.
[1788.40 --> 1802.80]  And I've also replaced the original hot end with an all-metal one, which is to say the original one had a piece of plastic tubing that goes all the way down almost to the nozzle to feed the filament.
[1802.80 --> 1819.28]  And the one I replaced it with has a fully metal body so that you don't have the issue of if you print it too high of a temperature that that tubing starts melting inside the hot end, which can happen once you start getting into things like PETG.
[1819.28 --> 1822.16]  So I just didn't want to deal with that.
[1822.24 --> 1824.52]  I went ahead and upgraded to the direct drive.
[1825.02 --> 1829.34]  I've also upgraded to what's called auto bed leveling.
[1829.34 --> 1849.50]  So with a normal 3D printer out of the box, typically, at least for the lower end ones, you have to manually go down there and measure down to the millimeter every corner and adjust the height so that it is the same distance from the nozzle all across the whole bed.
[1850.46 --> 1853.14]  Potentially every single time you print as well.
[1853.18 --> 1853.72]  Exactly.
[1853.72 --> 1859.50]  Sometimes the vibrations of the previous print cause your calibrations to be off.
[1860.48 --> 1865.52]  It was just, you know, I mentioned I had a CR10 in London, which I sold before I moved to America.
[1866.46 --> 1869.32]  And that had manual bed leveling on it.
[1869.38 --> 1872.00]  And it was just the most frustrating thing in the world.
[1872.06 --> 1876.52]  You just, you didn't know if it was going to work until the first layer was all completely done.
[1876.92 --> 1877.04]  Right.
[1877.44 --> 1877.96]  Yeah.
[1877.96 --> 1885.98]  So now with the auto bed leveling, it literally will, before print, go through and take measurements in nine different spots.
[1886.22 --> 1888.62]  And you can tune that depending on the firmware you're running.
[1888.86 --> 1892.10]  But on mine, it's nine different spots across the bed.
[1892.46 --> 1893.70]  Saves that value.
[1894.32 --> 1902.88]  And then when it goes to print, it pulls that value up, shows itself a mesh, and says, okay, this area is a little lower, so I need to compensate for that.
[1902.94 --> 1904.08]  This area is a little higher.
[1904.48 --> 1905.76]  I need to compensate for that.
[1905.76 --> 1911.40]  And so it takes something that's not level and essentially adjusts itself to make it level.
[1911.74 --> 1912.78]  One of the best upgrades.
[1913.12 --> 1918.46]  So you have just outlined my primary argument for not buying an Ender.
[1918.96 --> 1921.74]  Very, very eloquently, and I appreciate the fact that you did.
[1922.04 --> 1925.14]  I'm curious to know, how much did you spend on it in the first place?
[1925.20 --> 1927.22]  And then how much did you spend on upgrades?
[1927.74 --> 1928.60]  Yeah, I'm curious.
[1928.60 --> 1935.14]  So the original Ender I found on clearance at Micro Center for $200.
[1935.96 --> 1937.16]  That's a great price.
[1937.42 --> 1937.66]  Yes.
[1937.88 --> 1938.44]  Yes, it is.
[1938.52 --> 1939.66]  So I snapped that up.
[1939.66 --> 1943.82]  And then the upgrade kit with the auto bed leveling.
[1944.14 --> 1955.02]  And it also had the silent board, which is the upgraded V2 board, as well as the V2 screen, which the V2 is the next version up from the Ender 3 Pro.
[1955.02 --> 1959.30]  So I got all of that for under $100.
[1960.42 --> 1964.70]  And then the direct drive was about $60.
[1965.42 --> 1969.42]  The all metal hot end was about $40.
[1970.08 --> 1984.04]  And then I also replaced the cheap brass nozzles that typically are the things that come with it and that most people buy in packets of $20 because they wear out after three prints, in my opinion.
[1985.02 --> 1990.94]  I replaced that most recently with a Nozzle X, which the Nozzle alone was $40.
[1991.72 --> 1994.28]  So far, it is worth every penny.
[1994.54 --> 1997.24]  I'm 60% through my first print with it.
[1997.54 --> 2000.26]  And it has had no issues so far.
[2000.58 --> 2005.36]  Fingers crossed it's going to be a great upgrade that outlasts the actual printer.
[2005.96 --> 2008.88]  So all in, I mean, we're talking, what, less than $500?
[2009.88 --> 2011.96]  Yeah, probably around $400 or so.
[2012.02 --> 2012.36]  Yeah.
[2012.36 --> 2016.36]  And I feel like I've got a really good machine going now.
[2016.92 --> 2018.64]  Those are some solid bargains, dude.
[2018.90 --> 2019.28]  Mm-hmm.
[2019.80 --> 2027.40]  I think the next time I want to buy something off, you know, from Goodwill or something on clearance or Micro Center, I'm going to deploy Drew to go and find it for me.
[2027.44 --> 2027.82]  That's right.
[2028.72 --> 2029.72]  Deal hound, Drew.
[2030.06 --> 2031.96]  Find any 3D printers wherever you go.
[2031.98 --> 2032.42]  That's right.
[2032.42 --> 2032.98]  I like it.
[2034.26 --> 2041.96]  You know, to be honest, though, Drew, I think that that's probably about the same that I have into my Ender.
[2043.54 --> 2046.32]  Somewhere sub $500, I would say.
[2046.88 --> 2048.44]  So you went with an Ender as well, did you, Chief?
[2048.84 --> 2052.12]  Yeah, I went with the Ender 3, the Ender 3 Pro.
[2052.12 --> 2056.14]  So basically the same printer as Drew.
[2057.14 --> 2061.10]  I got it for $180-ish on sale through Creality.
[2061.56 --> 2062.08]  Good deal.
[2062.48 --> 2063.94]  I think they're wonderful printers.
[2064.18 --> 2072.88]  If you enjoy tinkering, you don't mind assembling it, you don't mind adjusting it to get it all dialed in, and you don't mind incrementally upgrading it.
[2072.88 --> 2078.90]  I think that's particularly interesting because I know that you've just bought yourself a Prusa.
[2079.28 --> 2079.56]  Yes.
[2079.78 --> 2094.60]  Which is something I'm a huge fan of, and I'm really curious to get your take as someone, you know, besides me that's just used both an entry-level now and what is considered the Rolls-Royce of FDM printers, the Prusa i3 Mark III.
[2095.30 --> 2098.96]  I'm curious to know what you think now you've used both.
[2098.96 --> 2103.12]  I think there's a place for both.
[2103.32 --> 2107.90]  I think the Ender is great to get started on and see if you like the hobby.
[2109.08 --> 2121.48]  And then I think most people find themselves looking at Prusa or other high-end 3D printer manufacturers for something that is more just kind of turnkey and reliable.
[2122.00 --> 2122.68]  Yeah, 100%.
[2122.68 --> 2125.20]  And that's definitely what I've gotten with the Prusa.
[2125.20 --> 2134.64]  Well, let's not forget as well that the Prusas are $750 as a kit and $1,000 pre-built.
[2135.28 --> 2136.08]  So they're twice the price.
[2136.48 --> 2137.86]  They are twice the price.
[2139.90 --> 2143.98]  I just splurged and bought the $1,000 kit, the pre-assembled kit.
[2144.84 --> 2147.74]  It came in obviously pre-assembled.
[2147.74 --> 2150.42]  See, I have strong opinions about this as well.
[2150.50 --> 2159.22]  I think that everybody that's buying a Prusa should, if they have the time and the means, you know, should go through the process of building it.
[2159.22 --> 2180.62]  Because the first time I built a Prusa, I've built two now, I learned so much about electronics, about how different screws fit through different things, and just quite what 3D printing is capable of in terms of, you know, part tolerances and the strength of different pillars and all that kind of stuff that's required.
[2181.28 --> 2183.22]  Highly fascinating procedure.
[2183.22 --> 2186.30]  Yeah, I mean, I think it's worth doing that.
[2186.82 --> 2188.02]  I'm not against that.
[2188.32 --> 2190.52]  But I felt that I had kind of already done that with Ender.
[2191.06 --> 2191.96]  I can see that.
[2192.22 --> 2201.20]  When I had gotten to the point where I wanted, because I generally don't purchase things like this for myself, I wanted to have something that was turnkey, right?
[2201.20 --> 2207.90]  So I just wanted to pull it out of the box, set it on the table, plug it in, go through the initial setup.
[2209.22 --> 2219.14]  Some of the things that you get with the Prusa that you don't get with, say, an Ender, the Prusa comes with a handbook that goes through everything you need to know about the printer.
[2219.38 --> 2220.42]  It's about as thick as a Bible.
[2221.02 --> 2221.36]  It's amazing.
[2221.36 --> 2224.92]  Yeah, it's a great handbook, great documentation.
[2226.48 --> 2229.96]  Not that you can't find great documentation for an Ender or something like that.
[2230.28 --> 2232.80]  Probably not through the vendor, more so through third parties.
[2233.00 --> 2235.88]  But there's documentation available there.
[2236.34 --> 2240.54]  Prusa sets the bar, in my opinion, for documentation, for customer support.
[2240.54 --> 2247.66]  And also, not to come across as too much of a fanboy, but everything they do is open source.
[2248.20 --> 2252.00]  The hardware designs, the drawings, everything is open hardware.
[2252.16 --> 2254.90]  It's all based off the original RepRap movement.
[2255.22 --> 2258.74]  It's all designed around 3D printers printing more 3D printers.
[2258.94 --> 2259.20]  Correct.
[2259.62 --> 2263.98]  Which is kind of a, it's machines making machines, so Matrix, watch out.
[2263.98 --> 2269.34]  But in my opinion, as a company, Prusa do so much right.
[2269.34 --> 2271.16]  They're based out of the Czech Republic in Prague.
[2271.28 --> 2274.86]  Joseph Prusa is incredibly present on social media.
[2275.06 --> 2276.40]  He also does a lot of YouTube stuff.
[2277.46 --> 2282.24]  You know, you'll frequently see him on with Joel Telling, who's the 3D printing nerd on YouTube.
[2283.34 --> 2289.22]  And, you know, there's so much in my life that is, you know, open source, you know, working for Red Hat, obviously.
[2289.68 --> 2293.28]  Open source is at the core of everything that pays my mortgage.
[2293.28 --> 2299.04]  And, you know, it's been a huge factor in my personal journey with Linux and everything else, you know.
[2299.04 --> 2306.30]  So the fact that I can also buy a piece of hardware that is totally open, 100% open,
[2307.04 --> 2313.38]  and the vendor has shown a commitment to doing everything open for a decade or so now.
[2313.98 --> 2318.22]  For me, Prusa is just a, you know, I'm a fanboy.
[2318.32 --> 2319.00]  I'm going to admit it.
[2319.10 --> 2322.14]  But Prusa is pretty much untouchable, in my opinion.
[2323.08 --> 2323.28]  Yeah.
[2323.28 --> 2326.16]  I mean, Prusa does a lot of good things, right?
[2326.20 --> 2330.46]  They even have their own prints library, similar to Thingiverse.
[2330.46 --> 2339.80]  But in that same vein, the Ender 3 from Creality is open source and open hardware.
[2340.76 --> 2342.96]  Only because of Prusa.
[2343.90 --> 2344.38]  Absolutely.
[2344.56 --> 2345.64]  Well, they set a bar, right?
[2346.00 --> 2347.00]  And it didn't used to be.
[2347.22 --> 2357.82]  If I recall correctly, it wasn't open, and then Creality bowed to public pressure and eventually released drawings that were of a questionable quality to start with.
[2357.82 --> 2359.34]  And then they've improved with time.
[2360.34 --> 2361.94]  Well, I mean, I don't know about that.
[2362.06 --> 2364.24]  I haven't, you know, I'm not here to bash on Creality.
[2364.34 --> 2369.00]  But I'm just saying that they also have open source their hardware, you know.
[2369.00 --> 2379.80]  I think that it's good to have someone like Prusa in the market to help push those narratives and to help push the way that things should maybe be conducted in an ecosystem, right?
[2379.90 --> 2385.56]  So by making these things open hardware and encouraging others to do so, I think it's awesome.
[2385.56 --> 2397.08]  I think I look at this through the lens of drone racing, where there's an awful lot of commodity parts put together onto flight controllers and things like that.
[2397.30 --> 2400.54]  And Chinese clones are a real problem in that industry.
[2400.54 --> 2412.54]  You'll have a lot of guys in the West that put a lot of IP into developing specific, you know, radios and flight control algorithms and all this stuff.
[2413.12 --> 2419.08]  And they will put that board out to be made at a factory in China at a decent price.
[2419.22 --> 2426.48]  And then two weeks later, a complete copy clone of that thing is floating around for half the price on the internet, you know.
[2426.48 --> 2434.34]  And for a while, I kind of felt like Creality were in that similar space of just copying IP.
[2435.06 --> 2438.70]  They have proven me wrong, I think, in general.
[2439.76 --> 2445.40]  They've done a lot of stuff to open source a lot of their drawings and stuff like that.
[2446.16 --> 2448.00]  But there's still a way for them to go, I think.
[2449.06 --> 2450.94]  Definitely think there's a way for them to go.
[2451.02 --> 2453.74]  I mean, I think there's a way for the entire industry to go as well.
[2453.74 --> 2463.28]  And I think, you know, going back to kind of why I had ended up going from Ender to Prusa.
[2463.94 --> 2465.58]  Prusa has a lot of nice features, right?
[2465.60 --> 2470.74]  It's got auto bed leveling built in with a really accurate probe.
[2471.38 --> 2478.86]  It's got a really nice bed that comes with it and the steel sheet to put on the bed.
[2478.86 --> 2483.52]  And Drew had mentioned earlier that it draws a mesh, essentially.
[2483.78 --> 2493.18]  So, mind you, all of these printers, regardless of which one it is, the bed is not going to be manufactured perfectly true.
[2493.48 --> 2495.42]  It's basically impossible for that to happen.
[2495.54 --> 2502.96]  That's why you see people use mirrors on their 3D printers is because mirrors are generally more true than a piece of glass.
[2502.96 --> 2508.96]  Because if you had a mirror that wasn't true or flat, then you would have a funhouse mirror.
[2509.44 --> 2515.08]  And I don't think, you know, everyone wants to wake up in the morning staring at a funhouse version of themselves while they brush their teeth.
[2515.22 --> 2519.44]  So, there are a lot of nice features that come with the Prusa.
[2519.60 --> 2525.98]  You get the direct drive extruder, which you can also love this feature, remove the filament.
[2525.98 --> 2532.06]  So, instead of, say, with my Ender, I would heat up the hot end and then just yank the filament out.
[2533.18 --> 2539.52]  With the Prusa, it will heat up the hot end and then reverse the drive gears in the extruder to pull the filament out.
[2539.68 --> 2541.98]  And I just pull the filament out of the top of the extruder.
[2542.20 --> 2542.88]  It's pretty nice.
[2543.26 --> 2544.62]  Super nice, super clean.
[2545.98 --> 2553.18]  The steppers and the drivers for the motors are, or the steppers themselves and the drivers for them are super quiet.
[2553.18 --> 2557.14]  I hear the fans more than I hear the motors, which wasn't true.
[2557.24 --> 2563.04]  And I'm sure, Drew, you can attest to this, that the original Ender board that you had in your Ender 3,
[2563.70 --> 2569.30]  the sound from whenever you upgraded from the original board to the version 2,
[2569.96 --> 2572.20]  just the drivers for the motors.
[2572.58 --> 2573.70]  Dude, it's night and day.
[2574.52 --> 2575.04]  Absolutely.
[2575.86 --> 2580.16]  Yeah, it's ridiculous how loud the Ender 3 Pro is out of the box.
[2580.16 --> 2585.20]  So let me ask you both, what kind of stuff do you print these days?
[2586.04 --> 2593.70]  So I've been printing lately things like cases and stands for various items that need them around the house,
[2593.84 --> 2597.78]  some things for some musical instruments and things of that nature.
[2598.20 --> 2602.90]  My wife and I, when we first started getting into 3D printing,
[2602.90 --> 2612.24]  part of the goal was to design things, print them, and then use her Cricut maker to print vinyl,
[2612.74 --> 2617.70]  which could then be 2D printed to have her designs on them,
[2617.84 --> 2622.24]  and then go on to the 3D objects to sell through her store.
[2622.66 --> 2623.50]  That's very cool.
[2623.82 --> 2626.14]  So that's coming.
[2626.76 --> 2631.08]  We both need a little more experience with our individual parts.
[2631.08 --> 2632.66]  Like I need to get a little better.
[2632.78 --> 2636.84]  I haven't designed anything yet as far as 3D printing is concerned.
[2637.24 --> 2640.12]  That's, you know, that's the next level up, right?
[2640.42 --> 2641.92]  That's a whole nother bowl game, man.
[2642.10 --> 2642.54]  Absolutely.
[2643.02 --> 2646.48]  I'm getting used to making the filament do what I want it to do
[2646.48 --> 2650.12]  before I try to make it do stuff that we're going to sell.
[2652.34 --> 2652.82]  Understandable.
[2653.46 --> 2653.98]  Absolutely.
[2653.98 --> 2662.82]  For me, I've been printing, well, shortly after, I would say maybe four months after we got our printer,
[2664.36 --> 2665.34]  COVID hit.
[2666.12 --> 2669.60]  And like many makers of the time, Alex, I know you're one,
[2670.24 --> 2672.96]  and had encouraged me to get onto the bandwagon as well,
[2673.02 --> 2677.56]  started pitching in and making face masks or shields
[2677.56 --> 2681.78]  using our 3D printers and some other materials.
[2682.54 --> 2684.22]  So I spent a lot of time doing that.
[2684.42 --> 2690.34]  Printed a ton of those for schools and nurseries and random public places.
[2691.00 --> 2695.14]  But I enjoy printing cases, little electronics projects.
[2695.14 --> 2698.42]  I think after seeing your recording sign project,
[2698.42 --> 2702.26]  and it also got me kind of into microcontrollers.
[2702.26 --> 2705.50]  And I think 3D printing helped kind of drag me there too.
[2705.72 --> 2714.16]  So like I've printed a little project that has a 0.96 inch OLED screen
[2714.16 --> 2718.54]  that basically connects to Octoprint, tells me the progress of a print,
[2719.30 --> 2721.88]  sits on my desk, it's powered by five volts.
[2722.14 --> 2726.76]  Just recently finished printing a case for a stream deck
[2726.76 --> 2731.08]  that I'm planning on making using a Arduino Pro Micro,
[2732.06 --> 2737.94]  some sliders, and actually some of the jade switches
[2737.94 --> 2740.26]  that are left over from the launch keyboards.
[2741.66 --> 2745.66]  Sometimes in our shipment of switches, we get bent pins.
[2746.28 --> 2748.40]  And so we have like a bent pin bucket.
[2749.26 --> 2752.34]  So I raided the bent pin bucket and found some switches
[2752.34 --> 2754.58]  to include in the project.
[2754.96 --> 2756.74]  So looking forward to getting that one done.
[2756.76 --> 2759.80]  But I think as you start with the hobby,
[2760.00 --> 2763.16]  you find just, you know, things that you can print online,
[2763.28 --> 2764.12]  things that are useful.
[2764.86 --> 2767.42]  Then you drift into kind of designing things.
[2767.66 --> 2773.20]  And the next thing you know, you're just absolved in it, I guess.
[2773.24 --> 2776.66]  It's kind of like a drug addiction to some extent, right?
[2777.22 --> 2779.74]  Maybe a drug addiction would be cheaper at times.
[2780.16 --> 2781.02]  At times.
[2781.20 --> 2782.18]  I mean, at times, right?
[2782.44 --> 2783.24]  Like maybe.
[2784.00 --> 2786.66]  I wouldn't imagine over the long term, right?
[2786.76 --> 2787.64]  Maybe short term.
[2788.14 --> 2791.90]  But like, you know, like Drew said, buying the upgrades and upgrading the thing,
[2791.98 --> 2794.30]  you just kind of get into this something.
[2794.44 --> 2795.16]  I don't know what it is.
[2795.20 --> 2799.00]  It's like this thing that just pulls you forward to like,
[2799.10 --> 2800.58]  let's make all of the things.
[2800.58 --> 2802.44]  How can I just make this myself?
[2803.36 --> 2810.06]  Instead of just being a consumer and just grabbing the first thing off the shelf that
[2810.06 --> 2813.34]  kind of fits your needs or solves your problem.
[2813.72 --> 2817.04]  It's nice to be able to actually make something yourself to solve that problem.
[2817.04 --> 2818.56]  Totally agree.
[2818.78 --> 2822.74]  An example of that in my life recently, my daughter recently figured out how to crawl.
[2823.02 --> 2825.90]  And so obviously, we started needing to baby proof the house.
[2826.08 --> 2831.94]  So I've printed corner protectors for, you know, things like coffee tables and the outlet
[2831.94 --> 2833.84]  prong protector things.
[2834.06 --> 2834.26]  Yes.
[2834.66 --> 2836.46]  All sorts of little things like that, you know.
[2836.86 --> 2840.34]  Have you printed any little door locks for like under the cabinet?
[2840.34 --> 2843.62]  No, but I think I will need to pretty soon.
[2843.88 --> 2844.02]  Yeah.
[2844.24 --> 2848.88]  I do a lot of stuff like shelf brackets and little widgets to help me, you know,
[2848.98 --> 2851.62]  in the workshop when I'm doing woodworking, that kind of stuff,
[2851.70 --> 2856.04]  like little templates and routing guides and jigs, that kind of thing.
[2856.90 --> 2861.32]  You know, there's just so many, so many little things you can do with it.
[2861.32 --> 2865.14]  There's a great subreddit called r slash functional print.
[2865.72 --> 2865.80]  Yes.
[2865.80 --> 2868.16]  And there's all sorts of great stuff on there.
[2868.16 --> 2872.28]  So if you're struggling for inspiration, take a look at that subreddit.
[2873.78 --> 2880.14]  Have you guys on the note of all of these printers and Alex, I'm sure you guys have.
[2880.80 --> 2884.20]  Drew, have you had a chance to see the new Prusa XL printer?
[2885.12 --> 2885.90]  That's a big boy.
[2886.36 --> 2887.10]  I have not.
[2887.20 --> 2887.88]  How big is it?
[2888.86 --> 2889.76]  It's XL.
[2889.76 --> 2892.10]  I mean, it's not double XL, but it's XL.
[2892.10 --> 2899.36]  But it also has automatic extruder tool head changes.
[2899.72 --> 2902.02]  So you can have multiple filaments loaded.
[2902.46 --> 2904.88]  Like, I think it's five filaments loaded at a time.
[2905.12 --> 2910.14]  And it will just pick the head and pull the hot end and head.
[2910.14 --> 2916.46]  Typically, a Prusa is nine inches tall by eight inches front to back and left to right.
[2916.72 --> 2916.86]  Right.
[2917.46 --> 2922.20]  The Prusa XL is 14 inches square.
[2922.80 --> 2926.46]  Just that's its build volume is front to back, left to right, up, down, 14 inches.
[2926.62 --> 2928.64]  So significantly larger.
[2928.64 --> 2934.88]  And in order to do that, they're charging $2,000 as a starting point for this printer.
[2935.26 --> 2937.40]  Bear in mind, a normal Prusa starts at $750.
[2937.80 --> 2942.60]  And they've got the Prusa Mini as well, which starts at $300, $400, something like that.
[2942.72 --> 2943.04]  Right.
[2943.14 --> 2944.08]  To compete with the Enders.
[2944.74 --> 2950.68]  But like Cheese says, the really cool game-changing feature that they've got on this new Prusa XL,
[2951.26 --> 2954.30]  it's not just the fact that they're changing the heads or anything.
[2954.42 --> 2956.06]  They're changing the whole tool.
[2956.06 --> 2960.18]  So it's five separate, you can have up to five separate extruders on this thing.
[2960.66 --> 2964.34]  So you could 3D print five completely different materials.
[2964.98 --> 2969.74]  So you could have dissolvable filaments, soluble filaments to do supports, for example,
[2969.74 --> 2972.04]  that you could then submerge your print and they would just dissolve.
[2973.14 --> 2977.20]  So there's all sorts of really interesting different applications you could use for that one.
[2977.60 --> 2983.96]  And it has a really neat new bed technology, the way that they've segmented the bed.
[2983.96 --> 2990.76]  So instead of it just being a flat bed, they've segmented the beds, leaving cooling and expansion channels in between.
[2990.76 --> 3003.34]  So that as the bed heats up and expands and contracts, you'll be less likely to have warped pages on the bottom of your prints where they're adhering to the bed and stuff.
[3003.58 --> 3011.48]  A lot of cool new tech definitely coming out from Prusa, which I think is going to set the bar for everyone else going forward.
[3011.48 --> 3017.58]  And, you know, hopefully we'll continue to do this ourselves.
[3017.88 --> 3020.10]  And next year we'll sit down and see where we are.
[3020.22 --> 3024.92]  But I did have a couple of questions for you, Alex and Drew as well.
[3026.36 --> 3031.84]  Do you guys weigh your filament before you put a print together?
[3031.84 --> 3043.16]  So if you know that you're going to have an extended print, do you weigh the filament that's on the roll before you load it into your printer to make sure you have enough filament?
[3043.30 --> 3046.24]  Or do you just cross your fingers and hope that you have enough filament?
[3046.84 --> 3048.56]  I do the cross and clench method.
[3048.88 --> 3048.98]  Yeah.
[3049.58 --> 3050.02]  Okay.
[3050.34 --> 3053.22]  The Prusa has a filament runout sensor, so I'm not too worried.
[3053.58 --> 3053.76]  Yeah.
[3053.76 --> 3060.08]  My upgrade kit also came with a filament runout sensor, which I haven't actually installed yet.
[3061.04 --> 3070.12]  I need to do that, but I also haven't gone through enough filament yet to really make it necessary as of now.
[3070.84 --> 3071.34]  Got you.
[3071.66 --> 3072.14]  Got you.
[3073.04 --> 3075.46]  But, I mean, do you weigh your filament?
[3075.62 --> 3079.48]  How do you measure to know if you have enough filament on a roll to complete a print?
[3079.60 --> 3082.48]  Do you just do the same method, just the cross and clench method?
[3082.48 --> 3083.22]  Yeah, pretty much.
[3083.22 --> 3084.34]  High baller.
[3085.66 --> 3087.96]  You're like, hmm, that's roughly half a roll.
[3088.74 --> 3090.32]  We can roughly get this much out of it.
[3090.40 --> 3094.76]  Well, I haven't gone even through half a roll of any of my individual rolls yet.
[3094.84 --> 3101.36]  I've got like eight different rolls of filament sitting around, and I've kind of played with each of them so far, you know.
[3102.46 --> 3109.20]  If you consider that each roll of filament is a kilo, typically it's a kilogram, that's a lot of plastic.
[3109.20 --> 3114.66]  So you'd be printing something pretty massive in order to go through an entire roll in a single print.
[3114.82 --> 3114.92]  Yeah.
[3114.92 --> 3118.24]  I think where it matters more is where you're trying to use up the dregs, for example.
[3118.72 --> 3118.90]  Absolutely.
[3119.26 --> 3120.74]  And that's why I'd asked, yeah.
[3120.74 --> 3125.70]  I got pretty good when I was doing the mask making that you referenced when COVID first started.
[3125.70 --> 3130.16]  Kind of doing like a hot swap, I would sort of sit, you know, printers next to me on my desk.
[3130.16 --> 3138.54]  Like, I'd sit and watch it, and then I would have the second spool ready, and I'd just sort of get a lighter and fuse it together really roughly.
[3138.74 --> 3139.42]  Wait, what?
[3139.90 --> 3141.40]  And then sort of file it down a little bit and sort of shove it.
[3141.42 --> 3142.94]  And it would be fine.
[3142.98 --> 3145.82]  It would jam occasionally, but most of the time it was fine.
[3147.12 --> 3148.82]  I never thought of that.
[3148.82 --> 3154.24]  While doing that, I would do the same, but I would just watch Octoprint and then hit pause.
[3154.54 --> 3155.12]  You could do that.
[3155.20 --> 3155.96]  That's probably safer.
[3156.52 --> 3158.00]  And then just swap the filament out real quick.
[3158.00 --> 3158.78]  That's probably safer.
[3158.78 --> 3161.02]  I never thought of it.
[3161.02 --> 3162.14]  I mean, that's a good way to do it.
[3162.18 --> 3166.00]  I mean, I guess you could potentially introduce clogs, but…
[3166.00 --> 3168.02]  I could potentially burn my house down, but apart from that.
[3168.76 --> 3176.14]  I mean, only, you know, the nozzles are only a few cents each if you get the cheap brass ones that Drew had mentioned earlier.
[3177.54 --> 3178.70]  What about maintenance?
[3178.90 --> 3180.76]  What do you guys do for maintenance on your printers?
[3181.96 --> 3187.88]  There is an excellent video by a Welsh guy on YouTube whose name escapes me, but I'll put a link to it in the show notes.
[3187.88 --> 3194.64]  Where he talks through dismantling a Prusa, for example, and all the different oils that you need to put on various different parts and what have you.
[3195.38 --> 3198.70]  I tend to do it on an annual basis or as often as I can be bothered.
[3199.38 --> 3202.60]  It really depends how much you're printing, how many hours a day you're printing, that kind of thing.
[3203.20 --> 3207.36]  My printer sits idle much more than it's printing, to be perfectly honest.
[3207.36 --> 3210.82]  So, I don't feel the need to do quite so much maintenance.
[3211.56 --> 3216.46]  But if I was running a print farm or something, I would definitely put it as part of a regular regime.
[3217.52 --> 3217.78]  Gotcha.
[3217.90 --> 3218.56]  What about you, Drew?
[3218.58 --> 3224.48]  I don't imagine you've done much since you haven't had a printer too long, but what kind of maintenance do you do?
[3224.78 --> 3229.64]  As far as, like, the printer maintenance that Alex is talking about, I haven't done any.
[3229.64 --> 3241.20]  However, you know, once a week or so, if I have an issue that I notice, like, there's, you know, the x-axis is a little wonky on a print.
[3241.32 --> 3242.84]  I'll go through and I'll check the belts.
[3243.62 --> 3244.02]  Right.
[3244.12 --> 3245.74]  You know, spot checking various things.
[3245.74 --> 3259.08]  One thing I will say is, after every print, I will go through with a microfiber cloth and just wipe down the bed, wipe off the nozzle, make sure that everything's, you know, clean and ready for the next time I go to print.
[3259.90 --> 3270.96]  That is one thing that I would say is well worth doing, is just having something around to just wipe down the bed and wipe down the nozzle, at the very least, every time you do a print.
[3270.96 --> 3281.64]  Just because you can get stuff that maybe attaches to the nozzle, although it's less of a problem if you have one of the nicer nozzles than it is with brass.
[3282.22 --> 3287.42]  But still, it's good practice to clean up after yourself in your workspace.
[3289.24 --> 3291.38]  Yeah, and I would say that I do that as well.
[3291.46 --> 3299.48]  Every time I have, like, a little spray bottle of isopropyl alcohol and a microfiber cloth that I just spray down and wipe the bed every time.
[3300.02 --> 3300.34]  Yeah.
[3300.34 --> 3301.12]  And finish with the print.
[3301.16 --> 3308.06]  I used to spray mine down, but now with the PETG, because I am printing on tempered glass, I do use glue stick.
[3308.20 --> 3308.36]  Ah.
[3309.12 --> 3311.40]  So I tend to leave the glue stick.
[3311.50 --> 3313.40]  I don't wipe that down after every use.
[3313.40 --> 3319.74]  I will, I'll do a number of prints before I go through and wash it off and reapply.
[3320.40 --> 3325.60]  That's one of the beautiful things about the Prusa, though, is I can't remember the last time I cleaned my bed.
[3326.68 --> 3329.50]  Maybe that's bad, but it just works every time.
[3330.34 --> 3336.38]  Well, I'm looking forward to that, but I'll probably still clean my bed every single time I print something.
[3336.70 --> 3337.94]  I just, it's habit, dude.
[3337.98 --> 3338.60]  I just can't not.
[3338.60 --> 3344.96]  I used to, I used to, I just out of habit from the CR10 that I had, but eventually I just stopped.
[3344.96 --> 3354.22]  And it, you know, whilst I was doing the masks, I got pretty good at figuring out what was actually needed versus what the internet told me I needed to do.
[3354.46 --> 3354.86]  Right.
[3354.86 --> 3365.66]  And generally speaking, as long as your house isn't in the desert, you know, full of dust, you should be fine with just the occasional wipe down.
[3365.78 --> 3373.84]  When I say clean, all I really mean is literally taking a microfiber cloth, running it across the bed, running it across the nozzle.
[3374.72 --> 3375.18]  Job done.
[3375.44 --> 3375.74]  Right?
[3376.26 --> 3376.50]  Mm-hmm.
[3376.50 --> 3382.26]  You know, we're not talking about you have to get in there and like scrub every nook and cranny or anything like that.
[3382.86 --> 3383.26]  No.
[3383.54 --> 3384.36]  You know, it's a-
[3384.36 --> 3387.46]  I had to do that on my glass bed with the Creality that I had.
[3387.52 --> 3388.12]  Oh, well.
[3388.74 --> 3394.66]  Take some dish soap and wash it with love and care and affection and then never touch it and get my-
[3394.66 --> 3395.94]  It was just a pain in the ass.
[3396.18 --> 3397.38]  After every print?
[3397.54 --> 3398.36]  Pretty much, yeah.
[3398.48 --> 3399.18]  Oh, God.
[3399.26 --> 3399.50]  Wow.
[3399.68 --> 3400.22]  That's horrible.
[3400.22 --> 3405.44]  Bear in mind, this was like four years ago before, you know, things have come on a bit of a way since then.
[3405.68 --> 3406.82]  That's fair, yeah.
[3407.08 --> 3419.54]  I mean, for anybody listening, if you're getting into it and you want to take my route where you're kind of spending a little less money and doing some DIY upgrades, go get yourself some decent quality glue stick.
[3420.58 --> 3421.90]  It makes a world of difference.
[3422.02 --> 3422.60]  It really does.
[3423.78 --> 3424.30]  100%.
[3424.30 --> 3426.22]  Now, thank you both for joining.
[3426.22 --> 3430.56]  I really appreciate you taking the time out of your schedules to come and talk to us today.
[3430.98 --> 3433.72]  Is there any way you'd like to send people to follow you or anything?
[3435.40 --> 3438.10]  I mean, you can follow me on Twitter at Cheese Bacon.
[3438.60 --> 3440.66]  That's C-H-Z-B-A-C-O-N.
[3441.42 --> 3445.36]  If you have any questions or just want to talk shop, feel free to reach out.
[3445.48 --> 3446.68]  My DMs are open.
[3447.34 --> 3448.20]  Yep, same here.
[3448.32 --> 3449.60]  Drew of Doom on Twitter.
[3450.18 --> 3451.36]  Feel free to reach out.
[3451.84 --> 3452.88]  Well, thank you both very much.
[3453.08 --> 3453.94]  Thank you for having me, man.
[3454.02 --> 3454.54]  Yeah, thank you.
[3454.54 --> 3458.66]  Maybe 2022 will be the year that I finally get a 3D printer.
[3458.76 --> 3459.80]  I know my kids would love it.
[3460.32 --> 3463.96]  And then I know I'd start printing stuff for my RV all the time.
[3464.36 --> 3469.24]  I want to say a special holiday thank you to our members over at selfhosted.show slash SRE.
[3469.66 --> 3471.28]  You make this show possible.
[3471.78 --> 3473.96]  Don't forget you also get the extra post show.
[3473.96 --> 3485.22]  And we now, after a lot of, I guess the term is popular demand, as they say, we now have a network membership at Jupiter.party.
[3485.34 --> 3486.52]  You can gift it as well.
[3487.38 --> 3489.26]  We'll have that for a little bit longer.
[3489.26 --> 3493.84]  And also, until the end of December, if you sign up, we're taking two bucks off.
[3493.84 --> 3498.46]  So normally the membership is just the cost of two memberships, but you get access to all the show special stuff.
[3498.62 --> 3499.46]  All the goodies.
[3500.12 --> 3502.14]  The behind-the-scenes stuff and love.
[3502.64 --> 3505.06]  The member stuff that you get only with self-hosted.
[3505.16 --> 3505.88]  Member show.
[3506.36 --> 3507.34]  The coder QA.
[3507.62 --> 3508.18]  All that.
[3508.18 --> 3511.00]  And Linux Action News.
[3511.78 --> 3512.56]  Totally ad-free.
[3512.70 --> 3513.88]  And any new content we add as well.
[3513.94 --> 3515.94]  For just the price of two memberships.
[3516.38 --> 3521.38]  But right now, until the end of the month of December, we're taking two bucks off for a year.
[3522.22 --> 3524.86]  This membership is designed to let us be picky.
[3525.80 --> 3527.76]  To make sure we choose the right sponsors.
[3528.46 --> 3536.72]  We get a lot of emails that come in and, you know, we don't want to be in a position where we have to work with a sponsor that we don't actively believe in.
[3536.72 --> 3539.36]  And this lets us be picky.
[3539.62 --> 3540.44]  It gives us runway.
[3540.70 --> 3543.88]  Because these good sponsorship deals, they don't happen overnight.
[3544.22 --> 3545.80]  They take months to develop a relationship.
[3546.22 --> 3547.76]  You give us the runway to do that.
[3548.38 --> 3553.98]  The episodes where there's fewer sponsorships, those are the episodes our members actually make possible too.
[3555.22 --> 3556.60]  So it's a pretty special thing.
[3556.64 --> 3559.28]  And it puts you in the driver's seat.
[3559.98 --> 3561.74]  Because you're funding the content.
[3562.10 --> 3563.14]  And that's fundamental.
[3563.32 --> 3564.58]  That changes everything.
[3564.58 --> 3568.70]  Jupiter.party if you'd like to be a member for the entire network.
[3569.14 --> 3573.26]  Or selfhosted.show.sre if you'd like to be a member just for this show.
[3573.70 --> 3575.50]  And even if you can't support us through a membership.
[3575.94 --> 3577.84]  We are so grateful for your downloads.
[3578.30 --> 3579.34]  For your community support.
[3579.76 --> 3580.76]  For maybe telling a friend.
[3581.20 --> 3582.54]  Maybe leaving a review somewhere.
[3583.14 --> 3585.02]  So happy holidays from the Self Hosted team.
[3585.42 --> 3588.46]  And feel free to reach out to us at selfhosted.show.contact.
[3588.46 --> 3589.78]  And ho, ho, ho.
[3590.14 --> 3591.82]  We'll see you right back here next year.
[3592.34 --> 3592.66]  You.
[3592.86 --> 3593.14]  You.
[3593.14 --> 3613.74]  000
