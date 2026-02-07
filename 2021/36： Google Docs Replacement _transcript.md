[0.00 --> 6.32]  Coming up on the show, I review Home Assistant's new dedicated hardware, Alex is literally buried
[6.32 --> 10.72]  in computers, and our favorite Google Docs killer has a big update. I'm Chris.
[11.10 --> 13.20]  And I'm Alex, and this is Self Hosted.
[14.44 --> 21.12]  Oh, Chris, I am surrounded by computer parts. I mean, literally, I could open a shop right now.
[21.20 --> 25.14]  I've got every single computer I own in pieces right now.
[25.14 --> 29.44]  I feel your pain. I am surrounded in laptop parts at the moment.
[30.00 --> 32.16]  Is that because of the XPS reviews you're doing?
[32.48 --> 36.90]  I have a couple of machines in for review at the moment, plus a personal server project that I'm working on.
[37.00 --> 42.40]  And then I was moving offices, and I had all of the different screws neatly organized for each laptop case.
[42.66 --> 48.16]  And my daughter came in and said, what are these, Daddy? And mixed them.
[48.26 --> 49.24]  Oh, no.
[50.38 --> 51.18]  Mixed them all.
[52.92 --> 54.54]  Screws are the worst as well.
[55.06 --> 55.30]  Yeah.
[55.66 --> 57.12]  Particularly laptop-sized ones.
[57.12 --> 60.10]  What are you, what are you, deepen projects over there, several at a time?
[60.50 --> 61.68]  Yeah, that's just it.
[61.80 --> 66.04]  So I built a system around the UNAZ and QuickSync a little while ago.
[66.52 --> 72.20]  But I decided that I wanted something that was a little more future-proof in terms of expansion and stuff like that.
[72.28 --> 81.74]  And the ITX board that the UNAZ case can fit only has one PCI port, which is taken up with the HBA disk expansion card that I have.
[81.74 --> 82.46]  Right.
[82.82 --> 90.88]  And so if I wanted to put, say, OpenSense as a VM on top of Proxmox, I don't have any PCI ports to add an extra NIC to the motherboard.
[91.52 --> 99.50]  So anyway, I decided to take my desktop motherboard and put it into my Rosewill server case that was housing my Dual Xeon system.
[99.50 --> 108.08]  Basically, all this comes as a result of me finally deciding to break up with my Dual Xeon system and go all in on QuickSync.
[108.26 --> 112.12]  It's worked really well for the last month or so as I've been testing it in the UNAZ build.
[112.30 --> 113.52]  So I'm going all in.
[113.66 --> 119.28]  My home lab's going to be an i5-8500 and my NAS is going to be also an i5-8500.
[119.28 --> 123.92]  So, yeah, I'll have two of those QuickSync capable systems in the house.
[124.24 --> 136.12]  And the idea is that I've got one system that is just sort of always on bulletproof and is running Blue Iris and Home Assistant and DNS separate from the storage,
[136.30 --> 142.36]  which will be running on the other system, which is housing Plex and media apps and that kind of stuff.
[142.86 --> 146.54]  Because the one you take offline most of all is the one with the hard drives in it.
[146.54 --> 154.86]  And it's not like I take it offline a lot, but when I do, it takes everything out because I've got, you know, all of my services running on one box.
[155.12 --> 163.04]  So it's been a pain because I've had to move all of my desktop out of its case and my server out of its case.
[163.26 --> 171.32]  And I've got literally four or five computers worth of parts around me and I'm selling stuff off to people and it's nuts.
[171.94 --> 174.94]  And doing the day job all off a laptop in the meantime, I suppose.
[174.94 --> 181.98]  Yes. Yeah. And the worst part is my IRC bouncer for Red Hat is currently in pieces on the table behind me.
[182.02 --> 184.08]  So I haven't been on IRC all day, which has been a bit bad.
[184.08 --> 193.24]  I was moving offices recently and like literally like my priority was get the desktop, reset up, get everything connected, get it powered on.
[193.66 --> 194.76]  It's got to be online.
[195.16 --> 199.82]  The best part was as well that my laptop decided it was going to screw up and I had to reinstall that today as well.
[199.90 --> 204.88]  So I've completely nuked and paved seemingly everything in this house and I'm starting from scratch.
[205.22 --> 205.62]  Wow.
[206.16 --> 206.94]  That's going to be fun.
[206.94 --> 210.74]  I haven't yet found out what I've forgotten to back up yet, but I'm sure there'll be something.
[211.36 --> 214.58]  And days of setting small little things up as it always goes.
[214.78 --> 215.02]  Yeah.
[215.08 --> 220.82]  Just before we were recorded, for example, I'd turn off Turbo Boost on my Mac so that the fans weren't spinning up.
[222.02 --> 222.94]  Oh, Max.
[223.02 --> 230.56]  Well, let's take a moment and say that this episode is brought to you by the all new Cloud Guru, the leader in learning for the cloud for Linux and other modern tech skills.
[230.56 --> 233.14]  They have hundreds of courses and thousands of hands on labs.
[233.24 --> 238.44]  So get certified, get hired and get learning at a cloud guru dot com.
[238.78 --> 249.14]  One of the things I have in my new office is a bench for projects and I have the new Home Assistant blue hardware on there, which I'm going to be talking about in a little bit in the show.
[249.14 --> 264.14]  But in the meantime, before we get there, Alex and I kind of wanted to do a PSA on the show and talk a moment about HedgeDoc, which might be a solution for anyone out there who wants a really modern Google Docs alternative that you can self host.
[264.50 --> 266.84]  And it happens to be an excellent markdown editor.
[267.80 --> 271.34]  Real time collaborative editing for markdown documents.
[271.60 --> 272.48]  It's great.
[272.72 --> 275.04]  You know, we've used it at JB now for how long?
[275.14 --> 275.68]  Two years?
[275.82 --> 276.02]  Three?
[276.62 --> 276.88]  Yeah.
[276.88 --> 276.96]  Yeah.
[277.24 --> 278.90]  So it's it stood the test of time.
[279.02 --> 280.50]  Battle tested in production.
[280.84 --> 281.28]  Air quotes.
[282.04 --> 284.80]  Use it for all the LUP show notes as well and stuff like that.
[284.88 --> 285.96]  And you and Wes use it.
[286.22 --> 287.42]  And we use it for all the shows.
[287.58 --> 290.92]  And now I use it for a lot of my notes just for JB stuff in general.
[291.28 --> 294.24]  It's the project for formerly known as Cody MD.
[294.60 --> 300.94]  They went through a name change to annoy just to avoid like naming conflicts out there.
[300.94 --> 303.02]  I guess there was another project that's had a similar name.
[303.02 --> 309.14]  And so now it's called HedgeDoc and it lets you just easily collaborate on markdown documents.
[309.30 --> 312.20]  And all you really have to do is get started and you just share a link with somebody.
[312.44 --> 314.40]  And now they're in and they can start editing.
[314.60 --> 318.50]  And then if you create an account, you get kind of like a document library.
[318.50 --> 326.84]  And it supports things like tags, which we don't use a lot, but it supports things that allow you to recall documents pretty quickly or categorize documents.
[327.34 --> 332.56]  It also does real time rendering of that markdown so you can see what you're writing in real time.
[332.56 --> 334.82]  And then it gives you a bunch of shortcuts.
[335.06 --> 338.76]  So maybe you don't remember how to do a table and markdown or embed an image.
[338.80 --> 340.04]  It's got a button for that as well.
[340.28 --> 340.62]  It does?
[341.14 --> 341.34]  Yeah.
[341.42 --> 342.06]  I didn't know that.
[342.06 --> 343.96]  Right along the top there.
[344.56 --> 344.68]  Yeah.
[344.98 --> 351.10]  And Alex, you recently reset it up for us because we were on an older Code EMD instance.
[351.50 --> 352.06]  Yeah, that's right.
[352.10 --> 354.40]  There's nothing more permanent than a temporary solution, right?
[354.66 --> 354.92]  Yeah.
[355.28 --> 358.46]  Wes threw it up on a, was it a droplet or something a couple of years ago?
[358.46 --> 362.46]  We wanted to test it for an episode of Linux Unplugged or something like that.
[362.46 --> 365.10]  And then we liked it so much, we just kept using it.
[365.30 --> 365.78]  That's right.
[366.14 --> 366.16]  So typical.
[366.56 --> 370.68]  And it was just hanging out on an open port with no TLS or anything.
[370.68 --> 372.74]  So I've been wanting to fix that for a while.
[372.84 --> 378.30]  So when I saw the renaming come through on the Linux server image, I was just like, yes,
[378.50 --> 381.54]  here's my excuse to push it to Chris and say, I can do it.
[382.00 --> 382.10]  Yep.
[382.38 --> 385.38]  So yeah, Wes sent me the database.
[385.84 --> 393.12]  He zipped up the Docker app data volume that stores the database and stuff like that,
[393.86 --> 400.38]  span it up in a container on Linode with just SCP the tar.gz file across.
[401.14 --> 404.54]  Unzipped it, pointed the container at the correct directory.
[405.20 --> 408.60]  And I think it uses Postgres on the backend, our setup.
[409.38 --> 414.34]  All the infrastructure, by the way, is open sourced on the self-hosted infra wiki.
[414.94 --> 415.36]  Not wiki.
[415.84 --> 416.16]  GitHub.
[416.54 --> 417.14]  GitHub repo.
[417.14 --> 420.88]  So, but yeah, it just came straight up.
[421.06 --> 422.30]  You know, there was no drama.
[422.50 --> 426.94]  The only slightly tricky bit was that you own the domain name and we had to point the name
[426.94 --> 432.90]  service for the domain name at my Cloudflare account so that we could get TLS through traffic
[432.90 --> 435.14]  working with the DNS challenge.
[435.14 --> 437.28]  Yeah, but I love what we ended up with.
[438.14 --> 443.06]  It's a cute little URL that's easy for the team to remember and it makes it possible to
[443.06 --> 446.92]  share easily with anybody and they'll remember it as well.
[447.08 --> 452.68]  So I think it turned out to be a pretty nice setup and maybe the perfect time to migrate.
[453.12 --> 458.68]  I mean, it seems like it was nearly flawless to import a somewhat stale Code EMD database
[458.68 --> 460.10]  right into HedgeDoc.
[460.10 --> 466.14]  So if you're using Code EMD today, it's probably a good time to upgrade because that migration
[466.14 --> 467.24]  is pretty simple right now.
[467.72 --> 468.08]  Easy peasy.
[468.20 --> 470.96]  Yeah, there's a couple of options for containers that you could use.
[471.48 --> 474.52]  Linux server, of course, make a container for this one.
[475.10 --> 481.20]  They've migrated over from Code EMD to HedgeDoc, but I actually ended up for our installation
[481.20 --> 484.04]  here using the one that the development team now provide.
[484.54 --> 488.50]  This is the thing about Linux server is a lot of their images make projects popular enough
[488.50 --> 491.12]  that the devs go, oh, we've got lots of people using it in Docker.
[491.80 --> 494.34]  And then the projects themselves start providing an image.
[494.52 --> 499.06]  And generally speaking, I will keep using the Linux server image until I have good reason
[499.06 --> 499.98]  to switch.
[500.62 --> 505.00]  And the migration seemed like a perfect excuse, as you say.
[505.18 --> 508.72]  So we're running out of the official HedgeDoc image.
[509.18 --> 510.38]  And yeah, it just works.
[510.46 --> 512.32]  And there's nothing more really to say about that.
[512.32 --> 518.56]  It's the best kind of tool because admittedly, it takes a little more skill set and a little
[518.56 --> 523.02]  more effort than just going and signing up for a Google Docs, for, you know, signing
[523.02 --> 525.46]  into a Google Docs account and using Google Docs.
[525.50 --> 526.98]  Like it takes a little more effort than that.
[527.50 --> 528.40]  But we own this.
[528.46 --> 529.34]  It's self-hosted.
[529.34 --> 533.04]  And we get to have fun with the domain because of that.
[533.24 --> 537.04]  We get to just sort of own the entire stack.
[537.46 --> 544.02]  And that's great because it's a tool we use every single day, six days a week to produce
[544.02 --> 544.56]  the shows.
[545.16 --> 550.26]  And replicate the data from the backend to a local endpoint.
[550.50 --> 552.68]  So it's completely backed up offline.
[552.98 --> 557.60]  So that if for any reason that Linode ever had a problem, we're good to go.
[559.34 --> 561.48]  Linode.com slash SSH.
[561.60 --> 565.50]  Go there to get a $100 60-day credit towards a new account and support the show.
[565.86 --> 569.10]  Like Alex was saying, they are our cloud server provider.
[569.32 --> 570.60]  We have the wiki on there.
[570.72 --> 572.48]  Perfect Media Server dot com is on there.
[572.56 --> 573.86]  HedgeDoc's on there and a lot more.
[574.22 --> 575.58]  We have the Matrix server on there.
[576.22 --> 577.74]  We have our Cast and Coding server.
[577.90 --> 578.52]  Next Cloud.
[578.96 --> 583.32]  A lot of our backend infrastructure and new things that we're working on that we haven't even
[583.32 --> 583.68]  announced.
[583.82 --> 585.46]  We're hosting them all on Linode.
[585.98 --> 589.18]  And personally, one of the things that I think is great about Linode is all the
[589.18 --> 590.18]  distributions they support.
[590.28 --> 595.20]  So whatever environment you're comfortable working in, even the Alpines, Arch, recent
[595.20 --> 600.70]  CentOS releases, Debian, Fedora, OpenSUSE, several versions of Ubuntu, on and on and on.
[601.52 --> 606.38]  But what I really like about Linode is you can tell when a company is passionate about the
[606.38 --> 607.56]  actual technology.
[608.24 --> 610.78]  And I think people listening to the show probably get that.
[610.78 --> 614.90]  When you're passionate about the technology, you have the insight into what it's capable of.
[614.90 --> 622.08]  And that's why Linode started in 2003 as one of the very first companies and in something we
[622.08 --> 623.94]  weren't even really calling cloud computing yet.
[624.02 --> 627.58]  That was three years before AWS even started.
[627.78 --> 630.34]  And now they're the largest independent cloud provider.
[630.34 --> 638.44]  And you can get a $100 credit and play with infrastructure that's professional grade with native SSDs,
[638.48 --> 643.46]  40 gigabit connections to the hypervisors, 11 data centers around the world, object storage,
[643.94 --> 648.26]  node balancers, a really nice, clean dashboard.
[648.90 --> 651.34]  You can get started at linode.com slash SSH.
[652.02 --> 655.98]  You go there, get that $100 60-day credit towards a new account and support the show.
[655.98 --> 659.62]  So that's linode.com slash SSH.
[661.48 --> 662.18]  All right, then.
[662.22 --> 664.38]  Why don't you tell me about this Home Assistant blue box?
[664.48 --> 667.04]  I've been pretty jealous, honestly, since I heard you got yours.
[667.38 --> 668.88]  You know, it's real.
[669.14 --> 673.96]  I was watching the Home Assistant conference when they announced it, and I ordered one as
[673.96 --> 674.76]  fast as I could.
[674.84 --> 678.16]  A lot of other people did, too, because the order page was having issues.
[678.16 --> 684.88]  But it is a small, tiny, I mean, it's not as small as a Raspberry Pi, but it's smaller
[684.88 --> 687.76]  than a NUC or any kind of desktop PC.
[688.42 --> 692.42]  And it is a dedicated Home Assistant box, and it's called the Home Assistant blue.
[692.68 --> 695.22]  It's a six-core ARM processor system.
[695.30 --> 697.64]  It has four gigs of DDR4 RAM.
[697.64 --> 705.56]  And a big upgrade over the Raspberry Pi 4 is it comes with 128 gigabytes of eMMC storage.
[705.78 --> 710.04]  Plus, of course, there's other ways to expand that, like through USB, because it has four
[710.04 --> 716.28]  USB 3.0 ports on the sucker, as well as an Ethernet and full HDMI out.
[716.84 --> 720.44]  And it's really well built, Alex.
[720.60 --> 722.20]  It's very, very solid.
[722.52 --> 727.60]  I would feel comfortable with this strapped to the RV going down the road for years.
[727.96 --> 729.40]  On the inside or the outside?
[731.00 --> 732.10]  Definitely the inside.
[732.64 --> 734.70]  But the top is a nice blue aluminum.
[734.96 --> 739.14]  They've made it look really nice with a classy white version of the Home Assistant logo.
[739.40 --> 742.98]  And the bottom is an integrated heatsink system.
[743.12 --> 743.52]  Oh, neat.
[743.76 --> 744.34]  How big is it?
[744.34 --> 753.28]  It's about four inches wide and about, I'd say about an inch and a half high at its peak,
[753.38 --> 755.70]  maybe, because it's kind of got an arched shape to the case.
[756.10 --> 758.68]  And it's about half a pound in weight.
[758.80 --> 760.66]  So it's just over half a pound.
[760.76 --> 763.36]  So it's got a really solid, hefty feel to it.
[763.80 --> 766.40]  So it's like, what, a couple of CD cases stacked on top of each other?
[766.74 --> 769.68]  Yeah, with a little bit of an arch at the top of it.
[770.30 --> 774.10]  And what's really at the heart of this thing is an Odroid N2+.
[774.10 --> 775.86]  That's really what this is.
[776.36 --> 780.78]  I've noted that the Home Assistant team has mentioned the Odroid N2+, a few times, and
[780.78 --> 785.90]  it seemed to be one of the favorite devices of one of the primary Home Assistant developers.
[786.56 --> 790.26]  So I think this box is kind of like their favorite experience.
[790.26 --> 792.64]  It's the one that they personally test on.
[792.64 --> 796.66]  And so to say it's well-supported is an understatement.
[797.00 --> 801.02]  And so I think it was a natural fit for them to just bundle it when they partnered up with
[801.02 --> 801.80]  a hardware provider.
[802.28 --> 805.66]  In terms of a smart home hub, it's lacking a couple of things.
[805.76 --> 810.18]  You need to add Z-Wave or ZigBee via USB, right?
[810.48 --> 810.70]  Yep.
[810.78 --> 814.66]  Although that's the same kind of trade-off you have with any of these other kind of ARM boards,
[814.66 --> 821.26]  because it's kind of competing between something like a smart things home hub and a Raspberry
[821.26 --> 822.36]  Pi DIY kit.
[822.46 --> 824.68]  It's like trying to live in that middle ground there.
[825.16 --> 826.42]  So remind me of the price then.
[826.50 --> 827.00]  How much was it?
[827.36 --> 835.04]  It's listed for $140, but after all in for me with $21 and change of shipping, it was $180
[835.04 --> 836.70]  total to get this device.
[837.14 --> 837.38]  Ooh.
[837.88 --> 838.20]  Okay.
[838.32 --> 841.46]  I had 100 in my mind for some reason, but 180.
[841.78 --> 842.00]  Wow.
[842.18 --> 842.38]  Okay.
[842.56 --> 843.68]  That's getting up there.
[843.68 --> 844.46]  Well, okay.
[844.62 --> 846.24]  So I'll get to the value.
[846.48 --> 850.44]  So the first boot experience, they're trying to make it very out-of-the-box friendly.
[850.58 --> 851.70]  Two steps to set up.
[852.00 --> 857.00]  You plug it in to your network and then go to your browser and you type in homeassistant.local
[857.00 --> 858.56]  and it's supposed to just come up.
[858.94 --> 860.50]  But of course, that's not how it works on my network.
[860.58 --> 864.64]  I already have a DNS and DHCP server set up and my system isn't just going to start resolving
[864.64 --> 865.74]  some new machine.
[866.30 --> 868.78]  But I was able to get the IP out of the DHCP log.
[868.84 --> 869.36]  Pretty simple.
[869.78 --> 870.42]  Put that in.
[870.52 --> 871.96]  Went to port 8123.
[871.96 --> 875.66]  And it's really at this point, it's a basic home assistant install.
[875.82 --> 879.56]  It's really kind of just what you'd expect if you'd set up the home assistant suite with
[879.56 --> 880.80]  supervisor and everything.
[881.22 --> 882.88]  You create the first time account.
[883.78 --> 886.46]  But Alex, it feels fast.
[886.56 --> 891.76]  It definitely feels noticeably faster in the UI than my Raspberry Pi 4.
[891.90 --> 894.90]  Granted, it's a new, happy, fresh install.
[894.90 --> 898.64]  But I've set up home assistant enough times on the Pi to know what it feels like.
[898.74 --> 901.64]  And I can tell you with confidence, this thing absolutely feels faster.
[902.22 --> 904.20]  Are you SD card based in the Pi then?
[904.66 --> 904.96]  USB.
[905.28 --> 906.06]  So it is on a disk.
[906.20 --> 906.58]  Oh, really?
[906.88 --> 907.12]  Yeah.
[907.22 --> 908.08]  That's interesting then.
[908.32 --> 909.52]  I think it's just got a little more horsepower.
[910.06 --> 912.90]  And I think the developers are optimizing for this thing.
[912.90 --> 917.66]  That's why, you know, when we talk about the value, so I'd say round it off to $200 or just
[917.66 --> 921.14]  under $200, you know, just as a concept price point.
[922.04 --> 929.46]  Well, what is a totally local, merges all the different vendors together with no subscription
[929.46 --> 935.48]  and is completely under your control, standalone box worth?
[935.48 --> 942.12]  So to me, home assistant, home assistant is one of the few open source projects that has
[942.12 --> 947.62]  changed my life at the level that, like say Linux has, where it has, it has changed.
[947.82 --> 951.56]  It has changed the quality of life for my entire family.
[952.20 --> 957.72]  And I also use it here at the studio to help with remote presence and other, other like,
[957.76 --> 959.42]  you know, just light management in the studio.
[959.76 --> 962.36]  And so it also helps in a professional capacity.
[962.36 --> 964.94]  So $200 for a dedicated box.
[965.02 --> 966.02]  It's really fast.
[966.10 --> 967.38]  It feels very well built.
[967.48 --> 973.60]  I mean, it feels like a polished product that is also supporting home assistant development
[973.60 --> 975.00]  at the same time when I buy it.
[975.60 --> 975.84]  Mm-hmm.
[976.02 --> 976.36]  Mm-hmm.
[976.66 --> 978.64]  I feel like that's, you know, under $200.
[978.90 --> 980.18]  It is a good value for this.
[980.20 --> 981.92]  And I think I'm actually going to buy another one.
[982.04 --> 984.70]  I'm going to buy one for the studio because this is what I set this one up for.
[984.74 --> 988.90]  I wasn't sure if I was ready to deploy my serious, serious home assistant setup yet.
[988.90 --> 993.56]  So I put it in production here at the studio where it's, it's kind of important, but honestly,
[993.72 --> 995.28]  like I could recreate it in a day.
[995.54 --> 995.98]  You know what I mean?
[996.16 --> 1003.54]  It's that level of, but at home, like, I just, I mean, I would take a snapshot and I would
[1003.54 --> 1008.22]  restore the snapshot, but it just has to be perfect at home because it literally impacts
[1008.22 --> 1009.00]  our quality of life.
[1009.10 --> 1013.30]  So I wanted to take it slow and I wasn't sure if I was ready to replace my raspberry pie,
[1013.30 --> 1019.02]  but I am a believer in having home assistant on its own dedicated host, either being a
[1019.02 --> 1020.32]  VM or on hardware.
[1020.66 --> 1025.78]  And I don't necessarily think having it live alongside a lot of my other services in Docker
[1025.78 --> 1030.34]  while trying to also use the supervisor is a good long-term strategy.
[1030.34 --> 1034.24]  Like in there, it gives me errors about being on an unsupported OS all the time.
[1034.36 --> 1039.92]  And I look at the development trajectory and I think if they're selling these machines and
[1039.92 --> 1043.16]  they are themselves are developing, like you have to imagine the developers all have these,
[1043.16 --> 1044.26]  or we'll all have these.
[1045.26 --> 1047.72]  That's likely where they're going to invest a lot of their time and energy and they're
[1047.72 --> 1051.16]  going to be developing with a mindset that they're doing it on a dedicated host.
[1051.66 --> 1055.98]  When I look at the power draw for this thing and I look at the, you know, I got to always
[1055.98 --> 1056.64]  do that math.
[1056.72 --> 1062.10]  Like if I bring a box in, I really have to be aware of what it's going to take because
[1062.10 --> 1064.32]  I want to be able to go off grid.
[1064.44 --> 1068.06]  I want to be able to survive on solar power alone, which means I got to extend the life of
[1068.06 --> 1069.68]  my batteries as long as possible.
[1069.68 --> 1075.38]  And this thing under load, and I'm not, you know, I didn't, I didn't do extensive testing
[1075.38 --> 1078.58]  here, but it went, it was right in line with what their specs were.
[1079.20 --> 1080.00]  Six Watts.
[1080.66 --> 1081.84]  That's pretty remarkable.
[1082.72 --> 1083.18]  Six Watts.
[1083.36 --> 1083.52]  Wow.
[1084.02 --> 1084.30]  Yeah.
[1084.68 --> 1088.52]  And, and around idle, it was around two Watts, sometimes two and a half Watts.
[1089.10 --> 1091.26]  I only really started testing it today.
[1091.26 --> 1095.40]  So I want to do more extensive testing, like, because it's a pretty simple home assistant install,
[1095.40 --> 1099.18]  but I was monitoring during the first load and getting all that stuff like first set up.
[1099.20 --> 1103.06]  And I monitored a little bit under, under just sitting there idle, you know, just like kind
[1103.06 --> 1104.46]  of just daily, just sitting there running.
[1105.08 --> 1105.80]  That's what I noted.
[1105.84 --> 1106.40]  And I went and checked.
[1106.48 --> 1108.48]  I looked up their specs for this, for this board.
[1108.54 --> 1110.14]  That's exactly what it's in line with the specs.
[1110.40 --> 1115.76]  Pretty sure my garage door opener uses more than six Watts just sat there doing nothing all
[1115.76 --> 1115.92]  day.
[1116.84 --> 1120.90]  I know there's power bricks that just sit there and plugged into the wall that use more than
[1120.90 --> 1121.38]  two Watts.
[1121.38 --> 1122.06]  Uh, yeah.
[1122.32 --> 1126.60]  So we'll see because that's the, that's the big deal breaker is if that ends up being
[1126.60 --> 1131.68]  a higher, higher load wattage, uh, that would be, that'd be a deal breaker.
[1131.68 --> 1137.04]  But at this point, I think plugging in a device that would be using around six Watts would be
[1137.04 --> 1139.42]  kind of just lost in the wash.
[1139.50 --> 1141.24]  I don't think I'm really going to notice that on my runtime.
[1141.50 --> 1145.02]  So I think it means from a power budget standpoint, I can put this thing in production.
[1145.88 --> 1147.66]  I think, I think I'm going to get another one.
[1148.14 --> 1151.02]  You do like highly available single board computers though, don't you?
[1151.02 --> 1153.96]  So there is something to this.
[1154.04 --> 1158.62]  You could, you know, if a guy really wanted, he could buy two of these.
[1158.62 --> 1162.18]  I'm not saying he should, but he could, and just keep one in the drawer, right?
[1162.50 --> 1162.66]  Yeah.
[1162.98 --> 1163.14]  Yeah.
[1163.30 --> 1165.12]  And keep a snapshot somewhere.
[1165.78 --> 1170.50]  And if one pops you in, in 35 seconds, you pull it out.
[1170.58 --> 1171.62]  All the plugs are all the same.
[1171.68 --> 1175.60]  You swap it in and you restore the snapshot and you're back in business.
[1175.60 --> 1182.24]  But if ever there is a use case for a literal plug and play appliance, it's your smart home
[1182.24 --> 1182.48]  hub.
[1182.80 --> 1183.02]  Yeah.
[1183.12 --> 1185.06]  And this is version one, right?
[1185.14 --> 1189.56]  And maybe even, and I'm not, I'm not knocking it when I say this, but maybe it's even version
[1189.56 --> 1194.56]  0.5 because I have a sense this kind of came along during the year and it's, it's, it's a
[1194.56 --> 1196.96]  really good, it's a really good first, first start.
[1196.96 --> 1203.16]  But I could see future ones that maybe have things like Zigbee or Z-Wave or, or whatever
[1203.16 --> 1206.72]  this new conglomerate standard is that I can't remember.
[1207.30 --> 1209.02]  Makes me think of the XKCD comic.
[1210.02 --> 1210.42]  Yeah.
[1210.60 --> 1211.88]  Just one more standard, Alex.
[1211.92 --> 1212.48]  That's all we need.
[1212.82 --> 1213.64]  There are 12 standards.
[1213.72 --> 1215.40]  We should have one that unifies them all.
[1215.66 --> 1215.80]  Okay.
[1215.84 --> 1217.00]  Now we have 13 standards.
[1217.24 --> 1217.42]  Great.
[1218.34 --> 1222.38]  Also they, you know, one that has wifi built in, I don't know how they would handle it with
[1222.38 --> 1226.44]  the metal housing because I think the casing is providing some heat transfer.
[1226.44 --> 1228.14]  It's mostly cool to the touch.
[1228.24 --> 1230.92]  The bottom's warm, but that's, that's kind of expected.
[1231.02 --> 1231.46]  It's a heat sink.
[1231.78 --> 1236.94]  Is, is wifi the right kind of expectation to set for reliability for this type of device
[1236.94 --> 1237.18]  though?
[1237.50 --> 1239.50]  Probably in that light, it's probably a good thing.
[1239.56 --> 1241.02]  They at least didn't put it in 1.0.
[1241.42 --> 1241.60]  Right.
[1242.16 --> 1247.04]  I'll tell you one thing that I am just a little concerned about, and I'd be really curious
[1247.04 --> 1253.96]  to see how this actually plays out in the longterm for you is EMMC write endurance is not
[1253.96 --> 1255.74]  famously very good.
[1256.08 --> 1261.20]  So I'd be curious to see how home assistant, which writes a lot of data to that database
[1261.20 --> 1266.44]  all the time will be, you know, in, in a year or two's time, whether it'll have burnt
[1266.44 --> 1267.48]  through that flash or not.
[1267.48 --> 1267.92]  Yeah.
[1268.08 --> 1273.76]  And I wouldn't be surprised if they have a way to switch it to USB storage.
[1273.76 --> 1278.52]  Cause I do remember there being some discussion about that during the product launch, but going
[1278.52 --> 1282.26]  through like the first time setup process, there's nothing that prompts you to store it
[1282.26 --> 1282.90]  anywhere else.
[1283.06 --> 1284.24]  You know, it's all on that EMMC.
[1284.60 --> 1286.56]  I got bitten with a PF sense box.
[1286.56 --> 1292.78]  Uh, this was, um, one of the APU one D boxes, I think several years ago, I didn't move the
[1292.78 --> 1295.42]  logs off of the, uh, M SATA SSD.
[1295.66 --> 1301.86]  So obviously M SATA is different to EMMC, but just to tend, you know, a related comment
[1301.86 --> 1306.76]  really that if you don't move logs off of SSDs, they can wear out pretty quickly.
[1307.60 --> 1307.62]  Yeah.
[1307.64 --> 1311.42]  I had a free NAS box that had the EMMC finally die on it.
[1311.56 --> 1312.58]  It was a really old one.
[1312.58 --> 1314.72]  It was like an appliance version that somebody prebuilt.
[1315.82 --> 1319.58]  And, um, that's when I learned that those things have a limit.
[1319.92 --> 1323.96]  Actually, that's when I learned that it was actually even using EMMC.
[1326.08 --> 1327.62]  And then I learned they had a limit.
[1328.62 --> 1329.28]  So you're right.
[1329.36 --> 1330.66]  That's a good thing to keep an eye on.
[1330.74 --> 1335.08]  I'm also going to, if I was going to put it in production, I would prefer to have all
[1335.08 --> 1339.48]  of the home assistant data and anything that needs a lot of read, write on external storage.
[1339.54 --> 1341.26]  I mean, the thing has plenty of USB ports.
[1342.58 --> 1348.50]  I want to take a moment and mention that a cloud guru has learn Docker by doing, which
[1348.50 --> 1353.42]  is a course that gives you a series of hands-on labs that are picked to showcase Docker and
[1353.42 --> 1354.34]  gain experience with it.
[1354.38 --> 1355.82]  You hear us talk about Docker all the time.
[1356.06 --> 1359.46]  If you want to learn Docker, you can learn it faster and better when you learn by doing.
[1359.76 --> 1361.42]  So check out the link in the show notes.
[1361.82 --> 1366.34]  They have a fundamentals course that features a 100% hands-on experience.
[1366.96 --> 1370.72]  Everything in the course is inside a real Linux environment provisioned with whatever you
[1370.72 --> 1374.38]  need through ACG's hands-on lab and cloud playground platform.
[1374.92 --> 1375.78]  There's no reason to wait.
[1376.10 --> 1377.38]  Learn by doing today.
[1377.56 --> 1379.24]  Get started at thecloudguru.com.
[1379.24 --> 1380.90]  Hello, people.
[1381.28 --> 1381.76]  Wake up.
[1381.96 --> 1383.24]  Chris and the Badger.
[1383.36 --> 1383.68]  Morning.
[1384.06 --> 1384.74]  All right, let's go.
[1384.82 --> 1385.22]  Let's go.
[1385.30 --> 1385.82]  Let's get up.
[1385.96 --> 1387.64]  Or whenever you happen to listen to it, I guess.
[1387.88 --> 1389.42]  On selfhosted.show.
[1390.26 --> 1391.06]  Isn't that amazing?
[1391.40 --> 1392.68]  That's so good.
[1393.00 --> 1396.50]  That's exactly what I was thinking of when I was talking about it.
[1396.58 --> 1397.92]  Do you know who sent that in?
[1397.96 --> 1399.42]  Because it's pure amazement.
[1399.66 --> 1400.14]  I do.
[1400.24 --> 1400.46]  Yeah.
[1400.64 --> 1403.20]  Someone on the Discord with the username, oh, yeah.
[1403.88 --> 1405.10]  That's perfect, actually.
[1405.66 --> 1406.06]  Wow.
[1406.80 --> 1407.82]  Yeah, I really like that.
[1407.94 --> 1409.04]  Yeah, I could see it, Alex.
[1409.18 --> 1413.84]  You know, you and I in another reality, we're just two morning AM DJs talking about people's
[1413.84 --> 1416.66]  tech problems and telling people about the morning commute.
[1417.06 --> 1417.96]  And the traffic.
[1418.38 --> 1418.50]  Yeah.
[1418.54 --> 1418.88]  Yes.
[1419.40 --> 1420.70]  Let's cut to the chopper.
[1421.06 --> 1421.24]  Yeah.
[1421.84 --> 1424.00]  We'd be good at it, I think, though, you know.
[1424.18 --> 1425.00]  Are we silly enough?
[1425.00 --> 1428.06]  Your whole bit would be like a silly face holding a coffee cup, right?
[1428.14 --> 1429.88]  And my thing would be hats.
[1429.88 --> 1434.58]  But it's a radio show, so it only works in the promotional material.
[1435.32 --> 1439.40]  We had a question from Gone in a Flash on Twitter, and he asked,
[1439.68 --> 1445.02]  I'm thinking about retiring my Docker on Rancher OS setup as it doesn't support Docker Compose.
[1445.58 --> 1449.90]  What's the most supported and easy way to manage an alternative Docker system?
[1450.08 --> 1450.98]  Is it something on Ubuntu?
[1451.56 --> 1454.12]  Is that light and small as possible?
[1454.34 --> 1454.66]  Thanks.
[1455.06 --> 1455.64]  Gone in a Flash.
[1455.64 --> 1460.72]  So he wants to move off of Rancher OS and embrace the Docker Compose lifestyle and is
[1460.72 --> 1462.88]  wondering what the simplest minimalist stack is.
[1463.64 --> 1463.86]  Whew.
[1464.56 --> 1468.06]  That's a hard question to answer because we don't know exactly what his use case is.
[1468.40 --> 1469.42]  What would you go, though?
[1469.48 --> 1470.44]  What would be your go-to?
[1471.20 --> 1472.18]  Perfectmediaserver.com.
[1473.04 --> 1473.38]  Yeah.
[1473.62 --> 1474.82]  That's an Ubuntu base, right?
[1475.30 --> 1475.58]  Yeah.
[1475.58 --> 1478.38]  So I base that off of Ubuntu 2004.
[1479.08 --> 1483.86]  I use an answerable role by GeelingGuy to install Docker.
[1484.42 --> 1487.38]  Although you could, of course, just install Docker however you like.
[1488.22 --> 1490.26]  Install Docker Compose, and that's it.
[1490.30 --> 1490.56]  You're done.
[1490.88 --> 1492.04]  Really isn't a lot to it.
[1492.38 --> 1495.36]  I think it's funny that this is coming from a Red Hat employee.
[1495.54 --> 1501.84]  If anybody ever needed proof that Alex is independent and speaks his mind, there you have it.
[1501.84 --> 1506.28]  But I think that's a fantastic setup, too, because the community support is huge.
[1506.72 --> 1511.92]  The free five-year patches from Canonical on an LTS are pretty tough to beat at this point.
[1513.88 --> 1516.80]  There's other games in town, but yeah.
[1517.34 --> 1521.04]  Well, I've avoided commenting on the whole CentOS thing quite deliberately,
[1521.04 --> 1523.76]  because obviously Red Hat pay my mortgage.
[1524.02 --> 1530.14]  But, you know, I feel somewhat vindicated in my choice of using Ubuntu for my personal systems
[1530.14 --> 1534.80]  and keeping that separation between work and pleasure with all this news.
[1535.02 --> 1537.16]  So it's been an interesting time.
[1537.62 --> 1542.10]  I know this is what nobody wants to hear right now because it's just too damn reasonable and low-key,
[1542.38 --> 1549.10]  but I will go on record right now in early 2021 and say that I bet you CentOS Stream
[1549.10 --> 1551.90]  makes for an excellent containers platform.
[1552.22 --> 1557.48]  If you wanted to run Docker or Podman, CentOS could make a great host OS,
[1557.48 --> 1560.90]  because, I mean, what was the thing that people loved about Core OS?
[1561.38 --> 1566.96]  It was essentially rolling updates at an enterprise scale for an enterprise distribution to run your containers.
[1567.86 --> 1570.22]  And what's CentOS Stream now?
[1570.70 --> 1576.48]  It's going to be a consistently updated rolling enterprise-grade distribution that can run your containers.
[1576.98 --> 1583.68]  I think it's worth considering going down that route, especially if you work with Red Hat systems.
[1583.68 --> 1587.38]  But otherwise, I just really have to agree with Alex.
[1587.84 --> 1593.30]  I think the Ubuntu ecosystem makes for a fantastic home server because there's such a good community support system out there.
[1593.74 --> 1597.38]  Canonical really has their eye on the ball when it comes to their LTS releases.
[1598.00 --> 1600.54]  And cloud support is just fantastic as well.
[1601.16 --> 1603.60]  I mean, you could go with Debian without much penalty.
[1603.82 --> 1606.78]  The reason that I go with Ubuntu really is for a couple of reasons.
[1607.16 --> 1610.68]  The first is ZFS support baked right into the kernel.
[1610.68 --> 1613.20]  That may or may not be important to you.
[1613.40 --> 1616.28]  The other one is WireGuard support baked right in as well.
[1616.36 --> 1619.88]  So for both of those things, you only have to install the user space tool.
[1619.98 --> 1623.26]  You don't have to do any DKMS modules or anything crazy like that.
[1623.78 --> 1625.58]  You could do the same thing on Debian.
[1625.84 --> 1631.94]  And arguably, you know, if you're a freedom-respecting person, like I purport to be,
[1632.20 --> 1633.74]  I should be running Debian everywhere.
[1633.74 --> 1637.30]  But I don't like DKMS, so I run Ubuntu everywhere.
[1637.30 --> 1637.58]  Yeah.
[1637.80 --> 1643.00]  And having seen a bit behind the curtain for the Ubuntu development process,
[1643.36 --> 1648.14]  I am keenly aware of the kind of attention that Canonical puts into an LTS.
[1648.32 --> 1650.64]  It's not that they don't put a lot of work into their other releases,
[1650.98 --> 1655.18]  but they really want to make sure that thing is enterprise-grade and supportable
[1655.18 --> 1657.30]  for the time that they're committed to support it.
[1657.30 --> 1663.30]  And that means it just gets a level of polish and pass that maybe Debian 9 doesn't.
[1663.30 --> 1665.92]  I just wish they'd stop pushing snaps.
[1666.54 --> 1670.08]  You know, it's such easy fodder for people when they come to me and say,
[1670.14 --> 1673.18]  oh, you shouldn't use Ubuntu because snaps are horrible.
[1673.76 --> 1677.32]  And, you know, when I want to install Docker, I don't want to install Docker as a snap.
[1677.40 --> 1678.86]  I just want it as a package and stuff.
[1678.94 --> 1679.68]  And I'm like, yeah.
[1679.84 --> 1680.56]  Well, yeah.
[1680.60 --> 1684.66]  I mean, you can go and grab the Docker dev file from wherever you like and install it.
[1684.70 --> 1685.84]  But the default is a snap.
[1685.94 --> 1688.20]  And as I always say, default is king.
[1688.52 --> 1690.74]  So yeah, I'm torn on that.
[1690.74 --> 1692.64]  I myself don't prefer it.
[1692.78 --> 1698.16]  But I've also heard from audience members who dip their toes into NextCloud for the first time
[1698.16 --> 1701.48]  because it was just a snap away and it was approachable for them.
[1701.76 --> 1705.24]  And, you know, like we got that email from the one guy who set it up on a snap first
[1705.24 --> 1707.22]  and then migrated it to a whole instance afterwards.
[1708.00 --> 1714.66]  I just don't like, I suppose, how snap is an Ubuntu canonical thing.
[1714.66 --> 1719.06]  I don't know, I can't really explain it or articulate it very well,
[1719.20 --> 1722.50]  but I feel like the packaging system should almost be vendor agnostic,
[1722.70 --> 1727.10]  which is kind of where Docker really wins or containers in general really win.
[1727.42 --> 1728.10]  Containers do, yeah.
[1728.16 --> 1730.12]  They'll just run on any Linux kernel.
[1730.36 --> 1731.44]  It doesn't really matter which.
[1731.80 --> 1736.02]  Yeah, I think there is some things that are always going to be vendor specific.
[1736.40 --> 1738.80]  Debian's always going to have apt and that's unique to them.
[1738.80 --> 1740.98]  You know, Debian and Debian derivatives.
[1741.50 --> 1747.82]  But there's some things that people really want to be vendor neutral in the Linux ecosystem.
[1748.00 --> 1751.14]  And it seems software distribution at that level is one of them.
[1751.60 --> 1755.34]  And I also can appreciate that a lot of projects want to host their own repositories.
[1755.38 --> 1760.62]  And I think that's what's really been nice for Flatpaks is you could host your own Flatpak repository.
[1761.14 --> 1763.64]  And, you know, I think our audience understands why people might prefer that.
[1763.88 --> 1764.94]  You can't do that with snaps.
[1765.40 --> 1766.62]  I mean, they have their place, don't they?
[1766.62 --> 1770.26]  But then again, when I'm on my desktop, I'll run Arch.
[1770.76 --> 1773.54]  Everything is just in one place.
[1773.62 --> 1775.28]  There's no installing repos.
[1775.38 --> 1776.74]  It's just all in the AUR.
[1776.98 --> 1784.46]  And if we could somehow get the AUR for every Linux distro, then problem solved, right?
[1784.68 --> 1786.94]  It sounds silly, but I agree so much.
[1787.36 --> 1788.54]  It's so nice.
[1788.68 --> 1791.02]  Just it's I manage everything with yay.
[1791.36 --> 1792.88]  It's yay for anything.
[1793.18 --> 1796.00]  And there's never any math of is this going to be isolated?
[1796.00 --> 1796.86]  Is this a Flatpak?
[1796.94 --> 1797.52]  Is this a Snap?
[1797.60 --> 1798.54]  Is this an app image?
[1798.82 --> 1800.24]  Is this an out of date version?
[1800.36 --> 1801.86]  I never have any of those questions.
[1802.26 --> 1803.56]  And you don't even have to Google it.
[1803.68 --> 1807.00]  You just search in yay first and nine times out of 10, you'll find it.
[1807.36 --> 1809.06]  It's so nice on the workstation side.
[1809.14 --> 1810.78]  Now, here's the thing, and I'll just wrap it up with this.
[1811.22 --> 1817.18]  Here's where I think snaps do play a role because I've seen this side of it too, is in the business world, it generally works.
[1817.18 --> 1824.34]  If you have something that's of a high value, like a piece of software like Adobe might have or Blackmagic or whoever, you want to talk to another company.
[1824.46 --> 1830.54]  You want to work with another company and you want to have a legal relationship and then you want to have like cross team relationships.
[1830.54 --> 1841.92]  So the packaging people at Plex, for example, interface with the Snap people at Canonical and they actually have a business to business relationship, Plex and Canonical.
[1842.46 --> 1848.16]  And there is a vendor relationship there where I think just for Plex, they package for everything.
[1848.16 --> 1862.14]  But I think a lot of companies like that kind of traditional relationship and that's a role where snaps can really kind of be more appealing to the commercial software industry because they can have an agreement with Canonical.
[1862.34 --> 1864.14]  They can distribute via Canonical store.
[1864.76 --> 1869.66]  It works on most distributions and they are the ones that can publish.
[1870.66 --> 1877.38]  I think that's really appealing to that type of business, but it just doesn't seem to really be appealing to community use cases as much.
[1878.16 --> 1882.30]  Despite all that I just said about snaps, I still use Ubuntu everywhere.
[1883.02 --> 1884.68]  Yeah, and you really learn the tricks.
[1885.08 --> 1886.24]  You know, you learn the tricks.
[1886.44 --> 1890.22]  I follow the directions on the Docker site for getting Docker set up really.
[1890.30 --> 1891.52]  I don't even use it from the repos.
[1891.68 --> 1894.66]  Yeah, get.docker.com and then pipe it to sudo bash, right?
[1894.84 --> 1895.78]  You could do that.
[1896.02 --> 1897.02]  You definitely could.
[1897.14 --> 1897.84]  What could go wrong?
[1897.94 --> 1905.62]  I thought maybe I should summarize like several emails we've gotten over the last couple of weeks since we talked about Powerline networking, which just super brief follow up.
[1905.74 --> 1906.38]  Still working awesome.
[1906.38 --> 1909.98]  I haven't even had to reset any of like the adapters or anything.
[1910.20 --> 1911.64]  They're still working great.
[1912.18 --> 1913.62]  It's like having Ethernet.
[1913.70 --> 1914.46]  It's so wonderful.
[1914.54 --> 1915.24]  It's just slightly slower.
[1915.62 --> 1917.82]  We have had a few people write in that have told me.
[1918.34 --> 1922.98]  Actually, we had a whole range of concerns like from my solar is going to generate too much interference.
[1923.12 --> 1927.70]  But of course, they're separate systems to turning my RV into a radio broadcast system.
[1928.04 --> 1931.90]  I don't think we've had a topic that has been quite so feedback generating.
[1931.90 --> 1935.82]  Yeah, it's really and a wide range of successes and failures.
[1935.96 --> 1938.06]  But there has been one consistent theme.
[1938.28 --> 1941.98]  And that is you got to go to the next level if you really want this to work great.
[1942.22 --> 1944.58]  And that is check out Ethernet over coax.
[1944.76 --> 1947.34]  People have been writing that in for a couple of weeks straight now.
[1947.34 --> 1955.84]  And the ActionTech MOCA network adapter for Ethernet over coax 2 pack has been linked a couple of times.
[1955.84 --> 1961.14]  And the word from these emails is it's night and day difference way better.
[1961.38 --> 1966.44]  If you if you've got coax pre run in your place, it's a way better route to go than power over Ethernet.
[1967.26 --> 1968.94]  Apparently haven't tested it myself.
[1969.08 --> 1973.98]  I do have a bit of coax, not in the areas where I would want to have servers.
[1974.90 --> 1976.76]  But I do have a bit of coax in the RV.
[1976.88 --> 1978.98]  So maybe at some point it could be useful.
[1979.44 --> 1984.04]  I could see maybe using it for like, say, a Nvidia Shield hookup or something where the TV is already at.
[1984.04 --> 1985.30]  And that's where a coax connection is.
[1985.30 --> 1987.08]  I think that's a perfect use case.
[1987.20 --> 1990.26]  Something I mean, a Shield's not going to be using crazy amounts of bandwidth.
[1990.96 --> 1995.68]  But the other thing to consider as well is that coax is a lot cheaper than Ethernet cable.
[1996.14 --> 2008.84]  And it can be purchased a lot cheaper than weatherproof Ethernet as well, which is also, you know, if you want to run it from the attic, say, down to your basement, probably the easiest route is going to be out the side of the building.
[2009.20 --> 2011.14]  And doing that with Ethernet could get expensive.
[2011.14 --> 2013.90]  So it's definitely an interesting thing.
[2013.96 --> 2015.34]  And it's not something I considered before.
[2015.52 --> 2017.84]  So I don't know, maybe next house.
[2018.24 --> 2019.48]  I'll give it a whirl.
[2019.84 --> 2022.24]  I'm going to keep it in my back pocket for a future project.
[2022.34 --> 2024.12]  And it has a cool acronym too.
[2024.54 --> 2024.84]  Mocha.
[2025.28 --> 2026.02]  M-O-C-A.
[2026.34 --> 2026.62]  Mocha.
[2026.92 --> 2027.88]  Mo-C-A-C-E-N-O.
[2027.88 --> 2028.18]  Mocha.
[2028.18 --> 2029.24]  So I kind of like it already.
[2029.46 --> 2030.08]  Sounds delicious.
[2030.30 --> 2030.52]  Mocha.
[2030.70 --> 2035.06]  If the reports from the email are true, it's like if they say it's a gigabit, it's a true gigabit.
[2035.14 --> 2036.12]  It's actually that fast.
[2036.62 --> 2037.06]  Mocha.
[2037.06 --> 2037.18]  Mocha.
[2037.18 --> 2037.46]  Mocha.
[2037.46 --> 2037.54]  Mocha.
[2037.54 --> 2037.82]  Mocha.
[2037.94 --> 2038.00]  Mocha.
[2038.00 --> 2038.12]  Mocha.
[2038.12 --> 2038.26]  Mocha.
[2038.26 --> 2039.14]  Mocha.
[2039.14 --> 2040.22]  Mocha.
[2040.22 --> 2041.30]  Mocha.
[2041.30 --> 2042.08]  Mocha.
[2042.08 --> 2042.38]  Mocha.
[2042.38 --> 2042.46]  Mocha.
[2042.46 --> 2042.64]  Mocha.
[2042.64 --> 2043.32]  Mocha.
[2043.32 --> 2044.48]  Mocha.
[2044.48 --> 2047.00]  our site reliability engineers who support the show.
[2047.32 --> 2048.50]  They keep us independent.
[2048.74 --> 2051.28]  They get a limited ad feed available to them as a member,
[2051.48 --> 2053.76]  and they get a little bit of extra content, a post-show.
[2054.18 --> 2056.38]  So if you'd like to support the show and become a member,
[2056.52 --> 2058.72]  go to selfhosted.show slash SRE.
[2059.08 --> 2062.00]  Yes, big thank you to our site reliability engineers.
[2062.30 --> 2066.18]  You can go to selfhosted.show slash contact to get in touch with us,
[2066.26 --> 2068.56]  and you can find me on Twitter at Ironic Badger.
[2068.78 --> 2069.32]  I'm there too.
[2069.44 --> 2074.04]  I'm at Chris LAS, and the show is at selfhostedshow.
[2074.04 --> 2076.52]  Don't forget at Jupitersignal for the network.
[2076.90 --> 2077.54]  Thanks for listening.
[2077.78 --> 2080.00]  That was selfhosted.show slash 36.
