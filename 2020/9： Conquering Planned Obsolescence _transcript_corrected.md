[0.00 → 6.22] In my searches for understanding how to integrate different temperature sensors and gadgets into Home Assistant,
[6.80 → 9.58] I kept coming across the Intermittent Tech channel.
[9.90 → 16.34] And when Alex suggested that we chat with Pindar today, I thought it was a great opportunity to really geek out.
[16.62 → 18.78] Pindar, welcome to the Self-Hosted program.
[19.14 → 19.80] Thank you very much.
[20.18 → 21.26] Thank you for joining us.
[21.26 → 25.66] Alex and I are both impressed with the amount of output that you have on your channel,
[25.66 → 31.02] but also the depth of detail that you seem to go into, like project after project.
[31.16 → 33.66] You must put a lot of work into that.
[34.30 → 41.46] Yeah, it takes up a lot of my free time, but I'm, I guess a geek you would call it by heart.
[41.72 → 48.34] And I like finding, going to the bottom of things and then trying to explain it to others so they can do it also.
[49.08 → 50.84] Well, I appreciate that.
[50.84 → 56.72] Well, it's kind of the ground basis why it started as a blog, and then it transitioned into a YouTube channel.
[56.94 → 57.46] So, yeah.
[57.94 → 61.02] There are some things that just don't translate into text, huh?
[61.36 → 61.56] Yeah.
[61.96 → 62.48] Very true.
[62.72 → 64.30] And the other way around too.
[64.60 → 69.06] So, like, heaps of code do better on a blog.
[69.20 → 70.44] So now I do kind of both.
[71.28 → 74.12] I appreciate that because I agree completely with that.
[74.22 → 76.48] And Alex has been striking a good balance with that himself.
[76.48 → 81.52] So, Alex, was it the recent home server series that put Quin dor on your radar this time?
[81.84 → 82.54] It was, yeah.
[82.66 → 85.48] So, you've been building a server lately, haven't you?
[85.60 → 90.36] With ZFS and doing some stuff with Ry zen and Proxmox and all that kind of stuff.
[90.86 → 91.06] Yeah.
[91.28 → 95.26] My old server was about six years old now, I think.
[95.84 → 100.18] And there were some disks starting to fail, and I started to have some other problems.
[100.18 → 106.36] And one of the ways we noticed that is I actually run Demotic and Home Assistant still at both.
[107.04 → 112.14] And, well, at some point the lights didn't turn on because a disk was crashing, stuff like that.
[112.20 → 114.86] So, I thought, okay, time to build a new one.
[115.28 → 117.64] That's the side of self-hosting people don't talk about very often.
[117.80 → 119.10] It's when it breaks, it's your fault.
[119.18 → 119.84] You've got to fix it.
[120.10 → 121.06] Sometimes it's an opportunity.
[122.28 → 122.72] Yeah.
[122.76 → 124.38] So, this server looks really sweet.
[124.54 → 126.80] It's a 100 terabyte, 10 gigabit server.
[126.80 → 130.38] That's the branding on all of your videos.
[130.84 → 138.18] How did you come to some of the decisions around choosing the hardware and Proxmox and stuff like that?
[138.40 → 141.36] For me, the server is kind of multipurpose.
[141.68 → 144.12] I have my YouTube channel, as we just mentioned.
[144.46 → 146.20] And for that, I need a lot of storage.
[146.42 → 150.34] I generate about six to eight terabytes of footage, raw footage a year.
[150.34 → 157.34] And I also like to live edit from the server, but my old server wasn't really up to that.
[158.16 → 163.56] And next to that, I run my home automation VMs, like with Demotic and Home Assistant from it.
[163.78 → 168.42] And for work, I also run some testing environments and things like that.
[168.54 → 171.32] So, I kind of wanted to renew it.
[171.58 → 174.68] And more cores is better in that regard.
[174.68 → 179.06] And the new Ry zen 3000 series was launching.
[179.88 → 188.02] So, I was like, okay, let's move my old Ry zen 1700 desktop to my server platform.
[188.26 → 194.32] And then buy a new Ry zen 3000 series and basically buy a new desktop, but get a new server out of it.
[194.68 → 195.96] Now, have you found the Ry zen switch?
[196.10 → 204.18] Because Intel these days, I don't know if you've seen the latest videos from like Jay's Two Cents and Linus Tech Tips and all that.
[204.18 → 206.76] But they are beating up hard on Intel these days.
[207.10 → 211.38] Yeah, well, this kind of started during the Ry zen 1000 series.
[211.58 → 213.88] So, as I said, I was one of the first guys to get it.
[213.96 → 221.38] And I did a whole series called The Road to Ry zen, getting the first eight cores, where I came from a quad-core.
[221.70 → 225.20] And Intel, well, they quickly followed with six and eight cores.
[225.20 → 236.08] But now I have a 12 core and Intel basically has nothing that can compete with it, even in the areas where they used to be better.
[236.26 → 243.26] So, in IPC and power usage and stuff like that, especially the Ry zen 3000 series is just better.
[244.02 → 244.42] Yeah.
[244.98 → 248.52] I'm curious specifically which workloads you see a big improvement on.
[248.80 → 249.88] Is it encoding work?
[249.88 → 253.96] What types of CPU loads are you using that benefit?
[254.34 → 257.66] Well, take my video rendering from the Intel box I had before.
[257.90 → 259.50] And granted, it was a few years old.
[259.94 → 262.30] That basically became four times as fast.
[262.50 → 263.24] Oh, that's wonderful.
[263.64 → 270.54] Yeah, from a four and a half gigahertz quad-core to basically a four and a half gigahertz with higher IPC 12 core.
[270.54 → 275.64] And the CPU was about the same during that era in price.
[276.58 → 279.84] And for on the server, that's now an eight core server.
[280.10 → 284.02] Well, like five years ago, that would have been ultra-high end.
[284.14 → 286.36] And now it's just like, oh, it's eight cores.
[286.46 → 286.88] It's okay.
[287.76 → 289.00] That is something, isn't it?
[289.30 → 295.30] And you said something in there that piqued my interest because it's something we've attempted to various degrees of success.
[295.30 → 299.94] Because you're live editing over that 10 gigabit connection you've built on that server.
[300.58 → 301.60] How is that?
[301.68 → 306.98] And did you have to do any particular tweaking to your network, your switches in general, your network car configuration to make that work?
[307.10 → 315.36] Well, it started in the design of the server, reusing a desktop platform, but wanting to have high bandwidth capabilities.
[315.36 → 317.44] You need to take a lot into account.
[318.00 → 322.42] So, for instance, a desktop platform is mostly limited in regard to PCIe bandwidth.
[322.42 → 330.82] So, I did some research and made some videos about that and how to look up how many PCIe lanes there are in your motherboard and how they're distributed.
[331.08 → 337.78] And then how you should basically distribute your cards over the available PCI slots so that there won't be a bottleneck there.
[338.64 → 343.38] And after that, I run Proxmox with ZFS under it.
[343.72 → 349.30] And I did a little bit of tuning in regard to flash-based caching in ZFS.
[349.30 → 361.64] So, basically, on the server, the project I'm editing, after a little while, especially if I'm ingesting footage, is basically all on the cache drive, which is an NVMe drive.
[362.06 → 365.50] So, I can basically edit at full 10 gig speeds.
[366.28 → 376.74] And although that's still slower than locally, especially the latency that it doesn't come from a hard disk, and, well, one gigabyte a second, that's plenty for us fast to edit video.
[376.74 → 378.90] I got to say, you're making me want to try it again.
[379.14 → 379.74] That's great.
[380.14 → 382.76] And then the storage is taken care of.
[382.82 → 384.66] You're investing your money in one place.
[384.78 → 387.08] You can focus your performance on the server.
[387.50 → 388.10] It's really clever.
[388.50 → 392.66] Yeah, but also things around it like backup scripts and stuff like that.
[392.80 → 397.52] We're all kind of lax in setting that up on our desktop or workstation and stuff like that.
[397.52 → 401.22] But on my server, I basically have directories where everything goes.
[401.44 → 409.34] So, I have some scripts running which make backups to my, as I call it, DIY cloud backup solution, which I set up a few years ago.
[410.00 → 411.24] And that always runs.
[411.34 → 415.02] That just runs during the night when my desktop is off, but my server is on.
[415.24 → 418.82] So, I know if my stuff is on there, it's good.
[418.82 → 422.48] Because using ZFS, you have the advantage of stuff like datasets.
[423.14 → 427.14] And do you make use of anything like ZFS Send for remote backups?
[427.40 → 430.12] Or do you even worry about off-site backups?
[430.54 → 433.84] Yeah, I don't make use of ZFS Send or Receive.
[433.96 → 440.28] But I do off-site backups using basically a DIY cloud backup solution I built a few years ago.
[441.10 → 444.74] Do you guys remember a backup service called Crash Plan?
[444.74 → 445.72] Oh, yeah.
[445.80 → 447.82] With a horrible Java client and everything.
[447.98 → 448.12] Yep.
[448.24 → 448.54] Wonderful.
[450.08 → 451.04] Okay, granted.
[451.28 → 457.94] But they were the first to offer online backups with an unlimited plan basically for like a few bucks a month.
[458.26 → 461.74] So, I had been using that for a few years and it was great.
[461.98 → 464.12] And they allowed you to back up 10 PCs.
[464.50 → 471.12] So, I backed up my mother's and father's PC and my sister's and mine and my laptop and some VMs I had.
[471.24 → 472.66] And that was all fine.
[472.66 → 474.54] And then they announced, well, we're stopping.
[475.46 → 483.60] And a lot of other cloud hosted backup solutions out there, they're limited to one client only.
[483.94 → 487.74] So, let's say you have Black place and you have their unlimited plan.
[488.16 → 490.96] They limit you to only a single client.
[491.28 → 494.54] But I have like 8 or 10 clients which have all my data.
[494.96 → 495.32] Naturally.
[495.32 → 504.92] So, I basically got together with a few friends and my parents' home just got 500 symmetrical megabits' fibre.
[504.92 → 509.14] So, we basically chipped in, got 5, 10 terabyte hard disks.
[509.46 → 514.66] And I set up a S3 server on their LAN which we could access remotely.
[514.66 → 517.96] And ever since, I've been backing up to that.
[517.96 → 530.12] Because it turns out if you buy 5 times 10 terabytes with like an Atom-based server and run Mini for S3, you can use all kinds of backup tools out there which talk S3.
[530.12 → 532.12] I'm currently using RUSTIC.
[532.92 → 535.26] And backup anything you want to that.
[535.48 → 541.52] And if you share that with a few friends, it's even a lot cheaper than the cloud if you look at it for like 5 years.
[541.52 → 541.92] Absolutely.
[543.42 → 550.18] I love that you chose to essentially implement self-hosted S3 services simply because of the client compatibility.
[550.38 → 552.14] That's probably a similar direction I would have considered going.
[552.20 → 552.58] Because you're right.
[552.64 → 554.78] You get so many good backup clients now.
[555.88 → 567.78] And yeah, even if once a year around like an annual sale, everybody goes in, and you buy one more hard drive or two more hard drives to add to the mix or whatever your plan is.
[568.10 → 569.44] Have you thought about that long term?
[569.44 → 572.84] Like will you just continue to add disks and add two at a time?
[572.98 → 576.28] Or what's your thoughts around long term five years like you were saying?
[576.90 → 582.76] Well, since I went to ZFS route, expandability isn't really a thing yet.
[583.14 → 590.18] So we went with 5 times 10 terabytes, which would basically be enough for the people involved for those five years.
[590.66 → 592.28] And just don't even have to worry about it then?
[592.60 → 593.28] No, no.
[594.84 → 596.58] That's going to be fine for a few years.
[597.34 → 598.34] That is fantastic.
[598.34 → 604.42] Well, going back to your new server, I don't want to spoil it because it's a series of videos and there are a lot of details in there.
[604.90 → 614.04] But something that Alex mentioned to me that I wanted to sort of not only get you to chat about here on the show, but it kind of is a great example of your attention detail.
[614.84 → 620.76] You spent some time in this home server build specifically paying attention to the PCI lane setup.
[620.76 → 623.06] I'm not really familiar with that part of the series.
[623.12 → 624.38] So could you fill me in on those details?
[624.90 → 635.12] Basically, if you're using a desktop platform, those are basically geared towards having you have everything on board and then having a graphics card.
[635.32 → 637.48] And nowadays, maybe an NVMe SSD.
[637.48 → 641.70] So the PCI lanes, so what is it particularly?
[641.88 → 645.30] Is it just more of them and more performance on the desktop boards versus a server board?
[645.64 → 651.22] Have you heard of the 8x or 16x graphics card situations?
[651.52 → 657.12] Like when you're plugging a graphics card in, it says, I'm running at 8x speed or 16x speed or whatever.
[657.38 → 657.78] Sure. Okay.
[657.78 → 664.40] And those refer to the number of PCIe lanes that are available for bandwidth between that device and the CPU.
[664.98 → 673.82] One of the nice things about Thread ripper is that it has, I forget the exact number, but it has like 30, or it might even be 60 PCIe lanes.
[674.20 → 679.24] Yeah, Thread ripper has 64 and the new generation that launched this year actually has 72.
[679.72 → 680.78] Holy crap.
[680.92 → 686.94] So like an NVMe SSD will generally have an X4 slot.
[686.94 → 692.52] So that will use four of your PCIe lanes, which is why it's so fast, because it's basically plugged directly into the matrix.
[693.16 → 702.06] When you're looking at a desktop platform, like Andreas says, one of the ways they save money is by not including so many PCIe lanes in the chipsets.
[702.56 → 712.10] If you do want to use your desktop chipset and platform for a server, and you want to hook up 24 drives and some NVMe cache and have 10 gigabits,
[712.10 → 723.96] you kind of need to take that into account because just plugging all those cards into your motherboard, it might work, but it'll be very limited in regard to bandwidth you're able to get.
[724.32 → 736.10] So in my case, if I plug in my graphics cards, even into a times one slot, my times four slot will get limited to times two instead of times four PCIe lanes.
[736.10 → 741.84] And that means I can only get about five, six gigabits over my 10 gig leg instead of getting 10.
[742.56 → 746.48] And that's, of course, easily testable using network performance tools.
[746.68 → 755.96] But if this happens to your HBA, which is hooked up to your hard disks, you'll be scratching behind your ears like, why isn't this performing the way I thought it would?
[756.36 → 757.12] But yeah.
[757.12 → 757.60] Okay.
[757.96 → 760.88] Because Ry zen needs a graphics card, right?
[760.96 → 765.06] It doesn't have a built-in GPU of any description like the Intel chips might.
[765.56 → 773.66] So one of the videos Andreas shows, he literally has a GPU that's just garbage just for installing the OS.
[773.66 → 784.86] And then he pulls it out, and he shows the difference between his network card running at six gig a second on a X2 or X4 link and then pulls it out.
[784.98 → 789.36] And then suddenly the extra PCIe lanes are available, and he gets the full 10 gig speed.
[789.56 → 791.08] It's actually pretty interesting to watch.
[791.66 → 792.54] That is fascinating.
[792.94 → 795.80] I love that you took the time to actually demonstrate that too.
[795.90 → 796.76] That's great.
[796.76 → 806.08] As you said, I think it's the details that the bigger YouTubers, they might build something cool, but they don't really have time to work that into videos.
[806.44 → 813.92] So I thought like, okay, let's do a whole series about this so that people who want to do the same actually know what to take into account.
[814.40 → 815.40] Because what's your background?
[816.28 → 821.22] I've picked up in some of the episodes that you might have an enterprise-y, storage-y type background.
[821.36 → 822.14] I'm just curious.
[822.14 → 833.84] I've been doing enterprise storage and mainly backup-focused storage and backup solutions for the past 20 years now in the bigger enterprise situation.
[834.00 → 841.10] So if you have like 500 terabytes or even a few petabytes, and you want a storage solution for that or a backup solution, I'm basically your guy.
[841.64 → 844.58] So what we're doing at home is kind of cute to you, I guess.
[844.58 → 849.38] In some ways, but it also teaches me a lot of stuff.
[849.58 → 853.80] So it's a win-win for both sides, basically.
[854.04 → 859.98] And how do you square off, you know, because in the enterprise everything's about being highly available, which will lead into another topic shortly.
[860.94 → 869.20] You know, how do you square off desktop hardware of, you know, having a single power supply only and stuff like that against that kind of enterprise?
[869.32 → 870.90] Let's have redundant everything.
[870.90 → 875.44] So in the enterprise, time is basically money.
[875.90 → 883.32] So if you can spend more money to not have downtime, basically, that's most often worth it.
[883.46 → 890.34] So having a dual PSU, which will cost you $600 instead of having a single one, which will cost you $200.
[890.34 → 897.30] But being down one-hour costs you $2,000, well, that choice is easy.
[898.00 → 909.42] But at home, $2,000 for like, oh, sorry, $600 for like a dual power supply is a lot of money, where $200 will work fine, except indeed if it fails.
[909.42 → 917.06] But then if it fails, I'll just run out, get a different power supply, plug it in, and I've been down maybe a day.
[917.70 → 922.98] And during that day, well, not $2,000 per hour were lost.
[924.04 → 927.60] So I can't really make the same judgment call.
[927.60 → 931.34] So my time is worth less money than it is in the enterprise.
[931.82 → 933.16] Yeah, it's a good rationale.
[933.64 → 935.92] And I can't argue with it, you know.
[936.08 → 941.74] But one thing that has come up in your latest video is highly available home assistant.
[942.24 → 944.12] I am super interested in this.
[944.22 → 947.50] So please talk us through what that is, first, what that means.
[947.52 → 952.36] Because some people listening to this may not be familiar with what highly available means.
[952.36 → 975.66] In the enterprise, next to having redundant components on a single server, they also have a term HA or called high availability, is that if a complete hardware box would go down, basically there's a cluster of hardware boxes, which then would take over the function or VMs or guests or whatever that other box was running.
[975.66 → 981.68] And then basically started again to make that service it was running or providing available again.
[982.36 → 990.06] So a really simple example of this in the real world would be if you only have one car, that's a single point of failure in your life, right?
[990.16 → 995.92] If your car breaks down, and you can't drive it anymore, suddenly you think to yourself, well, I should have a backup car.
[996.48 → 1001.18] Well, this is what we're talking about in terms of site reliability engineering here.
[1001.56 → 1007.52] It's a bit of a DevOps-y type topic, but it's very important in cloud architectures and that kind of thing as well.
[1007.52 → 1014.96] And I don't see any reason why we can't start implementing some of this stuff in our home setups, like Home Assistant and stuff like that.
[1015.02 → 1033.38] When you're running services in your house that you rely on to control your lighting, you're heating, et cetera, et cetera, having Home Assistant able to be able to move between a Raspberry Pi and your server and a NFC under the stairs, you know, so you've got two or three different devices that are capable of running that setup.
[1033.38 → 1039.86] You might have one that's your primary, beefy, you know, your best car or whatever, to go back to that analogy.
[1040.28 → 1045.32] But you might have your backup car that might be a bit old and a bit rusty, but it will get the job done in a pinch.
[1045.74 → 1053.38] Yeah, that's exactly as I've, well, I'm still trying to build this or looking into it, but that's basically what I have.
[1053.38 → 1060.24] I have the beefy new server, but the old server has become one of the nodes in a Proxmox cluster.
[1061.02 → 1064.34] And it certainly can't do everything the new server can.
[1064.62 → 1076.66] But if the new server would fail for whatever reason, I am, well, we'll go into it deeper, but you can basically start the Home Assistant VM again on one of the lesser power machines.
[1076.66 → 1081.42] So you won't get all functionality maybe, but you'll get the functionality you need.
[1082.00 → 1088.10] So what considerations do you have to make with Home Assistant when you're trying to run it in two places at once, effectively?
[1088.40 → 1093.56] Are you a CASSIO user, first, or do you run it out of a container or an LXC or what?
[1093.82 → 1095.18] I've been looking into that.
[1095.74 → 1100.18] And to start off, I've been a CASSIO user on a Raspberry Pi.
[1100.18 → 1111.24] And then I basically quickly moved into a VM because if you want to do something with InfluxDB and Grafana and stuff like that, the Pi will die a very quiet death.
[1111.56 → 1114.78] Well, the SD card, more specifically, will fail very quickly.
[1115.08 → 1115.20] Yeah.
[1115.52 → 1115.88] Yes.
[1116.12 → 1117.70] That's not good news for me.
[1118.84 → 1121.36] Yeah, because I'm feeling all what you're saying right now.
[1121.42 → 1126.10] I'm thinking to myself, yeah, I really don't want to be troubleshooting a struggling Pi at 9 p.m.
[1126.10 → 1128.26] when I'd rather just sit down on the couch.
[1128.38 → 1129.78] I can relate to that.
[1131.18 → 1134.86] You know if you do a lot of this stuff, there are certain times of the day when you just want to be done.
[1135.02 → 1138.04] And when it's something as important as Home Assistant, this just happened to me recently.
[1138.92 → 1142.18] Instead of going to bed, I was resolving a Home Assistant issue.
[1142.58 → 1144.82] And I thought to myself for a minute, I thought, you know what?
[1144.86 → 1149.74] I need to have a way to just switch over to another system or have a snapshot or something.
[1151.24 → 1156.56] So it might sound silly to think about making your Home Assistant system highly available.
[1156.56 → 1160.96] But listening to the two of you, I think you both make a very compelling argument.
[1161.10 → 1164.72] It's making me rethink some of my setup, even though it's so new, which I just hate that.
[1166.30 → 1167.54] Yeah, that's how it goes.
[1167.54 → 1177.62] Making locally run home automation highly available isn't talked about much, or at least I don't see a lot of topics about it.
[1177.62 → 1184.24] But for me, I've just encountered this where the box is down because of a hardware issue.
[1184.46 → 1187.56] And I know the VM is on there and I have another box.
[1187.92 → 1193.60] But, well, if you don't take any precautions, you're done.
[1193.60 → 1205.22] And that's basically what we're talking about here, making sure that by whatever means possible, the VM, if that hardware goes down, you can basically start it somewhere else.
[1205.58 → 1207.44] And it doesn't even have to be fully automated, right?
[1207.48 → 1213.98] Because a lot of stuff in the enterprise has health checks and heartbeats and all that kind of stuff that does automatic failover.
[1213.98 → 1221.02] But at home, you know, this weekend, for example, I spent a bit of time with CASSIO automating snapshots and stuff like that.
[1221.14 → 1230.52] So I now have the TAR files syncing from my CASSIO instance to a folder on my ZFS array.
[1231.22 → 1237.94] And maybe I could run a CASSIO VM on my desktop for a week whilst I wait for a part to come in or something like that using that snapshot.
[1238.26 → 1240.18] So is that the kind of approach you were taking?
[1241.12 → 1243.28] Yes, but a bit more enterprise-y.
[1243.28 → 1244.10] I guess you could say.
[1244.66 → 1251.14] So first, I built a four-node Proxmox cluster with basically hardware ahead around the house.
[1251.68 → 1255.62] Even if you just have two boxes instead of one, that's fine.
[1255.70 → 1258.52] You can build a Proxmox cluster with that.
[1258.52 → 1262.32] And then the first thing I set up was in Proxmox.
[1262.44 → 1266.60] A few versions back, they introduced ZFS replication.
[1267.72 → 1272.78] So basically, Proxmox will take a snapshot every 15 minutes of your VM.
[1273.28 → 1274.84] And send it to the other box.
[1275.06 → 1276.74] And the same VM is over there.
[1277.00 → 1277.96] It's just turned off.
[1278.48 → 1279.28] Oh, that's slick.
[1279.74 → 1280.70] I didn't know you could do that.
[1280.92 → 1283.14] That could turn the recovery time into five minutes.
[1283.42 → 1284.38] That's really great.
[1284.38 → 1292.72] I want to make sure we chat about something before we go because Alex and I have been getting really into LED light strips that are controlled by Home Assistant.
[1292.72 → 1295.96] And you have a really cool DIY project called Quinn LED.
[1296.80 → 1299.68] I'm not very familiar with it, but it looks like it could be right up our alley.
[1299.68 → 1303.92] I started this when I started building the house I'm currently living in.
[1304.18 → 1308.16] I wanted to have a dimmer for LED strips and LED lights.
[1308.28 → 1313.46] It's mainly for LED strips, which I could control using demotic at that time.
[1313.46 → 1317.82] And I started looking into this and Philips U just became a thing.
[1318.06 → 1319.88] And I started looking into that.
[1320.02 → 1323.66] I was like, okay, I can do this in my whole house, and it's cloud connected.
[1323.66 → 1327.04] And then I have to pay like $20,000.
[1327.52 → 1329.92] I was like, that's never going to happen.
[1331.50 → 1332.92] How can we do this otherwise?
[1333.22 → 1334.84] And I started looking into this.
[1334.84 → 1338.66] And I basically built the Quinn LED OG, as I now call it.
[1339.04 → 1341.58] It was in 2015, I think.
[1342.06 → 1347.58] And I basically designed a PCB and a board with some custom code on an ESP8266.
[1347.74 → 1349.60] It was an ESP01 at the time.
[1350.18 → 1353.76] And built a little dimmer board, which integrated into demotic.
[1354.72 → 1356.48] Now, fast-forward a few years.
[1356.60 → 1357.62] I've built more boards.
[1357.74 → 1359.66] I've built the Quinn LED Quad and DECA.
[1359.66 → 1361.92] That's a 4-channel and 10-channel board,
[1361.92 → 1365.58] which I, for instance, use for all the lighting in my home,
[1365.72 → 1368.36] but also in my film studio and stuff like that,
[1368.46 → 1371.80] because it's able to do very high PBM frequencies.
[1372.46 → 1376.10] And the newest board I've released is the Quinn LED Dig UNO.
[1376.80 → 1380.30] That's a single-channel digital LED controller.
[1380.50 → 1385.24] So where analog LEDs can basically only set their strip to a single colour
[1385.24 → 1387.74] or brightness intensity.
[1388.96 → 1391.78] Digital LEDs can do this per LED.
[1392.34 → 1396.18] So you can make all kinds of effects and patterns and all kinds of cool stuff.
[1396.72 → 1399.00] One thing that I never really considered,
[1399.12 → 1402.68] because the smart LEDs was the first project that got me into,
[1403.28 → 1405.38] you know, I used to build my own racing drones.
[1405.54 → 1406.58] Well, I mean, I still do.
[1406.72 → 1409.94] But that got me into electronics and soldering and that kind of thing.
[1409.94 → 1415.52] But the first thing that got me into building my own stuff at home was LED lighting.
[1415.96 → 1418.40] And I've got three or four of these things around my house right now.
[1418.90 → 1425.32] And then I watched your video about this Dig UNO with a fuse in it and polarity protection and all the rest of it.
[1425.32 → 1427.10] And I'm like, oh, yeah.
[1427.24 → 1429.56] No, I probably should have a fuse in there, shouldn't I?
[1429.56 → 1437.18] The Queen LED Dig UNO basically was like, okay, I want to do more with digital LEDs around the house.
[1437.18 → 1444.90] And you can just take an ESP8266 or an Arduino or something like that, hook up the pin to the LED strip,
[1445.18 → 1446.82] and then you can make the effects.
[1447.14 → 1451.54] But if you want to install this in somewhat more permanent fashion,
[1452.22 → 1454.62] you want it like controllable in home assistant,
[1454.62 → 1457.32] and you don't want it to burn down.
[1457.54 → 1461.72] Or if you're hooking it up at 3 a.m. and you cross the wires the wrong way,
[1462.24 → 1463.92] you don't want everything to blow up.
[1464.46 → 1467.44] And that's basically everything I put into the Dig UNO design.
[1467.58 → 1471.42] So if a fuse, reverse polarity protection, there is a level shifter on there
[1471.42 → 1477.82] because an ESP sends out 3.3 volts and the LED strip expects 5 volts.
[1478.26 → 1481.28] And most of the time it works, except when it doesn't.
[1481.28 → 1485.18] So I kind of incorporated all that into the board.
[1485.84 → 1490.12] For people who want to move on from the breadboard with DuPont connections,
[1490.20 → 1495.14] and if you wiggle it, it, well, turns off, to a bit more permanent setup.
[1495.80 → 1498.34] I absolutely love, and thank you for this.
[1498.50 → 1501.40] I love that you have open sourced the PCB design.
[1501.58 → 1503.04] I just think that's so cool.
[1503.44 → 1505.60] I basically want it to be available for everyone.
[1506.40 → 1508.96] I want to talk about 2-Year Convert for a few minutes.
[1508.96 → 1512.22] And for those of you that aren't familiar with this wonderful project,
[1513.02 → 1519.44] there are a bunch of smart plugs that you can buy based around the ESP8266 chip.
[1520.40 → 1524.92] Taken in the U.S. makes some, and I'm sure Andreas will fill us in on a few
[1524.92 → 1526.74] that are available in Europe.
[1527.32 → 1533.40] These things, they try and connect back to the manufacturer's data centre
[1533.40 → 1536.08] for some reason to get their firmware updates.
[1536.08 → 1540.92] And so what 2-Year Convert does, which there'll be a link in the show notes,
[1541.30 → 1548.08] is it emulates the update server on a Raspberry Pi or any other device with two NIC's.
[1548.20 → 1551.30] One has to be a Wi-Fi adapter, and one has to be an Ethernet.
[1552.04 → 1557.64] But essentially, you turn your Raspberry Pi into the update server of this company.
[1557.84 → 1562.18] You then flash Taste or whatever other firmware you want to onto these devices,
[1562.18 → 1564.16] and then you own them forever.
[1564.48 → 1565.60] It's really, really cool.
[1566.14 → 1569.64] And 2-Year Convert is something that you've got into a fair bit, right, Andreas?
[1570.12 → 1575.38] About a year or one and a half ago, a lot of 2-Year-based projects like light bulbs
[1575.38 → 1578.36] and also smart metering plugs became available.
[1578.90 → 1582.84] For fascinating prices, these were like $10, $15 a piece.
[1582.84 → 1589.34] And at the time, I wanted to measure some stuff in my home for power usage and things like that.
[1589.72 → 1594.44] And I basically want to have that data in Home Assistant so it can go to Influx and Grafana,
[1594.62 → 1596.28] and you can do all the stuff with it.
[1596.64 → 1601.48] But these plugs, as you said, for some reason have to have an online connection,
[1601.48 → 1603.42] and you can use an app and stuff like that.
[1604.00 → 1605.70] The hardware is in there.
[1606.08 → 1608.36] We just want to use it in our own way.
[1609.00 → 1613.34] But for some reason, these manufacturers, they don't allow that.
[1613.48 → 1617.62] They want you to run their firmware and then connect to their data centres
[1617.62 → 1620.32] and then be allowed to use your data.
[1620.52 → 1624.72] And I really don't know why it needs to know when I turn on my Christmas lights or not.
[1624.96 → 1626.38] What are they doing with that data?
[1626.38 → 1630.58] I often wonder, particularly something that is so random as a switch.
[1630.74 → 1634.34] What possible information can they have from a switch being on or off?
[1634.74 → 1636.06] Presence detection, at least.
[1636.08 → 1637.14] At least they know you're there.
[1637.52 → 1637.96] Do they?
[1638.36 → 1641.52] I mean, I've definitely left my soldering iron on when I'm not home.
[1643.30 → 1648.58] I mean, there's such a big community basically liberating these kinds of devices
[1648.58 → 1652.22] with ESP Home and Fashoda firmware that I think like, okay,
[1652.22 → 1656.68] if even one manufacturer would just give us the ability to easily do this
[1656.68 → 1663.08] by hitting a switch in some kind of web interface like allow custom third-party binary,
[1663.34 → 1665.32] you take all responsibility, click here,
[1665.32 → 1669.80] it would be an instant hit with the home automation community, I think.
[1669.98 → 1671.78] But nobody does this.
[1672.20 → 1674.26] And is our data worth that much?
[1674.40 → 1674.54] I mean...
[1675.20 → 1676.46] I can't imagine it is.
[1676.50 → 1679.48] And there are so many motivating factors for doing it for myself.
[1679.48 → 1683.90] I just want it to completely function offline with no internet connection.
[1683.90 → 1688.52] So when I take the RV somewhere where we have no connectivity, I want everything to remain
[1688.52 → 1691.64] functional, all of my automations to continue to work.
[1692.04 → 1695.82] I'm not as concerned about the privacy aspect, but that's number two on the list.
[1696.22 → 1698.38] Those are two pretty strong motivators right there.
[1698.38 → 1704.30] So I'm already adjusting my buying habits based on what the community seems to be able to
[1704.30 → 1706.68] ref lash at different times when I'm purchasing.
[1707.22 → 1709.06] And I know more, and more people are doing it.
[1709.10 → 1713.58] And it reminds me of the bad old days with cheap routers.
[1714.86 → 1715.38] DD WRT.
[1715.72 → 1715.84] Yeah.
[1715.98 → 1716.20] Yeah.
[1717.98 → 1718.46] Yeah.
[1718.46 → 1719.90] It's just like that all over again.
[1720.54 → 1724.08] Only more of them and of different varying quality now.
[1724.08 → 1727.88] There is a fun Twitter account that I like to follow called the Internet of Shit.
[1728.42 → 1735.24] And this talks about how the Internet of Things is vulnerable to quite a few things and isn't
[1735.24 → 1736.82] always updated and that kind of stuff.
[1737.00 → 1738.24] It's pretty funny.
[1738.58 → 1744.52] Well, and to Andreas's point a little bit more, why do all of these companies want to
[1744.52 → 1748.96] be cloud companies with infrastructure and vulnerabilities and services to maintain and
[1748.96 → 1750.14] APIs to update?
[1750.14 → 1754.16] Why does a smart plug manufacturer want to even get in that game?
[1754.56 → 1756.14] Planned obsolescence, Chris.
[1756.70 → 1757.36] You think it is?
[1757.54 → 1757.70] Planned?
[1757.76 → 1758.30] It could be.
[1758.44 → 1760.66] That's a little conspiracy bacon, Alex.
[1762.20 → 1762.72] Well, yeah.
[1762.78 → 1763.38] Think about it, right?
[1763.42 → 1770.38] If you're a hardware manufacturer, and you're selling what's essentially a $1 or $2 circuit
[1770.38 → 1774.52] board wrapped up in, let's say, another $2 or $3 worth of plastic.
[1774.52 → 1778.66] And then you've got to get an FCC rating and all that kind of stuff.
[1779.08 → 1782.88] There isn't going to be much money to be made, I wouldn't have thought, on a $10 smart
[1782.88 → 1783.16] plug.
[1783.30 → 1784.88] The margins are going to be quite small.
[1785.62 → 1790.24] So you've got to find some way to get people to buy these things every X number of years.
[1790.84 → 1797.22] And one fun way to do that is to accidentally, I mean, air quotes, accidentally brick the device.
[1797.22 → 1798.62] You don't even have to brick it.
[1798.72 → 1804.62] You just bring out a new app and then the new app can talk to the old devices, but all
[1804.62 → 1806.68] the new devices can only talk to the new app.
[1807.02 → 1808.26] Like the Philips Hue hub did.
[1808.72 → 1809.00] Yes.
[1809.50 → 1810.26] Yes, exactly.
[1810.38 → 1811.20] That's exactly what I was.
[1811.20 → 1816.94] I have that exact situation because I went into an old office that was shutting down and
[1816.94 → 1819.42] they had old Hue's lights all over the place.
[1819.46 → 1820.70] And I thought, well, how great is this?
[1820.78 → 1823.30] And of course, none of them could be controlled.
[1823.30 → 1829.04] I had to go spelunking for an old app that I had, I guess, had gotten at one point.
[1829.16 → 1830.62] And so I was able to retrieve it.
[1830.64 → 1833.16] I don't even know if that normally how it works on the iOS App Store.
[1833.98 → 1838.06] And then I had to bring it through a generational upgrade process.
[1838.44 → 1839.92] It was obnoxious.
[1840.26 → 1843.18] So, I mean, if you can own your hardware, I highly recommend doing it.
[1843.30 → 1848.48] And this two-year convert collection of scripts is really pretty cool.
[1848.48 → 1854.36] And there's been some updates over this course of this year, two-year or the two-year compatible
[1854.36 → 1857.58] device manufacturers patched a lot of the exploits that were being used.
[1858.32 → 1862.60] And then in September sort of time, an update came out and people have found another exploit
[1862.60 → 1863.98] and that's what we're currently using.
[1864.24 → 1866.68] So bear in mind, this could go away at any time.
[1866.68 → 1871.96] But a device I bought this week is the Taken SS30.
[1872.70 → 1880.66] And this thing has four individually controllable AC ports and four controllable USB ports.
[1881.02 → 1888.16] So in Home Assistant, I now have five switches that I can control on one power strip using
[1888.16 → 1889.64] the TAS motor firmware.
[1889.94 → 1893.24] And it's really great because I know that that's just going to carry on working now until the
[1893.24 → 1895.68] end of time or until that device physically fails.
[1895.68 → 1896.94] Wow, that is really great.
[1897.06 → 1899.34] Is this the one that's only $24 on Amazon?
[1899.64 → 1900.64] Yep, believe it or not.
[1901.24 → 1902.46] I'm going to drop a link to that in the notes.
[1902.54 → 1903.32] That's really cool.
[1903.58 → 1905.26] And all you need to flash it is a Raspberry Pi.
[1905.62 → 1905.82] Right.
[1905.90 → 1907.22] And then you own it forever.
[1907.84 → 1912.14] And they may not make that device forever, or they may patch that vulnerability.
[1912.38 → 1914.34] But that one, now that you own it, it's good.
[1914.42 → 1919.28] And if you were to buy a couple at a time, you could just kind of set up a production chain
[1919.28 → 1921.22] and just flash a few of them and get it over with.
[1921.22 → 1927.20] And the thing that Home Assistant enables is now that you can use Hue and your own flash
[1927.20 → 1931.94] plugs and all kinds of stuff from all kinds of brands and basically connect it all together
[1931.94 → 1934.24] as long as you can get it into Home Assistant.
[1934.64 → 1937.42] And it does that with a lot of cloud-enabled stuff too.
[1937.90 → 1944.42] But getting it in their native with Fashoda or ESP Home is just, it makes it work so flawlessly
[1944.42 → 1945.36] every time.
[1945.36 → 1946.36] Mm-hmm.
[1946.76 → 1950.90] Yeah, I really do appreciate that aspect of Home Assistant because it means that some
[1950.90 → 1953.12] of these old IoT devices aren't throwaways.
[1953.82 → 1958.20] Home Assistant doesn't care that these Hue bulbs that I got have old firmware on them.
[1958.26 → 1959.60] It still controls them just fine.
[1959.66 → 1961.30] Sometimes they pop offline.
[1961.68 → 1966.22] It's a little obnoxious, but it's so great at the same time to have three or four different
[1966.22 → 1969.40] vendors' products all controlled locally by one piece of software.
[1969.88 → 1975.22] But the key thing that I've found is now I shop with Home Assistant compatibility in mind.
[1975.36 → 1976.12] That's where I start.
[1976.36 → 1978.94] Or a reachability for that, but yeah.
[1979.08 → 1979.38] Right.
[1979.52 → 1979.86] Yep.
[1979.96 → 1980.14] Yep.
[1980.28 → 1981.32] Good point.
[1981.40 → 1982.46] That's another way to look at it.
[1982.70 → 1984.20] That's basically why I started.
[1984.46 → 1988.82] One of the reasons I designed my own hardware and dimmers and boards and stuff like that,
[1989.16 → 1992.28] it's all geared to being controlled with Home Assistant.
[1992.78 → 1995.54] Now it's an ESP, so you can run anything you want on it.
[1995.70 → 2002.02] But from what I gather and the people in Discord and on my website and stuff like that, 95% uses
[2002.02 → 2003.08] it with Home Assistant.
[2003.08 → 2003.56] Awesome.
[2003.76 → 2006.88] Well, Quin dor, I just want to say thank you again for not only all the great details.
[2007.10 → 2011.58] I came across your channel when I was looking for cheap integration thermostats into Home
[2011.58 → 2013.96] Assistant, which has made my life more comfortable.
[2014.66 → 2017.64] And I also just really appreciate the level of detail.
[2017.76 → 2021.48] So we will link to the Intermittent Tech YouTube channel in the show notes.
[2021.78 → 2025.10] Keep up the great work and keep us in the loop on future projects.
[2025.16 → 2026.08] And we'd love to chat about them.
[2026.46 → 2026.60] Sure.
[2026.80 → 2027.10] Will do.
[2027.20 → 2028.08] Thank you for having me.
[2028.08 → 2031.04] Is there anywhere you would explicitly like to send people?
[2031.14 → 2031.90] I mean, are you on Twitter?
[2032.20 → 2033.96] I know you have a Discord, for example.
[2035.36 → 2038.06] Well, people starting with the YouTube channel.
[2038.20 → 2041.06] And if they then want to join the Discords, the link and stuff are there.
[2041.22 → 2042.40] So start with the YouTube channel.
[2042.50 → 2043.66] I think that's a good starting point.
[2043.66 → 2048.40] And you can get more self-hosted show on Twitter at self-hosted show.
[2048.56 → 2050.32] I'm on Twitter at Ironic Badger.
[2050.60 → 2052.48] I'm at Chris LAS.
[2052.94 → 2054.96] And I'm there under Intermittent Tech.
[2055.10 → 2060.10] And you can find links to all of those good things in the show notes at self-hosted. Show
[2060.10 → 2061.08] slash nine.
[2061.08 → 2091.06] And you can find links to all of those good things in the show notes at self-hosted show.
