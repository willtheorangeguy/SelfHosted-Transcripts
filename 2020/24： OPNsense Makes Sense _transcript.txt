[0.00 --> 4.18]  Coming up on today's Self-Hosted, Chris figures out how hot is too hot,
[4.74 --> 7.54]  I attempt to perform an extreme remote firewall install,
[7.96 --> 10.46]  and we share some of our favorite SSH tricks.
[11.02 --> 11.64]  I'm Alex.
[12.06 --> 12.72]  And I'm Chris.
[13.00 --> 14.44]  And this is Self-Hosted 24.
[15.36 --> 17.02]  I have squirrels on my mind.
[17.22 --> 17.54]  Okay.
[17.86 --> 18.40]  Squirrel mail.
[18.72 --> 19.38]  Go on then.
[19.78 --> 23.28]  Well, I am not happy about this Google news.
[23.36 --> 24.48]  Have you seen this Gmail news?
[24.92 --> 25.36]  What's that?
[25.42 --> 28.16]  That they're rolling everything all into Gmail?
[28.16 --> 31.04]  One big productivity suite.
[31.74 --> 34.32]  And I'm just not having it.
[34.66 --> 35.56]  I just want email.
[35.92 --> 37.44]  I want decent web email.
[37.88 --> 41.58]  But I don't want to host it myself, I don't think.
[41.92 --> 43.92]  So that's when squirrel mail came to mind.
[44.32 --> 45.52]  We've been over this before, Chris.
[45.82 --> 49.22]  I think we decided that self-hosting email wasn't worth the trouble.
[49.46 --> 50.00]  What's changed?
[50.22 --> 50.96]  Here's what I'm thinking.
[51.56 --> 53.92]  Is instead of hosting the email myself,
[53.92 --> 57.96]  I just want a really nice web-based IMAP client.
[58.16 --> 59.78]  Something that would render well on mobile.
[60.28 --> 63.08]  That I could add all of my Google accounts to.
[63.20 --> 65.14]  Of which there are Minty for the various shows.
[65.62 --> 66.64]  There are plenty, I should say.
[66.76 --> 67.98]  Many and plenty Minty.
[68.14 --> 70.38]  And I bring them all into one web mail client.
[70.54 --> 72.78]  Where I can just check that one web mail client.
[73.18 --> 74.52]  And I want something nice.
[74.92 --> 75.96]  That is clean.
[76.20 --> 78.14]  Ideally could even support GPG encryption.
[78.30 --> 79.10]  But not required.
[79.80 --> 80.24]  You know what I mean?
[80.24 --> 81.64]  It does sound appealing.
[82.02 --> 85.52]  I mean, I'm sure there's plenty of ways to skin this particular turkey.
[85.80 --> 88.44]  But next cloud mail comes to mind.
[88.86 --> 89.00]  Yeah.
[89.12 --> 91.08]  And RoundCube also came to mind.
[91.18 --> 93.58]  I know, I think RoundCube might be my top contender.
[94.40 --> 96.50]  But I bet the people in Discord might know.
[97.02 --> 98.22]  Self-hosted.show slash Discord.
[98.36 --> 101.00]  I'd like to know if you have an IMAP client that you really like.
[101.04 --> 101.48]  Or something.
[101.98 --> 102.78]  Doesn't even, whatever.
[102.96 --> 104.02]  Just plugs into Google.
[104.02 --> 105.28]  That's really all it has to do.
[105.36 --> 108.02]  So I can get out of their email client.
[108.28 --> 110.52]  But still take advantage of their infrastructure.
[111.28 --> 112.20]  So speaking of the Discord.
[112.64 --> 116.18]  We had some really interesting discussions over there this week.
[116.18 --> 118.16]  About the best way to install Docker.
[118.58 --> 120.26]  It's changed a lot over the years.
[120.38 --> 123.86]  Because Docker decided to change their versioning.
[123.94 --> 126.08]  I think maybe two or three years ago at this point.
[126.12 --> 129.04]  Which broke a bunch of package repositories.
[129.04 --> 133.10]  And if you type apt install Docker in Ubuntu these days.
[133.10 --> 135.76]  It doesn't give you the latest version.
[136.34 --> 137.36]  It's really confusing.
[137.48 --> 137.96]  What do you think?
[138.34 --> 141.64]  There are a lot of ways to install Docker on a Linux box.
[141.94 --> 143.80]  In some ways it's almost easier on Mac and Windows.
[143.88 --> 148.86]  Because there's just one sort of official way for end users or consumers to deploy it.
[148.88 --> 149.60]  But on Linux.
[149.96 --> 153.64]  You can just go through the process of adding Docker's repos.
[153.68 --> 155.10]  And they have documentation on that.
[155.60 --> 156.08]  Or.
[156.58 --> 159.40]  And I think this was really the crux of the discussion on Discord.
[159.74 --> 161.98]  You can use what they call their convenience script.
[161.98 --> 167.52]  Which is just essentially curling a git-docker-sh file.
[167.74 --> 170.10]  And then just running it with pseudo privileges.
[170.76 --> 174.50]  And it goes through the process of setting up everything.
[174.74 --> 177.16]  Removing conflicting packages if necessary.
[177.36 --> 178.52]  Adding GPG keys.
[178.64 --> 180.06]  Getting the repos configured.
[180.72 --> 181.72]  Pulling down the software.
[182.00 --> 182.66]  Installing it all.
[183.22 --> 184.48]  It does all of it for you.
[184.48 --> 190.46]  But no one is generally that comfortable with just running an arbitrary script from the internet.
[190.46 --> 193.72]  Even when it's from a project as well known as Docker.
[193.96 --> 195.10]  What's the worst that could happen?
[195.50 --> 197.92]  Pipe to curl, pipe to bash, pseudo?
[198.36 --> 198.66]  You know?
[199.20 --> 200.34]  I admit it though, Alex.
[200.44 --> 203.16]  When I set up Docker on the Raspberry Pis.
[203.16 --> 205.40]  I went with the convenience script.
[205.50 --> 210.46]  Because I just, I wanted to be sure I had the right repos and the right packages for the Raspberry Pi platform.
[211.14 --> 211.28]  Yeah.
[211.40 --> 217.18]  So the script that you're talking about, I think, is served at get.docker.com.
[217.84 --> 222.22]  And this basically gives you at the top, there's a very short little disclaimer.
[222.22 --> 226.92]  And you can pipe this, basically they don't recommend you curl pipe to bash.
[227.02 --> 231.30]  They recommend you save it locally, chumod it, and then run the script.
[231.46 --> 233.16]  Which is perfectly fine.
[233.64 --> 239.92]  And the fact that you're going to get.docker.com looking at the script you're about to actually download.
[240.86 --> 243.64]  I think for me that removes a lot of the anxiety.
[243.64 --> 260.20]  Like, for example, when you're going to go and install Homebrew on macOS, for example, their lead installation method is curl this script and pipe it to pseudo bash so that you can install whatever this script on the internet is.
[260.30 --> 269.60]  Now, the reason that that's bad is that sometimes web hosts get hacked or malicious code is injected into the script.
[269.60 --> 273.90]  And if you're a bad guy hacker, you might not replace the entire script.
[274.10 --> 277.48]  You might just add a couple of small lines down in the corner that nobody notices.
[278.62 --> 291.32]  And so the whole purpose of verifying the scripts using the char hash that is there is to verify that the code you're looking at on the screen is actually the code that was downloaded.
[291.46 --> 294.40]  And there wasn't some clever, you know, injection going on somewhere.
[294.90 --> 294.96]  Yeah.
[294.96 --> 310.68]  I think it's for me, it's variations of seriousness, because another tool where I sort of abuse the bash curl, download a shell script and go thing is one of my absolute favorite data visualizers for system metrics, net data.
[311.96 --> 313.84]  Top installation source, right?
[313.92 --> 315.32]  That's the one liner.
[315.90 --> 317.46]  And God, I'm such a hypocrite.
[317.46 --> 318.32]  I realize now.
[318.54 --> 318.78]  Yeah.
[318.78 --> 321.00]  I know.
[321.44 --> 327.54]  I definitely curl pipe to bash on a more regular occurrence than I think I should.
[328.06 --> 328.50]  Yeah.
[328.86 --> 334.08]  Like I was saying, though, I would assign various like gradients of risk to my systems.
[334.30 --> 340.58]  I have boxes that are pretty unimportant, like quite literally a laptop that's come in for review.
[340.58 --> 348.58]  It's going to be in the studio for one week and we're just totally punishing this machine to try to get all of the performance data we can from it.
[349.18 --> 352.22]  I'll bash curl net data on that thing without a second thought.
[352.68 --> 360.40]  Now, if it's a primary system that has private information, I often will try to go a more traditional route, especially like if it's an arch box.
[360.46 --> 361.78]  I'll see if it's just in the AUR.
[361.78 --> 367.84]  If it's a Ubuntu box, I'll see if there's a PPA or a snap before I ever go that route.
[368.32 --> 373.00]  But you just have to kind of assess the risk in these each individual cases.
[373.76 --> 378.26]  And remember that the installation is just one spot where you're vulnerable.
[378.26 --> 386.70]  But a lot of times these things we're installing install other tools that bring all kinds of dependencies with them and have their own package repositories.
[387.04 --> 388.88]  So really, it's a rabbit hole, Alex.
[388.88 --> 391.86]  Always, always a rabbit hole with self-hosting.
[392.46 --> 398.70]  Another rabbit hole you could go down if you want to install Docker in a repeatable way is to use Ansible.
[399.10 --> 405.36]  So I've used the Jeff Geerling Ansible role from Ansible Galaxy for the best part of two or three years at this point.
[405.98 --> 407.00]  Just works flawlessly.
[407.26 --> 408.84]  So that's another route you could take.
[409.54 --> 410.00]  Like that.
[410.46 --> 412.48]  Another reason I should be using Ansible right there.
[413.52 --> 414.40]  One of many.
[415.78 --> 417.52]  So how was the heat?
[417.68 --> 418.62]  You're back from Texas.
[418.88 --> 419.98]  We did pretty well.
[420.46 --> 420.84]  Spoiler alert.
[420.92 --> 421.44]  Nothing died.
[421.92 --> 422.52]  Nothing died.
[422.66 --> 423.38]  So that's good.
[423.78 --> 427.56]  We did get up to 104.9 in the server booth.
[428.04 --> 428.26]  Hold on.
[428.34 --> 428.66]  Hold on.
[428.76 --> 430.10]  I'm going to have to do the maths on that.
[430.38 --> 432.14]  105 to Celsius.
[432.84 --> 434.62]  40.5 Celsius.
[434.86 --> 436.02]  That is what?
[436.12 --> 438.64]  So that's ambient air temperature or that's inside the server seat?
[438.98 --> 439.94]  That's inside the booth.
[440.02 --> 440.14]  Yeah.
[440.20 --> 440.98]  The server seat.
[441.14 --> 441.62]  That's high.
[442.00 --> 442.44]  It is.
[442.44 --> 446.58]  And I think I might have seen it thermal throttle a little.
[446.58 --> 453.80]  I might have seen some thermal throttle in action when we were watching Plex and we lost the playback session and then had to reconnect.
[454.02 --> 455.42]  And it took a little while to reestablish.
[455.48 --> 456.90]  It just seemed like things were running a little slow.
[456.90 --> 459.98]  So I think thermal throttling did kick in in that situation.
[460.24 --> 463.32]  But for the most part, the human venting procedure worked.
[463.86 --> 466.96]  Between Hadi and I, we managed to usually vent it every single day.
[467.38 --> 471.32]  So what we do is when we had the AC running and cranking, we'd vent it because the AC is right above it.
[471.40 --> 472.64]  So it can blow in there pretty well.
[472.64 --> 475.90]  And then we could try to ride that as long as we could.
[477.20 --> 477.96]  But that was nice.
[478.26 --> 479.40]  It was nice that it didn't die.
[479.48 --> 480.96]  I did run a reduced load.
[481.06 --> 484.14]  So now that I'm back in the Pacific Northwest, Shinobi's back online.
[484.64 --> 485.84]  Sync thing is running again.
[486.30 --> 490.30]  So it's, you know, back to full operational status now.
[490.78 --> 494.70]  I'm just picturing all of your gear breathing a sigh of relief going, oh, thank goodness.
[495.04 --> 497.82]  We're back home where the temperature isn't just hot.
[498.00 --> 498.30]  I know.
[498.30 --> 506.14]  I wouldn't be surprised if I shortened the life of power bricks and, you know, maybe my router.
[506.38 --> 507.90]  You don't really know, right?
[507.94 --> 511.02]  I could have just cut a couple of years off their life.
[511.18 --> 512.82]  But so does going down the road.
[513.20 --> 515.14]  It's amazing, the Texas heat, really.
[515.86 --> 524.00]  I think it was Carl George was saying in the Telegram group that the value of a parking spot in Texas is not valued by how close it is to the shop.
[524.26 --> 525.60]  It's valued by the shade.
[525.60 --> 530.44]  When we were driving home, we were heading west and north often.
[531.04 --> 535.86]  And that meant that the sun in the afternoon when it was its hottest was on the driver's side of the RV.
[536.28 --> 537.86]  It was slow cooking you.
[538.24 --> 540.04]  Oh, oh, it got so bad.
[540.12 --> 542.86]  And the AC, even in the dash, can only do so much.
[542.92 --> 545.14]  So it got to the point where it's basically blowing warm air at me.
[545.50 --> 546.80]  Oh, that sounds gross.
[546.80 --> 550.60]  We just could barely, barely stay alive because it was so hot.
[550.68 --> 552.38]  I mean, you just couldn't get comfortable some days.
[552.38 --> 562.10]  So we very much started taking like strategic parking spots as much as we could, which meant we ended up staying in a few areas that were fully off grid, which is really what I built the system for.
[562.56 --> 563.78]  It worked great.
[564.52 --> 566.52]  Plex is a bit of a pain in the neck.
[566.54 --> 570.56]  If you have multiple profiles, like I have a parent's profile and a kid profile.
[570.56 --> 573.36]  And you select it when Plex launches.
[573.60 --> 576.72]  And I think it uses their online service for that authentication.
[577.26 --> 577.62]  And so.
[578.02 --> 580.18]  You're going to be a bit of a diva trying to load that screen, huh?
[580.54 --> 581.52]  Oh, my gosh.
[581.68 --> 583.86]  So in those cases, we just fell back to Cody.
[584.22 --> 584.98]  I don't blame you.
[585.18 --> 585.34]  Yeah.
[585.70 --> 588.42]  And then I just have to remember to go back and, oh, yeah, Mark has watched.
[588.56 --> 589.18]  Mark has watched.
[590.40 --> 590.76]  Yeah.
[590.88 --> 593.42]  Because you can't even use the Plex plugin in Cody in that scenario.
[593.56 --> 594.52]  It just, it doesn't work.
[594.92 --> 596.92]  So Cody saved the day in that case.
[596.92 --> 608.62]  And then just an aside, when we got back, I was sort of concerned that our outdoor Z-Wave devices wouldn't work after being disconnected from the controller for 50 days.
[608.86 --> 613.44]  Because they get marked in Home Assistant as, and the term isn't offline.
[613.64 --> 617.60]  It's some other term, like dysfunctional or disconnected or something.
[617.82 --> 618.82]  I think it's disconnected.
[619.36 --> 625.32]  So, you know, when I would look at my devices, I'd see all of my outside stuff, which is a handful of devices marked as disconnected.
[625.32 --> 626.72]  And I just didn't like the error message.
[626.72 --> 632.70]  And I've done trips where I've been gone for a couple of weeks and come back and they've reconnected fine.
[632.82 --> 637.86]  But I thought, 50 days, you know, this may never work.
[637.96 --> 639.44]  I may have to redo my Z-Wave setup.
[640.34 --> 650.66]  And I got home and I completely had forgotten about it until I was walking around outside and I noticed my automatic sunset lighting coming on.
[651.32 --> 652.46]  And I was like, oh, yeah.
[652.46 --> 658.22]  Oh, so not only did it just pick right up, but it's working with the automations just like it always did to it.
[658.56 --> 660.12]  It just connected no problem.
[660.20 --> 662.74]  And I can go in and I can do a Z-Wave repair network.
[662.74 --> 672.60]  But if you're looking for yet another option to control outdoor stuff and for some reason, maybe Wi-Fi doesn't work or the devices aren't available.
[673.20 --> 677.36]  I give a hearty recommendation for Z-Wave because it may even work for like holiday equipment.
[677.50 --> 680.26]  Maybe you only bring it out for certain times a year.
[680.26 --> 684.38]  And I think it would just connect right back up and all the automations would pick right up.
[684.74 --> 686.38]  Don't have any Z-Wave stuff.
[686.70 --> 687.76]  Sorry, Z-Wave.
[688.56 --> 690.30]  It, I don't know.
[690.98 --> 699.04]  When I moved into this house, I wanted to investigate Zigbee and Z-Wave and all those different protocols.
[699.68 --> 703.88]  But in the end, they ended up sticking with Wi-Fi because I've just not had any issues with it.
[703.88 --> 705.58]  It just, just works fine.
[705.70 --> 711.30]  And I don't know if that makes a difference, you being in a tin can or anything to the Wi-Fi signals and stuff.
[711.58 --> 715.58]  But, you know, for the most part, I ended up using Z-Wave for sensors.
[716.02 --> 722.30]  That's an interesting use case because I, I generally speaking, when I'm building a sensor, it's a temperature sensor or something like that.
[722.30 --> 727.40]  Or everything I build is based around an ESP8266 pretty much.
[727.86 --> 733.66]  And for the most part, they, they just need Wi-Fi, you know, 2.4 gig Wi-Fi.
[733.66 --> 734.68]  And they just work.
[735.10 --> 739.10]  I think like 90% of my devices are on Wi-Fi.
[739.40 --> 749.50]  But I think early on, a lot of the manufacturers that do outdoor stuff like lighting and sprinkler controls and whatnot, I think they just went all in on Z-Wave.
[749.50 --> 756.14]  So a lot of the outdoor equipment that I have found that is ruggedized and rubberized and all of that is Z-Wave.
[756.14 --> 764.94]  And then these Aotec sensors that I love so much are both USB powered or lithium battery operated.
[765.58 --> 773.16]  And when you go with a lithium battery and you use Z-Wave as the radio, you get a year battery life off of one of those little lithiums.
[773.20 --> 774.20]  It just looks like a Duracell.
[774.52 --> 775.06]  Oh, man.
[775.10 --> 775.84]  That does sound good.
[776.08 --> 776.32]  Yeah.
[776.66 --> 778.74]  Aren't they like a mesh style thing?
[778.82 --> 780.44]  They all communicate to each other, don't they?
[780.44 --> 788.10]  That's the other thing that works really nice about them for outdoor devices is each one, well, depends on if you buy the right type, but they can extend the mesh network.
[788.48 --> 793.26]  And so that's why it's probably a good idea that I run a repair on my network.
[793.26 --> 800.86]  Because when you tell Home Assistant to repair the Z-Wave network, the nodes sort of rediscover their positioning and kind of set up a new mesh.
[801.20 --> 807.90]  And if you've had a device missing for a while and then you bring it back online, it's generally a good idea to run that repair so that the mesh network is stronger.
[807.90 --> 810.78]  I really need to investigate some Z-Wave stuff.
[811.16 --> 815.16]  I kind of feel like maybe it's sort of at the end of its era.
[815.16 --> 821.22]  You know, there's new standards coming out from Google and Apple and I don't know.
[821.60 --> 827.64]  I think most stuff now has enough horsepower and battery life to support just Wi-Fi always on.
[828.08 --> 832.36]  So it's sort of maybe on the decline, but I really like the ones I have.
[832.42 --> 833.46]  They sure do work reliably.
[834.28 --> 842.04]  And I just got a little stick that plugs right into my Raspberry Pi and Home Assistant detects it and just manages the whole Z-Wave network for me.
[842.04 --> 846.86]  I can manage all the particulars, like how often a device updates right through the Home Assistant UI.
[847.12 --> 849.58]  So how did you manage remote access whilst you were gone?
[849.82 --> 851.58]  Like SSH tunnels and stuff like that?
[851.92 --> 855.54]  Yeah, I am a fan of the good old simple SSH tunnel.
[855.74 --> 858.70]  When I'm coming into the studio, that's WireGuard.
[858.90 --> 860.90]  You know, that's all the connections into the studio.
[861.18 --> 863.74]  I'll use WireGuard and I love it, man.
[863.84 --> 865.16]  I've got it on my phone.
[865.28 --> 866.00]  I've got it on my tablet.
[866.08 --> 866.84]  I got it on my laptop.
[866.84 --> 879.64]  But if I want to connect into the RV remotely, which does come up, especially when there's things that I forget at home on my file server, you know, sometimes SCP gets the job done, Alex.
[879.84 --> 880.66]  We've all been there.
[880.92 --> 890.22]  I've talked about this before on Linux Unplugged, but I don't think I've ever mentioned my super sweet self-repairing SSH tunnel powered by Systemd setup.
[890.60 --> 891.62]  I was trying to get another S in there.
[891.62 --> 905.66]  But it is what I have, and I have a couple of resource links in the show notes, and I set this up on all of my, well, all my systems really, for the most part, I've started doing this on my laptop too, because it's just, I like having a backdoor in.
[906.26 --> 917.90]  And what I have done is set up a Systemd unit file that starts as a service in the background, and it does an SSH connection to a digital OSHAM droplet.
[917.90 --> 923.62]  And then from wherever I'm at, I can use that digital OSHAM droplet as a jump host.
[924.06 --> 930.60]  I log into that droplet, and then I jump to whichever machine I like based on the port number I've assigned it.
[930.86 --> 933.00]  And that gets around your carrier grade NAT problems?
[933.68 --> 943.48]  Absolutely, because the connection is, it's being initiated like on the Raspberry Pi or on the laptop, and it's SSHing outbound, and then it's connecting to the droplet.
[943.48 --> 952.18]  So it's not an inbound connection to the RV, it's an outbound connection, and Systemd monitors that, and if it goes down, it restarts it automatically.
[952.66 --> 953.44]  That's really nice.
[953.82 --> 958.26]  I think I've used something similar when I wanted to kind of get out from behind a corporate firewall.
[958.92 --> 959.96]  I probably shouldn't have done that.
[960.02 --> 962.14]  It was probably very much against their IT policy.
[962.60 --> 963.80]  I did the same thing, though.
[963.80 --> 969.44]  I even had like a whole virtual Linux box I used to remote desktop into so I could watch YouTube.
[970.10 --> 970.74]  Oh, yeah.
[970.90 --> 971.86]  Yeah, that was it, you see.
[972.04 --> 977.18]  You know, back in the dark ages, before mobile phones were a thing, like text messaging your wife was a pain in the butt.
[977.32 --> 980.92]  Whereas now it's just so easy, you don't really even think about that kind of stuff.
[981.08 --> 986.48]  But you can, you know, once you've got an SSH tunnel set up, you can route everything through it.
[986.48 --> 995.14]  So, I mean, I've mentioned SSH shuttle before, for example, but there's all sorts of stuff you can do, like remote port forwarding or local port forwarding.
[995.30 --> 1003.74]  So let's say you have a database running on a system and you want to give your friend access, just, you know, whilst you're doing some dev work or something.
[1004.54 --> 1012.72]  You could do remote port forwarding so that they could connect on their local system to a port, and it's as if they're on your machine for a few minutes.
[1012.72 --> 1016.06]  You know, there's some really cool stuff you can do with SSH.
[1016.68 --> 1018.14]  Maybe we'll touch on it one day.
[1018.64 --> 1025.84]  Yeah, and I'm also happy to report that port forwarding works through a jump host, which is fantastic for me.
[1025.90 --> 1035.44]  So I can get to my sync thing, Webman UI from the studio, and I can set up a sync between the studio and the RV from just the one location.
[1035.82 --> 1036.88]  It's really pretty great.
[1036.88 --> 1045.30]  And the kind of peace of mind, too, that I have this private, low-end, dedicated droplet, and that's the only thing my RV is connecting to.
[1045.68 --> 1048.82]  And then I can manage what systems I allow a connection in from.
[1049.30 --> 1052.44]  And so it's a pretty nice compromise of functionality and security.
[1053.12 --> 1056.06]  And digital oceans, you know, firewalls and all that kind of stuff.
[1056.14 --> 1058.28]  I mean, you can lock it down really quite a lot.
[1058.50 --> 1062.22]  And sometimes you end up locking yourself out.
[1062.22 --> 1065.56]  I've definitely not done that and had to reset the root password before.
[1065.92 --> 1065.94]  Yeah.
[1066.06 --> 1069.34]  But, yeah, I've done all sorts of similar stuff.
[1069.50 --> 1074.86]  And you just feel like you're in, what's it called, Mr. Robot or something when you're doing this kind of stuff, don't you?
[1075.72 --> 1077.88]  Especially when you're doing port forwarding through a jump host.
[1077.98 --> 1079.68]  That actually feels kind of cool.
[1080.20 --> 1090.18]  It boggles the mind when I pull up a web page that's hosted on a Raspberry Pi inside a dinette booth in an RV that's connected over a MiFi that's being relayed through a droplet in San Francisco.
[1090.18 --> 1093.38]  So are you familiar with the SSH config file?
[1093.82 --> 1093.98]  Yeah.
[1094.32 --> 1097.90]  There's a command you can put in there for each of your hosts called proxy jump.
[1098.44 --> 1102.54]  And that will let you transparently use that jump host that you mentioned.
[1103.12 --> 1106.64]  So, for example, let's say you have a host called server.
[1107.36 --> 1110.84]  You put in host server and then you type SSH server.
[1111.28 --> 1116.12]  You can put all sorts of parameters in there like user, port number, host name, that kind of stuff.
[1116.24 --> 1119.34]  So you don't want to type the IP address in every time, for example.
[1119.34 --> 1122.52]  You can just type SSH server and it will go straight to that IP address.
[1123.40 --> 1125.38]  Another one you can do is proxy jump.
[1125.54 --> 1128.80]  And so you can start chaining multiple SSH hosts together.
[1129.28 --> 1131.22]  And I'm just looking through my config here.
[1131.30 --> 1136.02]  And to get into my dad's house, I have about four or five different hops.
[1136.08 --> 1136.88]  I think it's five.
[1136.88 --> 1154.40]  So I go from here to my Bastion server in my LAN, which then goes to a DigitalOcean droplet, which then goes to the OpenSense firewall, which I'll come on to shortly, at my dad's house, which then goes to the host inside the LAN.
[1154.40 --> 1156.16]  So there's like five different hops there.
[1156.36 --> 1164.28]  And each of those hops only permits traffic from a specific place and a specific IP address on the WAN side anyway.
[1164.74 --> 1170.36]  And so I like to think, even though it's a really complex house of cards sometimes, that it's actually quite secure doing that.
[1170.86 --> 1171.90]  Very similar to what I'm doing.
[1172.42 --> 1175.64]  I did not add it to my config file, though.
[1175.72 --> 1177.48]  And that is a super good tip.
[1177.60 --> 1181.96]  I think I will, because why not save myself typing extra commands?
[1182.32 --> 1182.82]  That's great.
[1182.82 --> 1183.72]  I love that.
[1184.00 --> 1189.06]  I need to write a blog post on ProxyJump because I'll post you a little bit in Telegram right now.
[1189.58 --> 1194.40]  And you can take a look and you can see how you can chain these different things together and take a look.
[1194.50 --> 1196.18]  I think we may have ourselves a future topic there.
[1196.74 --> 1199.06]  But I heard you tease OpenSense.
[1199.48 --> 1200.40]  A little bit, yeah.
[1200.58 --> 1200.72]  Yeah.
[1200.78 --> 1204.54]  So when I moved into this house, I was running PFSense.
[1204.90 --> 1211.96]  And sometime in January or February, I don't remember, pre the event, I don't really remember much before the event,
[1211.96 --> 1217.60]  I switched to OpenSense purely because it supports WireGuard.
[1217.80 --> 1219.14]  It's the only reason I switched.
[1219.90 --> 1222.12]  And PFSense, to my knowledge, still doesn't.
[1222.92 --> 1229.38]  For this, you know, what's it been, four or five month period, I've had OpenSense at my house and PFSense at my dad's house.
[1230.14 --> 1231.14]  That's been working fine.
[1231.14 --> 1234.92]  And we had an open VPN server, you know, for our iPlayer usage and that kind of stuff.
[1234.98 --> 1241.66]  But I thought, come on, it would be cool to have OpenSense in both places and then set up a site to site WireGuard VPN.
[1242.44 --> 1254.50]  And what that means is that I can now type in IP addresses of my dad's remote LAN subnet and access them on my local laptop on my LAN as if I'm in England.
[1255.00 --> 1255.90]  Oh, that's the dream.
[1256.18 --> 1257.42]  That's the dream, Alex.
[1257.42 --> 1259.70]  It's pretty cool, I must admit.
[1260.12 --> 1268.72]  So I owe my dad a beer or two because as part of that thought process, obviously I had to replace PFSense remotely.
[1269.04 --> 1271.60]  Now you think about this, I want to paint you a picture for a moment.
[1272.00 --> 1274.74]  Oh God, I am already thinking about it.
[1274.88 --> 1280.18]  You want to remote install a firewall that only has serial console access.
[1280.76 --> 1281.84]  So think about what you need here.
[1281.88 --> 1283.18]  You need a null modem cable.
[1283.18 --> 1290.64]  So I'm running this on an APU2D, I think is what it's called, PC Engine's integrated system.
[1291.24 --> 1291.30]  Okay.
[1291.52 --> 1296.12]  So I need a serial null modem cable to convert the serial console output to USB.
[1296.50 --> 1303.34]  I need him to get his ThinkPad, put it next to that box in a cupboard dangling an Ethernet cable out the side.
[1303.34 --> 1312.06]  I need him to get me a USB stick so I can flash OpenSense onto that and then get him to put that into the APU2 so I can boot from that.
[1313.26 --> 1315.66]  But think about this, right?
[1315.74 --> 1318.30]  When you're installing a firewall, what don't you have?
[1318.80 --> 1319.86]  Internet access, Alex.
[1320.00 --> 1320.36]  Correct.
[1320.36 --> 1332.50]  And so my damn ass thought it would be a good idea to try and remotely install a firewall from America in my dad's cupboard in England when he barely has 3G in his house.
[1332.92 --> 1333.40]  Oh no.
[1333.56 --> 1342.42]  So he and I were resorted to SMS text for a few, maybe about half an hour whilst we tried to figure out which cable wasn't quite plugged in correctly.
[1342.42 --> 1348.82]  And I was expecting to be reduced to Telegram so at least we could send pictures.
[1349.14 --> 1353.72]  But no, we were reduced to SMS and MMS didn't seem to work.
[1353.92 --> 1356.92]  So yeah, that was a fun half hour.
[1357.06 --> 1360.74]  And I really apologise to my father for putting him through that.
[1361.20 --> 1368.28]  So I've got him plugged directly into the Virgin Media modem in modem mode so there's no NAT going on or anything.
[1368.28 --> 1374.04]  So the ThinkPad itself has a WAN IP address so you don't want to do that for very long on a Windows machine.
[1374.90 --> 1387.50]  And then I'm connected via TeamViewer into his laptop doing the install of OpenSense through PuTTY in a console session which went flawlessly.
[1387.76 --> 1390.12]  It took about 20 minutes to install OpenSense.
[1390.20 --> 1390.94]  That was no big deal.
[1390.94 --> 1393.22]  And then the moment of truth comes.
[1394.00 --> 1402.50]  You have to unplug the laptop and plug the firewall in in the correct order and trying to make sure that the WAN port was connected to what it was before.
[1402.74 --> 1405.00]  And there's just a lot of stuff that could go wrong.
[1405.62 --> 1410.78]  And there's just that puckering moment where you're like, right, disconnect it.
[1411.00 --> 1411.90]  Go on, just try.
[1412.14 --> 1413.40]  And then pray.
[1413.64 --> 1415.10]  You just pray that there's internet.
[1415.10 --> 1419.58]  And there was this horrible five minutes where he wasn't getting a WAN IP address.
[1420.16 --> 1430.30]  He was getting a 192.168.100.10, which I think means that the Virgin modem hadn't detected that the Mac had changed or something.
[1430.46 --> 1435.58]  So I got him to power cycle the Virgin Media modem and it worked.
[1436.86 --> 1436.94]  Wow.
[1437.58 --> 1438.06]  Wow.
[1438.06 --> 1444.78]  It would have been incredible if you could have had like a camera and, you know, Telegram, like you were saying.
[1444.90 --> 1449.80]  Like that would have made it so much simpler because you could have at least exchanged pictures of what was on the screen.
[1450.26 --> 1450.62]  Yes.
[1451.14 --> 1451.46]  Yep.
[1451.62 --> 1459.12]  It reminds me of a project I heard once that was a Python script that would take SSH commands in over SMS.
[1459.42 --> 1462.64]  So you couldn't interact with it, but you could send commands over SMS.
[1462.64 --> 1462.82]  Yes.
[1463.54 --> 1468.36]  My old UK server that I didn't bring with me when I emigrated is at my dad's house.
[1468.46 --> 1474.14]  And that's, I power it on once or twice a week, do my ZFS remote replication backup and turn it off.
[1474.56 --> 1477.20]  Now I do that over a WireGuard VPN site to site.
[1477.28 --> 1478.70]  So it's even better than before.
[1479.60 --> 1481.30]  But yeah, I don't know.
[1481.32 --> 1484.18]  There's got to be some way of doing a backup like that.
[1484.30 --> 1487.32]  But in reality, how often are you reinstalling a firewall?
[1487.96 --> 1489.32]  Well, in this case, would it have helped, right?
[1489.48 --> 1491.82]  Because you were taking out the internet connection.
[1491.82 --> 1503.54]  So even if you had some sort of remote management card in that server, or you had a second PC there that you could get a complete remote desktop session, it would have been disconnected when you took down the firewall.
[1503.86 --> 1504.06]  True.
[1504.28 --> 1504.46]  Yeah.
[1504.56 --> 1506.56]  I need a backup internet connection.
[1506.66 --> 1507.24]  That's what I need.
[1507.86 --> 1509.90]  You know what you need is a modem.
[1510.00 --> 1511.64]  Just a good old dial-up modem.
[1512.00 --> 1512.74]  Yeah, maybe.
[1513.16 --> 1513.36]  Maybe.
[1513.44 --> 1516.20]  It actually would have worked in this case since you're just dealing with a serial console.
[1516.20 --> 1523.58]  But that was, as ridiculous as it sounds, back in the day, what we did, what I had to do.
[1524.20 --> 1528.34]  I would have clients that had really serious business.
[1528.34 --> 1531.36]  Like they have to transfer medical records on this particular hour.
[1531.36 --> 1536.86]  And they had a T1 line, which was 1.5 megabits, I think.
[1537.06 --> 1539.86]  And it was $1,000 a month.
[1539.96 --> 1541.04]  And it would go out.
[1541.20 --> 1542.22]  It would go out.
[1542.34 --> 1543.18]  That is painful.
[1543.88 --> 1546.42]  And their backup was a 56K modem.
[1547.10 --> 1548.54]  It was actually sufficient.
[1548.66 --> 1549.34]  It was just slower.
[1549.34 --> 1552.44]  But the T1 was supposed to be for reliability.
[1553.18 --> 1562.28]  And I remember just thinking how funny it was because we had these procedures where after the transfer was done, the office lady would go around and unplug the phone from the back of the modem.
[1562.52 --> 1567.34]  And then like an hour before the procedure was to start, she'd go up to it and plug the modem back in.
[1568.06 --> 1569.92]  And that was the security control.
[1570.66 --> 1572.38]  I worked for a hotel for a little while.
[1572.38 --> 1579.18]  And I remember the night management manual had in it, you have to go and replace the tapes in the backup server.
[1579.30 --> 1580.12]  And I just...
[1580.12 --> 1580.44]  Oh, yeah.
[1581.20 --> 1583.24]  We had people that shared that job.
[1583.62 --> 1584.44]  It was their...
[1584.44 --> 1585.42]  They were on tape duty.
[1585.60 --> 1587.98]  And they'd had to drive it down to the alternative location.
[1588.32 --> 1589.76]  Rotate the tapes and drive it down.
[1590.12 --> 1590.44]  Crazy.
[1591.44 --> 1599.70]  So talking of backups and stuff like that briefly, one of the coolest features I discovered in OpenSense, besides the native WireGuard support,
[1599.70 --> 1603.92]  is you can back up your config files natively to Nextcloud.
[1604.40 --> 1605.28]  Well, I'll be dipped.
[1605.36 --> 1606.36]  It sends it to Nextcloud.
[1606.46 --> 1607.66]  Have you seen how large it is?
[1607.68 --> 1609.32]  It must be pretty small, right?
[1609.62 --> 1611.04]  It's a few kilobytes of XML.
[1611.22 --> 1611.98]  Let me go and have a look.
[1612.30 --> 1616.18]  You could just run that forever then and never have to worry about eating up your space.
[1616.24 --> 1616.88]  That's great.
[1616.88 --> 1618.70]  It versions it every day.
[1618.84 --> 1627.00]  So the file names have, you know, config firewall.ktz-datestamp timestamp at 1am.
[1627.62 --> 1629.78]  It's 120 kilobytes every day.
[1629.92 --> 1631.44]  So I think I can probably swing that.
[1631.80 --> 1634.46]  Now, do you have that pointed at another backup, Alex?
[1634.88 --> 1635.76]  One is none.
[1636.22 --> 1638.74]  Yes, but it's already my firewall backup.
[1638.96 --> 1643.28]  I mean, do I need to back that up more?
[1643.36 --> 1643.68]  I don't know.
[1643.74 --> 1644.34]  I don't think so.
[1644.34 --> 1649.52]  No, I just, as the guy who recently deleted some data, I have to, like, give you a hard time.
[1650.16 --> 1651.02]  Yeah, it's my job now.
[1651.02 --> 1663.04]  Yeah, well, I actually think having lost most of the previous weekend, actually previous week, to getting the site-to-site VPN working, I am going to make sure I back this up with my life.
[1663.22 --> 1663.46]  Right.
[1663.46 --> 1670.64]  Because the OpenSense documentation, God love it, particularly the bit for WireGuard, was about two years old.
[1671.30 --> 1676.92]  And so a lot of it was kind of in the right ballpark, but didn't really work properly.
[1677.44 --> 1680.46]  The site-to-site VPN thing is still old.
[1680.52 --> 1681.54]  So I'm going to rewrite that.
[1681.68 --> 1686.10]  But I've rewritten the man page for OpenSense and WireGuard.
[1686.10 --> 1692.90]  And that was merged this week, so it was one of my first proper, like, major open source documentation contributions.
[1693.34 --> 1693.98]  No kidding?
[1694.22 --> 1695.24]  You didn't tell me that.
[1695.44 --> 1696.80]  I'm really pleased with that one.
[1697.22 --> 1704.38]  That's a solid contribution, too, because I was sort of turned off from OpenSense when I reviewed that.
[1704.62 --> 1706.88]  And I thought, this looks really out of date.
[1706.98 --> 1708.92]  Maybe it isn't complete.
[1709.20 --> 1711.40]  Maybe it's not very good.
[1711.42 --> 1712.98]  And I kind of just moved on.
[1713.30 --> 1714.08]  I'm not joking.
[1714.08 --> 1716.26]  It wasn't complete, and it wasn't very good.
[1716.62 --> 1717.32]  So, yeah.
[1718.04 --> 1718.48]  Wow.
[1718.64 --> 1719.24]  That's so great.
[1719.42 --> 1720.42]  Hopefully the new one is there.
[1720.56 --> 1723.20]  And I just want to underscore that point to people.
[1723.66 --> 1729.98]  Anybody that's listening that's wondering how they get started with contributing to open source, there are many, many ways you can do it.
[1730.10 --> 1733.72]  Code is just one, and arguably one of the least important ways.
[1734.02 --> 1735.56]  I mean, obviously, without code, there's nothing.
[1735.74 --> 1740.24]  But somebody said to me on Discord earlier when I pointed at the pull request that they were like,
[1740.24 --> 1747.40]  oh, that's really cool, because when I'm maintaining a project and I'm the guy that knows the intricacies of this particular plugin,
[1747.78 --> 1753.40]  the last thing I want to be doing is fielding user requests about the baby stuff, the basics.
[1753.74 --> 1753.80]  Right.
[1753.80 --> 1756.66]  And equally, I don't want to be writing that stuff either.
[1756.82 --> 1765.36]  You know, I would rather that it was someone like you came along and did a good job, you know, writing the documentation that frees me up to do what I'm good at.
[1765.82 --> 1769.66]  And I hadn't really thought of it quite so clearly as that, so concisely as that.
[1769.66 --> 1776.96]  Yeah, it has a real benefit long term because it means less questions, which means that developer is saving time.
[1777.46 --> 1778.20]  That's huge, really.
[1778.58 --> 1782.12]  Yeah, so I found that the whole merge process only took a few days.
[1782.28 --> 1788.02]  So for those of you that aren't, you know, on GitHub all day every day for your day job, the process is really straightforward.
[1788.54 --> 1791.88]  You go to the repo that you want to contribute to.
[1792.14 --> 1794.76]  So in this case, it's the OpenSense docs repo.
[1794.76 --> 1806.48]  You press the fork button up in the top right hand corner, which then creates a full copy, a snapshot effectively, of that Git repo at that moment in time under your username.
[1807.34 --> 1811.86]  You're then free to make all the changes in the world that you want for as long as you want.
[1812.56 --> 1820.68]  If it's a particularly busy repo, try not to make it more than a few days because otherwise things will get out of sync and you'll have to have resolved merge conflicts.
[1820.68 --> 1824.86]  But in this case, there's not very much churn in the OpenSense docs repo.
[1825.08 --> 1830.08]  So it was on my computer for like a week and that was no problem.
[1830.36 --> 1836.88]  So once I'd finished writing the article, the next thing that I did was I opened what's called a pull request.
[1837.80 --> 1840.30]  Merge request, pull request, they kind of mean the same thing.
[1840.72 --> 1841.70]  It's just semantics.
[1841.70 --> 1853.56]  And what that does is it asks permission of the OpenSense repo owner's permission to say, this guy, ironic badger, wants to make these changes to your repo.
[1853.66 --> 1854.16]  Is that OK?
[1854.82 --> 1858.98]  And we had a little bit of back and forth about some of the wording and a few tweaks here and there.
[1859.30 --> 1861.24]  And I made a few changes based on his comments.
[1861.92 --> 1863.88]  And after a few days, wouldn't you know it?
[1864.40 --> 1864.74]  Merged.
[1865.06 --> 1866.00]  And that's it.
[1866.08 --> 1867.50]  You're a contributor to open source.
[1867.64 --> 1868.42]  It's as simple as that.
[1868.42 --> 1873.24]  This really makes me appreciate an aspect of self-hosting that we've never really touched on.
[1873.82 --> 1882.52]  And that is you can actually make a difference on the projects in a way that is maybe even not code related.
[1882.74 --> 1885.22]  And it benefits more self-hosters.
[1885.48 --> 1887.24]  And it makes what you use better.
[1887.80 --> 1895.08]  That's just an opportunity you don't have when you use a service that's hosted, say, on Google's cloud or Apple's cloud or whatever it might be.
[1895.08 --> 1898.66]  There's just no opportunity for you to have any voice there.
[1898.80 --> 1900.60]  You have no impact on its direction.
[1900.90 --> 1907.40]  And almost all the software that we run on our servers for self-hosting stuff is open source.
[1907.76 --> 1908.90]  It's free software.
[1909.16 --> 1910.90]  And you can actually make a difference.
[1911.12 --> 1913.70]  That's a big deal with self-hosting that we don't talk about much.
[1913.70 --> 1915.26]  It does feel scary.
[1915.88 --> 1929.50]  Even sat in this chair as a guy that has been, you know, working in DevOps now for five, six years, whatever it is, as my day job, I still got a little bit nervous when I pushed that merge request button, that pull request button.
[1929.80 --> 1931.90]  Because you're putting yourself out there.
[1931.96 --> 1933.30]  You're putting yourself out there for judgment.
[1933.58 --> 1935.90]  And sometimes people are going to say no.
[1935.90 --> 1941.20]  But in my experience in general, most people are just happy that somebody else is contributing.
[1941.38 --> 1944.76]  If it's a good quality contribution, then just go for it.
[1944.82 --> 1945.26]  Give it a go.
[1945.46 --> 1946.04]  What have you got to lose?
[1946.50 --> 1951.28]  There has to be more things like this that our community could have an impact with various self-hosted open source software.
[1951.44 --> 1953.94]  It's maybe something for further discussion down the road.
[1954.48 --> 1957.40]  Now, you're all about power monitoring and stuff like that, aren't you?
[1957.78 --> 1959.38]  I have been getting more and more into it.
[1959.40 --> 1959.60]  Yeah.
[1959.80 --> 1962.72]  I don't have a great solution now that's tied in with Home Assistant.
[1962.72 --> 1969.56]  I have a Victron system that has an app that gives me all kinds of data, but it just lives there.
[1970.06 --> 1972.32]  Now, I'm not going to go into the full details in this episode.
[1972.46 --> 1973.74]  We'll save it for a future episode.
[1974.26 --> 1988.84]  But I would like to draw our listeners' attention to a 100% open source hardware and software Raspberry Pi whole home power monitor project by user David00 over on Reddit.
[1989.34 --> 1989.82]  Okay.
[1990.18 --> 1992.02]  Well, this is starting to check some boxes.
[1992.72 --> 1993.12]  Yeah.
[1993.64 --> 1993.88]  Yeah.
[1994.04 --> 2000.24]  So, like I say, we are going to save the full reveal for this thing for probably a couple of episodes' time.
[2000.90 --> 2006.58]  But in the meantime, please check the show notes for the link to a flyer that David's put together.
[2007.12 --> 2009.32]  Now, we don't stand to make any money out of this, David or I.
[2009.38 --> 2011.50]  We're just trying to get together a group buy.
[2011.50 --> 2024.44]  So, the reason we're doing this is because there are, you know, a bunch of, you need to buy a few circuit boards, get some custom circuit boards made up, some fuses, a few components, nothing major, and some Raspberry Pis.
[2024.44 --> 2030.62]  And at the quantities that, you know, just one or two units would be, it's not really cost effective.
[2031.18 --> 2038.70]  But if we're able to get, you know, 50 to 100 people together that are interested in building these things, then it starts to make a lot more sense.
[2038.70 --> 2042.16]  And we're looking at sort of the $20 price range for a kit here.
[2042.40 --> 2053.98]  So, what this thing allows you to do is it allows you to monitor the energy going into and out of your house and then export that to a Telegraph Influx Grafana stack.
[2054.68 --> 2057.48]  And then, obviously, that will be compatible with Home Assistant as well.
[2058.04 --> 2060.66]  You can monitor up to six individual circuits.
[2060.66 --> 2066.90]  You can see in real time how much power they're using, you know, current, wattage, all that kind of stuff, and voltage.
[2067.62 --> 2075.16]  So, if you are at all interested in monitoring solar, it will also monitor inbound as well as outbound power.
[2075.44 --> 2077.82]  So, there's all sorts of different things you can do with this.
[2078.16 --> 2079.66]  I wonder if it would be compatible with my setup.
[2080.12 --> 2081.86]  I'm going to seriously look at this thing.
[2082.28 --> 2088.94]  Now, I think the next step for everybody is to, if you are at all interested in this project, take a look at the link in the show notes.
[2088.94 --> 2097.56]  And then, reach out to me on Twitter at Ironic Badger or self-hosted at jupiterbroadcasting.com on the email.
[2098.36 --> 2099.58]  And just let me know what you think.
[2099.68 --> 2107.64]  And if that $20 price point is of interest to you, if we get enough interest, we're going to put together a group buy probably and then get these things shipped out.
[2107.90 --> 2112.58]  And maybe we could come to some agreement because there is going to be some kind of soldering required.
[2112.58 --> 2119.24]  So, there is a slight downside, I'm sorry to say, that you might have to do some self, you know, some assembly.
[2120.10 --> 2123.22]  But I think it's a good starter project for a lot of people.
[2123.68 --> 2128.88]  And there isn't really much else like it out there on the market in that similar price bracket.
[2129.20 --> 2130.04]  It looks pretty cool.
[2130.14 --> 2135.28]  So, the idea is that it's a tool that will give you real-time information on your power consumption.
[2135.96 --> 2137.06]  Solar is on here too.
[2137.66 --> 2138.46]  Generator status.
[2138.58 --> 2139.30]  That's awesome.
[2139.30 --> 2140.56]  That's exactly what I need.
[2140.96 --> 2142.94]  And monitor six individual circuits.
[2143.06 --> 2145.04]  So, that's, I wonder how that would work for me.
[2145.60 --> 2145.80]  Huh.
[2146.26 --> 2147.24]  This is pretty neat.
[2147.68 --> 2149.40]  The PDF is pretty cool.
[2149.90 --> 2154.60]  The way that you monitor the actual current usage is you use what's called a CT clamp.
[2154.98 --> 2157.36]  And that basically just clips over the cable.
[2157.98 --> 2162.92]  So, there's an electrical field generated as current flows through a cable.
[2163.16 --> 2166.98]  And what these CT clamps are able to do is measure that somehow.
[2166.98 --> 2169.00]  I think that's just incredible.
[2169.30 --> 2172.06]  You don't need to splice into the cables or anything like that.
[2172.52 --> 2175.30]  And what these CT clamps generate is a very small voltage.
[2175.44 --> 2177.20]  Somewhere between zero and one volts.
[2177.84 --> 2183.76]  And then there's an integrated controller chip that reads that value and interprets that to say,
[2183.90 --> 2186.32]  okay, well, that means there's three amps flowing at this voltage.
[2186.76 --> 2188.54]  Therefore, you're using this number of watts.
[2189.34 --> 2190.62]  Super simple to do.
[2190.86 --> 2192.90]  And hopefully, we can get some interest.
[2193.58 --> 2193.66]  Yeah.
[2193.76 --> 2196.20]  So, it's not very invasive to set it up, what it sounds like.
[2196.32 --> 2196.76]  No, no.
[2196.76 --> 2202.06]  And then the software to actually do all the data collection and whatnot is also open source.
[2202.36 --> 2203.16]  It's a cool little project.
[2203.26 --> 2204.00]  You can put me down.
[2204.26 --> 2204.78]  Put me down.
[2205.12 --> 2205.40]  All right.
[2205.94 --> 2206.80]  I thought you'd be interested.
[2207.30 --> 2208.08]  Yeah, I like it.
[2208.08 --> 2209.54]  Looking at the GitHub project, too.
[2209.56 --> 2211.10]  I like what I see up there as well.
[2211.38 --> 2213.46]  We'll put links to all that stuff in the show notes.
[2213.84 --> 2215.48]  And yeah, please let me know if you're interested.
[2215.48 --> 2217.54]  Yeah, I could always use another Raspberry Pi.
[2217.84 --> 2218.80]  No, what have I done?
[2219.44 --> 2220.58]  This one's on you, too.
[2220.98 --> 2225.98]  You know, what's funny, too, is the RV might be in good shape now heat-wise, but now the
[2225.98 --> 2230.98]  studio heats up because the afternoon where we have the studio server is in the garage
[2230.98 --> 2234.24]  and the sunlight just bakes that garage in the afternoon.
[2234.24 --> 2237.84]  So it's about 92 degrees out there right now.
[2237.90 --> 2240.30]  And I went out and set up one of those portable air conditioners.
[2240.46 --> 2242.88]  So from the fire into the frying pan, Alex.
[2243.38 --> 2243.78]  Always.
[2244.04 --> 2244.76]  Always the way.
[2245.14 --> 2250.38]  Well, before we officially end Self-Hosted 24, I'll mention the contact page, self-hosted.show
[2250.38 --> 2251.34]  slash contact.
[2251.62 --> 2255.54]  And while I'm on a roll, self-hosted.show slash discord for the community.
[2255.88 --> 2257.90]  And so, yeah, please do go and check out the discord.
[2258.02 --> 2259.04]  It's hopping these days.
[2259.08 --> 2260.94]  We've got nearly 1,500 members.
[2260.94 --> 2262.84]  It's getting pretty crazy over there.
[2263.56 --> 2265.12]  So thanks very much for listening, everyone.
[2265.44 --> 2266.86]  That was Self-Hosted 24.
