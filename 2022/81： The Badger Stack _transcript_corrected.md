[0.00 → 6.30] Is there some sort of universal law that states that your infrastructure is going to fail whenever you're not around?
[6.46 → 8.54] Because I seem to always be subject to it.
[9.04 → 18.94] There I was, down at NASA's Jet Propulsion Laboratory, actually the night before, dreaming about what we might discover, thinking about what we might learn.
[19.38 → 25.56] I decide to check in on my intrepid RV, about seven hours north of where I was.
[25.88 → 29.34] I pull up the Home Assistant app, and it just isn't quite loading.
[29.34 → 31.62] And I think, hmm, that's strange.
[32.42 → 37.16] So I fire up Tail Scale, and I pull up the web interface, because the web interface always works when the app doesn't work.
[37.74 → 39.16] And it still doesn't load.
[39.22 → 43.02] And I think, huh, I wonder if something's wrong with Home Assistant.
[44.48 → 53.42] And a few days go by, and I finally make it back to the RV, and I discover that my Raspberry Pi home server that runs more than just Home Assistant.
[53.42 → 64.52] I mean, it runs my Plex instance, my Sync Thing instance, my Duplicate instance, my Smoke Ping instance, my Markdown Notes instance, and Home Assistant.
[66.18 → 66.54] Dead.
[67.26 → 67.90] Just dead.
[68.10 → 69.00] Dead as a doornail.
[69.14 → 70.62] Just totally dead.
[70.82 → 71.40] Uh-oh.
[71.40 → 73.18] And you know the worst part?
[74.06 → 75.22] I don't even know why it's dead.
[75.42 → 76.82] What do you mean you don't know why it's dead?
[77.04 → 77.98] I don't even know what happened.
[78.54 → 82.82] I mean, we've been on the road, and I've been trying to figure it out, but I just haven't had a chance.
[82.88 → 84.56] I haven't even hooked up an HDMI screen to it.
[84.58 → 85.34] Oh, I see.
[85.40 → 86.92] I did the hardware swap thing, you know.
[87.16 → 87.46] Yeah.
[87.54 → 89.12] So what was your plan with that hardware swap?
[89.18 → 91.12] Because it seemed like a brilliant plan at the time.
[91.26 → 91.72] Well, thank you.
[91.72 → 99.20] I mean, I bought a duplicate Raspberry Pi, same thing, Raspberry Pi 4, 8 gigs, in the same case, forever ago.
[99.48 → 100.64] Just ready to go.
[101.38 → 105.62] I swapped everything over, hit the power button, and nothing.
[106.14 → 111.78] And I looked at my dead Raspberry Pi, and I realized, oh, there's an SD card in here.
[111.82 → 112.90] Oh, Chris.
[113.30 → 116.26] I think it might—this is like the first one I ever set up.
[116.32 → 119.38] I think maybe it was using that SD card for like slash boot.
[119.38 → 126.48] I can't remember anymore, but when I first did this, there was kind of a workaround to get Ubuntu running on the Raspberry Pi 4.
[126.58 → 128.02] It was before official support had landed.
[128.44 → 132.72] And I think maybe the SD card was used for grub or something like that.
[133.24 → 135.70] But I don't know why it would have died while it was running.
[136.58 → 139.74] So I'm wondering if something more significant happened, but I just don't know at this point.
[140.34 → 141.74] Maybe there was an unattended upgrade.
[142.60 → 143.00] Maybe.
[143.36 → 144.48] Maybe a live patch.
[144.84 → 147.78] You know, I did the whole reboot thing, and of course I'm trying to SSH intuit.
[147.78 → 148.80] I can't ping it.
[148.80 → 151.62] I can't ping it on the tail scale IP either.
[152.06 → 153.06] It seems gone.
[153.26 → 158.42] And the worst part of that is it runs a lot of automations in the RV.
[158.68 → 167.34] Like all the lighting, the heating, of course the cooling, a lot of the outdoor stuff, it's all managed by Home Assistant on this stupid Raspberry Pi.
[168.08 → 171.28] And so it's like we're running things like animals with switches.
[172.32 → 175.72] Yeah, this place went from a five star to about a three and a half, I think.
[175.72 → 176.16] Wow.
[180.74 → 182.92] You let this guy into your home, Alex, you know.
[184.12 → 184.48] Indeed.
[184.70 → 188.16] Well, this seems like an appropriate moment to introduce Brent again.
[188.28 → 188.76] Hello, Brent.
[188.84 → 189.28] How are you?
[189.42 → 189.94] Welcome back.
[190.32 → 191.04] Thank you very much.
[191.18 → 192.28] And what about you, gentlemen?
[192.86 → 197.76] Well, actually, we had some feedback at the meetup in Pasadena that we don't introduce ourselves anymore.
[197.76 → 204.06] So let's just take a moment for anybody that hasn't worked out that I'm Alex and the other guy is Chris.
[204.22 → 204.96] Hey, Chris.
[205.62 → 206.68] Hello, everybody.
[206.88 → 207.80] Thank you for being here.
[207.88 → 208.46] Okay, good.
[208.52 → 209.28] Now that's out of the way.
[209.28 → 210.88] Welcome to episode 81.
[211.08 → 212.28] Now that's out of the way.
[212.28 → 221.34] I want to ask you if this has got you thinking about deploying some real hardware in a production system.
[222.00 → 222.56] Ooh.
[222.94 → 223.98] Throwing shade.
[225.48 → 226.42] Fair enough.
[227.30 → 231.56] You know, listener Jeff was really the MVP of our West Coast road trip.
[231.56 → 239.76] And he sent me home with an Atom-based unit that only draws five watts, and it's got two cores, but four gigs of RAM.
[240.00 → 243.90] I'm tempted to just build a dedicated home assistant system out of that.
[244.30 → 244.56] Why not?
[244.84 → 248.46] Well, I just got shipment notification about my home assistant yellow.
[248.70 → 250.66] I should be receiving it the Friday of this week.
[250.78 → 251.26] I did.
[251.36 → 252.10] No, you didn't.
[252.10 → 252.86] I have the UPS.
[253.36 → 256.22] I've got a UPS tracking number and everything.
[256.84 → 257.86] Where's it coming from?
[258.04 → 258.50] Guam.
[258.50 → 259.06] Guam.
[260.68 → 266.36] I think they landed in Texas and then some distribution place in Texas is sending them out from there.
[266.68 → 266.72] Right.
[266.98 → 267.24] Okay.
[267.34 → 274.56] It's so exciting because this marks the second crowd supply thing that I've ever backed that I'm actually going to receive.
[275.04 → 275.92] Very excited.
[276.50 → 279.80] And so the home assistant yellow is supposed to arrive this Friday.
[280.52 → 282.70] The only thing was I kind of wanted to go with something more powerful.
[283.14 → 283.36] Yeah.
[283.36 → 290.06] Well, I'll tell you what's got me thinking is you often run into these issues when you're on the road remotely and that kind of thing.
[290.28 → 290.42] Yeah.
[290.56 → 291.48] Almost exclusively.
[291.70 → 293.22] Oh, it's so annoying.
[293.60 → 297.12] I think you need to embrace PMI of some description.
[297.48 → 299.26] I think that needs to be a requirement for you.
[299.70 → 300.36] Oh, interesting.
[301.00 → 305.10] Oh, you know, I thought about that for the studio and I agree, but I had not thought about it for the RV.
[305.10 → 312.10] Well, of course, there's the Pi KVM project for x86 boards that don't come with a BMC chip built in.
[313.00 → 318.08] But, you know, you could probably build a server that does everything.
[318.24 → 320.78] How many Pis do you have deployed in dupes right now?
[321.48 → 322.56] Well, come on.
[322.60 → 323.22] I pared it down.
[323.28 → 324.34] I pared it down to only two.
[324.68 → 328.56] I'm not saying this to be a phallic object.
[328.82 → 331.00] I'm just saying this out of love.
[331.16 → 332.46] Like, genuine question.
[332.46 → 333.56] It was four.
[333.70 → 334.70] It was four in production.
[334.90 → 336.48] And over time, I pared it down to two.
[336.86 → 337.12] Okay.
[337.26 → 345.24] So if we allow a 10 watt budget per Pi, give or take, right, that's now it was 40 watts.
[345.32 → 346.24] It's now 20 watts.
[346.70 → 355.24] You could build a very capable x86 system that does everything all of those Pis do and has a BMC built into it.
[355.74 → 361.74] You know, given that power is it's not you're not quite as limited on power as the Mars rover is, but you're not far off.
[361.74 → 362.70] It's true.
[363.34 → 366.20] Every watt does count, especially watts that run continuously.
[366.76 → 368.26] What about heat consideration?
[368.90 → 369.82] That is a thing.
[370.16 → 371.18] That's a big thing.
[371.24 → 372.96] I've been really trying to do the math on that, too.
[372.98 → 378.82] When I build the next one, I'm trying to think, do I want to build it in a booth or do I want to go somewhere else and just drill holes?
[379.36 → 382.40] The Raspberry Pi, and maybe that's what finally killed it, was heat.
[382.50 → 382.94] I don't know.
[382.94 → 388.76] But the Raspberry Pi has done a remarkable job of holding up to intense temperatures over long periods of time.
[389.64 → 394.46] My bet really is what happened is there was some kind of power brownout that was enough to make the Pi reboot.
[394.80 → 398.70] And the SD card was toast in that time since it last rebooted.
[399.50 → 403.20] I don't obviously have any data to back that up, but that's what I suspect probably happened.
[403.20 → 409.60] So in total, I spent $169 on the Home Assistant Yellow.
[409.86 → 412.62] And I was watching their live stream today as we record.
[413.18 → 419.22] And I don't think they're going to make many more of these because they can't get their hands on the compute module.
[419.22 → 423.08] So they finally got this thing shipping.
[423.38 → 425.80] In fact, they don't even have the POE one sorted out yet.
[426.00 → 427.90] They have the nonuple one shipping.
[429.10 → 433.66] And they may not make many more just because you can't get them.
[434.14 → 434.82] That's a real shame.
[435.14 → 438.40] I mean, but on the flip side, it's not a good look for the project, is it?
[439.12 → 442.68] Charge people money for something and then not ship it for a year or two.
[443.70 → 446.22] I know it's not their fault, but...
[446.22 → 450.06] Yeah, I ordered it mid-September, and now we're here in early October.
[450.20 → 452.06] So it's just over a year ago that I ordered it.
[452.24 → 453.24] That's a long time.
[454.80 → 455.82] That's a very long time.
[456.20 → 458.30] I mean, if you look at what Valve did with the Steam Deck,
[458.30 → 465.98] I know that Valve, orders of magnitude, got more buying power than Home Assistant, Zebu Casa as a company.
[466.22 → 470.46] But I paid Valve $5 to sit in a queue, essentially.
[470.46 → 476.54] And then when the time came to actually ship my hardware, that's when my credit card got charged.
[477.44 → 479.64] Maybe something like that could work for Home Assistant.
[480.24 → 484.52] Yeah, I think, too, the tricky thing here is they based it on the Pi compute module.
[484.80 → 488.10] And that became one of the hardest things to get your hands on in bulk right now.
[488.52 → 492.38] The Raspberry Pi stuff is, like, still impossible to find.
[492.64 → 492.78] Yeah.
[492.78 → 498.64] I was just doing a check recently, and the most common thing you can find at the moment is the Pi 3.
[499.28 → 501.88] Which, from what I'm learning, isn't that useful for anything.
[502.36 → 509.50] Did you see that Jeff Deerling did a video just last few days when he talked with the founder of the Raspberry Pi project
[509.50 → 514.32] about availability and things like that, and how there's no end in sight?
[514.42 → 522.38] They're making 400,000 of these things a month, and something like 95% is going into industrial use cases.
[522.78 → 523.26] Wow.
[524.38 → 525.66] 95%?
[525.88 → 529.02] Is it even really meant for industrial use cases?
[529.68 → 533.02] You know, I noticed, you know, because Jeff also does an accompanying blog post,
[533.14 → 541.72] and I noticed that one of the comments on Jeff's blog post was sort of giving a different version of this story.
[541.72 → 546.82] They claim, I don't know how they would know, but they claim having inside knowledge,
[547.24 → 553.56] and that Broadcom is actually a bit pissed at the Raspberry Pi folks because they're going commercial.
[554.52 → 561.00] And essentially, like, the whole deal for getting a super cheap chip from Broadcom was that you were creating this educational device for kids.
[561.58 → 565.54] And now you've announced your intentions to IPO and make a commercial company out of all this,
[565.56 → 568.66] and now you need to pay the commercial rates, and you're going to be lumped in with our commercial clients,
[568.72 → 569.78] not our educational clients.
[570.20 → 574.08] And so they're also getting slower supply from Broadcom, according to this commenter.
[574.12 → 576.66] But I have to say, it kind of seems like it checks out.
[576.66 → 584.12] I think the Raspberry Pi Foundation, much like all of us, are kind of being caught off guard by just how ubiquitous it's become.
[584.12 → 592.98] And I think it's a perfect example of how, if you influence the right people, the nerds, the engineers, the people tinkering,
[593.94 → 598.34] if you influence them, they will then go into work and say, hey, well, why don't we just use a Pi?
[598.34 → 607.26] Like, if I, you know, I remember my last job we had on the wall, we had TV screens showing build statuses of all the different CI processes,
[607.58 → 613.60] and each one of them had a Raspberry Pi running, because one of the development team in that sprint team was like,
[613.68 → 615.56] well, we need to monitor the status.
[615.70 → 621.32] Why don't we just get a Pi, because it's only £35, stick it behind the TV, and jobs are good.
[621.66 → 627.00] And I think not only has the Pi Foundation been caught out by the success of their product,
[627.00 → 629.30] but so it sounds like has Broadcom.
[629.92 → 631.46] Perhaps. That would make a lot of sense.
[632.38 → 636.58] It's tricky, because I actually think if they don't figure something out,
[637.20 → 642.84] the M1 platform is going to make a pretty worthy successor for home libbers.
[643.16 → 649.10] If, imagine for a moment, if you would, Alex, there was decent Linux support for the M1,
[649.20 → 654.76] which we may be only nine months, ten months away from, and that includes Thunderbolt support.
[654.76 → 658.00] Because right now, I'm hanging USB disks off a Raspberry Pi.
[658.48 → 663.16] But if I had Thunderbolt support, I could have real, actual, PCI-attached storage.
[663.70 → 669.70] And if I had an M1 CPU, I would have something that has built-in HD64 decoding and encoding,
[669.96 → 671.10] like a Banshee.
[671.96 → 674.44] And if somehow Plex could come along and get support for that,
[674.60 → 676.26] then we'd really be cooking with gas.
[676.46 → 680.06] Don't you just wish that macOS Server wasn't terrible?
[680.06 → 683.28] Is macOS Server even a thing anymore?
[683.40 → 683.84] I think they might.
[684.04 → 684.26] No.
[684.26 → 685.30] I don't even know.
[685.80 → 687.26] I know, it's really sad.
[687.60 → 691.60] And honestly, I feel like Docker Desktop isn't good enough on the Mac for production use,
[691.64 → 692.24] the way I would want.
[692.32 → 693.28] I want something headless.
[693.40 → 694.22] I want it to be Linux.
[694.64 → 697.54] I mean, Asa hi, the last couple of weeks,
[698.18 → 703.32] released preliminary support for GPU acceleration under Linux with the M1 chip,
[703.40 → 705.52] which is a huge, huge milestone.
[705.52 → 707.38] Yeah, using a Rust driver.
[708.14 → 709.20] A Rust driver.
[709.62 → 710.46] I mean, that's amazing.
[711.20 → 713.32] So maybe, I mean, maybe it's not too far off,
[713.38 → 716.60] but it's not going to be within the time that I need to build my next home server.
[717.18 → 720.88] I think I'm going to have to, just out of practicality, base it around this yellow.
[721.26 → 722.92] It would seem crazy not to, you know,
[722.94 → 727.02] showing up on my doorstep as I'm returning in town and I need a new server.
[727.16 → 729.40] Yeah, if you need an appliance, it sounds like that might be it.
[729.46 → 730.38] But let me ask you this.
[730.38 → 735.84] If money was no object, what would you do in dupes?
[736.22 → 737.30] The trickiest thing is storage.
[737.46 → 741.20] If money was no object, I'd spend a lot on storage, and it'd be solid state storage
[741.20 → 742.30] because I have to go down the road.
[743.24 → 745.18] So that's where I'd probably blow a lot of money.
[746.02 → 748.62] You're not going to believe this, but I mean, for 90% of the time,
[748.66 → 751.30] I have found the Raspberry Pi 4 has been fast enough.
[751.72 → 753.74] The pages could have always loaded faster in Home Assistant.
[753.94 → 755.64] And I'm on a couple of versions behind now.
[756.14 → 757.46] Home Assistant could have always been faster.
[757.46 → 761.74] But Plex and Sync thing and like my Markdown Docs,
[761.76 → 763.80] I forget the name of the Markdown Docs website thing.
[764.26 → 766.04] Those all always ran totally fine.
[766.36 → 767.16] I was surprised.
[767.30 → 769.60] I was shocked that I got by with a Raspberry Pi.
[769.98 → 773.16] It was just Home Assistant that could be a little bit faster.
[773.74 → 776.80] But, you know, a lot of that might have come down to storage technology.
[777.44 → 779.70] That's why I think the M1 would be perfect, you know?
[779.80 → 780.02] Yeah.
[780.24 → 783.72] 10, 20 watts, a lot of horsepower, fast storage.
[784.42 → 785.50] Just don't want macOS.
[785.50 → 790.04] Well, if power was no object, I know we made money no object just then,
[790.10 → 792.30] but I think power is probably your biggest limiting factor,
[792.46 → 793.72] as well as maybe space.
[794.20 → 796.72] Like, you can't have a big 42U rack in there, can you?
[797.04 → 799.60] Like, if power was no object, would you do the same thing?
[800.08 → 803.52] If power was no object, I think I'd be tempted to build a rack unit
[803.52 → 805.76] into one of the storage bays, you know,
[805.80 → 807.60] and go with like a big x86 box.
[807.60 → 811.50] And probably do a lot of hosting in Joop's,
[812.20 → 814.74] just because that's...
[814.74 → 815.68] I like the idea of something.
[815.86 → 817.26] It's truly decentralized.
[817.56 → 818.20] I can move it.
[818.26 → 819.22] I can take it with me.
[819.80 → 822.04] And I'd rather have the source of truth here,
[822.08 → 823.08] as long as I had a good backup.
[823.54 → 826.04] Right now, I hold the source of truth in everything at the studio.
[826.50 → 828.80] So I'd probably build a rack unit, if I could go crazy.
[828.94 → 829.82] But I don't need it.
[830.26 → 832.54] You know, I didn't lose any data.
[832.54 → 834.82] My server's down, but I didn't lose any data.
[835.24 → 837.32] So the setup is working as I need it to.
[838.34 → 841.24] Well, the obvious thing that comes to mind for me
[841.24 → 846.86] is the Intel NUC, that kind of tiny mini micro thing.
[846.94 → 848.96] I don't know if you've been following Serve the Home at all
[848.96 → 849.94] over the last few months.
[850.60 → 852.82] They've been doing a series called Tiny Mini Micro,
[852.98 → 857.80] where they get these four, five, six, ten liters micro,
[858.52 → 861.08] essentially thin client machines designed for
[862.54 → 863.98] business applications.
[864.70 → 867.46] And they've got powerful chips in them
[867.46 → 870.80] and 32 gigs of RAM and, you know, all the rest of it.
[871.12 → 874.66] And they are the size of two or three CD cases
[874.66 → 875.82] stacked on top of each other.
[876.74 → 877.98] What about something like that?
[878.34 → 879.78] That is pretty tempting,
[880.42 → 882.96] especially if it's got, you know, reasonable horsepower
[882.96 → 885.16] and it can do decent video decoding.
[886.30 → 888.28] That would be, and networking and connectivity,
[888.82 → 890.64] because I always need to add more storage.
[890.64 → 893.36] I think what you'd be looking for there is your silver bullet
[893.36 → 895.56] for video decoding would be Quick Sync support,
[895.76 → 897.76] which does limit you to Intel.
[898.20 → 900.24] But, you know, speaking from experience,
[900.46 → 903.44] Quick Sync uses anywhere from four to six,
[903.54 → 906.46] maybe eight watts to transcode a 4K stream.
[906.74 → 908.50] And it's hard limited at eight watts.
[908.68 → 911.26] Like I've never been able to get it to go above eight,
[911.94 → 914.30] eight to 10 watts is about the maximum I've ever seen.
[914.52 → 917.18] So even if you're doing multiple transcodes at once,
[917.18 → 919.50] which in an RV I find very unlikely,
[920.28 → 921.24] Quick Sync is the way to go.
[921.82 → 922.42] That is the nice thing,
[922.46 → 924.62] is I only really need to build for like two televisions.
[925.00 → 926.64] Three is the max.
[926.74 → 927.78] Well, I guess there's always tablets,
[928.06 → 930.02] but very unlikely that we'd have three TVs
[930.02 → 931.42] and a tablet going in the RV.
[931.90 → 935.46] But you could negate the transcoding requirement entirely
[935.46 → 938.14] just simply by using something like TEAR
[938.14 → 940.48] or Handbrake to pre-encode the media.
[940.70 → 942.12] And you can automate all that stuff,
[942.48 → 944.30] you know, into the correct formats for the TV.
[944.30 → 946.06] You know, actually I think for the most part,
[946.52 → 947.94] I mean, for the most part,
[948.12 → 949.68] most of my stuff doesn't need transcoding
[949.68 → 951.74] because it's either an Apple TV or an NVIDIA Shield
[951.74 → 956.70] and it's H.264 and AC, MP3 or AC3 audio
[956.70 → 958.68] for the most part, not a hundred percent,
[958.92 → 961.62] but I'd say 85, 90%.
[961.62 → 963.72] How many terabytes do you need?
[964.16 → 966.08] Here in Joop's, I'd love four.
[966.22 → 967.98] I'm getting by with two, right?
[968.04 → 969.34] I would love to do more even.
[969.46 → 972.50] I mean, ideally I'd love 14, let's be honest.
[972.50 → 976.12] But I get what I do is I batch over
[976.12 → 977.42] just the stuff we're watching,
[977.52 → 979.08] like a couple of series for the kids,
[979.48 → 981.48] a couple of movies that are for Hades and I,
[981.56 → 982.82] a couple of movies that are for the kids
[982.82 → 984.08] and a couple of movies that are for family
[984.08 → 985.86] and just a few TV shows.
[986.30 → 987.74] And I just kind of keep like
[987.74 → 989.04] what the current season is
[989.04 → 990.72] that we're watching of a show on there.
[990.78 → 991.88] And I don't need to keep everything
[991.88 → 993.74] because I have a larger storage at the studio.
[994.22 → 996.26] I have no idea how reliable this is,
[996.32 → 997.22] but I just looked on Amazon
[997.22 → 998.26] just to sort of see
[998.26 → 1001.46] how much a two terabyte SSD costs these days.
[1001.88 → 1003.36] The brands you've heard of,
[1003.56 → 1005.98] Samsung, Crucial, et cetera,
[1006.22 → 1008.94] they're all in the 160 to 200 range
[1008.94 → 1010.28] per two terabytes.
[1011.08 → 1012.02] But there's a brand here
[1012.02 → 1013.54] I've never heard of called Leven.
[1014.44 → 1016.84] And these guys make a two terabyte
[1016.84 → 1021.84] 3D NAND SATA 3 internal SSD for $99.
[1022.26 → 1024.16] I mean, you throw a few of those in a raid,
[1024.26 → 1025.00] what could go wrong?
[1025.66 → 1027.76] You throw a few of those in Merger FS.
[1028.72 → 1031.00] And what I'm thinking is before a trip, right,
[1031.04 → 1033.48] you take one or two of these into the studio,
[1033.68 → 1034.96] sync across what you need to
[1034.96 → 1037.14] through a USB interface
[1037.14 → 1039.56] that's much faster than a network interface.
[1040.34 → 1041.52] And then you throw it back
[1041.52 → 1043.46] into your hot swap bay in dupes
[1043.46 → 1045.22] and you're good to go.
[1045.70 → 1045.78] Yeah.
[1045.86 → 1047.78] And then you just keep it topped off
[1047.78 → 1049.48] with a little sync thing action, you know?
[1049.84 → 1050.16] Yes.
[1050.54 → 1051.68] Yeah, that could totally work.
[1052.22 → 1054.90] What I'm kind of picturing is like a board, right?
[1055.00 → 1055.76] Like a removable,
[1056.16 → 1057.88] almost like a piece of plywood
[1057.88 → 1060.02] that has the yellow mounted to it
[1060.02 → 1061.96] and the disks mounted to it
[1061.96 → 1065.00] and the Zigbee and Z-Wave antennas mounted to it.
[1065.20 → 1068.12] And I can just insert this board into dupes
[1068.12 → 1069.74] and I can pull this board out of dupes.
[1070.12 → 1071.32] And if I need to work on it,
[1071.36 → 1073.30] I just remove the whole component,
[1073.40 → 1075.88] all of it put together as one piece.
[1076.04 → 1077.98] I take it to the studio and I work on it
[1077.98 → 1079.16] and then I bring it back into dupes
[1079.16 → 1081.02] and I just reinstall it and reconnect things.
[1081.52 → 1082.74] I love that modular approach.
[1083.22 → 1084.52] I'd love to add into that mix
[1084.52 → 1087.54] your new mixer plans too.
[1087.62 → 1088.58] That would be kind of fun, huh?
[1088.76 → 1091.30] Oh, imagine.
[1091.64 → 1092.96] The ultimate setup, right?
[1093.02 → 1095.18] Like server capacity, media capacity
[1095.18 → 1096.74] and production capacity
[1096.74 → 1097.82] and just slide them all in.
[1098.02 → 1098.80] You have, you know,
[1098.88 → 1100.92] like eight XLR inputs on the front of this thing
[1100.92 → 1102.54] for all your mics and what have you.
[1102.84 → 1103.74] And then on the back,
[1103.80 → 1105.66] you've got a couple of network jacks
[1105.66 → 1107.00] and a power cord going in
[1107.00 → 1107.80] and that's it.
[1107.80 → 1108.82] That would be pretty cool.
[1108.92 → 1110.18] That sounds really sweet, actually.
[1110.18 → 1112.22] Pretty, pretty, pretty great.
[1112.46 → 1113.36] Pretty, pretty great.
[1113.44 → 1114.48] Let's work on that then.
[1114.72 → 1117.84] But speaking of upgrades and stuff like that,
[1117.92 → 1119.70] I assume you saw that Paulus
[1119.70 → 1121.44] from the Home Assistant project
[1121.44 → 1123.80] has been very, very excited
[1123.80 → 1126.78] that Matter finally hit 1.0 this week.
[1127.62 → 1128.04] Damn it.
[1128.40 → 1129.62] Can you believe this?
[1130.70 → 1131.46] You know what that means
[1131.46 → 1132.32] is that they're beginning
[1132.32 → 1133.36] to pull it into Home Assistant.
[1133.56 → 1135.16] They're beginning to build in Matter support
[1135.16 → 1135.76] and a Home Assistant
[1135.76 → 1138.96] and an actual device shipped
[1138.96 → 1140.10] in the last week,
[1140.44 → 1141.88] a light bulb with Matter.
[1142.38 → 1143.72] It's actually happening,
[1144.28 → 1146.20] but you know it's really still like
[1146.20 → 1148.34] probably six months to a year out
[1148.34 → 1150.50] before just general devices are available.
[1151.42 → 1152.64] And of course,
[1153.22 → 1154.94] of course I'm doing this rebuild right now.
[1155.04 → 1156.40] Of course my server died.
[1156.50 → 1157.40] I couldn't hold out.
[1157.66 → 1159.12] You know I was holding out for Matter.
[1159.32 → 1160.78] You know that was what I did.
[1161.04 → 1162.76] That was my entire intention all along
[1162.76 → 1163.28] was to hold out
[1163.28 → 1164.44] and just replace my devices
[1164.44 → 1165.32] with Matter devices.
[1165.84 → 1167.08] And just as it becomes official,
[1167.28 → 1169.04] just as the first device ships,
[1169.36 → 1170.50] my system dies
[1170.50 → 1171.60] and I'm going to have to either go
[1171.60 → 1173.02] all in on Z-Wave or Zigbee.
[1173.98 → 1175.82] Zigbee's very well tested though.
[1176.28 → 1177.68] I wouldn't imagine Matter's
[1177.68 → 1178.96] going to be stable,
[1179.22 → 1180.06] properly stable,
[1180.06 → 1181.08] for another,
[1182.46 → 1183.72] I don't want to say five years.
[1184.10 → 1185.22] That might be a bit pessimistic,
[1185.42 → 1185.88] but you know,
[1185.94 → 1187.38] at least two or three
[1187.38 → 1188.56] before we've got,
[1188.68 → 1188.88] you know,
[1188.92 → 1190.44] the ubiquitous level of devices
[1190.44 → 1191.74] we have now in Zigbee land.
[1191.74 → 1193.74] I pulled the trigger
[1193.74 → 1194.60] and I pre-ordered
[1194.60 → 1196.12] the Home Assistant,
[1196.26 → 1196.98] I think they call it,
[1197.62 → 1197.96] link?
[1198.02 → 1198.94] What do they call it, Alex?
[1199.26 → 1200.50] Sky Connect, I think.
[1200.96 → 1201.52] Yeah, Sky Connect.
[1202.26 → 1204.02] It is a Zigbee radio.
[1204.68 → 1205.78] It has Zigbee and thread
[1205.78 → 1206.64] and they promise
[1206.64 → 1207.96] they'll do a firmware upgrade
[1207.96 → 1209.46] and add Matter to it.
[1209.90 → 1211.26] So Home Assistant Sky Connect
[1211.26 → 1212.92] is their own hardware
[1212.92 → 1214.52] Zigbee radio.
[1216.28 → 1217.08] Which seems like,
[1217.16 → 1217.40] okay,
[1217.52 → 1218.38] so Home Assistant's
[1218.38 → 1220.30] clearly going all in on Zigbee.
[1220.30 → 1221.96] This is a clear signal
[1221.96 → 1222.80] from the project.
[1222.96 → 1223.90] Zigbee is the future
[1223.90 → 1224.60] of Home Assistant
[1224.60 → 1225.76] and Matter.
[1226.66 → 1228.16] But then they made the announcement
[1228.16 → 1229.42] that they just full-time
[1229.42 → 1231.06] hired the Z-Wave integration guy.
[1231.78 → 1233.42] And now the Z-Wave integration guy
[1233.42 → 1235.12] is a Nebulas employee.
[1235.82 → 1236.24] Mixed messages,
[1236.36 → 1237.02] it sounds like.
[1237.02 → 1237.04] It is.
[1237.22 → 1238.42] I'm so confused
[1238.42 → 1239.24] as to what direction
[1239.24 → 1240.26] to go right now.
[1240.62 → 1242.38] I think what they're saying is,
[1242.50 → 1243.66] whatever you want to use,
[1243.70 → 1244.28] we're going to support.
[1244.62 → 1245.28] And we're going to try
[1245.28 → 1246.12] to support it really well.
[1246.16 → 1246.94] But they haven't, like,
[1246.98 → 1248.58] just clearly articulated that to me.
[1248.58 → 1249.52] So I'm trying to figure out, like,
[1249.82 → 1251.06] well, if I'm going to buy one device,
[1251.12 → 1251.80] should I buy Zigbee
[1251.80 → 1253.06], or should I be buying Z-Wave
[1253.06 → 1253.74] or what?
[1254.46 → 1254.72] It's like,
[1254.76 → 1255.38] I'm probably going to have to
[1255.38 → 1256.36] replace some of these devices
[1256.36 → 1257.38] because some of these things
[1257.38 → 1258.56] are probably not going to
[1258.56 → 1259.44] unpair very easily
[1259.44 → 1260.32] with my dead system.
[1261.84 → 1262.98] Or are they saying that
[1262.98 → 1264.30] when you buy this
[1264.30 → 1265.14] in a year from now
[1265.14 → 1265.94] when it actually lands
[1265.94 → 1266.42] on your door,
[1266.52 → 1268.16] then they'll be supporting it
[1268.16 → 1268.56] full-time.
[1268.68 → 1268.88] Yeah.
[1269.04 → 1269.92] It is a pre-order
[1269.92 → 1270.84] and it is, quote,
[1270.92 → 1272.18] available soon.
[1272.54 → 1273.64] So just as I'm finally
[1273.64 → 1274.54] receiving my yellow,
[1274.68 → 1275.54] we'll see how long it takes me
[1275.54 → 1276.46] to get my Sky Connect.
[1276.46 → 1280.84] linode.com slash SSH.
[1280.92 → 1281.76] Go there to get $100
[1281.76 → 1282.92] in 60-day credit
[1282.92 → 1283.58] on a new account.
[1283.72 → 1284.32] It's just a great way
[1284.32 → 1284.96] to support the show
[1284.96 → 1285.52] while you're checking out
[1285.52 → 1286.12] something awesome.
[1286.64 → 1287.56] Linde is fast,
[1287.68 → 1288.72] reliable cloud hosting
[1288.72 → 1289.98] with the best support
[1289.98 → 1290.58] in the business,
[1290.72 → 1291.40] real humans,
[1292.02 → 1292.68] every day.
[1292.92 → 1293.62] It's how we run
[1293.62 → 1294.76] everything we've built
[1294.76 → 1295.64] in the last few years
[1295.64 → 1296.08] in the cloud,
[1296.14 → 1297.52] like our brand-new website.
[1297.84 → 1298.54] You've got to go check it out,
[1298.60 → 1299.84] jupiterbroadcasting.com.
[1300.06 → 1300.88] We use it
[1300.88 → 1302.12] in our personal environments,
[1302.26 → 1302.72] we use it
[1302.72 → 1303.70] in our testing environments,
[1303.70 → 1304.16] and we use it
[1304.16 → 1305.04] in our production environments
[1305.04 → 1306.04] because Linde's tooling
[1306.04 → 1307.20] makes it really straightforward
[1307.20 → 1308.48] to do all of that.
[1309.04 → 1309.90] And Linde was built
[1309.90 → 1311.18] nearly 19 years ago,
[1311.28 → 1312.06] and they've just added
[1312.06 → 1313.52] better and better things.
[1313.62 → 1314.30] They've improved.
[1314.44 → 1315.62] They've refined the service
[1315.62 → 1316.06] over the years.
[1316.10 → 1316.46] So now,
[1317.22 → 1317.56] like,
[1317.84 → 1318.90] we're riding on top
[1318.90 → 1319.72] of years and years
[1319.72 → 1320.72] and years of investment.
[1321.26 → 1322.38] We get all of that
[1322.38 → 1323.84] as just part of the product,
[1323.94 → 1324.62] and Linde is still
[1324.62 → 1325.92] 30% to 50% cheaper
[1325.92 → 1326.88] than the hyperscalers
[1326.88 → 1328.00] that want to lock you
[1328.00 → 1329.10] into their crazy platforms
[1329.10 → 1329.88] that are just secondary
[1329.88 → 1330.86] to their main business.
[1331.78 → 1332.70] And on top of that,
[1332.70 → 1333.12] I think Linde
[1333.12 → 1333.94] has the best performance
[1333.94 → 1334.36] out there.
[1334.78 → 1335.54] And independent testing
[1335.54 → 1336.58] is also showing that.
[1336.84 → 1337.36] And right now,
[1337.44 → 1337.72] today,
[1337.90 → 1339.00] Linde has 11 data centres
[1339.00 → 1339.62] for you to choose from,
[1339.68 → 1340.60] and that's a bunch
[1340.60 → 1341.30] all over the world.
[1342.08 → 1343.06] But coming soon,
[1343.40 → 1344.50] there's going to be more
[1344.50 → 1345.58] than a dozen new
[1345.58 → 1346.44] Linde data centres
[1346.44 → 1348.34] firing up across the world.
[1348.96 → 1350.06] That's just going to be insane.
[1350.16 → 1350.46] You're going to have
[1350.46 → 1351.20] so much choice.
[1351.32 → 1351.52] And you know,
[1351.56 → 1352.84] Linde really is
[1352.84 → 1354.34] just the perfect balance
[1354.34 → 1355.44] of support,
[1355.84 → 1356.32] performance,
[1356.60 → 1357.60] and price.
[1357.92 → 1358.62] So with that $100,
[1359.06 → 1359.68] you get a chance
[1359.68 → 1360.52] to see it for yourself.
[1360.52 → 1361.82] That really is an opportunity
[1361.82 → 1362.72] to kick the tires
[1362.72 → 1363.68] and try it.
[1363.98 → 1365.04] So go build something,
[1365.58 → 1366.38] go learn something,
[1366.46 → 1367.66] go experiment with something,
[1367.84 → 1369.06] and support the show.
[1369.42 → 1370.22] Try it for yourself.
[1370.34 → 1371.26] Get that $100 at
[1371.26 → 1373.52] linode.com slash SSH.
[1373.68 → 1374.46] One more time,
[1374.54 → 1377.32] that's linode.com slash SSH.
[1378.82 → 1380.18] We're trying to review an app
[1380.18 → 1381.18] that I've actually put
[1381.18 → 1381.86] in the show notes
[1381.86 → 1382.74] more times
[1382.74 → 1383.76] than I can actually remember.
[1383.88 → 1384.70] We just never quite
[1384.70 → 1385.74] seem to get to it.
[1386.70 → 1387.60] This time,
[1387.94 → 1388.50] finally,
[1388.68 → 1389.36] Invoice Ninja
[1389.36 → 1390.16] has made the cut
[1390.16 → 1390.88] into the show.
[1390.88 → 1391.72] So I thought
[1391.72 → 1392.46] it would be good
[1392.46 → 1393.06] because I know,
[1393.38 → 1393.56] Brent,
[1393.64 → 1394.26] you do quite a lot
[1394.26 → 1395.26] of freelancing stuff
[1395.26 → 1396.02] with your photography
[1396.02 → 1397.40] and other things,
[1397.54 → 1397.72] you know,
[1397.80 → 1398.94] podcast-related stuff.
[1399.12 → 1399.76] So you're always
[1399.76 → 1400.38] sending invoices
[1400.38 → 1400.78] to people.
[1401.06 → 1401.66] So I thought
[1401.66 → 1402.28] whilst we had you
[1402.28 → 1402.68] on the show,
[1402.74 → 1403.60] it would be a good time
[1403.60 → 1405.00] to discuss
[1405.00 → 1405.90] Invoice Ninja.
[1406.48 → 1406.84] Now,
[1406.90 → 1407.48] this is a piece
[1407.48 → 1407.90] of software
[1407.90 → 1408.52] that allows you
[1408.52 → 1409.02] to create
[1409.02 → 1410.02] customizable
[1410.02 → 1411.10] and nicely designed
[1411.10 → 1412.40] invoices and quotes.
[1412.92 → 1413.50] So essentially,
[1414.80 → 1415.66] whenever I do
[1415.66 → 1416.26] a piece of freelance
[1416.26 → 1417.74] work for somebody,
[1417.74 → 1419.72] I create a customer
[1419.72 → 1420.96] in the Invoice Ninja
[1420.96 → 1422.26] software and then
[1422.26 → 1423.28] I create a product,
[1423.52 → 1423.74] you know,
[1423.76 → 1424.94] like a podcast episode,
[1425.04 → 1425.48] for example,
[1425.64 → 1427.06] or something like that.
[1427.18 → 1428.54] And then I put in there,
[1428.58 → 1428.80] you know,
[1428.84 → 1429.74] what the product is.
[1429.84 → 1430.84] It could be a physical
[1430.84 → 1431.18] thing,
[1431.22 → 1432.02] it could be a service,
[1432.16 → 1432.42] whatever,
[1432.62 → 1434.16] and it has a rate
[1434.16 → 1434.98] attached to it,
[1435.00 → 1435.80] a standard rate,
[1436.46 → 1437.28] which I can go in
[1437.28 → 1438.44] and customize if I want to,
[1438.52 → 1439.62] but typically it doesn't
[1439.62 → 1440.24] change that much
[1440.24 → 1441.10] between clients.
[1441.76 → 1442.36] After that,
[1442.44 → 1442.98] it automatically
[1442.98 → 1444.10] generates the invoice
[1444.10 → 1445.44] based on my information
[1445.44 → 1446.98] and the client's information.
[1447.98 → 1449.22] And if you get fancy
[1449.22 → 1450.94] and set up email with it,
[1450.98 → 1451.92] which I've never done,
[1451.98 → 1452.80] I always just download
[1452.80 → 1454.02] the PDF once it's
[1454.02 → 1454.84] generated the invoice
[1454.84 → 1456.72] and stick it in my email
[1456.72 → 1457.12] manually,
[1457.36 → 1458.38] but it can actually
[1458.38 → 1459.82] send emails directly
[1459.82 → 1460.80] from the Invoice Ninja
[1460.80 → 1462.10] software to the client,
[1462.58 → 1463.30] which is a really nice
[1463.30 → 1463.66] feature.
[1464.48 → 1464.50] Alex,
[1464.68 → 1465.62] you're right to include me
[1465.62 → 1466.38] because I have a lot
[1466.38 → 1467.16] of questions.
[1467.90 → 1468.24] Okay,
[1468.48 → 1468.96] fire away.
[1469.26 → 1469.44] Okay,
[1469.50 → 1470.26] you've been using this
[1470.26 → 1470.88] for how long now?
[1471.04 → 1471.74] I think it's been like
[1471.74 → 1472.46] two years,
[1472.52 → 1472.94] if I remember.
[1473.10 → 1473.70] Two years,
[1473.80 → 1474.76] plus however long it is
[1474.76 → 1475.56] since I set you up
[1475.56 → 1476.86] with your instance
[1476.86 → 1478.46] that is probably dead
[1478.46 → 1478.98] by now.
[1479.44 → 1480.70] You did send me a backup,
[1480.90 → 1481.86], so thank you for that.
[1482.10 → 1482.40] Okay,
[1482.58 → 1482.82] okay,
[1482.88 → 1483.08] good.
[1483.38 → 1483.58] Yeah,
[1483.62 → 1483.88] Alex,
[1483.96 → 1485.24] you shared with me
[1485.24 → 1485.86] Invoice Ninja,
[1486.00 → 1486.76] I think when you first
[1486.76 → 1487.24] found it,
[1487.38 → 1488.34] or maybe you were
[1488.34 → 1489.00] a few months in
[1489.00 → 1489.96] and you were crazy
[1489.96 → 1490.66] excited about it
[1490.66 → 1491.40] and I did get the
[1491.40 → 1492.32] chance to try it.
[1492.44 → 1492.58] Yeah,
[1492.70 → 1494.76] it's years old
[1494.76 → 1495.40] in my workflow
[1495.40 → 1496.10] now at this point.
[1496.56 → 1497.40] Everything you described
[1497.40 → 1498.02] to your introduction
[1498.02 → 1498.60] just there
[1498.60 → 1500.10] is not something
[1500.10 → 1500.92] that I think
[1500.92 → 1501.86] is unique.
[1502.26 → 1502.84] I'm curious
[1502.84 → 1503.74] from your perspective,
[1503.74 → 1505.04] what are the things
[1505.04 → 1505.56] that you're really
[1505.56 → 1506.22] loving about this?
[1506.30 → 1507.98] Is it the fact
[1507.98 → 1508.58] that you can
[1508.58 → 1509.32] self-host it
[1509.32 → 1509.84] really easily?
[1510.04 → 1510.70] Is it the fact
[1510.70 → 1511.48] that it's really
[1511.48 → 1511.92] responsive?
[1512.18 → 1513.24] Is it the interface?
[1513.54 → 1514.18] What is it about it
[1514.18 → 1514.88] that really grabs you?
[1514.96 → 1515.06] Yeah,
[1515.08 → 1515.96] I didn't touch much
[1515.96 → 1517.02] on the actual
[1517.02 → 1518.12] mechanics of hosting
[1518.12 → 1518.62] this thing.
[1519.12 → 1520.56] The Invoice Ninja project
[1520.56 → 1522.06] actually has hosted
[1522.06 → 1522.92] options which you can
[1522.92 → 1523.88] pay monthly for.
[1524.38 → 1524.76] However,
[1524.88 → 1525.52] I don't do that.
[1525.70 → 1526.50] I have a fully
[1526.50 → 1527.44] self-hosted version
[1527.44 → 1528.38] that lives on my server.
[1528.98 → 1530.04] This thing requires
[1530.04 → 1530.88] three containers.
[1531.08 → 1531.50] So there's the
[1531.50 → 1532.20] app container,
[1532.20 → 1533.20] there's a database
[1533.20 → 1534.50] container which in
[1534.50 → 1535.16] my case I'm using
[1535.16 → 1536.54] MySQL and then
[1536.54 → 1537.34] there's a front end
[1537.34 → 1538.24] which in my case
[1538.24 → 1539.08] I'm using Nginx
[1539.08 → 1539.98] which I then proxy
[1539.98 → 1540.72] through traffic.
[1541.64 → 1542.60] So I'll tell you
[1542.60 → 1543.38] what I like about it.
[1543.46 → 1544.22] Just as a piece
[1544.22 → 1544.68] of software,
[1545.40 → 1546.98] it looks nice.
[1547.48 → 1547.58] Yeah,
[1547.64 → 1548.30] I'll agree with that.
[1548.64 → 1549.32] I like the fact
[1549.32 → 1550.06] that when I create
[1550.06 → 1551.14] an invoice it gives
[1551.14 → 1552.18] me a little chart
[1552.18 → 1553.10] that says you're owed
[1553.10 → 1553.86] I don't know
[1553.86 → 1555.42] $500 this month
[1555.42 → 1556.30] and then until
[1556.30 → 1557.60] you mark that invoice
[1557.60 → 1559.32] as received
[1559.32 → 1559.94] or paid
[1559.94 → 1560.98] it will show you
[1560.98 → 1561.88] a pending number
[1561.88 → 1562.74] versus a last
[1562.74 → 1563.58] 30 day number
[1563.58 → 1565.36] versus a 90 day
[1565.36 → 1566.16] number or whatever
[1566.16 → 1566.56] you want.
[1567.42 → 1568.06] So I could see
[1568.06 → 1569.02] this being very useful
[1569.02 → 1569.78] for people who are
[1569.78 → 1570.36] actually sending
[1570.36 → 1571.46] hundreds of invoices
[1571.46 → 1572.12] every day.
[1572.56 → 1573.70] Less useful for me
[1573.70 → 1574.52] who sends maybe
[1574.52 → 1575.12] one a month
[1575.12 → 1575.84] or two a month
[1575.84 → 1577.58] but it's still nice
[1577.58 → 1578.32] to have a record
[1578.32 → 1578.72] of everything
[1578.72 → 1579.36] I've ever sent
[1579.36 → 1580.94] in one place.
[1581.64 → 1582.16] The other thing
[1582.16 → 1582.98] that I like about it
[1582.98 → 1584.06] too is that
[1584.06 → 1585.28] I can
[1585.28 → 1587.36] tweak stuff
[1587.36 → 1589.18] and I feel like
[1589.18 → 1591.04] I'm driving
[1591.04 → 1591.98] a really powerful
[1591.98 → 1592.78] sports car
[1592.78 → 1593.36] and I'm
[1593.36 → 1593.98] okay I'm only
[1593.98 → 1594.90] pooling down the road
[1594.90 → 1595.98] at 30 miles an hour
[1595.98 → 1597.64] but it's nice to know
[1597.64 → 1598.56] that it's got
[1598.56 → 1599.46] all of that other
[1599.46 → 1599.96] stuff there
[1599.96 → 1601.00] should I ever need it.
[1601.32 → 1601.80] Yeah and I think
[1601.80 → 1603.30] too it's pretty quick
[1603.30 → 1604.26] that the pricing
[1604.26 → 1605.08] on a lot of the
[1605.08 → 1606.20] hosted invoicing
[1606.20 → 1607.70] can get really
[1607.70 → 1608.44] expensive.
[1609.50 → 1610.04] You know I
[1610.04 → 1611.20] have been a customer
[1611.20 → 1611.74] of FreshBooks
[1611.74 → 1612.80] for a long time
[1612.80 → 1614.34] but I think
[1614.34 → 1614.68] I'm paying
[1614.68 → 1615.60] somewhere near
[1615.60 → 1616.80] $50 a month
[1616.80 → 1617.62] or something like that
[1617.62 → 1618.40] $60 a month
[1618.40 → 1619.00] for the package
[1619.00 → 1619.98] well JB does
[1619.98 → 1620.36] not me
[1620.36 → 1621.70] but it's actually
[1621.70 → 1622.64] kind of good deal
[1622.64 → 1623.44] for a lot of these things.
[1623.54 → 1624.04] People pay
[1624.04 → 1625.50] astronomical prices
[1625.50 → 1626.42] for QuickBooks
[1626.42 → 1626.98] and the invoicing
[1626.98 → 1627.50] components.
[1628.30 → 1628.92] So there's that
[1628.92 → 1630.16] aspect of invoicing
[1630.16 → 1631.20] besides the UI
[1631.20 → 1632.12] and besides the
[1632.12 → 1632.60] self-hosting
[1632.60 → 1633.12] and the tinkering
[1633.12 → 1633.62] there's the
[1633.62 → 1634.80] cost savings too.
[1635.32 → 1635.68] In addition
[1635.68 → 1636.72] it does a whole
[1636.72 → 1637.58] bunch of other stuff
[1637.58 → 1638.58] so I can set up
[1638.58 → 1639.24] things like
[1639.24 → 1640.34] recurring invoices
[1640.34 → 1641.14] if I want to
[1641.14 → 1642.12] in a separate area
[1642.12 → 1643.34] from individual invoices
[1643.34 → 1644.92] I can record
[1644.92 → 1645.66] manually
[1645.66 → 1646.70] all the payments
[1646.70 → 1647.36] that come in
[1647.36 → 1648.28] and attach those
[1648.28 → 1649.54] to specific invoices
[1649.54 → 1650.36] if I want to.
[1650.82 → 1651.94] I can also do things
[1651.94 → 1652.60] like quotes
[1652.60 → 1653.30] and proposals
[1653.30 → 1654.10] and set up
[1654.10 → 1655.10] specific projects
[1655.10 → 1655.64] and attach
[1655.64 → 1656.38] different things
[1656.38 → 1657.96] within Invoice Ninja
[1657.96 → 1659.36] to different projects
[1659.36 → 1660.22] and what have you
[1660.22 → 1661.14] which you know
[1661.14 → 1661.66] if I was
[1661.66 → 1662.52] I don't know
[1662.52 → 1663.24] let's say running
[1663.24 → 1664.38] a home improvement company
[1664.38 → 1665.38] that could be quite useful
[1665.38 → 1666.90] to have different quotes
[1666.90 → 1668.22] for the same person
[1668.22 → 1669.88] within a single project
[1669.88 → 1670.44] for example
[1670.44 → 1671.34] or something like that.
[1671.82 → 1672.90] I can also do things
[1672.90 → 1673.68] like track
[1673.68 → 1675.18] different vendors
[1675.18 → 1676.22] so I can say
[1676.22 → 1677.52] well this vendor
[1677.52 → 1678.76] I've sent them
[1678.76 → 1679.20] this money
[1679.20 → 1679.88] for this product
[1679.88 → 1681.40] and like I say
[1681.40 → 1682.88] it's an incredibly
[1682.88 → 1683.98] powerful piece of software
[1683.98 → 1685.26] that I'm really only
[1685.26 → 1686.46] scratching the surface of
[1686.46 → 1688.18] by pretty much
[1688.18 → 1689.16] only using the invoice
[1689.16 → 1690.00] portion of it
[1690.00 → 1692.50] but it has the ability
[1692.50 → 1693.52] to run some pretty
[1693.52 → 1694.86] sophisticated reporting
[1694.86 → 1695.26] as well
[1695.26 → 1695.78] so again
[1695.78 → 1697.16] if I was a bit more
[1697.16 → 1697.70] of a serious
[1697.70 → 1698.66] small business owner
[1698.66 → 1699.48] or something like that
[1699.48 → 1700.54] which I'm not
[1700.54 → 1701.70] I could
[1701.70 → 1702.28] you know
[1702.28 → 1702.94] let's say
[1702.94 → 1704.08] give me the last
[1704.08 → 1704.66] you know
[1704.66 → 1705.44] every invoice
[1705.44 → 1706.08] this year
[1706.08 → 1707.82] to a specific client
[1707.82 → 1708.88] or something like that
[1708.88 → 1710.54] and it'll just show me
[1710.54 → 1711.12] all those things
[1711.12 → 1711.84] in one place.
[1712.52 → 1712.82] Now Alex
[1712.82 → 1713.78] have you used anything else
[1713.78 → 1714.30] for invoicing
[1714.30 → 1715.00] or is this kind of
[1715.00 → 1716.06] your first foray
[1716.06 → 1717.52] into this style of software
[1717.52 → 1719.00] to help you accomplish things?
[1719.42 → 1720.32] I used to just have
[1720.32 → 1721.58] a Google sheet
[1721.58 → 1722.20] that I've
[1722.20 → 1722.50] you know
[1722.50 → 1723.48] manually changed
[1723.48 → 1724.66] and filled out things
[1724.66 → 1726.74] for a long time
[1726.74 → 1727.60] which is also
[1727.60 → 1728.32] very powerful.
[1728.78 → 1729.60] It can be
[1729.60 → 1730.68] but it's also
[1730.68 → 1731.56] you know
[1731.56 → 1732.08] you don't really
[1732.08 → 1732.86] have a record
[1732.86 → 1733.88] unless you do
[1733.88 → 1734.44] a new sheet
[1734.44 → 1735.08] per invoice
[1735.08 → 1735.50] or something
[1735.50 → 1736.66] of what you've done
[1736.66 → 1738.56] but this is the first
[1738.56 → 1739.68] kind of invoicing
[1739.68 → 1741.02] suite
[1741.02 → 1741.92] I guess
[1741.92 → 1742.56] that I've used.
[1743.20 → 1744.10] Because many of the features
[1744.10 → 1744.92] you described
[1744.92 → 1745.88] are yeah
[1745.88 → 1746.68] they're great
[1746.68 → 1747.48] they're not unique
[1747.48 → 1748.98] but what I have found
[1748.98 → 1749.66] when I used
[1749.66 → 1750.24] Invoice Ninja
[1750.24 → 1750.86] was that they're
[1750.86 → 1752.16] very well implemented
[1752.16 → 1753.08] and like you mentioned
[1753.08 → 1754.78] they allowed you
[1754.78 → 1755.78] to really tweak
[1755.78 → 1756.42] a lot of things.
[1756.80 → 1757.50] I have been using
[1757.50 → 1758.26] for many years
[1758.26 → 1759.10] a piece of software
[1759.10 → 1760.56] called Invoice Plane
[1760.56 → 1762.54] and it is
[1762.54 → 1763.72] far more basic
[1763.72 → 1764.74] it is self-hosted
[1764.74 → 1765.52] and I have some
[1765.52 → 1766.30] automated emails
[1766.30 → 1766.82] and stuff
[1766.82 → 1768.12] sending out of there
[1768.12 → 1770.68] but I do find
[1770.68 → 1771.90] after having used
[1771.90 → 1772.52] Invoice Ninja
[1772.52 → 1773.26] thanks to you
[1773.26 → 1774.04] that I feel
[1774.04 → 1774.88] it's lacking now
[1774.88 → 1775.84] and every time
[1775.84 → 1776.22] I use it
[1776.22 → 1776.48] I'm like
[1776.48 → 1776.92] oh god
[1776.92 → 1777.80] I really gotta switch over
[1777.80 → 1779.38] I have to change this
[1779.38 → 1780.46] so I think you
[1780.46 → 1781.50] made probably
[1781.50 → 1782.76] a really nice choice
[1782.76 → 1783.66] in choosing
[1783.66 → 1784.22] your first piece
[1784.22 → 1784.56] of software
[1784.56 → 1785.28] because often
[1785.28 → 1786.60] the hardest part
[1786.60 → 1787.76] is taking
[1787.76 → 1788.40] all that information
[1788.40 → 1789.30] out of these pieces
[1789.30 → 1789.72] of software
[1789.72 → 1790.46] and switching
[1790.46 → 1791.16] to something new
[1791.16 → 1791.82] that's one thing
[1791.82 → 1792.64] I really struggle with
[1792.64 → 1793.30] and so
[1793.30 → 1794.06] have you investigated
[1794.06 → 1794.58] at all
[1794.58 → 1795.98] what the
[1795.98 → 1797.64] importing and exporting
[1797.64 → 1799.52] parts of this
[1799.52 → 1800.56] database might look like
[1800.56 → 1801.66] and what that's like
[1801.66 → 1802.58] to port to something new
[1802.58 → 1803.22] if you so choose?
[1803.70 → 1804.38] Well I just
[1804.38 → 1805.18] whilst we were talking
[1805.18 → 1805.76] just then
[1805.76 → 1808.14] exported a CSV report
[1808.14 → 1809.26] of every
[1809.26 → 1811.76] invoice that I've sent
[1811.76 → 1812.22] this year
[1812.22 → 1812.94] so let's just take
[1812.94 → 1813.76] a quick look at that
[1813.76 → 1815.02] Apple Numbers of course
[1815.02 → 1815.50] is going to be
[1815.50 → 1816.80] a real fun time
[1816.80 → 1818.34] so the CSV
[1818.34 → 1819.16] is exactly
[1819.16 → 1819.86] what you'd expect
[1819.86 → 1820.72] it's just a bunch
[1820.72 → 1821.86] of this client
[1821.86 → 1822.52] this date
[1822.52 → 1823.34] this invoice number
[1823.34 → 1823.94] this amount
[1823.94 → 1824.54] status
[1824.54 → 1825.68] all that kind of stuff
[1825.68 → 1827.00] and so if you can
[1827.00 → 1827.94] get it out to a
[1827.94 → 1829.46] format that you
[1829.46 → 1830.24] you know
[1830.24 → 1832.08] own like a CSV file
[1832.08 → 1833.22] there's no
[1833.22 → 1834.54] QuickBooks or FreshBooks
[1834.54 → 1835.74] kind of proprietary
[1835.74 → 1837.28] license required
[1837.28 → 1838.34] and that's a huge
[1838.34 → 1838.96] thing for me
[1838.96 → 1839.82] given I just do this
[1839.82 → 1840.28] as a
[1840.28 → 1840.62] you know
[1840.62 → 1841.98] spare time thing
[1841.98 → 1842.76] so yeah
[1842.76 → 1843.02] I think
[1843.02 → 1844.28] CSV seems to be
[1844.28 → 1844.64] pretty good
[1844.64 → 1845.42] I haven't
[1845.42 → 1846.40] actually done
[1846.40 → 1846.96] anything with
[1846.96 → 1848.04] importing though
[1848.04 → 1849.52] Well I have
[1849.52 → 1850.04] another question
[1850.04 → 1850.46] for you
[1850.46 → 1851.60] I overheard
[1851.60 → 1852.02] when I was
[1852.02 → 1852.74] at your place
[1852.74 → 1853.14] last
[1853.14 → 1854.18] that your
[1854.18 → 1855.20] wife Catherine
[1855.20 → 1855.94] has been using
[1855.94 → 1856.48] it as well
[1856.48 → 1857.00] did you get
[1857.00 → 1857.50] any feedback
[1857.50 → 1858.46] from her
[1858.46 → 1859.04] using it
[1859.04 → 1860.02] in her business?
[1860.72 → 1861.12] Yeah I think
[1861.12 → 1861.60] it's massive
[1861.60 → 1862.12] overkill
[1862.12 → 1863.14] for just invoicing
[1863.14 → 1863.70] a little music
[1863.70 → 1864.20] students
[1864.20 → 1865.18] parents
[1865.18 → 1866.92] but
[1866.92 → 1868.18] she likes it
[1868.18 → 1868.34] I mean
[1868.34 → 1868.82] she has her
[1868.82 → 1869.26] own login
[1869.26 → 1869.94] she know
[1869.94 → 1870.98] has a shortcut
[1870.98 → 1871.66] on her
[1871.66 → 1872.30] browsers
[1872.30 → 1872.90] bookmarks
[1872.90 → 1874.32] she just logs
[1874.32 → 1874.78] in and just
[1874.78 → 1875.36] does the thing
[1875.36 → 1876.50] and like I do
[1876.50 → 1877.00] once a month
[1877.00 → 1877.38] I guess
[1877.38 → 1877.76] and just
[1877.76 → 1878.54] sends the invoice
[1878.54 → 1879.04] out and
[1879.04 → 1880.54] it's all good
[1880.54 → 1882.10] I've just found
[1882.10 → 1882.90] the import data
[1882.90 → 1883.58] pane by the way
[1883.58 → 1884.20] and it supports
[1884.20 → 1885.26] a huge number
[1885.26 → 1886.14] of different
[1886.14 → 1886.84] formats
[1886.84 → 1887.10] you've got
[1887.10 → 1887.52] CSV
[1887.52 → 1888.08] JSON
[1888.08 → 1888.96] FreshBooks
[1888.96 → 1890.18] blah blah blah
[1890.18 → 1891.16] invoice plane
[1891.16 → 1891.80] is one of them
[1891.80 → 1892.56] I would just say
[1892.56 → 1893.44] there's about
[1893.44 → 1894.52] 10 or 12
[1894.52 → 1895.28] different options
[1895.28 → 1896.18] for importing
[1896.18 → 1897.00] and exporting
[1897.00 → 1898.38] is CSV
[1898.38 → 1898.94] XLS
[1898.94 → 1899.58] or JSON
[1899.58 → 1900.26] sounds like
[1900.26 → 1900.56] you've got
[1900.56 → 1900.98] me hooked
[1900.98 → 1901.36] yeah there's
[1901.36 → 1901.84] no downside
[1901.84 → 1902.54] I can see
[1902.54 → 1902.98] next
[1902.98 → 1903.76] yeah and even
[1903.76 → 1904.38] if you try it
[1904.38 → 1904.62] and you don't
[1904.62 → 1904.92] like it
[1904.92 → 1905.36] it sounds like
[1905.36 → 1905.76] there's
[1905.76 → 1906.28] it's pretty easy
[1906.28 → 1906.74] to get out
[1906.74 → 1907.74] so it's no
[1907.74 → 1908.48] real downside
[1908.48 → 1909.08] to trying it
[1909.08 → 1910.76] I know a lot
[1910.76 → 1911.00] of people
[1911.00 → 1911.60] listening to
[1911.60 → 1911.98] this show
[1911.98 → 1912.94] probably love
[1912.94 → 1913.66] their YubiKey
[1913.66 → 1914.64] I've heard
[1914.64 → 1915.12] from some of
[1915.12 → 1915.28] them
[1915.28 → 1916.16] and it sounds
[1916.16 → 1917.18] like Cloudflare
[1917.18 → 1918.06] is going to
[1918.06 → 1918.94] work with
[1918.94 → 1919.54] YubiKey
[1919.54 → 1920.04] I really
[1920.04 → 1921.14] I mean I
[1921.14 → 1921.40] didn't know
[1921.40 → 1921.94] they didn't
[1921.94 → 1922.58] tell us all
[1922.58 → 1923.02] about this
[1923.02 → 1923.50] one Alex
[1923.50 → 1925.22] well the first
[1925.22 → 1925.70] thing about
[1925.70 → 1926.40] YubiKey
[1926.40 → 1927.52] we should explain
[1927.52 → 1927.96] what they are
[1927.96 → 1928.76] for those that
[1928.76 → 1929.28] don't know
[1929.28 → 1930.10] they're a
[1930.10 → 1930.52] hardware
[1930.52 → 1931.12] two-factor
[1931.12 → 1931.60] authentication
[1931.60 → 1932.24] token
[1932.24 → 1932.82] so essentially
[1932.82 → 1933.16] what that
[1933.16 → 1933.60] means is
[1933.60 → 1934.08] whenever you
[1934.08 → 1934.64] log into
[1934.64 → 1935.54] a specific
[1935.54 → 1937.04] login portal
[1937.04 → 1937.58] website
[1937.58 → 1938.46] piece of
[1938.46 → 1938.68] software
[1938.68 → 1938.92] whatever
[1938.92 → 1939.38] that needs
[1939.38 → 1939.84] 2FA
[1939.84 → 1941.82] that six-digit
[1941.82 → 1942.42] code or
[1942.42 → 1942.70] whatever
[1942.70 → 1943.64] it could be
[1943.64 → 1944.88] an alphanumeric
[1944.88 → 1945.28] string
[1945.28 → 1946.10] in the case
[1946.10 → 1946.72] of a YubiKey
[1946.72 → 1947.84] you have to
[1947.84 → 1948.84] physically plug
[1948.84 → 1949.42] in a USB
[1949.42 → 1950.18] device into
[1950.18 → 1950.76] your computer
[1950.76 → 1952.02] or your phone
[1952.02 → 1953.06] via NFC
[1953.06 → 1954.44] the two-factor
[1954.44 → 1955.42] piece is stored
[1955.42 → 1956.22] in the hardware
[1956.22 → 1957.24] of the YubiKey
[1957.24 → 1958.62] that has a few
[1958.62 → 1959.06] benefits
[1959.06 → 1960.54] obviously unless
[1960.54 → 1961.04] someone has
[1961.04 → 1961.80] physical access
[1961.80 → 1962.62] to my hardware
[1962.62 → 1963.60] two-factor token
[1963.60 → 1965.12] they can't
[1965.12 → 1965.64] log in
[1965.64 → 1966.74] the downside
[1966.74 → 1967.56] is that includes
[1967.56 → 1968.82] me and
[1968.82 → 1969.90] what I found
[1969.90 → 1971.08] when I got
[1971.08 → 1971.90] a free YubiKey
[1971.90 → 1972.28] back at
[1972.28 → 1972.78] Docker Con
[1972.78 → 1974.90] in 2015
[1974.90 → 1976.66] I think
[1976.66 → 1977.62] because they
[1977.62 → 1977.94] were doing
[1977.94 → 1979.04] some push
[1979.04 → 1979.56] to get people
[1979.56 → 1980.10] to sign
[1980.10 → 1980.74] Docker images
[1980.74 → 1981.26] back then
[1981.26 → 1982.42] so I tried
[1982.42 → 1982.98] it for a while
[1982.98 → 1983.26] because you
[1983.26 → 1983.94] can load SSH
[1983.94 → 1984.60] keys onto this
[1984.60 → 1985.22] thing as well
[1985.22 → 1986.34] secrets can
[1986.34 → 1986.80] include a
[1986.80 → 1987.54] private key
[1987.54 → 1989.42] all that kind
[1989.42 → 1989.70] of stuff
[1989.70 → 1990.60] even your
[1990.60 → 1991.20] Bitwarden
[1991.20 → 1991.66] two-factor
[1991.66 → 1992.10] authentication
[1992.10 → 1992.94] token can
[1992.94 → 1993.56] be stored
[1993.56 → 1994.54] and set up
[1994.54 → 1994.94] to work
[1994.94 → 1995.60] with a YubiKey
[1995.60 → 1997.00] the trouble
[1997.00 → 1998.76] is my
[1998.76 → 1999.26] YubiKey is
[1999.26 → 1999.66] always at the
[1999.66 → 1999.98] wrong end
[1999.98 → 2000.52] of the house
[2000.52 → 2001.60] it's always
[2001.60 → 2001.98] at the opposite
[2001.98 → 2002.38] end of the
[2002.38 → 2002.72] house from
[2002.72 → 2003.36] where I am
[2003.36 → 2004.18] and so whenever
[2004.18 → 2004.60] I want to
[2004.60 → 2005.02] log into
[2005.02 → 2005.66] something
[2005.66 → 2006.40] I'm like
[2006.40 → 2006.84] damn it
[2006.84 → 2007.44] I have to
[2007.44 → 2008.10] run from
[2008.10 → 2008.36] one end
[2008.36 → 2008.62] of the house
[2008.62 → 2009.04] to the other
[2009.04 → 2010.14] or just have
[2010.14 → 2010.80] multiple
[2010.80 → 2011.66] YubiKey
[2011.66 → 2012.70] I feel like
[2012.70 → 2012.96] there's some
[2012.96 → 2013.58] universal law
[2013.58 → 2014.36] about two-factor
[2014.36 → 2015.24] and the device
[2015.24 → 2015.66] you're using
[2015.66 → 2016.28] is always at
[2016.28 → 2016.60] the other end
[2016.60 → 2017.04] of the house
[2017.04 → 2018.00] yeah that's
[2018.00 → 2018.32] true
[2018.32 → 2019.18] I remember
[2019.18 → 2019.64] our friend
[2019.64 → 2020.56] Noah wears it
[2020.56 → 2021.16] around his neck
[2021.16 → 2021.68] for that very
[2021.68 → 2022.02] reason
[2022.02 → 2022.92] I mean so
[2022.92 → 2023.56] it's not to say
[2023.56 → 2024.14] that they're not
[2024.14 → 2024.68] good because
[2024.68 → 2025.50] they're incredibly
[2025.50 → 2026.78] useful in the
[2026.78 → 2027.74] workplace for
[2027.74 → 2028.40] example you want
[2028.40 → 2029.08] to give someone
[2029.08 → 2030.40] access to some
[2030.40 → 2031.26] privileged secrets
[2031.26 → 2032.56] you give them
[2032.56 → 2033.44] this hardware token
[2033.44 → 2034.36] and at work
[2034.36 → 2035.54] typically that's
[2035.54 → 2036.22] you know the
[2036.22 → 2037.46] most common use
[2037.46 → 2038.14] case for it I
[2038.14 → 2038.56] would say
[2038.56 → 2039.72] and so what
[2039.72 → 2040.52] Cloudflare are doing
[2040.52 → 2041.14] is they're running
[2041.14 → 2041.66] a promotion
[2041.66 → 2043.32] with YubiKey
[2043.32 → 2045.18] to provide
[2045.18 → 2046.06] these security
[2046.06 → 2046.94] keys at
[2046.94 → 2047.82] air quotes
[2047.82 → 2048.84] good for the
[2048.84 → 2049.44] internet
[2049.44 → 2050.38] end quotes
[2050.38 → 2050.96] pricing
[2050.96 → 2052.72] and they start
[2052.72 → 2053.42] as low as
[2053.42 → 2054.14] ten dollars
[2054.14 → 2054.96] per YubiKey
[2054.96 → 2055.52] now typically
[2055.52 → 2056.12] these things
[2056.12 → 2056.66] are thirty
[2056.66 → 2057.92] forty plus
[2057.92 → 2058.52] each
[2058.52 → 2060.18] so actually
[2060.18 → 2060.68] that could be
[2060.68 → 2061.50] a huge boon
[2061.50 → 2062.00] if you've been
[2062.00 → 2062.56] looking to get
[2062.56 → 2063.20] involved with
[2063.20 → 2063.80] the Cubic
[2063.80 → 2064.80] YubiKey stuff
[2064.80 → 2066.46] sign up to
[2066.46 → 2067.62] this offer
[2067.62 → 2068.22] that's in the
[2068.22 → 2068.62] show notes
[2068.62 → 2069.28] with Cloudflare
[2069.28 → 2069.96] it's not sponsored
[2069.96 → 2070.46] or affiliated
[2070.46 → 2071.32] it's just a
[2071.32 → 2072.62] Cloudflare thing
[2072.62 → 2074.08] and get yourself
[2074.08 → 2074.84] a cheap YubiKey
[2074.84 → 2076.46] good for the
[2076.46 → 2077.24] internet pricing
[2077.24 → 2078.10] is adorable
[2078.10 → 2078.66] I know
[2078.66 → 2080.60] I thought we're
[2080.60 → 2081.16] supposed to hate
[2081.16 → 2081.78] Cloudflare
[2081.78 → 2082.50] but I can't help
[2082.50 → 2082.96] but think this
[2082.96 → 2083.64] is a good idea
[2083.64 → 2084.66] this is truly
[2084.66 → 2085.16] good for the
[2085.16 → 2085.66] security of the
[2085.66 → 2085.94] internet
[2085.94 → 2087.24] you know Chris
[2087.24 → 2088.00] I did find a
[2088.00 → 2088.78] YubiKey in your
[2088.78 → 2089.82] closet one time
[2089.82 → 2090.48] I think the last
[2090.48 → 2091.14] time I was here
[2091.14 → 2093.28] Brent you're
[2093.28 → 2093.68] going through my
[2093.68 → 2094.04] closet
[2094.04 → 2094.78] no, no I just
[2094.78 → 2096.68] well we'll talk
[2096.68 → 2097.20] about it later
[2097.20 → 2100.00] you know there
[2100.00 → 2100.42] used to be lots
[2100.42 → 2101.08] of reasons not
[2101.08 → 2101.80] to use YubiKey
[2101.80 → 2103.60] laziness being
[2103.60 → 2103.94] at the wrong
[2103.94 → 2104.22] end of the
[2104.22 → 2104.74] house is one
[2104.74 → 2105.04] of them
[2105.04 → 2106.30] but they didn't
[2106.30 → 2106.86] used to make a
[2106.86 → 2107.88] USB-C specific
[2107.88 → 2108.90] one that was
[2108.90 → 2109.72] low profile for
[2109.72 → 2110.36] like MacBooks
[2110.36 → 2110.74] and stuff
[2110.74 → 2111.54] they fixed that
[2111.54 → 2112.44] that's now a
[2112.44 → 2113.12] low profile one
[2113.12 → 2114.36] for MacBooks
[2114.36 → 2115.38] they didn't
[2115.38 → 2115.90] used to work
[2115.90 → 2116.80] on mobile
[2116.80 → 2117.58] devices but
[2117.58 → 2118.20] they now do
[2118.20 → 2119.18] through NFC
[2119.18 → 2121.18] so really
[2121.18 → 2122.12] there's no real
[2122.12 → 2122.82] reason if you're
[2122.82 → 2123.74] curious not to
[2123.74 → 2124.48] try one at a
[2124.48 → 2125.58] $10 entry price
[2125.58 → 2126.70] that is a
[2126.70 → 2127.00] perfect
[2127.00 → 2127.86] point I've
[2127.86 → 2128.54] I've looked at
[2128.54 → 2130.10] these keys many
[2130.10 → 2131.00] times both the
[2131.00 → 2131.56] YubiKey and
[2131.56 → 2132.50] alternatives and
[2132.50 → 2133.04] I've always
[2133.04 → 2134.22] hesitated to pull
[2134.22 → 2135.64] the trigger an on
[2135.64 → 2136.24] price because
[2136.24 → 2137.06] actually you kind of
[2137.06 → 2137.74] need two of them
[2137.74 → 2139.04] one is your main
[2139.04 → 2139.82] one is the backup
[2139.82 → 2141.34] but the other
[2141.34 → 2142.08] reason was always
[2142.08 → 2142.88] that I couldn't
[2142.88 → 2143.78] quite figure out
[2143.78 → 2144.40] all the
[2144.40 → 2145.20] different features
[2145.20 → 2145.98] and you know
[2145.98 → 2146.76] which is it
[2146.76 → 2147.50] FIDO that I
[2147.50 → 2148.28] need to support
[2148.28 → 2148.92] everything it's
[2148.92 → 2149.50] like it seemed
[2149.50 → 2151.60] like 12 websites
[2151.60 → 2152.36] use this one
[2152.36 → 2153.46] proprietary way of
[2153.46 → 2154.14] doing it and
[2154.14 → 2154.82] the other 12
[2154.82 → 2155.48] use this other
[2155.48 → 2156.12] method, so I
[2156.12 → 2156.88] always got lost
[2156.88 → 2157.84] in all of those
[2157.84 → 2158.68] details and
[2158.68 → 2159.58] complexity and I
[2159.58 → 2160.70] hope that maybe
[2160.70 → 2162.06] that's been solved
[2162.06 → 2162.70] recently do you
[2162.70 → 2163.62] have any sense of
[2163.62 → 2164.32] whether they're
[2164.32 → 2165.26] easier these days
[2165.26 → 2165.64] than they were
[2165.64 → 2166.34] maybe five years
[2166.34 → 2167.06] ago I think
[2167.06 → 2167.38] they're more
[2167.38 → 2168.40] mature and they
[2168.40 → 2169.12] support a lot
[2169.12 → 2169.88] more stuff than
[2169.88 → 2170.78] they used to I
[2170.78 → 2171.20] don't know whether
[2171.20 → 2171.86] that makes it
[2171.86 → 2173.02] simpler or more
[2173.02 → 2173.84] approachable though
[2173.84 → 2174.96] if anything it
[2174.96 → 2175.60] makes it worse
[2175.60 → 2176.02] because there's
[2176.02 → 2176.66] more options
[2176.66 → 2178.12] that's why I
[2178.12 → 2178.50] kind of debate
[2178.50 → 2179.18] like maybe the
[2179.18 → 2179.78] maybe the sweet
[2179.78 → 2180.40] spot is like an
[2180.40 → 2181.26] authenticator app on
[2181.26 → 2182.78] your phone but I
[2182.78 → 2184.12] do kind of I
[2184.12 → 2184.96] love that idea of
[2184.96 → 2185.56] you plug in a
[2185.56 → 2186.30] hardware device
[2186.30 → 2187.38] that does something
[2187.38 → 2188.32] feels like you'd
[2188.32 → 2188.68] really want to
[2188.68 → 2189.86] combine a two
[2189.86 → 2190.96] factor code on
[2190.96 → 2192.28] authentication app
[2192.28 → 2193.16] with a hardware
[2193.16 → 2194.40] device with a
[2194.40 → 2195.30] password potentially
[2195.30 → 2197.08] or as a backup
[2197.08 → 2197.56] you know when
[2197.56 → 2198.66] places do SMS
[2198.66 → 2199.40] phishing attacks
[2199.40 → 2200.04] and stuff that's
[2200.04 → 2200.50] one of the most
[2200.50 → 2201.20] common attack
[2201.20 → 2202.92] vectors is people
[2202.92 → 2203.98] steal your SMS
[2203.98 → 2206.08] access send a
[2206.08 → 2206.92] two-factor code
[2206.92 → 2208.02] there whilst they
[2208.02 → 2208.80] have the temporary
[2208.80 → 2210.08] access before you
[2210.08 → 2211.66] notice and this
[2211.66 → 2212.34] would completely
[2212.34 → 2213.40] negate that as an
[2213.40 → 2214.00] attack vector
[2214.00 → 2215.02] but only if
[2215.02 → 2215.42] supported
[2215.42 → 2216.90] only if supported
[2216.90 → 2217.92] this takes me
[2217.92 → 2219.44] back to a few
[2219.44 → 2220.26] years ago where
[2220.26 → 2221.24] the company I
[2221.24 → 2221.88] worked at used
[2221.88 → 2223.10] YubiKey and
[2223.10 → 2224.56] in Slack multiple
[2224.56 → 2225.30] times a day
[2225.30 → 2225.96] different people
[2225.96 → 2226.94] accidentally touch
[2226.94 → 2227.78] their YubiKey
[2227.78 → 2228.66] and put in
[2228.66 → 2230.54] their 40
[2230.54 → 2231.40] character long
[2231.40 → 2232.76] string
[2232.76 → 2235.10] most of the
[2235.10 → 2235.44] days
[2235.44 → 2237.14] yeah I have
[2237.14 → 2237.82] seen that I
[2237.82 → 2238.24] see that in our
[2238.24 → 2239.04] chat room sometimes
[2239.04 → 2239.30] too
[2239.30 → 2240.34] I did it one
[2240.34 → 2240.64] time
[2240.64 → 2241.92] and Alex
[2241.92 → 2242.86] you've sent
[2242.86 → 2243.34] some of your
[2243.34 → 2244.56] passwords to
[2244.56 → 2245.24] GitHub if I
[2245.24 → 2245.84] remember correctly
[2245.84 → 2246.50] oh well that's
[2246.50 → 2247.08] that's different
[2247.08 → 2247.66] that's just me
[2247.66 → 2248.46] being an
[2248.46 → 2249.74] idiot, but that's
[2249.74 → 2250.12] different
[2250.12 → 2250.82] what's the
[2250.82 → 2251.20] difference
[2251.20 → 2252.16] well these
[2252.16 → 2253.04] strings aren't
[2253.04 → 2253.76] useful on their
[2253.76 → 2254.24] own because
[2254.24 → 2254.74] they're attached
[2254.74 → 2255.32] to a specific
[2255.32 → 2256.28] service and
[2256.28 → 2256.80] they're time
[2256.80 → 2257.46] limited and all
[2257.46 → 2257.90] that kind of
[2257.90 → 2259.08] stuff so if
[2259.08 → 2259.72] you happen to
[2259.72 → 2260.58] know exactly
[2260.58 → 2261.28] what service I'm
[2261.28 → 2262.04] logging into at
[2262.04 → 2262.54] that specific
[2262.54 → 2263.40] moment in history
[2263.40 → 2265.14] maybe it's useful
[2265.14 → 2265.84] for about the
[2265.84 → 2267.10] next 25 seconds
[2267.10 → 2268.36] but otherwise it's
[2268.36 → 2269.70] useless well I
[2269.70 → 2270.24] want to talk about
[2270.24 → 2270.92] something you came
[2270.92 → 2272.50] across that really
[2272.50 → 2273.38] piques my interest
[2273.38 → 2274.50] because I'm often
[2274.50 → 2275.60] using Reddit as a
[2275.60 → 2276.24] way to discover
[2276.24 → 2277.18] topics that seem
[2277.18 → 2277.70] like might be
[2277.70 → 2278.48] worth discussion
[2278.48 → 2279.52] and you found
[2279.52 → 2280.16] essentially an
[2280.16 → 2281.24] automatic archiver
[2281.24 → 2282.14] for Reddit I
[2282.14 → 2282.60] did I haven't
[2282.60 → 2283.40] actually tried it
[2283.40 → 2284.16] out yet but
[2284.16 → 2285.12] there's a piece of
[2285.12 → 2285.58] software in the
[2285.58 → 2286.50] show notes linked
[2286.50 → 2289.12] called expanse and
[2289.12 → 2290.64] this builds itself as
[2290.64 → 2291.88] a fully self-hosted
[2291.88 → 2292.96] multi-user web app
[2292.96 → 2294.34] which allows you to
[2294.34 → 2295.42] externally store
[2295.42 → 2296.44] Reddit items such
[2296.44 → 2297.12] as things you've
[2297.12 → 2298.02] saved created
[2298.02 → 2299.36] upvoted downvoted
[2299.36 → 2300.90] and hidden and
[2300.90 → 2301.84] this bypasses
[2301.84 → 2303.00] Reddit's 1000
[2303.00 → 2305.04] item listing limit
[2305.04 → 2305.58] which I didn't
[2305.58 → 2306.22] know was a limit
[2306.22 → 2307.14] and so essentially
[2307.14 → 2307.62] there's a quick
[2307.62 → 2308.96] demo in the
[2308.96 → 2310.04] GitHub repo
[2310.04 → 2310.82] short YouTube
[2310.82 → 2312.44] video and that
[2312.44 → 2312.86] was enough to
[2312.86 → 2313.28] sell me I'm
[2313.28 → 2313.74] hooked so we'll
[2313.74 → 2314.38] set this up the
[2314.38 → 2315.24] the earliest opportunity
[2315.24 → 2317.04] same what the
[2317.04 → 2317.44] video really
[2317.44 → 2318.48] demonstrates is it
[2318.48 → 2319.26] creates like a
[2319.26 → 2320.20] mirrored environment
[2320.20 → 2321.48] of Reddit so you
[2321.48 → 2322.16] kind of create some
[2322.16 → 2322.52] of the same
[2322.52 → 2324.12] categories of saved
[2324.12 → 2325.38] post upvoted post
[2325.38 → 2326.30] downvoted submitted
[2326.30 → 2327.62] commented you know
[2327.62 → 2328.42] that same kind of
[2328.42 → 2328.96] thing you get from
[2328.96 → 2329.58] your Reddit history
[2329.58 → 2330.50] it mirrors that
[2330.50 → 2331.76] UI in a cleaner
[2331.76 → 2333.28] way and just
[2333.28 → 2333.90] presents all that
[2333.90 → 2334.96] information to you
[2334.96 → 2335.68] and it just
[2335.68 → 2336.78] continues to just
[2336.78 → 2337.82] suck that information
[2337.82 → 2338.74] into your own local
[2338.74 → 2340.24] instance as you use
[2340.24 → 2340.78] Reddit like you
[2340.78 → 2341.86] normally might you
[2341.86 → 2342.34] don't have to do
[2342.34 → 2343.02] anything special
[2343.02 → 2344.04] pretty much like
[2344.04 → 2345.20] pocket for Reddit
[2345.20 → 2346.54] yeah like if
[2346.54 → 2347.72] like if everything
[2347.72 → 2348.44] you read just
[2348.44 → 2349.18] automatically went to
[2349.18 → 2349.92] pocket or something
[2349.92 → 2350.34] because it's
[2350.34 → 2350.96] everything you do on
[2350.96 → 2351.26] Reddit just
[2351.26 → 2351.84] automatically gets
[2351.84 → 2352.50] backed up to this
[2352.50 → 2353.72] thing it's kind of
[2353.72 → 2354.60] brilliant I wish I
[2354.60 → 2355.64] had that for all the
[2355.64 → 2356.50] services yeah can we
[2356.50 → 2357.10] get that for hacker
[2357.10 → 2358.52] news yeah and
[2358.52 → 2359.92] twitter and anything
[2359.92 → 2361.12] that's really like all
[2361.12 → 2362.60] the services for
[2362.60 → 2363.92] everything have you
[2363.92 → 2364.70] heard of RSS
[2364.70 → 2371.32] I see you found out
[2371.32 → 2372.60] that Bitwarden has
[2372.60 → 2373.76] integrated fast mail
[2373.76 → 2375.26] email aliasing so
[2375.26 → 2376.68] that way when you sign
[2376.68 → 2378.08] up now you can
[2378.08 → 2380.02] generate a fast mail
[2380.02 → 2382.50] unique email address for
[2382.50 → 2384.64] a service how great
[2384.64 → 2386.02] is this well this is
[2386.02 → 2387.76] amazing you know that
[2387.76 → 2389.12] google supports the
[2389.12 → 2391.74] plus delimiter in their
[2391.74 → 2392.68] email addresses so you
[2392.68 → 2395.42] can say Alex kHz plus
[2395.42 → 2398.06] twitter at Gmail or
[2398.06 → 2400.18] whatever, and it will
[2400.18 → 2402.58] send every email that
[2402.58 → 2404.50] twitter has to that
[2404.50 → 2406.16] specific email address
[2406.16 → 2408.18] the trouble is it relies
[2408.18 → 2410.18] on the service that's in
[2410.18 → 2411.32] question twitter or
[2411.32 → 2413.40] whoever to respect that
[2413.40 → 2414.96] and then also when they
[2414.96 → 2416.04] sell that information to
[2416.04 → 2417.14] third parties at what
[2417.14 → 2419.12] whatever point Elon decides
[2419.12 → 2419.88] to in the future
[2419.88 → 2422.50] they've also got to
[2422.50 → 2423.68] include that plus in
[2423.68 → 2424.58] there because everybody
[2424.58 → 2426.70] knows that plus is just a
[2426.70 → 2428.00] delimiter and so the
[2428.00 → 2429.20] real email address is just
[2429.20 → 2430.28] a bit before the plus
[2430.28 → 2432.44] what this fast mail
[2432.44 → 2433.54] integration allows me to
[2433.54 → 2435.50] do is set up a genuine
[2435.50 → 2439.48] email alias so you know
[2439.48 → 2440.82] it becomes two or three
[2440.82 → 2442.12] random words and a couple
[2442.12 → 2443.80] of random numbers instead
[2443.80 → 2445.46] of my actual email address
[2445.46 → 2449.32] being semi obfuscated and
[2449.32 → 2451.28] it's built directly into the
[2451.28 → 2453.54] bit warden clients so they
[2453.54 → 2454.78] have that generate password
[2454.78 → 2456.12] feature if you look
[2456.12 → 2457.24] at the checkbox the next one
[2457.24 → 2459.12] down there's now a generated
[2459.12 → 2460.74] username box which we've
[2460.74 → 2462.44] talked about before but if
[2462.44 → 2463.16] you look just a little bit
[2463.16 → 2464.68] further down than that there
[2464.68 → 2465.68] is a there's three or four
[2465.68 → 2467.24] services in there and one of
[2467.24 → 2469.52] them is now fast mail and
[2469.52 → 2471.88] so just by creating or
[2471.88 → 2473.32] generating an email address
[2473.32 → 2475.14] alias in the bit warden
[2475.14 → 2477.06] client it will go and talk
[2477.06 → 2478.62] to the fast mail API create
[2478.62 → 2480.20] the email alias and then
[2480.20 → 2481.30] from that point in history
[2481.30 → 2484.02] you have a bootable email
[2484.02 → 2486.08] address that is not your
[2486.08 → 2488.06] real email address but is the
[2488.06 → 2490.66] alias it's its brilliant you
[2490.66 → 2491.88] know it feels to me like we
[2491.88 → 2494.84] are creating a huge void
[2494.84 → 2496.56] between two worlds we now
[2496.56 → 2497.84] have you know most of us
[2497.84 → 2499.20] hopefully who are well
[2499.20 → 2500.34] educated about passwords
[2500.34 → 2501.94] using password managers you
[2501.94 → 2502.74] know you mentioned Yuri key
[2502.74 → 2504.16] earlier all of these things
[2504.16 → 2504.88] that are really great but
[2504.88 → 2506.78] then I feel like most people
[2506.78 → 2508.42] are just not even anywhere
[2508.42 → 2510.24] close to using a unique email
[2510.24 → 2513.42] address for each service I
[2513.42 → 2514.34] don't I think we need to
[2514.34 → 2515.22] figure out how to bridge that
[2515.22 → 2517.16] gap well the tooling helps you
[2517.16 → 2518.34] know building the tooling to
[2518.34 → 2519.52] do it I think that's what this
[2519.52 → 2520.38] I think that's what this is
[2520.38 → 2521.88] trying to do isn't it mm-hmm
[2521.88 → 2524.44] yeah I think you're right yeah
[2524.44 → 2526.38] okay you win I've been I
[2526.38 → 2527.26] mean this is not a sponsored
[2527.26 → 2528.16] thing I've been trying to get
[2528.16 → 2529.32] Brent on Bitwarden for weeks
[2529.32 → 2532.18] the man loves his uh key pass
[2532.18 → 2534.58] you know what I like about it
[2534.58 → 2536.64] is that um it's worked for the
[2536.64 → 2538.34] last 15 years and I don't need
[2538.34 → 2540.52] to question it and uh, but I've
[2540.52 → 2543.10] been trying to find that key
[2543.10 → 2545.08] reason that will make me switch
[2545.08 → 2548.58] and maybe this is it I think the
[2548.58 → 2549.66] key reason will be when you
[2549.66 → 2552.52] decide it's time uh if I know
[2552.52 → 2554.26] anything about you Brent
[2554.26 → 2555.26] it's that you have to decide
[2555.26 → 2556.30] it's a good idea before you'll
[2556.30 → 2557.56] do something shouldn't that be
[2557.56 → 2559.02] all of us yeah technically
[2559.02 → 2561.62] technically I think it might
[2561.62 → 2562.58] be time for some feedback
[2562.58 → 2563.78] gentlemen what do you think
[2563.78 → 2565.52] bring it on we've been getting
[2565.52 → 2567.74] a lot of various tail scale
[2567.74 → 2569.84] alternatives sent into the show
[2569.84 → 2571.54] and at first I was like okay
[2571.54 → 2573.32] okay but one that's come in a
[2573.32 → 2575.86] couple of times has been net
[2575.86 → 2576.92] bird and I don't know if either
[2576.92 → 2578.08] one of you guys have seen this
[2578.08 → 2579.98] but net bird is trying to check
[2579.98 → 2581.98] all the boxes and I hope the
[2581.98 → 2583.42] tail scale team takes this as a
[2583.42 → 2584.38] compliment because this is
[2584.38 → 2585.92] clearly an indication that
[2585.92 → 2587.00] they're on to something that
[2587.00 → 2588.12] all of these open source
[2588.12 → 2591.56] projects have cropped up um and
[2591.56 → 2592.64] I suppose for a lot of folks
[2592.64 → 2593.78] head scale has not been
[2593.78 → 2596.40] sufficient I guess but the net
[2596.40 → 2598.22] bird folks are attempting to
[2598.22 → 2599.92] get as close as you can to a
[2599.92 → 2602.18] wire guard based mesh network
[2602.18 → 2603.86] they're supporting single sign
[2603.86 → 2604.88] on and multifactor
[2604.88 → 2606.38] authentication like tail scale
[2606.38 → 2607.78] do they have some simple
[2607.78 → 2609.56] controls I don't think they
[2609.56 → 2611.18] have the installation down quite as
[2611.18 → 2612.72] smooth as tail scale does but
[2612.72 → 2615.42] really who would right but you
[2615.42 → 2616.76] get a lot of it you get a lot
[2616.76 → 2619.84] of the advantages um but you
[2619.84 → 2622.94] know it's 100% an uh well it
[2622.94 → 2623.72] doesn't have to be actually
[2623.72 → 2625.04] they're also offering their own
[2625.04 → 2627.14] hosted implementation as well of
[2627.14 → 2628.76] course which then I'm not even
[2628.76 → 2629.70] sure why it's even better than
[2629.70 → 2631.76] tail scale, but they do have a by
[2631.76 → 2633.28] default a host implementation but
[2633.28 → 2634.60] they make it really clear how to
[2634.60 → 2635.94] do all your own self-hosting if
[2635.94 → 2637.76] you like this is why we were all
[2637.76 → 2639.54] so excited about wire guard being
[2639.54 → 2640.78] put in the Linux kernel a few
[2640.78 → 2642.54] years ago it legitimized the
[2642.54 → 2645.42] project, and we hoped at the time
[2645.42 → 2646.36] that it would lead to this
[2646.36 → 2648.90] proliferation of solutions based
[2648.90 → 2651.84] upon it for VPN stuff I'm so
[2651.84 → 2653.22] pleased to see that that's coming
[2653.22 → 2655.52] true aren't you yeah absolutely
[2655.52 → 2657.52] and it looks like you know we're
[2657.52 → 2659.74] going to have a spoil of choices, so I
[2659.74 → 2661.98] I wonder if we'll go through a
[2661.98 → 2663.72] period of some of these sort of
[2663.72 → 2665.34] proving themselves out and tail
[2665.34 → 2666.94] scale will probably be a leader
[2666.94 → 2668.66] for a while because they got a
[2668.66 → 2670.34] huge start they have a commercial
[2670.34 → 2672.12] entity behind them that has some
[2672.12 → 2674.40] money, and they got a good product
[2674.40 → 2675.70] right but so now you're going to see a
[2675.70 → 2679.60] lot of I'd say um, um kind of not
[2679.60 → 2682.16] clones but this kind of what
[2682.16 → 2683.74] they are right, and we're going to have
[2683.74 → 2686.54] to see which one kind of wins out and
[2686.54 → 2687.60] which one ends up being the most
[2687.60 → 2689.00] popular in the community will it be
[2689.00 → 2690.72] tail scale and head scale for those
[2690.72 → 2692.80] that want to self-host or will it be
[2692.80 → 2694.60] something like net bird so if you've
[2694.60 → 2695.78] tried something like this out there
[2695.78 → 2697.50] let us know send us a boost or go to
[2697.50 → 2699.00] self-hosted that show slash contact
[2699.00 → 2701.76] and let us know your thoughts I am
[2701.76 → 2703.42] just so happy with tail scale and now
[2703.42 → 2705.42] that I'm doing subnet routing and all
[2705.42 → 2708.32] of that I'm really I'm really quite
[2708.32 → 2709.78] pleased I don't really see any
[2709.78 → 2712.34] particular reason to switch, and I'm
[2712.34 → 2714.34] also totally comfortable with their
[2714.34 → 2716.30] backplate managing some of the
[2716.30 → 2717.88] authentication and some of the
[2717.88 → 2719.40] connecting that's fine for me
[2719.40 → 2721.28] because I want this to work like a
[2721.28 → 2723.10] rock we talked a little bit about the
[2723.10 → 2725.58] subnet routing at the Airbnb in
[2725.58 → 2727.52] Pasadena with our questionable Wi-Fi
[2727.52 → 2730.86] situation that's generous, and it's
[2730.86 → 2733.42] it's fascinating I use the heck out
[2733.42 → 2735.62] of the subnet routing its amazing oh
[2735.62 → 2738.04] it's so handy especially for devices
[2738.04 → 2741.36] that aren't PCs or Raspberry Pis that
[2741.36 → 2743.44] you something you can't install software
[2743.44 → 2746.84] on like my Victory solar equipment and
[2746.84 → 2748.98] battery equipment I can't install tail
[2748.98 → 2751.10] scale on that it's an appliance but I
[2751.10 → 2752.54] have tail scale on my Raspberry Pi
[2752.54 → 2754.58] that's on the same LAN and I have
[2754.58 → 2756.48] subnet routing on, so now I'm like
[2756.48 → 2758.54] checking the solar when we're at the
[2758.54 → 2760.42] Airbnb making sure Joop's is doing
[2760.42 → 2762.84] okay, and then you know I wanted to
[2762.84 → 2764.74] check the temperatures at the studio so
[2764.74 → 2767.20] I have tail scale installed from hacks
[2767.20 → 2768.84] on home assistant with subnet routing
[2768.84 → 2770.44] turned on, and so I'm checking the
[2770.44 → 2771.96] temperatures in the garage to make
[2771.96 → 2773.70] sure the server is okay, and I'm just
[2773.70 → 2777.00] using local IPs for all of it, and I'm
[2777.00 → 2780.10] pleased to say that I did hope one
[2780.10 → 2782.00] day that this would exist that this
[2782.00 → 2785.00] world would be real and so I preemptively
[2785.00 → 2790.74] set the RV network to a 17216 subnet and
[2790.74 → 2796.22] the studio is a 192 1687 subnet and so
[2796.22 → 2798.26] the two are very different and that has
[2798.26 → 2799.80] made life like so just made it ready to
[2799.80 → 2801.70] go yeah when Brent was here I had to
[2801.70 → 2804.84] completely recharge my retool my cider my
[2804.84 → 2808.02] IP range in the house because there was
[2808.02 → 2809.88] some overlap between my house here and
[2809.88 → 2812.00] my dad's Starlink network because
[2812.00 → 2813.68] remember I moaned in an episode I
[2813.68 → 2816.54] couldn't change the DHCP range, so I had
[2816.54 → 2818.14] to completely retool so that's some good
[2818.14 → 2819.70] foresight from you there Christopher I
[2820.26 → 2822.58] tell you what the old days the old days
[2822.58 → 2824.94] of Opening like an animal building flat
[2824.94 → 2827.40] networks but let us know if you try out
[2827.40 → 2828.80] Net bird I'd be really curious to hear
[2828.80 → 2830.96] how it goes yeah same and I think in a
[2830.96 → 2832.98] future episode we might do a bit
[2832.98 → 2834.54] more of a deep dive into the subnet
[2834.54 → 2836.78] routing that I'm doing and the
[2836.78 → 2838.92] split DNS between different sites
[2838.92 → 2840.04] because I think that'd be of interest
[2840.04 → 2841.94] to folks so if you're interested in
[2841.94 → 2843.30] that let us know at self-hosted dot
[2843.30 → 2846.06] show slash contact I agree having
[2846.06 → 2847.50] chat a little bit about it at the
[2847.50 → 2848.96] Airbnb I think it would be a great
[2848.96 → 2851.10] topic we got some boosts into the show
[2851.10 → 2853.96] too and have boosted in with over 9000
[2853.96 → 2857.50] 9001 SATs, and we also got 1024 SATs
[2857.50 → 2859.72] from Amar who's having some trouble
[2859.72 → 2861.94] getting their audio whole home audio
[2861.94 → 2863.40] working, so these are a whole
[2863.40 → 2865.18] home audio boost that I wanted to follow
[2865.18 → 2867.14] up on so we'll start with Nev and he
[2867.14 → 2869.64] writes whole home audio as a concept
[2869.64 → 2873.96] has existed as long as human history so
[2873.96 → 2875.64] there are plenty of solutions moving
[2875.64 → 2877.82] around rather than getting fancy with
[2877.82 → 2880.60] software I might present an alternative
[2880.60 → 2883.88] he writes pulse audios network streaming
[2883.88 → 2888.56] and Cody now why Cody because Cody has a
[2888.56 → 2890.80] rich app ecosystem for remote controls
[2890.80 → 2893.78] and a web GUI plus it supports Plex Jellyfin
[2893.78 → 2896.94] MB and even air cast this solution I have
[2896.94 → 2899.78] been using for years now I would never
[2899.78 → 2902.62] have thought of Cody would you know and I
[2902.62 → 2905.06] think it's probably worth a mention because
[2905.06 → 2906.70] a lot of people love Cody that listen to
[2906.70 → 2910.32] the show and pulse audio network streaming
[2910.32 → 2912.54] has been around for years and I never
[2912.54 → 2914.72] think to mention it, but I constantly hear
[2914.72 → 2916.16] feedback from the audience that it works
[2916.16 → 2918.66] pretty well just anything with pulse audio
[2918.66 → 2922.84] gives me PTSD I think rustic has to
[2922.84 → 2925.08] verse a boosted with 2000 SATs and he
[2925.08 → 2926.60] echoed a sentiment we heard from multiple
[2926.60 → 2929.24] people out there what about volume or
[2929.24 → 2932.94] volume sorry I'm butchering that but it
[2932.94 → 2936.08] acts as an airplay Chromecast endpoint he
[2936.08 → 2937.74] says if you want a lot of them synced you'd
[2937.74 → 2939.74] have to pay, but it's a good project so it's
[2939.74 → 2941.26] worth paying for I had a couple of
[2941.26 → 2943.70] recommendations for volume actually the
[2943.70 → 2945.20] pricing doesn't put me off too much I
[2945.20 → 2946.90] don't mind necessarily paying for the
[2946.90 → 2949.28] right solution I mean the alternative
[2949.28 → 2951.78] would be just giving up and going for a
[2951.78 → 2954.18] Sonos based deployment right and that
[2954.18 → 2957.02] that ain't going to be free is it so the
[2957.02 → 2958.98] other thing that came in as a
[2958.98 → 2960.90] recommendation was there's a chap on
[2960.90 → 2963.34] YouTube called Dark that does he's got
[2963.34 → 2964.88] beautiful production quality on his
[2964.88 → 2970.54] videos he is a hi-fi audiophile nerd and
[2970.54 → 2972.52] he talks occasionally about how he
[2972.52 → 2974.86] streams music around his house one of
[2974.86 → 2976.24] the recommendations I had come in was
[2976.24 → 2978.06] something called Rune Audio it's not
[2978.06 → 2980.66] open source I don't think, and it is paid
[2980.66 → 2983.18] it does cost quite a bit per month but
[2983.18 → 2985.50] you know this will support along with
[2985.50 → 2989.08] volume multiple rooms based off a
[2989.08 → 2991.12] Raspberry Pi and that kind of thing I'm
[2991.12 → 2993.46] still stuck though on how to actually
[2993.46 → 2996.04] automate the speaker component the
[2996.04 → 2997.68] Raspberry Pi bit I think is actually
[2997.68 → 2999.44] the easy bit I mean there's a few
[2999.44 → 3000.90] options you know snap cast is another
[3000.90 → 3004.82] one out there it's just controlling the
[3004.82 → 3006.36] speaker component that's the tricky
[3006.36 → 3009.46] bit the broad link infrared emitter
[3009.46 → 3011.06] blaster that I talked about in the last
[3011.06 → 3014.54] episode sort of kind of is behaving
[3014.54 → 3017.40] itself, but I've ordered the components
[3017.40 → 3019.46] to build myself a blaster based off an
[3019.46 → 3021.64] ESP device as well see if that's any
[3021.64 → 3023.18] better than the broad link stuff because
[3023.18 → 3025.30] it's not it's just not reliable enough
[3025.30 → 3027.54] yeah, thanks for the recommendation I'll
[3027.54 → 3030.16] take a look at volume a bit more
[3030.16 → 3031.70] seriously over the next few weeks
[3031.70 → 3033.60] when I'm not travelling to LA it's a
[3033.60 → 3034.42] shame to hear you're having some
[3034.42 → 3036.04] trouble with the IR blaster because when
[3036.04 → 3037.34] you're doing the music stuff and you
[3037.34 → 3038.70] just you just want to hit a button and
[3038.70 → 3040.10] have it go you know you want it to be a
[3040.10 → 3041.66] really kind of chill experience that's
[3041.66 → 3043.84] not it's not when you want to do the
[3043.84 → 3045.52] troubleshooting it seems to me like
[3045.52 → 3046.90] the intersection of two very different
[3046.90 → 3049.96] worlds you know the hardware button
[3049.96 → 3054.14] audio file grade box that's sitting you
[3054.14 → 3055.44] know next to your TV or your
[3055.44 → 3058.24] entertainment system feels like maybe
[3058.24 → 3060.20] high-end technology of a very different
[3060.20 → 3062.80] era, and you're trying to kind of marry
[3062.80 → 3065.02] the two, so I understand there's clearly
[3065.02 → 3067.24] some challenge there but wouldn't
[3067.24 → 3069.50] it is great if they just made friends
[3069.50 → 3074.36] quick code wanted to know if anybody has
[3074.36 → 3076.42] any tips on content request systems for
[3076.42 → 3078.06] music you know how there are things out
[3078.06 → 3080.68] there like overseer and other tools for
[3080.68 → 3082.50] like books and stuff like that if
[3082.50 → 3085.72] anybody has suggestions for music send
[3085.72 → 3089.08] them into the show and then drew oof or
[3089.08 → 3093.46] dr oof boosted in with 5,678 SATs and he
[3093.46 → 3096.92] wanted to give a plus one to the zoos Z-Wave
[3096.92 → 3100.12] switches specifically the 700 series thank
[3100.12 → 3102.10] you very much for that detail he says I've
[3102.10 → 3103.26] been through a bunch of different brands
[3103.26 → 3105.44] of smart switches over the years and the
[3105.44 → 3107.76] zoos have been that's z-o-o-o-z have been the
[3107.76 → 3109.76] most reliable affordable and configurable
[3110.52 → 3112.72] to date I'm a network security engineer
[3112.72 → 3115.02] by trade, and I'm an enterprise-grade Wi-Fi
[3115.02 → 3116.64] throughout my house and property four
[3116.64 → 3119.78] different APs and even that can't keep up
[3119.78 → 3122.38] with my smart switches interesting my
[3122.38 → 3124.10] house is long and narrow so it just turns
[3124.10 → 3125.90] out 900 megahertz mesh network works
[3125.90 → 3127.88] better than Wi-Fi thanks for the great
[3127.88 → 3132.70] podcast I do love 900 megahertz I love
[3132.70 → 3137.44] 900 megahertz radio so much I wish we
[3137.44 → 3139.04] could have stayed there mega strike 3
[3139.04 → 3140.74] boosted in with 3,000 SATs hey Chris and
[3140.74 → 3142.64] Alex love the show I picked up an Ikea
[3142.64 → 3145.32] Zigbee light bulb as I begin to build out
[3145.32 → 3147.32] my smart home any recommendations for a
[3147.32 → 3149.84] home assistant Zigbee router currently I'm
[3149.84 → 3152.70] looking at the con be 2 thanks as always
[3152.70 → 3153.70] well he's already got my recommendation
[3154.22 → 3157.84] that con be I used the really cheap
[3157.84 → 3163.34] sewn off one to start with, and it was it
[3163.34 → 3166.20] was not good it was just not good but
[3166.20 → 3169.86] the con be 2 has been my favourite phrase
[3169.86 → 3174.52] rock-solid since I installed it you know
[3174.52 → 3177.16] what though I agree in fact I don't even
[3177.16 → 3178.68] have liked mine hanging off a dongle it's
[3178.68 → 3180.00] just like hooked up right to the back of
[3180.00 → 3182.12] my home assistant blue in the studio and
[3182.12 → 3183.56] I'm talking to devices that are on the
[3183.56 → 3186.78] other end of the house I will also link to
[3186.78 → 3189.56] the Salish Zigbee 3.0 stick that
[3189.56 → 3192.44] cloudfree.shop sells because I would
[3192.44 → 3193.90] imagine if cloud free is selling that
[3193.90 → 3195.76] that's probably a pretty good device but
[3195.76 → 3198.50] I too own the con be 2 USB Zigbee gateway
[3198.50 → 3200.48] and have been very happy with it and
[3200.48 → 3202.52] home assistant just picked it up right
[3202.52 → 3205.38] away so that was really nice don't
[3205.38 → 3207.02] forget we still got a coupon code over
[3207.02 → 3209.12] at cloudfree.shop if you put self-hosted
[3209.12 → 3210.70] in there you'll probably get a dollar off
[3210.70 → 3213.52] whatever you're buying at user 3513
[3213.52 → 3216.74] boosted in with 8,192 SATs I'd love
[3216.74 → 3218.86] to know how Alex is running promo and
[3218.86 → 3221.10] docker on his systems are you running an
[3221.10 → 3224.90] Ubuntu VM on top of promo or containers
[3224.90 → 3226.98] did you use a bare metal Linux and then
[3226.98 → 3228.80] somehow hack the packages to install
[3228.80 → 3233.40] promo onto it tell user 3513 Alex you
[3233.40 → 3235.00] know a bit this question has been coming
[3235.00 → 3238.54] up in discord a lot in the last month or
[3238.54 → 3241.18] so, and it's like something has changed
[3241.18 → 3245.02] and people just need to know
[3245.02 → 3246.84] exactly what I'm doing to copy it which I
[3246.84 → 3249.10] don't understand, but they can't buy pies
[3249.10 → 3250.92] anymore so they're finally giving in a
[3250.92 → 3253.24] buying x86 systems and going promo they
[3253.24 → 3254.96] are very sensible people you know they
[3254.96 → 3257.24] should you know you should
[3257.24 → 3258.56] consider doing that
[3258.56 → 3262.84] perfectmediaserver.com would be where I'd
[3262.84 → 3265.06] send people for actual documentation on
[3265.06 → 3267.52] on what I'm doing I put a new page up
[3267.52 → 3271.42] there in May I think badger stack in
[3271.42 → 3274.48] May just to tell because I was
[3274.48 → 3276.78] getting so many questions what are you
[3276.78 → 3278.16] doing Alex what are you doing, and I'm
[3278.16 → 3279.98] like well okay here it is here's the
[3279.98 → 3281.64] hardware I'm using the exact hardware the
[3281.64 → 3283.98] CPU the OS all that kind of stuff so
[3283.98 → 3286.48] in the original perfect meter server
[3286.48 → 3288.06] guides I used to recommend virtualizing
[3288.56 → 3291.88] Ubuntu and then passing through all of
[3291.88 → 3295.46] the drive controllers to those virtual
[3295.46 → 3298.36] machines that was in the days before I
[3298.36 → 3302.06] was an absolute quick sync snob and if
[3302.06 → 3304.92] you recall in the show a long time ago
[3304.92 → 3308.28] also I've written blog posts about it and
[3308.28 → 3310.94] it's on perfectmediaserver.com I was
[3310.94 → 3313.62] trying to do something called GTG to
[3313.62 → 3318.58] split the quick sync GPU the GPU up
[3318.58 → 3320.34] between multiple virtual machines and
[3320.34 → 3322.10] pass it through and all that kind of
[3322.10 → 3324.30] stuff it just didn't work the
[3324.30 → 3326.22] performance was no good and the
[3326.22 → 3329.34] complexity was off the charts and you
[3329.90 → 3331.90] know how it goes so essentially I
[3331.90 → 3334.12] decided at that point I've got no
[3334.12 → 3336.18] option if I want hardware transcoding
[3336.18 → 3338.72] using quick sync rather than having my
[3338.72 → 3341.02] dual Leon box pull 400 watts I only want
[3341.02 → 3342.42] to pull four watts when I'm doing a
[3342.42 → 3345.68] transcode and who wouldn't want me to've
[3345.68 → 3348.26] got to run Plex on the host and that's
[3348.26 → 3351.34] it that really drove the next wave of my
[3351.34 → 3353.46] builds which I've been doing now for
[3353.46 → 3355.98] about 18 months I would say all of my
[3355.98 → 3357.54] containers run directly on the host
[3357.54 → 3361.22] home assistant itself runs as a has OS VM
[3361.22 → 3363.14] or whatever they call it these days
[3363.14 → 3366.90] that's the only VM I have in Dropbox is
[3366.90 → 3369.10] literally just home assistant it's its a
[3369.10 → 3370.86] bit of a waste I mean occasionally I spin
[3370.86 → 3374.26] up a know an Ubuntu thing for testing
[3374.26 → 3377.34] or a fedora thing or whatever just
[3377.34 → 3379.20] literally for testing but in terms of
[3379.20 → 3381.50] production everything's on the promo
[3381.50 → 3383.38] host it's all done in Ansible in my
[3383.38 → 3384.92] GitHub repo which I'll put a link to in
[3384.92 → 3387.10] the show notes as well, and it's just
[3387.10 → 3388.86] really simple it's just an installation of
[3388.86 → 3391.00] Debian with promo installed on top
[3391.00 → 3393.80] of it I use the promo documentation to
[3393.80 → 3396.48] achieve that there's not much to if it's
[3396.48 → 3400.84] just Linux really it's very boring I think
[3400.84 → 3402.52] that's a good thing I was we were talking
[3402.52 → 3403.66] before we hit record I'm like you know
[3403.66 → 3404.74] there are a lot of things about Linux are
[3404.74 → 3406.42] getting boring, but that's what you need
[3406.42 → 3408.18] when it becomes like this layer in the
[3408.18 → 3411.12] industry it just needs to work so that's
[3411.12 → 3412.98] great, and we'll have a link to Alex's
[3412.98 → 3415.06] high-level overview in the notes
[3415.06 → 3418.72] including some links to also as Alex is
[3418.72 → 3420.60] adding them right now to documentation on
[3420.60 → 3422.38] how to get promo running on Debian 11
[3422.38 → 3426.58] the badger stack the badger stack well it
[3426.58 → 3429.50] can be confusing because promo provide an
[3429.50 → 3431.86] ISO directly so you can install promo
[3431.86 → 3435.12] directly from an ISO just you know from
[3435.12 → 3439.28] the project, or you can install Debian and
[3439.28 → 3440.98] then install promo on top of it and
[3440.98 → 3443.34] that can confuse some people either route
[3443.34 → 3445.20] is completely valid one is slightly more
[3445.20 → 3448.18] hands-on there than the other there's no
[3448.18 → 3449.96] real preference in my mind as to which
[3449.96 → 3452.04] one works better just do whatever makes
[3452.04 → 3454.20] you feel warm and cozy I'm wondering how
[3454.20 → 3456.02] you feel about this next one Alex john a
[3456.02 → 3459.58] boosting with 10,000 sets and he after
[3459.58 → 3462.00] listening to the last episode is soloing
[3462.00 → 3464.80] into setting up his own email server no
[3464.80 → 3467.28] yeah yeah he also is checking out pod verse
[3467.28 → 3469.50] which is awesome new podcast apps and we
[3469.50 → 3472.96] also heard from p4p4john who says I've
[3472.96 → 3474.78] started self-hosting my own email server
[3474.78 → 3476.72] this year I got a business Comcast
[3476.72 → 3479.18] connection with a static IP, and I'm using
[3479.18 → 3481.76] you know host it's going great we're
[3481.76 → 3483.52] somehow when we say I don't know if it's
[3483.52 → 3485.76] a good idea people are like thanks guys
[3485.76 → 3488.60] I'm doing it you guys are crazy I don't
[3488.60 → 3489.88] think it's a good idea to send us a
[3489.88 → 3491.38] million dollars that would be an awful
[3491.38 → 3494.14] idea don't you oh yeah yeah definitely a
[3494.14 → 3499.04] bad idea to know no, so I know I just
[3499.04 → 3500.66] think it's interesting so John you can
[3500.66 → 3502.12] email us from your shiny new
[3502.12 → 3503.82] email server to tell us how it's going
[3503.82 → 3505.52] huh and if we receive it we'll let you
[3505.52 → 3509.98] know right yeah definitely also let me
[3509.98 → 3511.36] know how the pod verse transition goes
[3511.36 → 3512.52] John I'm going to expect a boost from
[3512.52 → 3515.38] pod verse in the future also I just want to
[3515.38 → 3517.38] give a quick shout out we got 5,555
[3518.14 → 3520.52] SATs from soul trust sending in just some
[3520.52 → 3522.00] love for the show just wanted to wish us
[3522.00 → 3524.26] well I thought that was nice and then
[3524.26 → 3527.38] Brent you got this one right schnitzel
[3527.94 → 3530.86] I think it was schnitzel he says that
[3530.86 → 3532.44] he just wants to send us a series of ducks
[3532.44 → 3536.00] Huey Louie and Dewey, and we got 3,000
[3536.00 → 3539.00] SATs from four-legged emu who says he's
[3539.00 → 3542.38] loving calyx on his pixel so we got it I
[3543.16 → 3544.98] switched to graphene, and now I'm hearing
[3544.98 → 3547.28] about calyx constantly I heard you were
[3547.28 → 3549.42] testing graphene so maybe you need to
[3549.42 → 3551.40] switch and text calyx maybe I should just
[3551.40 → 3552.76] go back to the iPhone because this is
[3552.76 → 3555.30] just it's too much it's too much but we
[3555.30 → 3556.74] do love the boost we read all of them we
[3556.74 → 3558.22] only feature some of them on the shows
[3558.22 → 3560.22] now just to keep things tight, but we do
[3560.22 → 3562.28] appreciate everybody who sends one in if
[3562.28 → 3563.46] you'd like to boost the show you can grab
[3563.46 → 3565.44] a new podcasting app new podcast apps
[3565.44 → 3567.24] calm or if you don't want to switch
[3567.24 → 3569.98] podcast apps you can use breeze
[3569.98 → 3573.80] technology and keep your dang podcast app
[3573.80 → 3576.16] I think probably Alby deserves a mention
[3576.16 → 3577.96] as well Alby is a way to do it from the
[3577.96 → 3579.28] web if you don't want to use a mobile
[3579.28 → 3581.64] app at all and the Alby team seems to be
[3581.64 → 3582.84] really solid they're creating some great
[3582.84 → 3585.00] open source code I had a little call with
[3585.00 → 3587.20] one of their co-founders I really like
[3587.20 → 3590.26] where they're going an l b y for that can
[3590.26 → 3592.24] we give a little plug pug to office
[3592.24 → 3596.36] hours dot hair yeah it's something about
[3596.36 → 3598.24] plugs and hair but office hours dot hair
[3598.24 → 3601.10] lucky episode 13 I think it was we
[3601.10 → 3603.08] covered our some of the shenanigans
[3603.08 → 3606.78] on our trip and then in the most recent
[3606.78 → 3609.06] Linux unplugged we covered our JPL trip
[3609.06 → 3611.68] too which how great was the JPL trip
[3611.68 → 3614.90] Alex how was the JPL trip I just can't
[3614.90 → 3617.38] process it did that really happen to us
[3617.38 → 3619.38] like we're just normal people it's not
[3619.38 → 3620.94] like that doesn't happen to normal people
[3620.94 → 3623.48] does if it was so cool and to see
[3623.48 → 3624.98] the clipper to see them working on the
[3624.98 → 3628.54] next mission the Europa Clipper oh so
[3628.54 → 3630.86] cool Chris last night to tuning into
[3630.86 → 3632.74] the live cam that you can get for their
[3632.74 → 3635.98] when you oh cool yeah on YouTube go look
[3635.98 → 3637.50] up the if you look up the Europa Clipper
[3637.50 → 3638.76] stream it's on there I've checked it
[3638.76 → 3640.20] several times, and they've added a lot
[3640.20 → 3642.60] more to it since we saw it wow that's
[3642.60 → 3645.84] that's so cool I'm just so grateful I
[3645.84 → 3647.84] know I put a little clip in Linux unplugged
[3647.84 → 3650.46] for you saying how great the audience is and
[3650.46 → 3653.12] it sounds like a cliché but genuinely I
[3653.12 → 3654.96] think you said it that it's amazing we
[3654.96 → 3656.64] had you know 20 people show up for the
[3656.64 → 3658.78] tour and an about double that for the
[3658.78 → 3662.14] meetup not one person got lost everybody
[3662.14 → 3664.44] was on time everybody was friendly they
[3664.44 → 3666.16] brought stories they brought you know I
[3666.16 → 3669.64] was just like does any other podcast
[3669.64 → 3671.52] network have such an amazing audience I
[3671.52 → 3674.20] don't know but ours is pretty great I
[3674.20 → 3676.32] don't think, so I think how could they
[3676.32 → 3678.96] because we took all the good ones true I
[3678.96 → 3681.92] also learned so much just by chatting
[3681.92 → 3683.26] with people Alex I know you were
[3683.26 → 3684.98] fascinated but basically all night
[3684.98 → 3687.12] because I was kind of hanging around you
[3687.12 → 3688.24] and learning a bunch of stuff but Chris
[3688.24 → 3689.54] you were having a great time, and it was
[3689.54 → 3692.06] almost like 10 p.m. yeah oh we went for
[3692.06 → 3693.96] our meetup went for five hours strong and I
[3693.96 → 3696.32] still didn't get to everybody but let's
[3696.32 → 3699.04] let's be clear here Alex saved the night
[3699.04 → 3702.50] because our guest of the night Tim
[3702.50 → 3706.20] can't him from JPL brought a very
[3706.20 → 3708.40] exclusive little device he brought the
[3708.40 → 3710.22] computer from the Mars copter like that
[3710.22 → 3712.40] you know the earth version the test
[3712.40 → 3714.44] version the prototype version he brought
[3714.44 → 3716.88] that for show-and-tell so we can all see
[3716.88 → 3717.88] like just the parts that we don't
[3717.88 → 3720.08] recognize, and it's a know it's in
[3720.08 → 3722.96] this bag, and it's like secret top or
[3722.96 → 3724.94] it's like private property of NASA and
[3724.94 → 3727.14] JPL like it's, and then it's inside like
[3727.14 → 3729.88] this sealed case even you know, and it was
[3729.88 → 3732.78] like really a big deal and Tim bless his
[3732.78 → 3734.16] heart you know I think with just
[3734.16 → 3736.54] everything going on he got up walked
[3736.54 → 3739.04] away left it on the bench he left it on
[3739.04 → 3741.78] the bench we very nearly had our own
[3741.78 → 3744.28] iPhone 4 moment didn't we very nearly
[3744.28 → 3748.06] yeah you tapped him on the shoulder and
[3748.06 → 3749.48] you're like I think you forgot something
[3749.48 → 3752.54] and I think he was extremely grateful a
[3753.06 → 3754.66] little bit of history right there yeah
[3754.66 → 3757.78] what a lovely guy what a lovely guy yeah
[3757.78 → 3759.36] it was really nice of him to help us
[3759.36 → 3762.44] make all that happen and then to make
[3762.44 → 3764.44] it to the meetup as well and bring a
[3764.44 → 3766.90] little show-and-tell for everybody just
[3766.90 → 3768.48] so cool really a great
[3768.48 → 3769.56] experience something you'll never
[3769.56 → 3771.46] forget you know yeah huge thanks to
[3771.46 → 3773.52] Tim huge thanks to everybody at JB but
[3773.52 → 3775.10] of course thanks to Linde as well for
[3775.10 → 3776.96] enabling us all to go down there and
[3776.96 → 3780.12] take the tour you know yeah absolutely
[3780.12 → 3782.64] they really came through for us and
[3782.64 → 3783.82] you know we had some great swag we got
[3783.82 → 3785.24] to give away swag to people who came to
[3785.24 → 3787.00] JPL and came to all the meetups too and
[3787.00 → 3789.58] Linde gave us an updated shirt for the
[3789.58 → 3791.70] road with the new route on there and all
[3791.70 → 3794.60] that and brighter bolder colours so
[3794.60 → 3796.32] awesome you know we got to meet some
[3796.32 → 3797.50] members while we were down there as
[3797.50 → 3798.82] well so thank you to all the members
[3798.82 → 3799.94] who make this show possible
[3799.94 → 3802.60] self-hosted.show.SRE if you'd like to
[3802.60 → 3804.66] sign up you are our site reliability
[3804.66 → 3806.36] engineers, and you can support all the
[3806.36 → 3807.84] shows if you want to get an ad-free
[3807.84 → 3809.34] version and all their special features
[3809.34 → 3811.78] for the whole network at jupiter. Party
[3811.78 → 3814.48] the very last meetup is on the day that
[3814.48 → 3816.00] this episode airs so if you're a very
[3816.00 → 3817.96] keen listener you've still got time to
[3817.96 → 3820.10] catch Chris in Portland on his way
[3820.10 → 3823.30] back north at 6 p.m pacific time on
[3823.30 → 3825.48] October the 7th yep and if you missed
[3825.48 → 3827.60] us future meetups' meetup.com slash
[3827.60 → 3829.74] Jupiter broadcasting, although I do think
[3829.74 → 3832.02] we've we've done the meetups pretty
[3832.02 → 3834.20] heavily for the last few months I will
[3834.20 → 3835.26] say if you're going to be in Raleigh
[3835.26 → 3837.86] around Halloween at all things open I'm
[3837.86 → 3839.26] going to be in town obviously because I
[3839.26 → 3841.02] live here but so is Cheese Bacon
[3841.02 → 3842.90] longtime friend of the network I think
[3842.90 → 3844.66] system 76 are sending him over to
[3844.66 → 3848.86] Manor booth for the conference so we may
[3848.86 → 3851.98] do an informal meetup keep an eye on the
[3851.98 → 3854.94] matrix rally room, and we'll talk about
[3854.94 → 3856.20] any stuff that's going to happen in
[3856.20 → 3857.60] there mention in the shows too of
[3857.60 → 3859.78] course, but the details will be in the
[3859.78 → 3862.56] matrix room that's going to be fun all
[3862.56 → 3863.78] things open always seems like a good
[3863.78 → 3865.74] one to go to now we do love your
[3865.74 → 3867.24] feedback your questions your topic
[3867.24 → 3869.20] ideas self-hosted show slash contact
[3869.20 → 3870.68] is the place to go to get in touch with
[3870.68 → 3872.50] us and of course you can find me on
[3872.50 → 3874.96] Twitter I'm at Chris LAS and for now
[3874.96 → 3876.98] at least until Elon closes the deal
[3876.98 → 3882.74] finally I'm at ironic badger, and I'm at
[3882.74 → 3884.70] Brent Jervis we might have to revisit
[3884.70 → 3886.42] the whole Twitter topic again soon in
[3886.42 → 3888.76] the meantime there is yes there is a
[3888.76 → 3891.44] also a show account for some reason at
[3891.44 → 3894.86] self-hosted show you can follow it what
[3894.86 → 3896.68] a ringing endorsement that is and
[3896.68 → 3898.40] thanks for listening everybody that was
[3898.40 → 3900.84] self-hosted dot show slash 81
[3900.84 → 3902.84] stress panel
[3902.84 → 3904.38] opposites
[3904.40 → 3907.12] продукции
[3907.12 → 3908.48] Ulm warning
[3908.48 → 3909.24] series
[3909.24 → 3909.44] sell
[3909.44 → 3909.78] civilian
[3909.78 → 3910.54] EU
[3910.54 → 3910.92] 求
[3910.92 → 3911.60] cambia
[3911.60 → 3912.62] util
[3912.62 → 3913.00] unsuccess
[3913.00 → 3913.58] Damon
[3913.58 → 3925.94] 溢
[3925.98 → 3926.50] crises
[3926.50 → 3926.98] וא�
[3926.98 → 3928.00] Esperanto
[3928.00 → 3928.54] mg
[3928.54 → 3928.60] eh
[3928.60 → 3929.20] vote
[3929.20 → 3929.66] Parts
[3929.66 → 3929.68] David
