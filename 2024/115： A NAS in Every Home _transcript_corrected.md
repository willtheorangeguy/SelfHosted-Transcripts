[0.00 → 3.18] Well, your self-hosted podcast is assembled for episode 115.
[3.58 → 4.12] Hey there, Alex.
[4.20 → 5.56] We need a sound effect when we assemble.
[5.92 → 7.48] Yeah, it's like the home lab assemble.
[9.46 → 10.84] Actually, fun story.
[10.92 → 12.66] When we were first spinning up this show,
[12.78 → 15.62] you and I went through all sorts of old computer noises.
[15.76 → 16.10] Do you remember?
[16.28 → 16.44] Yeah.
[16.66 → 19.86] Like hard drives spinning up and old Blackett keyboards typing.
[20.06 → 21.60] Well, we also considered like, you know,
[21.62 → 24.28] the really obnoxious loud fans in server chassis.
[24.68 → 24.70] Yeah.
[24.94 → 28.44] But then we both decided that that was kind of lame.
[28.44 → 31.46] And those noises are sometimes annoying, at least the server fan.
[31.52 → 32.56] The old clunks are kind of funny.
[33.22 → 34.12] Who needs it?
[34.18 → 37.26] Or we just need to sample Brian Cantwell shouting into a bunch of servers.
[39.18 → 40.72] We got to focus on the content.
[41.28 → 44.94] This week, Brian Moses is joining us, and he has been blogging.
[45.60 → 48.74] Well, he blogs right up our alley, you might say.
[49.48 → 50.58] Welcome to the show, Brian.
[50.66 → 51.96] Thank you very much for joining us.
[52.64 → 53.76] Thanks for inviting me.
[54.30 → 55.68] Yeah, we've got a lot to talk about.
[55.68 → 63.12] I think you have been in and out of my various social media feeds for what feels like a decade.
[63.46 → 66.26] You are a man of many talents.
[66.38 → 68.22] So we're going to talk about a few things today in particular.
[68.58 → 73.50] The DIY NASS that you love to build and the off-site backup you built recently.
[73.78 → 74.66] 3D printers.
[75.06 → 75.88] Where would you like to start?
[76.10 → 76.52] You pick.
[76.64 → 81.60] Or maybe something that touches on multiple would be fun.
[81.60 → 89.08] I'll tell you what caught my attention is this $420 20-terabyte DIY NAS you're using for off-site backup.
[90.22 → 93.12] This hits a sweet spot for me right now.
[93.26 → 97.00] It's funny enough, I'm trying to figure out exactly how to get 20 terabytes off-site.
[97.22 → 98.68] That's the number, too, for me.
[99.22 → 100.06] Tell me about this setup.
[100.30 → 102.90] Well, my buddy, he's been doing it for a long time.
[103.34 → 104.24] You can't see it.
[104.24 → 108.62] I'm pointing over my shoulder, and this is on video, so this is very helpful.
[108.62 → 118.24] But a long time ago, he asked me if I would be willing to co-locate a Raspberry Pi, an external hard drive.
[118.88 → 120.16] Begins with a Pi.
[120.40 → 123.70] First, he's called it his backup, his off-site backup.
[123.70 → 128.74] But it's kind of turned into his, you know, it's just his, he uses C file.
[128.90 → 130.06] It's his cloud storage.
[130.32 → 144.98] And he has basically replaced his NAS with enough machines with big hard drives and, you know, his own cloud storage that he's got his data replicated in all sorts of different places.
[144.98 → 150.22] And his hardware redundancy is, it's not really a distributed file system.
[150.38 → 154.84] It's just distributed hard drives all synced up with the same data.
[155.64 → 158.86] And he said, you know, you've been doing this for me for months.
[159.00 → 162.58] You know, it's about time for you to get something over here.
[163.18 → 171.74] And that kind of synced up with the prices on mini PCs getting to be fantastic.
[172.20 → 172.70] Isn't it?
[172.70 → 178.44] I was looking at some of the specs that you were listing in this article, which there'll be a link to in the show notes, by the way.
[179.00 → 185.62] And you're comparing Ry zen chips and the new N100 Intel chip, which by all accounts, they've knocked it out of the park with.
[186.02 → 188.12] Have you got any experience with that particular chip yet?
[188.54 → 189.60] The N100?
[190.10 → 190.80] I do.
[191.04 → 192.14] I'm pointing over my shoulder.
[192.24 → 194.74] There's a little, that little white box over my shoulder.
[194.84 → 198.26] That's a two bay, kind of toaster style NAS.
[198.48 → 200.36] I reviewed it here recently.
[200.36 → 203.06] It's got an N100 CPU in it.
[203.16 → 204.62] And it's phenomenal.
[205.32 → 209.74] The one I think at my friend's house has an N5095.
[210.38 → 211.02] The Cameron.
[211.38 → 211.62] Yeah.
[211.70 → 214.74] Which is the N100's little, little brother.
[214.98 → 215.90] It's a younger sibling.
[216.32 → 217.24] It's a little bit older.
[217.42 → 218.84] They're very similar.
[219.42 → 224.38] The manufacturer B-Link, Mini B-Link, I think is the name of them.
[224.38 → 229.86] I have been looking at them on Amazon, which feels like for three or four years.
[230.04 → 233.14] And I just, I couldn't resist it anymore.
[233.26 → 236.42] It's like, I'm going to buy it, and I'm going to do something with it.
[236.46 → 237.80] I don't know what it was going to be.
[238.08 → 245.18] At one point, I thought it might be a Raspberry Pi, not a Raspberry, an Octobrist server for my 3D printer that I don't have anymore.
[245.18 → 253.58] Because I wanted something to transcode my really high-res time lapses that I was recording.
[253.98 → 263.30] And then eventually I said, you know, I really need to get some sort of, well, my off-site backup up until then was Back play's B2 storage.
[263.30 → 267.52] And my bill just kept getting more and more expensive.
[268.20 → 271.36] I mean, it was, I can't remember when I shut it off.
[271.40 → 274.22] I think I was near $80 a month.
[274.52 → 275.70] I could have fixed that.
[275.78 → 277.68] I mean, I was backing way too much stuff up.
[277.76 → 282.48] My media collection did not need to be in the cloud, but it was.
[283.00 → 285.46] I look at my collection from time to time, too, and I kind of pare it down.
[285.64 → 286.40] That helps with the backup.
[286.40 → 298.60] So you got a B-Link Mini 5 PC, an external 20-terabyte Western Digital Elements disk, and then the part that surprised me, and I want to hear your thoughts on this and how it's working for you, is True NAS scale.
[298.94 → 300.44] It worked great.
[300.62 → 304.50] I mean, I don't know how much you guys have worked with True NAS over the years.
[305.06 → 311.02] But, you know, I started back, you know, Free NAS 12 years ago when it was running.
[311.26 → 312.58] Well, and it still does.
[312.64 → 313.78] It's called True NAS Core now.
[313.78 → 327.06] When it was running FreeBSD and hardware support for everything, you know, either – well, and everything kind of that was in my wheelhouse, consumer-grade hardware, was just kind of dicey.
[327.12 → 330.50] You know, you would buy something and a component on the motherboard wouldn't work.
[331.00 → 340.14] And it was – you know, that kept me petrified on all of these mini PCs and things that – it's like I don't know what chipsets are in there.
[340.14 → 345.40] I don't want to go research FreeBSD versions to see if it's going to be supported.
[346.14 → 351.26] And then when True NAS scale came out, I just put it on everything.
[351.58 → 358.88] You know, it's based on Debian, so there's way more hardware support out there for consumer-grade hardware.
[358.88 → 365.76] And I've – everything that I've installed True NAS scale on since it came out has just worked.
[365.84 → 368.12] I haven't had a single problem.
[368.88 → 370.66] And that was the case with this.
[370.72 → 374.34] You know, like I expected and worried about problems.
[374.34 → 375.74] And I set it up.
[376.26 → 377.38] I had it running.
[377.38 → 382.70] I set up a replication task to back up the entirety of my NAS to it.
[383.06 → 385.10] And it took a – it took some time.
[385.24 → 389.28] You know, I had gigabit network between here and there.
[389.42 → 390.54] But it just worked.
[390.64 → 396.52] You know, I expected, you know, instability or, you know, this random kernel panic in the middle of something.
[396.76 → 399.12] And none of that – none of that ever happened.
[399.22 → 400.72] It was – it was awesome.
[400.72 → 408.06] The new Intel Arc GPUs have been the most recent example of me having to do some stuff with the kernel,
[408.22 → 412.38] which I've kind of gotten used to things just working these days.
[412.46 → 413.36] I'm kind of spoiled.
[413.70 → 419.58] And I think you mentioned, you know, you used to use True NAS back when it was still called Free NAS,
[419.72 → 423.42] back when you actually needed a proper hall pass to operate the thing, you know.
[423.76 → 424.10] Yes.
[424.20 → 424.80] So good for you.
[424.80 → 430.86] I think there's a real value in using the same system for so long.
[430.98 → 432.26] Like, you get to know a lot of its quirks.
[432.40 → 438.68] And obviously, if you're into that, you know, Free NAS, True NAS space, you're a ZFS zealot, right?
[439.26 → 440.64] I mean, I like it a lot.
[441.42 → 446.86] This is kind of interesting because, you know, when I started on this journey way back when,
[446.86 → 454.98] I had maybe installed Red Hat once on one PC and used it for like two weeks and said,
[455.18 → 458.70] I am not good at this.
[458.82 → 460.68] It's taking me too long to do everything.
[460.92 → 462.66] And I just stopped using that PC.
[462.84 → 469.42] And I've – I mean, I don't want to say I'm a Windows dummy, but, you know, Windows is my sweet spot.
[469.42 → 475.36] So anytime I've delved off into anything, you know, Linux or even Unix-based, but FreeBSD,
[475.62 → 478.26] I'm way outside my comfort zone.
[478.80 → 482.02] And that was definitely the case, you know, with ZFS.
[482.52 → 488.78] BSD is just different enough from Linux that every time I use it, I catch myself doing something.
[488.96 → 493.56] Like, the way in which, for example, as a command works is just subtly different,
[493.62 → 495.40] or said is just subtly different.
[495.50 → 497.66] And it's just enough to trip me up the whole time.
[497.66 → 503.08] So when True NAS Scale came along, as you mentioned, it's based on Linux and Debian these days.
[503.38 → 511.46] It really, for me, was like validation of all the hard work that Canonical put into shipping ZFS back in,
[511.56 → 513.46] I think, 2018 was the first time they did it.
[513.96 → 515.96] So, yeah, we're seeing the fruits of that labour now.
[516.04 → 525.82] And I wonder if we're at the tipping point yet whether Scale is now, like, the primary target for IX systems
[525.82 → 528.78] or whether, like, are we at that tipping point yet, do you think?
[528.78 → 531.78] I would think so, maybe.
[532.28 → 537.74] You know, I've seen, like, in their forums and maybe in their Subreddit, you know,
[537.78 → 543.78] a couple of things that folks from IX have said that make me think that, you know,
[543.82 → 548.76] that that might be, you might be seeing a shifting of focus between the two products.
[548.76 → 556.34] And, in fact, I saw something and I had to go apologize to someone in our Discord server because, you know,
[556.46 → 563.30] they said essentially that a couple of months ago that, you know, True NAS Scale was going to get all the attention
[563.30 → 567.84] and True NAS Core might, you know, I don't want to say be neglected.
[568.38 → 568.64] It's all right.
[568.66 → 569.16] You can say it.
[569.16 → 569.82] They're going to take it up.
[569.88 → 571.72] They're going to take it upstate to the farm.
[571.88 → 572.34] You know, it's fine.
[572.34 → 573.64] It's going to live up.
[574.26 → 580.92] And I said to him, I said, all the people who are paying money today to use True NAS are using True NAS Core.
[581.12 → 587.20] I mean, I don't know that many or any enterprise customers are using Scale yet.
[587.92 → 595.74] So, you know, when it's awesome that the community, the True NAS community is jazzed about True NAS Scale,
[595.74 → 603.82] but you need to see that, you know, trickle up to, you know, that enthusiasm transferring over to business places
[603.82 → 606.52] before I think we really see a bunch of movement.
[606.52 → 608.10] Did you ever consider anything else?
[608.24 → 610.18] Like, was Unpaid in the mix back in the day?
[610.60 → 616.16] Back in the day, like, when I did it, Free NAS was the one that I heard of,
[616.68 → 619.84] even though it wasn't as easy as I thought it was going to be.
[619.84 → 627.08] I liked the idea of taking a PC, you know, just a regular PC that I was upgrading every, you know,
[627.12 → 633.14] one to two years and reusing that old PC to do some network attached storage.
[633.48 → 636.84] That's what I would have done, except at the time I was buying laptops.
[637.62 → 639.10] You know, I was like, I'm just...
[639.10 → 642.66] Your blog tells me that that habit got a little bit out of hand.
[642.84 → 643.74] It really did.
[643.92 → 647.08] So that's a wild story all by itself.
[647.08 → 652.26] So I wanted, I knew I needed some sort of network attached storage at home.
[652.42 → 654.66] And I was evaluating all of my options.
[655.22 → 659.50] And I was going around looking at different products, looking in different communities.
[659.86 → 664.96] And I just wanted, I didn't want somebody's, I didn't want to poach somebody's recipe.
[665.64 → 669.84] But I wanted someone to say, here are the things, here are the components that I picked.
[670.22 → 671.44] Here's why I picked them.
[671.94 → 674.88] And I'm sharing it with whatever community I'm sharing it with.
[674.88 → 682.44] And my buddy and I, who at the time, like every Monday night, we were going to the same bar while our wives did exercise.
[682.88 → 686.68] And I was talking to him and I said, I want to build a NAS.
[687.22 → 694.72] I don't want to build it from the ground up using Linux because I'm, or anything other.
[694.72 → 698.12] I don't want to use Windows was right at the top of my head.
[698.92 → 700.78] And I don't really want to use anything else.
[700.84 → 703.02] I really need something that's an appliance.
[703.36 → 709.24] And all these places that I'm going, I'm not finding the content that I'm looking for.
[709.54 → 711.80] And he's like, well, you've, you've got a blog.
[712.40 → 715.12] Why don't you figure this out and write about it?
[715.12 → 722.42] And that, you know, at the time I was excited when 30 or 40 people went to my blog in a day.
[722.84 → 723.94] I remember that same feeling.
[724.14 → 724.40] Yeah.
[724.40 → 731.92] So I wrote a blog and for whatever reason, I wrote it, you know, essentially this is what I was looking for.
[732.00 → 735.02] This was, this was the content that I hoped that someone created.
[735.56 → 738.46] And I said, here are the here are the parts that I picked.
[738.58 → 739.74] Here's why I picked them.
[740.40 → 749.98] And, you know, I never, I never, and I still don't intend for people to just blindly look at my parts list and go, add all that to cart.
[749.98 → 755.26] And I've got, I've got the makings of my DIY NAS, but that's, that's kind of how it's turned out.
[755.34 → 763.00] You know, it's, I try every time I write a blog to say, Hey, I, I picked this motherboard because it met these few criteria.
[763.60 → 765.48] These criteria are important to me.
[765.56 → 767.34] They don't need to be important to you.
[767.74 → 774.48] But a lot of times people, they, they're like, well, if it, if it worked for you, you know, I want to, I want to build the same thing.
[774.48 → 782.84] And so because I do so much, maybe consumer grade hardware, you know, those inexpensive motherboards that are a good deal.
[783.02 → 788.32] When I built it, you know, six months later, you can't buy them, or they're way more expensive.
[788.96 → 795.48] And people were asking all the time, well, Hey, I can't find the motherboard or the Rams too expensive.
[795.98 → 797.56] You know what would you do today?
[797.80 → 802.40] And then I started to realize, well, this just needs to be a thing.
[802.88 → 803.78] An annual series.
[803.78 → 804.02] Yeah.
[804.06 → 812.62] So what, what Brian's talking about here is on, on his blog, he's got a DIY NAS 2015 edition that's happened pretty much every year since.
[813.02 → 813.14] Yeah.
[813.26 → 832.92] Well, like now, now too, because somewhere along the lines, you know, in my, uh, my affinity for doing free BSD, some of my builds got really complicated, expensive, you know, I don't want to say enterprise grade, but you know, really expensive hardware.
[832.92 → 841.90] And I, I kind of realized, I said, well, I, I would build this today because now I've, I've gone down the rabbit hole, and I'm a, I'm a zealot.
[841.98 → 843.32] I'm a DIY NAS zealot.
[843.32 → 847.82] This is, this is part of my, this is my part of my persona now.
[847.82 → 848.76] Isn't that funny?
[848.82 → 852.44] Cause when you started out, CPUs were basically potatoes.
[852.64 → 853.10] Yeah.
[853.10 → 860.06] And now, you know, the N100 is more powerful than probably the main CPU that you put into your primary NAS 10 years ago.
[860.06 → 867.14] And yet we still feel the need to build these Epic Rome based Cases that have 128 gigs of Ram.
[867.28 → 868.66] And isn't it weird?
[868.98 → 870.72] Yeah, that is, that is strange.
[870.72 → 878.98] Like I tell people that all the time when, when we're chatting, it's like, you don't need, if it's all you're interested in is serving up files.
[878.98 → 883.78] You don't need a ton of, a ton of CPU for sure.
[883.98 → 897.02] And you don't need, you probably don't need gobs of Ram, but you know, there we've kind of seen a convergence of home labs and network attached storage where people are doing.
[897.02 → 920.36] Those two things are kind of almost ubiquitous, you know, like the guy, like most, most of mine, you know, are built with the intention of, you know, running a handful of virtual machines or, you know, now with scale apps and containers and doing more other than just serving up, serving up files.
[920.36 → 930.34] And there's a huge subset of people, this isn't me, that are collecting media, and they need the, the CPU or GPO for transcoding.
[930.72 → 937.22] And they want, you know, they want to, their, their passion is the media collection and consuming that media.
[937.22 → 943.52] And the NAS is a, a vessel for that, for that hobby.
[943.92 → 944.22] Obsession.
[944.32 → 946.10] I think it's, it's the word you're looking for.
[946.10 → 950.42] Obsession's a kind of negative term sometimes.
[950.68 → 951.08] Yeah.
[951.16 → 951.42] It's true.
[951.62 → 952.30] Truthful though.
[953.88 → 954.36] All right.
[954.36 → 955.92] So let's talk about 3d printers for a little bit.
[955.96 → 957.08] Because I think that's another area.
[957.30 → 963.86] I also just noticed you have lots of posts about drone racing, which was another area that I was massively into for a while.
[964.42 → 965.36] Kind of funny, isn't it?
[965.36 → 972.04] Like I got into 3d printing because I wanted to print little, little bits from my racing drones in, in TPU back in the day, but.
[972.16 → 972.36] Yep.
[972.58 → 974.40] I can, I can understand that.
[974.40 → 976.84] You and I share, it's weird.
[976.92 → 977.98] The timeline that this happened.
[978.12 → 982.56] We, we both ended up on Black Friday ordering a bamboo lab P1S.
[983.00 → 983.44] Interesting.
[983.70 → 984.32] That's wild.
[984.78 → 985.90] I bought one too.
[986.10 → 989.54] I got an X1C almost a year ago.
[989.78 → 992.72] I had pre-ordered the Brusa XL.
[992.72 → 994.34] We were both Brusa fanboys.
[994.54 → 997.14] Let's just, let's just set the record straight here.
[997.34 → 1001.00] I don't like to say that I'm a, I'm a former Brusa fanboy.
[1001.00 → 1008.78] They've just, they've just had their apple cart upset by a new, a new company on the market.
[1008.92 → 1011.26] I had a Brusa Mark III for a long time.
[1011.52 → 1013.94] The Brusa XL, the day it was announced.
[1014.16 → 1015.52] I've still got mine behind me.
[1015.56 → 1016.48] I'm pointing to it right now.
[1016.58 → 1021.46] The day it was announced, I pre-ordered it and I waited in anticipation for it to come out.
[1021.46 → 1029.98] And it just didn't come out and, you know, bamboo labs came onto the market with the X1C that, or the X1 that they, they crowdfunded.
[1030.40 → 1032.50] Crowdfunded in air quotes, I think.
[1032.92 → 1034.36] Well, and they, they got a lot of flat.
[1034.44 → 1036.46] Well, I mean, maybe even deservedly.
[1036.56 → 1042.56] So there have been lots of crowdfunded 3d printing projects that have not gone spectacularly well.
[1042.56 → 1048.66] It was pretty rare to have one deliver and deliver like beyond folks, folks expectations.
[1049.14 → 1053.84] But yeah, I bought the X1C and fell in love with it and used it.
[1053.90 → 1054.94] And I kept my Mark III.
[1055.10 → 1060.32] I sell, I sell some 3d printed parts on Tiny for different things.
[1060.58 → 1067.44] And the whole idea was, you know, every now, and then I was 3d printing stuff on my Mark III, and it was a bottleneck.
[1067.44 → 1072.60] You know, I had to wait for a couple of hours for it to finish so that I could iterate on something else.
[1072.86 → 1076.56] And I got tired of waiting, and I wanted, you know, I wanted another printer.
[1076.56 → 1085.70] So I got, I got the X1C fully intending to use the X1C to, to print or to prototype.
[1085.70 → 1089.88] And the other one was going to be my, my workhorse for churning out orders.
[1089.88 → 1098.88] But then the X1C was so fast that I, I just didn't want to print to the Mark III anymore, which kind of makes me sad.
[1099.08 → 1101.04] I mean, I, I like the Mark III.
[1101.50 → 1103.74] I love the Octobrist project.
[1103.88 → 1104.98] I think that's fantastic.
[1105.54 → 1105.60] Yeah.
[1105.64 → 1114.66] It's interesting because, you know, Brusa really changed the game when they, when they came out, you know, they were expensive, particularly here in America.
[1114.66 → 1120.82] Shipping anything over from Prague is, it's really almost prohibitively expensive to buy filament from them.
[1120.88 → 1124.80] You know, you're looking at double the price of pretty much anything we can get on Amazon over here.
[1125.26 → 1128.52] But I look at the rep rap philosophy that Brusa followed.
[1128.52 → 1134.00] And I don't wonder whether they've taken it about as far as it can go in its current format.
[1134.20 → 1135.54] You know, you look at what Bamboo are doing.
[1135.64 → 1144.18] A lot of their components are injection moulded, for example, or they're just straight up stamped steel, you know, whereas Brusa 3d print.
[1144.18 → 1148.62] Everything that isn't metal on the printers, you know, near as they can.
[1149.08 → 1152.14] And it's just, it's just a totally different philosophy on how to build a product.
[1152.14 → 1162.22] Like I think it was Adam Savage said it on Tested that the bamboo stuff is as close to a kitchen appliance as a 3d printer can pretty much be.
[1162.36 → 1164.32] And I can't think of any higher compliment.
[1164.76 → 1164.86] Yeah.
[1165.02 → 1165.20] Yeah.
[1165.20 → 1165.76] That's perfect.
[1165.96 → 1171.20] I made a bad analogy the other day to the bamboo and like ink-jet printers.
[1171.20 → 1176.24] If you remember some of your first printers, the weird jet, I mean, they didn't, they weren't great.
[1176.66 → 1179.20] It wasn't something that I'm going to pick on my mom.
[1179.30 → 1180.52] I hope she doesn't listen to this.
[1180.62 → 1188.66] You know, it wasn't just something that my mom could pick up and use, but in an ink-jet printer, you know, at the beginning they were, you could just, you could use them.
[1188.66 → 1197.02] They were so much cheaper than all the other printers that were out there that pretty soon everybody had an ink-jet printer at home.
[1197.02 → 1203.60] Back when printers were really uncommon outside, you know, the computer library at school or the workplace.
[1203.98 → 1207.52] I think for sure bamboo labs is doing that for 3d printing.
[1207.60 → 1214.36] I mean, people ask me all the time, you know, Hey, I'm thinking about getting a 3d printer for the money.
[1214.36 → 1217.04] I can't suggest anything else.
[1217.18 → 1228.28] I mean, you pick a you pick a budget point and bamboo labs probably has the best performing best value proposition at that, at that price.
[1228.50 → 1233.32] Which is wild because two years ago, nobody had ever even heard of them.
[1233.86 → 1234.90] That's what surprised me the most.
[1234.90 → 1239.00] When I read through your post was just the pricing that I didn't realize that's where we're at now.
[1239.08 → 1239.36] Yeah.
[1239.58 → 1239.78] Yeah.
[1239.80 → 1240.70] That's, that's big.
[1240.70 → 1246.24] And even better, like the A1, the A1, the multicolour A1 is what?
[1247.00 → 1247.44] $460.
[1248.24 → 1251.26] I mean, we talked, this is, this is going to go back to another.
[1251.54 → 1259.36] We used to talk, our friends who were thinking about getting into drone racing or just drones, FPV drones at all.
[1260.44 → 1263.32] People would ask us, well, where do we get started?
[1263.32 → 1269.74] And we would always tell them, Hey, it's an expensive, it's an expensive hobby at the maker space.
[1269.74 → 1279.26] And it's, it's risky, you know, at the makers, at the maker space we used to volunteer at, we led, I think, three different drone building classes.
[1279.26 → 1285.46] And on the first day of flying each one of those drones, at least one person lost their drone.
[1285.82 → 1289.62] I mean, like flew it over a, I mean, a Creek.
[1289.74 → 1292.14] I mean, it was just, it was just gone forever.
[1292.14 → 1296.22] So there was a little, there was a little kit that you could buy.
[1296.32 → 1299.46] It was, I can't remember the tiny Hawk was the name.
[1299.62 → 1302.80] I can't remember who makes it, but it was like 200 bucks.
[1302.92 → 1308.86] You got really cheap goggles, a really cheap radio and a little inexpensive drone that you could fly around.
[1309.10 → 1310.80] You could fly around your house.
[1310.80 → 1318.22] And that was kind of a decent value for the $200 to figure out if you like a hobby or not.
[1318.34 → 1321.38] As far as hobbies go, that's, that's pretty inexpensive.
[1321.72 → 1322.60] Not a bad entry price.
[1322.76 → 1322.98] Yeah.
[1323.12 → 1328.38] And bamboo has gotten printers down around that price, you know, like, and they just work.
[1328.38 → 1335.04] I mean, it used to be, you could spend two or $300 on a printer, but that printer kind of became the hobby first.
[1335.04 → 1345.82] Getting that printer working and maintained and getting it to be reliably took a lot of, a lot of learning and a lot of effort on the, on the person who's doing it.
[1345.86 → 1347.18] And that was taxing.
[1347.32 → 1353.04] Or you could buy, you know, like the Brusa, you could spend, I can't remember how much my Mark III was.
[1353.08 → 1356.62] It was like $1,400 or $1,500 fully assembled.
[1356.62 → 1361.58] You know, it came to me, took it out of the box, dropped it down, turned it on and it printed something.
[1361.70 → 1363.42] And that was, that was fantastic.
[1363.42 → 1368.78] But now we've gotten to the point where, you know, $300 can, can get you that.
[1369.06 → 1369.18] Yeah.
[1369.44 → 1369.64] Yeah.
[1369.64 → 1370.92] I'm pretty excited about it.
[1371.38 → 1379.12] I, I also want to ask you, Brian, about a little, a little rumour that a little birdie told me about you doing a podcast at Texas Linux Fest.
[1379.18 → 1380.08] Can I pick your brain about that?
[1380.10 → 1380.66] What's going on?
[1381.06 → 1384.12] Well, Alex is a terrible influence on people.
[1384.12 → 1396.34] He, he asked me if I was, if I was going to any conferences and I told him about a friend of mine who's, who's been involved with Texas Linux Fest, has been talking, has been trying to get me to go there.
[1396.92 → 1400.08] He wants me to give a talk, and I'm, I don't think I'm ready for that.
[1400.50 → 1404.24] But I, I said that, and he's like, well, I'm going to be at Texas Linux Fest.
[1404.28 → 1406.62] I was like, well, forget it.
[1406.62 → 1407.98] I'm going to, I booked a hotel.
[1408.12 → 1408.90] I rented a car.
[1408.90 → 1410.46] I'm going to, I'm going to drive down.
[1410.76 → 1413.66] It's about three and a half, four hours from where I'm at.
[1414.12 → 1418.68] It's across the street from what I might rate as some of the best barbecue in America.
[1419.12 → 1419.36] Okay.
[1419.88 → 1420.76] Maybe the world.
[1421.30 → 1421.74] Maybe the world.
[1421.78 → 1435.70] Chris and I will both be there, but specifically Brian and I are going to do a live podcast on behalf of Tail scale talking about how Brian uses Tail scale as part of his backup situation and all that sort of VPN goodness.
[1435.70 → 1440.40] So until then, where else can folks go to find more about you, Brian?
[1441.14 → 1446.54] The best place to go would probably be my blog at blog.briancmoses.com.
[1446.72 → 1447.92] Well, thank you very much for coming on.
[1447.96 → 1450.80] It was an absolute pleasure, and I'm sure it won't be the last time.
[1451.18 → 1451.72] I hope not.
[1451.82 → 1452.66] This was fantastic.
[1454.66 → 1456.92] Tailscale.com slash self-hosted.
[1457.06 → 1462.02] Tail scale is the easiest way to connect any device and service to each other wherever they are.
[1462.02 → 1472.10] You'd think the internet would be better at this, but Tail scale has finally nailed it securely that uses WireGuard's noise encryption protocol to make it all safe.
[1472.62 → 1473.64] And it is fast.
[1473.80 → 1475.58] Like, really fast.
[1475.94 → 1482.34] Tail scale, you can get up and go in just minutes, but on top of that, you'll find the performance on your device is mind-blowing fast.
[1482.76 → 1483.68] And Tail scale is smart.
[1484.06 → 1486.12] Devices will talk directly to each other.
[1486.12 → 1491.08] Even when you're behind, like, crazy double carrier NAT stuff, I mean, I can testify to that.
[1491.54 → 1492.34] It has worked great.
[1493.02 → 1500.98] Another way to think about Tail scale is it's a simple way that lets you build networks across complex infrastructure.
[1501.82 → 1509.34] I mean, like, you could have Tail scale on a device that's running on your VPS and you could have it running on your phone and a VM that's running on your workstation.
[1509.46 → 1511.04] And they can all be on the same network.
[1511.04 → 1522.22] When I launch new services in a container now, I bind the container's networking to a Tail scale container and I do all the networking for my Docker containers through Tail scale now.
[1522.76 → 1527.44] Each application shows up on the Tail net like a node and I can talk directly to it.
[1527.52 → 1529.82] I can SSH into the container if it supports that.
[1529.90 → 1532.12] I mean, it's really super handy.
[1532.18 → 1537.80] And you can replace your legacy VPN infrastructure and have a mesh WireGuard-protected network with Tail scale.
[1537.80 → 1544.26] It literally transforms your network security and is redone the way I do not only my applications but my networking in general.
[1544.52 → 1551.64] And there are a lot of nice features in their like Tail scale Send, which I love because one of the fun things about Tail scale Send is it's built into every machine that has Tail scale.
[1551.82 → 1554.66] So, like, all your different OSes across different architectures.
[1555.26 → 1561.80] But you can start a Tail scale Send transfer, log into the machine you want to receive it after it's already started sending,
[1562.42 → 1564.68] and then tell that machine where to actually save that file.
[1564.68 → 1567.76] I know that sounds weird, but I just use that all the time.
[1568.06 → 1569.68] Oh, and I love Tail scale SSH.
[1570.36 → 1575.76] It's like managing my SSH keys for me now, but it's handled through my Tail scale authentication, which is slick.
[1576.18 → 1579.64] And if you're in a corporation, it supports your two-factor integration with your groups.
[1580.14 → 1581.52] It's really great for enterprises.
[1582.10 → 1584.58] And you don't have to have one of those big old VPN boxes anymore.
[1585.02 → 1589.70] So if you're a home lubber, or you're an enterprise, Tail scale will scale.
[1589.70 → 1595.96] And impressively so, I invite you to go check it out and get 100 devices for free at tailscale.com slash self-hosted.
[1596.44 → 1598.62] So go see what I've been talking about and support the show.
[1599.14 → 1608.18] Securely connect anything to anything, no matter what operating system, hardware type, or other weird configuration or network is in its place between them.
[1608.96 → 1610.58] It will work flawlessly.
[1611.00 → 1613.58] Try it out, support the show, and change your networking game.
[1613.58 → 1616.70] You go to tailscale.com slash self-hosted.
[1616.78 → 1619.80] That's tailscale.com slash self-hosted.
[1621.62 → 1625.20] You and I are at different ends of the Zigbee spectrum at the moment.
[1625.30 → 1629.46] I think you're ripping it out, and I'm going all in and just doubling down and everything.
[1629.90 → 1636.66] This week, I install what must have been, I think, about half a dozen Novel Blue Series Zigbee smart switches.
[1637.16 → 1640.06] I guess it depends on which week you catch me on.
[1640.06 → 1645.62] But two weeks ago, I would have told you my Zigbee network is as solid as a wired network.
[1645.78 → 1654.40] And then I added one smart plug, one Zigbee smart plug, and three, including the new one, three smart plugs just started dropping off the network.
[1655.24 → 1659.86] And that's what I find kind of frustrating about Zigbee is you can have it working really, really well.
[1659.86 → 1666.26] And then you add a certain type of device, and it seems like things can sometimes just go a little haywire.
[1666.90 → 1670.20] But, you know, I know other people have had better luck.
[1670.42 → 1673.98] And I also, you know, I have great luck with my switches and my sensors.
[1674.16 → 1675.30] Those never seem to drop off.
[1675.48 → 1676.46] It's just the smart plugs.
[1677.04 → 1679.72] I just wish it wasn't 2.4 gigahertz based, you know.
[1679.72 → 1687.14] It's so promising as a protocol, like self-healing, like the topology, it figures it out by itself.
[1687.36 → 1689.28] It's a separate thing from Wi-Fi even.
[1689.50 → 1696.96] So in some of these switches that I've replaced this week, I've actually been ripping out some of my Shelley's that have been in there for, I guess, four years.
[1696.96 → 1698.78] Because we've been in this house for about four years now.
[1699.56 → 1702.48] But I ripped out a few Shelley's and replaced them with these Novel smart plugs.
[1702.48 → 1706.18] And it is, they are just, they're expensive.
[1706.72 → 1717.18] I think they're like $55 a switch, which, you know, considering you can go to Home Depot and buy a bog-standard light switch for like $3 or $4 is criminally expensive.
[1717.84 → 1719.74] But they are fabulous.
[1720.00 → 1728.36] They have not only got like a rocker switch design, like the big paddle design, as opposed to like the, you know, lever, like flick switch design.
[1728.86 → 1731.48] So first, they're big and new, and they look nice and modern.
[1731.48 → 1737.58] Whereas a Shelley's, I've no idea whether it's back there or not, which is a pro or a con, depending on your point of view.
[1738.46 → 1743.52] But these Novel ones in particular have a little LED strip just down the side.
[1743.92 → 1746.84] It's almost like Star Trek, dare I say.
[1746.96 → 1749.32] Like my house looks modern.
[1749.44 → 1751.44] It looks smart with these switches in it.
[1751.80 → 1760.16] And so I've been able to do all sorts of fun things, like enable single taps to do one thing, double taps to do a number, triple taps to do another.
[1760.16 → 1769.50] And then based on what those things do, the LEDs can change colour, or they can do different effects or like, you know, it's just so cool.
[1770.16 → 1771.56] This does look really neat.
[1771.78 → 1777.88] And I suppose a step up from the Shelley's because now you have that little slider, you have that colour.
[1778.02 → 1781.88] So you actually have more information than when you just had a dumb switch there.
[1781.88 → 1782.60] Yeah, yeah.
[1782.72 → 1788.86] So for me, what I'm doing, I've got a pair of IKEA Zigbee smart blinds in this room, for example.
[1789.20 → 1796.32] I also ripped out and replaced the ceiling fan in my bonus room over the weekend, which was actually not as difficult as I expected.
[1796.62 → 1797.66] I've never done it before.
[1797.90 → 1802.42] You know, like American wiring is all, you know, it's pretty straightforward.
[1802.66 → 1804.40] It's black and white, you know, literally.
[1804.66 → 1805.16] That's it.
[1805.16 → 1808.44] But, you know, it's not too bad.
[1809.14 → 1810.56] But so what I've got now is...
[1810.56 → 1811.14] Finish your sentence.
[1811.26 → 1812.96] Are you telling me your fan is Zigbee?
[1813.52 → 1813.82] Yes.
[1814.70 → 1819.30] So now I looked high and low for a Zigbee fan.
[1819.42 → 1821.62] Well, it's not actually the fan itself.
[1821.62 → 1832.62] So if you look on the Novel website, they make, you know, that little plastic ballast thing that goes in the space above the fan itself for the LED lights, because all the new ones are LED.
[1833.90 → 1840.92] Novel, it's a pre-order only right now, but I reached out to them, and they sent me one, and it's awesome.
[1842.28 → 1843.36] I had to pay for it.
[1843.44 → 1844.64] It wasn't like sponsored or anything.
[1844.84 → 1847.08] I just said, like, I'd love to talk about it on the show.
[1847.18 → 1848.62] So, you know, full disclosure.
[1848.62 → 1855.34] But from that perspective, it just replaces the ballast that comes with the device from Home Depot.
[1856.04 → 1859.44] And then I can address it like any other device on my Zigbee network.
[1859.56 → 1861.94] I can control the three-speed fan.
[1862.22 → 1863.90] I can control the LED light separately.
[1865.12 → 1866.34] It's just the future.
[1866.48 → 1868.10] And then I've got the actual smart switch.
[1868.18 → 1876.94] So I've got not only the controller in the fan, I've also got the wall switch as well, which has to be rated for a continuous AC load, like a ceiling fan.
[1876.94 → 1878.50] So you can't just use the normal switch.
[1879.46 → 1879.92] So, you know.
[1880.04 → 1881.20] Man, I want this so bad.
[1881.24 → 1888.92] Yeah, I can double tap the switch on the wall over there and change the speed of the ceiling fan or have the Zigbee smart blinds go up if I triple tap.
[1889.14 → 1889.48] Interesting.
[1889.74 → 1894.98] The smart blinds are a totally different manufacturer, like Home Assistant and software for the win.
[1895.16 → 1897.10] Yes, it is great the way it all ties together.
[1897.68 → 1899.60] And the Zigbee devices, the way they all work together.
[1899.60 → 1902.76] These look like really top quality.
[1903.02 → 1904.82] I also note they do have a couple of Z-Wave.
[1905.06 → 1913.54] And for those of you in the Z-Wave world, they are Z-Wave 800, which that's the thing about Z-Wave is it hasn't stood still.
[1913.62 → 1915.52] It's been getting better and even better range.
[1915.56 → 1916.98] So it's nice to see them support both.
[1917.70 → 1923.12] This fan module could be a fundamental life changer for me here in the studio in the summer.
[1924.16 → 1926.12] Can you change the direction of the fan?
[1926.12 → 1934.82] Yeah, well, I mean, it's just that the fan is, I can't do that with the Novella thing, but there's a switch, you know, physical switch on the fan itself.
[1935.02 → 1935.80] Well, that's really neat.
[1935.94 → 1937.40] So how many of these did you end up with?
[1937.58 → 1942.44] I only got one of the LED ballasts things because, you know, like I said, they're not cheap.
[1942.86 → 1943.22] Sure.
[1943.42 → 1952.04] The main motivation was I'm actually kitting out one of my spare bedrooms as like a proper recording studio for all the tail scale like videos I'm doing and things.
[1952.04 → 1963.10] My wife, bless her, got, she didn't get shirty, she didn't put her foot down, but she just said enough times like there's a lot of camera gear in my lounge, you know?
[1964.26 → 1969.16] So I thought maybe I should actually put it in a room with a door, not in the middle of our lounge.
[1969.16 → 1977.70] So I just wanted to be able to control the ceiling fan whilst I was recording and, you know, walking the three steps to the wall and actually flicking the switch seemed like too much effort.
[1977.88 → 1983.70] So instead I replaced the light switch and I replaced the ceiling fan and went to Home Depot God knows how many times.
[1984.34 → 1985.38] Somehow that's less effort.
[1985.72 → 1990.74] And I assume because they're hardwired, they act as repeaters on the Zigbee network as well, so they would extend range.
[1990.74 → 1994.22] They are routers on the Zigbee network, always on, always powered.
[1995.36 → 1998.72] It's like Nirvana of Switch land.
[1999.06 → 1999.16] Yeah.
[1999.46 → 2000.02] Until it's not.
[2000.12 → 2009.68] But yes, I'm really, I'm really interested to know how they work for you long term because those I think would be really great in the studio in a couple of places like my office and in the actual physical studio.
[2010.18 → 2011.48] I could see those being really useful.
[2011.70 → 2013.52] They haven't missed a single beat so far.
[2013.60 → 2017.48] Now I will, I will caveat that it's probably Zigbee radio dependent as well.
[2017.48 → 2022.46] I'm still extremely happy with the tubes, Zigbee radio that I bought a while back.
[2023.00 → 2035.30] But what really made the difference for me was someone on the discord introduced me to trigger IDs and these in Home Assistant automation land will absolutely change your game.
[2035.80 → 2041.66] So these allow you to specify essentially variable names on specific triggers within a specific automation.
[2041.66 → 2049.52] So if you, for example, have a light switch that triggers a certain event like a double tap, you can give that a name.
[2049.64 → 2052.38] You can give that event, that trigger, a trigger ID.
[2052.82 → 2058.00] So let's call it Garage Switch Double Tap is the variable name.
[2058.40 → 2059.64] Camel case, do whatever you like with it.
[2060.48 → 2067.64] You can then refer to that trigger throughout the rest of the automation, throughout all the actions and do conditionals based on it.
[2067.64 → 2084.56] You can then also say just in one automation, you could have all the triggers related to that light switch in one place and then all the actions related to that trigger in one place rather than having to have five automations that handle all the edge cases.
[2085.24 → 2092.28] Because I don't know about you, whenever I ended up doing anything with automations, I ended up with 15 tabs open trying to keep track of which ones I had or had not updated.
[2092.28 → 2094.90] And this just totally changes the game.
[2095.50 → 2100.76] Yeah, boy, that would make it so much simpler too if you swap a switch out down the road, something like that.
[2101.02 → 2102.26] Save yourself a ton of time.
[2102.54 → 2109.72] Because you can very quickly, especially like with the quad panel buttons, that each one you can do multiple actions for hold and tap.
[2109.76 → 2112.42] You can really quickly just spiral out of control with the automations.
[2112.42 → 2121.38] It essentially allows you to do if this or if then else in a GUI based Home Assistant automation editor.
[2121.94 → 2129.22] It works the way that my brain understands logic should work, which is questionable sometimes, but it's fantastic.
[2129.36 → 2132.92] So if you haven't gotten into trigger IDs yet, highly recommend it.
[2132.96 → 2136.68] I'll put a link to the video that helped me understand them in the show notes.
[2136.68 → 2141.30] Jupiter Broadcasting has something new for you.
[2141.48 → 2143.42] I'm calling it the weekly launch.
[2143.74 → 2144.96] Let's warm up the week together.
[2145.18 → 2152.86] You can check out the weekly launch and I will guide you through the most interesting stories and clips that I think set the stage for the rest of the week.
[2152.98 → 2156.40] It's all part of a new content rotation coming to a brand-new feed.
[2156.74 → 2158.32] And I would love it if you checked it out.
[2158.38 → 2162.70] Now, be sure you have a podcasting 2.0 app and then search for Jupiter Station.
[2162.70 → 2173.32] You can catch Coda Radio and Linux Unplugged live when they are live and other live stream events, but also a rotation of new content, out takes and the weekly launch.
[2173.54 → 2177.46] You can tune in for exclusive live streams from Nixon as well when we hit the road.
[2177.90 → 2180.92] And it is a fully podcasting 2.0 feed.
[2181.12 → 2184.88] And that means you get to find out about a show going live within 90 seconds.
[2185.34 → 2187.64] We'll have transcripts and chapters when they're posted.
[2187.88 → 2190.98] And yeah, we'll finally have live item support.
[2190.98 → 2198.32] So go check out the weekly launch on Jupiter Station and then stick around for all the content coming to Jupiter Station as we hit the road to Nixon.
[2198.82 → 2206.66] Just search for Jupiter Station or you can put jupiterstation.live.rss in your player of choice.
[2207.50 → 2211.54] That's jupiterstation at jupiterstation.live.rss.
[2211.54 → 2217.76] Scale is fast approaching Southern California Linux Expo.
[2217.96 → 2221.62] But during that event are several other sub events.
[2222.00 → 2226.24] And the one I'm the most interested in is Nixon America.
[2226.88 → 2227.10] Yes.
[2227.20 → 2228.26] And it's the first.
[2228.46 → 2231.80] And they've just posted today as we're recording the schedule.
[2231.80 → 2236.62] I haven't gone through it completely, but I already see a couple of talks that I know I'm going to want to attend.
[2237.20 → 2240.32] So that runs alongside scale, like you said, March 14th to the 15th.
[2240.66 → 2243.54] Scale itself goes from the 14th to the 17th.
[2243.76 → 2247.10] And there is like a small ticket entry price.
[2247.26 → 2251.68] But if you use the promo code JBFTW, one word, it'll take 50% off.
[2252.06 → 2254.26] You will need a scale pass to get into Nixon.
[2254.82 → 2256.78] I am so excited about this.
[2256.90 → 2258.02] You're going to be there, right, Alex?
[2258.04 → 2258.62] You're going to make it?
[2259.04 → 2259.76] Yeah, I think so.
[2259.76 → 2264.64] So Tail scale have a booth, so I think I'll be there in official capacity as well as a JB capacity.
[2265.34 → 2272.04] In fact, between scale and Linux Fest Northwest and Texas Linux Fest, I've got a busy spring coming up.
[2272.74 → 2273.22] Yeah, we do.
[2273.46 → 2274.94] We're just going to basically be hanging out.
[2275.06 → 2277.80] We're going to be seeing each other in person more than we do remote shows.
[2277.86 → 2278.58] It's going to be great.
[2279.04 → 2283.54] And we will have more meetups announced soon for scale.
[2283.62 → 2286.66] We're just trying to get a sense of what the Nixon schedule was, and we have that now.
[2286.66 → 2294.20] So probably, you know, the next week or two, meetup.com slash Jupyter Broadcasting will have details of meetups in the Pasadena area.
[2294.68 → 2296.28] We'd love to see you guys there.
[2296.66 → 2297.50] Pasadena's so nice.
[2297.58 → 2301.34] We haven't been there since we did the tour of JPL a couple of years ago.
[2301.40 → 2301.92] That was awesome.
[2302.34 → 2304.16] I know, and it's been years since I've been to scale.
[2304.46 → 2306.80] Very much, very much looking forward to all of it.
[2306.88 → 2307.72] It's been my first one.
[2307.98 → 2308.44] Oh, cool.
[2309.26 → 2311.80] Well, I think you'll be impressed with the size of it.
[2312.36 → 2316.06] All right, well, we got some great boosts into the show that help support each production.
[2316.30 → 2321.36] And our baller came from Anonymous this week with 1, 2, 3, 4, 5, 6 SATs, a Space balls boost.
[2321.96 → 2324.16] And says self-hosting is king.
[2324.40 → 2326.42] Keep up the amazing work from Pod verse.
[2326.96 → 2327.42] Thank you.
[2327.82 → 2329.50] Thank you for the great support.
[2329.72 → 2332.62] Anonymous, whoever you are, our mysterious benefactor.
[2332.62 → 2336.88] Tom's dad came in with 54,321 SATs.
[2336.92 → 2341.30] And he echoed a question that I totally dropped the ball on.
[2341.36 → 2345.52] That, by the way, is a reverse Space balls boost, which is, that's clever, 54, 3, 2, 1.
[2346.08 → 2351.94] He says, Chris, do you have any pointers on your tail scale container, no reverse proxy config that you were talking about in the last show?
[2352.22 → 2353.60] It sounded fascinating.
[2354.08 → 2360.12] And, of course, several other people boosted in, like Shaw and others emailed in asking for that same thing.
[2360.20 → 2361.32] And that was really my bad.
[2361.32 → 2363.48] I can't believe I didn't link that in the show notes.
[2364.14 → 2366.40] Tom's dad came back, though, with one that he found.
[2366.48 → 2367.14] So we'll link that.
[2367.26 → 2371.30] And I have one that I found that I used originally that I will link in the show notes this time around.
[2371.92 → 2380.98] And fear not, dear listeners, this was, you know, as a man in the content space these days, I noticed that there were a lot of these feedback things coming in.
[2381.24 → 2382.54] And don't worry.
[2382.68 → 2384.82] I will make some videos on the tail scale YouTube channel.
[2385.02 → 2388.88] And you can nerd out with me about tail scale and Docker over there.
[2388.88 → 2393.00] I think it deserves wider appreciation, the concept.
[2393.40 → 2411.48] I think where it gets tricky, I was having this conversation on the Matrix, does I think if I wanted to do one Docker file with five or six different services or applications in there, how to get all of them to show up as individual application names on a tail net, I think would take a little more work than what I'm doing now.
[2411.48 → 2414.72] The short answer there would be sidecar containers.
[2415.08 → 2419.84] So you spin up six tail scale containers alongside the other six services.
[2420.16 → 2424.22] And then just each sidecar container becomes a node on your tail net.
[2424.42 → 2429.36] And you give it a host name, you dock a compose file or rename it in your admin console.
[2429.88 → 2432.68] And then if you use auth keys, you don't need to log in manually.
[2432.68 → 2438.88] You can just have them automatically appear with specific tags if you want to, because you can tag the auth keys, that kind of stuff.
[2438.96 → 2439.24] Don't worry.
[2439.42 → 2443.60] We'll go into all this detail on the official video when I get around to making it.
[2444.04 → 2444.58] Looking forward to that.
[2444.84 → 2447.52] He also wanted to give you, Tom's dad wanted to give you a shout-out.
[2448.38 → 2448.82] He says,
[2448.82 → 2454.76] I cargo cultured his public Nix config as the starting point for my Mac and Home Lab config.
[2455.32 → 2460.84] I absolutely had no idea what I was doing, but I managed to get it working and a successful starting point for my Nix journey now.
[2461.24 → 2469.54] I've since layered on Nix Anywhere and Nominate, as well as replacing my pie hole with vanilla DNS mask install with Steve Black host lists.
[2469.94 → 2471.20] And he links to the Steve Black host.
[2471.66 → 2473.84] He says, you guys should start a Nix podcast as well.
[2474.76 → 2475.78] Oh, maybe we should.
[2476.10 → 2476.28] Yeah.
[2476.28 → 2480.76] Honestly, I think you've probably overtaken me, Tom's dad, at this point.
[2481.02 → 2485.42] I went all in for a little while on Notifying my Mac setup.
[2486.14 → 2493.14] And then I wrote a bunch of stuff for Perfect Media Server in the kind of future tense about, oh, this would be interesting to do one day.
[2493.48 → 2496.04] And I haven't done anything with it since then, if I'm honest.
[2496.48 → 2498.66] So you probably at this point are ahead of me.
[2499.04 → 2500.52] But thank you for writing in.
[2500.58 → 2501.84] I really appreciate the feedback.
[2502.36 → 2502.54] Yeah.
[2502.68 → 2503.70] Well, great work.
[2503.70 → 2504.56] That's what I say.
[2504.64 → 2505.40] I say great work.
[2505.40 → 2505.70] Yeah.
[2506.20 → 2507.92] Farskapian comes in with 50,000 SATs.
[2508.02 → 2512.42] He wants to point us to a project of his called Sovereign-Stack.org.
[2512.90 → 2515.40] He says it's an Oculus Docker Bitcoin project.
[2515.98 → 2516.30] Interesting.
[2517.12 → 2518.36] Thank you for letting us know about it.
[2518.56 → 2519.44] I'll take a look at it.
[2520.30 → 2521.88] Eric D came in with 50,000 SATs.
[2521.96 → 2524.12] He says, all right, guys, I got a goal for 2024.
[2524.36 → 2528.04] It's to boost the show at least once a month as a sort of value for value membership.
[2528.04 → 2532.48] My project over the holidays was spinning up a dedicated server for Image.
[2532.62 → 2533.48] Hey, hey, hey.
[2533.90 → 2535.68] That is hosted by a cloud provider.
[2535.90 → 2542.00] I've been hosting it locally for a while now, but I want to be able to share videos with family, and my ISP upload isn't fast enough to support that.
[2542.00 → 2558.62] That being said, cloud server storage is pricey, and 4K iPhone videos are huge, so I'm experimenting with Back blaze B2 and R clone with local caching to mount B2 as the library file system for Image, at least until Image supports object storage directly.
[2558.62 → 2562.24] So far, so good, although I still have much testing to do.
[2562.52 → 2563.44] Thanks for the great show.
[2563.76 → 2566.82] Residential upload speeds are the bane of my life.
[2567.04 → 2574.98] I just wish, I just wish, for all of you guys out there on symmetrical gigabit fibre connections, I am jealous.
[2575.34 → 2578.18] I'll just, that's the safe for work version.
[2578.54 → 2579.78] I am jealous of you all.
[2579.78 → 2580.30] No kidding.
[2581.08 → 2586.54] Because, you know, if everybody had that situation, it would make a lot of self-hosting problems just kind of vanish.
[2586.98 → 2594.30] You do have some concerns around residential reliability for things like power outages, as well as obviously ISP outages.
[2594.56 → 2603.56] You know, one of my friends today who lives pretty close and has Google Fibre, which I can't get, he had an outage where none of his Google products would resolve DNS.
[2604.04 → 2604.98] Everything else worked.
[2605.10 → 2606.50] Like, he could still slap me and stuff.
[2606.96 → 2607.48] How ironic.
[2607.48 → 2608.10] Yeah, I know.
[2608.16 → 2609.38] I just found that one pretty hilarious.
[2610.30 → 2614.26] Yeah, I mean, there is a lot to consider when hosting these services at home.
[2614.48 → 2615.76] You know, have you got a UPS?
[2615.76 → 2618.56] Yes, how many internet connections is the right number?
[2618.64 → 2621.30] Do you need a backup WAN connection, you know?
[2621.62 → 2626.20] You know, but that upload issue is what I like about having an image locally.
[2626.28 → 2626.64] Oh, yeah.
[2626.78 → 2629.70] Because when I upload from my phone, it's just blazing fast.
[2629.96 → 2630.18] Yeah.
[2630.30 → 2632.66] Whenever I travel, I think, oh, God, this is slow.
[2632.70 → 2634.06] And then I realize actually what's happening.
[2634.16 → 2635.58] And then I think, actually, no, it's not slow.
[2635.58 → 2644.28] Yeah, although I have also considered using Back blaze B2 and R-Clone and doing kind of that same exact setup, Eric.
[2644.44 → 2647.50] So I'm very interested in a follow-up boost to know how that's going.
[2647.68 → 2647.98] Yes, please.
[2649.02 → 2654.28] That's a – because the cloud – large cloud storage is a huge issue.
[2654.28 → 2660.24] Well, rumour has it is that Hetzner have a few extra boxes available these days after they kicked all the Plex boys off, you know?
[2660.24 → 2665.72] Scott came in with a couple of ROA ducks, 4,444 SATs.
[2666.28 → 2670.38] And he wants us to know that he's been using Git T to sync his Obsidian vaults.
[2670.74 → 2672.84] The plugin lets him commit and push automatically.
[2673.22 → 2678.76] And conflicts are usually due to like a small set of config files in the workspace.Jason.
[2679.32 → 2681.08] But he puts that in Git ignore to solve that.
[2681.08 → 2687.46] He also would like to know what tools we use to diagnose failed hard drives.
[2687.58 → 2687.82] A hammer.
[2688.16 → 2689.04] I was going to say that.
[2689.04 → 2691.74] Once it's failed, what's the point?
[2692.22 → 2693.54] If it's dead, it's dead, right?
[2694.06 → 2697.88] But if it's not dead yet, you want to catch it before it dies, right?
[2698.00 → 2700.70] Yeah, I give hard drives precisely zero chances.
[2701.28 → 2708.14] As soon as I see any reallocated sectors, or I notice any kind – like if I'm in the basement, you know, getting the lawnmower out or something,
[2708.14 → 2710.60] I hear a noise that I shouldn't hear.
[2710.70 → 2713.74] I'll then go into like Sherlock Holmes mode, you know?
[2714.24 → 2718.72] I've just been bitten one too many times of leaving it just a little bit too long.
[2718.72 → 2728.30] I would rather spend a bit more money and replace the drive before I strictly need to than go through the hassle of trying to recover any data off of a drive that is actually toast.
[2728.76 → 2734.46] I'm in the process of scrambling right now because I use a tool which I totally recommend called Scrutiny.
[2734.46 → 2736.96] It's really easy to get running, just a little Docker Compose.
[2737.58 → 2741.50] And I've got three different drives that are kicking airs right now.
[2741.56 → 2742.22] All at once.
[2742.36 → 2743.10] All at once.
[2743.46 → 2745.38] See, this is exactly what I'm talking about.
[2745.46 → 2754.30] When I talk about replacing a couple of drives every year because you are now at the other end of the bathtub curve, right?
[2754.30 → 2760.06] So typically when I do the burning stuff, I'm talking about getting over the initial hump whilst you're still in the retailer's return period.
[2760.38 → 2768.36] You at seven years, my friend, are now at the other end where most of these hard drives are warranted at most for five years,
[2768.46 → 2771.84] which tells me that's the confidence level the manufacturers have in them.
[2772.52 → 2776.88] And so anything other than five years in my infrastructure – in fact, this is what happened in my UK server.
[2776.88 → 2780.78] They got to six years, and they all went bang all at the same time.
[2781.14 → 2782.50] And look what's happening to you.
[2782.80 → 2784.24] So don't be like me.
[2784.34 → 2785.16] Don't be like Chris.
[2785.72 → 2786.08] No.
[2786.50 → 2787.76] And I'm scrambling right now.
[2787.82 → 2793.78] And, of course, just because of the hardware I have, the data – when I am moving, I'm moving it over to a system that has drives all at the same age.
[2794.18 → 2795.84] And it's just not the way to go.
[2796.04 → 2796.36] It's not.
[2796.62 → 2798.78] But we make do with what we have, I suppose.
[2798.80 → 2799.60] Never mind boosts.
[2799.60 → 2800.94] People just need to send you hard drives.
[2803.80 → 2805.88] Thank you, everybody who supports the shows with the boost.
[2805.88 → 2811.20] We got some extra nice shout-outs, too, just because self-hosted has been slightly frostbitten by the ad winter.
[2811.76 → 2813.68] So Word sent in 48,000 SATs.
[2813.76 → 2818.30] So did Mc Zip, 25,000 SATs and 25,000 SATs from Rotted Mood, too.
[2818.96 → 2821.20] We have a bunch more boosts, though, that are in the boost barn.
[2821.44 → 2822.62] We'll have that linked in the show notes.
[2822.74 → 2824.00] 13 boosters in total.
[2824.14 → 2824.74] And get this.
[2824.96 → 2829.12] We stacked 420,011 SATs.
[2829.50 → 2830.34] Thank you, everybody.
[2830.48 → 2831.70] I really appreciate that support.
[2831.70 → 2836.78] I've been taking my share of the SATs, and I'm putting it towards our trip to scale as well.
[2836.96 → 2838.78] So very much appreciate that.
[2838.84 → 2844.04] If you'd like to boost in, go get a new podcast app and then subscribe to the Self-Hosted Show and boost in.
[2844.08 → 2846.00] We'll have links in the show notes that makes it real easy.
[2846.08 → 2847.64] Or you can just bypass that.
[2847.84 → 2851.10] If you'd like to just set it and forget it, you can become one of our Sees.
[2851.74 → 2852.22] That's right.
[2852.26 → 2854.86] We have a membership program, self-hosted.show.SRE.
[2854.86 → 2859.40] And as a thank you, we give you an ad-free feed and a little extra content.
[2859.62 → 2860.56] We give you the post show.
[2861.12 → 2861.58] Yeah, we do.
[2861.96 → 2864.26] I've started journaling this week.
[2865.14 → 2871.18] I've been watching maybe one too many January productivity YouTube gurus and thought I'd give journaling a go.
[2871.24 → 2873.16] So we're going to talk about that in today's post show.
[2874.04 → 2877.26] Self-hosted. Show slash contact is the place to go to get in touch with us.
[2877.34 → 2879.06] Though, of course, many of you know that already.
[2879.58 → 2882.12] You can find me over at alex.ktz.me.
[2882.12 → 2886.04] A bunch of links over there for where you can find all the various things I'm up to on the internet.
[2886.52 → 2888.66] Why not check out chrislass.com?
[2889.14 → 2892.96] I'm just going to try plugging Foster once or twice.
[2893.08 → 2899.26] I'm not really using it, but I thought maybe instead of sending people to Weapon X, I'll try Foster.
[2899.38 → 2902.10] So I set chrislass.com to point to my Foster profile.
[2902.10 → 2904.64] Oh, and there's a Levi right at the top.
[2904.90 → 2905.24] Oh, yeah.
[2905.66 → 2906.10] Oh, yeah.
[2906.12 → 2906.84] I love the Levi.
[2907.02 → 2907.96] I love tweeting about the Levi.
[2907.98 → 2910.26] We can't convince you to come over to that Mastodon yet, no?
[2910.26 → 2915.26] Well, I'm on Mastodon, but I use it for like just podcasting stuff with other podcasters.
[2915.38 → 2917.44] I've kind of niched down on Mastodon.
[2917.76 → 2919.78] But I do see there's a lot of good stuff going on over there.
[2920.32 → 2922.82] Though the pod is on Weapon X at Self-hosted Show, of course.
[2923.16 → 2923.78] So we're still over there.
[2924.12 → 2925.78] How is that website still going?
[2926.78 → 2928.24] Anyway, thanks for listening, everybody.
[2928.42 → 2930.72] That was self-hosted. Show slash 115.
[2930.72 → 2932.14] Bye bye.
[2932.14 → 2932.58] Bye bye.
[2932.58 → 2932.60] Bye bye.
[2932.68 → 2933.12] Bye bye.
[2933.78 → 2933.80] Bye bye.
[2934.40 → 2934.72] Bye bye.
[2934.78 → 2934.82] Bye bye.
[2934.82 → 2935.34] Bye bye.
[2935.36 → 2951.50] Bye bye.
[2952.02 → 2952.48] Bye bye.
[2952.60 → 2954.90] Bye bye.
[2954.92 → 2956.98] Bye bye.
[2957.14 → 2959.12] Bye bye.
