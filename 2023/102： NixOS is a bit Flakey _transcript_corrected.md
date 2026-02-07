[0.00 → 5.62] I'm really curious to know what your process is when something dies in your home automation setup.
[5.86 → 14.34] You know, one of these annoying things like a controller going out or a light bulb stopping working or, you know, something like that where it just falls off the Wi-Fi for no reason.
[14.34 → 17.88] And you're just like, oh, I've got to go and investigate this.
[18.06 → 18.72] What now?
[19.68 → 23.66] Yeah, that is inevitable when you have more and more devices.
[23.66 → 34.48] And, of course, these days, if I was going to deploy like an LED light strip or a temperature sensor, I would get a little ESP, put ESP home on there.
[34.48 → 41.62] You know, I would build it modally, and then I would just replace like the light strip if that died or just the controller if that died.
[41.92 → 46.08] But, you know, past Chris didn't really think that way.
[46.36 → 48.52] And I'll give you an example that just happened to me recently.
[48.70 → 51.58] I love these Li Fix light beam bars.
[51.58 → 57.74] They're these bars that are magnetic, and you can connect like up to multiple pieces and make shapes and whatnot.
[57.96 → 59.12] And they're great for the bedroom.
[59.24 → 60.18] They're great for the living room.
[60.24 → 64.74] They're just great products, except for they have a proprietary controller.
[64.86 → 66.64] And I don't think they even make it anymore.
[66.92 → 68.82] So go figure.
[68.90 → 70.02] One of ours died recently.
[70.02 → 74.64] I had to go on to like eBay and go buy a used controller so I could replace mine.
[74.64 → 77.28] And, of course, I've got this light because it's our it's our headboard.
[77.28 → 82.18] I've got this light in a couple of different scripts, multiple automations.
[82.62 → 85.46] I don't want to like to come up with a new name and then go change everything.
[86.10 → 91.54] So I have to go through this process with the Li Fix stuff where you join to its Wi-Fi on your phone.
[91.62 → 93.72] You use their little app to set it up initially.
[93.88 → 95.20] You get it on your Wi-Fi network.
[95.58 → 98.24] Then Home Assistant will detect it if you have the Li Fix integration.
[98.24 → 106.62] And what I do is before I take that step, and I'm curious to know if the audience out there has a better way to do this, I go rename the dead one.
[107.20 → 111.96] So I'll do like old underscore headboard light or whatever it might be.
[112.56 → 114.18] And I'll make sure I update that.
[114.28 → 120.32] And sometimes I'll even restart Home Assistant because I've noticed when I rename devices, it's not necessarily represented everywhere right away.
[120.32 → 122.66] And so I'll sometimes even restart Home Assistant.
[123.20 → 130.84] Then I will at that point when it detects the new light bar controller, I then go in there and add it and I give it the name of the old one.
[130.96 → 132.48] And that seems to work.
[133.14 → 134.22] I don't do it a lot.
[134.32 → 136.80] So I don't know if I could recommend it as the official process.
[136.94 → 137.80] Maybe there's a better one.
[138.30 → 142.98] I would love just to like a replace device option because these things inevitably die.
[142.98 → 152.02] Or I'd like to like to have like a hide when device doesn't respond because another one is I have smart plugs for Christmas decorations.
[152.44 → 157.66] I don't leave them plugged in throughout the year when we don't have Christmas decorations up.
[158.00 → 162.74] So I just in my main dashboard where I have all my devices, I just have these airs.
[163.36 → 164.40] You know, things are airing out.
[164.44 → 165.92] It just drives me crazy to see it.
[166.32 → 168.32] I'd love a hide when inactive kind of thing.
[169.02 → 170.38] But yeah, that's my process.
[170.58 → 171.50] I don't know if it's great, Alex.
[171.50 → 178.70] Well, whilst you were talking, I was sort of thinking, wouldn't it be great if there was just a single pane of glass with all of my entities in it?
[179.44 → 183.00] But then I got thinking that exists, that must exist in the interface.
[183.00 → 184.16] So I went digging.
[184.72 → 188.28] And on the integrations page at the top, there are four little buttons.
[188.62 → 190.86] And one of them turns out is devices.
[191.30 → 192.74] Another one is entities.
[193.50 → 200.74] So under that menu, there is an easy way to get into all the different names and sensors.
[200.74 → 202.54] And all the rest of it that you've got.
[203.98 → 211.94] However, you know, if I just take, for example, our Mazda is a 2022 model.
[212.10 → 214.94] So it's got a modem in it for some reason.
[214.94 → 219.18] And I connected it into Home Assistant so I could look at how much petrol was in the tank.
[219.94 → 230.80] And if I look at this thing, it's got, it must be at least 15 or 20 entities all part of this same vehicle or the same connected service.
[230.80 → 242.46] And when you go in and try and figure out which of these entities, because I mean, you know, a Philips Hue motion sensor, for example, also has a temperature and humidity sensor in it.
[242.50 → 249.18] So it's not uncommon for one entity to actually have five or 10 related things.
[249.18 → 259.32] So if I just click on one of these items, I can, of course, go to the related option in the Home Assistant interface and look at all the related entities.
[259.32 → 261.42] But it's not an editor that I'm in there.
[261.78 → 276.14] So I guess what I'm kind of pitching here is some kind of spreadsheet-issue entity editor that I could just actually go in and update in real time all the device names and get everything just formatted correctly.
[276.14 → 290.14] Right. You know, that was one of the reasons, one of the times I had to redo Home Assistant, I was sort of reluctantly grateful because, you know, the first time around using Home Assistant, I just took all the default names that it just auto-generates for stuff.
[290.44 → 297.30] And that was a nightmare when I had six or seven sensors that all essentially have the same name with a one, two, three, four affixed to them.
[297.60 → 302.26] And, you know, my life was so much easier when I realized I could go in there and name them something that made sense to me.
[302.26 → 311.88] But it was, like you said, those so many entities, my sensors, each sensor has seven or eight entities, maybe nine entities that it adds to Home Assistant.
[312.60 → 313.46] It was a nightmare.
[313.72 → 319.98] And so some way to just, like, if you could go to that entities or device screen and just go into mass edit mode, and you're right.
[320.00 → 325.58] If it just turned into editable fields where you could go in there and just change names, and it would update, that would be magic.
[325.58 → 336.94] Like, one nice thing they've added in the last year or so is if you go to the device, and you rename it at its main device screen, it will prompt you if you want to rename all the entities, too.
[337.04 → 341.58] So you can do it one-off like that, which is what I do when I'm renaming them to, like, the old device.
[342.42 → 345.00] Well, that's what I've been messing around with these last few days.
[345.12 → 347.60] But you have news of another variety, don't you?
[347.60 → 348.24] I do.
[348.46 → 351.18] I am unemployed officially as of this recording.
[351.86 → 353.84] I have no current employer.
[353.84 → 358.32] Yeah, I mean, I think for as long as I've made it.
[358.32 → 360.78] You were just getting the job at Red Hat, maybe, when I met you.
[360.90 → 361.80] Was that how it was?
[362.28 → 363.18] Something right around then.
[363.52 → 366.22] So it's been five and a half years, if you can believe it.
[366.38 → 366.60] Yeah.
[366.90 → 370.10] Obviously, this show has only been going, what, four or so?
[370.24 → 371.92] Coming up to four in September, I think.
[372.94 → 381.92] So, yeah, I guess that year that you and I first met Texas Linux Fest, the year before that, I was probably fairly new in my first year or so.
[382.36 → 383.24] Okay, okay.
[383.24 → 383.32] Yeah.
[383.62 → 385.88] But, yeah, it was just time for a change, really.
[386.16 → 388.24] You know, five and a half years at the same company.
[388.58 → 396.08] I started as an infrastructure consultant in the UK, and that was fine, but there was just too much travel in that role.
[396.20 → 399.78] And we were looking to emigrate anyway, so it was actually a perfect excuse.
[399.78 → 405.20] And I found an OpenShift TAM job dealing with commercial customers.
[405.20 → 407.44] So that meant that we moved to Raleigh.
[407.44 → 414.88] Even though it was a fully remote position, just having the Red Hat Tower just there, HQ there, I figured would be a good career move.
[414.88 → 421.08] Whenever anybody came to the Tower for a meeting or whatever, I could hang out and get FaceTime and all the rest of it.
[421.08 → 429.14] And, you know, with COVID, that actually, I mean, for the first year or two, it was a really, that bore out to be fairly true.
[429.14 → 436.36] But after COVID, I've been to the Tower, I don't know, twice this year, maybe, three times at most.
[436.68 → 437.42] And I'm not alone.
[437.56 → 439.44] They've closed a few floors of the building.
[439.44 → 443.64] It's just a shadow of what it was before COVID.
[443.94 → 449.76] So being in Raleigh for Red Hat lost a lot of its benefits, I suppose.
[450.96 → 453.12] So I wandered around within that role for a little while.
[453.18 → 457.66] I was made senior, and then I moved over to the partner account team from the commercial side.
[457.96 → 465.60] But more recently, I took a cloud success architect role, and that was to aid customers adopting OpenShift in the cloud and that kind of thing.
[465.60 → 472.58] However, right around that sort of time, three or four months ago, was when Red Hat announced the first round of layoffs.
[473.32 → 475.78] The mood in the company really changed after that.
[476.02 → 479.82] I can't, if you're not a Red Hatter, it's hard to explain.
[480.04 → 484.26] But people talk about the Ramification of Red Hat and stuff like that.
[484.34 → 487.72] And for the most part, it's just hype in the media.
[487.82 → 488.96] It doesn't really exist.
[488.96 → 496.26] Of course, there are higher level objectives from, you know, financial targets and stuff like that that will come down from upon high.
[497.04 → 502.96] But in the day-to-day side of things, we've been largely left alone until these layoffs.
[503.72 → 506.22] Now, I'm not saying IBM had anything to do with them.
[506.40 → 509.22] In fact, we've been told categorically that they did not.
[509.22 → 516.24] However, for me, it was just a shot across the bowels to say, OK, let's see what else is out there.
[516.56 → 520.56] And I actually posted on Twitter to say, hey, is anybody hiring?
[521.10 → 525.84] And someone from Tail scale reached out and said, yeah, we're hiring.
[525.90 → 527.60] You should apply to come work at Tail scale.
[528.46 → 530.64] So that's what I'm going to go and do.
[532.40 → 533.36] That's pretty great.
[533.44 → 534.84] I mean, we're huge fans of Tail scale.
[534.84 → 534.96] Tail scale.
[535.64 → 540.28] So, you know, there are a handful of companies I'd be up for working for and Tail scale is probably one of them.
[540.98 → 543.98] And it's a totally different kind of shift for you, right?
[544.60 → 546.04] Red Hat's a very large company.
[546.16 → 549.38] Tens of thousands of staff and contractors.
[549.74 → 551.96] And Tail scale is at a totally different end of the spectrum there.
[552.32 → 558.00] Well, when I joined Red Hat, it was around 11, 12, 13K, something like that, employees.
[558.34 → 562.12] I think they're at like 22,000, 23,000 now.
[562.12 → 564.26] So, I mean, the growth has been spectacular.
[564.84 → 568.98] And I don't know if it's true, but I've heard it's north of 40 if you add contractors.
[569.58 → 570.86] I couldn't comment on that.
[571.20 → 575.04] But in terms of Red Hat, certainly, it's almost doubled.
[575.28 → 578.66] Well, I guess it pretty much has doubled in the last five years or so.
[578.76 → 579.24] Yeah, crazy.
[579.40 → 581.96] But Tail scale is a team of about 100 people.
[582.06 → 586.98] So it's about as different as it could possibly be if it was just me and someone sat in a room with a laptop.
[587.32 → 588.86] Do you know if anybody else works in Raleigh?
[588.86 → 592.56] There is a chap who is just moving from DC locally.
[592.78 → 595.36] I'll spare his identity for now in case he doesn't want me to say.
[595.50 → 597.46] But yes, there is someone else in Raleigh.
[597.52 → 598.14] So that's nice.
[598.92 → 603.18] I just wanted to say as well, I've had folks ask me on Twitter and stuff like that if I was laid off.
[603.38 → 604.74] No, not at all.
[604.84 → 606.16] It was completely my decision.
[606.64 → 609.50] More so that this was just an opportunity that was so good.
[609.50 → 610.88] I couldn't really pass it up.
[611.04 → 614.42] So I'm going to be working over there as a developer advocate.
[614.42 → 623.42] So writing blog posts, dealing with YouTube stuff and videos and documentation and outreach to various different teams and stuff like that.
[623.42 → 631.20] And it's basically taking what I've been doing as a side hustle and turning it into Bobby job.
[631.76 → 636.16] And I'm really excited to exercise that creative muscle professionally.
[636.42 → 637.48] It's not something I've done before.
[637.48 → 643.20] And just totally selfishly, but you're probably going to get more opportunities to meet up with self-hosted audience too.
[643.52 → 645.70] I will, starting almost right away.
[646.22 → 651.98] Because DevOps Days in Chicago is coming up on August the 9th and 10th.
[652.08 → 653.78] And I will be there with Tail scale.
[654.44 → 659.68] So if you're in the area, I don't know what the details are going to look like for a last minute meetup.
[659.88 → 662.06] But it will either be the Tuesday or the Wednesday evening.
[662.06 → 667.56] I need to actually start working for the company next week before I can find out those details.
[668.10 → 673.58] And then I'll post something on the meetup page, and we'll mention it in the various shows that we can.
[673.90 → 676.44] I don't think this show will be out again before then, maybe.
[676.66 → 677.24] I don't know.
[678.04 → 679.94] But yeah, keep an ear to the ground for that one.
[680.16 → 683.32] And maybe we'll just go to find a bar and get a couple of beers or something.
[683.38 → 683.90] Nothing crazy.
[684.58 → 685.70] Oh, I wish I could be there.
[686.12 → 687.04] Well, congratulations.
[687.50 → 688.86] That's exciting news.
[689.30 → 692.98] And I am really kind of looking forward to seeing where things go.
[693.08 → 695.78] Because I think Tail scale's got a bright future ahead of them.
[695.86 → 697.10] You're going to be riding that wave, Alex.
[697.44 → 698.48] Startup life, baby.
[698.70 → 701.50] I am basically Ehrlich Barman personified.
[703.92 → 704.94] Yeah, all right.
[704.94 → 710.90] Well, let's talk about a company that is in a different phase of life where things aren't going so well.
[710.96 → 713.30] Some of us are just running away from Reddit these days.
[713.90 → 716.44] I don't know about you, but it's just not the same anymore.
[716.70 → 720.04] And there's perhaps better self-hosted ways to replace Reddit.
[720.48 → 721.90] Yeah, we've all known.
[722.12 → 726.76] We've all been using Reddit for years and thought, what happens when this goes away?
[727.80 → 735.04] And for me, the iOS client Apollo stuff and the boot and, you know, the API debacle that we've talked about before.
[735.64 → 742.92] That was enough of a push for me to be like, okay, I am done investing time and energy into this platform.
[742.92 → 750.56] It's still obviously useful as a resource of human knowledge, but that's going to decay pretty fast if people start leaving the platform.
[750.56 → 753.08] So it's going to be interesting.
[753.46 → 755.92] But that has left me with a hole to fill.
[756.26 → 757.56] You know, the poop time.
[757.56 → 759.94] You've got to have something to read or do.
[760.48 → 763.20] There's only so many times you can text Brent and say, hey, how are you doing, bud?
[763.22 → 764.10] How's Berlin this week?
[764.62 → 772.90] And we came across Wallaby, which is an offline article reader in the style of something like Pocket or Installer.
[772.90 → 775.68] And, of course, you can self-host it.
[775.76 → 779.52] They do actually offer a hosted version.
[779.74 → 781.08] It's MIT licensed, though.
[781.18 → 783.70] There is some Docker Compose instructions available.
[783.70 → 792.26] And they make an API and remote connection method available for apps like Android or iOS apps, browser extensions.
[792.88 → 798.68] It's everything you would expect from something like Pocket, but perhaps more of a power user version of it, right?
[798.76 → 801.78] Because you get this API.
[802.38 → 805.00] There's a GNOME Read It Later app that plugs in with it.
[805.00 → 812.22] It feels like it both replaces Inboard and Pocket for me, which I use both.
[812.26 → 816.94] I don't know if you're familiar with Inboard, but I use both those right now as kind of way to save content for getting to later.
[817.30 → 822.40] The nice thing about Wallaby is how it presents the articles to you, just as basically tiles.
[822.76 → 826.24] You can also change the interface to be a list view, that kind of stuff.
[826.34 → 828.14] But it downloads things to be offline.
[828.54 → 830.74] So it saves the text of these articles.
[831.34 → 833.06] You can add things like tags.
[833.06 → 835.22] You can mark them as starred.
[835.48 → 838.52] You know, refetch the original content is another option that's in there.
[838.66 → 845.92] So if it's a, you know, heavy updating blog or, you know, something else, you could update the content that way.
[846.12 → 849.24] It's also got a jump to random button, which I really appreciate.
[849.40 → 854.08] So if you're not quite sure what you want to dig into at the moment, you just press the random button and off you go.
[854.72 → 856.26] So it works really nicely in the browser.
[856.62 → 858.28] No complaints there at all.
[858.28 → 863.42] But obviously the mobile experience is a huge part of why I'm looking to do this kind of stuff.
[863.56 → 869.26] So I ended up coming across a tangentially related project called Fresh RSS.
[869.84 → 878.06] And the reason I mentioned this is that Wallaby exposes the articles that you add to it as an RSS feed.
[878.06 → 884.94] So I can then bring that into my RSS reader, which is actually spelt R-E-E-D-E-R, the client on iOS.
[885.80 → 891.14] I can bring in my Wallaby feed as an RSS feed as my read it later queues.
[891.54 → 901.50] And so then I've got one place to go for all the tech blogs and all the software updates and GitHub release notes that I want to follow as part of the different feeds,
[901.64 → 905.78] as well as my cultivated list of read it later articles.
[905.78 → 907.82] That is really nice that it pulls it in there.
[908.26 → 914.12] Fresh RSS is my favourite of the self-hostable RSS applications out there.
[914.22 → 917.72] It turns 10 this year, which is really amazing.
[917.88 → 923.74] You can pop podcast feeds in there too, which I really appreciate because there are some podcasts I kind of follow a little more casually.
[924.10 → 926.00] And so it's kind of a great spot for it.
[926.06 → 928.70] And I suppose if you're on mobile, you could probably just play it right there.
[929.28 → 931.20] And of course, you can just pop in your OPML feed.
[931.20 → 936.56] So if you're using something like Feebly or another RSS app, you can throw it in there.
[936.72 → 942.50] And I seem to recall that the Linux server IO folks have a fresh RSS image.
[942.62 → 946.40] I'm thinking that's probably the one I deployed the last time I tried it.
[946.60 → 951.90] You know what's funny is as part of all this, you know, let's leave Reddit behind idea.
[952.06 → 955.14] I started looking at the awesome self-hosted list.
[955.18 → 959.22] And for some reason, I picked out TTRSS, which is tiny, tiny RSS reader.
[959.22 → 960.60] Right. I've used that too.
[960.92 → 966.80] And I spent, it must have been three hours going through the deployment of this thing.
[966.98 → 970.04] There are, it's just, it's so opinionated.
[970.40 → 981.88] It's, it's, this developer has basically said, unless you do things exactly my way, including using the hard-coded container names, this stack ain't going to start.
[982.02 → 988.34] And it's like, dude, the whole point of containers is to remove that it works on my machine problem.
[988.34 → 993.30] And, you know, apparently I posted on Mastodon a little bit about it, had a bit of a rant.
[994.44 → 999.84] It turns out that developer has some, shall we say, strong opinions about the world.
[999.84 → 1004.72] And he is not necessarily the most friendly, approachable chap.
[1004.92 → 1010.72] So I haven't personally dealt with that, but that's the reputation that the project has, unfortunately.
[1010.72 → 1019.08] So it was a it was really a breath of, no pun intended, fresh air when I started using fresh RSS because I used the Linux server image.
[1019.22 → 1022.56] And within literally two minutes, I had the instance up and running.
[1023.12 → 1025.42] It's just so nice when stuff like that works.
[1025.42 → 1030.38] That is, that is the peak self-hosted Docker compose experience.
[1030.38 → 1033.70] You know, you set up your compose file, you do your Docker compose up.
[1034.20 → 1039.26] And I always, the first time I run it, I always just leave the logs, the output right there on the command line.
[1039.42 → 1041.16] And just to see if there are any errors.
[1041.36 → 1047.18] And when it, when it's something simple, and it fires right up, you're just, well, wall bag is a little bit more involved.
[1047.18 → 1052.10] It's not as bad as tiny, tiny RSS, but it's, and it's not as simple as fresh RSS.
[1052.10 → 1055.12] And you don't necessarily need wall bag to use fresh RSS.
[1055.26 → 1057.52] You could just throw an OPML file in there and look at feeds.
[1057.74 → 1064.36] But the two together, I think are a really compelling combination because you can use one to capture and archive stuff.
[1064.36 → 1069.38] And the other than to review it later in an application of your choice that, you know,
[1069.40 → 1076.08] where developers spend a lot of time just refining that application to really view those feeds nicely and clever.
[1076.08 → 1079.02] And you can point pretty much any of those at fresh RSS.
[1079.28 → 1082.90] And so it's like the stack you've created here is like, it's three layers, right?
[1082.90 → 1084.40] Because you got wall bag for the capture.
[1084.60 → 1087.52] You got fresh RSS for reviewing that and other stuff.
[1087.52 → 1091.16] And then you need a perfect mobile RSS application.
[1092.06 → 1094.68] But there's plenty of those on both Android and iOS.
[1095.22 → 1096.96] So I mean, it's a pretty clever stack.
[1097.50 → 1102.44] Now out of the box, I ended up deploying both of these, I think, with the SQLite database.
[1102.78 → 1105.76] You can change that backend, particularly on Wallaby.
[1105.76 → 1108.08] It supports Postgres and MySQL as well.
[1108.96 → 1111.00] With fresh RSS, the deal is the same thing.
[1111.46 → 1115.04] SQLite by default, particularly in the Linux server image, just for ease of setup.
[1115.34 → 1121.82] But if you want to go in there and tune the Postgres or MySQL databases as well, you can also do that.
[1121.82 → 1127.58] So what you could potentially have is just one database container shared between these two apps, maybe, if you want to do that.
[1128.18 → 1132.78] Although the overhead of having a second container is so small, I might just do that anyway.
[1132.78 → 1135.00] But they do link really nicely together.
[1135.60 → 1141.86] The big thing that I'm missing at the moment from the Reddit days is not the quality of comments, I will just say.
[1141.96 → 1149.04] Because it's been a real shock to my system going back to purposefully written articles and blog posts.
[1149.58 → 1159.16] You think someone's put some time into crafting this thing versus a comment that someone's literally just sh**Ted out onto Reddit that's given three seconds thought.
[1159.16 → 1167.98] I mean, there are the odd exception on Reddit, of course, but the majority of it is just brain dumps into random comments and arguments and that kind of stuff.
[1168.98 → 1178.84] But along with that kind of brain dump, low quality comments, comes a lot of discovery, which I'm really missing from this solution at the moment.
[1178.84 → 1186.84] I'm having to actively go and seek out blogs and go and seek out content and stuff like that in a way I haven't had to for a decade.
[1187.58 → 1200.76] So if you have a list of your favourite blogs or something like that, I've been considering putting together a list on the self-hosted wiki of your favourite blog posts, of your favourite blogs and things that you follow.
[1200.76 → 1210.78] So in categories and that kind of stuff, I'm not quite sure the format it will take yet, but I'll try and seed that before this episode airs on Friday, just so that we can all get an idea of what to do.
[1211.36 → 1215.68] Open a PR, open a merge request, and we'll take a look at it and get it merged into the wiki.
[1215.68 → 1224.24] Linode.com slash SSH. Head on over there to support the show, get $100 in 60-day credit, and check out the exciting news.
[1224.72 → 1233.86] Linde's now part of Akamai. All the developer-friendly tools like the cloud manager that's beautifully built, the API well-documented with lots of libraries ready to go, and the CLI I use on the daily.
[1234.30 → 1238.68] The stuff I've used, and you've used to build, deploy, and scale in the cloud, that's all still available.
[1239.20 → 1242.88] But now, it's combined with Akamai's power and global reach.
[1242.88 → 1248.92] They are the top-tier network, and they're expanding their services to offer more cloud computing resources and tooling,
[1249.14 → 1256.08] but making sure you still get that reliable, affordable, and scalable solution for yourself or a business of any size.
[1256.38 → 1260.72] And as part of Akamai's global network of offerings, their data centres are expanding worldwide,
[1260.92 → 1266.64] giving you access to more resources so you can grow your project or your business and serve more customers and more clients.
[1267.14 → 1270.52] So why wait? Go experience the power of Linde. Now, Akamai.
[1270.52 → 1277.28] Visit linode.com slash ssh. Go there to learn how Linde, now Akamai, can upscale your applications from the cloud to the edge,
[1277.44 → 1280.46] and you'll get $100 in 60-day credit while you support the show.
[1280.76 → 1282.90] It's a pretty sweet deal, and you can really kick the tires.
[1283.08 → 1285.50] Linode.com slash ssh.
[1287.68 → 1290.02] Anybody know Dust?
[1290.02 → 1294.34] Dust. This is an old one. That's a deep pull for some of the UK audience there.
[1294.76 → 1303.58] But I found an app recently called Dust, and this builds itself as a more intuitive version of DU in Rust, of course.
[1303.70 → 1305.70] We need the theme tune at some point.
[1306.30 → 1309.04] Was is going to come riding over the horizon.
[1309.48 → 1309.68] With the horns.
[1309.68 → 1314.58] That would be so great. That would be so worth it.
[1315.04 → 1316.84] I like the visual layout of this.
[1316.92 → 1323.18] I mean, first, these are really handy on the command line because I'm often shying into my file server or my media server,
[1323.68 → 1327.24] trying to figure out what folders I can go trim from.
[1327.42 → 1332.48] And so this gives you a really nice tree layout on the left-hand side,
[1332.48 → 1334.94] and on the right-hand side, it gives you a bar graph.
[1335.64 → 1337.32] It's a nice way to lay it out.
[1337.32 → 1343.06] It is, and the way that I've been doing it for the last several years has been using CDU.
[1343.38 → 1346.96] And it's kind of slow to index files.
[1347.04 → 1350.16] You get the impression it's actually reading every single file one at a time.
[1350.58 → 1355.28] Which leads me on to my next pick, which is an app called DUE, Duff.
[1355.88 → 1362.20] This is Disk Usage Free Utility, which also bills itself as a better DF alternative.
[1362.20 → 1368.82] So DF and DU, those two tools are pretty much interchangeable to find out different amounts of file system usage.
[1369.52 → 1373.66] And the thing about Duff is it's unbelievably fast.
[1374.34 → 1380.86] And it outputs to JSON, which I wouldn't use, but I know there are guys out there that could actually,
[1381.02 → 1385.30] if you could take that storage data, output it to JSON, you could feed that into something useful.
[1385.30 → 1390.86] Well, some kind of alerting server or something like that, maybe Prometheus would chew that in and be like,
[1390.92 → 1394.12] hey, bud, you've only got 10% left on this disk.
[1394.20 → 1396.46] You should probably do something about that soon, eh, bud?
[1396.62 → 1397.22] Hey, hey, hey.
[1397.48 → 1397.98] Hey there, bud.
[1398.26 → 1401.44] You know, it's a funny thing to say, and you're going to have to just accept it.
[1401.70 → 1403.66] These command line apps have beautiful interfaces.
[1404.04 → 1408.78] This is a great example of super easy to read, glanceable information
[1408.78 → 1413.32] that anybody new or experienced could look at this and understand what it's telling you.
[1413.60 → 1415.00] And it's crazy fast, like you're saying.
[1415.34 → 1416.60] Yeah, yeah, it is.
[1416.72 → 1419.76] And, you know, one of the issues that I have with DF typically is,
[1420.42 → 1425.02] and I've written a bash alias, which removes a lot of these tempos devices
[1425.02 → 1426.78] and all the Docker volumes and that stuff.
[1426.98 → 1431.10] But when you type DF-H typically, is it DF-H?
[1431.50 → 1432.48] Yeah, for human-readable.
[1432.66 → 1436.26] You get this list of like 500 devices.
[1436.26 → 1439.96] I'm like, no, dude, calm down.
[1440.24 → 1445.02] I just want to see how much free space I've got on one of my hard drives.
[1445.38 → 1445.92] You know, I don't-
[1445.92 → 1447.22] It's so bad if you've got snaps too.
[1447.28 → 1449.70] If you've got a few snaps running, it's, oh.
[1450.12 → 1451.04] Yeah, terrible.
[1452.40 → 1455.06] Now, I mentioned CDU a couple of minutes ago.
[1455.32 → 1462.64] This app, D-U-A-C-L-I, Duchy, is a disk usage analyzer tool,
[1463.06 → 1466.04] which is, I know I said the last one was fast.
[1466.04 → 1467.62] In terms of glanceable information.
[1467.78 → 1470.30] But when you run this, like compared to CDU,
[1470.48 → 1474.38] it literally feels like, how could it possibly be done already?
[1475.04 → 1475.20] Yeah.
[1475.30 → 1476.46] It's like, does it already know?
[1476.78 → 1481.34] Yeah, I use this one on the regular because it is so dang fast.
[1481.46 → 1482.46] D-U-A.
[1482.76 → 1485.84] And also like 90% written in Rust.
[1486.12 → 1489.06] So these Rust apps are just ludicrous fast.
[1489.52 → 1490.60] Yeah, they really are.
[1490.60 → 1493.96] Now, I came across these things whilst I was browsing through,
[1494.10 → 1496.28] and this is going to be a trigger topic, maybe.
[1496.54 → 1496.92] We'll see.
[1497.18 → 1498.14] We'll see how it goes.
[1498.58 → 1500.86] But whilst I was browsing through Wimpy's world,
[1501.16 → 1504.58] he has posted his NixOS config.
[1504.82 → 1505.16] Oh, really?
[1505.30 → 1505.50] Okay.
[1505.50 → 1508.20] I looked at a bunch of the packages that Wimpy was using,
[1508.34 → 1509.94] and I found these apps in there, and I was like,
[1510.24 → 1512.46] oh, hey, I should try these things out.
[1512.92 → 1513.40] And...
[1513.40 → 1514.14] Oh, I do that too.
[1514.20 → 1516.30] I look at people's Nix config, and I find the apps,
[1516.36 → 1517.08] and I try them out.
[1518.06 → 1521.12] So I think I've seen the light in the last week or so with Nix.
[1521.38 → 1523.48] Now, tell me what the breakthrough is.
[1523.54 → 1525.10] Right, because we've talked about Nix a bit,
[1525.24 → 1527.28] and I'm curious to know what the shift was.
[1527.28 → 1531.82] I can define my entire system in one file.
[1533.28 → 1536.12] Two, technically, if you include the hardware config file.
[1536.48 → 1538.60] But I can read it in...
[1538.60 → 1542.08] It's glanceable, almost like some of the command line tools
[1542.08 → 1543.92] that we just mentioned.
[1544.48 → 1546.08] I can say, well, what are my users?
[1546.60 → 1548.88] What is my static IP configuration?
[1549.66 → 1551.74] What are all the packages on this box?
[1552.50 → 1555.76] The reproducibility angle doesn't really bother me that much,
[1555.76 → 1560.44] certainly not to the degree that I would pick Nix
[1560.44 → 1562.30] because of the reproducibility.
[1563.20 → 1566.54] But if I was a developer building development environments
[1566.54 → 1568.52] and that kind of thing, oh my goodness,
[1568.68 → 1570.94] this is like the best thing ever.
[1571.00 → 1572.56] This is what containers promised.
[1573.22 → 1577.90] But the entropy of, you know, apt repos even,
[1578.60 → 1581.92] you can't guarantee that building a 10-year-old software package
[1581.92 → 1582.82] is going to build today
[1582.82 → 1585.24] because some of the upstream dependencies
[1585.24 → 1586.24] will have gone away.
[1587.20 → 1589.98] And with Nix, they solve that by having a huge,
[1590.04 → 1591.70] what they call, mono repo
[1591.70 → 1596.24] with over 80,000 packages in a single repo.
[1597.04 → 1600.30] And they have every version of that package
[1600.30 → 1603.50] that's ever been made stored in that repo.
[1603.84 → 1607.22] It just boggles the mind how expensive that storage must be.
[1607.62 → 1607.94] I know.
[1607.94 → 1612.16] And what I love about it is it's allowed me to experiment
[1612.16 → 1615.32] with mixing stable and unstable versions.
[1615.56 → 1618.10] So, for example, if you wanted to,
[1618.18 → 1620.62] you could run a sort of rolling Nix OS
[1620.62 → 1622.30] by going completely unstable.
[1622.50 → 1624.36] But you could then say,
[1624.50 → 1626.64] but always give me Plasma that's stable
[1626.64 → 1628.70] or always give me stable Firefox.
[1628.98 → 1630.12] And you could also do the flip.
[1630.22 → 1631.94] You could have a completely stable system,
[1632.06 → 1634.12] but always have the unstable version
[1634.12 → 1635.64] of some of your favourite packages.
[1635.64 → 1638.18] And you can mix it and Nix just totally manages it.
[1638.60 → 1639.10] And as you know,
[1639.14 → 1640.84] and this is true for other systems as well,
[1640.90 → 1644.90] but what I love compared to say apt or DNF
[1644.90 → 1647.08] is if something's going to break,
[1647.14 → 1648.76] and I'm not just talking like at a package
[1648.76 → 1651.04] resolution dependency level,
[1651.04 → 1653.94] I'm like talking the configuration of the service
[1653.94 → 1655.38] that you're about to deploy as well.
[1655.46 → 1656.70] Like if something's wrong in the config,
[1657.04 → 1658.42] it will stop.
[1658.68 → 1660.62] And it'll give you the line number to go fix it.
[1660.78 → 1664.14] And so you catch stuff before you actually deploy it.
[1664.14 → 1666.96] And that is to me so nice
[1666.96 → 1668.42] because I can sit there,
[1668.46 → 1669.10] I can tweak it.
[1669.22 → 1670.12] Okay, does it build now?
[1670.24 → 1670.56] Oh, nope.
[1670.64 → 1671.34] Okay, I have to go fix.
[1671.42 → 1672.16] Okay, does it build now?
[1672.20 → 1673.04] Oh, okay, I got it.
[1673.06 → 1673.70] All right, now I know.
[1674.08 → 1675.58] And then when I'm working on my desktop,
[1675.70 → 1677.42] because I have it running on my desktops
[1677.42 → 1678.32] and laptops too,
[1679.10 → 1681.70] I love using VS Code to edit my Nix config
[1681.70 → 1684.20] because I've got the Nix language extension.
[1685.56 → 1686.98] And I just fire up VS Code,
[1687.50 → 1689.32] change a line, save it.
[1689.32 → 1690.82] It prompts me for the pseudo password
[1690.82 → 1692.72] and I hit rebuild, and I'm done.
[1692.88 → 1695.06] It's such a slick way
[1695.06 → 1697.60] once you learn to live in that Nix config.
[1697.98 → 1699.72] And I know I could break it out more,
[1699.82 → 1700.24] but like you,
[1700.30 → 1701.34] I just put it in the main file
[1701.34 → 1702.34] plus the hardware file
[1702.34 → 1704.56] and everything that describes my system is there.
[1704.78 → 1706.12] And this last week, Alex,
[1706.14 → 1709.80] I was reviewing the Infinity Book Pro 14 from Tuxedo.
[1709.98 → 1712.38] And I wanted to try Tuxedo OS for a bit.
[1712.42 → 1713.92] And then I wanted to put Nix OS on there.
[1713.92 → 1717.72] And I loaded a bare Nix OS system on there,
[1717.78 → 1719.44] just a real basic kind of install,
[1719.68 → 1720.38] just command line.
[1721.02 → 1723.48] And SSH'd over a Nix config,
[1723.80 → 1724.76] changed the host name,
[1725.46 → 1727.58] changed a couple of the bootloader things.
[1727.82 → 1728.50] And that was it.
[1728.80 → 1730.60] Rebuilt the system, rebooted.
[1730.74 → 1732.38] And I had a full working desktop system
[1732.38 → 1733.46] with all my applications.
[1733.84 → 1734.24] Good to go.
[1734.64 → 1735.44] It is kind of crazy.
[1735.54 → 1738.50] And I think the use case really for me
[1738.50 → 1742.18] is as a somewhat, you know,
[1742.64 → 1746.78] educator on the internet of some description anyway,
[1746.98 → 1748.38] you know, perfectmediaserver.com.
[1749.60 → 1752.78] I've often struggled with the fact that,
[1752.90 → 1755.62] you know, compared to something like, say, Unpaid,
[1755.84 → 1759.40] which is flash this image onto a USB key and boot,
[1760.42 → 1762.54] you've had to go through the process.
[1763.16 → 1764.56] Admittedly, it's gotten a lot easier
[1764.56 → 1765.78] over the last decade,
[1766.36 → 1767.60] but you've had to go through the process
[1767.60 → 1769.50] of installing Linux from an ISO
[1769.50 → 1770.82] on the bare metal hardware.
[1772.08 → 1773.42] Then once you've done that,
[1773.60 → 1775.50] you know if you were to follow my dog food
[1775.50 → 1776.26] all the way through,
[1776.36 → 1777.86] you then have to go and learn Ansible
[1777.86 → 1780.06] and configure these complex playbooks
[1780.06 → 1781.62] and understand SSH
[1781.62 → 1783.48] and just all this stuff
[1783.48 → 1787.84] that I don't think is unreasonable to learn
[1787.84 → 1789.60] for someone who's in the industry.
[1790.14 → 1791.38] But if all you want to do
[1791.38 → 1793.16] is just set up a simple file server
[1793.16 → 1794.82] that's got some TV shows
[1794.82 → 1796.32] and some movies on it, for example,
[1796.32 → 1798.56] honestly, it's a bit much.
[1799.04 → 1802.44] Whereas if we tell people to install Nix OS,
[1802.64 → 1803.14] for example,
[1803.14 → 1803.86] and then I say,
[1804.04 → 1804.80] oh, by the way,
[1804.86 → 1808.24] you just copy pasta this exact Nix configuration.
[1808.70 → 1809.66] And by the way,
[1809.66 → 1811.54] you'll get ZFS out of the box.
[1811.80 → 1813.56] You'll get hardware acceleration
[1813.56 → 1815.66] for your GPU out of the box.
[1815.92 → 1818.14] And you can just set your static IP here
[1818.14 → 1819.26] and your users,
[1819.46 → 1820.50] and you can install a desktop
[1820.50 → 1821.62] if you want to.
[1821.62 → 1823.76] There is no downside.
[1824.60 → 1825.78] There is no downside.
[1826.00 → 1827.60] And that's really what hit me this week.
[1827.74 → 1829.46] It feels like we,
[1829.68 → 1831.08] it's finally a version of Linux
[1831.08 → 1832.72] that's fully managed and controlled
[1832.72 → 1833.94] the way Linux should be.
[1834.44 → 1836.60] Like a lot of times on a system
[1836.60 → 1838.74] that's RPM based or dev based,
[1839.00 → 1840.94] not 100% of the time,
[1841.06 → 1842.22] but most of the time,
[1842.22 → 1843.78] I don't uninstall software.
[1843.78 → 1845.36] I just install software
[1845.36 → 1847.10] because uninstalling software
[1847.10 → 1849.32] sometimes goes awry.
[1849.50 → 1850.20] And I've got,
[1850.20 → 1851.46] I've got Ubuntu systems
[1851.46 → 1853.20] that I've been running since 2018.
[1853.66 → 1856.42] And I'm probably underestimating
[1856.42 → 1857.94] if I say three times a year,
[1857.94 → 1859.54] I end up having to break down
[1859.54 → 1860.90] to like a TTY
[1860.90 → 1862.70] and like resolve a boot issue
[1862.70 → 1864.18] or solve some sort of
[1864.18 → 1865.38] broken package problem.
[1865.86 → 1867.86] And dash fix broken install
[1867.86 → 1868.82] or whatever it is.
[1868.98 → 1869.10] Yeah.
[1869.70 → 1870.14] Yeah.
[1870.18 → 1870.98] And then of course you have to,
[1871.08 → 1872.74] you have to go do the auto remove stuff
[1872.74 → 1873.80] and you have to make sure like
[1873.80 → 1874.84] you don't fill up the boot part.
[1874.94 → 1876.04] Like all these silly things
[1876.04 → 1878.86] that Nix just takes care of ahead of time
[1878.86 → 1881.36] and catches it before it does things.
[1881.60 → 1883.90] And you just follow that,
[1884.26 → 1885.52] which is essentially like YAML
[1885.52 → 1886.18] in the Nix config.
[1886.44 → 1887.60] And it's just easy to read
[1887.60 → 1888.28] and it makes sense.
[1888.30 → 1890.84] And it doesn't take a very long time
[1890.84 → 1892.38] to pick up if you're willing
[1892.38 → 1893.74] to just take it a little bit at a time.
[1894.52 → 1895.70] And the fact that there's so many good,
[1895.84 → 1896.96] and yours, you'll have it linked
[1896.96 → 1897.50] in the show notes,
[1897.64 → 1899.10] is a great clean example.
[1899.66 → 1900.98] There's a lot of really complicated
[1900.98 → 1901.88] Nix configs out there,
[1901.88 → 1902.82] but what I like about yours
[1902.82 → 1904.14] is it's just right, you know?
[1904.20 → 1905.28] And I think it's a good example
[1905.28 → 1906.14] for people to look at.
[1906.26 → 1907.64] And this defines a system.
[1908.24 → 1911.54] It's 115 lines with some comments
[1911.54 → 1912.70] in there and stuff like that.
[1912.82 → 1914.82] And it defines the entire environment.
[1915.28 → 1915.86] That's just it.
[1916.38 → 1918.30] Now, if you are looking
[1918.30 → 1920.10] to get more complicated,
[1920.58 → 1923.38] oh boy, will Nix OS let you.
[1924.12 → 1925.46] I thought, you know,
[1925.50 → 1926.72] I was watching some YouTube videos
[1926.72 → 1928.00] about it and doing some research.
[1928.00 → 1929.46] And I started going down
[1929.46 → 1931.48] the rabbit hole of flakes.
[1932.38 → 1934.50] Now, these things are,
[1935.14 → 1936.34] to quote Douglas Adams,
[1936.66 → 1937.12] big.
[1937.36 → 1939.26] So mind-bogglingly big
[1939.26 → 1940.16] that you won't believe
[1940.16 → 1943.04] just how big slash complex they are.
[1943.62 → 1946.38] They must be a software developer's wet dream
[1946.38 → 1949.74] because they are just unbelievably difficult
[1949.74 → 1950.88] to get started with.
[1951.26 → 1952.52] And I really tried.
[1952.60 → 1953.12] I really did.
[1953.12 → 1954.64] I spent two or three evenings
[1954.64 → 1956.98] and a good chunk of my weekend
[1956.98 → 1960.84] trying to implement these flakes.
[1961.22 → 1962.82] And the idea behind them is,
[1962.92 → 1965.40] as part of this reproducibility problem,
[1965.88 → 1967.98] they create a .lock file.
[1968.18 → 1969.70] So you have a flake. Nix file
[1969.70 → 1970.96] that you put some stuff into.
[1971.32 → 1972.30] And then alongside it,
[1972.34 → 1973.86] you have a flake. Lock file.
[1974.20 → 1977.88] And that creates a hermetically sealed timestamp
[1977.88 → 1979.38] for all the dependencies
[1979.38 → 1981.46] in that Nix flake file
[1981.46 → 1982.42] to say,
[1982.92 → 1984.46] on this exact moment in history,
[1985.10 → 1987.52] this flake must always be built
[1987.52 → 1988.76] against this .lock file.
[1989.08 → 1990.30] And you will always use
[1990.30 → 1992.46] this exact version of these packages
[1992.46 → 1993.30] forever,
[1993.60 → 1994.46] no matter what.
[1994.96 → 1997.62] I understand that that is actually amazing.
[1997.62 → 1998.96] And it solves a lot of problems
[1998.96 → 1999.74] for a lot of people.
[2000.38 → 2001.22] For me,
[2001.34 → 2003.40] it doesn't solve a problem that I have.
[2003.72 → 2004.84] What it does do
[2004.84 → 2007.26] is it creates a whole plethora
[2007.26 → 2009.80] of unbelievably complicated,
[2010.52 → 2012.06] like that house of cards,
[2012.30 → 2014.38] just trying to understand
[2014.38 → 2016.88] how the Nix OS language works.
[2017.06 → 2018.34] Okay, that's fine.
[2018.40 → 2019.52] It's not that complicated,
[2019.82 → 2020.82] really, to understand.
[2021.24 → 2022.72] I mean, I'm used to Python.
[2022.72 → 2025.02] I'm not used to Haskell
[2025.02 → 2025.92] or anything like that
[2025.92 → 2028.00] that's a bit more close
[2028.00 → 2029.22] to the Nix OS language.
[2029.64 → 2031.40] But I think if you're rooted
[2031.40 → 2032.58] in the world of being
[2032.58 → 2033.38] a software developer,
[2033.92 → 2034.92] maybe like Was,
[2035.50 → 2038.16] then Nix OS and Flakes
[2038.16 → 2040.04] will just be right up your street.
[2040.26 → 2040.96] But for me,
[2041.04 → 2043.62] it's just so difficult
[2043.62 → 2044.56] to understand
[2044.56 → 2046.02] what the concepts even are.
[2046.10 → 2046.28] I mean,
[2046.96 → 2048.58] I understand the hermetically sealed part.
[2048.90 → 2050.46] That bit's easy to understand.
[2051.00 → 2052.46] But everything else
[2052.46 → 2053.52] is just like,
[2054.16 → 2056.64] okay, so I need to inherit this from here
[2056.64 → 2057.84] and then I need to recreate
[2057.84 → 2060.04] Nix packages over there
[2060.04 → 2061.02] with this syntax
[2061.02 → 2062.36] and then I import it over here
[2062.36 → 2062.68] and like,
[2063.12 → 2063.76] before you know it,
[2063.76 → 2065.40] you've got 15 files in a directory
[2065.40 → 2066.12] and you're like,
[2066.80 → 2067.02] well,
[2067.70 → 2069.42] the whole drawer of this thing
[2069.42 → 2071.60] was the single config file
[2071.60 → 2072.52] of beauty,
[2072.66 → 2073.38] of simplicity.
[2074.50 → 2075.84] And I understand,
[2075.94 → 2076.08] you know,
[2076.08 → 2077.22] looking at Wimpy's config,
[2077.34 → 2077.84] for example,
[2078.78 → 2080.26] he's got one flake file
[2080.26 → 2082.66] that can define 15 systems.
[2084.16 → 2086.36] Okay, that is cool,
[2086.36 → 2089.08] but I could just have 15 files
[2089.08 → 2090.68] that define 15 systems
[2090.68 → 2092.04] without all the complexity.
[2092.66 → 2094.54] I don't know if that makes me a Luddite
[2094.54 → 2095.12] or what,
[2095.38 → 2097.70] but I've really tried with flakes,
[2097.80 → 2098.40] but they're just,
[2098.54 → 2100.42] they're just too hard.
[2101.24 → 2102.74] I feel like this is the number one sentiment
[2102.74 → 2104.70] I hear when the audience tries out Nix
[2104.70 → 2106.26] and it's exactly how I feel too, Alex.
[2106.36 → 2108.24] And I think the way I describe it is
[2108.24 → 2111.60] all the language that talks about flakes
[2111.60 → 2116.16] sort of presumes a bunch of tribal knowledge already.
[2116.48 → 2118.84] And so you almost have to spend a day
[2118.84 → 2121.60] learning how to speak flake and ease
[2121.60 → 2123.32] before you can even kind of start
[2123.32 → 2124.38] to wrap your head around it.
[2124.46 → 2125.82] And that's such a huge barrier.
[2125.92 → 2126.50] And I've tried to,
[2126.60 → 2128.24] I've tried to explain to the folks,
[2128.32 → 2130.20] like we have a Nix nerds matrix chat room,
[2130.28 → 2131.68] which is a great chat room,
[2131.70 → 2132.40] a great resource.
[2132.66 → 2134.34] And the folks in their know it so well,
[2134.40 → 2134.92] they're just like,
[2134.96 → 2135.52] oh, what are you talking about?
[2135.54 → 2135.90] You do this,
[2135.96 → 2136.22] this, that,
[2136.28 → 2136.38] and that.
[2136.40 → 2136.94] There's no big problem.
[2137.06 → 2138.18] You've got three different ways you can do it.
[2138.18 → 2138.56] It's easy.
[2138.82 → 2139.00] I'm like,
[2139.08 → 2139.50] well,
[2139.60 → 2141.34] it's like when you go to a mechanic shop
[2141.34 → 2141.74] and you're like,
[2141.78 → 2141.88] well,
[2141.88 → 2142.62] I've got this issue.
[2142.66 → 2142.94] And he's like,
[2142.96 → 2143.08] oh,
[2143.10 → 2143.20] well,
[2143.22 → 2146.80] you just need to replace the Regina Falange flux capacitor.
[2147.02 → 2147.34] And you're like,
[2147.88 → 2148.56] okay.
[2149.72 → 2150.40] Don't you got a lift?
[2150.48 → 2151.14] Just put it on your lift.
[2151.58 → 2152.46] And I,
[2152.54 → 2156.88] I look at it as I'm already felt like Nix is so far
[2156.88 → 2157.98] exceeding my expectations.
[2157.98 → 2158.64] Like I've got,
[2158.74 → 2162.58] not only do you have what you can define in the Nix configuration,
[2162.58 → 2165.42] but one of the things I love is somebody who's just trying stuff out
[2165.42 → 2168.38] all the time is Nix shell dash P package name.
[2168.38 → 2171.98] And Nix just builds a temporary environment with that application.
[2171.98 → 2172.88] And then when you close it,
[2172.92 → 2173.46] it's ephemeral,
[2173.54 → 2173.98] it's gone.
[2174.14 → 2177.88] And so I can just pull down any old package for a few minutes and use it.
[2178.06 → 2182.48] And that combined with what I can do with the just configuration already.
[2182.54 → 2182.88] I'm just like,
[2182.98 → 2184.16] I don't yet.
[2184.54 → 2186.84] I don't yet have the need for flakes because I,
[2186.92 → 2190.18] I never had that on any other distribution, and it's already doing more for me
[2190.18 → 2192.18] than any distribution already has done.
[2192.36 → 2193.78] So I've been happy,
[2193.78 → 2196.06] but I do feel like a bit like you're like,
[2196.14 → 2196.76] am I a little,
[2196.84 → 2198.34] I hear my missing out on something?
[2198.34 → 2200.96] Because the thing I always hear about flakes is,
[2201.08 → 2201.10] well,
[2201.10 → 2202.12] then you get home manager.
[2202.26 → 2202.52] Yes.
[2202.66 → 2206.38] And home manager is really where the like power tools are at.
[2206.40 → 2206.62] And I,
[2206.76 → 2207.96] I do feel that draw.
[2208.38 → 2208.80] Me too.
[2209.10 → 2209.50] And,
[2209.64 → 2209.90] uh,
[2209.92 → 2211.78] I will keep plugging away at flakes,
[2212.00 → 2216.76] but there just came a point where I'd spent maybe three or four days trying to
[2216.76 → 2217.36] understand it.
[2217.38 → 2217.88] And I was like,
[2218.28 → 2218.66] you know,
[2218.70 → 2220.32] this is beyond me, and it's not,
[2220.32 → 2221.10] you know,
[2221.32 → 2221.98] toot my own horn.
[2221.98 → 2223.72] It's not often that that happens with,
[2223.80 → 2225.08] with Linux and stuff these days.
[2225.08 → 2231.04] So it's kind of a deflating feeling to realize that and then admit it publicly in a podcast
[2231.04 → 2231.70] as well,
[2231.76 → 2232.10] you know?
[2232.16 → 2232.54] So,
[2232.70 → 2232.94] um,
[2233.78 → 2234.04] I,
[2234.08 → 2236.62] I spoke to a few people on Mastodon about,
[2236.76 → 2237.08] you know,
[2237.12 → 2241.58] trying to get some help and some example flake configs I could understand.
[2241.68 → 2243.44] And I think another part of the issue to,
[2243.50 → 2248.86] to build on everything you've just said is everybody does it slightly differently.
[2248.86 → 2251.66] And so there isn't like a recipe.
[2252.30 → 2257.14] And because they're still officially an experimental feature in the Nix world,
[2257.92 → 2258.30] the document,
[2258.40 → 2262.22] the official documentation doesn't really cover flakes at all,
[2262.32 → 2263.70] even though they are,
[2263.94 → 2265.64] everybody says the future.
[2266.16 → 2267.44] So for me,
[2267.52 → 2267.90] for now,
[2267.96 → 2272.92] I'll be sticking to configuration. Nix because it's something my simple eight brain can comprehend
[2272.92 → 2274.30] and understand nice and easily.
[2274.30 → 2275.44] And,
[2275.52 → 2275.74] uh,
[2275.74 → 2278.40] I'll probably migrate perfect media server.
[2278.82 → 2280.10] Maybe by the end of the year,
[2280.16 → 2283.46] I'll rewrite that a little bit just towards Nix OS,
[2283.70 → 2284.56] because it really,
[2285.02 → 2288.60] for most people are going to do everything that you need.
[2290.54 → 2292.98] Talescale.com slash self-hosted.
[2293.16 → 2296.58] Go check it out right now and get a free personal account for up to 100 devices.
[2296.58 → 2298.00] And it's a great way to support the show.
[2298.08 → 2300.78] So it's talescale.com slash self-hosted.
[2300.78 → 2301.44] Now,
[2301.50 → 2303.52] tale scale is a solution for a team of any size,
[2303.60 → 2313.66] an individual or a large enterprise that just doesn't want to have to deal with the annoying old style VPN systems that are costly and complicated to maintain.
[2314.14 → 2318.86] What tale scale does is it uses WireGuard to create a mesh network between your resources.
[2319.18 → 2322.74] It lets you easily build out in minutes per device,
[2322.84 → 2327.48] a network that's flat and talks directly to each other using WireGuard's noise protocol.
[2327.66 → 2330.02] It's perfect for those of us that like to self-host.
[2330.02 → 2335.10] You can put your services all on your tail net, and you don't need to bother with port forwarding on your firewall.
[2335.42 → 2337.76] If your ISP doesn't allow a certain inbound port,
[2337.98 → 2339.50] because it's all private traffic now.
[2340.06 → 2345.02] And each device like your phone or your tablet or a VPS or your desktop computer,
[2345.16 → 2349.38] but it doesn't matter what the OS is because they support ARM and Intel and just the whole range out there.
[2349.38 → 2352.68] And they give you great tooling to like tale scale send,
[2353.24 → 2354.52] which is sort of like airdrop,
[2354.52 → 2355.08] I guess,
[2355.16 → 2357.52] but for all of your devices on your tail net,
[2357.72 → 2360.42] doesn't matter their OS or tale scale SSH,
[2360.48 → 2363.02] which lets you log in to all of your tale scale devices.
[2363.14 → 2367.10] There's a lot more to Alex and I use it to share resources between our networks.
[2367.20 → 2368.70] So when we're trying something out for the show,
[2368.80 → 2370.18] we share it over tale scale.
[2370.26 → 2372.58] And then I just put his DNS domain name,
[2372.68 → 2373.38] put his port in,
[2373.38 → 2374.72] goes over tale scale,
[2374.96 → 2376.18] all protected by WireGuard.
[2376.36 → 2378.20] It's so elegant and so easy.
[2378.38 → 2380.06] It's going to change your networking game.
[2380.16 → 2384.30] So support the show and try it for 100 devices for free on a personal account.
[2384.46 → 2387.12] Just go to talescale.com slash self-hosted.
[2387.16 → 2387.54] That's it.
[2388.22 → 2390.18] And you get started for 100 devices right there.
[2390.28 → 2392.44] Talescale.com slash self-hosted.
[2393.82 → 2395.08] We're back in January.
[2395.44 → 2395.68] I mean,
[2395.72 → 2395.96] it's,
[2395.96 → 2397.06] it's July now,
[2397.08 → 2397.60] so we could do,
[2397.70 → 2399.32] we could have also done a Jellyfin July,
[2399.46 → 2399.82] I guess,
[2399.90 → 2401.50] but we did Jellyfin January.
[2401.50 → 2402.70] And for the most part,
[2402.76 → 2403.70] it's been going pretty well.
[2403.76 → 2407.30] There were a couple of rough edges that we touched on back in February,
[2407.86 → 2410.58] but I've been having a great time over there on the Jellyfin sauce.
[2411.10 → 2411.58] But,
[2411.68 → 2412.12] uh,
[2412.14 → 2414.02] you had a dad fail the other day.
[2414.40 → 2414.54] Oh,
[2414.56 → 2415.30] it was embarrassing.
[2415.50 → 2415.90] Alex,
[2416.22 → 2417.80] the worst case,
[2418.28 → 2419.02] worst case.
[2419.46 → 2420.72] One of those days,
[2421.28 → 2423.32] we're literally all day long.
[2423.32 → 2427.02] The wife and the kid are talking about how we're going to watch Dune tonight.
[2427.14 → 2428.12] We're going to have dinner.
[2428.32 → 2429.34] We're going to pop popcorn.
[2429.50 → 2431.44] We're going to sit down, and we're going to watch the whole Dune.
[2431.50 → 2431.74] movie,
[2431.84 → 2432.72] which is a long movie.
[2433.90 → 2434.58] I think great.
[2434.68 → 2437.24] I have a cash locally on my Jellyfin server here in the RV.
[2438.38 → 2439.04] Plenty of bats,
[2439.16 → 2440.26] plenty of charge in the batteries.
[2440.36 → 2440.98] We're good to go.
[2441.58 → 2442.90] I fire up in fuse.
[2444.78 → 2445.14] And,
[2445.20 → 2445.36] uh,
[2445.36 → 2446.06] it's going great.
[2446.18 → 2446.38] You know,
[2446.38 → 2446.98] it's a long movie.
[2447.06 → 2449.00] We're an hour and 25 minutes into it.
[2449.74 → 2452.28] And I accidentally bumped the Apple TV remote.
[2452.28 → 2453.10] And this thing,
[2453.14 → 2453.30] if you,
[2453.30 → 2455.12] if you fart on this Apple TV remote,
[2455.22 → 2455.38] it,
[2455.38 → 2456.26] it triggers stuff.
[2457.26 → 2457.64] And,
[2457.72 → 2457.94] uh,
[2458.40 → 2459.34] it closed the app.
[2460.14 → 2460.50] Okay.
[2460.50 → 2464.50] So I relaunched the app, and it resumes the app, and it tries to start resuming the video,
[2464.64 → 2465.88] but it fails.
[2465.92 → 2468.44] And it goes back to the main screen and airs out with a generic air.
[2469.24 → 2469.82] And it says,
[2469.88 → 2470.00] okay,
[2470.00 → 2471.98] would you like to resume in an hour and 25 minutes?
[2471.98 → 2472.72] I say yes.
[2473.78 → 2476.34] And after it waits, and it waits, and it waits,
[2476.34 → 2478.60] it resumes the movie at like six minutes.
[2479.86 → 2483.58] And then I pause, and I wait, and I wait, and it resumes at like 25 minutes.
[2483.86 → 2485.34] It's having to buffer at each time.
[2485.60 → 2489.84] And so we wait about 10 minutes trying to figure out what's wrong with it.
[2490.00 → 2493.24] And when we finally just decided to wait and let it buffer and then try to get to our time,
[2493.30 → 2495.82] it's playing just fine for about 10 more minutes.
[2495.82 → 2497.62] And then it crashes.
[2498.14 → 2498.70] It stops.
[2498.76 → 2499.40] The stream just stops.
[2499.48 → 2500.14] We get an error message.
[2500.22 → 2501.12] And I think what's going on.
[2501.14 → 2501.82] So I checked the server.
[2501.92 → 2502.80] Everything's looking okay.
[2502.96 → 2503.24] I think,
[2503.30 → 2503.42] all right,
[2503.46 → 2504.04] we're going to leave,
[2504.04 → 2505.20] we're going to leave infuse.
[2505.58 → 2506.72] Let's go use Swift fin.
[2507.12 → 2507.40] You know,
[2507.44 → 2509.78] that's a newer app built for Jellyfin.
[2509.88 → 2510.52] Let's use Swift fin.
[2511.34 → 2512.78] So if I go over to Swift fin,
[2513.54 → 2514.94] get it all configured again,
[2514.94 → 2515.90] because for whatever reason,
[2515.94 → 2516.70] it lost the config.
[2516.76 → 2517.14] That's fine.
[2517.16 → 2518.06] So I set it all up again,
[2518.12 → 2519.50] get it connected to my Jellyfin server.
[2520.02 → 2520.88] I hit play.
[2521.72 → 2524.98] And it's the same exact experience.
[2525.70 → 2527.58] It's exactly like what happened in infuse world.
[2527.76 → 2529.30] It plays six minutes instead of an hour,
[2529.38 → 2529.70] 25.
[2530.68 → 2532.92] We gave up with 20 minutes left on the movie.
[2533.38 → 2533.74] Ultimately,
[2533.74 → 2536.28] we gave up because we were having so many problems.
[2536.46 → 2537.84] Once that remote got bumped,
[2537.92 → 2539.98] we were never able to really get going again.
[2540.60 → 2541.24] And man,
[2541.26 → 2541.94] is that embarrassing?
[2542.26 → 2542.60] You know,
[2543.50 → 2544.32] major dad fail.
[2544.44 → 2546.02] And then the thing that really stung.
[2547.54 → 2549.18] Is I opened up the Plex app,
[2549.18 → 2551.22] which is configured to connect to the Plex instance.
[2551.22 → 2552.80] I still have running back at the studio.
[2552.94 → 2560.80] So over my Starlink and opened up Dune just to see and fast forwarded and went to the hour 25 mark.
[2561.68 → 2563.52] 15 seconds or so after buffering,
[2563.68 → 2564.88] it played just fine.
[2565.30 → 2565.66] Same file.
[2566.00 → 2566.22] Yep.
[2566.40 → 2567.02] Same file.
[2567.60 → 2568.20] Same file.
[2568.24 → 2570.62] Because I copied it from that server to my local copy.
[2570.72 → 2572.22] Cause that's where my mind went immediately.
[2572.46 → 2573.32] And it's not even a necessarily,
[2573.48 → 2574.28] it's not a big file.
[2574.36 → 2575.50] It's a 10 ADP file.
[2575.66 → 2575.96] It's,
[2576.08 → 2576.24] you know,
[2576.24 → 2577.36] it's like 13 gigs.
[2577.46 → 2578.40] I didn't get it.
[2578.40 → 2580.22] I didn't get a super high-res version either.
[2581.12 → 2586.18] And so you combine that with the fact that Was and Brent want to do watch along with Star Trek,
[2586.26 → 2587.02] strange new worlds.
[2587.02 → 2592.98] And I think the Plex feature set's just a lot more robust there for the watch along stuff.
[2593.70 → 2598.36] I'm feeling the Plex siren after like six months of being really happy with Jellyfin.
[2599.00 → 2599.08] Yeah.
[2599.12 → 2599.22] Well,
[2599.22 → 2599.44] I mean,
[2599.48 → 2601.68] we both still keep them knocking around anyway.
[2601.68 → 2602.70] You know,
[2602.82 → 2607.42] Prologue on iOS is the premier audiobook client.
[2607.52 → 2609.20] And you will not convince my wife otherwise,
[2609.46 → 2614.50] even though Audio bookshelf has had a lot of improvements over the last year or two.
[2615.14 → 2615.40] Yeah.
[2615.46 → 2615.72] But I mean,
[2615.76 → 2616.18] for me,
[2616.44 → 2618.88] if I open up Plex or Jellyfin on the client side,
[2618.96 → 2619.10] I mean,
[2619.12 → 2619.50] it's not a
[2619.56 → 2620.50] it's not a big deal,
[2620.50 → 2620.90] is it?
[2621.68 → 2624.44] As long as I guess you still try and default to Jellyfin,
[2624.44 → 2627.54] then everything's crayfish.
[2627.98 → 2630.02] What about all of our concerns of,
[2630.02 → 2631.26] you know,
[2631.36 → 2634.14] Plex as a company and their direction and scraping data?
[2634.36 → 2635.56] And they just laid people off.
[2635.62 → 2636.04] So clearly,
[2636.16 → 2636.48] you know,
[2636.58 → 2638.70] they're going to have to find a revenue stream from somewhere.
[2639.58 → 2641.34] I still maintain those concerns.
[2641.94 → 2642.60] I also,
[2642.90 → 2645.50] I just think Jellyfin is a better experience offline.
[2645.76 → 2645.94] I mean,
[2645.96 → 2646.14] yes,
[2646.16 → 2649.10] I know I can go allow the LAN access and all that kind of stuff in Plex,
[2649.16 → 2649.96] but it's a workaround.
[2650.08 → 2650.78] I don't like it.
[2650.94 → 2652.00] I don't like any of that.
[2652.04 → 2653.40] I don't like having to have a Plex account.
[2653.40 → 2654.66] You know,
[2654.70 → 2656.26] even though I'm a lifetime past subscriber,
[2656.38 → 2657.12] I still just,
[2657.26 → 2660.96] I just want to play my local files and I don't want anybody to know anything about what I'm watching.
[2661.50 → 2661.76] Ah,
[2661.86 → 2662.16] yes.
[2662.34 → 2663.82] The tinfoil hat approach.
[2664.58 → 2665.16] But then,
[2665.22 → 2665.40] you know,
[2665.44 → 2668.80] you're sitting there trying to watch a movie, and you're in the last 20,
[2668.84 → 2669.06] you finally,
[2669.14 → 2671.08] you make it to the last 20 minutes and you give up.
[2671.82 → 2673.34] That is almost a disqualified,
[2673.70 → 2674.04] you know,
[2674.16 → 2674.70] that moment.
[2675.18 → 2675.28] Well,
[2675.34 → 2676.38] do you want me to ruin it for you?
[2677.08 → 2677.42] Hmm.
[2677.82 → 2678.16] Okay.
[2678.60 → 2681.16] Everybody lives or dies.
[2681.36 → 2681.98] I don't know.
[2683.40 → 2684.00] We all poop.
[2685.10 → 2686.78] I don't have the time right now,
[2686.86 → 2688.14] so I'm probably not going to swap out,
[2688.46 → 2688.64] but,
[2688.76 → 2689.80] you know,
[2689.82 → 2690.78] I guess to finish the movie,
[2690.86 → 2694.44] we're going to watch it off Plex remotely instead of watching my local copy over the land.
[2694.86 → 2695.62] You filthy,
[2695.98 → 2696.50] proprietary,
[2696.70 → 2696.98] garbage,
[2697.06 → 2698.14] supporting man,
[2698.24 → 2698.44] you.
[2698.44 → 2699.02] I know.
[2699.02 → 2699.04] I know.
[2699.10 → 2699.90] It's not even local.
[2700.00 → 2700.84] It's my own cloud,
[2701.00 → 2702.60] but still somebody else's computer,
[2702.70 → 2702.84] right?
[2702.94 → 2703.76] Just my computer.
[2704.04 → 2704.26] Somebody,
[2704.38 → 2705.02] it's another place.
[2705.40 → 2706.82] I actually had a listener write in,
[2707.12 → 2709.20] just sent me a message in discord this week to say,
[2709.28 → 2710.92] because of you,
[2711.06 → 2714.22] I was going to put something in Trello the other day.
[2714.88 → 2717.20] And then I was thinking,
[2717.34 → 2719.78] do I trust this company with my data?
[2720.32 → 2720.72] No,
[2721.22 → 2722.14] I don't.
[2722.70 → 2724.70] And so they went and found a self-host alternative.
[2724.84 → 2726.14] The name escapes me right now,
[2726.22 → 2728.78] but I think it's a very important principle,
[2728.88 → 2733.68] this kind of guilt of using the non-perfect solution.
[2734.30 → 2736.34] Plex is the perfect example.
[2736.56 → 2739.18] We know there are flaws with their business model,
[2739.56 → 2741.66] with them as a company and all the rest of it,
[2742.02 → 2744.90] but sometimes it just gets the job done.
[2744.90 → 2746.72] And I don't know if,
[2746.80 → 2752.00] I don't know if just simply by the fact that we're using something like Plex puts us in the top,
[2752.00 → 2755.68] 1% of media consumers anyway.
[2756.36 → 2758.70] So people probably aren't looking at us,
[2758.84 → 2760.02] but you know,
[2760.08 → 2762.86] there is this sense of guilt for any self-hosted,
[2763.00 → 2767.32] for any hosted service that we should be doing the most pure,
[2767.44 → 2768.12] the most technically,
[2768.58 → 2769.40] you know,
[2769.74 → 2771.00] perfect approach.
[2771.14 → 2776.42] And I think one of the things I've always tried to do on this show is kind of lean into the pragmatism
[2776.42 → 2777.24] angle.
[2777.90 → 2779.66] It's a fine line to walk.
[2779.90 → 2780.92] I'd love to hear what you think.
[2780.92 → 2784.18] So please write in at self-hosted. Show slash contact.
[2784.96 → 2784.98] Yes.
[2784.98 → 2786.60] And speaking of the feedback,
[2786.74 → 2787.66] Jericho wrote in,
[2787.80 → 2790.16] he wanted to share something called Post Google.
[2790.30 → 2790.70] He says,
[2790.80 → 2793.86] it's a program after you get a self-hosted mail server,
[2794.02 → 2798.74] it'll let you set up an email server that is also a matrix bridge.
[2799.16 → 2800.38] Why would I want to do that then?
[2800.62 → 2800.82] I would,
[2800.90 → 2801.32] you know what?
[2801.74 → 2802.18] Well,
[2802.62 → 2804.72] if I could have,
[2804.82 → 2806.12] it's kind of like RSS in a way,
[2806.12 → 2808.80] if I could have my emails output to a room,
[2809.00 → 2809.12] if,
[2809.20 → 2811.02] if you're already living in element,
[2811.14 → 2811.56] let's say,
[2812.62 → 2812.84] you know,
[2812.84 → 2813.62] or maybe it's Slack,
[2813.70 → 2814.12] whatever it may be,
[2814.16 → 2815.26] but if you're already living in this case,
[2815.28 → 2815.74] an element,
[2816.36 → 2819.60] then it's kind of nice to just have a room that collects notifications because I can,
[2819.74 → 2820.44] I can get so busy.
[2820.48 → 2820.80] I can,
[2820.96 → 2821.24] you know,
[2821.50 → 2824.86] go a day without checking my email, and then I get a bunch of upset people in there.
[2824.86 → 2826.30] So I could kind of see it.
[2826.70 → 2827.22] I don't know.
[2827.28 → 2827.98] I could kind of see it.
[2828.24 → 2829.28] Google post Google.
[2829.90 → 2831.12] So we'll put a link in the show notes.
[2831.42 → 2833.60] I just wasn't sure of quite what the use case was,
[2833.66 → 2834.34] but that makes sense.
[2834.72 → 2834.82] Yeah.
[2834.84 → 2836.04] Or maybe like in our case,
[2836.16 → 2836.44] right?
[2836.48 → 2840.76] If like people wrote into the self-hosted show, and we had a shared room between us,
[2840.76 → 2843.38] then we would both get a notification in that shared room about an email.
[2843.72 → 2844.16] That could be cool.
[2844.96 → 2845.80] Martin writes in,
[2845.84 → 2846.02] it says,
[2846.08 → 2846.16] Hey,
[2846.22 → 2846.62] Chris and Alex,
[2846.70 → 2847.82] long time listener.
[2848.08 → 2850.90] I've been on the search for a note app and I know Chris was too lately.
[2850.90 → 2853.18] I've been finding a lot of value out of notion,
[2853.18 → 2854.34] like note apps.
[2854.54 → 2859.02] I stumbled on any type it's open source and encrypted and has mobile and
[2859.02 → 2859.92] desktop clients.
[2860.64 → 2861.00] Hmm.
[2861.26 → 2864.40] Any type.io and they offer a self-hosting setup.
[2864.50 → 2865.56] It is an alpha right now.
[2866.02 → 2866.46] Well,
[2866.48 → 2867.48] that's awfully helpful.
[2868.26 → 2871.94] We have a bunch of perfect recommendations that come in like on stuff to try.
[2872.80 → 2875.64] And it's hard to know which one to pull the trigger on,
[2875.72 → 2879.04] but there's a few in here this week that look perfect.
[2879.10 → 2879.68] You know,
[2879.76 → 2879.88] the
[2879.88 → 2880.30] the really,
[2880.54 → 2881.74] it's not frustrating,
[2882.06 → 2886.66] but it is a little bit frustrating is at some point you just got to stick a pin in
[2886.66 → 2887.70] it and actually pick one.
[2887.70 → 2892.40] And I feel like I just picked obsidian as my de facto,
[2893.18 → 2893.44] you know,
[2893.92 → 2895.80] personal knowledge system,
[2895.90 → 2898.66] replacing tiddly wiki from before,
[2898.84 → 2900.14] before then.
[2900.46 → 2911.56] And then any type comes along with this beautiful looking application and crazy fast load times and secure and decentralized sync as part of the product.
[2911.70 → 2911.94] You know,
[2911.96 → 2912.48] it's like,
[2912.48 → 2913.98] Oh,
[2914.14 → 2915.74] I just got it right.
[2915.86 → 2916.80] And I'm not going to help too,
[2916.86 → 2917.90] because Jen from a teak,
[2918.58 → 2920.32] Jen from a teak this week says,
[2920.34 → 2920.64] uh,
[2920.64 → 2925.18] he found an agile tool that he loves that replaces things like JIRA for him and,
[2925.28 → 2925.44] uh,
[2925.44 → 2926.26] some ticket tools.
[2926.34 → 2927.36] It's called Taiga,
[2927.52 → 2929.34] T A I G A I.
[2929.60 → 2930.00] Dot IO.
[2930.34 → 2931.66] And then on top of that,
[2931.66 → 2934.18] he has found a killer outlining application,
[2934.18 → 2935.88] which I've been checking out since Coder Radio.
[2935.88 → 2937.82] And it's called get outline.com.
[2938.60 → 2940.64] And you can also self-host that.
[2941.02 → 2942.16] So those are a couple of,
[2942.48 → 2943.72] where we have some perfect,
[2943.76 → 2946.92] this is like an app pick extravaganza episode.
[2947.36 → 2948.28] I'll tell you what,
[2948.48 → 2951.74] we'll make sure to put links to all of these things in the show notes,
[2951.74 → 2953.72] just in case you want to check them out.
[2956.52 → 2957.68] 45 home lab.com.
[2957.76 → 2958.66] It's happening.
[2958.78 → 2959.02] Big,
[2959.12 → 2959.40] strong,
[2959.52 → 2961.88] fast storage servers with high performance,
[2962.22 → 2966.28] high capacity and affordable for all data requirements,
[2966.42 → 2970.02] personal grade solutions that are ideal for your business or your home lab.
[2970.02 → 2972.08] Go learn more at 45 drives.com,
[2972.16 → 2972.30] right?
[2972.36 → 2973.88] That's where you get your enterprise drives.
[2974.08 → 2975.60] Everybody knows about 45 drives.
[2975.72 → 2979.24] And you might remember episode 98 of the self-hosted podcast,
[2979.40 → 2980.28] their mission,
[2980.38 → 2983.26] where they talked about the way they see the storage market and the vision for
[2983.26 → 2985.80] future products that it clicked with us.
[2985.88 → 2988.12] The home lab opportunity to us seems immense.
[2988.12 → 2993.20] They listen to the feedback from the podcast, and they're cooking up 45 home lab.com.
[2993.28 → 2994.52] I think it's going to be right up your alley.
[2994.58 → 2995.40] So go check it out.
[2995.80 → 2999.62] I think you guys will also like that 45 drives maintains an open design and
[2999.62 → 3002.16] ongoing relationship with the open source community.
[3002.58 → 3004.88] And we love the dedicated engineering team.
[3004.94 → 3005.92] That's ready to help you.
[3006.14 → 3007.10] Should you ever need it.
[3007.10 → 3011.54] So go learn how 45 drives does things differently and visit 45 drives.com.
[3011.64 → 3012.48] And when you get a chance,
[3012.62 → 3014.16] tell them the self-hosted podcast sent you.
[3014.50 → 3018.20] And remember they're cooking up something great just for our audience at 45
[3018.20 → 3019.74] home lab.com.
[3019.80 → 3020.48] You're going to love it.
[3020.62 → 3021.36] That's where you go.
[3021.48 → 3023.14] 45 home lab.com.
[3024.90 → 3027.10] And we've got some great boost coming into the show.
[3027.20 → 3028.18] Everybody's been really,
[3028.36 → 3033.10] really supportive since episode 100 and legit salvage came in with 75,000 stats.
[3033.18 → 3034.16] He's our baller booster.
[3034.16 → 3039.32] He's been catching up, and he has a brand new beautiful baby girl and,
[3039.40 → 3039.60] uh,
[3039.60 → 3041.02] well soon in about 12 weeks.
[3041.02 → 3044.98] And he is on the hunt for a proper baby monitor solution.
[3045.08 → 3047.72] He has IP cameras for his home with a DVR.
[3047.86 → 3051.14] And he's thinking about just adding a new camera to her nursery.
[3051.26 → 3052.76] So that would be a normal solution.
[3052.76 → 3053.16] However,
[3053.94 → 3055.06] since she's a preemie baby,
[3055.24 → 3055.54] uh,
[3055.54 → 3058.40] lung development and breathing will be a factor when bringing her home.
[3058.58 → 3059.82] So for peace of mind,
[3059.82 → 3062.96] I've been looking at video monitors that include visual sensors to monitor
[3062.96 → 3063.42] breathing.
[3063.42 → 3066.08] Like the name pro or Dufy space view.
[3067.16 → 3069.62] These don't appear to have non-connected options,
[3069.66 → 3070.04] or if they do,
[3070.10 → 3070.52] it's not clear.
[3070.58 → 3072.68] These features would work without phoning home.
[3072.78 → 3073.10] I would,
[3073.14 → 3073.46] that would be,
[3073.58 → 3074.56] I would suspect that as well,
[3074.56 → 3077.60] given all the incidents of baby monitors being hacked.
[3077.82 → 3079.04] He's concerned about it.
[3079.12 → 3081.06] And he wants to know if we have any suggestions.
[3081.14 → 3081.38] He says,
[3081.40 → 3082.36] he appreciates the content.
[3082.56 → 3084.86] It's a welcome distraction from the recent chaos in life.
[3084.92 → 3085.06] Yeah,
[3085.06 → 3085.22] man,
[3085.24 → 3085.94] that's got to be,
[3086.44 → 3087.64] that is not a
[3087.72 → 3088.70] that is not an easy time.
[3089.20 → 3089.60] Well,
[3089.68 → 3090.76] speaking from experience,
[3090.76 → 3091.94] my daughter arrived,
[3091.94 → 3092.70] uh,
[3093.44 → 3093.80] seven,
[3094.00 → 3094.70] eight weeks early,
[3094.70 → 3095.96] not quite 12,
[3096.64 → 3097.08] uh,
[3097.08 → 3098.20] like you good sir.
[3098.34 → 3098.66] But,
[3098.78 → 3099.12] uh,
[3099.34 → 3104.28] what I will say is now she's two and a half fully healthy and perfect and
[3104.28 → 3108.32] running about with baby shark towels on her head and will not eat her
[3108.32 → 3110.10] dinner without her flamingo hat on,
[3110.20 → 3110.62] you know?
[3110.62 → 3112.44] So it does get easier.
[3112.80 → 3112.82] Yeah.
[3112.82 → 3114.78] 12 weeks before due date is pretty serious,
[3114.78 → 3115.06] right?
[3115.66 → 3115.90] Yeah.
[3115.96 → 3116.14] 12,
[3116.14 → 3116.82] 12 weeks is,
[3116.88 → 3117.40] is not,
[3117.62 → 3117.94] you know,
[3118.14 → 3118.50] it's,
[3118.58 → 3119.96] it's no trifling matter.
[3120.30 → 3121.38] So what I will say is,
[3121.42 → 3121.84] first,
[3121.84 → 3123.66] if you want to reach out personally to me,
[3123.66 → 3124.20] um,
[3124.30 → 3126.54] and have a chat about someone who's gone through it recently,
[3126.54 → 3128.08] the whole NICU thing,
[3128.32 → 3128.66] you know,
[3128.74 → 3129.14] it's,
[3129.64 → 3130.58] it's a lot to process.
[3130.58 → 3132.24] So please feel free to reach out.
[3132.24 → 3133.52] But secondly,
[3133.74 → 3135.84] what I will also say is that,
[3135.84 → 3136.30] uh,
[3136.30 → 3139.60] we've had a huge amount of success with the wise cameras.
[3139.60 → 3144.50] We've put them into a black hole VLAN so that they're offline.
[3144.62 → 3145.70] They can't reach the internet,
[3145.70 → 3146.64] but the
[3146.82 → 3147.92] obviously the initial registration,
[3148.08 → 3148.54] they have to,
[3148.94 → 3149.80] but after that,
[3149.94 → 3150.34] uh,
[3150.34 → 3151.04] they don't.
[3151.10 → 3153.02] And I can connect to those cameras.
[3153.24 → 3153.60] Um,
[3153.60 → 3155.82] I'm not running a special firmware or anything like that,
[3155.82 → 3156.74] uh,
[3156.76 → 3157.46] over the LAN.
[3157.54 → 3163.18] It does the discovery over the LAN and then does a peer to peer video stream from one device to the other.
[3163.46 → 3163.94] Now,
[3163.98 → 3165.38] another piece of advice for you,
[3165.46 → 3165.82] um,
[3165.84 → 3169.58] you mentioned having sensors to check things like breathing.
[3169.60 → 3170.80] And all the rest of it,
[3170.80 → 3171.98] uh,
[3171.98 → 3173.12] the advice we were given.
[3173.12 → 3174.06] And in hindsight,
[3174.06 → 3174.88] I really,
[3175.06 → 3183.24] I'm glad that we were given it was don't fall into the trap of getting these socks that measure heart rates and apps that,
[3183.36 → 3187.18] because they just cause a lot of false positives and a lot of anxiety and that kind of stuff.
[3187.18 → 3190.36] If you're really worried about breathing and that kind of stuff,
[3190.42 → 3193.02] you can put like vibration things under the mattress.
[3193.26 → 3194.52] But honestly,
[3194.80 → 3197.14] from my personal opinion,
[3197.38 → 3197.78] um,
[3198.12 → 3204.88] the medical staff won't send the baby home until they're completely confident that the baby is ready and healthy.
[3204.88 → 3206.86] So from my perspective,
[3206.86 → 3208.00] I wouldn't,
[3208.00 → 3210.56] I know it's difficult not to want to do something as,
[3210.62 → 3211.00] as a
[3211.00 → 3211.42] you know,
[3211.50 → 3212.28] new parent,
[3212.48 → 3212.90] uh,
[3212.90 → 3213.88] everything you can.
[3214.02 → 3214.94] It's very difficult,
[3214.94 → 3215.42] um,
[3215.42 → 3218.36] to just close the door on the nursery and say,
[3218.48 → 3218.64] Hey,
[3218.70 → 3218.94] right.
[3218.94 → 3220.90] I will see you in the morning and not,
[3221.08 → 3221.38] you know,
[3221.94 → 3223.06] not sleep with the
[3223.06 → 3226.04] the phone wide open all night looking at the screen,
[3226.14 → 3226.28] you know,
[3226.28 → 3226.94] that kind of thing.
[3226.94 → 3227.22] But,
[3227.42 → 3228.48] you know,
[3228.48 → 3229.18] it does get easier.
[3229.40 → 3230.52] I will say that as well.
[3230.80 → 3231.00] Uh,
[3231.00 → 3236.16] the first six months are the hardest and so far everything after that has been downhill for us.
[3236.26 → 3237.42] So hang in there,
[3237.46 → 3237.64] bro.
[3238.02 → 3238.38] And,
[3238.50 → 3238.64] uh,
[3238.64 → 3239.12] like I say,
[3239.18 → 3240.02] reach out if you want to,
[3240.02 → 3240.98] if you want to chat some more.
[3241.40 → 3241.52] Yes.
[3241.56 → 3243.16] And thank you for the support as well.
[3243.90 → 3248.66] Hurricane Hernandez comes in with 51,273,
[3248.66 → 3249.76] long time listener,
[3249.88 → 3250.64] first time booster.
[3251.28 → 3252.60] He's been around for a long time.
[3252.66 → 3252.88] In fact,
[3252.92 → 3258.44] he says he goes way back with you probably since 2014 when you guys were regulars on the Lime Tech forums.
[3258.54 → 3259.12] Does that ring a bell?
[3259.36 → 3259.52] Yes,
[3259.56 → 3259.98] it does.
[3260.08 → 3260.88] Hurricane Hernandez.
[3261.16 → 3261.64] I think,
[3262.08 → 3265.76] I think we first met when we were trying to stream Formula One.
[3266.06 → 3268.78] Like I was going to get a sky sports subscription in the UK.
[3268.94 → 3271.16] This was well before F1 TV was a thing.
[3271.48 → 3273.94] And I was going to get a sky TV subscription in the UK,
[3274.24 → 3278.62] figure out how to strip the DRM from it and then stream it to his house using TV head end.
[3279.02 → 3280.30] And we were going to split the cost that way.
[3280.36 → 3280.96] That never happened.
[3281.22 → 3282.82] But that's what we were talking about back then,
[3282.84 → 3283.14] I think.
[3284.26 → 3289.74] He gives you a hard time too for being a VM believer when he was pushing containers back in the day.
[3289.74 → 3290.34] There was,
[3290.38 → 3293.04] there was a time before Alex used containers.
[3293.50 → 3293.66] I went,
[3293.76 → 3294.06] you know,
[3294.38 → 3294.78] that,
[3294.94 → 3295.66] that was a thing.
[3296.06 → 3296.20] Yeah.
[3296.20 → 3297.30] I was a VM user myself.
[3297.40 → 3297.98] Still love VMs.
[3298.02 → 3298.28] Come on.
[3298.66 → 3300.20] And he also continued with another boost.
[3300.24 → 3300.60] He says,
[3300.66 → 3304.44] I wrote a blog post as to why I'm leaving Ansible for Nix.
[3304.54 → 3305.64] You can find it on my blog.
[3305.70 → 3306.26] We'll put a link.
[3306.44 → 3307.44] It's goodbye Ansible.
[3307.90 → 3309.74] I'm here to challenge you to take the Nix OS challenge.
[3309.84 → 3313.38] You'll find I have replicated parts of the perfect media server in my Nix repos.
[3313.44 → 3313.90] Have a look.
[3314.36 → 3316.44] Stand by my decision to use containers over VMs.
[3316.44 → 3319.92] Just like I stand my decision on my decision to use Nix over Ansible.
[3319.92 → 3323.34] All hail from the great white north in Alberta.
[3323.84 → 3324.30] You know,
[3324.42 → 3326.24] I know we just talked about Nix earlier in the show,
[3326.32 → 3330.28] but it does feel like I'm seeing Nix everywhere at the moment.
[3330.44 → 3330.84] I know,
[3331.12 → 3332.46] I know I'm,
[3332.64 → 3335.76] I'm contributing to that problem by talking about it on this here show.
[3335.82 → 3336.06] But you,
[3336.14 → 3336.34] you know,
[3336.50 → 3336.68] Chris,
[3336.72 → 3337.88] you've been talking about it for a
[3338.00 → 3338.12] what,
[3338.16 → 3338.76] a year or,
[3338.84 → 3339.54] or more now.
[3340.12 → 3340.30] Yeah.
[3340.30 → 3341.86] I definitely noticed it's been picking up.
[3341.92 → 3342.04] Yeah.
[3343.00 → 3343.18] Yeah.
[3343.18 → 3347.44] I think it's solving more and more problems as people get comfortable with container technology
[3347.44 → 3349.78] and they get comfortable with all these other kinds of concepts.
[3350.04 → 3353.44] It's not that much more of a leap to then start wrapping your head around Nix.
[3353.86 → 3354.06] Well,
[3354.16 → 3355.98] why do I need a
[3356.36 → 3359.56] an operating system that I can build up a ton of cruft in?
[3359.78 → 3363.34] Why not just have it be declaratively configured?
[3363.52 → 3363.76] You know,
[3363.80 → 3364.38] all that stuff.
[3365.00 → 3365.40] So,
[3365.52 → 3365.68] you know,
[3365.72 → 3366.14] you're right.
[3366.22 → 3366.96] Hurricane Hernandez,
[3367.22 → 3367.90] as usual,
[3368.20 → 3369.78] it turns out you're ahead of the curve there.
[3369.84 → 3369.98] Good,
[3370.04 → 3370.26] sir.
[3370.26 → 3372.38] And Nix is the only way,
[3372.48 → 3372.84] apparently.
[3374.02 → 3374.92] This is the way.
[3374.98 → 3375.60] Of course not.
[3375.70 → 3376.14] Of course not.
[3376.24 → 3377.84] There are situations still,
[3377.96 → 3378.26] of course,
[3378.36 → 3379.82] where one is better than the other,
[3379.94 → 3380.16] but.
[3380.62 → 3381.08] You know,
[3381.10 → 3383.74] what's a lot of fun is putting the old Nix package manager on macOS,
[3383.98 → 3386.10] get rid of brew and go to Nix on macOS.
[3386.26 → 3386.38] See,
[3386.42 → 3391.52] I do have a brand new 16-inch MacBook Pro downstairs for,
[3391.62 → 3394.84] for my stuff with tail scale next week.
[3395.22 → 3396.06] And so I will be.
[3396.14 → 3396.76] Start with Nix on there.
[3396.76 → 3397.50] I will be.
[3397.62 → 3399.30] I've been using brew forever,
[3399.30 → 3400.88] but this is the chance.
[3401.28 → 3404.16] Green comes in with 24,543 sets.
[3404.58 → 3406.06] A long time listener since 2019.
[3406.28 → 3407.00] First time booster.
[3407.10 → 3407.86] He's been catching up.
[3407.90 → 3410.90] He had some downtime recently and heard the discussion about backups for the wives.
[3411.30 → 3414.34] I've been waiting until I got cut up to see if anybody else mentioned a solution.
[3415.36 → 3415.66] But he says,
[3415.70 → 3416.44] I think I'll give it a go.
[3416.94 → 3421.10] We all know that 95% of our home labs would be left to dust should anything happen to us.
[3421.16 → 3423.40] Even the best documentation would be wasted in the end.
[3423.48 → 3424.24] And let's be honest,
[3424.24 → 3426.52] nobody wants to take on someone else's kit.
[3426.52 → 3432.60] So I have a separate backup drive just for the wife that gets updated during maintenance tasks once a week.
[3432.60 → 3433.88] I update my lab,
[3433.94 → 3434.26] my host,
[3434.32 → 3434.82] my containers,
[3434.96 → 3435.28] et cetera.
[3435.36 → 3441.48] And the last thing I on the list is I plug in the wife's drive and I run a script to update with only what she cares about.
[3441.54 → 3442.30] Things like photos,
[3442.70 → 3443.56] important documents,
[3443.96 → 3444.46] the home videos,
[3444.58 → 3445.32] and things like that.
[3445.58 → 3449.44] The files get set to read only afterwards to ensure that nothing accidentally gets deleted.
[3449.90 → 3451.26] The drive is encrypted with Lux.
[3451.26 → 3452.82] And to make sure it all works,
[3452.96 → 3457.98] she uses this to access files and photos she needs to get from her elementary OS laptop.
[3458.18 → 3459.98] All her files are accessible on the network,
[3460.14 → 3464.12] but making sure she checks the backup drive keeps me feeling warm and fuzzy knowing it works.
[3464.80 → 3465.94] Congrats on Self-hosted 100,
[3466.08 → 3466.38] guys.
[3466.74 → 3468.62] And here's to many more to come.
[3468.86 → 3470.06] That's such a great idea.
[3470.18 → 3471.88] It's so blindingly,
[3472.02 → 3473.00] obviously simple.
[3473.00 → 3474.46] and,
[3474.46 → 3475.08] you know,
[3475.14 → 3476.82] just uses all of the
[3476.82 → 3477.10] uh,
[3477.10 → 3480.82] the technologies that are free and available to us anyway,
[3480.92 → 3481.74] like Lux and,
[3482.02 → 3482.86] and all the rest of it.
[3482.90 → 3483.82] So that's a great idea.
[3484.28 → 3486.36] Just a couple more boosts to round us out.
[3486.44 → 3487.66] Thank you everybody who does boost in.
[3487.72 → 3489.34] We'll try to fit a few more in.
[3490.12 → 3493.12] FreeTube comes in with 21,007 SATs from Pod verse.
[3493.26 → 3493.38] Hey,
[3493.44 → 3495.68] you teased your Rostra end pub at the end of the last show,
[3495.78 → 3497.50] but I don't see it in the show notes.
[3497.72 → 3498.28] I know.
[3498.54 → 3500.78] I got that a lot from the emails and the boosts.
[3500.90 → 3501.10] Uh,
[3501.10 → 3502.84] I don't know how to link a Rostra pub.
[3503.24 → 3503.84] I don't,
[3504.14 → 3504.88] I took a
[3504.92 → 3507.30] took a crack at it and I couldn't figure it out.
[3507.36 → 3507.72] And when I,
[3507.86 → 3508.74] when I tried linking,
[3508.82 → 3509.70] because I tested with somebody,
[3509.76 → 3510.00] they're like,
[3510.06 → 3511.78] this isn't a real active profile.
[3511.82 → 3512.04] I'm like,
[3512.08 → 3512.56] okay.
[3513.46 → 3515.56] So until I'm really getting serious about it,
[3515.56 → 3516.96] I probably won't worry about it too much.
[3516.96 → 3517.80] I suppose.
[3518.20 → 3518.32] Is it,
[3518.32 → 3520.66] is it not just x.com at Chris Lass?
[3523.12 → 3523.96] Too soon,
[3524.06 → 3524.36] Alex,
[3524.46 → 3525.04] too soon.
[3525.44 → 3528.00] I don't even like thinking about x.com.
[3528.08 → 3530.20] And you notice it's the X 11 logo too.
[3530.34 → 3530.52] Like,
[3530.58 → 3531.00] come on,
[3531.08 → 3531.20] man.
[3531.90 → 3532.40] Come on.
[3533.04 → 3533.40] Uh,
[3533.44 → 3536.08] I think we got a boost from Jared in Amelia,
[3536.30 → 3536.70] Idaho.
[3536.98 → 3537.24] No,
[3537.34 → 3537.64] Idaho,
[3537.86 → 3538.22] Ohio,
[3538.22 → 3538.58] Ohio,
[3538.72 → 3539.04] Ohio.
[3539.12 → 3540.22] I'm just checking right now on the map,
[3540.58 → 3540.86] Ohio.
[3541.08 → 3543.68] He sent us 10,000 and one seven SATs.
[3543.74 → 3544.86] And he gives us a zip code.
[3544.86 → 3546.32] So we could kind of figure out where he's at.
[3546.42 → 3546.62] He says,
[3546.62 → 3547.70] it's been a long time listener.
[3548.42 → 3548.74] And,
[3548.82 → 3548.98] uh,
[3548.98 → 3549.68] I like that.
[3549.76 → 3550.22] Thank you.
[3550.22 → 3551.16] And panicked ketchup,
[3551.32 → 3552.84] which is one of the best usernames out there.
[3553.32 → 3555.44] 13,000 SATs is our last booster this week.
[3555.48 → 3556.26] Cause you know,
[3556.26 → 3557.22] we got runtime here.
[3557.68 → 3558.20] He says,
[3558.28 → 3558.64] uh,
[3558.64 → 3561.82] I've been running a self-hosted unified controller on an old NFC with Ubuntu.
[3562.20 → 3566.44] I always kind of get nervous to do an update on the Ubuntu or the controller software.
[3566.54 → 3570.96] I was thinking about getting the unified cloud key generation two with the hard drive.
[3570.96 → 3576.62] I'm not sure if a dedicated device is the best option other than the option of doing a Ubiquity hosted,
[3577.22 → 3579.24] but I don't think I want to go that route.
[3579.46 → 3580.82] What do you guys think?
[3581.18 → 3582.82] If you're deploying this commercially,
[3582.82 → 3585.46] so you're running an MSP or something like that,
[3585.52 → 3586.72] you're charging people money.
[3587.46 → 3587.90] Absolutely.
[3588.28 → 3589.60] Cloud key all the way.
[3589.88 → 3591.38] And just don't worry about it.
[3592.06 → 3592.50] Uh,
[3592.68 → 3593.34] for,
[3593.48 → 3594.38] for home use though,
[3594.38 → 3597.66] I would say a self-hosted controller is more than adequate.
[3597.94 → 3599.50] You can back up the configs.
[3599.54 → 3600.32] You can export them.
[3600.32 → 3600.36] Um,
[3600.64 → 3602.64] I forget what the format is off the top of my head,
[3602.74 → 3604.20] but for example,
[3604.20 → 3606.84] when I did the 10 gig network upgrade in the spring,
[3606.84 → 3607.62] uh,
[3607.62 → 3614.68] I exported all of my devices from one site and imported them to another controller that I hosted in this building.
[3614.78 → 3617.04] So I used to only have a couple of Wi-Fi access points.
[3617.04 → 3620.96] And then I went all in on the Unify ecosystem and went to like 20 devices here.
[3620.96 → 3624.10] So I figured let's pull it out of the cloud and bring it in house.
[3624.56 → 3625.04] Uh,
[3625.04 → 3626.84] and that process was really painless.
[3626.98 → 3628.22] Don't fix what ain't broke,
[3628.60 → 3628.90] you know,
[3628.90 → 3629.50] uh,
[3629.50 → 3631.60] just make sure you've got regular backups and use,
[3631.60 → 3632.04] you know,
[3632.06 → 3634.82] ZFS data sets for the app data and you'll be fine.
[3635.36 → 3636.20] And maybe this is a
[3636.76 → 3642.50] something you just feel more comfortable running in a VM and you can take snapshots before major software upgrades.
[3642.76 → 3643.20] Um,
[3643.20 → 3646.04] and since we've gone so hard on Nix this episode,
[3646.18 → 3647.90] I'll make one more Nix mention.
[3648.34 → 3653.26] And that is just that this is one of the things you don't worry about in Nix anymore is these upgrades,
[3653.36 → 3654.18] breaking things.
[3654.36 → 3654.72] Um,
[3654.72 → 3658.28] if it does by some chance build and still break,
[3658.28 → 3661.78] you just select the last version in grub and go back to the way it was.
[3662.16 → 3663.10] That's really nice,
[3663.10 → 3666.58] but you can replicate that with any distribution with file system snapshots,
[3666.64 → 3668.64] or maybe even more simply VM snapshots.
[3669.28 → 3670.16] Good luck panicked.
[3670.38 → 3670.66] Uh,
[3670.66 → 3672.34] I think that's a good project to take on though.
[3672.62 → 3674.34] Thank you everybody that boosted in.
[3674.38 → 3674.78] I am sorry.
[3674.84 → 3675.78] We did not get to all of them,
[3675.82 → 3676.74] but we do read all of them.
[3676.80 → 3680.10] We share them in our team chat, and we store all of them in the show doc.
[3680.10 → 3682.12] So this episode's doc will have your boost forever.
[3682.34 → 3686.74] We had 31 boosts across 22 boosters.
[3686.84 → 3687.18] Totally.
[3688.08 → 3688.52] Awesome.
[3688.66 → 3688.98] Amazing.
[3689.12 → 3689.44] Thank you,
[3689.52 → 3689.88] everybody.
[3690.12 → 3690.32] Uh,
[3690.32 → 3693.08] some of you sending multiple messages with nice long messages,
[3693.08 → 3696.84] and we got a total of 239,313 SATs.
[3697.00 → 3699.64] You guys are absolutely the best, and we appreciate your support.
[3699.82 → 3705.08] You can boost into the podcast by getting a new podcast app at new podcast apps.com,
[3705.08 → 3707.96] or just go get Alfie and boost from the web,
[3708.04 → 3708.72] get albie.com,
[3708.72 → 3711.24] and then head over to the podcast index, and you'll find self-hosted over there.
[3711.30 → 3713.06] We got links to all of it in the show notes.
[3713.54 → 3713.56] Yes,
[3713.58 → 3713.90] we do.
[3714.00 → 3717.94] And of course we need to thank our site reliability engineers,
[3718.04 → 3719.14] the SRE subscribers.
[3719.52 → 3721.74] You are another part of what makes this show possible.
[3722.66 → 3723.02] Uh,
[3723.04 → 3723.82] you can go to self-hosted.
[3723.96 → 3725.22] Dot show slash SRE,
[3725.22 → 3728.74] and we've got an ad free feed over there for you with a post show.
[3728.86 → 3729.88] What are we going to talk about this week?
[3730.10 → 3733.18] I got a couple of ideas out here in the woods hunting animals.
[3733.28 → 3733.36] No,
[3733.40 → 3733.74] not really,
[3734.04 → 3734.96] but I do have a few ideas.
[3735.32 → 3736.06] Smoking those meats.
[3736.22 → 3736.46] I hope.
[3738.18 → 3738.70] Smoking the meat.
[3738.72 → 3739.36] And grilling.
[3739.54 → 3741.34] Thank you to our site reliability engineers.
[3741.44 → 3742.24] We really appreciate it.
[3742.30 → 3742.56] Alex,
[3742.64 → 3744.04] where can they find you on the internet?
[3744.30 → 3744.44] Well,
[3744.46 → 3746.94] don't forget about the meetup coming up in Chicago as well.
[3747.24 → 3748.10] Potential meetup.
[3748.18 → 3748.80] I will say,
[3748.90 → 3749.24] uh,
[3749.24 → 3750.18] around DevOps day,
[3750.30 → 3750.72] Chicago,
[3751.00 → 3752.98] probably the Tuesday or the Wednesday evening,
[3753.52 → 3754.68] maybe the Thursday evening.
[3754.68 → 3755.20] Who knows?
[3755.20 → 3756.46] Because I fly out on Friday morning.
[3757.54 → 3757.98] Um,
[3758.14 → 3759.08] but you can go to self-hosted.
[3759.22 → 3762.86] Dot show slash contact to send in your feedback directly to the show.
[3762.86 → 3764.98] And you can find me over at Alex.
[3765.34 → 3766.00] Katie's ed.
[3766.28 → 3766.54] Dot me.
[3766.88 → 3768.02] And come join us in the matrix.
[3768.72 → 3770.48] Jupiter broadcasting.com slash matrix.
[3770.58 → 3775.10] We've got a big old matrix or where we self-host with lots of rooms in there for every type of discussion,
[3775.20 → 3776.04] including self-hosting.
[3776.04 → 3776.90] And,
[3777.00 → 3777.02] uh,
[3777.02 → 3779.10] you can find me in there as well at Chris LAS.
[3779.30 → 3780.14] Thanks for joining us.
[3780.26 → 3781.74] This is episode one Oh two.
[3782.84 → 3783.48] Yeah.
