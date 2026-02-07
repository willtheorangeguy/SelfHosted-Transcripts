[0.00 --> 3.98]  Coming up on the show today, Alex shocks me with his latest project. Seriously.
[4.24 --> 8.52]  Then he lays down some quick fire picks. So get your notepad ready.
[8.78 --> 13.54]  And then we'll discuss what's going on with OpenSense's WireGuard setup. I'm Chris.
[13.84 --> 19.86]  I'm Alex. And this is self-hosted. No, wait, the RV and Home Assistant podcast, episode 38.
[21.14 --> 24.84]  Thought I'd open today's show with a quick shout out to the self-hosted subreddit.
[24.94 --> 28.58]  We had some love from you guys this week. Hello. Hello. Hi, if you're listening.
[28.58 --> 30.20]  Hey there. How's it going?
[30.48 --> 34.40]  It was pretty cool. Like someone tagged me in one of the threads who is on our Discord.
[34.68 --> 38.12]  And I don't know, it's just cool to see community come together like that.
[38.22 --> 45.10]  And we aren't like an official partner with the subreddit or anything, but I reached out to one of the mods or, well, they reached out to me.
[45.12 --> 49.98]  And we had a chat about a few things. We might have them on one of the shows in future.
[50.02 --> 54.36]  And it's sort of got my mind thinking about how we can involve the community a bit more.
[54.36 --> 65.78]  And, you know, getting random people on to talk about their setups and sort of figure out what containers people are running, how much storage they actually have, what the hardware underneath is.
[65.88 --> 71.86]  You know, maybe we could have a little 10, 15 minute segment every now and again with community members, like a community spotlight section.
[72.28 --> 78.72]  And you know what will end up happening is we'll get all these ideas from each other and we'll then all go off and build projects and get excited to do different stuff.
[78.88 --> 79.38]  That'd be awesome.
[79.38 --> 82.48]  People often accuse me of making them spend money. Well, it's not my fault.
[84.32 --> 85.98]  I can attest to that, actually.
[88.06 --> 89.94]  Yeah, I feel like that has definitely been the case.
[90.04 --> 94.18]  I mean, the thing is, is I love just getting ideas from the community in general.
[94.28 --> 98.38]  We get people that email into the show, but like you were saying, also over on Reddit, there's some great ideas.
[98.50 --> 102.16]  And our Discord, that's another spot where I see people kicking around stuff.
[102.16 --> 109.34]  And often either, either tried something and it, and then tell us about it or are thinking about trying something and want our advice.
[109.42 --> 111.00]  That kind of stuff goes down in there all the time as well.
[111.44 --> 114.70]  My favorite stuff to read about is, well, there's two things.
[114.84 --> 116.52]  One is the stuff that works really well.
[116.52 --> 128.56]  But the other thing is things, you know, all the stuff that people try and then abandon, for whatever reason, that's more often more interesting because that's what takes the time.
[128.76 --> 132.26]  That's what eats my time is trying stuff and failing and trying stuff and failing.
[132.42 --> 136.30]  And if I can community crowdsource that stuff, I'm in.
[136.30 --> 136.74]  Absolutely.
[138.02 --> 139.76]  There's always many ways to learn.
[139.88 --> 144.90]  Like our friends over at A Cloud Guru, they are the leader in learning for the cloud, Linux, and other modern tech skills.
[145.36 --> 148.12]  They have hundreds of courses, thousands of hands-on labs.
[148.24 --> 151.94]  You can get certified, you can get hired, you can get learning at acloudguru.com.
[152.56 --> 156.94]  Now, I've been doing a lot of travel the last few weeks back and forth to the hospital.
[157.68 --> 160.36]  And I've been needing to use a lot of hotspot data.
[160.36 --> 162.94]  And I came across, this was on Hack 5, I think, actually.
[162.94 --> 177.22]  Yeah, I came across just a really interesting little hack, little tip for anybody looking to do, you know, phone tethering and try and bypass the limits that people have that Verizon or AT&T and people like that set.
[177.38 --> 178.20]  Now you got my attention.
[178.48 --> 181.26]  Yeah, I'm sure I do, given that your house is on wheels.
[181.74 --> 185.68]  So the thing you can do is set something called a TTL, time to live parameter.
[186.00 --> 192.22]  And this is apparently how the phone providers recognize whether you're on a laptop or a phone.
[192.22 --> 195.28]  That seems too easy, too good to be true.
[195.34 --> 206.00]  But I can confirm, having been streaming Netflix over 4G, 5G for the last month, that I went from it being unwatchable to being usable.
[206.26 --> 207.08]  So it does work.
[207.14 --> 209.16]  And there's a link in the show notes to a Reddit thread about this.
[209.50 --> 210.18]  This is fantastic.
[210.84 --> 213.68]  I absolutely have struggled with this.
[214.26 --> 215.90]  I've experimented with this myself.
[215.90 --> 222.32]  So by checking the TTL of the IP packets, they seem to be able to suss out the type of device that it is.
[222.78 --> 227.20]  But you can tweak that yourself, which is what this guide walks you through.
[227.86 --> 228.96]  And there's other ways, too.
[229.50 --> 239.16]  I have found WireGuard to be an extremely successful way to get around carrier bandwidth shaping, which is really what's happening here is they're looking at your IP traffic, right?
[239.16 --> 243.50]  And they can say, okay, well, you're going to YouTube on port 443 or whatever it is.
[243.52 --> 246.10]  They can actually look at the traffic because it's all running over their gear.
[246.76 --> 248.74]  They have complete access to your traffic.
[248.74 --> 257.60]  And they have systems in place that will automatically force, and in some cases, in a really brute sort of lowbrow way.
[258.02 --> 270.66]  One of the ways AT&T will do this is they will just make YouTube smack up against a wall and try all of the different bit rates until YouTube, the servers, finally select a low enough bit rate.
[270.84 --> 274.20]  And then AT&T will allow the YouTube traffic to pass.
[274.58 --> 275.54]  And that's how they do it.
[275.54 --> 282.12]  Then you have others like T-Mobile who will actually re-encode your video traffic while it's in transit.
[283.10 --> 284.28]  Yeah, there's different approaches.
[284.62 --> 285.04]  That's nuts.
[285.16 --> 289.54]  That sounds, I mean, that's going to cost them a lot in CPU, surely, if nothing else.
[289.86 --> 291.36]  That may not be how they do it anymore either.
[291.44 --> 292.36]  They change as well.
[292.48 --> 297.08]  So that's why I say today in early 2021 may not be how they do it at the end of 2021.
[297.08 --> 303.58]  But I have found, so what I do is I have a kind of a special sauce VPN.
[303.84 --> 308.54]  It's a bit of a proprietary solution from a vendor, but it bridges AT&T and Verizon.
[308.84 --> 311.16]  And the endpoint is a couple of Linode servers.
[311.90 --> 315.52]  And the carriers just have no idea what I'm doing when I do that.
[315.56 --> 319.82]  And that allows you to get around this, but it doesn't allow you to get around bandwidth limitations.
[319.82 --> 325.26]  So if you still have, you know, X amount, you know, 18 gigs a month and you can't go over that, it doesn't solve that problem.
[325.44 --> 326.40]  Are you on an unlimited plan?
[326.92 --> 327.44]  I am, yes.
[327.66 --> 332.70]  My employer pays for it, so I don't really have to look at the bill, which is quite a nice position to be in.
[332.80 --> 334.54]  Oh, that is sweet.
[334.76 --> 341.68]  You mean, really, as a consumer, as an average consumer, it's pretty tricky to even get unlimited data to begin with, let alone get it for free.
[342.04 --> 346.60]  Well, I'm sure it's, you know, it's Verizon Unlimited, so it's probably got all sorts of T's and C's.
[346.60 --> 353.98]  I think I get 30 gig of hotspot data and then the rest is throttled down to like 600 kilobits or something like that.
[354.70 --> 363.06]  What this TTL parameter does is it basically gives you all of your data allowance that the T's and C's permit at full speed.
[363.60 --> 365.34]  That's effectively what this does.
[365.82 --> 366.44]  That is great.
[366.52 --> 368.26]  We will put a link to that in the show notes.
[368.52 --> 371.92]  It's going to be different per carrier, but that seems to work on Verizon.
[371.92 --> 372.74]  Mm-hmm.
[373.46 --> 377.76]  Now, have you been looking for a self-hosted file sync and sharing, like, web UI?
[378.38 --> 381.84]  This just came up, actually, within 24 hours.
[382.08 --> 384.98]  And I don't really know what's good anymore, so I'm hoping you have a solution for me.
[385.18 --> 394.68]  Well, I was spinning up some stuff on Proxmox the other day, and I had a VM, and I didn't have Samba installed on my server because I'd literally just built it.
[394.72 --> 397.20]  I hadn't run the Ansible, and I just needed one file.
[397.20 --> 401.22]  So I thought, why don't I find a web UI to browse my files?
[401.64 --> 402.62]  And I thought, well, I've got Nextcloud.
[402.72 --> 404.34]  I could just upload the zip file to Nextcloud.
[404.50 --> 407.24]  Oh, wait, I haven't deployed Docker yet.
[407.28 --> 408.32]  I haven't done all this stuff yet.
[408.44 --> 419.88]  So what I did was I ended up spending two hours to solve a five-minute problem by spinning up FileRun, which is a self-hosted file sync and sharing solution.
[419.88 --> 430.44]  It purports to install on any private Linux, Mac, or Windows server, but it will also support, you know, cPanel-style, PHP-based type stuff as well.
[430.76 --> 433.62]  I've got it running out of a container, well, four, actually.
[433.76 --> 438.16]  So it uses the FileRun container itself.
[438.26 --> 447.50]  It uses Elasticsearch and something called Apache Ticker to do file indexing as well as MariaDB or MySQL for a backend database.
[447.50 --> 454.52]  So it's not a super lightweight thing, but it is very pretty, it's very performant, and it does exactly what it says on the tin.
[454.86 --> 458.08]  I don't really need the search, so I don't need all that overhead.
[458.22 --> 466.50]  What I really wanted was just browse my files, but this does have something I hadn't considered, but now looking at the feature list would be extremely useful.
[467.28 --> 470.20]  And that is it lets you send file requests to somebody.
[470.20 --> 475.96]  So I could send you a request, say, hey, Alex, send me that, you know, send me that batch of pictures or whatever.
[476.62 --> 478.18]  And then it would give you a way to send those to me.
[478.62 --> 481.80]  It's not like you send and receive files around the internet for your day job or anything, is it?
[482.06 --> 482.64]  Yeah, right?
[482.92 --> 489.88]  And so to actually be able to request something from someone, it just seems like it's a, it's a sort of an extra level of care for guests on the network.
[489.88 --> 493.94]  And then it also supports guest users too, which I also would need.
[493.94 --> 501.18]  And so help me understand this, is it creating its own document space and what you upload and put into it is what you see through the web UI?
[501.34 --> 505.50]  Or does it let you browse existing folders and files on your server?
[506.08 --> 508.90]  So you're trying to compare it to a Nextcloud with that comment, I suppose.
[509.42 --> 513.96]  With Nextcloud, you end up sort of creating your own space within your file system.
[513.96 --> 522.02]  But this guy, FileRun, you just point it at a file share or an existing directory or a volume bind mount, in my case, with a container.
[522.78 --> 524.14]  And everything just showed up.
[524.18 --> 525.32]  I didn't have to change permissions.
[525.52 --> 526.98]  I didn't have to mess about with anything else.
[527.34 --> 534.16]  I've actually got it set to read only just because, well, I mean, the DNS that I have is exposed through traffic.
[534.36 --> 537.34]  So, I mean, it's not going outside my LAN anyway.
[537.82 --> 541.72]  But, you know, I feel like a web UI, it's a bit too easy to get a bit trigger happy sometimes.
[542.10 --> 543.62]  So it's read only for me.
[543.62 --> 545.90]  I just want to use it to download the odd file here and there.
[545.98 --> 549.20]  But it's very useful and no import is required.
[549.54 --> 551.84]  So, yeah, very easy to get started.
[552.36 --> 553.86]  That is exactly what I was hoping for.
[553.94 --> 558.98]  It seems it also even has file versioning, if that's something that matters to you, and has a trash.
[559.10 --> 562.28]  So if you delete something, it'll first store them in there before it gets permanently erased.
[562.34 --> 564.90]  So you kind of have an escape hatch if you need it.
[565.54 --> 565.88]  All right.
[566.48 --> 566.72]  Yep.
[567.10 --> 570.10]  I'm going to deploy this, especially since it seems like...
[570.10 --> 571.06]  You know what you need to do, Alex?
[571.06 --> 572.52]  You've got to send me your Docker Compose for me.
[572.52 --> 573.48]  Make it real easy for me.
[574.38 --> 574.80]  All right.
[575.52 --> 575.84]  Yeah.
[575.90 --> 576.76]  But no, I'm going to give it a try.
[576.90 --> 577.62]  That's a great find.
[577.70 --> 579.04]  It's called, again, File Run.
[579.42 --> 583.54]  So they do offer an enterprise version in case you see any prices or anything like that.
[583.60 --> 586.20]  It's free for up to 10 users for personal and family use.
[586.28 --> 591.10]  But they have paid versions for, you know, small businesses and enterprise as well.
[591.34 --> 592.60]  So they have a means to make money.
[592.66 --> 593.58]  They have a business side.
[593.58 --> 596.46]  And that means it's probably going to stick around.
[596.72 --> 597.76]  Does use web dev, though.
[598.00 --> 599.38]  I'm never mad keen on web dev.
[599.60 --> 603.34]  But that does mean you can do file syncing using, I think, the next cloud client.
[603.76 --> 604.68]  We'll talk to this.
[605.18 --> 609.64]  And if you're behind a corporate firewall, too, it's just kind of nice to do everything over the web ports.
[610.06 --> 612.74]  I'll put a link to my Compose snippet in the show notes.
[613.22 --> 615.78]  I did come across a new project called TermPad.
[616.02 --> 617.86]  I think it's termpad.io this week.
[617.98 --> 618.30]  All right.
[618.32 --> 619.02]  Let's take a look at this.
[619.20 --> 619.82]  TermPad, huh?
[620.10 --> 620.90]  TermPad.com.
[621.06 --> 621.74]  My apologies.
[622.36 --> 627.00]  And it's a very, very super simple, like, if you just create some text and then click save.
[627.28 --> 629.40]  Oh, that's what I'm seeing.
[629.70 --> 630.48]  Oh, my gosh.
[630.48 --> 634.20]  It's a full screen, not a terminal per se, but it looks kind of like one.
[634.64 --> 635.70]  This is just a write space.
[636.38 --> 636.98]  It's neat.
[637.38 --> 642.40]  You know, like, Docker containers come up with fake names if you don't name them, like Angry Torvalds or something.
[643.66 --> 644.02]  Yeah.
[644.02 --> 646.48]  It's funny my mind went to Angry Torvalds, isn't it?
[646.52 --> 646.86]  It's funny.
[647.02 --> 647.42]  Funny that.
[647.42 --> 656.74]  So the one I've just created for you was termpad.com slash awful wide eyed napkin, which is a really strange, random generated name.
[656.84 --> 662.84]  But it does code syntax highlighting as well, just for super simple, you know, paste bin stuff.
[663.00 --> 663.64]  There's no database.
[663.90 --> 665.48]  It's all just open.
[665.82 --> 668.90]  So termpad.com is a hosted version, free.
[669.02 --> 670.50]  I don't know what happens to the data on that one.
[670.72 --> 672.34]  But you can self host it as well.
[672.34 --> 675.10]  There is a container, which we'll put a link to in the show notes.
[675.10 --> 677.36]  Kind of surprisingly useful.
[677.60 --> 678.02]  I love it.
[678.60 --> 680.90]  Okay, let's see if you are two for two here, Alex.
[680.98 --> 682.12]  Tell me about TinyPin.
[682.52 --> 684.12]  We're going to be redoing our bathroom soon.
[684.24 --> 687.40]  So I was looking across Pinterest the other day and it's just garbage.
[687.54 --> 691.48]  They make you sign in and do all this kind of nonsense about tracking what you're looking at.
[691.66 --> 695.96]  And I mean, it's kind of okay from a discovery point of view, but it's also just garbage.
[696.72 --> 697.36]  I hate Pinterest.
[697.36 --> 703.06]  So I went on the look for something, you know, minimal to just share like a mood board almost.
[703.14 --> 704.42]  And I came across TinyPin.
[704.72 --> 706.08]  I'll put a link in the show notes, of course.
[706.36 --> 709.88]  And this is a self hosted minimalistic image collection board.
[710.66 --> 711.40]  Super simple.
[711.58 --> 715.06]  You can run it in a container and there isn't a lot else to say.
[715.20 --> 718.72]  It just does the job it's supposed to do, which I suppose is the praise that you want.
[719.20 --> 720.98]  And it's nice to see that they have Chrome extensions.
[721.50 --> 725.78]  And through iOS shortcuts, there's a way you could add it to your share sheet as well.
[725.78 --> 726.84]  It seems that's handy.
[727.16 --> 732.16]  I don't see necessarily something in here for Android, but there probably is a means if you can think it up.
[732.76 --> 743.54]  I had a quick look at TinyPin just before the show and it is very minimal, but it does a good job of laying images out in different sizes in a very dynamically scalable way.
[743.60 --> 747.88]  So you can have a tablet size, you can have a full web page version, or it can be on your phone.
[748.06 --> 753.44]  And it actually manages to sort of present the images in a unique way while also letting you get in there at full screen.
[753.44 --> 756.20]  So I kind of, I think this is a nice little find.
[756.26 --> 760.28]  I don't quite grok how it's, okay, can you explain to me how it's sucking the images in and storing them?
[760.32 --> 761.88]  Because that's the part I don't quite grok.
[762.18 --> 763.14]  No, I'm not sure.
[764.02 --> 766.94]  It stores in the backend, it stores stuff in a data directory.
[767.08 --> 769.10]  So it's just a volume bind mount on the file system.
[769.36 --> 771.86]  Nothing too crazy, no database needed or anything like that.
[772.14 --> 775.10]  And you could go sniffing through there and back them up pretty easily if you needed to.
[775.26 --> 775.58]  Mm-hmm.
[775.98 --> 777.10]  Okay, well, we're two for two.
[777.18 --> 778.22]  I think that's a pretty good find.
[778.34 --> 780.18]  I think also the wifey would really love that one.
[780.26 --> 783.04]  That'd be a good one to add to the home server to impress her, I think.
[783.70 --> 786.32]  Now I want to see if you can be three for three on this one, Alex.
[786.42 --> 788.80]  Tell me about OpenSense 21.1.
[789.16 --> 791.36]  I vicariously OpenSense threw you.
[792.56 --> 797.00]  Well, PFSense made a bit of a stink the other week by adding WireGuard support finally.
[797.56 --> 805.80]  And not to be outdone, the OpenSense project released 21.1, which is nicknamed Marvelous Meerkat.
[806.20 --> 806.54]  Hmm.
[806.54 --> 813.32]  They say that it has new and improved firewall rules, NAT categories, better traffic graphs, all that kind of stuff.
[813.76 --> 819.44]  And they have a really small dig in their release notes at PFSense, which I really enjoyed, which says,
[819.88 --> 828.00]  for those wondering, the WireGuard plugin has been available on OpenSense since 2019 and receives continuous improvements by its maintainer.
[828.00 --> 830.34]  And that feature is unlikely to change.
[830.34 --> 834.76]  My eyes were immediately drawn to that in their release notes.
[835.58 --> 838.24]  I didn't realize PFSense had added WireGuard, but this is really good now.
[838.32 --> 840.40]  We have it in both OpenSense and PFSense.
[840.84 --> 842.92]  Our WireGuard future has arrived.
[842.92 --> 848.92]  I'm just sad that it didn't make it into in 2020 because my prediction was that PFSense would ship WireGuard.
[849.62 --> 853.20]  But I guess those BSD guys just shit when they're ready.
[853.72 --> 855.52]  No plans for you to go back, I assume?
[855.72 --> 858.32]  You're going to stick with the old OpenSense, I would imagine?
[859.86 --> 861.58]  OpenSense is kind of driving me crazy.
[861.82 --> 862.06]  Oh.
[862.32 --> 863.18]  There's a few reasons.
[863.64 --> 865.74]  Mostly to do with WireGuard, if I'm honest.
[866.06 --> 867.92]  I just think the implementation is...
[868.72 --> 870.48]  Maybe it's user error.
[870.48 --> 886.22]  Okay, I will fully admit that I am not a network guy, but I spent, from the hospital, at least two or three weeks for maybe half an hour to an hour at a time, most days, trying to get WireGuard fully working.
[886.54 --> 889.48]  So I can connect in remotely just fine.
[890.00 --> 893.84]  I can ping the firewall just fine.
[893.92 --> 896.34]  I can connect to the web UI of the firewall itself just fine.
[896.58 --> 899.60]  I can route traffic through my home internet connection just fine.
[899.60 --> 904.84]  But I can't access any hosts on my LAN, which kind of defeats the purpose for me.
[904.92 --> 910.36]  I mean, I don't necessarily really want to route my traffic through my house, but it's a nice benefit of WireGuard.
[910.60 --> 917.70]  What I wanted was to be able to access Proxmox or ESXi remotely and continue rebuilding my servers, which I've been doing for the last couple of months.
[917.70 --> 925.40]  And I've wasted, I don't even know how many hours, trying to make this effing thing work.
[925.52 --> 930.96]  And I wrote the man page on WireGuard for OpenSense, and I feel like a fraud because I just can't make it work.
[932.36 --> 933.50]  I wrote the book.
[933.72 --> 936.70]  I'm convinced at this point that there is a bug that I can't find.
[936.70 --> 947.12]  So I'm probably going to NukemPave my OpenSense install, which is, I don't want to do it, but I've wasted so much time and I'm convinced I've got all the firewall rules set up correctly.
[947.68 --> 949.54]  I don't see that I'm left with any other option.
[950.30 --> 961.32]  And so that then makes me think, well, if I'm going to NukemPave OpenSense, why don't I try ViOS or some other, I don't know, there's a million different options to try out there.
[961.32 --> 966.26]  Or I could just go whole hog and run, you know, CentOS streams and IP tables.
[967.50 --> 969.42]  Go full West Payne on it is what you could do there.
[969.56 --> 970.26]  He does it home.
[971.00 --> 973.04]  Yeah, that WireGuard routing issue is tricky.
[973.16 --> 976.38]  He and I had to do some troubleshooting to get that working here at the studio.
[977.36 --> 980.34]  ViOS, I've heard the Discord talking about that recently.
[980.46 --> 981.42]  Is that a firewall platform?
[981.84 --> 982.28]  It is, yeah.
[982.30 --> 983.90]  It's Linux-based, so not BSD.
[984.60 --> 987.46]  There's no web UI whatsoever, so far as I'm aware.
[987.46 --> 995.60]  I did try it once about a year ago for a few hours and the learning curve is real, so I gave up.
[997.02 --> 1002.46]  The trouble is with learning a firewall is you go on the internet to Google stuff, don't you?
[1003.06 --> 1006.76]  But if your firewall's down, you have a hard time doing that.
[1006.88 --> 1012.36]  So there are some things that are so mission critical that I just almost can't be bothered to change them
[1012.36 --> 1016.72]  because I know how much work it's going to be to learn a new thing and OpenSense is good enough.
[1017.46 --> 1018.62]  I do love the project.
[1018.76 --> 1020.84]  I mean, I think it's very stable.
[1021.02 --> 1022.40]  I never have to reboot the box.
[1022.50 --> 1025.56]  I never have to worry about updates or anything like that.
[1026.08 --> 1028.56]  But this WireGuard issue is kicking my ass, to be honest with you.
[1028.96 --> 1029.30]  I agree.
[1029.38 --> 1030.24]  It is a great product.
[1030.72 --> 1036.44]  It is a solid project that, and PFSense before it, too, just I also really like it.
[1037.00 --> 1037.58]  But I get you.
[1037.70 --> 1038.36]  I know what you mean.
[1038.54 --> 1041.54]  And sometimes it's really easy with WireGuard because something has it built in,
[1041.62 --> 1044.82]  like some of the GI routers that we've talked about before.
[1045.46 --> 1047.24]  And sometimes it's something you've got to build up.
[1047.46 --> 1053.58]  I'm the guy that was trying to do WireGuard from behind a double carrier grade NAT to a Linode,
[1053.74 --> 1054.86]  then down to the studio.
[1055.24 --> 1057.26]  And I wanted to get to everything by its name.
[1057.46 --> 1058.96]  And I mean, that's quite the setup.
[1059.22 --> 1060.70]  Maybe we'll chat more about it sometime.
[1060.70 --> 1066.06]  What I did end up doing was I ended up looking at the Linux server WireGuard Docker image.
[1066.66 --> 1068.78]  Now, this thing is slick AF.
[1069.70 --> 1071.56]  So you spin up the container.
[1071.80 --> 1072.90]  You do it in Docker Compose.
[1072.98 --> 1075.60]  You name your peers just as an environment variable.
[1075.60 --> 1078.26]  So you can either say, I want peers four.
[1078.66 --> 1081.76]  You know, so I want four peers and just deal with peers via a number.
[1081.76 --> 1087.60]  Or you can say peers and then just put a space limited list.
[1088.10 --> 1094.06]  So, you know, you put phone space, desktop space, server, whatever, as the environment variable.
[1094.06 --> 1096.84]  And it will go and generate all the config files for you.
[1096.94 --> 1098.56]  But here's the really cool bit.
[1098.56 --> 1107.04]  They've built in an alias into the container that will print out a QR code for each of those setups from a single line command.
[1107.68 --> 1108.92]  It's just slick.
[1109.16 --> 1117.44]  You know, after messing about with OpenSense for so long and it's kind of older, less mature, I would say, implementation,
[1117.74 --> 1120.72]  to come across the Linux server container was just a breath of fresh air.
[1121.42 --> 1123.38]  And so I ended up using our sponsor, Linode.
[1123.58 --> 1126.74]  So you can use the coupon code linode.com slash SSH.
[1126.74 --> 1133.54]  I ended up using our sponsor, Linode, to spin up a host dedicated to running this Linux server WireGuard container.
[1133.82 --> 1135.28]  And it just works really well.
[1135.34 --> 1136.32]  The performance is great.
[1136.74 --> 1138.94]  And I'm able to back this thing up.
[1139.00 --> 1141.72]  So I know that if anything happens, I've got the Linode backups.
[1142.22 --> 1143.52]  It just works really, really well.
[1144.28 --> 1151.56]  And whilst I was fiddling about with this container, I ran across a blog post from John Muchovesch.
[1152.24 --> 1153.96]  I'm sorry, I probably butchered that name.
[1153.96 --> 1157.20]  The website link will be in the show notes, of course.
[1157.46 --> 1159.40]  And this is super cool.
[1159.70 --> 1165.48]  It lets you route specific containers through the WireGuard container as well.
[1165.56 --> 1172.50]  So you're able to use the Docker networking to potentially have multiple instances of WireGuard going to different places for different services,
[1172.50 --> 1174.00]  all on the same box.
[1174.76 --> 1187.56]  And it uses a parameter that is released as part of Docker Compose 3.8 schema of network mode service colon WireGuard to route the traffic through that container.
[1187.74 --> 1195.26]  So you could, for example, basically bind NextCloud or any other service to listen only on that WireGuard server,
[1195.62 --> 1198.24]  just using one line of config in your Compose file.
[1198.50 --> 1199.28]  Super cool.
[1199.28 --> 1201.06]  And I love this kind of stuff.
[1201.06 --> 1204.80]  linode.com slash SSH.
[1204.88 --> 1209.66]  Go there to get a $100 60-day credit towards a new account and go there to support the show.
[1209.74 --> 1211.80]  This is a great way to see what Linode can do.
[1212.26 --> 1213.86]  They're our cloud hosting provider.
[1214.04 --> 1218.40]  If it's backend infrastructure for the network, if it's a game server for my kids,
[1218.52 --> 1222.88]  or if it's a project we're working on for self-hosted, we run it all on Linode.
[1223.14 --> 1224.90]  You have $100 here to work with.
[1225.24 --> 1226.22]  I mean, I want to be frank with you.
[1226.22 --> 1229.04]  You can do so much at Linode with that much credit.
[1229.60 --> 1231.90]  Check out some of their GPU systems.
[1232.02 --> 1232.94]  These are crazy.
[1233.06 --> 1239.38]  And in fact, Cloud Spectator Benchmarking, it's a group that goes around and tries the performance aspects of different cloud providers.
[1239.38 --> 1248.80]  They recently said that Linode has the fastest GPUs in the industry, outperforming AWS, Azure, Google.
[1249.10 --> 1254.98]  I mean, if you have any kind of image manipulation workload that you need to do and you just want to crank it out super fast,
[1255.32 --> 1261.14]  go to linode.com slash SSH and get our $100 credit and use some of it for that.
[1261.60 --> 1267.76]  Image stuff is so cool right now because there's so many fun open source projects that you can play with and easily deploy on Linode.
[1267.76 --> 1275.78]  The entire stack, regardless of what kind of system you get, they all have super fast native SSDs, 40 gigabit connections into the hypervisors,
[1275.92 --> 1278.30]  and they have 11 data centers around the world.
[1278.38 --> 1282.60]  So there's probably something that's going to work for you, a client, a customer, et cetera.
[1283.08 --> 1289.94]  And additionally, they have all of this while being 30 to 50% less than AWS or Google, right?
[1289.98 --> 1290.96]  I mean, that's what's amazing.
[1291.12 --> 1293.74]  Fastest GPUs, crazy fast network connections.
[1294.10 --> 1296.40]  The reason why is they've been around since 2003.
[1296.40 --> 1299.30]  So they had a lot of time to figure out how to do this right.
[1299.62 --> 1303.44]  They have had a lot of time to get great deals, great network providers and connections.
[1303.94 --> 1308.38]  I mean, this is the benefit of being an independent cloud provider for as long as they have.
[1308.44 --> 1310.58]  They got a jumpstart on everybody else.
[1310.78 --> 1316.00]  And you can benefit now by going to linode.com slash SSH and you can support this here show.
[1316.96 --> 1320.82]  Linode is really dedicating to offering the best Linux experience in the cloud.
[1320.82 --> 1325.80]  If it runs on Linux, you'll be able to run it on Linode and be able to manage it easily with their cloud manager.
[1326.28 --> 1327.90]  Linode.com slash SSH.
[1328.06 --> 1330.32]  Thanks to Linode for sponsoring the self-hosted program.
[1330.84 --> 1335.72]  And thanks to everybody who supports our show by visiting linode.com slash SSH.
[1335.72 --> 1338.28]  What show is that?
[1338.28 --> 1343.80]  I mean, we had accusations this week of being the Raspberry Pi and RV Home Assistant podcast.
[1344.24 --> 1348.62]  Well, it kind of goes that way sometimes, but I think it's a reflection of the trends of the time, man.
[1349.44 --> 1352.36]  Pi's come to a really good price point and performance.
[1352.90 --> 1355.28]  Low power is more popular than ever.
[1355.72 --> 1357.24]  Also, low noise, I'll point out.
[1357.92 --> 1361.20]  And Home Assistant is just blown up in the last three years.
[1361.20 --> 1366.72]  You know what's really going to annoy that comment here in particular is that I have been running Home Assistant on the Pi.
[1366.92 --> 1370.58]  So we're going to talk about the Pi for a little bit right now for the last month.
[1370.70 --> 1371.64]  And it's been great.
[1371.72 --> 1372.30]  The Pi 4.
[1372.80 --> 1376.26]  I found an old SSD in a drawer, 120 gig SSD.
[1376.48 --> 1378.06]  That's probably five years old.
[1378.74 --> 1385.64]  And I have, from my shucking of easy stores, I have a USB to SATA converter.
[1385.84 --> 1387.48]  So I just reused that.
[1387.48 --> 1391.56]  So I'm upcycling, reducing e-waste, all that kind of good stuff.
[1391.76 --> 1392.12]  Go me.
[1392.78 --> 1401.34]  And I put the Raspberry Pi Home Assistant image on there, expecting it to be, you know, I'm coming from an x86 platform.
[1401.50 --> 1407.22]  So whilst I move across from my Xeons to the Intel system and sort of redo things and move things around,
[1407.28 --> 1411.70]  I got fed up of my DNS stopping working all the time because I was running AdGuard in a container.
[1411.70 --> 1419.34]  And I got fed up of Home Assistant not being up because it automates a lot more in my house than I really realized when it's not there.
[1420.30 --> 1424.36]  And I was expecting the Pi to be just a stopgap.
[1424.50 --> 1431.32]  I was expecting it to be good enough, but I was expecting to be ready to leave it after a few weeks.
[1431.32 --> 1437.54]  And I'm pleasantly surprised to report that I think it's fine for most people.
[1437.98 --> 1438.08]  Wow.
[1438.12 --> 1439.10]  I got to take all this in.
[1439.22 --> 1441.88]  This is a moment in the show.
[1441.96 --> 1442.74]  Episode 38.
[1442.86 --> 1444.16]  Mark it down in the books, everybody.
[1444.36 --> 1444.76]  Wow.
[1445.42 --> 1445.78]  Wow.
[1445.88 --> 1448.90]  Because I feel like you always thought I was a little silly for doing it on the Pi.
[1449.04 --> 1449.36]  I did.
[1449.62 --> 1450.12]  I'll be honest.
[1450.20 --> 1450.40]  Yeah.
[1450.40 --> 1453.82]  I mean, the storage thing is still a problem.
[1454.00 --> 1462.96]  I don't like having an SSD with its ass hanging out on my desk with some random SATA to USB board connected up.
[1463.16 --> 1468.98]  And I'm not comfortable, if I'm being honest, with so much of what I depend on running over USB.
[1469.50 --> 1469.80]  Yeah.
[1470.12 --> 1470.74]  I don't like it.
[1470.98 --> 1471.32]  I agree.
[1471.40 --> 1471.64]  Totally.
[1472.18 --> 1473.70]  But the performance has been good.
[1473.84 --> 1477.86]  I mean, I don't do anything too crazy with image processing or anything like that through Home Assistant.
[1477.86 --> 1483.92]  I do that generally through Blue Iris, which is a dedicated box in my closet over there.
[1484.44 --> 1486.82]  And this leads us nicely into some follow-up.
[1486.92 --> 1497.00]  So a little while ago, I talked about doing or wrote about doing Intel GVT-G pass-through, which is virtual GPUs.
[1497.12 --> 1504.30]  So you can slice up the graphics card built into your CPU into a couple of slices, give Plex and QuickSync one slice,
[1504.38 --> 1506.96]  and then give Blue Iris and QuickSync another slice over there.
[1506.96 --> 1512.16]  And then there's still some left for the host at the same time with no PCIe GPUs required.
[1512.88 --> 1514.42]  That's like the holy grail for me.
[1514.48 --> 1515.88]  That was like the perfect setup.
[1516.78 --> 1519.38]  Unfortunately, it didn't work very well.
[1519.48 --> 1520.36]  Didn't work out very well.
[1520.82 --> 1521.02]  What happened?
[1521.26 --> 1524.24]  I was getting kernel panics with Proxmox.
[1524.52 --> 1529.16]  I was getting hung processes without kernel panics.
[1529.16 --> 1532.92]  So it was fine as long as I wasn't running Blue Iris.
[1533.24 --> 1540.04]  And I think the Windows Blue Iris load was just too much for the GVT-G stuff to handle.
[1540.70 --> 1543.96]  And I wrote a blog post about how to do it with Proxmox.
[1544.08 --> 1547.20]  And a lot of people have been pinging me about the performance and stuff like that.
[1547.20 --> 1555.96]  So this is unfortunately my update is to say that I have bought and sold an HP 290 in the last month because I was so happy it worked.
[1556.04 --> 1559.00]  And then the proof in the pudding turned out to be it wasn't good enough.
[1559.06 --> 1564.40]  So I've gone back to a dedicated Windows box for Blue Iris with QuickSync.
[1564.40 --> 1576.06]  And now my server is still the i5-8500 that I purchased running Plex using QuickSync on that box with pass-through for the storage and that kind of stuff to a VM.
[1576.66 --> 1583.62]  So I'm running Plex on the host, but I'm still running most of my containers in a VM on that host with Proxmox.
[1583.76 --> 1585.62]  And a lot of people will think I'm mad for doing that.
[1585.62 --> 1591.94]  But I prefer doing it that way because it minimizes the number of reboots I need to do on the host.
[1591.94 --> 1596.42]  When you say you're running on the host, do you mean in a container or do you mean actually installed like a package?
[1596.84 --> 1599.12]  Plex is running in a container on top of Proxmox.
[1599.78 --> 1601.80]  A Docker container, not an LXC.
[1602.12 --> 1608.96]  I'm using LXC for stuff like AdGuard and a couple of other things like Bastion, SSH host and that kind of stuff.
[1609.12 --> 1615.10]  But for the most part, I like to try and keep the host as clean as possible to minimize host reboots.
[1615.20 --> 1619.56]  Because, you know, when I reboot that server, it takes a lot of services out and it's a pain in the bum.
[1619.74 --> 1621.04]  So I'd rather not do that.
[1621.04 --> 1624.92]  And Proxmox, does it still give you a GUI to manage a Docker container pretty well?
[1625.00 --> 1626.80]  Like all that's just built into Proxmox?
[1627.04 --> 1627.82]  Not Docker, no.
[1627.88 --> 1629.76]  It does LXCs, but not Dockers.
[1630.10 --> 1634.04]  So did you get on the host, like command line and install Docker?
[1634.70 --> 1635.60]  SSH, yeah, yeah.
[1635.78 --> 1637.94]  I mean, so Proxmox is built on top of Debian.
[1638.32 --> 1643.96]  And actually the route that I went to install Proxmox was a naked Debian install.
[1644.12 --> 1648.08]  And then you can install the Proxmox packages and repos on top of that.
[1648.08 --> 1652.82]  So it's just, you know, vanilla Debian with the Proxmox kernel effectively.
[1653.30 --> 1657.88]  It's not like FreeNAS where you start mucking about on the host OS and you could really screw stuff up.
[1658.30 --> 1660.02]  That's what's always put me off on these appliances.
[1660.30 --> 1660.58]  You could.
[1660.70 --> 1661.64]  I mean, it's Linux.
[1661.92 --> 1664.18]  But Proxmox isn't an appliance.
[1664.36 --> 1665.50]  It's an abstraction layer.
[1665.50 --> 1674.04]  So they do weird stuff with like networking and they put all the VM configs in, you know, bespoke places that are unique to Proxmox.
[1674.22 --> 1678.26]  And that's probably my biggest issue with Proxmox as a project, to be honest, is it's slightly esoteric.
[1678.62 --> 1683.60]  But once you learn those little foibles, does the job.
[1684.22 --> 1685.24]  Yeah, it doesn't seem like it's too bad.
[1685.28 --> 1686.28]  And you were able to get it working.
[1686.88 --> 1690.84]  So you kind of have a real, I mean, a bit of a hodgepodge right now.
[1690.84 --> 1694.74]  Sounds like you got like three different servers running in your house right now.
[1694.74 --> 1695.30]  I did.
[1695.48 --> 1695.66]  Yeah.
[1695.82 --> 1701.98]  So I predicated all of my buying and purchase decisions around this Intel GVTG stuff actually working.
[1702.72 --> 1710.22]  And it was only once it had been in production for a couple of weeks, I sort of really realized that now this isn't this isn't going to be reliable enough.
[1710.52 --> 1713.70]  And I'm going to have to constantly keep poking and tending this thing.
[1714.48 --> 1724.54]  And so, yeah, going back to the HP290 as a Windows box, the i5-8500 based system with Pi KVM.
[1724.74 --> 1726.06]  I'm going to have to be able to use it as my server.
[1726.42 --> 1734.26]  And then I've got a Homelab box as well, which currently is the Dual Xeons, which I was running for the last two, three years with 128 gigs of RAM.
[1734.26 --> 1738.24]  And I'm going to use that as like a Homelab slash backup box.
[1738.44 --> 1741.08]  So I'll power it on minimum, I don't know, once a week, whatever.
[1741.78 --> 1746.94]  Have a couple of 10 terabyte hard drives in there and mirror my ZFS array with ZFS send or whatever.
[1746.94 --> 1750.98]  And then that'll be my on-site backup, effectively.
[1751.32 --> 1764.34]  But what I'm thinking is that those Dual Xeons are massive overkill for running OpenShift in my context of developing infrastructure at work, which is its primary use case.
[1765.22 --> 1769.02]  And so I'm thinking maybe I could get away with a knock or two for that role.
[1769.02 --> 1772.98]  Or maybe I should just stop spending money and just use what I've got.
[1773.48 --> 1778.46]  Well, I think clearly you just haven't gotten the Pi religion enough because that just sounds like great uses for a bunch of Pis.
[1779.22 --> 1779.92]  Oh, yeah.
[1780.32 --> 1781.88]  Because you also have a Pi running now.
[1781.98 --> 1783.16]  You now have a Pi running with Home Assistant.
[1783.26 --> 1784.42]  So it is several systems.
[1784.42 --> 1785.86]  Yeah, I think so.
[1785.98 --> 1789.42]  I probably will take Home Assistant off the Pi.
[1790.28 --> 1794.14]  I'll probably put it back on Proxmox because I've got NVMA storage in there.
[1794.34 --> 1801.02]  It's going to be more performant than the Pi, particularly when you're loading lots of plugins like VS Code and the heavier stuff like Node.red.
[1801.40 --> 1803.30]  You do notice a difference there.
[1803.78 --> 1805.34]  Yeah, or snapshots or updates.
[1805.62 --> 1807.54]  Yeah, updates for sure.
[1808.02 --> 1810.92]  It takes 10 or 15 minutes instead of five.
[1810.92 --> 1815.04]  So, yeah, you do notice it's a less powerful system.
[1815.32 --> 1822.44]  But in terms of just day-to-day functionality of controlling your devices and automations, it does do the job just fine.
[1822.64 --> 1827.58]  Well, that's the thing about an automation, right, is it just happens without me knowing how long it takes.
[1827.82 --> 1831.74]  And if it takes eight milliseconds instead of four, I don't really care.
[1832.72 --> 1839.74]  No, and for me, in my particular use case, because in 2021, I think I will be off-grid more than I ever have been.
[1839.74 --> 1841.22]  And power matters more than ever.
[1841.34 --> 1843.08]  I've actually been condensing down.
[1843.82 --> 1845.34]  I'm now down to just two Pis.
[1845.56 --> 1849.98]  And I'm going to try to condense down to maybe just one Pi or the Odroid item.
[1850.06 --> 1850.64]  I'm not sure yet.
[1850.98 --> 1853.68]  The Pi intervention that we staged appears to be working then.
[1854.08 --> 1854.56]  Yeah, it's funny.
[1854.62 --> 1856.98]  As I'm sort of scaling down, you're scaling up your Pi usage.
[1857.12 --> 1858.58]  I think you'll be on the show soon.
[1858.66 --> 1860.76]  Tell me about more Pi deployments you've done.
[1860.76 --> 1862.34]  You say that.
[1862.74 --> 1867.68]  But I was looking at the Odroid stuff, particularly after Home Assistant Blue came out.
[1867.78 --> 1869.50]  I was like, okay, well, this is the future of Home Assistant.
[1869.64 --> 1872.14]  I should just buy one of those and call it good.
[1872.30 --> 1874.08]  But they're $180.
[1876.08 --> 1877.16]  That's too much.
[1877.32 --> 1881.86]  Like compared to what you can buy as a used Dell or a used HP system,
[1882.58 --> 1886.90]  the HP 290 that's now running my Blue Iris was $140 shipped.
[1886.90 --> 1889.60]  And for that, I got a 500 gig hard drive.
[1889.96 --> 1896.70]  I got eight gigabytes of RAM and a QuickSync capable eighth gen Intel CPU with two PCIe slots.
[1897.02 --> 1898.88]  So I can add an NVMe drive.
[1899.16 --> 1900.02]  X86 compatibility.
[1900.46 --> 1902.02]  Yeah, and X86 as well.
[1902.46 --> 1906.44]  So I could add any eighth gen Intel CPU into there if, for whatever reason,
[1906.50 --> 1908.10]  the Celeron that's in there isn't good enough,
[1908.46 --> 1912.18]  which it is actually for the six cameras that I have with QuickSync.
[1912.74 --> 1914.82]  I could add an NVMe drive in there.
[1914.88 --> 1915.96]  I could add more RAM.
[1915.96 --> 1917.76]  I can do PCIe slots.
[1918.12 --> 1919.04]  And it was $140.
[1919.62 --> 1920.80]  It is too expensive then.
[1920.90 --> 1922.14]  The Eldroid is just too expensive.
[1922.28 --> 1925.74]  And it doesn't have the compatibility that the Raspberry Pi 4 does.
[1926.00 --> 1928.52]  I'm still feeling the pain from that Helios purchase.
[1928.92 --> 1929.12]  Yeah.
[1929.24 --> 1936.64]  I still feel really almost burned by that because I thought ARM would be better by now.
[1936.82 --> 1937.76]  It's just a struggle.
[1938.16 --> 1939.76]  Like whenever you're trying to do something,
[1939.76 --> 1947.52]  you'll always come across some edge case of the container you want to run doesn't have an image for the correct architecture.
[1948.08 --> 1953.34]  Or, you know, some package isn't built for ARM or it's not got QuickSync.
[1953.34 --> 1955.38]  I know I keep going on about QuickSync, but it is amazing.
[1956.34 --> 1970.64]  And for me, the price I pay of a few extra watts and a few extra liters of space in my house being used up is totally worth it for not having to futz around with ARM stuff for another year or two until it's ready.
[1970.64 --> 1974.06]  Yeah, I think that's a perfectly reasonable outlook.
[1974.52 --> 1975.96]  Even you make a good price argument.
[1976.34 --> 1984.56]  I think the reality is that if I could only choose between an x86 box or an Odroid type system for my home hosting,
[1984.76 --> 1987.38]  I would absolutely choose the x86 box every single time.
[1988.18 --> 1992.44]  There are kind of examples in the market, though, that show us where ARM is going.
[1992.74 --> 1994.92]  So I think this is going to be a solved problem.
[1995.20 --> 1999.10]  It really kind of demonstrates how it's all about implementation.
[1999.10 --> 2003.44]  You look at Apple with the M1, look what they're capable of doing with ARM,
[2003.78 --> 2010.16]  and then you look at, say, the Raspberry Pi Foundation and the different kind of scale of machines they can do with ARM
[2010.16 --> 2014.74]  and the ecosystem they've built around it now and the foundation that they have built around it.
[2015.34 --> 2019.66]  There are implementations that do it really well, and then their implementations are a little bit rough.
[2019.76 --> 2024.72]  And I think it's so nuanced, it's hard for consumers to understand the value differences there.
[2024.72 --> 2029.96]  And I think that's why you and I have been kind of chilling on this recently is because these are sort of the unspoken things
[2029.96 --> 2033.66]  that aren't necessarily specs that are bullet points on a web page.
[2033.74 --> 2037.54]  These are the more nuanced things that you learn over time when you use them in production.
[2038.28 --> 2039.22]  By using it, yeah.
[2039.72 --> 2045.84]  By trying to solve a particular problem and butting your head up against endless forum posts,
[2046.06 --> 2051.72]  or in some cases, because what you're trying to do, you might be the first trying to do it on ARM.
[2051.72 --> 2055.18]  There are no forum posts, and good luck to you, you know.
[2056.54 --> 2061.70]  Well, our friends at A Cloud Guru want you to know about their Linux networking and troubleshooting course this month.
[2062.14 --> 2067.04]  This is something you may want to look into if you need the fundamentals or want to know more about tools and techniques
[2067.04 --> 2072.02]  or use cases to configure, manage, and troubleshoot Linux in a networking context.
[2072.42 --> 2076.70]  By the end of their course, you'll feel comfortable in working with a large variety of networking tools
[2076.70 --> 2081.08]  and configurations to manage complex Linux networking implementations.
[2081.08 --> 2085.42]  It's at A Cloud Guru, and we will have a link in the show notes to go specifically to this course
[2085.42 --> 2087.36]  or go to acloudguru.com.
[2088.98 --> 2093.48]  Continuing talking about the pie, just to annoy that one specific Reddit commenter.
[2094.34 --> 2096.18]  I'm full troll mode today.
[2096.72 --> 2101.26]  We talked about backing up Home Assistant last time through a Google Drive plugin,
[2101.84 --> 2105.30]  and a little birdie tells me you tried it out at last.
[2105.78 --> 2107.20]  You talked me into it. You did.
[2107.30 --> 2107.68]  Hooray!
[2107.68 --> 2110.38]  You in the audience, we got a couple of emails in about it too.
[2110.58 --> 2113.74]  And so I finally gave this Google Drive backup a try.
[2113.90 --> 2115.92]  It's an add-on specifically for Home Assistant.
[2116.14 --> 2121.06]  And this is a good example of why it's kind of nice to have the full supervised Home Assistant setup
[2121.06 --> 2124.96]  is it's easy to add repositories for this kind of stuff, and you're off to the races.
[2125.70 --> 2128.70]  And what it lets me do, and if you're not familiar, we talked about it a little bit,
[2128.76 --> 2131.22]  is it lets you take your snapshots and send them up to Google Drive.
[2131.30 --> 2132.78]  Pretty simple. That's all it does.
[2132.78 --> 2139.44]  What I've learned now after using it for a little bit is it has a couple of nice built-in management features.
[2139.56 --> 2144.88]  It'll keep four snapshots locally, and by default it'll keep four snapshots in Google Drive,
[2144.96 --> 2146.94]  but that is totally configurable.
[2147.42 --> 2150.42]  You can also have it automatically create the snapshots for you,
[2150.56 --> 2154.68]  which is probably a feature I needed more than I realized.
[2154.68 --> 2160.54]  I was only doing snapshots right before major events, but if you think about it, it could break at any time.
[2161.08 --> 2161.86]  Something could die.
[2162.22 --> 2163.70]  You need stuff that's more current.
[2163.80 --> 2170.10]  So I set this every three days at 2 a.m. to take a snapshot and then upload it to Google Drive.
[2170.28 --> 2175.64]  And what I really was impressed by is how it displays what snapshots are local only,
[2175.74 --> 2179.60]  what snapshots are on Drive, and just really easy options to manage it.
[2179.92 --> 2183.84]  And as you would expect, it's stupid easy to connect it to your Google account.
[2183.84 --> 2188.20]  It just uses all of Google's authorization stuff where you go through all the standard Google login screens,
[2188.32 --> 2190.56]  and it's set up and you're off to the races.
[2190.64 --> 2192.04]  I can't believe how easy it was.
[2192.18 --> 2193.62]  And now it's just hands off.
[2194.02 --> 2195.94]  There's a little triangle as well that shows up to say,
[2196.18 --> 2200.20]  this snapshot will be deleted when I run the next backup set,
[2200.28 --> 2205.12]  just so that you know, oh, right, that's my weekly snapshot falling off the end of the conveyor belt.
[2205.30 --> 2208.06]  I like this pairing with Duplicati too.
[2208.18 --> 2211.18]  So this is how I'm still backing up any of my system level stuff.
[2211.18 --> 2213.70]  This has nothing to do with Raspberry Pi or Home Assistant.
[2213.82 --> 2216.90]  You could use this on any Linux box, and I really, really love it.
[2217.60 --> 2222.00]  Duplicati is what I use for off-siting my Docker Compose files,
[2222.12 --> 2225.02]  my configuration files in general, Etsy Config,
[2225.56 --> 2229.66]  any of those kinds of things that I think I would want to be able to restore
[2229.66 --> 2231.96]  if I were to reload a base system.
[2231.96 --> 2234.74]  I use Duplicati to off-site that system level stuff.
[2235.12 --> 2238.82]  So now I have this Home Assistant Google Drive paired for the snapshots,
[2239.04 --> 2243.14]  which is the application level stuff, and Duplicati for the system level stuff.
[2243.42 --> 2247.30]  And I feel like I probably have my backup more dialed in than I ever have right now.
[2247.74 --> 2252.04]  Are you not ever tempted to use, you know, Git to manage your config files?
[2252.10 --> 2253.24]  Because they are just text files.
[2253.70 --> 2257.34]  You've put that seed in my mind a little while ago, and I have been considering it.
[2257.34 --> 2262.10]  It's mostly just taking the time to set it up and bother.
[2262.68 --> 2266.36]  Because what I have now kind of works, so I don't have like an impetus to replace it.
[2266.62 --> 2270.02]  But I know I probably should replace it before I have that impetus.
[2271.10 --> 2278.22]  I'm reminded of a conversation I had at my first developer job with one of the senior architects.
[2278.50 --> 2283.04]  I came in fresh out of my computer science degree.
[2283.42 --> 2284.06]  Just a lad.
[2284.40 --> 2284.68]  Yeah.
[2285.22 --> 2286.90]  Saying, well, why don't we just rewrite this?
[2286.90 --> 2287.90]  Why don't we just rewrite that?
[2288.00 --> 2288.72]  I mean, this is stupid.
[2288.82 --> 2289.46]  This is really old.
[2289.54 --> 2290.98]  Why are we still running Java 5?
[2291.12 --> 2291.98]  And blah, blah, blah, blah, blah, blah.
[2292.68 --> 2295.30]  And he sort of sat me down, and it was over like lunch break.
[2295.34 --> 2297.04]  It wasn't like a super formal thing.
[2297.10 --> 2301.90]  But he was like, well, what you've got to realize, Alex, is that when you rewrite code,
[2302.34 --> 2304.42]  obviously there's a cost to rewriting the code.
[2305.26 --> 2307.04]  Someone has to pay that bill.
[2307.72 --> 2311.04]  The business, in air quotes, the business has to pay that bill.
[2311.04 --> 2318.18]  Some product manager somewhere has to sign off product owner and say, yes, I'm going to pay for this out of my budget and do that.
[2318.98 --> 2319.32]  All right.
[2319.40 --> 2320.12]  Okay, cool.
[2321.16 --> 2322.86]  What's the spec going to be?
[2323.38 --> 2325.64]  Well, at a minimum, it's got to be what it already does.
[2325.64 --> 2330.48]  But what the product owner is looking for is something extra.
[2330.72 --> 2338.06]  They want to add a new type of credit card that they can accept, or they want to add a new feature, whatever it might be.
[2338.06 --> 2354.10]  And so the bill for them to add a new feature to the existing pile of crap that's already there is, you know, 5% versus 105% of rewriting the entire code base, which could take multiple years.
[2354.78 --> 2362.56]  During which time, you still have to innovate to keep ahead of your competition and patch and write code for the old code base.
[2362.56 --> 2379.22]  And you're just like, oh, yeah, now I see why massive enterprises have code bases that are 30, 40 years old that people are scared to touch because what they have just works and is a stinking cash cow.
[2379.40 --> 2381.26]  So the spec is the code.
[2381.32 --> 2382.16]  The code is the spec.
[2382.36 --> 2384.40]  Why would anybody fit?
[2384.54 --> 2390.18]  If it ain't broke, don't fix it or just keep fixing the minimum viable fixes, you know?
[2390.18 --> 2393.76]  What you call technical debt, they call an investment.
[2394.96 --> 2396.02]  It's very true.
[2396.38 --> 2397.22]  It's very true.
[2397.76 --> 2401.78]  Yeah, I've very much had that same arc over my career.
[2401.94 --> 2404.72]  I was the bull in the china shop.
[2404.76 --> 2407.98]  Let's come in and tear it all down and replace it with the new stuff guy.
[2409.00 --> 2413.34]  And towards the end, I was the guy being like, well, let's not replace it.
[2413.40 --> 2414.72]  Let's build on what we've got.
[2414.72 --> 2417.88]  But I feel like in some ways, you know, you learn how to do things better.
[2418.10 --> 2420.32]  And by the end, you should be able to build on what you've done.
[2420.98 --> 2423.00]  But software is tricky like that.
[2423.32 --> 2424.64]  Sometimes it is better just to restart.
[2424.80 --> 2426.78]  And we see it a lot with the projects we use to self-host.
[2426.88 --> 2433.90]  You'll see them either fork or you'll see them just sort of reboot completely with a little bit less features because that's the only way they could get it out the door.
[2434.74 --> 2436.40]  Well, we're just about done, I think.
[2436.70 --> 2438.24]  But we have more in the post show.
[2438.36 --> 2440.30]  If you are a member, you get a little extra show.
[2440.30 --> 2444.24]  You can go to self-hosted.show slash SRE if you'd like to become one.
[2444.64 --> 2449.24]  Not only do you support the show, but you do get a limited ad feed and that extra content out there.
[2449.86 --> 2452.36]  As always, you can go to self-hosted.show slash contact.
[2452.66 --> 2454.34]  That's the place to go to get in touch with us.
[2454.44 --> 2456.54]  And you can find me on Twitter at Ironic Badger.
[2456.94 --> 2458.60]  I'm there too at Chris LAS.
[2458.68 --> 2460.70]  And the show is at self-hosted show.
[2461.06 --> 2462.88]  Don't forget the network at Jupiter Signal.
[2463.14 --> 2465.74]  And that was self-hosted.show slash 38.
