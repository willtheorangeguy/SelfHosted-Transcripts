[0.00 --> 5.84]  Coming up on Self-Hosted 26, we have Mike and Wes joining us to discuss the new Docker news.
[6.30 --> 9.14]  We talk about freeing your robot vacuum from the cloud.
[9.94 --> 13.24]  And Alex really goes for the hard sell on Terraform.
[13.78 --> 14.22]  I'm Chris.
[14.58 --> 15.12]  And I'm Alex.
[15.28 --> 16.70]  And this is Self-Hosted 26.
[18.02 --> 21.38]  This episode is brought to you by a cloud guru.
[21.74 --> 26.14]  Are you looking to get a high-paying career, maybe move into the cloud and make some good change?
[26.26 --> 29.40]  Well, there's no better place to start than getting a certification.
[30.02 --> 33.04]  ACG has helped more than 2 million people scale up on the cloud.
[33.12 --> 35.80]  AWS, Azure, and Google Cloud Platform.
[36.74 --> 38.98]  Head over to cloudguru.com and get started.
[39.32 --> 43.18]  So being a Seattle guy, you know, you probably follow the ins and outs of Microsoft, don't you?
[43.54 --> 45.04]  The new flight simulator's out.
[45.14 --> 46.06]  Oh, is it actually released?
[46.16 --> 48.22]  That's why I'm seeing so many screenshots.
[48.22 --> 51.70]  I just wasn't sure if it was like extreme hype cycle mode or what.
[52.14 --> 56.54]  But I've been seeing people take screenshots of the real world and then compare it to flight simulator.
[57.02 --> 57.76]  The hype is real.
[57.76 --> 63.56]  They've used Azure and Bing Maps to kind of do machine learning and all this kind of stuff.
[63.62 --> 67.90]  And obviously the first thing anybody does in a flight simulator is go and try and find their house, right?
[68.40 --> 69.56]  And I'll tell you what.
[69.64 --> 78.66]  I was able to follow the roads from the local airport near my house, follow the actual roads, the highways, the small roads, everything, and find my house in a flight simulator.
[78.82 --> 80.76]  I could actually see it with my car on the driveway.
[80.94 --> 82.08]  It's amazing.
[82.08 --> 84.24]  Was it amazing or did it feel slightly creepy?
[84.64 --> 85.80]  No, 100% amazing.
[85.94 --> 91.24]  Because I remember, you know, Flight Sim 98, 2000, I think 2002 was another one.
[92.14 --> 97.16]  And I remember trying to do those things, you know, fly with visual references and stuff, looking out the window.
[97.42 --> 100.46]  And, you know, it was just generated low res garbage.
[100.60 --> 103.84]  Whereas now I can actually see and navigate with my eyes.
[103.94 --> 105.22]  It's amazing.
[105.22 --> 114.96]  Imagine how cool this could be fast forward into the future where cars are driving around with LiDAR sensors and they're mapping things in real time in a 3D universe.
[115.28 --> 119.48]  And then they somehow collect that information safely because you know they're going to.
[119.80 --> 122.14]  And then they could use that to inform game design.
[122.68 --> 124.42]  Now, my brain just exploded a bit.
[124.54 --> 126.52]  That is in 20 years.
[126.58 --> 130.86]  So if you look at the generational leap from Flight Sim 2000 to Flight Sim 2020.
[131.78 --> 133.24]  Flight Sim 2040?
[133.86 --> 134.48]  Oh boy.
[135.22 --> 141.34]  It's almost as cool as robot vacuums, which I'm wondering how is the robot vacuum life going for you?
[141.74 --> 142.44]  It's great.
[142.68 --> 148.76]  You know, there's just a base level of cleanliness that you get from having these machines, these robots going around.
[149.20 --> 154.52]  But what I wanted was the ability to dispatch the RoboVac to a specific part of my house.
[154.84 --> 157.06]  You know, clean up on aisle five type situation.
[157.06 --> 166.22]  And with Valetudo, I've been able to not only free my RoboVac from Xiaomi's cloud clutches.
[166.60 --> 172.44]  I've also been able to program in some pretty cool stuff like room based cleanups in Home Assistant.
[172.80 --> 174.20]  And it's pretty sweet.
[174.56 --> 174.80]  Wow.
[175.28 --> 177.92]  I got to see this when we're traveling again.
[177.92 --> 179.52]  I have got to see the setup.
[179.94 --> 181.26]  And then I've got to get you to do it at the studio.
[182.46 --> 184.00]  Well, lucky for you, Chris.
[184.08 --> 185.92]  I've written a blog post on the topic.
[186.38 --> 186.68]  Really?
[186.84 --> 188.04]  Well, how lucky is that?
[188.08 --> 189.82]  If only there was a place we could link that.
[190.16 --> 190.76]  Oh, I know.
[190.86 --> 191.92]  The show notes, Alex.
[192.56 --> 192.92]  Yeah.
[193.08 --> 193.28]  Yeah.
[193.36 --> 193.52]  Yeah.
[193.76 --> 194.76]  Well, it's pretty cool.
[194.76 --> 197.14]  So it uses an open source firmware called Valetudo.
[197.90 --> 204.50]  And then you can create in the, it basically turns your robot vacuum into an Ubuntu Linux computer.
[204.80 --> 207.34]  You can SSH into it and all that kind of cool stuff.
[207.42 --> 209.40]  But it also presents a web UI.
[209.80 --> 215.98]  And that web interface lets you drag certain zones and create a name, certain zones based on coordinates.
[215.98 --> 223.08]  And then you can reference those names in Home Assistant automations, create vacuum cards and with icons and stuff.
[223.08 --> 228.28]  So, for example, my RoboVac tends to run overnight, but our bedroom door is always closed.
[228.60 --> 236.30]  And so what I wanted was at, you know, 11 a.m. or something, once we're definitely out of bed and stuff, is for it to go and do the bedroom.
[236.74 --> 239.76]  And 11 a.m. every morning, it doesn't do the rest of the house.
[239.90 --> 245.56]  It literally just goes and finds its way to the bedroom, cleans the bedroom, and then goes back to its charging dock all by itself.
[246.90 --> 247.86]  It's so cool.
[247.92 --> 249.56]  I love the screenshots in your blog post.
[249.64 --> 251.52]  Definitely worth checking out.
[251.52 --> 259.18]  We wanted to chat a little bit about Docker today because they've been in the news recently in a way that impacts the enthusiast and, I think, the small business market.
[259.68 --> 260.56]  And it's something worth chatting.
[260.74 --> 265.34]  So we wanted to bring on two prime individuals to discuss this topic.
[265.66 --> 269.82]  Mr. Michael Dominick from the recently returned Coder Radio podcast is joining us.
[270.24 --> 274.74]  And Mr. Wes Payne from Linux Unplugged to help us go through all of this.
[275.24 --> 275.74]  Well, hello, gentlemen.
[275.88 --> 277.04]  Welcome to the Self-Hosted Podcast.
[277.52 --> 278.30]  Thank you for having us.
[278.48 --> 278.88]  Thank you.
[278.88 --> 283.24]  So let's set this story up, just recap in case people aren't familiar with it.
[283.68 --> 289.34]  As of while we were recording about a week ago, Docker announced some pretty significant changes to their terms of service.
[289.66 --> 296.42]  So Docker, everyone knows, world's largest container technology and also image repository at the Docker Hub.
[296.48 --> 301.54]  They currently store more than 15 petabytes of image data.
[301.54 --> 313.68]  And they write, after a detailed analysis of the container images stored on Docker Hub, we found that 4.5 petabytes of the data had not been pushed or pulled within six months or longer.
[314.06 --> 322.52]  We are making this move to optimize operations and make the Docker Hub service even stronger for developers and development teams around the world.
[322.52 --> 330.20]  So the new policy is after a certain amount of time, they will automatically delete your image from the Hub.
[330.66 --> 336.04]  So as of this recording, the default retention time for free plans will be six months.
[336.08 --> 338.76]  If you don't push or pull within six months, they're deleting it.
[338.98 --> 343.52]  And then there's paid plans that have longer retention times, which will probably all change over time.
[343.52 --> 347.66]  So to keep this kind of evergreen, I'll just be vague, but you can pay to have it retained longer.
[347.80 --> 353.50]  So this is upsetting a lot of people who don't frequently update their containers.
[353.78 --> 355.28]  I'm curious what your thoughts are, Mike.
[355.72 --> 357.00]  Thanks for having me, Chris and Alex.
[357.30 --> 358.66]  And Wes, good to hear from you again.
[359.46 --> 365.52]  So I have solved this problem in the most neckbeard freedom way by simply hosting my own Docker container registry.
[365.84 --> 366.32]  It's great.
[366.74 --> 368.90]  DigitalOcean will give you a droplet for like 20 bucks.
[369.00 --> 369.94]  I'm very happy about it.
[369.94 --> 382.32]  Having said that, I think there's a little bit of a GitHub problem here where some folks who are maybe on the business side of things are confusing Docker Hub with Docker, the technology itself, right?
[382.72 --> 385.60]  Docker Hub is just a service to host your Docker images.
[386.46 --> 394.52]  And, you know, just like you wouldn't get be able to easily pull them and update them and whatever, where there's absolutely no reason you cannot use the open source Docker project.
[394.74 --> 398.12]  Spin up your own server running there again, open source software.
[398.12 --> 400.94]  And, well, frankly, self host it, right?
[401.00 --> 401.70]  It's the name of the show.
[402.14 --> 404.78]  I would strongly recommend if you're like me.
[404.96 --> 419.38]  And, for instance, I have a few legacy containers that are like older versions of Rails that I have for clients that, while I don't use them often, certainly not every six months, I do use them, you know, every once in a while, they want to upgrade their physical servers, right?
[419.38 --> 422.66]  And they need a new, you know, a new copy or a new image rather.
[422.66 --> 431.22]  So, I would strongly suggest, especially the JP audience, it is just not that hard to run your own Docker registry and go for it.
[431.22 --> 436.90]  An interesting angle that you see in a lot of the commentary online is this reproducible build situation.
[436.90 --> 452.44]  And when you look at most of the images that are on Docker Hub, some, not all, I would say the percentage has increased over the last five years or so, include a Docker file alongside the image that's been published.
[452.44 --> 469.72]  Many people argue that those Docker files represent reproducible builds, but I disagree quite strongly because the moment you have something like apt-get update or apt-get install package blah, without pinning it to a specific version, it's not a reproducible build.
[469.90 --> 470.04]  Yes.
[470.04 --> 477.50]  And so, running that Docker file today will give you a different result than it gave you six months to 12 months ago and so on.
[477.50 --> 486.44]  And I think a lot of the outcry from certainly some of the areas of the community is because we're losing that kind of historical artifact.
[487.02 --> 492.24]  Now, that is kind of offset a little bit when you self-host a registry because obviously you're in full control.
[492.42 --> 502.02]  But the lens that I'm looking at this through is my former project, linuxserver.io, where we have tens of thousands of pulls a day from Docker Hub.
[502.02 --> 510.08]  The bandwidth cost alone, even from DigitalOcean, who are very reasonable, it's just not sustainable for an open source project.
[510.08 --> 521.12]  Yeah, I think this is kind of where things get confusing because Docker has been and still is a lot of different things from the, you know, sort of Mobi-ish nebulous backends of how you make containers work at all.
[521.12 --> 527.40]  But then also this sort of community aspect, this common area that you could all share at.
[527.80 --> 533.58]  And yes, you can often go rebuild things, but that's not where people first meet Docker, right?
[534.00 --> 537.24]  Sometimes it's go build your first Docker file and build it that way.
[537.32 --> 543.76]  But so many people, and Alex, I think you're spot on there, especially, you know, coming from Linux server, using the great Linux server images.
[543.76 --> 554.98]  Well, I'm just going to go pull down that software, and it's more of an application packaging format of this, you know, these binary file system layers than it is anything about playing a role in a CICD system.
[555.28 --> 559.92]  And that's where it kind of gets confusing because there's just a lot of stuff under this one Docker name.
[560.40 --> 560.72]  That's true.
[560.80 --> 565.52]  And I do think it's hard to divorce Docker's success from Docker Hub.
[565.52 --> 582.20]  I think Docker, while obviously it's possible to host your own images and have alternative hubs and third-party repositories, I think it was the combination of Docker and Docker Hub and being so easy to invoke images from Docker Hub with very little command syntax.
[582.64 --> 586.42]  I think it contributed pretty significantly to the success of the project.
[586.86 --> 592.32]  Like often said, what happens to the default matters a lot because it will impact the majority of users.
[592.32 --> 617.34]  And just to clarify for those that aren't really familiar with what Chris is talking about, when you do Docker pull image, there is some code, basically hard-baked into the Docker software, that substitutes Docker pull image for Docker pull docker.io slash image colon tag, like short code for that default tag is latest.
[617.34 --> 629.92]  So by hijacking effectively that root namespace, Docker by default captured so much of the traffic and they must get absolutely hammered every day.
[630.02 --> 631.64]  I mean, what did you say at the beginning?
[631.86 --> 634.12]  45 petabytes worth of images.
[634.26 --> 640.32]  I mean, that's just, that's a huge amount of data and they're storing this stuff on S3, according to my research.
[640.32 --> 642.60]  And, you know, we know that isn't going to be cheap.
[642.74 --> 650.00]  And so from, you know, a businessman perspective, I can absolutely understand why they can't continue giving this away for free.
[650.34 --> 655.30]  But I look at some of the parallels between this and say GitHub, for example, and how they used to charge for stuff.
[655.56 --> 659.64]  And isn't Docker.com, what's the purpose of Docker.com or the Docker Hub?
[659.64 --> 674.00]  I think originally it was kind of that the first hit is free and we'll get people in to buy stuff for the enterprise and we'll subsidize Docker.com and the hub through this kind of insidious, you know, namespace hijack.
[674.50 --> 678.36]  But Docker Inc. is now owned by Mirantis, I think.
[679.00 --> 682.42]  And I'm not even honestly sure who owns Docker Hub now.
[682.52 --> 684.98]  I can't tell you if it's Mirantis or not.
[684.98 --> 692.18]  I think you're right about that because it is, you know, there is still Docker contributing, but they sold off their enterprise business to Mirantis.
[692.42 --> 696.86]  And so in some ways, the, you know, the GitHub journey, it's the opposite where now they're a part of Microsoft.
[696.86 --> 699.98]  They've got this big backing of a giant corporation.
[700.26 --> 706.14]  And now Docker Inc. is left as this sort of small progenitor of, you know, the Docker tooling and the ecosystem.
[706.14 --> 712.42]  But without all those lucrative enterprise contracts and is apparently just trying to focus more on the tooling side of things.
[712.84 --> 716.28]  But yeah, still has to pay for petabytes and petabytes of storage.
[716.88 --> 719.22]  And there's the historical perspective here.
[719.46 --> 727.02]  Way back when we had them on Coder, when they were still .cloud, Docker was just a way for .cloud, the business, to sell hosting services, right?
[727.54 --> 730.66]  Like they made their money charging you for running your applications.
[730.66 --> 736.10]  You know, honestly, Alex, I didn't even think of the open source project perspective because I'm, you know, I guess still evil.
[737.46 --> 741.76]  But I'm thinking more of a small ISV where, yeah, I mean, my images are relatively small.
[741.84 --> 743.48]  It's just easy to throw up an instance, right?
[744.12 --> 753.30]  It's certainly true that now that their primary business is not, in fact, hosting your applications, that, yeah, these petabytes of traffic are got to be killing them financially.
[753.30 --> 756.72]  And you touched on it there, and I kind of bring it back to the original story.
[756.82 --> 769.12]  I think it is small businesses that are selling some sort of slow-moving piece of business class software to a client or a customer that are going to be hit the worst by this change.
[769.12 --> 781.06]  Because it's entirely possible that a back office piece of software that runs a small doctor's clinic or an accountant's office may not get changed in three years.
[781.52 --> 784.04]  And so it could easily trip the six-month window.
[784.48 --> 791.78]  And I could see if you're a small shop, you're just packaging things up into a container for your clients, and you're publishing it on Docker Hub because it's simpler that way.
[791.78 --> 804.96]  Some scenario to that I could see impacting small business pretty significantly, but I think it's probably pretty easy for Docker to make the argument that if you're using this for professional services, you should have a paid account.
[805.60 --> 806.64]  I think I agree with you.
[807.64 --> 816.84]  So to work around this issue, a lot of the online commentary was, okay, I'm just going to write a cron job, a bash script that's going to pull this image every 5.99 months or whatever.
[817.10 --> 817.88]  Of course.
[818.26 --> 818.78]  Love it.
[818.78 --> 832.10]  But if you look at the small print towards the end of the announcement, the free tier limits you to 100 unauthenticated pulls every six hours and 200 every six hours that are authenticated.
[832.36 --> 835.22]  So again, this is coming at it from the Linux server perspective.
[835.64 --> 847.16]  If, let's say, even just a few dozen of those users all ran scripts that happened to run the last or the first day of the month or whatever, are you not able to pull images at all?
[847.16 --> 848.86]  Do you just get sorry, rate limit exceeded?
[849.10 --> 850.58]  Or what happens?
[850.64 --> 857.94]  And I think a lot of that fear for me is really centered around open source projects that rely on Docker Hub.
[858.50 --> 866.76]  Because my day job is working in the enterprise on OpenShift, which has built-in registries and everything's hosted behind the firewall.
[866.88 --> 871.34]  I'm not really too worried about Docker Hub from a business perspective.
[871.34 --> 875.08]  Because, you know, like Mike said, you just spin up your own and it's super simple.
[875.26 --> 879.90]  And it's become the, dare I say it, the standard packaging format for the server.
[880.42 --> 880.50]  Yeah.
[880.74 --> 882.72]  Nginx's image, that's not going anywhere, right?
[882.72 --> 883.28]  There's a company.
[883.84 --> 884.36]  But you're right.
[884.42 --> 888.18]  I mean, here in the terms of service, they reserve the right to enforce if they want to.
[888.32 --> 893.68]  And that includes stuff like quantity of data, age of data, poll rate, and number of image auto builds.
[893.68 --> 897.78]  So it'll be interesting to see which projects they actually choose.
[897.94 --> 901.50]  You know, is this really meant to cull the images that are never used anywhere?
[901.64 --> 910.32]  Or will there be large, successful open source projects that have been using Docker Hub as, you know, the way to distribute their project, but can't afford a non-free plan?
[910.32 --> 918.34]  You have to wonder if this is the beginning of a different, more services-based monetization strategy.
[918.64 --> 922.28]  You look at Docker and you look at the history of the projects.
[922.40 --> 925.48]  We've been tracking this thing since, what, 2013?
[925.48 --> 932.32]  And you saw a lot of really rapid innovation and security issues be discovered and fixed.
[932.50 --> 939.82]  And overall system-level changes to accommodate containers happen really between 2013 and 2015.
[940.36 --> 943.26]  That's when the OCI launched the Open Container Initiative.
[943.40 --> 946.26]  And that was really kind of creating an open standards body for containers.
[946.26 --> 948.48]  And we kind of got this normalized approach.
[948.48 --> 957.62]  I mean, since really 2015, 2016, there hasn't been massive accomplishments or changes or innovations in Docker.
[958.14 --> 958.86]  They changed the name.
[959.30 --> 961.62]  Yeah, there's been a lot of weird company stuff going on.
[961.98 --> 966.68]  But I wonder if this is a bit of a hands-up approach saying, well, maybe this is how we're going to make money.
[967.02 --> 971.42]  You know, they were pushing Swarm for quite some time, but clearly Kubernetes won that race.
[971.74 --> 972.86]  That didn't take off.
[972.92 --> 976.56]  And so now they're left having to, you know, try to make, what's the point of Docker?
[976.56 --> 978.02]  We already have these images, right?
[978.02 --> 980.50]  We know that there's standards outside of their control.
[980.98 --> 988.68]  And all their sort of retooling around Mobi, a lot of that was just to also, you know, piecemeal things out and use a lot of things like RunC and LibContainer.
[988.86 --> 991.22]  All the stuff that's also out there in the community.
[991.46 --> 993.74]  So their role is just shrinking and shrinking.
[994.26 --> 999.92]  Yeah, and we know right now, as around the time we're recording this, they're raising money.
[1000.42 --> 1002.86]  They just got a $1.3 billion valuation.
[1003.28 --> 1005.78]  So they're on the market looking for an investor.
[1005.78 --> 1009.14]  I kind of expected Microsoft to buy Docker for quite a long time.
[1009.54 --> 1009.80]  Yes.
[1010.06 --> 1010.80]  Well, maybe.
[1011.08 --> 1012.56]  I mean, if you're buying TikTok, why not?
[1015.56 --> 1023.40]  Sometimes, you know, the trying to raise funds initiative turns into a getting purchased initiative that has happened in the history of tech companies.
[1023.40 --> 1026.94]  So am I the only one who's maybe a little too simplistic about this?
[1027.46 --> 1033.96]  I mean, when they were .cloud and Chris, you and I spoke to them, their business was hosting your application and making deployment super easy.
[1034.24 --> 1034.46]  Yeah.
[1034.90 --> 1036.84]  Why can that not be the business today?
[1037.06 --> 1037.38]  Right.
[1038.74 --> 1040.36]  Because they waited too long.
[1040.52 --> 1043.90]  And now there's tons of places to host Docker containers for cheap.
[1043.98 --> 1044.22]  Sure.
[1044.64 --> 1046.06]  Did Heroku exist back then?
[1046.28 --> 1046.72]  It did.
[1046.82 --> 1049.34]  But Heroku was very expensive at that point, right?
[1049.34 --> 1053.02]  It was before Salesforce dumped a wad of money into them and said, lower your prices.
[1053.66 --> 1058.24]  I'd argue that that's probably the biggest one-click app competitor to that kind of model.
[1058.50 --> 1058.90]  Absolutely.
[1059.10 --> 1059.22]  Yeah.
[1059.56 --> 1061.68]  And also, Kubernetes wasn't a thing.
[1061.94 --> 1062.14]  Yeah.
[1062.14 --> 1070.64]  I know I'm probably slightly biased, but people like Red Hat hadn't woken up to, you know, Kubernetes and VMware now have got their own Kubernetes.
[1070.98 --> 1073.64]  And anybody who's anybody has a Kubernetes play now.
[1074.08 --> 1076.76]  And Docker Swarm is just not relevant.
[1076.76 --> 1087.02]  And I think if you look at the history of Docker as a company, their largest misstep was around that kind of 2016 timeframe when they kind of made an enemy of Red Hat.
[1087.16 --> 1094.30]  And then Red Hat decided to make Podman and Cryo and, you know, basically stop shipping Docker.
[1094.74 --> 1097.30]  We like your idea, but we'll do it our way.
[1097.70 --> 1097.92]  Yeah.
[1098.26 --> 1098.48]  Yeah.
[1098.52 --> 1099.46]  No, Alex makes a great point.
[1099.54 --> 1102.44]  I mean, AWS, Red Hat, all the big services.
[1102.60 --> 1104.98]  I think even Azure offers Kubernetes support now, right?
[1105.14 --> 1105.60]  Yeah, they do.
[1105.68 --> 1105.78]  Yeah.
[1105.78 --> 1107.12]  The future will be interesting.
[1107.34 --> 1110.60]  So they're getting an influx of $75 million.
[1111.02 --> 1116.80]  These are all, according to people familiar with the matter, the deal is supposed to close at the end of this month.
[1117.34 --> 1129.42]  And it looks like they're going to use the funds to hire salespeople, marketing team, and have them go after corporate clients, according to people familiar with the matter.
[1129.80 --> 1133.24]  So Docker apparently sees the future in corporate.
[1133.24 --> 1143.08]  By the way, what was interesting during this entire process, they've only increased in a billion valuations since they were last evaluated in 2015.
[1143.08 --> 1144.08]  Interesting.
[1144.08 --> 1144.64]  Interesting.
[1144.64 --> 1148.00]  You know, there's also sort of a lag in a lot of this stuff.
[1148.08 --> 1156.94]  You know, there's still maybe smaller or just lagging behind enterprises that haven't made the shift fully into the containerized world or just starting to play in that space.
[1156.94 --> 1165.24]  And I wonder, you know, a lot of the developers I know who maybe aren't super into the technology but need to use these tools, they've recently tried Docker.
[1165.38 --> 1166.14]  They've been using Docker.
[1166.14 --> 1170.76]  I think we'll still see the Docker name being used, at least on the command line, for a while to come.
[1170.84 --> 1176.36]  But it'll be interesting to see if, you know, eventually just the other sorts of tools supplant them as the default.
[1176.98 --> 1179.02]  It's the Kleenex of containers.
[1179.30 --> 1179.70]  Exactly.
[1180.28 --> 1182.96]  So moving on to Terraform, let's have Wes stick around.
[1183.14 --> 1184.86]  Thank you, Mr. Dominic, for joining us.
[1185.40 --> 1186.80]  And shift gears to news.
[1187.00 --> 1188.32]  This is a news-heavy episode.
[1188.44 --> 1191.06]  And shift gears to Terraform 0.13.
[1191.06 --> 1194.96]  Now, most of you are probably wondering, why on earth this is even a big deal?
[1195.06 --> 1197.26]  0.13 doesn't sound that important.
[1197.88 --> 1203.16]  Well, Terraform have revolutionized the way that I deploy infrastructure.
[1203.36 --> 1212.16]  So for those that aren't even familiar with what Terraform is, it's a way to declaratively define infrastructure as code.
[1212.68 --> 1215.26]  Much like we would do with a piece of software.
[1215.72 --> 1217.30]  We would say, here are our dependencies.
[1217.80 --> 1220.86]  Here is what, you know, the various different interfaces we have and stuff like that.
[1221.46 --> 1223.34]  We can do the same with our infrastructure.
[1223.52 --> 1227.44]  We can say, I want this, you know, let's say a droplet, for example.
[1227.70 --> 1233.86]  I want this firewall rule to allow traffic on port 80 to this IP address, etc., etc., etc., right?
[1233.86 --> 1240.54]  And the benefits of doing this stuff with Terraform is that you can store it as code in a Git repo.
[1240.82 --> 1243.82]  So you can version everything that's happening.
[1243.82 --> 1254.48]  So let's say that I am part of a development team at work and we want to, you know, change the size of our default droplets from the $5 to the $10 one, for example.
[1255.02 --> 1265.66]  I can go in and make that change, but I have to commit it to Git in order for that change to be picked up by my CI pipeline and then push those changes to production.
[1265.66 --> 1270.92]  So it's basically a way of enabling a paper trail for infrastructure changes.
[1271.58 --> 1280.20]  Now, the reason that 0.13 got me so excited is because I use it a lot at home for doing home lab stuff with OpenShift.
[1280.20 --> 1287.64]  And with 0.13, you can do something which doesn't sound like a big deal until you've tried it.
[1288.56 --> 1291.02]  Terraform has this concept of count.
[1291.42 --> 1295.48]  And what that lets me do is it says, right, I want three web servers.
[1295.84 --> 1297.82]  Count equals three on my web servers.
[1298.66 --> 1301.28]  Traditionally, that only worked at the resource level.
[1301.40 --> 1304.02]  So each thing that you create is a resource.
[1304.58 --> 1306.58]  Now I can define a module.
[1306.58 --> 1311.48]  So what that lets me do is reuse different bits of code from across the code base.
[1311.58 --> 1320.78]  Now I've written a blog post about this because some of these concepts are a little abstract to explain in a podcast without making it sound super duper boring and training-y.
[1321.24 --> 1321.68]  No kidding.
[1321.98 --> 1324.94]  So in the blog post, I talk about count and modules.
[1325.14 --> 1333.90]  And so what this lets me do is write reusable chunks of resource definitions that I can then call from the parent module.
[1333.90 --> 1339.72]  So I can create, you know, one file that defines how all of my droplets are created.
[1340.04 --> 1347.96]  And then I can recall or reuse that piece of code from anywhere else in my code base and pipe in a bunch of variables in real time.
[1348.36 --> 1349.56]  It's super duper cool.
[1349.72 --> 1356.08]  And if you aren't using Terraform or any kind of automation to create infrastructure, I highly suggest you take a look.
[1356.86 --> 1359.36]  Now, Wes, you use Terraform a little bit, don't you?
[1359.68 --> 1360.04]  I do.
[1360.04 --> 1366.88]  You know, when Terraform first came out, I was so excited because, especially at the time, I was using a lot of AWS.
[1367.72 --> 1380.90]  And after you have a few people, maybe a couple different generations of teams that have all gone into the console, which, as people who use it know, keeps adding more and more and more buttons to click, you've got this infrastructure that, I mean, yes, you can document it.
[1380.90 --> 1386.00]  But it's a real pain because there's all kinds of different systems, different networks, different VPCs.
[1386.08 --> 1387.02]  How many databases?
[1387.16 --> 1388.48]  How many instances did you spin up?
[1388.76 --> 1390.20]  Were those settings the settings you meant to?
[1390.26 --> 1393.58]  Are those just the settings that you applied at the time and they don't make sense anymore?
[1393.58 --> 1404.20]  And with Terraform, you've just got all of that packaged for you right there, let alone the advantages you can have because, well, the AWS API is different than the DigitalOcean one.
[1404.32 --> 1407.10]  But it turns out I've got infrastructure on each of those.
[1407.48 --> 1410.02]  I don't want to have to wrap all those API calls up myself.
[1410.66 --> 1413.06]  Well, Terraform took care of that so nicely.
[1413.54 --> 1414.14]  And you're right.
[1414.24 --> 1417.92]  I think one of my biggest complaints about it, it's doing a great job.
[1417.96 --> 1420.98]  And I like the configuration language, HCL.
[1421.46 --> 1422.38]  It's declarative.
[1422.50 --> 1424.40]  You know, you get to say, like, this is what I want.
[1424.40 --> 1432.54]  And instead of telling the computer how to do it, well, you know, Terraform has modules, has functionality built into it to go build those things out for you in the real world.
[1433.18 --> 1441.72]  But I have noticed having to repeat myself a little more than I would like and made me wish that I could reach for a little more full powered language or something.
[1441.72 --> 1443.78]  So these changes, huge.
[1444.38 --> 1450.16]  It's one of those changes that when it came out or was announced anyway, I was like, oh, this is the way it should have been.
[1450.56 --> 1452.94]  It's one of those changes that you just think, yes, this is a good one.
[1453.08 --> 1454.76]  This is absolutely needed.
[1455.66 --> 1463.98]  And you touch on one of the most important things about Terraform for me is how it basically abstracts you away from the underlying infrastructure.
[1463.98 --> 1474.38]  So I can write code that will target VMware and Amazon and DigitalOcean and Linode and insert all of the other cloud providers as well.
[1474.82 --> 1478.40]  I think KVM recently got some updated stuff for Terraform.
[1478.52 --> 1480.44]  I think Proxmox might have done as well.
[1480.44 --> 1492.36]  So, you know, there is no real excuse in my mind, at least, not to be using these kinds of things to automate infrastructure deployments because, let's face it, we've all been there.
[1492.50 --> 1497.16]  We've all installed a server and we're like, how did that get there?
[1497.16 --> 1500.10]  You know, six months later, how did I deploy this?
[1500.18 --> 1501.24]  Which image did I use?
[1501.38 --> 1506.22]  Which firewall rule applies to this particular thing or whatever?
[1506.48 --> 1510.28]  And by having your infrastructure as code, it's there right in front of you.
[1510.30 --> 1511.44]  The answer is always there.
[1511.60 --> 1515.48]  So what's it going to take to convince Chris to use it, though?
[1515.60 --> 1516.44]  That's what I want to know.
[1516.72 --> 1517.80]  That's a good question.
[1518.10 --> 1519.00]  Raspberry Pi support?
[1519.22 --> 1519.92]  Ha ha ha ha.
[1520.52 --> 1521.12]  I can't help it.
[1521.18 --> 1521.48]  I have to.
[1521.48 --> 1525.00]  Well, the thing is about Terraform is that it's at the infrastructure layer.
[1525.00 --> 1531.54]  So it's more about creating virtual machines and the ancillary stuff that goes around them.
[1532.36 --> 1536.64]  So I would say for configuring the Pis themselves, Ansible is probably a better bet.
[1537.06 --> 1540.80]  And I tend to use Ansible for configuring the machines once Terraform has brought them up.
[1541.06 --> 1541.10]  Right.
[1541.58 --> 1541.92]  Hmm.
[1542.40 --> 1542.80]  Let's see.
[1543.08 --> 1546.26]  We often see a lot of confusion about, you know, which tools should I be using?
[1546.32 --> 1550.28]  Because, I mean, Ansible technically can do a lot of what Terraform does.
[1550.28 --> 1555.84]  Because I find personally that the delineation between one tool to create the infrastructure
[1555.84 --> 1560.64]  and another tool to quote unquote configure the infrastructure, I find that separation
[1560.64 --> 1561.34]  quite helpful.
[1561.64 --> 1564.22]  And the two, you can call them from one another as well.
[1564.70 --> 1564.78]  Yeah.
[1564.98 --> 1570.18]  In a past life, I was managing a system that provisioned a whole bunch of EC2 resources using
[1570.18 --> 1575.32]  entirely Ansible and moving the parts of that that were just infrastructure specific and
[1575.32 --> 1579.90]  not all the, you know, OS configuration out to Terraform made it so much clearer.
[1580.16 --> 1583.96]  And it was just simpler because honestly, Terraform does a great job of keeping up with all the
[1583.96 --> 1584.86]  AWS changes.
[1585.36 --> 1587.88]  Oftentimes, they've got stuff even before CloudFormation does.
[1587.96 --> 1589.44]  So it's just a better tool.
[1590.00 --> 1590.60]  It's a funny story.
[1590.74 --> 1596.02]  I actually found out that DigitalOcean were releasing VPC support by reading the Terraform
[1596.02 --> 1597.86]  docks before it was announced on DO.
[1598.30 --> 1601.24]  I found it in the Terraform docks, which I thought was quite cool.
[1601.88 --> 1602.82]  Well, I know we got to get going.
[1603.02 --> 1606.50]  But before we do, I think you ordered something new.
[1607.22 --> 1610.22]  And I think maybe you forgot you got role swapped here, Alex.
[1610.26 --> 1614.72]  I thought I was the super cool small board computer NAS guy.
[1615.24 --> 1619.46]  Well, don't tell my wife, but I might have impulse bought a single board powered system.
[1619.76 --> 1622.66]  It's the Helios 64 from COBOL.io.
[1622.66 --> 1626.34]  And this thing is the ultimate ARM powered NAS.
[1627.24 --> 1631.98]  It has four gigabytes of RAM, a built in battery pack.
[1632.24 --> 1638.48]  It supports five three and a half inch hard drives, has a USB 3 type C input.
[1638.96 --> 1641.44]  So you can use it as a DAS as well as a NAS.
[1642.08 --> 1648.54]  And I don't know, like I'm not super duper thrilled about only four gigs of RAM, but I
[1648.54 --> 1653.82]  think for a few media apps and a little bit of file storage here and there should do the
[1653.82 --> 1654.70]  trick really nicely.
[1655.06 --> 1655.56]  What do you think?
[1655.80 --> 1658.68]  Yeah, I can't wait to buy it from you secondhand after you're done with it.
[1660.96 --> 1661.76]  Yeah, maybe.
[1661.96 --> 1662.36]  We'll see.
[1662.80 --> 1666.08]  I mean, I saw it and I thought of you because it's got a couple of gigabit NICs.
[1666.12 --> 1667.60]  It's got a few USB ports.
[1668.24 --> 1670.00]  I think it's got an HDMI out as well.
[1670.00 --> 1675.42]  So one of the screenshots they show on their website is of it running Kodi on your TV.
[1675.68 --> 1677.54]  So that could be an interesting use case.
[1677.80 --> 1678.08]  Huh.
[1678.38 --> 1682.58]  I like reducing down a little bit the NAS and the TV box all in one.
[1682.74 --> 1684.66]  You know, it's going to play back good in that scenario.
[1685.00 --> 1689.32]  Yeah, it's also got USB-C and runs off DC power.
[1689.46 --> 1692.86]  And like you said, that built in battery, that could be really handy too.
[1693.46 --> 1695.20]  I can't wait to hear your thoughts on this.
[1695.58 --> 1696.48]  It ships in August.
[1696.48 --> 1699.98]  So we're still technically in August by a few days here as we record.
[1700.18 --> 1701.10]  So I don't know.
[1701.24 --> 1701.72]  Come on, guys.
[1701.82 --> 1703.02]  Get mine out the door, please.
[1703.12 --> 1705.02]  I want to tell the good self-hosted people.
[1706.02 --> 1708.72]  Well, that brings us to the end of self-hosted.
[1708.96 --> 1710.78]  Well, you can find our sponsor on social media.
[1710.88 --> 1714.28]  Cloud Guru is at twitter.com, youtube.com and facebook.com.
[1714.32 --> 1715.86]  They're all just slash a Cloud Guru.
[1716.22 --> 1716.96]  Couldn't be easier.
[1717.32 --> 1718.18]  Thank you to Wes.
[1718.20 --> 1722.76]  You can find links to Wes and Mike's Twitter accounts in our show notes.
[1722.78 --> 1725.88]  And of course, you can go get more Wes Payne on the Linux Unplugged.
[1725.88 --> 1727.12]  Anything else you want to mention, Wes?
[1727.18 --> 1728.06]  Thank you for having me.
[1728.16 --> 1729.54]  I'm off to my home lab.
[1731.04 --> 1732.04]  Thanks for being here.
[1732.40 --> 1732.74]  All right.
[1732.84 --> 1734.10]  That's self-hosted 26.
