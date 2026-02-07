[0.00 --> 7.16]  Welcome in to episode 135 of the self-hosted program and I want to start right off the top
[7.16 --> 11.78]  of the show by living vicariously through Alex if we could because Apple has been teasing us
[11.78 --> 16.04]  this week with some hot new product releases and a little birdie tells me you might have nabbed one.
[16.56 --> 21.14]  I was thinking about it yeah those new Mac minis or should we call them Mac nanos they look they
[21.14 --> 26.84]  look pretty nice huh? You know me I've always kind of thought a Mac mini headless running a
[26.84 --> 31.96]  Linux could be a really nice low power home server yes and this new one's even smaller.
[32.98 --> 39.66]  It's got Thunderbolt 5 which is the real kicker for me so that that port has 120 gigabits of
[39.66 --> 43.96]  throughput. Yeah so you could attach some real storage. Some proper storage on the Thunderbolt
[43.96 --> 49.64]  interface and you know you can get Thunderbolt docs now okay they're not cheap by some standards but
[49.64 --> 55.40]  neither is building a full-on server so yeah you know you get the Mac mini as the brains and then
[55.40 --> 60.50]  you can upgrade that over time and then the Thunderbolt storage enclosure just remains for
[60.50 --> 67.06]  a decade. I think it still comes down to like what is the premium you put on power consumption
[67.06 --> 74.30]  because you could probably for less money get more memory and storage in like a x86 box but it
[74.30 --> 80.36]  wouldn't necessarily be tiny silent and sip power so it's kind of like how do you prioritize those things
[80.36 --> 85.06]  and are you thinking about maybe a use case where power would be kind of like one of the top
[85.06 --> 90.54]  requirements you have to watch for? Well I'm thinking about my UK backup server here it would make a
[90.54 --> 96.60]  fantastic I mean I'm presupposing all of this based on it running Asahi Linux in some future version like
[96.60 --> 104.32]  I don't want to run macOS as a server no thank you I am presupposing this will run Linux and right now
[104.32 --> 109.04]  at least the Mac mini and we don't have numbers on the new one but you know take this as a ballpark
[109.04 --> 117.16]  idles at about seven watts which is just bonkers good for the for the processing power available
[117.16 --> 122.72]  you know when you're putting a machine in at a family member's house or a friend's you know it's
[122.72 --> 127.16]  something to consider do you want to put something in there's going to be drawing 300 watts all the time
[127.16 --> 133.32]  right and you know that adds up for them it's it's like running a small space heater all the time
[133.32 --> 137.60]  right and something something that's the site you know by the time you've got an external hard drive
[137.60 --> 145.02]  or two and the Mac mini you know it's it's the size of a few cd cases you know it's it's really
[145.02 --> 151.16]  small and it can fit under almost any relative's tv or friend's tv or something if if you ask nicely
[151.16 --> 156.36]  enough yeah I think I haven't heard a lot about thunderbolt 5 support but I think intel's been pretty good
[156.36 --> 161.44]  I wonder if anybody out there if you boosted and tell us if you you have any experience with
[161.44 --> 166.44]  thunderbolt 5 on linux because you'd have to watch for that too but you know this is like Alex is
[166.44 --> 171.14]  saying this is not something you do right now but you wait for the Asahi project to maybe even get
[171.14 --> 177.34]  one of these rigs try it out and you know by the time they have that maybe there's another arm system
[177.34 --> 184.76]  out there like system 76 announced an arm thaleo desktop that's a much bigger rig still a lot less
[184.76 --> 192.40]  power than say an equivalent amd system or intel system but maybe it starts there if we start getting
[192.40 --> 198.08]  more of these arm boxes that run linux then you start getting more drivers developed and the
[198.08 --> 204.54]  situation starts to improve pretty quickly yeah I mean you can run utm virtual machines and lima
[204.54 --> 208.98]  virtual machines and the performance through rosetta on mac os is it's pretty good to be honest even
[208.98 --> 217.68]  with x86 emulation which is crazy but you know there's nothing that there's nothing that feels
[217.68 --> 224.62]  quite the same as running a linux kernel bare metal on that box is there that's for sure you know what's
[224.62 --> 231.64]  funny too is some things just push you to just go further and further like we often talk about how
[231.64 --> 238.90]  plex or jellyfin is kind of a gateway to a home lab setup or you know a solar system running off battery
[238.90 --> 242.94]  is often the gateway to trying to figure out how to get the most performance out of low power
[242.94 --> 250.92]  I feel like I had one of those moments recently where to make one thing work well I ended up redoing
[250.92 --> 257.82]  a whole bunch of stuff there's a phrase for that in the industry you know what is it yak shaving
[257.82 --> 264.22]  yeah you know you got to do it the right way well you know I'm gonna go and make myself a cup of tea
[264.22 --> 268.52]  but in order to do that I need to grow the tea leaves yeah but in order to do that I need to get
[268.52 --> 273.04]  gather the soil and then I need some manure so I'm gonna go and find my friend who's who by the way
[273.04 --> 277.10]  needs his yak shaving in return you know what I'm saying like before you know it you're shaving a
[277.10 --> 282.16]  yak yeah well if you got your self-hosted bingo card get ready to cross this off because I'm gonna
[282.16 --> 289.26]  mention ersatz tv again and it's really ersatz tv that got me to just sort of like flip the table
[289.26 --> 295.20]  on so many things you know because I for a long time I've been very happy with the apple tv
[295.20 --> 301.80]  infused a jellyfin setup but when I wanted to integrate live tv streaming channels which is
[301.80 --> 307.28]  one of my favorite things I've done in my home media setup well I you know I started looking for
[307.28 --> 314.42]  clients that worked on tvOS that did good streaming and I could find individual like IPTV apps and stuff
[314.42 --> 317.88]  like that but nothing that really integrated with the whole jellyfin experience and what I was finding
[317.88 --> 323.34]  is if the family had to bail from jellyfin they would not go back into jellyfin etc etc I inevitably ended
[323.34 --> 327.66]  up on the android tv platform again because I have a couple of nvidia shields like we've talked about
[327.66 --> 335.32]  only I kept running into issues where about once a day the wi-fi would just drop off and there's even
[335.32 --> 340.44]  in like the quick settings menu on these boxes there's a there's a button right there to restart the wi-fi
[340.44 --> 346.42]  probably a bad sign and so I thought to myself I wonder if there's a way I could automate this
[346.42 --> 351.70]  and it was just and it's like these series of can I fix this can I fix this so here I am a few minutes
[351.70 --> 357.66]  later installing adb bridge integration into home assistant then yeah I'm looking up I'm looking up
[357.66 --> 365.30]  the actions or whatever they call it now to use adb to restart android tv and then before you know it
[365.30 --> 371.58]  I'm just kind of like loading up more and more kind of automations for android tv so it auto reboots them
[371.58 --> 378.04]  uh it wakes them up at a certain time it shuts them down with our with our bedtime scripts now
[378.04 --> 384.00]  so there's been a lot of like little improvements that I've done that have kind of increased my
[384.00 --> 388.08]  dependency on android tv I guess you could say but when you use the adb bridge with home assistant
[388.08 --> 394.16]  it really smooths some of that stuff over but then you can also install things like the home
[394.16 --> 399.04]  assistant fire remote card and I have a link to this in the show notes uh Alex you should take a look
[399.04 --> 405.26]  at this thing because what it does is it replicates several different popular remotes obviously the
[405.26 --> 411.82]  fire remotes but also apple tv all the various nvidia shield remotes look at that and so you can have
[411.82 --> 419.16]  a dashboard on home assistant that is a virtual remote and it's so handy because if you lose the
[419.16 --> 424.96]  remote you can just pull this up but it also lets you create virtual buttons on the remote so I have
[424.96 --> 430.72]  buttons one press to launch jellyfin one press to launch the ip tv camera app that's tuned into the
[430.72 --> 435.94]  front dash camera so we can see the driveway one button to launch the wife approval factor on that
[435.94 --> 443.28]  must be they don't have to learn right entire second interfaces just press the button yep and because
[443.28 --> 448.32]  it's on home assistant that means if she's in the kitchen and the kids are being loud or the tv's up too
[448.32 --> 453.08]  loud she has access to the volume control she can pause it from the kitchen she doesn't have to go find
[453.08 --> 456.70]  the remote like if one of the kids has the remote she doesn't have to go track it down she can also
[456.70 --> 463.60]  pull it up on her phone it's so great and it's it's a really well done little home assistant I got it
[463.60 --> 468.92]  through I think I probably installed it through hacks so all of this was I was really feeling pretty happy
[468.92 --> 478.56]  with my setup but the real cherry on top of all this was jellyfin 10.10.0 came out since last episode
[478.56 --> 484.08]  and they introduced the groundwork for something that looked like it was on the outs they figured
[484.08 --> 490.16]  it out and I'm so thrilled to be able to say that they have introduced what they call segment skipping
[490.16 --> 497.48]  now they introduced this idea of media segments inside a file and they install they store information
[497.48 --> 504.12]  about certain time spans in a particular video that clients can then access it's like in the database and
[504.12 --> 510.18]  they can call that and so there could be a media segment type called intro there could be a media
[510.18 --> 514.16]  segment type called credits you know you could have all kinds of segments whatever you want to label
[514.16 --> 521.24]  them as long as you have a scanner that can recognize them and so in 10.10 jellyfin now has just the
[521.24 --> 526.76]  general structural support for these media segments now you still need a plug in that does the scanning
[526.76 --> 533.92]  and identifies them but this is the groundwork Alex for truly at the core level intro skipping support
[533.92 --> 539.72]  that clients can use as an API call I think that's probably a much more sensible way to architect it
[539.72 --> 547.30]  too because that way different plugins can come along over the next 5 10 20 years whatever as media
[547.30 --> 552.72]  formats change as tastes change you know whatever is required as long as you've got that framework
[552.72 --> 558.82]  there for those plugins to hook into the plugins can do whatever they like yeah I mean if I was if I
[558.82 --> 564.74]  was sponsor block you know the YouTube plugin for Firefox or whatever I would I'd be looking at
[564.74 --> 569.94]  making a jellyfin plugin right now oh my gosh pinch flat that you mentioned in the last episode
[569.94 --> 577.54]  yeah I've been using the heck out of that yes that's all been part of it have that plug into this you
[577.54 --> 583.50]  know somehow exactly perfect yeah yeah so trick play is also a feature they've been working on recently
[583.50 --> 592.04]  and in 10 10 it got a major overhaul up to a 100x improvement depending on your hardware configuration
[592.04 --> 594.46]  and if you're not what's trick play
[594.46 --> 601.86]  so trick play is a way the jellyfin can scan and find interesting segments so when you're like you're
[601.86 --> 607.64]  doing a fast scrub through the video it can show you frames in a in a like a really optimized smart way
[607.64 --> 612.86]  that doesn't bog down the client and it can generate that stuff ahead of time so it's available for the
[612.86 --> 618.82]  client in it like a stream it's really cool oh I see so that makes your scrubbing experience feel
[618.82 --> 623.36]  buttery yeah yeah yeah okay nice and then they also made major enhancements I mean there's a lot
[623.36 --> 627.72]  Alex but I'm just giving you the top three then they also made major enhancements to uh their
[627.72 --> 636.46]  transcoding and playback support they I saw that ffm mapping of HDR 10 now yeah yeah ffmpeg 7 which is
[636.46 --> 643.02]  nice to see there are some breaking changes network paths and in your library no more no no no no more
[643.02 --> 648.54]  so I was definitely that guy for a while where I had like a samba path or something like that I think
[648.54 --> 654.68]  that's out now also how would you get around that with let's say docker you could probably mount the
[654.68 --> 659.48]  samba share on the host itself and then present that path as a volume to the container instead yeah
[659.48 --> 663.06]  that'd probably be the way to go a little more clunky perhaps I wonder why they've done that one
[663.06 --> 667.88]  did they say yeah I I didn't dig into it I wouldn't be surprised if it's just old code
[667.88 --> 674.56]  yeah probably time to go you know also which I'm surprised they didn't do this before and I have
[674.56 --> 682.62]  experienced the consequences of this ffmpeg is just absolutely vital vital to how jellyfin runs and now
[682.62 --> 687.38]  jellyfin will refuse to start if ffmpeg can't be found or it's the incorrect version or something
[687.38 --> 694.68]  is wrong like a missing dependency and what can happen with jellyfin is it can kind of be an
[694.68 --> 700.06]  insidious failure that you don't even realize is taking place because jellyfin could be functional
[700.06 --> 704.36]  enough for your standard decodes to happen so you don't really notice it in your day-to-day tv
[704.36 --> 710.22]  watching or movie watching but if you go to try to manually run one of the back-end tasks like
[710.22 --> 716.56]  generate trick play images or you know scan for intros or you know whatever all normalization of audio
[716.56 --> 721.68]  whatever you might have scheduled tasks for if you went to manually run them and you know scanning
[721.68 --> 726.30]  these files is a big job maybe you just added a whole new tv show and you go to scan the files and
[726.30 --> 732.86]  it happens instantly it takes a second and it says job done that typically was a communications failure
[732.86 --> 737.60]  or an ffmpeg failure and the jellyfin client just oh everything's fine and didn't really have any
[737.60 --> 743.62]  intelligence or smarts to tell the user that the task actually failed because ffmpeg finished so jellyfin
[743.62 --> 749.32]  thought it was done and and no work was actually ever accomplished and so now jellyfin will flag
[749.32 --> 752.72]  you and say hey your ffmpeg installation is broken you got to fix this before i'm going to work
[752.72 --> 759.04]  correctly just seems like necessary kind of stuff i've also really appreciated the faster release cadence
[759.04 --> 764.08]  they've had with these releases the next jellyfin release is going to come out as early as april 2025
[764.08 --> 770.18]  so we're getting these new features and i feel like the jellyfin project this last year or two is
[770.18 --> 778.26]  really just maturing at a really nice click yeah and the clients as well i know i mentioned infuse
[778.26 --> 782.02]  that's not one of their direct clients but their jellyfin support has been really solid but uh
[782.02 --> 786.34]  swift fin and the actual jellyfin apps themselves have gotten really good this year it's
[786.34 --> 791.66]  you know i think we switched at the right time i'm feeling you know maybe some people think we were
[791.66 --> 798.72]  late we did i feel like it was yeah i i never i'm not really missing anything from plex other than
[798.72 --> 803.52]  the library sharing that some of my extended family still participates in and all that stuff but
[803.52 --> 809.32]  for my home setup not missing at all and with tail scale i can still watch all my stuff wherever i go
[809.32 --> 815.24]  so it doesn't impact me it's just you know for friends and family it's a little they don't really
[815.24 --> 819.90]  have a way to watch it right now well i did put a video up on youtube on the tail scale channel
[819.90 --> 826.96]  showing you how to create a vps with a caddy reverse proxy and then you point your friends
[826.96 --> 830.78]  and family at that and then they stream through that which is connected over tail scale back to
[830.78 --> 836.20]  your house so yeah i could see going that route one day you could put yours up on the moose my friend
[836.20 --> 841.90]  that's true that's true there will be a day when starship is a thing and they're launching much bigger
[841.90 --> 846.30]  star links too that i'll probably have you know even more bandwidth available at home and i could start
[846.30 --> 850.26]  just hosting it from home too possibly yeah maybe one of these days we'll put a true nas into space
[850.26 --> 857.64]  huh that'd be great speaking of the true nas 24.10 release just came out and normally we don't talk
[857.64 --> 862.92]  about true nas too much on this show primarily because neither of us actually use it i don't think
[862.92 --> 867.88]  in anger or certainly not the modern versions but this one's worth your attention good listeners
[867.88 --> 878.82]  because they are switching from a kubernetes based app back end to a docker based back end with compose
[878.82 --> 886.66]  front and center much better much much less complicated yeah why push water uphill huh so i had
[886.66 --> 892.04]  you know tried it out back in the day where it was k8s under the hood and inevitably with all these
[892.04 --> 898.54]  things i ended up dropping down to the command line to do something and my lord when i saw how
[898.54 --> 904.06]  complicated all that was just so i could set up samba shares in a gui and you know set up a few zfs
[904.06 --> 909.74]  dis in a gui i i bailed i just couldn't i couldn't couldn't so but their evolution over the last couple
[909.74 --> 914.16]  of years has been really interesting right because they've you know transitioned completely to linux they've
[914.16 --> 919.08]  been moving away from the k8s under the hood setup they've been simplifying it they've kind of been
[919.08 --> 926.20]  moving to a more cloud first kind of design so i i think yeah it's probably worth another look
[926.20 --> 933.46]  in no small part thanks to all of the work done on the linux-based open zfs implementation yeah and
[933.46 --> 938.38]  if you trace that back actually i don't wonder if we don't need to give ubuntu some credit here
[938.38 --> 944.32]  oh really well they were the first ones to ship zfs right they were the first ones that had the
[944.32 --> 950.12]  courage to say all right oracle the license is the license but we're going to ship it anyway
[950.12 --> 958.52]  i would love to dig in and figure out how they're shipping zfs is it a dkms module i wonder how they're
[958.52 --> 962.34]  working i'd love to so you know i don't know let's figure it out yeah i think we should look at it
[962.34 --> 968.04]  see how it works just see if that kind of stuff could get brittle at all because like you know
[968.04 --> 974.46]  that kind of build on demand module stuff can break from time to time but uh yeah i mean i think i think
[974.46 --> 979.70]  true nas is shipped as an atomic release so i would imagine you just update an image but yeah we'll
[979.70 --> 985.16]  we'll report back on that yeah that might make all the difference now another common complaint with
[985.16 --> 993.08]  zfs in particular mostly from home users or or users of you know less than wendell-sized petabyte
[993.08 --> 1001.10]  arrays worth of disks yeah is that there's no real easy way to expand a vdev but with this release they
[1001.10 --> 1008.22]  are adding raid z vdev expansion too geez really it's happening it's actually happening now yeah
[1008.22 --> 1014.90]  yeah no i think this might come thanks to the hex os stuff that they've they've had some pressure from
[1014.90 --> 1020.90]  hex os to kind of do some some of this stuff to make it more palatable to unraid refugees that kind of
[1020.90 --> 1027.12]  thing and you know i'm just glad to see it finally land to be honest i think i first read about this
[1027.12 --> 1034.26]  roughly when i was in diapers no kidding well this is great because it makes everything downstream of
[1034.26 --> 1039.90]  this better right so unraid can incorporate these fixes of course you know ubuntu users will be able
[1039.90 --> 1046.54]  to get these that's just that's that was that was a complaint of mine from ages ago um yeah this
[1046.54 --> 1052.26]  man we're just the cfs project is just really got i got in such a great solid spot right now we're
[1052.26 --> 1060.94]  lucky to have it we are indeed so it looks like a really good release that's true nas 24.10 electric
[1060.94 --> 1067.58]  eel now another project that saw some really nice updates this week was the mealy recipe app project
[1067.58 --> 1073.84]  with their 2.0 release you finally got me to try it with this one oh did i good i don't know why i was
[1073.84 --> 1080.22]  sleeping on this recommendation i guess i kind of had this solved but oh it's so good now they
[1080.22 --> 1084.68]  they introduced a feature that i think i'm going to use on day one and this might have been what got
[1084.68 --> 1089.54]  me is they have this thing called households now and i guess it was one of their most requested
[1089.54 --> 1094.02]  feature and it required quite a bit of technical rerouting under the hood it was a big change they
[1094.02 --> 1101.58]  said it touched 300 plus files and 10 000 lines of code and so a household is a subdivision of groups
[1101.58 --> 1107.42]  groups with a collection of users so groups can be considered completely separate on their own
[1107.42 --> 1111.82]  right so they have their own sets of everything but households can mix their data with each other
[1111.82 --> 1117.34]  and so uh you know we have the kids house we have my house we have the studio like i could actually see
[1117.34 --> 1122.72]  setting up each household with the recipes that work best at each household or maybe at the studio or
[1122.72 --> 1127.44]  with the kids or whatever it could be it's really a nice it's a really nice feature that's a very yeah
[1127.44 --> 1133.24]  you're a very unique customer for this aren't you two sets of kitchens really yeah with with
[1133.24 --> 1139.04]  completely unique requirements you know an rv's cooker versus a you know electric stovetop or
[1139.04 --> 1145.12]  whatever you have you know how interesting i hadn't thought of that so now i think it just this 2.0
[1145.12 --> 1150.76]  version just looks so good um and i'm also kind of curious to try out their shopping list generation
[1150.76 --> 1155.88]  because they've i guess they've revamped that i never had a really i i looked at it once before but i
[1155.88 --> 1161.42]  never really used it for very long um they've all got it's one of those apps that is just a
[1161.42 --> 1168.20]  constantly i think i don't do that much cooking that requires recipes but when i do it's always
[1168.20 --> 1175.12]  like six months between uses yes and i think oh how did i smoke those ribs six months ago what was the
[1175.12 --> 1180.52]  sauce combo i used or you know whatever and sure enough i wrote it into my obsidian and then pasted it
[1180.52 --> 1186.16]  into mealy six months ago and bada bing bada boom i can just search for it on my phone and all is
[1186.16 --> 1191.20]  well holidays are often a time where i'll have to look something up so mealy is yeah i think will be
[1191.20 --> 1196.66]  great for that before i'd use next cloud recipes which i did like but mealy really takes it to the
[1196.66 --> 1201.60]  next level and version 2.0 just seems like they've they've added so many things that people have been
[1201.60 --> 1206.70]  using it for a while have requested it's a great time to jump in and it's a very simple docker compose
[1206.70 --> 1210.28]  away i think we'll talk more about next cloud after the break
[1210.28 --> 1219.86]  unraid.net slash self-hosted unraid it's a powerful easy to use operating system for self-hosted servers
[1219.86 --> 1224.60]  or network attached storage that you've been dying to build go make the most out of the hardware you
[1224.60 --> 1230.02]  already have no matter how many or what types of drives you have on hand unraid is a flexible easy
[1230.02 --> 1235.36]  to use operating system that will help you manage all of that so yes even those mismatched drives it
[1235.36 --> 1240.88]  is possible with unraid it has a simple ui that makes it easy to manage your entire stack of docker
[1240.88 --> 1247.70]  applications or vms or many of the many many many more community provided applications it's a flexible
[1247.70 --> 1254.44]  linux-based nas os that has tooling built around docker and vm management built-in vpn support thousands
[1254.44 --> 1262.04]  of apps plugins and zfs support and with unraid 7 beta they're completely rounding out unraid zfs
[1262.04 --> 1268.68]  capabilities i'm talking full integration of zfs boys let's go pew pew pew pew pew pew it's looking
[1268.68 --> 1276.34]  really good i am so excited about where unraid is going it is an example of in a very approachable
[1276.34 --> 1283.20]  but yet powerful system perfect for those of you who don't have days and days and days to commit to
[1283.20 --> 1289.28]  this thing and build it from scratch you can start with a powerful easy to use ready to go unraid
[1289.28 --> 1294.38]  operating system and unraid 7 is looking really good i think the beta is getting pretty close to
[1294.38 --> 1298.96]  being done so it could be the time now to check it out here's how you get started you probably know
[1298.96 --> 1303.80]  about unraid but go check it out and support the show it's unraid.net slash self hosted maybe you've
[1303.80 --> 1307.38]  thought about getting something going but you just haven't had the time maybe you've got hardware
[1307.38 --> 1312.78]  around that you could use but you're just not sure if you want to manage all of it unraid can solve
[1312.78 --> 1317.24]  that problem for you and a lot more also great for small businesses or your own projects in your
[1317.24 --> 1323.34]  go check it out unraid.net slash self hosted that's unraid.net slash self hosted
[1323.34 --> 1332.02]  i want to start this section just really sharing some really rather tragic news to be honest
[1332.02 --> 1339.62]  the developer ttech who is the chap behind the really rather excellent proxmox helper scripts if
[1339.62 --> 1344.28]  ever you've come across those has unfortunately announced today that he's been transferred into a
[1344.28 --> 1351.14]  hospice for you know hospice related things yeah dang that is really awful so there was an
[1351.14 --> 1354.74]  announcement on the github issue for the project that he's obviously going to be stepping back from
[1354.74 --> 1361.60]  maintenance of the things you're no kidding yeah uh so yeah really just a quick psa heart goes out to
[1361.60 --> 1365.18]  you buddy and thanks for all there thanks for all the work you've put into this project over the years
[1365.18 --> 1371.26]  definitely it's it's one person can have such a huge impact on so many people with those types of
[1371.26 --> 1376.72]  projects so grateful for the people that have spent any other time contributing to that i spent a lot
[1376.72 --> 1382.48]  of my time sort of ripping out my setup since the last episode and then putting things back in so not
[1382.48 --> 1388.14]  only was i kind of rehauling some of the media stuff but uh i had a full-on divorce with next cloud
[1388.14 --> 1393.72]  since our last episode i was gonna say does hadia know about this yeah you know i i didn't really
[1393.72 --> 1399.68]  tell her at first and so her machine wasn't sinking for a few days uh i shut it down i mean i stopped the
[1399.68 --> 1405.30]  container i was done alex i was like i went for a few days with it just offline but at the end of
[1405.30 --> 1412.02]  all of it probably about a five six day window i ended right back up with next cloud which i totally
[1412.02 --> 1416.50]  am going to recommend but with a better setup so what what were what were you doing like you thought
[1416.50 --> 1422.14]  right this is it i'm i'm done with next cloud yep it's too flaky i just want to do it like you know
[1422.14 --> 1427.78]  individual apps or it's just we were growing apart like i for months i've been having this super
[1427.78 --> 1432.64]  annoying problem i don't know if anybody else out there's ever had this and if they ever fixed it
[1432.64 --> 1437.44]  i'd love to know what they did because my fix was blow away the instance for a very brief period of
[1437.44 --> 1442.90]  time alex i had auto upload turned on for my photos because that's initially how i was going to back up
[1442.90 --> 1447.46]  my photos but i didn't like the performance of next cloud photos so i switched to prism and photo sync
[1447.46 --> 1453.30]  and i turned off next cloud sync and then after prism for a short period of time i switched to image and
[1453.30 --> 1457.90]  i've been on image and the image app since you know maybe over a year or two now i don't know
[1457.90 --> 1466.06]  but that entire time my next cloud client has never stopped auto uploading every single picture i take
[1466.06 --> 1471.92]  i've gone in the app and turned it on and off you know i've uninstalled the app twice totally deleting
[1471.92 --> 1477.62]  all the data installed it from the play store installed it from fdroid no matter what i do once it's
[1477.62 --> 1482.44]  signed in it starts auto syncing even though the settings off it starts auto syncing my photos
[1482.44 --> 1488.50]  and then because it does this it has file conflict uploads and i'm getting notifications about conflicts
[1488.50 --> 1493.50]  it's duping files and burning up disk space and burning up backup and burning bandwidth up
[1493.50 --> 1499.72]  and i just wasn't using the web ui much either and i realized why don't i just get rid of this thing
[1499.72 --> 1506.14]  and all i need is cal dev card dev and task syncing and there's a couple of projects out there
[1506.14 --> 1514.28]  that are just servers that let you sync endpoints they don't offer any web ui but they are listening
[1514.28 --> 1519.22]  and they allow you to connect and sync your devices and i thought that's the that's the route i want to
[1519.22 --> 1525.94]  go and i ended up setting up edibase and it looked really good for the text because it's really
[1525.94 --> 1532.62]  it's an end-to-end encrypted database client setup and it allows you to sync many things including
[1532.62 --> 1541.72]  calendar contacts tasks but other things as well and i thought here we go so you know with claude's
[1541.72 --> 1549.06]  help i start setting up edibase and generating a nix config and i get pretty far into it and i realize
[1549.06 --> 1556.96]  okay but i still have to solve tasks okay you know i can do that and i i still need to solve notes
[1556.96 --> 1565.04]  hmm and i realized what was my what was my original goal my original goal to essentially recreate
[1565.04 --> 1574.34]  a sort of my own icloud like experience that runs on my gear uses my software and by that i mean like
[1574.34 --> 1580.36]  i create a task or a calendar or a contact or a note on a phone or on a desktop doesn't matter which device
[1580.36 --> 1585.22]  it syncs to all of them and if i've set a reminder to alert me i get an alert on the phone i get an alert
[1585.22 --> 1590.98]  on the desktop and that's really important for me because i have such a bad memory i have such bad
[1590.98 --> 1596.28]  add that i need to set myself reminders and tasks from whatever device i'm at because if i go too
[1596.28 --> 1601.24]  long i just it completely is out of my mind and i do want photos but i have that with images i started
[1601.24 --> 1606.22]  thinking about all this and i thought i'm going to end up just recreating next cloud that's what i'm
[1606.22 --> 1610.50]  going to do as i because i probably every now and then i probably will want a web interface to some
[1610.50 --> 1614.82]  of this from time to time because i move machines all the time that's when i realized
[1614.82 --> 1622.14]  maybe instead of trying to replace every component of next cloud i should do an mvp next cloud
[1622.14 --> 1628.64]  set up a little bit better you know just try one more time to really try to get this right you know
[1628.64 --> 1633.66]  what i mean like this is the time i'll take all of my lessons learned and apply it to this setup
[1633.66 --> 1640.38]  so what's the crack then did you end up doing it exactly the same way like a next module or what
[1640.38 --> 1646.68]  so before i had it as um a docker composed and i don't know if i was using the linux server io image
[1646.68 --> 1652.18]  or if i was using the the one that's up from next supposedly next cloud on docker hub but i was using a
[1652.18 --> 1657.90]  docker composed setup that worked pretty well that whole thing is so confusing by the way yeah it is
[1657.90 --> 1663.42]  which docker image to use it's just like just make one like why is there an all-in-one and that anyway
[1663.42 --> 1670.84]  i digress so this time i did opt to go the next module route and the one of the reasons is is
[1670.84 --> 1676.52]  because you can pull in redis and it'll configure it to be a front-end cache and so i set that all up
[1676.52 --> 1685.14]  and i had a couple of issues but pretty straightforward got it working got to the login screen decided i go
[1685.14 --> 1692.58]  to bed wake up the next morning and next cloud's completely locked down it's got an error saying too
[1692.58 --> 1697.90]  any login attempts no way you can get access i haven't done anything with it yet i hadn't even
[1697.90 --> 1702.80]  really logged in it just just immediately got locked down because i think my android device was trying to
[1702.80 --> 1707.96]  sync all night and every time i tried to sync it was a login attempt so you know first thing i'm doing
[1707.96 --> 1716.96]  is i'm busting out the occ command to fix it but this is where it is so nice to be on a nix module setup
[1716.96 --> 1723.62]  because back in the day alex back in the battle days of the late 90s and the early aughts we didn't have
[1723.62 --> 1730.42]  vms we didn't have containers everything got installed on the host system which meant like
[1730.42 --> 1734.08]  all the dependencies broke when you had to upgrade and all that kind of stuff but every package
[1734.08 --> 1740.46]  was on the host system and while that's a mess it has one major advantage that is still really nice to
[1740.46 --> 1746.34]  this day it's not a big deal but it's nice and that is everything's in your path and you don't
[1746.34 --> 1750.90]  have to like figure out what container you have to execute into and what bespoke crappy little
[1750.90 --> 1755.88]  container environment it has and what tools are available what's in that path everything is actually
[1755.88 --> 1762.46]  on your system it's properly managed with nix yes the caveat being right nix but that's so the
[1762.46 --> 1768.16]  occ command was just in my path you know and i just right and i just put my user in the next cloud
[1768.16 --> 1772.98]  group so he can run all the occ stuff i didn't have to like execute into anything it was it's
[1772.98 --> 1778.40]  just and then everything is managed with systemd so if i make a change and i and i want to restart i
[1778.40 --> 1783.74]  just restart the systemd service right it's using the tooling built into my operating system instead
[1783.74 --> 1790.82]  of recreating and replacing like init systems it just uses the built-in stuff and it it is definitely
[1790.82 --> 1795.90]  faster on the same hardware it's not not blow away fast but i don't use the web interface a lot
[1795.90 --> 1802.20]  yeah i could see that i still i don't know like i i think maybe i'm just i'm i stockholm syndrome at
[1802.20 --> 1808.12]  this point with docker like i just end up finding that that compartmentalization is actually quite
[1808.12 --> 1813.54]  useful because again once you exec into the container everything's on your path but i've been
[1813.54 --> 1819.04]  fighting around with nix a lot in the last month or two doing a lot of stuff with like flake refactoring
[1819.04 --> 1826.50]  and you know helper modules and that kind of stuff um it's it's so nice until it isn't and i do
[1826.50 --> 1832.22]  sometimes find that the whole nix module system adds enough friction that i think to myself
[1832.22 --> 1838.72]  eh i'll do it later whereas a compose a compose yaml is just like 10 lines of code i'm like yeah
[1838.72 --> 1843.66]  come on alex you can set that up yeah i mean my nix i bet you my nix configs probably
[1843.66 --> 1849.88]  i bet it's probably 25 ish lines but there is you know there's some stuff in there like i'm also
[1849.88 --> 1855.86]  doing the database in there and things like that as well yeah yeah it's it's a different it's a
[1855.86 --> 1860.68]  different kind of isolation like there is a there is something nice about when you have something in
[1860.68 --> 1866.46]  a container it's just essentially totally detached from the os there's some there's some nice aspects
[1866.46 --> 1873.54]  to that too but what i love about this particular setup right now is it's not like i don't have to
[1873.54 --> 1879.08]  worry about who publishes what images it's all just right there in the config file as well so
[1879.08 --> 1883.88]  i had an issue with the app store not working and i can just go look at somebody else's config file
[1883.88 --> 1889.46]  oh i i have apps enabled but i don't have extra apps enabled i have to have extra app but you know
[1889.46 --> 1894.64]  you can just figure that stuff out by just comparing config files within 10 minutes do i have do i have a
[1894.64 --> 1900.92]  tip for you yeah okay the github code search have you ever come across this yeah yeah okay and you can
[1900.92 --> 1906.40]  just search for the nix line you're looking for oh that's a great idea and look at like 500 examples
[1906.40 --> 1913.48]  of that specific nix service oh man it's the way to go i i the other thing i really like is nginx is
[1913.48 --> 1919.44]  all managed as well so i just add one more line you know i define what the host name is what the port
[1919.44 --> 1924.12]  it's what port is on of course in this case it's 80 and 443 but you know and so the nginx stuff and the
[1924.12 --> 1930.80]  ssl certs all handled at that point and you go into you can go into the config of my next cloud
[1930.80 --> 1936.10]  dot nix file and you can say tell next cloud it's using https even if it doesn't know it because it's
[1936.10 --> 1942.08]  behind a reverse proxy just tell it that and i don't have to go like dig through their config dot php
[1942.08 --> 1946.50]  or anything like that and the other nice thing is is when i show it to wes he can review and be like
[1946.50 --> 1949.76]  oh i see okay that's how you turn that on right like he doesn't have to go dig through on my
[1949.76 --> 1955.18]  individual php files or wherever next cloud sticks that kind of stuff so i'm pretty happy
[1955.18 --> 1960.58]  with the setup in terms of like maintenance i'm happier with the performance and i think kind of
[1960.58 --> 1967.10]  starting with a clean slate and just re-importing things like files and calendars directly was the
[1967.10 --> 1972.50]  way to go because so far i don't think the auto sync has happened although i haven't checked it today
[1972.50 --> 1978.88]  i haven't taken many photos can i let you into a little secret yeah my media server's been running
[1978.88 --> 1986.88]  nix os for the last nine months you madman i switched silently because i i would you know
[1986.88 --> 1995.94]  i just wanted to do it on my own my own terms it is the most stable any server of mine has ever been
[1995.94 --> 2001.00]  because it's so it's not difficult to tinker that's not the phrase i mean to say it's just like
[2001.00 --> 2007.90]  i've got it set up and the config is self-documenting and why would why would i change it it's working
[2007.90 --> 2014.44]  perfectly it's also it's it's anti-fragile yes it's not brittle yeah at all i could like make
[2014.44 --> 2019.84]  a guess and like okay how is this supposed to work what how and i could i could try to build i could
[2019.84 --> 2025.58]  test build it and it either passes or it fails and i don't have to commit it and so it gives me
[2025.58 --> 2031.16]  license to experiment well assuming you can decipher the esoteric nix error message that you get
[2031.16 --> 2037.24]  so you know what my trick is and i'm going to fully admit it but it kind of works is i just give
[2037.24 --> 2042.22]  claude ai a little context of what i was doing and then i just straight up copy the error message paste
[2042.22 --> 2047.80]  it into claude and then ask claude to explain it to me when i and it does a remarkably decent job yeah
[2047.80 --> 2053.28]  that's been my trick you know i haven't really missed google much at all this month
[2053.28 --> 2060.10]  yeah no i i think claude and perplexity and search xng right i mean you combine the three of those for
[2060.10 --> 2070.24]  me and uh google's feeling old yeah it is it feels it feels like google search is from a bygone era
[2070.24 --> 2077.34]  it you're right it does i think we'll come up with our full-on conclusions next episode i've been looking
[2077.34 --> 2085.74]  at a self-hosted perplexity alternative which puts together searching search xng with olama and an app
[2085.74 --> 2092.78]  called perplexicar which gives you a fully self-hosted way of of doing these kind of ai searches i need to
[2092.78 --> 2097.52]  look for a claude self-hosted version i haven't quite gotten there yet but we'll give you our full
[2097.52 --> 2103.74]  thoughts in the next episode of no googtober but spoiler alert it's going pretty well
[2103.74 --> 2112.86]  tailscale.com slash self-hosted go try out tailscale for free on 100 devices and three users while you
[2112.86 --> 2118.18]  support the show at tailscale.com slash self-hosted that's not a limited time deal it's the plan i'm on
[2118.18 --> 2123.88]  right now it is the easiest way to connect devices and services directly to each other wherever they
[2123.88 --> 2128.62]  are regardless of the network conditions between them tailscale is incredible at connecting devices
[2128.62 --> 2133.00]  and letting them communicate directly even when you're behind double carrier grade nat
[2133.00 --> 2139.54]  i can attest to that you can build out a flat simple mesh network across multiple networks like
[2139.54 --> 2146.74]  say a vps a dc a mobile device your home lab whatever it might be all these locations maybe you
[2146.74 --> 2151.02]  have multiple offices and branches and you want them all to be able to share resources tailscale
[2151.02 --> 2157.50]  creates a flat mesh network it's privacy for everyone it's super approachable it's easy to deploy
[2157.50 --> 2164.74]  it's a no fuss vpn and if you're in the business world it makes all the business solutions look like
[2164.74 --> 2170.34]  something from 1987 so a tail scales 100 user plan you can really get a feel for it and go from there
[2170.34 --> 2177.94]  and just this week you could now add a new aws vm to your tail net right from your tail scale admin
[2177.94 --> 2183.58]  console you select your options you click through a couple of pre-configured ec2 instances boom boom
[2183.58 --> 2188.82]  wham bam boom you've got a new instance up and running on your tail net every node we spin up
[2188.82 --> 2195.14]  we spin up on our tail net i have no inbound ports on any of the firewalls in fact there are services
[2195.14 --> 2200.44]  and resources you use with jupiterbroadcasting.com and associated services around us they're getting
[2200.44 --> 2204.36]  delivered over our tail net and you don't even know it but on the back end it's all protected it's
[2204.36 --> 2209.60]  all secure and the nodes can be mobile it's powerful stuff and it's super simple to get started
[2209.60 --> 2215.78]  and it's a great way to support the show while you up your networking game so one more time check
[2215.78 --> 2222.30]  it out get 100 devices for free and three users when you go to tailscale.com slash self-hosted
[2222.30 --> 2230.28]  tailscale.com slash self-hosted so mike salgado writes in i don't really understand why people
[2230.28 --> 2237.30]  choose plex or jellyfin as their media servers what are the benefits over these versus using just dnla
[2237.30 --> 2242.82]  i've been using this for many years in fact since i was in college i'd like to hear your thoughts or
[2242.82 --> 2248.20]  if you guys have already discussed this thanks for the great show mike i mean there's an advantage to
[2248.20 --> 2255.76]  keeping it simple sometimes sometimes for me it's uh i've got a couple of tvs and so i want to
[2255.76 --> 2260.50]  synchronize the watch state that's how it started of course there's a lot more reasons now but that's
[2260.50 --> 2264.34]  how it started i want to synchronize the watch state across all my machines do you remember back in
[2264.34 --> 2270.12]  the day where with xbmc where you used to host a my sequel database and have it hook into that and
[2270.12 --> 2274.50]  yeah yeah i mean you know and there's people still doing that and if that setup still works for you
[2274.50 --> 2279.58]  it's fine but then there's like it evolves like now i want something where i can download a bunch
[2279.58 --> 2284.30]  of files onto my device when i'm traveling and there's a lot of advantages jellyfin has because it's
[2284.30 --> 2290.52]  a centralized database so for example i mentioned ersatz tv earlier ersatz talks to jellyfin's
[2290.52 --> 2296.22]  database via the api and is aware of and makes available all of the shows that the jellyfin server
[2296.22 --> 2302.64]  is indexing and so other applications can create an ecosystem because plex and jellyfin both have
[2302.64 --> 2308.98]  very comprehensive apis around them as well yeah i think for me to add on to what chris is saying as
[2308.98 --> 2316.36]  well it's things like rich metadata it's things like sharing with friends and family it's things like
[2316.36 --> 2322.42]  transcoding on the fly if the format isn't supported by the target device lots it's like death by a
[2322.42 --> 2329.36]  thousand paper cuts none of those things on their own are enough to condemn dnla but for me all of
[2329.36 --> 2336.90]  those things combined make it that i i will always use a media server over just a directory of files
[2336.90 --> 2343.36]  wherever possible and you could try it out and still use dlna if you want because jellyfin can act as
[2343.36 --> 2347.54]  a dlna server so you could play around with it and point it at your files and see if you like what
[2347.54 --> 2351.96]  it does and still just interface with it over that if that's your preference can it use that as a
[2351.96 --> 2357.10]  library source or is it well i don't i've never used it but i would imagine it creates like a when i've
[2357.10 --> 2361.92]  used dlna before it kind of creates like a directory structure of your library and then you kind of
[2361.92 --> 2367.06]  browse through it almost like folders and then you can select the file that in my previous life when
[2367.06 --> 2371.12]  i've tried it i have not tried it yeah yeah neither of us are dnla experts by the sound of it
[2371.12 --> 2376.14]  no i mean i've you know it was nice especially back when i we used my console my game consoles
[2376.14 --> 2381.32]  as media center boxes because a lot of times like the playstations will do dlna and things like that
[2381.32 --> 2386.32]  but these days i just have set top boxes oh that's probably another reason media centers have become
[2386.32 --> 2392.36]  more popular right set top boxes are app based and so you know you put the jellyfin app on there and
[2392.36 --> 2396.72]  pulls in all your library information and also they don't completely suck anymore you know like that is
[2396.72 --> 2402.24]  their video shield and what have you is as meant that that 10 foot interface that we were all
[2402.24 --> 2408.56]  chasing with xbmc or whatever it actually works now yeah yeah they've surpassed cody in terms of ui
[2408.56 --> 2414.14]  design i'm gonna say it but for a long time they hadn't and so you know there's there's that too so
[2414.14 --> 2417.72]  great question though really that's you know sometimes it's good to kind of question some of the
[2417.72 --> 2424.12]  fundamentals i think we got some boosts this week self-hosting is life is our baller booster
[2424.12 --> 2431.82]  with 40 000 sats and they wrote i am loving search or crx ng however you say it uh thanks for the
[2431.82 --> 2436.30]  recommendation guys even though it's preventing tracking with cookies you can still be tracked by
[2436.30 --> 2442.50]  your ip address so you might want to run it through a search vpn uh maybe it's paranoia but i think it's
[2442.50 --> 2447.62]  really necessary to remain anonymous keep up the great work boy the energy that takes but i respect that
[2447.62 --> 2454.48]  you know it's interesting that you say that self-hosting is life because there was there was a
[2454.48 --> 2458.80]  period i think it was you know just i'm gonna say thursday morning it doesn't matter when it was does
[2458.80 --> 2463.18]  it but there was a there was one morning where i literally every search i put through searching
[2463.18 --> 2468.96]  just said too many requests and so i came out through an exit node which happened to be a digital
[2468.96 --> 2477.38]  ocean droplet and suddenly it worked instantly and so i'm like hmm maybe google don't actually like me
[2477.38 --> 2485.52]  not being trackable oh i like that bacon that's some good one yeah i i uh i wonder i think you know
[2485.52 --> 2490.86]  you have so many other services still i don't think i don't think we can fully hide from google
[2490.86 --> 2496.38]  but i fantasize about the ability to be totally anonymous online just for fun like i never actually
[2496.38 --> 2502.76]  get around to doing it but it i'll bet you there are plenty of graphs in alphabet hq that are not going
[2502.76 --> 2507.48]  up and to the right these days yeah i bet you're right you know thank you for the boost self-hosting
[2507.48 --> 2517.18]  his life and uh i agree gob right comes in with a row of mcducks 22 222 sats says maybe and he's
[2517.18 --> 2522.08]  talking to me you should consider two gpus in that new system one for linux desktop and one for machine
[2522.08 --> 2527.50]  learning you could consider the machine learning gpu in external enclosure it's not the low cost option
[2527.50 --> 2530.68]  but you buy once you cry once
[2530.68 --> 2538.50]  yeah you know what if you were to do something like pcie pass through this is this is basically
[2538.50 --> 2544.54]  what i do with that epic box that i have in my basement i have the arc pro card for transcoding
[2544.54 --> 2552.20]  and the nix vm i talked about just a moment ago and then i have an nvidia a4000 and i'm not suggesting
[2552.20 --> 2557.46]  you need a card that is that powerful for machine learning and olama and stuff but it sure is nice
[2557.46 --> 2562.84]  if you can get it you can then pass that through with pcie pass through to a separate vm so i have
[2562.84 --> 2569.90]  a nix i call it nix nv llama nvidia llama is what i call this one uh and that runs my image machine
[2569.90 --> 2576.28]  learning library it does olama it was what i use for perplexica this week uh yeah i like you know
[2576.28 --> 2582.02]  just having a gpu on the network yeah whether you throw it in the moose or not could be another option
[2582.02 --> 2587.64]  i i was thinking that too really damn handy and you think oh i'm not going to use it that much
[2587.64 --> 2591.32]  and then you realize you're using it every day for some some little task and you're like oh
[2591.32 --> 2597.90]  and it doesn't break because it's nix you're like oh this is this is yeah i am fully self-sufficient
[2597.90 --> 2602.90]  right now this is cool i could see going with two gpus and putting one of them in the moose and then
[2602.90 --> 2610.14]  having an excuse to go then with an amd or even an intel arc i mean one of my guilty pleasures is the
[2610.14 --> 2615.22]  intel arc i have it in the machine i'm sitting in front of right now in the studio rock solid just
[2615.22 --> 2622.26]  the most rock solid video card on linux it's like oh man it's just perfect it's been i felt your pain
[2622.26 --> 2628.34]  hard this week because i tried to put nix os on my desktop and i have a 3080 in there yeah yeah
[2628.34 --> 2634.42]  wayland does not even the nix os installer booted just to a black screen with a white cursor
[2634.42 --> 2640.96]  so i had to change for a different tty and do the nix install that way then in make sure i had the
[2640.96 --> 2646.50]  correct nvidia driver installed before i did the reboot with you know nix os switch whatever once i
[2646.50 --> 2653.22]  booted to my desktop it booted me into a plasma wayland session and everything seemed fine it picked
[2653.22 --> 2661.56]  it picked 1920 by 1028 on a 5k 2k monitor so that was fun yeah so i fixed that it also then it picks
[2661.56 --> 2668.32]  30 hertz on 120 hertz monitor so i fixed that yeah and then i loaded up factorio which isn't
[2668.32 --> 2674.48]  exactly a graphically demanding video game it runs perfectly happy on an m1 macbook air just to give
[2674.48 --> 2682.28]  you an example and it was just black screen flickering nonsense i'm just like yeah i just
[2682.28 --> 2687.10]  don't want to pass this yet no i mean they're you know they're working on like their later generation
[2687.10 --> 2691.30]  graphics cards are going to be supported pretty well by the new open source drivers they've been
[2691.30 --> 2697.54]  working on but man i just you know i've been using the proprietary drivers in nix yeah that that's
[2697.54 --> 2702.98]  that's trickier with wayland they have this new open source kernel driver they're working on that
[2702.98 --> 2709.16]  that is going to make the experience better and will work with wayland much better is that nouveau or
[2709.16 --> 2713.22]  is that something else um it's i think they're using part of nouveau for the user space but they're
[2713.22 --> 2717.82]  building a new kernel module i'll have to give that a look then yeah yeah maybe and that would make
[2717.82 --> 2724.38]  the nvidia experience more tolerable but i feel like it's not there yet so i'm i like this suggestion
[2724.38 --> 2733.10]  a lot i would i was reminded this week why nvidia on linux turns people into graybeards yeah and then
[2733.10 --> 2737.74]  you put an amd card in there or an intel arc and it's so simple you don't even think about the video
[2737.74 --> 2743.94]  card because you literally never have to everything just works it's a total 180 yeah thank you geo appreciate
[2743.94 --> 2750.76]  that shaft and spanner came in with 20 000 that's a great one uh thanks for your no google october
[2750.76 --> 2757.22]  coverage yeah it took me a while to set up uh how do you say it alex search i think searching just
[2757.22 --> 2764.22]  searching okay search xng yeah i know it took me a while to set up searching or search xng and tube
[2764.22 --> 2771.82]  archivist so i'll be doing a no oct no google november okay uh yeah we need to name like a
[2772.42 --> 2777.30]  november or something november something there's probably a name in there you could come up with
[2777.30 --> 2781.94]  he says unfortunately just as i was starting to persuade my wife that it would be good to watch
[2781.94 --> 2788.80]  her youtube subscriptions with maybe no ads via jellyfin an ad came up on youtube for a holiday in japan
[2788.80 --> 2795.62]  a very expensive 2025 holiday location has now been chosen and she wants to keep seeing ads in the
[2795.62 --> 2802.28]  middle of her youtube video she wants to see the ads you know i do hear this argument from some people
[2802.28 --> 2808.96]  that like i enjoy ads i enjoy google telling me what to buy and i'm like i really don't have enough
[2808.96 --> 2815.18]  money well i mean i try to make enjoyable ads so i appreciate that sentiment but i've never been a big
[2815.18 --> 2819.58]  fan of the youtube ads just never really worked so yeah no but your ads are different you know like
[2819.58 --> 2825.68]  in this episode tailscale and unraid for example they are products that you and i both use or have
[2825.68 --> 2832.74]  used and personally would use and endorse like yeah it's not like we're selling box fresh meals or
[2832.74 --> 2838.84]  whatever that's very true in fact if i could find a good box fresh meal that i like maybe i would but i
[2838.84 --> 2844.08]  haven't found one yet i tried one recently did not like it maybe we should get sponsored by
[2844.08 --> 2849.30]  squarespace do you think that would work for this audience you know those those bastards uh i emailed
[2849.30 --> 2854.82]  them a couple of years ago maybe before the show even i said hey this is like a couple years this
[2854.82 --> 2858.58]  maybe three four years i don't know it was a while ago hey you want to sponsor we had a show that i
[2858.58 --> 2863.58]  thought would be a good fit at the time and they told me they were pulling out of podcasts at that time
[2863.58 --> 2868.08]  it was like years ago but everybody knows about them now i don't think it's a good fit with this
[2868.08 --> 2873.62]  audience though maybe wordpress.com instead there you go that should be real smooth
[2873.62 --> 2880.30]  no problem there at all uh vt52 has a jar jar boost 5000 sats says it's been a while since i boosted
[2880.30 --> 2885.76]  so i thought i'd drop a couple of self-hosted recommendations number one is dumb a self-hosted
[2885.76 --> 2893.16]  alternative to front-end genius the lyric site and it's fantastic so dumb don't you just love the name
[2893.16 --> 2900.28]  i do love the name um and then you got gluten which uh gluten right uh tired of worrying about
[2900.28 --> 2907.18]  linux's iso traffic egress use docker gluten makes all traffic egress through open vpn or a wire guard
[2907.18 --> 2912.88]  endpoint yes and if so if you have a mulvad subscription or anything like that you can
[2912.88 --> 2919.44]  funnel all of the traffic using the docker network mode through that egress point it also supports
[2919.44 --> 2924.90]  things like kill switches and dns leak tests and it's a really nice solution if you need it
[2924.90 --> 2932.50]  some solid uh recos there wink wink nudge nudge hint hint thank you vt really appreciate that and our
[2932.50 --> 2940.54]  last boost this week is undead fable and he comes in with or they come in at least with 2500 sats
[2940.54 --> 2949.54]  for the gpu topic this is a hot tip i just purchased an rtx 4060 from jawa.org j-a-w-a.org
[2949.54 --> 2959.00]  which is a second-hand marketplace for 256 greenbacks after tax and shipping wow okay an rtx 4060 for 256
[2959.00 --> 2966.10]  i'm gonna go over to jawa jawa.gg it is it has enough internal ram at 8 gigs for a lot of models on
[2966.10 --> 2972.62]  llama and it has a high 15.11 tflops value and i can use it for av1 encoding that's all those are
[2972.62 --> 2978.64]  all that's nice uh from what i have seen it was the sweet spot to slot into my server for all my tasks
[2978.64 --> 2983.90]  yeah so the thing about putting a gpu in a server you're not only worried about performance of course
[2983.90 --> 2986.90]  but you're also worried about the power budget and therefore the heat that it generates yeah
[2986.90 --> 2992.06]  so you've got to find that sweet spot and it seems like this guy's found a good a good balance yeah i
[2992.06 --> 2997.90]  mean 15 tflops isn't going to be blow away right but it's still going to be better than the cpu and
[2997.90 --> 3002.34]  you know then the cpu is available for other stuff i suppose have you ever run olama on a cpu
[3002.34 --> 3010.12]  yes yes yes it's it's just painfully bad yeah that's how i knew that my nvidia drivers weren't
[3010.12 --> 3015.78]  working on my on my nixon store to start with because it just defaulted to the cpu i'm like oh well
[3015.78 --> 3021.60]  this sucks chat gpt is way faster and then i realized that it didn't find the cuda device and then when it
[3021.60 --> 3026.54]  did it was like oh oh there we go this is this is more like it doesn't it make you kind of just
[3026.54 --> 3031.10]  be in awe of the amount of power that is behind these different chatbots these huge public
[3031.10 --> 3036.48]  chatbots oh yeah yeah and you think how many millions of requests they're getting every minute
[3036.48 --> 3040.98]  yeah you know yeah it's really something well that's it thank you everybody who boosted in we
[3040.98 --> 3044.86]  didn't have a blow away show we we had five boosters this week so if you've been thinking about boosting
[3044.86 --> 3050.10]  in now would be a great time to step up we did have 30 folks stream as they listened though so our
[3050.10 --> 3055.22]  streamer stacked 106 038 sats combined with our boosters we have a grand total this week
[3055.22 --> 3062.46]  of a humble 195 760 sats but we still appreciate everybody who participated in the value for value
[3062.46 --> 3067.70]  system if you're our member or if you're a booster thank you we appreciate it very very much especially
[3067.70 --> 3073.42]  as the ad winter goes on your support really means more than ever so you can do that with a
[3073.42 --> 3078.76]  completely self-hosted setup something like albi hub maybe get like something start nine going or let
[3078.76 --> 3082.96]  fountain do the infrastructure for you fountain.fm we'll have links to get started in the show notes
[3082.96 --> 3091.68]  thank you everybody self-hosted.show slash sre big shout out to our members this spot right here is
[3091.68 --> 3098.52]  available jupiter broadcasting is booking q1 of 2025 if you can believe it and if you would like to reach
[3098.52 --> 3103.94]  the most sophisticated intelligent audience in technology i mean it self-hosted audience is really
[3103.94 --> 3109.08]  incredible contact me chris at jupiter broadcasting.com i'd love to work with somebody who is
[3109.08 --> 3116.50]  also a listener of our shows the support has been down we got a good clip and memberships um about
[3116.50 --> 3121.70]  three weeks ago and we had a good amount of boost come in but since then the show has been trending
[3121.70 --> 3127.84]  downward and that's difficult after a prolonged ad winter even this spot here is available in self-hosted
[3127.84 --> 3133.76]  which traditionally has been sold out so if you've been thinking about boosting there is an incredible
[3133.76 --> 3141.38]  opportunity for somebody who likes to self-host tools like start nine and albi hub and so many
[3141.38 --> 3147.44]  others allow you to participate in the boost process entirely self-hosted on your own infrastructure
[3147.44 --> 3152.28]  using free software over a peer-to-peer network now you don't have to you could also grab something
[3152.28 --> 3157.10]  like fountain and use their infrastructure that makes it really quick but i just think sometimes the
[3157.10 --> 3162.32]  self-hosters in our audience miss that there's a way to do all of this and support the self-hosted
[3162.32 --> 3167.32]  podcast using entirely self-hosted infrastructure of course you can always set it on autopilot and
[3167.32 --> 3173.82]  become a member at self-hosted.show slash sre and as a little thank you we cut out these types of ads
[3173.82 --> 3179.78]  all the ads but we also give you a little post show a little extra content as a thank you for putting
[3179.78 --> 3184.08]  your support on autopilot so boost in and get your message right on the air or put your support on
[3184.08 --> 3189.00]  autopilot and get a post show either way we really appreciate it and if you think maybe this spot could be
[3189.00 --> 3193.74]  yours you got something you want to promote to our audience chris at jupiterbroadcasting.com
[3193.74 --> 3199.56]  and thank you to all of you that came and said hello all things open in raleigh this week as we
[3199.56 --> 3206.88]  record it's wednesday and all things open just wrapped up and we had a fantastic meetup at trophy
[3206.88 --> 3212.74]  brewing with the unraid crew and some of you that came got discount coupons for unraid which is pretty
[3212.74 --> 3219.36]  cool uh it's just nice to see your faces sometimes you know and and everyone that says oh hey alex i
[3219.36 --> 3224.38]  recognize your voice and all that it's just people walk by and it takes them a second and then they hear
[3224.38 --> 3230.32]  you they overhear you hey that's alex yeah yeah now hey he's he's uglier than i thought he was i gotta
[3230.32 --> 3235.92]  know should i go to this like i i feel like i'm missing out like i feel like all things open has gone
[3235.92 --> 3241.72]  to the point when i don't go i feel a little fomo yeah it's about 3 000 people this year i think i think
[3241.72 --> 3247.28]  somewhere in the 3 000 to 3 500 range that's a that's a good size it's quite a big conference now
[3247.28 --> 3254.00]  but it it straddles that line really nicely between being a community conference with a decent hallway
[3254.00 --> 3260.74]  track and also attracting decent sponsors and decent speakers too that you would get at say the bigger
[3260.74 --> 3266.28]  conferences like a kubecon or a reinvent or summit or something like that and because it's red hats
[3266.28 --> 3271.34]  home turf it's literally two blocks away from the tower in downtown raleigh you've got a whole bunch
[3271.34 --> 3275.48]  of red hat folks there so it's really good for networking and just chatting you know carl george
[3275.48 --> 3280.96]  came in and and stayed with me this week whilst uh whilst he was at the conference so you know we
[3280.96 --> 3286.14]  were talking to the alma linux folks at the booth next to us oh that's great yeah alma linux was there
[3286.14 --> 3292.72]  i think rocky were there uh there was a mechanical keyboard stand there from the keev.io people yes
[3292.72 --> 3297.88]  who turns out they're in durham and i'm i've ordered a keyboard and i'm gonna go to the warehouse
[3297.88 --> 3301.86]  and pick out pick it out and try all the different switches and stuff oh that's so cool you gotta take
[3301.86 --> 3305.80]  some video when you do that yeah i think what's really great is it just underscores
[3305.80 --> 3313.06]  for me at least there is so much on my doorstep i didn't have a clue about like try i met the guys
[3313.06 --> 3319.42]  from tri-log triangle linux users group i met a few people who live all you know in in this general
[3319.42 --> 3324.10]  area that are like oh we go to the pub on wednesdays and talk about you know left-wing politics
[3324.10 --> 3327.94]  and blah blah blah you should come down and i'm like what what are you trying to say
[3327.94 --> 3334.92]  that sounds really nice socialist i know all right i gotta try it i got it i gotta try it because it
[3334.92 --> 3339.52]  does seem like the networking would be good be good for the pods be good for me i got the yeah there
[3339.52 --> 3344.72]  were there were a few podcast networks there there was the changelog guys were there uh was it whiskey
[3344.72 --> 3350.80]  web and something i forget what the name was there were a few guys there doing me um and jay from
[3350.80 --> 3357.86]  linux linux tv was there jim salter was there alan pope was there you know so good good bunch of
[3357.86 --> 3362.78]  folks and you know some of those people you don't get to see very often in fact popey i think i've
[3362.78 --> 3369.28]  only ever met in america so isn't that funny yeah yeah given he's you know from 20 minutes away from
[3369.28 --> 3374.86]  my hometown it's just weird well maybe next year it sounds like it's one to put on the calendar
[3374.86 --> 3379.04]  and you know for the last couple years too you've had a nice meetup around all things open too so i
[3379.04 --> 3384.98]  fomo on that as well yeah i think i think the next big conference on my radar is probably fozdem
[3384.98 --> 3392.44]  though brussels in february doesn't really thrill me but you know i know and i'm already working on
[3392.44 --> 3399.52]  linux fest northwest and i'm probably going to be at scale oh yeah yeah yeah i think i overdid it this
[3399.52 --> 3403.48]  spring with too many conferences so i'm gonna dial it back a little bit i gotta figure out where to cut
[3403.48 --> 3408.94]  problem is my favorite ones are in the spring they're all back to back to back but you know
[3408.94 --> 3413.58]  that's why we have the meetup page whichever ones we actually end up doing meetup.com slash jupiter
[3413.58 --> 3417.20]  broadcasting if you just follow that when we do have an event we'll we'll post it up there
[3417.20 --> 3424.14]  sure will and you can find me on these here interwebs at alex.ktz.me yeah if you want to come
[3424.14 --> 3430.36]  play with the wild side find me on nostr chris las.com i'm also on weapon x or matrix you know what we got a
[3430.36 --> 3434.30]  matrix server you can find it at jupiterbroadcasting.com slash matrix lots of rooms including
[3434.30 --> 3439.58]  some self-hosted chatter indeed in fact this week we colonized the rally room so if you're at one of
[3439.58 --> 3444.20]  these conferences make sure to check our matrix for a relevant room now thanks for listening
[3444.20 --> 3447.04]  everybody that was self-hosted.show slash 135
