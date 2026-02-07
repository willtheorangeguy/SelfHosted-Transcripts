[0.00 → 4.56] Well, it's the end of the month, and that means it is the end of our Jellyfin Challenge.
[5.40 → 6.28] We all tried it.
[6.68 → 8.32] I don't know if we're any worse for the wear or not.
[8.38 → 10.24] We'll find out as the episode goes on.
[10.30 → 12.82] But Alex, I see a smile on your face, so it couldn't have gone that bad.
[13.08 → 14.00] It's still running.
[14.26 → 16.06] It's defied all expectations.
[16.98 → 20.34] Hey, we're giving the good stuff away in the first 30 seconds of the episode here.
[20.36 → 21.00] What's going on?
[21.00 → 26.98] If we were proper podcasters, we'd say some boring stuff for the first 15, 20 minutes,
[26.98 → 30.14] and then say, don't forget to watch to the end, like, comment, and subscribe.
[30.96 → 31.20] Oh, yeah.
[31.28 → 32.96] Do you guys want to have some friendly banter?
[33.04 → 35.74] We could have a line in the doc that says friendly banter.
[35.88 → 38.30] We could do that for a little bit and tease it out.
[38.36 → 40.80] No, we wanted to get right to it this week because it's a big topic.
[41.16 → 46.90] And to help us fill out the roundtable is, of course, our buddy Brent is back.
[47.00 → 47.72] Hello, Brent Lee.
[47.76 → 48.14] Well, hello.
[48.26 → 49.12] Thanks for having me again.
[49.50 → 51.44] Well, thank you for joining us on this Jellyfin Challenge.
[51.52 → 54.62] And then I think for the first time ever on the show, Alex's wife Kat's here.
[54.74 → 55.20] Hello, Catherine.
[55.28 → 56.06] Thanks for joining us.
[56.06 → 56.38] Hi.
[56.38 → 56.58] Hi.
[56.76 → 56.98] Hi.
[57.06 → 60.80] And thanks for also being willing to give us the spousal approval factor,
[61.40 → 64.46] the legit, genuine spousal approval factor right here on the show.
[64.60 → 65.36] The real review.
[66.08 → 66.82] The real deal.
[66.98 → 67.60] So appreciate it.
[68.20 → 71.40] I just thought it was super important to get the wife's perspective,
[71.60 → 77.54] given that she is at least 50% of the user base of the TV in this house.
[79.14 → 80.06] For now.
[80.38 → 81.26] For now.
[81.46 → 83.30] Until that kid of yours gets older.
[83.66 → 84.34] Ella's coming.
[84.58 → 84.72] Yeah.
[84.72 → 85.32] She's coming.
[85.32 → 88.50] And you're going to have a whole new set of libraries just for the kid.
[88.70 → 89.28] It's starting.
[89.58 → 90.98] We've got Bluey already, Mike.
[91.40 → 91.98] On tap.
[94.02 → 97.68] Well, you know, we've talked on and off about the switch to Jellyfin.
[97.68 → 101.94] Just to recap, if you're joining us now, the idea was to see if we could make it a whole
[101.94 → 104.20] month switching from Plex.
[104.20 → 105.90] And we're all huge Plex enthusiasts.
[105.90 → 112.20] So it seemed like something worth trying because we like the ideas of our media server not requiring
[112.20 → 116.10] any connection to the internet or login, not really necessarily having a strategy tax where
[116.10 → 117.62] they have to look like a streaming company.
[117.62 → 120.00] And of course, we like it to be open source.
[120.00 → 122.50] If it's got something we're going to self-host and run for a long time.
[123.04 → 127.66] Jellyfin checked all those boxes, but we knew it would have some issues compared to Plex.
[128.04 → 133.76] Intro skipping is only available via plugin and the support is spotty at best.
[133.76 → 138.88] And of course, remote streaming and library sharing are definitely more challenging and
[138.88 → 140.20] more manual with Jellyfin.
[140.60 → 144.24] But there's also been a lot of upsides since we started this challenge.
[145.22 → 150.64] Swift fin came out, which is their native Apple TV client, which I was able to try.
[151.32 → 155.24] And Alex, I feel like since we started the Jellyfin challenge as well, you've kind of had a
[155.24 → 159.80] philosophy change in terms of inbound traffic to the land and kind of how you're going to
[159.80 → 161.06] do it with Jellyfin going forward.
[161.06 → 164.06] So it seems like it's kind of made you rethink a few things.
[164.66 → 169.94] Yeah, I mean, I think port 32400 was pretty much the last one that was open in my firewall
[169.94 → 170.52] for Plex.
[171.12 → 173.22] I just don't want anything open at all.
[173.60 → 179.16] And we've gone back and forth on the Discord with several people, as well as people on Twitter
[179.16 → 185.18] and stuff like that, trying to figure out a decent way to do remote access for Jellyfin.
[185.52 → 190.94] And there are lots of different ways you could skin that particular turkey if you wanted
[190.94 → 191.28] to.
[191.54 → 194.90] But none of them really did it for me.
[194.96 → 202.64] Because at the end of the day, I don't want a publicly routable DNS entry of any description,
[203.14 → 208.66] whether it's on a VPS tail scale tunnelled or WireGuard tunnelled from that VPS into my LAN,
[209.02 → 213.92] or there's some kind of outbound punch with, like I say, tail scale to somewhere else.
[213.92 → 221.86] Without that kind of third-party cloud authentication server that Plex has, there is no real way
[221.86 → 223.24] to do it with Jellyfin.
[223.78 → 228.60] The only solution I could really come up with is it's got to be baked into Jellyfin itself.
[228.60 → 237.96] There's got to be some way for me to host a Jellyfin endpoint on a VPS that speaks a Jellyfin-specific
[237.96 → 244.66] protocol or some kind of connection language back to the server in my LAN that then I can
[244.66 → 248.28] point clients from a remote LAN to on that VPS.
[248.48 → 251.18] It's not an advertised publicly routable DNS.
[251.62 → 253.04] Maybe it's some...
[253.04 → 255.66] I don't know the technicalities of how that would work.
[255.92 → 257.14] You know how you could do it, Alex?
[257.18 → 258.98] It's sort of the Nebulas model with Home Assistant.
[259.42 → 259.62] Yeah.
[260.00 → 262.66] Security through obscurity with a massively long URL.
[262.84 → 262.96] Yeah.
[263.20 → 268.14] And basically, it's an upsell that supports the development of Jellyfin, but they also
[268.14 → 271.08] take care of that proxying for you.
[271.22 → 271.98] That would be huge.
[271.98 → 273.88] And then, you know, the client...
[273.88 → 278.62] The reason it's important to bake it into the client and the server are so that you can do
[278.62 → 282.74] some kind of peer-to-peer connection once you actually start the stream.
[283.04 → 286.66] Because if you're trying to stream it all through, let's say, a Linde VPS, for example,
[287.24 → 290.10] you'd very quickly hit your one terabyte cap if you're not careful.
[290.58 → 294.86] And, you know, then it's just not necessary to stream it through a remote endpoint like
[294.86 → 295.00] that.
[295.44 → 298.22] I think it kind of depends on what your objective is.
[298.22 → 301.98] Because I think with this whole thing, too, I've been like, all right, no more inbound.
[303.10 → 307.28] But I have to be real, and I have to think, well, what am I going to do when I'm travelling
[307.28 → 307.68] again?
[308.42 → 312.46] Because a big part of travelling for me is, like, if I'm gone for several days, what I've
[312.46 → 314.86] done in the past is I've watched a show in the hotel.
[315.02 → 318.80] Like, I'll put the wife on a video call, and we'll watch a show or something like that.
[319.38 → 322.92] And I'm trying to think how I'm going to do that in my post-Jellyfin world.
[322.92 → 324.32] Well, it's fine for you, isn't it?
[324.50 → 328.00] Because you can pretty much connect all of your clients to Tail scale.
[328.38 → 328.60] Yeah.
[328.60 → 332.42] And then you can route the DNS through your reverse proxy, and it's all fine.
[332.78 → 334.60] Except for, like, hotel TVs and stuff.
[334.68 → 335.20] But yeah, you're right.
[335.28 → 336.52] For a lot of my personal devices.
[336.86 → 337.92] It's for family members.
[338.16 → 339.24] It's for hotel TVs.
[339.50 → 345.94] It's for ROK's, Chromecast's, that kind of client that Jellyfin just isn't going to work
[345.94 → 346.56] for me remotely.
[346.84 → 347.02] Right.
[347.24 → 351.74] I've been delighted with it in the LAN on my Android TVs, my pair of shields that I have
[351.74 → 352.22] in the house.
[352.38 → 354.18] Performance has been fantastic.
[354.18 → 357.00] The library just loads really quickly.
[357.38 → 359.44] Playback's been pretty much flawless.
[359.54 → 360.46] How have you found it, Catherine?
[361.08 → 361.48] Yeah.
[361.60 → 367.94] As a user, I haven't really noticed much difference in usability from Plex.
[368.48 → 372.58] I mean, it looks slightly different, but it's been pretty intuitive to just be like, oh,
[372.78 → 373.82] okay, it looks slightly different.
[373.98 → 375.86] Okay, well, cat.
[375.96 → 376.60] I'll go in cat.
[376.74 → 377.42] Oh, movies.
[377.56 → 377.70] Yeah.
[377.80 → 378.08] Okay.
[378.26 → 379.84] And it loads, and it's just done.
[380.24 → 382.34] I was like, oh, okay, I can live with this.
[382.34 → 386.86] I don't have to fiddle around with anything and I can't skip the credits though.
[386.96 → 388.80] That is a little irritating.
[389.52 → 390.16] The intro skipping.
[390.50 → 390.68] Yeah.
[391.00 → 391.76] That's what I mean.
[392.82 → 394.36] Cat, have you tried fast forwarding?
[394.46 → 398.26] Because it is perfect at going through and finding the chapters.
[398.56 → 400.46] I think you might have to turn it on in the Jellyfin dashboard.
[400.54 → 400.96] I don't recall.
[401.60 → 404.98] But if you do that, it'll mark the intro as one of the chapters.
[405.20 → 409.36] And then if you just skip that chapter, it's essentially like intro skipping.
[410.02 → 411.52] I haven't tried that, but.
[411.52 → 413.40] But if your playback tries it, yeah.
[413.48 → 413.60] Okay.
[413.64 → 415.18] I think the client has to support that too.
[415.28 → 416.40] So I'm not positive.
[416.78 → 421.12] There are a couple of things for the Android TV client that have been bugbears of mine.
[421.24 → 425.10] And they are very, very minor things compared to the client of a year ago.
[425.68 → 428.16] This 0.15 update is fantastic.
[428.98 → 432.34] So when I want to skip through, I have to press the left or right buttons,
[432.36 → 435.56] as you would expect, to jump 30 seconds forward and 10 seconds back.
[435.64 → 436.58] That works fine.
[436.58 → 442.46] But when you press the right arrow to jump forward, you then also have to press enter,
[442.62 → 445.38] like the OK button, for it to actually start playing.
[446.46 → 448.32] It's a tiny little thing, but it's annoying.
[448.84 → 453.36] The second thing is I have an OLED TV and I rely on the screensaver,
[453.88 → 456.88] the timeout on the Shield of, I think it's 10 or 12 minutes or something,
[456.94 → 458.26] to turn the screen off.
[458.26 → 461.20] And there's been a couple of times when we've paused the video
[461.20 → 464.64] and it's just stayed paused on that.
[464.80 → 466.28] It hasn't even dimmed the screen.
[466.54 → 469.04] And there was one time we left it on for like three or four hours
[469.04 → 470.36] before we came back in the room.
[470.36 → 472.00] And I'm like, oh, crap.
[472.20 → 473.90] Because, you know, it's a three-year-old TV.
[474.02 → 476.02] And so far, there's no burn-in at all.
[476.22 → 477.90] I'd like to keep it that way if I can.
[479.46 → 480.86] I have a question for you, Brantley.
[481.40 → 484.24] So I know you went ahead and did a full setup.
[484.24 → 487.76] And I know you've also been doing some watch-along with Was.
[488.34 → 490.96] And I'm just curious to know what some of your impressions were
[490.96 → 493.16] with that process, how reliable it's been,
[493.24 → 494.98] if you've had any challenges with the setup
[494.98 → 496.96] or running a local instance, et cetera.
[497.30 → 497.54] Hmm.
[498.24 → 498.98] Yeah, where to start?
[499.36 → 504.34] Well, Was and I did watch one of your favourite recent shows together.
[504.54 → 506.46] You've been trying to get us to watch that for a year.
[507.06 → 509.30] You know, we chose not to do the watch-along.
[509.68 → 512.64] And the reason for that is that we wanted to test
[512.64 → 515.44] both of our instances concurrently
[515.44 → 518.22] and be able to discuss the experience.
[518.82 → 520.58] So what we ended up doing was
[520.58 → 523.70] he shared some media with me.
[523.78 → 525.20] So we had the identical files.
[525.48 → 526.96] And then I played it locally,
[526.96 → 529.10] and he played it on his setup.
[529.24 → 530.64] I think his setup's on a VPS.
[531.28 → 533.16] So we, on purpose, didn't try
[533.16 → 536.24] the like, play syncing feature.
[536.70 → 538.34] I know we tried that, Chris.
[538.38 → 540.08] I think it was, like, almost a year ago.
[540.08 → 541.66] And it was actually perfect.
[541.66 → 543.72] So we had some good confidence
[543.72 → 545.98] that it would just be fine and continue to be fine.
[546.06 → 550.92] But it was fascinating to play the same media concurrently
[550.92 → 552.28] on two different setups.
[552.28 → 553.24] Because for me, locally,
[553.64 → 555.60] I had a few, like, initial difficulties
[555.60 → 559.40] with media naming and such
[559.40 → 560.94] with some of my own files.
[561.58 → 564.16] Luckily, Was sought that all for me with his files.
[564.64 → 565.34] But it was curious,
[565.34 → 568.38] because when we kind of did it like old school,
[568.60 → 569.86] okay, three, two, one, play.
[570.36 → 571.46] So it was not perfect.
[571.68 → 573.48] But we knew that going in, right?
[573.54 → 574.38] That wasn't the point.
[574.50 → 576.16] The point was to see what our experience
[576.16 → 577.84] was going to be concurrently.
[577.94 → 578.82] It was fascinating.
[579.12 → 583.58] So for me, it played with subtitles on by default.
[583.68 → 585.14] And I was able to just turn those off.
[585.60 → 586.98] But for Was, he was like,
[587.00 → 587.88] oh, I want subtitles.
[588.20 → 589.98] And despite having all the same files
[589.98 → 591.40] from the identical folders and everything,
[591.46 → 592.28] it wasn't working for him.
[592.46 → 593.36] And I was like, wait a second.
[593.36 → 595.88] Like, that's such a fascinating thing.
[596.00 → 598.36] And I think he ended up
[598.36 → 600.14] just kind of, like, refreshing the interface.
[600.44 → 601.94] And then it worked, you know?
[601.94 → 603.86] So those, like, little tiny things
[603.86 → 605.84] were interesting to observe
[605.84 → 608.32] in real time with someone else
[608.32 → 609.52] and their setup.
[610.12 → 611.82] I'd love for you to repeat that test
[611.82 → 615.26] with Plex and or any other system.
[615.72 → 617.32] Because I think all the quirks,
[617.40 → 620.18] you know, we are splitting hairs here.
[620.26 → 621.92] We are picking out needles in a haystack.
[621.92 → 623.48] And a lot of these quirks exist
[623.48 → 625.60] just with media playback in general.
[625.92 → 627.64] Not Jellyfin-specific stuff.
[627.98 → 628.86] That's a great point.
[629.04 → 629.20] Yeah.
[629.92 → 630.30] I agree.
[630.74 → 631.24] It worked.
[631.32 → 632.06] You did get it done.
[632.78 → 634.72] And for you, I would imagine, Brent,
[634.76 → 636.44] since you're not heavily invested in Plex,
[636.56 → 637.76] this is probably a no-brainer
[637.76 → 639.20] just to stick with Jellyfin, right?
[639.30 → 640.12] It really is.
[640.22 → 640.38] Yeah.
[641.24 → 642.68] I've used Plex lots
[642.68 → 644.18] from a streaming media
[644.18 → 645.60] from each of your servers.
[645.60 → 647.62] So that was certainly something
[647.62 → 648.58] I missed this month.
[648.78 → 650.48] I felt like I was, you know,
[650.56 → 652.38] a bit lesser this month for that reason.
[652.52 → 653.44] And I will admit,
[654.50 → 655.86] I did cheat one evening.
[656.46 → 658.74] Drew happened to leave his server on
[658.74 → 659.96] and I was out of town
[659.96 → 661.50] in a pretty crummy hotel
[661.50 → 663.02] and I needed to pick me up.
[663.66 → 664.60] And so my brother and I
[664.60 → 665.52] watch Rick and Marty.
[666.80 → 667.42] Oh, Geez.
[667.78 → 670.90] So that was one night.
[671.22 → 672.88] And I admitted it instantly.
[672.88 → 675.04] So I feel like I need to put that out there.
[675.24 → 675.66] Yeah, that's true.
[675.74 → 676.56] You did a fess up.
[677.10 → 677.90] We all knew about it.
[678.00 → 678.78] That's a fair point.
[679.42 → 680.12] I'm glad it sounds like
[680.12 → 681.60] you intend to stay with it.
[681.98 → 683.10] For me, it wasn't
[683.10 → 685.00] a foregone conclusion necessarily.
[685.74 → 687.10] One thing that I think maybe Plex
[687.10 → 689.06] does a little bit smoother
[689.06 → 690.76] is handle media
[690.76 → 692.56] that it doesn't know anything about,
[693.18 → 695.18] especially in Swift FIN.
[695.26 → 696.28] The Swift FIN client,
[696.78 → 697.34] unfortunately,
[698.18 → 700.38] keeps showcasing YouTube videos
[700.38 → 701.06] that I downloaded
[701.06 → 702.40] that it doesn't really know
[702.40 → 703.16] what to do with.
[703.26 → 704.48] And so I just have these ugly,
[704.72 → 706.62] blank, really weird-looking
[706.62 → 707.64] file-named videos
[707.64 → 708.88] that are just like the banners
[708.88 → 710.82] in Swift FIN.
[711.36 → 712.08] It's kind of gross.
[712.16 → 713.86] So I set out on a
[713.86 → 714.94] kind of journey
[714.94 → 716.06] to see if I could fix that.
[716.16 → 716.82] And I discovered
[716.82 → 718.34] that there are a couple of different ways
[718.34 → 719.14] to do this.
[719.70 → 720.38] Number one
[720.38 → 722.22] is there is a plugin
[722.22 → 723.38] for Jellyfin
[723.38 → 724.28] that will go out
[724.28 → 725.38] and get the metadata
[725.38 → 726.46] for a YouTube video.
[726.54 → 727.18] So if you leave
[727.18 → 728.28] the YouTube ID
[728.28 → 729.08] in brackets
[729.08 → 730.18] like YouTube DLP
[730.18 → 731.28] might do by default,
[731.72 → 732.30] if you leave that
[732.30 → 733.00] in the file name,
[733.44 → 735.00] then the YouTube
[735.00 → 735.90] metadata plugin
[735.90 → 736.44] that I'll have linked
[736.44 → 737.16] in the show notes
[737.16 → 738.40] will just go out
[738.40 → 739.14] and fill out
[739.14 → 740.30] all the NO information,
[740.42 → 740.76] all of that
[740.76 → 741.72] that Jellyfin can read
[741.72 → 742.94] and just make it display
[742.94 → 743.40] like it would
[743.40 → 744.72] a regular series video,
[744.78 → 746.00] which is really nice.
[746.54 → 748.02] There's some powerful stuff
[748.02 → 748.62] with YouTube
[748.62 → 749.98] and Jellyfin integration.
[750.28 → 751.04] I actually found,
[751.14 → 751.28] though,
[752.12 → 753.24] most of it was overkill.
[753.32 → 753.88] I don't really want
[753.88 → 754.86] to subscribe to a channel
[754.86 → 755.82] and import it all the time
[755.82 → 756.54] and that sort of stuff.
[756.94 → 757.82] I want to get one-off
[757.82 → 759.04] how-to videos
[759.04 → 760.02] and I want to put them
[760.02 → 760.30] in there
[760.30 → 761.24] and not lose them
[761.24 → 761.86] in case the author
[761.86 → 762.88] ever wants to take them down
[762.88 → 763.64] or they get pulled
[763.64 → 764.10] or whatever.
[764.82 → 765.86] So I found
[765.86 → 768.46] YTD-sub
[768.46 → 770.50] and that'll automate
[770.50 → 771.42] the downloading process
[771.42 → 772.40] if you want to go
[772.40 → 773.78] just all in
[773.78 → 775.76] and just get crazy with it
[775.76 → 777.78] and that'll really take
[777.78 → 778.46] Jellyfin and YouTube
[778.46 → 779.64] to a full-level integration
[779.64 → 781.12] where your YouTube videos
[781.12 → 782.24] from channels and playlists
[782.24 → 783.36] get downloaded to your server
[783.36 → 784.62] with all their metadata information.
[784.78 → 785.62] You can play them offline
[785.62 → 786.12] in Jellyfin
[786.12 → 786.74] and it's beautiful.
[787.50 → 788.42] But if that's not for you
[788.42 → 788.96] and you just want
[788.96 → 789.84] the occasional video
[789.84 → 790.64] like I do,
[791.66 → 792.46] YouTube DLP,
[792.64 → 793.46] YT DLP
[793.46 → 795.36] will write
[795.36 → 797.72] all the JSON info
[797.72 → 798.92] that Jellyfin can read.
[799.02 → 800.10] There's just a real simple
[800.10 → 801.06] dash write
[801.06 → 802.32] dash info dash JSON
[802.32 → 803.76] that you can tack on
[803.76 → 805.08] to the YT DLP command
[805.08 → 806.46] and you can do
[806.46 → 807.94] dash write dash thumbnail
[807.94 → 809.76] and Jellyfin
[809.76 → 810.94] will just pick all of that up
[810.94 → 812.20] and import it automatically.
[812.58 → 813.90] So you get the thumbnails
[813.90 → 815.84] of person holding item.
[816.16 → 816.54] I don't know.
[816.74 → 817.54] Pill bottle.
[817.94 → 818.10] Yeah.
[818.32 → 819.48] With a silly face.
[819.76 → 819.94] Yeah.
[821.86 → 822.76] Oh gosh.
[824.04 → 824.44] Yes.
[824.66 → 825.48] Actually, yes.
[825.48 → 826.40] It's a lot of that, Alex.
[826.52 → 827.74] But the nice part is
[827.74 → 828.22] you also get
[828.22 → 829.76] you get like the description.
[830.34 → 831.28] You get like,
[831.36 → 831.60] you know,
[831.62 → 832.44] the other information
[832.44 → 833.36] about the video.
[833.44 → 834.00] But yeah, you're right.
[834.02 → 835.10] It is also the obnoxious
[835.10 → 835.86] thumbnail generally.
[836.86 → 837.84] Jellyfin really started
[837.84 → 839.42] making a bigger impression
[839.42 → 841.36] when I spent a bit more time
[841.36 → 842.92] actually going into the plugins.
[843.14 → 843.82] I put on Twitter
[843.82 → 845.58] and Mastodon one day
[845.58 → 847.44] that I spent an afternoon
[847.44 → 848.58] spelunking into
[848.58 → 850.38] the plugin ecosystem.
[850.74 → 851.46] And there's an awful lot
[851.46 → 852.30] of stuff you can do
[852.30 → 853.56] in regard to metadata
[853.56 → 855.52] and tweaking that
[855.52 → 856.68] on a per library,
[856.98 → 857.24] you know,
[857.28 → 858.66] specific settings
[858.66 → 859.70] per library basis.
[860.26 → 861.48] And that really improved
[861.48 → 862.48] the experience for me
[862.48 → 865.12] for things like album art,
[865.40 → 866.48] particularly for music,
[866.48 → 867.94] was a big improvement
[867.94 → 868.54] after that.
[869.12 → 870.12] There were several covers
[870.12 → 871.56] missing in my
[871.56 → 873.66] standard folder structure.
[873.80 → 875.44] I use Sonar and Radar
[875.44 → 876.50] to organize all of my
[876.50 → 877.74] TV shows and movies,
[877.88 → 878.80] not just, you know,
[878.86 → 879.86] downloads and stuff like that,
[879.92 → 880.62] but stuff I ripped
[880.62 → 881.72] years ago.
[881.84 → 882.96] And it's fantastic at that
[882.96 → 883.90] because you can put things
[883.90 → 885.02] like custom naming
[885.02 → 885.98] conventions in there
[885.98 → 886.64] so you can have,
[886.72 → 886.82] you know,
[886.88 → 888.06] quality, bit rate,
[888.62 → 889.86] audio, codex,
[889.96 → 890.56] et cetera, et cetera,
[890.56 → 891.78] right there in the file name.
[891.96 → 892.62] That's great.
[893.04 → 893.32] Yeah.
[893.70 → 895.18] And so, you know,
[895.18 → 896.86] you can use those programs
[896.86 → 898.36] for nefarious purposes,
[898.36 → 899.18] but they're also
[899.18 → 900.32] incredibly useful
[900.32 → 902.14] for just basic
[902.14 → 903.22] media organization.
[903.48 → 903.92] There are plenty
[903.92 → 904.62] of others as well.
[904.72 → 905.70] Yet another media manager
[905.70 → 906.38] is a good one.
[907.30 → 908.82] File bot is a good one too
[908.82 → 909.58] if all you need to do
[909.58 → 910.58] is take a bunch of files
[910.58 → 912.14] and apply some rules
[912.14 → 912.84] like, you know,
[912.90 → 915.00] one file per folder
[915.00 → 916.12] based on the file name
[916.12 → 916.84] type stuff.
[917.14 → 917.88] File bot's perfect
[917.88 → 918.32] for that.
[918.64 → 920.32] But metadata seems
[920.32 → 921.14] to trip a lot of people
[921.14 → 921.84] up on the internet.
[922.14 → 922.98] It's curious to hear
[922.98 → 924.18] both of you as well
[924.18 → 925.66] have little quirks,
[925.66 → 926.24] but, you know,
[926.38 → 927.44] I've run all my stuff
[927.44 → 928.84] through the R's for years
[928.84 → 930.34] and never had a problem.
[930.98 → 931.36] Yeah, actually,
[931.48 → 932.02] to that end,
[932.10 → 933.10] just as a quick aside,
[933.58 → 934.34] I don't think Jellyfin
[934.34 → 935.02] has misidentified
[935.02 → 936.28] a single television show
[936.28 → 936.82] or movie.
[937.02 → 938.44] So that has been exceptional.
[938.56 → 938.94] It's just like
[938.94 → 940.32] the random YouTube videos
[940.32 → 941.08] because there's no,
[941.16 → 941.96] like, movie DB
[941.96 → 944.00] or TVDB can go query.
[944.10 → 945.04] So it struggles with that.
[945.10 → 945.98] Yeah, it's true.
[946.12 → 947.14] I have a question
[947.14 → 948.04] about metadata for Brent
[948.04 → 948.76] and then I want to hear
[948.76 → 949.72] about audiobooks.
[949.72 → 950.08] I think we're going
[950.08 → 950.76] to talk about that.
[950.88 → 951.22] But Brent,
[951.32 → 952.26] I know you also
[952.26 → 953.14] had a note on metadata.
[953.66 → 954.56] Yeah, it was the thing
[954.56 → 955.28] I struggled with
[955.28 → 955.98] when this month
[955.98 → 957.08] challenge started
[957.08 → 957.74] because I thought,
[957.80 → 958.84] oh, I'm going to go
[958.84 → 960.44] and, you know,
[960.52 → 961.32] it actually started
[961.32 → 962.08] with a YouTube channel
[962.08 → 963.16] of a British show.
[963.92 → 965.38] You two might appreciate this.
[965.44 → 966.64] I discovered a show
[966.64 → 967.02] that I,
[967.68 → 968.28] turns out I love
[968.28 → 969.14] called Taskmaster
[969.14 → 970.10] and they host
[970.10 → 971.16] all of it on YouTube.
[971.16 → 972.30] But my internet connection
[972.30 → 973.02] here has been,
[973.88 → 974.56] let's just say,
[974.64 → 975.60] changing this month.
[975.70 → 976.82] So I thought,
[976.82 → 977.82] well, I'm going
[977.82 → 979.04] to grab them all
[979.04 → 980.50] so that I can try them
[980.50 → 981.54] on this Jellyfin instance.
[981.54 → 983.44] and they are part
[983.44 → 984.28] of the
[984.28 → 984.72] you know,
[984.88 → 986.24] TBDBs and such.
[987.08 → 988.16] But I really struggled
[988.16 → 989.66] with trying to get
[989.66 → 990.50] all of that organized
[990.50 → 991.44] in a really nice way.
[991.70 → 994.14] I took a bunch of advice
[994.14 → 994.74] from online
[994.74 → 995.66] and found File bot,
[995.90 → 996.68] but it turns out
[996.68 → 998.08] that their,
[998.08 → 998.46] like,
[998.56 → 999.42] licensing has changed
[999.42 → 999.86] recently
[999.86 → 1000.48] and I didn't quite
[1000.48 → 1002.00] feel comfortable with...
[1002.00 → 1002.58] Oh, has it?
[1002.68 → 1003.46] What's changed?
[1003.54 → 1004.56] Because it used to just be,
[1004.64 → 1004.98] I don't know,
[1005.18 → 1006.06] five, ten bucks
[1006.06 → 1007.18] for an annual license.
[1007.50 → 1008.50] I guess maybe
[1008.50 → 1009.78] I just wasn't willing
[1009.78 → 1010.48] to pay for something
[1010.48 → 1011.12] that I didn't know
[1011.12 → 1011.56] anything about
[1011.56 → 1012.20] and I didn't ask
[1012.20 → 1012.70] either of you
[1012.70 → 1013.52] whether it was good or not.
[1013.58 → 1014.16] So this was like
[1014.16 → 1015.66] my first initial jump in.
[1015.92 → 1016.74] So I feel like
[1016.74 → 1017.26] the ten dollars
[1017.26 → 1018.18] would be probably worth it
[1018.18 → 1019.22] from the reputation I heard,
[1019.30 → 1020.48] but I just didn't
[1020.48 → 1021.36] give that a go.
[1021.56 → 1022.38] Maybe that was a mistake.
[1023.12 → 1023.68] So because of that,
[1023.72 → 1024.68] I look for other solutions
[1024.68 → 1028.48] and I spent far too much time
[1028.48 → 1029.38] trying to find something
[1029.38 → 1030.86] and struggled with a few of them
[1030.86 → 1032.22] and really didn't get
[1032.22 → 1032.88] anywhere useful.
[1033.30 → 1034.48] So I now have
[1034.48 → 1036.80] a bunch of Taskmaster episodes
[1036.80 → 1039.06] with German titles and such
[1039.06 → 1039.96] and it was just a bit
[1039.96 → 1040.86] of a failed experiment.
[1041.72 → 1042.10] But Chris,
[1042.18 → 1042.94] this plug-in sounds
[1042.94 → 1043.92] just right up my alley.
[1044.66 → 1045.62] EIN Taskmaster!
[1046.76 → 1048.04] You just say any word
[1048.04 → 1049.04] aggressively and that,
[1049.18 → 1049.46] you know,
[1049.64 → 1050.54] that's the German.
[1051.02 → 1051.88] Apart from butterfly,
[1052.04 → 1052.60] do you know what the German
[1052.60 → 1053.48] for butterfly is?
[1053.60 → 1053.92] No.
[1054.20 → 1055.12] Please, tell us.
[1055.36 → 1055.80] Skittering.
[1056.34 → 1057.72] It's such a beautiful word,
[1057.80 → 1058.26] skittering.
[1058.80 → 1060.60] Says a German descendant.
[1060.74 → 1061.82] I don't speak German though.
[1061.88 → 1062.50] Perhaps I should.
[1062.50 → 1065.02] tailscale.com
[1065.02 → 1066.40] slash self-hosted.
[1066.46 → 1067.44] Go there to get it for free
[1067.44 → 1068.40] for up to 20 devices.
[1068.70 → 1069.46] Not a trial,
[1069.90 → 1071.08] not a limited time thing
[1071.08 → 1072.16] for up to 20 devices
[1072.16 → 1073.28] at tailscale.com
[1073.28 → 1074.66] slash self-hosted.
[1075.16 → 1076.60] Tail scale is a straightforward
[1076.60 → 1077.44] mesh VPN
[1077.44 → 1078.84] protected by WireGuard.
[1078.98 → 1079.76] You're going to get it
[1079.76 → 1080.50] on your devices
[1080.50 → 1082.20] in just minutes
[1082.20 → 1083.50] and then they all connect
[1083.50 → 1084.86] directly to each other
[1084.86 → 1086.28] and it's a beautiful,
[1086.48 → 1087.22] secure thing.
[1087.50 → 1088.46] I love that it's all built
[1088.46 → 1089.42] on top of WireGuard.
[1089.58 → 1090.76] You know that noise protocol
[1090.76 → 1092.80] encryption is absolutely top-notch
[1092.80 → 1094.42] and even if your devices
[1094.42 → 1096.00] are separated by firewalls
[1096.00 → 1097.54] and complicated carrier nets
[1097.54 → 1098.18] and subnets,
[1098.84 → 1099.84] tail scale can navigate
[1099.84 → 1100.60] all of that
[1100.60 → 1102.18] and tail scale is clever enough
[1102.18 → 1103.06] to know what traffic
[1103.06 → 1104.40] to send to your tail scale nodes
[1104.40 → 1105.38] versus what you just want
[1105.38 → 1106.00] to go out to like
[1106.00 → 1106.98] the general internet
[1106.98 → 1107.96] or some other subnet
[1107.96 → 1109.34] and of course it also
[1109.34 → 1110.04] is clever enough
[1110.04 → 1110.98] to just talk directly
[1110.98 → 1111.64] to the machine
[1111.64 → 1113.04] so if it's on your LAN
[1113.04 → 1114.52] and you use the tail scale IP
[1114.52 → 1116.04] it still goes over your LAN
[1116.04 → 1116.86] it doesn't like route out
[1116.86 → 1117.66] to the internet first
[1117.66 → 1118.14] or something.
[1118.30 → 1119.28] It's clever like that
[1119.28 → 1120.52] and it always feels like
[1120.52 → 1121.22] everything's local
[1121.22 → 1122.44] regardless of where you're at
[1122.44 → 1123.46] so I have a DNS
[1123.46 → 1124.42] server using Spyhole
[1124.42 → 1125.22] in my tail net
[1125.22 → 1126.66] and now all my devices
[1126.66 → 1128.24] can just use name resolution.
[1128.54 → 1129.04] It just doesn't matter
[1129.04 → 1129.62] where I'm at.
[1129.88 → 1130.56] Anywhere I'm at
[1130.56 → 1131.94] I can use tail scale
[1131.94 → 1133.56] and I can use DNS resolution
[1133.56 → 1134.66] and it's glorious.
[1134.78 → 1135.12] You guys know
[1135.12 → 1135.58] it's the only way
[1135.58 → 1136.56] I do my next cloud now.
[1137.04 → 1138.22] I don't even have a public IP
[1138.22 → 1139.48] for any of that stuff.
[1140.04 → 1141.60] It's so, so great.
[1141.98 → 1142.88] I could go on and on about it.
[1142.92 → 1143.92] You know Alex and I love it.
[1143.98 → 1144.52] We use it.
[1144.60 → 1145.46] Our family uses it.
[1145.48 → 1146.32] Our friends use it.
[1146.54 → 1147.70] We are big advocates
[1147.70 → 1149.94] and I love that we're working with us
[1149.94 → 1151.32] and that you can go try it out
[1151.32 → 1153.36] on up to 20 devices for free
[1153.36 → 1154.74] for as long as you want
[1154.74 → 1156.14] because the way they've built this
[1156.14 → 1158.34] the traffic goes between your machines
[1158.34 → 1159.10] so they're not paying
[1159.10 → 1160.52] for a bunch of bandwidth, right?
[1160.82 → 1161.68] And then they layer on
[1161.68 → 1162.38] a bunch of services
[1162.38 → 1163.52] that make it so useful
[1163.52 → 1164.54] like tail scale send
[1164.54 → 1165.50] essentially airdrop
[1165.50 → 1167.18] for all your tail scale devices
[1167.18 → 1168.76] even your Android Linux boxes.
[1169.22 → 1169.98] Tail scale SSH
[1169.98 → 1171.40] allows you to get an SSH connection
[1171.40 → 1172.28] between your devices
[1172.28 → 1174.50] using the tail scale network.
[1174.50 → 1176.28] They're continually adding features too
[1176.28 → 1177.68] so go check out their social feeds
[1177.68 → 1178.76] to get an idea
[1178.76 → 1180.20] of just how quick they're moving here.
[1180.62 → 1181.60] And of course they have ACL
[1181.60 → 1182.86] so you can share out machines
[1182.86 → 1184.20] and do controls right there
[1184.20 → 1185.10] through a web UI.
[1185.40 → 1186.08] Like I mentioned
[1186.08 → 1187.00] it'll support DNS
[1187.00 → 1188.20] lots of ways to solve that
[1188.20 → 1190.30] but I just tossed a pie hole in mine
[1190.30 → 1191.54] and they have other
[1191.54 → 1193.44] even more innovative solutions now too.
[1194.24 → 1195.28] It's always getting better.
[1195.66 → 1196.42] It's a game changer
[1196.42 → 1197.68] and I'm so happy
[1197.68 → 1199.16] that we can send you there
[1199.16 → 1200.24] and you can support the show
[1200.24 → 1201.22] by signing up for tail scale.
[1201.22 → 1204.38] That is a win-win.
[1205.06 → 1205.76] So just go to
[1205.76 → 1206.66] tailscale.com
[1206.66 → 1207.94] slash self-hosted
[1207.94 → 1208.50] one more time.
[1208.88 → 1209.46] Support the show
[1209.46 → 1210.20] by going to
[1210.20 → 1211.40] tailscale.com
[1211.40 → 1213.06] slash self-hosted.
[1214.74 → 1215.60] I've been threatening
[1215.60 → 1217.06] to do a tail scale deep dive
[1217.06 → 1217.82] for a little while
[1217.82 → 1218.56] on how I'm doing
[1218.56 → 1219.26] the split DNS
[1219.26 → 1220.50] between different sites
[1220.50 → 1221.18] and stuff like that.
[1221.26 → 1221.92] One of these days
[1221.92 → 1223.42] I promise we will get to it
[1223.42 → 1225.66] but my good lady wife
[1225.66 → 1226.12] Catherine
[1226.12 → 1226.92] has joined us
[1226.92 → 1228.06] for this episode
[1228.06 → 1228.94] and we wanted to talk
[1228.94 → 1229.54] a little bit about
[1229.54 → 1230.24] your experience
[1230.24 → 1231.70] with Plex
[1231.70 → 1232.54] and Jellyfin
[1232.54 → 1233.66] and audiobooks
[1233.66 → 1234.34] specifically
[1234.34 → 1235.30] in this segment
[1235.30 → 1237.06] because you're a bit
[1237.06 → 1238.36] of an audiobook nerd
[1238.36 → 1238.80] right?
[1239.22 → 1239.42] Yeah
[1239.42 → 1241.30] I think audiobooks
[1241.30 → 1242.68] is my thing
[1242.68 → 1243.70] I probably listen
[1243.70 → 1245.76] to double the amount
[1245.76 → 1246.36] of audiobooks
[1246.36 → 1247.38] that I watch TV
[1247.38 → 1248.06] or use
[1248.06 → 1248.96] Jellyfin or Plex
[1248.96 → 1249.74] or whatever so
[1249.74 → 1250.50] I mean
[1250.50 → 1251.58] I can catch you
[1251.58 → 1252.88] any time of the day
[1252.88 → 1253.22] or night
[1253.22 → 1253.84] with your phone
[1253.84 → 1254.90] with your AirPods in
[1254.90 → 1255.76] or just walking
[1255.76 → 1256.38] around the house
[1256.38 → 1257.12] and there's always
[1257.12 → 1258.02] an audiobook
[1258.02 → 1258.56] some people
[1258.56 → 1259.20] it's podcasts
[1259.20 → 1259.74] for you
[1259.74 → 1261.00] it's audiobooks
[1261.00 → 1261.60] or you know
[1261.60 → 1262.10] some people
[1262.10 → 1262.58] it's radio
[1262.58 → 1264.02] and so me
[1264.02 → 1264.96] turning off Plex
[1264.96 → 1266.60] and separating you
[1266.60 → 1267.58] from your beloved
[1267.58 → 1268.74] prologue instance
[1268.74 → 1269.64] a month ago
[1269.64 → 1270.40] was
[1270.40 → 1271.88] how was it?
[1272.24 → 1272.58] Tricky
[1272.58 → 1273.34] Tricky
[1273.34 → 1276.66] so I had some backups
[1276.66 → 1277.46] in case
[1277.46 → 1279.14] I really didn't like
[1279.14 → 1280.94] my new situation
[1280.94 → 1282.98] I had Libby
[1282.98 → 1283.66] which is
[1283.66 → 1284.42] like a
[1284.42 → 1284.84] you know
[1284.84 → 1285.46] library
[1285.46 → 1286.50] county
[1286.50 → 1287.54] based thing
[1287.54 → 1288.26] yeah in America
[1288.26 → 1288.94] you can sign up
[1288.94 → 1289.68] for a library card
[1289.68 → 1290.24] and they give you
[1290.24 → 1291.10] access to
[1291.10 → 1293.30] free digital audiobooks
[1293.30 → 1293.98] but you can sort of
[1293.98 → 1294.62] rent them from a
[1294.62 → 1295.38] digital library
[1295.38 → 1296.38] it's like a
[1296.38 → 1296.92] it's like
[1296.92 → 1297.84] Audible
[1297.84 → 1299.28] but like a library
[1299.28 → 1300.64] yeah it's a bit
[1300.64 → 1301.18] like a library
[1301.18 → 1301.96] a bit like Audible
[1301.96 → 1302.48] you can
[1302.48 → 1303.30] there's an app
[1303.30 → 1303.84] you can use it
[1303.84 → 1304.44] on your phone
[1304.44 → 1306.06] but you only get
[1306.06 → 1307.16] 14 days to listen
[1307.16 → 1307.76] to a title
[1307.76 → 1308.34] and you often
[1308.34 → 1309.04] have to wait
[1309.04 → 1309.98] and you've run out
[1309.98 → 1310.64] a couple of times
[1310.64 → 1310.92] I have
[1310.92 → 1311.40] yeah
[1311.40 → 1312.16] because sometimes
[1312.16 → 1313.14] you have to wait
[1313.14 → 1313.90] a very long time
[1313.90 → 1314.80] to be given access
[1314.80 → 1315.66] because they only have
[1315.66 → 1316.50] a certain amount of
[1316.50 → 1317.62] they have to pay
[1317.62 → 1319.56] on a per rental
[1319.56 → 1320.56] basis effectively
[1320.56 → 1321.54] to the publishers
[1321.54 → 1322.74] and so they
[1322.74 → 1324.18] only buy a certain
[1324.18 → 1324.86] number of licenses
[1324.86 → 1325.78] for each title
[1325.78 → 1326.72] and then when
[1326.72 → 1327.50] those licenses
[1327.50 → 1328.02] are exhausted
[1328.02 → 1328.48] they have to go
[1328.48 → 1328.88] and either buy
[1328.88 → 1329.48] another batch
[1329.48 → 1329.98] or they have to
[1329.98 → 1331.10] so it's expensive
[1331.10 → 1331.80] for the library
[1331.80 → 1332.60] to do that
[1332.60 → 1333.04] so that's why
[1333.04 → 1333.72] there's a limit there
[1333.72 → 1334.06] yeah
[1334.06 → 1334.96] so sometimes
[1334.96 → 1335.32] you could be
[1335.32 → 1337.22] waiting up to
[1337.22 → 1338.46] four months
[1338.46 → 1339.54] to listen to a title
[1339.54 → 1340.22] so you kind of
[1340.22 → 1341.34] have to have them
[1341.34 → 1342.36] ready in advance
[1342.36 → 1343.24] and plan them out
[1343.24 → 1343.72] a little bit
[1343.72 → 1344.40] but I had that
[1344.40 → 1344.90] as a backup
[1344.90 → 1346.96] and I had Audible
[1346.96 → 1347.94] and I could spend
[1347.94 → 1349.08] money as a backup
[1349.08 → 1349.88] you're the sort of
[1349.88 → 1350.58] girl that has the
[1350.58 → 1351.52] two credits a month
[1351.52 → 1352.66] Audible subscription
[1352.66 → 1352.90] right
[1352.90 → 1353.26] I do
[1353.26 → 1354.52] and I use them
[1354.52 → 1355.28] yeah
[1355.28 → 1355.96] that's fine
[1355.96 → 1356.38] hey girl
[1356.38 → 1356.90] me too
[1356.90 → 1357.58] me too
[1357.58 → 1358.20] yeah
[1358.20 → 1359.18] and you're used
[1359.18 → 1359.76] to me going
[1359.76 → 1360.32] into Audible
[1360.32 → 1361.42] and backing
[1361.42 → 1362.10] these things up
[1362.10 → 1362.80] with in Audible
[1362.80 → 1363.46] which we've talked
[1363.46 → 1364.02] about in the show
[1364.02 → 1364.36] before
[1364.36 → 1366.06] and removing the DRM
[1366.06 → 1366.84] and never really
[1366.84 → 1367.32] having to worry
[1367.32 → 1367.80] about Audible
[1367.80 → 1368.26] itself
[1368.26 → 1368.72] you know
[1368.72 → 1369.32] going away
[1369.32 → 1369.78] or changing
[1369.78 → 1370.62] licensing on you
[1370.62 → 1371.28] there you go
[1371.28 → 1371.74] those books
[1371.74 → 1372.18] you own them
[1372.18 → 1372.46] forever
[1372.46 → 1373.12] you've paid
[1373.12 → 1373.44] for them
[1373.44 → 1373.82] and I think
[1373.82 → 1374.42] it's only fair
[1374.42 → 1375.48] that we own
[1375.48 → 1375.90] them forever
[1375.90 → 1377.14] so when I
[1377.14 → 1377.50] switched off
[1377.50 → 1378.44] Prologue
[1378.44 → 1380.70] I had to come
[1380.70 → 1381.04] up with an
[1381.04 → 1381.92] alternative solution
[1381.92 → 1382.32] for you
[1382.32 → 1383.00] and Jellyfin
[1383.00 → 1383.56] doesn't really
[1383.56 → 1385.04] have much
[1385.04 → 1385.36] in the way
[1385.36 → 1385.78] of audiobook
[1385.78 → 1386.36] support
[1386.36 → 1386.96] so far
[1386.96 → 1387.34] as I could
[1387.34 → 1387.76] tell
[1387.76 → 1388.72] that was
[1388.72 → 1389.20] any good
[1389.20 → 1390.14] so I
[1390.14 → 1390.68] threw you
[1390.68 → 1391.20] down the
[1391.20 → 1391.62] gauntlet
[1391.62 → 1392.80] of audiobook
[1392.80 → 1393.38] shelf
[1393.38 → 1394.28] how did you
[1394.28 → 1394.82] find that
[1394.82 → 1395.32] yeah
[1395.32 → 1396.32] it's not
[1396.32 → 1396.86] for me
[1396.86 → 1399.60] it works
[1399.60 → 1400.94] it works
[1400.94 → 1401.30] fine
[1401.30 → 1401.94] it doesn't
[1401.94 → 1402.24] lose your
[1402.24 → 1402.74] place or
[1402.74 → 1403.10] anything
[1403.10 → 1405.08] but it
[1405.08 → 1405.46] just
[1405.46 → 1406.42] it's not
[1406.42 → 1407.66] a particularly
[1407.66 → 1408.96] exciting place
[1408.96 → 1409.52] to be in
[1409.52 → 1409.88] it just
[1409.88 → 1410.64] doesn't
[1410.64 → 1411.94] like graphically
[1411.94 → 1412.98] speak to me
[1412.98 → 1413.92] you mean
[1413.92 → 1414.16] you're not
[1414.16 → 1414.48] a fan
[1414.48 → 1414.80] of that
[1414.80 → 1415.74] skeuomorphic
[1415.74 → 1416.74] fake bookshelf
[1416.74 → 1417.50] look
[1417.50 → 1417.92] no
[1417.92 → 1418.04] no
[1418.04 → 1418.88] it's very
[1418.88 → 1419.74] iOS 5
[1419.74 → 1420.20] isn't it
[1420.20 → 1420.60] yeah
[1420.60 → 1421.14] and just
[1421.14 → 1421.74] going into
[1421.74 → 1423.26] it doesn't
[1423.26 → 1423.68] fill me
[1423.68 → 1424.20] with joy
[1424.20 → 1424.78] yeah
[1424.78 → 1425.36] Marie Kondo
[1425.36 → 1425.86] that is one
[1425.86 → 1426.12] thing
[1426.12 → 1426.70] Plex and
[1426.70 → 1427.22] Prologue in
[1427.22 → 1427.88] particular does
[1427.88 → 1428.34] very well
[1428.34 → 1428.98] is it presents
[1428.98 → 1429.54] things
[1429.54 → 1430.88] beautifully
[1430.88 → 1431.66] another thing
[1431.66 → 1432.14] it doesn't
[1432.14 → 1432.62] do which
[1432.62 → 1432.94] some of the
[1432.94 → 1433.34] others have
[1433.34 → 1433.80] done is it
[1433.80 → 1434.18] doesn't give
[1434.18 → 1434.82] me any sort
[1434.82 → 1436.14] of hey
[1436.14 → 1436.56] do you want
[1436.56 → 1436.82] to listen
[1436.82 → 1437.30] to this
[1437.30 → 1437.90] kind of
[1437.90 → 1438.64] pokes
[1438.64 → 1439.54] or prods
[1439.54 → 1440.10] you know
[1440.10 → 1440.58] Jellyfin
[1440.58 → 1440.98] if you go
[1440.98 → 1441.30] on the
[1441.30 → 1441.70] home menu
[1441.70 → 1442.36] goes hey
[1442.36 → 1442.78] the next
[1442.78 → 1443.38] one in your
[1443.38 → 1444.86] series is up
[1444.86 → 1445.14] do you want
[1445.14 → 1445.56] to do it
[1445.56 → 1447.10] and yeah
[1447.10 → 1447.56] the audiobook
[1447.56 → 1448.06] you have to
[1448.06 → 1448.42] kind of have
[1448.42 → 1449.00] a plan
[1449.00 → 1450.68] and go in
[1450.68 → 1451.14] and go oh
[1451.14 → 1451.60] I want to
[1451.60 → 1452.16] listen to this
[1452.16 → 1453.42] today and
[1453.42 → 1453.96] know what the
[1453.96 → 1454.42] name of it
[1454.42 → 1454.98] is and be able
[1454.98 → 1455.62] to search for
[1455.62 → 1456.18] it and find
[1456.18 → 1456.46] it
[1456.46 → 1457.00] because I had
[1457.00 → 1457.38] you using
[1457.38 → 1457.82] book sonic
[1457.82 → 1458.34] for a long
[1458.34 → 1459.18] time and
[1459.18 → 1459.60] one of your
[1459.60 → 1460.32] favourite features
[1460.32 → 1461.16] as I recall
[1461.16 → 1461.54] was the
[1461.54 → 1462.80] random button
[1462.80 → 1464.20] yeah I love
[1464.20 → 1465.16] that because
[1465.16 → 1466.42] Alex's mum
[1466.42 → 1467.12] and Alex's
[1467.12 → 1467.94] sister and
[1467.94 → 1468.96] my mum also
[1468.96 → 1470.20] put their
[1470.20 → 1471.22] audiobooks into
[1471.22 → 1472.20] our collection
[1472.20 → 1472.58] we've got a whole
[1472.58 → 1473.34] system going
[1473.34 → 1474.02] it's pretty
[1474.02 → 1474.38] great
[1474.38 → 1475.80] so I also
[1475.80 → 1476.60] have access
[1476.60 → 1477.14] to theirs
[1477.14 → 1477.52] which are
[1477.52 → 1477.90] stored on
[1477.90 → 1478.34] my server
[1478.34 → 1479.38] on sorry
[1479.38 → 1480.34] our server
[1480.34 → 1481.36] the server
[1481.36 → 1481.92] let's go with
[1481.92 → 1482.16] that
[1482.16 → 1486.06] so I love
[1486.06 → 1486.56] just going
[1486.56 → 1487.36] on random
[1487.36 → 1488.68] and I've
[1488.68 → 1489.10] found some
[1489.10 → 1489.96] amazing books
[1489.96 → 1490.78] that I never
[1490.78 → 1491.20] would have
[1491.20 → 1492.34] picked or
[1492.34 → 1492.98] haven't come
[1492.98 → 1493.76] up and you
[1493.76 → 1494.02] know been
[1494.02 → 1494.72] promoted by
[1494.72 → 1495.78] audible or
[1495.78 → 1496.54] Amazon or
[1496.54 → 1497.18] Barnes and
[1497.18 → 1497.58] Noble or
[1497.58 → 1497.84] whatever
[1497.84 → 1498.22] let's be
[1498.22 → 1498.52] honest you
[1498.52 → 1498.96] found some
[1498.96 → 1499.52] crap too
[1499.52 → 1499.80] right
[1499.80 → 1500.40] yeah
[1500.40 → 1501.44] yeah okay
[1501.44 → 1502.70] oh and
[1502.70 → 1503.56] Aaliyah's part
[1503.56 → 1504.02] of this too
[1504.02 → 1504.62] I forgot that
[1504.62 → 1505.06] as well
[1505.06 → 1506.32] she's joined
[1506.32 → 1506.90] in the
[1506.90 → 1508.98] audiobook love
[1508.98 → 1510.08] over here
[1510.08 → 1511.26] so I have
[1511.26 → 1511.94] all of hers
[1511.94 → 1512.70] how's Aaliyah
[1512.70 → 1513.56] found not
[1513.56 → 1514.08] having access
[1514.08 → 1514.68] to prologue
[1514.68 → 1515.34] this month
[1515.34 → 1515.76] not good
[1515.76 → 1516.14] that's not
[1516.14 → 1516.62] been smooth
[1516.62 → 1516.94] Alex
[1516.94 → 1517.78] that's not
[1517.78 → 1518.40] been a smooth
[1518.40 → 1519.20] aspect of it
[1519.20 → 1520.48] I told her
[1520.48 → 1520.98] I promised
[1520.98 → 1521.80] that eventually
[1521.80 → 1522.28] I'd replace
[1522.28 → 1522.50] it with
[1522.50 → 1522.76] something
[1522.76 → 1523.48] but she has
[1523.48 → 1523.90] a couple of
[1523.90 → 1524.56] audible credits
[1524.56 → 1525.46] and a couple
[1525.46 → 1525.86] of books
[1525.86 → 1526.76] in there's
[1526.76 → 1527.30] a not Libby
[1527.30 → 1527.96] I think
[1527.96 → 1528.88] yeah
[1528.88 → 1529.18] yeah
[1529.18 → 1529.60] that's what
[1529.60 → 1529.86] we were
[1529.86 → 1530.44] talking about
[1530.44 → 1531.32] yeah okay
[1531.32 → 1531.90] I'm not sure
[1531.90 → 1532.36] if it's Libby
[1532.36 → 1532.90] or if it's
[1532.90 → 1533.28] in audible
[1533.28 → 1534.38] but she's in
[1534.38 → 1534.72] one of those
[1534.72 → 1535.22] right now
[1535.22 → 1536.24] while I have
[1536.24 → 1536.86] everything down
[1536.86 → 1538.24] it's not great
[1538.24 → 1538.90] Alex it's not
[1538.90 → 1539.50] great hasn't
[1539.50 → 1539.74] been the
[1539.74 → 1540.36] the smoothest aspect
[1540.36 → 1540.74] no
[1540.74 → 1541.82] I'll tell you
[1541.82 → 1542.38] one thing
[1542.38 → 1542.84] actually I
[1542.84 → 1543.30] used audio
[1543.30 → 1543.82] bookshelf
[1543.82 → 1544.50] as I was
[1544.50 → 1545.04] falling asleep
[1545.04 → 1545.58] with
[1545.58 → 1545.96] some books
[1545.96 → 1546.42] this month
[1546.42 → 1547.28] just to test
[1547.28 → 1547.74] it for
[1547.74 → 1548.34] for myself
[1548.34 → 1550.18] and when I
[1550.18 → 1550.68] do that I
[1550.68 → 1551.36] set a 45
[1551.36 → 1552.12] minute timer
[1552.12 → 1553.28] every time
[1553.28 → 1553.82] and so you
[1553.82 → 1554.20] know I have
[1554.20 → 1554.78] to go back
[1554.78 → 1555.88] half an hour
[1555.88 → 1556.92] I do the same
[1556.92 → 1557.58] thing yeah
[1557.58 → 1558.68] every night
[1558.68 → 1559.34] and gradually
[1559.34 → 1559.92] I make my way
[1559.92 → 1560.44] through the book
[1560.44 → 1561.48] yep I do that
[1561.48 → 1562.08] but one of the
[1562.08 → 1562.68] most frustrating
[1562.68 → 1563.22] things about
[1563.22 → 1563.96] audio bookshelf
[1563.96 → 1565.00] on iOS at least
[1565.00 → 1566.10] is that the
[1566.10 → 1567.74] Scrabble bar
[1567.74 → 1568.92] is right next
[1568.92 → 1569.72] to the little line
[1569.72 → 1570.14] at the bottom
[1570.14 → 1570.68] of the iPhone
[1570.68 → 1571.38] that you swipe
[1571.38 → 1571.96] left or right
[1571.96 → 1572.50] to go between
[1572.50 → 1573.00] apps on
[1573.00 → 1574.04] and so
[1574.04 → 1574.90] if you're trying
[1574.90 → 1575.72] to swipe back
[1575.72 → 1576.24] 10 minutes
[1576.24 → 1577.00] you can very easily
[1577.00 → 1577.78] swipe back to
[1577.78 → 1578.60] the previous app
[1578.60 → 1579.18] and so on
[1579.18 → 1580.40] you find yourself
[1580.40 → 1581.26] tapping instead
[1581.26 → 1581.92] of swiping
[1581.92 → 1582.60] and sometimes
[1582.60 → 1583.26] it doesn't register
[1583.26 → 1583.76] the tap
[1583.76 → 1584.28] because it thinks
[1584.28 → 1584.62] you're tapping
[1584.62 → 1585.06] on the little
[1585.06 → 1585.70] white bar
[1585.70 → 1586.18] at the bottom
[1586.18 → 1586.68] and not the
[1586.68 → 1587.32] seek button
[1587.32 → 1589.34] and so there
[1589.34 → 1590.48] I think probably
[1590.48 → 1591.40] audio bookshelves
[1591.40 → 1592.24] the biggest issue
[1592.24 → 1592.62] right now
[1592.62 → 1593.40] the biggest impediment
[1593.40 → 1595.20] is the interface
[1595.20 → 1596.42] generally speaking
[1596.42 → 1597.14] I feel like
[1597.14 → 1597.78] there's a place
[1597.78 → 1598.76] here just thinking
[1598.76 → 1599.52] about our nighttime
[1599.52 → 1600.56] every single night
[1600.56 → 1601.24] we listen to an
[1601.24 → 1601.70] audiobook
[1601.70 → 1602.34] we specifically
[1602.34 → 1603.34] pick audiobooks
[1603.34 → 1603.86] that are like
[1603.86 → 1604.50] perfect for
[1604.50 → 1605.44] falling asleep to
[1605.44 → 1606.72] they're interesting
[1606.72 → 1608.06] but not so interesting
[1608.06 → 1608.74] that if you miss
[1608.74 → 1609.76] five minutes of it
[1609.76 → 1610.92] it's not the end
[1610.92 → 1611.16] of the world
[1611.16 → 1611.68] because I'll back
[1611.68 → 1612.38] up as well
[1612.38 → 1613.40] but sometimes
[1613.40 → 1613.82] I don't back
[1613.82 → 1614.36] up enough
[1614.36 → 1614.86] and I miss
[1614.86 → 1615.28] a couple of
[1615.28 → 1615.46] minutes
[1615.46 → 1615.78] but like
[1615.78 → 1616.08] it's just
[1616.08 → 1616.68] it's fine
[1616.68 → 1617.02] because it's
[1617.02 → 1617.32] not like
[1617.32 → 1618.14] a critical book
[1618.14 → 1619.10] but man
[1619.10 → 1619.56] if I thought
[1619.56 → 1619.88] wouldn't it
[1619.88 → 1620.34] be great
[1620.34 → 1621.24] if I get in
[1621.24 → 1621.94] and I've got
[1621.94 → 1622.60] an NFC tag
[1622.60 → 1624.14] by my headboard
[1624.14 → 1625.10] I scan that
[1625.10 → 1625.82] NFC tag
[1625.82 → 1626.88] and it kicks
[1626.88 → 1627.60] off the whole
[1627.60 → 1628.54] last call
[1628.54 → 1628.96] routine
[1628.96 → 1629.60] which starts
[1629.60 → 1630.10] shutting down
[1630.10 → 1630.54] the lights
[1630.54 → 1631.00] turns on
[1631.00 → 1631.66] the noisemakers
[1631.66 → 1632.80] and would just
[1632.80 → 1633.70] start playing
[1633.70 → 1634.94] the audiobook
[1634.94 → 1635.82] for 45 minutes
[1635.82 → 1636.28] and then
[1636.28 → 1637.58] automatically
[1637.58 → 1638.66] kick it back
[1638.66 → 1639.42] I don't know
[1639.42 → 1640.14] 15 minutes
[1640.14 → 1640.82] or 10 minutes
[1640.82 → 1641.16] or whatever
[1641.16 → 1642.14] every single time
[1642.14 → 1642.78] feels like
[1642.78 → 1643.14] there's some
[1643.14 → 1643.54] automation
[1643.54 → 1644.56] possibility there
[1644.56 → 1645.00] there are those
[1645.00 → 1645.58] apps that can
[1645.58 → 1646.32] do sleep tracking
[1646.32 → 1647.00] just based on
[1647.00 → 1647.60] listening to you
[1647.60 → 1647.94] breathing
[1647.94 → 1648.52] right
[1648.52 → 1648.86] yeah
[1648.86 → 1649.62] yeah
[1649.62 → 1650.10] sleepers
[1650.10 → 1650.46] android
[1650.46 → 1650.74] will do
[1650.74 → 1651.12] some of this
[1651.12 → 1651.54] but I want
[1651.54 → 1651.88] something like
[1651.88 → 1652.36] around home
[1652.36 → 1652.86] assistant
[1652.86 → 1653.42] yeah
[1653.42 → 1654.38] yeah
[1654.38 → 1656.06] well I guess
[1656.06 → 1656.60] there's a solution
[1656.60 → 1656.92] in there
[1656.92 → 1657.18] somewhere
[1657.18 → 1657.72] but I think
[1657.72 → 1658.20] that touches
[1658.20 → 1658.60] on another
[1658.60 → 1658.92] point
[1658.92 → 1659.44] specifically
[1659.44 → 1659.80] about
[1659.80 → 1660.34] Jellyfin
[1660.34 → 1661.02] that
[1661.02 → 1661.70] Catherine
[1661.70 → 1662.26] you and I
[1662.26 → 1662.54] were talking
[1662.54 → 1662.86] about in the
[1662.86 → 1663.20] car on the
[1663.20 → 1663.44] way home
[1663.44 → 1664.04] from daycare
[1664.04 → 1664.34] earlier
[1664.34 → 1665.86] just the general
[1665.86 → 1666.68] fit and finish
[1666.68 → 1667.34] of Jellyfin
[1667.34 → 1668.08] you talk about
[1668.08 → 1668.44] that a little
[1668.44 → 1668.64] bit
[1668.64 → 1669.04] yeah
[1669.04 → 1669.54] it just
[1669.54 → 1670.28] doesn't
[1670.28 → 1670.90] have
[1670.90 → 1672.18] it's like
[1672.18 → 1673.24] the edges
[1673.24 → 1673.72] have not
[1673.72 → 1673.98] just
[1673.98 → 1674.66] someone hasn't
[1674.66 → 1675.06] gone around
[1675.06 → 1675.50] with every
[1675.50 → 1676.18] single pixel
[1676.18 → 1676.54] and gone
[1676.54 → 1677.36] oh this is
[1677.36 → 1677.74] perfect
[1677.74 → 1678.08] you know
[1678.08 → 1678.42] how when
[1678.42 → 1678.78] you go on
[1678.78 → 1679.44] google or
[1679.44 → 1680.26] Amazon or
[1680.26 → 1680.54] something
[1680.54 → 1681.26] it's just
[1681.26 → 1682.40] just so
[1682.40 → 1683.36] correct
[1683.36 → 1684.48] unless you end
[1684.48 → 1684.80] up on the
[1684.80 → 1685.50] Amazon page
[1685.50 → 1686.06] from the
[1686.06 → 1686.62] early days
[1686.62 → 1686.88] when you're
[1686.88 → 1687.06] trying to
[1687.06 → 1687.28] get a
[1687.28 → 1687.60] refund
[1687.60 → 1688.04] and it's
[1688.04 → 1688.58] still got
[1688.58 → 1689.66] that original
[1689.66 → 1690.18] branding
[1690.18 → 1692.98] but it's
[1692.98 → 1693.92] it's like
[1693.92 → 1695.06] when I try
[1695.06 → 1695.62] and make
[1695.62 → 1696.02] things look
[1696.02 → 1696.44] pretty on
[1696.44 → 1696.82] the internet
[1696.82 → 1698.52] and no matter
[1698.52 → 1699.18] what I do
[1699.18 → 1699.90] and whatever
[1699.90 → 1700.58] I type in
[1700.58 → 1700.94] CSS
[1700.94 → 1702.22] it is looks
[1702.22 → 1702.74] okay
[1702.74 → 1704.44] but it just
[1704.44 → 1705.44] isn't
[1705.44 → 1705.86] absolutely
[1705.86 → 1706.28] perfect
[1706.28 → 1707.40] and as a
[1707.40 → 1708.42] user I just
[1708.42 → 1709.58] think oh
[1709.58 → 1711.08] oh it's just
[1711.08 → 1711.90] not a
[1711.90 → 1713.16] really happy
[1713.16 → 1714.10] exciting place
[1714.10 → 1714.48] for me to
[1714.48 → 1714.94] want to go
[1714.94 → 1715.26] to it
[1715.26 → 1715.60] doesn't make
[1715.60 → 1716.54] me go oh
[1716.54 → 1717.46] I want to
[1717.46 → 1717.94] watch this
[1717.94 → 1718.46] or listen to
[1718.46 → 1718.88] that I just
[1718.88 → 1719.40] go yeah
[1719.40 → 1719.80] okay it
[1719.80 → 1720.12] works
[1720.12 → 1720.72] that said
[1720.72 → 1721.10] though there
[1721.10 → 1721.52] are some
[1721.52 → 1721.92] particularly
[1721.92 → 1722.62] nice ways
[1722.62 → 1723.16] in which it
[1723.16 → 1724.22] surfaces things
[1724.22 → 1724.86] like movies
[1724.86 → 1725.46] like it has a
[1725.46 → 1725.94] really nice
[1725.94 → 1726.88] canvas for how
[1726.88 → 1727.54] it displays all
[1727.54 → 1728.10] the posters
[1728.10 → 1729.16] reminds me a lot
[1729.16 → 1729.72] of what Cody
[1729.72 → 1730.76] used to do
[1730.76 → 1731.74] in the XBMC
[1731.74 → 1732.84] era it was
[1732.84 → 1733.64] just a complete
[1733.64 → 1734.40] canvas maybe
[1734.40 → 1735.02] even media
[1735.02 → 1735.78] browser if I
[1735.78 → 1736.14] remember the
[1736.14 → 1736.60] name right
[1736.60 → 1737.96] from years ago
[1737.96 → 1738.20] it was a
[1738.20 → 1738.80] beautiful skin
[1738.80 → 1739.34] for media
[1739.34 → 1740.00] browser that did
[1740.00 → 1740.62] that as well
[1740.62 → 1741.76] and I like
[1741.76 → 1742.74] actually seeing
[1742.74 → 1743.42] a lot of
[1743.42 → 1744.10] content at
[1744.10 → 1744.68] once I'm
[1744.68 → 1745.28] quite good at
[1745.28 → 1746.04] taking in
[1746.04 → 1746.38] you know
[1746.38 → 1748.40] three four
[1748.40 → 1749.04] different rows
[1749.04 → 1749.80] with you know
[1749.80 → 1750.78] wide worth of
[1750.78 → 1752.06] content all at
[1752.06 → 1752.70] once from movie
[1752.70 → 1754.08] posters and
[1754.08 → 1754.62] Plex doesn't do
[1754.62 → 1755.08] that very well
[1755.08 → 1756.02] at all, and I'll
[1756.02 → 1756.34] tell you the other
[1756.34 → 1756.80] thing that I've
[1756.80 → 1757.90] really enjoyed is
[1757.90 → 1759.72] I loaded up Plex a
[1759.72 → 1760.18] couple of nights
[1760.18 → 1761.14] ago just to
[1761.14 → 1762.84] remind myself
[1762.84 → 1763.72] before we did
[1763.72 → 1764.94] this episode it
[1764.94 → 1765.90] was fully 15
[1765.90 → 1766.78] seconds after
[1766.78 → 1767.50] hitting go
[1767.50 → 1768.72] before Plex
[1768.72 → 1769.38] had loaded me
[1769.38 → 1770.22] at my homepage
[1770.22 → 1770.86] on the
[1770.86 → 1771.64] Android TV
[1771.64 → 1772.80] client you
[1772.80 → 1773.12] know there's
[1773.12 → 1773.96] now a new
[1773.96 → 1774.56] Plex logo
[1774.56 → 1774.92] where it
[1774.92 → 1776.02] swipes in
[1776.02 → 1776.48] from the
[1776.48 → 1777.14] side with
[1777.14 → 1777.50] the yellow
[1777.50 → 1778.64] arrow and
[1778.64 → 1778.90] then it
[1778.90 → 1779.48] fades and
[1779.48 → 1779.72] then it
[1779.72 → 1780.34] pauses and
[1780.34 → 1780.86] thinks about
[1780.86 → 1781.38] life a little
[1781.38 → 1781.78] bit and then
[1781.78 → 1782.38] goes am I a
[1782.38 → 1783.00] media player
[1783.00 → 1783.76] am I a
[1783.76 → 1784.42] chainsaw
[1784.42 → 1785.46] what am I
[1785.46 → 1786.02] doing here
[1786.02 → 1786.36] and then
[1786.36 → 1787.06] eventually it
[1787.06 → 1788.70] loads what I
[1788.70 → 1789.16] asked it to
[1789.16 → 1790.40] load and
[1790.40 → 1790.86] then once I'm
[1790.86 → 1791.26] in the app
[1791.26 → 1791.96] too browsing
[1791.96 → 1792.60] libraries and
[1792.60 → 1792.94] stuff like
[1792.94 → 1794.14] that Jellyfin is
[1794.14 → 1795.30] night and day
[1795.30 → 1795.96] faster at
[1795.96 → 1796.80] browsing libraries
[1796.80 → 1797.48] and media and
[1797.48 → 1798.08] stuff like that
[1798.08 → 1799.66] 100% local I
[1799.66 → 1800.30] think has to be
[1800.30 → 1800.82] the reason for
[1800.82 → 1801.18] that although
[1801.18 → 1801.88] there could be
[1801.88 → 1802.74] some server side
[1802.74 → 1804.14] code improvements
[1804.14 → 1806.24] versus Plex who
[1806.24 → 1807.40] knows yeah but
[1807.40 → 1808.16] generally speaking
[1808.16 → 1808.76] it's that
[1808.76 → 1809.52] performance it's
[1809.52 → 1810.20] that snappiness
[1810.20 → 1810.92] that has got me
[1810.92 → 1811.90] really excited
[1811.90 → 1813.14] about Jellyfin I
[1813.14 → 1813.46] love the
[1813.46 → 1814.32] performance myself
[1814.32 → 1815.02] it is really
[1815.02 → 1816.36] nice now it's
[1816.36 → 1817.34] important question
[1817.34 → 1818.78] time I'm not
[1818.78 → 1819.06] going to ask
[1819.06 → 1819.68] Catherine because
[1819.68 → 1820.12] she doesn't have
[1820.12 → 1822.40] a choice we're
[1822.40 → 1822.92] going to have Plex
[1822.92 → 1823.76] and Jellyfin here
[1823.76 → 1825.28] simply because we
[1825.28 → 1825.62] have to leave
[1825.62 → 1826.34] Plex on for your
[1826.34 → 1826.78] audiobooks
[1826.80 → 1827.60] and then Jellyfin
[1827.60 → 1828.36] for the TVs
[1828.36 → 1829.74] what about you
[1829.74 → 1830.20] Brent are you
[1830.20 → 1830.84] gonna stick with
[1830.84 → 1832.12] Jellyfin well if
[1832.12 → 1833.32] you're asking me am
[1833.32 → 1834.06] I gonna stick with
[1834.06 → 1835.16] Jellyfin for
[1835.16 → 1836.22] remote accessing
[1836.22 → 1838.42] your media which
[1838.42 → 1839.42] you don't have a
[1839.42 → 1840.14] solution for then I
[1840.14 → 1840.60] think the answer is
[1840.60 → 1843.20] no but if we're
[1843.20 → 1844.28] talking about here
[1844.28 → 1844.82] at home on my
[1844.82 → 1845.78] local network I
[1845.78 → 1846.38] think I touched on
[1846.38 → 1847.02] a little earlier
[1847.02 → 1848.34] yeah absolutely
[1848.34 → 1849.38] there's a function
[1849.38 → 1850.72] that I've been
[1850.72 → 1852.44] loving which is
[1852.44 → 1854.52] you know I live in
[1854.52 → 1855.66] a tiny cabin, so I
[1855.66 → 1856.04] set up some
[1856.04 → 1856.90] speakers for this
[1856.90 → 1858.14] challenge connected
[1858.14 → 1858.78] to my little
[1858.78 → 1859.88] laptop server that
[1859.88 → 1860.60] Jellyfin's sitting
[1860.60 → 1862.62] on, and I can walk
[1862.62 → 1863.16] anywhere in my
[1863.16 → 1864.24] place and use my
[1864.24 → 1865.08] phone to stream
[1865.08 → 1866.30] media on that
[1866.30 → 1867.70] computer over there
[1867.70 → 1868.72] through those
[1868.72 → 1870.08] speakers so that's
[1870.08 → 1870.76] been a beautiful
[1870.76 → 1871.76] function that I've
[1871.76 → 1872.66] really enjoyed here
[1872.66 → 1875.58] and I don't think
[1875.58 → 1876.74] Plex can do that
[1876.74 → 1878.10] but you know tell
[1878.10 → 1878.62] me if I'm wrong
[1878.62 → 1879.70] well also you're
[1879.70 → 1880.40] you're a bit more
[1880.40 → 1881.56] of a don't want
[1881.56 → 1882.34] to say a zealot but
[1882.34 → 1883.38] you're more into the
[1883.38 → 1884.40] privacy side of things
[1884.40 → 1885.48] and yeah you're
[1885.48 → 1886.36] more of a purist I
[1886.36 → 1887.84] think than I am and
[1887.84 → 1888.54] so I just think
[1888.54 → 1889.56] Jellyfin fits a lot
[1889.56 → 1890.26] better with your
[1890.26 → 1892.46] overall ethos than
[1892.46 → 1894.04] Plex every can will
[1894.04 → 1894.78] I don't know if you
[1894.78 → 1895.70] both saw the article
[1895.70 → 1897.08] this week came out
[1897.08 → 1897.94] literally this week
[1897.94 → 1899.58] saying Plex now has
[1899.58 → 1900.70] more streaming users
[1900.70 → 1901.80] than media server
[1901.80 → 1903.88] users that is an
[1903.88 → 1904.74] indictment of where
[1904.74 → 1905.66] Plex as a company is
[1905.66 → 1906.44] going in future I
[1906.44 → 1907.06] don't know what is
[1907.06 → 1908.58] I completely agree
[1908.58 → 1909.64] and if we're going to
[1909.64 → 1910.62] get to the question of
[1910.62 → 1911.62] am I sticking with it
[1911.62 → 1913.24] this headline basically
[1913.24 → 1914.46] made my decision for
[1914.46 → 1916.66] me unfortunately I
[1916.66 → 1918.24] I like you a suspect
[1918.24 → 1919.10] I'll keep some Plex
[1919.10 → 1920.84] around, but I imagine
[1920.84 → 1921.60] it'll be more like
[1921.60 → 1923.52] Plex on demand I'll
[1923.52 → 1924.38] fire up a docker
[1924.38 → 1925.80] container when I'm
[1925.80 → 1926.48] going to be travelling
[1926.48 → 1928.40] and you know I'll
[1928.40 → 1930.12] throw a series in
[1930.12 → 1931.62] there a movie or two
[1931.62 → 1933.00] in there and then
[1933.00 → 1934.54] I'll destroy it after
[1934.54 → 1936.46] the trip so it just
[1936.46 → 1938.34] really for me is that
[1938.34 → 1939.08] headline right there
[1939.08 → 1940.86] that story really seals
[1940.86 → 1941.46] the deal because that's
[1941.46 → 1942.82] where Plex has to go
[1942.82 → 1944.16] and I can't begrudge
[1944.16 → 1945.14] them for it, I really
[1945.14 → 1946.40] appreciate what a
[1946.40 → 1947.44] great project it has
[1947.44 → 1948.42] been I really
[1948.42 → 1949.48] appreciate how
[1949.48 → 1950.72] accessible they made
[1950.72 → 1952.20] having your own home
[1952.20 → 1953.62] streaming setup and
[1953.62 → 1954.16] I'm going to be
[1954.16 → 1955.34] grateful for the years
[1955.34 → 1957.10] of use I got out of
[1957.10 → 1958.10] Plex and I do not
[1958.10 → 1958.96] regret my lifetime
[1958.96 → 1960.24] membership at all even
[1960.24 → 1960.72] though I'm going to be
[1960.72 → 1962.02] using Jellyfin now but
[1962.02 → 1963.42] I also have to be
[1963.42 → 1964.74] realistic as a company
[1964.74 → 1966.34] they can't, they can't
[1966.34 → 1967.42] grow and become
[1967.42 → 1968.64] successful by being the
[1968.64 → 1969.34] people that enabled
[1969.34 → 1970.38] piracy that just
[1970.38 → 1972.18] cannot be what makes
[1972.18 → 1973.64] them successful and
[1973.64 → 1975.32] I'm glad to see that
[1975.32 → 1976.18] their streaming strategy
[1976.18 → 1976.86] does seem to be
[1976.86 → 1978.26] working and my hope is
[1978.26 → 1979.18] that they do really
[1979.18 → 1980.16] they leave the local
[1980.16 → 1981.26] playback in at least
[1981.26 → 1982.30] you know to some
[1982.30 → 1983.48] degree for folks that
[1983.48 → 1984.44] can have a little bit
[1984.44 → 1985.46] of both and for the
[1985.46 → 1986.82] folks that are 100%
[1986.82 → 1987.86] all in on local and
[1987.86 → 1988.62] not really interested
[1988.62 → 1989.44] all in the streaming
[1989.44 → 1990.36] there's going to be
[1990.36 → 1992.06] Jellyfin however that
[1992.06 → 1993.60] said before we wrap up
[1993.60 → 1994.88] Alex I'm curious if
[1994.88 → 1996.64] you're if you're using
[1996.64 → 1997.58] Jellyfin with the home
[1997.58 → 1998.22] run if you're going to
[1998.22 → 1999.12] do live TV streaming
[1999.12 → 2000.60] because that's been a
[2000.60 → 2001.36] bit of feedback we've
[2001.36 → 2002.20] gotten from the audience
[2002.20 → 2002.98] who's trying this along
[2002.98 → 2004.22] with us that they say
[2004.22 → 2005.16] hasn't worked great
[2005.16 → 2006.72] with Jellyfin I've had
[2006.72 → 2007.58] the opposite experience
[2007.58 → 2008.38] I'm curious if you've
[2008.38 → 2009.76] tried it I did try it
[2009.76 → 2011.60] yeah I found the whole
[2011.60 → 2013.14] setup process just had a
[2013.14 → 2013.94] few more rough edges
[2013.94 → 2015.50] than Plex which is you
[2015.50 → 2016.60] know not difficult given
[2016.60 → 2017.86] that Plex is perhaps the
[2017.86 → 2019.80] absolute easiest live TV
[2019.80 → 2021.22] setup going you just log
[2021.22 → 2023.46] in say hey oh that's my
[2023.46 → 2024.36] HD home run over there
[2024.36 → 2026.40] you click connect it asks
[2026.40 → 2027.38] you then for a postcode
[2027.38 → 2029.02] or a zip code and then
[2029.02 → 2030.44] downloads the relevant
[2030.44 → 2032.12] XML data with Jellyfin
[2032.12 → 2033.80] yeah it's the EPG data
[2033.80 → 2035.38] that's the hard part
[2035.38 → 2036.36] but once you've got that
[2036.36 → 2038.18] figured out it seemed to
[2038.18 → 2039.18] work just fine I didn't
[2039.18 → 2040.08] use it a ton because there
[2040.08 → 2041.44] weren't any huge you know
[2041.44 → 2042.26] sporting events or
[2042.26 → 2044.30] anything like that on at
[2044.30 → 2046.18] the moment but
[2046.18 → 2047.02] generally speaking my
[2047.02 → 2047.94] experience with Jellyfin
[2047.94 → 2049.54] you all know I was pretty
[2049.54 → 2050.80] skeptical going into this
[2050.80 → 2052.26] that it would stick I'm
[2052.26 → 2053.54] delighted that it is
[2053.54 → 2055.66] sticking for TV and
[2055.66 → 2057.46] movies and general video
[2057.46 → 2058.46] playback in the house on
[2058.46 → 2059.80] the TVs like they've
[2059.80 → 2061.14] solved the 10 foot
[2061.14 → 2062.10] interface problem the
[2062.10 → 2063.04] sitting on the couch with
[2063.04 → 2065.32] a remote watching videos
[2065.32 → 2067.52] that has been near
[2067.52 → 2069.94] flawless for me where I
[2069.94 → 2070.74] still need some
[2070.74 → 2072.42] improvements to do full
[2072.42 → 2073.80] adoption is the
[2073.80 → 2075.04] ancillary stuff you know
[2075.04 → 2075.92] the peripheral stuff
[2075.92 → 2077.12] around that experience
[2077.12 → 2078.14] like audiobooks for
[2078.14 → 2080.10] example if we could just
[2080.10 → 2081.52] port prologue to support
[2081.52 → 2082.94] Jellyfin that would be
[2082.94 → 2085.40] amazing some stuff around
[2085.40 → 2086.58] Fin amp you know you look
[2086.58 → 2087.58] at what Preamp's done
[2087.58 → 2089.48] that's still night and
[2089.48 → 2091.30] day miles and miles ahead
[2091.30 → 2092.30] of Fin amp and all the
[2092.30 → 2093.22] different music players
[2093.22 → 2095.10] but generally speaking you
[2095.10 → 2096.24] know I don't think I
[2096.24 → 2098.12] mind I can just disable
[2098.12 → 2099.36] the video libraries in
[2099.36 → 2100.46] Plex, although that might
[2100.46 → 2101.60] upset Brent I might leave
[2101.60 → 2102.32] I might just leave them
[2102.32 → 2105.32] or I might just give him a
[2105.32 → 2106.30] tail scale login who
[2106.30 → 2107.28] knows do I trust you
[2107.28 → 2108.64] Brent I don't know we're
[2108.64 → 2109.96] about to find out I think
[2109.96 → 2111.30] remember when he is like lived
[2111.30 → 2112.64] at your house I know for
[2112.64 → 2113.46] like three weeks
[2113.46 → 2118.22] he's been on your land
[2118.22 → 2119.30] Alex he's been there
[2119.30 → 2121.14] so ultimately I think we
[2121.14 → 2122.24] can call Jellyfin January
[2122.24 → 2124.12] a huge success I mean
[2124.12 → 2125.10] all three of us are
[2125.10 → 2126.24] keeping at least some
[2126.24 → 2128.10] level four of us
[2128.10 → 2129.12] Catherine sorry are
[2129.12 → 2130.08] keeping some level of
[2130.08 → 2131.04] Jellyfin in the house
[2131.04 → 2132.54] and that was not my
[2132.54 → 2133.72] expectation a month ago
[2133.72 → 2135.26] so I'm I'm really
[2135.26 → 2135.96] pleased about that
[2135.96 → 2137.48] yeah I'm really glad
[2137.48 → 2138.82] it's at this point it's
[2138.82 → 2139.62] something I think that's
[2139.62 → 2140.72] been kind of the elephant
[2140.72 → 2141.70] in the room almost since
[2141.70 → 2143.62] the show started and
[2143.62 → 2144.56] it's really nice to see
[2144.56 → 2145.64] it there especially for
[2145.64 → 2146.36] I think where we've
[2146.36 → 2147.78] landed it's great like
[2147.78 → 2149.38] you said on the TV I'm
[2149.38 → 2150.88] super happy with it and
[2150.88 → 2152.10] I also agree that the
[2152.10 → 2153.36] performance seems really
[2153.36 → 2155.66] fantastic so it's an if
[2155.66 → 2156.52] you're out there I know
[2156.52 → 2157.02] a lot of you have been
[2157.02 → 2158.00] trying it out there and
[2158.00 → 2158.60] you have a different
[2158.60 → 2159.68] take let us know
[2159.68 → 2160.46] self-hosted that show
[2160.46 → 2161.44] slash contact
[2161.44 → 2164.68] leno.com slash SSH go
[2164.68 → 2165.32] there to get a hundred
[2165.32 → 2166.58] dollars and 60 day credit
[2166.58 → 2167.54] and it's a great way to
[2167.54 → 2169.06] support the show if
[2169.06 → 2169.72] you've been thinking it's
[2169.72 → 2170.46] time to set up some
[2170.46 → 2171.36] infrastructure in the
[2171.36 → 2172.18] cloud, but you want it
[2172.18 → 2173.44] to be the right host with
[2173.44 → 2174.18] the right kind of
[2174.18 → 2176.10] controls and maybe even
[2176.10 → 2177.60] their postal snap in with
[2177.60 → 2178.28] whatever integration
[2178.28 → 2179.20] tooling you have
[2179.20 → 2180.42] Linde's the one I want
[2180.42 → 2181.66] you to consider they've
[2181.66 → 2182.38] been around for nearly
[2182.38 → 2183.48] 19 years, and they've had
[2183.48 → 2184.52] to survive that entire
[2184.52 → 2185.62] time on the merits of
[2185.62 → 2186.32] their product they've had
[2186.32 → 2187.28] to make a great product
[2187.28 → 2188.76] with great support and
[2188.76 → 2189.92] it's 30 to 50 percent
[2189.92 → 2190.58] cheaper than the big
[2190.58 → 2191.74] hyperscalers that want to
[2191.74 → 2192.24] lock into these
[2192.24 → 2194.00] complicated platforms that
[2194.00 → 2194.98] don't give us self-
[2194.98 → 2195.88] posters the flexibility
[2195.88 → 2197.56] that we like to see if
[2197.56 → 2198.58] you like to nuke and
[2198.58 → 2199.42] pave and roll your own
[2199.42 → 2200.44] infrastructure with your
[2200.44 → 2201.34] own central management
[2201.34 → 2202.46] tools or if you like to
[2202.46 → 2204.14] click and deploy with
[2204.14 → 2206.10] just a few clicks maybe a
[2206.10 → 2207.62] quick guide Linde's got
[2207.62 → 2208.56] it down for you whichever
[2208.56 → 2209.52] one you like whatever
[2209.52 → 2211.38] style you got Linde will
[2211.38 → 2212.64] work for you and if you
[2212.64 → 2213.54] ever get stuck they've got
[2213.54 → 2215.34] great support too so when
[2215.34 → 2216.38] I think about where I want
[2216.38 → 2216.96] to go I think of
[2216.96 → 2217.96] something fast I think
[2217.96 → 2218.68] about something that'll be
[2218.68 → 2220.30] highly available I think
[2220.30 → 2221.10] about something that I
[2221.10 → 2222.48] can rely on that I can put
[2222.48 → 2223.46] my infrastructure on that
[2223.46 → 2224.06] I don't have to think
[2224.06 → 2225.40] about all the time that's
[2225.40 → 2226.38] what I want when I go to a
[2226.38 → 2227.84] cloud hosting provider and
[2227.84 → 2228.90] Linde checks all those
[2228.90 → 2229.92] boxes, and they have a
[2229.92 → 2230.68] bunch of great features
[2230.68 → 2231.66] too like their S3
[2231.66 → 2232.98] compatible object storage
[2232.98 → 2233.64] tie that in with your
[2233.64 → 2235.26] backups you can use that
[2235.26 → 2235.88] for the back end for
[2235.88 → 2236.88] next cloud there's a lot
[2236.88 → 2238.44] of things you can do so
[2238.44 → 2239.04] go get that hundred
[2239.04 → 2240.30] dollars play around with
[2240.30 → 2241.54] something support the show
[2241.54 → 2242.70] and see what Linde is
[2242.70 → 2243.70] capable of I think you'll
[2243.70 → 2244.74] be really impressed with
[2244.74 → 2245.88] the performance and the
[2245.88 → 2247.04] selection so go to
[2247.04 → 2249.14] linode.com slash SSH one
[2249.14 → 2250.04] more time to support the
[2250.04 → 2250.68] show and get that hundred
[2250.68 → 2254.18] bucks linode.com slash SSH
[2254.18 → 2256.66] all right it's hard drive
[2256.66 → 2258.16] giveaway time how exciting
[2258.16 → 2259.34] is this I've been waiting
[2259.34 → 2260.46] for this I have to say
[2260.46 → 2261.40] Alex I wasn't able to
[2261.40 → 2262.36] read all of these some of
[2262.36 → 2263.08] them were just heart
[2263.08 → 2265.40] wreckers there is a 10
[2265.40 → 2266.68] terabyte hard drive here
[2266.68 → 2267.66] with someone's name on it
[2267.66 → 2269.04] and we have a clear
[2269.04 → 2270.38] winner thank you very much
[2270.38 → 2272.12] to everybody that voted we
[2272.12 → 2273.88] had a winner with 24 votes
[2273.88 → 2274.98] the next closest one had
[2274.98 → 2276.50] 10 so very, very clear
[2276.50 → 2278.68] winner in there but I
[2278.68 → 2279.56] thought we'd read the top
[2279.56 → 2280.90] three because you know
[2280.90 → 2282.02] there's some really
[2282.02 → 2283.00] interesting stories in
[2283.00 → 2284.46] there so Brent why don't
[2284.46 → 2285.14] you kick us off with
[2285.14 → 2286.72] third place I've royally
[2286.72 → 2287.86] screwed up with
[2287.86 → 2289.42] irreplaceable data I know
[2289.42 → 2290.82] this is a lot but it all
[2290.82 → 2291.78] comes together in the end
[2291.78 → 2293.90] so have some patience I
[2293.90 → 2294.94] can show receipts too if
[2294.94 → 2296.84] anyone asks my wife and I
[2296.84 → 2298.82] got married in 2010 and
[2298.82 → 2300.32] were immediately moved to
[2300.32 → 2302.62] DC by the military by 2012
[2302.62 → 2303.98] and after the third
[2303.98 → 2305.60] miscarriage we gave up on
[2305.60 → 2306.82] trying to have kids of our
[2306.82 → 2308.44] own consoled by a
[2308.44 → 2309.62] conversation about how the
[2309.62 → 2310.82] world doesn't need more
[2310.82 → 2311.86] people anyway
[2311.86 → 2313.66] despite this we still
[2313.66 → 2315.32] wanted to be parents and
[2315.32 → 2317.64] in 2013 we were moved to
[2317.64 → 2318.80] Las Vegas and started
[2318.80 → 2320.90] foster parent classes it
[2320.90 → 2322.42] can't be overstated foster
[2322.42 → 2324.10] care is hell for all
[2324.10 → 2325.62] involved often the kids
[2325.62 → 2327.02] come out of one garbage
[2327.02 → 2328.26] situation only to be
[2328.26 → 2329.50] dropped right into another
[2329.50 → 2331.26] we also tried to adopt
[2331.26 → 2332.62] every kid that we had the
[2332.62 → 2334.48] opportunity to which led
[2334.48 → 2335.90] to several instances of
[2335.90 → 2337.66] having a kid we weaned off
[2337.66 → 2339.00] drugs from their first day
[2339.00 → 2341.30] of life being literally torn
[2341.30 → 2342.54] out of our hands as a
[2342.54 → 2343.92] toddler and handed back to
[2343.92 → 2345.10] the person who put them in
[2345.10 → 2346.22] that situation in the first
[2346.22 → 2348.72] place despite that for every
[2348.72 → 2350.10] terrible situation there was
[2350.10 → 2351.86] one that made us happy to
[2351.86 → 2353.32] hand them off one kid
[2353.32 → 2354.74] literally drove away in his
[2354.74 → 2356.10] uncle's Porsche after spending
[2356.10 → 2357.64] a week with us that was
[2357.64 → 2359.10] shocking since he entered the
[2359.10 → 2360.22] system after his abusive
[2360.22 → 2361.60] mother was arrested for
[2361.60 → 2363.00] trying to beat a random
[2363.00 → 2365.04] person on the street his uncle
[2365.04 → 2366.66] didn't even know he existed and
[2366.66 → 2367.66] when he found out about him
[2367.66 → 2369.56] gave him a real rags to
[2369.56 → 2371.50] riches childhood turnaround
[2371.50 → 2373.96] regardless of the end state
[2373.96 → 2376.54] beautiful or horrifying while
[2376.54 → 2378.02] they were in our house they
[2378.02 → 2379.84] were our children we intended to
[2379.84 → 2381.96] adopt everyone possible and
[2381.96 → 2383.82] treated them as our own there
[2383.82 → 2384.86] were so many memories created
[2384.86 → 2386.88] over those years and I can be
[2386.88 → 2390.04] quite the documentarian though I
[2390.04 → 2391.60] was really frugal with the
[2391.60 → 2393.24] storage I was actually kind of
[2393.24 → 2395.96] proud that I only accrued a
[2395.96 → 2397.20] couple of terabytes over that
[2397.20 → 2399.16] time frame and that counts all
[2399.16 → 2400.20] the other stuff that I
[2400.20 → 2402.46] generated as well this was a
[2402.46 → 2404.28] necessary couple of terabytes
[2404.28 → 2406.46] as we weren't allowed to upload
[2406.46 → 2407.90] anything publicly and I never
[2407.90 → 2409.52] got straight answers about
[2409.52 → 2411.28] whether I could even use
[2411.28 → 2412.54] cloud storage though I was
[2412.54 → 2414.34] pretty sure I could, I wasn't
[2414.34 → 2416.02] about to run the risk that meant
[2416.02 → 2418.46] everything went on bod array in
[2418.46 → 2420.66] my closet I left the military in
[2420.66 → 2422.80] 2017, and we moved back to our home
[2422.80 → 2425.44] state in the move some things got
[2425.44 → 2428.12] jostled out of smart induced
[2428.12 → 2430.78] anxiety I decided to consolidate
[2430.78 → 2433.28] everything down into one array of
[2433.28 → 2435.76] five one terabyte drives in ZFS
[2435.76 → 2438.96] RAID 3 thinking I was honey dory I
[2438.96 → 2440.92] tossed the old drives into my hard
[2440.92 → 2443.54] drive graveyard one serial ATA
[2443.54 → 2445.56] controller malfunction later I found
[2445.56 → 2447.48] myself desperately digging through
[2447.48 → 2449.88] drawers trying to recover anything at
[2449.88 → 2452.68] all some was recoverable some though
[2452.68 → 2455.36] was gone forever birthdays Christmases
[2456.02 → 2458.88] vacations tearful reunions those are
[2458.88 → 2462.04] all gone kids we never see again kids
[2462.04 → 2463.62] that were our family for years have
[2463.62 → 2466.02] been erased completely I still hold
[2466.02 → 2468.14] out hope that I can somehow recover
[2468.14 → 2470.20] something off of that array since it
[2470.20 → 2472.58] was God's file system, but I don't have
[2472.58 → 2474.18] a controller right now that can handle
[2474.18 → 2477.58] the five plus one drives I would need to
[2477.58 → 2479.90] this day I gun shy everything is in
[2479.90 → 2482.24] multiple locations encryption keys are
[2482.24 → 2483.64] written on notebooks in different
[2483.64 → 2485.58] buildings pictures are printed despite
[2486.22 → 2487.96] it all none of this will bring back
[2487.96 → 2490.80] what was lost all I can do is ensure
[2490.80 → 2492.94] the future is remembered and protected
[2492.94 → 2495.46] appropriately since I'm not made of
[2495.46 → 2497.38] money keeping a backup strategy has been
[2497.38 → 2500.48] painful I find myself deleting things
[2500.48 → 2503.20] that I wouldn't if I had more space 10
[2503.20 → 2504.80] terabytes would be enough to let me
[2504.80 → 2507.04] spread out and prioritize instead of
[2507.04 → 2509.04] squeezing everything into a few drives
[2509.04 → 2512.20] over and over and over what a moving
[2512.20 → 2514.36] story huh man if that's not the
[2514.36 → 2518.00] worst case yeah right thanks for sharing
[2518.00 → 2520.02] that there is that horrible feeling at the
[2520.02 → 2521.70] pit of your stomach when you've lost some
[2521.70 → 2525.12] pictures and an SD card once corrupt
[2525.12 → 2528.12] mid-shoot on me the pictures weren't
[2528.12 → 2530.22] super-duper important you know it wasn't a
[2530.22 → 2532.38] wedding or anything like that but
[2532.38 → 2534.38] children I'll never see again but there
[2534.38 → 2536.20] are just I don't know 30 or 40 pictures
[2536.20 → 2538.96] on my hard drive that I know in my mind's
[2538.96 → 2540.44] eye what they should be, but they're just
[2540.44 → 2542.56] empty files and if I've still got them
[2542.56 → 2545.56] and it hurts so I can only imagine what
[2545.56 → 2547.76] this guy went through as a photographer
[2547.76 → 2551.10] I've helped countless professional
[2551.10 → 2553.64] photographers try to recover images off
[2553.64 → 2557.52] of you know f cf cards that have been
[2557.52 → 2559.88] run over by their cars or like cameras
[2559.88 → 2563.52] that have been thrown into pools at a
[2563.52 → 2566.96] wedding and like crazy situations so you
[2566.96 → 2569.14] might imagine I think I've been lucky
[2569.14 → 2572.08] that I was always tech-savvy even when I
[2572.08 → 2573.88] first got into it, so I don't think I've
[2573.88 → 2575.44] lost anything super important but the
[2575.44 → 2576.96] number of times I've tried to help others
[2576.96 → 2580.72] I don't have enough hands for it takes I
[2580.72 → 2583.10] think genuinely a couple of data loss
[2583.10 → 2586.34] incidents per person before you really
[2586.34 → 2588.96] understand you know there's probably a
[2588.96 → 2590.86] bunch of stuff that I had on my computers
[2590.86 → 2594.34] as a teenager even in my early 20s whilst
[2594.34 → 2596.36] you know we were figuring out computers
[2596.36 → 2598.40] whilst Windows XP was becoming you know
[2598.40 → 2600.30] it wasn't just me at fault it was the
[2600.30 → 2602.16] entire industry we didn't really have the
[2602.16 → 2604.00] stability that we've had of the last 5-10
[2604.00 → 2606.52] years of mobile devices and the cloud and
[2606.52 → 2608.92] everything and so backups you know in the
[2608.92 → 2610.32] old days were even more important
[2610.32 → 2612.54] arguably than they are now, although they're
[2612.54 → 2614.20] just as important I guess as they ever
[2614.20 → 2616.42] were so yeah this sub story really
[2616.42 → 2618.18] had me going it was interesting to see
[2618.18 → 2620.34] that resonated with several of the audience
[2620.34 → 2624.10] as well so that was third place Chris why
[2624.10 → 2626.24] don't you take us through second place
[2626.24 → 2628.30] this yeah all right this is this one this
[2628.30 → 2630.58] one got me so it's funny I am the one that
[2630.58 → 2633.60] reads it now about 10 years ago I convinced
[2633.60 → 2636.12] my wife to stop using Google Photos and
[2636.12 → 2638.12] allow me to back up all our photos to a
[2638.12 → 2640.60] local hard drive I was fairly new to Linux
[2640.60 → 2642.32] at the time and I needed to reinstall
[2642.32 → 2644.64] Ubuntu to fix some problems during the
[2644.64 → 2646.42] install my one terabyte hard drive was
[2646.42 → 2648.18] appearing twice in the list of devices
[2648.18 → 2650.66] confused by this but convinced it was a
[2650.66 → 2653.26] quirk of the Ubuntu installing I wiped
[2653.26 → 2655.44] both hard drives and reinstalled oh no
[2655.44 → 2658.08] after the first boot I suddenly realized
[2658.08 → 2659.74] that I'd left my one terabyte external
[2659.74 → 2662.74] drive attached, and it wiped the only copy
[2662.74 → 2665.20] of all of my wife's photos dating back to
[2665.20 → 2667.34] her very first digital camera as a
[2667.34 → 2670.10] teenager including her a year spent living
[2670.10 → 2672.60] and working in Thailand knowing what I know
[2672.60 → 2674.62] about storage devices I probably could have
[2674.62 → 2676.50] saved the data but at the time I just
[2676.50 → 2678.48] accepted all was lost and begged for
[2678.48 → 2682.64] forgiveness man oh man that stinks we've
[2682.64 → 2684.94] all been there we've all wiped the wrong
[2684.94 → 2688.14] disk with a fat finger g disk command
[2688.14 → 2691.92] or something yes this one hurts I was lucky
[2691.92 → 2693.54] because those photographers I mentioned this
[2693.54 → 2696.02] is like the typical story test disk and
[2696.02 → 2697.68] photo rescue they're kind of a combined
[2697.68 → 2700.42] thing I use that countlessly to save these
[2700.42 → 2702.32] situations you know it creates a giant
[2702.32 → 2704.98] folder of just JPEGs or whatever you've got
[2704.98 → 2707.32] but at least you've got them you know maybe
[2707.32 → 2709.34] you have to sort them or whatever that's a
[2709.34 → 2713.10] great tool and I think I was so lucky to
[2713.10 → 2716.38] learn from others that I literally made it a
[2716.38 → 2718.56] rule that I unplug all the drives I don't
[2718.56 → 2720.52] want to lose stuff from before I do a
[2720.52 → 2722.36] reinstall for this very reason you learn
[2722.36 → 2724.16] that lesson the hard way for sure you think
[2724.16 → 2727.24] I'd be fine I won't screw it up I'll, it'll be
[2727.24 → 2730.14] fine particularly you know in this situation
[2730.14 → 2732.80] with just a what sounds like an innocent
[2732.80 → 2735.66] USB drive let's get left connected so easy
[2735.66 → 2738.00] done one is none right Alex one is none
[2738.00 → 2740.54] may as well be so anyway this brings us on
[2740.54 → 2743.26] to our winner and this was the winner by a
[2743.26 → 2745.96] very clear margin with 24 votes way more
[2745.96 → 2748.30] votes than anybody else, so I'll take us
[2748.30 → 2750.48] through this one hi I'm Micah Stepson I'm
[2750.48 → 2753.40] 11 years old I enjoy biking and skiing and
[2753.40 → 2756.98] even have my own website called micahstenson.com
[2756.98 → 2760.16] I recently built my first PC for Christmas
[2760.16 → 2763.64] it's an AMD Ryzen system with a 512 gig
[2763.64 → 2766.22] hard drive I installed Linux Mint, and I'm
[2766.22 → 2768.88] really enjoying it when I'm older I wish to
[2768.88 → 2771.12] become a programmer or a computer engineer
[2771.12 → 2773.42] I've been listening to Jupiter Broadcasting
[2773.42 → 2776.10] podcasts to learn more about Linux, and I'd
[2776.10 → 2777.82] like to enter for the hard drive you mentioned
[2777.82 → 2781.82] oh that's great wow I should have had my kid
[2781.82 → 2785.58] right in, but that is fantastic well all Dylan
[2785.58 → 2787.48] has to do is look in a drawer, and I'm sure
[2787.48 → 2789.58] he'll find a drive that Brent shucked five
[2789.58 → 2792.60] years ago that top drawer in the studio is a
[2792.60 → 2795.06] good place yeah now I'm I have some
[2795.06 → 2797.36] questions because it wasn't mentioned what
[2797.36 → 2800.40] the hard drive would be used for or what
[2800.40 → 2802.60] they were hoping to learn from using said
[2802.60 → 2804.46] hard drive, so I'm curious if there will be
[2804.46 → 2806.88] a little bit of mentorship here and what
[2806.88 → 2809.20] the journey might look like I'm hopeful we
[2809.20 → 2811.08] can get a little soundbite from Micah or
[2811.08 → 2812.34] something obviously you need to get in
[2812.34 → 2813.70] touch with us Micah and let us know how
[2813.70 → 2815.20] you'd like us to ship the hard drive to
[2815.20 → 2817.10] you maybe your parents could let us know
[2817.10 → 2819.88] that self-hosted dot show slash contact
[2819.88 → 2821.54] you already know how to get in touch with
[2821.54 → 2822.68] us though because you sent this in
[2822.68 → 2824.92] obviously it would be great to hear a
[2824.92 → 2827.30] little bit more of the use case for
[2827.30 → 2828.60] this hard drive we'll get it sent out to
[2828.60 → 2829.62] you as soon as we have the shipping
[2829.62 → 2832.42] information over the next few days and
[2832.42 → 2834.88] yeah maybe we can record a little you
[2834.88 → 2836.18] know a couple of minutes segment for the
[2836.18 → 2838.26] show and let the audience know what you're
[2838.26 → 2840.04] doing with this disc I hope it's a
[2840.04 → 2841.76] massive Plex stash that's going to be
[2841.76 → 2845.76] awesome congratulations Micah yeah you
[2845.76 → 2846.64] know I just wanted to pull something
[2846.64 → 2848.94] from the headlines if you are looking
[2848.94 → 2850.88] for work recently or if you happen to be
[2850.88 → 2853.84] hiring we have set up a Jupiter jobs
[2853.84 → 2856.62] matrix chat room and this is just a place
[2856.62 → 2859.36] for those looking and those giving jobs
[2859.36 → 2861.84] and I figure if they're in the JB
[2861.84 → 2863.54] community they're probably pretty great
[2863.54 → 2865.30] to begin with and if you're listening to
[2865.30 → 2867.50] this podcast and hearing me mention this
[2867.50 → 2869.80] the hit rate of the quality of candidate in
[2869.80 → 2872.02] that chat room or the quality of job is
[2872.02 → 2873.82] going to be really high, so I don't expect
[2873.82 → 2876.04] like you know thousands, but I expect a
[2876.04 → 2876.98] few dozen in there, and they're probably
[2876.98 → 2878.58] all going to be pretty great so we will
[2878.58 → 2881.70] link to that, or you can just I don't
[2881.70 → 2883.10] know go to Jupiter broadcasting dot com
[2883.10 → 2886.44] slash matrix and get our space, and it's
[2886.44 → 2889.86] listed in there it's a matrix space or you
[2889.86 → 2893.18] can go to bit dot LY slash JB jobs you
[2893.18 → 2896.06] know Chris I got a message from one of our
[2896.06 → 2898.34] listeners just yesterday saying hey I
[2898.34 → 2901.08] really want to hire a JB listener and how
[2901.08 → 2902.52] do I go about doing that I've got this
[2902.52 → 2905.04] cool project I'm working on, so this is a
[2905.04 → 2906.48] perfect example I'll make sure to get
[2906.48 → 2909.06] them in there how it came up was I got
[2909.06 → 2910.80] contacted by somebody who wanted to buy
[2910.80 → 2912.84] it by me have me buy into a scheme where
[2912.84 → 2914.44] we would all kind of like basically make
[2914.44 → 2916.38] money by people buying and selling jobs
[2916.38 → 2918.74] on a podcast or job board I didn't want
[2918.74 → 2920.20] to do that but then somebody hit me up on
[2920.20 → 2921.50] matrix, and they said well what if we just
[2921.50 → 2923.54] did a chat room and I thought let's just
[2923.54 → 2925.58] go simple we don't need to grift on this
[2925.58 → 2928.22] we'll just make people have a know a
[2928.22 → 2930.12] nice little connection in there speaking
[2930.12 → 2931.74] of audience support we're going to just
[2931.74 → 2933.38] do the top four boosts in this week's
[2933.38 → 2934.34] episode because we're going to keep it
[2934.34 → 2936.00] tight for time we did get everybody's
[2936.00 → 2938.14] boosts thank you very, very much and
[2938.14 → 2941.08] appreciate them but Another 76 came in
[2941.08 → 2946.72] with our top boost this week at 177,776
[2946.72 → 2950.76] that's to say he is super excited about
[2950.76 → 2952.82] you getting into Kubernetes at home I'd
[2952.82 → 2954.82] love to see some I'd love to even come
[2954.82 → 2956.10] on air and talk about debunking the
[2956.10 → 2959.28] complexity I run a discord Kubernetes at
[2959.28 → 2960.72] home group where we get together and
[2960.72 → 2962.64] talk about doing Kubernetes for the
[2962.64 → 2964.90] needful, and also you wanted to plug and
[2964.90 → 2966.20] I'll have a link in the show notes to
[2966.20 → 2968.80] k8s at home search where you can do a
[2968.80 → 2970.80] search there and look for all kinds of
[2970.80 → 2973.78] things like ways to deploy home
[2973.78 → 2975.80] assistant for example, and he says the
[2975.80 → 2977.80] great thing about infra as code as we
[2977.80 → 2979.30] can share and compare deployment
[2979.30 → 2981.56] strategies Alex or Chris get in touch if
[2981.56 → 2983.90] you want to chat more, and so I checked
[2983.90 → 2985.66] out the k8 search have you looked at
[2985.66 → 2987.40] this is so cool yeah I think we
[2987.40 → 2988.90] linked this in the last episode as well
[2988.90 → 2991.62] it's a beast I am still very much in my
[2991.62 → 2994.10] infancy with this k3s stuff at home the
[2994.10 → 2996.72] new firewalls working out great and in
[2996.72 → 2998.16] the interest of time we've punted a
[2998.16 → 2999.48] segment today I was going to talk about
[2999.48 → 3003.22] my new automated DHCP and DNS setup that
[3003.22 → 3005.60] I built primarily because I was fed up with
[3005.60 → 3007.32] entering mac addresses into open sense
[3007.32 → 3009.28] manually by copying and pasting for each
[3009.28 → 3012.12] virtual machine so now I can automate
[3012.12 → 3014.00] that using Ansible and terraform which
[3014.00 → 3014.30] is
[3014.30 → 3018.48] it's fantastic awesome and nerdy and yeah
[3018.48 → 3020.80] I recognize this and man does this make
[3020.80 → 3022.46] this is the kind of that's the
[3022.46 → 3024.30] kind of tooling that's appealing to me
[3024.30 → 3027.08] too k3s is awesome says gene bean yeah I
[3027.08 → 3028.66] agree so you know what Alex you struck a
[3028.66 → 3029.86] note there I wondered if we were going
[3029.86 → 3031.94] too far into the nerdy territory and you
[3031.94 → 3033.24] proved we weren't so it's nice to get
[3033.24 → 3035.42] that feedback that's good to know well I
[3035.42 → 3037.80] do need some help at the moment I don't
[3037.80 → 3040.26] really have a good handle on storage
[3040.26 → 3042.64] distributed storage so one of my goals
[3042.64 → 3046.12] is to run just a handful of critical
[3046.12 → 3047.94] services, so things like my wiki as I
[3047.94 → 3049.84] mentioned last time I think and some
[3049.84 → 3052.58] other stuff maybe now my pinhole I'd
[3052.58 → 3054.06] like to distribute that because I've
[3054.06 → 3055.72] switched from AdGuard home to pinhole
[3055.72 → 3058.68] more details next time it would be great
[3058.68 → 3060.92] to you know use something, so I know
[3060.92 → 3062.80] pinhole has gravity sync anyway I
[3062.80 → 3065.38] digress there is longhorn I could use
[3065.38 → 3067.42] for storage there's also rocket which
[3067.42 → 3069.42] I could use for storage you know I'll
[3069.42 → 3071.80] be syncing a few megabytes maybe a gig
[3071.80 → 3074.28] or two at most I'm not syncing media
[3074.28 → 3076.12] files or anything like that between
[3076.12 → 3077.42] these nodes and one of them will be a
[3077.42 → 3079.80] Raspberry Pi and the other two or three
[3079.80 → 3083.08] nodes will be x86 boxes so it would be
[3083.08 → 3085.76] great if whatever solution you recommend
[3085.76 → 3089.46] to me internet hive brain supports
[3089.46 → 3092.10] multi-arch stuff as well but yeah it's a
[3092.10 → 3096.04] huge beast and so far I like what
[3096.04 → 3098.68] I've seen, and it's its quite refreshing
[3098.68 → 3101.38] I did a did an open shift course at
[3101.38 → 3104.50] work last week, and it was just it's nice
[3104.50 → 3107.36] when you know what all the commands do
[3107.36 → 3108.76] when you see them written down before you
[3108.76 → 3110.34] run them you know in the training course
[3110.34 → 3112.82] like that, and it's you know large a large
[3112.82 → 3114.32] part because of the experimentation in
[3114.32 → 3116.32] the homeland man that's when the home lab is
[3116.32 → 3118.72] really truly serving its purpose that's so
[3118.72 → 3121.66] great Monty came in with 6,000 SATs hey
[3121.66 → 3123.56] guys short time United States Air Force
[3123.56 → 3126.04] listener here less than two years I've
[3126.04 → 3127.58] listened to every episode of UP self
[3127.58 → 3129.88] hosted LAN and the extras I love all of
[3129.88 → 3132.70] them and can't wait for a northeast meetup
[3132.70 → 3134.66] so I can maybe join you've sparked my
[3134.66 → 3137.56] tinkering interest with the WZ mini hack
[3137.56 → 3139.76] in episode 88 that was the firmware for
[3139.76 → 3141.86] the wise cams says I'm struggling to find
[3141.86 → 3143.64] an Ethernet to USB adapter that will work
[3143.64 → 3145.06] though can you guys suggest one that's
[3145.06 → 3147.24] worked for you PS enjoy the SATs keep up
[3147.24 → 3149.50] the great work I heard a couple of people
[3149.50 → 3151.02] were looking for Ethernet adapters for
[3151.02 → 3153.06] their wise cams now I know that the WZ
[3153.06 → 3157.40] mini hack folks list a handful of
[3157.40 → 3160.38] compatible USB adapters and I linked to
[3160.38 → 3161.88] that in last week's show notes I don't
[3161.88 → 3164.04] know if those specifically do POE but if
[3164.04 → 3165.46] you look at what the devs using because
[3165.46 → 3168.74] the dev of the firmware themselves is
[3168.74 → 3171.04] doing POE adapter so you could probably
[3171.04 → 3174.56] trace it back from there I mean to me
[3174.56 → 3176.42] that's probably like a spring project for
[3176.42 → 3177.66] one of our road trips, so I'll probably
[3177.66 → 3179.42] know around then is I'm really
[3180.08 → 3182.42] hoping that I don't accidentally update
[3182.42 → 3184.32] the firmware on any of my wise cameras
[3184.32 → 3188.82] until I can try this I don't know I feel
[3188.82 → 3190.08] like they're just gonna auto update or
[3190.08 → 3192.00] something you know like I just we'll see
[3192.00 → 3193.90] but I'm really hoping to get a chance to
[3193.90 → 3195.08] try the Ethernet because I think that
[3195.08 → 3196.14] should make the picture quality really
[3196.14 → 3198.46] solid especially for such cheap cameras
[3198.46 → 3200.96] I put that new firmware on my wise v3
[3200.96 → 3202.92] straight after the show last week and
[3202.92 → 3204.90] I've done nothing with it is just
[3204.90 → 3206.46] continues to work as if I did nothing
[3206.46 → 3208.08] at all, so I suppose that's a good thing
[3208.08 → 3210.58] that's a good thing yeah yeah Scott came
[3210.58 → 3212.02] in with a row of ducks that's just
[3212.02 → 3213.96] Quakers he says this is my first time
[3213.96 → 3217.26] ever communicating with any kind of media
[3217.26 → 3219.48] entity ever and yeah I'm a longtime
[3219.48 → 3221.60] listener everything's on a pie here
[3221.60 → 3224.40] Apache Jellyfin Nextcloud Wikimedia the
[3224.40 → 3226.00] Jellyfin video processing is done on the
[3226.00 → 3228.68] NVIDIA Jet son NATO 2 gig and don't tell
[3228.68 → 3231.16] anyone but my media is actually hosted on a
[3231.16 → 3232.98] Windows 7 machine and shared out to the
[3232.98 → 3236.24] pipe but hey this pie is running tail
[3236.24 → 3237.92] scale and I can access it from anywhere
[3237.92 → 3239.84] I got another 8 gig pie running with
[3239.84 → 3241.70] umbral with well pretty much everything
[3241.70 → 3244.68] that's not Bitcoin related that's awesome
[3244.68 → 3246.60] there's a saying if it works it ain't
[3246.60 → 3249.98] stupid but sometimes that saying gets
[3249.98 → 3252.30] stretched a little bit we're not often
[3252.30 → 3254.22] too critical about somebody's setup but a
[3254.22 → 3257.42] Win 7 file server is Windows 7 end of
[3257.42 → 3259.76] life now I think so right oh yeah oh
[3259.76 → 3263.32] yeah yeah yeah little side note 1804
[3263.32 → 3266.24] Ubuntu 1804 end of life at the end of
[3266.24 → 3267.74] April so if you've got your server based
[3267.74 → 3271.06] on 1804 maybe time to upgrade or time to
[3271.06 → 3273.04] buy the extended maintenance program oh
[3273.04 → 3275.16] that's good to know how is it five years
[3275.16 → 3278.40] that is I know these are the
[3278.40 → 3279.66] facts of life that we help you keep
[3279.66 → 3281.38] track of in Linux action news little plug
[3281.38 → 3283.52] there and our last boost rail 69 came in
[3283.52 → 3285.94] with Leftists hey gang love the Jellyfin
[3285.94 → 3287.82] January challenge and I hope the trend
[3287.82 → 3289.82] will continue throughout the year regarding
[3289.82 → 3292.06] donations and supporting projects last
[3292.06 → 3294.06] year I decided on a specific amount of
[3294.06 → 3295.74] money that I would spend and donate each
[3295.74 → 3298.18] month to a project which Is am use
[3298.18 → 3301.92] extensively be would be very sad if it
[3301.92 → 3303.86] disappeared and see doesn't have a
[3303.86 → 3305.88] commercial way to get funding this year
[3305.88 → 3307.80] Jellyfin takes the funds for the first
[3307.80 → 3310.44] month thanks for the amazing content I love
[3310.44 → 3313.82] this so much what a fantastic idea as you
[3313.82 → 3315.78] know we donated some of our affiliate
[3315.78 → 3320.24] revenues from cloudfree.shop and mylocalbytes.com
[3320.24 → 3324.88] to Jellyfin and the matrix project so it's
[3324.88 → 3326.28] something we're doing here too, but I love
[3326.28 → 3327.94] to hear audience members doing if it's
[3327.94 → 3330.78] fantastic in the future when we have per
[3330.78 → 3333.52] episode splits enabled for the boost we'll
[3333.52 → 3337.00] do things like a split for the image project
[3337.00 → 3339.46] because the image project takes Bitcoin and
[3339.46 → 3341.64] so we'll put them in as a split and your
[3341.64 → 3343.38] boost will go towards those projects that's
[3343.38 → 3345.30] coming in the new year, but I agree I think
[3345.30 → 3347.14] it's I like the overall idea of whatever
[3347.14 → 3348.68] way they want to take the funds you pick a
[3348.68 → 3350.94] couple of projects throughout the year that
[3350.94 → 3352.88] you can contribute to, and I think Jellyfin is
[3352.88 → 3355.36] a perfect contender I think a lot of
[3355.36 → 3357.96] these that help you bring something on
[3357.96 → 3361.14] premises that's totally sovereign they're
[3361.14 → 3364.18] just never going to be a huge customer base I
[3364.18 → 3366.98] mean I'd like to say it's growing but the
[3366.98 → 3368.34] pool of people that are going to support
[3368.34 → 3370.22] them is much, much smaller than say
[3370.22 → 3372.94] something like Plex or something
[3372.94 → 3374.74] commercial I think you hit the nail on the
[3374.74 → 3376.36] head early with Jellyfin and their remote
[3376.36 → 3378.70] access kind of home assistant model they
[3378.70 → 3380.52] just need to copy that, and then they've got
[3380.52 → 3383.04] funding for days you know I hope maybe they
[3383.04 → 3385.28] will thank you everybody who boosted it even
[3385.28 → 3387.04] those that didn't make it on the show we do
[3387.04 → 3388.80] absolutely love them and read them, but we're
[3388.80 → 3390.66] trying to keep it tight this week you can
[3390.66 → 3392.20] boost in with a new podcast app at new
[3392.20 → 3395.58] podcast apps.com or from the podcast index go
[3395.58 → 3397.90] search for self-hosted over there and of
[3397.90 → 3399.86] course a huge thank you to our members our
[3399.86 → 3401.40] site reliability engineers that keep the
[3401.40 → 3404.20] show going and let us say no, no to those
[3404.20 → 3407.24] job board crazy creepy emails and instead
[3407.24 → 3408.90] just set up a chat room we appreciate it
[3408.90 → 3410.38] you can support the show directly at
[3410.38 → 3412.88] self-hosted. Show slash SRE or all the
[3412.88 → 3414.88] shows at jupiter. Party you get the show
[3414.88 → 3417.56] ad-free, and you get the post show here on
[3417.56 → 3419.22] the self-hosted show which we appreciate
[3419.22 → 3422.68] very much self-hosted. Show slash SRE I'd
[3422.68 → 3424.42] love to hear your ideas for challenges we
[3424.42 → 3426.48] could do over the coming months as well
[3426.48 → 3429.30] obviously we did Jellyfin in January if
[3429.30 → 3430.96] it's alliterative it stands a much better
[3430.96 → 3432.94] chance of being adopted I'll just say that
[3432.94 → 3433.54] right now
[3433.54 → 3437.40] 100% luckily there isn't a month beginning
[3437.40 → 3439.76] with p for Rodman, so I'd have to switch
[3439.76 → 3442.82] away from docker quite yet but maybe
[3442.82 → 3444.52] someone invent a new month or something
[3444.52 → 3446.16] or there's a month beginning with p in a
[3446.16 → 3449.44] different language who knows but until
[3449.44 → 3451.08] then you can go to self-hosted. Show
[3451.08 → 3452.64] slash contact for all the ways to get in
[3452.64 → 3454.40] touch with us Brent where can people find
[3454.40 → 3456.26] you these days I think the Linux Unplugged
[3456.26 → 3458.66] podcast great place to go Linuxunplugged.com
[3458.66 → 3460.32] Brentley thank you for joining us and of
[3460.32 → 3462.82] course you can get more Brent office hours. Hair
[3462.82 → 3466.24] as well I'm going to plug the Jupiter tube
[3466.24 → 3468.46] generally it's working like it was this
[3468.46 → 3470.28] week eventually, and we do the show live
[3470.28 → 3472.54] every other Wednesday over at
[3472.54 → 3475.08] Jupiter. Tube and jupiterbroadcasting.com
[3475.08 → 3476.62] slash calendar to get that converted to
[3476.62 → 3478.26] your local time it's working as long as we
[3478.26 → 3479.42] have a Was bot on hand
[3479.42 → 3482.62] very handy when you have a Was bot that
[3482.62 → 3484.46] can kick things into gear, and thanks for
[3484.46 → 3486.02] listening everybody that was self-hosted
[3486.02 → 3487.48] dot show slash 89
[3487.48 → 3488.88] you
