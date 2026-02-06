[0.00 → 5.52] Joining us on the show today from serverbuilds.net is JDM. He's my go-to hardware guru.
[6.16 → 11.48] We also cover the new Raspberry Pi release and I stage an intervention for Chris's Raspberry Pi
[11.48 → 19.58] habit. I'm Alex. I'm Chris and this is Self-Hosted 21. Alex has you ever had the perfect system
[19.58 → 23.66] end up being the machine you built yourself? There's no such thing as the perfect system
[23.66 → 29.84] is there it's just between upgrades. I don't know I kind of think the workstation I have upstairs
[29.84 → 37.38] is one of those kind of perfect builds where I had kind of the confluence of the core series of CPUs
[37.38 → 42.78] were at good maturity. Six cores was a good bang for the buck. It was a good price to get 32 gigs of
[42.78 → 48.34] RAM. Fast storage was cheap enough that I can have multiple disks. I just love this box I built.
[48.34 → 56.50] I feel that way about this one I'm talking to you via it's an i7 8700k with a couple of NVMe storage
[56.50 → 62.48] drives and all my actual storage is in the basement, but you know I've got an SSD for Windows and an SSD
[62.48 → 67.56] for Linux for pass-through and stuff like that. It does everything I could ever dream of it just
[67.56 → 73.38] it's just a champ. What's yours? Mine's my Linux box upstairs that I run Manjaro on with my three
[73.38 → 81.68] 27-inch screens. It's got an AMD 580 graphics card in it. Intel 6 core CPU. 64 gigs of RAM in this thing
[81.68 → 85.72] because I like to run lots of VMs and I have multiple disks. I have a dedicated disk for my home
[85.72 → 92.10] a dedicated disk for my root and a dedicated disk for my VMs and a dedicated disk for my Steam games
[92.10 → 97.96] and also my sync folders. That's the way to go man. It's pretty great. Now it's fun when you're
[97.96 → 104.38] building a desktop, but it like really matters when you're building a server and that's why it's really
[104.38 → 109.62] great that we are joined by a very special guest today who helps the community figure these things out
[109.62 → 116.26] with his website serverbuilds.net. JDM welcome to the show. Hey guys thanks for having me. Man thanks
[116.26 → 120.90] for being here and for those that are not familiar with serverbuilds.net can you give them like the
[120.90 → 126.10] elevator pitch on what the website is? Well our website's a little stale at the moment but the
[126.10 → 131.28] forums are really where it's happening and uh that's where the action is. Yeah, the forums and uh the
[131.28 → 138.30] discord so we got almost uh probably what I would say 10k users like including Reddit discord
[138.30 → 146.06] but it's a very community focused um well for lack of a better word community so we uh I try to
[146.06 → 151.98] engage as much as possible, but anyone can write a guide and post it on the forum and then if it's
[151.98 → 156.96] good enough like we'll help you edit it and it can become featured, but mostly I write guides on
[156.96 → 164.56] hardware getting used or enterprise off-lease hardware um sometimes it's not even sometimes used
[164.56 → 171.22] it's brand new it's just old stock um, but it's all very affordable and I basically just try to make
[171.22 → 176.00] it is easy if you're like used to building gaming pcs and whatnot, and you want to build a server
[176.00 → 181.96] um it's just as easy as that. Yeah, but you do help kind of um give people an area to focus in and some
[181.96 → 185.64] of these guides are pretty useful because I think Alex you've used one of them in the past to build
[185.64 → 191.86] your setup. I certainly have so yes hi JDM welcome to the show. Thanks. I built when I emigrated a brand
[191.86 → 199.04] new server and uh I built your anniversary uh I think it was 1.0 build at that point which has a
[199.04 → 211.96] pair of dual LGA 2011 Eons 128 gigabytes of RAM 100 plus terabytes in the Rosewall LSV 4500 I think
[211.96 → 219.16] case and uh that was all about a couple of thousand dollars um, so I mean the bang for buck that you and
[219.16 → 224.90] your site enabled me to get was just astonishing really that power you know five years ago would
[224.90 → 232.62] have cost three four five times what it cost me uh a year ago. The CPUs that you have if you
[232.62 → 237.48] look at the retail price of them they could be in the two thousand to three thousand dollars each uh back
[237.48 → 244.66] when they were brand new, but now you can get them on eBay for maybe a couple of hundred bucks 150 dollars.
[244.66 → 250.48] I think the magic sauce really that you have there are a few tools that you kind of share
[250.48 → 255.94] with the community there's a absolutely awesome spreadsheet the CPU compendium spreadsheet that you
[255.94 → 265.58] have which lists every single Leon in that era and compares the price to performance to TDP to you
[265.58 → 269.10] know everything that you're trying to think about when you're building one of these servers so
[269.10 → 276.64] stuff like idle power draw is obviously quite important for a 24 7 home based box but then you
[276.64 → 281.76] know Plex transcoding performance might be important for some people, or you know there's just a whole
[281.76 → 286.02] bunch of stuff that's in there that's just really great and um one of the things you actually helped
[286.02 → 290.70] me with I don't know if you remember this about six to eight months ago was uh I was having some
[290.70 → 297.74] temperature issues in my build, and I was posting on the forums, or I think it was discord actually with you
[297.74 → 303.20] all the pictures and things like that, and it turned out that the fan configuration I had in my box I
[303.20 → 308.68] just didn't even look I just bought Noctua uh just because that's what I've always done and then you
[308.68 → 316.14] told me no Alex you need high static pressure fans because of xyz I was already to buy a new case at
[316.14 → 321.12] this point you know um and I changed the fan configuration based on your advice, and you saved me
[321.12 → 327.20] probably another few hundred dollars, so thanks for that oh absolutely and uh we try to
[327.20 → 333.06] do a full service recommendation where um if you're in that situation, and you're like okay I've
[333.06 → 338.82] got the hardware, but I don't have these little tiny details fleshed out um I try to do my best to pay
[338.82 → 344.14] attention to that and say like okay well uh if you're in a server chassis, and you do need those high
[344.14 → 351.92] static pressure fans um here's not only the ones you should buy but here's those uh those fans compared
[351.92 → 356.74] to what else is on the market and here's why they're a better value you can get like you know for the
[356.74 → 360.98] ones that you got they were I don't know five packs for 28 bucks or something like that yeah they
[360.98 → 366.26] weren't even they weren't really even very expensive so right, and sometimes it's just about buying the
[366.26 → 371.40] correct hardware, and it doesn't always have to be the most expensive and especially for servers I mean
[371.40 → 377.80] why did you go that route uh like I know you came across it and all that but what was so attractive
[377.80 → 383.32] to you about that versus going for something more modern I like the idea I had dual tanking on board
[383.32 → 389.54] as well as uh PMI and dual Leon is obviously quite attractive from a Plex transcoding perspective
[389.54 → 394.50] my use case was I wanted to be able to run a couple of Kubernetes clusters at once in addition
[394.50 → 400.36] to my normal server workloads that is I needed to be able to have at least 96 gigs of ram, but I went
[400.36 → 407.98] for 128 in the end because I'm a baller and why not that board actually tops out at like 512 or 768
[407.98 → 414.18] yeah it's kind of insane what you can get, and it just blew my mind I mean I kind of because I was
[414.18 → 418.84] emigrating I didn't really have a lot of time to you know dig into the minutiae like you and
[418.84 → 424.22] your team obviously do, and it was just really helpful to have all that information in one place
[424.22 → 427.76] and be able to say right if I buy this board I'm going to expect roughly this performance
[427.76 → 432.68] it's going to all work together, and you're actually lining up vendors as well so I bought from
[432.68 → 438.76] I think the IT mart at that point we've been trying our best to work with a lot of these vendors that
[438.76 → 446.08] do um either off-lease uh servers or they just um they're like resellers or refurbishers and there's a
[446.08 → 454.60] ton one bay, but they're all very professional in the business of uh reselling server hardware, and you can
[454.60 → 460.48] get some fascinating stuff that the public just doesn't even know about for example like you
[460.48 → 468.22] said there's a vendor that we do group buys with and um he had a few 6.4 terabyte NVMe drives
[468.22 → 475.78] they went for I think 600 a piece on group buy and if you think about that for a second consumer
[475.78 → 482.96] NVMe drives your two terabyte brand new is maybe 270 bucks so if you're getting 6.4 terabytes for 600
[482.96 → 490.20] and then the best part is that it has a 60 petabyte right uh endurance so that drive's never going to die
[490.20 → 496.18] oh could you ping me next time that comes up right absolutely I mean it's that's the kind of thing
[496.18 → 500.76] that you would see in the discord and that I mean maybe that was a little bit of a rare deal but
[500.76 → 506.66] um stuff like that does come up we try to establish that relationship because these vendors they don't
[506.66 → 511.94] know that there are communities out there for that they're just selling to um businesses and things like
[511.94 → 517.22] that where if I can establish the link between the vendors and this large community that's still
[517.22 → 523.26] growing I mean it's growing at a fantastic rate that helps everyone I think what you do so nicely
[523.26 → 528.94] is you bridge the gap between googling I want to build my own server and actually having a functional
[528.94 → 533.84] list of parts that all work together which is just really nice at different price points as well and
[533.84 → 539.16] different performance points so we've talked about the anniversary build that's kind of like the uh
[539.16 → 544.46] no compromises build almost there's another one that you guys do called the NAS killer tell us about
[544.46 → 550.08] that one the home NAS is something that's becoming very, very popular you can run a bunch of applications
[550.08 → 554.48] on it, you throw a bunch of hard drives in, and you've got local storage that you can serve to your
[554.48 → 560.42] network, and it's nice to have because you don't have to rely on the cloud you can have it local it's
[560.42 → 569.72] fast and overall it's a great idea however companies like Synology or QNAP or um you know WD they have
[569.72 → 574.76] their own little NAS devices, but really they end up being very expensive for the hardware you get
[574.76 → 584.04] and so the NAS killer was my vision of how you can build a NAS for the same price or cheaper and have
[584.04 → 593.22] the hardware be much more powerful, so I found some uh early e3 eons and uh you know the pass mark was
[593.22 → 600.56] like 7 000 compared to uh even the high end Synology is only like 1900 pass mark so you're getting four
[600.56 → 608.20] times the performance uh you can build it yourself, and then you have anywhere from 8 to 15 to 30 drive
[608.20 → 614.00] bays just depending on what your setup's like but really the NAS killer series has evolved and currently
[614.00 → 619.46] we're on NAS killer 4 NAS killer 5 is in the works um the hardware is getting newer and newer as
[619.46 → 626.74] time passes and stuff starts to go again like off lease so you start to see the hardware even
[626.74 → 631.42] though it's a little bit older starts to come through and prices start to drop a little bit more
[631.42 → 638.74] but uh yeah the NAS killer is our most popular guide and I think there's like 30 000 views or something
[638.74 → 645.02] just on the forum post alone but yeah it's just designed to be the all-in-one home NAS you can run
[645.02 → 649.38] any software you want, but it's designed to give you that starting point that could
[649.38 → 652.98] make me want to build one of those, but I can't figure out how to fit it in the RV I could make
[652.98 → 660.10] that work for sure do you have any advice for anyone who's looking to build a low power box that's
[660.10 → 668.24] going to be on 24 7, so I mean something that could form the basis of a self-hosted router for example
[668.24 → 673.70] you know running open sense or of sense something like that what's fascinating about computer
[673.70 → 679.92] hardware especially I would say within the past five to seven years performance hasn't increased
[679.92 → 686.74] a lot so like IPC instructions per clock yes it's improving but really where the improvements
[686.74 → 695.30] have come about is through power usage if you look at the modern 1151 sockets from intel for example
[695.30 → 702.26] intel's eighth and ninth gen CPUs they're extremely power efficient for example the hp290
[702.26 → 708.40] uh it's an it's a little like all-in-one consumer grade device, but it idles at like seven watts and
[708.40 → 717.00] there's a there's a 54 watt TDP seller on it and that's the TDP not the power usage but at idle it's
[717.00 → 721.88] only about seven watts I used one for my of sense and I think that box was only a hundred dollars
[721.88 → 729.18] honey base shipped, but we just look for like little deals like that and um it is really just depends on
[729.18 → 735.12] what your needs are but like you said for of sense it's not going to be super high of sense or for
[735.12 → 739.94] home assistant or something like that there's just going to be always on you know if you don't want
[739.94 → 745.28] to build a huge box like I did and run them all as VMS with pass through and stuff like that
[745.28 → 753.62] it's a perfect idea to consider one of these smaller lower power x86 based systems because you know
[753.62 → 759.56] legacy software is going to support it um and one of the issues with using the Raspberry Pi uh for
[759.56 → 765.64] all of this type of stuff is that you have to hang everything off the USB bus number one and then
[765.64 → 772.46] number two um every arm CPU is different, so there's no guarantee that just because a vendor says they
[772.46 → 776.94] support arm through you know a docker container or something like that there's no guarantee it's
[776.94 → 783.26] actually going to run on your setup, so I mean that could be proved by the recent Raspberry Pi 4
[783.26 → 788.24] and if you look at the software support for that compared to the three and any model below it's
[788.24 → 793.88] totally different the pi 4 went through some more significant changes with the video that are for the
[793.88 → 799.10] better uh and a couple of other areas with the bootloader which has caused that lag but the two to
[799.10 → 804.64] three series and there were lots of iterations in between there was pretty successful I look at it
[804.64 → 812.14] like this Alex it's early days still with the platform and like any early adoption there's a series of
[812.14 → 820.90] trade-offs but also benefits like for example the USB bus it is a limitation of the Raspberry Pi
[820.90 → 828.38] platform, but there are several small board computer platforms that now either have eMMC in addition to
[828.38 → 835.08] PCI or SATA even and then of course with the Raspberry Pi 4 a guy like yourself you really could do all the
[835.08 → 841.00] storage over the gigabit Ethernet which is now on its own dedicated connection um you know you could issue
[841.00 → 845.66] everything really I might have bought a Raspberry Pi this week I think you should try using the
[845.66 → 850.14] network as your primary storage location I think that'd be an interesting experiment it's in England
[850.14 → 857.48] so I bought one of those brand-new eight gigabyte Raspberry Pi 4s to use as a remote ZFS storage
[857.48 → 862.54] endpoint I was going to ask if you got the eight gig one yeah I did I mean i I really don't need eight
[862.54 → 868.96] gigs on a pi but why not have the headroom for future tasks yeah um because that means in the
[868.96 → 874.54] future you could also throw something on their like sync thing you have plenty of overhead for all
[874.54 → 878.80] kinds of additional applications that are just a container away I mean it's not necessarily a bad
[878.80 → 884.76] idea and i would also just say in my hands-on experience with say the pine 64 rock pro 64
[884.76 → 891.80] and the pi 4 I could run everything in every container on either I didn't I didn't run any
[891.80 → 897.38] particular compatibilities the OS kind of abstracts that aspect once you have the core OS
[897.38 → 904.52] as long as it's a mainstream Linux like an arch base or Debian base you're pretty much good yeah
[904.52 → 911.06] because you were talking about Raspberry Pi OS for a little bit on up 357 and how they've I mean
[911.06 → 916.34] they've just renamed Raspbian to Raspberry Pi OS um and talking a little bit about why you don't
[917.12 → 922.50] really rate it versus say an Ubuntu well that's a good question because I think the for me, and it's
[922.50 → 927.80] something maybe I haven't made implicitly clear on this show is the transition for treating the
[927.80 → 932.28] Raspberry Pi a little more seriously came when canonical announced that they were going to make
[932.28 → 939.12] it is a first class Linux platform for them like it's actually got staff that are working to support future
[939.12 → 944.78] raspberry pies and that that resonated with me pretty strongly because the Raspberry Pi models tend
[944.78 → 951.26] to stick around for at least five years you know you can still buy older pies and Ubuntu LTS is a
[951.26 → 956.52] professional grade operating system it might not be everyone's favourite, but it's a professional
[956.52 → 962.98] operating system that is designed to run in production environments Raspbian to me or I'm sorry
[962.98 → 968.64] Raspberry Pi OS their art is formerly known as Raspbian I think is great and I think it's really well
[968.64 → 972.98] suited for new users of the platform and I think it's really well suited for people who want a
[972.98 → 978.80] lightweight desktop with a web browser but for those of us that want to use it as a home server or
[978.80 → 984.10] like a backup server even like in your case Alex which is a great use case I think you need something
[984.10 → 989.90] on there that is a little more production grade and just to the point of uh low power consumption
[989.90 → 997.10] just keep in mind that with low power consumption generally comes low performance as well uh and it
[997.10 → 1003.14] may be relatively higher performance compared to another model but if you compare to for example a low
[1003.14 → 1008.96] power consumption Leon that has eight core 16 threads Raspberry Pi is never going to touch it
[1008.96 → 1017.48] even though maybe the power consumption's let's say uh 50 watts at idle on the Leon yes it's its more
[1017.48 → 1023.98] power for sure but how much more compute horsepower do you have here's a fascinating consideration
[1023.98 → 1033.30] though so my sister is not a techie in fact she works in um pharmaceuticals and when the pi 4 8 gig came out
[1033.30 → 1041.86] this weekend I ordered one and sent it to her, she put it together plugged in the USB hard drive in half an hour
[1041.86 → 1050.42] over a Skype call I can't imagine asking her to put together a remote Leon system for me, I know that
[1050.42 → 1057.64] building computers is just like adult Lego but I've been doing it since I was 13 she's never even
[1057.64 → 1061.64] so much as I mean when her mac breaks she goes to the Apple Store and takes it there you know
[1061.64 → 1067.98] it's someone else's problem yeah so the pi for me at least fulfills a really great need of being
[1067.98 → 1075.18] like a computer in a box that I can still mostly own every piece of like I can choose the case I can
[1075.18 → 1081.14] choose the bootloader and that kind of thing uh without having to install a CPU or a power supply
[1081.14 → 1088.34] or something like that I totally agree and uh I think that it absolutely has a purpose uh and I'm
[1088.34 → 1094.02] not against a pi or anything like that, but you do have to consider that it's still not x86 so if
[1094.02 → 1098.84] there are applications that you want to run there uh you do run into that hard limitation I think that's
[1098.84 → 1103.86] very fair you have to go into it with the acknowledgement that there's just not the level of software
[1103.86 → 1108.48] compatibility to both the point you guys have both made and I have to agree with, and you are
[1108.48 → 1114.74] probably not going to get quite the right bang for your buck I wonder though because I run three right
[1114.74 → 1120.72] now is what I have remaining uh raspberry pies that are currently running and being even when even with
[1120.72 → 1127.76] the overhead of being inverted from DC power um I think all three of them are maybe drawing 30 watts
[1127.76 → 1132.38] I'm not sure because it's mixed in with my router my switch and a Wi-Fi access point in there
[1132.38 → 1139.38] but the draw is so substantially low that I can, you know I can run them for days off the battery
[1139.38 → 1145.14] power that's pretty great yeah so Chris you uh your server seat I think that's what we're going to dub it
[1145.14 → 1152.88] now JDM had potentially some ideas for what we could do to maybe replace I don't know if we can replace
[1152.88 → 1158.74] the pi obviously uh you love yours but yeah maybe we could do something a bit different I'm open to the
[1158.74 → 1163.84] idea i have to be honest I think the Raspberry Pi would be a good like one year experiment right now
[1163.84 → 1171.32] but i I really wish at the end of the day all of this was virtualized that everything was in a VM
[1171.32 → 1180.10] so I'm trying to stage a pi intervention here JDM help me out so what has built-in KVM a battery backup
[1180.10 → 1188.90] and is x86 and low power do you know a ghost I was going to say it sounds like a super nook
[1188.90 → 1199.54] it's a laptop oh very fair yeah okay all right so I have actually found great success using even low-end
[1199.54 → 1207.68] consumer refurbished laptops for situations like yours because a lot of times they have NVMe slots
[1207.68 → 1213.70] so you can have one or two NVMe slots even on like let's say a 300 laptop, and maybe it has like
[1213.70 → 1221.70] an intel penny in gold uh I believe the model is like the uh g5405 or something like that it's a
[1221.70 → 1226.22] two core four thread it's got intel quick sync so if you want to do Plex transcoding you can do
[1226.22 → 1233.96] 15 transcodes easily it's got an x86 CPU so you can run Linux you can run windows you can run
[1233.96 → 1241.26] basically anything you want um you can do 16 32 gig of ram, and it's got Ethernet Wi-Fi
[1241.26 → 1246.76] again built-in battery backup you can leave the lid closed tuck it away somewhere on a shelf
[1246.76 → 1253.92] that screams to me laptop you know I didn't uh didn't expect this uh line uh i have to say that's
[1253.92 → 1260.28] pretty did you have a specific laptop in mind um the ones that come one bay that I've been eyeing and
[1260.28 → 1266.94] I've used personally like right now at my home I have a LTE network that's completely separate it's
[1266.94 → 1272.96] an i kind of jokingly call it a plan it's an it's a physical land it's its not a VLAN it's its
[1272.96 → 1281.56] totally separate uh but right now I'm running that off of uh router OS on an uh Lenovo I have to look at
[1281.56 → 1285.94] the exact model number maybe you can put it in the show notes but uh it's just a Lenovo like I said it's
[1285.94 → 1293.32] got the Pentium gold, and then it runs um an USB LTE connection and that is just for my smart home
[1293.32 → 1298.76] devices so it's totally separate from my regular uh LAN, but you could do something similar
[1298.76 → 1305.24] where uh if you want to run docker and containerize everything on the laptop um you could do that yeah
[1305.24 → 1310.70] I was thinking the ThinkPad yeah that's that and the other advantage is if I have to go into crash
[1310.70 → 1317.06] mode it has a built-in screen and keyboard absolutely and that has saved uh saved my
[1317.06 → 1322.20] butt quite a few times and especially in your situation leave the lid closed leave it plugged
[1322.20 → 1328.02] in, and then you can actually run it off of an ups or whatever battery you have, and then you also have
[1328.02 → 1333.46] the laptop's internal battery, so the possibilities are endless, and you obviously don't have to go that
[1333.46 → 1337.66] route you could go for a UK those are a little bit more expensive for the performance you get
[1337.66 → 1344.06] actually um, but again you don't have the screen, and you know KVM and all that right I mean it's hard
[1344.06 → 1348.22] to argue with a use ThinkPad because honestly it's still going to be more powerful than the raspberry
[1348.22 → 1353.94] pi and what I'm using these pies for is going to work great on a laptop if it's just a headless
[1353.94 → 1362.34] Linux with KVM um home assistant of course Plex obviously sync things a big deal for me, I have a very
[1362.34 → 1368.36] simple markdown viewer application that I like to use those things will be no problem the one that's
[1368.36 → 1373.90] tricky and I don't know exactly what to do with is Shinobi because that's a lot of disk Io it's a lot
[1373.90 → 1379.58] of network Io and Shinobi is one of those applications that just wants to have the entire OS which either
[1379.58 → 1383.68] means I got to virtualize it or I got to put it on dedicated hardware could you give me a quick
[1383.68 → 1391.56] rundown of Shinobi and what the yeah it's basically just a closed circuit um self-hosted capture system
[1391.56 → 1397.40] for RTS camera feeds so I have a bunch of wise cameras that have a firmware on them that just lets
[1397.40 → 1402.50] me capture the video off them directly over the network and this thing provides recording of those
[1402.50 → 1408.06] videos and playback and viewing kind of like a DVR system, and you can pull up all the feeds and look
[1408.06 → 1413.58] at them in a dashboard and cut out clips and segments, and it's great because sometimes I take my RV
[1413.58 → 1418.16] in wild places and I want to have surveillance when I'm not there or like right now it's in a shop and
[1418.16 → 1423.68] I want to check in on what's going on sometimes I found that it is basically keeps the box
[1423.68 → 1431.30] totally busy the entire time I don't want to run two laptops well okay that's fair um have been you
[1431.30 → 1438.60] aware of what quick sync is yeah like intel's built-in improved uh h.264 encoding accelerator correct and
[1438.60 → 1445.14] it's its seen a huge generational improvement so um this is something that's been very popular on
[1445.14 → 1451.96] serverbuilds.net we've been recommending quick sync transcoding boxes for Plex um a seventh gen Cameron
[1451.96 → 1462.02] two core can do 20 transcodes from 1080p to 1080p or 720p um without a sweat did you just say 20 20
[1462.02 → 1470.68] wow okay so that's a scale I just did not appreciate that's including laptop CPUs the
[1470.68 → 1476.12] the biggest performance increase that we've seen with quick sync and through my testing has been
[1476.12 → 1482.18] generational so you go from seventh gen to eighth gen to ninth gen intel, and currently we're on 10th gen
[1482.18 → 1489.02] you can get a 10th gen intel quick sync laptop for about 300 bucks off eBay, but it really doesn't really
[1489.02 → 1497.26] matter what the processor is it's more about again the generation there's some indication that faster
[1497.26 → 1505.22] processors are faster and do support more transcodes but even the very baseline models support a ton and
[1505.22 → 1511.24] you were talking about Shinobi I'm not sure if that can leverage quick sync it might be able to but I know
[1511.24 → 1516.86] that its competitor blue iris which is a Windows-based application can absolutely leverage quick sync and they
[1516.86 → 1525.10] just had a recent update where it almost completely removes the CPU usage entirely I actually use
[1525.10 → 1533.84] quick sync for twitch streaming and recording so I have an i9 9900k in my desktop but if I were to use
[1533.84 → 1540.04] nine which is NVIDIA's encoding on the GPU I would lose a little bit of performance and there is some
[1540.04 → 1546.44] indication that it does mess with your frame times a little bit whereas if I use the GPU which you do
[1546.44 → 1553.06] have to enable manually uh in your bios but um that GPU is not doing anything there are no monitors
[1553.06 → 1559.92] plugged into it or anything it's just sitting there idle so using it to encode like a twitch stream for
[1559.92 → 1568.86] example or a YouTube video it works fantastically the quality is amazing uh it sees about 0.6 CPU usage
[1568.86 → 1575.34] while it's doing it wow that's pretty great hardware circuitry huh yeah that is really great and the
[1575.34 → 1581.48] other thing that's tricky for me along with this is heat because it is in this seat um my it's tricky
[1581.48 → 1586.98] for to keep my ambient temperature below 80 degrees Fahrenheit I wouldn't worry about it too much with
[1586.98 → 1593.42] the laptop um they can handle it and uh like I said quick sync is very power efficient it doesn't
[1593.42 → 1599.68] really require too much of a CPU resource so for example if you were to run that original setup like
[1599.68 → 1606.66] we were talking about um you could run docker on Linux on the laptop and then if you were to run
[1606.66 → 1611.70] Plex on it, and you say okay well I want Plex to leverage that CPU transcoding you can actually pass
[1611.70 → 1620.42] just the GPU through to Plex uh through the Plex container and leverage it that way but if you were
[1620.42 → 1627.36] to do a separate uh NVR build like you said with Shinobi or um I would prefer blue iris because I know it
[1627.36 → 1632.04] can leverage quick sync very well uh I would recommend a separate box, and maybe I just keep a
[1632.04 → 1636.30] pie doing that and then move everything else the laptop idea is a good one I'm trying to ride the
[1636.30 → 1641.26] raspberry pies out for a year just as like a self-education program and I know that a lot of people out
[1641.26 → 1646.10] there in the community are trying to use pies so i just I want to be well versed in them and i
[1646.10 → 1652.64] definitely am now I'm definitely deep um I'm like I'm like dribbles with uh with the raspberry pies
[1652.64 → 1657.76] in the RV these days but i I could see this probably I don't know I'd have to go look back
[1657.76 → 1662.84] when we started this see where my year mark is I could see switching to this is how it goes
[1662.84 → 1668.76] with JDM Chris he has these little nuggets of ideas that kind of sprinkle into your brain you go away
[1668.76 → 1672.64] for a couple of weeks, and you're like damn it that's what I need to do I need to buy an old think
[1672.64 → 1679.58] pad now well you know what's funny is for like a hot half a second I think I glanced at an old
[1679.58 → 1684.60] laptop in the studio and I looked at that and I went huh I wonder if that'd work as a server and
[1684.60 → 1689.66] I thought nah I'm not a laptop especially if you could power it directly off DC if you got the
[1689.66 → 1695.88] voltage right absolutely you can that they're most mostly 19 volt DC yeah I bet I could make it work
[1695.88 → 1701.54] the other thing that I want you to think about and I don't know this is for me personally this is
[1701.54 → 1707.28] the way I work but uh you said that you're using pies because you like to play, and you like to learn
[1707.28 → 1713.28] and that's something you're trying to learn um for me, I don't like to play with things that I just want
[1713.28 → 1718.94] to play and work yeah there is that yeah so if you can get your baseline setup where you've got your
[1718.94 → 1725.80] router virtualized and all of your services that you need to work on like let's say the laptop
[1725.80 → 1731.28] setup we're talking about or something else then you would actually have more freedom to play with the
[1731.28 → 1739.26] pies where uh you don't necessarily have that back of your head saying oh well if I mess this up
[1739.26 → 1746.04] then I need to redo everything yeah there's there are advantages to like I don't want to be too critical
[1746.04 → 1751.36] of the pies because I'm impressed that the advantage to me diving into this and really using
[1751.36 → 1757.62] them is I truly am learning what they're capable of and not and I have to say they really have run
[1757.62 → 1761.92] pretty solidly the biggest mistake I made early on was I used Raspbian and I had to rebuild a couple
[1761.92 → 1769.10] of things but now I'm quite happy in fact I having my storage on the USB bus hasn't really been an
[1769.10 → 1774.52] issue because I'm getting these Samsung t5 discs they transfer it like 280 megabytes a second which
[1774.52 → 1780.48] is as good as my Wi-Fi is going to do for the Plex playback so even the disc i o I've been fairly happy
[1780.48 → 1784.80] with and then I'm going to also add in there because of the cost what I'm doing now on this trip I'm
[1784.80 → 1792.66] taking is I've brought a cold pie ready to go in a case all set up and um I have them installed in
[1792.66 → 1797.70] Velcro to the inner walls of the seat so if one of these pies dies I just grab the cold standby
[1797.70 → 1803.52] literally just pull the one Velcroed in pop the new one in it has Velcro on it already cook some
[1803.52 → 1808.22] all put all the same connections in and power it up it's good to go oh, but cold pie is not as tasty
[1808.22 → 1815.22] it's true but I do feel like I am constantly walking on eggshells I will acknowledge that
[1815.22 → 1820.54] aspect of it, but that could also just be because it's such a new platform to me right but i I think
[1820.54 → 1827.90] that you would gain a lot more experience where um you can sort of piecemeal implement things that
[1827.90 → 1833.02] you're testing with the pie if you have a good backbone yeah I could be riskier if it wasn't my
[1833.02 → 1837.62] production device and that's the same reason I ended up splitting out my of sense I mean I used to run
[1837.62 → 1843.78] it on top of promo with a quad intel gigabit nick card in the main hypervisor in that anniversary
[1843.78 → 1851.68] build I ended up building a separate of sense box I've since switched it to open sense but I ended up
[1851.68 → 1856.96] building a separate box because I didn't want my internet to go down every time I rebooted my server
[1856.96 → 1865.66] right the uptime now is 115 days or something but when it happens or what was happening to me with
[1865.66 → 1872.34] promo was I was getting um hard lockups you know kernel panics basically um and so every time
[1872.34 → 1876.68] that happened I had to walk down to the basement and push the button because PMI wasn't working or
[1876.68 → 1883.00] something it was completely weird and uh I just ended up thinking right my internet needs to be separate
[1883.00 → 1888.66] from my server that's just something that needs to happen part of uh building a home lab is identifying
[1888.66 → 1895.28] those key points of this needs to not fail what do I need to do to make it perfectly reliable
[1895.28 → 1901.44] and then on the other hand uh what kind of hardware do I want to play with where I have that freedom
[1901.44 → 1907.26] and the flexibility yeah a home lab and this is a bugbear of uhm organ actually he was on the show a
[1907.26 → 1911.64] couple of episodes ago he and I were talking the other day, and he was like a home lab is not just
[1911.64 → 1917.50] someone's server like a home lab is an actual thing with you know multiple switches and multiple servers
[1917.50 → 1922.22] and whatever so you know the purists out there will be probably cringing a little bit at my
[1922.22 → 1927.52] definition of a home lab as one box but hey home labs can be virtual too they don't have to be just
[1927.52 → 1933.26] physical it's true that is true um so I have a question for you JDM about you know your setup and
[1933.26 → 1939.26] you know how many terabytes you have and what does your home lab look like being a hardware guy I'm
[1939.26 → 1946.42] expecting some good stuff here yeah uh it's been an interesting process because uh we just recently
[1946.42 → 1953.78] moved to Denver um and that was a cross-country move for us but as some of you may know I do stream
[1953.78 → 1960.90] occasionally on twitch and um in the past couple streams I've been implementing a coordinator so uh
[1960.90 → 1970.14] that was kindly given to us by a fellow um server builds member who works at back blaze um and uh I spent a
[1970.14 → 1976.32] little bit of time implementing that and I've got 30 drives of uh mixed 8 and 10 terabytes running
[1976.32 → 1981.58] unpaid on that box I have to wipe the pool of drool from underneath my chin right now a coordinator
[1981.58 → 1987.84] oh that's the stuff of dreams i just recently posted about it on Twitter and uh it was nice to have
[1987.84 → 1995.24] unpaid retweet me but um it's its been an interesting challenge to get that to work um in the past I've run
[1995.24 → 2002.62] pretty much all super micro servers uh a couple three use the 16 bays and then a 45 bay was which is a
[2002.62 → 2011.16] direct attached storage it's just basically a bod juncture just a bunch of disks and um that connects to the
[2011.16 → 2017.08] main server so uh in the past I've run that and I've condensed down a little bit into the coordinator where I can
[2017.08 → 2024.52] have 45 bays in for you so are you running unpaid on that yes I run unpaid mostly and uh
[2024.52 → 2031.26] shout out to you guys for having the best docker containers I run uh exclusively LSI when possible
[2031.26 → 2036.82] oh we'll have to change that because I'm, i'm not part of them anymore are you officially not part of
[2036.82 → 2043.20] them I'm officially not no oh okay well I use them too and I still think they're great thanks for any
[2043.20 → 2050.10] work that you did do on them because uh they've been pretty great um but aside from that uh yeah I do
[2050.10 → 2055.04] run unpaid and of course you know Plex and all that that's kind of where I got started was the
[2055.04 → 2060.18] Plex Subreddit and I was a mod there and helped out the team there for a while I started doing a
[2060.18 → 2065.46] couple of hardware builds and split off into server builds.net because we just really took over
[2065.46 → 2071.14] the Plex Subreddit uh and I didn't really want to continue to do that so right it's fascinating
[2071.14 → 2076.02] because it's a theory I think we even we probably said on the show a couple of times but Alex and I talk
[2076.02 → 2084.54] about it off-air all the time that a lot of this journey starts at Plex and sometimes our audience
[2084.54 → 2088.70] kind of hates to hear that because we got a know we got a pretty hardcore open source aficionados
[2088.70 → 2094.48] out there and they prefer we talk about other things but I think you really got to give Plex
[2094.48 → 2099.18] credit it draws a lot of people into this space, and it's its kind of like the toe in the water
[2099.18 → 2104.20] that leads to bigger and bigger things so JDM I'm curious now that you've kind of got a fairly
[2104.20 → 2111.06] sophisticated setup what do you find to be the most frustrating or troubling aspect of the setup
[2111.06 → 2117.72] like what's the thing that you have to constantly deal with or manually fix luckily not much because i
[2117.72 → 2125.88] choose my hardware in a way that I don't need to do anything with it once it's implemented and now
[2125.88 → 2131.48] I'm more geared at helping other people find hardware or I can start playing around with software
[2131.48 → 2137.18] because uh you know everyone has their specialties I love hardware I love working with hardware
[2137.18 → 2142.16] but software is definitely one of my weaker points so if I can start to gain experience with that
[2142.16 → 2147.84] because I have that solid hardware base where I have the freedom to do whatever I want basically
[2147.84 → 2154.10] yeah that is my goal really is just to start moving into more software developing my own experience
[2154.10 → 2160.06] with that and relaying those experiences to other people uh because everyone has their own way of
[2160.06 → 2167.32] doing things and uh not to say my way is any better than anyone else's but we both uh you know you guys
[2167.32 → 2173.08] and server builds we have our own communities and I'm sure that you know there's a crossover there but
[2173.08 → 2178.32] we do have our own ways of doing things and um if there's more information out there on how to do
[2178.32 → 2184.32] something or if there's a gap in knowledge I'd like to try to fill that you know but as far as
[2184.32 → 2191.40] challenges go I don't really have a lot um right now it's kind of uh getting everything to
[2191.40 → 2200.16] where it is what I would say uh like peak efficiency so I'm trying to cut down power usage where I can
[2200.16 → 2206.46] if it's downgrading a processor or moving to a different system dialling it in a sense that's great
[2206.46 → 2210.92] that's a great I love that phase and uh unfortunately i kind of live by the motto it's
[2210.92 → 2216.40] like oh I have a spare part it's not really a spare part it's not it's an unfinished build now so now i
[2216.40 → 2222.86] have to do something with it that could get expensive real fast oh absolutely so back when
[2222.86 → 2227.46] we had Wendell on the show I asked him how many terabytes he had and I had this vision of like a
[2227.46 → 2233.28] top gear style leaderboard for guests as to how many terabytes they have oh sweet yeah I don't know
[2233.28 → 2239.10] if I've asked every guest but I'm going to ask you how many terabytes do you have raw or formatted
[2239.10 → 2244.74] oh you know I don't think we've ever clarified I guess I mean I think we should consider
[2244.74 → 2254.14] raw potential versus available yes because Wendell just dropped the petabyte bomb so I mean I don't
[2254.14 → 2259.14] think we're going to compete with that but maybe I'm not quite there uh I do have multiple
[2259.14 → 2263.48] unread setups so I do have the one in the store Nader I have one that's in a 15 bay and I have
[2263.48 → 2270.16] another one that's I'm prepping for another 15 bay but I'm nearing half a petabyte wow okay that's
[2270.16 → 2274.34] pretty cool where do you buy your drives from and what sort of things do you look for when you're
[2274.34 → 2283.74] buying hard drives I exclusively buy WD shuck ables and me too exclusively they're fantastic because
[2283.74 → 2291.24] they're really just host helium drives for the most part um with a little bit of uh firmware trickery but
[2291.24 → 2297.54] there's really not a lot to consider buy eight terabyte WDS or higher so eights tens twelves
[2297.54 → 2303.54] fourteens soon to be coming out sixteens and uh they're the best value for the money and uh
[2303.54 → 2310.30] nothing can touch them right now that's a great tip Alex is a shocking fan, and it's uh his favourite
[2310.30 → 2315.06] thing so I don't think you could have had a more perfect answer for this show yep yep i
[2315.06 → 2320.60] love if there are a couple different models there's like the elements there's the um easy stores
[2320.60 → 2325.76] which are best buy exclusive, but it doesn't matter they're all the same drives inside um the only
[2325.76 → 2330.20] thing that you have to consider just like SAS hard drives if anyone's familiar with SAS hard drives
[2330.20 → 2337.10] they have a 3.3 volt standby there's a guide on our forum on how to surpass this issue a lot of
[2337.10 → 2342.10] people use capped on tape to uh just tape off the pins, but you can just simply remove this the
[2342.10 → 2348.16] correct state of wire, and it'll function just cut the wire yeah cut the green one I don't know if
[2348.16 → 2352.88] it's green please don't cut the green wire check which one you're cutting if you're using like a
[2352.88 → 2357.74] server backplate like a super micro they already have the 3.3 volt standby like taken care of so you
[2357.74 → 2361.90] don't even need to worry about it um but yeah they're they're extremely versatile they're they're even
[2361.90 → 2367.34] great in their own USB 3.0 enclosure for those Raspberry Pi guys that we won't talk about
[2367.34 → 2374.52] all right well JDM thank you very much for joining us it's been a real pleasure to talk to you is there
[2374.52 → 2379.90] any way you'd like to send folks um yeah you can check out serverbuilds.net uh like I said in the
[2379.90 → 2385.02] intro the uh website's a little stale right now really everything's happening on the forums uh which
[2385.02 → 2390.00] is forums.serverbuilds.net, and you're on Twitter aren't you I'm on Twitter I don't really do a whole
[2390.00 → 2397.80] lot on there um apart from give me grief about my TV stand that's true uh at JDM underscore what
[2397.80 → 2403.50] with three a's you can also just hit me on discord everyone bothers me on discord uh I think we've got
[2403.50 → 2408.08] about 8 000 members in our server so it's its growing, and it's pretty large we'll put a link
[2408.08 → 2413.60] to the discord and the forums in the show notes and I think it's a great companion discord to our own
[2413.60 → 2418.86] those are two discords in a pod is that yeah was that a thing can we make that a thing
[2418.86 → 2424.56] oh absolutely i I think we should do like a partnered uh discord something and maybe just
[2424.56 → 2429.24] cross-link or something like that I love it, and you've given me a lot to think about I think the
[2429.24 → 2434.22] laptop is a serious route that I'm going to consider when the pi experiment ends, and now it's just a
[2434.22 → 2440.68] matter of how soon does the grand experiment end and can I find the right ThinkPad one bay I'm kind of
[2440.68 → 2445.66] hoping I can stretch it out long enough to get a great deal on a 10th gen to really take advantage of
[2445.66 → 2450.52] quick sync think about it this way you don't need a ThinkPad because that is their sort of mid to
[2450.52 → 2456.32] upper tier laptop right you just need the hardware the screen doesn't matter keyboard doesn't matter
[2456.32 → 2462.82] mouse doesn't matter it's really just what CPU does it have does it have the name slots that I need or
[2462.82 → 2467.58] hard drive slots uh how much ram can it support and that's about it is makes a good point Chris
[2467.58 → 2472.68] wise words JD, and maybe we'll have you back when i uh when I do make the switch oh awesome I would
[2472.68 → 2478.24] look forward to it and just one other thing there is uh one guide that I do want you to check out
[2478.24 → 2484.98] Chris I wrote it about a year ago it's called uh how to create a mobile media server with Plex's new
[2484.98 → 2493.40] app for windows so it's right now it's a windows' thing only um, but it would be somewhat interesting
[2493.40 → 2498.28] to you particularly because what you can do is uh just to give a TLDR
[2498.28 → 2506.36] you can use Plex's new app download media from any shared server onto the app uh like you're
[2506.36 → 2512.34] syncing it locally and then also run Plex media server on that computer and then share that media
[2512.34 → 2518.76] out oh sure it's really easy, and it's got a nice like UI it's not an intended use for the app
[2518.76 → 2524.12] but it does work so check that one out I just found it I will thank very much JD and for joining
[2524.12 → 2528.90] us thanks guys for having me I hope I could I mean I know we talked about a lot of different things but
[2528.90 → 2533.24] the rabbit hole goes way deeper we'll have to chat more well I look forward to chatting on discord but
[2533.24 → 2536.72] I look forward to having you back on the show too of course thanks for having me guys appreciate it
[2536.72 → 2554.80] av Japan um
