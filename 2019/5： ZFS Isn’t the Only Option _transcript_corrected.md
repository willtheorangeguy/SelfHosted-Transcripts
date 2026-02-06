[0.00 → 1.20] So far, I think I hate Shinobi.
[1.34 → 1.84] Oh, no.
[2.06 → 3.44] I thought I was going to love it.
[3.52 → 3.70] Yeah.
[3.90 → 4.12] No.
[4.34 → 4.88] I think I hate it.
[5.00 → 5.84] You're supposed to love it.
[6.12 → 6.42] I know.
[6.48 → 9.84] And I went, and I bought all the cameras before I even tried it.
[9.90 → 12.04] So I got five Waze Cams.
[12.62 → 15.68] I ref lashed all the Waze Cams to the RTSP firmware.
[16.06 → 18.78] So that way I could just stream directly from them over my LAN.
[18.78 → 22.72] I got a Raspberry Pi 4 dedicated to the Shinobi installation.
[23.40 → 25.40] Set up the Shinobi DVR software.
[25.96 → 27.60] Or I guess it's not technically DVR.
[27.60 → 31.76] It's whatever the term is for a closed circuit recording system.
[32.06 → 33.14] Got it all loaded up.
[33.78 → 35.48] And I'm just not thrilled.
[35.58 → 37.92] First, by default, it doesn't support motion detection.
[38.04 → 40.44] That's a plug-in which is broken right now on ARM.
[41.72 → 46.08] And just three cameras is slamming the Pi.
[46.90 → 48.48] Maxed out all the cores on the Pi.
[49.02 → 50.08] That's a real shame.
[50.52 → 52.50] I mean, I've used Shinobi a little bit.
[53.14 → 54.54] I'm not an expert.
[54.72 → 56.88] I've got three Waze Cams feeding into it here.
[56.88 → 58.56] And it's running on my big Leon downstairs.
[58.82 → 62.42] But the interface is a little bit confusing, I've found at times.
[62.62 → 62.80] Right?
[62.88 → 65.72] So when you're trying to pull in the feeds, you have to set all sorts of parameters.
[66.28 → 66.64] Yeah.
[66.84 → 69.04] And I think I may have some finessing to do there.
[69.70 → 73.02] And I probably should also mention the big caveat that I did.
[73.84 → 77.10] I broke my own rule with using the Raspberry Pi 4 in production.
[77.10 → 79.48] And I did not put Raspbian on it.
[79.88 → 81.84] Because I'm not super comfortable with Raspbian.
[82.06 → 86.58] And when it does big update and stuff, I just don't have experience with it to trust it.
[86.86 → 92.44] I'd rather use like an LTS Ubuntu or a CentOS, something that I just have more faith in.
[92.44 → 94.86] And I let that doubt get to me.
[95.12 → 103.80] And I loaded it with a community build of Ubuntu 18.04 LTS that swaps out Ubuntu's kernel and puts the Raspbian kernel in.
[104.12 → 107.54] And I thought, maybe this will work pretty well.
[107.68 → 108.96] Maybe it'll support all the drivers.
[109.12 → 109.94] But maybe it's not.
[109.94 → 114.68] And so today I brought the Raspberry Pi in with me into the studio.
[114.92 → 121.42] I'm going to ref lash it over to Raspbian, reset up Shinobi on that, and then see if maybe I have better GPU acceleration.
[121.64 → 123.60] Because I need to pull in more cameras than three.
[123.78 → 127.94] And so if it can only do three cameras, I don't think I'm going to do a Pi for every three cameras.
[128.04 → 129.40] I think I'd have to go to x86.
[129.88 → 130.72] Yeah, that's a bit expensive.
[131.02 → 137.26] Are you running into issues when you load up the UI, the web interface, or is it just constantly slammed?
[137.70 → 144.20] It's definitely worse when the web UI is up, but it's still very slammed even when I don't have the web UI running.
[144.62 → 151.14] The other thing is, is in Shinobi I'm seeing more frame loss, like chunks of the video go missing, you know, like with encoding errors.
[151.52 → 157.54] I do not have that same problem when I open up the same video stream and just pass the URL to MPV or VLC.
[157.80 → 159.10] Opens right up, no problem.
[159.10 → 159.40] Yeah.
[159.78 → 166.62] If I had a tiling window manager and could just put eight, you know, versions of VLC, that might work well.
[166.62 → 172.02] So you know what I've done in the meantime, and it's not great, but I've pulled the RTSP feeds into Home Assistant.
[172.30 → 173.20] Oh, how's that working?
[173.44 → 173.84] Pretty good.
[173.90 → 174.58] I get real time.
[174.70 → 184.76] I don't get recording, but I now just have a tab in my Home Assistant dashboard called security, where I've put my motion sensors, my outside cameras, and my inside cameras all on one tab.
[184.88 → 186.42] I tap that and pulls them all up.
[186.70 → 189.52] So it's a really nice just get a look at the state of things.
[190.32 → 191.44] It works really well for that.
[191.44 → 203.28] We haven't really touched on your camera setup much yet, and I think we'll probably get to it in a future episode of like the perfect IP camera, the perfect POE camera, like if such a thing even exists, right?
[203.38 → 203.84] Oh, totally.
[203.96 → 205.58] Yeah, we can totally do a dedicated episode.
[205.88 → 212.46] I'm holding on to this Y stuff just for a little bit longer because I'd really like to figure out how to make it work for people.
[212.46 → 219.42] Because these are $25 cameras that you can put RTSP support on, and they make for such a great addition to your home security.
[219.76 → 222.32] And they support person detection, motion detection.
[222.68 → 230.14] They have two-way speakers and a microphone, obviously, for $25, and you can completely run them offline on your own local LAN.
[230.48 → 238.70] So I'm going to stick with it for a bit, see if I can't tweak my Shinobi config, because I'd love to come on the show and tell people how to get it all rocking on a Pi with Waze Cams.
[238.70 → 242.06] Because for $100, you could have a full camera security system.
[242.06 → 245.38] For the price of one, not even, one Nest Cam.
[245.68 → 245.84] Yeah.
[246.38 → 250.14] The other thing is, is I was not able to get Shinobi running in a container.
[250.48 → 255.28] I've had, like, that's the first application where it's like, I bailed on the container approach and built it on the host.
[255.46 → 258.84] Bro, you should, you know, hook up your container expert over here.
[258.94 → 260.64] No, I thought about bugging you, actually.
[261.14 → 264.62] But I thought you were dealing with your own container issues at the time, so I didn't want to bother you.
[264.86 → 265.32] Oh, probably.
[265.32 → 271.54] Yeah, actually, interestingly enough, so I mentioned Stating in an episode recently.
[272.06 → 279.82] And Joe Kensington pinged me a few hours after it aired and went, Alex, your Stating is down.
[280.10 → 281.16] And I'm like, no.
[281.64 → 284.42] I thought I'd been DDoS'd by the show audience or something.
[284.50 → 287.90] But it turned out I'd actually just been a bit honey badger with the updates.
[287.90 → 290.84] The ironic badger goes honey badger.
[291.02 → 291.38] Right.
[291.66 → 296.52] So I have this, I use Docker Compose to do all of my container management.
[296.92 → 302.22] I just, you know, log in randomly and just do Docker Compose pull, Docker Compose up.
[302.96 → 305.74] And that's my update process for updating my apps.
[305.80 → 306.66] It's as simple as that.
[307.38 → 309.04] I probably should script it, right?
[309.04 → 312.76] I should probably have like DigitalOcean do a backup, or what's it called?
[312.78 → 318.84] A snapshot via the API and then do the updates and then have some kind of sanity checks afterwards.
[318.84 → 321.66] But I'm not doing this for business.
[321.80 → 323.82] I'm doing this for my own personal pleasure.
[324.14 → 324.98] You do know better.
[325.08 → 326.50] You're just choosing not to do it.
[326.60 → 327.36] I just couldn't be bothered.
[327.68 → 327.78] Yeah.
[328.46 → 329.84] All the config is in Ansible.
[329.98 → 332.56] So at least I have it all, you know, stored in Git somewhere.
[332.56 → 334.48] So I'm not going to lose it overnight.
[334.78 → 338.56] But anyway, the interesting issue with this one was I logged into the droplet.
[338.68 → 345.38] I was actually in a hotel room in Florida at the time, connected via my slate WireGuard VPN,
[345.80 → 350.44] you know, the little travel router, connected back to my house in Raleigh.
[350.68 → 352.32] I'm ordering another one of those slates.
[352.54 → 356.00] I've got to, we talked about it recently, like two episodes ago,
[356.00 → 362.28] but this is a little open WRT powered box that has WireGuard support and CAPTCHA support.
[362.28 → 365.58] So you can throw it on a hotel Wi-Fi, VPN up all your traffic.
[366.02 → 369.02] And that becomes the access point for every device in your room.
[369.42 → 372.32] I'm travelling mid-November, and I'm picking one of those up for the trip.
[372.76 → 373.04] Good shout.
[373.40 → 374.54] I swear I should be on commission.
[374.66 → 377.04] I think I've sold about 15 of those devices since then.
[378.34 → 378.70] Really?
[379.14 → 380.82] They don't have like an affiliate deal or something.
[381.02 → 381.40] Yeah, right.
[382.02 → 386.62] So anyway, I logged into the droplet via SSH and I looked at the logs for the container
[386.62 → 388.38] and it said schema error.
[388.52 → 390.92] You're now running Progress 12 instead of 11.
[391.26 → 391.58] Oh.
[391.58 → 391.72] Oh.
[392.16 → 396.08] Stating was running against Postgres 11.
[397.04 → 402.08] So it was just a case of going into the Docker Compose file, adding a tag,
[402.18 → 404.84] because currently I didn't actually have any tag specified,
[405.00 → 406.00] so it was just pulling latest.
[407.12 → 412.76] And so it rolled back from version 12 to version 11 in about eight seconds.
[412.76 → 416.48] When it pulled the old image down again, I pressed Docker Compose up
[416.48 → 419.62] and lo and behold, Stating came straight back up.
[420.00 → 420.60] Isn't that amazing?
[420.60 → 421.94] Oh, it's so good.
[421.94 → 428.80] Are you able to fully appreciate how much better that is than the old way of doing things
[428.80 → 433.50] where if you installed everything via a package, it would have spewed libraries all over your
[433.50 → 438.78] system, and it would have been a massive uncoupling to walk back, especially if other components
[438.78 → 442.28] or applications on the system were dependent on that package?
[442.28 → 446.34] Less than five minutes from diagnosing the issue to having it resolved.
[446.78 → 453.46] It's, I mean, luckily for me, the database hadn't updated its schema itself like automatically or anything like that.
[453.54 → 457.84] But just rolling back the image of the database was super-duper easy.
[457.84 → 462.34] So if you want a sales pitch for why containers are great, that's definitely up there.
[463.50 → 466.34] Containers today on the self-hosted podcast.
[466.70 → 467.20] Yeah, right.
[467.36 → 469.16] That's the container corner segment for today.
[469.16 → 482.64] I have another thing I need to admit is my current storage setup is already starting to fail me because I'm starting to do multiple disks attached directly to the Pi, each Pi, which is now three of them.
[482.84 → 483.42] Via USB?
[483.72 → 484.64] Yeah, USB 3.
[484.64 → 490.36] I don't have super high performance requirements because I'm accessing these mostly over Wi-Fi.
[490.74 → 492.30] So it's just a reliability thing.
[492.38 → 496.66] I've just seen USB devices drop off the bus for no reason.
[497.02 → 498.32] That never happens with SATA.
[498.56 → 504.10] If you run a machine for 100 days, I would way more bet on a USB disk disappearing than a SATA.
[504.10 → 506.06] A SATA just wouldn't disappear unless the disk fails.
[507.54 → 511.32] The other thing is, does I don't have enough storage for the cameras.
[511.32 → 519.38] I don't need a lot of disk, but I'd like probably at least three solid days worth of storage so I can go back if, you know, something happens.
[519.48 → 520.50] A week would be ideal.
[520.96 → 532.90] But also I need to accommodate things like Plex, which holds my books, my audiobooks, my music, my videos, about a terabyte of local media, and some pictures I need to accommodate, some notes.
[533.02 → 540.26] I've also got things like Docker configs and the containers-related data that I all need to store.
[540.26 → 551.02] And I don't know if I should – what I've done so far is I've got, went on sale, these Samsung MV&E drives that are bus powered over USB 3, and they're tiny.
[551.38 → 553.10] I'm holding one up to you now on Telegram.
[553.28 → 554.06] I've just sent you a picture.
[554.26 → 555.98] That's the SanDisk one you have there, right?
[556.02 → 558.12] Yeah, it's not even half the size of a credit card.
[558.24 → 558.44] No.
[558.78 → 559.94] And it's ruggedized.
[560.12 → 561.82] It sort of has a rubber coating.
[562.42 → 566.80] And it's also very well rated in terms of performance with the Raspberry Pi.
[566.80 → 569.26] I just recently went through some disk benchmarks.
[570.04 → 582.10] Here's the other thing that really, really is a tricky thing for me in the RV is whatever disk solution I implement needs to be able to withstand a level 4 earthquake on the Richter scale.
[582.52 → 588.70] Because when I drive, that's essentially what the conditions inside the RV is, is a level 4 earthquake.
[588.70 → 597.82] And so the disks ideally could stay online while we drive because I might have the children on board, and they'd like to watch television or use the services while we're going down the road.
[598.10 → 600.28] Man, that would have made road trips so great as a kid.
[600.50 → 610.28] Can you even imagine just having – not just, you know, I mean, when I was a kid, like, we used to play games in the car, like, count the number plates that start with the letter L, you know?
[610.28 → 611.28] Right, right.
[611.56 → 620.46] Meanwhile, they've got Wi-Fi with internet, and they've got a Plex library of their favourite shows, and they have a total blank check to marathon them because what else can they do?
[620.58 → 623.06] Kids these days don't even know they're born, Chris.
[623.20 → 624.34] I know, I know.
[625.28 → 628.58] And so I need to accommodate all these different factors.
[628.82 → 630.96] So it kind of seems like I need to go solid state.
[631.24 → 632.86] Yeah, you probably do, right?
[632.86 → 636.78] And solid state's getting there, you know?
[637.42 → 650.68] Linus Tech Tips did a video not that long ago about a new 3.84 terabyte – I mean, it's four terabytes to all intents and purposes – SSD released by, I think it was either Samsung or SanDisk, probably Samsung.
[651.28 → 653.24] But they're still $500 a pop.
[653.76 → 659.70] Whereas these one terabyte ones that you're talking about, the ruggedized ones, they're about $100 a pop or something.
[659.70 → 670.30] I mean, it's not cheap, but it's enough now that I can move – so my use case for the little SSD that I have is my photo library lives on here for each year.
[670.70 → 672.82] So every year I'll rotate my photo library.
[673.00 → 679.50] When I'm travelling, like, I just have everything that I've shot this year with me physically and everything else is at home.
[679.90 → 681.96] And generally speaking, that works pretty well.
[681.96 → 686.24] So at the end of each year, I'll rotate my photos.
[686.50 → 691.56] And drone footage is an exception because it's so much bigger, but just images fit just fine on here.
[691.90 → 696.60] Do you only keep the year's images on that disk or do you also store them somewhere else?
[696.80 → 697.22] Oh, so yeah.
[697.30 → 701.88] I mean, I'd be a loser if I only had one copy of my photos from this year, right?
[702.00 → 702.62] This wasn't clear.
[702.86 → 704.06] I was getting upset for a second.
[704.76 → 705.26] Yeah, no.
[705.34 → 708.86] So generally whilst I'm travelling, my use case is quite straightforward.
[708.86 → 712.86] And I actually did a post about this on my blog very recently about my photography workflow.
[713.64 → 722.72] And I talk a little bit in there about how my backup situation works and how by the time it's all said and done, I've probably got about six or seven copies of this data.
[723.46 → 726.74] You know, all automatic once it hits my server back in Raleigh.
[726.82 → 729.66] It just then all sort of spiders webs out across the internet.
[730.00 → 736.22] We should put a link to that in the show notes to that blog post because that could also help answer the Ask SSH we're going to get to in a little bit.
[737.22 → 737.86] Yeah, okay.
[737.86 → 744.90] I mean, so the way I look at it is I have a couple of options here is I could just hang a terabyte disk off of each Pi.
[745.30 → 747.38] So about $300 worth of disk.
[748.12 → 753.62] That's not the end of the world when you're talking about a network storage solution in terms of price, but it's not very elegant.
[754.72 → 760.68] Then I'm wondering if it's just ridiculous and crazy to buy yet another Raspberry Pi.
[761.18 → 761.62] Probably.
[761.62 → 768.20] And then make that thing an iSCSI host for like the biggest disk or the most amount of disk I can attach to it.
[768.36 → 772.20] Can't you just get like a 512 gig SD card these days?
[772.42 → 772.62] Yeah.
[772.70 → 777.98] So the way I tend to use the SD card in the Raspberry Pis is just the root file system is on the SD card.
[777.98 → 781.08] Because I'm just so paranoid they're going to just die on me.
[781.24 → 781.42] Yeah.
[781.64 → 784.62] I've had a few do that, especially in power loss situations.
[784.62 → 785.74] That can be a real issue.
[786.24 → 790.44] So I kind of feel like just like a lot of times in a server, I'll have a small internal SSD.
[790.78 → 790.96] Yeah.
[791.18 → 791.80] I do the same.
[792.08 → 792.24] Yeah.
[792.30 → 793.64] The arrays on a pool of disks.
[793.64 → 807.56] So I had thought about taking a Raspberry Pi 4, attaching like three or four disks to it, and then sharing that out over Samba NFS and making it an iSCSI target as well.
[808.08 → 816.32] And, you know, we talk with the developer of Mergers in an upcoming Jupyter Extra that will probably be released the week this episode comes out.
[816.42 → 818.78] And Mergers could potentially be a solution here.
[819.40 → 821.00] There are a lot of ways I could go with this.
[821.06 → 823.98] So I'm kind of hoping you can give me some of your thoughts on just disks in general.
[824.12 → 831.46] If Mergers maybe would be a good use case for me, especially since I'm dealing with more limited amounts of RAM and hardware.
[831.88 → 836.16] And I know that you and I have been talking offline a lot about your storage setup.
[837.02 → 838.84] So give me an advice here, Doctor.
[838.88 → 839.46] What's your prescription?
[840.12 → 846.30] Well, over the years, I mean, I've talked about on my Brunch with Brent, I talked about how there was a 1.5 terabyte hard drive that failed.
[846.30 → 849.48] And that's kind of what led me down this rabbit hole of self-hosting.
[849.60 → 852.60] And I've bought a lot of hard drives over the years.
[852.68 → 858.70] I was trying to calculate it, but I think I've probably bought somewhere in the region of 30 to 40 three and a half inch drives.
[858.82 → 861.50] Just this is my personal, you know, purchase history.
[862.00 → 862.02] Yeah.
[862.02 → 866.26] I hate to think how much disk I've bought over the years for the JB productions.
[866.78 → 866.94] Oh.
[867.34 → 870.08] So I've got a few, you know, rituals that I follow.
[870.16 → 871.56] I've got a few thoughts.
[872.22 → 876.84] I've read a lot of posts on Reddit, on different forums.
[877.78 → 882.88] And this is just my personal experience over the last five, six, seven years of doing this stuff.
[882.88 → 886.52] I appreciate some people have different opinions, but these are mine.
[887.34 → 893.24] And I think a lot of it boils down to several key things, right?
[893.88 → 899.86] And I cover a lot of this stuff in the Perfect Media Server series that's on the linuxserver.io blog.
[901.20 → 904.12] There are a few things you need to take into consideration, right?
[904.30 → 907.50] First, you know, what are your requirements?
[907.50 → 911.50] Are you running high performance databases?
[912.00 → 917.36] Probably not if you're self-hosting, but things like Plex take a surprising amount of IO, right?
[917.50 → 923.04] So if you're going to put your Plex metadata directory onto a spinning Rust drive,
[923.48 → 927.50] you'll notice a significant speed bump if you then put that onto an SSD later on.
[927.66 → 931.54] So there are just different use cases, even within a home setup that you might want to consider.
[932.12 → 936.46] Also, I think it's worth mentioning there are ways you could even set up spinning Rust
[936.46 → 937.72] to get pretty good throughput.
[937.92 → 941.22] You may miss out on data integrity or protection.
[941.64 → 950.56] Like, for example, forever, for editing, I will use a bunch of as fast as I can get spinning Rust.
[950.64 → 952.32] Usually 10,000 RPM is what I go for.
[952.36 → 955.88] I know I can get slightly faster, but I go for 10,000 usually, so not as fast, I should say.
[956.76 → 958.32] The exact opposite of what I just said.
[959.20 → 960.98] And I'll put those suckers in a RAID 0.
[961.22 → 961.38] Yeah.
[961.84 → 962.80] Fantastic performance.
[962.80 → 968.06] Then I make sure that the disk pool is labelled Scary Raid.
[968.30 → 969.54] I call it Scary Raid.
[969.82 → 970.30] Good.
[970.58 → 971.36] Oh, I like it.
[971.94 → 976.26] So for those that aren't familiar, RAID 0 is striped across both disks.
[976.40 → 982.26] So if either of those disks fail, or any of the disks in the RAID 0 array fail, you're boned.
[982.40 → 982.54] Yeah.
[982.98 → 989.02] And so that Scary Raid label always reminds me, don't trust anything on that array,
[989.10 → 990.18] because you could lose it at any time.
[990.18 → 997.14] Now, when you're working on a video project, in theory, you have your source materials still either on the camera,
[997.32 → 999.72] or on the OBS machine, or however you were doing it.
[1000.04 → 1005.24] And so if my array were to go away during a project, I would just have to redo that project.
[1005.56 → 1009.78] Well, I think a lot of this stuff is a little old school in terms of thinking nowadays.
[1010.08 → 1010.18] Yeah.
[1010.18 → 1014.24] Terabyte SSDs, terabyte SSDs are in that $100 sweet spot, right?
[1014.90 → 1017.44] And we're not talking that long ago.
[1017.54 → 1021.84] We're talking, you know, two, three years when a terabyte was $300 or $400.
[1021.84 → 1024.60] And that's just not realistic.
[1024.80 → 1027.24] You know, I'm not going to spend that much on that price per gigabyte.
[1028.10 → 1030.98] Which leads me nicely on to my other consideration, right?
[1030.98 → 1034.22] You need to decide what capacity requirements are.
[1034.26 → 1040.70] So if you're working on video like Chris, you know, you're going to be needing hundreds of gigabytes
[1040.70 → 1042.36] for a single project, potentially.
[1042.36 → 1048.66] It is funny because when we switched to primarily doing audio, all of a sudden I had to do this
[1048.66 → 1049.72] huge shift on it.
[1049.78 → 1053.92] We had so much additional storage because we had projected for the next couple of years
[1053.92 → 1056.52] using video, and then we made a transition to audio.
[1057.02 → 1059.62] And then all of a sudden I went a year without having to buy discs.
[1059.72 → 1060.72] It was beautiful.
[1061.06 → 1066.34] And now in the RV with my limited options, I think about storage differently.
[1066.34 → 1073.02] I think, what do I need immediately available versus what can I store in like a colder storage
[1073.02 → 1075.24] that's remote and slower to get to?
[1075.32 → 1079.74] So I kind of even break it up to what do I need is hot files versus cold files.
[1079.90 → 1085.52] And so the hot files I'll put on the SSDs and the cold files I'll store on spinning rust
[1085.52 → 1085.86] somewhere.
[1086.02 → 1088.44] Like here in the studio, we have plenty of spinning rust storage.
[1088.88 → 1093.44] So the other thing to consider is that there's an article by a chap called, and I'm going to
[1093.44 → 1095.36] butcher this name, Laurentian.
[1095.36 → 1097.36] And this is from January 2016.
[1097.36 → 1103.78] And it's actually been something which has influenced my strategy and how I've purchased
[1103.78 → 1105.86] hard drives pretty much since then.
[1106.08 → 1107.02] It's like a thought model, huh?
[1107.20 → 1107.44] Yeah.
[1107.52 → 1111.86] And this post is entitled, the hidden cost of using ZFS for your home NAS.
[1112.58 → 1117.04] Now I want to underscore the last two words for your home NAS.
[1117.20 → 1118.84] I'm not talking about small business.
[1118.94 → 1120.78] I'm not talking about your use case here, Chris.
[1120.78 → 1126.70] Um, I'm talking about, you know, people like me that have a media server, which has five,
[1126.78 → 1133.88] six, seven, eight, nine discs in it that stores, uh, media that is written once and read a few
[1133.88 → 1139.88] times date, you know, things like drone footage, um, ripped media, music, that kind of stuff.
[1139.88 → 1140.12] Right.
[1140.16 → 1143.12] That is not, you know, the performance is not critical.
[1143.12 → 1149.54] So a lot of the benefits that you get with ZFS kind of pale into insignificance, but the
[1149.54 → 1156.94] the thrust of his blog post here, and I totally agree with this is that when I'm expanding my NAS
[1156.94 → 1162.28] over the last few years, I, I tend not to buy more than one or two drives at the same time.
[1162.28 → 1168.38] Um, I tend to buy one drive every, if I know I'm expanding, I'll buy a drive every month or two.
[1168.98 → 1174.34] Um, generally speaking, I, I, over the last couple of years, I've bought a drive every six to seven
[1174.34 → 1175.02] months or so.
[1175.58 → 1181.70] Um, now with ZFS, that's just not going to work because you need to pre-allocate your, uh, V devs
[1181.70 → 1184.94] and your pools and all that kind of stuff, uh, upfront.
[1184.94 → 1187.84] So you need to have drives that are the same size.
[1187.84 → 1192.86] You need to ideally have drives that are the same brand and firmware models so that there's
[1192.86 → 1197.50] not some kind of random problem occurs at the, at the hardware level there.
[1197.96 → 1204.68] Um, and so for me, it really makes the ZFS kind of sell a lot more difficult because purchasing
[1204.68 → 1208.06] multiple drives at once is not realistic.
[1208.94 → 1214.66] Now, then I moved to America and I had access to Best Buy, and they have this wonderful thing
[1214.66 → 1217.48] called the, the Western Digital Easy Store.
[1217.84 → 1220.12] And this, this has really changed the game for me.
[1220.12 → 1227.72] So I now, uh, have access to 10 terabyte hard drives, 10 terabyte drives.
[1227.84 → 1229.52] Just one drive is 10 terabytes.
[1229.78 → 1234.84] My entire array used to be 10 terabytes, but anyway, for 160 or $170.
[1235.48 → 1239.10] The caveat is it comes in like a USB enclosure.
[1239.10 → 1240.92] So it's like an external hard drive.
[1241.28 → 1245.50] Um, but you can pop those bad boys out of those cases in 10 minutes flat.
[1245.50 → 1251.62] And then you have, to all intents and purposes, a white label, Western Digital 10 terabyte
[1251.62 → 1252.36] hard drive.
[1252.70 → 1256.74] And they're generally of decent quality discs too, because, um, they don't want them popping
[1256.74 → 1258.56] and then having a consumer, uh, RMA.
[1258.78 → 1263.06] There is also like a is there like a slight electrical bit of work that has to be done
[1263.06 → 1264.50] to the disc once you shuck it?
[1264.70 → 1265.72] Well, that's an interesting one.
[1265.76 → 1269.22] So this, I think you're referring to the 3.3 volt mod that you might have to do.
[1269.34 → 1269.98] That's what it was.
[1270.00 → 1270.14] Yeah.
[1270.14 → 1273.46] And this is actually in the SATA spec, the SATA power spec.
[1273.88 → 1277.12] I read, I read a post on this a few months ago, so I might get the details a little bit
[1277.12 → 1285.20] wrong, but the gist is this enterprise gear uses the 3.3 volt rail to reset failing hardware.
[1285.20 → 1290.90] So if you're a hard drive in a data centre, you don't necessarily want to have to be power
[1290.90 → 1294.48] cycled physically by a human coming in and pushing a button and all that kind of stuff.
[1295.10 → 1299.56] Data centres need a way to reset hardware without physically being present.
[1299.56 → 1303.30] And the way in which hard drives do that is on the 3.3 volt rail.
[1303.76 → 1310.46] So in a server situation, if that disc receives a signal on the 3.3 volt rail, it will reboot
[1310.46 → 1311.82] just that disc.
[1312.26 → 1319.26] Now, most consumer power supplies over the last decade have either omitted that, um, rail
[1319.26 → 1323.30] or just not followed the SATA spec for, you know, trying to save money because nobody really
[1323.30 → 1324.28] uses it for power.
[1324.40 → 1326.42] They just use it for that use case.
[1326.42 → 1330.66] But some power supplies do respect the SATA spec.
[1331.00 → 1334.52] And if yours is one of those, you need to do one of two things.
[1335.00 → 1340.08] The first option is you can either just cut the 3.3 volt wire, which is what I did.
[1340.18 → 1345.56] I actually made some custom SATA power connectors, which omitted that wire altogether.
[1345.56 → 1352.14] Uh, you can buy, I think it's a one to five SATA power splitter thing on Amazon.
[1352.52 → 1358.02] And then you can use the DIY, uh, SATA power connectors and just sort of pull the cable
[1358.02 → 1360.48] down inside it and slice and cut the connectors for you.
[1361.06 → 1364.28] It takes about half an hour to do five, uh, the first time.
[1364.28 → 1365.54] And then you get quicker after that.
[1366.14 → 1366.96] Just be careful.
[1366.96 → 1368.86] You get the wires in the right order.
[1368.86 → 1372.34] Cause if you put the 12 volt rail on the five volt thing, you're going to let the magic
[1372.34 → 1372.84] smoke out.
[1373.12 → 1373.74] Not that you would know.
[1373.96 → 1375.04] No, I actually don't.
[1375.22 → 1378.66] But yeah, thankfully I was very careful when I checked with a multimeter that I got it all
[1378.66 → 1378.98] correct.
[1379.86 → 1384.22] Um, the other thing you can do, and there are plenty of videos on YouTube on this is you
[1384.22 → 1388.92] can actually get a piece of Tapton tape, uh, or something like electrical tape or something
[1388.92 → 1392.94] and cover a couple of the power pins on the drive itself.
[1393.22 → 1395.52] So that's a very, very non-destructive mod.
[1395.56 → 1395.84] Okay.
[1395.92 → 1400.12] And that will just prevent the drive from being able to receive that 3.3 volt signal and it
[1400.12 → 1402.14] will just work as you would expect.
[1402.32 → 1403.14] That's not so bad.
[1403.14 → 1409.38] I do agree, um, with your overall assessment that if you're going to implement ZFS, you need
[1409.38 → 1412.80] to go into it knowing that when you want to add capacity, you'll be buying multiple
[1412.80 → 1413.44] discs at a time.
[1413.44 → 1415.26] And this for me is the beauty of Merger FS.
[1415.78 → 1420.56] So we spoke to Antonio during the JB sprint, uh, Drew and Brent and I had a chance to sit
[1420.56 → 1422.34] down with him and ask him some questions.
[1423.02 → 1427.22] Um, I've worked quite closely with him on a few things like some of my blog posts, for
[1427.22 → 1431.36] example, like I've submitted them to him for review and made sure that it's all technically
[1431.36 → 1432.46] accurate and that kind of thing.
[1433.00 → 1438.18] But where Merger FS comes in and the magic of it really is you can have any number of mismatched
[1438.18 → 1440.26] drives, any file system.
[1440.64 → 1442.10] It could be a USB drive.
[1442.18 → 1443.24] It can be a SATA drive.
[1443.24 → 1444.94] It could be a CD-ROM drive.
[1445.06 → 1446.88] It could be an R clone mount point.
[1447.40 → 1452.60] And you can combine all of those different things under a single mount point.
[1452.82 → 1457.70] So I use slash mount slash storage as my pool mount point.
[1457.70 → 1463.76] And under there I have, uh, you know, 12 different discs combined and an R clone mount point and
[1463.76 → 1466.88] the ZFS stuff that I have on my system all in one place.
[1467.06 → 1469.14] And does Merger FS manage the parity as well?
[1469.24 → 1471.28] Does it keep things like if a disc fails?
[1471.28 → 1480.22] No, Merger FS is just a fuse layer user space file system that combines the all of those mount
[1480.22 → 1481.14] points underneath it.
[1481.14 → 1491.38] Um, if you want parity, which is the thing that lets you rebuild from drive failures, uh, I use snap raid for that for my media and then ZFS for the really important stuff.
[1491.84 → 1494.08] Um, we'll cover snap raid later, I think.
[1494.08 → 1506.24] But it's in short, it takes a snapshot, uh, of the state of the drives at a moment in time and calculates the, uh, parity data, uh, for those drives.
[1506.24 → 1517.68] Um, I think, uh, there's, you know, in terms of like the other options that you've got that do have similar functionality, unpaid will support multiple mismatched drive sizes as well.
[1518.10 → 1523.24] Um, the advantage of unpaid is it has real time parity calculation instead of snapshot.
[1524.00 → 1525.80] Downside is it's not open source.
[1526.26 → 1529.04] So, you know, and you have to put, you have to buy a license.
[1529.22 → 1532.10] So it depends on what floats your boat there.
[1532.10 → 1540.30] Um, open media vault will support merger FS and snap raid, uh, out the box, but you'll have to go through the GUI and configure it yourself.
[1540.70 → 1541.56] I like that for you.
[1541.64 → 1544.40] That's a downside for some people.
[1544.48 → 1545.90] It's like, Oh God, it's got a GUI.
[1545.96 → 1546.56] Thank goodness.
[1547.88 → 1548.24] Yeah.
[1548.44 → 1550.56] Well, I'm the sort of guy that puts everything in Ansible.
[1550.78 → 1550.94] Yeah.
[1551.28 → 1557.02] And if you just take the time to learn the configuration syntax, it will last with you forever.
[1557.02 → 1560.14] And it's, it is simpler and quicker and easier to back up.
[1560.14 → 1564.14] Somebody was asking me in the JB telegram the other day about how to configure Samba.
[1564.34 → 1566.38] And I just dropped them in my Samba config file.
[1566.46 → 1567.02] And I was like, there you go.
[1567.14 → 1567.34] Done.
[1567.54 → 1567.64] Yeah.
[1567.78 → 1570.56] You know, it's 30 lines worth of text, and it's done.
[1570.82 → 1570.94] Right.
[1571.38 → 1572.98] It's worth recapping for a moment.
[1573.14 → 1574.54] There's a lot to consider.
[1575.26 → 1581.48] How fast you need the disk to be, how much storage you need, what other kind of usage requirements you have.
[1581.66 → 1586.86] Then you have how much storage you plan to add to it, how much it will change and what your budget is.
[1586.86 → 1589.28] You have how critical the data is.
[1589.94 → 1593.78] Is it okay to put it on one disk?
[1594.36 → 1599.32] Maybe if you've got a perfect backup, but you need to consider what your options are if you need to go with a RAID.
[1599.44 → 1600.32] One is none, Chris.
[1600.52 → 1600.78] Right.
[1601.14 → 1601.90] One is none.
[1601.90 → 1609.82] And then you have other things to consider as well, like ZFS versus a different file system.
[1610.12 → 1612.66] If you have enough RAM, I mean, there's a lot to it, Alex.
[1612.76 → 1620.48] So how do you really get to any of these answers without being really intimately familiar with what your setup requirements are?
[1620.48 → 1625.76] Like for me, like I'm sitting here parsing this thinking, well, what should I do for my storage solution?
[1626.46 → 1628.76] Because I have all these weird use cases.
[1629.02 → 1632.62] One use case is camera recording, which is fairly high I.O.
[1632.84 → 1635.30] The other is notes.
[1635.42 → 1640.76] Like I have this huge spectrum of like super low I.O. and super intense I.O.
[1640.76 → 1642.64] I want everything redundant.
[1642.96 → 1646.02] And I don't have a lot of backup options either.
[1646.02 → 1649.58] So other than offsite, which I won't always have connectivity.
[1650.30 → 1653.44] And I also have that whole problem of a level four earthquake.
[1654.02 → 1654.54] Yeah.
[1654.98 → 1656.96] I'm a massive Mergers fanboy.
[1657.16 → 1663.66] I tried dozens and dozens of other things over the three or four years previous to settling on it in 2016.
[1664.20 → 1667.32] And I've just it's just been absolutely rock solid.
[1667.52 → 1667.80] Right.
[1667.86 → 1670.72] And I actually hate it when people use that phrase rock solid.
[1671.16 → 1672.84] But it's never missed a beat.
[1672.96 → 1675.76] I haven't ever had to go in and tweak it.
[1675.76 → 1682.76] There's not been any random-hidden files created like with MHDFS, for example, is another one I tried.
[1685.02 → 1686.34] It's just been flexible.
[1686.50 → 1686.64] Right.
[1686.68 → 1699.06] So any anything I've needed to bend it to do, I've been able to get Mergers to do it with no data loss, no having to copy files and have, you know, you know, you know, that slide puzzle you get where you've got to move the little cubes around.
[1699.06 → 1699.34] Yeah.
[1699.34 → 1699.90] Yeah.
[1699.90 → 1706.26] If you're migrating from one ZFS pool to another, you actually have to play that game with your data sometimes, right?
[1706.34 → 1712.58] Where you're trying to re-architect a VDE that you built knowing what you knew at the time when you built it.
[1712.64 → 1718.00] But it turns out three years later, oh, oops, that's not the most optimal way to do it.
[1718.24 → 1718.52] True.
[1718.52 → 1718.56] True.
[1718.68 → 1723.84] That is a bit of an issue I'm having now with the storage here at the studio.
[1724.02 → 1729.10] I feel like it's less of a problem in a more static environment where things don't change as much.
[1729.18 → 1735.08] Like, for example, ours is architected for these huge, huge, like storage requirements around production video.
[1735.58 → 1736.76] And we just don't have that anymore.
[1736.86 → 1739.76] And now I'm looking at it going, oh, man, I think I need to redo this.
[1740.10 → 1740.78] Flexibility, man.
[1740.94 → 1742.64] That's where Mergers really wins out.
[1742.64 → 1742.96] Yeah.
[1743.16 → 1744.58] I really don't want to have to deal with that.
[1744.82 → 1745.56] I really don't.
[1745.68 → 1752.60] But at the same time, I feel like if it's super important and critical, I'm still going to end up dealing with these limitations of ZFS, if you will.
[1752.84 → 1760.38] But the thing is, right, so Mergers, the reason it wins out so heavily for me is it supports any file system underneath it.
[1760.82 → 1771.08] So if you want to have ZFS on a pair of drives and then pool it with a bunch of other EXT4 drives or XFS drives, Mergers will just handle that absolutely fine.
[1771.08 → 1778.40] And then using the policies that Mergers has, you can say only write this data to a drive that already has that existing directory.
[1779.04 → 1788.66] So the way that I do it for all of my Docker app data, for example, does I tell it through the file system table, the FS tab, only create that directory on that drive.
[1788.78 → 1791.10] So it's existing path, most free space.
[1791.56 → 1795.32] But you're not allowed to create that directory on a drive where it doesn't already exist.
[1795.46 → 1798.38] The operation should just fail, and you'll alert me to that.
[1798.38 → 1802.68] So I'm not going to end up with files scattered around multiple different disks.
[1802.82 → 1806.46] But here's the other thing that really, really wins on Mergers for me.
[1806.90 → 1813.76] I can pull that drive from one system and I go and stick it into any other Linux box, and it will just be able to be read.
[1813.96 → 1814.94] It's just a disk with files.
[1815.08 → 1815.46] Yeah, right.
[1815.56 → 1820.24] Unlike a ZFS array, which I have to bring the whole pool over and then import it.
[1820.38 → 1822.62] And it now belongs to that operating system.
[1822.84 → 1825.88] And you have to hope that you've got the correct ZFS version and blah, blah, blah.
[1825.88 → 1828.84] You're kind of winning me over, especially for my home setup use case.
[1829.04 → 1831.88] It's just flexible, and it will support hot plug of USB devices.
[1832.80 → 1837.58] You know, this like whatever I come up with may not work out because it may be a bit of a roll of a die.
[1837.88 → 1840.52] I'm not even sure if I'm going to stick with Raspberry Pis long term.
[1840.62 → 1842.48] I mean, I really hope it works for my use case.
[1842.82 → 1844.32] It's very low commitment, right?
[1844.32 → 1851.42] And for those of you with commitment issues, you know, it's a really easy, really easy thing to get started with.
[1852.74 → 1857.98] Yeah, I think step one will be listening to your interview with the Mergers dev when that comes out on extras.
[1858.32 → 1864.42] And then step two would be for me to get you to send your config over so I can just read what that looks like.
[1864.52 → 1866.12] It's one line in your FS tab.
[1866.32 → 1868.10] I'll try and see if I can get it in the show notes.
[1868.20 → 1871.02] No, your Mergers, there must be a Mergers config file somewhere.
[1871.02 → 1876.02] Nope, it's in my FS tab. I'm literally Shying in now, and I'm going to put it to you on Telegram and send it to you.
[1876.02 → 1876.40] Oh my gosh.
[1876.72 → 1877.64] One line.
[1877.92 → 1878.98] I got to check this out.
[1879.16 → 1881.00] So do you think this would be ridiculous?
[1881.58 → 1892.30] Raspberry Pi 4 with two 2 terabyte SSDs hanging off of it on the USB 3 bus and then on the USB 2 bus a parity disk, like a 1 terabyte.
[1892.56 → 1894.94] Can I do that with Snap Rate? Can you have a separate parity disk?
[1895.10 → 1896.12] That's what you need to do, yeah.
[1896.64 → 1899.40] So, okay, we're going to get into Snap Rate now.
[1899.58 → 1900.56] Okay, you made me do it.
[1900.56 → 1903.44] Well, let's do a brief, because we should do a whole episode once I try it too.
[1903.62 → 1903.92] Yeah, yeah, yeah.
[1904.38 → 1909.26] So Snap Rate, the parity disk has to be as big or larger than your largest data disk.
[1909.56 → 1909.88] Okay.
[1910.74 → 1911.10] Okay.
[1911.56 → 1912.86] That's a lot of disks that we buy.
[1912.90 → 1913.60] That's the requirement.
[1915.50 → 1916.64] Okay, all right.
[1916.78 → 1920.20] But Snap Rate will support up to six parity drives if you are really paranoid.
[1920.20 → 1926.72] I think people should let me know, at Christmas, am I crazy to set up a Raspberry Pi storage server with disks running off the USB bus?
[1927.34 → 1929.64] Is there a SATA hat for the Raspberry Pi 4?
[1929.78 → 1931.66] Because I'd love to get a Raspberry Pi SATA hat.
[1931.66 → 1937.94] So I think, to me, at this point, you're pushing what the Pi is really suitable for.
[1938.02 → 1938.82] Damn it, I know.
[1939.30 → 1939.68] I know.
[1939.80 → 1944.24] I'm wondering if you shouldn't just build a $100 used x86 system.
[1944.24 → 1952.14] I built for my pfSense a little while ago an i5, I think, third gen system for $100.
[1953.86 → 1955.90] I mean, maybe for the storage, I could see it.
[1956.04 → 1962.28] I think if I did the storage over iSCSI, all the Pis are Ethernet gigabit wired in.
[1963.30 → 1965.20] And on the Pi 4, it's on its own bus now.
[1965.42 → 1967.42] And it seems fully capable.
[1968.32 → 1972.08] Here is the reason why I'm being resistant to the idea of going somewhere else.
[1972.08 → 1974.64] Because they're disposable at $25, $35.
[1975.28 → 1977.12] They're inside a seat.
[1977.68 → 1979.34] They're inside my dinette seat.
[1979.48 → 1981.04] And it gets hot in the summer in there.
[1981.56 → 1983.16] I mean, they might just burn up over time.
[1983.26 → 1989.84] But all I have to do is pull out the SD card, pop in the SD card into a new replacement Pi, and I'm out $35.
[1990.06 → 1993.58] If I have to replace them once every year or two, that's pretty reasonable.
[1994.06 → 1997.84] Plus, the way I've done it is I Velcroed them because they're so little.
[1998.18 → 2001.40] I Velcroed them to the wall of the seat inside.
[2001.40 → 2002.64] It's a wood.
[2003.22 → 2004.24] How would you explain this?
[2004.28 → 2006.16] It's a dinette seat, but people don't know what a dinette is.
[2006.20 → 2006.72] It's a booth.
[2006.90 → 2007.72] It's a booth.
[2007.90 → 2014.92] It's a booth seat with a hollow inside that you can take the cushion off and take the board off the top of the booth.
[2015.10 → 2016.50] And it's all empty inside.
[2016.50 → 2028.50] And praise be to Thor, this is where they decided to install my subwoofer for the sound system, which is on an inverter.
[2028.82 → 2037.60] And to power this one small subwoofer, they ran an entire AC outlet into the inside of this booth seat.
[2037.92 → 2042.54] So there is an AC plug on the inverter that runs off of my house batteries.
[2042.54 → 2043.76] Wait, wait, wait, wait, wait, wait.
[2044.26 → 2046.42] Doesn't the Pi run on DC power?
[2046.94 → 2047.28] Yes.
[2047.60 → 2049.18] That's for a future episode, Alex.
[2049.36 → 2049.66] Okay.
[2051.24 → 2053.68] Once I go solar, I've got to get everything on DC.
[2053.90 → 2054.14] Okay.
[2054.46 → 2061.04] But right now I just have, I have a surplus, well not a surplus, but I have 200 amp hour lithium-ion batteries.
[2061.04 → 2067.06] So I can get about 12 to 18 hours of using the RV off battery power.
[2067.06 → 2070.34] I wonder how long you could run just a Pi 4 off that battery for.
[2070.90 → 2071.66] Years probably.
[2071.88 → 2078.46] Very, very long time because a 3,800 William battery supposedly will run it for like 16 hours.
[2079.76 → 2081.94] So there's a plug inside this booth seat.
[2082.20 → 2085.78] And I have every, so I have installed all of my equipment inside this booth seat.
[2086.12 → 2088.32] I have my switch Velcroed to the wall of it.
[2088.60 → 2094.62] My router, all three Raspberry Pis, the discs that are attached to them, their USB hubs.
[2094.62 → 2097.70] Everything's Velcroed in really nice and secure and snug.
[2098.44 → 2099.52] But don't call it Velcro.
[2099.62 → 2100.20] It's loop and hook.
[2100.96 → 2102.46] And so I'd hate to go away from that.
[2102.84 → 2102.96] Yeah.
[2103.46 → 2107.24] You know, you have a unique set of requirements.
[2108.24 → 2112.86] I don't think most people need to drive their data down the road every week.
[2113.04 → 2114.54] But, you know, if you do.
[2114.54 → 2116.08] I think you'd be surprised.
[2116.24 → 2120.26] Digital nomads are a bigger and bigger, bigger work demo.
[2120.70 → 2126.34] People who, because really what I'm doing is I'm trying to build a system for anybody who needs to work and travel at the same time.
[2126.50 → 2130.44] Mine's going to be at a larger scale, but the concepts are applicable to anybody who works and travels.
[2131.12 → 2140.34] And so I am trying to solve these in a way that is low power, works off of maybe solar, and is as best as possible noiseless.
[2141.66 → 2142.24] I don't know.
[2142.28 → 2143.04] You might be right, though.
[2143.50 → 2145.96] I'd like to hear what the audience thinks I should do for my storage setup.
[2145.96 → 2148.32] Yeah, you can use the hashtag Ask SSH.
[2148.52 → 2153.48] Now, speaking of the hashtag, Matty McGraw wrote in through JB Telegram,
[2154.10 → 2158.68] For data security, I want to do mirroring of my data DIES directories.
[2159.20 → 2161.04] Is ZFS the best choice?
[2161.20 → 2163.48] I don't have tons of RAM.
[2164.06 → 2171.16] You know, I recently did some testing that shows that if you have even like 16 gigs of RAM, you'll probably be all right with certain storage mounts and reason.
[2171.26 → 2173.52] It really kind of scales to how much storage you have with CFS.
[2173.52 → 2181.24] I think in the old days, the recommendation that I certainly recall, and maybe we should hit Alan up for an up-to-date recommendation, was one gig per terabyte.
[2181.40 → 2183.14] I don't know if that still holds true now or what.
[2183.38 → 2184.86] Is, I think, is the old recommendation.
[2185.10 → 2193.02] But I think the other question that is embedded within the question is, if you want data integrity, do you have to go with CFS?
[2193.08 → 2197.60] Let's say it's like pictures of the family, and, you know, they're just irreplaceable.
[2198.28 → 2200.52] Does that, can you, is your only option using CFS?
[2200.52 → 2200.84] ZFS?
[2201.56 → 2202.12] I don't know.
[2202.16 → 2204.00] I think after our conversation today, it might not be.
[2204.36 → 2206.72] Let's take the merger FS snap raid situation, right?
[2207.36 → 2208.62] Snap raid does checksum.
[2208.80 → 2217.88] So every time it calculates parity, it is checking the integrity of those files at the file level, not the block level, which is where ZFS wins out.
[2217.88 → 2233.12] But what's interesting is that you can do a snap raid scrub, which has much the same kind of connotations as a ZFS scrub, which, again, just checks the, you know, the checksums and makes sure that the file integrity is there.
[2233.12 → 2241.42] You do get things like compression with CFS, you get encryption, and obviously you get a bit rot protection, which is one of their favourite things.
[2241.48 → 2243.24] But really, that just means it's checking the data.
[2243.96 → 2249.66] And you get other things that are more advanced that can be really great for backup, like ZFS send and receive.
[2250.16 → 2250.98] And data sets.
[2251.18 → 2252.86] I'm falling in love with data sets.
[2253.10 → 2253.24] Yeah.
[2253.24 → 2261.90] However, if this is not – if everything – is the words we just used do not excite you, it may not be the file system for you.
[2262.02 → 2263.36] That could just be the measure you use.
[2263.36 → 2272.44] And I am such a big believer in using systems that you are comfortable administering and keeping up to date and secure if you choose to self-host.
[2272.84 → 2277.06] This is why I took Free NAS off of our storage server here at the studio.
[2277.56 → 2278.82] Free NAS is a great product.
[2280.14 → 2282.88] I am not the right type of user for Free NAS.
[2283.24 → 2292.78] When I have a problem with my system, my troubleshooting technique is to get a command line and look at the logs, look at the output of the system, and start troubleshooting and start fixing.
[2293.40 → 2294.66] That breaks Free NAS.
[2294.74 → 2296.34] You need to use Free NAS through the GUI.
[2296.70 → 2297.82] It's not my use case.
[2297.96 → 2301.22] I also – I'm not as familiar with FreeBSD as I am with Linux.
[2301.42 → 2309.86] And if it's my super valuable data, I want it to be on a system that I know how – like Alex said, I know how to rip the hard drive out, put it in another system, and get to that data.
[2310.06 → 2311.44] I got to know how to do that.
[2311.44 → 2317.94] And what ended up happening is once we flipped that thing over to Linux, I used it 100 times more.
[2318.24 → 2320.36] We've now got so many applications on there.
[2320.44 → 2321.58] We've got backups.
[2322.16 → 2327.34] We've got – we've taken care of things like getting properly signed SSL certificates.
[2327.86 → 2332.42] Like it just went – it went much further than I was expecting once I switched to a system I was comfortable with.
[2333.00 → 2334.82] So, Matty, that's my number one advice.
[2334.82 → 2340.38] I know you've got some experience with Linux, so I would recommend maybe not doing Free NAS.
[2340.54 → 2343.74] I would also recommend maybe looking at something like Snap Raid.
[2343.90 → 2350.38] You don't need Mergers to use Snap Raid if you just want the snapshooting and backup capabilities of Snap Raid.
[2350.68 → 2352.66] And then look into getting that data off-site.
[2353.24 → 2357.10] So, this is an important thing to focus on, which you're looking at right now.
[2357.10 → 2360.48] But like we mentioned earlier in the show, one is none.
[2361.42 → 2362.66] And two is not enough, really.
[2363.16 → 2364.44] No, no, it really isn't.
[2364.84 → 2373.80] But the other thing to consider, right, let's say that he went really simple and used something like sync just to copy data from one place to another, one server to another, one directory to another.
[2373.88 → 2374.96] It doesn't really matter.
[2375.06 → 2375.86] sync doesn't care.
[2375.86 → 2382.28] What you've got to think about is, let's say that you have some kind of, what's that?
[2382.34 → 2384.34] Is it crypto malware or something?
[2384.86 → 2385.54] Oh, yeah.
[2385.64 → 2386.34] Showing what you mean, yeah.
[2386.60 → 2387.64] Crypto ransomware.
[2387.74 → 2388.26] Ransomware.
[2388.34 → 2388.70] Thank you.
[2388.88 → 2389.58] Thank you, Brain.
[2390.12 → 2399.94] So, let's say you have some ransomware situation, right, where the files on your source of truth, your main system, get encrypted, and you don't know how to encrypt them.
[2399.94 → 2401.52] Or you delete something.
[2401.92 → 2404.40] Or you just generally screw up, right?
[2404.40 → 2420.58] If you have a script which is automatically overwriting data at the other end every time, like sync would, you're also going to sync the encrypted copy potentially over the top of your quote unquote backup.
[2421.04 → 2424.64] Or a damaged file or deleted files potentially, depending on how you have it set up.
[2424.94 → 2426.44] There are a lot of ways that it could break.
[2426.44 → 2431.04] So, this is one of the things where ZFS send would come into play because you'd have data sets to play with.
[2431.04 → 2435.30] And you could just roll back to the old data set before the ransomware happened.
[2435.86 → 2438.32] But is that a common problem?
[2438.64 → 2442.16] I mean, the deletion thing is probably quite common for people.
[2442.34 → 2448.08] But there are tools like snapshot that will do similar sorts of things on a non-ZFS system.
[2448.66 → 2450.30] There are a lot of options, to be honest.
[2450.70 → 2454.28] Alex and I both like to use Duplicate as a way to back up some of our server stuff.
[2454.62 → 2454.84] Yes.
[2454.88 → 2456.10] How did I forget Duplicate?
[2456.10 → 2458.20] Yeah, I use that every day, and it just works.
[2458.66 → 2461.24] But it suffers from the same situation, right?
[2461.28 → 2467.42] If my source of truth here gets encrypted, or I delete something, it's going to also delete it on the other end.
[2467.42 → 2474.34] The nice thing about applications like Duplicate, another one that's super great for local backups is Backup PC.
[2474.54 → 2479.00] Been using it, I think, since like 2008, 2005.
[2479.32 → 2479.78] I love it.
[2480.36 → 2484.92] Backup PC and Duplicate will support revisions, which is really nice.
[2484.92 → 2486.34] So you can revert.
[2487.22 → 2490.18] You can also have it configured not to do that.
[2490.44 → 2492.20] So that's why it's important to go through it.
[2492.62 → 2496.46] When you decide to self-host, this is going to be like my soapbox for like the first 10 episodes.
[2496.70 → 2499.92] When you decide to self-host, you're taking on a little additional responsibility.
[2500.36 → 2501.40] You've got to check these things.
[2501.44 → 2502.18] Do I have revisions?
[2502.72 → 2503.40] And stuff like that.
[2503.74 → 2504.26] But here's the thing.
[2504.42 → 2506.08] When it breaks, it's on you.
[2506.72 → 2510.54] Not some massive data breach like Equifax or something like that, right?
[2510.54 → 2512.66] Like it's your fault.
[2512.92 → 2515.88] And I actually kind of appreciate the honesty of that.
[2516.32 → 2521.68] There's also the reality that you're not nearly the target that Equifax is or Amazon, right?
[2522.22 → 2526.46] You're almost in some ways enjoying the obscurity, I would say.
[2527.08 → 2531.56] And I kind of like it to be on me because it is my stuff.
[2531.88 → 2536.24] This is just the digital version of my stuff, just like the security of my home is on me.
[2537.00 → 2538.48] So I prefer it that way.
[2538.50 → 2542.54] I'd rather not outsource the security of my house or my RV or the studio.
[2542.90 → 2548.56] So, yeah, I think it's a little more stress, but it's also very gratifying.
[2549.06 → 2555.50] Like when my setup that I'm – when this stuff I'm doing in the RV works, like with Home Assistant, it genuinely gives me joy.
[2555.82 → 2557.04] Like it just gives me so much joy.
[2557.04 → 2561.76] And I feel like I have – I know I've done a good job, like with the wire running for the cameras.
[2561.86 → 2562.70] I'm proud of that.
[2563.48 → 2567.70] Where I mounted things, how I've done the – the pies are mounted and run the wires for that.
[2567.74 → 2568.40] I'm proud of that.
[2568.44 → 2570.14] Like I've put craftsmanship into it.
[2570.14 → 2576.84] It's given me an opportunity at the end of the day to come home and work on something for an hour or two that gives me genuine satisfaction.
[2577.18 → 2580.14] And it also improves our digital well-being.
[2580.68 → 2581.34] So there you are, Matty.
[2581.34 → 2587.02] I'm sure we've just completely made that even more complicated for you by giving you 15 more different options.
[2588.18 → 2592.84] You see, why wouldn't everyone want to hashtag Ask SSH and get their question on the show?
[2592.84 → 2593.12] Exactly.
[2593.50 → 2596.46] So you can get more of the show at self-hosted.show.
[2596.96 → 2598.66] I'm on Twitter at Ironic Badger.
[2599.04 → 2600.32] I'm at Chris LAS.
[2600.42 → 2602.28] The network is at Jupiter Signal.
[2602.68 → 2609.46] And don't forget extras, extras. Show with our Merger FS interview coming up, probably already out by the time you're hearing this episode.
[2609.46 → 2614.64] And also a plug for another brunch that was excellent recently was the Alan Jude brunch with Brent.
[2614.92 → 2619.54] So, you know, we talk – he talks more about, you know, ZFS, of course, because it's Alan.
[2619.84 → 2620.22] Yes.
[2620.42 → 2622.06] And his free BSD stuff.
[2622.16 → 2625.46] And, yeah, that'd probably be a fun episode for people that are into self-hosting.
[2625.56 → 2626.38] Great, great point.
[2626.46 → 2628.00] Yeah, check out Brunch with Brent and Alan.
[2628.08 → 2628.62] That was a good one.
[2628.98 → 2632.66] And then one final JB plug is Tech Snap. Systems.
[2632.82 → 2633.20] Yes.
[2633.56 → 2638.08] Talk about getting simple explanations of how these complicated ZFS things work.
[2638.08 → 2641.06] Jim Salter is a master at explaining ZFS.
[2641.50 → 2642.22] He's perfect.
[2642.74 → 2647.68] And particularly Tech Snap 4.14 is all about ZFS.
[2648.06 → 2649.96] And I really enjoyed the snapshot discussion.
[2650.46 → 2653.82] And 4.15 is going to be about benchmarking, which should be fascinating.
[2654.32 → 2654.54] Absolutely.
[2655.02 → 2657.24] So thanks, everybody, for listening.
[2657.54 → 2660.38] That was self-hosted. Show slash five.
[2660.38 → 2661.96] So, what a lack of matters.
[2662.10 → 2662.16] And I'll play it.
[2676.62 → 2678.82] Welcome to initiatory ZFS.
[2678.96 → 2679.72] I'll play it.
[2679.76 → 2680.42] It's an is household.
[2680.56 → 2681.04] I'll play it.
[2681.08 → 2681.94] It's so joyful.
[2682.02 → 2682.50] And I'll play it.
[2682.54 → 2682.94] And I'll play it.
[2682.98 → 2683.88] If you want to play, I'll play it.
[2683.92 → 2684.56] Let's see if you can.
[2684.56 → 2684.88] I'll play it.
[2684.88 → 2685.20] I'll play it.
[2685.62 → 2685.64] I'll play it.
[2685.72 → 2686.98] I'll play it.
[2686.98 → 2687.40] I'll live.
