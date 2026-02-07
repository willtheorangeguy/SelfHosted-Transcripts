[0.00 --> 5.26]  If we had a laws of self-hosting, I think this would be in the top 10.
[5.50 --> 8.02]  And it would be the easier something is to set up and share,
[8.68 --> 12.24]  the more likely it's eventually going to cost you something.
[12.38 --> 16.68]  Like those 10-minute, super smooth, really nice UI, get things set up,
[16.74 --> 20.20]  and now you're using some sort of proxy cloud service to share stuff.
[20.76 --> 22.44]  Eventually someone has to pay that bill.
[22.68 --> 23.24]  You know what I mean?
[23.30 --> 25.02]  Like it always ends up happening that way.
[25.26 --> 27.62]  And the easy stuff always seems to be where it goes first.
[27.62 --> 30.58]  I absolutely feel that way about snaps.
[30.94 --> 31.88]  The Ubuntu snaps?
[32.20 --> 33.92]  Yeah, yeah, Ubuntu snaps.
[34.06 --> 35.48]  Sorry any Ubuntu people listening.
[35.76 --> 39.18]  But, you know, for example, someone setting up Nextcloud,
[39.44 --> 41.62]  oh, you just do snap install Nextcloud.
[42.22 --> 44.14]  Okay, but where's the data live?
[44.36 --> 45.88]  What's the database back end?
[46.04 --> 50.46]  Like there's a bunch of questions that you should be answering before you set things up.
[50.48 --> 55.20]  And I don't want to sound too gatekeepy in saying this stuff.
[55.20 --> 59.18]  Like we should be working towards making things easy,
[59.18 --> 63.84]  but there's also a balance, a trade-off to be made between the level of magic
[63.84 --> 68.18]  and the simplicity of deployment.
[68.46 --> 70.18]  Like too much magic is a bad thing.
[70.90 --> 71.92]  Yeah, I agree there.
[72.02 --> 75.68]  I think, I was just thinking, what if they had like a little YAML file
[75.68 --> 78.60]  and you could specify, and I'm like, well, you just created Docker Compose.
[78.62 --> 79.78]  You just created Docker Compose.
[79.78 --> 86.68]  Yeah, I started thinking about that really just because of the news this week from Plex.
[87.04 --> 88.34]  They've had a week, haven't they?
[88.46 --> 89.24]  My goodness.
[89.70 --> 93.76]  It's like they're trying to burn, deliberately burn any goodwill they've got left.
[93.76 --> 98.60]  Yeah, I was thinking, Alex, their arc on this show, it starts with Plex.
[99.20 --> 100.52]  We're doing great.
[100.66 --> 102.58]  We had them on the show.
[102.80 --> 104.70]  Like it was the gateway into self-hosting.
[104.98 --> 111.54]  And here we are at episode 145 now, and it feels like they've really taken a turn.
[112.12 --> 115.50]  Now, of course, there's a price increase that always makes some people upset.
[115.62 --> 117.68]  That's taking effect April 29th, 2025.
[118.50 --> 121.26]  But this is their first price hike in a while.
[121.26 --> 124.20]  So, okay, it's not so bad, I suppose.
[124.42 --> 128.52]  You're going from $120 for the lifetime now to $250 for the lifetime.
[128.70 --> 129.64]  So it's a jump.
[129.76 --> 130.22]  It's a jump.
[130.44 --> 132.56]  But that's not really the bad news.
[133.32 --> 133.70]  No, not really.
[133.76 --> 139.86]  I bought my lifetime pass 10 years ago for about $75, and that was looking like a smarter and smarter investment.
[139.86 --> 153.20]  But on top of the price increases, Plex are also making some significant changes to putting remote playback behind a paywall.
[153.30 --> 158.96]  They're taking a free feature and locking it behind the Plex Pass subscription.
[158.96 --> 161.20]  Yeah, that's the big one.
[161.44 --> 172.42]  So after April 29th, you'll have to have Plex Pass to remotely stream from someone else's Plex server or any users you've invited to stream from your Plex server.
[172.92 --> 176.34]  They're also going to offer now a remote watch pass.
[176.42 --> 177.32]  This is like a new thing.
[177.46 --> 179.64]  It's $2 a month or $20 a year.
[180.32 --> 184.04]  So you can get that for a little bit less than a Plex Pass, easy for me to say.
[184.16 --> 187.52]  And then you can still get remote streaming from friends and family, I guess.
[187.70 --> 188.70]  So, I mean, it's $2 a month.
[188.74 --> 189.92]  If you use it a lot, maybe it's worth it.
[190.34 --> 204.54]  Now, we should probably temper any panic at this point by saying that if you already have a subscription for a lifetime pass or a Plex Pass before the cutoff date of, what is it, April 29th, you will be grandfathered in.
[204.54 --> 210.22]  I don't know how that works for rolling monthly customers at least, but certainly for lifetime customers.
[210.52 --> 218.18]  You'll be grandfathered in, at least for now, to be able to continue doing remote watch and all that kind of stuff.
[218.58 --> 228.26]  And anybody that, if you are as the admin of the server, are the Plex Pass subscriber, anybody that you share that server with, so friends and family, they won't need a Plex Pass.
[228.50 --> 230.28]  Only the admin of the server does.
[230.28 --> 236.84]  So, for now, at least, in the short term, it's not a pants on fire emergency situation.
[237.12 --> 252.32]  But what it does do, for me, is it highlights a very worrying trend in the Plex management suite of, let's take our core product and monetize the heck out of it in the most egregious way that we can, you know?
[252.32 --> 259.94]  Right, the red flag here really is a core product feature, which has always been free, is now going behind a paywall.
[260.46 --> 261.48]  The feature.
[261.98 --> 263.20]  Take your media anywhere.
[263.40 --> 265.56]  Wasn't that Plex's strapline for a while?
[265.70 --> 266.26]  Watch anywhere?
[266.74 --> 267.10]  Indeed.
[267.42 --> 271.20]  I mean, it's, to me, an indication that maybe things are desperate.
[271.66 --> 273.26]  I mean, that's just speculation on my part.
[273.26 --> 281.98]  I mean, everybody on the internet knows you don't take something that's been free the whole time and part of the core product and move it behind the paywall.
[282.14 --> 287.66]  You knew cool stuff that adds a lot of value that people really want, but it's new.
[288.12 --> 290.72]  They put that behind the paywall all the time and people live with that.
[290.90 --> 292.16]  But something that's been free?
[292.80 --> 294.52]  And then you make you pay for it?
[295.00 --> 296.60]  I mean, that always gets people upset.
[296.86 --> 297.80]  That's just the way it is.
[297.94 --> 298.12]  Yeah.
[298.12 --> 301.36]  Once it's free, it should always be free.
[301.90 --> 310.00]  And, you know, I just wonder, why is there no innovation from Plex to add new features?
[310.52 --> 314.84]  One feature that comes to mind immediately is audiobook support.
[315.30 --> 318.62]  We've been asking for that for years.
[319.16 --> 322.92]  And, yes, there's Prologue on iOS and Plapper and Audiobookshelf.
[322.92 --> 332.22]  There are apps that have come along to fill that gap, but it's been a top feature on the Plex request in the forum for years at this point.
[332.60 --> 344.52]  And if they'd come out today and said, we're going to add audiobooks and it's a one-time unlock of $50 or something for even if you're a lifetime subscriber or something, different story.
[344.90 --> 348.26]  But taking a feature that was free and making it paid is just no bueno.
[348.98 --> 350.56]  There are things that are low-hanging fruit.
[350.56 --> 362.94]  You know, those of us that are on limited connections, I would happily, happily understand if they made downloading on the Android TV and iOS TV platforms a paywalled feature.
[363.50 --> 365.86]  I mean, I wouldn't love it, but I understand.
[366.02 --> 376.08]  Just let me download files on the TV so that way I can, before a movie starts, maybe I can get 15 minutes in so I don't have to worry about buffering and I can look at watching the highest quality.
[376.14 --> 377.14]  It's just such a basic feature.
[377.14 --> 378.84]  There are some improvements.
[379.02 --> 382.66]  The one-minute playback limitation on iOS and Android apps is going to be removed.
[383.14 --> 385.36]  So local playback on mobile is now free.
[386.30 --> 392.74]  And then I think probably the bigger thing that's a longer-term win, Plex is updating their privacy policy in terms of service.
[393.44 --> 395.62]  They say they're adding transparency about data usage.
[396.30 --> 400.58]  And they say no data about your personal media or server usage will be sold or collected.
[400.58 --> 404.10]  And consent for new data use will be requested.
[404.46 --> 408.68]  Yeah, that's a pretty big change in stance for the company, actually.
[408.80 --> 418.20]  If we think back to the faux social network that they tried to put together a few months ago, where they started to broadcast everybody's watch history to everybody else.
[419.20 --> 421.04]  You know, okay.
[421.04 --> 423.54]  If this is true, great.
[423.74 --> 425.14]  I'm glad to see that.
[425.64 --> 432.38]  But, you know, the good news is tempered with yet more bad news because the watch together feature is going away as well.
[432.84 --> 433.06]  True.
[433.40 --> 433.58]  Yeah.
[433.58 --> 440.34]  Yeah, that, I mean, maybe there was some sort of server side I could understand, you know, their proxy and the connections there.
[441.04 --> 442.86]  So maybe there was some cost to them.
[442.94 --> 449.92]  But as far as I understood, once the streaming started, it was from Plex instance to Plex client.
[450.04 --> 451.62]  It didn't have to go through their servers.
[451.62 --> 457.20]  So you wouldn't think it was a big overhead for them, but I'm sure it's technically a tricky feature to maintain.
[457.50 --> 457.60]  Yeah.
[457.62 --> 458.18]  What do we know?
[458.24 --> 459.88]  We're just pesky end users, huh?
[460.30 --> 460.54]  Yeah.
[461.16 --> 461.96]  Pesky end users.
[462.06 --> 463.16]  Just like our features.
[463.58 --> 468.50]  I mean, the reality is I'm very happy with my Jellyfin setup now.
[468.60 --> 469.54]  It works fantastic.
[469.70 --> 477.40]  But when I travel, I almost always end up falling back on Plex because either where I'm staying, they have a Plex app built into the TV.
[478.22 --> 482.94]  Or where I'm staying, it's easier to stream from one of my friend's systems, perhaps.
[483.64 --> 489.32]  And so I lean on Plex still for basically the friends and family streaming aspect of it.
[489.56 --> 492.06]  And I, like yourself, have the lifetime subscription.
[492.06 --> 500.18]  But I don't think I'm going to, in good conscience, recommend friends and family that get new systems down the road, get Plex and get the lifetime subscription.
[500.18 --> 504.08]  I just feel like the deal's changing too often.
[504.48 --> 506.54]  I do appreciate the new privacy policy improvements.
[506.54 --> 510.14]  But all in all, I think the package isn't quite as attractive as it used to be.
[510.76 --> 511.86]  I mean, what do you make of this, right?
[511.92 --> 512.84]  Plex is a company.
[513.30 --> 513.58]  Okay.
[513.72 --> 515.20]  And companies have to make money.
[515.20 --> 527.66]  And the reality of the situation is that most people with Plex libraries acquired their content in interesting ways.
[527.98 --> 530.16]  And there is no way to monetize that.
[530.64 --> 538.54]  We've put up with the in-s***-fication creep over the last few years of adding ad-supported this and ad-supported that.
[538.68 --> 540.40]  And do you remember Plex Arcade for a bit?
[540.48 --> 541.58]  That kind of came and went.
[541.58 --> 543.42]  And is that even still a feature?
[543.50 --> 543.88]  I don't know.
[544.38 --> 546.72]  But, like, they've got to make money somehow.
[547.54 --> 551.02]  And I just think they're going about it in the wrong way.
[551.20 --> 555.62]  Like, innovate rather than what's even the right word?
[555.90 --> 556.88]  Like, feature gate?
[557.02 --> 557.96]  I mean, the reality is.
[558.20 --> 558.46]  Innovate.
[558.62 --> 559.40]  Don't feature gate.
[559.60 --> 561.08]  That's the strap line.
[561.08 --> 573.74]  I feel like they need to go out into the real world and use Plex in the real world and just feel the pain points that are just out there that are low-hanging fruit that they could monetize.
[574.46 --> 576.08]  We've mentioned a couple of them in this show.
[576.12 --> 576.52]  They're there.
[576.94 --> 578.56]  They're available for the grabbing.
[579.00 --> 580.98]  But I think maybe they're too insulated.
[581.12 --> 584.98]  They're looking at it from a KPI and kind of goal standpoint.
[584.98 --> 590.02]  They're not looking at it from actual end users out in the real world, at least it seems to me.
[590.10 --> 592.02]  Otherwise, some of these features would be obvious to them.
[592.60 --> 594.98]  Yeah, don't even get me started on the current state of downloads.
[595.10 --> 597.38]  I mean, yes, technically they do work.
[597.50 --> 603.80]  But I can only set – I used to be able to set a per movie or a per series quality threshold.
[603.90 --> 608.32]  And it would transcode the files and then shoot them across the network to my iPad or whatever.
[608.38 --> 609.76]  And I used to do that every night before.
[609.76 --> 614.18]  I used to have to commute from Norwich to London on the train for two-plus hours each way.
[614.26 --> 618.48]  So I used to load the iPad up the night before with the current episodes or whatever I was watching.
[619.08 --> 619.10]  Yeah.
[619.50 --> 621.06]  And, you know, it was great.
[621.16 --> 625.54]  I could just be like, right, well, this cartoon I'll put in 480p because I really don't care about South Park.
[626.08 --> 629.56]  And we should note, when you got back, what you watched would sync up with your server.
[629.64 --> 633.64]  So the watch status would be all in sync with your mobile setup and your home setup.
[633.88 --> 634.12]  Yeah.
[634.72 --> 635.56]  It was great.
[635.64 --> 638.50]  I used it consistently for flights for a long time.
[638.50 --> 649.68]  Stuff like that, I would happily – the transaction from Plex, for me, was $75 one time 10 years ago.
[649.82 --> 653.08]  And I've used it every single day near enough since.
[653.56 --> 655.26]  I understand that's not sustainable.
[656.18 --> 660.02]  But as I keep saying, innovate, don't feature gain.
[660.54 --> 660.70]  Right.
[661.18 --> 662.30]  Create Plex Plus for me.
[662.68 --> 666.42]  Plex Pass Plus and improve the mobile clients.
[666.42 --> 675.24]  Improve the TV clients and then give me as a Plex Plus user, let me have access to the beta APK.
[675.96 --> 677.94]  You know, I mean, let's fix these features.
[678.04 --> 678.80]  Fix the download client.
[679.10 --> 690.12]  Why have both of Alex and I switched to use Infuse with local files on the file system on our iOS devices for travel instead of using PlexSync or something like that?
[690.60 --> 691.92]  It's just they've slid.
[691.92 --> 692.56]  You're right, Alex.
[692.92 --> 694.46]  Once again, you've nailed it.
[695.40 --> 699.28]  And then, you know, the comment sphere on Reddit, of course.
[699.90 --> 701.86]  All roads lead to Jellyfin, apparently.
[702.00 --> 706.40]  I'm not necessarily sure I 100% agree with that take.
[707.10 --> 709.72]  Jellyfin, as you know, on this show back in – when was it?
[710.10 --> 712.20]  January, what, two years ago?
[712.20 --> 718.40]  We did Jellyfin January and both Chris and I were very pleasantly surprised by the state of Jellyfin.
[719.12 --> 722.20]  There are just a few rough edges still remain.
[723.50 --> 728.40]  You know, just stuff like tone mapping support, HDR stuff is a little bit wonky sometimes.
[729.10 --> 731.44]  Live TV is not always perfect.
[732.34 --> 739.36]  Just a general fit and finish of the clients just isn't quite as high-end as the Plex clients.
[739.36 --> 758.56]  And this is all very minor stuff, but those paper cuts add up to, overall, a mildly worse user experience, which is just enough sometimes to push me over the edge, particularly when traveling, to go back to Plex, which I've kept running in the background because it runs my wife's audiobook server for Prolog.
[758.56 --> 762.88]  So it's not much of a stretch for me to switch between the two.
[763.02 --> 765.02]  And on my TVs, it's fine.
[765.16 --> 766.78]  I just use Jellyfin all the time.
[766.98 --> 767.44]  It just works.
[767.62 --> 768.90]  It does the thing for the most part.
[769.78 --> 771.42]  But I've always got Plex running in the background.
[771.56 --> 786.98]  And I would really genuinely love if Jellyfin could just close that last 5%, 10% in user experience to match Plex and really just shut this conversation down once and for all.
[786.98 --> 792.06]  Tailscale.com slash self-hosted.
[792.16 --> 796.84]  Tailscale is the easiest way to connect devices and services to each other, wherever they are.
[797.08 --> 798.14]  It's modern networking.
[798.42 --> 800.42]  It'll connect your devices securely.
[800.58 --> 801.46]  It's great for companies.
[801.98 --> 803.74]  And it's great for self-hosters, too.
[803.74 --> 810.16]  I'm talking secure remote access to your production systems, your servers, your database, your mobile device, whatever it might be.
[810.60 --> 812.62]  And Tailscale's really, really fast.
[812.62 --> 815.88]  It's privacy for everyone and every organization.
[816.30 --> 817.62]  And it's protected by WireGuard.
[818.70 --> 823.38]  I use Tailscale exclusively for managing and syncing all of my private data.
[823.76 --> 825.98]  My mobile devices only sync over Tailscale.
[826.32 --> 829.38]  All of my self-hosted infrastructure exists on my Tailnet.
[829.72 --> 831.86]  I have nothing exposed to the public internet.
[831.86 --> 843.46]  And the thing that's great about Tailscale is you can sign up at tailscale.com slash self-hosted and get it for free for up to 100 devices and three users, no credit card required, not a limited time trial.
[843.88 --> 844.96]  That's the starting plan.
[845.22 --> 846.32]  You'll get a taste of it.
[846.60 --> 848.82]  You'll be plenty at 100 devices for yourself.
[848.98 --> 851.56]  But then you'll know, hey, maybe this is something we want to use at work, too.
[852.44 --> 854.00]  There's lots of great options for businesses.
[854.00 --> 860.70]  And thousands of companies like Instacart, Hugging Face, Duolingo, Jupyter Broadcasting, and many more have switched to Tailscale.
[861.14 --> 863.10]  It's so great and fast to set up, too.
[863.42 --> 868.52]  And I use Tailscale also to authorize all of my SSH logins so I don't have to copy keys around.
[868.86 --> 873.04]  If a device is authorized to my Tailnet and my client is authorized, I sign right in.
[873.12 --> 873.78]  No password.
[874.02 --> 875.66]  It's chef's kiss.
[875.96 --> 877.98]  There's lots of great tooling built around Tailscale.
[878.34 --> 880.58]  So go check it out and support the show.
[880.58 --> 886.48]  See why I and so many others in the audience and thousands of businesses just love Tailscale.
[886.66 --> 890.36]  It makes old VPNs seem like something out of the 90s.
[890.54 --> 892.38]  This is the way it should have always been.
[892.84 --> 893.42]  And you'll love it.
[893.50 --> 896.42]  Tailscale.com slash self-hosted.
[897.94 --> 900.64]  Now, did listener Jeff deliver my package to you?
[901.08 --> 907.14]  I got this tiny little Apollo Air one that fits in the palm of my hand.
[907.64 --> 910.02]  And when they say it's compact, they are not kidding.
[910.02 --> 917.14]  And it is the Air one quality sensor that integrates automatically with Home Assistant from Apollo.
[917.28 --> 918.82]  It's powered by USB-C.
[919.34 --> 920.88]  It starts out on Bluetooth.
[921.30 --> 927.52]  Home Assistant immediately detects it and then walks you through getting it on Wi-Fi and into ESP Home.
[927.80 --> 929.00]  And then it shows up as a sensor.
[929.20 --> 932.74]  And I got the unit that has an actual CO2 sensor in it.
[932.76 --> 933.92]  You know, I've been looking for this.
[934.26 --> 937.10]  And they say that the sensors in this thing have about a 10-year lifespan.
[937.10 --> 940.00]  Now, the CO2 sensor is an add-on.
[940.50 --> 942.42]  So the unit starts at $92.99.
[943.06 --> 946.86]  But if you add the CO2 sensor, it comes out to about $113.
[946.86 --> 949.44]  So it's an optional add-on.
[949.54 --> 956.62]  And it technically doesn't meet the requirements for CO2 safety monitoring per, like, you know, government agencies and all that kind of thing.
[956.86 --> 958.16]  But it's monitoring CO2.
[959.04 --> 963.32]  Which is really what I wanted because it's been a journey trying to find the right one.
[963.32 --> 967.90]  And the software that runs on this thing and the CAD drawings are available up on GitHub.
[968.66 --> 970.62]  So it's all there if you kind of want to go through it.
[971.10 --> 972.76]  And it essentially runs on ESP Home.
[973.48 --> 976.24]  Designed, engineered, and assembled in the USA.
[977.14 --> 977.30]  Yeah.
[977.30 --> 991.20]  So, yeah, this is the same Apollo automation company that we talked about in the last episode that had just been certified as the first made-with-ESP Home that works with Home Assistant certified product line.
[991.90 --> 992.04]  Yeah.
[992.12 --> 996.42]  And it's pretty cool that we're at that point where that's a thing companies want to do.
[996.62 --> 997.56]  Heck, yeah, it is.
[997.76 --> 998.22]  It is.
[998.28 --> 999.86]  And it's so nice.
[999.86 --> 1001.42]  I mean, I'm not kidding.
[1001.50 --> 1003.14]  I plugged this thing into the USB-C power.
[1003.78 --> 1010.22]  And by the time I brought up the Home Assistant dashboard, you know, five seconds later, it was already in my notifications that it detected the device.
[1010.44 --> 1010.62]  Yeah.
[1010.80 --> 1012.60]  Because it just broadcasts over Bluetooth, doesn't it?
[1012.62 --> 1012.80]  Yeah.
[1013.02 --> 1016.36]  Yeah, I have the Bluetooth dongle hanging off of my Home Assistant box.
[1016.40 --> 1016.84]  So that helps.
[1016.92 --> 1019.46]  But then once you start the process, it's all Wi-Fi after that.
[1019.62 --> 1029.30]  That's the culmination of Home Assistant's strategy with ESP Home for, goodness me, when did they buy ESP Home or acquire them?
[1029.30 --> 1029.90]  They didn't buy them.
[1030.06 --> 1031.68]  They sort of acquired the project, didn't they?
[1031.74 --> 1032.12]  It's been a minute.
[1032.26 --> 1032.68]  It's been a minute.
[1032.98 --> 1033.22]  Yeah.
[1033.30 --> 1035.52]  And this is the culmination of years' worth of work.
[1035.60 --> 1041.36]  I remember, do you remember when we did a self-hosted live hack stream about WLED back in the day?
[1041.66 --> 1042.08]  Yeah, I do.
[1042.08 --> 1048.00]  And we were flashing Arduino code onto these boards, and it was all a little bit kind of sketchy and hacky.
[1048.20 --> 1049.60]  And it was fun, don't get me wrong.
[1049.60 --> 1065.20]  But for Home Assistant and its associated ecosystem of products like the Air One from Apollo Automation, to really stand a chance for muggles in the marketplace, it has to be as easy as you just described.
[1065.20 --> 1068.28]  I've really enjoyed testing it, too.
[1068.82 --> 1076.00]  So what I've realized is that when I'm home, the CO2 in the RV shoots up.
[1076.22 --> 1078.34]  And then when I leave, it goes down.
[1078.56 --> 1082.76]  And I definitely see it spike when I start the diesel heater for a bit.
[1082.82 --> 1087.14]  Just for a couple of minutes, when the diesel heater's starting up, it spikes up.
[1087.14 --> 1094.88]  And so it's been fun going to perplexity and researching the different parts per million CO2 levels, what they do.
[1095.30 --> 1096.12]  Do you feel it?
[1096.46 --> 1104.04]  Because I think one of the things, I got one of the, I forget the name of it now, but I got a different air quality sensor a little while ago for my office.
[1104.18 --> 1105.44]  That's only a small room right now.
[1106.18 --> 1114.08]  And I noticed that when I have the door closed when I'm filming, that I just feel a little prickly sometimes when the room is short of air.
[1114.08 --> 1119.42]  And sure enough, I can correlate that feeling with high CO2 levels.
[1119.50 --> 1120.66]  Have you felt anything like that?
[1121.12 --> 1123.80]  I haven't gotten there yet, although I'm going to start paying attention to that.
[1124.12 --> 1129.54]  But what I have noticed is definitely makes a difference when we're cooking if we have a window cracked.
[1130.06 --> 1136.72]  Now, I know that's obvious to say, but it is interesting, something that's just sort of, you know, common knowledge passed down.
[1136.80 --> 1139.44]  Everybody says, oh, yeah, crack a window if you have a gas stove or something like that.
[1140.14 --> 1142.64]  It's really fascinating to actually see it in the data.
[1142.64 --> 1152.92]  Yeah. And so I guess, according to perplexity, you usually have to get pretty high before it starts affecting, like, you know, your decision making and mental acuity.
[1153.56 --> 1159.00]  But, you know, maybe I'll get there, especially, you know, as I go through winter and I use different heaters and stuff like that.
[1159.08 --> 1160.82]  So I'm going to start paying attention.
[1160.98 --> 1163.78]  And I'll probably blame it on the CO2 levels regardless now.
[1164.16 --> 1166.88]  Yeah, yeah, you've got a new excuse under your belt, huh?
[1166.88 --> 1170.82]  Right. I can point at the chart and be like, look, honey, the CO2 levels were high. I couldn't make a decision.
[1171.20 --> 1174.86]  So this thing's about the size of what, a deck of cards or so?
[1175.38 --> 1178.60]  Yeah, it's a 3D printed case. It's a really well done one.
[1178.60 --> 1184.50]  And it's maybe a little narrower and a little thicker, but it's around the size of a deck of cards.
[1185.02 --> 1189.22]  And it says here in the documentation that it's just running an ESP32 inside.
[1189.52 --> 1189.68]  Yeah.
[1189.68 --> 1195.34]  So sometimes the temperature sensor needs a little offset due to heat buildup from that device that's inside.
[1196.02 --> 1198.18]  But have you found it to be accurate?
[1198.68 --> 1202.96]  Like, I don't have the temperature sensor up on a dashboard anywhere that I constantly am monitoring.
[1203.06 --> 1206.50]  But I did notice when I first fired it up that it seemed like it was reading a little bit warm.
[1207.40 --> 1208.82]  So that doesn't surprise me too much.
[1208.94 --> 1212.20]  In fact, if I go look at it right now, one of the things they do, this is really cool,
[1212.58 --> 1216.42]  is they do separate out in Home Assistant they have, when you're looking at the device,
[1216.42 --> 1220.84]  a separate diagnostic panel where they'll tell you the ESP's temperature.
[1220.96 --> 1225.00]  So right now the ESP that's running this thing is at 91.2 degrees.
[1226.46 --> 1231.24]  And it also tells me that it has a negative 29 BBM for the Wi-Fi.
[1231.64 --> 1232.84]  Yeah, in freedom units.
[1232.84 --> 1233.20]  Okay.
[1233.44 --> 1238.58]  And this current version, since I rebooted, it has been up for 83,000 seconds.
[1239.66 --> 1240.54]  So there you go.
[1240.82 --> 1241.06]  Yeah.
[1241.70 --> 1245.26]  Although it says my air quality is extremely abnormal right now.
[1245.26 --> 1250.06]  Oh, have you been eating baked beans or something?
[1250.88 --> 1252.10]  Maybe I'll have to ask the wife.
[1252.14 --> 1252.80]  She was home last.
[1253.40 --> 1253.98]  I'll have to ask her.
[1254.22 --> 1257.10]  Hey, my VOC meter says things are volatile.
[1257.34 --> 1258.36]  What's going on right now?
[1258.98 --> 1259.22]  Yeah.
[1259.80 --> 1264.30]  So I should point out, we had a couple of listeners write in and offer up a correction
[1264.30 --> 1270.30]  saying that you and I were talking about CO2, when actually they thought we meant CO for carbon monoxide.
[1270.30 --> 1278.26]  Obviously, it's an important distinction, but they are two different sensors that you can optionally add to this unit.
[1278.26 --> 1283.56]  So the unit that Chris has has the CO2 sensor optionally installed.
[1283.76 --> 1295.90]  You can also add a gas sensor based around a mix 4514 sensor that will detect CO, so carbon monoxide, ethanol, ammonia, and methane levels as well.
[1295.90 --> 1298.36]  Yeah, that I really want to add.
[1298.46 --> 1302.36]  You know, it does add to the cost a little bit, but their page makes it really easy to go through and configure.
[1303.02 --> 1305.24]  I'll put a link to this in the show notes because the page is awesome.
[1305.34 --> 1306.72]  So you start with no sensor.
[1306.84 --> 1308.06]  So you add the CO2 sensor.
[1308.36 --> 1313.44]  And if you add the gas sensor, you can also then add a GPIO header, which is kind of neat.
[1313.48 --> 1315.60]  And you can also opt to get it with a charger if you want.
[1315.60 --> 1318.18]  But I already have USB-C, so I don't need to do that.
[1318.52 --> 1325.44]  And when I add it with the gas sensor and the CO2 charger, the total price comes out to about 153 US dollars.
[1325.86 --> 1328.76]  Now, for me, I think it's worth it.
[1328.98 --> 1332.96]  I'd probably buy two of these, and they last about 10 years.
[1333.60 --> 1335.80]  And they're always going to work with Home Assistant.
[1335.92 --> 1342.30]  And I never have to worry about a cloud connection or even the vendor going away because the software is open source and it's ESPHome.
[1342.30 --> 1345.54]  So for me, it's open source, the little components inside.
[1345.80 --> 1347.06]  Yeah, it's kind of a no-brainer.
[1347.06 --> 1348.36]  Read and available from AliExpress, you know.
[1348.44 --> 1351.04]  And generally, good sensors are not cheap.
[1351.14 --> 1352.30]  That's what I have been discovering.
[1352.90 --> 1355.42]  I've seen stuff as expensive as, you know, 300, 400 bucks.
[1355.84 --> 1362.30]  So $153 with a gas sensor and a CO2 sensor and a temperature sensor and other things, it's not bad.
[1362.58 --> 1366.00]  I think I probably ended up ordering two myself.
[1367.54 --> 1369.84]  Then the review unit's done its trick, huh?
[1369.96 --> 1370.84]  Yeah, I guess so.
[1370.84 --> 1377.58]  So, of course, because it's an ESP32 underneath as well, it's got Bluetooth tracking capabilities built right in.
[1378.52 --> 1380.86]  You know, I hadn't really thought about what I would use that for.
[1380.92 --> 1386.86]  Is that maybe presence detection or what, like when just getting information on one of a certain devices nearby?
[1387.00 --> 1391.88]  Yeah, well, one of the use cases they have here is, say, attach a beacon to your dog's collar.
[1392.26 --> 1392.66]  Oh.
[1393.54 --> 1394.36]  Is Levi home?
[1394.82 --> 1396.60]  You know, that actually is a pretty great idea.
[1396.60 --> 1405.10]  That would be really great because I've thought about how do I set certain automations for when the humans are gone but the dog is home.
[1405.40 --> 1405.50]  Yeah.
[1405.68 --> 1405.92]  Hmm.
[1406.16 --> 1406.54]  That's how.
[1407.06 --> 1407.08]  Hmm.
[1407.90 --> 1408.38]  Cool.
[1409.10 --> 1418.16]  You just get yours and Hadia's Bluetooth IDs added into the database, whatever, and then have automations that track those three items and you're good to go.
[1418.16 --> 1422.28]  Unraid.net slash self-hosted.
[1422.48 --> 1428.32]  Unraid 7.1's beta is cooking right now and it is packed with exciting new features.
[1428.32 --> 1440.36]  First up, the big one for me, you wouldn't think it, but wireless networking is now officially supported, which means you can connect your Unraid server via Wi-Fi, which is great for setups where you just don't have access to Ethernet.
[1440.80 --> 1443.78]  Dorm rooms, city flats, you know, my RV.
[1444.08 --> 1446.64]  I mean, seriously, this is great for mobile rigs now, too.
[1447.14 --> 1451.90]  Or like the past week when I was at an Airbnb and all we had was access to Wi-Fi.
[1451.90 --> 1454.80]  We sort of roughly set up something that worked.
[1454.94 --> 1456.76]  This would have just made things so much easier.
[1456.94 --> 1468.86]  And the other nice thing that's in 7.1, especially for those of you that are moving from other platforms, it's now possible to import foreign ZFS pools easier than ever.
[1469.24 --> 1478.74]  So if you're switching, say, from TrueNAS or Proxmox or Ubuntu, Unraid will automatically detect and import your ZFS pools, simplifying that migration.
[1478.74 --> 1485.78]  And 7.1 just made virtualization and GPU support even better.
[1486.82 --> 1492.44]  Enhanced GPU support for Linux VMs in particular, including multi-screen setups.
[1493.10 --> 1495.72]  And I think the user VM templates feature is going to be really nice.
[1495.84 --> 1500.96]  Save and reuse custom VM configurations make it really streamlined to just spin up a new VM.
[1501.62 --> 1507.48]  And, of course, there's an updated Linux kernel in there, too, which has support for Intel's next-gen battle image, Goopoo.
[1508.00 --> 1508.16]  Yeah.
[1508.74 --> 1509.52]  I call it Goopoo.
[1509.60 --> 1509.98]  So what?
[1510.62 --> 1512.90]  What matters is that you go check out Unraid.
[1513.16 --> 1514.54]  Go check out the new features.
[1514.98 --> 1516.08]  Participate in the beta, too.
[1516.34 --> 1519.48]  It's available at unraid.net slash self-hosted.
[1519.74 --> 1520.72]  Head on over right now.
[1520.78 --> 1521.40]  Support the show.
[1521.56 --> 1523.92]  Unraid.net slash self-hosted.
[1524.24 --> 1524.58]  Unraid.
[1525.04 --> 1526.10]  Unleash your hardware.
[1527.86 --> 1528.50]  All right.
[1528.50 --> 1530.96]  So server shame time.
[1530.96 --> 1535.28]  My Epic server, as you all know, died just before I went to scale.
[1535.84 --> 1543.50]  And here we are over two weeks, nearly three weeks later, and I still don't have a functioning server.
[1544.14 --> 1544.36]  Oh, man.
[1544.38 --> 1545.02]  That's rough.
[1545.16 --> 1548.50]  Travel makes it hard to, you know, fix a server.
[1548.50 --> 1549.56]  So there's that factor.
[1549.96 --> 1550.06]  Yeah.
[1550.12 --> 1554.56]  I mean, putting together a server doesn't take that long.
[1554.56 --> 1559.12]  But I have had a time with Threadripper Pro.
[1560.12 --> 1560.90]  Oh, really?
[1561.50 --> 1563.20]  I take it not a good time?
[1563.58 --> 1563.90]  No.
[1564.20 --> 1564.58]  No.
[1564.78 --> 1564.92]  Okay.
[1565.08 --> 1566.00]  What's going on?
[1566.00 --> 1567.28]  We're about to part ways.
[1567.62 --> 1571.00]  So I'm going to take another trip to Charlotte to return it to Micro Center.
[1571.36 --> 1572.16]  Back to Micro Center?
[1572.16 --> 1573.50]  You just want to go back to Micro Center.
[1573.70 --> 1574.30]  I know you.
[1576.48 --> 1576.88]  Yeah.
[1577.00 --> 1577.74]  Well, okay.
[1577.78 --> 1581.34]  So there are lots of very nuanced reasons for this.
[1581.34 --> 1585.18]  But the biggest reason, well, there's two biggest reasons.
[1585.58 --> 1590.56]  First of all, it was a two grand purchase for a Zen 3 part.
[1591.22 --> 1594.72]  Now, Zen 3 was released about three years ago.
[1594.72 --> 1600.46]  Zen 3 is the architecture of the Threadripper Pro CPU 5000 series that I purchased.
[1601.16 --> 1602.58]  It doesn't sound like a big deal.
[1602.68 --> 1605.72]  You think, oh, yeah, two, three-year-old processor, fine, whatever.
[1606.52 --> 1614.58]  But then I started actually looking at benchmarks of the Zen 3 Threadripper Pro versus a 9950X,
[1614.62 --> 1618.02]  which is a Zen 5 AMD part, the Ryzen chip.
[1618.02 --> 1624.64]  It has roughly a 32% higher aggregate performance score compared to the Threadripper Pro,
[1624.76 --> 1632.54]  which when you consider that it's a desktop class chip versus a gargantuan hunk of silicon
[1632.54 --> 1639.10]  that's designed to go in a server with a million PCIe lanes, the performance is something you can't really ignore.
[1639.10 --> 1641.64]  So then I was going to live with it.
[1642.04 --> 1644.74]  And then I ran into a bunch of issues.
[1645.02 --> 1648.36]  I couldn't boot the Proxmox installer.
[1648.88 --> 1650.70]  Oh, OK.
[1651.48 --> 1655.28]  Yeah, I could boot the Nix installer, the Arch installer, Ubuntu.
[1655.48 --> 1656.26]  It was all fine.
[1656.62 --> 1660.04]  But Proxmox just would not boot.
[1660.04 --> 1664.88]  I have a HP, like one of their cheap servers that's in a workstation case.
[1665.00 --> 1666.28]  It was given to me, so I'm very grateful.
[1666.40 --> 1666.88]  I'm not complaining.
[1667.10 --> 1667.74]  But same deal.
[1667.90 --> 1670.32]  I can boot everything but Proxmox on that.
[1671.16 --> 1676.92]  So I ended up spelunking onto the internet trying to find out all the different PCI,
[1677.64 --> 1681.34]  all the different kernel command line flags that I could pass this thing.
[1681.84 --> 1686.30]  And in the end, I found one that worked, which was PCI equals NOM CONF,
[1686.70 --> 1688.00]  which is some kind of memory.
[1688.00 --> 1694.36]  It changes the way that PCI devices address the kernel or something.
[1694.52 --> 1694.72]  I don't know.
[1694.74 --> 1695.26]  It's kind of weird.
[1695.64 --> 1695.86]  OK.
[1696.28 --> 1699.24]  So that allowed me to boot the installer and get Proxmox installed.
[1700.18 --> 1703.24]  But I'm seeing a ton of errors in DMessage as I do it.
[1703.26 --> 1705.74]  And I'm like, oh, well, hopefully they'll go away once it reboots.
[1706.36 --> 1709.04]  So I rebooted into the fresh install.
[1709.14 --> 1716.64]  And I'm still seeing a bunch of errors related to PCI devices, bad TLP, bad DLLP errors.
[1716.64 --> 1721.00]  So I start, you know, asking Claude and perplexity, like, what's going on?
[1721.06 --> 1721.88]  What do these errors mean?
[1722.58 --> 1732.64]  And it turned out that the WRX80 motherboard from Asus has a pair of six-pin auxiliary power cables to power the seven PCI slots.
[1732.94 --> 1736.98]  I hadn't plugged them in because I was like, well, I've only got three devices in here, three of them.
[1736.98 --> 1737.60]  Oh, OK.
[1738.26 --> 1739.80]  So I'm like, doesn't matter.
[1740.00 --> 1740.72]  It'll be fine.
[1741.12 --> 1742.56]  So anyway, I plugged them in.
[1742.74 --> 1746.32]  And there are so many flipping PCI power ports on this motherboard.
[1746.46 --> 1749.36]  It's got the two eight-pin CPU ports.
[1749.58 --> 1754.26]  But it's also got an extra eight-pin port on the motherboard for the CPU because it draws so much.
[1754.34 --> 1763.20]  So there are three eight-pins for the CPU plus two six-pins for the PCI ports plus whatever ports are on the graphics cards themselves.
[1763.20 --> 1766.88]  My brand-new 1,200-watt power supply was out of cables.
[1767.28 --> 1778.08]  So I went to my old Bitcoin mining rig box of cables to pull out some old PCIe splitter power cables I used to have for that and got it powered up.
[1778.24 --> 1781.34]  And lo and behold, a couple of the PCIe errors went away.
[1781.96 --> 1783.04]  So lesson learned.
[1783.20 --> 1785.86]  Don't assume that power ports are optional, Alex.
[1786.02 --> 1788.68]  Just plug into them and have a good time.
[1788.68 --> 1799.04]  But no matter what I did, I could not get rid of the bad DLLP and bad TLP errors.
[1799.58 --> 1807.28]  So I reached out to a friend of the show, Wendell, to see if he could help me because he's done pretty much the only deep dive on this board on YouTube.
[1807.40 --> 1808.32]  So I knew he had one.
[1809.22 --> 1813.84]  And he went through the BIOS settings with me and we found a couple of extra things in there.
[1813.84 --> 1824.72]  Interestingly, AMD chips ship with IOMMU enabled, which is like the virtualization grouping of PCIe devices, enabled out of the box.
[1825.20 --> 1827.20]  And the BIOS setting says auto.
[1827.56 --> 1831.04]  So I take that to mean as, well, the AMD chip ship with it on.
[1831.28 --> 1831.88]  BIOS says auto.
[1831.98 --> 1832.80]  That means it's on, right?
[1833.34 --> 1833.58]  Nope.
[1834.12 --> 1837.36]  Turns out you can actually turn it more on than just on.
[1837.36 --> 1846.56]  So if you set it explicitly to on in the BIOS, then it will boot without the PCIe non-conf setting, I think.
[1846.72 --> 1846.80]  I see.
[1846.92 --> 1848.66]  So auto didn't mean auto on?
[1848.86 --> 1849.74]  It meant auto off?
[1849.94 --> 1852.26]  Just meant auto kind of halfway house.
[1853.24 --> 1853.64]  Yeah.
[1853.84 --> 1856.48]  Like if the OS triggers it in the right way, I guess?
[1856.60 --> 1856.84]  Yeah.
[1856.84 --> 1857.16]  It's strange.
[1857.32 --> 1857.52]  Okay.
[1858.96 --> 1860.42]  So, I don't know.
[1860.60 --> 1862.50]  I kind of got to thinking.
[1862.50 --> 1867.40]  And I took the weekend whilst we were at scale and I had a lot of time on the plane to think about what I was going to do.
[1868.08 --> 1884.52]  And I just couldn't live with the fact that I was going to drop two grand on a three-year-old part that was incompatible without some major messing about with Proxmox, the OS that I'm going to run on this thing.
[1884.52 --> 1891.76]  So I reached out to Micro Center and asked them if I could extend my return window by just a couple of days so I could take it back after scale.
[1892.20 --> 1894.76]  And they said, sure, we'll give you up to 30 days.
[1895.10 --> 1899.48]  So I'm probably going to go back to Charlotte this weekend as we record to take it back.
[1899.64 --> 1905.04]  And that led me down the path of thinking, well, okay, I don't have a Threadripper Pro in my life anymore.
[1905.78 --> 1906.60]  What am I going to do?
[1906.62 --> 1907.40]  I still need a server.
[1907.98 --> 1909.88]  And my media server is a separate box.
[1909.88 --> 1915.92]  There's an i5-13600K in the basement that's got a ton of hard drives in it and it's separate.
[1916.18 --> 1932.62]  And I'm very glad I made that decision to separate those two things between my home lab and pseudo-prod, you know, because it's meant that for the last month, well, three weeks or so, that my media situation hasn't been impacted at all by any of this messing about.
[1932.62 --> 1945.92]  So, you know, my budget for the upgrade was about two grand and I was looking at my options and AMD just went and dropped a 9950X 3D this week, didn't they?
[1946.34 --> 1948.12]  Okay, I'm following you now.
[1948.12 --> 1953.70]  So, the 9950X is the non-3D part.
[1953.84 --> 1972.34]  So, what that means, that difference, the X3D part means that it's got a bunch of extra V-cache, which is useful for highly sensitive workloads like gaming, where even the tiniest latency spike will result in a latency drop in frame buffering and that kind of stuff.
[1972.88 --> 1975.46]  On a server, I don't really care about that.
[1975.46 --> 1990.72]  You know, most of my workloads can be pinned to specific CCDs because the 9950X has two chiplets inside and there's huge latency if you try and access a workload from one CCD on the other one as it copies stuff across between those two contexts.
[1992.12 --> 2004.56]  And so, I sort of looked at the price difference and a 9950X 3D is about 750 if you can find one in stock versus the 9950X, which is about 500.
[2004.56 --> 2007.74]  And I'm thinking, well, that's half my motherboard paid for.
[2008.30 --> 2024.68]  So, I've gone for a 9950X and I've paired it with an Asus ProArt X870E motherboard, which seems like an odd choice, but there's a couple of really good reasons why I went for the kind of like high-end gaming motherboard on this system.
[2024.68 --> 2031.80]  And it's because the X870E, you can think of the E almost like extra, it gives you an extra chipset.
[2031.98 --> 2039.02]  So, the 9950X itself only provides 28 PCIe lanes out of the box.
[2040.04 --> 2046.54]  And 28, as you can probably do the maths, is a lot less than 128 that Threadripper Pro was offering me before.
[2047.00 --> 2047.38]  Yeah, okay.
[2047.38 --> 2053.08]  But the X870E adds 12 more lanes to that, so I've actually got 40 to play with.
[2053.60 --> 2056.12]  Remind me kind of roughly what you figure, how many you needed?
[2056.70 --> 2060.90]  Yeah, well, I should probably, you know, remind folks what a PCIe lane is even for.
[2061.36 --> 2065.02]  So, your graphics card will typically ask for 16 lanes.
[2065.02 --> 2075.12]  And what that means is it's got 16 direct electrical connections back to the CPU to copy data into and out of memory and, you know, process data and that kind of thing.
[2075.72 --> 2078.42]  An NVMe SSD might typically ask for four.
[2078.60 --> 2083.62]  Some high-end ones want more lanes than that, but for the most part, it's four lanes per SSD.
[2083.62 --> 2094.64]  So, by the time you add that up over a server, let's say you've got half a dozen SSDs all wanting four lanes each and a graphics card or maybe two, depending on what you're doing.
[2095.18 --> 2099.72]  You know, you can see how 40 lanes, you can run up against the limit of 40 pretty quickly.
[2100.34 --> 2106.52]  I can definitely see, especially for your use case, when you're going to have storage, you're going to have a GPU in there, you're going to be doing stuff that's definitely going to fill up that.
[2106.52 --> 2118.64]  So, this has led me to the conclusion that rather than building the one box to rule them all, one giant box of pain when it dies, why don't I build two?
[2119.12 --> 2126.90]  Because for the same money, I can literally build two 9950X systems as I could for one Threadripper Pro system.
[2127.82 --> 2132.98]  Now, I'm not going to build a second 9950X system because I don't need that much power.
[2132.98 --> 2137.38]  Because the 9950X is a screaming fast chip.
[2137.92 --> 2144.50]  So, I used to use, up until a few months ago, as my main gaming desktop, the i7-8700K.
[2145.10 --> 2155.92]  That chip clocks in at roughly 400% slower than the 9950X, just to give you an idea of how fast the Zen 5 parts are.
[2156.18 --> 2156.42]  Okay.
[2156.42 --> 2165.56]  And so, I'm just going to, I think, turn the i7, or the, I might use my old i5-8500 that I've still got from my old media server.
[2165.78 --> 2170.72]  I might use that as just a bog standard kind of storage box.
[2171.20 --> 2171.34]  Sure.
[2171.34 --> 2177.24]  So, I might end up with more servers on the LAN, but they were each going to have dedicated tasks.
[2177.48 --> 2183.20]  And if one goes out, then it doesn't, it's not like a domino effect that takes, like, everything with it.
[2183.24 --> 2188.14]  One's an app server, one's a storage server, one's a kind of home lab mucking about server.
[2188.38 --> 2190.62]  And that's kind of where I'm at.
[2191.08 --> 2196.08]  I could see you probably being a little more hands-on with the server that's going to be used for AI workloads,
[2196.08 --> 2197.34]  that's going to have the GPU.
[2197.48 --> 2198.78]  That could be touched a little more often.
[2198.78 --> 2200.64]  The storage box could last a long time.
[2201.16 --> 2201.44]  Exactly.
[2201.76 --> 2201.98]  Yeah.
[2202.46 --> 2204.16]  It's almost like there's a pattern for this.
[2204.22 --> 2208.64]  It's almost like people have figured this out before, and it's taken me years to get to the same conclusion.
[2209.04 --> 2211.44]  Well, it always kind of depends what, like, if you look at it from the,
[2211.54 --> 2215.58]  how can I reduce the amount of hardware and power usage and, you know, sprawl.
[2215.70 --> 2215.96]  Right.
[2216.08 --> 2218.00]  Then, you know, you get to the one box solution.
[2218.10 --> 2221.42]  But then when you think about it from a redundancy or reliability or simplicity,
[2221.90 --> 2223.84]  sometimes it does make sense to go multiple boxes.
[2224.22 --> 2228.76]  That was another thing about Threader Ripper Pro, too, is it sucks down the juice.
[2229.76 --> 2231.98]  Idle was about 220 watts.
[2232.08 --> 2232.26]  Oh!
[2234.16 --> 2239.78]  And, like, as soon as I fired up a Windows VM, a lot of the cores came out of sleep state,
[2240.50 --> 2242.76]  and it went straight up to 400 watts.
[2243.08 --> 2243.22]  No!
[2243.22 --> 2248.98]  Yeah, pretty much just sat there doing nothing but having VMs, you know, just waiting to do stuff.
[2249.94 --> 2253.02]  Yeah, sort of 380, 400 watts, pretty easy.
[2253.34 --> 2257.52]  So, not to say that Zen 5 is particularly fantastic.
[2257.72 --> 2260.74]  It's probably the only criticism I can levy against Zen 5, to be honest.
[2260.74 --> 2266.66]  At idle, the 9950X draws about 30 to 40 watts, which is still reasonable,
[2266.94 --> 2269.00]  but it's a lot more than an Intel chip would draw.
[2269.68 --> 2274.96]  However, the Intel chips, when you push them, the sky is the limit for those things.
[2275.14 --> 2277.60]  They can pull 300, 400 watts, no problem.
[2277.60 --> 2283.08]  Whereas the Zen 5 part, the 9950X, is kind of limited about 180 watts.
[2283.76 --> 2287.22]  So, you know, it's much more efficient under load, not quite as efficient at idle.
[2287.58 --> 2288.06]  Eh.
[2288.06 --> 2291.92]  Keeb.io slash self-hosted.
[2291.98 --> 2294.42]  K-E-E-B.io slash self-hosted.
[2294.46 --> 2297.80]  Head on over there, sign up for the newsletter, and get 5% off your next order.
[2298.26 --> 2302.32]  Let's face it, your keyboard might be one of the most important things you own.
[2302.72 --> 2308.14]  It took me a while to appreciate that, but, I mean, I'm interfacing with it every day, most of the day.
[2308.62 --> 2310.80]  It's the primary interface to my computer.
[2311.22 --> 2315.62]  And there's a lot of options out there, but I'm kind of somebody that likes a fancy keyboard now.
[2315.62 --> 2318.16]  I wasn't always this way, but I've seen the light.
[2318.72 --> 2323.58]  Keeb.io, they range from regular keyboards, and they really specialize in those cool split keyboards.
[2324.14 --> 2328.80]  And the keyboards, they'll come fully built, ready to use if that's how you like it, out of the box.
[2329.10 --> 2332.22]  Or you can get it as a kit and assemble it, do some hot swapping.
[2332.70 --> 2334.16]  There's no soldering for those parts.
[2334.26 --> 2336.06]  So it might be a fun project for home, too.
[2336.50 --> 2339.02]  Or, you know, if you just want to get started, you can get one that's fully built.
[2339.32 --> 2343.36]  The other thing that I think you should look at, and you could kind of up your game a little bit,
[2343.36 --> 2344.80]  is their macro pads.
[2345.02 --> 2347.92]  With those 9 to 16 keys, you can use them for all kinds of things.
[2348.00 --> 2351.26]  You can put phrases on there and have it connected to something like BitFocus.
[2352.26 --> 2353.80]  You could have it control OBS.
[2354.60 --> 2358.60]  You know, there's probably a way, using the Stream Deck software, to tie it in with Home Assistant as well.
[2358.82 --> 2361.24]  Or maybe it's a nice way to control your home media PC.
[2361.98 --> 2363.38]  I think those are so handy.
[2363.46 --> 2364.74]  We have a couple of them right here in the studio.
[2364.74 --> 2368.44]  In fact, I've got, look at this, I've got one right here.
[2368.44 --> 2372.92]  I love these little side things, you know, hook it up over USB.
[2373.08 --> 2373.80]  It's pretty great.
[2374.30 --> 2379.52]  I think people normally think of mechanical keyboards as loud and clicky, and those do exist.
[2379.92 --> 2385.58]  But they also have the versions with silent switches to keep things quiet and low-key in the office or at home.
[2385.82 --> 2388.32]  You know, I lack my loud typing.
[2388.52 --> 2389.60]  I'll be honest with you guys.
[2389.78 --> 2394.10]  But not everybody does, or sometimes the people around you don't.
[2394.10 --> 2399.62]  They stock lots of DIY parts and microcontrollers, and they're big supporters of open source.
[2399.72 --> 2405.64]  They publish the 3D print case parts, and they're also part of the core QMK team for the firmware.
[2405.84 --> 2408.00]  And all their boards use the QMK firmware.
[2408.56 --> 2410.02]  I love that.
[2410.66 --> 2412.16]  You deserve a great keyboard.
[2412.32 --> 2413.74]  Check them out and support the show.
[2414.12 --> 2417.40]  Go to keeb.io slash self-hosted.
[2417.48 --> 2420.82]  That's keeb.io slash self-hosted.
[2420.82 --> 2429.04]  So we mentioned Plex Arcade, and whether it died a death or not, I'm still honestly not sure.
[2429.12 --> 2431.28]  But I think you found a replacement anyway.
[2432.00 --> 2433.36]  Oh, have I?
[2433.44 --> 2434.10]  I'm really in love.
[2434.20 --> 2434.92]  And you know, it's funny.
[2435.88 --> 2438.40]  Desperation truly is the mother of invention.
[2438.70 --> 2447.62]  So this really all started because, I guess, I'm an old stick in the mud now, and I just love the Super Nintendo and some of the Super Nintendo games.
[2447.62 --> 2452.34]  And I wanted to see if I could get a better experience on my desktop than on the Switch emulator.
[2452.46 --> 2456.72]  Because the Switch emulator, when you're playing Super Ghouls and Ghosts, lags out real bad.
[2457.10 --> 2458.98]  And I think I could do better on my desktop.
[2459.16 --> 2462.76]  So I got like ZS, NES, or whatever it was, up and going for a couple of days.
[2463.06 --> 2463.84]  And it was doing better.
[2464.38 --> 2465.94]  And so I started getting my old games.
[2466.12 --> 2468.24]  You know, I got my old folder filled with ROMs.
[2468.42 --> 2470.98]  Like, it's got like 300 ROMs in this or more.
[2471.34 --> 2471.90]  Wow, really?
[2471.90 --> 2474.30]  Yeah, it's just a collection I've had forever.
[2475.16 --> 2476.60]  And I start going through them.
[2476.70 --> 2477.92]  I'm playing them, and I'm enjoying them a lot.
[2478.62 --> 2482.66]  And I don't know if I did a system update or if I rebooted or what I did.
[2483.06 --> 2489.04]  But when I came back next time to use ZS, NES, or whatever it was, I just got a blank screen, and I couldn't play the games.
[2489.36 --> 2490.00]  Nothing would play.
[2490.94 --> 2493.86]  And, you know, I played around trying to get it working again.
[2494.14 --> 2494.82]  Couldn't get it working.
[2494.94 --> 2496.84]  And I thought, there's got to be a better way.
[2497.24 --> 2499.24]  There needs to be a way that's system independent.
[2499.24 --> 2501.66]  I don't want to have to set this up every time.
[2502.12 --> 2504.12]  That's where I came across ROMM.
[2504.70 --> 2505.94]  Stands for ROM Manager.
[2506.78 --> 2511.70]  And you could think of it as a bit of a plex or a jellyfin for your ROMs.
[2512.20 --> 2513.42]  I mean, it scans them.
[2513.50 --> 2514.62]  It pulls down the metadata.
[2514.88 --> 2516.32]  It gives you a nice web interface.
[2516.72 --> 2518.88]  It does collections and favorites.
[2520.62 --> 2524.10]  And perhaps the best part, which solved my problem,
[2524.10 --> 2529.88]  it allows you to play many of those games directly in the browser using Emulator.js.
[2530.06 --> 2531.06]  Oh, really?
[2531.56 --> 2531.82]  Yeah.
[2531.96 --> 2532.14]  Cool.
[2532.72 --> 2533.68]  Yeah, it's pretty great.
[2533.88 --> 2537.48]  It supports MAME, Nintendo games, Sony PlayStation games,
[2537.60 --> 2540.48]  anything that Emulator.js supports, which is a lot of them.
[2541.24 --> 2545.54]  And it also supports some, you know, classic PC games.
[2545.54 --> 2549.70]  But you upload the ROMs or you just have it, you point it at a folder structure.
[2549.86 --> 2556.14]  I will say it is very picky about the folder structure and the naming of the ROM files.
[2556.34 --> 2558.60]  You got to do it exactly like they say.
[2558.66 --> 2564.30]  It's like the old days when, you know, like old TV media is really before Plex and some of those.
[2564.54 --> 2568.96]  Like you really had to be very careful about the folder structure of your media files.
[2569.16 --> 2570.36]  It's very much like that.
[2570.36 --> 2572.10]  So you do want to read through their docs.
[2572.18 --> 2573.70]  I'll link to the quick start guide.
[2574.28 --> 2576.72]  But assuming you get the directory structure and the naming right,
[2577.24 --> 2579.38]  then, of course, it's a Docker composed setup.
[2579.52 --> 2582.38]  So you punch through where you have the files at.
[2583.18 --> 2588.68]  And you do need to either get a few credentials or APIs for some of the services that they use
[2588.68 --> 2590.20]  to scrape the metadata.
[2590.38 --> 2592.34]  And if you don't, you don't get metadata.
[2592.60 --> 2594.24]  So you do have to do that part.
[2594.74 --> 2597.26]  So you're uploading, you know, like for me,
[2597.26 --> 2599.66]  I had to go create an account at like Steam Grid DB.
[2601.24 --> 2602.46]  And some of the services.
[2602.46 --> 2605.86]  I was going to ask, is that one of those need to know question and answer situations?
[2606.06 --> 2607.68]  No, it's their normal services.
[2607.68 --> 2609.06]  Like another one's owned by Twitch.
[2609.54 --> 2610.52]  It's all in their docs.
[2610.72 --> 2610.90]  Yeah.
[2611.22 --> 2614.24]  So if you have a Twitch account, you have access to like, I guess,
[2614.40 --> 2617.26]  scrape a library of video game images and metadata.
[2618.30 --> 2618.94]  Of course.
[2619.44 --> 2621.24]  And you just need an API key for that.
[2621.76 --> 2624.42]  So it's not like FanArt TV that's just open.
[2625.44 --> 2625.80]  No.
[2626.00 --> 2626.94]  No, unfortunately not.
[2626.94 --> 2627.64]  I was hoping.
[2627.96 --> 2629.18]  I didn't want to have to go do it.
[2629.18 --> 2632.22]  I tried first not to put any credentials or API keys in there,
[2632.28 --> 2633.52]  and I got no metadata at all.
[2634.70 --> 2636.34]  Can you cache that stuff locally?
[2636.46 --> 2636.76]  Do you know?
[2637.68 --> 2637.80]  Yeah.
[2637.88 --> 2641.30]  I assume it's putting it locally.
[2641.38 --> 2643.84]  Although I don't know about on the end client, but yeah, on the server.
[2644.46 --> 2648.78]  Once you grab it, but it's really finicky on the naming.
[2649.04 --> 2651.90]  And the manual search is slow, but there is a manual search process.
[2652.00 --> 2653.56]  And then it'll pull it all down and save it locally.
[2654.76 --> 2655.12]  Awesome.
[2655.12 --> 2656.48]  Yeah, that's nice.
[2657.02 --> 2660.26]  I have to say, very impressed with how well it works.
[2660.72 --> 2662.04]  Had a few audio issues in Firefox.
[2662.32 --> 2663.94]  Had zero problems in Chrome.
[2665.24 --> 2669.28]  And once it's up and going, it's delightful.
[2669.62 --> 2672.12]  I am really, really, really pleased with it.
[2672.12 --> 2679.68]  And I'm already collecting some of my favorites into like, you know, I have a Mario collection across multiple platforms.
[2679.86 --> 2685.52]  So you go into one collection, it's Mario for, I don't know, six or seven different consoles.
[2685.70 --> 2686.94]  So it's like all the Mario games.
[2687.04 --> 2687.74]  It's really great.
[2688.14 --> 2690.20]  Do the save games end up living on the server side?
[2690.92 --> 2692.04]  That is client side.
[2692.52 --> 2693.56]  That is client side.
[2693.72 --> 2696.20]  You can export a file and then bring that with you.
[2696.20 --> 2700.44]  And then when you load the client in the web version, you can load in a save version.
[2700.52 --> 2702.82]  But if you're always playing from the same web browser, it'll save.
[2704.22 --> 2704.40]  Yeah.
[2704.46 --> 2707.38]  It also supports like Game Genie cheat codes if you want to roll that way.
[2708.84 --> 2709.64]  I don't know.
[2710.16 --> 2711.46]  That just wrecks the game for me.
[2711.50 --> 2712.46]  But I love that it has it.
[2712.70 --> 2717.92]  And Alex, it's pretty slick because, you know, when you're dealing with these old ROMs, small.
[2717.92 --> 2723.04]  And so I have this thing running on my old Droid, which, as you know, is behind my Starlink.
[2723.52 --> 2730.50]  And I'm pulling up these SNES and Game Boy games in the web browser here at the studio, streaming them over the Starlink.
[2731.00 --> 2732.84]  And it's perfectly, perfectly fine.
[2732.86 --> 2733.06]  Overstop?
[2733.18 --> 2733.42]  No.
[2733.82 --> 2734.02]  Yeah.
[2734.28 --> 2736.30]  Yeah, because it pulls the ROM down and then plays it.
[2736.50 --> 2739.34]  So, you know, the ROM is only like a megabyte or whatever.
[2739.66 --> 2741.12]  So it's like instant, basically.
[2741.14 --> 2741.56]  Oh, right.
[2741.96 --> 2742.20]  Yeah.
[2742.90 --> 2744.14]  And I assume that's over tail scale.
[2744.58 --> 2745.34]  Yes, of course.
[2745.34 --> 2748.38]  And, you know, now I'm thinking I'm going to use it on the road, too.
[2748.50 --> 2749.68]  This is the way I'm going to play these now.
[2750.16 --> 2751.56]  Now, there are a few games.
[2751.86 --> 2753.36]  Like, it doesn't have a Switch emulator.
[2753.82 --> 2757.62]  It doesn't have a couple of other emulators built into the web client.
[2758.12 --> 2759.64]  But it will still organize them.
[2759.68 --> 2760.44]  It'll still do the metadata.
[2760.64 --> 2761.68]  You can still add them to collections.
[2761.88 --> 2766.22]  And then when you pull it up in the web page, it gives you just a real quick button for any of these.
[2766.32 --> 2769.96]  But even the ones that doesn't have a built-in emulator gives you just a quick button to download the ROM.
[2770.52 --> 2771.46]  Assuming you have a local player.
[2771.46 --> 2778.50]  So it's still, even if it doesn't have built-in playback support, a really nice way to organize various ROMs.
[2778.72 --> 2780.26]  Like maybe Xbox 360 ROMs.
[2780.28 --> 2782.82]  I think it's another one that doesn't play yet in the browser.
[2783.02 --> 2786.88]  But it still has all of the back-end support for those types of games.
[2787.36 --> 2792.12]  Also, they've been really clever in how they support games that have multiple files.
[2792.24 --> 2795.28]  So some of the PlayStation games, some of the MAME games.
[2795.42 --> 2797.28]  They have a whole directory of files.
[2797.42 --> 2798.68]  And it's aware of that.
[2798.68 --> 2804.04]  And then lastly, what I really like about it is you can choose to manage the files on your file system.
[2804.20 --> 2805.68]  Like, you know, I brought 300 ROMs.
[2806.48 --> 2811.40]  But then going forward, you tell the system, my SNES games are here.
[2811.82 --> 2813.04]  You know, my Game Boy games are here.
[2813.12 --> 2814.56]  My PlayStation games are in this folder.
[2815.06 --> 2819.24]  So then going forward, you can upload a ROM directly from the web interface.
[2819.24 --> 2824.56]  And it will properly categorize and file it on the back-end into the correct directory on your file system.
[2825.06 --> 2826.04]  So you could use either approach.
[2826.32 --> 2834.74]  And it will rescan kind of like your Plex or Jellyfin will from time to time on a scheduled basis to make sure it's got all the files and all the metadata for those files.
[2834.74 --> 2839.22]  These last two segments are why I love self-hosting so much.
[2839.44 --> 2839.76]  Yeah.
[2840.24 --> 2841.78]  You own the data.
[2842.06 --> 2843.96]  And also you own the outages too.
[2844.12 --> 2847.46]  Like, you know, if it goes out, there's nobody to blame but yourself.
[2847.80 --> 2858.32]  But also, like this one, you know, the ROM manager, you are putting craft and care into organizing this collection probably now for the last time in your life.
[2858.74 --> 2860.04]  This will stick with you forever.
[2860.04 --> 2863.98]  Yeah, and it's great too because I message the kids, you know, I'm like, hey, it's set up.
[2864.06 --> 2866.04]  Just go to this URL because they're on the tail net.
[2866.26 --> 2867.30]  They're all on the tail net.
[2867.42 --> 2872.28]  So I just send them a URL in their browser or in their message app and they click it and they're playing the games.
[2872.68 --> 2873.48]  It's so cool.
[2873.72 --> 2873.84]  Wow.
[2874.40 --> 2876.18]  Kids have never been less productive, huh?
[2876.30 --> 2876.60]  I know.
[2876.80 --> 2877.88]  They're so dang lucky.
[2879.82 --> 2880.18]  Yeah.
[2880.62 --> 2883.82]  Your self-hosting is just, it's the gift that keeps on giving.
[2883.82 --> 2889.02]  And I know that sounds like when that's the name above the door, it sounds like a shill.
[2889.02 --> 2890.94]  How can I shill something that's free?
[2891.12 --> 2893.06]  And just, it's such a great community.
[2893.06 --> 2895.34]  And I was struck by that at scale once again.
[2895.42 --> 2904.32]  Like every time I meet people in Meatspace, it's just a reminder of how awesome the people on the other end of this microphone are listening.
[2904.62 --> 2908.02]  And projects like ROM app, they're just fantastic.
[2909.24 --> 2915.02]  Clearly, they were created to scratch the itch of one or two people at the beginning and they've blossomed.
[2915.02 --> 2918.92]  I mean, this is on version 3.8 now, so it's clearly been around for some time.
[2920.12 --> 2922.10]  Oh, what a fantastic project.
[2922.56 --> 2922.68]  Yeah.
[2922.82 --> 2925.50]  And I should mention, it is AGPL.
[2925.74 --> 2927.54]  So it's open source.
[2927.72 --> 2928.42]  It's free.
[2928.88 --> 2932.14]  And like Alex said, they're pretty active.
[2932.50 --> 2935.86]  It's mostly a Python app on the back end.
[2936.34 --> 2938.70]  You know, all you have to worry about is a little Docker Compose.
[2938.76 --> 2940.14]  And it's a pretty simple Docker Compose.
[2940.14 --> 2943.92]  It does set up a couple of database stuff, but nothing too major there.
[2944.12 --> 2947.06]  The project looks like it's about to celebrate its second birthday.
[2947.22 --> 2952.04]  It was V1 was uploaded to GitHub on March the 27th, 2023.
[2953.04 --> 2955.40]  Now we have a couple of boosts to get to.
[2955.50 --> 2956.98]  We just have a few this week for time.
[2957.44 --> 2961.98]  And Bronze and Wing is our first booster with 13,332 sats.
[2962.88 --> 2967.44]  And Adversaries is technically our baller booster, but we read his, we snuck his in a little early.
[2967.44 --> 2970.50]  They ask, have you seen Kometa for Plex?
[2970.58 --> 2973.16]  It's a Python script that adds metadata to your library.
[2973.34 --> 2978.62]  I'm using it to pull in from commonsenseratings.org to replace the awful PG and PG-13 rating scheme.
[2978.94 --> 2981.40]  Then I restrict my kids' accounts to their appropriate age.
[2981.90 --> 2983.76]  The Plex accounts are clean content only.
[2983.88 --> 2984.58]  It's super nice.
[2985.72 --> 2988.02]  Although, not happy about the killing the watch together feature.
[2988.82 --> 2989.98]  Are you familiar with these?
[2990.22 --> 2993.32]  I mean, I know there's lots of this kind of stuff out there, but this one in particular,
[2993.32 --> 2997.64]  this co-meta that seems like it pulls from commonsense ratings.
[2998.08 --> 3000.30]  It could be interesting as, you know.
[3000.88 --> 3001.94]  Yeah, it's interesting, actually.
[3002.22 --> 3006.78]  This comment is almost foreshadowing Plex's announcement today.
[3007.10 --> 3007.40]  Yeah.
[3007.72 --> 3012.84]  Actually, one thing we didn't talk about in the news segment was Plex are adding a native
[3012.84 --> 3020.90]  integration with commonsense ratings or commonsense media for child-friendly or parent-approved
[3020.90 --> 3026.06]  ratings, not just, you know, the Film Bureau or Board of America-approved ratings.
[3026.54 --> 3026.68]  Yeah.
[3026.76 --> 3030.04]  But Co-Meta used to be called Plex Meta Manager.
[3030.22 --> 3030.72]  You might know it.
[3030.72 --> 3031.30]  Oh, yes.
[3031.64 --> 3032.00]  Oh, yes.
[3032.04 --> 3033.54]  You're the artist formerly known as.
[3033.94 --> 3034.14]  Yep.
[3034.20 --> 3034.44]  Okay.
[3034.80 --> 3038.38]  And this thing is, it's really very, very powerful.
[3038.50 --> 3042.02]  You can use it to spin up collections for Halloween and Christmas and stuff like that.
[3042.02 --> 3046.80]  But it's configured through a very complicated series of YAML files.
[3046.90 --> 3049.52]  And honestly, it's kind of a pig to set up.
[3049.70 --> 3052.74]  It's, once you've got it set, it's fine.
[3053.30 --> 3057.94]  But it's just not, I don't know how you'd make it any better, to be honest.
[3058.14 --> 3061.26]  So, you know, Alex, STF you.
[3061.46 --> 3065.06]  But it's just one of those projects that I'm really glad it exists.
[3065.30 --> 3067.08]  And I have set it up several times.
[3067.08 --> 3069.00]  And then it broke for some reason.
[3069.00 --> 3072.88]  And I've never bothered to fix it because I remember how hard it was the first time.
[3073.22 --> 3073.96]  That was me, too.
[3074.18 --> 3075.32]  And then Halloween rolls around.
[3075.40 --> 3077.12]  And I'm like, oh, well, I want my holiday collections.
[3077.26 --> 3079.04]  And it's pretty much an annual tradition at this point.
[3079.84 --> 3081.68]  So, you know, I agree.
[3081.88 --> 3087.16]  And my really low-key solution is I just broke out Halloween and Christmas into their own libraries.
[3087.16 --> 3091.38]  And then I disable those libraries until it's time appropriate.
[3091.64 --> 3100.32]  But Bronze Wing's suggestion here of restricting the kids' accounts to their age rather than, because, you know, I have a separate library for Ella right now.
[3100.48 --> 3101.68]  Yeah, that's how I do it, too.
[3101.84 --> 3102.38]  It's fine.
[3102.44 --> 3104.14]  Like, it doesn't take up that much disk space.
[3104.26 --> 3106.96]  But, you know, she asked for a Wallace and Gromit movie the other day.
[3107.04 --> 3109.84]  And I have those in the adult library because I like them.
[3110.12 --> 3110.46]  Yes.
[3110.84 --> 3112.12]  And I was looking in the kids' library.
[3112.20 --> 3112.98]  I'm like, where are they?
[3113.00 --> 3113.74]  I know I've got them.
[3113.74 --> 3115.88]  I do that, too, like with Back to the Future.
[3116.38 --> 3116.58]  Yeah.
[3116.86 --> 3117.38]  Other things.
[3117.48 --> 3117.68]  Yeah.
[3117.94 --> 3122.02]  And now that my kids are getting older, they're starting to watch some of the same shows we are.
[3122.14 --> 3123.96]  So the line's blurring even further.
[3124.40 --> 3124.68]  Yeah.
[3124.82 --> 3128.34]  And now it's, like, getting really out of date that I have a kid's library and a parent's library.
[3128.50 --> 3129.78]  I do have to figure it out soon.
[3129.84 --> 3141.40]  It's almost like I wish there was a way, as part of the metadata schema, to tag a show or a movie to be a member of multiple libraries.
[3142.06 --> 3142.42]  Yeah.
[3142.42 --> 3146.40]  I guess you could maybe do it through a collection, like a family collection, but that's not really what you want.
[3146.56 --> 3147.62]  I like your idea better.
[3148.08 --> 3148.38]  Yeah.
[3148.58 --> 3148.86]  Yeah.
[3149.08 --> 3150.14]  Like a meta library.
[3150.26 --> 3150.46]  Yeah.
[3150.58 --> 3163.14]  Like some kind of info file that you could put in the directory with the files or something that Plex or Jellyfin will pick up and say, you know, if you find a library that matches this name, be a member of this one and this one.
[3163.50 --> 3164.18]  Yeah, I like that.
[3164.86 --> 3165.14]  There you go.
[3165.20 --> 3166.00]  I've just solved it for you.
[3166.00 --> 3166.54]  There's another feature.
[3166.68 --> 3168.78]  Three great features we've given them this week.
[3168.78 --> 3172.12]  They also added, I just swapped from Blue Iris to Frigate.
[3172.28 --> 3172.72]  Wow.
[3172.80 --> 3173.50]  What an improvement.
[3173.94 --> 3178.80]  The AI detections are amazing and you can run it all on the IGU.
[3179.26 --> 3181.48]  Maybe a Frigate April challenge.
[3182.14 --> 3182.28]  Yeah.
[3182.36 --> 3183.04]  It's about time.
[3183.10 --> 3187.08]  My Blue Iris box has been chugging away for about, well, when did I buy this house?
[3187.34 --> 3187.78]  2019.
[3188.52 --> 3192.14]  It's been chugging away, you know, quite happily in the corner all that time.
[3193.10 --> 3193.54]  Maybe.
[3194.20 --> 3195.06]  Maybe it's time.
[3195.46 --> 3202.12]  I've got to find new cameras, you know, because I've been using these old modified Wises forever and they're not great for this kind of thing.
[3202.54 --> 3208.68]  But I don't have Ethernet and I do have USB micro where all these Wise cams are.
[3209.10 --> 3216.04]  So I need something that would work great with Frigate that could do Wi-Fi and maybe I could power over USB.
[3216.70 --> 3220.68]  And if I could find something like that and I could replace those Wises, that'd be so great.
[3221.06 --> 3222.00]  Write in and let us know.
[3222.00 --> 3226.04]  I would love to know what you're doing for sort of AI person detection.
[3226.28 --> 3227.26]  There's Frigate.
[3227.42 --> 3229.20]  There's another one that's name escapes me.
[3229.52 --> 3233.06]  But a lot of these things are based around that Coral TPU.
[3233.46 --> 3233.82]  Right.
[3233.92 --> 3237.64]  Which at this point, I recall, was out of stock during COVID.
[3237.84 --> 3243.72]  So surely it's there's like a Coral 2 or something available now.
[3243.96 --> 3249.62]  Or maybe we can run it through an LLM or something for better detection.
[3250.20 --> 3250.50]  Right.
[3250.50 --> 3252.66]  Where's the LLM powered one?
[3252.76 --> 3253.26]  Where's that?
[3253.62 --> 3253.92]  Yeah.
[3254.10 --> 3255.20]  Let us know what you're doing.
[3255.30 --> 3258.42]  I want to take my CCTV to the next level.
[3258.98 --> 3259.60]  Yeah, there you go.
[3260.14 --> 3263.36]  WH-2250 is with you on Micro Center.
[3263.92 --> 3266.86]  It says, I lived five minutes from one when I was in grad school and broke.
[3267.24 --> 3271.94]  Now that I can do more than walk around and dream, the closest is 5.5 hours away.
[3272.60 --> 3274.28]  But it's worth the overnight trip.
[3274.64 --> 3274.86]  Yeah.
[3274.86 --> 3277.82]  Well, you heard earlier in the show, I found an excuse to go back.
[3278.44 --> 3278.64]  Yeah.
[3278.86 --> 3279.64]  That's a good trick.
[3279.74 --> 3280.54]  That's a good way to do it.
[3281.38 --> 3283.12]  Last but not least, I pulled this one up.
[3283.16 --> 3287.42]  The hotel guy with 1,000 sats, he just wanted to chime in on Alarmo.
[3288.30 --> 3289.10]  So did listener Jeff.
[3289.14 --> 3291.82]  He says, you can pick up a Z-Wave keypad and integrate.
[3292.34 --> 3297.42]  Personally, I picked up a ring keypad, added it through Z-Wave, and I used this blueprint, which he linked me to.
[3298.24 --> 3299.04]  Fantastic, yeah.
[3299.16 --> 3300.10]  So I'm looking into that.
[3301.26 --> 3305.18]  That's two plus ones I've gotten for the ring keypad of all things.
[3305.26 --> 3305.86]  Who would have known?
[3305.86 --> 3307.24]  I never would have looked at that.
[3307.46 --> 3307.56]  No.
[3308.16 --> 3308.82]  Thank you, everybody.
[3308.98 --> 3313.16]  I am thinking I'm going to start slowly but surely building this alarm system.
[3313.54 --> 3315.84]  I don't really have like a master plan at the moment.
[3315.84 --> 3323.96]  But with NFC tags and maybe a keypad, I think I could have everything I need to arm and disarm it.
[3324.12 --> 3327.62]  And what would be really great would be to work it in with a camera system.
[3328.26 --> 3329.02]  That would be great.
[3330.00 --> 3333.66]  Well, you sure have a perfect spot to do it with the RV.
[3333.94 --> 3337.48]  It shouldn't cost you an arm and a leg to arm that space.
[3337.96 --> 3338.20]  Right.
[3339.02 --> 3340.58]  It's kind of how crazy do I want to go?
[3342.18 --> 3343.40]  Always super crazy.
[3343.40 --> 3352.02]  Now, last episode, we talked a little bit about notifications and how people break through, do not disturb, and that kind of thing.
[3352.04 --> 3355.80]  And we mentioned pushover thanks to some feedback that we got from a listener.
[3356.32 --> 3363.98]  But we also got a bunch more feedback about the feedback that we didn't mention Notify, a self-hosted alternative to pushover.
[3364.42 --> 3367.84]  So consider Notify mentioned duly on the show.
[3367.84 --> 3376.38]  This is a self-hosted way of hosting a notification library on your own infrastructure, and it will support all of the major endpoints.
[3376.62 --> 3387.00]  I think it's an apprise type situation where it will interface with a bunch of other APIs and endpoints to send notifications natively as well as through other services.
[3387.00 --> 3390.08]  It's something I do think about about once a year.
[3390.28 --> 3398.02]  And then I kind of end up on this sort of conclusion that I would probably still end up needing the Play API because some apps wouldn't support this.
[3398.46 --> 3404.74]  So any in-the-real-world experience with how that works, or maybe there's solutions for that, I would also love to know.
[3404.74 --> 3408.08]  And also, how truly self-hosted is it?
[3408.18 --> 3411.72]  Is there some kind of forwarding server in the cloud?
[3411.76 --> 3419.26]  Because there is a paid Notify Pro tier where you can pay, I think, about $5 a month if you want to to support the development.
[3419.42 --> 3423.84]  But does that give you any kind of a hosted version?
[3424.04 --> 3427.52]  Like, how truly self-hosted and self-contained is this thing?
[3427.86 --> 3428.02]  Yeah.
[3428.08 --> 3430.56]  We'll do some research for an upcoming episode as well, of course.
[3430.56 --> 3433.02]  But if you're already using it, write in and let us know.
[3433.46 --> 3433.86]  Yeah, definitely.
[3433.86 --> 3435.80]  And thank you, everybody, who boosted into the show.
[3436.02 --> 3440.10]  We'll have links to Fountain and Strike, which are easy ways to get sats and boost and support the show directly.
[3440.22 --> 3441.66]  That was episode 145.
[3442.14 --> 3447.00]  And all of the boosts that didn't make it in the show and more will be in the Boost Barn linked in the show notes.
[3447.58 --> 3453.40]  You mentioned it, but just a quick formal shout-out to everybody who came and said hi at the Scale meetup.
[3453.46 --> 3454.18]  That was great.
[3454.36 --> 3454.78]  Oh, yeah.
[3455.78 --> 3458.94]  I think we upset the Mexican restaurant that we went to a bit.
[3458.94 --> 3459.12]  Yeah.
[3459.40 --> 3461.74]  They were champs, so we didn't know.
[3461.74 --> 3463.82]  In the end, they were super grumpy when we got there.
[3464.02 --> 3464.80]  Yes, yes.
[3465.26 --> 3466.08]  Yes, they were.
[3466.52 --> 3474.86]  Well, here's the thing is we had about 35 people sign up for the meetup, and so we told them to expect about 40, 45-ish.
[3475.38 --> 3480.64]  And so they set aside one of their little ballrooms for us, and then over 100 people showed up.
[3480.64 --> 3487.32]  So they scrambled and quickly set up another ballroom on the other side of the bar.
[3487.42 --> 3489.04]  So we had a bar between us, which was kind of nice.
[3489.36 --> 3493.82]  But it did mean people got separated out, and some of them spilled out into the general dining area, too.
[3494.50 --> 3498.86]  They did eventually recover and said, okay, next year, let's plan for a bigger one.
[3498.94 --> 3503.00]  And they have a whole plan of attack, and so they're willing to work with us again.
[3503.08 --> 3504.88]  So we didn't piss them off too much, I guess.
[3504.88 --> 3505.12]  Good.
[3505.34 --> 3506.12]  Good to hear that.
[3506.36 --> 3506.70]  I know.
[3507.02 --> 3507.34]  It was a good meetup.
[3507.34 --> 3508.74]  A deer must have worked her magic on them.
[3509.14 --> 3509.78]  Yeah, she did.
[3509.88 --> 3510.56]  That's always nice.
[3510.64 --> 3512.50]  The wife is great at smoothing those things over.
[3512.58 --> 3514.60]  And then if she can't do it, you throw Brent at them, you know?
[3514.60 --> 3517.58]  Yes, that's, yeah.
[3518.32 --> 3520.42]  Between the two of them, you usually get smoothed over.
[3520.82 --> 3521.60]  But it was great.
[3522.10 --> 3524.24]  And it's always really nice people come up and say they're members, too.
[3524.48 --> 3526.16]  I always like to give them a good handshake.
[3526.24 --> 3526.98]  So thank you to everybody.
[3527.62 --> 3531.60]  Even if we didn't get to see you, if you support the show with a membership, we really appreciate it.
[3531.72 --> 3532.76]  You get a little extra.
[3532.88 --> 3535.54]  You get an ad-free version of the show, and you get a post-show.
[3535.78 --> 3536.66]  A little extra content.
[3537.38 --> 3540.60]  Details and sign up at selfhosted.show.sre.
[3540.60 --> 3541.26]  S-R-E.
[3541.48 --> 3547.66]  And if you do want to come to a future meetup, you can go to meetup.com slash Jupiter Broadcasting.
[3548.28 --> 3554.72]  Our spring season isn't quite as crazy as last year, but Linux Fest Northwest is around the corner, right?
[3555.14 --> 3555.40]  Yeah.
[3555.86 --> 3557.86]  Yeah, there's a few things coming up, you know?
[3557.90 --> 3561.06]  And then there'll be a Texas Linux Fest later in the year if we can make that work.
[3561.18 --> 3561.72]  So definitely.
[3562.14 --> 3562.92]  And all things open.
[3563.02 --> 3563.70]  Are you coming to that?
[3563.96 --> 3564.20]  Yeah.
[3564.32 --> 3566.20]  Well, if I can, that'd be another one I'd love to come to.
[3566.30 --> 3569.10]  So at least a few that we try to get some meetups around.
[3569.10 --> 3572.08]  So meetup.com slash Jupiter Broadcasting could be worth watching.
[3572.64 --> 3576.86]  I think there's a full road trip in your itinerary.
[3576.94 --> 3577.42]  Oh my gosh, I'd love that.
[3577.42 --> 3579.88]  Because you've got Texas Linux Fest.
[3580.32 --> 3582.78]  I think it's 6 and 7 of October.
[3582.78 --> 3585.42]  And then you've got all things open about a week later in Raleigh.
[3585.42 --> 3586.26]  Ah, okay.
[3586.30 --> 3588.32]  It's only a time to get from Austin to Raleigh, I'm just saying.
[3588.36 --> 3589.92]  I like what you're cooking, Alex.
[3592.02 --> 3596.30]  As always, you can go to selfhosted.show slash contact to get in touch with us.
[3596.30 --> 3598.72]  Or selfhosted at jupiterbroadcasting.com.
[3598.80 --> 3600.20]  Or, of course, boost in as well.
[3600.94 --> 3604.30]  And you can find me on the wild web, chrislas.com.
[3604.78 --> 3606.40]  Or pretty much chrislas everywhere.
[3606.88 --> 3607.96]  On all the different places.
[3608.42 --> 3609.06]  You can find me there.
[3609.58 --> 3612.10]  The show is at selfhostedshow on Twitter.
[3612.46 --> 3613.78]  I still refuse to call it X.
[3613.84 --> 3615.92]  And honestly, I've kind of dropped it these days.
[3616.02 --> 3617.62]  Like I'm on Mastodon.
[3617.94 --> 3620.06]  If you want to find me over there, techhub.social.
[3620.56 --> 3621.48]  Thanks for listening, everybody.
[3621.48 --> 3624.22]  That was selfhosted.show slash 145.
[3626.30 --> 3656.28]  Thank you.
