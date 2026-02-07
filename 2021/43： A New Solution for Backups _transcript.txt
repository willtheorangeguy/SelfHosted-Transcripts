[0.00 --> 7.90]  I have an idea for a charging station in the home that I think would be a brilliant way to save battery life.
[8.38 --> 9.74]  I think I'm on to something here.
[10.18 --> 13.30]  So if you need to save battery life, why do you need a charging station?
[13.72 --> 18.20]  Here's the thing. So you got your devices, right? Like your laptops and your iPads.
[18.20 --> 25.50]  And the actual truth is you shouldn't keep these things at 100% charge state all the time, right?
[25.76 --> 27.04]  Wow. No, no, no.
[27.04 --> 34.42]  In fact, somewhere between 40% and 60% is probably ideal for the type of lithium-ion batteries that are in our devices. Do you agree?
[34.76 --> 43.72]  Yeah. When I worked in the Genius Bar, I can't tell you the number of MacBooks I saw with batteries that were exploding through the keyboard or stopping the trackpad from working.
[43.72 --> 53.24]  I wish there was a way to just set in any OS. I want my battery level to be at this unless I press I'm going traveling button.
[53.24 --> 62.84]  Here's what I'm thinking. So there's a couple of ways I think I could solve this, but I've got a really old MacBook from like 2013 and the battery is still kind of working and I want to keep it alive.
[63.04 --> 67.82]  And it dawned on me that they have that Home Assistant app for macOS that tracks your battery life.
[68.00 --> 69.00]  Oh my God, you're a genius.
[69.66 --> 77.16]  Right? So you just put the adapter, you plug that into a smart plug and you have Home Assistant automatically turn off the smart plug when the Mac gets to 60%.
[77.16 --> 84.34]  And I think you could probably do it with Linux. I just, I'm wondering maybe somebody in the audience knows how you could report back a battery status to Home Assistant, but.
[84.64 --> 86.12]  That's a great idea, Brent.
[86.52 --> 91.44]  So I want to expand the idea for other devices as well. So I want input from people on how to do this.
[91.44 --> 99.16]  But essentially my goal would be to use a couple of smart plugs that are managed by Home Assistant to charge things for a while and then turn the charge off.
[99.16 --> 106.48]  And if there was a way to do it intelligently, maybe I don't even need the sensor data. Maybe I could just do it by like some math. I don't know.
[107.16 --> 112.50]  That's my current goal at home right now. So if anybody has some suggestions, I'd like them.
[112.50 --> 122.06]  In the meantime, if you just have a Mac that you want to limit the maximum charging for, you should look into Al Dente. It works with Intel or M1 Macs.
[122.24 --> 128.34]  And it's just letting you set a hard limit on the charge before the system continues to charge, I suppose.
[129.04 --> 130.52]  You can look into that. We'll have a link in the show notes.
[131.00 --> 136.32]  This is fantastic. I gave my wife my old laptop last year sometime.
[136.32 --> 143.20]  And I know for a fact, even though I've told her, you need to unplug it at least once a month and cycle the battery.
[143.76 --> 147.52]  I know it's been sat there since my daughter was born and hasn't moved.
[148.28 --> 154.94]  Right. Well, we have like one Mac here in the studio that's for effects processing and it just sits there always plugged in.
[155.00 --> 158.04]  So I put this Al Dente on there and capped it at 60%.
[158.04 --> 163.18]  And then I started thinking, how can I do this where it's not Mac OS specific or maybe it could be for multiple devices.
[163.18 --> 169.30]  So I'm going to expand the idea. In the meantime, you could expand your mind at a Cloud Guru.
[169.44 --> 172.60]  They are the leading in learning for the Cloud, Linux and other modern tech skills.
[172.92 --> 175.56]  Hundreds of courses, thousands of hands-on labs.
[175.96 --> 179.84]  Get certified, get hired, get learning at a CloudGuru.com.
[180.28 --> 184.16]  I think we've talked about this before. I'm talking, of course, about healthchecks.io.
[184.36 --> 191.60]  But I've had a little epiphany with healthchecks recently and I've started using it quite heavily for my own purposes.
[191.60 --> 193.30]  I wonder if you have used it for anything.
[193.84 --> 199.94]  You have talked about it before and I've considered it, but I haven't been able to grok if it's worth the setup time yet.
[200.02 --> 202.02]  It was actually one of the things I've been meaning to talk to you about.
[202.48 --> 206.74]  I did go last time we talked about it with the hosted service.
[207.10 --> 213.38]  And one of the struggles of being a self-hoster is do I self-host? Do I use the hosted version?
[213.38 --> 216.76]  And with different services, I fall on different sides of that line.
[216.96 --> 222.20]  And, you know, Bitward and I use the hosted service and I pay, I think it's $10 or $12 a year for that.
[223.06 --> 227.38]  And with healthchecks, their hosted version is actually free for up to 10 healthchecks.
[227.48 --> 230.06]  Beyond that, they have a pricing page.
[230.94 --> 236.04]  So the hobbyist is actually free for up to 20 jobs, not 10, my mistake.
[236.04 --> 241.58]  Beyond that, you can pay $5 a month and you'll get some phone support and some email support.
[241.78 --> 247.34]  And then they have business plans at $20 and up for 100 jobs and stuff like that.
[247.94 --> 252.04]  And I was doing a bunch of different ZFS replication tasks.
[253.12 --> 258.46]  And what I wanted to happen was I've just done a whole bunch of hardware shuffles in my house.
[258.84 --> 259.44]  You? Never.
[259.44 --> 267.80]  Well, this all stems from January when I was basing everything around GVTG and wanting to do everything with that single Intel box.
[268.04 --> 269.70]  And it didn't work out.
[269.76 --> 273.86]  So I've had to kind of, you know, rewind and kind of reconfigure a few things.
[273.98 --> 277.48]  So my old Dual Xeon box is now purely HomeLab.
[277.62 --> 283.46]  That is running ESXi and it's just going to sit in a corner turned off for 95% of its life now.
[284.74 --> 288.78]  Just such an overkill for that box because it's so powerful.
[288.78 --> 291.86]  But it consumes a lot of power in the process.
[292.50 --> 296.28]  And the Intel i5 system in the basement is the full-time one.
[296.78 --> 304.34]  But what I figured I could do was take a couple of these slightly older 10 terabyte hard drives I have that are two or three years old at this point.
[304.82 --> 311.50]  Put those into the HomeLab box and then schedule that to turn on at least once a week.
[311.58 --> 315.24]  I'll probably turn it on more whilst I'm working during the week and doing OpenShift stuff.
[315.24 --> 319.56]  But what I wanted to happen was to have a local backup.
[320.08 --> 326.50]  So I wanted my ZFS in the basement to replicate to the ZFS in my HomeLab box upstairs.
[326.50 --> 333.12]  And to keep track of when the last backup was, I needed some kind of a tool to do that.
[333.18 --> 337.82]  Because I've got a lot going on, as we all do, and I'm going to forget stuff.
[338.04 --> 342.74]  And the last thing I want is to come, you know, to need that backup and go,
[343.66 --> 346.42]  oh, yes, the last time it ran was 2019.
[346.84 --> 347.20]  Oh, dear.
[347.66 --> 347.78]  Right.
[348.06 --> 351.28]  Well, and you recall that did happen to me where I had a Google account outage.
[351.28 --> 354.68]  And so the backup hadn't run for a little bit and I didn't realize it.
[355.04 --> 355.16]  Absolutely.
[355.84 --> 361.18]  And so I finally got round to setting up the self-hosted version of the health checks.
[361.38 --> 371.08]  Now, I'm running this on Linode because I actually foresaw a situation where all the servers in my house are off for, you know, a couple of weeks.
[371.16 --> 376.42]  Let's say I'm taking a vacation or something or traveling to England to see grandparents or whatever.
[376.92 --> 379.46]  Or maybe your power is turned off because you're getting solar installed.
[379.46 --> 381.60]  Yes, that is happening soon, actually.
[382.38 --> 387.36]  And so I thought, right, where can I run this that is reliable and is going to be more reliable than my house?
[387.40 --> 389.36]  And I thought Linode was a perfect fit for that.
[389.56 --> 393.66]  So this is running on one of their $5 a month Linodes.
[394.00 --> 399.68]  It's the same one that's doing perfectmediaserver.com and my personal blog and all the rest of it.
[399.72 --> 403.96]  So this box is serving like quintuple duty at this point.
[404.08 --> 405.46]  It's doing a lot of stuff for me.
[405.52 --> 406.26]  And it's only a five.
[406.26 --> 407.50]  It's only a five or a month.
[407.82 --> 409.16]  I love it.
[409.16 --> 416.22]  The self-hosted version of HealthChecks, I'm running the Linux server docker, which was written by one of my friends, also called Alex.
[417.28 --> 423.26]  He has done a bunch of work with making sure that it pulls in the latest code from the HealthChecks repo.
[423.26 --> 430.46]  So there is, as always with containers, it seems, a choice to be made about which container do I run.
[430.54 --> 435.32]  Do I run the official one or do I run the Linux server one or some other random one?
[436.00 --> 440.32]  I try and run the Linux server ones for obvious reasons whenever I can.
[440.68 --> 445.28]  If for no other reason, then they auto-update, which is kind of nice when you restart the app.
[445.28 --> 451.70]  So you get all the features with this self-hosted version that you don't get on the hosted version.
[451.84 --> 459.38]  So actually, in this case, self-hosting gives you more functionality than the hosted version, which is always nice.
[459.74 --> 461.26]  And there are a bunch of integrations.
[461.26 --> 468.82]  I'm just using one with Pushover, which is a push notification service, which you configure through environment variables for the container.
[469.00 --> 476.90]  You generate a token with Pushover and pass that through an environment variable in your Docker Compose file or however you like to do that.
[476.90 --> 482.74]  It also supports a bunch of other interesting stuff like Prometheus, Ops Genie.
[482.90 --> 485.24]  If you're doing something for work, this can be useful.
[485.82 --> 489.86]  You can have it ping Slack, Discord, Microsoft Teams, Mattermost.
[489.98 --> 491.06]  It does webhooks.
[491.56 --> 494.24]  There really are a lot of integrations for alerting.
[494.50 --> 495.96]  I'm just using Pushover, as I said.
[496.36 --> 500.72]  It's really nice because I don't really see it if it's in the log file.
[500.72 --> 509.44]  But if I got a message in the same communications tool I'm using to chat with you and Wes or something like that, then I'm definitely going to see it.
[509.50 --> 510.94]  And then I'm going to be able to take action on it.
[511.24 --> 516.56]  And so just those small things like being able to send a message to Slack, it makes a huge difference for me, Alex.
[516.80 --> 517.94]  It supports Telegram as well.
[518.04 --> 519.62]  So if you have a group of people.
[519.74 --> 520.76]  Yeah, there you go.
[520.90 --> 525.52]  You can actually have it interact with bots as well, I think, and do a bunch of stuff with that.
[525.52 --> 533.88]  So you could make this really quite deeply integrated into some kind of an incident response solution type thing.
[534.36 --> 535.54]  I don't really need that.
[535.62 --> 538.96]  I just need to be reminded that, hey, dummy, you haven't run your backups for two weeks.
[540.40 --> 545.86]  Did I track that in that description of yours, you transitioned from the hosted solution to the self-hosted version?
[546.28 --> 546.46]  Yeah.
[546.76 --> 547.50]  And why was that?
[547.62 --> 551.26]  Well, number one, I was running up against the 20 job limit, which I thought was 10.
[551.26 --> 555.42]  So maybe I wasn't running up against it, but I knew I was going to be running into that limit soon anyway.
[555.84 --> 555.90]  Okay.
[556.20 --> 563.50]  And I also, you know, as part of being the host of this show, feel a responsibility to try these things out on occasion.
[564.12 --> 565.04]  That's how I felt.
[565.18 --> 573.98]  Not just because of that, but I thought because I could host it, say, on a VPS, and then I could check even the systems here on the LAN at the studio, it might be worth doing.
[574.66 --> 576.30]  What kind of setup am I looking at, though?
[576.48 --> 579.80]  Because things I'd like to monitor is like, is NextCloud running?
[579.80 --> 580.80]  So what does that mean?
[580.82 --> 582.78]  It means, is the web port available?
[583.06 --> 584.64]  Is the database server online?
[584.64 --> 586.56]  I guess is the web page loading?
[587.00 --> 588.54]  I'd like to know that kind of stuff.
[589.02 --> 590.34]  But there's all kinds of other things.
[590.40 --> 592.94]  Like, I'd like to know, we have our Matrix server that we run.
[593.46 --> 596.40]  That isn't on the LAN, but it's a server we manage.
[596.40 --> 600.36]  And Matrix eats a crap ton of RAM right now.
[600.36 --> 603.50]  The Synapse server is definitely a work in progress.
[604.10 --> 609.88]  And it's something that we have to log in and manage from time to time and even restart sometimes or go through some sort of cleanup.
[609.88 --> 615.92]  And I'm wondering, like, what about those kind of scenarios where the system's running out of memory?
[615.92 --> 619.50]  Does it do that kind of monitoring, that kind of reporting?
[619.62 --> 623.22]  Or is it more failed, yes, or working, that kind of stuff?
[623.22 --> 629.42]  It's a great question because it's a bit of a confusing area, all this monitoring and alerting type stuff.
[629.92 --> 636.60]  So HealthChecks is primarily designed to be run as part of a script or a cron job or something like that.
[636.60 --> 641.08]  And the way it works is you curl a URL, you hit a URL.
[641.80 --> 646.44]  The HealthChecks API on the other end receives that request and goes,
[646.60 --> 651.30]  hey, I've just been pinged on this random string of URL, UUID type stuff.
[651.60 --> 653.26]  That's a phoning home.
[653.46 --> 654.86]  That is that job completing.
[655.08 --> 665.10]  So if you put it at the end of a backup script, say, the very last line is curl HTTPSHealthChecks.com slash your UID,
[665.10 --> 672.32]  then the software knows that you've successfully got to the end of that script and it assumes everything's gone well.
[672.64 --> 676.12]  What you're looking for, I suspect, is something more along the lines of Prometheus,
[676.24 --> 683.38]  which is designed to monitor disk space and memory usage and CPU temperatures and percentage and all that kind of crap.
[684.12 --> 688.12]  And Prometheus will then output to something called Alert Manager.
[688.76 --> 692.48]  And you can write what's called PromQL, Prometheus Query Language.
[692.48 --> 695.04]  Queries sounds complicated.
[695.18 --> 697.26]  It's much easier than SQL to get started with.
[697.36 --> 702.24]  So if you've ever had to write an SQL query, you can probably write a PromQL one.
[703.06 --> 706.36]  And that's probably more what you're after in terms of monitoring.
[706.56 --> 710.04]  You know, is Matrix, is the API still available, for example?
[710.32 --> 713.00]  Can I still hit a certain URL?
[713.20 --> 714.50]  Is that website still available?
[714.50 --> 718.26]  In the meantime, I've been keeping an eye on it with net data, which feels like a cheat.
[718.50 --> 721.38]  I feel like I almost am ashamed to admit it, but it's been handy.
[721.62 --> 724.16]  And I've used that to kind of keep an eye on the system.
[724.22 --> 725.78]  But I know I need to take it to the next step.
[725.84 --> 727.86]  Maybe a topic for a future episode.
[728.28 --> 729.64]  Who doesn't love a pretty graph, eh?
[729.64 --> 734.84]  Speaking of which, did you know about this command I found out quite recently about this one?
[735.50 --> 736.38]  Docker stats.
[736.62 --> 739.56]  Just go to a box where you've got a few containers running and take a look at this.
[739.88 --> 740.54]  This is pretty great.
[740.62 --> 746.36]  In fact, this is one of the ways I realized how much memory and CPU Matrix actually takes.
[746.92 --> 748.24]  The snaps, or at least.
[748.60 --> 751.38]  This is kind of like top for your Docker containers.
[751.52 --> 756.12]  It gives you CPU usage, memory, IO, and all that kind of stuff.
[756.12 --> 763.00]  And you can also just get a list for a single container if you specify that container, if that's what your permissions only allow for.
[763.30 --> 769.74]  But if you can see all of the containers, then you can just run Docker stats on its own and get a list of everything on the box.
[770.04 --> 773.84]  And I was surprised because I run ping stat here at the studio.
[773.94 --> 775.64]  So I just thought, well, I'll check it right before the show.
[776.00 --> 777.40]  And I ran that.
[777.52 --> 778.62]  And it comes up.
[779.00 --> 781.84]  And ping stat, which is just pinging stuff and graphing it, right?
[781.84 --> 786.70]  I ran this command.
[786.96 --> 788.28]  And I'm like, what is it doing?
[788.60 --> 791.04]  But then I sat there and watched it for probably five minutes.
[791.16 --> 793.14]  And it never once again really did anything.
[793.32 --> 799.96]  But that brief moment when I brought it up, Alex, is 300% of my CPU on my server for ping stat.
[800.66 --> 802.10]  Yeah, it's pretty interesting, isn't it?
[802.10 --> 811.60]  If I go into my CloudVPS where the Unify controller is running, that damn thing has 117 processes under one container.
[812.02 --> 812.24]  Yeah.
[812.54 --> 813.42]  Yeah, that's...
[813.42 --> 814.90]  I don't know how that makes me feel.
[815.20 --> 817.18]  It doesn't make me feel good, I'll be honest.
[817.18 --> 821.18]  Linode.com slash SSH.
[821.92 --> 826.30]  Go there to get a $100 credit on a new account for 60 days.
[826.44 --> 828.34]  And, of course, you support the show.
[828.80 --> 832.28]  Linode is the largest independent cloud computing provider out there.
[832.48 --> 837.06]  No matter what technology stack you're familiar with, you're going to find Linode easy to use.
[837.22 --> 840.88]  And if you're an expert, under the hood, there's a little thing here or there,
[840.88 --> 846.58]  little hints that you'll see for us long-time Linux users that will make things even quicker and more efficient.
[846.58 --> 848.04]  And things you'll really appreciate.
[848.80 --> 858.26]  And if you ever run into any trouble, Linode has fantastic, amazing, great customer service 24-7 by phone or by ticket, whatever you prefer.
[858.56 --> 861.36]  And they have hundreds of guides and tutorials to help you get started.
[861.94 --> 863.80]  And we often will link to some in the notes.
[864.36 --> 868.94]  There's one that I recommend anybody that wants to run PHP My Admin, give that one a read.
[869.36 --> 872.64]  That's just a few steps you can go through to make that a much more secure installation.
[873.44 --> 876.14]  Linode is easy to use and they have a powerful cloud dashboard.
[876.14 --> 879.48]  And they also have S3-compatible object storage.
[879.90 --> 882.66]  This could be something that works great for your backup strategy.
[882.86 --> 887.38]  A lot of applications and tools can integrate and backup to S3-compatible storage.
[887.90 --> 889.72]  And Linode has fantastic pricing.
[890.12 --> 892.80]  And you could build that right into your backup or recovery strategy.
[893.18 --> 895.66]  But additionally, you could also just use it for a static website,
[895.80 --> 900.18]  for hosting any kind of files you need out in the cloud where you don't want to have to run a server in front of it.
[900.18 --> 903.64]  And they have simple one-click application deployments, if that's more of your drive,
[903.94 --> 907.64]  which I totally respect because Linode is a fantastic learning platform as well.
[908.00 --> 910.42]  Deploy an application, learn how it works.
[910.80 --> 911.80]  Linode's great for that.
[911.86 --> 914.98]  With our $100 credit, there's all kinds of things you can try.
[915.36 --> 919.34]  And learning something, trying it out, is a great use of that too.
[919.34 --> 921.30]  I mean, absolutely, you can put it in production.
[922.08 --> 924.68]  But why not use that credit to learn something new as well?
[924.98 --> 926.86]  So go to linode.com slash SSH.
[926.94 --> 930.48]  Get that $100 60-day credit and support the show.
[930.64 --> 933.16]  That's linode.com slash SSH.
[934.92 --> 937.62]  Now, you know how I love me some Blue Iris stuff.
[937.74 --> 943.06]  Some pretty exciting news in the last couple of weeks about deep stack integration with Blue Iris.
[943.06 --> 952.68]  Traditionally, what you had to do to get object detection, you know, bird, car, plane, bear, I think was one of the options.
[953.14 --> 954.44]  You want bear detection for sure.
[954.78 --> 955.62]  Yeah, probably.
[956.16 --> 960.58]  Yeah, if a bear is in the woods, does it, how does the saying go?
[961.12 --> 962.54]  Actually, I don't care where you are.
[962.62 --> 967.30]  If there's a bear in your backyard, even where you live, Alex, I think you'd want to know about it.
[967.30 --> 974.78]  But what's particularly exciting about this latest Blue Iris update is that built right in now to the Blue Iris software,
[975.10 --> 981.06]  you can launch deep stack natively on the Windows system that it's running on.
[981.20 --> 989.56]  So you don't need a helper program or any kind of JPEG kind of detection intermediary software anymore.
[989.56 --> 991.44]  It's just all done within Blue Iris.
[991.44 --> 996.46]  So I've put a link to a YouTube video in the description, which talks you through how to set that up.
[996.46 --> 1002.00]  Deep stack gets even better, tempting me to come over to the Windows side, but it's not going to happen just yet.
[1002.54 --> 1007.26]  You know, I actually find a lot of utility in just bringing the video feeds into Home Assistant
[1007.26 --> 1011.38]  and having a dashboard and Home Assistant I can go to and just get live camera feeds.
[1011.82 --> 1017.26]  So that, you know, that would just be a great integration one day is something that manages all of that.
[1017.44 --> 1017.76]  Absolutely.
[1018.32 --> 1019.88]  Alex, I know you're a big ZFS guy.
[1019.98 --> 1022.16]  So have you seen ZFS.rent?
[1022.48 --> 1023.04]  I have.
[1023.14 --> 1023.32]  Yes.
[1023.42 --> 1023.92]  Oh, my goodness.
[1023.92 --> 1026.00]  This thing looks really, really cool.
[1026.00 --> 1027.64]  I can't remember where I discovered it.
[1027.98 --> 1029.78]  I think it was on the self-hosted Discord.
[1030.00 --> 1033.50]  Somebody just said to me, have you, why don't you use ZFS.rent?
[1033.60 --> 1035.36]  And I'm like, because I didn't know about it.
[1036.82 --> 1043.14]  The whole premise behind ZFS.rent is that it's a simple cloud service to store ZFS snapshots.
[1043.90 --> 1048.54]  Effectively, it's like having a ZFS send, but in a co-located data center.
[1048.54 --> 1051.80]  But their business model is really pretty interesting.
[1051.80 --> 1058.70]  So these guys rent out KVM virtual machines and they have dedicated hard drives to each VM.
[1058.84 --> 1060.32]  So I guess they're using pass-through or something.
[1060.80 --> 1064.12]  There is no sharing and no overcommitting on these VMs.
[1064.62 --> 1070.98]  And when you sign up to their service, you receive a root password, a dedicated IBV4 address.
[1071.24 --> 1075.30]  So you could, you know, alias that to a subdomain of your choosing.
[1075.30 --> 1078.98]  And then you get a pre-formatted and mounted ZFS pool.
[1079.74 --> 1081.52]  Here's where it gets really, really interesting.
[1082.10 --> 1088.34]  You can send them hard drives with data already on them to their data center.
[1089.00 --> 1089.68]  I love that.
[1090.30 --> 1090.80]  That's great.
[1090.92 --> 1095.46]  You know, you were just talking about how you had those 10 terabyte drives that you were kind of using as just scratch drives for backup.
[1095.66 --> 1096.66]  That's a great example.
[1096.74 --> 1098.54]  You could load those suckers up and send them off.
[1098.72 --> 1099.06]  Absolutely.
[1099.22 --> 1099.38]  Yeah.
[1099.72 --> 1101.42]  Now, pricing is pretty straightforward.
[1101.54 --> 1103.04]  It's 10 bucks a month per drive.
[1103.04 --> 1112.42]  So if you can go on Best Buy and find one of their easy stores on a cheap deal, you could have, you know, a 14 terabyte drive for $200.
[1113.34 --> 1117.02]  Load that sucker up with all of your data, send it off to this data center.
[1117.42 --> 1120.48]  And for 10 bucks a month, you've got 14 terabytes of cloud storage.
[1120.94 --> 1122.80]  You know, that is doable for what I do here.
[1122.94 --> 1123.24]  Right?
[1123.52 --> 1124.24]  It's one of those things.
[1124.32 --> 1126.44]  You sort of read the website and you're like, where's the catch?
[1126.48 --> 1127.28]  There's got to be a catch.
[1127.82 --> 1130.88]  I was actually speaking with Ryan, who's the guy behind ZFS.rent.
[1130.88 --> 1133.70]  And I'm hoping to get him on the show to do an interview shortly.
[1133.90 --> 1135.42]  But he seems like a really great guy.
[1135.66 --> 1143.80]  And honestly, I have no qualms about recommending this service, even just as a, hey, guys, you know, audience, did you know this is a cool thing existed?
[1144.36 --> 1144.38]  Yeah.
[1144.50 --> 1144.68]  Nope.
[1144.72 --> 1146.98]  No sponsor, no relationship of any kind.
[1147.00 --> 1148.28]  It's just something we came across.
[1148.76 --> 1153.46]  Each plan includes one terabyte of base bandwidth data movement per month.
[1153.46 --> 1156.74]  They don't distinguish between upload or download.
[1156.84 --> 1158.06]  A terabyte is a terabyte.
[1158.52 --> 1163.58]  They have a rate of an additional $5 per terabyte after that, which is actually pretty reasonable.
[1164.54 --> 1170.02]  If I'm uploading more than a terabyte in a month, my ISP is probably knocking on my door.
[1170.52 --> 1175.84]  I would imagine the time where you would actually need to exceed a terabyte is the initial seeding.
[1176.10 --> 1182.02]  Well, we can get around that by sending them the drive preceded or in a disaster recovery scenario.
[1182.02 --> 1191.20]  And if I'm at the point where I need to download 14 terabytes of data from my backup, I think I can probably swing, you know, the hundred bucks or whatever it is to get that.
[1191.52 --> 1196.08]  That's just what I was thinking is that's really the only time it would be costly is when you're actually pulling it all back down.
[1196.22 --> 1201.84]  I wonder if they would do that, although you wouldn't really want to wait, but I guess they could maybe reload a disk.
[1201.92 --> 1203.88]  You could send them the disk and they could reload it up.
[1205.10 --> 1206.88]  Now, did you see this on their homepage?
[1207.72 --> 1207.84]  What?
[1207.84 --> 1210.88]  Users have a choice of from OSes.
[1211.22 --> 1216.54]  CentOS, with maintenance support until 2029, crossed out to 2021.
[1217.62 --> 1218.82]  Oh, too soon.
[1218.98 --> 1221.16]  Also, Ubuntu and Debian.
[1221.98 --> 1228.30]  But here's where I thought it got super interesting is, as an Arch guy, no pre-installed OS.
[1228.30 --> 1238.24]  You can attach your own Linux ISO to the KVM virtual machine and install via a tunneled VNC client any OS that you want.
[1239.08 --> 1240.20]  That's adorable.
[1240.96 --> 1243.28]  That's a really great setup.
[1243.28 --> 1252.18]  They also do support Debian 10.7 out of the box and Ubuntu 20.04 until 2025, which is honestly what I would just do.
[1253.14 --> 1254.42]  I think it's too.
[1254.72 --> 1258.80]  It's so great that they left the 2029 on there and crossed it out.
[1258.90 --> 1260.10]  Like, that's such a statement.
[1260.86 --> 1261.16]  Yeah.
[1261.16 --> 1266.36]  I've actually just deployed my first CentOS 8 stream box in production.
[1266.66 --> 1272.68]  We're doing a small, limited Jupyter Colony mail server for like a handful of people right now.
[1273.08 --> 1275.62]  And it's all running on CentOS 8 stream.
[1275.98 --> 1277.16]  Look at you, you hipster.
[1277.44 --> 1277.70]  Yeah.
[1277.88 --> 1281.22]  So I'm going to give it a go and see how it is to run a mail server.
[1281.66 --> 1282.76]  I'll report back.
[1282.76 --> 1285.46]  I suspect there's going to be crappy aspects to it.
[1287.96 --> 1294.70]  This episode is brought to you by Synology, makers of network attached storage devices, networking and surveillance equipment.
[1295.18 --> 1303.20]  In late 2020, they released the DS1621 Plus, a six bay NAS unit with a four core, eight thread Ryzen CPU.
[1303.92 --> 1308.42]  As a result, this system runs cool and quiet whilst being a powerhouse under the hood.
[1308.42 --> 1314.16]  And if you need it, there's a PCIe slot for add in cards such as 10 gigabit networking as well.
[1314.86 --> 1319.62]  What really sets Synology units apart from their competition for me, though, is their level of fit and finish.
[1320.08 --> 1324.26]  Their enclosures are beautiful and their software is really great as well.
[1324.56 --> 1327.14]  I'm talking about their disk station management software.
[1327.96 --> 1330.80]  DSM is like using a desktop session inside a browser.
[1331.10 --> 1333.30]  It's really cool if you haven't seen it.
[1333.30 --> 1338.42]  And we've got a link for a live demo for you at selfhosted.show slash Synology.
[1339.04 --> 1344.72]  This simple and intuitive UI is perfect for those just getting started on their self hosting journey.
[1344.94 --> 1347.28]  I've used Synology now for many years.
[1347.40 --> 1350.58]  I still can't quite believe how they pulled this off in a browser.
[1351.32 --> 1358.92]  You can also find tons of apps available in their built in store, as well as community provided repos and more recently Docker support.
[1358.92 --> 1363.68]  With this Docker support, you can run darn near anything you like on these boxes.
[1364.28 --> 1368.66]  And remember that with that Ryzen chip, you've got full x86 compatibility.
[1368.66 --> 1371.36]  So there's no ARM weirdness going on here.
[1372.10 --> 1380.08]  To find out more about Synology and their other NAS products, visit selfhosted.show slash Synology so that they know we sent you and to support the show.
[1380.20 --> 1382.98]  A big thanks to Synology for sponsoring our show.
[1384.84 --> 1388.66]  Synology wanted us to actually have a chance to try out some of their hardware.
[1388.66 --> 1390.70]  And so we thought we'd share our thoughts with you.
[1390.76 --> 1395.04]  And they sent a DS1621 Plus to Alex to kick the tires.
[1395.46 --> 1396.54]  They did indeed, yes.
[1396.66 --> 1400.50]  So I am the proud recipient of a Ryzen-powered NAS.
[1400.70 --> 1401.50]  That's pretty neat.
[1401.84 --> 1404.66]  That left me thinking, how do I go about reviewing a NAS?
[1404.76 --> 1409.34]  Because it's, you know, it's something you just throw files on and forget about for the next few years.
[1409.52 --> 1413.12]  And when I hear Ryzen, I think it probably has a fair amount of CPU power in that thing.
[1413.48 --> 1414.80]  This is one of their embedded chips.
[1414.88 --> 1416.66]  This is the Ryzen V1500B.
[1416.66 --> 1421.88]  It's a 4-core, 2.2GHz, 8-thread CPU.
[1422.74 --> 1427.60]  And it supports up to 32GB of ECC memory, which is pretty nice.
[1428.04 --> 1434.84]  The motherboard built into the Synology also has a couple of NVMe slots, which I thought was particularly interesting.
[1434.84 --> 1442.62]  And one of the things, actually, that I was most disappointed about with the COBOL, you know, the Helios 64, was that it was a 5-bay NAS.
[1443.28 --> 1448.44]  But if you used the NVMe slot that came with it, you turned it into a 4-bay NAS.
[1448.52 --> 1449.76]  Well, there's none of that going on here.
[1449.84 --> 1455.78]  This remains to be a 6-bay NAS with two extra PCIe NVMe slots as well.
[1455.78 --> 1460.00]  So you can fit effectively eight drives in this thing, which is great.
[1460.66 --> 1461.00]  That's great.
[1461.06 --> 1461.58]  Yeah, that is.
[1461.86 --> 1465.02]  Now, the fit and finish really is next level on this thing.
[1465.12 --> 1470.36]  Within five minutes of taking it out of the box, I had the drive cages removed.
[1470.36 --> 1478.94]  With the tool-less, hot-swappable drive cages they have, I had the drives installed, put them into the enclosure.
[1479.34 --> 1484.92]  One important thing to note is that you must populate the first drive slot with a drive.
[1485.06 --> 1487.28]  And if you don't, the Synology will fail to boot.
[1487.38 --> 1492.98]  And I assume this is because they're installing the DSM OS onto that first drive.
[1492.98 --> 1501.72]  Now, I don't know what that means for the long-term reliability of a spinning drive in that first slot, but it's something I can report back on in a few months' time.
[1502.12 --> 1502.52]  Yeah.
[1502.98 --> 1507.14]  And it could just be that maybe it just doesn't proceed because what's the point of a NAS with no disk?
[1508.10 --> 1513.04]  Well, you say that, but these things have full-on app stores these days, and they can run Docker as well.
[1513.18 --> 1521.30]  So, you know, you could conceivably buy a Synology unit and not put any drives in it and still run some services if you liked.
[1521.30 --> 1523.16]  I don't know why you would, but you could.
[1523.90 --> 1525.80]  It is easy to deploy applications on, I suppose.
[1525.96 --> 1527.06]  So that's a good point.
[1527.48 --> 1531.20]  I'm curious about just physical size and noise and those kinds of things.
[1531.26 --> 1531.88]  How is all that?
[1532.12 --> 1532.62]  And how big?
[1532.74 --> 1534.76]  Like, give me an idea of, like, how much space this thing takes up.
[1535.06 --> 1535.78]  Noise is great.
[1536.38 --> 1539.02]  The fans that are included in the unit are very, very quiet.
[1539.52 --> 1546.20]  I've actually had it in a closet right just off my office, you know, a few feet from where we're sat right now.
[1546.92 --> 1549.16]  And I close that door and I can't hear it.
[1549.16 --> 1551.28]  It's just, oh, it's pretty quiet.
[1551.36 --> 1559.06]  You'll hear if it's on the desk next to you, but that's more a result of the fact of having mechanical hard drives than it is fan noise right next to you.
[1559.78 --> 1567.00]  In terms of the size of the thing, it's, I think, it's about five kilos, give or take.
[1567.54 --> 1571.20]  I don't know, the footprint's about the size of a 16-inch laptop, maybe a little bit less.
[1571.20 --> 1575.12]  And then, I don't know, nine inches tall or so.
[1575.88 --> 1580.78]  Basically, think of six hard drives lying on their side with a couple of inches either side.
[1581.12 --> 1581.92]  That absolutely makes sense.
[1582.00 --> 1585.62]  And now, also, I think that means you're a ButterFS user, which I think is fantastic.
[1586.06 --> 1588.00]  Well, it would if I'd chosen ButterFS.
[1588.34 --> 1588.94]  Oh, you sure.
[1588.94 --> 1589.76]  Which I did, I did.
[1589.88 --> 1590.34]  I'm such a tease.
[1590.36 --> 1590.74]  Oh, okay.
[1591.48 --> 1592.92]  Hello, welcome to the club.
[1593.30 --> 1595.34]  You and I are now running ButterFS at home.
[1595.34 --> 1600.66]  But the reason I picked ButterFS is because it enables compression and snapshots.
[1601.28 --> 1608.58]  And that's an option that's exposed to the users at the time of creating the array or the volume of storage in the DSM software.
[1608.92 --> 1610.56]  So, let's talk about software for a little bit.
[1610.62 --> 1616.88]  So, this thing does run the DSM, which is their OS, and it has a nice interface on it, which has an app store.
[1617.64 --> 1620.50]  But you are, you know, you're a long-termer.
[1620.62 --> 1624.72]  You don't necessarily always like the graphical environments on top of stuff in the management tool.
[1624.72 --> 1626.20]  So, how did you handle all of that?
[1626.26 --> 1627.06]  How did you react to it?
[1627.10 --> 1627.70]  What were your thoughts?
[1628.12 --> 1630.98]  So, I'll tell you who I think this system is actually perfect for.
[1632.04 --> 1638.42]  It's those people just getting started in self-hosting who want their hand-holding a little bit,
[1638.66 --> 1645.30]  but are also comfortable with the idea that they have to learn some stuff to, you know, run these services.
[1645.96 --> 1650.28]  And through the UI, you are guided through the process of setting up Docker containers,
[1650.28 --> 1656.82]  of sharing folders, of doing file service sharing, like Samba, and all the rest of it, you know,
[1656.86 --> 1660.82]  like time machine backups and all that kind of stuff, creating users.
[1661.24 --> 1667.16]  A lot of times, people ask me when they read the perfect media server, what's the best GUI?
[1667.38 --> 1668.74]  And I'm like, well, it's the command line.
[1669.00 --> 1669.22]  Silly.
[1669.66 --> 1671.44]  But actually, I think it's something like this.
[1671.44 --> 1677.62]  I don't think a really good GUI for server management on Linux truly exists.
[1677.72 --> 1684.10]  I know you like cockpit, but I don't think there's anything quite on this scale for vanilla Linux.
[1684.86 --> 1684.88]  Right.
[1684.98 --> 1685.94]  Nothing this straightforward.
[1686.16 --> 1688.38]  Nothing this straightforward and nothing this comprehensive.
[1688.80 --> 1688.98]  Yeah.
[1689.14 --> 1690.70]  This does a lot more than cockpit.
[1690.90 --> 1691.88]  Yeah, it absolutely does.
[1692.52 --> 1695.68]  And sometimes that can be to its detriment because you think, right,
[1695.68 --> 1700.60]  I just want to have a compose file and paste it in and create these five containers like this, please.
[1701.16 --> 1701.56]  Right.
[1701.78 --> 1707.26]  Whereas with the UI that Synology has, you have to click through a few things and create volumes.
[1707.50 --> 1712.18]  And all the knobs and switches are labeled all the same as they would be in a compose file.
[1712.38 --> 1714.28]  But you just have to go through and click them.
[1714.72 --> 1718.36]  Which, you know, if I'm trying to explain this to my mother over the phone, for example,
[1719.12 --> 1724.08]  and she's actually had a Synology unit in her house now for, I want to say, five years.
[1724.08 --> 1727.74]  And I've not really had to touch it or think about it.
[1727.82 --> 1730.56]  I mean, it just keeps on working, this thing.
[1730.88 --> 1736.96]  And I think the long-term outlook for this Synology unit, for me, is going to be,
[1737.42 --> 1738.70]  it's going to end up at a parent's house.
[1739.04 --> 1740.88]  Which is no bad thing, in my opinion.
[1741.00 --> 1746.24]  I think it's a sign of, you know, I said this a few episodes ago.
[1746.32 --> 1750.54]  I bought a Raspberry Pi for eight gig and an external USB hard drive.
[1750.54 --> 1757.90]  And I've been having the most difficult time trying to get that thing to USB boot with my sister's fiancé,
[1758.02 --> 1763.24]  trying to talk him through how to set the Raspberry Pi up with USB boot and then flash it remotely.
[1763.64 --> 1765.54]  And, oh, what a pain.
[1765.80 --> 1770.22]  And I'm thinking to myself, well, if I just had this Synology, I could just send it to them.
[1770.28 --> 1771.66]  And it looks nice.
[1771.72 --> 1772.70]  It's nice and quiet.
[1772.88 --> 1777.00]  There's no cables to be unplugged by the cat, you know.
[1777.00 --> 1783.12]  I think Angela's been running one at her house for probably seven to eight years.
[1783.30 --> 1784.22]  I don't even know.
[1784.36 --> 1787.26]  It's crazy how long that thing has been running.
[1787.72 --> 1789.64]  So it seems like it's been pretty solid.
[1789.98 --> 1795.58]  I think for the people who like to deploy something and then begin to figure it out and learn how it works,
[1795.72 --> 1797.52]  it fits that so well.
[1798.22 --> 1801.24]  I worked with Synology to get one of these for Wes for Christmas.
[1801.24 --> 1809.34]  Because it's not that Wes doesn't know how to manage a server, obviously, but he just doesn't really have the time.
[1809.42 --> 1810.90]  He's got other stuff to do, right?
[1810.90 --> 1819.18]  He still wants to be able to run Jellyfin, in his case, and manage his media and save files to a centralized location on his network.
[1819.54 --> 1824.54]  But he doesn't have the time to build a box and set up all of the services, even though he knows how.
[1824.54 --> 1827.10]  And so I thought a Synology would be perfect for him, too.
[1827.16 --> 1833.60]  And so we say it's for beginners, but it's also just for people who got a lot going on.
[1833.72 --> 1841.24]  Like people just kind of like in your situation that just maybe have a little less time or interest in building it completely from scratch.
[1841.72 --> 1842.72]  I think I agree totally.
[1842.72 --> 1849.84]  Now, one thing I would like to discuss is the version of Docker that's running on the NAS.
[1850.08 --> 1856.32]  And it's running 18.09, which, as the name suggests, comes from 2018.
[1856.88 --> 1863.26]  So what this means is if you SSH into the Synology, you can get in behind the scenes and go and tinker with what's going on.
[1863.64 --> 1871.16]  And you think to yourself, great, I'm just going to use Docker Compose and I will circumvent the UI and just do it that way.
[1871.16 --> 1879.20]  But unfortunately, because that version of Docker is so old, it means a lot of the newer features in Docker Compose aren't supported.
[1879.46 --> 1883.90]  So you then think to yourself, hmm, I could upgrade the version of Docker, couldn't I?
[1884.02 --> 1885.16]  And yes, you can.
[1885.24 --> 1889.00]  There is a GitHub repo to do that in an unsupported fashion.
[1889.00 --> 1896.98]  And then you quickly run into all sorts of problems trying to figure out how networking bridging works and all that kind of stuff and wish you'd never bothered.
[1896.98 --> 1903.92]  So my recommendation with Docker would be to just stick to the UI on the Synology and it will just work brilliantly.
[1904.78 --> 1912.46]  And then if you're a crazy kid like Alex, you could just end up using your Synology as an iSCSI endpoint and point your VMware infrastructure at it.
[1912.94 --> 1913.78]  That's true, actually.
[1913.88 --> 1918.60]  Yeah, you see Synologies in the backgrounds of so many tech YouTuber videos.
[1918.60 --> 1923.84]  Network Chuck, Lawrence Systems, Tom from Lawrence Systems.
[1924.04 --> 1926.40]  They've all got Synologies blinking away in the background.
[1926.52 --> 1931.62]  And I've often wondered, what are these guys that surely know better, right?
[1931.84 --> 1932.52]  In air quotes.
[1932.96 --> 1934.90]  What are they all doing with their Synologies?
[1935.04 --> 1941.08]  And it turns out, actually, if you fill this sucker up with SSDs and put a 10 gig networking card in there,
[1941.08 --> 1949.62]  you can get some seriously good performance over iSCSI with VMware, which Synology have worked very hard to get the official certification for.
[1950.04 --> 1954.14]  Yeah, I remember we were talking to Wendell and he even thought that was pretty remarkable back in the day.
[1954.70 --> 1955.94]  But it is pretty good to see it.
[1955.98 --> 1957.64]  And a nice little HomeLab addition.
[1958.00 --> 1965.72]  So if you have something like an Intel NUC that doesn't have much storage and you want a cheap way to add, you know, six, eight or more drives,
[1965.72 --> 1975.04]  because Synology offer a lot of different products, buy Synology, use iSCSI, and then your NUC suddenly has, you know, 20 terabytes to go at.
[1975.52 --> 1976.20]  I can see it too.
[1976.30 --> 1982.12]  Like, maybe one day I'll have all these Raspberry Pis and then there'll just be one centralized storage.
[1982.50 --> 1984.04]  To be able to support VMware is pretty great.
[1984.16 --> 1991.24]  But when you were messing around with this, one thing I didn't hear you talk about was if you dug into what your backup options would be,
[1991.24 --> 1996.86]  if you felt like you were limited, maybe by the DSM, by what your backup options could be.
[1997.00 --> 1998.22]  What was that experience like?
[1998.50 --> 1999.64]  Well, it's not running ZFS.
[1999.96 --> 2005.88]  So I needed a way in which to do version snapshots and incremental backups.
[2006.58 --> 2013.30]  Incremental backups are really important because rather than sending the entire file system every single time,
[2013.84 --> 2016.28]  it only sends the bits and bytes that have changed.
[2016.28 --> 2024.76]  Now, ZFS does this at the block level, but because I'm going from ZFS to ButterFS, there's no mechanism in place to do that.
[2025.34 --> 2031.46]  Now, I could use R-Sync, but then it's going through and it's checking MD5 hashes every time, and it can be a bit slow and a bit clunky.
[2032.24 --> 2034.32]  And I tripped over something called Minio.
[2034.92 --> 2038.22]  I actually mentioned this, I think, with the orange one last week.
[2038.22 --> 2042.66]  I tripped over Minio, which is a S3 front end.
[2043.02 --> 2049.62]  Now, this provides the S3 object storage API on your LAN, effectively, backed by your own storage.
[2050.14 --> 2061.50]  Now, the advantage that that gives you is that you can use a tool such as Restic to do incremental version snapshot backups to this S3 endpoint backed by the Synology.
[2061.50 --> 2066.56]  All right, so pause, because this is a big deal, and this is probably something we should dedicate an entire episode to,
[2066.68 --> 2072.90]  but this lets you build your own S3 object storage on your LAN or maybe up in the cloud.
[2073.40 --> 2075.92]  There's a lot of ways you could use this if you think about it.
[2076.58 --> 2080.30]  Yeah, we should come back to this as a separate topic, but okay, so let me unpack this.
[2080.32 --> 2089.32]  So you have something like this set up on your LAN running, exposing some storage that you're then making available to the DSM software, or how does this work?
[2089.32 --> 2090.98]  Minio is running as a container.
[2091.18 --> 2096.78]  That's then backed by a volume mount to one of the volumes on the Synology itself.
[2097.02 --> 2102.22]  Lots of volumes terms going on here, but that's where it gets a little confusing.
[2102.96 --> 2105.96]  So essentially what happens is Minio is running as a container.
[2106.38 --> 2117.60]  It presents itself as an API that I can then call from Restic, and Restic will then just store the data on those S3 buckets as objects.
[2117.60 --> 2124.00]  That's worth doing too, Alex, because it seems like you could use that for other stuff in the future as well, because there's a lot of things that will just plug right into that.
[2124.18 --> 2127.72]  It does free you up from the ZFS kind of train, if you like.
[2127.72 --> 2138.06]  So if something like ZFS.rent isn't up your street, and you want to host just a few hundred megabytes of files, then something like Restic is going to do you really well.
[2138.54 --> 2141.62]  One of the most difficult parts of using Restic is configuring it.
[2142.08 --> 2148.66]  Now, I came across a project this week which solves that problem in a really beautiful way called AutoRestic.
[2148.66 --> 2158.60]  Now, there's a link to this thing in the show notes, but essentially what happens is you define the locations and the backends in a YAML file, and you're done.
[2159.08 --> 2160.22]  That's not so bad to manage.
[2160.38 --> 2164.10]  I mean, that sounds like something that I could probably wrap my head around.
[2164.34 --> 2177.26]  What's really nice as well is if you just have a local backend, which is just some dumb USB hard drive, you can actually have as one of your backends just HDD type local path, my external storage.
[2177.26 --> 2178.92]  And it's as simple as that.
[2179.24 --> 2182.50]  Oh, although my backend is never dumb, but that does seem really nice.
[2183.04 --> 2184.86]  I didn't mean it as an insult, darling.
[2186.72 --> 2190.54]  There's a bunch of other cool stuff that AutoRestic supports as well, like hooks.
[2190.74 --> 2201.80]  So if you want to perform some commands before or after a specific backup, let's say you want to delete some files after a backup's happened, for example, you can do that using the hooks that are built into AutoRestic.
[2202.22 --> 2204.40]  You can also exclude files as well.
[2204.84 --> 2206.20]  And there is a forget policy.
[2206.20 --> 2224.56]  So one of the favorite things about ZFS Send for me is when I use Jim Salter's Sanoid tool, it has a policy-driven snapshot engine, which will automatically keep the last hour or the last six hours and then the last six days and then the last six weeks and then the last six months.
[2224.72 --> 2227.88]  It will keep one snapshot from each of those different timestamps.
[2227.88 --> 2237.84]  AutoRestic also has a forget and prune policy engine built right into it, which you configure again in the YAML right next to the location that you're defining.
[2238.26 --> 2240.96]  It's just, it's the way Restic should work.
[2241.44 --> 2242.44]  Yeah, that does sound nice.
[2242.90 --> 2243.60]  Well, very good.
[2243.60 --> 2247.76]  We will have a link to that at selfhosted.show slash 43.
[2248.14 --> 2252.38]  Now, before we go, Alex, Jace Novell wrote in on the Discord.
[2252.62 --> 2255.16]  So I guess that's more like sent a message on Discord.
[2255.42 --> 2257.56]  And then we thought that's a good question to read on the show.
[2257.66 --> 2261.72]  But he says, I'm working through the planning stages of building a new home.
[2262.06 --> 2263.54]  Oh, I love that.
[2263.64 --> 2263.88]  Yeah, Lee.
[2263.88 --> 2264.78]  Oh, I'm envious.
[2265.12 --> 2265.28]  Yeah.
[2265.62 --> 2275.54]  He writes, if you're all starting from scratch, how would you design a smart home that would get the wife approval factor, but at the same time, not be too much overkill?
[2275.90 --> 2280.74]  Well, that actually feels like that's how you achieve the wife approval factor is by not going overkill.
[2280.88 --> 2283.26]  But I get the spirit of his question.
[2283.38 --> 2289.22]  Like, what's a reasonable kind of build it in while I have the opportunity, but not go excessive?
[2289.82 --> 2292.14]  Automated flamethrowers on the driveway should do the trick.
[2292.14 --> 2295.52]  Right, and don't forget laser pointers on articulating arms.
[2296.38 --> 2301.16]  So that way you can, you know, you can just put that out there and that way the pets stay entertained.
[2301.32 --> 2307.24]  No, but really thinking about it, it comes down in my mind, like the first place I go to is just solid networking.
[2307.58 --> 2312.12]  Whilst you've got those walls open, run as many high quality cables as you can.
[2312.32 --> 2312.50]  Yeah.
[2312.62 --> 2315.24]  I would suggest starting with Cat6A as a minimum.
[2315.86 --> 2317.74]  Yes, it could be considered a little bit overkill.
[2317.74 --> 2324.38]  You know, 5E will do quite comfortably gigabit ethernet and even, it'll even do 10 gig over a very short distance.
[2324.66 --> 2327.94]  But Cat6A will give you 10 gig guaranteed.
[2328.20 --> 2331.30]  I think it's like three or 500 feet, something like that.
[2331.30 --> 2341.90]  And if you're thinking about the lifetime of a house, which could be 50 plus years, you really want to put in there as good as you can afford to at the time you're building it.
[2341.94 --> 2347.70]  Because having retrofitted a couple of houses with ethernet cable, let me tell you, pulling cable is no fun.
[2347.70 --> 2354.20]  It's how you'll do everything from cameras to smoke detectors to sensors to Wi-Fi endpoints.
[2354.90 --> 2359.70]  Everything's better with ethernet or just workstations, televisions, media set top boxes.
[2360.16 --> 2362.10]  You'll never beat wired.
[2362.26 --> 2366.60]  As good as wireless gets, it cannot just beat a physical copper connection.
[2366.80 --> 2368.96]  It's just the reality of physics right now.
[2369.06 --> 2371.52]  And I just so completely agree with Alex.
[2371.58 --> 2375.98]  I have a buddy right now who is building a tiny home and it's a really cool place.
[2375.98 --> 2387.66]  And in this tiny home, which is probably 250 square feet, I don't actually know, he has 18 ethernet jacks in different places.
[2387.66 --> 2389.36]  Some of them are multiple panels and stuff.
[2389.62 --> 2391.12]  But, you know, you think about it.
[2391.20 --> 2392.40]  That's how he's going to do his phone.
[2392.72 --> 2394.18]  That's how he's going to do all of his TV.
[2394.46 --> 2396.58]  HDMI is going to be over ethernet in the wall.
[2397.12 --> 2398.46]  That's how he's going to do all of his cameras.
[2398.60 --> 2399.88]  That's how he's going to do his desk.
[2400.24 --> 2402.36]  That's how he's going to bring his internet connection in.
[2403.02 --> 2405.92]  I really just completely, totally agree with you, Alex.
[2406.24 --> 2408.76]  And it would be nice as well not to have to daisy chain switches.
[2409.18 --> 2413.60]  One of the ways in which I extend the ethernet around some of the larger rooms in this house,
[2414.26 --> 2419.28]  in walls that are more difficult to pull cable through, like external walls, stuff with insulation in,
[2419.74 --> 2423.72]  I actually just run an ethernet cable along the skirting board, the baseboard,
[2423.72 --> 2427.58]  and then have a switch and then just carry on.
[2427.66 --> 2431.86]  So actually, if I think about it between the switch that's carrying my voice to you,
[2432.46 --> 2433.90]  there's probably four switches.
[2435.02 --> 2437.04]  It's a horrible network design, but it works.
[2437.04 --> 2441.66]  I wish I could shake up so many industries too, like the hotel industries should all be putting
[2441.66 --> 2443.38]  ethernet in the rooms for me to use.
[2443.94 --> 2444.40]  RVs?
[2444.46 --> 2448.92]  Oh my gosh, Alex, I wish the RV manufacturers would build an ethernet to every RV.
[2449.48 --> 2450.72]  All home manufacturers.
[2450.96 --> 2452.72]  You shouldn't build a home today without ethernet.
[2452.82 --> 2455.64]  And it's happening still, Alex, in 2021.
[2455.64 --> 2458.92]  Without ethernet, but also without a proper server cupboard.
[2459.50 --> 2464.56]  And I think, you know, having some kind of a central place where all that ethernet comes into
[2464.56 --> 2469.94]  with a patch panel and space for all the different bridges that you need these days,
[2470.02 --> 2474.42]  your Zigbee bridge, your Z-Wave bridge, your Philips Hue light bulb bridge,
[2474.90 --> 2475.74]  all this kind of stuff.
[2475.80 --> 2478.98]  Like the solar installer came and did a survey on my roof last week,
[2478.98 --> 2481.68]  and he said, can I take a look at your internet router?
[2481.68 --> 2488.50]  And I'm like, okay, this is going to be complicated unless you tell me why you need to see that.
[2489.52 --> 2493.84]  And he said, well, we have this monitoring thing that connects via Zigbee to the solar
[2493.84 --> 2498.34]  on the roof and does a bunch of, you know, consumption monitoring stuff.
[2498.44 --> 2500.30]  And I said, okay, so tell me what you need.
[2500.34 --> 2501.44]  Is it just an ethernet jack?
[2501.50 --> 2502.28]  And he went, yes.
[2502.46 --> 2503.70]  I'm like, I've got you covered.
[2504.96 --> 2506.62]  Yeah, that's a great example.
[2506.80 --> 2509.00]  But just so many other things.
[2509.00 --> 2515.76]  Like you'll have like your ISPs box you need to put somewhere and like a phone or a cable television thing
[2515.76 --> 2517.36]  if you go that route.
[2517.54 --> 2522.12]  So absolutely think of that and think of noise because some of these things that you're going to have in that space,
[2522.16 --> 2525.12]  like a switch, have very loud fans.
[2525.72 --> 2529.58]  Also, just before we completely go away from ethernet, label, man.
[2530.20 --> 2535.44]  The first, a couple of times, the first time and then a second time, but no, no, nonsense.
[2535.44 --> 2539.60]  But a couple of times, twice in a row, unfortunately, I got screwed.
[2539.76 --> 2542.48]  And the guys that did my ethernet didn't properly label stuff.
[2542.72 --> 2544.52]  And it is such a pain in the arse.
[2544.92 --> 2545.80]  Let me tell you.
[2546.22 --> 2548.44]  So label everything you're doing.
[2548.68 --> 2549.68]  Consider fan noise.
[2549.84 --> 2550.62]  Consider heat.
[2551.12 --> 2552.30]  Because that could also be a problem.
[2552.36 --> 2558.52]  Because if it was me, I would like to have my switch and my server and all of that in the same space.
[2558.52 --> 2566.20]  So if I were really designing everything from scratch, I may actually consider putting all of that in my garage where I have a little room built off.
[2566.84 --> 2571.88]  Anything you can do now is an investment that will save you problems later because you're going to have heat issues.
[2571.88 --> 2573.06]  You're going to have power issues.
[2573.10 --> 2574.56]  You're going to have noise problems.
[2574.76 --> 2576.94]  You're going to have growth and sprawl problems.
[2576.94 --> 2581.60]  So if you can give consideration to that in some way, I absolutely would think of that.
[2581.66 --> 2588.68]  And then also maybe if you're going to do cameras, consider doing something like PoE from the start and how you might build for that.
[2589.16 --> 2589.22]  Absolutely.
[2589.70 --> 2594.24]  And one of the other things I would consider in that server cupboard is you mentioned heating and cooling.
[2594.46 --> 2598.84]  But I would suggest if you can get a dedicated electrical circuit just for that equipment.
[2598.84 --> 2608.60]  It would make things much easier to troubleshoot if that room with thousands, probably thousands of dollars worth of equipment in it has its own electrical supply.
[2609.04 --> 2613.34]  And you could build a UPS type system in around it as well.
[2613.58 --> 2616.78]  But it's possible that that thing is going to be drawing quite a few amps.
[2617.06 --> 2621.00]  So it's worth having that separate circuit.
[2621.56 --> 2628.04]  And if you did later want to have like a backup power supply for that, or maybe you wanted even solar power or something like that.
[2628.04 --> 2634.24]  If you have that gear already isolated on its own circuit, that just got way simpler down the road.
[2634.74 --> 2636.00]  So that's something to think of too.
[2636.56 --> 2639.76]  And you really, I don't think you can overdo it with Ethernet.
[2639.84 --> 2642.90]  And I don't think you can overdo it with circuits for independent stuff.
[2643.42 --> 2649.86]  When I had my place built years and years ago, which I don't live in anymore, but I had a circuit for my home office.
[2650.00 --> 2651.70]  Oh, actually, and here I did it in the studio too.
[2651.76 --> 2657.50]  Now that I think about it, the studio has three separate power circuits just in the studio.
[2657.50 --> 2662.74]  The reason for that is really overkill because of ground loops and noise like that.
[2663.32 --> 2669.56]  And then our offices upstairs, each room upstairs is on its own circuit because we run so much computer gear.
[2670.04 --> 2672.80]  We didn't want to be popping each other's breakers.
[2673.20 --> 2677.86]  I never used to really worry about that when I lived in England because obviously everything's at 220 volts over there.
[2677.96 --> 2679.48]  So half the amps.
[2680.00 --> 2683.58]  But over here at 110 volts, it really makes a difference.
[2683.58 --> 2685.66]  Yeah, so those are, I don't think they're overkill.
[2685.78 --> 2694.82]  And the way you sell them is in long-term reliability and a reducement in replacements, in hacky solutions, and in stress.
[2695.12 --> 2700.80]  And just learning from people who have tried this the cheaper way and have had to make adjustments since.
[2700.88 --> 2702.90]  And if it's your only route, you'll make it work, man.
[2702.90 --> 2703.38]  No problem.
[2703.38 --> 2709.72]  But if you do have the ability to do some of this stuff ahead of time, man, future you is going to be so thankful.
[2710.28 --> 2711.38]  Yes, absolutely they will.
[2711.50 --> 2718.96]  Having retrofitted a few houses myself, I can tell you there is nothing worse than going through a crawl space with cockroaches trying to pull ethernet.
[2719.16 --> 2720.92]  So save yourself some headaches.
[2721.58 --> 2726.64]  Now, if you'd like to get your question answered or discussed on the show, you can go to selfhosted.show slash contact.
[2726.64 --> 2727.64]  There you go.
[2728.12 --> 2732.20]  And also selfhosted.show slash SRE if you'd like to become a member.
[2732.56 --> 2737.88]  You support the show, you get a limited ad feed, and you get extra content a post show.
[2738.20 --> 2742.62]  And I think it's like $5 a month, which is like our best deal on the network right now.
[2743.06 --> 2746.96]  Selfhosted.show slash SRE and get additional content.
[2747.64 --> 2748.50]  Best deal for the best show.
[2748.66 --> 2749.08]  Dang right.
[2750.74 --> 2753.70]  Now, you just launched jupitergarage.com, didn't you?
[2753.70 --> 2757.18]  Man, you and I, I know you have the same problem.
[2757.32 --> 2758.22]  Way too much gear.
[2758.64 --> 2759.70]  Stuff's all over the place.
[2759.80 --> 2763.22]  So jupitergarage.com, we've been selling off some things that we have in the studio.
[2763.52 --> 2766.66]  Plus, I've kind of mixed it with some original stuff in there.
[2767.32 --> 2777.16]  And you and I were talking about it, and we were thinking now that you've got a different NAS situation, maybe we ought to put the Helio 64 in the garage sale.
[2777.58 --> 2777.74]  Yeah.
[2777.98 --> 2779.44]  Well, I'm not really using it for anything.
[2779.64 --> 2783.12]  So I figured I'll save someone else having to wait for it to be delivered.
[2783.12 --> 2788.20]  So we'll put it on there for a good price, and it'll go live on Monday, which will be April the 26th.
[2788.46 --> 2789.84]  Yeah, jupitergarage.com.
[2789.96 --> 2792.96]  I just sold the free NAS that I used to have here in the studio.
[2793.52 --> 2794.44]  I sold it for $200.
[2795.14 --> 2796.26]  Man, that is a steal.
[2796.82 --> 2797.32]  Yeah, it is.
[2797.42 --> 2801.38]  You know, in some part, it's just because I don't – this gear's just been sitting around anyways.
[2801.80 --> 2803.94]  So it's not like I'm doing anything with it.
[2804.06 --> 2806.42]  Might as well go to a home with somebody in the audience.
[2806.54 --> 2808.10]  That just seems like kind of awesome, you know.
[2808.10 --> 2812.38]  So, yeah, the Helio 64, it will probably go pretty fast.
[2813.04 --> 2820.30]  So maybe we should say Monday a.m. Seattle time just to kind of give people an expectation.
[2820.64 --> 2820.96]  Absolutely.
[2821.44 --> 2822.80]  All right, jupitergarage.com.
[2822.90 --> 2826.20]  Also, you can find our sponsor, Cloud Guru, on social media.
[2826.36 --> 2826.82]  It's simple.
[2826.92 --> 2829.22]  They're just slash a Cloud Guru everywhere.
[2829.22 --> 2834.22]  And if you're looking for all the different ways to subscribe to the show, you can go to selfhosted.show slash subscribe.
[2834.66 --> 2836.50]  I'm on Twitter at Ironic Badger.
[2836.92 --> 2839.32]  Yeah, I'm there too, at Chris L-A-S.
[2839.46 --> 2842.80]  And the whole show right here, this show, this one, at Self Hosted Show.
[2843.00 --> 2843.46]  This show?
[2843.80 --> 2844.26]  Which show?
[2844.48 --> 2844.90]  This show?
[2845.00 --> 2845.48]  The whole show?
[2845.74 --> 2846.56]  This one, yeah.
[2846.90 --> 2847.84]  No, the whole thing.
[2848.04 --> 2851.82]  It's all there in just the hundred and whatever it is characters now, 200 and whatever.
[2852.18 --> 2855.16]  Actually, it's really just a good resource to get show announcements and news.
[2855.44 --> 2857.04]  And maybe send us questions, I suppose.
[2857.04 --> 2859.82]  And if all that isn't too much for you, I'd like to thank you for listening.
[2860.06 --> 2862.42]  That was selfhosted.show slash 43.
