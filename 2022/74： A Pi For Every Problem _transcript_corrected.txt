[0.00 → 3.96] Well, joining us on the show today, we have a colleague from Red Hat of mine,
[4.24 → 10.82] Josh Lasker. But before we introduce Josh, I just need to warn anybody, like a trigger warning.
[11.64 → 14.94] This man has more Raspberry Pis than Chris Fisher.
[15.28 → 19.80] I know. I think there is some discussion about creating a law against owning this many Raspberry
[19.80 → 25.12] Pis. Well, we have a leaderboard for the amount of storage people have. I think we might need
[25.12 → 30.36] to create a new leaderboard for the number of Pis. Anyway, welcome to the show, Josh.
[31.06 → 34.34] Thank you so much. Long time listener and excited to be here.
[34.60 → 38.18] Well, very good. Before we get into the show proper, let's just do some housekeeping stuff,
[38.26 → 44.50] shall we? The London meetup is coming up fast on August the 5th. We have finally nailed down
[44.50 → 51.70] a location that everybody seems to be happy with. So we're going to go for the Jubilee Gardens,
[51.70 → 56.68] right underneath the London Eye-Hunger ford Bridge down by the River Thames in London,
[56.94 → 63.36] next to Waterloo Station. There is a big grassy area with a bunch of paths kind of winding their
[63.36 → 68.66] way through it right next to the South Bank River frontage. I think if we just all meet up there
[68.66 → 76.50] around about six o'clock British summer, there's been some consternation in the group about GMT versus
[76.50 → 82.66] BST. Sounds like a load of BS to me, but there we go. Six o'clock, as you look at your watch,
[83.40 → 88.62] in British summer is when we'll be meeting down in the Jubilee Gardens in London.
[89.08 → 94.18] I am super happy that you have found a location. I know that was a bit of consternation,
[94.28 → 98.70] especially because you're doing it from afar. So that's perfect. It's like getting real now,
[98.78 → 102.66] Alex. Yeah. Well, I mean, when we were here, we did the one in Raleigh, I could go and check it out
[102.66 → 106.40] and make sure it was all good. But in London, it's a lot more tricky. And I actually had several
[106.40 → 110.70] offers from folks. There was a lovely venue near Covent Garden. There was another one in Woolwich
[110.70 → 115.54] that we were offered, but they were indoors. And some of the folks who are meeting with us,
[115.66 → 120.70] just that's a hard line for them. You know, Friday night in London, there aren't too many outdoor
[120.70 → 126.08] options. So I thought we'd just keep it simple and do something fairly central that is fairly
[126.08 → 132.60] touristy and therefore reasonably safe so far as London goes. And yeah, that's where we
[132.60 → 137.62] ended up. Meetup.com slash Jupyter Broadcasting for the meets on that. And of course, you guys have
[137.62 → 143.00] been organizing this. This really was birthed in the self-hosted matrix itself, self-hosted discord
[143.00 → 149.68] at self-hosted. Show slash discord. The Freudian slip on the matrix there was because this did inspire
[149.68 → 157.64] us to realize and take action. And that was, we created a JB Meetups matrix space. So at matrix,
[157.64 → 163.52] there's this concept of a space where you can have like a bunch of collection of rooms. So we have a
[163.52 → 168.48] meetup space. And then in there, we're going to have location specific chat rooms that are going to be
[168.48 → 173.20] standing chat rooms. So that way we can build crowds. Like I'd like to create a Raleigh one. I want to
[173.20 → 178.24] create a California one. We already have a London colony, a Pacific Northwest colony, and the mumble
[178.24 → 183.06] colony. So we can also do virtual events, but I could see more in the future. I'm just kind of feeling it
[183.06 → 187.62] out right now. And there is already folks organizing in the London colony. We'll have a link in the show
[187.62 → 192.56] notes to that as well. Because what we were talking about was potentially going for some air quotes,
[192.76 → 199.34] pre-drinks or pre-eats before the main meetup somewhere nearby as a smaller group. Because I
[199.34 → 205.08] know, you know, we pick 6pm because then anybody that's got to travel after work or has work in the
[205.08 → 210.44] London area can still make it at the official time. But I don't know, like three, four o'clock,
[210.44 → 214.50] something like that. Maybe a few of us might meet up a little bit earlier and go and get some food or
[214.50 → 219.94] something like that. And then head over at 6pm proper. Very good. I want to say thanks to Tim
[219.94 → 225.72] for filling in last episode. Did a great job while I was out sick, which was horrible timing.
[226.02 → 231.18] I hope you're feeling better. Yeah, I'm like 90% better. I still have some junk in my chest and in
[231.18 → 236.32] my sinuses, but I'm like 90% better. The worst timing ever, really. It was just a horrible time to get
[236.32 → 240.16] sick. So I was doing pre-records. We were trying to do this show. I was trying to travel. It was like
[240.16 → 244.40] the worst possible time to get sick. Well, when we had Tim on, we turned it into the
[244.40 → 250.12] Kubernetes action show in your absence. Yeah. Yeah. I enjoyed it. I enjoyed it a lot. And we
[250.12 → 254.50] got some nice comments too. So thank you to Tim for filling in. For those of you that have been
[254.50 → 259.60] following along with the show, I sent in, I think it was probably about six weeks ago now, I sent in
[259.60 → 266.02] to Western Digital a failed, shucked hard drive. I finally got the replacement through yesterday.
[266.02 → 270.70] Okay. Well, okay. Do you know how long it was, Alex? I've lost track of how long it actually took
[270.70 → 274.60] for the replacement to come. Well, I removed the drive from the server when Brent was here.
[274.86 → 279.34] So that should give you some idea. It was a while ago, six, eight weeks, something like that.
[280.22 → 284.76] So all I did was I took the failed drive, which was a shuck drive, about two years old,
[285.00 → 291.66] out of the server, wrapped it in some bubble wrap in a box from, reused from Amazon, sent it across to
[291.66 → 298.28] Western Digital. And then a few days later, the RMA said, completed. I got an email. It didn't,
[298.34 → 303.68] didn't give me any, any problems whatsoever. It just changed from, we've received your item to
[303.68 → 311.04] completed. There were no other updates. And a few days later, what arrives? I get a brand new
[311.04 → 317.14] drive in a box, an unshocked hard drive. I got a Western Digital My Book delivered.
[317.14 → 322.16] Unshocked, ready to go. So you sent them a shuck drive and they, so they must've realized there was,
[322.32 → 328.30] and they sent you back a My Book. It feels passive-aggressive almost like they know what you're up to.
[328.72 → 333.38] And here's the thing, right? The drive that I sent them was originally an easy store drive,
[333.44 → 338.24] which is a Best Buy exclusive. And they send me back a My Book, which is not.
[338.50 → 338.74] Right.
[338.88 → 344.36] So there's been conjecture and guesswork on the internet for eons about the fact that they're
[344.36 → 346.88] the same drive. I guess we have some proof now.
[347.56 → 352.52] Yeah. It does seem like it is a data point at least. Josh, have you tried this shucking thing
[352.52 → 353.68] that Alex talks about all the time?
[354.10 → 359.10] Most definitely. I've done it both for my Synology boxes when I've grown over time. I've
[359.10 → 364.00] got three up to this point, one at my local place of worship and then two here in the lab.
[364.14 → 367.38] So both a four bay and a two bay. And I've had success with it.
[367.38 → 372.44] I have one drive right now that is actually my, it's my one shucked drive. It's been great.
[372.44 → 376.86] And that's been in production since Brent was here, which is even longer than since
[376.86 → 381.10] Brent was at Alex's place. We measure things in Brent time now.
[382.32 → 386.34] Brent standard time. BST. What could go wrong using that acronym?
[386.76 → 389.68] But I mean, you got a disc, right? I mean, you got to shuck it.
[390.04 → 394.24] Yeah. I mean, to be honest with you, I already bought the replacement because I don't like
[394.24 → 399.96] being down for that long. So I'll probably throw it up on eBay. If somebody wants a 12 terabyte
[399.96 → 402.86] drive for cheap, send me a message and...
[402.86 → 407.46] You're not keeping it as a backup? Oh, what about a hot swap? Come on, Alex.
[408.48 → 413.74] I've already got one of those in there. I don't need, I don't need a backup for my hot spare.
[414.34 → 416.54] Mister, I don't need 12 terabytes over here.
[417.32 → 421.90] Okay. Here's the thing, right? I went through, and so I used, I use radar a lot, right? I know
[421.90 → 426.80] we don't talk about this stuff very much, but I use radar a lot too much if I'm being perfectly
[426.80 → 435.72] honest. And I added some automations to automatically based on lists, right? So in any given week,
[436.48 → 445.14] 50 to a hundred movies appeared on my system. And I just had no idea where I was going to find the
[445.14 → 450.08] time to watch all this stuff. So about when that drive failed, actually, I just went through and
[450.08 → 458.32] deleted terabytes and terabytes of stuff. So my array, let me have a look, merger FS, here it is,
[458.80 → 467.98] 71 terabytes right now, used 25, remaining 47. So I think I'll be all right without the extra 12.
[468.12 → 472.88] I think. Yeah, you'll be all right. You'll be all right. I just recently did that too. I was getting
[472.88 → 477.96] ready for the trip or something like that. I wanted to grab some shows and I realized I was down to like
[477.96 → 485.76] two terabytes of free space and I had like four terabytes in my queue. And I knew as I was looking
[485.76 → 491.10] at everything, I was like, before this finishes, I'm going to run out of disk space. You know,
[491.20 → 497.06] one of those moments. And I just went on a deleting rampage, dude. And it felt so good. Like it felt so
[497.06 → 500.70] good to just delete stuff. I know I'm never going to watch. I got a bunch of stuff on there.
[500.70 → 506.96] There was like, just I, I, if I had it on DVD, I backed it up. Or if somebody, like a friend wanted
[506.96 → 511.38] to request something, the system would go grab it for them. And there was so much stuff that I was,
[511.52 → 517.20] nobody was watching ever. It felt so good to purge. It felt so good. Now I've really refined it down to
[517.20 → 522.18] like the stuff that I've either handcrafted or, you know, the stuff that is like in the watch queue
[522.18 → 527.02] or something like that right now. Let the internet be your backup. How about that? See, I was still
[527.02 → 531.86] kicking it old school to where I bought my DVDs and Blu-rays, ripped them across, put them onto
[531.86 → 536.52] my Plex media server. And then when, and if something were to happen, yeah, I can always
[536.52 → 543.44] re-rip those down. So I haven't made that next step. You know, I have to say proudly, proudly that
[543.44 → 549.80] the Blu-rays that I have ripped are always better than the ones that you can get off the internet.
[549.80 → 555.84] Like, I don't know, man, maybe it's, maybe it's just because I know what the FFM peg commands do.
[555.84 → 561.46] I don't know what the difference is, but it always, my encodings years later, like I'll come back,
[561.50 → 567.26] like we're watching, my wife and I are re-watching Star Trek Enterprise. I hand ripped every one of
[567.26 → 573.14] those episodes, right? And I did it meticulously with two pass encoding and like all the right,
[573.30 → 578.96] all the right settings. And it just, it holds up. And I did that work years ago. Very proud of that.
[579.04 → 580.46] So that kind of stuff I did not purge.
[580.46 → 582.70] With the setting, make my CPU hurt, huh?
[583.12 → 590.12] Yeah. All right. So I, I have to ask the audience, Josh, you too. You know, I've talked
[590.12 → 596.28] positively about the HomePods as a voice control mechanism for Home Assistant. I like them. Not
[596.28 → 600.84] only do I think they are the best sounding Home Assistant, but the commands to interface with
[600.84 → 606.36] Home Assistant using the HomeKit API are all done over the LAN. The voice transcription is done remotely,
[606.36 → 613.30] but once it figures out what you've requested, the HomePod executes that request locally over the LAN
[613.30 → 619.92] to your Home Assistant server using the HomeKit API. It's very nice. It's more private. I just have
[619.92 → 627.72] preferred it. I don't know what's changed, but Siri has lost it. Like lost it. Like if I say,
[628.18 → 633.56] hey, Lady Tube, turn off the entry bar, her response after she thinks about it will be,
[633.56 → 640.12] okay, I've turned off the Apple TV 4K. I'm sorry. The Apple TV 4K is not responding.
[640.92 → 644.92] I didn't say anything about that. If I say, hey, Siri, turn off the bed skirt.
[646.00 → 650.20] She just won't say anything. Like nothing happens. Like commands that I used to do on a daily basis
[650.20 → 656.16] as I was coming and going from my home just in the last week, quit working. She just thinks I've
[656.16 → 661.22] said something completely different from what I've said. Completely different. And then I don't know how,
[661.22 → 665.42] I don't know if my wife tapped something or what happened, but somehow personalized results have
[665.42 → 670.18] been turned on, and now it's doing voice recognition. And of course it like sees a different set of
[670.18 → 675.68] devices for some reason when my wife has a command versus when I have a command. This just changed.
[675.96 → 681.36] And it feels like somebody came into our home and moved all the light switches around
[681.36 → 687.84] and hooked them up to different stuff. And it's super frustrating because like the wife approval
[687.84 → 692.48] factor, which has been very high on this entire system is on a decline right now.
[693.60 → 697.42] Have you guys experienced this with, with any of these voice assistants? Is this something unique
[697.42 → 702.32] to Siri? Is anybody in the audience? I'm like, I'm lost for words and I don't know what to do
[702.32 → 706.22] because of course I've got these stupid home pods all over the place, and now they're working for
[706.22 → 711.00] crap. And it might actually be home assistant's fault. That's the other thing is I opened up my home app
[711.00 → 716.42] and the home assistant stuff didn't look right. I don't know what was going on. So it may actually
[716.42 → 721.30] be something in home assistant, but more troubleshooting needed. You got to warn us when
[721.30 → 726.34] you're getting your site box out, dude. I know. I know. Josh, have you experienced this?
[726.74 → 732.30] So I'll be honest with you, Chris. I've just put my big toe finally into the home automation side of
[732.30 → 736.80] the house and I still don't trust any of the voice command stuff. I want to make sure it's all
[736.80 → 741.94] here locally toward the point where I put that entire thing on pause. I didn't own my home yet.
[742.22 → 747.10] I now have bought my first home. The issue was I needed to make sure I could segment my network
[747.10 → 753.72] correctly to where I had an IOT network. I had a home computer network. I had a security system
[753.72 → 759.70] network completely separated to make sure they can't see each other. And then just then literally
[759.70 → 765.30] last week after listening to you guys forever on using home assistant, that's, what's running on the
[765.30 → 770.72] silver pie behind me is I've got that in the con B running, and I've started playing with that.
[770.82 → 775.34] And it can't see other than what I told it to because it's only on that network.
[775.76 → 779.16] Yeah. I like that you started with the security first. That's a great idea. You know, the utility
[779.16 → 785.64] of the voice commands, especially because home family members don't want to walk to tablets every
[785.64 → 791.42] time has been really like crucial. I think in the approval factor by the whole family, because
[791.42 → 796.64] you know, everybody from, you know, kids to new people that are visiting can do it really quick.
[796.64 → 799.94] But now it's gone totally sideways, and it makes the whole system look loony.
[800.42 → 804.70] I'm hoping that Mycroft gets a little bit better and or we get more to where we're doing it locally
[804.70 → 809.38] again, because like one of the things that I've got is the re-speaker with the four mic setup.
[809.38 → 815.80] And when I tried testing that about a year and a half ago, it wasn't great. Not that the hardware
[815.80 → 822.84] wasn't great. Software wasn't great. So I think it's coming, but it's not there yet. So I'm not
[822.84 → 826.74] going to hit that button. I must say, I'm not particularly surprised to hear Josh hitting the
[826.74 → 833.70] security angle pretty hard from the get-go because you're involved with the DEF CON scene, aren't you?
[833.70 → 838.86] I am. I've been going to DEF CON for a few years now. I enjoy the security aspect of it. So
[838.86 → 843.26] DEF CON's coming up here. It's not like in 45 days and so many hours. This is fine.
[844.22 → 849.04] I see. I see. Well, it's a good angle to look at this stuff. I think you should always start from
[849.04 → 854.54] a position of not trusting these devices at all, you know, and you like, I'm sure like you guys,
[854.76 → 860.92] I am before I buy anything these days, I tend to do a lot of research on if it can be locally
[860.92 → 865.64] controlled, what, you know, what it's built on information about the company, like buying a
[865.64 → 870.96] device these days feels like you have to like almost get in a relationship with a company.
[871.30 → 874.62] That's one of the things I really appreciated about local control. Anytime there's a local API,
[874.84 → 879.56] that's a big win for me. I feel like that was one of the things I liked about the HomePods.
[880.24 → 882.78] And I mean, like I just, another thing, I just got a Napoleon.
[882.96 → 883.20] Nice.
[883.38 → 886.84] And these things are, these are really nice. They're wood. They look like wood on the walls.
[886.98 → 888.22] But you got the wood ones. Sweet.
[888.22 → 891.00] And they look really great. They just look, they almost look like art on their own,
[891.08 → 895.90] even when they're off. And true to the documentation, when you power that thing and
[895.90 → 900.38] you get it on your Wi-Fi, Home Assistant automatically detects it and suggests, hey,
[900.40 → 905.24] would you like to install the Napoleon integration? And it was just a little wonky at first,
[905.26 → 910.38] but it's been totally solid since. All local API, no cloud, no cloud account, no nothing like that.
[910.52 → 915.60] It's very nice. So, you know, there's wins and losses. So I feel like the Napoleon win,
[915.60 → 921.80] like offset, like the HomePod loss recently. But now I'm just kind of, you know, now I've just
[921.80 → 922.84] kind of equalized everything out.
[923.74 → 928.54] I recently picked up the Napoleon hexes and absolutely love them. Exactly. Same experience
[928.54 → 932.32] to where once you turned it, connected it to the network, then from there, Home Assistant just
[932.32 → 933.14] picked it up. No problem.
[933.34 → 934.38] And they're just neat looking.
[934.72 → 940.42] Against my better judgment, I bought some LEDs from Gov recently. I say recently,
[940.42 → 947.02] it was probably six months ago. And when I got them, the integration was cloud polling integration
[947.02 → 954.92] and it just worked fine. About two months ago, Gov just decided to rate limit the API requests.
[955.28 → 961.70] And suddenly all the lights just stopped working with Home Assistant. I opened a support ticket and
[961.70 → 966.22] they were like, well, we don't know what you're talking about. Like the support people just had
[966.22 → 972.32] no clue what even an API probably was, sadly. But thankfully, I was able to go into the integration
[972.32 → 977.46] and update the polling rate, which meant that now they work. They're a bit slower than they were,
[977.56 → 981.74] but they work at least. So yeah, let that be a lesson, kids.
[982.32 → 986.88] You know if they don't want to handle the API requests, maybe they could just let the API
[986.88 → 991.92] requests go locally. Hmm. I mean, I'm just going to put that out there. But if your cloud service
[991.92 → 996.00] can't handle the customer demand, maybe you should re-architect it so it doesn't require
[996.00 → 1000.48] your cloud service. How would you collect the data then, Chris? That's the real question.
[1001.20 → 1007.06] Right. What data are you collecting on how many minutes my LED strip underneath my bed is on for?
[1007.22 → 1012.12] I mean, really? Because we need to calculate how much longer it's going to be until you buy the
[1012.12 → 1017.82] next set of LEDs, Alex. Well, there's that. But also there is sort of like this metadata information
[1017.82 → 1022.74] of, now they don't know if it's not automation, but most people probably are not automating these
[1022.74 → 1027.94] things. So they can kind of probably assume Alex was home during these times or something like that.
[1028.00 → 1032.42] I don't know. I don't think it's so much about collecting data with these types of vendors.
[1032.76 → 1039.44] I think it's more about an ecosystem that they build this mode around, and they try to get you,
[1039.52 → 1043.74] every one of these vendors, even Napoleon does this, has like a million products.
[1043.74 → 1048.62] Like, have you looked at the Wise store recently? Oh, yeah.
[1049.08 → 1053.04] Have you looked at that thing, dude? Like they went from selling cameras to like,
[1053.18 → 1059.24] now they sell scales and stuff, like weight scales and stuff. Like they're just like everywhere, man.
[1059.50 → 1062.58] Everybody does this. They all want to be, they want to make a million products.
[1063.04 → 1067.76] The Wise store is like walking into one of those markets in Taiwan where you've got like 15 different
[1067.76 → 1071.86] stores at all moments, and they've just gone, yeah, we'll have that. We'll have that. Yeah.
[1071.86 → 1077.10] We'll stick our logo on that. Yeah. We'll throw our logo on that too. And yeah. Yeah. That's fine.
[1077.16 → 1081.06] That'll do. We're not going to worry about the support. Like, you know, with the first gen cameras
[1081.06 → 1085.58] or anything, we're just going to slap a sticker on it. Right. Talk about a Trojan horse company.
[1086.22 → 1091.50] I think that's sort of the overall motive with these companies and their cloud only APIs and whatnot.
[1091.88 → 1096.70] But like, that's not how you get my loyalty. That is the business model. You're right.
[1096.70 → 1098.50] It is. I have to agree.
[1126.70 → 1133.04] It's a mesh network based around WireGuard's noise protocol. They're using like the best VPN
[1133.04 → 1139.02] technology in a super, super clever way. You can quickly and easily create a flat mesh network
[1139.02 → 1144.28] where your devices get a static IP. And if you're a maniac, you could throw like a pie hole box or a
[1144.28 → 1149.94] DNS server in that mix, and you can actually start doing name resolution on that network. It's so great.
[1149.94 → 1154.52] You can also do things like share one machine with a friend like Alex and I do for some of
[1154.52 → 1158.14] these testing we'll do here on the shows. But you know what else they've recently introduced,
[1158.26 → 1162.82] which blows my mind is they've introduced a new product, a new feature, I guess,
[1163.26 → 1169.46] called Tail scale SSH. You can now easily manage your SSH connections with Tail net.
[1170.30 → 1175.72] Tail scale SSH allows you to establish SSH connections between your devices in your Tail scale network
[1175.72 → 1179.84] and authorized by your access controls. You don't have to sit around and
[1179.84 → 1185.88] copy your keys like a caveman anymore. And it authenticates your SSH connection using WireGuard.
[1186.12 → 1192.80] It's so great. Tail scale is a breakthrough VPN technology. It's the kind of thing I knew they'd
[1192.80 → 1197.44] build once WireGuard was a thing. That's why I wanted it to be mainline for so many years,
[1197.72 → 1202.02] because I knew we get cool stuff like this. I've got to run on everything. My Arch servers,
[1202.02 → 1207.78] my Soon servers, my x86 boxes, my Raspberry Pis, my portable devices. It's on my phone right now.
[1207.78 → 1211.86] I always leave it connected too, because the client is really smart about what it routes to
[1211.86 → 1215.48] your Tail scale network versus what it routes out to the internet and stuff like that. So you're not
[1215.48 → 1219.02] accidentally sending every single webpage load over your Tail scale or something like that.
[1219.42 → 1223.20] So go try it. Support the show and get it for free up to 20 devices when you go to
[1223.20 → 1230.38] Tailscale.com slash self-hosted. Imagine one flat network for all your devices, your containers,
[1230.38 → 1235.98] your VMs, your physical devices, your mobile devices, friends, family, colleagues, all protected
[1235.98 → 1241.78] by WireGuard that you get up and running in minutes. Tailscale.com slash self-hosted.
[1243.90 → 1249.82] Now I teased at the top of the show that we have a dare I call it a Raspberry Pi hoarder?
[1250.06 → 1252.34] I don't know if that's a correct word, but-
[1252.34 → 1252.74] Collector.
[1253.24 → 1254.90] Collector. Okay, let's go with that.
[1254.90 → 1259.48] Yeah, I mean, I don't know, Josh. I feel like you could almost create a currency based on how
[1259.48 → 1260.70] many Raspberry Pis you have.
[1260.70 → 1265.04] I don't have that many Pis. Come on now, Chris. And they are getting hard to get a hold of.
[1265.28 → 1269.68] Okay, tell the people, Josh, tell the people, how many Raspberry Pis do you have?
[1269.68 → 1277.98] So I've currently got 43 Pis and 8 Pi Picks. When we actually list these things off, it's one
[1277.98 → 1284.76] compute module for 13 Raspberry Pi 4s, seven Raspberry Pi 3s, three Raspberry Pi 2s, six Raspberry
[1284.76 → 1290.42] Pi 1s, 11 Raspberry Pi 0s, and one Raspberry Pi 0s.
[1290.76 → 1293.26] And a partridge in a pear tree.
[1293.52 → 1295.38] I forgot. There was a 400 in there as well.
[1295.76 → 1296.76] My goodness, Steve.
[1296.76 → 1297.96] Oh, sure. Yeah, you have to have a 400.
[1297.96 → 1301.94] You have to have the 400, right? That's what you can actually get a hold of nowadays, too.
[1302.06 → 1304.06] So you can still find those at decent price.
[1304.16 → 1304.88] Those are great machines.
[1305.28 → 1309.86] That is a lot of Raspberry Pis, whatever way you slice it.
[1310.16 → 1310.40] Yes.
[1310.46 → 1314.16] How are you going to justify having so many to us? Please.
[1314.56 → 1319.62] So I have been collecting these literally from the beginning. I was super excited. Before I was
[1319.62 → 1325.64] in working for my current employer, I wanted to get into Linux. And the Raspberry Pi was a great
[1325.64 → 1330.68] way to do that. And playing with Linux on the side was always fun, but you never had a dedicated
[1330.68 → 1335.08] machine for that. Or you'd be dual booting and wiping Windows and Linux and going back and forth.
[1335.48 → 1341.84] Hey, the Pi's filled that need, which was awesome. So creating their own cases. I was one of the
[1341.84 → 1346.22] early adopters to where when I bought them, they actually have like the misprint on there to where
[1346.22 → 1352.68] it's the 10 M on there instead of the 100 megabit to where it was super, super early days. So I've
[1352.68 → 1357.84] just been buying a couple per time they come out with a new one and then finding tasks for them.
[1357.98 → 1367.34] So it started off with just a thin client. And from there, I was able to use the thin client OS to go
[1367.34 → 1374.30] over to my ESXi instance, my Proxmox instance. Early days, 10 years ago, back when these came out back
[1374.30 → 1380.56] in 2011 and 2012. And then from there, I made myself a lap deck, which was the old school Motorola
[1380.56 → 1385.44] flip up to where you could be used to go through and plug in like your own cell phone back before that
[1385.44 → 1391.64] was a thing. And I built my own cables to where I could have a portable Linux Raspberry Pi laptop,
[1392.00 → 1395.44] went to my hacker space, went and talked about it. And it just kept on growing from there.
[1396.00 → 1401.26] So what was it about the Raspberry Pi platform that seems to have drawn you so early on? Because for me
[1401.26 → 1407.12] personally, I think it really took to the Pi 3 and definitely once the Pi 4 landed where I said
[1407.12 → 1412.22] to myself, this is really something I can use now. And you kind of it seems like you honed in on a
[1412.22 → 1413.06] lot earlier than I did.
[1413.56 → 1418.38] So early adopter with it because I was young and dumb at that point because I wanted to always try
[1418.38 → 1424.44] the newest, latest and greatest. And hey, Raspberry Pis with SD cards instead of being able to afford
[1424.44 → 1429.38] full up machines, even if you were trying to get them returned from like a thrift shop or whatnot,
[1429.38 → 1435.54] you had more ecosystem, more of a community behind the Raspberry Pis than anything else you could do.
[1436.08 → 1439.70] Very true. There was that network effect very early on in a way that most devices didn't get.
[1439.96 → 1444.56] You must have experimented with Pi alternatives, though, right? Because as a Pi user,
[1444.60 → 1448.36] you're constantly being told there's a much better device out there if you just bought the right device.
[1448.36 → 1452.54] I completely agree with that. And I was young and dumb and stupid and bought many of them. And then I
[1452.54 → 1457.98] finally figured out there's not the community. And even with like the Litre boards that were out there,
[1457.98 → 1461.48] I backed those on Kickstarter. And when trying to get them up and running,
[1462.22 → 1467.50] the Pi just had it. And it comes down to open source. It comes down to the open community.
[1467.76 → 1470.86] And when you bridge those together, that's where you've got the magic sauce.
[1471.34 → 1474.66] So that's what Raspberry Pi just did. And it kept on hitting it off for me.
[1475.04 → 1478.70] And then I agree with you, Chris. Early days, I like, oh, I'm going to implement this.
[1478.74 → 1483.94] It's going to be my full-time desktop. Yeah, not powerful enough. Oh, I can do my Plex server on this.
[1483.94 → 1488.94] Yeah, no, that's not powerful enough either. So I quickly learned over the years,
[1489.10 → 1494.32] the performance that the Raspberry Pi could do would most of the time not meet the need that I
[1494.32 → 1499.86] needed. So when the new one came out, oh, let's try this again. Hey, it worked better. We went from
[1499.86 → 1507.86] a single core to a quad-core. But that RAM, oh, that RAM hurts. No. So I agree. Once we got to the
[1507.86 → 1514.98] Raspberry Pi 4, that's why I've got 13 of them, because they got so much more powerful.
[1515.48 → 1525.30] So here's the thing for me, Josh. And I just, wouldn't a single virtualization server replace
[1525.30 → 1526.70] all of these?
[1526.94 → 1531.64] So that is a good question. Back when I was still, when I was not working from home,
[1531.64 → 1536.50] I went through that point and saying, I'm going to virtualize everything. I got the pizza box.
[1536.84 → 1543.18] Everything was happy-go-lucky. Until my wife called and said, hey, this service is down. Oh,
[1543.30 → 1549.64] why don't you go ahead and just SSH and then just, you know, I'll be home and I'll fix it. Versus,
[1549.64 → 1553.72] hey, go unplug the Pi, plug the Pi back in. It's working now.
[1554.08 → 1558.88] Have you heard of our Lord and Saviour tail scale? You could just VPN in and fix that bitch.
[1558.88 → 1562.76] That should be their slogan.
[1565.50 → 1570.36] So the significant other buy-in was part of that, to be honest with you, Alex. So some things, yes,
[1570.38 → 1576.34] we do virtualize other things. Like when you're just getting into a network, and you're trying to
[1576.34 → 1581.90] find out more about your home network, throwing in a Raspberry Pi 4 for Pi Hole gives you so much
[1581.90 → 1586.34] more insight of how many devices are reaching back out to the internet that you would have to buy like
[1586.34 → 1591.64] ubiquity grade or more enterprise grade gear to start getting that insight. But let's be honest,
[1591.76 → 1596.78] you can buy a hundred dollars worth of Raspberry Pi kit, plug it in and get that information now.
[1597.06 → 1600.18] So how many dollars do you think you're deep into this hole then?
[1600.40 → 1608.30] I don't want to even think about that, but I've only ever paid the MSRP. I've not gone through and
[1608.30 → 1610.46] supported the scalpers. That's all I got to say.
[1610.46 → 1615.78] Good for you. Good for you. If we ignore the dollars and cents, let's talk about something a
[1615.78 → 1620.60] little more tangible because you live in the desert, right? Where heat is a problem.
[1620.94 → 1626.02] These things are going to consume, I don't know what, 5 to 15 watts depending on what they're doing
[1626.02 → 1626.52] each?
[1626.96 → 1630.72] Yes. Yes, they will. And that's why I've had to go through and pick my favourite cases.
[1631.10 → 1635.14] Because I've been collecting for so long, I buy a lot of cases. I buy a lot of hats,
[1635.14 → 1641.62] all the Raspberry Pi cameras. And I've got to say, honestly, for my area in the desert is the
[1641.62 → 1648.14] Villa rose all aluminum cases are by far the best because it's completely passive. You're not having
[1648.14 → 1652.20] to worry about dirt getting into it. They actually come with thermal paste to where you could go
[1652.20 → 1658.76] through and apply it on the case itself and touch all the parts. And it keeps it clear and cool.
[1659.12 → 1663.30] And that's literally what I have running on every single Raspberry Pi when it comes to the force.
[1663.30 → 1667.02] Have you tried the Flirt case that also comes with a little thermal pad?
[1667.38 → 1672.60] I have their previous Flirt cases for the three, and I still honestly prefer the Villa rose.
[1672.98 → 1675.50] Yeah, because I was thinking, you know, I definitely have been in situations where
[1675.50 → 1679.60] it gets really, really hot and those Raspberry Pis are definitely at like thermal throttle levels.
[1680.14 → 1683.38] So that would be good. All right. Send me a link to that. I'll try to add that to the show notes.
[1683.82 → 1688.74] There's a Geek worm one that I really like that is all aluminum as well. And that does
[1688.74 → 1694.44] completely passive cooling. And that's what's just there on the live stream, running that 3D printer
[1694.44 → 1699.12] back there doing Octobrist. Speaking of the live stream, I loved FOSS accountants comment
[1699.12 → 1704.82] in here. I no longer need to feel bad about having an unused eight gigabytes Pi 4 in my drawer.
[1706.46 → 1712.52] So used Pis versus if they're actively being, if they're just sitting in a drawer sad, or if they
[1712.52 → 1716.80] have a project waiting for them, how many you have in production versus how many you have just
[1716.80 → 1720.94] sitting around are two different things. So I mean, there's still naming and shaming that should
[1720.94 → 1723.00] be going on there if they're just sitting in a drawer.
[1724.02 → 1729.56] I agree. I agree. I got, I agree. Furthermore, I got, I got more projects than I got Pis at this point. Furthermore, I need
[1729.56 → 1730.02] more Pis.
[1730.26 → 1734.88] So speaking of projects, right, we've talked about Pi Hole. We've talked about Thing Clients. There
[1734.88 → 1736.64] must be some other stuff you use these things for.
[1737.02 → 1741.24] Like I said, the lap deck was one of them. Being into the security side of the house as well,
[1741.88 → 1746.60] standing up your own pen testing box or a Cali instance where you can slap that in there.
[1746.80 → 1750.70] Before Cali was officially supported, there were other earlier spins that was like called the
[1750.70 → 1756.28] Pwn Pi or Sticky Fingers. There's also the damn vulnerable Pi. So if you needed to pen test against
[1756.28 → 1760.66] something, you could do that as well. If you're more into the Wi-Fi hacking and tracking, you've
[1760.66 → 1764.56] got the Kismet Pi. Lots of different projects when it comes to the security side of the house.
[1765.00 → 1767.76] There's a link to all these different projects in the show notes, by the way.
[1768.02 → 1773.48] Along with that, getting my kids also into computing. That was their onboarding process to where
[1773.48 → 1779.14] we went from going to a Maker Faire to, hey, here's the older Raspberry Pi. So I'd get the
[1779.14 → 1785.74] brand new one. It would be implemented into my new project, and then I'd give them the old one.
[1785.84 → 1790.28] They'd have to learn to go plug in all the cables. I wasn't going to completely cry over if they
[1790.28 → 1796.24] plugged in the HDMI wrong and broke something to where it was a spare Pi, but they got real life
[1796.24 → 1799.82] experience with it. And then that actually helped them later on to where they could build up their
[1799.82 → 1805.56] full-up machines and then move it, unplug it, rep lug it back in and know the components well.
[1806.06 → 1810.58] So talk to me a little bit about this SDR monitor station that's in the list. I've kind of wanted
[1810.58 → 1814.04] to get into software-defined radio for some time. What do you do with it?
[1814.46 → 1819.54] So these are set up for different use cases on if you're tracking aircraft. I'm also curious to
[1819.54 → 1823.12] have more of these implemented now that I'm starting with Home Assistant and using the Zigbee side of
[1823.12 → 1828.66] the house. When you get into SDR, you can start with the RTL SDR, which is like starts at 20 bucks.
[1829.26 → 1833.42] Those are my understanding as over in Europe, you would go through and use these to receive
[1833.42 → 1838.28] TV signals. But here in the States, you can go through and pick those same things up,
[1838.36 → 1843.20] use a couple of specialized pieces of software and track aircraft. You can go through and see
[1843.20 → 1848.76] other things that are talking, anything from some cell phone, depending on which bandwidth that
[1848.76 → 1853.52] you're looking at, which antennas that you have, all the way up to you can buy a dedicated software
[1853.52 → 1859.62] defined radio like the Hack RF. And then you have a huge area that you can go through and listen to
[1859.62 → 1865.46] where anything from the FM, like 900 or the 90 megahertz, all the way up to the six gigahertz range.
[1865.68 → 1869.68] For me, I'm only listening because I don't have my hand license. So I'm not going through and
[1869.68 → 1873.44] injecting anything that goes to the you need to go have a hand license if you want to start
[1873.44 → 1877.98] transmitting. So what can you do with that? Once you've listened to a certain
[1877.98 → 1884.70] frequency and got some information, like I get the fact that you see the pretty graph with the
[1884.70 → 1889.80] nice colours and the shadow traces of all the stuff, but then what? What do you do with it?
[1890.18 → 1895.06] What I want to go through and do with it is set up a tracking to where if something is moving within
[1895.06 → 1898.90] my yard, this is one of the ways to go through and do that. You can do that partly with Wi-Fi,
[1898.90 → 1903.96] you can do that with these other ones as well. Oh, cool. So making more of that map to where you can
[1903.96 → 1908.26] go through and find out how closely can you track this. If I've got an evil mother-in-law
[1908.26 → 1910.60] walking under the property, I want alarms to be going off.
[1913.00 → 1916.14] I mean, I was thinking actually, you know, if you had an F-16 land in your front yard,
[1916.20 → 1917.12] you'd probably notice.
[1917.48 → 1921.80] Yeah. I mean, most likely, but I tell you what, when I've gone through and used the SDRs when I've
[1921.80 → 1927.52] been like in larger metropolitan areas, like San Diego, LA and such, seeing all the flights,
[1927.52 → 1934.56] I was rocking those back on my old school netbook. And after like 250 flights, the thing would crash
[1934.56 → 1938.44] because there was so much data going on because it does not only them taking off their airspeed,
[1938.54 → 1942.34] their tail numbers and such, but also their destination. So you can actually see it mapped
[1942.34 → 1948.12] across the entire situation. So that's one step. You could also go to like starting to track Zigbee,
[1948.46 → 1953.18] Z-Wave and seeing the actual traffic going on there. If you have the right sensors as well,
[1953.18 → 1959.62] you can also then start looking at your water meters, your electrical, and there are things
[1959.62 → 1964.80] that we can hook into like home assistant now that you buy a product that goes through and does that.
[1965.28 → 1969.26] What I want to learn more about is actually doing it for myself versus going and just buying a product
[1969.26 → 1973.08] to do it. See, Chris, you've got some catching up to do, brother. I could use that to maybe measure
[1973.08 → 1977.92] tanks. As far as aircraft tracking goes to, you know, it'd be great there for recording, Alex.
[1978.28 → 1982.30] Whenever the system could tell us when a plane is about to be overhead, we could stop recording
[1982.30 → 1987.14] so we don't have bad audio. What is your absolute favourite Raspberry Pi project that you've either
[1987.14 → 1992.64] done or want to do? My favourite Raspberry Pi project I've done. The one I'm most proud of is
[1992.64 → 1998.08] probably the lap deck, to be honest with you. It's one of my first ones, and it was done a long time
[1998.08 → 2002.24] ago. I'll have to include some pictures, update the show notes. But the one that I'm most looking
[2002.24 → 2010.62] forward to is doing Kubernetes on the Pi. I ended up getting three Raspberry Pi for eight gigs for that
[2010.62 → 2015.42] purpose. Doing some more studying up on that, making sure that we've also got the external
[2015.42 → 2022.14] USB something drives to where your USB is going to pass through the four 400 megabits per second.
[2022.50 → 2027.74] If you go watch Jeff Green's video on it, he's got certain adapters that he recommends going down
[2027.74 → 2031.48] that route to make sure you're getting the full read write speed from the SSD.
[2032.34 → 2034.72] That guy basically is a Raspberry Pi engineer at this point.
[2034.96 → 2036.96] Right? Absolutely. Absolutely.
[2036.96 → 2040.82] So how are you going to go about running Kubernetes? We should have had you on last
[2040.82 → 2043.90] time with Tim, and we could have had a Kubernetes nerd down.
[2044.46 → 2049.06] So I'm still learning about it because that's partly where I'm pivoting to in my day job as
[2049.06 → 2054.30] well with more of what used to be Stack. But that's a whole other kit and caboodle.
[2054.44 → 2059.30] Well, we don't talk about OpenShift very much on this show, but Josh is a colleague of mine at Red Hat.
[2059.52 → 2065.00] I'm a technical account manager by day and so is Josh, but you focus on a slightly different area of
[2065.00 → 2067.90] technologies, right? Right. I'm more of the platform, Tim.
[2068.84 → 2072.96] And I've gone down the Ansible side of the house as well.
[2073.10 → 2078.30] But there is a need for my team to be able to bring up ACS or the advanced cluster security.
[2078.76 → 2082.50] So that's where I'm starting to deep dive now. So with that, sure, you can run that in Kubernetes.
[2082.80 → 2087.00] You can run that on K3, K8 and on OpenShift.
[2087.00 → 2092.22] So it's like, oh, it's just a small, small little, you're just going to learn just a little bit to run this one program.
[2092.38 → 2093.02] This is fine.
[2093.44 → 2098.62] There's a line in the chat room. Be right back, convincing my team to move our OpenShift clusters to Raspberry Pis.
[2099.70 → 2102.60] Yeah, I mean, you could swap them out easier, that's for sure.
[2102.98 → 2104.92] I'm not sure that you'd have as much downtime.
[2104.92 → 2115.78] The power efficiency is also something else that we should go through and talk about, because when you're talking about doing that virtual machine and having the old school pizza boxes, you can get them cheap.
[2115.94 → 2125.06] But sitting there at 300 watts sucking out of the wall versus a Raspberry Pi is not sucking that much or even going to like an Intel NUC instead.
[2125.38 → 2126.88] But it can't do as much either, dude.
[2127.22 → 2132.96] I agree. There are very limited use cases for it, but those are legitimate.
[2132.96 → 2135.72] And I think I touched on this with Tim last time.
[2136.48 → 2143.50] The main reason for doing Kubernetes at home is not to do Kubernetes at home, it's to learn Kubernetes for somewhere else.
[2143.94 → 2155.34] Because it's so complicated and coming back to your point about your wife approval factor of, oh, you just do this, and then you tickle this particular thing under that armpit to make it work.
[2155.84 → 2158.94] Doing Kubernetes at home is complete overkill.
[2158.94 → 2164.90] Yeah, just spin up yourself a Rodman and at that point you're sitting so much better.
[2165.02 → 2167.90] Whether you're Rodman or Docker, it's easy enough just to install.
[2167.98 → 2171.98] If you've got a Linux box, install Cockpit and be done with it.
[2172.16 → 2173.68] Install Rodman, and you're done.
[2174.10 → 2175.68] I just run everything in Perl scripts.
[2175.90 → 2177.10] That's the way I go.
[2177.88 → 2179.16] Whatever floats your boat, man.
[2180.50 → 2181.44] Sounds about right.
[2181.44 → 2186.32] We have a storage leaderboard on our self-hosted .wiki website.
[2187.20 → 2191.90] How many raw terabytes do you have on your LAN?
[2192.56 → 2196.50] Live on my LAN, I've only got about 20 terabytes.
[2196.90 → 2201.64] Sitting in a case to be digitized, I've got over 96 total.
[2201.64 → 2211.38] I've not got the Synology's all set up to be able to bring in all the previous because I've also got to bring things from the IDE drives and all those conversions because all the family pictures I'm responsible for.
[2211.96 → 2213.72] So I'm low on the chart.
[2213.84 → 2214.40] I'm only 20.
[2214.84 → 2215.72] What do you think, Chris?
[2215.90 → 2218.00] Do we give them 20 or do we give them the W?
[2219.36 → 2222.78] I mean, I feel like this sets a precedent, Alex.
[2222.96 → 2225.06] You said live on LAN, so it's only 20 terabytes.
[2225.32 → 2227.08] It's not the case.
[2227.66 → 2228.86] You did say live on LAN.
[2228.86 → 2230.80] You did say live on LAN, and I think we've got to be careful.
[2231.22 → 2231.86] I did.
[2232.10 → 2232.34] Yeah.
[2233.52 → 2235.40] That's not bad, right?
[2235.58 → 2236.62] I mean, it's not bad.
[2236.72 → 2237.24] It's not bad.
[2237.40 → 2237.70] It's not.
[2238.04 → 2239.26] It's manageable right now.
[2239.44 → 2247.42] It's not that I'm out of space because it's not like I'm so close to filling that up or anything because I am, but that's what I've got live.
[2247.64 → 2248.42] What's the file system?
[2248.88 → 2254.78] I'm using the Synology file system so where I can go through and plug in those other Hot Swap larger drives.
[2255.20 → 2255.94] Is that Butters?
[2256.16 → 2258.10] I think I actually use Butters under the hood.
[2258.10 → 2259.30] I might be wrong on that.
[2259.66 → 2263.26] I think there was talk about switching to Butters, but it's like SH something.
[2263.52 → 2263.76] Okay.
[2264.22 → 2266.40] Synology hybrid raid, I think is what they call it.
[2266.42 → 2268.26] Maybe I'm thinking of the Ready NAS anyway.
[2268.66 → 2269.16] That could be.
[2269.66 → 2271.18] You know, I was surprised, Josh.
[2271.24 → 2275.84] You could have connected to this episode with the Raspberry Ninja project.
[2275.84 → 2283.34] This is an image created by the Video Ninja developer, which is the video chat app we use.
[2283.46 → 2289.70] And it essentially turns a Raspberry Pi into a dedicated remote camera that does an RTMP stream.
[2289.70 → 2291.76] And so you'd plug this thing in.
[2291.84 → 2298.74] It'll use GPU acceleration on the Raspberry Pi and then connect back and stream video just kind of out of the box.
[2298.74 → 2299.98] It looks really neat.
[2299.98 → 2310.94] I will have to definitely give that a try because between Son Bus, there are so many different things that you can literally slap on a Pi, especially when you're going through, and you're starting to do interviews with people remotely.
[2310.94 → 2323.16] You're actually doing like an away kit that you can send them through the mail, like starting off with the inexpensive Racer microphones or you step up to the better microphones with like the Samsung 2QU.
[2323.52 → 2328.16] And then you ship a Pi to them, and then you've got a better audio quality in a Pi.
[2328.26 → 2328.96] You just plug it in.
[2329.26 → 2329.68] Absolutely.
[2329.90 → 2330.52] I'm down with it.
[2332.44 → 2334.80] Linode.com slash SSH.
[2334.80 → 2340.10] Go there to get $100 and 60 day credit on a new account, and you go there to support the show.
[2340.10 → 2344.78] A simple, innovative, affordable and accessible Linux cloud solution.
[2345.42 → 2353.24] See why developers and Linux users, the DevOps pros of the world, all of you out there, many of our listeners have chosen to use Linde.
[2353.46 → 2354.90] You can get up and going in moments.
[2355.24 → 2359.70] I love the fact that they have a slick, clean, easy to use API.
[2360.02 → 2362.00] You can integrate with their command line tool.
[2362.10 → 2365.26] You can use like a Python library if you're living that Python lifestyle.
[2365.26 → 2370.44] And if you just want to use the web interface, they have an easy, intuitive cloud manager.
[2370.74 → 2372.00] It's simple to get things going.
[2372.20 → 2378.12] If you've never set up a server before or if you've been deploying them for 15 years, it's going to be just fine.
[2378.50 → 2382.26] They have really powerful boxes with AMD EPIC processors, MIME PCIe storage.
[2382.26 → 2388.38] And of course, they have a bunch of really great backend services too, like a powerful DNS manager, DDoS protection.
[2388.74 → 2391.38] They have Kubernetes support and Terraform support.
[2391.58 → 2394.64] And of course, they have S3 compatible object storage.
[2395.04 → 2397.26] And the benchmarks are out there.
[2397.86 → 2404.86] Linde performs better and faster than those hyperscalers that want to lock you in to their crazy esoteric platform.
[2404.86 → 2409.20] And Linde has free 100% human support.
[2409.74 → 2415.56] No handoffs, no tiers, 24-7, 365 support you can actually talk to.
[2416.04 → 2419.40] And because they've been doing this for nearly 19 years, they know how to build it right.
[2419.60 → 2425.76] With 11 data centres around the world and 99.99% uptime and over a million customers.
[2426.34 → 2428.00] And Linde is their own ISP.
[2428.34 → 2430.12] So they kind of get infrastructure too.
[2430.12 → 2434.98] It could also be a great alternative to some of those hyperscalers.
[2435.24 → 2438.62] Maybe you need a little hybrid action in your cloud, want to diversify a bit.
[2438.84 → 2439.66] It's a great option too.
[2440.30 → 2442.26] Build a portfolio or support your business.
[2443.08 → 2445.98] Linde can do it all, and you can support the show while trying it out and learning something.
[2446.50 → 2449.88] Just get started by going to linode.com slash SSH.
[2450.10 → 2451.28] That's how you support the show.
[2451.72 → 2452.78] That's how you get the 100 bucks.
[2453.28 → 2455.96] Linode.com slash SSH.
[2455.96 → 2461.52] Now Tom H writes in with some Orange Pi feedback.
[2462.06 → 2465.38] I've been using a mixture of non-Raspberry Pi since around 2016.
[2465.80 → 2469.52] I started with an Orange Pi 1 and an Orange Pi PC.
[2470.06 → 2473.00] They were pretty much on par with the Raspberry Pi 3B at the time.
[2473.14 → 2476.28] I think they were about 10 or 15 pounds each on eBay.
[2477.06 → 2482.34] Since I have moved on to other boards like the Friendly Arms stuff and the Pine64 boards,
[2482.34 → 2487.44] the trouble I have with the Orange and Friendly Arms were the images you're provided by them.
[2487.80 → 2491.02] They're often on an old kernel and often not updated.
[2491.40 → 2493.62] Some manufacturers do a much better job than others.
[2494.08 → 2496.06] Then I found Arabian.
[2496.66 → 2500.76] Arabian is an amazing project and the work they do to support a lot of these,
[2501.00 → 2504.12] air quotes, non-Raspberry Pi SBCs.
[2504.38 → 2508.40] I also found new boards on their downloads page that I never even knew existed.
[2508.84 → 2510.90] I highly, highly recommend Arabian.
[2511.22 → 2511.86] Thanks, Tom.
[2512.34 → 2517.26] Josh, I'm curious what OS you prefer on the Raspberry Pis and if you have much experience with Arabian.
[2517.80 → 2521.20] I have not worked with Arabian, so I can't give a comparison there.
[2521.44 → 2526.68] I've run pretty much every OS under the sun in the last 10 years on any Raspberry Pi I can get a hold of.
[2527.24 → 2530.94] And again, back for the community's sake, it's going to be Raspbian.
[2531.06 → 2533.64] Or what used to be Raspbian now is Raspberry Pi OS.
[2534.20 → 2537.06] Pop OS is interesting on the Raspberry Pi,
[2537.06 → 2542.36] but by default, if you just want to be able to throw a Raspberry Pi at somebody and get them started,
[2543.18 → 2544.08] just go with the default.
[2545.04 → 2545.86] Like a brick.
[2545.98 → 2549.28] Not all of us have enough Pis to throw around, Josh, but yeah, I get what you're saying.
[2550.24 → 2552.90] So to that point, I mean, I help run a hacker space,
[2552.98 → 2554.72] so I'm trying to get people into technology.
[2555.02 → 2559.46] If they show interest, being able to feed that by throwing them a Raspberry Pi.
[2559.46 → 2565.74] I've also, although I think Raspbian or Raspberry Pi OS is a good idea for that kind of scenario,
[2565.74 → 2571.94] but I've also found that the Ubuntu team has put a lot of hard work into making Ubuntu LTS run really well on the Pi.
[2572.40 → 2576.08] Arabian, though, it's great for that outside the Raspberry Pi ecosystem,
[2576.46 → 2580.68] like Tom here writes, you know, the Orange Pi and some of those other boxes
[2580.68 → 2585.96] where it really feels like Arabian is trying to go above and beyond to include those devices in its support.
[2585.96 → 2591.90] So I think it's nice to get a pro Arabian user on the air because none of us are really one.
[2592.76 → 2594.30] How about we move to Mads here?
[2594.42 → 2597.68] Mads writes in about upgrading Home Assistant databases.
[2598.14 → 2598.76] Thanks for the show.
[2598.84 → 2599.68] Gives me a lot of ideas.
[2599.80 → 2602.28] I've been looking into Home Assistant for a while now, and I want to get started.
[2602.74 → 2605.68] I've decided to go to the official Docker container for my setup,
[2605.94 → 2610.44] and I'm running each add-on as a separate container, like Frigate, ESPHomeDashboard, etc.
[2611.10 → 2613.66] You guys seem to talk about a lot of things related to Home Assistant,
[2613.66 → 2618.52] so I was wondering, have you had any issues with just using the built-in SQLite database,
[2619.30 → 2621.68] or have you already migrated to something like MariaDB?
[2622.32 → 2623.14] Thanks for the info.
[2623.46 → 2624.42] I'll be honest, Mads.
[2624.42 → 2627.12] It's not something I give a great deal of thought on a daily basis.
[2627.58 → 2633.54] I think, therefore, that means I must be using the SQLite database, just the default one.
[2633.54 → 2638.86] And occasionally, if things go a bit wonky, I'll just delete the database file.
[2638.96 → 2642.00] I don't really need to know what my front door was doing three years ago,
[2642.20 → 2644.70] whether it was open or shut for three seconds or not.
[2644.92 → 2648.88] I mean, there are some things I think it would be nice to do data samples on,
[2649.10 → 2651.54] like temperature trends and stuff like that,
[2651.72 → 2654.60] are kind of nice once in a while to look back at,
[2654.68 → 2657.64] but they're really not that important for me.
[2657.64 → 2660.14] So my answer is I stick with the default.
[2660.66 → 2661.30] I think I have too.
[2661.64 → 2666.46] The only thing that would maybe make me change that is if we saw significant improvements,
[2666.46 → 2669.72] and we have seen some pretty good improvements in some of the more recent Home Assistant releases,
[2669.86 → 2676.04] but like something in the energy metrics area where I'd really want to keep that data for a while
[2676.04 → 2679.12] might kind of nudge me to improve the database,
[2679.20 → 2682.36] because I really think it's going to be metrics that, you know,
[2682.98 → 2684.66] where you're going to feel the performance issue.
[2684.74 → 2686.16] And otherwise, I kind of agree, Alex.
[2686.16 → 2687.46] But here's the thing.
[2687.94 → 2693.04] You can still use SQLite, but ship out everything into Influx anyway.
[2693.42 → 2694.52] Yeah, true, true, true.
[2694.82 → 2695.08] Right.
[2695.16 → 2699.38] That is a time series database which is designed for exactly that use case.
[2699.76 → 2699.90] Yeah.
[2700.22 → 2703.30] And I'm only three weeks into running mine, so I haven't had that experience yet.
[2703.30 → 2705.36] So I'm also just running the built-in.
[2705.64 → 2707.46] Yeah, I mean, mine's a couple of years old.
[2707.78 → 2709.08] It's not really a big issue.
[2709.66 → 2712.26] And the Home Assistant team in the last two releases
[2712.26 → 2716.04] has made significant improvements in the database performance.
[2716.24 → 2718.56] So I think it's getting even faster with SQLite.
[2719.22 → 2722.94] Marcel boosted in seven days ago with 500 SATs, wishing me to get better soon.
[2723.18 → 2723.74] Thank you, Marcel.
[2723.84 → 2724.68] It must have been the reason.
[2724.98 → 2726.10] We all wished it to.
[2726.24 → 2727.20] Not just Marcel.
[2727.50 → 2727.94] Oh, okay.
[2728.04 → 2728.24] All right.
[2728.30 → 2728.54] Okay.
[2729.88 → 2731.44] What do you think this next one is?
[2732.44 → 2733.24] FunDeckHermit?
[2734.30 → 2735.02] FunDeckHermit.
[2735.10 → 2735.26] Yeah.
[2735.26 → 2736.46] I got it, huh?
[2736.84 → 2743.84] With Elite Boost 1337, with a tip of the week, the Authentic, which is Authentic,
[2744.50 → 2746.58] makes single-sign-unaccessible for the home user.
[2746.68 → 2750.82] You can use LDAP, OAuth 2, maybe even integrate with a reverse proxy.
[2750.94 → 2752.88] I've been using it for eight months without any problems.
[2753.02 → 2753.56] Love the show.
[2753.96 → 2755.06] Greetings from Sylvania.
[2755.78 → 2759.08] So Authentic is something I've been wanting to look at for a very long time.
[2759.08 → 2765.92] I started using one of its other competitors, which is not really Authentication, but it's
[2765.92 → 2767.62] a project called Australia.
[2767.92 → 2772.54] Essentially, this does like a transparent authentication proxy in front of applications.
[2773.32 → 2778.36] But I think where Authentic makes a lot more sense is for applications that have integration
[2778.36 → 2783.40] with LDAP and OAuth and that kind of thing, which unfortunately is not all of them.
[2783.40 → 2789.18] And I think that really is Authentic's biggest issue is you have to rely on the underlying
[2789.18 → 2795.62] application to support some kind of, for want of a better phrase, proper authentication
[2795.62 → 2798.44] mechanism in order to be able to use it with Authentic.
[2799.16 → 2804.50] So if you've just got a simple HT access authentication, for example, then you're not going to see any
[2804.50 → 2805.66] benefit with Authentic.
[2805.84 → 2809.70] But there are other apps, you know, Gift is one of them, Nextcloud.
[2809.70 → 2815.04] There's a few that we run right in this community that will absolutely integrate very well with
[2815.04 → 2815.60] Authentic.
[2816.14 → 2818.82] So thanks for writing in, Funded Hermit.
[2819.26 → 2820.20] What a name.
[2820.98 → 2822.78] I need to give it a look.
[2823.84 → 2829.40] I wanted to ask Josh what he does for authentication, given he's an elite hacker DEFCON man.
[2829.86 → 2831.02] That's a good question.
[2831.18 → 2831.32] Yeah.
[2831.42 → 2833.46] Wiping, formatting and reinstalling, man.
[2833.46 → 2839.98] Um, so when it comes to trying to build that out, even for, for home use versus for a hacker space
[2839.98 → 2843.82] use versus for what we're going through and doing at DEFCON, I would say our three different
[2843.82 → 2845.00] situations there.
[2845.06 → 2847.92] I've run free IPA in the past, and I've been pretty happy with that.
[2848.14 → 2850.22] And for our hacker space, that's worked out pretty well.
[2850.62 → 2856.04] The issue is when it comes to getting other people to support it, it's been pretty straightforward
[2856.04 → 2860.68] when we were trying to do it from like my location here in the desert down to like somebody
[2860.68 → 2861.44] else in San Diego.
[2862.06 → 2866.10] It's been interesting to make sure that we have the mirroring on that working correctly.
[2866.48 → 2870.64] Otherwise, honestly, if you have a Synology, why aren't you just using the one that's built
[2870.64 → 2871.12] into that?
[2871.42 → 2875.80] And honestly, for my mom and dad's business, that's what we've just gone through and done
[2875.80 → 2876.92] there because it's built in.
[2877.16 → 2877.58] Make it easy.
[2878.30 → 2878.74] Make it easy.
[2878.84 → 2881.42] I think that is absolutely the right advice.
[2882.10 → 2886.18] So Cast Plan writes in with 3,690 SATs.
[2886.56 → 2887.20] High signal.
[2887.58 → 2888.08] Great show.
[2888.34 → 2888.60] Thanks.
[2889.30 → 2890.46] I think you liked last episode.
[2890.46 → 2894.44] High signal is like a good compliment in the Booster gram world.
[2895.00 → 2895.92] That's rare.
[2896.24 → 2896.36] Yeah.
[2897.00 → 2900.02] The Golden Dragon boosted in seven days ago with a row of ducks.
[2900.32 → 2902.64] Says it was a great show with Techno Tim.
[2902.90 → 2903.82] It absolutely was.
[2903.88 → 2908.52] I had a blast and I really hope we didn't bore you all too much talking nonstop about
[2908.52 → 2910.88] Kubernetes for an hour, but I had a great time.
[2911.06 → 2915.02] I found it educational, and I don't really even have a use case for Kubernetes myself, but
[2915.02 → 2919.50] it's still something I like to keep a, you know, a kind of, at least not an ear on,
[2919.56 → 2923.20] but kind of, some, at least an informed background on, I suppose.
[2923.28 → 2924.64] And the conversation was perfect for that.
[2924.64 → 2931.40] Now, Turquoise Fox writes in with a controversial, is this controversial piece of feedback?
[2931.90 → 2936.60] I mean, I don't, probably not in our audience because there's probably others that feel this
[2936.60 → 2936.84] way.
[2937.12 → 2937.80] I would imagine.
[2938.02 → 2939.86] We've, this is an issue we've come up with before.
[2940.48 → 2943.00] And Turquoise technically boosted in twice for this one.
[2943.00 → 2948.76] So I combined them to 6,269 sets, but some Discord hate here.
[2948.88 → 2949.48] Boo Discord.
[2949.72 → 2949.86] Yay.
[2949.96 → 2950.38] Matrix.
[2950.50 → 2951.82] When will self-host it be on Matrix?
[2952.58 → 2953.66] And we get this sometimes.
[2953.66 → 2959.38] We know we've explained it before on the show, but sometimes there, we try to walk this balance
[2959.38 → 2964.94] between the perfect being the enemy of the good enough and Discord took off like a weed.
[2965.22 → 2969.40] There's a really great community over there and there's more good than there is negative
[2969.40 → 2970.20] as a result.
[2970.20 → 2976.22] And because really the network effect, it has been very beneficial to just have a strong
[2976.22 → 2978.08] Discord presence for the show too.
[2978.14 → 2978.98] It's helped the show a lot.
[2979.38 → 2980.90] Things like this London meetup, right?
[2980.90 → 2987.00] They are birthed in that Discord, but there is two Matrix self-hosted rooms.
[2987.12 → 2991.52] They're not crazy busy, but they are available on the Jupiter Broadcasting Matrix for those
[2991.52 → 2996.20] of you, because like Turquoise here doesn't basically don't want to put a phone number
[2996.20 → 2998.00] in or put information into the Discord service.
[2998.26 → 2999.92] And there's going to be people out there that feel that way.
[2999.92 → 3000.62] I totally understand.
[3000.62 → 3006.16] So I've got an interesting take on this because if not this community, what community, right?
[3006.34 → 3008.66] Because this would be the one to be doing it.
[3008.76 → 3013.44] So with our hacker space, with our folks that we work with at DEF CON, it's like, hey, we
[3013.44 → 3015.06] want this to be more private, more secure.
[3015.30 → 3019.86] But the barrier to entry is so much higher, let alone just trying to get our own family
[3019.86 → 3020.82] members onto it.
[3021.06 → 3022.54] That's where it gets hard.
[3022.54 → 3028.08] And until we make it easier for folks to onboard with that, it's much like I think that there
[3028.08 → 3034.32] are better signal or messaging, secure messaging like signal versus wire.
[3034.56 → 3037.88] But the problem is, what's your onboarding process?
[3038.14 → 3042.14] If it's not seamless, if it's not easy, you're not going to get as many people on.
[3042.32 → 3047.04] So depending on your paranoia, depending on you actually having to do threat modelling for
[3047.04 → 3050.68] yourself and your community, you're going to land in different areas.
[3050.68 → 3055.54] And I could see too, like if this was a podcast that was doing, you know, war crime journalism
[3055.54 → 3058.44] in Ukraine, maybe we wouldn't want to be on Discord, right?
[3058.50 → 3061.08] Maybe we'd want to be using really secure encrypted communications.
[3061.08 → 3065.36] But at the end of the day, this is a podcast and everything we produce is ultimately public
[3065.36 → 3065.68] too.
[3066.30 → 3068.70] We've almost got 5,000 people in the Discord now.
[3068.82 → 3074.88] And I really don't think we would have so many people in a Matrix server.
[3074.88 → 3081.96] I may well be wrong, but my feeling is that the friction to joining a new Discord server
[3081.96 → 3086.50] for those that are already using Discord, which at this point is a lot of people that listen
[3086.50 → 3087.52] to this podcast, right?
[3087.60 → 3091.28] The cross-section Venn diagram is quite large.
[3092.04 → 3097.40] The friction to joining yet another Discord server is quite low compared to signing up for
[3097.40 → 3101.46] Matrix and then having the right client and then waiting whilst Chris and Was add more
[3101.46 → 3102.42] RAM to the box.
[3102.84 → 3111.40] And so for me, I stand by what we said originally, that the mission of the chat server, in this
[3111.40 → 3119.34] case, it's a Discord server, is not necessarily to be the ultimate in self-hosting dog food,
[3119.56 → 3120.58] for want of a better phrase.
[3120.58 → 3125.84] And it's to further the mission by allowing people to collaborate and ask questions in
[3125.84 → 3126.88] a friction-free way.
[3127.50 → 3131.60] Yeah, it's sort of like we stream on Peer tube now, but we're also streaming on YouTube and
[3131.60 → 3134.20] Twitch because we want to be where the audience is at.
[3134.74 → 3137.08] And just like with Matrix, we have a self-hosted solution.
[3137.22 → 3138.46] That is something we self-host.
[3138.72 → 3140.64] I'm long on Matrix, right?
[3140.82 → 3143.92] I feel like give another five years, it's just going to continue to grow.
[3144.04 → 3148.38] When we first launched our Matrix server, we had 200 users a year ago, you know?
[3148.38 → 3153.98] So today, we have like 2,500 users and our largest room is like 1,300 people.
[3154.34 → 3158.30] But it's not as big as the self-hosted Discord because the Discord network effect is so much
[3158.30 → 3158.62] larger.
[3158.96 → 3161.98] But I am very happy with that kind of growth for a year.
[3162.30 → 3166.40] And I imagine if that continues, at some point, Matrix will be a real big part of what we
[3166.40 → 3166.62] do.
[3166.78 → 3171.52] And it is already for me, it's already the it's out of all the different platforms
[3171.52 → 3175.30] that I'm available on, Matrix is the one that I hang out on the most.
[3175.30 → 3179.30] I do check those self-hosted Matrix rooms from time to time if you want to jump in there,
[3179.36 → 3179.68] Turquoise.
[3180.08 → 3182.20] One day, one day we'll make the switch.
[3182.34 → 3183.32] Just, just not yet.
[3183.92 → 3190.82] And I think it's going to come soon because we had some Red Hatters jump from Red Hat over
[3190.82 → 3197.60] to the Element community and seen some interviews online from Eric, the IT guy, with what they're
[3197.60 → 3199.74] doing and how they're onboarding it easier.
[3199.90 → 3201.28] They're making those bridges happen.
[3201.60 → 3203.98] If you throw a couple bucks at them a month, it's making it a lot easier.
[3203.98 → 3208.46] To me, it made me go and say, huh, it might be time to go relook at that now.
[3208.76 → 3209.18] That's true.
[3209.60 → 3212.48] Red Hat does, is getting a bigger and bigger Matrix present too.
[3212.56 → 3216.86] Not just, not just the team people over at the Element stuff, but like Red Hat itself,
[3217.30 → 3221.10] I am in, I'm in a couple of Red Hat rooms actually on Matrix.
[3221.78 → 3224.40] So I, I may be in rooms that you guys are not in.
[3224.48 → 3225.22] How weird is that?
[3225.36 → 3226.06] I'm not surprised.
[3226.06 → 3233.66] We do have one last boost that came into the show from Sea moon or maybe Simon, perhaps.
[3234.00 → 3235.44] One day ago, 500 SATs.
[3235.94 → 3238.26] Hey guys, I recently learned about the Fountain FM app.
[3238.38 → 3239.68] That's one of the new podcasting apps.
[3239.98 → 3240.98] So here's some SATs from you.
[3241.02 → 3242.10] I got a question though.
[3242.64 → 3243.60] And this is a good question.
[3243.66 → 3244.58] I thought a lot about this.
[3244.58 → 3249.86] He writes, when you got the Bitwarden one-time authentication code token that you can put
[3249.86 → 3253.74] in when you're, when you have the tokens at Bitwarden, he says, isn't that sort of against
[3253.74 → 3258.52] the idea of a two-factor authentication to store that code right next to the password?
[3259.10 → 3259.92] Greetings from Germany.
[3260.34 → 3261.12] Keep up the great work.
[3261.74 → 3262.04] Simon.
[3262.44 → 3262.64] Why?
[3262.80 → 3263.04] Yes.
[3263.18 → 3263.82] Yes, it is.
[3264.00 → 3268.10] But I refer you to an argument I made with the in the last episode with Tim.
[3268.88 → 3272.98] It's sometimes about just not being the tallest nail, right?
[3273.10 → 3278.56] If you have two-factor turned on, on your Amazon account, anybody that's got your password,
[3278.94 → 3282.76] assuming it's not your Bitwarden password, of course, is going to look at that account
[3282.76 → 3283.84] and go, there, can't be bothered.
[3284.08 → 3285.66] Move on to the next one that doesn't have it.
[3285.78 → 3286.48] And that's it.
[3286.54 → 3288.82] That really, that's all two factors good for, in my opinion.
[3289.12 → 3294.00] And so for me, the convenience of having it in Bitwarden and be just a paste away as
[3294.00 → 3299.76] part of the keystrokes that I autofill with, that risk profile for me is worth it.
[3299.84 → 3305.26] Now, there are a couple of places that I remain phone two-factor authentication.
[3305.58 → 3306.82] So GitHub is one of them.
[3307.04 → 3308.46] My Nextcloud is another one.
[3308.88 → 3313.68] There's a couple that I keep out of Bitwarden, Bitwarden itself being a great example.
[3314.46 → 3319.68] Most of the time, I keep things in Bitwarden just because it's easier, which is not the
[3319.68 → 3322.16] the best security answer, but that's the reality.
[3322.66 → 3323.60] I mean, I like your answer, though.
[3323.60 → 3324.30] I think it makes sense.
[3324.36 → 3326.02] What is the threat model exactly, though?
[3326.14 → 3327.98] I mean, it seems like it's a physical one, right?
[3328.28 → 3331.26] Isn't it mostly a physical threat model with that situation?
[3331.36 → 3334.04] Which, you know, I think that's a real balancing act there.
[3334.18 → 3335.76] You got to decide what you're going to protect against.
[3335.86 → 3340.04] And if you're in a scenario where somebody could physically take advantage of that, they
[3340.04 → 3341.74] may also have access to your phone.
[3342.58 → 3343.30] Physical access, man.
[3343.42 → 3347.06] Once you got physical access and if your kid can then go through and buy stuff from Amazon
[3347.06 → 3351.14] or from whatever else, do you want that all in one device and one app?
[3351.20 → 3352.58] Yeah, that's true.
[3352.58 → 3356.92] I think Alex made a perfect point, though, that he did his risk model to figure out that's
[3356.92 → 3358.02] not his use case.
[3358.16 → 3360.46] For other people in other situations, that might not be.
[3360.94 → 3361.88] Wait till his daughter's older.
[3363.38 → 3368.54] But my Bitwarden authenticates with my face on my phone or my thumb on my MacBook.
[3369.08 → 3373.08] Like, unless she's chopping my thumb off when I'm sleeping, which I'll probably notice.
[3373.96 → 3378.62] She's not going to unlock my Bitwarden unless she literally knows the password, which one day
[3378.62 → 3379.48] she will, I'm sure.
[3379.62 → 3384.96] But if you'd like to send a boost into the show, go get a new podcast app at newpodcastapps.com.
[3385.04 → 3386.12] Load your wallet up with a few SATs.
[3386.20 → 3386.76] They're on sale.
[3387.40 → 3389.82] So it's a great time to boost the dip and send it in.
[3390.32 → 3392.64] What is Bitcoin with a price check today?
[3393.70 → 3397.74] Not that I'm looking, but $20,000, $16.19.
[3398.08 → 3398.90] I don't know why you'd ask that.
[3398.90 → 3400.60] Well, it's above $20,000.
[3400.70 → 3402.76] I suppose that's considered a W these days.
[3403.22 → 3406.84] Let's be honest, not for long, but that's, don't get me into the doom and gloom of the
[3406.84 → 3407.82] economy that's coming.
[3408.16 → 3410.76] So it's a great time to boost the show.
[3410.88 → 3411.68] I'll just put it that way.
[3412.16 → 3413.70] It's a long-term investment, right?
[3413.78 → 3414.20] Just hold.
[3414.38 → 3414.78] That's right.
[3415.42 → 3417.50] Put your boost to work by getting them cheap today.
[3417.78 → 3418.06] Hold.
[3418.24 → 3418.52] Hold.
[3418.96 → 3419.56] Hold indeed.
[3420.24 → 3423.02] And also, just a major thank you to our members.
[3423.54 → 3426.20] Our site reliability engineers make the show possible.
[3426.20 → 3429.10] And as a thank you, we give you an ad-free feed of the show.
[3429.20 → 3429.86] So no ads.
[3430.52 → 3435.06] And we are working, still doing the plumbing on live versions.
[3435.16 → 3436.36] We'll have a live feed as well.
[3436.42 → 3437.74] You'll have both options as a member.
[3438.18 → 3440.90] And I'm just kind of in the early stages with that.
[3441.06 → 3445.36] So if you are an RSS generator wizard, reach out.
[3445.66 → 3450.40] I could use your help on that at self-hosted. Show slash SRE if you want to sign up.
[3450.66 → 3453.42] And then you can also support all the shows on the network.
[3453.88 → 3455.14] Become a member for all the shows.
[3455.14 → 3458.88] Get all the special features, all ad-free, at jupyter.party.
[3459.12 → 3464.42] And one of those nice features is a self-hosted bonus post show, which will be coming up in
[3464.42 → 3464.98] just a little bit.
[3465.38 → 3468.02] Going to talk about yet another golf that I've purchased, I think.
[3468.32 → 3468.90] I can't wait.
[3469.12 → 3473.32] I've specifically made Alex wait to tell me, so that way I can hear about it in the post
[3473.32 → 3473.48] show.
[3473.92 → 3475.14] I bought number seven.
[3475.70 → 3475.82] Yeah.
[3477.24 → 3478.62] It's becoming a problem.
[3479.52 → 3481.34] We're going to need dinner, have an intervention.
[3481.34 → 3486.34] Now, I really do want to see all of your smiling faces in London on August the 5th.
[3486.58 → 3490.12] Meetup.com slash Jupiter Broadcasting for all the details.
[3490.54 → 3493.86] And on the day itself, we'll probably be posting in there as well.
[3493.94 → 3497.46] If you're not quite sure exactly where to find us, keep an eye on that meetup page.
[3497.52 → 3499.24] That's where the source of truth is for that.
[3499.66 → 3502.80] To write into the show, it's self-hosted. Show slash contact.
[3502.94 → 3504.34] That's the place to go to get in touch with us.
[3504.62 → 3507.10] And you can find me on Twitter at Ironic Badger.
[3507.22 → 3507.90] How about you, Josh?
[3507.90 → 3511.18] So you can find me at Oscar underscore hawk.
[3511.24 → 3515.02] So that's J-S-K-A-R underscore H-A-W-K.
[3515.44 → 3516.68] Thank you very much for joining us.
[3516.70 → 3517.38] It was a blast.
[3517.96 → 3518.28] Absolutely.
[3518.46 → 3518.90] My pleasure.
[3519.14 → 3519.90] Thanks for having me on, guys.
[3520.30 → 3520.84] It was a lot of fun.
[3520.90 → 3524.98] We'll put a link to your GitHub for all the projects for the Raspberry Pi, as well as your
[3524.98 → 3526.00] social in the show notes.
[3526.36 → 3529.60] You can find the podcast on Twitter at selfhostedshow.
[3529.70 → 3530.70] I'm at Chris LES.
[3531.04 → 3534.90] And don't forget, we're doing the show live on Wednesdays now, every other Wednesday.
[3534.90 → 3538.64] You can get your local time and date at jupiterbroadcasting.com slash calendar.
[3538.80 → 3542.78] And you can catch video replays of the show at Jupiter.tube.
[3542.90 → 3545.56] As also, you can catch the live stream there.
[3545.66 → 3547.98] It's just like one place to remember, Jupiter.tube.
[3548.24 → 3552.70] Whilst I'm in England, that might go on hiatus for a week or two, but we'll see.
[3552.86 → 3553.16] We'll see.
[3553.46 → 3555.94] Yeah, there's always trickiness when you're travelling.
[3556.14 → 3557.76] So we'll have to be flexible.
[3557.96 → 3561.16] One of the places I'm staying, the primary internet is Starlink.
[3561.16 → 3563.94] So who knows if it's cloudy?
[3564.42 → 3567.92] It depends on if there are any obstructions and if Dish turns on their 12 gigahertz
[3567.92 → 3569.18] interference stuff.
[3569.58 → 3570.38] Right, right.
[3570.90 → 3572.36] So thanks for listening, everybody.
[3572.72 → 3574.96] That was self-hosted. Show slash 74.
