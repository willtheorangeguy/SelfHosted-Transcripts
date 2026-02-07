[0.00 → 4.96] Coming up on today's show, we have Jeff Deerling. You may know him as Deerling Guy in Ansible Galaxy.
[5.42 → 8.62] He's also on a bunch of work recently with the Raspberry Pi.
[9.48 → 16.28] Chris loses his mind a little bit when Jeff tells him how he hooked up 16, yes, 16 drives to a Raspberry Pi.
[16.70 → 17.22] I'm Alex.
[17.64 → 19.82] I'm Chris, and this is Self-Hosted 41.
[21.06 → 25.40] Alex, we have a lot to talk about today, and we also have a special guest.
[25.40 → 33.12] We do indeed, yes. We have Deerling Guy, Jeff Deerling, the Raspberry Pi Ansible maestro, all the sorts of superlatives.
[33.74 → 37.52] My new YouTube habit. I love what he's putting out.
[37.58 → 38.78] Yeah, I thought you might like him.
[40.04 → 43.92] Yeah, I do. I want to say thanks to a Cloud Guru for sponsoring this episode.
[44.06 → 47.28] They are the leader in learning for the cloud, Linux, and other modern tech skills.
[47.38 → 49.52] Get hundreds of courses, thousands of hands-on labs.
[49.94 → 53.66] Get certified, get hired, get learning at cloudguru.com.
[53.66 → 58.54] So the interview really will be the bulk of the show today, because there are so many great things we get into.
[58.96 → 64.72] But before we start, I kind of wanted to chat with you about Nebulas buying ESP Home.
[65.24 → 65.94] How do you feel about it?
[65.98 → 70.18] I mean, when I first heard the news, I was like, oh, I wasn't quite sure how to feel.
[70.18 → 79.32] And then some more details trickled out about how the original creator, Otto, was, you know, basically burning out.
[79.32 → 84.56] And I think overall, it's a great way to save an open source project.
[84.56 → 91.56] That is one of my personal favourite ways to configure, you know, ESP boards.
[92.24 → 94.88] It's a clear value for the Home Assistant community.
[95.60 → 97.34] And this was, you're right.
[97.42 → 100.62] I had my first read of this was sort of like, I'm not so sure.
[100.62 → 103.10] Because they're a small team with a lot to do.
[103.42 → 110.28] But when you read between the lines, it seems pretty clear that Otto was about to hit the nope out button.
[110.88 → 115.46] And the project would have been left without its leader and lead developer.
[116.10 → 119.26] This is kind of nice because this gives the project room to grow.
[119.44 → 121.12] It'll bring in some new contributors.
[121.80 → 123.16] Otto is taken care of.
[123.46 → 126.90] He's able to participate if he likes, but, you know, he's going to focus on life for a bit.
[126.94 → 128.26] He's shutting down the Patreon account.
[128.26 → 131.24] He doesn't have to worry about the management side of things.
[131.88 → 134.72] And it continues to be a free software project.
[135.48 → 141.68] And if anything, I would expect it will be even tighter integrated into Home Assistant now.
[141.94 → 142.98] We're seeing some of that already.
[143.48 → 152.16] Frank, one of the main developers for Home Assistant, has already made some significant improvements to the VS Code plugins for how that interfaces with ESP Home.
[152.56 → 155.44] So there's some autocomplete stuff coming and things like that.
[155.44 → 159.46] But let's just back up a little bit and explain what ESP Home is.
[160.10 → 168.16] So the way I got started with it was I was programming these ESP8266 single board computers, if you like.
[168.24 → 171.80] They're kind of in the same space as an Arduino, more than a Raspberry Pi.
[172.06 → 173.34] So they don't run a full OS.
[173.42 → 175.56] They actually run a precompiled firmware.
[175.56 → 186.20] And that used to require writing an Arduino sketch and uploading it to the board and, you know, all the stuff that comes with the Arduino IDE and universe and that kind of thing.
[186.74 → 194.48] And what ESP Home does, and it is pure magic in my opinion, is you define the firmware as a YAML file.
[194.48 → 205.24] You add a couple of modules here with a couple of lines to, you know, enable Wi-Fi and then another couple of lines to enable logging and then another couple of lines to enable the Home Assistant API, for example.
[205.96 → 217.28] And then you flash that binary that is generated from the YAML file onto the ESP8266 without having to write a single line of C code or whatever the Arduino equivalent would be.
[217.28 → 219.90] And it just makes it so approachable.
[220.36 → 223.84] Yeah, and there are so many devices that run off this type of firmware out there.
[224.40 → 230.04] And you can really see long term the value that Home Assistant, if Home Assistant can make this even simpler.
[230.84 → 238.88] Imagine a future, if you would, Alex, where Home Assistant could even auto-detect devices and guide the user through generating the firmwares.
[239.18 → 244.08] And maybe even has a way to deploy it with some DNS magic or something, depending on the device.
[244.08 → 249.62] But they could really make this a whole inclusive package at some point.
[250.14 → 250.66] Absolutely, they could.
[250.76 → 260.44] Because with this acquisition, Nabu NASA now owns the copyright to Otto's Code and therefore the ESP Home organization on GitHub and Docker as well.
[260.74 → 263.68] Yeah, and ESPHome.io is a great resource.
[263.84 → 266.64] So if you want to learn a little bit more, go check out ESPHome.io.
[266.74 → 268.82] And of course, we'll have a link in the notes.
[269.36 → 271.80] Which, as always, you can find at self-hosted.show.
[271.80 → 275.74] Linode.com slash SSH.
[275.86 → 281.16] Linode.com slash SSH gives you a $100 60-day credit towards a new account at Linde.
[281.36 → 283.18] And of course, it supports the show.
[284.04 → 285.78] Linde is our cloud hosting provider.
[285.98 → 289.42] Anything we want to try out or anything we put in production, we put it up on Linde.
[289.58 → 290.84] We get emails into the show.
[290.92 → 292.40] We try stuff out on Linde.
[292.54 → 294.18] It's really quick to get going.
[294.30 → 296.20] But also, it's because it's fast.
[296.38 → 298.74] We know it's just going to get done really quick.
[298.74 → 302.20] And sometimes you just want to prototype something as fast as possible.
[302.42 → 307.16] Now, we host all of our major infrastructure for Jupyter Broadcasting 3.0 on Linde, of course.
[307.82 → 312.52] But even the stuff that never makes it public, that never is listener-facing, we run on Linde as well.
[312.58 → 313.32] They're superfast.
[313.40 → 324.42] They have native SSD storage, 40 gigabit network, totally easy to use cloud manager, really simple to take snapshots and get an idea of the last time your computer, or I should say Linde, was backed up.
[324.42 → 331.20] You can really simplify your infrastructure while also reaping the benefits of great performance at a great price.
[331.66 → 336.14] Linde costs 30% to 50% less than AWS or Google Cloud or Azure.
[336.66 → 341.22] And it really works well if you want to just blend a little bit of on-premises and cloud as well.
[341.34 → 342.56] That's how I use it for Nextcloud.
[342.92 → 345.72] I have a cloud component to my Nextcloud setup on Linde.
[346.08 → 351.14] And then the big bulk of the storage, like the archival stuff, it's all here locally on my LAN.
[351.26 → 352.58] It works fantastic that way.
[352.58 → 356.46] And with 11 data centres worldwide, you're going to find just the right spot to deploy.
[356.68 → 364.78] And you'll rest easy knowing that Linde's rocking fast and has great monitoring tools that can alert you to problems before you even notice them.
[365.04 → 369.02] Of course, these things are really important, but performance matters as well.
[369.10 → 370.58] And Linde has you covered there too.
[371.02 → 376.40] Cloud Spectator recently did a study of the different cloud providers, like all of them.
[377.02 → 379.46] Did, Amazon, Google.
[379.46 → 383.78] Google looked at Azure, all of them, put them in there, and saw who was the fastest.
[384.28 → 392.50] And one of the things that really makes Linde stand out is their dedicated CPU rigs have AMD EPIC processors that are just cranking faster than the other providers.
[392.50 → 398.56] And Linde's disk storage is superfast, so you can feed those processors faster than the other providers.
[398.56 → 411.02] And what Cloud Spectator survey shows is that not only does Linde have the best CPU and disk performance, but it has the best continuous performance as well, which really matters when you have large jobs that need processing, or you're getting a lot of traffic.
[411.18 → 412.56] You need that sustained performance.
[413.46 → 417.16] I mean, Linde started in 2003 as one of the first companies in cloud computing.
[417.16 → 419.08] So they really know what they're doing.
[419.28 → 424.76] They're independently owned and founded on a love for Linux open source technologies and the community that surrounds them.
[425.06 → 426.94] So just go try what I'm talking about.
[427.12 → 428.86] I've told you about the object storage before.
[428.98 → 430.66] I've told you about the cloud firewall before.
[430.74 → 432.34] There's a lot to check out with Linde.
[432.48 → 435.20] And what they've chosen to do, they do really well.
[435.50 → 436.72] So go spend that $100.
[437.44 → 439.32] Linode.com slash SSH.
[439.46 → 442.04] Go see what I've been talking about and support the show.
[442.38 → 444.38] Linode.com slash SSH.
[444.38 → 452.00] Well, I'm delighted to welcome to the show somebody whose work I've been following for many years as an Ansible user.
[452.26 → 454.12] We have Jeff Deerling on the show today.
[454.22 → 454.72] Welcome, Jeff.
[455.18 → 456.24] Thanks for having me.
[456.60 → 457.50] Thank you for being here.
[457.86 → 462.18] And more recently, of course, a YouTube extraordinaire content creator.
[462.62 → 464.04] Yeah, that's how I came to know you.
[464.38 → 464.66] Yeah.
[465.14 → 468.32] So you've been doing a lot of videos lately on the Raspberry Pi 4 compute module.
[468.42 → 469.90] I thought we'd talk to you a little bit about that.
[469.90 → 478.42] But before we get to that side of the discussion, I wanted to sort of talk to you a little bit about what I knew you for first, which was Ansible.
[478.64 → 483.54] So you have a really rather excellent 101 getting started course.
[483.54 → 494.10] Before Jeff Deerling existed and created this, you know, de facto guide for people getting started with Ansible, how did you get involved with the project?
[494.10 → 500.10] I started off by having a few servers, then many servers, and then dozens of servers.
[500.36 → 506.32] And once I went from many to dozens, I realized I had to switch to some sort of configuration management system.
[507.12 → 509.66] And at the time, Ansible was pretty much brand new.
[510.14 → 516.76] That was 2012, 2013, when I was making that transition from shell scripts and run books to something more formal.
[516.76 → 519.62] So I tried out Chef, but I'm not a Ruby developer.
[520.32 → 522.18] And I didn't really like it.
[522.38 → 529.74] It felt too much like programming to me and learning Ruby when, you know, I did PHP and Node.js and things like that.
[530.14 → 533.20] So I got into Ansible at that time.
[533.52 → 538.34] And at the time, it was so simple that you could pick everything up in a day.
[538.36 → 542.48] And it was focused really on just Linux administration, not all the other things that it does today.
[542.48 → 547.82] Um, but the documentation was great, but there wasn't a ton of examples out there.
[547.98 → 551.36] So I just started blogging about my experiences.
[551.36 → 554.00] And then I realized that there wasn't a book for it.
[554.10 → 561.80] So I put my blog post together into like a 50 page sampler thing and stuck it onto Lean Pub,
[561.90 → 566.20] which was also pretty new at the time, and started self-publishing this little e-book.
[566.20 → 572.78] And my goal was to maybe sell 100 copies or 200 copies and, you know, help some people learn Ansible.
[573.10 → 577.96] And lo and behold, a couple of years later, since it was one of the first books on Ansible,
[578.08 → 580.28] it became one of the most purchased books.
[580.50 → 584.20] And to this point, I don't remember how many tens of thousands of books I've sold,
[584.34 → 587.46] but lots of thousands of books have been sold.
[588.10 → 594.90] It was the number one bestseller for infrastructure automation for a number of periods on Amazon.
[594.90 → 600.82] And has been in the top five, top 10 books on Lean Pub for years now, too.
[601.18 → 601.54] Congratulations.
[602.30 → 602.86] Yeah, thanks.
[603.06 → 603.88] I don't doubt it.
[604.10 → 609.62] You know, every time you search for anything related to a specific role or something like
[609.62 → 613.86] that for Ansible, you're looking, there's a Jeff Deerling role in there in Ansible Galaxy.
[614.28 → 618.54] So some of our listeners will be familiar with Ansible, but some won't.
[618.64 → 622.12] So what's your quick kind of elevator pitch of what Ansible is and does?
[622.12 → 627.36] There's an XKCD about whether you should automate something.
[628.06 → 631.14] And I think that that's a good illustration of what Ansible is.
[631.26 → 635.68] Once you reach the point where you're doing something, maybe to a group of computers or
[635.68 → 640.34] to network switches or to servers, or even I use it to manage my own computer.
[640.46 → 645.40] If you're doing a repetitive task that can be automated, Ansible can automate that.
[645.60 → 647.94] Almost anything in the world that has to do with technology.
[647.94 → 650.82] So that's what it does.
[650.94 → 652.02] And it's very simple.
[652.22 → 657.54] That's the big selling point for it compared to other tools is it uses YAML configuration,
[657.92 → 660.66] which is very approachable, very easy to learn.
[661.10 → 666.74] And that's why I liked it over the other solutions at the time, Chef and Puppet that I was looking at.
[666.74 → 674.54] People back in 2012, 13 time were just moaning about how YAML was so complicated with its white space.
[674.60 → 681.24] And I never quite understood the hate, to be honest with you, because JSON, people say,
[681.42 → 682.66] oh, I'd much rather write JSON.
[682.82 → 683.80] I'm like, are you mad?
[685.12 → 686.52] YAML is way easier to work with.
[686.52 → 695.92] Yeah, I think a lot of people maybe don't, they aren't used to having like a code editor do formatting for them and things like that.
[696.00 → 701.66] It's much more common nowadays, especially in the infrastructure space than it was 10 years ago.
[701.90 → 703.44] And I think that's the biggest difference.
[703.58 → 709.52] Nowadays, YAML, people complain about it mostly because they see people do things that you shouldn't do in YAML.
[709.52 → 712.98] But back then it was more the syntax and the formatting.
[713.16 → 717.56] They're like, I could put in anything in JSON or God forbid, XML.
[718.56 → 720.52] But, you know, YAML is going to complain about it.
[720.64 → 725.38] And I think nowadays we're past the formatting stage, and we're into the, you know,
[725.46 → 730.64] what could be a next generation format for configuration that's even better than YAML because it does have shortcomings.
[730.82 → 739.30] But it's, in my opinion, it's a thousand times better than JSON, XML and SOAP and all the other protocols we used to have to know to be able to configure things.
[739.52 → 740.44] Couldn't agree more.
[740.76 → 740.94] Yeah.
[741.24 → 747.90] So I think, you know, speaking of things that people shouldn't do, turning Ansible into a programming language is probably up there, right?
[748.02 → 750.36] I mean, you can do some pretty crazy stuff in Ansible.
[750.72 → 753.92] And my day job is related to OpenShift at Red Hat.
[754.10 → 759.02] And a lot of the OpenShift installer stuff for version three, the last major version,
[759.72 → 764.76] there was some pretty crazy hacky stuff going on in those Ansible playbooks and stuff like that.
[764.92 → 767.98] But what's the most crazy thing that you've seen with Ansible?
[767.98 → 772.76] I think it's the abuse of when condition in tasks.
[773.44 → 778.16] When your when condition is longer than the rest of your Ansible task for a given piece of automation,
[778.52 → 779.84] I think that's where you've failed.
[780.46 → 784.38] At that point, in Ansible, you can write modules in Python.
[784.58 → 789.76] You can actually, there are ways to write modules in other languages too, but typically you'd write it in Python.
[790.30 → 794.74] And if you're going to use complex logic to determine whether to do something or how to do something,
[794.74 → 796.58] that should be in Python.
[796.88 → 802.90] At that point, you're getting into advanced Ansible usage that requires you to have some of that programming knowledge.
[803.48 → 806.30] Programming in YAML is a terrible, terrible idea.
[806.54 → 807.22] Never do it.
[807.62 → 812.18] Every time I have gone further than an if-then or an if-else type condition,
[812.36 → 813.46] I've regretted it.
[813.52 → 814.62] And the maintenance is a nightmare.
[814.62 → 820.28] And then there's always the ginger 2 stuff that people do, the crazy emulating, for loops, all that kind of stuff.
[820.60 → 821.12] So yeah.
[821.52 → 823.30] Anyway, should we talk about Ansible 3 for a minute?
[823.54 → 826.96] There's been a big release in the last few weeks of Ansible 3.0,
[827.04 → 830.58] which brings a lot of changes to the way in which modules are delivered to users.
[830.86 → 832.52] What do you make of all that change?
[832.52 → 834.80] It's been an interesting transition.
[835.18 → 840.78] And I think it's ongoing and will be ongoing for another period of time, six months to a year, probably.
[841.36 → 847.72] Mostly because Ansible 2.9, which is the previous major version of what you would get when you installed Ansible
[847.72 → 850.52] using PIP or a package manager or something like that.
[851.06 → 853.62] Ansible 2.9 will still be supported for a while.
[853.62 → 859.58] Ansible, mostly because I think there's just a lot of people who the transition to the new version of Ansible
[859.58 → 863.50] does introduce some changes that could impact people's workflows a little bit.
[864.04 → 867.94] The good thing about the transition is that all my existing playbooks,
[868.00 → 870.54] and I have a ton of playbooks that do a ton of different things,
[871.04 → 876.54] they all work fine if I just upgrade Ansible using PIP, which is the Python package manager.
[876.94 → 881.82] There are other ways to install Ansible that might not work with Ansible 3 the same way anymore.
[881.82 → 883.28] So you have to watch out for that.
[883.46 → 886.96] And that's why I always recommend using PIP to install it.
[887.16 → 889.92] It's a Python program and PIP is the preferred way.
[890.66 → 898.72] But the big, big change is that collections of modules used to all be maintained in one giant code base.
[899.26 → 902.06] And there were various reasons that was not very sustainable.
[902.76 → 906.58] There were something like 4,000 or 5,000 different plugins and modules.
[906.84 → 910.28] And the core team of developers who managed the releases and things,
[910.28 → 911.66] it was just a lot to coordinate.
[912.28 → 917.30] So the main goal was to move all of that content out into smaller collections
[917.30 → 921.34] that could be maintained by people with more knowledge of just the modules in that collection.
[921.50 → 927.90] Like, there's no reason why a let's say, an F5 network load balancing module
[927.90 → 935.86] should be under the same maintenance umbrella as a, I don't know, like an email script thing.
[935.86 → 941.66] All these different modules were lumped together from network vendors and storage vendors and cloud vendors and Linux and Windows.
[941.96 → 943.56] So now it's all broken out.
[944.18 → 950.88] But the challenge has been making it all come together back into what we install if we do a PIP install Ansible.
[950.88 → 957.16] And the nice thing is it all works, but the downside is there are a few little bumps,
[957.26 → 959.36] especially if you have specialized use cases.
[959.62 → 966.94] But another cool side effect is you could install Ansible without all that stuff and just add in the few things you need.
[967.04 → 971.26] So if you just do Linux administration, you can install Ansible plus the Linux modules
[971.26 → 975.16] and not install Windows, not install networking, not install cloud.
[975.16 → 981.00] So it does offer some flexibility, but I think there's going to be some growing pains over the next year.
[981.40 → 983.50] We've seen that trend quite a lot in technology at the moment.
[983.84 → 987.98] You know, Docker being an example with Rodman coming along to kind of break that out into,
[988.22 → 992.18] you know, being less of a monolith type deployment model.
[992.64 → 994.12] So I think it's a good thing personally.
[994.50 → 998.14] And, you know, the work that's gone in has clearly been very well-thought-out.
[998.14 → 1005.48] Are there any particularly good resources that you'd recommend people visit to get their head around what the major changes are?
[1005.92 → 1010.08] The documentation is the best place to know what's going on.
[1010.16 → 1014.32] There's not only is there a guide for upgrading Ansible in the release notes.
[1015.18 → 1022.06] And if you are involved in using Ansible, I would highly recommend subscribing to the Ansible project mailing list on Google Groups.
[1022.28 → 1025.94] But the guides and the documentation are by far the best.
[1025.94 → 1032.10] They encapsulate everything that I could ever think of that people could be that could affect someone's workflow.
[1032.96 → 1035.84] And also, I did update my book recently.
[1035.84 → 1042.64] So if you are interested in learning Ansible and you don't know it yet, Ansible for DevOps has a major second revision.
[1042.84 → 1045.22] I've actually revised it 25 times now.
[1045.72 → 1051.00] But a major revision happened to incorporate some of the information about collections, especially.
[1051.00 → 1056.96] And I'm still working on fully revising the book to be up-to-date with Ansible 3.
[1057.60 → 1058.30] It all works.
[1058.38 → 1060.90] It's just there are some things that could be optimized a little more.
[1060.90 → 1065.12] Datadog.com slash self-hosted.
[1065.28 → 1072.00] Analyze code level performance across your entire environment and troubleshoot issues faster with Datadog.
[1072.38 → 1078.60] Datadog has a continuous profiler that automatically collects profiles from your production servers all the time.
[1078.68 → 1083.50] So you can then analyze your data quickly with minimal overhead when you need.
[1083.50 → 1088.68] Get a snapshot in time and troubleshoot and then visualize it with their beautiful dashboards.
[1088.68 → 1096.58] Get a unified picture of your environment by correlating code performance metrics with your other monitoring data with real-time dashboards.
[1096.66 → 1097.86] You've got to see these dashboards.
[1097.98 → 1103.34] Go to datadog.com slash self-hosted to get a free trial and to see these beautiful dashboards.
[1103.56 → 1106.18] And you'll get a free t-shirt when you sign up a trial and create a dashboard.
[1106.18 → 1117.46] With tightly integrated APM, tracing, log management, and continuous profiler products in one single platform, Datadog enables you to pinpoint the root cause of issues faster than ever.
[1117.46 → 1124.14] Are you seeing the value here when you can visualize everything at once down to the application level, server stuff, even website performance?
[1124.26 → 1125.90] It's all in Datadog.
[1126.02 → 1127.90] And you can get smart alerts as well.
[1128.38 → 1135.48] Try Datadog's products for free for 14 days by visiting datadog.com slash self-hosted for a limited time.
[1135.56 → 1139.66] If you start a free trial and create one dashboard, you'll get a free Datadog t-shirt.
[1139.88 → 1141.18] And who doesn't love free swag?
[1141.44 → 1144.78] So that's datadog.com slash self-hosted.
[1144.78 → 1148.84] So Jeff, I've been watching on your YouTube channel.
[1148.96 → 1152.36] You've been doing the impossible with Raspberry Pis.
[1152.46 → 1156.88] I'm talking like, I think one of your setups was like 10 SATA disks.
[1157.36 → 1158.74] 16 hard drives.
[1159.08 → 1160.02] How is this possible?
[1160.14 → 1161.72] How is this madness accomplished?
[1161.88 → 1165.76] Is it all with using the new Pi compute module?
[1165.76 → 1166.24] Yes.
[1166.68 → 1174.34] And the funny thing is the Raspberry Pi 4, the one that's been out since I think 2019, that was the Pi Day release back then.
[1174.82 → 1178.46] The Raspberry Pi 4 actually has the same processor and capabilities.
[1178.78 → 1185.18] But the big difference the compute module has is it exposes the internal PCI Express lane.
[1185.40 → 1185.64] Yeah.
[1185.64 → 1187.14] And that's the big game changer.
[1187.26 → 1189.58] With the Pi 4, you could hack it.
[1189.64 → 1194.72] You could resolder a chip on it, the VL805 chip that controls USB 3.
[1194.78 → 1199.42] You could resolder that, wire up some jumpers, and get PCI through it.
[1199.50 → 1200.86] And a couple of people actually did that.
[1200.92 → 1204.28] That was the first time that I started working with the compute module.
[1204.28 → 1211.96] I was looking at their work because PCI Express support is rudimentary right now on Raspberry Pi OS.
[1212.38 → 1216.42] And they were kind of like the groundbreaking people that got that going.
[1217.06 → 1224.30] But the compute module 4 includes a standard PCI Express slot on the I.O. board that you can buy with it.
[1224.84 → 1230.64] And the cool thing is that a lot of people are building boards around it that have different PCI form factors.
[1230.64 → 1244.74] So M.2 slots for things like LTE modems or for storage with NVMe drives or SATA drives that are either in M.2 form factor or using a SATA controller.
[1244.88 → 1247.34] And you can plug in hard drives and things like that.
[1248.00 → 1250.06] So a really cool thing happened.
[1250.20 → 1254.38] Somebody from Broadcom actually contacted me after they saw some of the work I was doing and said,
[1254.48 → 1258.88] Hey, we want to see if we can get a hardware RAID controller, an enterprise storage controller.
[1258.88 → 1260.88] These things cost like a thousand bucks.
[1261.54 → 1263.42] We want to see if we can get that working on a Pi.
[1263.66 → 1264.98] And we can't get a Pi.
[1265.24 → 1273.82] Like they work at Broadcom, but they had trouble sourcing a Raspberry Pi because the compute module 4 has been in such high demand since the launch.
[1274.54 → 1275.78] So they shipped me the card.
[1275.90 → 1280.34] They shipped me a storage controller and had me work with a couple of storage engineers.
[1280.48 → 1282.22] And we got it working.
[1282.22 → 1285.18] So at that point, I had eight drives on the Pi.
[1285.28 → 1289.02] But then I found that I could also plug in eight more drives with the card I had.
[1289.18 → 1294.96] So I did a live stream and got all 16 hard drives plugged into the Pi and in one giant RAID array.
[1295.50 → 1295.72] Wow.
[1295.92 → 1296.60] How was performance?
[1297.10 → 1297.28] Yeah.
[1297.34 → 1297.80] How is it?
[1297.82 → 1298.08] Because, right?
[1298.16 → 1303.56] I mean, that's always the thing about the Pi is everybody says the Pi 4 is great, except for the IO really limits it now.
[1303.64 → 1305.36] But this seems like that changes that a little bit.
[1305.56 → 1306.72] It changes it a little bit.
[1306.78 → 1308.64] It doesn't fix all the problems.
[1308.64 → 1309.54] That's for sure.
[1309.92 → 1314.26] The big problem is that it's X1, a Pi 1 lane.
[1314.46 → 1314.64] Yeah.
[1314.88 → 1318.22] So it's PCI Express Gen 2 by 1.
[1318.68 → 1323.44] And the maximum throughput you can get with that is 5 gigabits per second.
[1324.16 → 1325.82] But that's theoretical.
[1326.04 → 1330.40] So the maximum real-world throughput that I've gotten, I've tested 10 gig Ethernet.
[1330.48 → 1331.76] I've tested the storage controller.
[1331.88 → 1334.34] I've tested all kinds of different crazy things so far.
[1334.34 → 1341.52] And the maximum real-world throughput is about 3.2 gigabits, a little over 400 megabytes per second.
[1342.06 → 1345.22] So I threw this hardware RAID storage controller on it.
[1345.30 → 1348.02] It could do like 10 gigabytes per second.
[1348.30 → 1350.94] But I can only put through 400 megabytes per second.
[1350.94 → 1358.84] So it's not going to give you magically access to all the wonderful things you could throw into like a modern Thread ripper PC.
[1358.84 → 1367.60] But it does give us a lot more options than with the Pi 4 where you just have USB 3.0, which has its own limitations.
[1368.22 → 1373.30] I mean, the fact that you could have redundant storage is an upgrade beyond the fact that it's slightly faster too.
[1373.76 → 1380.46] But do you think this kind of is maybe an indication of where the Pi is going to go?
[1380.58 → 1384.22] Is this compute module a hint of what we might see maybe in the Pi 5?
[1384.22 → 1385.20] I hope so.
[1385.58 → 1389.58] Another thing to keep in mind is there are a lot of Pi competitors.
[1389.94 → 1393.32] And it's, you know, which one is going to be the Pi killer?
[1393.48 → 1404.68] Nothing's going to kill the Raspberry Pi just because the Raspberry Pi has a community and a force behind it that is unparalleled in all the other kind of maker space single board computing realm.
[1405.12 → 1411.98] And don't you think that's kind of the advantage of using the compute module in another board versus getting an SBC that just has all this stuff?
[1411.98 → 1416.90] It's like you're getting the Raspberry Pi ecosystem with some of these cool new toys.
[1417.24 → 1417.68] Yeah, yeah.
[1417.84 → 1423.22] On the flip side, though, there are some boards like the what is it, the Rock chip RX?
[1423.58 → 1425.22] I forget what the specific chip is.
[1425.38 → 1425.98] Rock chip Pro.
[1426.18 → 1428.54] Yeah, it has a Pi 4 lane.
[1428.68 → 1434.38] So you get more bandwidth and more lanes so that you can do more with it and have more I.O. speed.
[1434.38 → 1439.34] There's still limitations just based on the fact that the CPU is not superfast.
[1439.50 → 1451.04] And even if you give it, you know, let's say we get 10 gigabits or 20 gigabits of throughput, the CPU is going to be limited in other ways on these cheaper ARM SBCs like the Raspberry Pi.
[1451.42 → 1461.48] For instance, today I'm doing some testing for a 2.5 gigabit NAS that I'm building with a Pi to see if it can compete with an out of the box NAS from QNAP or Synology or something like that.
[1461.48 → 1473.46] And without overclocking the CPU, I can only pump through 1.7 gigabits of network traffic because the way the CPU is architected, all packets go on one core on the CPU.
[1473.62 → 1475.80] It's a four core CPU, so it could support more.
[1476.18 → 1481.40] But the way the network throughput works on the Pi, it's stuck on one core and it maxes out.
[1481.52 → 1483.50] So you have to overclock it to get more speed.
[1483.70 → 1487.50] I think, you know, there are two things I really want to see in the next Pi.
[1487.64 → 1489.76] One is maybe more PCI bandwidth.
[1489.76 → 1492.54] The other is just a faster CPU.
[1492.82 → 1494.04] And we've seen what's possible.
[1494.22 → 1505.08] Apple with their M series, even the A series, just blows away the competition in terms of performance per watt and, you know, single threaded performance for any kind of mobile device.
[1505.70 → 1510.34] So I think that the ARM SBCs have a bright future.
[1510.34 → 1517.46] And that's, I'm hoping that IO speed and CPU speed, which is becoming the bottleneck for a lot of my projects.
[1517.90 → 1520.34] Those are the two things I really hope to see improved.
[1520.76 → 1522.82] I wonder where you come up with some of these ideas, man.
[1522.94 → 1524.32] Now your head must be an interesting place.
[1524.32 → 1529.62] If you want to come over to my house sometime, I will show you the pile.
[1529.78 → 1532.82] I have so many projects that I really, really want to work on.
[1533.40 → 1536.30] And I don't think I'll get to them in the next few months, unfortunately.
[1536.60 → 1537.16] Are you near me?
[1537.24 → 1537.90] Are you in Raleigh?
[1537.98 → 1539.88] No, I'm in St. Louis, Missouri.
[1540.10 → 1543.16] But, you know, fly over here after the coronavirus is over.
[1543.56 → 1545.16] Oh, maybe one day we'll do another road trip.
[1545.24 → 1545.56] Hey, Chris?
[1545.90 → 1546.52] Yeah, for sure.
[1546.60 → 1547.74] I don't think that's a maybe.
[1547.88 → 1549.02] Nothing about that's a maybe.
[1549.02 → 1553.84] So if we were to come visit, what kind of stuff would we see you self-hosting in your place?
[1554.24 → 1558.68] Right now, the major thing that I'm hosting is pydramble.com.
[1558.80 → 1560.74] This has been a project since 2014.
[1560.94 → 1561.88] I started doing it.
[1562.10 → 1568.54] It was to see if I could host a Drupal site specifically, because I'm involved in the Drupal open source community.
[1569.10 → 1578.10] If I could host Drupal in my house long term, and that site has had 99.997 or 8 uptimes since 2014.
[1578.10 → 1579.64] Running on Raspberry Pis.
[1579.74 → 1581.20] Now, I cheated in 2016.
[1581.20 → 1585.46] I switched to use Cloudflare as a front end, but the cache is only 30 minutes.
[1586.02 → 1589.14] So if I do have a major outage, it will go down after 30 minutes.
[1589.42 → 1590.66] So I don't think that's cheating.
[1590.74 → 1591.64] That's just good engineering.
[1592.42 → 1597.98] Yeah, well, I was getting tired of, you know, if my ISP goes down for two minutes, I would get a notification.
[1598.32 → 1602.08] I was going to say, like, how have you managed to have ISP uptime that high at home?
[1602.22 → 1603.46] That was the most impressive part.
[1603.58 → 1605.96] Well, I've switched to in St. Louis.
[1605.96 → 1607.80] Of course, we have spectrum, but...
[1607.80 → 1608.48] Yeah, me too.
[1608.66 → 1609.20] It sucks.
[1609.40 → 1614.06] Yeah, it's difficult because the ISPs, they have a monopoly, basically.
[1614.30 → 1619.58] And another fun thing that I'm going to be trying, I actually just got last week a Starlink.
[1619.84 → 1620.28] Awesome.
[1620.28 → 1622.58] And I'm going to be testing it out.
[1623.74 → 1631.98] My ultimate goal is to have, either through the router, I have an ASUS router, either through that or maybe through a Raspberry Pi.
[1632.64 → 1636.00] I'm also testing a router build using a Raspberry Pi compute module.
[1636.26 → 1636.54] Of course.
[1636.54 → 1642.84] Having a redundant link that will automatically fail over and possibly do link aggregation.
[1643.00 → 1644.92] But for now, I just care about the redundancy.
[1645.38 → 1647.22] Just because I do work from home.
[1647.50 → 1648.06] I do streaming.
[1648.28 → 1649.60] I do video uploads.
[1649.60 → 1652.14] And I just, I need a lot of bandwidth and I need reliability.
[1652.14 → 1656.14] And I do want to host more besides just the Pi Bramble site.
[1656.36 → 1658.72] I want to host my personal site here at some point.
[1658.80 → 1666.52] I want to host some other things that are more high impact and, you know, could survive an outage of one of the two network links, which Starlink could give me.
[1666.78 → 1671.38] I don't think we've seen many people discussing hosting services on Starlink, either.
[1671.68 → 1674.24] I'd be curious to see what they allow, what can get through.
[1674.90 → 1675.60] Have you heard much?
[1676.10 → 1677.38] It's a mixed story there.
[1677.48 → 1680.10] So they don't give you a consistent IP address.
[1680.22 → 1684.36] And they also don't, they don't pass through traffic in a way that you can host directly from home.
[1684.44 → 1685.98] So I'd have to use some sort of proxy.
[1686.52 → 1694.76] And I, you know, I can have a one of the VPSs I have at DigitalOcean or something like that pass through the traffic for me.
[1695.12 → 1695.22] Sure.
[1695.42 → 1700.46] So give us an idea of what other, so I heard you have a sounded like you're running Drupal on a Raspberry Pi server.
[1700.74 → 1702.92] Any x86 boxes in that mix we'd see?
[1702.92 → 1711.94] I do have one x86 server that mostly what it's doing is allowing me to RDP into it and do Windows things when I need to.
[1712.12 → 1714.10] It's running Windows 10 Pro.
[1714.34 → 1719.48] And I use it for a lot of network testing because it has a Eleanor card inside of it.
[1719.50 → 1721.66] So I can get 10 gig network tests done on it.
[1722.20 → 1724.80] Especially if it's a long test that's going to take a few hours.
[1724.94 → 1727.44] I don't want to do it on my main workstation, which is a laptop.
[1727.88 → 1730.04] Because then it's stuck wherever I have it running.
[1730.42 → 1731.20] Yeah, I know that.
[1731.20 → 1733.38] Like, why did I start that job on the laptop?
[1733.60 → 1734.04] Dang it.
[1734.56 → 1734.92] Exactly.
[1736.08 → 1739.08] And then you have to come back downstairs later and find it.
[1739.64 → 1746.02] And then the other things that I do, I have a couple PI's that run around the clock doing just little tasks around the house.
[1746.02 → 1754.94] Checking on things, keeping track of temperature and like my sump pump, checking the level of the pit and just logging that data.
[1754.94 → 1762.80] The other thing that I have running right now, and this is part of the motivation for all this Pi experimentation, does I have a 2011 Mac Mini.
[1763.32 → 1764.06] Ancient.
[1764.78 → 1766.54] The OS is not even supported on it.
[1766.56 → 1767.52] I can't upgrade it anymore.
[1767.98 → 1771.84] It's still my primary network storage device, which is terrible.
[1771.84 → 1777.68] Like, I've set up all these different NASA's and things, and I still am using this Mac Mini, which has USB 2.
[1778.00 → 1784.74] So my external 12 terabyte single hard drive, not a RAID, my single hard drive is running at USB 2 speed.
[1784.86 → 1789.78] So I'm doing file copies with, you know, 20 gigs, 40 gigs at 30 megabytes per second.
[1789.78 → 1792.16] So this would be a bad time to ask you how many terabytes.
[1792.32 → 1796.92] One of the questions we tend to ask all of our guests is how many terabytes do you have on your LAN?
[1796.96 → 1800.18] And we had Wendell on a few months ago, and I think he had a petabyte.
[1800.62 → 1803.48] So maybe you won't quite match that.
[1803.54 → 1804.52] But how many do you have, Jeff?
[1804.72 → 1805.44] No, no.
[1806.18 → 1808.94] Online right now, I have about 24 terabytes.
[1809.36 → 1813.26] But in the house, I have about 60 or so.
[1814.08 → 1821.02] There are a lot of terabytes of hard drives that are sitting on my desk over there that are being tested and not in use.
[1821.12 → 1825.76] Because when you're testing, you don't want to have production data on a hard drive you're running benchmarks against.
[1826.12 → 1828.02] Ready to go in that NAS you were talking about.
[1828.58 → 1829.40] Yes, yeah.
[1829.40 → 1841.78] And the other thing that I mentioned on, I don't remember if it was a video or a live stream, but my goal is at some point in the next year, if I can get a storage vendor to work with me, I would love to build a petabyte Pi.
[1841.78 → 1845.32] Have one Raspberry Pi controlling a petabyte of storage.
[1845.48 → 1847.08] I think that would be something fun.
[1847.16 → 1848.96] It'd be 400 megabytes per second.
[1849.50 → 1852.22] It'd be such a waste, but it'd be so cool to see that.
[1852.60 → 1854.72] Petabyte Pi project rolls off the tongue, too.
[1854.78 → 1855.14] I like it.
[1855.22 → 1855.92] It's bop, bop, bop.
[1856.20 → 1856.60] Exactly.
[1856.96 → 1859.60] Is a petabyte 1,000 or 100 terabytes?
[1859.70 → 1860.36] I can never remember.
[1860.52 → 1860.92] 1,000.
[1861.32 → 1862.02] Oh, my goodness.
[1862.18 → 1863.06] How would you even do that?
[1863.76 → 1864.16] Wow.
[1864.54 → 1864.68] Yeah.
[1864.86 → 1866.62] You've got to get at least 100 hard drives.
[1866.62 → 1870.48] So it would not be super fun to do the project.
[1870.68 → 1871.76] I mean, it'd be super fun.
[1871.96 → 1881.76] But the hardware, I would probably have to build a rack or something and figure out a place, maybe in my wood workshop or something, to try to fit that.
[1881.98 → 1885.36] If you've got a 3D printer, you could probably rustle something up with one of those.
[1885.54 → 1886.18] There you go.
[1886.46 → 1887.36] How did I know?
[1887.44 → 1888.20] How did I know?
[1888.28 → 1889.68] That would be your suggestion, Alex.
[1889.68 → 1894.36] Well, see, this is why I'm going to say subscribe to your channel, Jeff, because there are just some great videos over there.
[1894.52 → 1896.86] And maybe one day I'll see that project on there.
[1897.18 → 1897.74] I hope so.
[1897.90 → 1898.52] That would be fun.
[1898.76 → 1904.20] Well, Jeff, before we get out of here, I was wondering if there's any way you'd like to send people your channel or Twitter or something like that.
[1904.62 → 1908.10] Everything is linked from my personal website, jeffgearling.com.
[1908.62 → 1913.40] I started my personal site back in 2001 or 2002 or something like that.
[1913.88 → 1916.98] And I like to have my data in my site.
[1916.98 → 1919.54] So I typically post things preferentially there.
[1920.46 → 1924.22] And, you know, I can't do video hosting and things like that.
[1924.36 → 1931.56] I could, and I actually did at one point, but I realized that YouTube does it way better than I ever could with streaming and all that kind of stuff.
[1931.66 → 1933.92] So I like to take ownership of that.
[1934.08 → 1936.96] So jeffgearling.com is where I throw everything primarily.
[1937.16 → 1939.58] And then you can go to the other sites from there.
[1940.02 → 1941.28] We'll have a link in our show notes, too.
[1941.38 → 1942.26] Thanks for joining us, Jeff.
[1942.56 → 1944.00] Yeah, thanks so much for having me.
[1944.00 → 1947.28] And a big thank you from me because you saved my bacon.
[1947.84 → 1951.20] I can't count the number of times with the roles on Ansible Galaxy.
[1951.46 → 1952.68] So huge, huge past Alex.
[1952.84 → 1953.78] Thanks, current Jeff.
[1956.82 → 1959.42] Well, now I'm even more excited about the Raspberry Pi.
[1959.56 → 1960.58] Thanks to Jeff for coming on.
[1960.62 → 1964.74] And of course, like we said, we have links to his channel and everything in the show notes.
[1964.94 → 1968.40] And I want to mention you can find our sponsor, Cloud Guru, on social media.
[1968.40 → 1973.76] It's just slashed a Cloud Guru at YouTube, Twitter, Facebook, like all the social media platforms.
[1973.84 → 1974.68] Just slash a Cloud Guru.
[1974.80 → 1975.88] It's super, super easy.
[1976.34 → 1980.24] And a big thank you to our members over at self-hosted. Show slash SRE.
[1980.46 → 1982.54] Our site reliability engineers support the show.
[1982.86 → 1987.54] You guys get a limited ad feed and a little bit of extra post show every week.
[1987.88 → 1988.10] Oh, yeah.
[1988.10 → 1989.74] I haven't told you what I want to talk about yet.
[1989.80 → 1991.28] That's coming up for the members.
[1991.46 → 1991.94] No, no.
[1992.00 → 1993.32] It's going to be a surprise to me, too.
[1994.04 → 1996.20] And you can go to self-hosted. Show slash contact.
[1996.42 → 1998.06] That's the place to go to get in touch with us.
[1998.06 → 1999.78] I'm on Twitter at ironic badger.
[2000.18 → 2001.84] Yeah, I'm there, too, at Chris LAS.
[2002.06 → 2004.66] And the show is at selfhostedshow.
[2004.80 → 2006.78] And don't forget the network at Jupyter Signal.
[2007.26 → 2008.20] Thanks for listening, everyone.
[2008.40 → 2010.66] That was self-hosted. Show slash 41.
