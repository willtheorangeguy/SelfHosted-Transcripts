[0.00 --> 3.32]  Coming up on today's show, we discuss the Home Assistant Security Bulletin.
[3.76 --> 9.58]  I've got some pretty cool Bluetooth low-energy OLED temperature sensors for you from Xiaomi,
[10.00 --> 12.62]  and we get philosophical in the feedback section. I'm Alex.
[12.98 --> 15.74]  I'm Chris, and this is Self-Hosted 37.
[16.92 --> 20.74]  You know, it was only the last few weeks I realized that we just sort of blew right past
[20.74 --> 22.38]  our one-year anniversary in September.
[22.92 --> 23.74]  We're one.
[23.98 --> 28.74]  Yeah, and I think it was just because we were doing the whole going independent thing again.
[28.74 --> 30.66]  And so we just had a lot on our plate.
[30.96 --> 32.66]  What's your opinion on first birthdays?
[32.96 --> 36.26]  I think the show's been really well-received, and it seems like it's still growing,
[36.42 --> 38.04]  but it's found its audience.
[38.52 --> 41.80]  And I think it's a good first year, especially because we're not weekly.
[42.10 --> 45.36]  And so for some podcasts, that can be rough, but it doesn't really seem to have held us back.
[45.72 --> 49.26]  I wasn't talking about that. I was talking about kids, first birthday.
[49.50 --> 52.76]  Do you make a whole big deal about it? Because obviously, they're not going to remember it.
[53.00 --> 54.20]  That's true. That's true.
[54.20 --> 58.84]  Yeah, I don't know. I feel like for podcasts, it's a good sign that it's a stable podcast,
[59.20 --> 66.20]  but there's like kind of this, the real, I think, real landmark for a podcast is five years.
[66.32 --> 67.94]  That feels like the one you celebrate to me.
[68.40 --> 71.76]  Yeah, you've done a few that have reached episode 300. I think for me, that's a big number.
[72.14 --> 77.04]  Yeah, that's also a pretty big one. Yeah, so congratulations, though, on the anniversary.
[77.16 --> 80.92]  We thought this seems like the perfect episode to follow up on a lot of things because of that.
[80.92 --> 87.34]  You know, it's going to take us 11 and a half years, twice a month, to reach episode 300.
[89.02 --> 93.02]  Maybe we'll have to step it up at some point. Maybe we'll go daily for a last little bit.
[93.74 --> 98.94]  We have flirted with the idea of weekly, but you know, with going indie, you've had so much on your plate again.
[99.70 --> 102.50]  It's not really been feasible for both of our schedules yet.
[102.86 --> 107.64]  Yeah, life is busy, but you never know. Things change in the future, but right now we don't have many plans to change it.
[107.64 --> 113.00]  We have discussed it from time to time. The future is, well, it hasn't happened yet.
[113.62 --> 120.32]  But this episode has happened. It's happening right now, and it's brought to you by a Cloud Guru, the leader in learning for Cloud Linux and other modern tech skills.
[120.70 --> 126.82]  Hundreds of courses, thousands of hands-on labs. Get certified, get hired, get learning at cloudguru.com.
[126.82 --> 134.98]  I got a rather alarming set of emails and Reddit posts from the Home Assistant project this week about a security bulletin.
[135.72 --> 143.62]  And I wanted to get your take on how they're handling it, because to me it seems like controlled, well, not even controlled. It just seems like chaos over there.
[143.98 --> 149.06]  Yeah, they're really trying to get the word out. That's one of the reasons, I think by now, when this episode comes out, people will know about it.
[149.06 --> 154.56]  But just because this seems to be really important, I even got a notification again this morning via their Discord community.
[155.08 --> 158.18]  So there was a security bulletin put out by the Home Assistant project.
[158.18 --> 171.20]  We will have the blog post linked in our show notes, but there's not much to it, other than it just strongly encourages you to update as fast as possible and spread the word as far as possible.
[171.50 --> 180.00]  There is a specific callout in the blog post to an issue with custom components, which are not reviewed by the core Home Assistant team.
[180.00 --> 184.04]  But otherwise, there's really zero information in the bulletin as we record.
[184.16 --> 186.16]  This is several days after the bulletin as well.
[186.70 --> 192.84]  We were told there would be an update with more information, but it so far hasn't shown up anywhere.
[193.78 --> 204.98]  However, we do have several questions that we'd like to have answered, like which integrations were leaking stuff, under which circumstances were those integrations leaking stuff, and does the update that's been released fully address those issues?
[204.98 --> 210.32]  Or, as some are speculating right now, is it just merely mitigating them?
[210.80 --> 215.30]  Will there still be some risk after updating if we use whatever integration this supposedly was?
[215.34 --> 220.42]  So there's definitely questions that haven't been properly answered by the Home Assistant project right now.
[220.96 --> 223.18]  I wonder if that's because they just don't have the answers yet.
[223.56 --> 224.64]  You speculate, really.
[225.30 --> 229.70]  And at this point, I want to just let the audience know we are recording this a couple of weeks ahead of time.
[229.92 --> 232.56]  I've got some personal stuff coming up, so it's unavoidable.
[232.56 --> 240.04]  But, you know, from my perspective, I want to see like CVE-style clarity here.
[240.20 --> 241.38]  I want to know what the problem is.
[241.46 --> 244.50]  I want to know what they've done to fix it or that they haven't fixed it.
[244.66 --> 253.62]  I actually don't necessarily mind if they haven't because at least I know what the problem is, so I could maybe go and try and contribute to creating a fix, perhaps.
[254.06 --> 255.02]  Yeah, I'm sure they're very busy.
[255.44 --> 260.64]  But there are basic questions like if I didn't use any custom components, do I have any cause for concern?
[260.64 --> 269.34]  Now, if you go by the code, because it's an open source project, it looks like maybe they caught that some nasty things were happening via the HTTP API.
[269.34 --> 274.52]  Seems like maybe they've added some basic filters to the code for some common web-based attacks.
[275.12 --> 276.66]  But really, the context matters here.
[276.74 --> 278.32]  So that's only something the project can provide.
[278.84 --> 290.94]  Yeah, I see some stuff in the code for one of the commits that's referenced in the forum post about the security bulletin about file injection attacks at certain web URLs as well as SQL injection protections and stuff like that.
[290.94 --> 292.92]  So who knows what's going on?
[293.48 --> 302.42]  This is where it's a really tricky balance, especially for an overburdened project and especially a new one that hasn't really had to deal with a security issue quite like this yet.
[302.92 --> 309.06]  There is a real high standard for a platform, a really high standard of clear communication.
[309.06 --> 314.88]  And even if that communication is a status update that they don't have the full report yet, it needs to be communicated.
[315.38 --> 316.84]  It's a hard lesson to learn.
[317.00 --> 318.76]  You also have to create process.
[319.12 --> 321.92]  It's a human problem as well as a process problem.
[322.44 --> 326.56]  But clear communication is critical for any kind of popular platform.
[327.42 --> 330.94]  And I know that they're very busy, but that's always going to be the case.
[330.94 --> 336.96]  And as more and more people integrate their homes and businesses around this, it's pretty important that we know what's going on.
[337.60 --> 342.80]  That's where the communication is probably going to be a bit of a learning opportunity in the future.
[342.98 --> 350.72]  But it also reminds me that they're still, you know, as far as a project goes of this scope, relatively young.
[351.34 --> 354.12]  And they still have things that they're going to have to figure out.
[354.12 --> 364.80]  And it's not why it's a knock when I say this, but it sort of speaks to why I'm not a huge fan of their entire integrated approach with the OS and Home Assistant and the supervisor.
[365.44 --> 370.50]  I'm not a huge fan of this project building an OS.
[372.04 --> 381.38]  With these types of security things, with the underlying platform, that's just an area I'd like to outsource that work to the folks at Canonical, Red Hat, or Debian.
[381.38 --> 385.12]  I just don't really prefer having the project control the entire stack.
[385.46 --> 389.12]  I understand why they do it, and it's an entirely separate conversation.
[389.30 --> 397.68]  But it's one of my arguments why I hope they keep making it possible for folks like me to deploy the entire Home Assistant experience on the OS of my choice.
[398.02 --> 406.86]  Because just for my personal comfort and just the way I view the world, I like to know that a vendor like Red Hat or Canonical is behind the server OS that I'm using.
[406.86 --> 416.36]  I mean, I see on a daily basis at work, a lot of the stuff that goes on behind the curtain of maintaining a kernel, of maintaining a Kubernetes distribution and that kind of stuff.
[416.48 --> 418.68]  And it's an astronomical amount of work.
[419.00 --> 420.14]  And I've got to agree with you.
[420.14 --> 440.46]  I think if the project were to take the limited resources that they have and kind of share them out in their area, well, not share them out, but like delegate the responsibilities of the more complex tasks like building an OS to vendors whose day job it is and who have 25 plus years.
[440.58 --> 443.70]  I'm looking at Debian experience in doing this kind of stuff.
[443.70 --> 449.16]  And then they can focus on what they're good at, which is building a brilliant home automation platform.
[449.58 --> 450.84]  But to their credit, they caught this.
[450.98 --> 456.66]  And the other thing I think they've done right in this process is they have communicated the need to upgrade.
[456.88 --> 464.52]  They haven't been particularly great about communicating why other than security, but they have been very good at getting the word out.
[465.20 --> 469.34]  And there is a pretty safe process to do that upgrade.
[469.34 --> 473.86]  So I decided to do it over the weekend so that way I could report back here on the show.
[474.48 --> 480.44]  And my setup is it's Ubuntu 2004 running on a Raspberry Pi 4.
[480.78 --> 487.56]  I can't even remember how I set it up now, but I have the full supervised home assistant setup so I can install the add-ons and take snapshots.
[487.98 --> 491.88]  And I really love that setup, even though it's not technically a supported setup anymore.
[492.18 --> 495.72]  But I went into my home assistant supervisor and I clicked update.
[495.72 --> 498.44]  Well, first I took a snapshot, actually, did the snapshot.
[498.64 --> 512.42]  And whenever I'm doing something that may introduce a breaking change, because it wasn't clear here, if there was an issue with custom integrations, I thought it's possible they just disabled custom integrations until they have this thing fixed.
[512.60 --> 514.80]  And so I thought, this could be a breaking update.
[514.88 --> 515.32]  I don't know.
[515.54 --> 517.28]  There's not really been any information about that.
[517.28 --> 522.50]  So I took a snapshot and then I downloaded that snapshot to my local hard drive, just in case.
[522.96 --> 526.84]  Then I head over to the update button, click the update, nothing happens.
[527.38 --> 529.66]  Click it again, nothing happens.
[529.96 --> 533.16]  And it's not exceptionally good at communicating status.
[533.46 --> 534.92]  So I SSH into the server.
[535.08 --> 537.16]  Again, I love that it's a server I can just get access to.
[537.20 --> 538.78]  And I have things like Bashtop installed.
[539.12 --> 540.70]  And I run Bashtop and Htop.
[540.76 --> 541.42]  And I get an idea.
[541.54 --> 543.80]  It's like, is there anything happening in the background?
[543.80 --> 546.32]  And I pretty quickly determine nothing's happening.
[547.12 --> 550.12]  So I turn to an integration that I have.
[550.14 --> 555.26]  And this is one of the reasons I wanted the full Home Assistant experience and not just Home Assistant core.
[555.80 --> 571.32]  Because there's integrations like the upgrade configuration checker that will download the latest version of Home Assistant, do a fake contained install, and then check it against your config YAML and tell you if there's anything that's going to break in the upgrade.
[571.32 --> 572.86]  So I thought, I'll run that.
[573.30 --> 574.26]  Only it broke.
[574.46 --> 583.28]  And I had to go digging for the logs on the file system to discover that there was some issue with, quote, custom integration, quote, but they didn't say which integration it was.
[583.64 --> 586.26]  So I didn't really know what was going to happen.
[586.38 --> 593.70]  But I decided for the good of the show, I'd pull the trigger, and I did the update, and it still did nothing.
[594.38 --> 595.20]  Okay, what's going on?
[595.36 --> 597.30]  So the configuration check failed.
[597.60 --> 599.14]  The update has failed.
[599.14 --> 601.26]  There must be something wrong.
[601.54 --> 605.78]  So I reboot the whole machine, figure, let's just get that out of the way.
[606.28 --> 607.48]  Home Assistant loads back up.
[607.54 --> 608.62]  I verify functionality.
[608.92 --> 609.98]  I go into Supervisor.
[610.12 --> 613.36]  I hit the update button, and I start to get the circle of progress.
[613.84 --> 616.44]  It starts working all of a sudden, even though I hadn't changed anything.
[616.50 --> 617.20]  I just did a reboot.
[617.30 --> 621.10]  And the machine had only been rebooted about 24 hours ago, too, which I thought was kind of funny about it.
[621.62 --> 622.62]  It pulls it down.
[622.96 --> 623.92]  It does the update.
[624.02 --> 626.28]  And so far, I don't see any issue.
[626.38 --> 627.60]  I have now the latest version.
[627.60 --> 629.16]  Everything seems to be going just smooth.
[629.76 --> 632.18]  And I'm not quite sure why I had the problems with it updating.
[632.28 --> 634.46]  I'm not quite sure why my config check had problems.
[635.26 --> 637.30]  But everything's tested and working.
[637.84 --> 643.00]  The only time I've had issues with the config checker is when there's been an error in my config, actually.
[643.44 --> 643.72]  Yeah.
[643.72 --> 647.70]  I created an include that was pointing at a missing file or something.
[647.70 --> 652.72]  And rather than telling me that, the config checker just sat there and span and span and span.
[653.04 --> 658.92]  And it takes a while, too, on the Raspberry Pi because you're downloading it, which I don't have the fastest connection in the RV.
[659.46 --> 660.46]  So I wait for that.
[660.46 --> 660.96]  Oh, yeah.
[661.04 --> 662.20]  It can take a beat.
[662.28 --> 662.86]  That is true.
[663.04 --> 666.24]  At least I would say set aside two or three minutes.
[666.52 --> 666.64]  Yeah.
[666.70 --> 667.14]  Oh, yeah.
[667.46 --> 668.02]  Or more.
[668.30 --> 669.00]  Maybe 15.
[669.40 --> 670.24]  But you see the error.
[670.32 --> 671.70]  I put it there in the show notes for you.
[671.84 --> 675.26]  It just says invalid config for script integration.
[675.26 --> 677.84]  And then it's just blank.
[678.38 --> 679.58]  And it says not found.
[679.96 --> 681.26]  Two quotes that are just empty.
[681.44 --> 681.94]  Very helpful.
[682.12 --> 682.28]  Yeah.
[682.76 --> 684.02]  So I'm going to pull it up.
[684.28 --> 686.78]  It says it's on line 21, so I know where to go look.
[687.04 --> 690.96]  But I decided to run the update since I had a snapshot and everything went through.
[691.16 --> 694.14]  I have the latest version and it's working perfectly fine.
[694.48 --> 702.50]  But I do kind of wonder what that custom integration airs about and if it's related to some of the fixes they just did since their fixes are related to custom integration.
[702.50 --> 705.58]  So I'll be diving deeper into that into the future.
[705.94 --> 708.44]  But have you decided to pull the trigger on the upgrade for you?
[708.84 --> 715.40]  Well, I mean, I was I was quite busy the other night and I just saw the notification come through and was like, oh, so I just hit upgrade.
[715.46 --> 716.38]  I don't have time to check.
[716.82 --> 719.64]  I subscribed through the Nabucasa app.
[719.76 --> 726.00]  So technically, my install is Internet facing, even if you have to guess a very long obfuscated URL.
[726.32 --> 727.48]  When did you start doing that?
[727.50 --> 728.24]  I didn't know that.
[728.36 --> 730.10]  Well, I started supporting the project.
[730.10 --> 737.10]  That was the reason I actually started paying for it was was really to support development, not necessarily because I wanted the remote features.
[737.18 --> 742.02]  But it actually turned out to be pretty handy because, you know, with with COVID, I haven't really left the house that much.
[742.02 --> 745.94]  So I haven't had the need to SSH into my house remotely very much.
[746.64 --> 752.14]  And I got to where I was going and found out I couldn't connect to my house to pass the time or whatever.
[752.14 --> 768.40]  And so I opened up Home Assistant in the phone app, looked at the URL, typed that into on my on my laptop and then used the VS Code plugin with the built in shell to create the SSH keys I needed.
[768.52 --> 769.12]  And I was good to go.
[769.56 --> 772.30]  That's a great little example of how all that stuff can really come together.
[773.06 --> 773.24]  Yeah.
[773.30 --> 774.32]  So I got the update loaded.
[774.32 --> 782.86]  I haven't actually updated the version on my Home Assistant Blue hardware at the studio, but I'm, you know, more a couple of weeks into using that and I'm still loving that as well.
[783.14 --> 784.36]  I'm grateful they're doing the update.
[784.82 --> 785.80]  What do you use for snapshots?
[786.04 --> 788.30]  I use the built in supervisor tool that does the snapshots.
[788.58 --> 791.06]  Have you come across the Google Drive backup plugin?
[791.46 --> 792.50]  I don't think I have.
[792.72 --> 792.96]  No.
[793.10 --> 794.56]  It's not in the main store.
[794.56 --> 798.26]  I'm pretty sure it's an external thing, but it is awesome.
[798.58 --> 810.94]  So I think in the self-hosted live hack that we did a few months ago, I showed it off there where I basically took a completely fresh install of Home Assistant, applied the snapshot, which was taken by this Google Drive plugin.
[811.32 --> 814.50]  So it automatically does stuff like snapshot rotation.
[814.50 --> 818.74]  So you can have a daily, a weekly, a monthly, yearly snapshot, that kind of thing.
[818.88 --> 819.28]  Really?
[819.50 --> 821.88]  I can have up to seven days and four months or whatever.
[822.06 --> 822.86]  You got to link this.
[822.98 --> 823.76]  You got to link this up.
[823.76 --> 824.58]  I got to check this out.
[824.76 --> 825.00]  All right.
[825.04 --> 827.48]  Yeah, it's pretty slick and it obviously integrates with Google Drive.
[827.66 --> 832.06]  So, you know, each snapshot's 200 megs or so in my setup.
[832.50 --> 834.32]  So it doesn't really take much storage.
[835.88 --> 837.74]  Linode.com slash SSH.
[837.82 --> 841.56]  Go there to get a $100 60-day credit and support the self-hosted podcast.
[842.26 --> 843.84]  Linode is our server provider.
[843.84 --> 848.78]  Whenever we're building something for the show or my personal infrastructure and now JB 3.0's infrastructure.
[849.46 --> 851.42]  Yeah, it's all up on Linode.
[851.42 --> 854.30]  And gamers, Linode is your DIY of choice.
[854.30 --> 863.04]  They make it really easy and there are plenty of simple one-click deployments for things like Minecraft and CSGO servers.
[863.16 --> 868.32]  That's a really simple way and a really nice and fast way to get a nice private gaming space.
[868.32 --> 876.00]  And they will have you fill out like just some of the basics you need to get some of the fundamental server options set and they'll deploy it pre-configured for you.
[876.24 --> 877.34]  So make sure you check that out.
[877.42 --> 882.00]  Every plan comes with Linode's amazing human-powered customer support.
[882.00 --> 888.20]  We've had story after story from our audience of great experience with Linode's customer support.
[888.32 --> 893.48]  You can email, you can hit them up on social media, you can pick up a phone and talk to an actual human.
[894.10 --> 895.00]  How about that?
[895.30 --> 896.08]  I mean, Linode gets it.
[896.10 --> 897.56]  They've been around for a long time.
[897.90 --> 901.28]  They started in 2003 as one of the first companies in cloud computing.
[901.62 --> 904.98]  Three years before AWS and other enterprise providers.
[905.26 --> 909.06]  And they're independently owned and they're founded on a love for Linux and open source technologies.
[909.06 --> 911.80]  And they really support the community that surrounds them.
[911.90 --> 919.46]  Like this show, like the Kubuntu project, like LinuxFest Northwest, which you know is very special to us.
[919.92 --> 920.94]  Linode's a supporter of them.
[921.30 --> 926.58]  But you get a $100 credit when you go to linode.com slash SSH.
[926.70 --> 929.84]  So you can play around with their really powerful systems if you want.
[930.20 --> 932.46]  Try out building some tools around object storage.
[932.68 --> 935.48]  It's a great opportunity to experiment with different stacks.
[935.48 --> 940.68]  That's one of the things I've done on Linode is I tried several different WordPress stacks to see which one I like.
[940.78 --> 945.14]  You know, with Nginx or I even tried a web browser where everything runs out of RAM.
[945.24 --> 951.12]  And they have all of this stuff that is just ready to go as configuration scripts that you can just kick off and get going.
[951.68 --> 952.76]  It's really simple.
[953.42 --> 955.32]  And they also offer a lot of powerful tools.
[955.42 --> 956.78]  They don't hide that stuff from you either.
[957.12 --> 957.68]  So try it out.
[957.92 --> 959.92]  Linode.com slash SSH.
[959.92 --> 968.18]  How often do you ask yourself the question, when does it make sense to build versus buy a solution?
[968.54 --> 972.06]  I mean, a lot of times that's one of the first or second questions I ask myself.
[972.16 --> 973.70]  I very frequently do that math.
[973.90 --> 974.88]  You must as well.
[975.26 --> 978.82]  Yeah, what's particularly annoying is that I actually built a solution last year.
[979.12 --> 986.56]  And there's a solution I can now buy that is so much better for half the price that I'm kind of sat here going,
[986.80 --> 988.64]  I wish I hadn't built one now.
[988.64 --> 990.46]  Yeah, it's tricky, right?
[990.50 --> 995.26]  Because things like temperature sensors and humidity sensors, you might end up wanting a lot of them.
[995.52 --> 995.96]  You do, yeah.
[996.06 --> 999.30]  So, I mean, probably every single room is a bit of overkill.
[999.48 --> 1006.86]  But certainly at the other end of the spectrum, just a single thermostat as a single point of measurement in a house is,
[1007.30 --> 1009.38]  I've always, it's always struck me as weird.
[1009.62 --> 1011.16]  It's absolutely nutty.
[1011.24 --> 1014.20]  It's even nutty in a tiny space like a tiny home or an RV.
[1014.20 --> 1018.74]  Yeah, because one room, if you shut a door, can get to, you know, several degrees higher than the hallway.
[1019.22 --> 1019.34]  Yeah.
[1019.76 --> 1022.56]  So, I'm holding in my hand up to the camera so you can see it.
[1022.90 --> 1024.84]  This is the little temperature sensor I've bought.
[1025.02 --> 1026.14]  It's from Xiaomi.
[1026.46 --> 1029.88]  So, it's a Bluetooth low energy temperature sensor with an OLED screen.
[1030.56 --> 1032.08]  There'll be a picture of it in the show notes.
[1032.08 --> 1037.12]  It's about the size of three or four keys on my keyboard square.
[1037.26 --> 1038.32]  So, it's pretty small.
[1038.46 --> 1039.96]  Fits in the palm of my hand very comfortably.
[1040.90 --> 1047.30]  And they supply these things with a small little piece of adhesive tape that you can use to just stick it on the wall anywhere.
[1047.86 --> 1049.06]  They're fully battery powered.
[1049.06 --> 1054.24]  They connect to an ESP32, which you flash with ESP Home.
[1054.76 --> 1061.70]  You give it the Bluetooth MAC address of this device and then ESP Home will connect to these sensors.
[1062.26 --> 1063.26]  There is a catch.
[1063.80 --> 1066.38]  You need to flash a custom firmware on the sensors as well.
[1067.08 --> 1072.82]  So, expect to set aside an evening to do this if you're flashing, you know, half a dozen sensors or so.
[1073.20 --> 1076.92]  But the best part is that it's $9 for a four pack of these sensors.
[1077.42 --> 1077.88]  No.
[1078.88 --> 1080.50]  With the screen on there?
[1080.54 --> 1081.82]  I mean, that's what I love about them.
[1082.06 --> 1082.40]  I know.
[1082.86 --> 1083.70]  It's crazy, isn't it?
[1083.76 --> 1087.68]  I have very expensive temperature sensors that'll do all kinds of fancy things.
[1088.12 --> 1091.58]  But, you know what they don't do is they don't actually just display the temperature on them.
[1091.58 --> 1096.58]  And, in a way, that's a killer feature because you get the context right there for the room you're in.
[1096.68 --> 1098.12]  And it's also being fed to Home Assistant.
[1098.44 --> 1104.86]  The temperature and the humidity on the screen, which in the southeast of the U.S., humidity is the bane of my life.
[1104.86 --> 1107.02]  So, yeah.
[1107.12 --> 1109.16]  So, you want to keep an eye on that damn thing.
[1109.38 --> 1109.50]  Yeah.
[1109.50 --> 1113.70]  How long would you say for four of them to get that flashing process done?
[1113.70 --> 1120.44]  Well, there's actually a really slick sort of web configurator thing built into the GitHub repo that's linked in the show notes.
[1120.76 --> 1122.24]  So, what you do is you fire up your phone.
[1122.36 --> 1124.32]  You connect your phone's Bluetooth to this thing.
[1125.06 --> 1126.72]  Flash the firmware through a web browser.
[1126.72 --> 1129.90]  And then listen for the MAC address in the logs that way.
[1129.98 --> 1132.36]  And then paste that into the ESP Home configuration.
[1132.92 --> 1134.86]  And flash that to your ESP32.
[1135.18 --> 1136.54]  It sounds like a lot of steps.
[1136.94 --> 1140.28]  But it really isn't that bad if you're familiar with ESP Home.
[1140.68 --> 1142.16]  Doesn't sound bad at all, actually.
[1142.42 --> 1143.34]  Sounds quite doable.
[1143.62 --> 1144.14]  Yeah, very slick.
[1144.22 --> 1145.18]  I've been very impressed with it.
[1145.42 --> 1149.30]  I think I came across this first on the Intimate.tech YouTube channel.
[1149.38 --> 1150.78]  We had him on a few episodes ago.
[1151.40 --> 1152.58]  The Quinn LED guy.
[1153.08 --> 1154.36]  They just seem to work really well.
[1154.36 --> 1160.22]  I had a couple of Bluetooth dropouts with the ESP32s being on a different end of the house.
[1160.34 --> 1165.78]  So, I've ended up buying four ESP32s, which is the most expensive part of the setup.
[1166.52 --> 1168.98]  One on each floor, at each end of each floor.
[1169.54 --> 1172.52]  And they're basically stacked on top of each other, each end of the house.
[1173.28 --> 1179.66]  So, I mean, even at $11 each on Amazon for an ESP32, we're not talking crazy amounts of money.
[1179.86 --> 1184.12]  And you can definitely order them a lot cheaper than that on AliExpress if you're willing to wait for the slow boat.
[1184.36 --> 1187.62]  So, now that you're getting the temperature data, what are you going to do with it?
[1187.62 --> 1188.74]  Are you going to do any automations?
[1188.92 --> 1191.40]  Because that's, I mean, that's really where it gets next level.
[1191.90 --> 1192.60]  Yeah, I want to.
[1192.72 --> 1194.26]  I haven't quite figured it out yet.
[1194.38 --> 1196.94]  So, we're going to talk more about this in the post-show, I think.
[1197.02 --> 1201.52]  We've got something in there about thermostats and the Venn style unit that I use.
[1201.52 --> 1206.84]  But what I want to do is take the average, and this is something Dr. Z does a lot of.
[1207.12 --> 1213.44]  He takes the average of several sensors and then uses that as his thermostat input number.
[1213.78 --> 1219.36]  What I would like to see is I take the average across the entire top floor of my house, for example,
[1219.36 --> 1222.36]  and then use that as the input to the thermostat.
[1222.36 --> 1228.54]  I haven't figured out how to use a custom input with a thermostat that has an integration.
[1229.02 --> 1233.12]  You can do that with the generic thermostat module of Home Assistant,
[1233.36 --> 1238.80]  but I haven't quite joined all the dots up to make it work with a pre-configured one.
[1239.20 --> 1240.50]  Justin wrote into the show.
[1240.50 --> 1246.94]  So, he said he was actually writing in because on Coder Radio, which, by the way, not this podcast.
[1247.44 --> 1248.02]  Where's my robe?
[1248.24 --> 1249.46]  Yeah, I'm working on it.
[1249.82 --> 1251.64]  I am wearing the minimum viable robe at the moment.
[1251.88 --> 1256.62]  I was talking to Mike about his problems with he moved into a new place and it comes with a smart thermostat,
[1257.16 --> 1259.32]  and it's been freezing him out at night.
[1259.62 --> 1261.84]  And mine has my system every now and then.
[1262.76 --> 1266.42]  Something happens and the automation triggers don't fire and I cook out.
[1266.42 --> 1267.34]  I get too hot.
[1267.50 --> 1268.74]  A heater doesn't get turned off.
[1268.74 --> 1274.76]  And I generally, this fix has always just been, I reboot my Home Assistant host,
[1274.94 --> 1277.16]  and then it doesn't happen for another couple of weeks.
[1277.32 --> 1281.06]  But Justin wrote into the show and he said, you'd mentioned that failed automation.
[1281.38 --> 1284.24]  Home Assistant, like you were just talking about, Alex, he says,
[1284.68 --> 1287.60]  has a generic thermostat component and it is fantastic.
[1287.80 --> 1289.86]  I use it in several rooms of our house.
[1290.16 --> 1295.32]  You provided a temperature sensor and a switch and the component handles all of the rest.
[1295.32 --> 1302.34]  It looks like there's some affordance for it understanding if you want something in a target temperature,
[1302.34 --> 1307.28]  that it might need to kick in a little bit at a different time in order to actually get that temperature just right.
[1307.36 --> 1313.78]  Like it seems clever and like a way better idea than me completely building this automation from scratch like I have been.
[1313.78 --> 1317.16]  So when you do go down that route, I agree with listener Justin.
[1317.40 --> 1318.66]  Check out the generic thermostat.
[1319.20 --> 1320.98]  Yeah, I need to connect those dots for sure.
[1321.10 --> 1327.12]  I mean, in my specific situation, the room above my garage happens to be where we spend most of our time.
[1327.58 --> 1331.60]  And if I close the door to the hallway on this room and the heat is running,
[1332.20 --> 1336.32]  it can easily get four or five Celsius higher in this room than the hallway.
[1336.32 --> 1339.82]  When the forced air is blowing, it gets very dry, the air,
[1339.94 --> 1342.98]  and the static electricity becomes a bit of a problem and stuff like that.
[1343.10 --> 1348.98]  So what I really want is just a way to use that sensor that I'm looking at right now in this room
[1348.98 --> 1351.66]  as the dedicated input to the thermostat.
[1351.74 --> 1353.82]  If I can use an average, then, well, even better.
[1353.94 --> 1356.78]  But what I absolutely want is an automation that fires
[1356.78 --> 1362.40]  when that particular sensor gets above a certain threshold that it just doesn't turn off the heating
[1362.40 --> 1363.56]  because that's not what I want.
[1363.56 --> 1368.56]  I just want it to stop heating me for a bit right now and then evaluate things in 10 minutes
[1368.56 --> 1372.58]  and figure out whether it needs to still keep blasting us with the heat or not.
[1373.04 --> 1380.82]  And to add an extra layer of complication, if it could also be somehow energy efficient aware,
[1381.16 --> 1386.16]  so if you were running off grid or maybe in your case you have like a Tesla Powerwall
[1386.16 --> 1388.28]  and the grid was down and you were running off battery,
[1388.54 --> 1393.00]  if the system could adjust to use less power but still maintain a minimum comfort,
[1393.00 --> 1394.46]  that'd be the next level.
[1394.70 --> 1396.88]  You know, like that's what I really want now for Joops.
[1397.32 --> 1398.56]  That's our next business idea.
[1398.96 --> 1400.44]  You know, we had cloudfree.shop.
[1400.90 --> 1406.80]  You know, the next one is this sort of mega thermostat that beats the pants off the nest.
[1407.12 --> 1407.44]  Right.
[1407.92 --> 1412.76]  So Jim wrote into the show and he wants just our thoughts on going solar.
[1412.88 --> 1416.88]  He says, I'm looking for solar for my home and I'm not really sure where to start looking.
[1416.88 --> 1420.46]  Everywhere I go, I get bombarded with ads and people who seem like salesmen.
[1420.96 --> 1423.52]  I've looked at businesses like Tractor Supply and other sources,
[1423.72 --> 1426.90]  but I worry about what they're selling and if they're actually the best tech.
[1427.60 --> 1430.04]  And he wonders what we did to look into this,
[1430.06 --> 1431.86]  because I know you've considered solar for the home,
[1431.94 --> 1433.62]  you've considered Powerwalls for the home.
[1434.48 --> 1438.90]  I'm curious what your route and trajectory is when you go off on a research binge for this.
[1439.30 --> 1443.28]  It's amazing how quickly you end up at the Tesla stuff when you start Googling this stuff.
[1443.28 --> 1446.68]  They must spend a lot on marketing or SEO or something.
[1446.68 --> 1452.22]  I ended up looking at getting, I think it was like 12 panels put on my roof.
[1452.32 --> 1456.28]  Ultimately, it ended up being too expensive to consider right now.
[1456.30 --> 1458.50]  And they weren't in North Carolina yet and stuff like that.
[1458.58 --> 1460.30]  So I haven't done it yet.
[1460.52 --> 1467.42]  It's definitely on my list because I do feel guilty about burning several hundred watts a day of permanent,
[1467.74 --> 1469.84]  you know, server electricity and stuff like that,
[1469.88 --> 1473.10]  that could very easily be supplied through solar.
[1473.10 --> 1477.32]  So, you know, part of it is I want to try and do my bit for the environment.
[1477.50 --> 1479.76]  But the other part is it'd be nice to save some money too.
[1480.20 --> 1482.90]  Yeah, the research of it for me has always kind of been,
[1483.26 --> 1487.16]  I try to find communities that are discussing the type of builds that I'm doing.
[1487.24 --> 1489.60]  So in my case, they're more mobile builds, but, you know,
[1489.78 --> 1491.82]  we just shift communities depending on the build.
[1492.20 --> 1496.14]  And then also YouTube tends to play a pretty significant role.
[1496.46 --> 1501.74]  And it's really a process of finding and refining the selection of YouTubers you find
[1501.74 --> 1502.64]  and getting their advice.
[1503.12 --> 1506.82]  I went to a company called AM Solar to have my mobile install done.
[1506.96 --> 1512.88]  And I did that through a process of reading lots of reviews about people's solar installs
[1512.88 --> 1517.62]  and finding forums where people were discussing getting solar installed
[1517.62 --> 1521.02]  and kind of narrowed it down to a few companies.
[1521.26 --> 1526.30]  And then, you know, had my geographic location and they were kind of within my striking distance.
[1526.30 --> 1531.02]  And then I went and looked up pictures of their work, which I think is another really good tip.
[1531.10 --> 1535.46]  If you can find any on their website or on Google Images, I went and found pictures of their work
[1535.46 --> 1538.12]  and thought that, you know, everything looked really good and tidy.
[1538.26 --> 1540.92]  And that was something that was important to me in this installs.
[1540.96 --> 1543.02]  I didn't want it to be just a ball of wires.
[1543.02 --> 1547.40]  I wanted it to look like it was maybe built from the factory that way.
[1547.78 --> 1549.02]  And they did absolutely that.
[1549.08 --> 1550.62]  So that was sort of my process.
[1551.18 --> 1554.88]  I don't know about you, but the more salesy a company is, the less interested I am.
[1554.88 --> 1557.82]  Yeah, and when it comes to that kind of stuff, too, it's easy to get scammed.
[1557.96 --> 1561.80]  So just take your time, you know, get multiple opinions on stuff.
[1562.20 --> 1564.48]  And the other thing is, and this is a very U.S.-centric comment,
[1564.70 --> 1569.78]  but there are some federal tax incentives that tend to expire at the end of each calendar year.
[1570.08 --> 1576.12]  So I noticed the number of texts I was receiving about sign up for solar now in December
[1576.12 --> 1577.70]  was a lot higher than it has been in January.
[1577.88 --> 1579.56]  So just factor that in as well.
[1579.78 --> 1580.58]  So Phil wrote in.
[1580.64 --> 1582.96]  He's a fan of your Perfect Media Guide.
[1582.96 --> 1584.74]  I think it's really helped him a lot.
[1584.88 --> 1589.70]  And he had questions about your VDEV configurations that you're using for the Perfect Media Server.
[1590.10 --> 1595.56]  From what I understand, if you use one disk per VDEV, there is no protection benefit for ZFS.
[1596.26 --> 1601.96]  I'm researching options for setting up a DIY NAS and need to have a cost to bring to the wife
[1601.96 --> 1603.60]  to get the spousal approval.
[1605.12 --> 1605.68]  Yeah, we've been there.
[1605.92 --> 1610.12]  You know, my biggest fear in life is that my wife sells my service for what I told her they cost.
[1610.12 --> 1614.04]  Yes, and I know she's listening to this.
[1614.12 --> 1614.86]  So hello, wife.
[1614.86 --> 1618.18]  I run in a mirror VDEV.
[1618.50 --> 1619.30]  Very, very simple.
[1619.52 --> 1626.34]  I just mirror two drives and that gives me 50%, you know, space efficiency and stuff like that.
[1626.34 --> 1632.38]  So I can sustain one drive failing locally before I need to start resorting to backups.
[1633.12 --> 1638.12]  Standard moment where I say RAID is not a backup and you should never rely on it as such.
[1638.12 --> 1643.74]  I very much look at it as that's my primary source of truth.
[1644.16 --> 1647.88]  But if anything was to go wrong with that server or both of those drives were to fail at once,
[1648.42 --> 1653.04]  I actually have just, you know, I've been using the Helios 64 since the review for this,
[1653.10 --> 1662.72]  but I'm just putting together a new system to act as a local ZFS mirror of the mirror VDEV in my house.
[1662.72 --> 1667.58]  So that will live at the other end of the building in case one end, I don't know, catches fire or something, God forbid.
[1668.22 --> 1670.44]  So the short answer is mirrored VDEV.
[1670.74 --> 1677.32]  And if you can swing it as well, a second copy of the data somewhere else and preferably another copy offsite.
[1677.56 --> 1679.92]  Well, this is right on topic because listener Phil wrote in.
[1679.98 --> 1684.82]  He said, you guys often talk about syncing files offsite for a backup, but I'd like to hear a little bit more detail.
[1685.20 --> 1689.60]  How are you guys protecting your backups from things like ransomware or accidental mass deletion?
[1689.60 --> 1693.22]  In those cases, maybe you're not even aware that something is wrong for months.
[1693.78 --> 1698.64]  I know we do it in the enterprise level, but I'd love your thoughts on using tools for yourself for folks at home.
[1698.82 --> 1700.12]  Thanks and keep up the good work, Phil.
[1700.74 --> 1701.82]  How do you protect your backups?
[1701.90 --> 1706.36]  And I think you might mean encryption and other things like, you know, the whole gamut.
[1706.98 --> 1709.32]  Well, ZFS recently added data set encryption.
[1709.90 --> 1713.92]  So the remote system in my setup isn't encrypted.
[1714.28 --> 1715.14]  It's at my dad's house.
[1715.20 --> 1716.86]  So I do trust that as an endpoint.
[1716.86 --> 1721.60]  But I think that is a valid thing that I want to try and implement moving forward.
[1721.78 --> 1727.50]  But this is one of the primary reasons I run ZFS is snapshot support.
[1727.50 --> 1738.16]  So I can roll back to a specific snapshot, you know, much like the Home Assistant Google Drive plugin that lets me do hourly, daily, weekly, monthly backups.
[1738.16 --> 1740.64]  ZFS lets me do that as well.
[1740.72 --> 1743.96]  And I use Jim Salter's Sanoid tool to configure.
[1744.78 --> 1747.92]  I think I've got like 24 hours worth of hourly backups.
[1748.12 --> 1750.16]  And then I've got a week's worth of daily backups.
[1750.68 --> 1754.74]  And then I've got four weeks worth of backups going back a month.
[1754.78 --> 1758.76]  And then I've got one month backup going back six months, I think.
[1758.80 --> 1760.52]  And then I've got an annual thing as well.
[1760.52 --> 1762.90]  So pretty well covered, I think.
[1763.38 --> 1770.14]  But I don't know how I would spot ransomware other than just going to access a file and be like, oh, crap.
[1770.58 --> 1773.98]  Ransomware I'm not particularly concerned about because it would have to get executed.
[1774.38 --> 1776.44]  And, you know, the server environment's my data setting on.
[1776.54 --> 1778.08]  That's not particularly likely.
[1778.66 --> 1784.72]  Kind of like yourself, I have the NAS here at the studio is kind of like a central repository of truth.
[1784.72 --> 1789.58]  And then JB as a business has several cloud instances of different data sets.
[1790.08 --> 1792.28]  I have my data set personally in Lady Joops.
[1792.46 --> 1797.02]  I sync all of that back to the NAS here at the studio.
[1797.56 --> 1801.28]  I don't have a great backup solution for that NAS.
[1801.42 --> 1807.60]  Now, most of the data on it is actually reproducible by all the other locations if I just brought them all back again.
[1807.84 --> 1812.84]  But now I have a little bit more historical information on there that isn't necessarily duplicated anywhere else.
[1812.84 --> 1819.06]  And I'm starting to change my opinion on backing up my media stuff.
[1819.06 --> 1822.28]  In the past, I always thought, well, I have the source material.
[1822.74 --> 1826.16]  And what I can't find on disk, I could probably find on the Internet.
[1826.70 --> 1830.20]  And I'm OK with that because I've likely paid for it at some point.
[1830.44 --> 1832.22]  So I think I'm OK.
[1832.34 --> 1835.58]  But now I actually have found that that's not necessarily the case.
[1835.66 --> 1837.70]  I've had trouble getting DVDs and Blu-rays.
[1837.84 --> 1840.96]  And I've had trouble finding things online of some series.
[1840.96 --> 1844.80]  So now I'm actually thinking maybe I need to back up absolutely everything.
[1845.04 --> 1851.16]  But that becomes like, you know, a 15 terabyte problem I have to solve.
[1851.34 --> 1852.32]  It becomes a race to the bottom.
[1852.52 --> 1853.34]  Yeah, very quickly.
[1854.16 --> 1854.34]  Yeah.
[1854.42 --> 1861.24]  And there's just I mean, I think the only way would be I need to create like a box that maybe I mean,
[1861.24 --> 1872.24]  maybe it's possible with USB storage if I had the money, if I wanted to invest that kind of money into it and sync it here locally and then take it off site via myself, set it up somewhere off site and sync it up.
[1872.44 --> 1879.80]  That is the solution, you know, is to build a server and stick 100 terabytes in it and just forget about it.
[1879.80 --> 1880.16]  Yeah.
[1880.88 --> 1882.42]  Well, in my case, my parents house.
[1882.88 --> 1883.80]  I could do my dad's.
[1883.86 --> 1885.40]  I could probably even do it at Angela's house.
[1885.62 --> 1887.48]  You know, she has fiber at her at her place.
[1887.58 --> 1888.50]  She's a pretty good connection.
[1889.00 --> 1889.32]  I know.
[1889.82 --> 1890.24]  I know.
[1890.54 --> 1891.26]  I would love that.
[1891.72 --> 1901.44]  As far as protecting my backups that I send to Google Drive, which are things like my Docker config directories, my Docker compose files, that kind of stuff.
[1901.44 --> 1909.30]  I still am very happily using duplicati, which I think I've been using for the entire run of the show, and that will do encryption for me.
[1909.60 --> 1913.68]  And it handles the both sides, encrypting and decrypting side of it.
[1914.04 --> 1915.40]  And I just love it.
[1915.48 --> 1924.80]  And I've experimented with using duplicati to save to multiple different cloud providers, which is kind of what I would do in the case of, say, mass deletion on Google Drive or some sort of issue.
[1925.24 --> 1929.60]  But I haven't pulled the trigger yet just because of the bandwidth requirements every single night to do that.
[1929.60 --> 1932.30]  It's not like Google ever killed a product either, is it?
[1932.68 --> 1935.90]  It seems like Drive's pretty core, but you never know, right?
[1935.96 --> 1942.38]  They could also start doing stupid things like revoking API access for third-party applications.
[1942.78 --> 1945.96]  Google Drive itself as a core product is probably safe.
[1946.06 --> 1946.28]  Yeah.
[1946.56 --> 1948.22]  Although nothing truly is with Google.
[1948.22 --> 1961.30]  But the workarounds that I've been using for the last several years of buying one seat of G Suite or whatever it's called this week, and then just uploading three or four terabytes, I think those days are numbered.
[1961.70 --> 1962.28]  So, yeah.
[1962.38 --> 1968.32]  I don't know if you saw, but they're also revoking sync access to the Chromium upstream, you know, open source browser.
[1968.50 --> 1971.50]  They change the terms all the time, and I could see them revoking.
[1971.68 --> 1977.14]  They've also revoked, like, the sign-on for Geary, the email client on Linux.
[1977.14 --> 1977.22]  Nice.
[1977.66 --> 1979.12]  That's just hostile, isn't it?
[1979.18 --> 1980.74]  I thought their slogan was, don't be evil.
[1981.02 --> 1984.56]  Well, I think their slogan now is, become ginormous?
[1984.96 --> 1985.42]  I'm not sure.
[1985.76 --> 1990.44]  They've done a lot of stuff with turning the screws on storage, particularly in the last six months.
[1990.66 --> 1990.88]  Yeah.
[1990.96 --> 2000.52]  So I really don't think that relying on Google anymore as your off-site backup is going to be a viable strategy beyond, I think it's June this year.
[2000.52 --> 2007.08]  The Google Photos Unlimited Storage for Pixel Owners deal that ended is now officially done, too, as this episode is out.
[2007.20 --> 2007.80]  So that's all over.
[2008.26 --> 2008.62]  Yeah, you're right.
[2008.66 --> 2009.80]  There has been a lot of changes there.
[2010.22 --> 2011.98]  That's why you mentioned it earlier.
[2011.98 --> 2021.50]  I think things like cloudfree.shop are the way to go because they're devices that have just been, they're pre-divorced from the cloud when you get them.
[2021.98 --> 2029.66]  They've been pre-flashed with OSs that are open source, that just use your local network, that don't need any cloud connection.
[2030.12 --> 2034.10]  And like Alex said, it's somebody in the community that built this, and I just think it's so cool.
[2034.76 --> 2036.84]  They're like our official, unofficial sponsor.
[2037.06 --> 2038.28]  We do have a promo, right?
[2038.38 --> 2039.10]  Do we have a promo code?
[2039.10 --> 2039.88]  We do, yeah.
[2040.02 --> 2041.64]  Self-hosted is the coupon code.
[2042.20 --> 2046.18]  I think you get 10% off a light bulb, and we get a little kickback from anything else that you buy.
[2046.70 --> 2048.10]  Oh, you know what?
[2048.14 --> 2049.56]  I need light bulbs at the studio.
[2049.88 --> 2056.44]  I was going to mention they have that outdoor smart plug, too, which is slick, but I actually am in the market for light bulbs.
[2056.96 --> 2059.32]  Correction, I think it's smart plugs, not smart bulbs.
[2059.60 --> 2060.18]  My bad.
[2060.46 --> 2060.72]  Sorry.
[2061.40 --> 2062.34]  You know what, man?
[2062.38 --> 2063.40]  You got me so excited.
[2063.50 --> 2065.56]  I thought he's got like some sort of light bulb.
[2065.66 --> 2066.64]  It's all built in over there.
[2066.70 --> 2067.20]  No, that's cool.
[2067.58 --> 2067.98]  That's cool.
[2067.98 --> 2070.14]  The smart plugs, smart plugs will do.
[2070.54 --> 2071.92]  I thought of a slogan for them, though.
[2072.04 --> 2074.66]  Cloudfree.shop, your cloud prenup.
[2075.82 --> 2076.78]  That's pretty good.
[2077.26 --> 2078.12]  I like that.
[2078.22 --> 2078.82]  I like that.
[2079.02 --> 2079.42]  Yeah, you're welcome.
[2079.56 --> 2080.08]  That's free.
[2080.44 --> 2084.52]  What do you say we do a couple of NFC automation tricks that the audience wrote in about?
[2084.64 --> 2086.96]  Because, you know, we've talked about these NFC tags a couple of times.
[2087.02 --> 2091.88]  I have one right here on the mixer that I've set up to do like D&D and stuff like that and turn on lights.
[2091.88 --> 2095.66]  This is particularly relevant for me right now because I've just switched to iOS.
[2096.10 --> 2098.94]  I wanted to take my camera game to the next level.
[2099.18 --> 2101.62]  And boy, is the camera on this thing good.
[2101.84 --> 2110.32]  But moving some of the NFC stuff across and just some of the, you know, more esoteric Android stuff that I like has been tricky.
[2110.32 --> 2120.18]  So with iOS, what happens is when I tap my NFC tag, I then have to tap on a notification that comes in on the phone, which is just, it's just one extra step, right?
[2120.28 --> 2122.14]  But someone wrote in with a workaround?
[2122.60 --> 2122.82]  Oh, yeah.
[2122.90 --> 2124.58]  And this, we got two workarounds.
[2124.78 --> 2126.26]  And I was wondering about these.
[2126.32 --> 2129.94]  So that's why I love these emails because I had seen these as possibilities.
[2130.20 --> 2133.04]  In the back of my mind, I was chewing on it as maybe something to try.
[2133.58 --> 2136.16]  But this confirms my suspicions.
[2136.28 --> 2137.42]  Billy wrote in with the first one.
[2137.42 --> 2140.78]  On episode 35, you guys talked about NFC tags in the car.
[2140.92 --> 2143.92]  I also use an NFC tag to open my garage door just like the Badger.
[2144.24 --> 2150.40]  I switched recently from Android to an iPhone and figured out a way to run the NFC automation without having to click the notification.
[2150.90 --> 2156.66]  It does require that you have your garage door brought into HomeKit, which I am using via Home Assistant.
[2157.42 --> 2160.14]  He says, then you just create an automation in the Home app.
[2160.28 --> 2163.82]  When a specific tag is tapped, like toggle the garage door.
[2163.82 --> 2168.42]  It kind of sucks that you have to do it that way, but it is triggering a Home Assistant action.
[2168.54 --> 2172.26]  If you're already using the app, this is very easy and it's simple to make it work.
[2172.42 --> 2178.28]  You could just create a Boolean that acts as a virtual switch in the Home app and then triggers a Home Assistant automation or action.
[2178.92 --> 2179.60]  That's great.
[2179.84 --> 2180.92]  That is a great idea.
[2181.00 --> 2188.52]  And I actually, I have encouraged you off air, but I am encouraging you on air at some point in the future to play around with the HomeKit integration with Home Assistant.
[2188.52 --> 2199.68]  I don't know if this gets talked about enough because I think maybe we have a lot of Android users out there that are Home Assistant users, but it brings all of the functionality in Home Assistant into HomeKit.
[2200.20 --> 2204.70]  And that makes it work with your watch, with the HomePods, with Siri.
[2204.88 --> 2205.82]  It's pretty great.
[2206.36 --> 2208.12]  I am glad that Billy wrote in with that one.
[2208.24 --> 2210.72]  I'm also even more gladder.
[2211.04 --> 2213.98]  That's not a word, but you know what I mean, that he called me the Badger.
[2214.10 --> 2214.56]  That's fun.
[2214.96 --> 2215.62]  That is fun.
[2215.62 --> 2215.78]  Yeah.
[2216.42 --> 2218.90]  Quinton Ronan with maybe even a better one, though.
[2219.32 --> 2222.00]  He's also, he says he's a site reliability engineer.
[2222.78 --> 2225.20]  I think one of you commented about using NFC tags.
[2225.44 --> 2226.80]  I found a way around this.
[2227.24 --> 2235.66]  You create a web hook in Home Assistant and then use an automation on the phone, which is created with the shortcuts app, to call that web hook.
[2236.06 --> 2240.84]  You're allowed to trigger these from an NFC scan without having to confirm the action manually.
[2240.84 --> 2247.20]  And he has linked us to a post where he explains it more on his blog, so I will include that in the show notes.
[2247.66 --> 2251.68]  But this is, if you look in the Home Assistant app, you'll see this web hooks action.
[2252.02 --> 2255.72]  You combine that with the shortcuts app, and you've essentially solved the problem.
[2255.92 --> 2259.36]  So you've got two options, and one of them doesn't require you mess around with HomeKit at all.
[2259.80 --> 2260.12]  That's neat.
[2260.28 --> 2262.94]  I mean, I've only ever really used web hooks when it comes to Jenkins.
[2262.94 --> 2267.24]  So the fact that we can use them for something actually fun and useful.
[2267.88 --> 2268.24]  Cool.
[2268.96 --> 2270.10]  Hey, just a thank you to our members.
[2270.26 --> 2280.68]  I've noticed some of these emails are from SREs, and we really appreciate everyone who becomes a site reliability engineer, helps the show stay independent, and as a thank you, you get a little extra content.
[2280.84 --> 2283.64]  A limited ad feed with a little extra content at the end.
[2283.80 --> 2287.54]  If you'd like to help the show and become a member, it's selfhosted.show slash SRE.
[2287.82 --> 2289.42]  And so Linus writes in.
[2289.66 --> 2291.56]  I don't know if it's that Linus, although I doubt it.
[2291.78 --> 2292.52]  Let's just pretend.
[2292.52 --> 2295.00]  Okay, Mr. Torvalds.
[2295.50 --> 2297.34]  I'm going to give you advice on something.
[2297.48 --> 2297.74]  Yeah, right.
[2297.86 --> 2298.00]  Okay.
[2298.48 --> 2299.30]  Linus writes in.
[2299.48 --> 2302.32]  Could you give your opinions on how your setup will survive you?
[2302.68 --> 2305.50]  What will happen to your awesome setup if you aren't around anymore?
[2305.68 --> 2307.96]  Will your spouse just pick up everything and it just work?
[2308.50 --> 2311.66]  How can I strive towards such a situation if worse comes to the worst?
[2312.02 --> 2313.72]  Thanks for a great podcast, Linus.
[2314.04 --> 2314.80]  Deep question.
[2315.14 --> 2317.54]  One that's a little uncomfortable to think about sometimes.
[2317.54 --> 2325.52]  I do think this played a little role in my recent renewed push to document as much as my setup as possible in Markdown.
[2325.52 --> 2332.06]  But I know that, no, my family wouldn't really use these systems.
[2332.48 --> 2337.42]  I have documented the passwords in a password vault that they have the password to.
[2337.52 --> 2339.96]  So they, if they needed to, could get access to that.
[2340.06 --> 2346.36]  And then they could share that with somebody like Alex who could help spin stuff up or down for them and, you know, transition them.
[2346.36 --> 2347.64]  I think that's a great point.
[2348.10 --> 2354.20]  Plain text all the things as much as possible and have a Bitwarden or a LastPass or something like that.
[2354.52 --> 2354.66]  Yeah.
[2354.78 --> 2356.18]  So right now it's in LastPass.
[2356.32 --> 2365.68]  However, I have been thinking about transitioning to something else like Bitwarden or something that is, I mean, it's something I want to have a conversation with them because I need to have their buy-off as well.
[2365.68 --> 2370.68]  But I want to share, you know, primarily with my wife, but there's some things that I would leave for Angela too.
[2370.80 --> 2375.26]  And so I kind of wanted something that could accommodate different logins with different credentials.
[2375.42 --> 2377.76]  So if anybody has any suggestions, I'd love to know.
[2377.86 --> 2381.80]  But what do you think about, do you think your wife would keep it going for a bit?
[2381.88 --> 2383.50]  Do you think she'd ask just for somebody to help?
[2383.64 --> 2389.08]  Or do you think she'd just shut it down and get a cable subscription and start reading books?
[2389.18 --> 2390.54]  I mean, what do you think she would do?
[2391.08 --> 2393.90]  Well, at the end of the day, this stuff is my hobby.
[2394.06 --> 2394.32]  Right.
[2394.32 --> 2399.36]  And it just so happens I've been lucky enough to turn it into a podcast and Linux as a job.
[2400.06 --> 2403.06]  But I also enjoy doing this stuff in my spare time as well.
[2403.36 --> 2403.52]  Yeah.
[2403.72 --> 2419.54]  I just don't see how she or anyone else in my family would have that level of interest to keep things on the road beyond, you know, the initial 6, 12 months, you know, that these things would probably continue running for untouched.
[2420.18 --> 2424.20]  There are some things I think that would be missed in terms of quality in life.
[2424.32 --> 2428.06]  Like Plex, like BookSonic, like Home Assistant.
[2428.06 --> 2440.72]  But are they sufficiently useful that it's not worth just buying a Netflix membership or buying some proprietary smart home automation stuff?
[2440.72 --> 2446.78]  Like a lot of what we've done is ultimately boils down to being nice to have versus absolutely critical.
[2446.96 --> 2450.88]  I view it as critical because of my value set and who I am.
[2450.88 --> 2459.92]  But there's a huge swathe of people in my immediate circle in my family that wouldn't care if that stuff went away tomorrow, really.
[2459.92 --> 2463.54]  So I think it would continue to work for some time.
[2463.62 --> 2467.86]  But ultimately, it would sort of decay and die with me, which is a bit sad to think about.
[2468.36 --> 2468.38]  Yeah.
[2468.50 --> 2473.22]  I think the things that they would care more about would be things like documents and photos.
[2473.22 --> 2477.26]  I think that is something that would be a little more significant.
[2477.62 --> 2485.66]  And so that's something I try to give thought to a little bit long term is just in that maybe I haven't done a good enough job with that currently.
[2485.66 --> 2491.56]  But it wouldn't take a lot of work to make that pretty accessible to my wife without my help.
[2492.00 --> 2498.08]  Maybe the way to think about this is try to think of things that they would want access to and then make it as easy as possible for them.
[2498.64 --> 2502.94]  But it's always worth thinking and trying to build your systems that way, if nothing else.
[2503.02 --> 2508.76]  Because even though it's a little bit of a morbid thought, I think it actually leads to building better systems.
[2509.20 --> 2509.56]  Totally does.
[2509.56 --> 2516.94]  I mean, just stop and ask yourself the question now, if something did happen to you tomorrow or, well, even if it doesn't, right?
[2516.96 --> 2531.74]  If you just had to give your partner or your brother or sister or parent or something your laptop and say, go and do something, you know, download a photo or find this tax return or whatever it is.
[2532.50 --> 2537.10]  Do you think they'd be able to do it without you going, oh, you just do this or you just do that?
[2537.10 --> 2552.46]  You know, and if the answer is no, then like Chris says, maybe you need to write some better documentation and print it out or something and put it in a safe or something and say, go to this web URL and you will find the answers to the kingdom, you know.
[2552.92 --> 2560.36]  It kind of goes back to a topic that comes up on our show, well, several times over the, you know, the year plus run now because it's over a year now.
[2561.02 --> 2561.50]  Craftsmanship.
[2561.88 --> 2562.28]  Absolutely.
[2562.86 --> 2565.48]  You know, and that can be another aspect of craftsmanship about your setup.
[2565.48 --> 2566.04]  And why not?
[2566.08 --> 2567.40]  Because nobody else is going to do it.
[2567.50 --> 2568.46]  And it's your setup.
[2568.88 --> 2570.90]  It's your opportunity to show a little craftsmanship.
[2571.00 --> 2574.48]  And also it's another, it's another nice way for people to remember you by.
[2574.54 --> 2577.42]  Look at the time and effort he took to make this accessible for us.
[2577.64 --> 2578.56]  So it's a win-win.
[2578.70 --> 2579.92]  It's just a matter of time.
[2580.28 --> 2583.34]  And I kind of pulled back on it a little bit, but you know what?
[2584.00 --> 2585.24]  Mr. Torvald's writing in here.
[2585.30 --> 2587.40]  It's got me feeling like I'm going to keep up with it again.
[2587.40 --> 2591.86]  It's like inheriting someone else's workshop tools, you know.
[2592.12 --> 2592.42]  Yeah.
[2592.66 --> 2595.70]  When my wife's dad passed away, we inherited a bunch of his workshop stuff.
[2595.96 --> 2601.96]  And it was, I don't know, just odd to be in someone else's cave, you know.
[2602.16 --> 2604.72]  And I guess it's a similar situation with these types of systems.
[2604.92 --> 2609.08]  So I'm all sad now thinking about this.
[2609.54 --> 2612.14]  I feel like if I logged into your box, though, I'd feel pretty comfortable.
[2612.14 --> 2613.18]  I'd have a pretty quick.
[2613.18 --> 2615.56]  Yeah, but you're a massive nerd, mate, you know.
[2616.10 --> 2616.76]  I know, I know.
[2616.84 --> 2620.10]  But that's what's, I mean, there's something about that that's like kind of weird, like
[2620.10 --> 2621.24]  server swapping.
[2621.40 --> 2623.52]  We should try that sometime and then record our reaction.
[2624.40 --> 2626.08]  Yeah, like wife swap, but shitter.
[2627.96 --> 2631.68]  Yeah, just like almost like that, but just a little bit different.
[2633.04 --> 2634.12]  Just see what it's like.
[2634.22 --> 2634.88]  Where would it air?
[2634.94 --> 2635.88]  Would it air on TLC?
[2636.12 --> 2636.88]  Would that be the place?
[2637.38 --> 2639.02]  No, I don't think they'd want it.
[2639.10 --> 2641.60]  But, you know, it's funny is if you look at some of my servers,
[2641.60 --> 2647.16]  you can really see transitions and how I organize stuff or just legacy stuff.
[2647.26 --> 2652.64]  Like the way we have the NAS set up here is really, really far and removed on how I build
[2652.64 --> 2655.56]  a system now and the way I lay out the disks and all of it.
[2655.72 --> 2661.16]  And actually, the ZFS array that we're using was originally set up and partitioned and managed
[2661.16 --> 2661.92]  by Alan Jude.
[2662.12 --> 2664.54]  So it's like extensively complex.
[2665.32 --> 2666.30]  The man, the myth, the legend.
[2666.64 --> 2668.38]  Yeah, he set it up while he was out here.
[2668.38 --> 2669.92]  And it's worked with us.
[2670.02 --> 2673.72]  I mean, it's clearly scaled for years because we've changed out operating systems.
[2673.86 --> 2674.62]  We've moved hardware.
[2674.98 --> 2679.02]  But that ZFS pool just continues to grow and survive.
[2679.70 --> 2684.26]  But if you look at it now, it's a total, total misrepresentation of how I would build
[2684.26 --> 2684.72]  a system.
[2685.70 --> 2687.78]  Not to mention just because it's an Arch server.
[2688.26 --> 2691.60]  Didn't it start life on BSD and now, yeah, like you say, it's running Arch?
[2692.14 --> 2693.52]  Yeah, BSD for a while.
[2693.60 --> 2695.38]  I think it lived on Fedora for a bit.
[2695.62 --> 2696.88]  And now it's on Arch.
[2697.08 --> 2700.54]  And so far, it stayed there because it's a minimum viable Arch.
[2700.68 --> 2703.84]  So it's just the absolute bare minimum of a system we need.
[2704.10 --> 2704.98]  Yeah, I was listening to that.
[2705.02 --> 2707.56]  Was it Coda where you were talking about minimum viable server?
[2708.06 --> 2713.62]  And I was resonating so hard with that because I've just switched over to Proxmox and all
[2713.62 --> 2715.28]  of its weird abstractions and stuff.
[2715.36 --> 2718.16]  And I was thinking, oh, if I was just on Arch, this would have been so easy.
[2718.20 --> 2719.92]  It would have been done 10 minutes ago, you know.
[2719.92 --> 2720.76]  Yep, yep, yep.
[2721.00 --> 2722.28]  Yeah, there is something to that.
[2722.52 --> 2725.78]  I also want to mention our sponsor, Cloud Guru, is on social media.
[2725.88 --> 2728.66]  So if you are learning this stuff right now and you want to engage with them on social
[2728.66 --> 2732.60]  media, they're just slash a Cloud Guru on YouTube, Twitter, and Facebook.
[2733.14 --> 2736.00]  Alex, you're probably on Twitter too, I bet.
[2736.34 --> 2737.32]  I sure am.
[2737.42 --> 2739.20]  I'm there at, let's stop that.
[2739.26 --> 2740.14]  Let's stop that right now.
[2740.60 --> 2742.28]  I am there at Ironic Badger.
[2742.54 --> 2742.74]  Yep.
[2742.80 --> 2745.58]  And you can contact the show, self-hosted.show slash contact.
[2745.90 --> 2748.72]  That's the place to get in touch and get your email on the show.
[2748.72 --> 2753.92]  I'm at ChrisLAS and the show itself is at self-hosted show on the Twitter.
[2754.38 --> 2755.44]  Okay, I almost started doing it again.
[2755.48 --> 2755.78]  I'm sorry.
[2756.08 --> 2757.20]  I don't know what came over me.
[2757.56 --> 2758.46]  It was weird.
[2758.70 --> 2759.40]  It got weird.
[2759.72 --> 2760.86]  Oh, I shouldn't do accents.
[2760.92 --> 2761.62]  That's what we've learned.
[2762.04 --> 2763.98]  You can find the network at Jupiter Signal.
[2764.40 --> 2767.02]  And that was self-hosted.show slash 37.
[2767.02 --> 2770.60]  Neverland Fluge Event
[2772.68 --> 2772.70]  at Jupiter Signal.
[2772.78 --> 2772.88]  To 1st.
[2772.96 --> 2773.32]  To 1st.
[2773.52 --> 2775.58]  To 2nd.
[2775.66 --> 2776.48]  To 2nd.
[2776.56 --> 2777.56]  To 2nd.
[2779.72 --> 2780.48]  To 2nd.
[2784.54 --> 2784.76]  To 2nd.
[2785.78 --> 2786.08]  To 2nd.
[2786.62 --> 2786.92]  To 2nd.
[2787.70 --> 2787.98]  To 2nd.
[2787.98 --> 2788.66]  To 2nd.
[2788.76 --> 2789.14]  To 1st.
[2789.28 --> 2789.80]  To 2nd.
[2789.92 --> 2789.94]  To 4th.
[2789.94 --> 2790.86]  To 5th.
[2790.92 --> 2791.78]  To 2nd.
[2792.00 --> 2792.66]  To 3nd.
[2792.72 --> 2793.08]  To 4th.
[2793.10 --> 2793.90]  To 3rd.
[2794.02 --> 2794.10]  To 4th.
[2794.12 --> 2794.58]  To 530.
