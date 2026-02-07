[0.00 --> 2.66]  We kick off with a special episode of the Self-Hosted program.
[2.86 --> 6.02]  Alex is out on assignment at All Things Open this week.
[6.84 --> 11.16]  But both Brent and Jeff are in studio because we're getting ready for LinuxFest.
[11.32 --> 12.92]  Welcome into the Self-Hosted show, guys.
[13.32 --> 14.04]  Well, thank you.
[14.28 --> 14.66]  Hello.
[14.92 --> 15.74]  Thank you for being here.
[16.26 --> 17.86]  Audience, you probably remember listener Jeff.
[17.90 --> 20.20]  He's helped us with lots of projects over the years.
[20.26 --> 22.82]  And Brent, you were just here like the last episode or something like that.
[22.84 --> 23.22]  It's funny.
[23.28 --> 25.74]  Last episode we said, oh, you haven't been here in like six months.
[25.94 --> 26.54]  Here I am.
[26.54 --> 32.48]  And when Jeff and Brent are here, that means it's project time.
[32.66 --> 33.16]  It's on.
[33.32 --> 36.86]  And it has been on like crazy.
[37.02 --> 41.10]  We have been knocking off some projects that have been on the list for a couple of years.
[41.88 --> 47.84]  And this week, I think the one that I'm most excited about is we have my water heater,
[48.02 --> 51.12]  which is both gas and electric, both sides of it.
[51.12 --> 59.56]  And the water pump are now all on relays attached to an ESP device, which of course is communicating with Home Assistant.
[59.56 --> 62.42]  So I can now automate my water pump and my water heater.
[63.02 --> 64.90]  I've wanted that for so, so long.
[65.38 --> 66.40]  And Jeff came over.
[66.48 --> 68.74]  He brought like boxes of stuff.
[68.96 --> 70.74]  And I thought, well, he doesn't need to bring anything.
[70.80 --> 71.76]  I got a ton of stuff.
[71.90 --> 73.80]  But I think we ended up putting all your stuff in the wall.
[73.80 --> 79.20]  Mainly because I know where it's at, you know, what I have and how it works.
[80.12 --> 81.96]  Did you, Chris, have a look at his trunk?
[82.36 --> 88.26]  It's like a radio shack went out of business and he pulled up and just opened up trunk, you know.
[88.34 --> 89.22]  Give it all to me.
[89.48 --> 90.56]  It's so precise.
[90.56 --> 95.46]  When you're operating in an RV, things are never as simple as they should be.
[95.62 --> 102.04]  So, of course, we crack this central panel open that has all these switches and it has status lights for tank fill.
[102.24 --> 106.16]  And you can start the generators, kind of like the central control panel of the RV.
[107.18 --> 112.80]  And this is where we want to, in line, install the relays so we can control the pumps and the water heaters.
[112.80 --> 115.82]  How hard could that be to find a negative?
[116.56 --> 118.48]  You know, there's this panel full of wires.
[119.16 --> 122.02]  I mean, 50, 60 different wires in there at least.
[122.26 --> 122.68]  Bundles.
[123.78 --> 126.94]  And, Jeff, how hard was it to find ground?
[128.02 --> 130.90]  Well, we assumed the one we had would work and it didn't.
[131.46 --> 135.90]  We tried the thermostat and ended up turning on the furnace.
[136.06 --> 137.44]  Yeah, it uses negative for signaling.
[137.72 --> 137.90]  Yeah.
[138.00 --> 140.78]  And when you cut the negative, the furnace turns on.
[140.94 --> 141.92]  Or just put a load on it.
[141.92 --> 143.94]  Yeah, it freaked out about that.
[144.38 --> 148.00]  And that was after we already had it all buttoned up and thinking, yeah, this is the right way to go.
[148.06 --> 148.54]  It's tested.
[148.68 --> 149.10]  It works.
[149.26 --> 149.38]  No.
[150.10 --> 150.28]  Yeah.
[150.50 --> 150.80]  Yeah.
[151.06 --> 153.38]  That feels so confusing to me.
[153.42 --> 155.64]  Like, why is that the choice that they made?
[155.76 --> 157.16]  Surely that's not a standard, right?
[157.16 --> 158.58]  It's one less wire they had to run.
[158.78 --> 159.62]  That's exactly it.
[160.08 --> 161.50]  And, you know, they're running it across the RV.
[161.66 --> 162.16]  I don't know.
[162.16 --> 162.56]  Yeah.
[163.28 --> 169.72]  But there is also a little LCD panel on there that shows you the runtime of the generator.
[169.98 --> 171.74]  You know, that's how you kind of keep track of your generators.
[171.74 --> 172.68]  Here's the hours it runs.
[173.34 --> 174.84]  And Jeff was looking at that.
[175.46 --> 177.34]  And we'd mentioned it at one point.
[177.42 --> 179.64]  But I think maybe we dismissed it for some reason or another.
[179.74 --> 180.20]  I don't remember.
[180.52 --> 184.56]  I was more worried that we'd turn something else on unintentionally.
[184.56 --> 185.18]  Yeah.
[185.42 --> 193.20]  I had to run around and, like, physically disable my slides because we'd kept setting the panel down on the counter, which would then push the buttons for the slides.
[193.24 --> 194.92]  And the slides would start coming in while we were working.
[195.34 --> 195.98]  Like, hold on.
[196.02 --> 196.76]  I'll go unplug them.
[197.38 --> 200.12]  So there was a little bit of, you know, we're working on a live system here.
[200.90 --> 205.52]  But honestly, once you found the ground, the rest was really simple.
[205.68 --> 208.16]  It's ESP home on these little devices.
[208.88 --> 210.84]  Standard little relay that you can get off of Amazon.
[210.98 --> 212.16]  We'll have some links in the show notes.
[213.10 --> 215.52]  And then Home Assistant discovers it.
[215.52 --> 218.94]  And the relay shows up as a switch to Home Assistant.
[219.10 --> 220.32]  So I can just toggle that relay.
[220.78 --> 222.26]  And I'm toggling the water heater.
[222.38 --> 223.84]  I'm toggling the water pump on and off.
[225.24 --> 226.42]  I've wanted it for so long.
[226.84 --> 229.22]  Now, Jeff, I think you learned a few things during this project, right?
[229.54 --> 229.74]  Yeah.
[229.80 --> 234.14]  A few words of caution when dealing with relays and these ESP boards.
[234.26 --> 237.08]  We're using, like, a D1 Mini or a clone of it.
[237.12 --> 237.98]  It's all the same thing.
[238.04 --> 240.88]  You can use a NodeMCU, just about any of those boards.
[241.28 --> 245.32]  Make sure you look at the board you're using and find its pinout.
[246.52 --> 250.96]  And there are certain pins that you're not supposed to use relays on.
[251.32 --> 256.48]  When it gets power, it might hammer it and not actually close or open just as they're in vibrates.
[256.62 --> 259.68]  And that's something in the past that tripped me up for quite a while.
[260.02 --> 263.58]  But these little devices can have numerous relays.
[263.74 --> 266.48]  I believe the D1 Mini was four or five.
[266.88 --> 267.64]  We're using three.
[267.92 --> 269.90]  And all three of them are just fine.
[269.90 --> 270.78]  They're 5-volt relays.
[271.14 --> 272.98]  And they're all taking power through the D1 even.
[273.54 --> 274.80]  So we'll see how long that lasts.
[274.80 --> 275.84]  But it should be okay.
[275.84 --> 280.92]  We were thinking, like, we want to build this in a way that is repairable.
[281.16 --> 287.62]  So if a component fails, we can kind of just unplug the relay in the ESP home and just plug the standard switch back in.
[288.04 --> 290.56]  And then things just go back to the way they were before we did anything.
[290.56 --> 293.90]  That, though, is less of my concern.
[293.90 --> 309.38]  Because what I feel like I have learned over the last few years of when I first started trying smart home automation and all that was really available was, like, the Hughes products and the really expensive commercial products, I don't know if I've ever had a single one that doesn't eventually die on me.
[309.54 --> 310.28]  They die out.
[310.36 --> 310.98]  They burn out.
[310.98 --> 317.26]  And then you end up having this $300 piece of lighting equipment that is entirely proprietary.
[317.26 --> 323.84]  And what I'm kind of coming around to, especially with these relays and whatnot, is all of them are modular.
[324.34 --> 325.74]  The relay can be replaced.
[326.42 --> 328.18]  The ESP home can be replaced.
[328.42 --> 330.24]  The power supply can be replaced.
[330.24 --> 335.20]  And they can just be swapped out with standard stuff that is documented everywhere.
[335.98 --> 345.26]  And I'm a lot more comfortable building that into the wall than I would be, like, a TP-Link smart switch or a Hughes light dimmer or something.
[345.36 --> 349.44]  I just would not ever want to build that into the wall and then seal it.
[349.44 --> 361.36]  But with something like an ESP, and especially since ESP home is so easy to manage with Home Assistant, it's a different kind of – it's not reliability.
[361.58 --> 362.30]  What would you call that?
[362.62 --> 364.74]  Not worried about the obsolescence issue either.
[364.90 --> 365.14]  Yeah.
[365.28 --> 371.62]  It's not going to, like, in five years, I'm not going to log into the app to update the app or update the firmware or something.
[371.62 --> 379.70]  Now, I think it was, like, a year or two ago, I was at Alex's place, and he had me do something similar with Shelleys, throw a bunch of them behind switches and things like that.
[379.88 --> 381.54]  Why not use those?
[381.74 --> 384.92]  Because I know those are pretty well built and they're well tested and all that.
[385.38 --> 388.30]  The Shelleys, I believe, are all using 120-volt AC.
[389.02 --> 390.56]  So they're meant for residential wiring, right?
[390.86 --> 393.28]  I think they might have one or two that's DC, I think.
[394.16 --> 395.42]  It's definitely an option, right?
[395.50 --> 396.04]  I like them.
[396.14 --> 400.16]  In fact, some of them even have some features these don't have, like power monitoring built in and whatnot.
[400.16 --> 404.84]  I guess one downside, they throw up their own Wi-Fi AP, right?
[405.18 --> 405.96]  Well, there's that.
[406.18 --> 408.70]  I think you can flash them, but there's that.
[408.78 --> 415.46]  But the other thing is these, I mean, a four-pack of these is, like, you know, nothing.
[416.02 --> 419.56]  The pricing is such that you can bang out a whole bunch of them.
[420.38 --> 422.14]  Yeah, a three-pack is $16.99.
[422.40 --> 423.74]  And have spares on site, too.
[423.88 --> 424.10]  Yeah.
[424.58 --> 426.66]  And so that's really nice.
[426.90 --> 429.92]  And then there's a good community around the ESP Home stuff, too.
[430.64 --> 431.56]  So I like that a lot.
[431.60 --> 434.06]  And I think the integration, there's a little tighter with Home Assistant.
[434.22 --> 438.36]  And if you're thinking about something, I'm going to need a firmware update for 10 years or some five years or whatever.
[439.22 --> 442.86]  I think I prefer that route, the community open source route with the ESP Home stuff.
[442.94 --> 444.68]  But I think the Shelleys are good devices.
[444.92 --> 446.72]  Do you have a strong preference yourself, Jeff?
[446.84 --> 448.26]  I haven't played with the Shelleys at all.
[448.26 --> 453.86]  And funny enough, Alex is actually the one to introduce me to ESP Home and help me through it.
[454.22 --> 459.22]  Because my thinking with these ESP boards was I need to get a binary and flash it with PyFlasher.
[459.36 --> 463.22]  Like, there's a, you know, ESP board flasher for Linux and or for anything.
[463.84 --> 464.94]  And that was my first thinking.
[465.04 --> 466.54]  I couldn't find a binary anywhere.
[466.72 --> 467.48]  I'm looking everywhere.
[467.48 --> 469.48]  Like, where's the ESP Home binary?
[469.68 --> 470.68]  I just couldn't find it.
[470.88 --> 474.34]  And I'm going through the documentation, realizing that everybody's compiling it.
[474.54 --> 475.90]  And I've had issues with that before.
[476.42 --> 477.48]  And eventually, it's like, no, dummy.
[477.56 --> 478.76]  Do it through Home Assistant.
[479.60 --> 480.22]  What do you mean?
[480.30 --> 483.94]  You just put the ad on in Home Assistant, plug the dang thing in, and follow the instructions.
[483.94 --> 486.34]  And eventually, it finally clicked in my dumb brain.
[487.10 --> 489.06]  And it is really that simple.
[489.20 --> 493.88]  You plug it into either your host laptop that you're on or the Home Assistant machine, which is a little bit easier.
[494.44 --> 495.86]  And you just follow the instructions.
[496.20 --> 500.54]  It'll write a full config that works with ESP Home standard.
[501.00 --> 504.32]  And then you can edit that YAML config to what you want to use it for.
[504.76 --> 509.06]  Yeah, you can tweak device name or add additional relays like we did with switch names.
[509.10 --> 510.90]  And then you can name the individual relays in the YAML.
[510.96 --> 511.90]  It's all really easy to read.
[511.90 --> 514.40]  It's the first time I'd ever done it, and it all made sense to me.
[514.94 --> 517.58]  So now, you may both have different answers to this question.
[517.66 --> 521.36]  But I'm curious what you think was the most challenging part of this project in particular.
[521.62 --> 524.14]  It's always the little things, right?
[524.32 --> 530.94]  Like trying to figure out where to pull ground from, how to get them installed where they don't block the wiring,
[531.28 --> 533.70]  or getting these screws in this one spot.
[533.78 --> 535.26]  Don't you feel like it's always the little things?
[535.74 --> 538.90]  Yeah, it's the addition of everything together, the small things together.
[538.90 --> 543.88]  You know, the ground issue we brought up, and we tried running wire from one side of the wall to the other through the crevices.
[544.04 --> 544.58]  That didn't work.
[544.64 --> 547.00]  I mean, just all sorts of little stuff like that.
[547.28 --> 549.70]  There's also a bit of a tedium when building these.
[549.96 --> 551.28]  A lot of small solder joints.
[551.80 --> 555.62]  You know, we're working one ESP with three relays.
[555.62 --> 559.20]  That's three 5 volts, three grounds, three data transfer.
[559.68 --> 565.88]  And then making all the connectors for it to be compatible with the original switches as well.
[566.62 --> 567.46]  That's a separate thing.
[567.52 --> 570.70]  So I don't want everything screwed in the screw terminals because they're quite terrible.
[570.86 --> 571.90]  I wanted everything soldered.
[572.26 --> 574.42]  But I also wanted them to be easily disconnected.
[574.56 --> 578.96]  So we're using the same quick disconnects you'd find in anything automotive, including these RV switches.
[578.96 --> 583.08]  All that together, it's fun for me.
[583.30 --> 585.40]  So it's not really a hard thing, but it's a tedium.
[585.56 --> 588.36]  And then you have to decide ahead of time what your plan is.
[588.48 --> 592.12]  You know, I've never used more than one relay on these ESP boards.
[592.48 --> 594.26]  I wasn't certain it was possible.
[594.36 --> 596.76]  You see those relay boards with multiple relays on them.
[597.22 --> 598.48]  But they usually are not.
[598.56 --> 603.02]  I don't know about usually, but the ones I've seen with, say, 10 relays on them, they do it through I2 squared.
[603.38 --> 606.48]  I've never touched that stuff or whatever that protocol is called.
[606.80 --> 608.08]  I've never used that stuff before.
[608.08 --> 609.02]  I've never used that protocol.
[610.32 --> 611.76]  It's still learning for me, too.
[612.36 --> 613.86]  So a little bit of extra research.
[614.18 --> 614.96]  Of course, scope creep.
[615.14 --> 617.64]  You know, oh, well, we're doing the one.
[617.72 --> 619.40]  We've got to do the other one as well.
[619.52 --> 620.70]  And what about the water pump?
[620.80 --> 621.24]  You know, we're adding.
[621.72 --> 622.54]  Which is fine.
[622.80 --> 624.30]  And that's always fun to learn.
[624.86 --> 628.32]  Well, in reality, it starts with, this button broke.
[628.60 --> 629.66]  We should fix this button.
[629.98 --> 634.64]  And then it goes to, well, if we're going to fix the button, we might as well hook it up to a relay.
[634.90 --> 635.92]  We might as well upgrade it.
[635.98 --> 636.90]  Yeah, and make it better.
[636.90 --> 641.58]  And then it's like, well, if we're going to hook up the electric side to a relay, we've got to hook up the gas side.
[641.66 --> 644.46]  And if we're going to hook up the heater, we've got to have the pump.
[646.16 --> 648.22]  It starts with, let's fix this button.
[648.60 --> 650.38]  Yeah, and literally the physical button is broken.
[650.48 --> 651.60]  That's something else we did, right?
[651.66 --> 655.50]  We had to figure out how to pop those buttons out or the switches out and repair those.
[655.58 --> 657.04]  There was a repair function we were doing, too.
[657.04 --> 659.66]  Yeah, it's all just, it all kind of adds up.
[659.78 --> 660.90]  But it's fun.
[660.98 --> 661.22]  I mean.
[661.72 --> 667.20]  I look at it as, I've tried to look at when things break or, you know, die and need replaced.
[667.30 --> 672.70]  I try to look at it as an opportunity to replace it and build it back better with something that is open.
[672.70 --> 677.54]  You know, I'm big about building back better and open.
[677.54 --> 681.54]  Leno.com slash SSH.
[682.38 --> 687.18]  Head on over there, get $100 in 60-day credit, support the show, and really try things out.
[687.26 --> 689.16]  With that $100, that's their vote of confidence.
[689.32 --> 693.18]  And now, Leno goes from strength to strength because they're now part of Akamai.
[693.28 --> 697.50]  All the tools we like, like the cloud manager that's beautifully built, the API that's well-documented,
[697.58 --> 702.54]  it's got libraries for days, and the command line client, which I'm telling you, hot tip,
[702.60 --> 703.62]  put that in your Quake dropdown.
[703.78 --> 705.36]  All of a sudden, you're like a cloud lord.
[705.78 --> 706.40]  So nice.
[706.40 --> 707.50]  All that stuff's still there.
[707.98 --> 713.40]  They're investing in more, too, because it's combining with the power and global reach of Akamai.
[713.54 --> 715.62]  And you guys know, Akamai is the best of the best.
[716.44 --> 718.62]  They are the really, like, high-end network.
[718.80 --> 723.96]  And they're investing in more cloud computing resources and tooling to give us more reliable
[723.96 --> 729.28]  and still that affordable service that we love that will scale for individuals or a business of any size.
[729.62 --> 732.42]  And now you get access to that global network of offerings.
[732.48 --> 733.98]  Like, the data centers are going in more.
[734.04 --> 735.02]  They just spun up a few more.
[735.02 --> 737.38]  They're launching a whole bunch this year.
[737.56 --> 740.68]  They're going to give us access to more resources and help us grow our business.
[740.78 --> 744.04]  You can serve your project, your customers, your family, whatever it might be.
[744.82 --> 748.00]  You've been thinking about it, or maybe it's time to go deploy a game server for the kids,
[748.06 --> 750.18]  or maybe it's time to go deploy a chat server for work.
[751.52 --> 753.20]  Whatever it is, it doesn't matter.
[753.32 --> 754.98]  They've got the pricing and the scalability.
[754.98 --> 756.30]  So try it out right now.
[756.92 --> 760.16]  Go see The Power of Linode, now backed by Akamai.
[760.28 --> 767.84]  Go to linode.com slash SSH to learn how Linode, now Akamai, can help scale your applications from the cloud all the way out to the edge.
[767.94 --> 771.50]  Like Brent's cabin hanging off a Starlink edge.
[771.70 --> 772.60]  You're going to be impressed.
[773.12 --> 773.54]  Yeah, that.
[773.54 --> 773.94]  I know.
[774.60 --> 776.64]  Linode.com slash SSH.
[776.64 --> 782.08]  Well, back on the show, and it's been forever since Paulus and I chatted.
[782.16 --> 785.96]  I don't know if you remember Paulus, but I think it was still just the first year of Home Assistant.
[786.16 --> 788.46]  You and I had a little video chat a while ago.
[788.56 --> 790.42]  So it's been way overdue.
[790.52 --> 791.08]  Welcome back.
[791.28 --> 791.46]  Yeah.
[791.60 --> 792.30]  Thanks for having me.
[792.72 --> 795.52]  Now, there is so much to get into this week.
[795.52 --> 797.70]  Some of the stuff I'm most excited about this year, actually.
[797.90 --> 801.84]  But I wanted to start with something that caught our co-host Alex's attention,
[801.84 --> 809.90]  and that was the sort of immediate abrupt news about Mazda going after a library, I think, if I have this right, a library dev,
[810.72 --> 818.26]  that unfortunately resulted in also the integration for the Mazda connected services and Home Assistant having to get removed.
[818.26 --> 826.24]  And it's sort of just this heavy-handed, I feel like, strongman tactic that really has me thinking about ownership and what we have rights to.
[826.30 --> 827.04]  It's our own cars.
[827.62 --> 831.18]  And so, Paulus, I know Home Assistant had to make some news on the blog.
[831.18 --> 833.02]  You made a blog post on October 13th.
[833.04 --> 834.22]  Can you kind of fill us in a little bit?
[835.20 --> 835.32]  Yeah.
[835.40 --> 843.70]  So what happened is that a person in our community who maintains a library to interact with Mazda,
[844.34 --> 851.32]  he got a DMCA takedown from GitHub, or GitHub got a DMCA takedown claiming that he had violated copyright.
[851.64 --> 851.94]  I see.
[852.00 --> 853.98]  So Mazda's lawyers went to GitHub.
[854.74 --> 855.02]  Yes.
[855.02 --> 855.92]  Well, two things.
[855.92 --> 862.42]  They went to GitHub and said his Python library violated copyright of both the iOS app and the Android app.
[863.24 --> 871.12]  And they also sent him a cease and desist letter saying he has to stop abruptly all his activities related to integrating Mazda stuff.
[871.12 --> 875.72]  And he was also the maintainer of the Mazda integration and Home Assistant.
[875.96 --> 878.74]  And the Mazda integration and Home Assistant used his library as well.
[878.90 --> 879.18]  I see.
[879.44 --> 886.16]  And so, you know, for him, like, this is just, you know, a person in his spare time working on this.
[886.24 --> 887.74]  Like, he obviously owns a Mazda car.
[887.74 --> 891.16]  So that's why he was invested in this and, like, building this.
[891.26 --> 895.28]  And he was like, yeah, I didn't sign up for this, right?
[895.30 --> 895.90]  I don't want this trouble.
[896.56 --> 896.72]  Yeah.
[897.20 --> 901.38]  And so, yeah, he came to us and we're like, yeah, let's just delete it.
[901.60 --> 903.88]  Because, you know, we've seen it in the past.
[904.00 --> 906.58]  Like, you know, this is a very blunt tactic.
[906.86 --> 911.48]  Like, you know, I don't, it's very, I wish they wouldn't have just sent us an email, right?
[911.54 --> 913.00]  That we can, like, talk about things.
[913.56 --> 916.28]  But the intention is clear, right?
[916.28 --> 918.30]  They don't want to be integrated in Home Assistant.
[918.62 --> 921.02]  And there are many ways to block users.
[921.48 --> 922.74]  Why do you suspect that would be?
[923.38 --> 928.44]  It just doesn't, it doesn't make sense to me because it seems like it just results in dissatisfied customers.
[928.44 --> 931.44]  And it's not, it's not like it's costing them anything, is it?
[931.50 --> 936.66]  I mean, it costs them in that they have a cloud service and, like, they get more API calls, right?
[936.66 --> 945.36]  So, but the Mazda integration had in Analytics 227 users, which, Analytics is opt-in, right?
[945.36 --> 948.48]  With Home Assistant, and it's around one-third opt-in.
[948.56 --> 952.00]  So let's say it's like 750 people were talking to Mazda servers.
[952.44 --> 952.52]  Yeah.
[952.62 --> 954.72]  I doubt that that showed up, right?
[954.88 --> 955.64]  Like, that's just...
[955.64 --> 957.10]  And if it did, they need to build a better infrastructure.
[958.16 --> 958.56]  Yes.
[958.86 --> 961.20]  Because if they sell too many more cars, they're going to be in a problem.
[961.64 --> 961.84]  Yeah.
[961.84 --> 971.78]  I struggle to understand it other than it's like they just want to have their own service, maybe their own app, and they don't want anybody going anywhere else.
[971.84 --> 972.92]  Do you think that could be a component?
[973.10 --> 973.90]  It's just...
[973.90 --> 978.24]  I think it's about, yeah, controlling what users can do and controlling the experience.
[978.50 --> 978.68]  Yeah.
[978.68 --> 984.58]  I think, I mean, this is interesting because this kind of gets into, for example, why some manufacturers are not happy about Matter.
[984.72 --> 987.36]  It's about owning the user experience, right?
[987.36 --> 991.90]  Like, you open the Mazda app and they can upsell you, I don't know, new tires, for example.
[992.32 --> 995.26]  You open the Home Assistant app, we're never going to sell Mazda tires.
[995.66 --> 1001.26]  One question I have around there is, you know, this feels like a bit of a dirty tactic, as you alluded to.
[1001.26 --> 1007.68]  If this worked so easily on this project, do you think they'll just be encouraged to do it elsewhere?
[1008.04 --> 1015.18]  And so how do we, as open source software creators and just a huge community, deal with that?
[1015.52 --> 1018.36]  Because it seems, I don't know, like a real problem.
[1019.20 --> 1023.48]  I think the bigger thing here is that we shouldn't buy those products, right?
[1023.48 --> 1028.78]  Like, in the end, a company, one way or the other, can lock people out of their own data.
[1028.78 --> 1034.24]  And the best way to work around it is to make sure you buy products where that's not possible, right?
[1034.30 --> 1040.24]  So anything with an open standard or anything that can talk locally can just work.
[1040.36 --> 1044.16]  Like Zigbee, Z-Wave, or Matter device, they can never take away from you, right?
[1044.20 --> 1045.82]  There's just no cloud necessary.
[1045.94 --> 1048.38]  There's no ping back home necessary to set it up.
[1048.42 --> 1049.16]  It just works.
[1049.90 --> 1052.70]  You have also, like, non-open standards.
[1052.70 --> 1055.46]  Like, you know, you have those Shelly relays.
[1055.60 --> 1057.08]  They open an access point, right?
[1057.08 --> 1058.90]  And locally, you connect to it, you set it up.
[1059.20 --> 1061.64]  There's also no cloud necessary to configure.
[1061.90 --> 1067.52]  And those companies can, you know, once you have that product, you can do whatever you want with it.
[1068.36 --> 1072.98]  The car is maybe a problem for the future.
[1072.98 --> 1079.96]  But you guys have made incredible progress this year on solving this problem for the voice assistants.
[1079.96 --> 1081.34]  And it's been the year of voice.
[1081.90 --> 1086.80]  And we've been watching chapter one and chapter two come out and chapter three.
[1087.02 --> 1090.92]  And now in October, we've got chapter four, Wake Words.
[1090.92 --> 1091.42]  The big one.
[1091.60 --> 1092.28]  The big one.
[1092.42 --> 1095.58]  I have to imagine this was what everybody was asking for from the very beginning.
[1096.24 --> 1096.38]  Yeah.
[1096.38 --> 1098.34]  So, you know, we did chapter one in January.
[1098.64 --> 1102.76]  And, you know, we started, like, we called it, I was like, we were reading the book backwards, right?
[1102.76 --> 1107.38]  So we started with just intent recognition without even dealing with speech or Wake Words.
[1107.48 --> 1110.36]  It was just intent recognition because you kind of built everything on top of that.
[1110.96 --> 1113.46]  And since January, people are like, where's Wake Words?
[1113.56 --> 1116.52]  Like, how can this ever replace my Google if there's no Wake Words?
[1117.04 --> 1117.14]  Yeah.
[1117.14 --> 1119.02]  And it's not that we didn't know.
[1119.14 --> 1122.08]  It's just like, no, all these different pieces have to be in place.
[1122.24 --> 1125.54]  Like, a voice assistant is a very complicated stack, right?
[1125.58 --> 1127.48]  Like, it's all these different parts.
[1127.74 --> 1129.76]  And everything has to work well enough.
[1130.04 --> 1131.94]  Otherwise, the chain falls apart.
[1132.94 --> 1133.00]  Yeah.
[1133.06 --> 1137.56]  From connectivity to room quality and audio quality.
[1137.56 --> 1145.10]  And so I'm really, really impressed with what is version one, or if you'll even call it that, seems to be.
[1145.10 --> 1147.30]  And can you kind of describe the stack?
[1147.38 --> 1155.26]  Because the way I break it down, Paul, is what we're really looking at now is three incredible open source projects that are coming out of Nebukasa.
[1155.60 --> 1157.60]  Piper, we have the Open Whisper.
[1158.12 --> 1159.98]  Well, actually, four if you consider the Wyoming Protocol.
[1160.20 --> 1161.68]  And now we have Open Wake Word, right?
[1161.76 --> 1173.88]  So in my world, I see these as three containers that I can run on my system that now give me the capability to do local text-to-voice and voice-to-text and speech recognition.
[1173.88 --> 1175.08]  It's a pretty incredible stack.
[1175.82 --> 1176.06]  Yes.
[1176.32 --> 1176.46]  Yeah.
[1176.46 --> 1179.54]  And this is actually how we've always envisioned it, right?
[1179.62 --> 1181.18]  Like, I mean, home assistant is about choice.
[1182.00 --> 1191.22]  And so we've been building it up to make sure that through the Wyoming Protocol, which is really the piece that unlocks this all,
[1191.22 --> 1199.26]  which is an open protocol for integrating voice assistant pieces into, like, a bigger voice assistant stack.
[1199.42 --> 1202.98]  And so, you know, the home assistant box itself might not be the most powerful.
[1203.22 --> 1205.24]  People are running Open Whisper on it.
[1205.32 --> 1206.14]  The speech or text.
[1206.14 --> 1209.32]  People are running Piper on it.
[1209.80 --> 1211.60]  Whisper is not so good on a Raspberry Pi.
[1211.74 --> 1213.86]  It takes too long to really transcribe.
[1214.48 --> 1217.86]  Piper is good enough because we cache all the outputs that it generates.
[1217.86 --> 1220.02]  So the first time it's slow afterwards, it's fast.
[1220.60 --> 1223.80]  But because of Wyoming, it doesn't have to run on home assistant, right?
[1223.82 --> 1224.92]  You have a bigger server.
[1226.00 --> 1227.50]  It can just run over there.
[1227.76 --> 1229.34]  You're subscribed to home assistant cloud.
[1229.44 --> 1230.66]  It can also run in the cloud.
[1230.66 --> 1232.72]  You don't even have to run it locally if you want to.
[1233.40 --> 1236.06]  And it really allows for choice.
[1236.36 --> 1240.32]  And I think what is more important for us is it allows for experimentation.
[1240.92 --> 1244.68]  So open source people are always tinkering with stuff, right?
[1244.76 --> 1247.16]  Like, home assistant didn't just start.
[1247.34 --> 1250.46]  Like, it was because I was tinkering with something and it kind of grew into something.
[1250.66 --> 1253.78]  And the same with every other open source project.
[1253.98 --> 1258.62]  So allowing people to easily tinker with text-to-speech or speech-to-text or wake words
[1258.62 --> 1263.26]  and seeing how that fits into a whole voice assistant, that's now super easy.
[1263.90 --> 1268.64]  And that will hopefully result in even more and better projects that we can all leverage.
[1269.18 --> 1274.74]  Well, I definitely see the wheels spinning already because what I think is pretty fantastic here
[1274.74 --> 1278.22]  is with Wyoming, I can run components individually.
[1278.36 --> 1281.98]  So in my example, my home system runs off of a yellow.
[1282.32 --> 1288.50]  But I also have an Odroid that I run the more processor-intensive stuff on.
[1288.62 --> 1290.22]  And it just connects over Wyoming.
[1290.48 --> 1291.82]  And it's wicked fast.
[1291.96 --> 1298.56]  But I actually got started by using the built-in Nebukasa service stuff just to experiment to
[1298.56 --> 1299.70]  see if it was worth playing with.
[1299.88 --> 1301.94]  And that took 10 seconds to set up.
[1302.40 --> 1303.90]  And it's really good.
[1304.86 --> 1307.64]  So that, I mean, a lot of people would be happy with just that, I think.
[1307.70 --> 1309.10]  What's the privacy story there?
[1309.10 --> 1316.96]  So the privacy story there is that there's two different types of clouds, more or less, right?
[1316.98 --> 1321.48]  You have an IoT-specific cloud where every data you upload is tied to your user account,
[1321.66 --> 1324.18]  tied to your devices and states and these kind of things.
[1324.56 --> 1331.24]  And then you have the more service-oriented cloud, like just pure AWS, pure Azure, pure Google
[1331.24 --> 1331.72]  cloud.
[1331.72 --> 1337.56]  And our voice APIs in the Nebukasa offers, they're not tied to a user.
[1337.82 --> 1341.28]  They are tied to like the authentication token.
[1341.88 --> 1343.90]  And it's not connected to a user account.
[1344.38 --> 1345.80]  We don't store that data.
[1345.98 --> 1347.60]  Azure doesn't store that data.
[1347.78 --> 1349.72]  It's just giving you the text back.
[1349.92 --> 1351.52]  It doesn't go through Home Assistant Cloud.
[1351.70 --> 1354.16]  Like your Home Assistant instance is talking directly to Azure.
[1354.42 --> 1358.62]  And it's not tied to your home or identity in any way.
[1358.62 --> 1361.46]  So it doesn't like, you're not going to see Facebook ads, right?
[1361.46 --> 1363.74]  Because you asked about like whatever.
[1364.16 --> 1368.86]  So it's significantly better than compared to say using an Echo or the Google Home Assistant.
[1369.08 --> 1369.18]  Yeah.
[1369.52 --> 1369.72]  Yeah.
[1369.74 --> 1373.00]  Because if you look at Echo or Google, you could go into the history.
[1373.14 --> 1377.98]  You can actually see, you know, they will tell you all the things you've told them and
[1377.98 --> 1380.48]  they will show it to you in context of your home, right?
[1380.52 --> 1383.40]  So it's like, oh yeah, they have made that link directly.
[1383.72 --> 1384.80]  That's the goal.
[1385.06 --> 1385.24]  Yeah.
[1385.40 --> 1386.58]  They're not even hiding it anymore.
[1386.58 --> 1386.74]  Yeah.
[1387.32 --> 1387.64]  Yeah.
[1387.66 --> 1390.40]  I remember when I first tried the Echo, you could even go back and I don't know if they
[1390.40 --> 1391.80]  still do this, but you could play the clip.
[1392.78 --> 1392.90]  Yeah.
[1392.90 --> 1393.10]  Yeah.
[1394.62 --> 1394.98]  Okay.
[1395.02 --> 1400.56]  So one of the things obviously that is really exciting about an open project like this
[1400.56 --> 1404.00]  is people will be able to set their own wake words.
[1404.40 --> 1406.22]  You come with a bunch of presets.
[1406.58 --> 1410.58]  Like I think the okay now boo is a good one just because that's probably not a very common
[1410.58 --> 1411.04]  phrase.
[1411.76 --> 1413.66]  Hey, Jarvis is also kind of fun in there.
[1413.66 --> 1418.02]  Um, but you know, pause, everybody wants to make their own wake words.
[1418.22 --> 1423.50]  And, uh, I did play around with the collab book that you guys link in the blog post, but
[1423.50 --> 1426.28]  you know, when I crank it up, it doesn't really want to play along.
[1426.72 --> 1428.76]  What are sort of the future plans there?
[1428.76 --> 1433.80]  If any, to make it approachable for people to create their own wake words, maybe even
[1433.80 --> 1435.98]  through the home assistant UI one day or something like that.
[1435.98 --> 1440.50]  So the right now it requires quite a lot of training.
[1440.50 --> 1445.04]  The notebook that we put out, like at the bottom, you can change some of the parameters.
[1445.60 --> 1449.00]  And the reason that it like, it really creates a basic wake word.
[1449.10 --> 1455.74]  The wake words you create with that collab notebook are using the same pipeline as, uh, you know,
[1455.74 --> 1457.06]  the open wake word pipeline.
[1457.18 --> 1461.98]  I'm not sure if I can explain how it works where like it uses a base model from Google.
[1461.98 --> 1466.98]  It uses Piper to generate a lot of different sentences based on different speakers.
[1467.24 --> 1472.84]  And then it is able to mix speakers to create new kind of like sounding voices.
[1472.84 --> 1479.02]  So we can generate like 20, 30,000 samples of saying the wake word that you want to use.
[1479.40 --> 1481.92]  And also you inject different types of background noise too.
[1481.98 --> 1484.94]  I saw it pulling down flacks of different kinds of noise environments.
[1484.94 --> 1485.38]  Yes.
[1485.82 --> 1490.96]  So we do noise environments and we also, um, mutate the sounds so that like close to the
[1490.96 --> 1494.20]  microphone, far away from the microphone, these kinds of things.
[1494.44 --> 1498.84]  And then we fine tune that model to detect, you know, that wake word.
[1499.34 --> 1503.00]  And the last step is that we run it against a negative sample.
[1503.20 --> 1506.08]  So there's like podcast databases out there.
[1506.30 --> 1511.18]  And you just basically play all that podcast to the model and say, this is not the wake word.
[1511.22 --> 1512.00]  This is not the wake word.
[1512.04 --> 1512.86]  This is not the wake word.
[1513.04 --> 1513.72]  That's great.
[1513.92 --> 1514.22]  No way.
[1514.22 --> 1519.06]  And that's like, you know, you put 2000 hours of podcast against it and it's actually like,
[1519.14 --> 1522.04]  you know, it really helps the model learn the wake word even better.
[1522.34 --> 1528.82]  And so the Colab notebook that we made available, we kind of limited all those steps just so
[1528.82 --> 1531.32]  that it fits within the free compute that Google offers.
[1531.50 --> 1531.60]  Right.
[1532.02 --> 1533.12]  Which, which is limited.
[1533.12 --> 1536.88]  And it almost made me want to go sign up and see if I could put it in a much more powerful
[1536.88 --> 1539.54]  machine because I wanted, I just wanted to crank it.
[1540.12 --> 1540.24]  Yeah.
[1540.24 --> 1541.84]  But you can run all of this at home, right?
[1541.86 --> 1543.08]  Even on a desktop computer.
[1543.08 --> 1544.10]  To a degree.
[1544.22 --> 1544.90]  To a degree.
[1545.02 --> 1545.94]  I did give it a go.
[1546.58 --> 1548.02]  We got close, Paul.
[1548.08 --> 1551.74]  We got close to getting the whole Python environment working, but I don't think we got it at 100%.
[1551.74 --> 1553.58]  That's the problem, right?
[1553.64 --> 1556.24]  Like setting up like these scientific environments.
[1556.24 --> 1558.62]  They're very particular about all the versioning.
[1558.62 --> 1563.40]  We've been looking into a Docker container, but then you need like GPU pass through and these
[1563.40 --> 1564.34]  kinds of things for training.
[1564.34 --> 1569.52]  And that's just, there needs to be a better way, but there is actually already one kind
[1569.52 --> 1573.72]  of shortcut that we can take that open wake word supports, but that home assistant doesn't
[1573.72 --> 1574.16]  support.
[1574.16 --> 1579.18]  And it's called, actually, I'm not sure how it's called, but it's fine tuning with voice
[1579.18 --> 1584.12]  samples recorded by the voice satellite who is going to feed audio into the model.
[1584.12 --> 1590.60]  So by you talking to your microphone, that is the one in your RV, for example, it will
[1590.60 --> 1591.78]  learn about the room.
[1591.96 --> 1595.88]  And basically you say three times or four times and the model can get really tailored
[1595.88 --> 1596.74]  to your voice.
[1597.06 --> 1597.62]  That's so neat.
[1598.18 --> 1598.54]  Right.
[1598.54 --> 1600.64]  Like some real world training right then and there.
[1600.82 --> 1601.04]  Yeah.
[1601.60 --> 1602.56]  Oh, that's cool.
[1602.58 --> 1604.48]  That part we're going to bring to home assistant, right?
[1604.52 --> 1608.42]  So that is like a small step, but should help with like the training.
[1611.10 --> 1612.38]  45homelab.com.
[1612.48 --> 1613.26]  It's here.
[1613.40 --> 1614.02]  It's big.
[1614.10 --> 1614.60]  It's strong.
[1614.64 --> 1615.48]  And it's fast.
[1615.96 --> 1620.32]  The 45 Home Lab, that's a new division from 45 drives that takes their enterprise design
[1620.32 --> 1624.84]  philosophy and brings it to a scale that works for us home labbers.
[1624.84 --> 1627.80]  And the HL 15 has launched.
[1627.80 --> 1630.34]  It is available for purchase right now.
[1630.46 --> 1632.04]  It comes in different configurations.
[1632.22 --> 1633.18]  You can get just the chassis.
[1633.34 --> 1638.12]  You can add the backplane, add a PSU or get the fully built unit ready to go.
[1638.60 --> 1641.70]  I mean, the early response from the self-hosted community was strong.
[1641.82 --> 1644.72]  We gave them a lot of feedback, way more than they expected, they said.
[1645.52 --> 1648.86]  And they've really built a solution based on that feedback.
[1649.16 --> 1650.86]  And it's powered by open source.
[1650.98 --> 1652.02]  It's running Rocky Linux.
[1652.16 --> 1653.22]  It's an open design.
[1653.38 --> 1655.74]  So you get freedom and control over the system.
[1655.74 --> 1661.80]  All of the HL 15 units are using the 45 drives well-known direct wired approach, which means
[1661.80 --> 1666.28]  you open up the lanes directly to the motherboard, providing high performance for that home lab.
[1666.36 --> 1667.28]  It's a screamer.
[1667.74 --> 1671.28]  And they've also got an applications hub where they've done some handpicked applications so
[1671.28 --> 1671.96]  you can get up and running.
[1672.36 --> 1673.36]  They got a couple of examples.
[1673.36 --> 1676.76]  I love to see over there like Home Assistant and Nextcloud and Plex.
[1677.00 --> 1680.62]  There's also a community forum that's popping off and people are getting engaged over there
[1680.62 --> 1682.36]  to help support each other that are picking these up.
[1682.44 --> 1685.96]  And they'll have more information soon over at 45homelab.com.
[1686.02 --> 1686.72]  But it's there now.
[1687.12 --> 1689.56]  And it looks so good.
[1689.66 --> 1692.18]  With the different options too, it really fits your different price points.
[1692.26 --> 1695.00]  You know, if you just want the fully built service, that's probably the way I would go.
[1695.42 --> 1695.94]  That's great.
[1695.94 --> 1698.56]  But if you just want to get a chassis and a backplane, you can do that.
[1698.62 --> 1701.26]  Or just the chassis, the backplane and the PSU, you can mix and match.
[1701.74 --> 1703.14]  It's so beautiful.
[1703.14 --> 1708.70]  And it's assembled in North America, built with steel and the real screws, not rivets.
[1708.72 --> 1712.58]  You can actually get access to this thing, modify and take it apart to your heart's desire.
[1713.10 --> 1715.22]  It looks like they nailed it.
[1715.28 --> 1718.90]  Go check it out and order one if you're ready at 45homelab.com.
[1718.94 --> 1720.52]  And if you get one, I'm jelly.
[1720.52 --> 1723.96]  I feel like they ought to send the pod a review unit.
[1725.94 --> 1727.70]  I really want one.
[1727.78 --> 1728.24]  Can you tell?
[1729.60 --> 1730.20]  All right.
[1730.24 --> 1732.92]  Congratulations to the team over at 45 Drives.
[1733.08 --> 1736.12]  And go check it out at 45homelab.com.
[1737.80 --> 1740.88]  It sounded like you're both very happy with some of the results.
[1740.90 --> 1746.62]  But it sounded like there was also some areas you already know you want to improve upon in the pipeline or maybe in the recognition.
[1747.16 --> 1747.34]  Yeah.
[1747.34 --> 1750.32]  You know, we really like Open Wake Word.
[1750.46 --> 1752.28]  But it's based on this model by Google.
[1752.28 --> 1756.72]  And this is actually really necessary because speech to text is hard.
[1757.22 --> 1764.34]  And to create a proper speech to text model, you need to basically have a lot of input data.
[1764.46 --> 1766.64]  You need like Google scale of data, right?
[1766.64 --> 1773.86]  So the fact that Google put this model out open source is great because they have traded on whatever input they have access to, which is a lot.
[1774.54 --> 1777.62]  However, Google's model doesn't run on ESP32.
[1778.00 --> 1782.94]  And that's why we have to run it inside Home Assistant or, you know, with Wyoming on another server.
[1782.94 --> 1791.46]  But it means for the user experience, if they add like multiple voice satellites, I think the limit is five right now for Raspberry Pi 4.
[1791.76 --> 1795.92]  You're going to max out whatever your Raspberry Pi 4 can do, right?
[1795.96 --> 1802.06]  So we really would love for the wake word detection and some of the audio cleanup all to happen on the ESP32.
[1802.06 --> 1805.88]  Where it doesn't think that means that you can just scale up.
[1805.98 --> 1816.38]  Like if you have like, I don't know, you want one in every bedroom, bathroom, living room, kitchen, like you might end up with like eight voice satellites and it shouldn't impact how Home Assistant runs.
[1816.90 --> 1817.88]  Yes, that would be really nice.
[1818.40 --> 1819.26]  Because I'm going to be that guy.
[1819.46 --> 1819.88]  I am.
[1820.28 --> 1821.52]  I'm going to have him outside.
[1821.70 --> 1822.56]  I'm going to have him everywhere.
[1822.56 --> 1823.04]  Yeah.
[1824.24 --> 1834.90]  Also, the cool thing is right now with present sensors, you could disable wake word listening if you're not in that room to make sure that nobody is, it doesn't overload the system.
[1835.08 --> 1837.02]  That's a great idea.
[1837.68 --> 1838.16]  Yes.
[1838.56 --> 1838.90]  Okay.
[1839.00 --> 1842.22]  That'll be, that'll be my little hack that I'll use until we get that sorted out.
[1842.64 --> 1847.52]  I kind of also, though, do like the satellite streaming model.
[1847.52 --> 1851.06]  I see what you're saying and the advantages of local processing do sound really good.
[1851.06 --> 1858.66]  But the benefits of the streaming model that it is, that we have now is, it means the satellite requirement is basically nothing.
[1858.98 --> 1859.08]  And.
[1859.50 --> 1859.68]  Yeah.
[1860.16 --> 1864.66]  That gives me a lot of options in terms of like building little custom rigs.
[1864.72 --> 1870.50]  I don't know if that's really going to happen, but it feels like I have a lot more options when the satellite's just kind of a dumb stream.
[1871.34 --> 1871.94]  Oh, for sure.
[1872.00 --> 1877.02]  I mean, you, I don't know if you saw the video of Paul who made that robot from Star Wars.
[1877.02 --> 1877.22]  Yeah.
[1877.22 --> 1878.20]  That is now a voice assistant.
[1878.20 --> 1888.14]  Like that wouldn't have been possible if he also, besides having to learn how to 3D print and servo move robots around, also had to build a voice assistant into that.
[1888.24 --> 1888.38]  Right.
[1888.52 --> 1888.74]  So.
[1889.48 --> 1889.96]  Yeah.
[1890.02 --> 1891.92]  It's really, in that part, I agree.
[1892.30 --> 1896.36]  The challenge there is that not every microphone is the same.
[1896.36 --> 1911.90]  So Espressif has made some, the ESP32 S3 box available, which is two microphones and they made algorithms available to do like a blind source separation, acoustic ego cancellation, a bunch of these cleanup things.
[1912.00 --> 1913.74]  And that is happening on device, right?
[1914.32 --> 1914.54]  Yes.
[1914.54 --> 1915.58]  That would happen on device.
[1915.72 --> 1915.96]  Yeah.
[1915.96 --> 1920.66]  That does look like, that seems like that's the box I want to really go in on.
[1920.66 --> 1922.24]  I think when it becomes generally available.
[1923.14 --> 1923.30]  Yeah.
[1923.64 --> 1925.74]  So that, that's, that's their next target.
[1925.88 --> 1926.72]  I would say also, right?
[1926.76 --> 1928.28]  Like it's to get that box.
[1928.98 --> 1931.32]  Eventually I want to, we want to build our own hardware.
[1931.68 --> 1935.62]  We want to, cause that box doesn't look nice, right?
[1935.62 --> 1938.88]  It looks still too geeky.
[1938.88 --> 1942.58]  Like, you know, you're, we think about the home approval factor, right?
[1942.60 --> 1944.36]  Like, Hey, you want to put this in your living room.
[1944.36 --> 1949.70]  And like right now I just have a cord dangling with an atom ego at the end of the floor in my living room.
[1949.90 --> 1950.02]  Yeah.
[1950.32 --> 1950.54]  Yep.
[1950.98 --> 1951.20]  Yep.
[1951.36 --> 1953.00]  And that, you know, it needs to look nice.
[1953.04 --> 1955.42]  It needs to fit in with the decor and these kinds of things.
[1955.56 --> 1963.08]  So we want to build some hardware that really blends in, but I think we want to have on device wake words ready for that.
[1963.96 --> 1969.38]  The, the bigger challenge will be, can we get custom wake words running on that device?
[1969.52 --> 1969.84]  Yeah.
[1970.52 --> 1971.94]  That would be pretty great.
[1971.94 --> 1973.50]  Um, okay.
[1973.50 --> 1975.72]  So here's my last kind of your voice question.
[1975.84 --> 1981.68]  As I'm looking at the broader open source ecosystem, of course, I'm a long time Linux desktop user.
[1982.28 --> 1991.84]  I'm very, very excited by the projects that have come out of the year voice because they are not necessarily dependent on home assistant.
[1991.84 --> 1993.50]  They can just run on Linux.
[1993.54 --> 1995.20]  And I think there's a lot of possibilities there.
[1995.20 --> 2002.40]  Have, have you seen any, any other projects looking at this work at using some of this work in some of their projects?
[2003.56 --> 2003.72]  Yeah.
[2003.76 --> 2004.98]  Especially around Piper.
[2005.14 --> 2007.44]  Piper has seen a lot of uptick.
[2007.58 --> 2011.90]  Um, because Piper is a neural network yet.
[2011.90 --> 2018.72]  We optimize it to run on a Raspberry Pi 4, which means that if you run it on a Linux desktop with like an Intel processor, it's going to run fast.
[2018.72 --> 2019.16]  Mm-hmm.
[2019.16 --> 2029.60]  And so there was a bunch of screen readers that have adopted Piper now so that they, because, you know, if you're on a screen reader and you want to quickly skip through every button, right?
[2029.62 --> 2034.46]  So you're like pressing, read the next part, read the next part, like, you know, for, for blind people to navigate.
[2035.22 --> 2037.02]  And Piper can just keep up, right?
[2037.06 --> 2039.02]  Like Piper is really useful there.
[2039.02 --> 2044.32]  We also see that there was this, the, the National University of Uzbekistan.
[2045.00 --> 2046.10]  No, was it Kazakhstan?
[2046.90 --> 2048.00]  I think it was Kazakhstan.
[2048.66 --> 2059.86]  They are using Piper to, uh, in their scientific research because there are not a lot of models trained for their language and they were able to train their own models themselves because it's all open.
[2060.14 --> 2060.26]  Right.
[2060.84 --> 2061.04]  Yeah.
[2061.66 --> 2068.40]  And at some point there was also, we lost track of that person, but he was using Piper to, um, get books.
[2068.40 --> 2077.06]  I think in the Philippines, like they turned into audio books so that like more, he could easily distribute like to rural areas, like more, uh, books.
[2078.46 --> 2086.58]  So, you know, once you start doing it, I think somebody made a unity plugin as well so that your NPCs can all have like unique voices.
[2086.98 --> 2089.08]  You know, it can be used for everything really.
[2089.56 --> 2094.60]  I'm excited to maybe see even somebody take a stab at some sort of Linux desktop assistant or something.
[2094.60 --> 2094.90]  Yeah.
[2095.74 --> 2099.44]  I mean, it should be fairly easy because you can use all our different parts.
[2099.54 --> 2103.76]  It's just the, you know, the sentence processing you would have to do for Linux specific.
[2104.08 --> 2104.30]  Okay.
[2104.34 --> 2110.96]  So I want to shift gears a little bit because by around the time, it'll be late this week, Friday morning-ish, this episode's coming out.
[2111.76 --> 2116.14]  We'll probably have some news about a security audit that was conducted at Home Assistant.
[2116.24 --> 2118.36]  Do you have any details there you can share with us at this point?
[2118.36 --> 2121.90]  So the blog post is not out as we record this.
[2122.10 --> 2134.78]  We are still planning to, but because it might be delayed, I cannot like give all the details, but we had, uh, we've hired a company to do a security audit of Home Assistant and they were focusing on our authentication stack, our web stack.
[2135.18 --> 2142.80]  Um, at the same time, or like slightly after that, um, another security team did an audit of Home Assistant.
[2142.80 --> 2149.84]  Now they also found, both, both parties found things, uh, no authentication bypasses.
[2149.90 --> 2150.72]  So that's really good.
[2151.04 --> 2153.80]  Mainly ways to, uh, trick users.
[2154.58 --> 2160.94]  The, the reason we went for a paid audit, because like over the years we've been, you know, sometimes get security issues reported.
[2161.12 --> 2168.02]  We get people auditing Home Assistant and sometimes, you know, like, but you don't know if they've covered everything.
[2168.02 --> 2179.90]  So we did a paid audit to make sure that we define the scope, but we know that they go through all the different parts of our authentication layer to make sure that it, it, it's, uh, audited and it's secure.
[2180.44 --> 2183.58]  Are they looking at the Nabucosta services too in that audit?
[2184.16 --> 2184.46]  Yes.
[2184.56 --> 2188.04]  So they looked at the remote, uh, end-to-end encrypted remote connection as well.
[2188.38 --> 2188.52]  Yeah.
[2188.88 --> 2189.20]  Great.
[2189.20 --> 2205.20]  Um, yeah, because that was like the, in a way we wanted to have the whole stack of like, how do people access Home Assistant, um, from both Home Assistant cloud, but also if you just expose a port on your router, both stacks are fully audited to the authentication core.
[2206.32 --> 2209.98]  And, um, sounds like, uh, there was a couple of things, but nothing too major.
[2209.98 --> 2212.28]  And most of that stuff's already been rolling out patch-wise.
[2213.10 --> 2213.32]  Yes.
[2213.54 --> 2213.76]  Yes.
[2213.76 --> 2221.78]  But we are, um, a bunch of the stuff was done this summer and the audit was done this summer and the fixes have been rolling out in the last couple of months.
[2221.78 --> 2225.80]  So if you've been keeping up to date, you should be good to go.
[2226.00 --> 2230.00]  If you've not been keeping up to date, you could get tricked, I guess.
[2230.06 --> 2230.30]  Right.
[2230.54 --> 2236.72]  Um, but it's not like they can just like go to show them, find Home Assistant instances and like hack, hack, hack, hack, hack.
[2237.12 --> 2237.26]  Good.
[2237.62 --> 2238.18]  Well, that's good.
[2238.36 --> 2242.70]  Now, are you planning to publish some aspects of the report, all of the report or anything like that at some point?
[2242.70 --> 2243.02]  Yeah.
[2243.12 --> 2246.70]  So we're doing a whole, every, every, we have requested CVEs.
[2246.78 --> 2255.52]  Everything is on our, uh, uh, security tab on the Home Assistant core repository, which is basically our, that's the place now where we track all the security issues.
[2255.52 --> 2264.76]  We're also going to, uh, we've updated our security page where we just got to publish a timeline and we want to make it more normal for our community that, hey, security issues happen.
[2264.76 --> 2266.32]  And we're public about it.
[2266.32 --> 2267.16]  We're open about it.
[2267.20 --> 2271.92]  And here you can find them and just have this be more, uh, day to day business.
[2272.30 --> 2274.38]  Like, oh, look, there's a new security issue.
[2274.46 --> 2275.16]  We fixed it.
[2275.30 --> 2276.60]  Uh, please update your stuff.
[2277.28 --> 2286.16]  Uh, because, you know, if you are like an enterprise or a business and you buy software and sometimes you get the security updates, you just update and you kind of go with your day.
[2286.16 --> 2292.42]  Usually users are just not used to that process as much or that their software has leaks and these kinds of things.
[2292.60 --> 2299.94]  So we kind of have to educate them in that sense of like, hey, security issues happen everywhere and it's okay.
[2300.10 --> 2300.96]  We solve them.
[2301.24 --> 2306.60]  And as long as we, you know, are on top of it, we're probably in a good spot.
[2306.98 --> 2307.00]  Yeah.
[2307.00 --> 2307.16]  Yeah.
[2307.52 --> 2309.84]  It's, it's almost impossible, right?
[2309.88 --> 2311.44]  I mean, humans make the software.
[2311.54 --> 2314.30]  It's a very, very, very sophisticated piece of software.
[2314.72 --> 2319.68]  I just, I like the peace of mind of knowing that you guys are on top of it and you're doing the audit thing.
[2319.68 --> 2329.54]  Uh, Paul, as you know, I, I got to admit at the beginning of the year when I think I was watching the stream, when you announced the year of voice, I thought, ah, it's a long shot.
[2330.30 --> 2332.92]  I thought, well, okay, we'll see what we get.
[2333.12 --> 2335.94]  Uh, and now here we are and it's not even the end of the year.
[2335.94 --> 2338.34]  And yeah, I am thrilled.
[2339.16 --> 2339.48]  Yes.
[2339.68 --> 2355.56]  I think that what really helped is it like, you know, the, the things that have come out, some of it was kind of already in the pipeline, like, uh, Piper, like Mike was working on it already, but things like whisper, we didn't know that whisper, like whisper came out of open AI, right.
[2355.58 --> 2361.16]  And open AI created whisper because there was not enough text for them to train chat GPT on.
[2361.24 --> 2362.62]  So they were like, we need more text.
[2362.62 --> 2365.10]  Like let's start transcribing audio and train on that.
[2365.10 --> 2370.82]  And then they made it open source because I don't know exactly why, but it's great for us.
[2371.20 --> 2373.20]  And so open wake word as well, right?
[2373.28 --> 2379.86]  Like, um, David found that model and all of a sudden realized it with Piper and all these pieces falling into place.
[2380.04 --> 2380.16]  Yeah.
[2380.16 --> 2386.80]  And you know, the atom echo, it's not amazing, but it's a $13 little piece of hardware I can use to play around with this.
[2386.88 --> 2388.56]  That's, that's pretty great.
[2388.94 --> 2389.04]  Yeah.
[2389.06 --> 2390.76]  Right now it's sold out everywhere.
[2390.76 --> 2397.48]  But by the end of October, there should be like 3000 more, uh, M5 stack told us, and then they're going to make a bunch more.
[2397.48 --> 2403.58]  Uh, we're also going to look, talk to them because right now you can buy these $13 devices and then you have to go to our website.
[2403.58 --> 2407.24]  And we have this installer browser based installer for ESP devices.
[2407.40 --> 2412.28]  It installs the software on, uh, on the device, but we're actually talking to M5 stack.
[2412.36 --> 2414.70]  Like, Hey, can we just put the voice assistant firmware on it?
[2414.70 --> 2417.90]  Because nobody else uses these devices really, right?
[2417.92 --> 2419.58]  Like this is mainly used for home assistant.
[2419.90 --> 2422.40]  So let's get working out of the box.
[2422.54 --> 2422.72]  Yeah.
[2422.80 --> 2423.92]  So they are looking into that.
[2424.36 --> 2425.94]  Oh, that'd be so great.
[2426.66 --> 2427.24]  Uh, yeah.
[2427.32 --> 2432.80]  In, in the RV when, once, uh, you know, I think I'm going to use the motion detection, the presence detection for this trick.
[2433.18 --> 2433.82]  I'm not kidding.
[2433.86 --> 2435.16]  I'm going to put them in my storage bays.
[2435.26 --> 2439.66]  I'm going to have these little things everywhere outside in the yard so I can control the lights outside.
[2439.84 --> 2442.98]  So let's get it easy because I'm going to be doing a lot of these.
[2442.98 --> 2443.26]  Nice.
[2443.48 --> 2447.24]  Well, Paulus, just, would you please pass our congratulations onto the team?
[2447.34 --> 2447.60]  I will.
[2447.72 --> 2448.28]  And our gratitude.
[2448.94 --> 2456.68]  I think this thing is going to be, uh, a real fire when people really start to figure it out and start playing with it and start building their own devices.
[2457.06 --> 2462.42]  I think it's just going to be a massive hit and, uh, just really excited to see where it goes now that, you know, we're at chapter four.
[2462.56 --> 2466.90]  So keep us posted and, uh, come back in the near future and, uh, give us an update on it, would you?
[2467.06 --> 2467.86]  Yeah, definitely.
[2468.00 --> 2468.74]  Uh, we'll do.
[2469.10 --> 2469.62]  Thank you.
[2469.74 --> 2470.02]  All right.
[2470.02 --> 2470.48]  Thank you.
[2470.48 --> 2474.84]  Tailscale.com slash self hosted.
[2475.02 --> 2477.84]  Go there to get a free personal account for up to 100 devices.
[2478.00 --> 2480.64]  It's a great way to support the show and you can keep it.
[2480.70 --> 2482.02]  It's not a limited time trial.
[2482.28 --> 2483.98]  You can really use it for up to a hundred devices.
[2484.06 --> 2484.68]  So what is it?
[2485.22 --> 2492.48]  Well, Tailscale is a zero config VPN that you can get up and running on your devices in minutes and it's protected by WireGuard.
[2493.42 --> 2493.80]  That's right.
[2493.80 --> 2496.42]  The noise protocol to quickly build out a mesh network.
[2496.42 --> 2500.00]  Doesn't matter if it's Linux, Windows, a mobile device, a VPS, a VM.
[2500.52 --> 2504.18]  A lot of applications have plugins now like VS Code and you can plug it into your container.
[2504.32 --> 2505.86]  Home Assistant has an add-on for it.
[2505.88 --> 2507.44]  I mean, it's just everywhere now.
[2507.80 --> 2509.76]  It also has this great feature called subnet routing.
[2509.76 --> 2516.26]  So if there's a device you can't run Tailscale on, you can turn on a subnet router and then you can get to devices on that subnet.
[2516.68 --> 2518.70]  I do this for like my solar gear.
[2518.80 --> 2521.16]  I do this for my electrical monitoring stuff.
[2521.26 --> 2524.94]  Anything that's like an appliance, like a router that maybe I can't install software on anymore.
[2526.00 --> 2527.40]  Subnet routing takes care of that.
[2527.88 --> 2533.88]  And because it's built on WireGuard, you just have that sort of peace of mind knowing that you're using the best VPN encryption in the business.
[2533.88 --> 2539.18]  And if you're behind double-knack crap like I am, I can attest, Tailscale works like a champ.
[2539.62 --> 2544.72]  And then, guys, you'll start building it out and you'll realize there's just better ways to do things on Tailscale now.
[2544.94 --> 2555.26]  And now with like the Apple TV app as well, you can have totally private media streaming all over an encrypted VPN, flat network, with IPs you know, with names you can resolve.
[2555.48 --> 2557.92]  And then you can use some of the great tooling like Tailscale Send.
[2558.20 --> 2560.52]  It's like AirDrop, but for all your machines on Tailscale.
[2561.40 --> 2563.36]  Or Tailscale SSH, another great one.
[2563.88 --> 2566.64]  Then you can just log in with your Tailscale credentials right as the machine comes up.
[2566.74 --> 2567.76]  That's so handy.
[2567.82 --> 2569.88]  There's a lot more, including the new Mulvab partnership.
[2570.44 --> 2575.44]  So go check it out and support the show by going to tailscale.com slash, you know it, self-hosted.
[2575.50 --> 2578.00]  That's tailscale.com slash self-hosted.
[2579.58 --> 2583.48]  Last episode, I asked for some feedback on a bunch of NextCloud things, which we'll get to.
[2583.56 --> 2585.00]  But first, Ben wrote in.
[2585.72 --> 2591.84]  He says, the one thing keeping me from deleting my Plex container was the fantastic Plex amp for my music.
[2591.84 --> 2596.26]  As none of the Jellyfin alternatives I tried were anywhere near as good.
[2596.90 --> 2600.80]  Recently, however, I discovered the brilliant Symphonium Android app.
[2601.28 --> 2605.88]  You can use the Jellyfin music library as the back end, and it's incredibly customizable.
[2606.24 --> 2607.12]  Well, worth a look.
[2607.42 --> 2608.86]  Cheers and keep up the good work.
[2609.10 --> 2609.36]  Hmm.
[2609.36 --> 2611.14]  It does look like a really good app, actually.
[2611.64 --> 2617.22]  Put a link to this in the show notes, boys, because this is one of the number one things we hear about the Plex switch.
[2618.02 --> 2622.30]  I'd love to switch to Jellyfin, but I'm sticking with Plex because of Plex amp.
[2622.84 --> 2625.18]  So Symphonium, and you can find it in the Play Store, it looks like.
[2625.98 --> 2626.30]  Boom.
[2626.56 --> 2629.24]  Link in the show notes for those of you listening.
[2629.24 --> 2631.66]  Thank you, Ben, for that information.
[2632.08 --> 2634.70]  If I've heard of that before, I completely forgot about it.
[2634.72 --> 2635.56]  So appreciate that.
[2636.44 --> 2639.42]  And speaking of feedback, we got a bunch of great boosts this week.
[2639.44 --> 2642.76]  We're going to try to answer a bigger batch because there's been a lot of good questions.
[2643.48 --> 2648.56]  VT-52 is our baller this week with 110,621 SATs.
[2648.72 --> 2649.08]  Oh, impressive.
[2649.48 --> 2651.88]  And he's got two interesting devices to share with the class.
[2651.96 --> 2653.86]  And he says they're attractive and hackable.
[2654.44 --> 2654.78]  All right.
[2654.96 --> 2655.98]  You're on the right show for that.
[2655.98 --> 2661.40]  One is the Zima board, Z-I-M-A board, around $120 to $200.
[2662.14 --> 2663.88]  It has two to four Celerons in there.
[2663.98 --> 2670.16]  It can go up to eight gigs of RAM, 32 gigabyte eMMC, six-watt TDP, two SATA connectors,
[2670.32 --> 2673.94]  two gigabyte Ethernet, two USB 3, a PCIe 2.0 slot.
[2675.28 --> 2676.60]  Oh, no, I'm sorry.
[2677.24 --> 2679.30]  Four PCIe 2.0 slots.
[2679.36 --> 2680.04]  They're just one X.
[2680.66 --> 2684.04]  It's got a mini DisplayPort and QuickSync.
[2684.04 --> 2687.04]  He also mentions it's passively cooled.
[2688.20 --> 2693.54]  And then the other one, and I have seen this one before, is the Zima Blade, which is bare
[2693.54 --> 2694.32]  bones at $64.
[2694.74 --> 2699.64]  Same specs as above, but only one SODIMM and only one gigabyte Ethernet, only one, you know,
[2699.70 --> 2701.16]  fewer ports and stuff like that.
[2701.46 --> 2703.14]  It's zimaboard.com.
[2703.20 --> 2704.72]  I'm going to put a link to that in the notes, too.
[2705.18 --> 2707.86]  It seems like there are so many options these days for these boards.
[2707.98 --> 2712.76]  Like if I, they mostly get given to me, which is quite a wonderful position to be in.
[2712.76 --> 2713.70]  So thank you everyone for that.
[2713.76 --> 2716.20]  But if I had to choose one, I don't even like, how do you choose?
[2716.24 --> 2716.94]  There's so many.
[2717.46 --> 2721.24]  I've seen this one mentioned before on the show because it's like, you look at it, it's
[2721.24 --> 2724.98]  looks like it's designed to go in a car or a van.
[2725.20 --> 2732.18]  It's got like, it's, it looks like a ECU almost for a car only, you know, way more expensive.
[2732.18 --> 2737.56]  Uh, and I'm curious to know how often they update this because I have been looking at
[2737.56 --> 2742.38]  this with a curious eye since their Kickstarter about 302 years ago.
[2743.02 --> 2747.98]  And, uh, uh, the question is, is like, is it a one-time run or they keep revving it?
[2747.98 --> 2750.52]  If you know, uh, please boost in.
[2750.78 --> 2752.82]  But VT wanted to continue talking about auth.
[2752.88 --> 2756.08]  He says, I've searched, but I've only find internet arguments instead of solid advice.
[2756.18 --> 2757.40]  I don't know if I'm missing something.
[2757.46 --> 2759.10]  It seems to be like a really fragmented space.
[2759.10 --> 2761.12]  There's a service that supports LDAP.
[2761.20 --> 2762.34]  This one is HTTP basic.
[2762.46 --> 2763.74]  The other one might be OIDC.
[2764.28 --> 2765.80]  It's all kind of just weird to me.
[2766.14 --> 2768.18]  Each is a snowflake requiring special config.
[2768.90 --> 2770.14]  Is this my life now?
[2770.32 --> 2774.18]  I'm usually currently using Kandem OAuth 2 proxy and traffic.
[2774.96 --> 2779.96]  Uh, he says, if we convert the boost amount, we get hex, which comes out as 16D8D if my math
[2779.96 --> 2782.72]  is right, but I, I don't know what it means.
[2783.48 --> 2788.24]  Uh, LDAP ultimately is the mother authentication backend.
[2788.24 --> 2790.34]  All things collapse to LDAP.
[2791.58 --> 2794.18]  Marquis comes in with 60,770 sets.
[2794.26 --> 2794.74]  Thank you.
[2795.64 --> 2796.50]  Using Podverse.
[2797.08 --> 2798.02]  First time booster here.
[2798.08 --> 2799.84]  Your show is everything I've been looking for and I love it.
[2799.88 --> 2802.12]  Here's some sets to you on the topic of small home servers.
[2802.26 --> 2805.32]  I bought myself a Zim aboard and it's amazing.
[2805.86 --> 2813.78]  It has an X64 Intel with two RJ45 PCI and PCIe slots and two SATA three ports all for 120 bucks.
[2814.28 --> 2816.44]  The top version has 16 gigs of RAM if I remember right.
[2816.54 --> 2817.22]  That's all for now.
[2817.22 --> 2818.00]  Thanks for the show.
[2818.22 --> 2818.78]  You're the best.
[2819.06 --> 2820.18]  Are they coordinating out there?
[2820.26 --> 2822.20]  How about some real time follow up there?
[2822.30 --> 2822.76]  Thank you, Marquis.
[2822.88 --> 2823.40]  That's nice.
[2823.50 --> 2824.32]  And thank you for the boost.
[2825.38 --> 2826.30]  Self hosting is life.
[2826.42 --> 2828.40]  Comes in with 50,000 and one sets.
[2829.24 --> 2830.46]  Keeping that boost train rolling.
[2830.56 --> 2833.02]  Hey guys, how about a deeper look at NVR software?
[2833.44 --> 2835.42]  I know you covered it before, but a lot has changed.
[2835.48 --> 2839.40]  I finally got fed up with Blue Iris and I decided to give Frigate a go and I haven't looked
[2839.40 --> 2839.72]  back.
[2839.78 --> 2841.42]  Would love to hear an updated take from the two of you.
[2841.42 --> 2847.62]  Well, Jeff has been working with Frigate and you've gone with the CPU for a while and you
[2847.62 --> 2851.38]  just recently put like one of those corals in there to get accelerated recognition.
[2852.34 --> 2855.02]  Sounds like you're liking it with some caveats.
[2855.02 --> 2861.00]  With some caveats, it seems plenty fast and there's one big caveat to hardware.
[2861.54 --> 2862.42]  It's an Intel Atom.
[2862.50 --> 2866.76]  It's a Baytrail Intel Atom and it's got a whopping four gigs of RAM.
[2866.94 --> 2868.08]  So that's going to be a bottleneck.
[2868.16 --> 2869.98]  It's going to be a big bottleneck.
[2869.98 --> 2873.40]  It did fine actually to recognize people.
[2873.54 --> 2876.88]  The inference time was about 1200 milliseconds if people have used Frigate.
[2877.00 --> 2879.92]  It's really slow, but it seemed real stable.
[2880.06 --> 2881.40]  It seemed to find people every day.
[2881.46 --> 2885.84]  I just had to look the next day to see, you know, people, right?
[2886.56 --> 2887.72]  Which is okay.
[2888.48 --> 2890.10]  Not quite what you're looking for.
[2890.36 --> 2890.44]  Right.
[2890.52 --> 2896.04]  So I did put the TPU in there and the inference time was way faster, about 10 to 12 milliseconds.
[2896.86 --> 2898.50]  And it seemed to work really, really well.
[2898.50 --> 2902.18]  But ever since then, it just hasn't been stable.
[2902.28 --> 2906.76]  I've got to reboot it every other day to make it do the detection again.
[2907.36 --> 2908.86]  And that's my fault.
[2908.96 --> 2909.92]  I guarantee it's my fault.
[2909.98 --> 2911.10]  I'm running the stupid thing on Arch.
[2911.44 --> 2912.16]  That's my fault.
[2912.68 --> 2915.74]  But hey, it's just to play with it.
[2915.78 --> 2917.84]  I am also fed up with the various NVR solutions.
[2918.30 --> 2921.26]  And so far, Frigate is my favorite on Linux.
[2921.38 --> 2926.70]  So I'll re-ramp that onto something better, something more stable and give it another go.
[2926.70 --> 2927.84]  But for now, I'm loving it.
[2927.90 --> 2930.16]  And the TPUs are dirt cheap and they work really well.
[2930.76 --> 2938.76]  We were looking and I do see success stories, too, of folks using Wyze cams with Wyze bridge into Frigate.
[2939.44 --> 2941.14]  So I'm giving it a contemplation.
[2941.14 --> 2947.14]  I have Shinobi that I turn on from time to time, kind of when I'm like AFK, AF RV.
[2947.62 --> 2950.36]  And I think maybe Frigate would be a better solution for that.
[2950.70 --> 2952.14]  So self-hosting is life.
[2952.22 --> 2953.16]  Let us know if you keep playing with it.
[2953.18 --> 2954.94]  And I'm going to keep following Jeff's progress.
[2955.70 --> 2959.26]  Bronzenwing comes in with 50,000 cents using Fountain.
[2960.36 --> 2962.80]  And they're going to switch to Albion Cast-O-Matic.
[2962.98 --> 2963.34]  Nice.
[2963.34 --> 2966.02]  That's a great setup.
[2966.42 --> 2967.80]  They're passing on some sats.
[2967.84 --> 2970.30]  I want to say thanks for turning them onto Tailscale.
[2970.78 --> 2976.06]  I recently set it up with PFSense and HA Proxy with the VPN On Demand feature.
[2976.24 --> 2983.92]  It has, I have it advertise my local subnet and then advertise my local virtual IP for my internal reverse proxy and my local services domain.
[2984.54 --> 2987.52]  Now when I leave the house, it's like I never left.
[2987.52 --> 2993.12]  I can access my local services with their fully qualified domain names, but they aren't exposed to the internet.
[2993.34 --> 2993.82]  It's magic.
[2994.22 --> 2995.36]  It's just pure magic.
[2995.70 --> 2996.94]  Well done.
[2997.28 --> 2998.14]  Well done.
[2999.24 --> 3011.40]  So they have PFSense with HA Proxy and the VPN On Demand feature, and they have it advertise their local subnet and then advertise their local virtual IP to their internal reverse proxy and their local services domain.
[3011.74 --> 3014.84]  That's a slick setup.
[3015.28 --> 3016.36]  That is a slick setup.
[3016.46 --> 3016.94]  Very impressed.
[3016.94 --> 3017.98]  Thank you for the boost.
[3018.90 --> 3019.66]  Darylman comes in.
[3019.92 --> 3022.40]  Darylman comes in with 10,000 satsues in Podverse.
[3022.40 --> 3023.98]  Okay, so Plex.
[3024.12 --> 3031.46]  I'm responsible for the infra of about a million plus user app, and I'm also a self-hoster.
[3032.16 --> 3035.00]  They write, it doesn't matter if it's a professional or a hobby.
[3035.12 --> 3039.62]  My main takeaway after 20 years in the area, just stick to plain open source.
[3040.46 --> 3043.48]  I keep my fingers off the closed source or pursuit of open source software.
[3043.96 --> 3046.42]  Mid to long term, it always hurts to use it.
[3047.14 --> 3048.86]  Long live Jellyfin and all the others.
[3048.86 --> 3052.20]  I redid the math on that number there, Chris.
[3052.54 --> 3053.18]  Oh, on my hex?
[3054.74 --> 3058.14]  No, on this one with many, many zeros here.
[3058.30 --> 3058.54]  Oh, yeah.
[3058.64 --> 3060.96]  I think that's actually 100 million users.
[3061.54 --> 3062.76]  Oh, that's a lot of zeros.
[3063.16 --> 3063.82]  That's a lot of zeros.
[3063.92 --> 3064.58]  Well, it says plus.
[3064.78 --> 3066.00]  What app could that be?
[3066.24 --> 3066.90]  What app?
[3067.08 --> 3068.74]  It reduces the list somewhat.
[3068.84 --> 3069.00]  Yeah.
[3069.00 --> 3069.44]  Yeah.
[3071.68 --> 3073.38]  Well, that's some great feedback.
[3073.68 --> 3076.64]  And it echoes, I think, our sentiments as well.
[3076.86 --> 3078.88]  It's definitely true.
[3079.18 --> 3084.90]  And it kind of, my philosophy for why I'm using the ESP hardware with relays I, you know,
[3084.94 --> 3086.42]  you can get off Amazon and ESP Home.
[3086.54 --> 3090.64]  It's sort of, it's just, maybe it's not quite as polished as the commercial solution.
[3090.70 --> 3092.30]  It requires a little bit more of Jeff's work.
[3092.30 --> 3097.42]  But, you know, it's going to last forever and it's super replaceable.
[3097.92 --> 3100.68]  Well, and I feel like, you know, you buried this thing in your wall.
[3101.24 --> 3105.60]  Hopefully, you're allowed to forget about it in the sense that it's there for many, many
[3105.60 --> 3105.84]  years.
[3105.96 --> 3106.60]  It just keeps working.
[3106.84 --> 3107.22]  Works like hardware.
[3107.40 --> 3110.44]  Let's say seven years from now, it just kind of gives out.
[3110.60 --> 3116.18]  Well, I think there would be enough resources out there for you to even solve the problem.
[3116.22 --> 3119.56]  Even if, you know, ESPs are probably long gone by then.
[3119.68 --> 3120.92]  But relays are relays.
[3120.92 --> 3122.24]  Uh-huh, exactly, right?
[3122.44 --> 3124.00]  And you just need to trigger that relay.
[3124.64 --> 3125.22]  Yeah, yeah.
[3125.78 --> 3127.58]  Gene Bean comes in with a row of ducks.
[3127.74 --> 3132.88]  Brent, answering your question from last week, I'm using the NextCloud Snap today, but I want
[3132.88 --> 3133.62]  to get away from it.
[3134.00 --> 3138.72]  I'm considering trying the NextCloud Pi after talking to a community member about it, but
[3138.72 --> 3143.00]  I'm still undecided and I'm interested in what others have to say.
[3144.46 --> 3147.82]  That's a tough question because, and I want to loop it in with Andre 2K.
[3147.90 --> 3148.46]  I think they're related.
[3148.46 --> 3150.88]  He sent in 6,666 sets.
[3151.02 --> 3151.72]  Thank you, Gene.
[3151.84 --> 3155.04]  And here, Andre's kind of along your same kind of line of thinking.
[3155.10 --> 3158.48]  He says, I'm using NextCloud from Linux Server IO.
[3158.74 --> 3163.40]  I had to migrate from MariahDB to Postgres because of newer versions not working out about
[3163.40 --> 3164.00]  a year ago.
[3164.46 --> 3169.36]  I've been thinking about switching to the all-in-one Docker to get hardware support for
[3169.36 --> 3169.94]  Recognize.
[3170.32 --> 3174.64]  But I didn't like the setup of the container since it was so different from other containers.
[3174.64 --> 3180.48]  And so this is a question, I think, a lot of people that are dipping their toe into NextCloud,
[3180.62 --> 3185.12]  maybe taking their NextCloud setup from the I want to test it to the actually want to use
[3185.12 --> 3185.62]  it stage.
[3186.32 --> 3188.48]  Jeff's been fighting with his NextCloud setup.
[3188.74 --> 3191.58]  He's got kind of like a basic container setup, right?
[3191.66 --> 3193.92]  I think you're using, are you using the Linux Server IO image?
[3194.36 --> 3195.60]  No, I don't believe so.
[3195.98 --> 3197.88]  But you are on the old MariaDB.
[3198.14 --> 3198.48]  Yes.
[3198.48 --> 3205.04]  And the question you've been having recently, is it worth tearing down that DB, moving to
[3205.04 --> 3207.50]  the new stuff and going with just a straight up container?
[3207.90 --> 3209.74]  Or is it worth doing the all-in-one?
[3210.26 --> 3210.54]  Right.
[3210.62 --> 3212.20]  And having it kind of manage all that stuff?
[3212.68 --> 3212.92]  Right.
[3213.04 --> 3213.16]  Yeah.
[3213.22 --> 3218.46]  Getting help setting it up, you know, the way it is now with the reverse proxy.
[3219.98 --> 3220.96]  It's above my head.
[3221.16 --> 3224.08]  You know, I don't fully understand it and I need to fully understand this.
[3224.24 --> 3227.06]  And if I don't fully understand it, it needs to manage itself.
[3227.06 --> 3231.38]  So the all-in-one kind of seems like a good deal, but not too sure.
[3231.66 --> 3232.40]  I'm in the same boat.
[3232.70 --> 3238.34]  I think it kind of depends on how solid their implementation is of all of it.
[3238.42 --> 3244.72]  Like I was saying before, off-air, I kind of look at it from a repairability standpoint.
[3245.18 --> 3249.42]  And the simpler the setup is, the easier it is to repair once you do understand it.
[3249.80 --> 3253.58]  And it's kind of like a new car that's totally sealed up that you can't really repair and
[3253.58 --> 3256.98]  do work on versus an older car that the engine bay has tons of room.
[3257.06 --> 3258.04]  And you know what everything does.
[3258.10 --> 3261.70]  And you can actually trace one thing to another thing and go, oh, that's probably this and
[3261.70 --> 3262.10]  fix it.
[3262.54 --> 3268.12]  If you just go simple and stand up a database container and a Nextcloud container and then
[3268.12 --> 3272.46]  put Nginx in front of that to do reverse proxy, you could use traffic if you want, but just
[3272.46 --> 3273.90]  keep it really simple.
[3274.76 --> 3279.22]  You will be able to open the configs in all three of those cases and understand what they're
[3279.22 --> 3279.52]  doing.
[3279.60 --> 3281.94]  But you'll never understand what the all-in-one setup is doing.
[3282.62 --> 3283.72]  So I think there's that consideration.
[3283.72 --> 3286.88]  Now, if it doesn't break and it doesn't really have any other downsides, maybe that's
[3286.88 --> 3287.46]  fine, right?
[3287.98 --> 3292.42]  I mean, Volvo tells me that my four-wheel drive system, it never needs maintenance.
[3292.74 --> 3294.50]  But then, of course, I got 100,000 miles into it.
[3294.52 --> 3295.50]  And it turns out, oh, we were wrong.
[3295.54 --> 3297.18]  It actually does have a fundamental problem.
[3297.18 --> 3298.02]  And you have to fix that.
[3298.06 --> 3299.64]  And to fix that, you have to take the whole thing apart.
[3300.18 --> 3301.90]  But of course, it was never designed to be taken apart.
[3302.92 --> 3305.40]  And so now I just have something that's kind of a time bomb, possibly.
[3305.54 --> 3306.54]  And I don't like that.
[3306.60 --> 3311.26]  It's sort of the same implication you have with those other whole home server out-of-a-box systems.
[3311.26 --> 3314.76]  I think the real approach is simplicity.
[3315.00 --> 3320.42]  Now, Eric sent in a row of ducks to let us know that he has been very happy using Nix
[3320.42 --> 3322.26]  to set up NixCloud and Postgres.
[3322.40 --> 3323.86]  And he also has a flake that does it.
[3324.38 --> 3329.78]  And the nice thing there is that's a whole other level of one place to read it and you
[3329.78 --> 3330.74]  understand what it does.
[3331.06 --> 3334.96]  After the show, I'll show you my NixCloud Nginx config in Nix.
[3335.06 --> 3337.10]  And you'll read that and go, oh, yeah, I know exactly what that's doing.
[3337.10 --> 3340.78]  And that kind of, to me, is like how you make it approachable to repair.
[3341.20 --> 3345.98]  So I don't know if I like the pie image and I don't know if I like the all-in-one as much,
[3346.06 --> 3347.20]  but I'm open to the ideas.
[3347.98 --> 3352.90]  But traditionally, my experience has always been when I use one of these types of all-in-one
[3352.90 --> 3357.16]  solutions, I inevitably, if I want to put it in production seriously, end up tearing
[3357.16 --> 3359.80]  all that down and just going building the essential system.
[3359.80 --> 3367.38]  I feel like, though, some of these projects are trying to aim at different types of users.
[3367.76 --> 3367.90]  Yeah.
[3367.96 --> 3371.76]  Because that advice is super sound for someone who at least wants to get their feet wet in
[3371.76 --> 3375.66]  those technologies, which I think is likely most of us here listening to this.
[3376.42 --> 3381.20]  But just reading the pie documentation, for instance, it's clear that they're trying to
[3381.20 --> 3386.00]  build something that is kind of literally all-in-one.
[3386.20 --> 3387.82]  Like it has backups in there and has everything.
[3387.82 --> 3391.42]  And I know the all-in-one container is attempting to do that, but I think it also reaches for
[3391.42 --> 3392.10]  a different audience.
[3392.36 --> 3398.16]  And so it might be similar to me in the sense that five years ago, I installed the Snap
[3398.16 --> 3401.24]  because it was as much as I could bear back then.
[3401.32 --> 3403.36]  But as you grow, you move into new solutions.
[3403.68 --> 3404.64]  So it's a tricky problem.
[3405.58 --> 3405.68]  Yeah.
[3405.74 --> 3409.14]  And I think Jeff and probably a lot of the listeners that boosted in are kind of in this
[3409.14 --> 3412.40]  spot where you're kind of deciding, do I want to go all-in and learn it this way?
[3412.44 --> 3414.02]  Do I want to go all-in and learn it this way?
[3414.34 --> 3417.14]  And so you're really kind of, you're almost looking at, do you want an iPhone?
[3417.14 --> 3417.96]  Do you want an Android?
[3418.10 --> 3418.82]  Do you want a Mercedes?
[3419.08 --> 3420.26]  Do you want an old Toyota?
[3420.44 --> 3423.28]  Like you're kind of making a similar type of decision.
[3423.46 --> 3428.28]  And ultimately, I think like maybe you're actually an old Toyota guy because you like,
[3428.36 --> 3430.24]  you know, these old 80s Toyotas are super repairable.
[3431.02 --> 3432.98]  But, you know, the new ones are really sweet.
[3433.04 --> 3435.24]  And they got that auto driving feature and they're half hybrid.
[3435.40 --> 3437.72]  And that's really, and that kind of draws you in.
[3437.92 --> 3441.06]  And you get into it a couple of years and you're like, oh crap, I can't do anything with this.
[3441.06 --> 3442.00]  I don't know.
[3442.04 --> 3442.74]  It could be a bad analogy.
[3442.86 --> 3447.88]  But I think that's kind of where I think Gene Bean and Andre are kind of sliding.
[3448.00 --> 3449.52]  I don't know about Jeff, but perhaps too.
[3450.54 --> 3454.26]  MegaStrike came in with 5,011 sats and one, I think this is our last next slide?
[3455.04 --> 3455.30]  Maybe.
[3455.30 --> 3459.28]  But was asking about using it on a VPS to host.
[3459.36 --> 3463.42]  And if we don't use it on a VPS, do we use it on systems that have ECC memory?
[3464.04 --> 3467.10]  They want to get it on their LAN, but they want to do it right the first time.
[3467.74 --> 3469.20]  Now, take note of this one, Jeff.
[3469.26 --> 3472.86]  They said in the past, they did run the NextCloud all-in-one setup.
[3473.66 --> 3476.72]  But they say it was slow to release.
[3477.76 --> 3482.62]  And they had one breaking update, but it was pretty bad.
[3482.62 --> 3487.50]  And well, every update breaks for me, so still one to consider.
[3487.80 --> 3488.92]  MegaStrike, thank you for the boost.
[3489.00 --> 3493.82]  No, I don't follow very carefully all the ECC stuff.
[3493.86 --> 3494.80]  I just load it on the system.
[3494.88 --> 3496.08]  I don't really think about the RAM.
[3496.30 --> 3498.56]  I mean, I do prefer it on server-grade hardware in general.
[3499.02 --> 3502.04]  And I would totally take ECC if I could, but it's not a hard requirement.
[3502.42 --> 3502.98]  Not at all.
[3503.14 --> 3506.80]  Not even like a little bit, but not a bad thing to think of if you can afford it.
[3506.80 --> 3512.00]  It feels to me like part of the success for pieces of software like NextCloud and Home Assistant
[3512.00 --> 3516.50]  really is their flexibility, if you will.
[3516.68 --> 3517.58]  Flexibility in hardware.
[3517.80 --> 3522.52]  You can run it in so many different places and so much different type of hardware
[3522.52 --> 3526.36]  from little tiny single boards to some really bigger stuff.
[3526.36 --> 3534.32]  It feels to me like there's a trade-off there because you get a bunch of users who would
[3534.32 --> 3536.54]  otherwise never get their feet wet in these technologies.
[3536.86 --> 3542.18]  But as people grow, especially into careers or whatever, and they use more sophisticated
[3542.18 --> 3545.94]  technologies, then the software can grow with them, which is actually kind of cool.
[3546.08 --> 3550.14]  It is good, but it leads to kind of confusion as to which path that should be taken.
[3550.24 --> 3550.68]  It's true.
[3550.68 --> 3557.02]  Yeah, and I wonder if those projects can have more clarity to guide users in that specific
[3557.02 --> 3557.20]  way.
[3557.26 --> 3562.66]  Because if I was new to NextCloud, this is really what I'm trying to solve is like,
[3562.74 --> 3564.48]  where do you go?
[3564.60 --> 3569.60]  The first red flag was probably years ago when the Linux server IO version of NextCloud
[3569.60 --> 3571.04]  container started getting popular.
[3571.14 --> 3573.32]  It was clear they were addressing a market need there.
[3574.38 --> 3575.64]  All right, here's our last boost, boys.
[3575.68 --> 3576.24]  We're going to wrap it up.
[3576.24 --> 3581.16]  But I think this one would be probably someone in the audience would be capable of answering.
[3581.30 --> 3582.36]  We'll see if we have any ideas, though.
[3583.08 --> 3588.42]  B2 Thread comes in at 10,000 sats using Fountain, and they write, I was trying to save my sats
[3588.42 --> 3591.76]  to do a zip code boost, but I'm beating my head against the wall for a problem.
[3591.98 --> 3592.68]  I need some help.
[3592.98 --> 3596.34]  I'm trying to set up an HP Thin client with 16 gigs of Flash on board.
[3597.06 --> 3598.82]  Mint XFCE is just too big.
[3598.82 --> 3602.72]  I'd like to throw something else on there and then just remote desktop connect into my Fedora
[3602.72 --> 3605.80]  desktop, which has a Ryzen and plenty of free resources.
[3606.24 --> 3608.44]  But I just can't seem to get them to talk.
[3609.14 --> 3611.44]  What should I put on the Thin client to easily talk to Fedora?
[3611.60 --> 3614.38]  And what should I put on the box that could easily access it?
[3614.72 --> 3617.36]  Should I just hop distros and maybe go to Ubuntu on both?
[3618.44 --> 3619.82]  I don't know if I have a great answer.
[3621.38 --> 3628.50]  But I think you could probably easily find a Linux that is smaller than Linux Mint XFCE
[3628.50 --> 3634.36]  if you're just trying to get a Linux environment on that little Thin client.
[3634.44 --> 3636.28]  Maybe even a minimal install of Fedora.
[3636.70 --> 3637.80]  Something just came to mind.
[3637.90 --> 3641.18]  There are distros specifically for RDP.
[3641.54 --> 3642.16]  Extremely small.
[3642.26 --> 3643.18]  They're built for Thin clients.
[3643.78 --> 3644.38]  Try one of those.
[3644.54 --> 3644.68]  Yeah.
[3644.68 --> 3649.64]  One thing that we were thinking about during our prep for the show that Jeff brought up
[3649.64 --> 3658.00]  is the one maybe advantage to doing the same distro on both ends would be that the server
[3658.00 --> 3663.30]  of the RDP server and the RDP client are probably going to pretty well match up in capabilities
[3663.30 --> 3663.88]  and features.
[3664.38 --> 3666.10]  Make sure you can actually connect B2.
[3666.40 --> 3670.48]  Make sure the internal GNOME RDP server is working.
[3670.48 --> 3674.52]  Because if you're on an older version of GNOME by a couple of releases, you could just be
[3674.52 --> 3676.40]  running into some fundamental functionality problems.
[3676.60 --> 3681.80]  So get it running and then just launch Romania or even the Microsoft RDP client.
[3681.88 --> 3686.38]  But if you're on the local host, run Romania, something like that, and just do a local host
[3686.38 --> 3687.68]  connection in and see if that works.
[3687.82 --> 3689.20]  Verify your RDP is working.
[3689.98 --> 3695.98]  And then the idea with RDP is that it's the protocol and the clients are the display end.
[3696.06 --> 3697.34]  So you just got to find the appropriate client.
[3697.42 --> 3698.64]  I think Romania is a pretty good one.
[3698.64 --> 3701.36]  And it doesn't actually have to be the same OS.
[3701.48 --> 3702.74]  It doesn't have to be even the same versions.
[3702.98 --> 3705.40]  But the closer you get, the less problems you'll have there.
[3705.94 --> 3709.40]  If anybody out there in the audience has some good experience with thin clients, especially,
[3709.62 --> 3713.34]  you know, I'm talking actual thin clients and getting OSs on there and getting connected,
[3713.88 --> 3714.50]  let us know.
[3714.68 --> 3718.32]  This is a topic of mine that is one of my OG passions.
[3718.98 --> 3723.38]  One of the first big projects I had at scale was deploying Linux terminal services in libraries.
[3723.38 --> 3726.70]  And then later on, I ended up working on Microsoft terminal services.
[3726.70 --> 3730.38]  So I really love thin clients and I love the remote desktop stuff.
[3730.48 --> 3733.44]  So if anybody out there has some geekery to share, please boost in.
[3733.56 --> 3736.82]  If you'd like to boost in, you can get a new podcast app at podcastapps.com.
[3737.34 --> 3739.06]  And then you top it off and you just boost in.
[3739.10 --> 3739.94]  They got a button right there.
[3740.26 --> 3743.04]  Or if you want to keep your dang podcast app, I know you.
[3743.22 --> 3744.06]  I know you like your app.
[3744.68 --> 3745.44]  Just get Albie.
[3745.56 --> 3746.32]  Get albie.com.
[3746.40 --> 3747.46]  And then you can boost from the web.
[3747.52 --> 3749.38]  It's something like podcast index or fountain FM.
[3749.50 --> 3750.46]  We'll have links in the notes.
[3750.46 --> 3751.90]  It's all on the Lightning Network.
[3752.14 --> 3755.04]  So you just top it off however you like and you boost in.
[3755.36 --> 3757.04]  Now, we did get 22 total boosters.
[3757.18 --> 3758.84]  We couldn't fit everybody in because of the runtime,
[3759.04 --> 3761.68]  but we sure do appreciate and read all of them.
[3762.10 --> 3766.42]  And we stacked a grand total of 367,659 stats.
[3766.56 --> 3768.72]  Thank you, everybody who supports this production directly.
[3769.52 --> 3772.14]  And, of course, thank you to our SRE subscribers.
[3772.30 --> 3773.90]  You are our site reliability engineers.
[3774.34 --> 3777.52]  You can support the show directly with a monthly membership.
[3777.52 --> 3780.56]  You get an ad-free version of the show and you get a post show.
[3781.20 --> 3785.26]  And, of course, the warm fuzzies of keeping us going at selfhosted.show.sre.
[3786.12 --> 3789.16]  Now, this, for us, is pre-LinuxFest.
[3789.50 --> 3792.92]  For most people listening, though, LinuxFest will have happened by the time of listening to this.
[3792.94 --> 3794.26]  And all things open will have happened.
[3794.76 --> 3798.32]  So I imagine when we get together again, perhaps we'll have some stories to share.
[3798.48 --> 3799.82]  We'll get caught up with Alex.
[3800.42 --> 3802.44]  But I want to thank Paulus for coming on the show.
[3802.60 --> 3804.00]  It was really great to chat.
[3804.00 --> 3808.98]  But I've been so, so thrilled with the progress of the Year of Voice.
[3809.20 --> 3810.86]  I have it set up everywhere here at the studio.
[3811.38 --> 3812.70]  And I have multiple pipelines.
[3812.92 --> 3815.70]  See, one of the cool things you can do is you can have multiple assistants.
[3816.48 --> 3818.30]  And so I have local pipeline.
[3818.70 --> 3820.94]  I have, like, a slow one that I'm trying on the Raspberry Pis.
[3821.12 --> 3824.02]  And then I have the Nebukasa Cloud, Home Assistant Cloud pipeline.
[3824.02 --> 3831.08]  And not only that, but on Android, you can replace the Google Assistant with Home Assistant.
[3831.66 --> 3835.64]  And so you can trigger the Assistant and it pulls up just Home Assistant.
[3836.00 --> 3836.04]  What?
[3836.48 --> 3841.54]  And then from there, even, once the UI is up, you can even switch between your different Home Assistant servers.
[3841.62 --> 3844.60]  So I can switch between the studio and the RV for different voice commands.
[3845.14 --> 3846.78]  That is so cool.
[3846.90 --> 3848.04]  And really thoughtful.
[3848.36 --> 3849.32]  Like a thoughtful integration.
[3849.70 --> 3851.34]  It's been fun playing with the back-end tech, too.
[3851.44 --> 3853.02]  Just as much fun playing with the back-end stuff.
[3854.02 --> 3855.44]  It's just been pretty great to see.
[3855.54 --> 3860.08]  I can only imagine where it's going to be in another year because some of those people are working there full-time now on this stuff.
[3861.10 --> 3861.56]  All right.
[3861.60 --> 3862.42]  That's it for us.
[3862.66 --> 3864.32]  Thank you so much for tuning in this week's episode.
[3864.50 --> 3868.48]  You can get the links to everything we talked about today at selfhosted.show slash 108.
[3869.14 --> 3871.84]  And, of course, you can email us at selfhosted.show slash contact.
[3871.98 --> 3877.76]  You'll find the links to contact Alex and I and Brent and Jeff and all that stuff there as well.
[3878.40 --> 3879.04]  Thanks for listening.
[3879.20 --> 3880.92]  That was Self Hosted 108.
[3883.02 --> 3913.00]  Thank you.
