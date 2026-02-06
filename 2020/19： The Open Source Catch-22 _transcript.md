[0.00 --> 5.10]  Coming up on this week's show, we talk through how too much automation can sometimes be a bad thing.
[5.86 --> 11.88]  Chris has a mini Home Assistant freakout and continues to collect Raspberry Pis at, frankly, an alarming rate.
[12.40 --> 12.92]  I'm Alex.
[13.38 --> 15.80]  I'm Chris, and this is Self-Hosted19.
[16.92 --> 18.78]  I bought another Raspberry Pi 4.
[19.18 --> 19.68]  Uh-oh.
[20.36 --> 20.66]  Yeah.
[21.32 --> 28.94]  I just wanted a test rig that I could do some experiments with without affecting my production Raspberry Pis.
[28.94 --> 32.96]  You know, the number on the end of the model name is not the number you're supposed to own.
[33.46 --> 36.30]  Good, because I think this is my sixth, maybe.
[37.60 --> 39.22]  Your sixth Raspberry Pi 4?
[39.56 --> 40.46]  I think it might be.
[40.60 --> 41.78]  Oh, dude, you have a problem.
[42.18 --> 43.76]  The Self-HostedDiscord, I blame them.
[43.82 --> 48.96]  They've been asking me questions, and I was like, you know, I want to test this for these guys, but I don't want to do it on my production system.
[49.76 --> 50.34]  So it's their fault.
[50.88 --> 51.20]  Production.
[51.88 --> 52.78]  Oh, you're so cute.
[53.80 --> 54.72]  No, it is.
[54.80 --> 57.38]  They're server-grade Pis, and don't you forget it.
[57.38 --> 59.04]  Mmm, sound delicious.
[59.30 --> 60.18]  Server-grade Pis.
[60.30 --> 61.46]  That should be the title right there.
[61.66 --> 62.40]  Does sound delicious.
[62.70 --> 72.46]  The thing that the Discord's been asking me is, once you move your system over to the USB SSD, that's kind of a funny saying, a lot of acronyms there.
[73.10 --> 79.50]  But once you move over to that SSD that's on USB, and you boot from it, is the SD card still required?
[79.50 --> 94.38]  This is a frequent question that's come in, because the performance improvements by doing this, where you take the Raspberry Pi 4 image for, say, like Ubuntu 2004, and then you flash that to a USB SSD drive, like you would an SD card.
[94.38 --> 96.20]  You can actually boot from that.
[96.70 --> 105.54]  But after some testing today, with this new Raspberry Pi, I realized you absolutely still have to have, in this current setup, the SD card in there to load the kernel.
[105.88 --> 110.94]  So the SD card is just necessary for the very, very early stages of the boot process.
[111.36 --> 117.70]  Once the kernel is loaded, it switches over to your external SSD drive, and everything runs from that.
[117.80 --> 120.34]  And you, in theory, could probably remove the SD card.
[120.34 --> 124.68]  Yeah, slash boot has to remain on the SD card.
[124.90 --> 127.70]  You can work around that with a Pixie boot if you want to.
[127.76 --> 133.44]  So you could network boot the Pi's completely SD card-less if you really wanted to.
[133.56 --> 134.44]  So another option.
[134.98 --> 135.14]  Yeah.
[135.40 --> 143.02]  I mean, I find it to be a pretty good compromise, though, Alex, because it's only using the SD card for a very short amount of time when the system's booting.
[143.10 --> 144.90]  And then after that, it doesn't even touch it.
[144.90 --> 149.18]  It's not making any rights to it unless you're doing kernel upgrades.
[149.18 --> 156.68]  So I guess the only time at which you'd be at risk is when you're actually writing data to the SD card of it failing.
[157.34 --> 164.54]  Yeah, and that's such a simple setup that it's no problem to just DD that to another SD card as a hot standby every now and then.
[165.10 --> 166.24]  And it doesn't need to be a big one.
[166.54 --> 171.58]  So how do you go about migrating the root file system from the SD card to the SSD?
[171.84 --> 173.38]  Is it rsync or what?
[173.50 --> 173.90]  How do you do it?
[173.90 --> 174.90]  No, it's even simpler.
[175.02 --> 180.54]  You just write the image that you would have written to the SD card to the USB drive, to the SSD.
[181.16 --> 185.52]  What happens if the kernel gets out of sync with what's in slash boot and what's on the image?
[185.98 --> 192.14]  This is where you have to take careful precautions to mount the right boot and have that so you're updating the right slash boot.
[192.42 --> 193.34]  Okay, that makes sense.
[193.56 --> 195.66]  Once it's done, you get pretty spectacular performance.
[195.66 --> 200.32]  It's about the best performance you're going to get on a Raspberry Pi 4 without overclocking it.
[200.32 --> 202.02]  They are the little boxes that can.
[202.26 --> 203.44]  I've mentioned it before.
[203.54 --> 208.52]  My 3D printer has been running a Pi 3B Plus for the last year plus.
[208.94 --> 209.82]  It just works.
[209.92 --> 211.26]  And it's been running from an SD card.
[211.38 --> 215.40]  So I really shouldn't worry too much about deploying to production with an SD card.
[215.52 --> 218.18]  But the right performance from an SSD is pretty great.
[219.20 --> 220.62]  It's hard to argue with that.
[220.96 --> 225.94]  Now, Home Assistant, should we talk about that and the drama this week?
[226.34 --> 229.92]  Yeah, because this honestly would invalidate my entire setup if this had gone through.
[230.32 --> 237.36]  I really took this hard when they announced that they were deprecating the supervised mode of Home Assistant on generic Linux.
[237.54 --> 242.76]  Well, before we get to explaining the nitty gritty of supervised and everything else,
[242.96 --> 251.74]  I think it's worth stating that Home Assistant lately have been on somewhat of a crusade to change things and do rebranding,
[252.26 --> 255.58]  kind of redefining their relationship as a project with the community.
[255.58 --> 261.88]  We had a few weeks ago a situation where they were doing a bunch of stuff around YAML in the UI,
[262.42 --> 269.08]  kind of taking away or abstracting away a lot of the YAML controls into just click-click UI-based stuff.
[269.44 --> 274.78]  And then that led to a whole series of blog posts and an episode of the Home Assistant podcast dedicated to it.
[274.78 --> 276.28]  And now we have this.
[276.50 --> 277.74]  So, I don't know.
[277.76 --> 280.46]  There's a few things happened and let's break it down.
[280.62 --> 288.54]  So, you have Home Assistant, which is a combination of Home Assistant Core and Supervised DE,
[288.70 --> 294.18]  which manages a lot of things for Home Assistant, keeps it up to date, allows you to take snapshots,
[294.26 --> 295.76]  it allows you to install add-ons.
[296.22 --> 297.88]  We've talked about that on the show before.
[297.88 --> 299.46]  So, that's Home Assistant.
[300.00 --> 304.24]  Home Assistant Core is just the base functional part of Home Assistant.
[304.48 --> 307.68]  You can get that as a Docker image on any Linux box today.
[308.46 --> 314.60]  And then you have the whole OS that they provide as an image that you can deploy to Raspberry Pis or in a VM.
[315.50 --> 319.54]  And the bit that they were deprecating, which they have now revised their plans,
[319.66 --> 325.00]  but when announced, the bit they were deprecating was the ability to install the overall Home Assistant package
[325.00 --> 328.80]  that includes Core and Supervised DE on any Linux box.
[329.30 --> 333.38]  If you wanted Home Assistant on Linux, you could only get the core version.
[333.72 --> 339.70]  No plugins, no themes, no community add-ons, no Supervised DE to do the backups and the updates,
[340.40 --> 343.56]  just the Docker image of just the core Python application.
[344.10 --> 348.78]  Or you had to grab their pre-built image that includes an entire Linux OS.
[349.28 --> 352.12]  I think one of the things that wound me up a little bit about this announcement
[352.12 --> 359.24]  wasn't the announcement itself because open source projects are generally created by people volunteering their time.
[359.34 --> 364.74]  And if the project goes in a way I don't like, then I'm perfectly within my rights to fork it.
[365.36 --> 369.50]  But this time, Home Assistant is turning into a company.
[370.00 --> 373.84]  So, we've got this Nabu Kasa company who have been founded in the last year.
[373.84 --> 377.42]  They've hired a few people, Frank being one of them,
[378.02 --> 380.30]  Paulus, you know, the founder of Home Assistant is another.
[380.46 --> 384.08]  There's a few other actual staff working on Home Assistant now.
[384.80 --> 389.72]  And so, it's kind of going through growing pains of transitioning from a free and open source project
[389.72 --> 393.94]  entirely built off voluntary, you know, time donations
[393.94 --> 398.48]  to being almost like a pseudo product in a way.
[398.48 --> 403.56]  One of the key arguments in the blog post was developers' health.
[404.34 --> 408.16]  And there was a line in there which just rubbed me up the wrong way.
[408.84 --> 412.42]  I know that this blog post will make a subset of our community angry.
[413.00 --> 416.28]  There are people that think they deserve other people's work,
[416.66 --> 418.78]  even if it costs them their health.
[419.36 --> 420.08]  You're wrong.
[420.90 --> 425.08]  Just as with our recent decision to limit the usage of YAML in some cases,
[425.88 --> 428.30]  Home Assistant will keep choosing health over features.
[429.10 --> 434.84]  Open source is not about us having to support every feature anyone on the internet can think of.
[435.42 --> 439.82]  Open source means that anyone can do that themselves and choose to share this or not.
[440.48 --> 448.06]  Now, that paragraph with the you're wrong section has since been removed from the blog post entirely.
[448.40 --> 452.16]  And for me, that's kind of a tacit, you know, a tacit agreement that,
[452.56 --> 456.18]  yeah, okay, perhaps we were a bit almost rude in that one.
[456.18 --> 459.40]  It feels like it's coming from a place of burnout, doesn't it?
[459.90 --> 460.10]  Yeah.
[460.28 --> 463.54]  And there was a comment, this was on Reddit.
[463.66 --> 466.62]  I mean, there was a huge, huge number of comments on Reddit about this,
[467.56 --> 472.24]  saying that users are basically coming from a place of entitlement.
[472.24 --> 480.80]  But actually, if you think about it, the developers saying that the users are entitled is itself an entitled position.
[480.80 --> 492.92]  And I find it interesting how this happens with open source all the time, that as project gains traction, the reason that it gained popularity was because it is what it was.
[492.92 --> 496.16]  And then if you take things away from it, it no longer is what it was.
[496.20 --> 500.08]  So, of course, people are going to be upset because they've built their lives around this thing.
[500.78 --> 504.24]  We're both, Chris and I, are feeling a bit locked in to Home Assistant these days.
[504.78 --> 504.86]  All right.
[504.88 --> 506.30]  Well, let's zoom in on this for a moment.
[506.36 --> 512.84]  Because what I find interesting here is you have the burnout, you have the entitlement story that's quite common in the open source world.
[512.84 --> 516.16]  And then you also have this mismatch with user expectations.
[516.72 --> 523.38]  And in this case, which is not always true in these situations, but in this case, the end users might be right.
[523.98 --> 533.84]  From a security standpoint, I think you could make a pretty solid argument that if you have experienced system administrators who are deploying common operating systems with multiple years of support
[533.84 --> 545.98]  and a standardized way to patch and monitor the vulnerabilities on those systems, those are probably likely more secure than Home Assistant's custom-built OS, no matter how minimal it is.
[545.98 --> 558.28]  Because the reality is a group like Canonical or Red Hat has entire teams of engineers just dedicated to building a production-grade operating system.
[558.28 --> 566.68]  Nebukasa has a couple of guys who are making a massive, huge project that needs an OS to run on top of.
[566.90 --> 568.94]  The OS isn't their primary focus.
[569.16 --> 576.66]  As a longtime system administrator who runs all of my own systems now, I don't want to run somebody else's operating system.
[576.88 --> 584.90]  I want to run what is my standard deployment that I know how to maintain, patch, reproduce, backup, restore, etc.
[585.92 --> 587.90]  I don't want somebody else's custom OS.
[588.28 --> 592.10]  I want that kind of stuff out of my infrastructure as much as possible, actually.
[592.90 --> 599.94]  So there was a mismatch with what the end users wanted and expected, and potentially what looks like might be the widely deployed scenario,
[600.32 --> 605.46]  versus what the developers want, perhaps from a product standpoint and simplified development perspective.
[605.80 --> 610.80]  And I think this is a classic mismatch that we have here, only this time it's really complicated,
[610.80 --> 617.36]  because it does mean that Home Assistant was nearly about to make a change that would completely invalidate my setup.
[617.36 --> 631.10]  And I had one of those moments where I felt just as locked in to Home Assistant as I would any other cloud service or any kind of smart things central hub that has a subscription or has a license.
[631.10 --> 639.24]  I felt caught in a trap because I was being told that my setup was deprecated and there were no plans to support it.
[639.24 --> 646.94]  And sorry, if you want to keep running it on your own OS, then you better switch back to Core, which listeners of the show will note I just migrated from.
[646.94 --> 648.96]  So the timing on this was horrible.
[649.24 --> 651.82]  And I realized, well, I've just done it again.
[651.94 --> 654.20]  Only this time I've spent all the money on the hardware.
[654.42 --> 656.40]  I've spent all the hours setting it up myself.
[656.54 --> 658.04]  And now I'm just as locked in.
[658.62 --> 662.78]  What's wrong with them saying in that scenario, sorry, Chris, we're not going to support you.
[663.42 --> 665.00]  We'll still leave supervisor there.
[665.06 --> 666.14]  We'll still maintain it.
[666.50 --> 672.08]  But if you get into a situation that you can't fix, well, you're on your own.
[672.12 --> 673.64]  I mean, that's kind of the Linux way, isn't it?
[673.64 --> 685.54]  I think there is a scenario where they would set a timeline, a 90-day window or something, where they would inform users that at this point, this will no longer be a supported deployment methodology.
[685.80 --> 691.30]  And in that 90-day period, there would be a call to action to create documentation to help users.
[691.30 --> 706.24]  Because that was, I think, the thing that really pushed this over the edge and made them roll this back is they realized very quickly there was a massive lack in documentation to actually support the way they were telling people to deploy it now.
[706.78 --> 710.10]  And the user base was rightfully upset about that.
[710.40 --> 712.24]  You just told me to go use this new method.
[712.40 --> 715.86]  And the documentation is out of date and wrong in some cases.
[715.86 --> 718.02]  And so they had to reverse course.
[718.24 --> 722.08]  But I think if you had set a timeline, maybe it could be as short as 90 days.
[722.40 --> 726.02]  If you had made a good case for it, maybe had a call for support.
[726.08 --> 731.32]  Because, again, this is an open source project and people don't know to help until you ask for it.
[731.34 --> 737.40]  As silly as that sounds to the people making it, the consumers of the product are not aware of the day-to-day strife.
[737.50 --> 740.06]  They don't know where help is needed unless you tell them.
[740.06 --> 745.24]  That's why whenever we have developers on this show or our other shows, we always say, how can people help?
[745.30 --> 745.92]  They don't know.
[746.58 --> 752.50]  So communicating that initially, even before it came to this, if you were to rewind the clock, would be the first step.
[752.64 --> 754.36]  Then setting a timeline to migration.
[754.76 --> 757.40]  And then updating the docs and improving them in the short term.
[758.26 --> 761.06]  If you have to make the change, there is a way to do it.
[761.12 --> 768.60]  I still wouldn't have been thrilled, but it wouldn't have been this immediate pulling the rug out from underneath me saying it's already deprecated as of this post.
[768.60 --> 770.96]  And so who are these changes aimed at?
[771.28 --> 780.62]  It feels to me like Home Assistant is trying to pivot into this new friendly, new user, mythical new Linux user friendly product.
[780.82 --> 781.90]  Who are these people?
[782.32 --> 783.38]  Yeah, deployed on your Pi.
[783.54 --> 791.78]  It seems like they're targeting the people that have bought small board computers or perhaps they are targeting a product themselves.
[791.78 --> 800.88]  That was a sense I got from this is maybe if they're going to make a Home Assistant hardware device one day, it will need its own OS.
[801.28 --> 806.18]  And so if they're going to work towards that, that would be a logical focus of their resources.
[806.18 --> 809.30]  This is a point I made in the Linux spotlight that I did with Rocco.
[809.86 --> 818.00]  I think more people come to Linux these days through headless server apps like Home Assistant or Plex and whatever than they actually do through the desktop.
[818.76 --> 820.72]  Linux is dominant on the server side.
[820.72 --> 828.20]  And it feels to me like Home Assistant is leveraging that kind of Linux ecosystem to get them off the ground.
[828.20 --> 829.94]  And they've built up this reputation now.
[830.44 --> 835.18]  And they're trying to abstract away a lot of stuff that made it great.
[835.40 --> 842.78]  You know, declarative configuration through YAML files is being abstracted away a little bit to, you know, the UI.
[842.78 --> 853.66]  And with this supervised D change, OK, it's been rolled back, but it just feels like another screw that's being turned to make it a black box and appliance that can be productized.
[854.30 --> 855.34]  Yeah, it could go that way.
[855.66 --> 858.94]  I hope not, because I think your analysis is correct.
[859.40 --> 864.80]  A lot of early adopters of Home Assistant pip installed it because it was a pip install away.
[865.16 --> 869.72]  And then the next wave came and it was Docker users that installed the containers.
[869.72 --> 879.96]  And now I think the area they're focused on, like some of their primary developers even for their main Home Assistant setups, are using things like the Odroid or Raspberry Pis.
[880.70 --> 883.64]  Or they're recommending people go buy a NUC and deploy their image on it.
[884.10 --> 887.28]  Yeah, so it's a worrying time for the Home Assistant project in general.
[887.60 --> 892.12]  I don't know what this means for the future, because officially nothing's changed at this point.
[892.50 --> 895.96]  But you've got to imagine that something somewhere is going to give at some point.
[895.96 --> 904.78]  And whether it's the developer's health being used as an excuse, I'm not saying that people should work themselves into the ground for my benefit, you know, for free.
[904.96 --> 909.16]  But at some point, you know, I'm paying Nabu Casa five bucks a month.
[909.42 --> 912.26]  I've submitted a couple of pull requests to Home Assistant.
[912.76 --> 913.94]  I've been on their podcast.
[914.46 --> 917.62]  And I've still got told by people on Reddit that I didn't qualify to have an opinion.
[918.10 --> 923.08]  You know, at what point do the users qualify for that opinion?
[923.08 --> 925.00]  You know, I'm just worried.
[925.06 --> 930.28]  It's a red flag for me that maybe all is not well at the head of the project.
[930.80 --> 932.02]  I think it is a red flag.
[932.52 --> 939.92]  However, that flag is maybe not quite as bright red because they did dial it back, which means they're listening.
[940.68 --> 941.46]  And that's a good sign.
[941.72 --> 943.84]  It's more sort of burnt sienna now.
[944.18 --> 945.04]  Right, exactly.
[945.04 --> 948.68]  And that feels like, okay, there's room for negotiation here.
[948.70 --> 956.08]  And I think that's important because the community around Home Assistant, especially when it comes to integrations and whatnot, is super important.
[956.56 --> 960.78]  And building that up in a competitor will take, I mean, how long has Home Assistant been around?
[960.92 --> 961.20]  Years.
[961.54 --> 962.92]  It would take just as long, I think.
[963.24 --> 965.10]  So long live Home Assistant.
[965.10 --> 965.66]  Home Assistant.
[966.18 --> 975.12]  Yeah, although I'm sure people, and actually welcome, jump in the Discord at selfhosted.show slash Discord or send us an email at selfhosted.show slash contact.
[975.48 --> 977.72]  Are you using something besides Home Assistant?
[977.92 --> 978.80]  And how do you like it?
[978.84 --> 980.50]  Because there's commercial products out there.
[980.76 --> 982.66]  There's other open source projects.
[982.96 --> 984.10]  I'd like to hear from you.
[984.74 --> 988.62]  Now, in the last episode, I promised you a reverse proxy roundup.
[988.98 --> 990.36]  I don't have one for you today.
[990.44 --> 994.08]  But what I do have is a plug for the latest episode of TechSnap.
[994.08 --> 998.74]  That's episode 429 at TechSnap.Systems slash 429.
[999.00 --> 1003.60]  Yeah, in the meantime, since our last episode, Wes and Jim did a pretty nice overview.
[1004.08 --> 1007.32]  They were talking about Caddy, which just dropped version 2 recently.
[1007.84 --> 1011.98]  I've taken a little look at it, and I had a bit of a, you know, a Twitter exchange with a developer.
[1012.66 --> 1015.32]  I'll keep my opinion to myself on that one for now.
[1015.74 --> 1020.12]  I don't think I'll be switching away from my beloved Nginx quite yet, though.
[1020.50 --> 1022.50]  I'm still trying to get you to switch to traffic, so.
[1022.76 --> 1023.70]  Yeah, yeah.
[1023.70 --> 1028.80]  And talking of the Discord, I want to give a quick shout out to user Anther76.
[1029.34 --> 1037.18]  He has been really helpful in helping me figure out how to get past the host mode problem that I talked about in last episode with traffic.
[1037.64 --> 1044.02]  So there's a couple of lines you can add to your config of the traffic container, which is extra underscore hosts.
[1044.02 --> 1048.34]  And then you put in the IP address of your Docker network.
[1048.80 --> 1054.48]  And then by doing that, you can run Plex in host mode and use traffic as a full reverse proxy.
[1054.98 --> 1063.92]  There is an example, which I'll have a link to in the show notes, in my infrastructure GitHub repo of my example Docker Compose file that I'm just using to test stuff.
[1063.92 --> 1066.16]  So if you're curious, take a look in the show notes.
[1066.86 --> 1068.64]  And I just mentioned those contact methods.
[1068.76 --> 1072.82]  Those are also perfectly viable if you want us to go more into reverse proxies.
[1072.90 --> 1073.56]  Just let us know.
[1073.92 --> 1076.74]  We're just waiting for you to ask selfhosted.show slash contact.
[1076.96 --> 1080.04]  In the meantime, though, you didn't have a chance to play with something else.
[1080.04 --> 1088.06]  And they build themselves as your, quote, offline first privacy centric personal data center, HomeLab OS.
[1088.68 --> 1089.70]  So this is an interesting one.
[1089.80 --> 1095.64]  HomeLab OS proposes to be my favorite project of the year.
[1095.86 --> 1099.32]  If you think about all the technologies that are involved here, it's using Linux.
[1099.60 --> 1100.48]  It's using Ansible.
[1100.76 --> 1102.66]  It's written and configured in YAML.
[1103.02 --> 1107.42]  And it deploys lots of Docker containers and WireGuard.
[1107.78 --> 1109.60]  And magic happens.
[1109.60 --> 1110.04]  Yeah.
[1110.18 --> 1114.36]  And it claims over 100 click deploy services, easy backup and restores.
[1114.80 --> 1117.76]  And it will automatically publish it all on Tor hidden services.
[1118.00 --> 1121.30]  So you basically don't need to worry about port forwarding as long as you got Tor.
[1122.02 --> 1125.22]  And you get the whole thing up and running with one line deployment.
[1125.52 --> 1127.70]  I mean, this is like everything that would be checking your boxes.
[1128.54 --> 1129.92]  It largely does, to be fair.
[1130.06 --> 1131.04]  I mean, what are we talking here?
[1131.16 --> 1132.80]  Is it a script that you run on top of Linux?
[1133.30 --> 1136.84]  It's a framework, I suppose, is the best way I can think of to describe it.
[1136.84 --> 1140.48]  And largely speaking, that's my issue with it.
[1140.48 --> 1149.72]  It's using Terraform under the hood to create a Bastion server to make the magic happen about having a remote endpoint that you can target and a Bastion server.
[1149.84 --> 1151.18]  If you're familiar with that concept.
[1151.18 --> 1157.22]  It's something that you would connect to that is open to the internet without being your main box.
[1157.32 --> 1159.58]  It's like a jump post is another word for it you might hear.
[1160.22 --> 1163.74]  So you wouldn't connect directly to your server running on your LAN.
[1163.74 --> 1169.26]  And you'd go through the Bastion, which then your firewall knows what the public IP address of that is.
[1169.30 --> 1173.74]  So you can limit internet facing traffic to a very specific place.
[1174.84 --> 1179.62]  So in terms of security and basic protocols like that, it's a good thing to have.
[1179.64 --> 1180.84]  And it's pretty common in industry.
[1181.48 --> 1186.08]  And what's clear is that the developer of this project, Nick Busey, he really knows what he's doing.
[1186.08 --> 1194.20]  You know, I spent a good couple of days digging through the code here and he's using Ginger templating to template out all of the Docker Compose YAML files.
[1195.14 --> 1199.16]  And it's really, you know, must have been a lot of work to get to this point.
[1199.42 --> 1201.62]  And it supports hundreds of applications.
[1202.48 --> 1206.02]  But the trouble is, it wasn't invented here.
[1206.14 --> 1211.58]  And I don't mean that as a necessarily a bad thing, but it's so complicated.
[1211.58 --> 1221.24]  Even though I've spent months working as a consultant on Ansible code bases, it took me a good few hours to get my head around just what this thing was doing under the hood.
[1221.56 --> 1223.16]  Now, maybe that's not the point of this thing.
[1223.24 --> 1225.90]  Maybe I should just run the one line deploy and just go with it.
[1226.18 --> 1228.04]  But I like to know what things are doing under the hood.
[1228.12 --> 1232.30]  And it's so complicated and so abstracted away from what's actually happening under the hood.
[1232.84 --> 1237.28]  In the end, I ended up kind of being a bit turned off from it, sadly.
[1237.86 --> 1239.28]  That was my impression as well.
[1239.28 --> 1242.88]  So that's interesting because I thought we were going to have two different views on this.
[1243.70 --> 1246.20]  I don't need all of this.
[1246.20 --> 1255.20]  And I've kind of solved this in its own way for each one of these using, you know, Duplicati and other just backup systems.
[1255.44 --> 1262.62]  And having Docker containers where I've just hand deployed a handful of applications and I just managed it all from Compose files.
[1263.20 --> 1265.08]  I don't particularly need this anymore.
[1265.08 --> 1270.98]  But I do see it for somebody who is curious, like, hey, I got this box.
[1271.10 --> 1272.00]  I've heard about this Linux thing.
[1272.04 --> 1276.84]  I'll throw this Ubuntu on here and see how far I can get at replicating what I use the cloud for.
[1276.96 --> 1280.20]  I'll tell you where this thing I think actually is the most useful.
[1280.20 --> 1282.00]  It's for examples.
[1282.22 --> 1293.98]  It's for showing what's possible with automation and getting people involved in infrastructure as code and committing all of those configuration files to a Git repository somewhere.
[1293.98 --> 1302.62]  And so that when you're trying to do some kind of a server rebuild or, you know, save yourself writing bash scripts, which, you know, may or may not work.
[1302.70 --> 1307.70]  You're using Ansible, which is battle tested by Red Hat and millions of customers across the world.
[1308.32 --> 1312.10]  A lot of stuff that's in here is industry standard stuff.
[1312.10 --> 1321.56]  So if you can start looking at this sort of code base and understanding it and figuring out what it's doing, then, you know, you're pretty well set for, you know, a DevOps job.
[1322.24 --> 1322.72]  It's a good point.
[1322.98 --> 1325.00]  And it's a good example of what can be done.
[1325.58 --> 1327.34]  I mean, it's pretty neat to see something like this.
[1327.42 --> 1333.56]  That's not just the crazy like bash scripts or PHP command line scripts that are running, but it's actual.
[1334.08 --> 1339.06]  Well, I mean, it's a combination of bash scripts, but it's actual best practices being applied to assemble these systems for you.
[1339.44 --> 1340.38]  It's kind of neat to watch it.
[1340.38 --> 1343.50]  I've seen simpler code bases as part of government projects.
[1343.68 --> 1344.44]  Let's just put it that way.
[1345.20 --> 1347.90]  Yeah, it's not a great learning tool in that sense.
[1348.04 --> 1350.96]  That said, the developer behind it, Nick, is a great guy.
[1351.06 --> 1356.12]  He hangs out on our Discord and he quite often does Twitch live streams and stuff like that.
[1356.30 --> 1359.20]  And he's very open to feedback and stuff like that.
[1359.36 --> 1363.22]  I would say in general, he's a bit of a Steve Wozniak looking for a jobs.
[1363.92 --> 1370.02]  If you're, you know, willing to put some spit and polish and make it a little more consumable for mortals, then...
[1370.38 --> 1372.80]  You know, I think that's going to take the project to the next level.
[1372.96 --> 1374.60]  But for now, it's a bit much for me.
[1375.06 --> 1375.84]  I'll tell you what, though.
[1375.96 --> 1380.16]  I've made this point before on other shows, but I think it's something that's worth repeating.
[1380.38 --> 1384.56]  Is you do need projects like this to showcase open source and get it up and running.
[1384.56 --> 1391.16]  Because the barrier to running things like Nextcloud or your own mail server or a hosted Bitwarden installation, etc.
[1391.68 --> 1395.80]  Is sometimes you don't even know the fundamentals to install software on a Linux box.
[1396.54 --> 1398.90]  And you don't know if it's worth it to learn.
[1399.14 --> 1404.52]  And so when you can one-line deploy something and then have a UI to go through and deploy applications.
[1405.08 --> 1408.56]  And then experience things like setting up your own syncing or your own mail server.
[1408.56 --> 1412.08]  It can be a big motivator to learn and to go on a journey.
[1412.54 --> 1413.34]  You were touching on it.
[1413.42 --> 1418.56]  Like it's a validation or it's a way to prove out something before you begin a journey.
[1419.12 --> 1422.82]  And open source software, there's such a need for showcasing like that.
[1422.90 --> 1424.16]  So I like it from that standpoint, too.
[1424.68 --> 1431.44]  I think what I'd like to see really with this type of project is to separate out the constituent components into building blocks.
[1431.44 --> 1439.62]  So let's say I want to generate a Docker Compose file from a YAML dictionary full of different variables, for example.
[1440.46 --> 1444.92]  So I don't have to keep typing in the paths that I'm using for the Docker volumes.
[1445.12 --> 1450.12]  Or I don't want to expose my port numbers in my Git repo or whatever.
[1450.18 --> 1451.94]  So I can encrypt this kind of stuff, right?
[1452.18 --> 1452.46]  Right.
[1452.62 --> 1453.02]  Yep.
[1453.02 --> 1471.54]  If HomeLab OS was a series of, let's say, Ansible roles that you could consume and reuse different building blocks of that were written in a very generic, non-opinionated fashion, then I think this thing has huge, huge potential.
[1471.54 --> 1478.20]  But as it stands, I think the fact that it's got such strong opinions on the way things is done is great for it.
[1478.34 --> 1482.82]  But it means that it's very limited in terms of other use cases.
[1483.32 --> 1485.94]  But a cool project, and I definitely recommend trying it.
[1486.10 --> 1488.00]  You know, even if you just throw in a VM for a bit.
[1488.22 --> 1490.54]  But HomeLab OS will have a link in the show notes.
[1490.96 --> 1493.60]  I'm sorry I wasn't very nice, Nick, but I do like the project.
[1493.72 --> 1494.00]  Promise.
[1495.30 --> 1496.20]  Great job, though.
[1496.20 --> 1501.26]  I mean, if this is the work of a single individual, it makes me feel like I have not accomplished much in life.
[1501.54 --> 1502.14]  Yeah, right.
[1502.28 --> 1503.54]  What have you been doing with your life, Chris?
[1504.40 --> 1505.40]  I don't know.
[1505.66 --> 1507.00]  Too many road trips, I guess.
[1507.56 --> 1509.76]  Or too many installations of Ubuntu 2004.
[1510.08 --> 1516.06]  So you and I both had a very different experience with remote installations this week of Ubuntu 2004.
[1516.72 --> 1518.18]  Mine was really kind of tame.
[1519.20 --> 1520.10]  Flashed an image.
[1520.80 --> 1522.68]  Threw that image on a headless box.
[1523.08 --> 1526.70]  Waited for the DHCP server to issue a new lease.
[1526.82 --> 1531.04]  And then I just grabbed that IP from the log, SSHed into it, and began my setup.
[1531.04 --> 1533.42]  And I was in a nice, comfy SSH session.
[1533.52 --> 1534.14]  Can't complain.
[1534.70 --> 1536.64]  I think your experience was a little different, though.
[1537.18 --> 1542.30]  Before I emigrated, I made some plans with, you know, different servers and stuff like that.
[1542.36 --> 1546.46]  And I managed to convince my dad to leave my old server in his house.
[1546.80 --> 1549.54]  It's in a Fractal Define R5 case.
[1550.20 --> 1554.58]  The motherboard that's in there is an X8 Super Micro something.
[1555.32 --> 1558.14]  The Xeon chip that's in there is a V1.
[1558.14 --> 1559.44]  So it's quite old.
[1559.44 --> 1560.80]  It's only got 16 gigs of RAM.
[1561.50 --> 1566.34]  And it's really just designed to be a remote endpoint for my storage.
[1566.76 --> 1570.74]  So I had about 50 terabytes worth of storage in my server in the UK before I left.
[1570.84 --> 1573.94]  So I just left it all there and bought new drives when I came here.
[1574.82 --> 1580.74]  You know, it's got, I think, like five or maybe four, eight terabyte drives and a couple of six terabyte drives.
[1581.20 --> 1582.24]  No SMR drives.
[1582.32 --> 1584.54]  I did check after the drama lately.
[1584.54 --> 1585.68]  Yeah, you never know.
[1585.80 --> 1586.82]  They might sneak in.
[1586.88 --> 1588.36]  That's a TechSnap reference.
[1588.94 --> 1592.42]  And before I emigrated, as I just said, I left this at my dad's house.
[1592.68 --> 1593.94]  I installed Debian on it.
[1594.00 --> 1595.98]  And it's been working absolutely flawlessly.
[1596.64 --> 1608.00]  But recently, I decided to start investigating WireGuard and then thought, well, wouldn't it be cool if I could do some of the ZFS send and receive stuff that Jim and Alan Jude keep talking about?
[1608.00 --> 1612.64]  So then I started having to install DKMS modules on Debian.
[1613.04 --> 1615.54]  And this was, I don't know, a couple of months ago.
[1616.52 --> 1620.98]  And for some reason, last night, apt was just getting its knickers in a complete twist.
[1621.68 --> 1624.38]  The DKMS stuff was just not working.
[1624.48 --> 1625.26]  I couldn't fix it.
[1625.40 --> 1628.94]  And in the end, I thought to myself, you know what would solve all of my problems?
[1629.38 --> 1633.74]  Just going from Debian 9 to Ubuntu 2004.
[1634.46 --> 1636.64]  Which, of course, there's no direct upgrade path.
[1636.64 --> 1638.46]  You can't. That's nothing you're going to be able to do?
[1638.64 --> 1640.44]  No, you have to wipe and start from scratch.
[1640.96 --> 1643.02]  And this is in London, right?
[1643.12 --> 1648.00]  This box is in a closet in my dad's house at 2 a.m. British time.
[1648.14 --> 1651.14]  So it's quite high stakes game of poker here.
[1651.62 --> 1654.00]  Did you consider not going with WireGuard?
[1654.62 --> 1654.92]  No.
[1655.48 --> 1656.18]  No, of course not.
[1656.24 --> 1656.74]  Of course not.
[1656.74 --> 1660.26]  So I'm running PFSense as the firewall at his house.
[1660.50 --> 1663.94]  So I've got an open VPN tunnel I mostly use to stream iPlayer.
[1663.94 --> 1667.34]  Because iPlayer requires a residential IP block.
[1667.78 --> 1672.40]  So if you try and go through DigitalOcean or something like that, they know that those IPs aren't residential.
[1672.40 --> 1673.48]  So it won't work.
[1673.80 --> 1677.42]  So you have to go through, you know, like a parent's house or something like that.
[1677.94 --> 1678.92]  It works great for us.
[1679.42 --> 1691.26]  But so I connected through OpenVPN from a crusty old Windows VM that's running Java 8 to the ikvm, ipmi, java interface.
[1691.26 --> 1692.12]  Oh boy.
[1692.26 --> 1697.26]  I then downloaded the ISO to the VM that was running in my basement here.
[1698.12 --> 1706.84]  Mounted remotely the Ubuntu ISO into the, you know, virtual storage media manager that's part of this IPmi client.
[1707.66 --> 1710.72]  It then took about 25 minutes to boot.
[1711.16 --> 1712.60]  So I just got to visualize all of this.
[1712.70 --> 1716.86]  So first of all, it's like one of the worst interfaces ever created on the planet, right?
[1716.90 --> 1718.46]  For the IPKVM, I'm assuming.
[1718.78 --> 1719.10]  Yeah.
[1719.10 --> 1720.72]  It's about three frames per second.
[1720.86 --> 1720.98]  Yeah.
[1721.28 --> 1721.50]  Yeah.
[1721.56 --> 1721.80]  Okay.
[1722.38 --> 1734.00]  So you're on your desktop and you're accessing the ESXi console where inside there you're remotely viewing a Windows VM, which is remotely running this Java IPKVM.
[1734.44 --> 1734.94]  Yes.
[1735.78 --> 1737.00]  That sounds really horrible.
[1737.18 --> 1738.40]  It's pretty inception, isn't it?
[1738.60 --> 1739.70]  It's pretty inception.
[1739.70 --> 1758.00]  I'm running Windows on ESXi, accessing Windows through Firefox in a browser session, accessing the console output of my server in England through a Java client, mounting an Ubuntu ISO through the virtual media manager.
[1758.00 --> 1762.52]  And somehow I managed to get booted into the ISO on the third try.
[1762.52 --> 1770.76]  It was quite fun because my upload here is only 30 meg, which is, you know, it's still reasonable for cable, but it's not the gigabit that I had last year.
[1771.84 --> 1779.48]  And it was just absolutely pegging at 30 meg the entire upload whilst it booted the ISO, which I found really interesting.
[1779.94 --> 1780.58]  But it worked.
[1780.58 --> 1783.28]  Now, did you go with the server ISO or did you go with the net?
[1783.38 --> 1786.56]  I went with the server ISO and I think that was critical to my success.
[1786.94 --> 1788.38]  There was no clicking required.
[1788.50 --> 1796.32]  I could just press one button on the keyboard, wait for the latency to catch up and then press the next arrow button or press the next tab.
[1796.66 --> 1802.56]  Wait for that keystroke to actually occur and update and refresh and then move on to the next one.
[1803.22 --> 1806.64]  I think if you're trying to do this with an actual UI, you might struggle.
[1807.16 --> 1807.22]  Right.
[1807.30 --> 1808.96]  That would be horrible with the GUI.
[1808.96 --> 1812.70]  And then you also get to take advantage of some of the server's other features during the installation.
[1813.34 --> 1813.44]  Yeah.
[1813.64 --> 1821.36]  I mean, the installation of Ubuntu itself was relatively uneventful until I got to the point where it asked me if I wanted to import my SSH keys.
[1821.68 --> 1823.54]  And then my mind exploded.
[1823.94 --> 1826.84]  So this is something I've relied on Ansible to do for years.
[1827.48 --> 1830.66]  I keep all of my SSH keys up to date on GitHub.
[1830.66 --> 1838.98]  And then I use the authorized keys module to import all of my GitHub public keys onto specific hosts.
[1838.98 --> 1846.82]  But there's a new command they learned about called SSH-import-id, which will do the same damn thing for you.
[1846.88 --> 1847.40]  Isn't that great?
[1847.54 --> 1851.66]  And to make it even better, they've built it into the Ubuntu server installer.
[1851.66 --> 1861.06]  So all I type in is my GitHub username, press go, and then the cloud init file that it generates imports all of the SSH keys from GitHub that I have.
[1861.52 --> 1864.62]  So then I'm kind of curious, did you use ZFS for the entire thing?
[1864.66 --> 1869.20]  Or did you do Extended 4 on the root OS and ZFS on the data drives?
[1869.20 --> 1870.24]  What's the approach here?
[1870.28 --> 1877.02]  Because I assume there must have been a pool already existing that you were hoping you could reconnect to once the installation was done.
[1877.56 --> 1885.64]  I just made a very simple mirror of the two 6TB SSDs that I had in that box and then used that as my ZFS volume.
[1885.92 --> 1889.06]  I did install root on ext4.
[1889.40 --> 1893.78]  I didn't see an option exposed in the server installer for ZFS on root.
[1893.94 --> 1896.24]  So I didn't think to do that.
[1897.00 --> 1898.18]  Yeah, I didn't even think about that.
[1898.18 --> 1899.44]  Well, very interesting.
[1899.64 --> 1906.32]  And I suppose now you've been able to play around with some of the ZFS send and receive things that you were initially attempting to get to.
[1907.06 --> 1907.98]  Yeah, yeah.
[1908.32 --> 1913.76]  So I've now got WireGuard configured not to connect through the PFSense firewall.
[1914.06 --> 1922.12]  It's a point to point, you know, my media VM connects directly to the server that runs in my dad's house, you know, through WireGuard.
[1922.20 --> 1923.24]  So it's a point to point tunnel.
[1923.72 --> 1927.12]  And now ZFS send and receive will work over that tunnel.
[1927.12 --> 1942.06]  So I started using Jim Salter's Sanoid tool and Syncoid tool to manage not only the snapshots in terms of like a configurable hourly, daily, monthly, weekly type situation, but also to send them as well.
[1942.06 --> 1956.56]  So one of the really cool things about ZFS that's blowing my mind a little bit is that I can send data from one server and it will arrive in the same exact layout on the other server.
[1956.56 --> 1964.36]  That doesn't sound amazing until you realize that includes all the data sets, all the permissions, all of the snapshot history, all of the ACLs.
[1964.62 --> 1972.10]  Every single parameter that is attached to those files in America is now attached to those files in England.
[1972.68 --> 1974.38]  Right. And your file system is doing this.
[1974.44 --> 1978.72]  It's not some demon you're running in the background like R-Sync or something that's like me.
[1978.76 --> 1981.36]  I use Sync thing to move stuff around between my boxes.
[1981.36 --> 1984.66]  But this is being managed at a file system block level.
[1985.00 --> 1989.10]  Yeah, I've always kind of scoffed a little bit at the hidden cost of ZFS.
[1989.78 --> 1997.00]  You know, that you have to set pools up up front and that the penalty for getting it wrong, you know, let's say you set your A-shift wrong, for example, or something like that.
[1997.06 --> 1999.98]  So your partitions don't quite match the cylinders on the disk and stuff.
[2000.82 --> 2002.18]  The penalties are quite high.
[2002.30 --> 2005.80]  But I tell you what, when it works, it's amazing.
[2006.04 --> 2008.42]  It's cheaper than Glacier 2, I think, doing it this way.
[2008.42 --> 2010.66]  Yeah, if you have a place to send it to, for sure.
[2011.02 --> 2019.84]  I have this hybrid setup where at the studio I have this big super micro box that has the ZFS array where everything is ultimately stored.
[2020.18 --> 2030.14]  But then in my mobile RV setup, I have a pool of XFS for the storage drives and extended for the OS and SD cards.
[2030.14 --> 2034.26]  Because I just want as minimal overhead as possible on those boxes.
[2034.54 --> 2044.50]  And then I use SyncThing and Duplicati and other tools to move data around and just sort of negate the benefits of ZFS in the mobile setup.
[2044.62 --> 2046.80]  But I find that user space tools, you know, they work for me.
[2046.84 --> 2047.70]  They move data fine.
[2048.12 --> 2048.76]  Backup happens.
[2048.82 --> 2049.56]  I have snapshots.
[2049.64 --> 2050.26]  It's all fine.
[2050.62 --> 2054.22]  It's just not as tight and integrated into the file system as it could be.
[2054.40 --> 2056.18]  But here at the studio, I do take advantage of that.
[2056.18 --> 2061.38]  So I kind of have been enjoying the differences of these setups because there's things I like about both of them.
[2061.40 --> 2062.52]  And I think they're both pretty valid.
[2062.60 --> 2068.26]  It just sort of I think it is worth the time to investigate if you keep hearing people talk about it a lot.
[2068.36 --> 2072.86]  They just did a really good ButterFS compared to ZFS roundup on two and a half admins.
[2073.26 --> 2078.14]  And I think that's worth checking out, too, if you're curious about that, because there's a lot of tradeoffs there as well.
[2078.68 --> 2080.90]  And it really comes down to the workload.
[2080.90 --> 2084.48]  But if you haven't tried it, like Alex is saying, it's so easy to do now.
[2084.62 --> 2086.14]  It's so easy to just give it a go.
[2086.66 --> 2093.44]  Yeah, that's over at 2.5admins.com with Alan Jude, Jim Salter, and the beloved Joe Ressington.
[2094.00 --> 2096.56]  But of course, I just run APFS on everything.
[2096.98 --> 2097.76]  You madman.
[2098.62 --> 2103.20]  Now, it's not like ZFS has completely replaced everything on my file servers.
[2103.20 --> 2112.10]  Because media, you know, like movies and TV shows and that kind of stuff, stuff that's easily replaced is still being handled by MergerFS.
[2112.72 --> 2116.12]  What I'm using ZFS for is stuff that's irreplaceable.
[2116.20 --> 2119.04]  So I'm talking like photos, drone footage.
[2119.68 --> 2122.56]  Also, I'm using it for container app data.
[2123.00 --> 2126.72]  So I have a different data set for each container that I'm using.
[2126.72 --> 2136.14]  And then that way, before I make a change to the configuration of a particular app or something like that, I have a snapshot now that gets taken with Sanoid.
[2136.66 --> 2143.02]  If I screw up the configuration change, I can just roll back to the previous snapshot and I'm good to go.
[2143.02 --> 2147.68]  So there's lots and lots of different things that you can do when you're using ZFS.
[2148.32 --> 2158.88]  And the checksumming and, you know, the data integrity checks that it does for me on stuff like photos and music that I've ripped from my CDs I don't physically own anymore.
[2159.40 --> 2160.14]  Stuff like that.
[2160.24 --> 2163.18]  It's just I want to take every precaution I can with that stuff.
[2163.44 --> 2167.60]  So one thing I have yet to implement and I'm going to look into something.
[2167.60 --> 2174.88]  I'm curious, Alex, if you have any advice is I still would like to have checksums as well because that's something ZFS offers when you talk about boot rot.
[2175.40 --> 2185.46]  Really what you're talking about, especially with spinning media, but I suppose theoretically possible with solid state, is a failure of a block over time or an area of the disk that becomes unreliable.
[2185.64 --> 2188.06]  And the things you stored there are lost.
[2188.22 --> 2193.00]  And that's something that you have to check against if you're using spinning media.
[2193.08 --> 2195.44]  But I think it's worth checking against with solid state as well.
[2195.44 --> 2197.66]  And that's something ZFS includes.
[2198.18 --> 2202.52]  XFS and ButterFS and other file systems include checksumming for the metadata.
[2202.90 --> 2212.06]  So they sometimes are labeled as checksummed file systems, but they're not actually checksumming at the block level at each individual file all the way down the file system tree.
[2212.16 --> 2217.58]  They're just checking the metadata head, which is nice, but isn't going to tell you the entire picture.
[2218.04 --> 2222.78]  Before I moved to ZFS last year, this was after LinuxFest Northwest, actually.
[2222.78 --> 2225.48]  Alan and Jim were very persuasive.
[2225.96 --> 2228.98]  I actually have been using SnapRaid and I still do use SnapRaid.
[2229.24 --> 2233.58]  And that does do checksumming every day for me on my movies and TV shows.
[2234.24 --> 2237.30]  And that is snapshot parity calculations.
[2237.52 --> 2239.40]  So it knows when stuff has changed.
[2239.40 --> 2244.98]  I'm never super 100% convinced it's as effective as ZFS.
[2245.20 --> 2247.88]  I've not really got any way to check or any real way to know.
[2248.54 --> 2253.94]  Because if the bit changes overnight, well, when I run the SnapRaid sync the next day, it will go, oh, that bit's changed.
[2254.00 --> 2256.56]  So I'll just recalculate that bit of parity, no?
[2257.04 --> 2259.74]  So I don't know if that's how it would work or whatever.
[2259.92 --> 2262.06]  But SnapRaid does claim to do that.
[2262.40 --> 2262.48]  Yeah.
[2262.56 --> 2262.86]  Okay.
[2262.86 --> 2265.78]  I remember you talking about SnapRaid, and it's something I've been meaning to try.
[2265.90 --> 2272.30]  I also, I know in the past, I've come across tools like MD5Deep and HashDeep, which will go through.
[2272.42 --> 2276.46]  They'll crawl your whole file system, generate checksums, and then they can check against that.
[2277.06 --> 2280.76]  But hit those contact links or the Discord and let me know what you use.
[2280.76 --> 2291.64]  I would like something that I could cron or get some kind of output that would run every night on these pies, but isn't going to totally abuse the disk IO and the CPUs.
[2291.70 --> 2293.02]  So if you have any suggestions, let me know.
[2293.48 --> 2296.52]  If you're doing those jobs on cron, you should check out healthchecks.io.
[2296.70 --> 2303.88]  You can self-host that as a container, and that will let you check in with curl every night and send you an email if that cron job fails.
[2304.14 --> 2306.20]  You're going to get me to use healthchecks one of these days.
[2306.50 --> 2307.08]  You're right.
[2307.38 --> 2308.80]  I think I'm heading down that path.
[2309.12 --> 2309.62]  I like it.
[2309.62 --> 2311.44]  We'll put a link to that in the show notes as well.
[2311.78 --> 2315.86]  Everything we talked about is at selfhosted.show slash 19.
