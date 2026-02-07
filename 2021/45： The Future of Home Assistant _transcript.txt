[0.00 --> 3.28]  Well, we've got a special interview for episode 45 today.
[3.48 --> 5.44]  We're going to have our guest coming up in just a moment.
[5.50 --> 7.28]  So I want to thank our sponsor, A Cloud Guru.
[7.52 --> 10.64]  They are the leader in learning for the cloud, Linux, and other modern tech skills.
[11.04 --> 13.28]  Hundreds of courses and thousands of hands-on labs.
[13.40 --> 17.74]  Get certified, get hired, get learning at acloudguru.com.
[18.18 --> 22.22]  So today, instead of a bunch of different segments, we're really kind of just doing one thing.
[22.50 --> 22.84]  Hey, Alex?
[23.16 --> 23.68]  We are indeed.
[23.80 --> 27.26]  Yes, we've got Paulus, who is the founder of Home Assistant, on the episode today.
[27.26 --> 35.94]  And Chris and I talked to him about all sorts of different subjects, from how Home Assistant is becoming more turnkey ready, through to the ESP home acquisition.
[36.34 --> 39.72]  And there's a couple of interesting tidbits about the future in there as well.
[40.76 --> 50.84]  Well, I don't know if you remember, but you and I chatted back in 2017 on a Linux Action Show special about Home Assistant, what feels like 100 years ago now.
[51.36 --> 52.28]  Yeah, no, I do remember.
[52.34 --> 54.88]  Well, I remember it was somebody from Jupyter Broadcasting.
[55.00 --> 55.94]  I didn't realize it was you.
[55.94 --> 56.42]  Yeah.
[57.20 --> 59.50]  And man, have things come a long way.
[59.68 --> 62.52]  So thank you for joining us to catch us up on stuff.
[63.18 --> 66.80]  I am the happy owner of a Home Assistant Blue device.
[67.04 --> 67.68]  Love it.
[67.96 --> 68.20]  Awesome.
[68.62 --> 72.46]  I put the order in during the live stream, so I got it fairly early.
[73.22 --> 77.42]  And I got to say, you know, months into it, the performance holds up compared to the Raspberry Pi 4.
[77.54 --> 79.58]  I think it is outperforming the Raspberry.
[79.92 --> 81.24]  I mean, it's a beast.
[81.84 --> 83.68]  The N2 is just like, it's amazing.
[83.68 --> 87.08]  So are there any plans for more expansions in that direction?
[87.44 --> 89.74]  Is that going to be a focus going forward?
[89.78 --> 92.00]  Because it really seems like a pretty sweet integration.
[92.50 --> 92.68]  Yeah.
[92.74 --> 94.26]  So there are definitely plans.
[94.66 --> 96.36]  Nothing to announce just yet.
[96.80 --> 101.42]  We realized with the N2+, like we only made the case, right?
[101.46 --> 103.20]  So it's just a board.
[103.52 --> 110.78]  And when people think of home automation, they obviously think of like Zigbee or Z-Wave or Chip or Matter, whatever it's going to be called.
[110.78 --> 116.66]  And so that's something that we want to, you know, if we want to address, we want to include that as well.
[116.74 --> 129.50]  And I think the, you know, the Home Assistant Blue was really like, you know, the ultimate race car, but it was not very accessible in that the price was not, the price was pretty steep for like, you know, a device.
[129.60 --> 132.10]  And also you needed to add like a Zigbee stick and these kind of things.
[132.10 --> 147.28]  So I think we are definitely going to look into something as a successor, nothing to announce just yet, but it will also be hopefully lower priced and more capable out of the gate to be like, you know, used for smart home.
[147.80 --> 147.88]  Yeah.
[148.06 --> 154.84]  I can absolutely see how that would be way simpler for new users to get into the space as well.
[154.84 --> 155.24]  Yeah.
[155.34 --> 162.56]  And I think, you know, when we look at these things, it's not just like, we don't just want to create a box that competes with like Philips Hue or anything, right?
[162.56 --> 163.80]  Like we're Home Assistant.
[164.00 --> 169.22]  So it needs to be, you know, kind of hackable, playful, open.
[169.48 --> 173.22]  Like it just needs, you know, just like the Odoid N2 Plus or the Home Assistant Blue.
[173.34 --> 175.70]  I mean, you can flash anything on it that you want, right?
[175.76 --> 182.56]  We wouldn't, we're not interested in like building a lockdown box that like will just keep the users out.
[182.56 --> 185.82]  Well, that is completely understandable, especially now having used one.
[185.98 --> 191.56]  But so what about guys like me who will always have a use case where I'm going to want to run it on a server?
[191.64 --> 194.32]  Like here at the studio, we have a server that's doing like a hundred other things.
[194.42 --> 199.62]  And so running Home Assistant in a container is perfect for the use cases of just controlling studio lights.
[199.62 --> 202.32]  And we're not really using any integrations and stuff like that.
[202.62 --> 204.54]  How do you see that user base being addressed in the future?
[204.92 --> 207.14]  Right now we have four installation types.
[207.46 --> 211.08]  We have the Home Assistant operating system.
[211.08 --> 217.88]  We have the Home Assistant supervised, the Home Assistant container, and then Home Assistant core, which is just like running it in Python yourself.
[218.26 --> 223.10]  And all the other three installation approaches all rely on containers.
[223.34 --> 224.80]  And so they all use the same image.
[225.28 --> 227.60]  So it's like the core technologies are all very similar.
[227.76 --> 229.22]  Yeah, it's all the same thing, really.
[229.22 --> 236.92]  The only one that's different is core because you maintain your own Python virtual environment.
[237.52 --> 238.92]  The other three are all Docker based.
[239.02 --> 240.02]  So it's all the same thing.
[240.54 --> 243.82]  So those four installation types are pretty much set in stone right now.
[243.94 --> 252.28]  I think that if you, in your studio, you can either run the container or you can run a virtual machine with Home Assistant operating system.
[252.28 --> 257.44]  You know, the benefit, of course, of the virtual machine is that you have one-click updates of Home Assistant.
[257.96 --> 266.80]  Well, with the container, it really depends on like your container management software, which can be Unraid or Portainer or Synology or whatever.
[267.28 --> 270.72]  You know, that software then has to do the update of the container.
[271.14 --> 272.58]  I think that's the only real difference.
[272.58 --> 276.38]  In the end, all of these containers, they're all run Alpine.
[276.74 --> 278.50]  They run Python.
[278.64 --> 279.80]  And we maintain that, right?
[279.82 --> 282.54]  So we have a big wheel server.
[282.76 --> 287.44]  We make sure that all the dependencies work and compiled and are just up to date and running.
[287.90 --> 290.54]  And that's just, you know, a big benefit as a user.
[290.66 --> 294.22]  And I think that moving forward, you just want to run Home Assistant container?
[294.70 --> 295.74]  That will be possible.
[296.26 --> 296.48]  I see.
[296.56 --> 302.56]  So it's not like it's ever going to go away, but you just feel like there's a lot of benefits to Home Assistant managing the entire system.
[302.58 --> 305.02]  Because of all of the interdependencies.
[305.40 --> 305.52]  Yeah.
[305.58 --> 307.20]  I mean, there's just so many moving parts.
[307.38 --> 314.26]  I think that if you look at our requirements.txt, which is where we define like the Python dependencies, it's like over a thousand.
[314.78 --> 314.92]  Right?
[314.94 --> 319.62]  Because each integration comes with its own Python library, which is a requirement we made ourselves.
[319.76 --> 322.78]  So it's obviously like, you know, our own guidelines.
[322.96 --> 328.18]  But, you know, the reason we always do this is that we want integrations to rely on like an SDK.
[328.28 --> 332.08]  So an SDK is a Python package of the standalone that translates.
[332.58 --> 334.80]  The protocol into like Python objects.
[335.08 --> 338.98]  And that way, other Python projects, not just Home Assistant, can also use this package.
[339.14 --> 339.28]  Right?
[339.34 --> 342.72]  So we don't want protocol-specific information inside Home Assistant.
[343.22 --> 350.00]  Because we want to make sure that other Python-based home automation systems or just one-off scripts can use these protocols as well.
[350.00 --> 350.44]  Wow.
[350.44 --> 350.56]  Wow.
[350.74 --> 355.56]  So it kind of sounds like to me what you guys did as a team is you looked at the kind of, if you will, the whole problem.
[355.56 --> 367.00]  And you said, quite frankly, it is easier for us as a team to just do a whole OS than say, you must have considered, well, bless Ubuntu LTS as the supported Home Assistant platform.
[367.00 --> 368.76]  And anything else is DIY.
[369.08 --> 372.20]  But if you want our official way or our official image, it's all Ubuntu-based.
[372.38 --> 372.58]  Yeah.
[372.68 --> 380.96]  But the problem with that is that your virtual environment that runs Python is going to be, has to be maintained as well.
[381.02 --> 383.12]  So, I mean, this is, of course, how Home Assistant started.
[383.22 --> 386.08]  It was just a Python application that we distributed through PyPI.
[386.50 --> 386.68]  Sure.
[386.68 --> 390.00]  And people would run into, like, they would do pip upgrades.
[390.30 --> 393.34]  And then, of course, some people will upgrade from the last release.
[393.46 --> 395.84]  Some people will update from, like, six releases ago.
[395.98 --> 398.32]  And people got stuck all the time.
[398.42 --> 404.32]  And the way it works with our Docker containers is that we install all the Python dependencies fresh in each container.
[405.26 --> 410.16]  And so when you update your container, all your dependencies are thrown away.
[410.16 --> 414.56]  We make sure you have the latest and greatest dependencies all work together.
[414.56 --> 417.82]  And that way it just works.
[418.16 --> 418.74]  Yeah, that makes sense.
[419.06 --> 423.64]  I can see how that also is just much more manageable and supportable by you guys as well.
[423.80 --> 426.68]  And I got to say, you know, on the blue, it's working really great.
[426.80 --> 431.14]  I kind of am, I'm a user of both use cases, just the core version and the whole OS stack.
[431.42 --> 434.32]  And I do really like the snapshots.
[434.46 --> 439.82]  I feel like the more recent updates that have also set it so you can have a snapshot right before you upgrade is brilliant.
[439.96 --> 441.72]  All that kind of stuff just keeps getting better.
[441.72 --> 445.50]  Yeah, and I think, you know, the features are really driven.
[446.20 --> 448.40]  You know, we look at the way people use Home Assistant.
[448.70 --> 452.76]  And we look at the issues we see on our forums and on our Discord.
[453.08 --> 456.00]  And then we just ask ourselves, like, why is this?
[456.12 --> 458.44]  What can we do to make it easier and better?
[458.64 --> 461.88]  And we just constantly try to, like, kind of tackle this.
[461.88 --> 471.52]  And, you know, we're really focused on making Home Assistant easier to use while still also, you know, making sure that our power users, of course, can do their things.
[472.16 --> 474.76]  And, you know, it's been really paying off.
[474.80 --> 479.40]  I think that, like, we launched Home Assistant Analytics, like, a month ago, two months ago already.
[479.40 --> 479.72]  Right?
[480.40 --> 484.82]  And I think, like, around, we didn't do much promo, but, like, 45,000 people have opted in.
[485.20 --> 488.70]  And you can actually see our operating system is, like, 65% of our users.
[488.92 --> 489.38]  Oh, okay.
[489.76 --> 491.60]  I mean, that was pretty unexpected.
[492.08 --> 493.86]  Like, we knew it was high.
[494.02 --> 497.82]  I think, you know, internally we were like, ah, that's probably, like, 50%.
[497.82 --> 499.48]  But it's actually 65%.
[499.48 --> 503.26]  And I also understand it because it's just convenience, right?
[503.26 --> 507.96]  Like, if you want to be a system administrator at home, you can be, of course.
[508.04 --> 511.64]  But if you want to be, like, automating your home, you can be that, too.
[513.26 --> 515.16]  Linode.com slash SSH.
[515.22 --> 518.08]  Go there to get $100 in 60-day credit on your new account.
[518.22 --> 520.68]  And you support the self-hosted podcast.
[521.22 --> 522.80]  Linode is my playground to learn.
[522.90 --> 524.84]  And it can be yours, too, without a $100 credit.
[525.12 --> 528.80]  And, sure, maybe ultimately you decide to self-host something on your LAN.
[528.80 --> 538.90]  But every now and then, and that's more and more these days, there's a job that's really perfect out in the cloud on a service provider you can trust and you have full control.
[539.24 --> 545.58]  That's one of the things I like about Linode is, unlike entry-level hosting services, they don't try to lock you into their platform with gimmicks.
[546.00 --> 549.94]  Linode gives you full back-end access to customize and control your server to fit your needs.
[550.18 --> 553.32]  And their DNS manager allows you to easily switch your domain to your new server.
[553.32 --> 560.08]  You can manage SSL certificates with Breeze and deploy applications with a single click or build the server up from scratch if you want.
[560.30 --> 566.22]  If you need a simple personal server for a blog or portfolio or maybe a game server, in fact, they make that really straightforward,
[566.62 --> 570.02]  or maybe you want to set yourself up a NextCloud server and sync your own files.
[570.10 --> 573.94]  Whatever the scale of your task or your business or even when your app goes viral,
[574.54 --> 577.74]  Linode is going to reliably serve to millions of users.
[577.84 --> 581.98]  It can be just you and your friends and family or it can be millions of users.
[581.98 --> 584.66]  And we've really put it to the test here at Jupyter Broadcasting.
[584.86 --> 588.70]  And like I say, it really is a fantastic playground to learn as well.
[588.96 --> 593.26]  And that $100 credit means you can play around with all kinds of different hardware and configuration stacks,
[593.42 --> 595.26]  which has been a massive advantage for me.
[595.70 --> 600.20]  Before I deploy something in production, I'll sometimes spin up a couple of versions of it on different stacks.
[600.52 --> 602.62]  You know, maybe this one's on Nginx and this one's on Apache.
[602.78 --> 603.62]  Maybe this one's on Ubuntu.
[603.76 --> 604.80]  Maybe this one's on CentOS.
[605.12 --> 606.60]  I'll try them out and test them right there.
[606.86 --> 608.52]  And then I'll just keep the winner and destroy the others.
[608.52 --> 614.28]  That kind of flexibility and not having to mess around with some slow VM software on my laptop to test that stuff out.
[614.72 --> 615.44]  Well, it's just brilliant.
[615.74 --> 619.00]  And then, of course, there's the perk as a listener of supporting this here podcast, too.
[619.22 --> 622.84]  And we use their S3 compatible object storage as the back end storage for our next cloud,
[622.98 --> 625.76]  which means we're not constantly managing disk space all the time.
[626.02 --> 628.92]  They've really got this stuff dialed in because they've been doing it since 2003.
[629.16 --> 630.26]  So I want you to go try it.
[630.66 --> 632.88]  So go to linode.com slash SSH.
[632.98 --> 636.00]  Go there, get that $100 in credit and support the show.
[636.40 --> 637.52]  Linode.com slash SSH.
[637.52 --> 644.74]  Yes, I mean, Home Assistant's been headed down the more turnkey route for quite a while now.
[645.26 --> 648.92]  And I think HASSOS is, or am I calling it the right thing?
[649.04 --> 650.76]  I'm still confused by the name change.
[651.76 --> 655.10]  It's been headed down the turnkey route for quite a while.
[655.90 --> 657.76]  What else do you have planned in that space?
[657.84 --> 660.36]  I mean, there's been a lot of work around automations recently,
[660.36 --> 664.32]  as well as some other aspects of the experience.
[664.32 --> 668.30]  So I think that our goal really, like in the longer term,
[668.34 --> 674.88]  is that we want to make sure that a lot of people have access to having like great home automation at home
[674.88 --> 677.72]  that, you know, focuses on local control and privacy.
[677.94 --> 681.44]  And so having Home Assistant be accessible is important to us.
[681.50 --> 685.86]  But for example, we've also, you know, the company behind Home Assistant,
[685.86 --> 689.08]  my company, Nabucasa, we've also recently acquired ESP Home.
[689.82 --> 694.20]  ESP Home is a firmware for ESP devices that runs on a,
[694.58 --> 698.50]  which is a firmware that can run on a lot of products that come from China,
[698.66 --> 700.82]  like light switches, lights.
[700.82 --> 705.38]  And with ESP Home, we are also trying to make it easier for people to get,
[705.64 --> 711.52]  you know, access to devices that work locally and work private and work with Home Assistant.
[712.52 --> 716.24]  So yeah, our long-term goal is really just to make it accessible to everybody.
[716.38 --> 720.82]  And I think that launching hardware was a really obvious step.
[721.08 --> 725.68]  I feel that for a long time, I didn't want to go down that route because logistics,
[726.00 --> 727.50]  just like all that stuff.
[727.50 --> 731.04]  But at the end of the day, we were looking at it and we were like,
[731.32 --> 733.76]  we've been working on making it so much easier to use.
[734.04 --> 737.78]  But then the first step of instructions is download Etcher,
[737.98 --> 740.18]  download this image and flash it to an SD card.
[740.42 --> 742.36]  And most people don't even know those words.
[743.06 --> 743.74]  Yeah, it's true.
[744.16 --> 747.48]  That has me thinking about something like, you know, the Made for iPhone program?
[747.74 --> 747.92]  Yeah.
[748.06 --> 752.32]  Makes me think with ESP Home in particular, I know it's aimed primarily at hackers
[752.32 --> 756.60]  and people that want to build and make and solder and all that kind of stuff.
[756.60 --> 759.04]  But it's got me thinking, it's acquisition of ESP Home.
[759.16 --> 761.36]  Why isn't there a Made for Home Assistant program?
[761.78 --> 769.26]  Well, I think that the main thing about Made for Home Assistant is that we don't have an API ourselves,
[769.62 --> 769.78]  right?
[769.80 --> 771.66]  Like we always integrate with the other products.
[772.08 --> 778.42]  I did consider like starting one or like having like at least some certification and more official certification.
[778.42 --> 786.66]  But we see that there's not much interest in it in a way that like, you know, manufacturers will come to us and be like,
[786.96 --> 787.66]  well, what's your API?
[787.80 --> 788.30]  We'll integrate.
[788.90 --> 790.84]  And I'm always like, no, that's not what we want.
[790.90 --> 792.72]  We want you to create an open API.
[793.02 --> 794.14]  We will integrate with it.
[794.14 --> 797.62]  But other projects should also be able to allow to be integrated with it.
[798.08 --> 801.02]  And then we see a lot of companies be like, ah, that's not in our interest.
[801.38 --> 808.46]  Or, you know, we were talking to Ring because, you know, they wanted to say like, hey, can we get like a partnership going?
[808.92 --> 809.90]  And then we looked at it.
[810.02 --> 814.00]  And the first step is sign NDA to make sure that you don't expose the APIs.
[814.20 --> 814.46]  Right.
[814.46 --> 815.88]  And like, we're open source.
[816.02 --> 816.96]  This is not going to happen.
[817.06 --> 822.64]  And the same thing happened to us with Sonos, who also was like, yeah, we want to keep it to partners only.
[823.10 --> 825.08]  It's like, ah, okay, that doesn't work.
[825.42 --> 827.46]  Oh, that's super frustrating to hear that kind of stuff.
[827.52 --> 833.32]  Because some of those companies you listed, you know, Ring and Sonos, they're big players in this space.
[833.34 --> 839.16]  And that's kind of frustrating to hear that they're not compatible with an open source ethos yet.
[839.50 --> 840.76]  Well, their partnerships are not.
[840.88 --> 842.38]  But I mean, we still integrate with them.
[842.48 --> 842.68]  Right.
[842.68 --> 842.92]  Right.
[842.92 --> 848.64]  It's just less official because they still have APIs and people have been able to figure out those APIs.
[849.54 --> 851.30]  And so we will still integrate with them.
[851.60 --> 856.98]  It's just, if you are a partner, they will make sure it stays working or they will give you a heads up so you can adjust.
[857.74 --> 859.00]  And that's something we don't have.
[859.06 --> 859.24]  Right.
[859.28 --> 861.28]  So we sometimes get caught off guard.
[861.40 --> 863.98]  Like some, some brand will change an API.
[864.64 --> 865.70]  Home Assistant stops working.
[866.26 --> 869.10]  We have to update our code, ship a hotfix, and it will work again.
[869.10 --> 872.78]  Which leads me nicely into my next question, which is about the velocity of change.
[872.78 --> 875.92]  Now, I've been using Home Assistant for a couple of years myself.
[875.92 --> 879.58]  So I've been through quite a few breaking config changes over that time.
[880.32 --> 888.42]  I feel like, and this is just anecdotal personal experience, that that experience has gotten better, that the pace of change hasn't decreased.
[888.42 --> 894.94]  But the amount of changes that break stuff, that has decreased significantly from my perspective.
[894.94 --> 904.56]  What things are you doing from, you know, a Home Assistant side to make that velocity of change more easy for people to handle?
[904.56 --> 912.10]  So the biggest change there, and it was actually, it started out with a policy change and then like it resulted also in code changes.
[912.28 --> 913.88]  But so there's this thing called config flow.
[914.04 --> 916.30]  So through the UI, you can set up an integration.
[917.08 --> 921.34]  And what we said is that this is going to be mandatory moving forward.
[921.54 --> 928.98]  So it used to be that you could like go into YAML and then, for example, let's say for your Philips U bridge, you would say this is the IP address.
[928.98 --> 935.68]  And then, well, Philips U is maybe a bad example because you would still have to press a button in the UI and it was storing some extra data.
[935.84 --> 940.90]  But for some things, you have to like, here's a username, password, and IP address of a device on my network.
[941.34 --> 945.30]  But then when the IP address would change, Home Assistant wouldn't work.
[945.42 --> 952.16]  And Home Assistant couldn't find the new IP address because you had it hardcoded in your configuration files and we're not changing your configuration files.
[952.86 --> 957.08]  And so those cases, we really had to handle through a UI.
[957.08 --> 960.94]  We had to like say, hey, this is a temporary IP address, but we still have an identifier.
[961.36 --> 967.64]  So if your Chromecast changes IP address, we can still find it and we will set it up again or your Shelly or whatever you have.
[968.36 --> 980.30]  And then we realized that, oh, actually, a lot of our breaking changes is because people are adding support to having to go from one device, support multiple devices or these kind of things.
[980.42 --> 985.74]  And so when we go for a config flow, Home Assistant is responsible for how it is written to disk.
[985.74 --> 988.28]  So Home Assistant knows exactly the configuration format.
[989.06 --> 996.62]  And if we have to change it because we are going to support multiple devices, we can actually migrate that data because we own how it is stored.
[997.30 --> 1004.92]  If it is a configuration file, and this is kind of silly, but we kind of programmed our way into like a corner we can't get out of.
[1004.92 --> 1011.34]  Because if you look at configuration.yaml, we have all these advanced structures to break up your configuration files.
[1011.46 --> 1016.34]  There's packages with includes and then include their name, include their list.
[1016.50 --> 1018.36]  And there's all these different types.
[1018.52 --> 1026.24]  And what that means is that Home Assistant cannot go update your configuration file anymore because it doesn't know where your configuration file is.
[1026.24 --> 1029.36]  We would have to reverse track all your includes.
[1029.54 --> 1036.08]  And then we need to find like a YAML writer that respects your comments and respects your indentations exactly how it was.
[1036.72 --> 1038.32]  And it's just, it's impossible.
[1038.92 --> 1040.80]  I think safe mode was a really good invention.
[1041.16 --> 1043.02]  That, well, not invention, idea, right?
[1043.08 --> 1047.06]  Where Home Assistant still starts and then just goes back to a safe mode.
[1047.50 --> 1047.68]  Yeah.
[1047.80 --> 1051.44]  So safe mode was really driven by the blue, right?
[1051.44 --> 1055.72]  So we had the blue in mind and we were like, okay, we're going to have a box.
[1055.82 --> 1056.76]  We're going to sell these people.
[1056.98 --> 1061.60]  Like it will actually allow more people to use Home Assistant than previously were not using Home Assistant.
[1061.80 --> 1066.02]  So how can we make sure that they can always boot and always have a UI?
[1067.16 --> 1072.76]  That shows you just how long it takes to develop a product because they were released a long time apart, those two things.
[1072.90 --> 1073.66]  Oh, yeah, yeah, yeah.
[1073.66 --> 1076.42]  I mean, it took us a year to make that case for the blue.
[1076.42 --> 1084.64]  So it's, I mean, a pandemic happened and like with other stuff, but yeah, it took us a year all in all to just get a case.
[1084.96 --> 1088.22]  So I hope our next product will not take that long.
[1088.56 --> 1090.18]  At least, I mean, we'll see.
[1090.36 --> 1090.70]  But yeah.
[1092.42 --> 1093.72]  Yeah, it is very tricky.
[1093.86 --> 1094.06]  It is.
[1094.42 --> 1101.92]  It's fascinating, though, how thinking about from a developer perspective, how to ship something for an end user, we got a feature like that.
[1102.00 --> 1104.72]  I think that's kind of telling how created that use case.
[1104.72 --> 1107.32]  So I'm curious, let's shift gears to the personal side.
[1108.00 --> 1111.02]  If you do have some self-hosted services, what are you running on your LAN?
[1111.54 --> 1115.72]  And roughly how much storage do you have on this set, quote unquote, LAN?
[1115.90 --> 1125.50]  So I run Unraid at home and I made a server that must have been like six, seven, eight years ago or something.
[1125.84 --> 1127.22]  Like now it's six years.
[1127.30 --> 1128.32]  It's getting really old.
[1128.36 --> 1129.94]  It's like a core i5 still.
[1130.02 --> 1133.46]  And I think it takes up way too much power compared to what it does.
[1134.72 --> 1139.88]  You know, I chose Unraid because this was during the beta phase of Unraid.
[1140.02 --> 1141.74]  So beta phase of Unraid 5.
[1142.24 --> 1144.96]  And Unraid 5 was where they introduced the Docker containers.
[1146.14 --> 1152.54]  So that was like almost kind of right away, I kind of shifted into like this perfect world of having all these containers at home.
[1152.60 --> 1156.80]  And so I'm actually still the maintainer of the Home Assistant core template for Unraid.
[1157.02 --> 1157.46]  Love that.
[1157.46 --> 1162.44]  So that's how I used to run Home Assistant for a long time.
[1162.54 --> 1164.28]  I was like, I just have my container at home.
[1165.24 --> 1168.90]  And then I have like, I have Plex running and some other stuff.
[1169.22 --> 1171.90]  And then you had to go and make it a whole OS.
[1172.06 --> 1172.34]  No, I'm kidding.
[1172.52 --> 1172.60]  Yeah.
[1173.38 --> 1174.72]  I hear Plex in there.
[1174.82 --> 1175.18]  Interesting.
[1175.50 --> 1176.30]  What's that setup like?
[1176.30 --> 1184.40]  I mean, so I mainly use Plex because a bunch of the, so I'm in the, I'm from the Netherlands, but I live in the United States.
[1184.40 --> 1188.08]  And there's a bunch of content from the Netherlands that is geo blocked.
[1188.08 --> 1190.34]  And so I cannot access it in the United States.
[1190.58 --> 1190.84]  Yeah.
[1190.98 --> 1194.76]  So I have to jump on a VPN and download either stuff on YouTube or whatever.
[1194.76 --> 1198.92]  And then I also don't want my son to be on YouTube, like unsupervised.
[1198.92 --> 1205.72]  So that's also why I pull in some videos and then I'll just have a Plex account for my son and he can kind of just browse through it.
[1206.06 --> 1207.46]  I do that same thing for my kids.
[1207.66 --> 1207.84]  Yep.
[1207.92 --> 1208.30]  Exactly.
[1208.36 --> 1209.60]  It's a great use case for Plex.
[1209.92 --> 1210.06]  Yeah.
[1210.14 --> 1212.82]  Well, that's, and then how much storage roughly would you estimate?
[1213.66 --> 1216.14]  I think it's like eight terabyte.
[1216.14 --> 1222.06]  I just got some smart errors the other day, two months ago, some CRC smart check error.
[1222.36 --> 1225.78]  So I just, but then, I mean, with Unraid, you have this parity disk.
[1225.78 --> 1229.98]  Your parity disk needs to be the same size or bigger than your biggest disk.
[1230.06 --> 1232.12]  And so my biggest disks were like four terabytes.
[1232.30 --> 1235.62]  And so I was like, wow, I should really update to like eight terabyte disks.
[1235.74 --> 1238.38]  And so I only updated my parity disk now.
[1238.52 --> 1240.62]  And that took like more than a week, right?
[1240.62 --> 1243.30]  Because you have to like pre-clear it and all that stuff.
[1243.60 --> 1243.72]  Yeah.
[1245.08 --> 1248.28]  And then I have, I still have one disk that is like on Riser FS.
[1248.48 --> 1251.38]  And I think they stopped using Riser FS and they're using something else.
[1251.38 --> 1253.72]  And I was looking into, should I migrate this?
[1253.72 --> 1257.12]  And then I was like, no, this is just like, no, it's too much.
[1257.52 --> 1258.50]  It still kind of works.
[1258.62 --> 1261.20]  And so I actually only updated the parity disk.
[1262.02 --> 1268.42]  And then I've, the old parity disk I installed now as in my rate, because there's only a couple of errors.
[1268.42 --> 1271.36]  And then I read online that like, ah, it's okay if you have a couple of errors.
[1271.62 --> 1274.16]  And that was, that was already after I did my whole process.
[1274.36 --> 1275.10]  But of course, I mean.
[1275.42 --> 1276.96]  That just means it's time to start shopping.
[1277.46 --> 1277.74]  Yeah.
[1278.08 --> 1278.48]  Exactly.
[1278.82 --> 1279.20]  Yes.
[1279.20 --> 1281.86]  I'm waiting for some like deals, right?
[1281.94 --> 1284.10]  Because I, those disks are expensive.
[1284.36 --> 1288.12]  I was like, I use the Western Digital Red, I think.
[1288.42 --> 1290.30]  Are you familiar with shucking drives?
[1290.44 --> 1292.02]  Is that of any interest to you?
[1292.46 --> 1292.98]  What is that?
[1293.52 --> 1298.54]  So you buy, you buy a USB hard drive from Amazon or Best Buy or something.
[1298.68 --> 1300.36]  This is Alex's favorite thing to do.
[1301.56 --> 1302.34]  I'll show you.
[1302.40 --> 1303.46]  I've literally got one over here.
[1303.46 --> 1305.62]  It's just like it sounds.
[1305.74 --> 1308.82]  You grab the disk off Amazon and you shuck it out of the case.
[1309.22 --> 1314.80]  I paid for this Iron Wolf NAS Pro $170 for a 10 terabyte drive.
[1314.94 --> 1315.32]  Oh, wow.
[1315.52 --> 1320.80]  And all I had to do to get this was buy a USB enclosure drive and pop it out the USB enclosure.
[1320.94 --> 1322.46]  It took five minutes.
[1323.14 --> 1325.38]  And it's a, it's a normal SATA drive.
[1325.50 --> 1328.20]  There's nothing special about it once you get it out of the case.
[1328.20 --> 1333.34]  If you look just on eBay, just for this drive on its own, I could sell this thing for $350.
[1333.76 --> 1334.88]  In fact, why don't I do that?
[1335.94 --> 1336.46]  There you go.
[1336.60 --> 1338.08]  You got to pay for that solar setup somehow.
[1340.68 --> 1341.04]  Yeah.
[1341.14 --> 1342.84]  So the shucking technique is Alex's favorite.
[1342.96 --> 1347.26]  Sometimes it requires a little more work than that, but it is a great way to get drives at a great price.
[1347.58 --> 1348.80]  Oh, that's a good, a good tip.
[1349.52 --> 1351.94]  Hey, I really talk about solar, Alex.
[1352.14 --> 1352.40]  Yeah.
[1352.64 --> 1356.28]  We're actually working or we have an intern at Home Assistant.
[1356.28 --> 1362.10]  And, well, he actually, he's an intern at Nabokasa, but he's working on Home Assistant stuff.
[1362.16 --> 1365.78]  And his focus right now is create a solution.
[1366.04 --> 1372.98]  How do we get, use Home Assistant to give the user insight into their energy usage and allow optimizing it?
[1373.62 --> 1380.26]  So, of course, Home Assistant has been very, always very focused on home control, home automation.
[1380.26 --> 1381.58]  And it's been like our strength.
[1382.20 --> 1384.38]  History has not been our strength that much, right?
[1384.38 --> 1388.38]  Like our database has been clunky and it's pretty shitty.
[1389.46 --> 1392.74]  So, I mean, we're actually changing this right now.
[1392.82 --> 1395.22]  So in the next release, it's going to be what we call statistics.
[1395.80 --> 1397.96]  And it's going to be a new table in our database.
[1398.42 --> 1400.88]  And it will take like a snapshot every hour.
[1401.06 --> 1403.96]  It will analyze like certain entities that you have.
[1404.22 --> 1405.96]  Right now it's temperature and energy.
[1405.96 --> 1410.50]  We calculate the min, the max, the mean, the sum, all that stuff.
[1410.50 --> 1423.52]  And then the goal is to get like, start generating dashboards on your energy usage and to show like predictions and show, you know, comparing like current period, current week to last week, these kind of things.
[1423.52 --> 1430.46]  Now that second part is not going to be in the next release, but we're already going to start generating statistics in the next release.
[1430.46 --> 1431.46]  Sounds fantastic.
[1431.68 --> 1437.18]  And I'll tell you, the solar company that's doing my install, it's a local one in North Carolina.
[1437.52 --> 1442.22]  They want to charge me $800 for energy monitoring.
[1442.66 --> 1447.68]  So I'm using the, I think SolarEdge is the manufacturer of the panels.
[1447.68 --> 1454.66]  And they have a cloud API, which Home Assistant can poll every 15 minutes, I think, to get the data.
[1454.82 --> 1457.20]  But I'm like, it's in my house.
[1457.20 --> 1459.62]  Why do you need to go to the cloud to get this stuff?
[1459.92 --> 1464.04]  So I'm thinking I might get one of these Shelly energy monitors.
[1464.20 --> 1468.36]  And then, you know, with everything you've just said, I think I might be in business.
[1468.60 --> 1468.96]  No kidding.
[1469.42 --> 1469.68]  Right.
[1470.16 --> 1473.22]  You know, Paul, I know too, I got to speak up for the van lifers out there.
[1473.22 --> 1476.96]  The Victron Venus system speaks MQTT.
[1477.64 --> 1483.00]  And so I know there's guys out there that are pulling that information into their Home Assistant setup as well.
[1483.28 --> 1483.40]  Yeah.
[1483.48 --> 1490.78]  And so we've really been looking at, or we have, I don't know if you, we tweeted it from the class, tweeted it like two weeks ago, I think.
[1490.96 --> 1494.18]  But he has already, has a lot of paper mockups and he's been like playing.
[1494.32 --> 1496.76]  I think he has interviewed like 20 different people.
[1497.12 --> 1501.20]  And he's been really focusing on, can we kind of gamify it?
[1501.20 --> 1509.52]  Where like, for example, if you know your yesterday's usage and we show your today's usage, can we tell you like, hey, tone it down a little?
[1509.66 --> 1512.76]  Because otherwise you're going to use more than like yesterday.
[1513.34 --> 1514.36]  I've actually had an idea.
[1514.86 --> 1517.84]  A friend of mine, I've just had my first kid, by the way.
[1517.84 --> 1523.48]  A friend of mine was telling me they were doing that automating nap time, a light in the nursery with Home Assistant.
[1524.30 --> 1528.08]  You know, certain times if the light bulb's green, then the kids are allowed out of the room.
[1528.12 --> 1529.08]  And if it's red, they're not.
[1529.44 --> 1532.94]  I'm thinking we could play games with colored light bulbs and children at this point.
[1533.06 --> 1534.38]  That's where my brain's going.
[1534.90 --> 1535.34]  Oh, I do it.
[1535.42 --> 1535.78]  I do it.
[1535.84 --> 1539.28]  That's, you know, I train my kids with a series of light changes at night for bedtime.
[1539.28 --> 1541.86]  And then noisemakers come on throughout the rig.
[1542.34 --> 1542.96]  It's real.
[1543.36 --> 1543.94]  It's brilliant.
[1543.94 --> 1545.60]  I can't wait to play with that.
[1545.68 --> 1549.94]  And gamifying, it feels like that's an idea that could be applied to a lot of things.
[1550.40 --> 1562.04]  As somebody who uses Home Assistant to manage an off-grid setup, I would love something around energy history and a gamification system that would encourage the family to maybe conserve energy.
[1562.04 --> 1570.64]  Because one of the things I did that really encouraged family adoption was we got a fire tablet and we just put Home Assistant up on it all the time.
[1570.64 --> 1574.26]  It's on the wall and it's always there so the kids can see what's going on.
[1574.32 --> 1577.58]  And once I did that, it like it clicked for everybody.
[1577.70 --> 1582.66]  So to get something up on that screen would, man, they just take my off-grid game to like the next level.
[1583.42 --> 1587.50]  Yeah, I think honestly, just getting people inside in it is like step one.
[1587.58 --> 1593.76]  Then all of a sudden they start to realize it's like, oh, I can actually, you know, we can generate more energy than we used today.
[1593.88 --> 1594.72]  Let's go for it.
[1594.98 --> 1595.16]  Right.
[1595.20 --> 1596.34]  I think that's going to be fun.
[1596.34 --> 1600.18]  So my last question, I think, before we let you go is about automations.
[1600.60 --> 1604.36]  This kind of goes back to the turnkey aspect, I suppose, and simplification.
[1604.78 --> 1611.60]  There's been a lot of work around making the YAML automation interface built into Home Assistant easier.
[1612.40 --> 1616.80]  But I always find myself for the more complex things reaching for Node-RED.
[1616.94 --> 1621.04]  And I wondered how you felt about people like me doing that.
[1621.28 --> 1624.68]  Do you want us to all be using YAML all the time or do you not really care?
[1625.06 --> 1625.84]  I don't really care.
[1625.84 --> 1641.34]  In fact, I think it's great that our APIs are so generous that you can get anything out, that you can actually build Node-RED and do a full automation engine without being part of the Home Assistant integrations.
[1641.74 --> 1644.32]  And I think that, you know, each has their own.
[1644.40 --> 1649.50]  And I think because Node-RED exists, we don't have to make a lot of things ourselves, right?
[1649.50 --> 1654.10]  A lot of feature requests that would normally come to us are now, ah, I will just use Node-RED.
[1654.10 --> 1656.66]  And I just saw a pull request.
[1656.66 --> 1667.60]  I mean, I guess it's been like one and a half months ago from the maintainer of the Node-RED Home Assistant integration who makes like the nodes for Node-RED.
[1668.00 --> 1674.34]  And I think he's been working on getting the triggers from the Home Assistant Animation YAML into Node-RED as well.
[1674.34 --> 1678.28]  So we have a lot of triggers that are not very accessible yet.
[1678.80 --> 1681.82]  A lot of advanced triggers that are not accessible in Node-RED yet.
[1682.48 --> 1690.58]  But that would allow Node-RED to use anything that a normal YAML automation can would be possible inside Node-RED, which I think is really cool.
[1690.58 --> 1695.88]  Because all of a sudden it makes Node-RED a lot more powerful or any other automation engine.
[1696.78 --> 1703.34]  And, you know, in the end, one way or the other, if you have like local control, local data, we succeed.
[1704.06 --> 1704.72]  Yeah, I totally agree.
[1704.72 --> 1709.34]  And I think my number of input booleans could use some spring cleaning.
[1709.52 --> 1711.02]  So I'm happy to hear that.
[1711.02 --> 1728.02]  Go there to try out Provado for free and, of course, support the show.
[1728.26 --> 1731.42]  Provado VPN is a zero log VPN.
[1731.82 --> 1734.38]  That means there's no records of your activity.
[1734.38 --> 1738.56]  We looked into this for you guys, and we wouldn't feature them unless it was this way.
[1738.56 --> 1746.26]  And even in the event of a legitimate authority requesting logs associated with your activity when connected to Provado, they got nothing to give.
[1746.68 --> 1749.10]  And even better, they're backed by Swiss privacy laws.
[1749.26 --> 1753.74]  In addition to having that strict zero log policy, Provado VPN is based in Switzerland.
[1754.28 --> 1758.82]  That means you're protected by the absolute strongest consumer privacy laws in the world.
[1759.54 --> 1761.28]  And Provado has the tech where it matters.
[1761.38 --> 1764.68]  They own and operate their own data centers and fiber lines.
[1764.68 --> 1770.78]  And the network is composed of hundreds of servers physically located in 45 countries and 58 cities around the world.
[1770.94 --> 1773.68]  What that means for you is you can connect in seconds.
[1773.68 --> 1778.22]  And no matter what server you choose, you're going to get incredibly fast speeds every time you connect.
[1778.80 --> 1782.96]  Provado VPN's network was built from the ground up and fully optimized for lightning fast speeds.
[1783.04 --> 1788.36]  So visit provadovpn.com slash SSH and try it out right now for free.
[1788.36 --> 1798.48]  The free account provides the same service level and unlimited speeds as the premium version, as well as 10 gigabytes a month of data transfer and access to the top 12 servers for one device.
[1798.92 --> 1804.34]  And all Provado VPN users get access to their dedicated team of customer support that's 24-7.
[1804.54 --> 1809.50]  And they also have an unlimited plan with hundreds of servers, P2P traffic support, and more.
[1809.76 --> 1814.40]  So go check it all out at provadovpn.com slash SSH.
[1814.40 --> 1822.18]  So, I mean, if you buy a Chromecast or whatever, then sometimes you have to, like, connect to an access point and then, like, your phone.
[1822.28 --> 1826.96]  And then sometimes it crashes and you're, like, lost and you don't know how to set up the Wi-Fi.
[1827.26 --> 1831.70]  So we're building a Bluetooth spec that is going to be built into ESP Home.
[1831.92 --> 1833.52]  It's going to be built into the Home Assistant app.
[1833.66 --> 1839.80]  So if you buy it, well, I mean, eventually we hope you're going to be able to buy ESP Home products.
[1839.80 --> 1845.62]  But if you build an ESP Home product and you give it to your friend, they would just be able to go on with Bluetooth.
[1845.92 --> 1847.48]  And we even have a web Bluetooth SDK.
[1847.68 --> 1850.86]  So you can use, like, a Chrome browser to actually just set it up.
[1851.76 --> 1852.88]  Oh, that is cool.
[1853.52 --> 1853.80]  Yeah.
[1853.82 --> 1854.24]  I like that.
[1854.40 --> 1854.68]  Right?
[1854.84 --> 1860.48]  And, I mean, I think I really want, like, you know, they're, like, on Tindy, people are selling their creations.
[1860.74 --> 1863.94]  I just want, like, more of that because those products are way cooler.
[1863.94 --> 1874.18]  Or, like, it's just, like, you know, we had the tech reader last year and there's, like, actually for the energy meters in the Netherlands, they actually have a protocol called P1.
[1874.56 --> 1882.88]  And we're going to have an ESP Home-based device somebody's building that, like, you know, people can just plug it in and, boom, all the energy data is available in Home Assistant.
[1883.48 --> 1884.38]  I'm sure you do.
[1884.38 --> 1890.28]  But do you realize just how perfectly positioned you are to uniquely so to do this?
[1890.96 --> 1891.74]  No, yeah, definitely.
[1891.98 --> 1892.26]  Definitely.
[1892.26 --> 1900.36]  It's because, you know, ESP Home, like, we acquired it mainly because, like, the original founder was, like, burned out.
[1900.64 --> 1903.48]  But he was still getting, like, all these donations, right?
[1903.50 --> 1907.80]  So we couldn't really say, hey, we're going to hire somebody full-time to make this great.
[1908.60 --> 1910.00]  So we acquired it from him.
[1910.12 --> 1911.88]  We have now Jesse working on it full-time.
[1912.08 --> 1916.48]  And, like, you know, just we keep, you know, pumping out cool stuff.
[1917.42 --> 1921.44]  Yeah, a full-time employee is going to, you know, they've got some time to fill.
[1922.26 --> 1928.78]  You know, it's, yeah, well, the thing is, because we're so big, like, you know, we are 13 people full-time now.
[1930.38 --> 1930.98]  That's crazy.
[1931.50 --> 1932.18]  Yeah, thanks.
[1932.74 --> 1933.48]  Lucky 13.
[1933.48 --> 1938.46]  But the thing is, they work all over the place, right?
[1938.48 --> 1939.94]  Like, we have the operating system guy.
[1940.04 --> 1942.46]  We have the supervisor people.
[1942.58 --> 1943.92]  We have the front-end people.
[1944.04 --> 1948.08]  And so we're actually very thinly spread because there's just so much happening.
[1948.82 --> 1949.46]  For sure.
[1949.76 --> 1949.94]  Yeah.
[1950.20 --> 1957.68]  Yeah, it's both a lot of people from when you started at one, but it's also not a lot of people for the scope of work there is out there.
[1957.68 --> 1958.12]  Exactly.
[1958.88 --> 1962.30]  Can you even imagine how many people, you know, a commercial entity?
[1962.46 --> 1968.94]  Let's just hypothetically say you were owned by EA or some massive conglomerate like that, right?
[1969.06 --> 1972.74]  How many people would they employ to write a piece of software like Home Assistant?
[1972.94 --> 1976.10]  And it's just, to me, that speaks to the power of open source, right?
[1976.18 --> 1980.64]  I mean, we couldn't have things in the world like Home Assistant without open source.
[1980.64 --> 1982.02]  No, I think so.
[1982.12 --> 1987.30]  I mean, there's just, you know, we get people from, like, all over the place.
[1987.38 --> 1990.00]  They're brilliant programmers, but they have their day jobs.
[1990.38 --> 1992.18]  And, like, you know, it's funny.
[1992.30 --> 1993.72]  We have a couple of people.
[1994.26 --> 1995.86]  One is a CEO of a company.
[1996.12 --> 1998.20]  The other is, like, a director of software engineering.
[1998.34 --> 1999.14]  So he's, like, a manager.
[1999.68 --> 2002.40]  And, like, they just don't get to code at work anymore, right?
[2002.44 --> 2004.16]  So they come home and they're like, well, f*** it.
[2004.76 --> 2005.54]  I'm going to have it.
[2006.58 --> 2007.36]  Yeah, absolutely.
[2007.44 --> 2007.70]  I agree.
[2007.70 --> 2020.24]  And also those sorts of people who have had a lot of training in programming and stuff like that in the past, they've got a lot that they can bring to the table, but their motivation might be sporadic.
[2020.74 --> 2024.52]  And, you know, it's not really suitable to do a full-time job that way.
[2024.62 --> 2030.08]  But absolutely, you can contribute, you know, a couple of weeks' worth of evenings of your brain to an open source project.
[2030.54 --> 2033.92]  Well, I mean, that's how our core was originally all in threads.
[2034.12 --> 2035.86]  And, like, we had, like, deadlocks all the time.
[2035.86 --> 2040.82]  And then somebody came along who works in Mozilla, and he had a lot of Python experience.
[2041.06 --> 2042.62]  He made, like, pylons in the past.
[2042.86 --> 2047.10]  And, yeah, he rewrote our core to async.
[2047.32 --> 2049.84]  And that's what we still run today, and that's why we're so fast.
[2050.32 --> 2052.44]  So that's just a random guy that came along.
[2053.04 --> 2065.14]  You know what else I love as well about the number of people you've just shared work for Nebukasa is the fact that that means that somebody like a Mozilla isn't needed to come out and buy you out to keep you sustainable.
[2065.14 --> 2068.94]  It's a self-sustaining funding model you've created here.
[2069.04 --> 2069.64]  I think that's great.
[2069.96 --> 2070.10]  Yeah.
[2070.10 --> 2071.30]  No, it's been really great.
[2071.40 --> 2078.12]  I think, you know, we have no investors and no loans and these kind of stuff because it misaligns incentives, right?
[2078.18 --> 2080.16]  Because, you know, they want, like, return on investment.
[2081.52 --> 2081.72]  Yeah.
[2081.80 --> 2083.68]  I mean, it's working great so far.
[2083.68 --> 2091.76]  I mean, I expect as the pandemic, like, wees off that maybe people are spending less time at home, maybe spending less time on home assistance.
[2091.92 --> 2092.36]  Who knows?
[2092.94 --> 2094.70]  But they might need remote access.
[2095.06 --> 2095.52]  That's true.
[2096.36 --> 2096.72]  You know?
[2096.72 --> 2114.10]  I mean, I happily, happily pay that because I think it's a – not only is it a fantastic service and I like how you are implementing it, but I also appreciate sort of the virtuous cycle of it incentivizes the company to make home assistance better, which just continues to drive more value to my subscription.
[2114.54 --> 2118.12]  And it's legitimately one of those arrangements that I happily pay.
[2118.58 --> 2118.94]  That's awesome.
[2118.94 --> 2119.92]  Yeah, same.
[2120.02 --> 2121.10]  I don't really need it.
[2121.18 --> 2126.38]  I could quite happily set up my own reverse proxy with WireGuard and – in fact, I used to.
[2126.52 --> 2127.74]  And then Nebu Kasa came on.
[2128.00 --> 2128.26]  Yeah.
[2128.26 --> 2129.56]  That's the origin of the name, by the way.
[2129.64 --> 2132.10]  That word Nebu is quite unusual.
[2132.10 --> 2139.64]  So Nebu is – it was some god of the wisdom in some – somewhere in some religion or language.
[2141.28 --> 2142.84]  And so then we had, like, the word –
[2142.84 --> 2143.06]  Yeah.
[2143.56 --> 2143.82]  Okay.
[2144.16 --> 2144.90]  I like it.
[2145.14 --> 2148.12]  And then we also have the URL nabu.kasa, right?
[2148.12 --> 2150.88]  Because that actually – we kind of set it on Nabu.
[2150.96 --> 2153.46]  And then I was looking at domains and all of a sudden I said Nabu Kasa.
[2153.56 --> 2154.86]  And I was like, that's it.
[2155.38 --> 2157.80]  So it essentially comes down to Wise House.
[2158.10 --> 2159.96]  Is that – that's great.
[2160.22 --> 2160.60]  That is good.
[2160.66 --> 2160.82]  Yeah.
[2160.92 --> 2161.94]  And now we're waiting.
[2162.12 --> 2166.96]  Razer had a smartwatch called Nabu in 2015 or 16 or something.
[2167.38 --> 2169.62]  And we're just waiting for their trademark to lapse.
[2170.22 --> 2171.12]  Maybe we can –
[2172.26 --> 2175.06]  Get a little more mileage out of that name.
[2175.36 --> 2176.20]  That's great.
[2176.20 --> 2178.78]  I mean, I know lawyers have a reputation.
[2179.04 --> 2183.36]  But can you confuse a house automation system and a watch?
[2184.24 --> 2185.72]  You know, smartwatches.
[2185.76 --> 2187.70]  Smartwatches you can talk to nowadays.
[2189.08 --> 2189.92]  And so –
[2189.92 --> 2190.14]  Yeah.
[2190.20 --> 2191.58]  Who wants to even worry about a fight?
[2191.72 --> 2192.42]  Why just – yeah.
[2192.80 --> 2192.96]  Yeah.
[2193.60 --> 2196.64]  But, boss, thank you so much for joining us and updating it on these things.
[2196.64 --> 2205.44]  And also thank you and thanks to the team for making a piece of software that has improved my family's quality of life on a daily basis.
[2205.70 --> 2208.80]  Not much actually touches our lives in that way.
[2209.14 --> 2210.58]  So we're just really grateful for that too.
[2210.80 --> 2210.98]  Awesome.
[2211.08 --> 2211.62]  Well, you're welcome.
[2211.62 --> 2214.80]  So I hope you enjoyed that interview with Paulus.
[2214.96 --> 2218.66]  Now, we're not going to actually do any feedback this week just in the interest of time.
[2218.88 --> 2226.48]  But next episode, we're going to discuss the distributed file system question that Chris posed last week.
[2226.50 --> 2229.40]  We've had lots of feedback in the mailbag about that one.
[2229.40 --> 2232.62]  Oh, I can't wait to see what people have suggested.
[2233.10 --> 2235.36]  I feel like I'd be cheating if I read ahead.
[2235.48 --> 2237.36]  But now I kind of want to go in there and take a look.
[2237.90 --> 2238.70]  But I'll wait.
[2238.80 --> 2239.14]  I'll wait.
[2239.18 --> 2239.96]  I'll wait for the show.
[2240.28 --> 2241.92]  So that way my reaction is fresh.
[2242.06 --> 2242.34]  Awesome.
[2242.76 --> 2242.88]  Yeah.
[2242.90 --> 2252.94]  If you have any tips, selfhosted.show slash contact on how you could take advantage of the random amounts of free space on the hard drives all around your LAN.
[2253.24 --> 2256.74]  And thank you to our members at selfhosted.show slash SRE.
[2256.74 --> 2260.36]  You can support the show and become a member at selfhosted.show slash SRE.
[2260.56 --> 2265.24]  And you get a limited ad feed, full production, just a little bit tighter and cleaner.
[2265.70 --> 2269.88]  Extra content at the end of the show as well with a special members only post show.
[2270.02 --> 2272.04]  And thanks to our sponsor, Cloud Guru.
[2272.12 --> 2274.02]  You can find them on social media everywhere.
[2274.20 --> 2275.74]  That's basically a social media site.
[2276.04 --> 2277.64]  They're just slash a cloud guru.
[2277.84 --> 2278.82]  That's really simple.
[2279.24 --> 2282.82]  And as always, you can find me over on Twitter at ironicbadger.
[2282.92 --> 2286.18]  And the show is selfhosted.show slash contact.
[2286.18 --> 2286.66]  Indeed.
[2286.88 --> 2289.58]  I'm over on the Twitter as well at Chris Elias.
[2289.72 --> 2293.54]  And the podcast is over there too at selfhosted.show for news and announcements.
[2294.04 --> 2294.88]  Thanks for listening, everybody.
[2295.08 --> 2297.20]  That was selfhosted.show slash 45.
