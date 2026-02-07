[0.00 --> 3.30]  1.41 is going to kick off with some follow-up from our previous episode.
[3.40 --> 7.44]  We talked about NetData, and I still really like NetData,
[7.52 --> 12.48]  but Alex, I don't know if you saw, in the last week since our previous episode,
[12.82 --> 20.02]  it's come to light that NetData is now limiting how many nodes can be in your local dashboard to five.
[20.46 --> 20.82]  Oh, really?
[21.34 --> 23.60]  Yeah, and you've got to use the cloud product if you want more than that.
[23.60 --> 26.64]  Oh, well, we're going to get into some proper n-tification stuff later,
[26.64 --> 30.00]  but this sounds of a similar vein, no?
[30.74 --> 36.04]  And it was a feature change, quote-unquote, that was supposed to happen in August,
[36.22 --> 39.12]  if I'm reading the thread right, but a bug prevented it.
[40.12 --> 45.38]  And so they fixed that bug since our last episode, and now it's limiting the nodes.
[45.56 --> 50.14]  And I don't know, I like NetData, it's a good project, I still have it installed on several systems,
[50.98 --> 54.50]  but I'm wondering if 2025 is kind of the beginning of my breakup.
[54.50 --> 55.74]  It's heavyweight, though.
[56.64 --> 57.46]  It's really heavy.
[57.82 --> 59.34]  Yeah, it's relative.
[59.82 --> 64.28]  You know, there's other tools that are even heavier, but like we talked about in episode 140,
[64.88 --> 66.38]  there's also lighter tools you can use.
[66.70 --> 69.74]  Yeah, that bezel one seems to be quite popular these days.
[70.10 --> 74.56]  So, I mean, the downside of that is it doesn't give you anywhere near the level of insight,
[74.60 --> 75.92]  I mean, you know, pros and cons,
[76.26 --> 79.94]  it doesn't give you anywhere near the level of insight that you get with NetData.
[79.94 --> 84.20]  I just love stuff like looking at my ZFS arc, for example.
[84.36 --> 86.32]  It's like right there in NetData, boom.
[86.70 --> 92.26]  I can see exactly which disk is busy, which, you know, and it's all nicely laid out.
[92.54 --> 98.08]  And I understand, you know, companies like this got to make money, but I don't know,
[98.08 --> 103.96]  it feels kind of like forgetting who put you where you are, like, in these moments, no?
[104.46 --> 106.56]  Yeah, or what was your special value prop?
[106.64 --> 107.72]  Like, what made you great?
[107.82 --> 110.18]  What brought you to greatness?
[110.18 --> 114.52]  And they, or it's exactly what, they know exactly what it is,
[114.56 --> 117.44]  and that's how they figure out how to monetize it, which is even more cynical.
[118.24 --> 122.52]  Similar thing with VMware and, well, since Broadcom bought them anyway,
[122.60 --> 128.96]  it's like there's tens of thousands of small to medium shops out there with VMware-based tooling,
[128.96 --> 136.50]  and all of the sysadmins that get trained on those tools feed then into that top 10% of customers
[136.50 --> 141.16]  that make 90% of the money for Broadcom VMware.
[141.96 --> 144.74]  And without that kind of pool of talent to pick from,
[144.80 --> 149.26]  it becomes a very different proposition for CISOs to pick what they're going to do moving forward.
[149.36 --> 154.16]  And I think, you know, NetData is kind of beginning the slide of that same playbook here.
[155.00 --> 155.40]  I think so.
[156.40 --> 156.88]  I think so.
[156.92 --> 158.46]  Well, let's talk about something more positive.
[158.80 --> 159.14]  Yeah, okay.
[159.22 --> 162.80]  So this week I found a cool little tool called Tiny Feed.
[162.80 --> 170.46]  This allows you to generate a static HTML page from a collection of feeds using nothing but a simple CLI tool.
[170.96 --> 172.76]  This is so slick.
[173.08 --> 177.42]  I've been aware of this, love this tool, and I never have an excuse to use it.
[177.48 --> 179.46]  And the output, by the way, that it creates is beautiful.
[179.60 --> 181.64]  I'm wondering what are you using Tiny Feed for?
[182.20 --> 184.70]  I'm not, but I kind of want to for something.
[184.94 --> 187.20]  It's one of those things like a show research pops up.
[187.20 --> 193.10]  It's a case of looking at just trying to simplify my digital life.
[193.34 --> 196.86]  Like, I've cut Reddit out pretty much completely.
[197.24 --> 202.30]  And I still find myself reaching for my phone and thinking, I'm going to open it.
[202.34 --> 202.92]  I'm going to unlock it.
[202.94 --> 204.64]  I'm going to do something with it.
[204.70 --> 207.88]  And I've got a couple of RSS feeds and things like that in there.
[207.88 --> 212.78]  And the trouble with RSS readers is they're only as good as their inputs.
[213.10 --> 218.98]  And I know that's going to be true of this too, but I just don't have the same...
[218.98 --> 225.00]  I suppose what I'm trying to say here is actually that I kind of miss an algorithm serving me up stuff.
[225.86 --> 225.90]  Hmm.
[226.06 --> 227.78]  Yeah, I do follow what you mean there.
[227.90 --> 234.38]  I like the idea, though, of kind of having more control over the information diet and being more selective.
[234.38 --> 237.70]  And then branching out from there if you need to.
[237.88 --> 242.08]  And since this is a command line app, it's real simple to set up a cron job.
[242.14 --> 244.38]  And I'm just thinking, how popular are dashboards?
[244.50 --> 247.32]  Well, what if this was your dashboard of sense?
[247.72 --> 251.70]  Like, you open up your web browser and it loads this, and maybe it runs every five minutes.
[252.36 --> 259.50]  And it's pre-selected information sources that don't get you triggered or aren't talking about stuff you don't care about.
[259.62 --> 262.26]  And it's just sort of like Alex's news feed.
[262.26 --> 265.36]  And if you need more than that, then you fire up the social media app.
[266.10 --> 267.60]  No Elon Musk allowed.
[268.20 --> 269.22]  There you go, right?
[269.30 --> 271.48]  In your social media stream, there's no Elon.
[272.14 --> 281.26]  So what occurs to me, actually, as you're talking, is what would be kind of cool is one of the reasons I keep coming back to Hacker News is it's a fairly well curated,
[281.98 --> 287.88]  although it's maybe arguably not as curated as it used to be, just series of text links.
[287.90 --> 290.44]  And then I get to choose based on the words, not even any pictures.
[290.44 --> 291.66]  I like that simplicity.
[292.50 --> 300.30]  If we could kind of combine that with the blue sky feature of kind of like starter packs or whatever they have over there.
[300.30 --> 310.62]  I'm just imagining a world where we as a self-hosted podcast community come together and build a bunch of RSS starter packs for people of,
[311.04 --> 314.76]  well, here's the 50 or so blogs that I've picked out over the last decade.
[315.44 --> 321.06]  And someone, you know, like Orange One on Discord or something comes along with his 50 top 50 picks or whatever.
[321.06 --> 326.30]  And before we know it, we've got a starter pack of a thousand blogs all related to self-hosting and that kind of thing.
[326.50 --> 328.96]  And then we feed it into a tool like Tiny Feed.
[329.08 --> 332.22]  And then we just put it, you know, feed.selfhosted.show or something.
[332.78 --> 333.04]  Yeah.
[333.28 --> 336.46]  If that's of interest to you, write in and let us know and we'll build it.
[336.56 --> 337.28]  That sounds kind of fun.
[337.66 --> 339.96]  Now, I feel like the community in general could do more with RSS.
[339.96 --> 348.22]  RSS is such a great tool and so many services and sites have an RSS feed and so few things are done with it.
[348.72 --> 348.80]  Yeah.
[348.92 --> 351.38]  Let's see an RSS renaissance.
[353.72 --> 354.20]  Yeah.
[354.32 --> 357.76]  And the funny thing about that is renaissance contains RSS.
[357.90 --> 358.40]  I know.
[358.56 --> 359.22]  It's great.
[359.62 --> 360.18]  Look at that.
[361.60 --> 367.82]  In the news feeds this week was OpenZFS, as you would say, 2.3.
[367.82 --> 372.40]  And I get the vibe that this is kind of a big deal release.
[373.58 --> 379.80]  Well, how long have we been waiting for OpenZFS to add RAID-Z expansion?
[380.30 --> 382.80]  I mean, technically, since 1.0.
[383.70 --> 384.06]  Technically.
[384.42 --> 386.40]  It's been a very, very long time.
[386.52 --> 387.42]  Yeah, it has.
[387.72 --> 390.84]  So RAID-Z expansion kind of does what it says on the tin.
[390.94 --> 395.62]  It allows you to add extra drives to an existing RAID-Z VDEV.
[395.62 --> 396.96]  Caveat.
[397.28 --> 399.86]  It will not work unless it is a RAID-Z.
[400.22 --> 403.46]  I went to Perplexity and asked it, how do I do this with a mirror?
[404.24 --> 407.70]  Very quickly find out that that's not, Alex, that's not a RAID-Z.
[407.84 --> 408.38]  That's a mirror.
[408.76 --> 410.98]  So it's got to be a RAID-Z grouping.
[411.60 --> 417.38]  And then it will do the data reflowing and allow you to add an extra disk to an existing VDEV.
[417.38 --> 425.16]  Yes, and the expansion process can pause if a disk fails and will resume if you recover the disk.
[425.28 --> 428.70]  So that was the first thing I was wondering is what happens if a disk fails during this process.
[428.78 --> 429.82]  Yes, they've thought of that.
[430.70 --> 432.42]  Of course, there's things you need.
[432.54 --> 437.66]  You're going to have to turn on specific disk flags, and those are not going to be backwards compatible with previous versions of ZFS.
[437.66 --> 441.72]  So that's something to keep in mind if you're moving to an older server at some point, but probably not likely.
[442.48 --> 453.36]  There's a bunch of technical details that if you want to get into the nitty-gritty, there's a fantastic video on YouTube from Matt Arens, who's one of the ZFS developers,
[453.82 --> 462.42]  talking about how they're moving all the blocks around and making this happen and all of the stuff they're doing with, you know, stripe width and data-to-parity ratios and all that kind of stuff.
[462.42 --> 472.08]  I won't get into that here because it's extremely technical and very dry, but it's just a great option to make ZFS more flexible for home users.
[472.34 --> 487.30]  I'm not sure I'd rely on it in a production setting, but honestly, if you're using ZFS in that kind of a setting where you are buying half a dozen drives or more at a time to build an entire new pool when you need to expand,
[487.30 --> 493.50]  you're not who this is targeted at anyway. This is targeted at you and me of the world that just want to buy,
[493.86 --> 499.46]  we want to go to Best Buy and buy a drive that's on sale right now and just throw it into our array and kind of, you know,
[499.50 --> 506.04]  it's a sticking plaster over the, it's always a bit of flex tape over my pool being full.
[506.28 --> 512.32]  That's who it's aimed at. And, you know, the hex OSs of this world who are looking to make things more approachable,
[512.68 --> 514.36]  make ZFS more approachable for the masses.
[514.36 --> 522.78]  And I think it's just really nice to see because ZFS is such a powerful file system and this really rounds out the feature set to something like,
[523.06 --> 528.94]  I think perhaps people listening that aren't super familiar with ZFS might have expected this just to already have existed.
[529.24 --> 531.78]  So it is really good to see this land in here.
[532.26 --> 537.52]  Now, Alex, you and I are both very happy Jellyfin users, been rocking Jellyfin for a while now,
[537.64 --> 542.30]  but there was some information that came out that seems to be good news for Plex users.
[542.30 --> 547.80]  And in this story, I discovered something interesting about the Plex media server.
[548.26 --> 552.16]  This is from a Plex employee on Reddit, and this was from a little while ago.
[552.26 --> 552.52]  They wrote,
[552.52 --> 557.74]  The Plex media server was originally designed only to transcribe H.264.
[558.56 --> 564.34]  And they had to shoehorn HVAC support in there, and they've been refactoring it now for a while to try to make it work on other systems.
[564.48 --> 573.54]  I didn't, I guess I hadn't thought about it really, but I didn't really think that the media server would be designed for only one codex.
[573.60 --> 577.94]  See, this is where Jellyfin sort of has an advantage because they outsource that to FFmpeg.
[577.94 --> 582.20]  Right. I mean, doesn't Plex outsource it to FFmpeg?
[582.42 --> 587.60]  Well, that's what I thought, but maybe it's their own fork or something here because this was, I was surprised,
[587.68 --> 592.56]  and they said it was much easier to add AV1 support, but HVAC support has been a real challenge.
[592.80 --> 598.82]  I wonder why. Maybe it's to do with different licensing aspects or some technical thing.
[598.82 --> 602.78]  I got the impression from the post on Reddit, which we'll have a link in the show notes.
[602.98 --> 604.82]  This is from a little bit ago, so I know they've been working on it.
[605.30 --> 609.26]  I got the impression it was just technically difficult because of the way they designed PMS.
[610.22 --> 610.92]  Oh, interesting.
[611.66 --> 618.68]  I think it probably comes down to licensing for the X.265 stuff in software versus hardware.
[618.68 --> 628.74]  And I think the big news coming out of Plex this week in regards to HEVC encoding is that it's QuickSync-based HEVC encoding that's coming to Plex.
[629.06 --> 633.24]  Right. They had to make some real big changes to make this work, so it's cool to see.
[633.68 --> 639.36]  Absolutely, yeah. And I'm going to assume that Jellyfin will follow soon if they don't already support it.
[639.80 --> 643.10]  Do you have any H.265 content on your system?
[643.70 --> 646.06]  You know, this is a funny admission.
[646.06 --> 655.14]  This is story time. So, you know, I rebuilt my media server in the middle of last year to a 13th gen Intel system, and I switched to Nix OS in the process.
[655.84 --> 655.98]  Yeah.
[656.96 --> 665.14]  Well, little one today was like, because it snowed outside overnight here in Raleigh.
[665.32 --> 668.90]  And New Orleans got like 10 inches of snow yesterday. We only got one inch.
[669.08 --> 671.14]  So, I mean, New Orleans is hoarding all the snow.
[671.58 --> 673.84]  We got an inch. We got to do some sledging this morning. It was all fine.
[673.84 --> 678.42]  But afterwards, obviously, it snowed. She's like, can we watch a Christmas movie?
[678.60 --> 681.78]  Because school's out for the day because of an inch of snow shuts down the state.
[682.36 --> 683.86]  Right. And when you see snow, you think Christmas.
[684.12 --> 694.26]  Yeah. So we watched the Grinch movie, and it turns out that that is a 4K HDR10 file that I have for the animated one from, I think, 2016 or so.
[694.26 --> 697.64]  So it's actually a really great movie, by the way, for kids.
[697.88 --> 701.46]  You know, it's in the same sort of style as like the Lorax or something like that.
[701.54 --> 703.10]  Really bright colors and all that.
[703.20 --> 705.48]  Anyway, it's not a movie review show.
[706.06 --> 711.66]  Turns out when I press play on that file, there was like a 15 second pause before it started playing.
[711.74 --> 713.16]  And I'm like, what's going on?
[713.16 --> 714.38]  What the deuce is going on?
[714.64 --> 714.82]  Yeah.
[714.82 --> 717.48]  So I opened up the terminal because I had my laptop on my knee.
[717.74 --> 718.12]  Of course.
[718.28 --> 723.04]  And I was like, oh, my server's drawing 300 watts right now.
[723.18 --> 724.52]  What is going on?
[725.04 --> 726.00]  CPU's doing the load.
[726.26 --> 726.90]  Yeah, exactly.
[727.14 --> 731.58]  Normally, it draws like 100, you know, in sort of idle-ish standby mode.
[731.58 --> 744.52]  So it turns out that my Supermicro motherboard that I bought like nine months ago, I haven't had any hardware transcoding for like nine months.
[744.56 --> 746.00]  And I haven't noticed until today.
[747.38 --> 750.46]  And I feel like a chump, honestly.
[750.98 --> 751.94]  I mean, if it's working, though.
[752.00 --> 754.16]  I mean, I know it uses more power, but it's working for you.
[754.42 --> 757.92]  And the software encoding is probably better quality and all that, you know.
[757.92 --> 762.04]  So and ideally, maybe the set-top box is playing it direct in most cases.
[762.70 --> 762.80]  Yeah.
[762.88 --> 768.06]  Well, this was an NVIDIA Shield plugged into a cheap like $300 Roku TV.
[768.34 --> 771.42]  So I think it does HDR, but not HDR10.
[771.54 --> 775.70]  So it had to transcode it, whereas my OLED upstairs, it can play it just fine.
[775.74 --> 776.92]  So maybe that's why I haven't noticed.
[776.92 --> 780.74]  I have the same exact problem on my living room TV versus the bedroom TV.
[781.36 --> 781.46]  Yeah.
[781.56 --> 787.90]  So I don't know what I'm going to do because the Supermicro motherboard kind of shares the video output with the Intel GPU.
[787.92 --> 789.04]  It kind of hogs it.
[789.10 --> 792.54]  I had the same problem with my ASRock board on the 8th gen stuff.
[792.70 --> 797.04]  So I needed to wait until a little one was in bed, probably after we finished recording, to be honest,
[797.40 --> 804.70]  before I could take Plex offline for long enough to actually do some maintenance on the thing without causing a ruckus, you know.
[805.16 --> 805.98]  Taking a look around.
[806.54 --> 809.38]  Yeah, I do love the file savings.
[809.38 --> 822.36]  So especially if they're not HDR, if they're just like a television episode that you're backing up and if you go to H.265, a 700 megabyte, 800 megabyte episode can now be 380 megabytes.
[822.72 --> 823.90]  So that's great.
[824.16 --> 827.24]  Especially for me when, yeah, my home media storage is all on SSD.
[827.62 --> 830.06]  So I'll take the savings.
[830.06 --> 836.86]  I know some people run their libraries through TDAR and that kind of thing to reduce the amount of space on disk.
[837.44 --> 839.40]  And the savings can be really quite considerable.
[839.68 --> 845.10]  But what I would probably consider doing instead is rather than re-encoding and encode,
[845.10 --> 854.22]  if you can just put the correct keywords into your indexer or whatever you use and download the pre-encoded version from wherever.
[855.14 --> 856.38]  That's probably the way to go.
[857.06 --> 859.54]  Not that, of course, Linux ISOs are encoded.
[859.78 --> 860.90]  I don't know what we're talking about here.
[863.48 --> 865.96]  Tailscale.com slash self-hosted.
[866.18 --> 871.98]  Tailscale is the easiest way to connect your devices and services to each other wherever they are.
[871.98 --> 876.48]  It is modern networking for connecting your devices securely to each other.
[876.80 --> 879.40]  It's great for companies and it is great for self-hosters.
[879.88 --> 885.24]  Secure remote access to your production systems, your LAN, your databases, whatever it might be.
[885.30 --> 886.42]  And it is fast.
[886.86 --> 888.06]  Really, really fast.
[888.30 --> 891.50]  And it's privacy for every individual and every organization.
[892.16 --> 899.32]  It's intuitive to use and it's also advanced with features like programmable ACLs and other ways to manage your Tailscale system,
[899.32 --> 902.82]  including tying it into your existing authentication and tooling infrastructure.
[903.30 --> 904.26]  They have a personal plan.
[904.34 --> 910.30]  So when you go to tailscale.com slash self-hosted, you get 100 devices for free forever for up to three accounts.
[910.52 --> 912.26]  That's a great way to kick the tires.
[912.70 --> 913.60]  See what I'm talking about.
[913.66 --> 914.88]  No credit card required.
[915.30 --> 918.50]  The 100 user plan has been all I've ever needed for my personal account.
[918.50 --> 924.38]  Now, after using it for a couple of years in my personal account, we're using it as back-end infrastructure for Jupyter Broadcasting as well.
[924.76 --> 930.02]  Thousands of other companies like Instacart, Hugging Face, Duolingo, and others have switched to Tailscale.
[930.36 --> 933.98]  Go see how easy it is to set up and why I rave about it all the time.
[934.08 --> 937.04]  I have no inbound ports on any of my firewalls anymore.
[937.16 --> 940.20]  Try it out for yourself or for your business and support the show.
[940.52 --> 942.84]  Go to tailscale.com slash self-hosted.
[942.90 --> 943.06]  Yep.
[943.56 --> 944.14]  It's easy.
[944.28 --> 945.18]  You get 100 devices.
[945.28 --> 946.08]  No credit card required.
[946.08 --> 949.28]  It's tailscale.com slash self-hosted.
[950.60 --> 953.62]  Well, let's talk about something that seems to have people upset.
[954.18 --> 960.58]  And I'm a little disappointed because I was beginning to circle the sales funnel around Bamboo.
[960.80 --> 963.54]  Kind of encouraged by you, and I've been thinking more and more.
[963.60 --> 968.64]  If I do get into it, I want something as close to the Star Trek replicator as possible because I have limited time.
[969.06 --> 971.40]  But my roll has been slowed, Alex.
[971.40 --> 977.54]  Bamboo Labs this week appear to be speed running the n***ification process for 3D printing.
[978.38 --> 989.02]  On January the 16th, Bamboo Labs announced a ton of information about new authorization systems for their 3D printers in the name of security.
[989.66 --> 990.92]  Won't somebody think of the children?
[990.92 --> 1005.56]  Quote, as part of our ongoing commitment to enhance the overall security of our products, we are introducing an authorization and authentication protection mechanism for the connection and control of Bamboo Lab 3D printers.
[1005.74 --> 1006.84]  This is a good thing, right?
[1007.88 --> 1008.36]  Yeah.
[1008.74 --> 1011.24]  One would read that and think, okay, this is a good thing.
[1011.30 --> 1013.98]  It sounds like an Apple-esque explanation for a crackdown, though.
[1013.98 --> 1015.48]  Well, we've heard this before.
[1015.90 --> 1027.00]  And it's funny, you know, it's funny you mention Apple right off the bat because Bamboo Labs have a bit of a reputation for being the Apple of the 3D printing world.
[1027.14 --> 1028.68]  It's a bit of a closed ecosystem.
[1028.94 --> 1032.64]  Like, all of the parts that go into their printers are proprietary.
[1033.16 --> 1034.82]  All of the firmware is proprietary.
[1034.82 --> 1038.26]  And, I mean, there's a lot of parallels with Apple.
[1038.50 --> 1040.74]  Like, it's our way or no way.
[1041.52 --> 1046.12]  But that's not the way 3D printing as a community has come into the world.
[1046.20 --> 1048.50]  It's been a very open, a very collaborative thing.
[1049.08 --> 1053.34]  I mean, Prusa have really been hurting as a result of Bamboo Labs' dominance lately.
[1053.88 --> 1061.22]  Prusa, unfortunately, are responding to that by walking back some of their open source principles a little bit in their upcoming printers.
[1061.36 --> 1063.38]  But we'll get to that probably another day.
[1063.38 --> 1077.38]  So, as part of this Bamboo Labs announcement, this authentication and authorization layer affects not only their cloud-based mechanisms, but also machines that are in what's called LAN-only mode.
[1077.80 --> 1078.02]  Okay.
[1078.16 --> 1082.52]  Now, LAN-only mode would make me think of something that doesn't communicate to the Internet at all.
[1083.26 --> 1090.78]  So, then I would expect all functionality that would require the Internet to be broken, but things like cameras and other things to work.
[1091.24 --> 1092.72]  Oh, Chris, you silly sausage.
[1092.72 --> 1093.04]  No?
[1093.04 --> 1094.14]  No, no, no, darling.
[1094.54 --> 1098.80]  The following operations will require these new authentication controls.
[1099.32 --> 1102.38]  Binding and unbinding a printer from Bamboo Lab services.
[1102.90 --> 1103.12]  Okay.
[1103.76 --> 1105.44]  That one actually seems fine.
[1106.24 --> 1110.78]  Initiating remote video of the webcam that's inside the printer inside your house.
[1111.10 --> 1113.94]  Needs to go through the cloud for some reason.
[1114.90 --> 1115.82]  Firmer updates.
[1116.30 --> 1116.64]  Okay.
[1116.86 --> 1117.82]  I can kind of understand.
[1118.00 --> 1119.98]  You know, you don't want to have unsigned firmer updates.
[1120.48 --> 1120.88]  Fine.
[1120.88 --> 1122.06]  That one I kind of understand.
[1123.10 --> 1124.66]  Initiating a print job.
[1125.38 --> 1127.42]  Whether you're in LAN or cloud mode.
[1127.50 --> 1128.22]  So, yes, that's right.
[1128.22 --> 1134.22]  Your LAN mode printer needs to authenticate with the cloud to start a print.
[1134.22 --> 1136.26]  Yeah, that doesn't sound like LAN mode.
[1136.56 --> 1136.84]  No.
[1137.48 --> 1140.72]  And then a bunch of other stuff like controlling motion and other core systems.
[1141.22 --> 1143.94]  Here's a list of the things that don't require authentication.
[1144.60 --> 1145.76]  It's quite short.
[1146.82 --> 1149.00]  Status updates via MQTT.
[1149.00 --> 1156.36]  So, this allows Home Assistant or other things that speak MQTT to hook into the Bamboo printer and get status updates.
[1156.46 --> 1157.46]  Like read-only stuff.
[1157.96 --> 1161.34]  And starting prints from the SD card only.
[1162.00 --> 1166.68]  So, basically anything that requires write access must go through Bamboo.
[1167.10 --> 1168.02]  Anything that doesn't.
[1168.56 --> 1169.58]  Like read-only stuff.
[1169.76 --> 1170.44]  Status updates.
[1170.44 --> 1172.26]  You can just.
[1172.56 --> 1175.04]  You don't need to authenticate to get that information.
[1176.40 --> 1184.30]  And the reason this is a big deal is because this locks out a lot of the ecosystem that's kind of sprung up around Bamboo printers from the community.
[1184.30 --> 1191.12]  Things like the Panda Touch, which is a small little touchscreen device that you can put on the front of your Bamboo.
[1191.60 --> 1194.86]  The cheaper Bamboo printers that don't ship with color touchscreens.
[1195.44 --> 1199.04]  That hook into some of these APIs and some of these things that are available now.
[1200.20 --> 1204.20]  It feels to me like Bamboo are trying to funnel people towards their top-end printers.
[1204.42 --> 1208.66]  So, if you're not familiar with the Bamboo lineup, they've got the X1 Carbon at the top.
[1208.74 --> 1213.30]  It's like the Halo printer, which is about $12, $13, $1400, something like that.
[1213.30 --> 1217.64]  And then there's a sliding scale all the way down to the A1 Mini.
[1218.26 --> 1222.16]  And that's about a $200-ish printer, I think.
[1222.78 --> 1226.50]  And there's printers at every single sort of $100 or $200 price point in between.
[1227.28 --> 1232.18]  And they take away features like frame rates on cameras and touchscreens and all, you know.
[1232.30 --> 1237.20]  We've seen it a million times with Apple where they drip-feed features just to get you over the line of,
[1237.32 --> 1239.26]  oh, it's only $200 to the next tier.
[1239.54 --> 1241.18]  I'll just buy the next one up, you know.
[1241.18 --> 1250.42]  And I think things like Panda Touch came along and enabled people to put open-source touchscreens on the cheaper printers.
[1251.42 --> 1257.62]  And if I was in Bamboo corporate, I'd be like, hmm, you know, putting my conspiracy hat on here.
[1258.28 --> 1260.60]  What can we do to lock people out of doing that?
[1260.60 --> 1266.46]  So they have to walk our SKU tree to find the color touchscreen they want.
[1266.58 --> 1267.12]  Ah, I know.
[1267.16 --> 1268.78]  We can lock down the API access.
[1269.68 --> 1271.86]  And, of course, this is the first kind of thing they go after.
[1271.94 --> 1273.28]  And who uses this kind of stuff?
[1273.90 --> 1275.32]  The most passionate folks.
[1275.60 --> 1278.30]  The folks that couldn't afford the more high-end gear.
[1279.60 --> 1280.32]  You know, ugh.
[1280.32 --> 1291.26]  It also locks out things like Orca Slicer, which is, well, the slicer is the piece of software that takes your model file and creates the G-code that the printer executes.
[1291.42 --> 1293.18]  So it's what does the conversion.
[1293.30 --> 1299.64]  And a lot of people use a program called Orca Slicer instead of the Bamboo official slicer called Bamboo Slicer.
[1299.64 --> 1308.78]  Both of these things, or many of these other third-party things, rely on a network plugin using network plugin APIs for third-party authentication, that kind of stuff.
[1309.30 --> 1313.52]  And these are all just going to be completely locked out with this new update.
[1314.30 --> 1315.52]  Are they not making money, Alex?
[1315.56 --> 1316.10]  Are they struggling?
[1316.86 --> 1317.22]  I don't know.
[1317.28 --> 1321.34]  There's a lot of rumors swirling around about their backing from the CCP.
[1321.84 --> 1324.04]  I don't know what the truth of that kind of thing is.
[1324.22 --> 1328.36]  You know, it's a Chinese company, so the details are thin on the ground at best.
[1328.36 --> 1331.86]  So anything I do say here would just be pure speculation.
[1332.14 --> 1345.16]  But I think they've got to a point in the market now where they have a huge amount of trust built up, honestly, with users like myself, who have been using the Bamboo X1 Carbon for over a year.
[1345.32 --> 1347.12]  And it's a great printer.
[1347.88 --> 1350.80]  And I've switched away from Prusa for the most part.
[1350.86 --> 1358.10]  I've still got a Mark III downstairs, but I don't use it anywhere near as much as the Bamboo, just because the Bamboo works first time every time.
[1359.08 --> 1363.00]  If you have a job and you've got the two sitting by each other, you've been defaulting to the Bamboo.
[1363.26 --> 1363.86]  I have, yeah.
[1364.16 --> 1364.28]  Yeah.
[1364.78 --> 1364.96]  Huh.
[1365.38 --> 1368.62]  It's like how you know which laptop you like best, because that's the one you always reach for.
[1368.76 --> 1369.92]  Right, right, right.
[1370.82 --> 1378.22]  Also, it strikes me that the customer demographic they're going to go after for the next five plus years probably doesn't even know about this stuff.
[1378.22 --> 1384.30]  That seems like maybe the bigger problem is that they're very likely going to get away with it.
[1384.30 --> 1393.06]  I don't wonder if they've seen the fact that they've made Prusa capitulate a little bit and think, ah, okay, well, we've moved the goalposts slightly.
[1393.16 --> 1396.96]  So now if we move our goalposts again, maybe it's fine.
[1397.02 --> 1398.30]  Maybe we've got a big enough customer base.
[1398.30 --> 1410.40]  Maybe we've made enough of a splash now and got enough loyal customers that they won't care if we gently funnel them towards the lock-in, the vendor lock-in, the proprietary side of things.
[1410.40 --> 1415.86]  I'm curious if you have a sense of how the community reaction has been to all of this, because it sounds really bad.
[1415.92 --> 1417.96]  So I imagine there's been a lot of upset.
[1418.08 --> 1420.02]  I saw Louis Rossman had a video on it.
[1420.10 --> 1423.12]  He seemed pretty, you know, well, upset about it.
[1423.60 --> 1425.64]  He's known for his calm takes, huh?
[1426.04 --> 1426.50]  Well, yeah.
[1426.58 --> 1428.12]  Let's say Louis was disappointed.
[1429.14 --> 1429.40]  Yeah.
[1430.06 --> 1435.04]  So Louis Rossman, for those of you who aren't familiar, is a huge advocate of something called right to repair.
[1435.04 --> 1442.06]  He's been in front of Congress a couple of times and helped fight legal cases and yada, yada, yada.
[1442.14 --> 1445.48]  Guys in this area is a bit of a hero, I think.
[1445.76 --> 1457.40]  And he has a few very detailed videos on his YouTube channel talking about how the trouble with all of this stuff really began, not necessarily because of the announcement,
[1458.12 --> 1462.88]  although changing the terms of service on customers after they've already bought the product stinks.
[1462.88 --> 1475.64]  The trouble really began when Bamboo began shadow editing their own blog posts and then gaslighting users into believing that, no, no, no, you're just misunderstanding what we said,
[1476.58 --> 1480.02]  whilst also completely changing the words of what they actually said.
[1480.76 --> 1485.92]  That's, you know, that's a sign that they know they've stepped in it and they're trying to manage the situation.
[1486.36 --> 1486.96]  Oh, 100%.
[1486.96 --> 1488.78]  They're in damaged imitation mode right now.
[1489.06 --> 1489.20]  Yeah.
[1489.20 --> 1492.44]  And they even released a blog post that said,
[1492.78 --> 1498.30]  these baseless allegations include things such as the phrase,
[1498.56 --> 1501.70]  firmware updates will block your printer's ability to print.
[1501.92 --> 1505.26]  We want to be sure, we want to be certain that that is not the case.
[1505.90 --> 1508.72]  Yet, the Bamboo terms of service state,
[1509.40 --> 1512.58]  if you do not take the most recent firmware update,
[1512.86 --> 1517.40]  your product may block new print jobs before the update is installed.
[1517.40 --> 1519.50]  So, basically in English,
[1519.92 --> 1522.14]  update to the latest or you can't print.
[1522.78 --> 1522.84]  Yeah.
[1522.98 --> 1524.72]  And then you're stuck with all this new stuff.
[1525.78 --> 1529.48]  I mean, I bet you somebody listening right now is just screaming at their podcast player saying,
[1529.56 --> 1530.64]  I told you so.
[1530.86 --> 1531.76]  Yeah, definitely.
[1532.42 --> 1535.70]  My inner monologue was screaming at me as I was reading this, to be honest.
[1537.04 --> 1538.58]  You just don't want it to be true.
[1538.76 --> 1541.60]  And there's a lot of things like that going around in the world right now where you think,
[1541.76 --> 1542.70]  oh, really?
[1542.78 --> 1544.18]  Is this the route we're going?
[1544.18 --> 1547.14]  Can we just, anyway, not about that.
[1547.68 --> 1549.74]  So, what did the internet do in response to this?
[1550.00 --> 1556.12]  Well, within 24 hours of the gaslighting blog post,
[1557.00 --> 1561.06]  someone had hacked the Bamboo Labs firmware and leaked the private keys.
[1561.58 --> 1563.64]  Oh, that is so beautiful.
[1563.80 --> 1564.42]  I mean, that's horrible.
[1564.56 --> 1564.96]  That's bad.
[1565.10 --> 1565.68]  That's so bad.
[1565.68 --> 1566.08]  Yeah.
[1566.30 --> 1566.70]  Yeah.
[1566.86 --> 1577.28]  Well, I think, you know, if the update was in the name of security, then the existing firmware is clearly horrible and, you know, leaky and all that.
[1577.42 --> 1581.54]  So, maybe the updated firmware won't be vulnerable to such things.
[1581.74 --> 1589.58]  But you can now jailbreak your X1 series of printers and install a custom firmware on it called the X1 Plus.
[1589.58 --> 1594.96]  This enables all sorts of goodies for your Bamboo Lab 3D printer.
[1595.82 --> 1598.40]  And there is a website in the show notes to the GitHub repo.
[1598.96 --> 1604.28]  The X1 Plus firmware enables enhancements like custom splash screen graphics.
[1604.66 --> 1605.02]  Hooray.
[1605.32 --> 1606.22]  Who doesn't want that?
[1606.56 --> 1606.74]  Yeah.
[1606.92 --> 1607.90]  That's worth it.
[1607.98 --> 1608.68]  Yeah, right.
[1609.66 --> 1612.96]  SSH access to the underlying Linux system.
[1613.40 --> 1614.08]  All right.
[1614.44 --> 1617.18]  So, now I'm wondering, can I install Tailscale on that bad boy?
[1617.18 --> 1621.36]  So, extensive statistics for the printer and filament usage and blah, blah, blah.
[1621.46 --> 1622.14]  A bunch of other stuff.
[1622.22 --> 1628.44]  But I think most importantly is it kind of protects you and shields you from everything we just talked about.
[1628.98 --> 1629.20]  Yeah.
[1629.46 --> 1631.98]  I mean, the Linux access alone is great.
[1634.72 --> 1636.06]  That is worth it right there.
[1636.12 --> 1637.12]  That got my attention.
[1637.70 --> 1638.64]  Yeah, I bet it did.
[1640.12 --> 1645.02]  Well, many of you will know that I'm in the midst of having my attic converted into a new studio space.
[1645.02 --> 1649.14]  And as such, I've been taking a ton of photos and videos lately.
[1649.48 --> 1651.60]  And I had a little niggle with Image.
[1651.70 --> 1653.26]  So, I reached out to Alex from the Image Project.
[1653.36 --> 1654.00]  And we got talking.
[1654.12 --> 1656.58]  And I was like, when was the last time you were on the show?
[1656.66 --> 1658.90]  And he was like, November 2023.
[1659.60 --> 1661.34]  So, we figured we'd have him back on the show.
[1663.48 --> 1665.36]  Unraid.net slash self-hosted.
[1665.42 --> 1668.26]  Go there, support the show, and check out the new Unraid 7.
[1668.44 --> 1669.66]  It is actually here.
[1669.82 --> 1670.62]  And it's glorious.
[1670.90 --> 1672.72]  Unraid.net slash self-hosted.
[1672.72 --> 1675.58]  If you haven't checked it out yet, this could be the time.
[1675.76 --> 1679.96]  Unraid is famous for being a solid platform that is great for your home lab or your small business.
[1680.36 --> 1685.60]  And you can get started with mix and match disks just right now with the stuff you have in your closet.
[1686.02 --> 1688.76]  But Unraid 7 really takes it up to a whole other level.
[1689.30 --> 1692.52]  They have really filled out the ZFS feature support.
[1692.98 --> 1694.24]  Hybrid ZFS pools.
[1694.60 --> 1695.86]  Improved fault recovery.
[1696.16 --> 1696.98]  Luxe encryption.
[1697.84 --> 1698.94]  Array-free operation.
[1699.28 --> 1701.84]  And lots of improvements to the UI as well.
[1701.84 --> 1708.20]  Speaking of new UI, they have a new file manager with GUI tools that are just chef's kiss.
[1708.58 --> 1714.86]  Navigate directories, copy, move, delete, do what you need inside the directory, all with their nice web UI.
[1715.22 --> 1718.48]  And you can quickly search in there and find stuff with their new built-in search tool.
[1719.16 --> 1725.06]  And they have an enhanced VM manager, making it much easier to manage, snapshot, clone your VMs.
[1725.06 --> 1727.74]  And, of course, Docker has also gotten some improvement.
[1728.32 --> 1732.90]  Upgrades to networking like Tailscale plug-in so you can have Tailscale built right into your Unraid machine.
[1733.28 --> 1733.68]  Yes!
[1733.90 --> 1734.82]  I love it!
[1735.34 --> 1740.66]  And all the things you've come to expect, like file sharing, even those things like small stuff, macOS, time machine issues.
[1740.74 --> 1744.52]  Just all those things have all been rounded off in Unraid 7.
[1744.52 --> 1748.34]  When they, you know, have the opportunity, they really just went at it.
[1748.36 --> 1750.92]  And they got stuff under the hood and all the way up to the UI.
[1751.42 --> 1755.60]  They even have new power modes to optimize performance and balance out operation and power efficiency.
[1756.10 --> 1757.00]  There's so much.
[1757.04 --> 1760.26]  They have a blog post that goes over all of it because I'm just scratching the surface.
[1760.98 --> 1762.84]  But I think this is the time to check it out.
[1763.38 --> 1768.84]  All these new features, these capabilities, and the integration with Tailscale, it just makes it such a killer release.
[1769.18 --> 1770.88]  Support the show and try out Unraid.
[1771.08 --> 1773.92]  Go to unraid.net slash self-hosted.
[1773.92 --> 1776.98]  That's unraid.net slash self-hosted.
[1778.78 --> 1782.80]  Welcome back to the show, Other Alex, from the Image Project, of course.
[1783.60 --> 1786.34]  It's been, what, how long have you guys been with Futo now?
[1786.42 --> 1788.02]  Maybe eight months or so?
[1788.32 --> 1791.54]  And we wanted to get you on the show, have a little update, see how things are going.
[1792.06 --> 1793.38]  Thank you for having me here.
[1793.60 --> 1794.30]  It's been a while.
[1794.54 --> 1802.44]  Last time we talked was in November 2023, and last year was kind of a whirlwind with Futo approaching us and we joining the team.
[1802.44 --> 1804.52]  So, thing has been going well.
[1805.02 --> 1808.24]  You're a professional open source developer now, if such a thing exists, right?
[1808.30 --> 1808.56]  Right.
[1809.50 --> 1809.98]  Congratulations.
[1810.34 --> 1810.96]  Dream job.
[1811.46 --> 1825.24]  Who would have thought that, you know, a project that I started for my wife now that become the main source of the income for the house and making a lot of people happy and having a really good team and the community.
[1825.24 --> 1825.32]  It's crazy.
[1825.72 --> 1826.50]  It's crazy.
[1826.94 --> 1831.34]  So, that's, I'm sure, been a game changer for you in terms of focus on the project.
[1831.80 --> 1838.52]  And I just thought maybe we'd also get a little update on what some of the recent developments are feature set-wise and project-wise for Image.
[1838.52 --> 1848.16]  Well, as you know, since we joined Futo, it's kind of crazy to think that you have the full autonomy of how to run the project.
[1848.38 --> 1855.38]  So, the way that I've ran the project hasn't really changed much since the last eight months.
[1855.38 --> 1860.38]  Like, the team members still have their autonomy to work on the things that they love.
[1861.24 --> 1869.20]  And the only thing changed is that instead of saying no rush, now we would say, hey, well, we might need this by this date.
[1869.38 --> 1870.74]  That's the only thing that changed.
[1871.28 --> 1871.38]  But...
[1871.38 --> 1872.60]  That's kind of great, though, isn't it?
[1872.72 --> 1872.98]  Yeah.
[1872.98 --> 1873.46]  Huh.
[1874.66 --> 1878.88]  I mean, I suppose that's sort of a best-case scenario in that you've been able to...
[1878.88 --> 1883.50]  Essentially, it sounds like there's really been no influence or pressure from the Futo folks.
[1883.62 --> 1887.40]  And you've had a little more guarantee in team support.
[1887.56 --> 1892.16]  So, you know, like, we talk about our goals for the futures.
[1892.52 --> 1896.60]  And it just aligns with how the team view the project.
[1896.60 --> 1906.02]  So, there is nothing really different of how the expectation between the team member and also from the Futo folks.
[1906.66 --> 1919.08]  The first is always to support open source and to make the user happy and to build a really good software that has a delightful experience.
[1919.34 --> 1920.94]  So, that is our main goal.
[1920.94 --> 1926.46]  Like, image is always self-hosting first, not service.
[1926.60 --> 1937.52]  So, I think that helps a lot with how we can focus on the features and then the experience with our main user base right now.
[1937.86 --> 1948.28]  Yeah, because you've had a lot of, dare I say, choppy waters when it comes to open source and supporting and, you know, the financial side of things in particular.
[1948.74 --> 1951.70]  I'm talking, of course, about the supporter badge that you added.
[1952.38 --> 1952.96]  When was it?
[1952.98 --> 1954.62]  In the middle of last year, something like that.
[1955.14 --> 1956.44]  How's that been going?
[1956.44 --> 1959.74]  Because initially, there was a bit of, you know, Reddit drama.
[1960.32 --> 1961.74]  And has that died down now?
[1962.28 --> 1967.86]  I would say it's completely gone now because we have been doing what we said we would do.
[1968.56 --> 1973.14]  And not, you know, like, doing some type of rug pulling people.
[1973.44 --> 1974.38]  There's still time.
[1976.60 --> 1977.80]  No rug to pull.
[1977.80 --> 1998.96]  But it's actually, you know, an experience that the futile folks want to do is to really pushing out great software with great support and asking people to pay but not bothering you or not limiting you of any means if you don't want to pay.
[1998.96 --> 2014.70]  And surprisingly, by just asking people nicely and explaining, like, what it takes to be such software and the way that we support people, too, I think it makes the notion quite successful.
[2014.70 --> 2028.24]  I have other open source maintainer reach out to me and ask if it works because the donation model just cannot get them to focus and work on the project full time.
[2028.94 --> 2029.72]  And what do you tell them?
[2029.96 --> 2031.32]  Has it been a great success?
[2031.32 --> 2040.76]  Yeah, I say that you should, you know, change the hours facing message instead of, hey, donate to the software.
[2041.18 --> 2042.84]  You should buy the software instead.
[2043.68 --> 2050.78]  So with that, it encouraged people to actually, you know, like putting out the money to support the software.
[2051.18 --> 2053.34]  Granted that you have to build the good software first.
[2053.34 --> 2060.30]  It's the first, I think, the first ingredient of success is you need to give people the reason to support you.
[2060.30 --> 2063.70]  We take that as given with Image these days.
[2064.16 --> 2065.58]  I have another question for you, Alex.
[2065.84 --> 2072.38]  The banner is still there at the top of the Image website saying, this project is under very active development.
[2072.86 --> 2074.84]  Expect bugs and changes.
[2075.42 --> 2078.60]  Do not use it as the only way to store your photos and videos.
[2079.40 --> 2081.32]  Are we ever going to see that disappear?
[2081.56 --> 2084.52]  Are you ever going to trust yourself enough to take it away?
[2085.88 --> 2089.48]  Well, we actually have a plan to take it out soon now.
[2090.30 --> 2100.60]  So recently we have going through a lot of the internal changes that is mainly on the code side.
[2100.60 --> 2109.42]  So we make it easier for us to develop features and not running into issue.
[2109.42 --> 2114.82]  So that takes a while and it's almost done now.
[2115.46 --> 2129.26]  And once that's done, we will be able to focus on some of the final items to making sure that when we take that banner down and pushing out a stable release,
[2129.26 --> 2139.64]  people can trust that within a major version, you have the backward compatibility between the server and the client.
[2139.64 --> 2148.78]  Although I think the special thing of Image is that it comes with a mobile app and the server application, right?
[2149.44 --> 2155.06]  On Android, you can side loading APK.
[2155.58 --> 2160.42]  You can use different stores to download the app.
[2160.42 --> 2164.60]  But it's such a hassle on the iOS side.
[2165.34 --> 2173.98]  So it is a challenge for self-hosting stuff that comes with a mobile app.
[2174.08 --> 2181.06]  Because we don't have a way to distribute the iOS app for you to stay on a version that you want, right?
[2181.42 --> 2181.68]  Right.
[2181.76 --> 2184.14]  On iOS, it's just the latest version is what you get.
[2184.56 --> 2184.90]  Correct.
[2184.90 --> 2194.10]  And so your goal is, is once this banner is down, that maybe there could be a couple of version changes on the back end,
[2194.18 --> 2197.24]  but the mobile app, particularly on iOS, would continue to work?
[2197.62 --> 2197.94]  Correct.
[2198.22 --> 2198.40]  Yep.
[2198.52 --> 2201.34]  So we will go full Semver.
[2201.78 --> 2202.98]  Right now, we don't go with Semver.
[2202.98 --> 2211.96]  So we can have breaking changes between a minor release because I was not having experience with version back then.
[2211.96 --> 2216.20]  So I just pumped from 0.19 something depth to 1.0.
[2217.80 --> 2221.68]  Yeah, because it was just me and my wife was using the app.
[2221.74 --> 2222.72]  So who care, right?
[2223.04 --> 2223.26]  Sure.
[2223.26 --> 2229.82]  Until it's gaining traction and all the developers like, hey, why is it 1.0 when you guys have breaking changes between minor release?
[2230.14 --> 2234.94]  You know, Alex, that I can imagine is just a frustrating thing to deal with in general with a fast-moving project
[2234.94 --> 2241.72]  is you then have the delay of the iOS app release and you want to try to coordinate those two things as closely as possible.
[2242.20 --> 2242.40]  Yep.
[2242.86 --> 2247.06]  And I think it's just the expectation you would have to help people to understand.
[2247.06 --> 2254.88]  And I think if I come from, like, people in those background, I would understand, like, how frustrated they would feel that,
[2255.16 --> 2261.56]  hey, I'm using the 1.0 app, but why there's breaking changes that my instance cannot connect it in anymore
[2261.56 --> 2263.94]  and I have to go make changes to the Docker file.
[2263.94 --> 2267.74]  Especially as maybe image starts to reach the next wave of users.
[2268.50 --> 2274.38]  I also wanted to talk to you about, well, first of all, I wanted to say I'm really impressed that since we've chatted,
[2274.38 --> 2279.62]  there's been a lot of features that have landed in image, but I don't feel like the UI has gotten overly complicated.
[2280.50 --> 2283.92]  Like, recently, I know you added the ability to create tags on the fly.
[2284.56 --> 2287.94]  There's been some other fixes that have been landing in the most recent updates.
[2288.34 --> 2292.74]  It feels like since the new year, things are kind of like in a stabilizing mode.
[2292.74 --> 2294.44]  Is there something big going on in the background?
[2294.60 --> 2296.12]  Is it about bug fixes right now?
[2296.22 --> 2297.88]  Where are things at in the immediate future?
[2297.88 --> 2306.40]  We have moved completely away from an ORM for database to a query builder.
[2307.04 --> 2313.18]  So that has taken, you know, a great month and a half, two months of work for the whole team
[2313.18 --> 2317.88]  because we have to migrate every single query from an ORM to a query builder.
[2317.88 --> 2318.24]  Okay.
[2318.52 --> 2320.18]  So that's why.
[2320.96 --> 2330.90]  But this would open up a lot of possibility for us to clearly understand what is going on behind the scene for the query.
[2330.90 --> 2338.28]  And we have seen a huge improvement in performance of the apps already when we switch over
[2338.28 --> 2345.66]  because you don't rely on the magic of the ORM anymore, but you know exactly what's going on.
[2345.76 --> 2349.88]  So some query, we got like 2x, 3x faster.
[2350.26 --> 2356.06]  So for the next release, I would expect you to see the timeline will be a lot snappier.
[2356.06 --> 2359.98]  Like when you're just jumping around and dragging around.
[2361.30 --> 2362.22]  That's not bad now.
[2362.22 --> 2363.06]  Yeah, I'd love to hear that.
[2363.10 --> 2363.52]  That's great.
[2363.66 --> 2364.46]  I'm already happy.
[2364.58 --> 2365.32]  So that's even better.
[2367.16 --> 2373.88]  And we have one of the core team members just out the blue.
[2374.00 --> 2378.06]  Hey, I re-implemented the timeline calculation in Rust.
[2378.06 --> 2384.06]  So now we can put like placing fast on image.
[2384.20 --> 2386.14]  We love us some Rust over here at JB.
[2386.54 --> 2387.08]  That's true.
[2387.56 --> 2394.60]  So a question for you on the, one of the features I actually find to be very good is the duplicate detector.
[2395.16 --> 2397.60]  Do you have any plans to make that?
[2397.80 --> 2401.64]  Because at the moment I've got like 6,000 duplicates in my image library.
[2401.64 --> 2405.72]  And I have to go through them all one by one or accept all.
[2405.86 --> 2410.06]  Can you find a way in the UI somehow, Alex, to make this?
[2410.86 --> 2411.64]  Feature request.
[2411.86 --> 2412.64]  Feature request alert.
[2412.88 --> 2413.74]  Better at volume.
[2413.88 --> 2415.36]  You've got to try, haven't you, Chris?
[2416.60 --> 2418.14]  He wants checkboxes, I think.
[2418.78 --> 2421.56]  I think, yeah, if I'm managing 6,000 assets at once.
[2421.66 --> 2424.32]  Like I want an easier way than just one by one.
[2424.56 --> 2425.72]  I don't know what that would be.
[2425.72 --> 2434.62]  Well, we have a bulk action option already where you can either duplicate all or remove all.
[2435.28 --> 2436.38]  Yeah, that seems dangerous though.
[2436.44 --> 2438.10]  If I don't know what I'm clicking remove all on.
[2438.54 --> 2444.74]  Yeah, I guess another iteration of that feature is, I guess you would have, you know, like 100 in one page,
[2444.98 --> 2451.06]  which you can choose to either select it or keep or handle duplication.
[2451.06 --> 2455.36]  But showing up all at once would probably help.
[2456.96 --> 2461.44]  Yeah, you know, like a lot of the features in image is just going through its first path.
[2461.60 --> 2468.42]  And there are so many ways that we can enhance on one specific features.
[2469.44 --> 2471.38]  So it's still going.
[2471.52 --> 2477.70]  I feel like image is going to be, the work will never end for image.
[2478.26 --> 2479.26]  That's kind of exciting though.
[2479.26 --> 2483.60]  I mean, you know, it's great to have something that you can continue to refine on and make better over time.
[2483.98 --> 2487.80]  There's always going to be people that have a need for something like this.
[2487.96 --> 2492.80]  And our digital photos are some of our most important assets that I think people own.
[2493.34 --> 2497.76]  And I think people really appreciate that you're a good steward of the project and take it very seriously.
[2497.96 --> 2499.78]  So I'm excited about the future.
[2499.98 --> 2504.68]  And I appreciate you taking time this evening to come on and give us a little bit of an update on how things are going.
[2504.72 --> 2507.92]  Because it's absolutely one of my favorite projects out there right now.
[2507.92 --> 2509.42]  Thanks, Chris.
[2509.50 --> 2510.02]  Thanks, Alex.
[2510.48 --> 2514.42]  It's all thanks to the community, the support that people have.
[2514.42 --> 2520.78]  Even with the core team now, they are started as the community contributor.
[2521.28 --> 2526.58]  And they're just growing their love for the project and eventually join the team to work full time.
[2526.88 --> 2529.26]  So we have a great team.
[2529.44 --> 2534.20]  And it's such a nice way that you can hire people without interviewing them.
[2534.20 --> 2537.30]  Because you know that they love the project and then they don't just slack up.
[2537.84 --> 2540.72]  And they have the technical ability to help you.
[2540.72 --> 2541.98]  So that's amazing.
[2543.14 --> 2543.90]  I imagine.
[2544.24 --> 2546.04]  We will be in Fostem next week.
[2546.14 --> 2549.50]  So if you guys in Fostem, stop by and see us.
[2550.00 --> 2554.64]  We will have some surprise also during that week for Image.
[2555.18 --> 2555.44]  Ah.
[2555.98 --> 2556.54]  Stay tuned.
[2556.54 --> 2556.96]  All right.
[2557.08 --> 2558.32]  Fostem is a great conference.
[2558.44 --> 2559.24]  I'm glad to hear you going.
[2559.34 --> 2559.60]  Yeah.
[2559.74 --> 2561.48]  People keep an eye out for you guys.
[2561.96 --> 2562.18]  Yep.
[2562.18 --> 2564.60]  And we will have a live stream there as well.
[2564.80 --> 2564.92]  So.
[2567.00 --> 2568.82]  Keebo.com slash self-hosted.
[2568.92 --> 2572.34]  That's K-E-E-B dot I-O slash self-hosted.
[2572.64 --> 2581.18]  Now, I had a realization a few years ago that it's worth investing in a great keyboard because I'm using my computer all the time.
[2581.34 --> 2583.28]  And how do I interface with that?
[2583.36 --> 2585.16]  What am I actually physically touching all the time?
[2585.58 --> 2586.66]  My keyboard.
[2587.02 --> 2588.14]  That's why I love Keebo.
[2588.30 --> 2590.82]  Keebo.com slash self-hosted.
[2590.82 --> 2592.32]  We'll also have a link in the show notes.
[2592.52 --> 2597.62]  They specialize in great keyboards, including those split keyboards that really helped with my RSI.
[2598.20 --> 2601.48]  They also have the regular keyboards you might like and expect as well.
[2601.72 --> 2607.10]  They come fully built or, if you like, you can also do a little bit of hot swapping.
[2607.24 --> 2608.90]  No soldering for any of that stuff.
[2609.28 --> 2616.32]  They also have macro pads with the 9 to 16 keys that people use for like, you know, a printing machine, shortcuts.
[2616.32 --> 2617.32]  You can also use it.
[2617.32 --> 2623.48]  One of the ways we use it is a way to switch cameras with OBS or maybe like you have a home theater machine.
[2623.62 --> 2626.28]  You can use one of those little macro pads.
[2626.36 --> 2626.98]  I think is what they call them.
[2627.04 --> 2627.52]  A macro pad.
[2627.58 --> 2630.06]  It's like 9 to 16 keys to control something.
[2631.14 --> 2636.46]  You know, and I also want to mention that they have stuff for those of you that aren't a fan of the big clacky noises.
[2636.46 --> 2642.68]  So you can still get the comfort, that kind of classy feel, that high-end feel without the noise.
[2642.76 --> 2643.72]  They've got those as well.
[2644.34 --> 2649.58]  They also stock lots of DIY parts if you need to make repairs or like to build your own, including microcontrollers.
[2649.80 --> 2652.96]  And they support open source and publish 3D printed parts.
[2653.32 --> 2656.20]  So you can print the case if you need to, make repairs.
[2656.62 --> 2656.86]  I don't know.
[2656.92 --> 2658.24]  Maybe you threw it at somebody and cracked it.
[2658.30 --> 2659.24]  Not saying I ever did that.
[2659.24 --> 2667.62]  And also, they're part of the core team of QMK, which I'm probably, you know, the least experienced person with the QMK firmware.
[2667.74 --> 2668.28]  I'm aware of it.
[2668.32 --> 2673.32]  I know it's preferred amongst the high-end keyboard community, I'll just say.
[2673.46 --> 2677.74]  But I think it's really great as a sign to see that they're a core contributor to that team.
[2678.02 --> 2680.02]  And all their boards use QMK as well.
[2680.36 --> 2681.02]  That's pretty neat.
[2681.56 --> 2682.44]  It's really good to see that.
[2682.94 --> 2685.04]  So support the show and go get yourself something nice.
[2685.04 --> 2688.58]  Start by going to keeb.io slash self-hosted.
[2688.58 --> 2689.52]  Support the show.
[2689.72 --> 2694.52]  And when you go to that URL and sign up for the newsletter, you'll get 5% off your first order.
[2694.68 --> 2698.04]  K-E-E-B dot I-O slash self-hosted.
[2699.44 --> 2700.88]  Is it time for some feedback?
[2701.16 --> 2702.16]  How's your SAT looking?
[2702.70 --> 2707.32]  Let's dig in and start with our top four boosts this week.
[2707.40 --> 2709.24]  We're trying something new and doing just the top four.
[2709.88 --> 2713.52]  And Fuzzy Mistborn comes in with 6,666 SATs.
[2713.62 --> 2713.82]  Ooh.
[2714.54 --> 2716.20]  And he's got feedback on the Echobee.
[2716.20 --> 2719.10]  He says it's a great product, especially with the remote sensors.
[2719.70 --> 2725.52]  My biggest annoyance for new users is they no longer accept developer accounts for using the cloud API.
[2726.10 --> 2731.48]  And while the HomeKit integration is top notch, there are actually a few things that you cannot control.
[2731.86 --> 2734.74]  My main use for the cloud API is setting up vacation mode.
[2734.74 --> 2746.54]  I add dates and times to a specific vacation calendar and Home Assistant is then able to set up a vacation on the Echobee, which then helps set up the house to an extended away mode when I go on trips.
[2746.54 --> 2749.54]  I heard from someone else this week in the Discord, too.
[2750.00 --> 2751.96]  Self-hosted.show slash Discord, by the way.
[2752.60 --> 2763.02]  That they wanted to use the microphone built into some of the higher-end Echobee thermostats as like a, you know, always listening microphone to control Home Assistant or something.
[2763.60 --> 2766.86]  And I don't think you can do that using the HomeKit integration either.
[2767.02 --> 2769.74]  So, yeah, it's good to know that these limitations exist.
[2769.74 --> 2777.02]  Yeah, and there are definitely ways you could solve that through Home Assistant automations, but it wouldn't be as simple.
[2777.58 --> 2778.70]  The scheduler card might help.
[2778.92 --> 2780.06]  I'm plugging it one more time.
[2780.16 --> 2780.84]  Scheduler card.
[2780.92 --> 2781.26]  Love it.
[2781.84 --> 2783.88]  Adversary 17 comes in with a Jar Jar boost.
[2783.94 --> 2785.14]  That's 5,000 sats.
[2785.26 --> 2790.98]  And adversary says, Chris, Alex, audience, I'm looking for an easy setup with Docker self-hosted budgeting app.
[2791.32 --> 2792.56]  Something that has good mobile support.
[2792.68 --> 2793.62]  Thank you in advance.
[2794.56 --> 2796.54]  Do you have a self-hosted budgeting app?
[2796.54 --> 2798.64]  I feel like we've talked about invoicing.
[2799.74 --> 2803.80]  Ooh, there was a new one I saw on the vine this week.
[2804.50 --> 2805.34]  On the vine?
[2805.48 --> 2806.18]  You old man.
[2807.30 --> 2809.68]  What makes me old man about that?
[2809.70 --> 2810.60]  On the grapevine?
[2810.68 --> 2811.86]  That's what my grandma used to say.
[2811.92 --> 2813.20]  I heard on the grapevine.
[2815.32 --> 2815.72]  Yeah?
[2815.94 --> 2816.26]  All right.
[2816.32 --> 2816.64]  All right.
[2816.74 --> 2817.88]  Us Brits, you know.
[2818.04 --> 2818.96]  Yeah, that's true.
[2819.06 --> 2819.88]  We do it old school.
[2820.28 --> 2820.64]  You do.
[2820.92 --> 2823.40]  You get a lot of mileage out of those old sayings.
[2823.68 --> 2825.58]  Mon-et-er, I think is how you spell it.
[2825.90 --> 2829.16]  Like it's money, but instead of Y, it's T-R at the end.
[2829.16 --> 2833.44]  If anybody knows and has any suggestions too, I wouldn't mind looking at a few of these.
[2834.06 --> 2837.48]  Yeah, I'm going to send you this link in, how should I do it in Slack?
[2837.60 --> 2838.62]  Is that the best way?
[2839.30 --> 2840.28]  Whatever you want, darling.
[2841.00 --> 2841.88]  Whatever you want.
[2842.68 --> 2843.28]  I'm on all of them.
[2843.32 --> 2844.26]  Yeah, take a look at this.
[2844.56 --> 2845.80]  Mon-et-er.
[2846.16 --> 2846.48]  Why?
[2846.84 --> 2848.00]  Okay, open source developers.
[2848.44 --> 2851.12]  Can we just have a word about us poor podcasters?
[2851.32 --> 2853.06]  We have to say these names out loud.
[2853.06 --> 2853.14]  God.
[2854.24 --> 2856.66]  Yeah, it must be like monitor, like you're monitoring your money.
[2856.94 --> 2858.04]  Yeah, or money tree.
[2858.28 --> 2858.76]  I don't know.
[2859.28 --> 2864.14]  Anyway, this is an app that lets you take control of your finances and is fully self-hosted.
[2864.38 --> 2867.78]  Jeez, it looks way better than I was expecting for an app like this.
[2868.02 --> 2868.42]  Mm-hmm.
[2869.18 --> 2873.70]  Where these things often fall down for me, though, and I don't mean any disrespect to this particular app,
[2873.70 --> 2881.84]  and I haven't looked at it at all beyond what you just heard, but it is how they actually integrate with the day-to-day spending that I do.
[2882.00 --> 2888.64]  They often rely on, is it Plaid is the thing that scrapes, is like an API that scrapes these things?
[2889.04 --> 2889.18]  Yeah.
[2890.32 --> 2895.14]  It's kind of a crapshoot as to whether your institution supports it or not, and I don't know.
[2895.44 --> 2902.92]  Often with Plaid, you can just give a gibberish for a bank search, and then it'll let you just put your ACH routing information in there,
[2902.92 --> 2907.90]  but it may not be able to do the scrape you're looking for because what it does with the full login is it goes in.
[2907.96 --> 2910.12]  It actually can read everything in your online banking.
[2910.26 --> 2910.88]  It's kind of gross.
[2912.50 --> 2920.92]  I don't love it, but it's how a lot of these work, and sort of the state of the financial system is there's lots of intermediary datament like this.
[2921.70 --> 2929.20]  Particularly in the U.S., actually, that was one of the things that surprised me most when I emigrated is just how old school the finance system here is.
[2929.20 --> 2934.88]  I wrote a check last week for the first time since I literally was about 11 years old.
[2935.48 --> 2935.64]  God.
[2935.98 --> 2941.12]  I think you really feel it when you try to move money, like, between financial institutions.
[2941.58 --> 2947.58]  Like, I have an account I pay my bills out of, so payday comes, and then I move money into a bill-paying account,
[2947.72 --> 2950.90]  but it takes two or three days for the money to move.
[2951.04 --> 2952.50]  It's been so wild.
[2952.50 --> 2958.90]  Wise Papa John sent 4,544 sats instantly over the Lightning Network.
[2959.34 --> 2960.42]  Hey, guys, it's been a while.
[2960.92 --> 2963.92]  I've been out of the podcast game for a few months, but I'm catching back up,
[2963.96 --> 2967.76]  and I was wondering, what do you guys use for dash cams in your car?
[2968.28 --> 2971.82]  I have a cheapo Chinesium cam, and it just records to micro SD,
[2972.50 --> 2974.88]  and it can't even read license plates when I review the footage.
[2975.34 --> 2980.12]  A cam that maybe could even tie into Home Assistant or maybe some sort of self-hosted NVR would be great.
[2980.12 --> 2983.36]  I do have a couple of Wyze V3s sitting around.
[2983.98 --> 2985.06]  Maybe I could do something with those.
[2986.46 --> 2988.70]  Dash cams are a weird space, aren't they?
[2989.24 --> 2992.44]  They have very strange requirements.
[2992.58 --> 2996.02]  They've got to be hardened against extreme cold and extreme heat,
[2996.26 --> 3001.00]  and also have the sun shining on them for hours at a time as you go down the road,
[3001.06 --> 3003.44]  so the lenses have to be hardened.
[3003.70 --> 3007.96]  Like, if anybody's ever shone a camera at the sun as a kid for too long and damaged,
[3007.96 --> 3012.24]  burnt film, God, I'm dating myself, burnt film or something like that,
[3012.32 --> 3015.74]  you'll appreciate the sun is powerful, right?
[3015.76 --> 3016.46]  Yeah, yeah.
[3017.02 --> 3019.62]  But generally, the video quality out of these things,
[3019.72 --> 3026.34]  it's a balance between blocky McBlockface and taking up tons and tons of SD card storage,
[3026.40 --> 3028.60]  which we all know SD cards are notoriously unreliable.
[3029.64 --> 3032.50]  Generally, dash cams suck, if we're being honest.
[3032.50 --> 3034.10]  The quality's pretty poor.
[3034.38 --> 3036.52]  There's a lot of them that you have to sift through.
[3036.52 --> 3037.72]  Oh, yeah, yeah.
[3037.92 --> 3040.84]  And they're from brands you've never heard of on Amazon.
[3040.84 --> 3042.84]  And some of them have features that are so annoying,
[3043.16 --> 3047.00]  like traffic light camera detection and lane guidance detection.
[3047.08 --> 3048.16]  You think that sounds great?
[3048.30 --> 3048.56]  No.
[3048.66 --> 3050.52]  It just means it's beeping at you at random times.
[3050.58 --> 3051.36]  You don't want that.
[3053.06 --> 3057.64]  Also, what's with all you narcissists that have the dash cams that put the camera on your face?
[3058.04 --> 3059.68]  Like, you're never picking your nose while you drive?
[3060.04 --> 3063.14]  You actually want to be on camera looking like an idiot when you get in an accident?
[3063.76 --> 3064.02]  You know?
[3064.10 --> 3065.42]  Like, why do you want the camera on your face?
[3065.42 --> 3069.08]  I think my dash cam would just pick me air drumming most of the time.
[3070.22 --> 3071.20]  I'm just thinking, too.
[3071.28 --> 3075.34]  Like, talk about a waste of SD card space as my dumb face is sitting there staring at the road.
[3076.32 --> 3079.24]  I mean, so there are a couple of things I look for in a dash cam, to be honest.
[3079.30 --> 3085.48]  And this isn't really self-hosting related because I don't know of a good way to really get the data off the dash cam
[3085.48 --> 3090.10]  besides just marking the file by pressing the button on the cam and then popping the SD card out.
[3090.30 --> 3094.92]  Or I think some of them create like a Wi-Fi hotspot from the camera and you can kind of transfer files.
[3094.92 --> 3095.58]  Yeah.
[3095.58 --> 3096.46]  To your phone that way.
[3096.58 --> 3098.74]  And it's a bit slow, but it works.
[3099.70 --> 3103.34]  I just want a camera that points out the front and a camera that points out the back.
[3103.42 --> 3104.84]  And ideally, it's one system.
[3104.94 --> 3107.42]  So it's all kind of synced together.
[3107.42 --> 3114.10]  So I've been using the Vantrue S1 for a couple of years in the Gulf and it's been fine.
[3114.60 --> 3117.36]  I think it was a couple of hundred dollars with a hard wire kit.
[3117.98 --> 3118.88]  Does the thing.
[3119.46 --> 3119.60]  Yeah.
[3119.60 --> 3125.62]  I would just say to address the question about the Wyze cams, I'm going to say that's a negative there, big dog.
[3125.86 --> 3136.02]  As somebody who drives down the road in his RV with an actual dash cam and a Wyze 3 cam side by side, it's great, but it's not what the Wyze cam is meant for.
[3136.42 --> 3138.38]  It doesn't run as well as you'd think continuously.
[3138.38 --> 3143.80]  And you really want something that's a dumb piece of equipment that doesn't need a Wi-Fi connection to operate.
[3143.92 --> 3147.14]  It can just turn on and start recording when it detects motion.
[3147.32 --> 3151.26]  So for something that you're going to use for like actual insurance purposes, get a hardware camera.
[3151.48 --> 3156.62]  Plus, you do like the SD card because you can just turn that right over to the cops, assuming you don't have yourself being a dumbass on there.
[3156.62 --> 3163.62]  And our last boost is rounded out by Forward Humor, who comes in with a row of ducks, 2,222 sats.
[3164.00 --> 3164.90]  Hey, guys, I'm curious.
[3165.50 --> 3168.12]  You both mentioned using Claude as an AI copilot.
[3168.32 --> 3169.48]  What helped you draw?
[3169.80 --> 3172.06]  What drew you to this over the others?
[3172.18 --> 3172.66]  Why Claude?
[3172.66 --> 3182.32]  I found it to be better at sort of development coding tasks when futzing around with my Nix configs over Christmas.
[3182.32 --> 3190.38]  I still prefer perplexity for doing research and things that require sources and things like that.
[3190.46 --> 3194.88]  But for code, I do find the Claude models to be better.
[3195.46 --> 3202.14]  Yeah, I think Claude has been, especially the Sonnet, has been particularly trained on development.
[3202.86 --> 3207.74]  And so I think that's one thing is that Claude is really good at that syntaxical kind of stuff.
[3208.24 --> 3209.68]  I think you're right with perplexity.
[3209.68 --> 3212.06]  It seems to be the best research and current events tool.
[3212.32 --> 3216.68]  And then I think OpenAI has a really good language and reasoning system.
[3216.76 --> 3222.20]  So if you want something to help you with language or working through a problem, OpenAI seems to be pretty good there.
[3222.68 --> 3224.76]  And then, you know, you have your local LMs.
[3224.88 --> 3227.98]  And I'd love to know the audience experience with how those rate in these areas.
[3228.42 --> 3229.08]  What's your experience?
[3229.20 --> 3230.36]  I know you play with them a bit.
[3231.22 --> 3231.76]  Yeah, I do.
[3231.98 --> 3238.18]  And it's the trouble is, is that the the models locally are actually fine.
[3238.18 --> 3247.82]  My problem is that I'm running my Olama instance on a Nix box and I keep breaking it.
[3248.02 --> 3251.64]  And I know it takes me a long time to then get around to fixing it.
[3251.86 --> 3251.98]  Yeah.
[3252.14 --> 3254.04]  You can just go to the website and use Claude right now.
[3254.04 --> 3254.52]  Yeah.
[3254.88 --> 3255.20]  Yeah.
[3255.36 --> 3261.04]  And the the the ironic thing is that sometimes I'm using Claude to help me fix.
[3261.64 --> 3262.96]  Oh, that's funny.
[3263.30 --> 3263.48]  Yeah.
[3263.60 --> 3265.92]  No, it's been very useful for that kind of stuff.
[3265.98 --> 3266.16]  All right.
[3266.16 --> 3267.02]  So we have more boost.
[3267.08 --> 3268.06]  We'll link them in the boost barn.
[3268.12 --> 3269.00]  It wasn't a big week, though.
[3269.04 --> 3269.78]  But thank you, everybody.
[3269.84 --> 3271.58]  We had 34 unique senders overall.
[3271.58 --> 3274.22]  And you sat streamers out there.
[3274.26 --> 3275.12]  There was 30 of you.
[3275.30 --> 3279.54]  So highly represented by the sat streamers this week doing the heavy bulk of the lift.
[3279.64 --> 3282.30]  They helped us stack twenty eight thousand seven hundred fifty eight sats.
[3283.06 --> 3287.86]  Then when you combine that with the boosters, it's a very humble forty nine thousand five hundred and twelve sats.
[3288.24 --> 3290.12]  But we appreciate it.
[3290.14 --> 3295.94]  Nonetheless, if you'd like to boost, get Fountain FM and strike and get going or go the Albie Hub route with your own self hosted node.
[3295.94 --> 3297.80]  There is an entire journey out there for you.
[3298.18 --> 3300.40]  We'll have some links in the show notes to help you get started.
[3300.40 --> 3301.92]  Absolutely.
[3302.24 --> 3306.88]  And as usual, you can go to Alex dot Katie's dot me to find all of the places that I'm online.
[3307.28 --> 3312.02]  And also, I want to say a great big thank you to our site reliability engineers, our subscribers.
[3312.40 --> 3314.90]  You really make the show possible with your direct support.
[3315.00 --> 3317.38]  You get an ad free feed with a post show.
[3317.56 --> 3321.12]  You can go to self hosted dot show slash S.R.E. to find out more.
[3321.28 --> 3323.80]  I want to mention colony events dot com.
[3323.80 --> 3326.34]  It's a self hosted gather instance that we're running.
[3326.34 --> 3331.28]  And on February 2nd, it will be Linux Unplugged episode 600.
[3331.62 --> 3336.90]  And we're inviting the audience to attend more than a dozen different meetups that are being organized or create their own.
[3336.96 --> 3341.18]  So you can do that on the Gavio instance if you'd like and do a listen party.
[3341.30 --> 3344.98]  Jump in our mumble room or jump on JBLive dot FM for LUP 600.
[3344.98 --> 3347.16]  We have details at colony events dot com.
[3347.82 --> 3350.82]  And then, you know, just around the corner, it's scale.
[3351.08 --> 3352.18]  It's Planet Nix.
[3352.72 --> 3354.16]  It's Linux Fest at Northwest.
[3354.72 --> 3356.20]  And we're going to be at those events.
[3356.34 --> 3357.14]  We'll be doing meetups.
[3357.40 --> 3359.34]  It's going to be a really busy season.
[3359.50 --> 3363.78]  So we'll have all kinds of details for you on those events coming up very soon as well.
[3364.10 --> 3366.70]  And last but not least, don't forget links to what we talked about today.
[3366.86 --> 3370.06]  That's itself hosted dot show slash one forty one.
[3370.06 --> 3373.10]  And you can find me at Chris LAS dot com.
[3373.40 --> 3375.98]  How are you finding Gavio, by the way, before we get out of here?
[3376.50 --> 3380.20]  You know, I like it a lot in the sense that any other folks can create their own events.
[3380.28 --> 3384.36]  And then once the event's over, it just sort of after a certain amount of time self-destructs.
[3384.40 --> 3385.66]  So they're ephemeral, which is great.
[3385.74 --> 3387.50]  So you don't have like this huge back catalog.
[3388.16 --> 3392.12]  But it has a good and bad feature where there's no user login system.
[3392.80 --> 3396.38]  So it generates like a key for you when you create your first event.
[3396.38 --> 3399.08]  And you have to save that key if you want to go back and edit later.
[3399.08 --> 3404.80]  Or if you if you use the same browser and don't clear your cookies, you know, it just goes right back into edit mode.
[3404.84 --> 3408.42]  But if you go from another computer or a different browser, you have to have that key.
[3409.08 --> 3410.88]  And so that surprised a few folks.
[3411.46 --> 3415.60]  And it does tell you, but it's it's not crazy clear.
[3415.66 --> 3417.40]  And it's like the only tool that does it this way.
[3417.46 --> 3418.88]  So people aren't really ready for it.
[3419.14 --> 3425.42]  But at the same time, I kind of prefer it over having to have a username and password database that JB has to run.
[3425.54 --> 3425.76]  Right.
[3425.82 --> 3426.64]  So that's kind of nice.
[3427.14 --> 3427.94]  But that's the downside.
[3427.94 --> 3428.94]  Hmm.
[3429.60 --> 3436.04]  If only there was a way to do like single sign on OAuth or something and just outsource authentication completely.
[3436.22 --> 3437.16]  You know, there might be.
[3437.40 --> 3438.00]  I actually haven't.
[3438.08 --> 3438.46]  You know what?
[3438.50 --> 3438.92]  There might be.
[3438.98 --> 3439.62]  I haven't dug into that.
[3439.62 --> 3440.06]  But the good.
[3440.20 --> 3450.46]  The good news is there are ways if you have admin privileges on the server and you can get into the SQL database, you can actually get those keys and recover those keys and then get them back to the user.
[3450.46 --> 3454.12]  So, like, if you can get that far, there are ways to recover the key.
[3454.22 --> 3454.96]  It's not gone forever.
[3455.90 --> 3456.26]  Okay.
[3456.60 --> 3464.78]  Well, you can go to gath, G-A-T-H dot I-O, gathio, to the website to find out more about what we were just talking about.
[3464.78 --> 3466.90]  And thank you so much for listening, everybody.
[3467.10 --> 3470.64]  And until next time, that was self-hosted dot show slash one for one.
