[0.00 --> 2.26]  Can you believe scale is next week?
[2.32 --> 6.18]  We're almost at conference silly travel season already.
[6.42 --> 7.22]  How has that happened?
[7.94 --> 12.46]  Today just started packing my remote broadcasting bag.
[12.96 --> 16.68]  I'm thinking through this because I'm going to try to do four live streams.
[17.04 --> 17.50]  Ooh.
[18.64 --> 19.24]  Yeah.
[19.46 --> 20.24]  The struggle's real.
[20.24 --> 22.98]  I mean, you know, now I make videos for a living somehow.
[23.30 --> 28.16]  I've got to pack camera gear and tripods and microphones and all sorts of nonsense.
[28.16 --> 31.88]  Are we doing a live JB thing whilst we're there?
[32.28 --> 32.50]  Yeah.
[32.66 --> 32.90]  Yeah.
[32.98 --> 33.28]  Oh, yeah.
[33.34 --> 33.48]  Yeah.
[33.48 --> 34.08]  I want to do a couple.
[34.22 --> 35.46]  And then there's – we'll see.
[35.52 --> 38.76]  I haven't decided what we're doing for Unplugged, but it does happen that Sunday.
[39.42 --> 40.86]  So I've got to figure out something for it.
[41.06 --> 41.46]  Yeah.
[42.08 --> 42.44]  Soon.
[42.78 --> 44.54]  I know there's like so much to plan and pack.
[44.62 --> 47.26]  I can't believe that we're just a few days away from hitting the road.
[48.06 --> 48.66]  Not ready for it.
[48.66 --> 51.42]  And then shortly after that, it's Texas Linux Fest and then Linux Fest Northwest.
[52.42 --> 55.42]  And rumor has it I may be at Red Hat Summit as well.
[55.50 --> 57.66]  So a lot of events coming up in a short period of time.
[57.66 --> 58.66]  Red Hat Summit Hut.
[58.76 --> 61.22]  You know, I never got to go to Summit as an employee.
[62.02 --> 63.96]  I was always a little bit miffed about that.
[64.06 --> 65.38]  But, you know, such is life.
[65.94 --> 66.08]  Yeah.
[66.22 --> 66.72]  Oh, yeah.
[66.74 --> 67.40]  It's a good party.
[67.46 --> 70.46]  The last time I went was just before the IBM acquisition.
[71.20 --> 72.80]  So it'll be an interesting comparison.
[73.36 --> 73.94]  Ah, yes.
[73.96 --> 74.44]  That's right.
[74.48 --> 75.60]  Because I'd just moved here.
[75.66 --> 76.84]  We'd just started the show.
[77.18 --> 77.62]  Yeah.
[77.70 --> 81.02]  I remember actually thinking I almost made it to that one.
[81.18 --> 81.48]  But, yeah.
[81.66 --> 82.76]  Anyway, that was a long time ago.
[83.46 --> 86.84]  Joining us on the show today is John Seeger, a VP at Canonical.
[86.84 --> 90.16]  Looks after Juju and a bunch of other infrastructure related stuff.
[90.80 --> 93.84]  However, we're going to talk to him about Nix primarily today.
[94.22 --> 97.84]  So if you're into Nix, you will enjoy this interview with John.
[98.30 --> 99.46]  Well, John, welcome to the show.
[99.74 --> 105.64]  And I recall that you work in the Juju and Charms area at Canonical, which I'm vaguely familiar with.
[105.70 --> 111.80]  But I thought maybe we could start with an explanation of what Juju and Charms are and how people manage infrastructure with them.
[111.80 --> 112.98]  Yeah, of course.
[113.22 --> 122.12]  So Juju is an orchestration tool that is used for deploying all kinds of different workloads on any kind of infrastructure.
[122.30 --> 125.34]  So it kind of prides itself on being super multi-cloud.
[125.48 --> 129.50]  So you can deploy to bare metal, to LexD containers, to AWS, to Kubernetes.
[129.92 --> 132.02]  You can use it to deploy a Kubernetes on AWS.
[132.02 --> 136.36]  And the way it does that is with packages called Charms.
[136.68 --> 139.84]  So Charms are just applications, right?
[139.90 --> 146.86]  So they're composed of a workload, maybe Postgres, for example, and typically some Python code, which is the charm itself.
[146.98 --> 152.42]  And that is a pretty simple piece of Python that responds to essentially events that are sent from the controller.
[152.52 --> 157.40]  So the controller will say, stand up a machine, and then it will feed it a sequence of events like install.
[157.40 --> 161.38]  And there'll be a callback essentially in the Python code that will then go and install Postgres.
[161.50 --> 165.78]  It might then send in a configure hook, and there'll be callbacks in there to respond.
[166.48 --> 169.80]  But the deployment side is kind of the least interesting side.
[169.88 --> 173.92]  It has this concept called integrations, previously known as relations.
[174.62 --> 182.40]  And the kind of big thing, point about Juju, is how to make the integration and operations side much more easy.
[182.56 --> 186.42]  So I think the deployment of apps is kind of boring, kind of a solved problem.
[186.42 --> 187.52]  Ansible can do this.
[187.62 --> 188.44]  Terraform can do this.
[188.66 --> 189.64]  CloudFormation can do this.
[189.68 --> 192.28]  We've been deploying apps with code for years.
[192.52 --> 193.98]  But integration is always really hard.
[194.02 --> 196.34]  Like you get to the data center, the customer has this thing.
[196.42 --> 197.68]  You've got this existing Prometheus.
[197.78 --> 199.84]  You've got this existing database or this old legacy app.
[199.90 --> 201.18]  How do you tie it all together?
[201.32 --> 204.20]  And Juju tries to kind of solve that with these integrations.
[204.86 --> 209.00]  So my role at Canonical is to lead the development of Juju, which is a big Golang project,
[209.00 --> 220.76]  and then a whole suite of teams who are building kind of first class operators for Postgres and MySQL and Grafana and Ori and Kubeflow and kind of a huge range of apps.
[221.40 --> 222.36]  It's a fascinating product.
[222.56 --> 231.10]  I think I first ran across it, probably Config Management Camp in like 2015, 16, something like that.
[231.28 --> 231.64]  And Mark...
[231.64 --> 232.26]  There's a niche conference.
[232.26 --> 235.44]  Yeah, Mark himself was actually talking at the conference about Juju.
[235.56 --> 236.88]  I think it was quite new back then.
[237.38 --> 240.96]  But it's one of those projects I've just sort of followed from a distance.
[241.36 --> 244.30]  And it's certainly got an interesting use case.
[244.84 --> 246.38]  It's a hell of a rough start.
[246.56 --> 247.90]  It's been around for about 10 years now.
[247.94 --> 251.44]  And it's had a very kind of interesting journey.
[251.64 --> 257.98]  We've really kind of picked up in the last three years, really focusing on building the operators that people need to use it, right?
[258.02 --> 259.96]  So now as a developer, you can turn up.
[259.96 --> 268.40]  And if you need a really great HA Postgres that knows how to back itself up and can do cross-region replication, you can just get that.
[268.64 --> 270.56]  You just deploy it and it just does its thing.
[270.78 --> 272.26]  Previously, those things didn't exist.
[272.34 --> 273.66]  So you kind of had to invest yourself.
[273.82 --> 276.20]  But now we are spending the time and effort to do that.
[276.30 --> 279.78]  So all of the apps that you hopefully would come to your mind will be available.
[280.28 --> 286.54]  It's interesting you call them operators because that word in my mind is inextricably linked to Kubernetes.
[287.06 --> 287.42]  Yes.
[287.42 --> 296.46]  When I think of an operator, you know, it's kind of like a capturing of operationalizational – god, that's a difficult word to say, isn't it? – knowledge.
[297.04 --> 303.78]  And, you know, I long ago compared it to like an MSI installer back in the Windows days where it's a bunch of scripts.
[303.94 --> 308.00]  It's a bunch of stuff all wrapped up into one that just captures knowledge.
[308.00 --> 312.46]  Is that a fair comparison to what a Juju operator is?
[312.92 --> 314.86]  The term became popularized by Kubernetes.
[315.22 --> 321.72]  But what's really interesting is that the approach that that kind of captures is exactly what Juju has been doing since 2009.
[321.94 --> 326.00]  So the way I like to characterize it is – take Postgres as the example again.
[326.00 --> 332.24]  Imagine going and finding the person who in your circle knows the most about running Postgres in production.
[332.40 --> 334.54]  Proper gnarly Postgres production, right?
[334.74 --> 338.70]  You know, 10,000 days, lots of backups, lots of replication, lots of connections.
[339.04 --> 347.20]  Take everything that person knows about running Postgres in production and turn it into really clean, well-tested Python code that anyone can get access to.
[347.20 --> 352.74]  And so you move from not just having open source application code – we kind of won that fight, right?
[352.90 --> 356.60]  Postgres, Linux, Grafana, all these amazing applications, there's so much choice.
[357.62 --> 360.78]  But that doesn't necessarily mean people can actually use it in their environment.
[360.92 --> 371.08]  So the move with the operators is almost trying to say, okay, we've got the open source apps, let's go and get open source operations code that lets people actually put it down in their environment and have real faith that it's going to work.
[371.44 --> 374.26]  So you're including the batteries in all of these projects, essentially.
[374.58 --> 374.94]  Exactly.
[375.08 --> 376.08]  We are adding the batteries.
[376.08 --> 377.84]  Yeah, okay.
[378.20 --> 386.70]  So the reason that I actually wanted to talk to you today – forgive me, Gigi's very interesting – but I find Nix at the moment is just all-consuming for me.
[387.28 --> 392.92]  And you've been all over my various feeds, packaging things for Nix and doing this and doing that.
[393.44 --> 398.56]  Why do we need Nix if we're doing integrations with Gigi?
[399.16 --> 400.40]  Why do we need Nix?
[400.40 --> 406.24]  So I got into Nix because I'm just an insufferable Linux desktop nerd, have been for many years.
[406.76 --> 411.66]  I was a very long-time Arch user, some 10, 12 years.
[411.86 --> 412.36]  By the way.
[412.82 --> 413.56]  Yeah, by the way.
[414.06 --> 416.02]  Nix just kept popping up in places.
[416.02 --> 419.66]  And I actually tried it about two or three years ago and, like, bounced off it so hard.
[419.74 --> 421.24]  I was like, don't have the time.
[421.72 --> 422.12]  Ignore.
[422.62 --> 430.96]  And then about, I guess about 18 months ago, I had a spare Intel NUC laying around and kept seeing more and more about it.
[430.96 --> 435.90]  It was about the time that I moved from Twitter to Mastodon where things all got a little bit more interesting.
[435.90 --> 437.90]  And I just gave it a go.
[438.16 --> 441.86]  And the way I got into it was, you know, I was fortunate enough to have another machine.
[442.16 --> 443.78]  And so I installed Nix on it.
[443.90 --> 445.90]  The install process felt pretty familiar to Arch, right?
[446.02 --> 449.18]  But then did all the usual, like, oh, how do I install something?
[449.66 --> 452.06]  I can't change the configuration files.
[452.18 --> 453.54]  And honestly, it was pretty slow.
[453.92 --> 456.60]  But I just slowly, I watched the Will Taylor Nix videos.
[457.32 --> 459.34]  I happened across Flakes really early.
[459.44 --> 461.32]  And so I've only ever really done Flakes.
[461.46 --> 464.20]  I have very little experience with the old way of doing things.
[464.20 --> 466.18]  I'm a software engineer by trade.
[466.22 --> 468.08]  And I think that is kind of quite a nice fit.
[468.64 --> 469.54]  And yeah, I just built it up.
[469.68 --> 476.38]  And what I decided was at the time I was running an Archbox with Sway and a whole bunch of pipe wiring, which at the time was quite bleeding edge.
[476.70 --> 480.84]  And I basically decided I was going to try and build this box up to be exactly the same as my desktop.
[481.54 --> 484.68]  And I sort of got there and thought, all right, well, I'll just go all in.
[484.82 --> 491.56]  Like, I'll just, and I sat here one night, you know, on like a Tuesday evening or something, installed it on my desktop and just like started using it.
[491.56 --> 496.14]  And from then on, well, now it's on all of my personal machines, essentially.
[496.26 --> 501.36]  And it's even on a machine in my parents' and-law's house running a little Telsky Alexa node for them.
[501.48 --> 503.26]  I've sort of just completely fallen for it.
[503.36 --> 506.86]  It feels very difficult to go back for my personal machines.
[507.48 --> 507.72]  I agree.
[507.94 --> 511.84]  I'm definitely at that stage now where family members' computers are all getting nicks.
[512.56 --> 514.02]  Everything's just getting nicks now.
[514.02 --> 516.58]  Unless, you know, unless it's for a specific project.
[517.20 --> 525.46]  But I do think a very common bit of feedback we get is, why do I need nicks if I have something like Juju?
[525.58 --> 527.92]  Or why do I need nicks if I have something like Ansible?
[528.36 --> 534.70]  And it sounds like you're kind of on the school of thought that I have, which is there's room for both.
[534.82 --> 535.56]  Can you expand on that?
[535.56 --> 535.96]  Yes.
[536.64 --> 545.12]  So I definitely sold on the immutable operating system for a workstation or a bunch of servers you kind of manage.
[545.98 --> 547.98]  More in the kind of sysadmini way.
[548.06 --> 551.64]  More in like, here's my collection of my machines that I look after and that I shepherd.
[552.18 --> 556.58]  I'm absolutely certain that using nicks to do things like building containers, right?
[556.62 --> 558.98]  Building OSU Docker containers is a good idea.
[559.06 --> 559.72]  I do this myself.
[559.72 --> 566.00]  My blog is a Docker container built with nicks shipped off to fly.io, and that's how I host it.
[566.42 --> 571.18]  I'm less convinced in big enterprise deployments of lots of HANUS.
[571.30 --> 574.76]  Now, maybe I just don't have the skills yet.
[575.22 --> 579.28]  Like, you still need something to sit in the middle and coordinate all of that, right?
[579.34 --> 585.20]  So at the simplistic end, you've got people punching commands into keyboards and pressing enter with their SSH keys.
[585.52 --> 586.56]  You can level that up a bit.
[586.56 --> 591.98]  There are things like deployRS and Colmina and other deployment frameworks, which you can power with CI, right?
[592.04 --> 593.32]  Like, you write your nicks flake.
[593.40 --> 594.10]  You run the checks.
[594.44 --> 596.06]  You commit it into a Git repository.
[596.60 --> 598.42]  And a CI runner picks that up and deploys it.
[598.94 --> 600.36]  That works for simple things.
[600.48 --> 601.64]  That would work for my lab.
[602.32 --> 608.50]  I don't think that would necessarily work in JP Morgan, where they've got 15 different Postgres databases.
[608.74 --> 610.40]  They have enterprise identity going on.
[610.60 --> 614.62]  They don't necessarily have the engineers to troubleshoot the fact that something's missing a library.
[614.62 --> 616.46]  Do you know what I mean? Because it hasn't been patched properly.
[616.66 --> 617.10]  I don't know.
[617.52 --> 620.64]  You know, this has been the case for many tools over the years.
[620.76 --> 624.38]  But I think with Nix in particular, it is...
[624.38 --> 626.82]  I don't want to say a problem, because it's not.
[626.92 --> 634.04]  It's just a fact, a truth, that there are multiple different ways to solve every single problem.
[634.18 --> 635.48]  And I look at your flake, John.
[635.54 --> 638.54]  And I look at Mitchell Hashimoto's flake.
[638.54 --> 643.80]  And then I look at mine, and they're all solving similar problems, like Wimpy's flake.
[644.00 --> 647.70]  They're all solving the same problem in different ways, like totally different ways.
[648.42 --> 650.28]  It's super hard to get yourself in trouble.
[650.46 --> 655.26]  I worked with this Italian fellow who was a bit of an observability ninja for a little while.
[655.56 --> 659.34]  And he had this phrase, which I think is so apt.
[659.74 --> 661.74]  He was like, it's like radioactive Lego.
[661.92 --> 664.38]  It's super fun to play with, but there might be consequences, right?
[664.38 --> 667.90]  But I think, I'm sure there are people doing Nix at scale.
[668.08 --> 673.44]  But for me, I haven't yet grokked how you would really pull that off as a big operation.
[674.36 --> 676.72]  Nix at the moment for me is all-consuming.
[677.00 --> 680.40]  But I do find myself yak shaving quite often with it.
[680.56 --> 682.86]  Like, I think to myself, okay, good example.
[683.02 --> 684.52]  Plasma 6 came out this week.
[684.58 --> 688.04]  And I thought, I would like to try Plasma 6 on my framework.
[688.38 --> 689.00]  Oh, look at that.
[689.06 --> 692.36]  There's one line in my config of services.plasma5.enable.
[692.36 --> 695.12]  I'm just going to rev that to say Plasma 6.
[695.56 --> 696.08]  Rebuild.
[696.80 --> 697.34]  Oh, wait.
[697.46 --> 697.62]  No.
[697.80 --> 700.92]  Services is a custom keyword within Nix configuration.
[701.74 --> 710.02]  And I need to now not only rebase my entire framework configuration off of Unstable and rebuild the whole thing,
[710.08 --> 718.64]  but I can't just do an overlay for one specific module without an awful lot of spelunking into the inner workings of how the modules system works.
[718.64 --> 723.68]  Little things like that are rough edges that we're making excuses for computers with by saying,
[723.84 --> 728.00]  oh, you just disabled a module and then you just import this and do that and do the other.
[728.66 --> 730.10]  Like, it's not straightforward.
[730.40 --> 732.60]  It should honestly just be.
[732.70 --> 737.70]  Like, the whole 2311 unstable versus, like, it's just confusing.
[737.70 --> 747.58]  And I'd love to get, particularly given the fact you've been doing so much packaging lately, get your take on that whole kind of Nix consumability thing.
[747.98 --> 749.76]  The learning curve is tough.
[750.52 --> 755.22]  I first tried to do it by just sitting down and, like, grizzing through it, basically.
[755.32 --> 756.04]  Like, I'm a developer.
[756.16 --> 757.46]  I'm like, how can it be?
[757.50 --> 758.06]  I'm a developer.
[758.26 --> 761.92]  I'm a long-term, long-term, you know, Linux user.
[762.06 --> 763.40]  I'm pretty comfortable with the command line.
[763.54 --> 765.98]  I'm, you know, feel like I've been there.
[766.04 --> 767.98]  And I sat down and I just didn't get it.
[767.98 --> 772.28]  And so the approach I took was to go back and say, like, okay, well, let's first understand the Nix language.
[772.40 --> 773.32]  Let's understand the syntax.
[773.44 --> 775.66]  So when I read something, I know what's actually going on.
[775.88 --> 779.30]  Then I sort of started to read a bit about, you know, how the store is structured.
[779.68 --> 782.10]  And I just sort of slowly built up like that.
[782.60 --> 783.42]  It is tough.
[783.64 --> 786.20]  And actually, I think, but I think packaging is tough.
[786.38 --> 793.04]  I mean, part of my role at Canonical is to look after Snapcraft, which is the tool for building snaps, right?
[793.08 --> 796.06]  And in fact, I package Snapcraft for Nix in a weird turn of events.
[796.06 --> 798.20]  But it's similar, right?
[798.26 --> 799.90]  Like people look at it and go, well, this is hard.
[800.32 --> 807.16]  And in reality, like we're building a whole set of patterns which translate across building containers and snaps and charms and all kinds of things.
[807.24 --> 807.82]  But it is hard.
[808.02 --> 813.10]  Like packaging, I think the craft, the setup of the crafts now is really, really elegant.
[813.28 --> 814.30]  You still have to learn it, right?
[814.32 --> 815.58]  It still has its idiosyncrasies.
[815.66 --> 820.96]  You're still talking about taking a package, compiling it potentially in some kind of weird prefix.
[821.06 --> 823.50]  You might have to patch the location of a bunch of libraries.
[823.50 --> 826.90]  You have to create something that's going to launch it and manage it.
[827.06 --> 829.00]  Like it is quite hard, right?
[830.28 --> 832.68]  I don't see them necessarily as comparable.
[832.90 --> 841.20]  But I remember going through the experience of learning how to write sort of more complicated snaps and feeling a similar feeling of like, okay, this is complicated.
[841.44 --> 845.34]  And it's the same if you actually try to build a dev package that ideas to Debian policy, right?
[845.38 --> 847.04]  Like that's a fine art.
[847.26 --> 848.00]  It's not just something.
[848.32 --> 851.76]  Not anyone can just yeet a dev together and get it accepted into Debian, right?
[851.76 --> 853.22]  It's just not that simple.
[854.24 --> 856.56]  I would say that's a feature, to be honest with you.
[856.64 --> 858.64]  Otherwise, the quality just wouldn't be there.
[859.12 --> 864.66]  I have spoken with individuals that would probably be familiar with people using Nix at scale.
[864.96 --> 868.44]  And they really are taking more of a Flake-based approach to managing software.
[868.58 --> 871.76]  They're not really dealing with the software channels or release channels.
[871.90 --> 874.74]  You know, they're really focused on just deploying software through Flakes.
[874.74 --> 879.26]  And I think that's something that Flakehub is also hoping to help manage.
[879.52 --> 887.24]  You know, one of the things that I've learned to appreciate is they have a shared namespace where you can actually set up ACLs and all of this stuff for people using it at scale.
[887.48 --> 889.58]  So that kind of stuff is being built out right now.
[889.94 --> 891.74]  You know, but I think your criticism is fair.
[892.44 --> 899.44]  You know, your example of like, you know, managing 10 or 50 different Postgres databases on different systems throughout the company where you got different departments and divisions.
[899.44 --> 902.48]  Like, it is really not quite there yet.
[902.58 --> 906.26]  And that's an area where existing products are really focused on for decades.
[907.02 --> 908.82]  But we already see the tooling getting built.
[909.12 --> 910.68]  Yeah, I think the potential is there, right?
[910.86 --> 922.92]  But, you know, and if you're a boutique software house with 10, 15, 20, you know, 100 super enthusiastic bright folks, I am absolutely certain you could make it work and build something we'd all be very envious of.
[923.20 --> 924.04]  Yeah, or a home lab.
[924.20 --> 928.18]  And I think is another or, you know, for us here at JB, we've got, you know, a dozen servers.
[928.18 --> 929.36]  What a great use case, right?
[929.40 --> 933.76]  You solve a whole bunch of niche stuff with Jack and Pipewire and never have to solve it again, right?
[933.82 --> 934.78]  Like, problem solved.
[935.18 --> 941.02]  The other thing to think about, like, if I think about it, you know, in my personal life, it's Nix all the way.
[941.10 --> 944.64]  In my work life, I clearly do the Ubuntu thing pretty often.
[945.38 --> 952.56]  If you think about it from like a supportability perspective and, you know, I have a lot of confidence in a lot of the folks who maintain Nix OS.
[952.56 --> 959.08]  Yes, I don't have a strong view of what the security story is, but, you know, I know how much of an effort that is at Canonical.
[959.18 --> 962.78]  Like, I know how much time and money and resource it takes to pull off what they pull off.
[963.46 --> 965.50]  And so, you know, I think it has the potential.
[965.64 --> 973.82]  I think the approach is super interesting, but it is like you've got to really want to know it before you're going to get competent at it, right?
[973.82 --> 983.38]  So speaking of, you know, taking things forward, I noticed that you packaged Scrutiny, the hard disk smart monitoring tool that we talked about.
[983.60 --> 984.62]  It was funny on Mastodon.
[984.72 --> 989.86]  You were like, in a recent episode of Self Hosted, and I messaged you back and said, yeah, that was like three years ago, dude.
[989.88 --> 991.56]  You definitely mentioned it in a recent show.
[991.64 --> 994.34]  It came back on my radar, maybe end of last year.
[994.38 --> 994.82]  I don't know.
[995.16 --> 995.56]  Probably.
[995.56 --> 1007.56]  I found this particular app pretty interesting, though, because it just so happened that that week as well, I'd gone through my first contribution to Nix packages doing a very basic Go app.
[1007.94 --> 1009.86]  Nothing quite on the scale of Scrutiny.
[1010.88 --> 1014.30]  Why don't you talk us through the process of contributing to Nix packages?
[1014.54 --> 1023.08]  Yeah, actually, this is one of the things that got me super hooked on Nix is the ability for people to show up and contribute and get reviews and actually become a contributor.
[1023.08 --> 1029.10]  Like, you can contribute to an operating system with relatively little experience with almost no barrier.
[1029.28 --> 1031.24]  One Git repository full of text files.
[1031.48 --> 1032.54]  You make a pull request.
[1032.66 --> 1033.34]  You ask some help.
[1033.44 --> 1035.64]  People will give you a bunch of reviews, and you can land it.
[1036.18 --> 1044.28]  And that really, for me, just captured me in terms of like, oh, wow, not only can I make all these local additions, I can actually get this stuff landed.
[1044.80 --> 1049.88]  So Scrutiny was about my third or fourth kind of package or module, some combination.
[1049.88 --> 1057.98]  It looks a little bit more complicated, but in reality, it's two Go binaries, one of which has a Node.js front end embedded into it.
[1058.02 --> 1058.70]  So it's two packages.
[1059.50 --> 1067.36]  The module system, you know, takes a bit of getting used to, but fundamentally, you give the user a set of options, and that generates a set of config.
[1067.44 --> 1070.84]  And the config is users, systemd units, that sort of thing.
[1070.84 --> 1074.90]  The thing that I love, one of the things I think is super powerful is the test framework.
[1075.30 --> 1076.46]  It's really, really interesting.
[1076.68 --> 1084.28]  Like, the tooling to spin up virtual machines with different configurations and assert against the state of that machine using something convenient like Python.
[1084.46 --> 1086.00]  I think it's super interesting.
[1086.16 --> 1090.60]  Like, that's a battle that traditional Linux operating systems have been fighting for many years.
[1090.70 --> 1094.66]  Like, how do you do integration testing of all of these packages and all of these configurations?
[1094.66 --> 1106.44]  And Nix is doing that with the test suite, and they're slowly getting to more and more coverage, and they can test some really complex kind of combinations of different things on a system because of it.
[1106.58 --> 1111.92]  Their GitHub Action sort of CI pipeline is absolute beast mode on that thing.
[1112.08 --> 1112.74]  Yeah, it's bonkers.
[1112.74 --> 1114.84]  You open a PR, and it's hours.
[1114.84 --> 1121.16]  I mean, the initial tests happen pretty fast, but, like, for the full test suite to run, it takes several hours.
[1121.90 --> 1129.20]  What I like about it is because of the kind of ethos of it and the fact that you can build it all from source and it's all reproduced to the like.
[1129.34 --> 1134.86]  To get that, like, if you want to run the integration test for scrutiny on your machine, you can do that.
[1135.02 --> 1136.00]  Like, super simple.
[1136.10 --> 1136.84]  One command, right?
[1136.92 --> 1140.54]  Like, Git clone, build the Nexus test for scrutiny, and you're away.
[1140.54 --> 1146.54]  And that, to me, again, was something that really captured me was this – it felt so hackable.
[1146.70 --> 1149.94]  It's like, okay, there's loads of them, but it's still just a pile of text files, right?
[1150.90 --> 1156.54]  I think, for me, the one that got me was the Build Go module sort of wrapper, like a helper.
[1157.18 --> 1158.56]  I don't know what to call it, really.
[1158.98 --> 1169.20]  I don't know much about building Go applications, and the app that I picked to package was figurine, just like a little – it's like a message of the day, like, just print out text, colourful, written in Go.
[1169.20 --> 1170.00]  Nothing too clever.
[1170.00 --> 1175.94]  So that's certainly not as good as scrutiny with, you know, a database and all that kind of stuff underneath and a collector and all the rest of it.
[1176.40 --> 1183.88]  But I noticed that you use Build Go module in your build as well, and I wondered if there are any tips, tricks, anything like that?
[1184.28 --> 1186.98]  I think the tips and tricks are – and I learned a few of them on the way through.
[1187.10 --> 1193.24]  Like, part of the reason I publicized it was because of – I think it highlights what an opportunity it is to learn by going through the process, right?
[1193.24 --> 1196.82]  I think the helpers in Nix are really great.
[1196.90 --> 1199.08]  You've got the kind of cargo package one, the Go module.
[1199.26 --> 1200.90]  There's ones for building node packages.
[1201.38 --> 1208.40]  And what I would try – what I would probably say is, like, wherever possible, stick to the kind of supported way through.
[1208.40 --> 1212.70]  Like, it'll have a predefined patch phase, build phase, install phase, check phase.
[1212.98 --> 1214.08]  And you can override them.
[1214.14 --> 1217.08]  You'll see various people saying, you know, defining their own install phase.
[1217.58 --> 1218.80]  I've done that a bunch of times.
[1218.88 --> 1220.60]  I did it on scrutiny the first time around.
[1220.60 --> 1230.04]  And then kind of, as I went through and read the docs more and more deeply, started to understand that a lot of it was already catered for, and I didn't need to kind of do that overriding.
[1230.68 --> 1236.72]  So I would say, yeah, the docs are a little terse at times, I think it's safe to say.
[1237.12 --> 1237.46]  Safe to say.
[1237.66 --> 1241.02]  But I also – one of the tricks I do is I just do lots of searching.
[1241.54 --> 1244.16]  So, for example, GitHub's new code search I find pretty handy.
[1244.16 --> 1252.84]  So you browse to the Nix packages repository, like hit the forward slash key, and type build go module, and just take a look at 10, 15 examples and see how other people have solved the same problems.
[1252.98 --> 1258.48]  With, you know, 80-something thousand packages, you're unlikely to be the first person with that problem is kind of how I look at it.
[1258.84 --> 1260.86]  Unless, as it turns out, you want to run image.
[1260.94 --> 1261.76]  I was looking the other day.
[1261.84 --> 1264.14]  You know, the self-hosted photo backup image.
[1264.86 --> 1270.46]  Apparently, there's a whole bunch of upstream dependencies for that particular application, which aren't yet in Nix.
[1270.68 --> 1272.20]  And there's a whole thread about it.
[1272.20 --> 1277.54]  I'll put a link to that and all of John's blog posts in the show notes.
[1277.68 --> 1280.48]  I wrote one as well about my adventures packaging for Nix.
[1281.30 --> 1288.30]  We'll also put a link in the show notes to an hour-long chat that I saw John had with Victor Peterson over on YouTube,
[1288.30 --> 1296.40]  talking about a lot more of the intricacies of Nix and the sort of general ethos about, you know, why Ubuntu guy is using Nix in the first place.
[1296.40 --> 1307.50]  And it also struck me during that interview that even the Linux guys, the guys building Canonical software and, dare I say, Linux, you know, tools for people,
[1307.82 --> 1310.28]  even they're starting to get sucked into the Nix vortex.
[1311.24 --> 1311.36]  Yeah.
[1311.58 --> 1313.20]  So, Victor, I met through Canonical.
[1313.74 --> 1317.42]  Victor runs a company called Screenly, which is a digital signage company.
[1317.56 --> 1318.24]  Super interesting.
[1318.34 --> 1319.60]  All runs on Ubuntu Core.
[1319.60 --> 1321.54]  And I did this episode with him.
[1321.62 --> 1323.42]  He's been interested in Nix for a little while.
[1323.50 --> 1328.18]  And I did the episode to kind of having just packaged their CLI tool for the Nix packages.
[1328.32 --> 1329.10]  He was interested in that.
[1329.20 --> 1330.54]  And so it's exactly that.
[1330.60 --> 1336.42]  It's a deep dive into what Nix is as a language, as a package manager, and as an operating system.
[1336.58 --> 1340.40]  And then a bit of some questions on reproducibility and how it can be used.
[1340.40 --> 1347.20]  One thing it does highlight, though, which is really interesting, is you guys will definitely be familiar with Ubuntu Core, our immutable offering.
[1347.76 --> 1357.84]  And one of the really interesting things about the immutable distro scene at the moment is nearly all of them rely upon some kind of file system fanciness for immutability.
[1358.18 --> 1360.04]  Butter Affair, some kind of AB route.
[1360.76 --> 1363.18]  Ubuntu Core and Nix are the two closest going.
[1363.84 --> 1369.68]  If you think about the way they work, right, like they literally just swap out a kernel and it points a different path to the system, a different revision of the snap.
[1369.68 --> 1372.82]  It's actually there's a surprising amount of similarity.
[1373.00 --> 1380.46]  I wouldn't call them the same, but it's interesting how similar they are by comparison to something like Silverblue, for example.
[1380.88 --> 1381.66]  That's a great point.
[1381.86 --> 1386.42]  That is I had not I think I was getting to that conclusion, but I hadn't put it all together.
[1386.82 --> 1388.08]  That is a very good point.
[1388.28 --> 1390.28]  Well, John, thank you so much for joining us.
[1390.40 --> 1392.36]  It was a great chat and keep up the great work.
[1392.36 --> 1396.98]  Tailscale.com slash self-hosted.
[1397.04 --> 1403.00]  Head on over there, support the show and get 100 devices for free when you go to Tailscale.com slash self-hosted.
[1404.06 --> 1409.94]  Tailscale is the easiest way to connect your devices and services to each other directly wherever they are.
[1410.06 --> 1415.24]  Secure remote access to production, database servers, your Kubernetes cluster, whatever it might be.
[1415.24 --> 1417.22]  And it's really fast.
[1417.68 --> 1421.92]  Build your own flat mesh noise protected network.
[1422.02 --> 1424.88]  Yeah, that's the WireGuard protocol using Tailscale.
[1425.18 --> 1427.74]  I use Tailscale to bridge everything together.
[1428.72 --> 1431.02]  My systems are behind double carrier grade net.
[1431.46 --> 1433.72]  And that has always proved to be very, very challenging.
[1434.18 --> 1436.54]  And so I've had to use third party services here and there.
[1436.58 --> 1440.96]  And I ended up with like a mix and match of inbound ports and different VPN services.
[1442.26 --> 1443.98]  Tailscale let me unify all of it.
[1443.98 --> 1450.48]  I built out a simple network at first and then have layered on top of that ACLs and additional services over time.
[1450.96 --> 1452.94]  And it's a new way for me to do networking.
[1453.14 --> 1453.92]  It's intuitive.
[1454.08 --> 1454.70]  It's programmable.
[1454.78 --> 1458.36]  And I've created my own flat mesh network.
[1458.60 --> 1462.16]  Just as an example, if you're an iOS user, you can integrate shortcuts.
[1462.36 --> 1464.18]  So I have a shortcut on my wife's iPhone.
[1464.34 --> 1469.08]  When she plugs in her iPhone, it just launches and makes sure Tailscale is connected.
[1469.40 --> 1473.76]  That's really handy because then I can also have other things like her photo start backing up at that point.
[1473.76 --> 1475.12]  Over the Tailscale connection.
[1475.76 --> 1480.38]  On Android devices, I've tied it in with NFC connections to make sure Tailscale is connected.
[1480.68 --> 1484.68]  And then in Home Assistant, run a script that turns the thermostat on at the office.
[1484.78 --> 1489.38]  So right as I'm leaving home, I scan that NFC tag and it turns the heater on.
[1489.48 --> 1493.76]  So by the time I arrive at my office, I have a decent temperature.
[1494.32 --> 1499.16]  The other thing that I'll use quite frequently is I'll start a project inside a VM or on a VPS.
[1500.04 --> 1504.52]  And then I'll want to move to a different system or maybe I'll want to go home and I want to have access to that VM.
[1505.18 --> 1506.66]  I just put Tailscale in that VM.
[1507.26 --> 1510.36]  And I can work on it if I'm there at the physical studio or not.
[1510.72 --> 1511.80]  And this is way out there.
[1511.80 --> 1518.74]  But one thing that I've been doing recently that I just have to tell you guys about is I put the Sunshine server on my Linux desktop here at the studio.
[1518.74 --> 1521.90]  That lets you do streaming using the Steam Link protocol.
[1522.32 --> 1525.32]  And I run the Sunshine client on my Oculus VR headset.
[1525.32 --> 1529.22]  So I connect Tailscale, which also runs on my Oculus VR headset.
[1529.48 --> 1531.00]  Yep, I sideloaded the APK.
[1531.54 --> 1542.10]  And then I can stream my GNOME Linux desktop inside my Oculus headset on a giant 110-inch screen using moonlight and sunlight over Tailscale.
[1543.04 --> 1549.00]  I know that's a big lot of jumble words, but people that know what I'm talking about, I think maybe they can appreciate how awesome this is.
[1549.00 --> 1563.12]  Because then I can pull up that Linux desktop on any machine, my iPad, my other desktops, anything I have connected to my Tailnet now has a very performant, because it's designed for game streaming, on-demand streaming Linux desktop.
[1563.54 --> 1568.90]  If I'm on the Mac that day and I need to get to something on Linux, I just pull up Moonlight on the Mac and I connect over Tailscale.
[1569.38 --> 1571.66]  And I'm streaming my GNOME desktop running Nix OS.
[1571.66 --> 1581.06]  I'm just telling you, you can build such powerful combinations of things that you don't even realize the power of it before you get started.
[1581.52 --> 1591.02]  And for businesses, it can streamline your remote access, and you can integrate it with your existing authentication infrastructure, your two-factor, your access and controls.
[1591.38 --> 1598.78]  But more importantly, you don't have to have some wild, huge VPN system that costs you who knows how much.
[1598.78 --> 1601.34]  I mean, I have seen the different hardware boxes.
[1601.80 --> 1603.70]  I have seen different licensing schemes.
[1604.58 --> 1620.60]  Enterprises have needed to address this for a long time, and Tailscale does it in a way that uses your ACL policies so you can make sure everything is secured the way you already have it and replace your legacy VPN infrastructure in just minutes, at least on the client end.
[1620.64 --> 1623.24]  You can get it installed on any OS in just minutes.
[1623.56 --> 1626.84]  I can't account for how long the bureaucracy will take you, but it'll be worth it.
[1626.84 --> 1627.98]  Go try it, you guys.
[1628.06 --> 1628.56]  I love it.
[1629.06 --> 1631.16]  Tailscale.com slash self-hosted.
[1631.22 --> 1632.96]  Try it for 100 devices for free.
[1633.02 --> 1633.92]  Just see what I'm talking about.
[1634.42 --> 1635.52]  Put your mobile devices in there.
[1635.56 --> 1636.86]  Put a couple of containers in there.
[1637.28 --> 1640.62]  Put a VPS and a desktop or two in there, and start working the magic.
[1640.82 --> 1642.96]  Tailscale.com slash self-hosted.
[1645.12 --> 1647.66]  Been busy on the old YouTubes the last couple of weeks.
[1647.70 --> 1650.10]  A couple of videos that folks have been...
[1650.92 --> 1655.14]  I always wonder when people are like, oh, I've had loads of people ask me about this.
[1655.20 --> 1656.58]  Like, how many people is loads?
[1656.58 --> 1660.40]  I had probably a dozen people saying, when are you going to get to this server build, Alex?
[1661.04 --> 1661.80]  You know.
[1661.92 --> 1664.42]  So for me, I've had a few people asking about it.
[1664.62 --> 1667.96]  And I have built myself the Epic...
[1667.96 --> 1670.12]  I feel like I want to be in Sparta right now.
[1670.22 --> 1671.40]  This is Epic.
[1671.56 --> 1672.22]  This is Sparta.
[1673.34 --> 1676.18]  Epic Rome home server.
[1676.18 --> 1681.52]  The specs on this thing are, frankly, kind of bonkers.
[1682.36 --> 1685.00]  It's an AMD Epic 7402 CPU.
[1685.74 --> 1686.66]  24 cores.
[1687.14 --> 1688.08]  48 threads.
[1689.54 --> 1691.58]  256 gigs of ECC memory.
[1692.24 --> 1696.16]  Coupled with, goodness knows how many NVMe SSDs.
[1696.18 --> 1698.62]  A couple of U.2 NVMe drives as well.
[1699.16 --> 1700.24]  A couple of graphics cards.
[1700.24 --> 1707.96]  I had a listener actually sell me their Arc Pro A40 single slot OEM only graphics card.
[1708.02 --> 1710.24]  So I can actually do quick sync on this thing as well.
[1710.84 --> 1711.28]  Slick.
[1711.44 --> 1711.70]  Git.
[1711.82 --> 1712.52]  That's perfect.
[1713.12 --> 1713.40]  Well, yeah.
[1713.40 --> 1714.78]  My currency now with this motherboard.
[1715.00 --> 1715.38]  Because, okay.
[1715.42 --> 1716.44]  Let me set the scene.
[1716.62 --> 1716.76]  Okay.
[1716.76 --> 1722.60]  So, for the last few years, my media server has been an i5-8500 based system.
[1722.72 --> 1730.54]  And I've actually kind of been proud that my main server CPU is from like 2019, 2018.
[1730.86 --> 1733.14]  It's a fairly old boy, right?
[1734.02 --> 1735.98]  But it doesn't have very many PCIe lanes.
[1736.10 --> 1739.66]  And about a year ago, when I upgraded all of my home networking to 10 gig,
[1739.66 --> 1743.96]  I really started to feel that problem quite acutely on that box.
[1744.06 --> 1749.84]  Because that motherboard that I have in the i5 system is an ASRock rack motherboard,
[1749.92 --> 1751.24]  which I've talked about in the show before.
[1751.46 --> 1753.34]  There's a link on my blog, which will be in the link,
[1753.60 --> 1755.30]  which will be in the show notes down below too.
[1755.98 --> 1761.98]  But the issue with that CPU is Intel consumer CPUs don't expose very many PCIe lanes.
[1762.22 --> 1764.42]  The CPU itself gets, I think, 16.
[1764.68 --> 1767.26]  And then the chipset gets another 20 or so.
[1767.26 --> 1771.26]  And by the time you've taken care of things like the IPMI,
[1771.94 --> 1774.42]  the built-in BMC chip having some PCIe lanes,
[1774.52 --> 1777.64]  and then the SATA controller, and then the onboard NICs,
[1777.66 --> 1778.36]  and that kind of stuff,
[1778.60 --> 1782.34]  it doesn't leave a huge number of lanes left for actual peripherals,
[1782.54 --> 1785.46]  like an SFP plus 10 gig networking card.
[1786.36 --> 1789.08]  And so what happens is to kind of work around that,
[1789.28 --> 1792.74]  ASRock rack put inside the motherboard PCIe switches.
[1792.74 --> 1799.08]  And so when you put a 16x card into your 16x slot,
[1799.74 --> 1803.62]  and you also put another card into the third slot on that motherboard,
[1804.42 --> 1805.82]  the PCIe switch engages,
[1806.28 --> 1810.04]  and suddenly your 16x slot becomes two eight slots.
[1810.30 --> 1813.38]  And so you can only run an 8x PCIe card in there,
[1814.04 --> 1815.24]  which doesn't sound too bad,
[1815.30 --> 1819.08]  except I was trying to run one of those fancy M.2 cards
[1819.08 --> 1823.30]  that splits four M.2 devices across a single slot using bifurcation.
[1823.74 --> 1824.24]  Of course.
[1825.08 --> 1827.88]  And so, you know, I've limped along for the last year,
[1828.32 --> 1831.50]  poor old Alex, with a single NVMe drive
[1831.50 --> 1834.78]  for my download unpacking.
[1834.92 --> 1837.54]  That's what I end up having to need the most IOPS for,
[1837.58 --> 1839.30]  is when I'm downloading stuff at gigabit speed,
[1839.86 --> 1841.04]  unpacking all those files.
[1841.16 --> 1843.10]  Like, it's pretty tough on the disk, actually.
[1843.70 --> 1845.90]  And so I've limped along for a year with that being the case.
[1845.90 --> 1848.94]  But finally, with this Epic system, I've gone up from,
[1849.06 --> 1851.00]  what was that, 16 plus 20 lanes,
[1851.10 --> 1856.48]  I've gone up to 128 PCIe lanes directly into the CPU.
[1857.02 --> 1860.32]  No chipsets, no Northbridge, Southbridge nonsense,
[1860.66 --> 1866.18]  just 128 direct wired PCIe Gen 4 lanes, no less.
[1866.68 --> 1868.06]  So I've got bandwidth for days.
[1868.16 --> 1869.84]  I've got PCIe slots for days.
[1869.92 --> 1871.00]  I've got on this new motherboard,
[1871.58 --> 1875.02]  it's a Supermicro H12 SSL-I motherboard.
[1875.02 --> 1881.52]  I've got five 16x PCIe slots and two 8x PCIe slots.
[1881.72 --> 1886.78]  On top of that, there are a pair of M.2 NVMe slots
[1886.78 --> 1888.04]  on the motherboard itself,
[1888.36 --> 1891.82]  each of which have four PCIe lanes to boot as well.
[1892.72 --> 1895.74]  And it's got a built-in LSI SAS controller
[1895.74 --> 1898.10]  built directly into the motherboard as well.
[1898.20 --> 1901.26]  Like, it's just completely bonkers and overkill
[1901.26 --> 1903.14]  in all the best kinds of ways.
[1903.14 --> 1905.32]  In all the ways you need and want, right?
[1907.10 --> 1910.02]  And what about noise, you know, these types of things?
[1910.10 --> 1911.64]  Like, you know, the quality of life things.
[1911.90 --> 1912.70]  That's not too bad.
[1912.78 --> 1915.52]  I mean, so Sligar are a case manufacturer
[1915.52 --> 1918.52]  that saw my HomeLab 15 review
[1918.52 --> 1921.16]  and were kind enough to send me over another case.
[1921.22 --> 1923.50]  So I've now got three home server cases in the house.
[1923.64 --> 1925.64]  This is actually quite a nice unit, the CX4712.
[1925.64 --> 1929.90]  It takes 10 3.5-inch spinning hard drives.
[1930.06 --> 1934.60]  And it's also got a pair of 5.25-inch drive bays in the front as well.
[1934.82 --> 1939.82]  So I bought a 6-in-1, 2.5-inch SSD slot-loading,
[1939.82 --> 1943.20]  you know, tray-based system, hot swap system,
[1943.20 --> 1946.30]  to go in the front of my Sligar case.
[1946.40 --> 1949.36]  So I've got room for, well, potentially 12 SSDs.
[1949.36 --> 1952.06]  I'm only using three or four of them right now.
[1952.20 --> 1955.34]  But I'm only using three or four of them right now.
[1955.56 --> 1956.40]  But, you know, it's...
[1956.40 --> 1957.50]  You've got some room to grow.
[1958.16 --> 1959.02]  Exactly, exactly.
[1959.28 --> 1962.54]  And that really was the motivation for this entire build,
[1962.66 --> 1963.46]  to be honest with you.
[1964.00 --> 1967.92]  I've been doing a lot more virtualization for work lately.
[1968.18 --> 1971.44]  You know, I'm trying to build out entire demo environments
[1971.44 --> 1975.18]  for YouTube videos where I've got three or four machines
[1975.18 --> 1976.88]  on a separate VLAN for one video
[1976.88 --> 1978.16]  and the same for another video.
[1978.16 --> 1980.94]  And, like, I'm building out these complete fake environments
[1980.94 --> 1982.70]  as if you're building real infrastructure.
[1983.16 --> 1985.30]  Like, I'm building out a whole server over here
[1985.30 --> 1986.52]  and then a desktop over there
[1986.52 --> 1989.06]  and a little CADdy reverse proxy over here.
[1989.14 --> 1992.06]  And, like, running out of PCIe lanes is one thing,
[1992.14 --> 1994.16]  but running out of RAM is another.
[1994.32 --> 1997.82]  Like, the i5 can only really support about 64 gigs of memory.
[1997.92 --> 2000.44]  I mean, some people put 128 in there,
[2000.52 --> 2002.54]  but it's not the most stable in my experience.
[2002.62 --> 2003.90]  So I kind of stuck at 64.
[2005.02 --> 2007.38]  This new build, 256 gigs.
[2007.38 --> 2010.06]  I've got RAM to last me for days,
[2010.06 --> 2013.86]  and if I wanted to, I could double it to 512 with no problem.
[2014.24 --> 2014.36]  Wow.
[2014.66 --> 2018.18]  Well, I look forward to buying that from you used after a few years.
[2019.28 --> 2021.04]  Well, yeah, speaking of buying it,
[2021.16 --> 2023.30]  the price is something that's worth talking about
[2023.30 --> 2023.78]  because...
[2023.78 --> 2024.18]  Oh, yeah, sure.
[2024.52 --> 2028.54]  ...brand new, these things were just out of the reach
[2028.54 --> 2030.40]  of most home labbers, to be honest with you.
[2030.40 --> 2032.48]  But, you know, if you start looking at the fact
[2032.48 --> 2034.76]  of what this system can do for me,
[2034.86 --> 2037.90]  and I'm replacing three or four systems in this house
[2037.90 --> 2039.28]  with just one box,
[2039.78 --> 2041.56]  it makes the price a little bit easier to swallow.
[2042.00 --> 2043.40]  I'm sort of dancing around it here
[2043.40 --> 2044.24]  because it's a big number.
[2044.56 --> 2047.40]  It was $1,750 for the motherboard,
[2047.74 --> 2049.38]  the CPU, the RAM,
[2049.38 --> 2051.00]  and a CPU cooler as well.
[2051.44 --> 2052.24]  Not including disk, then?
[2052.54 --> 2053.18]  No disks.
[2053.38 --> 2054.74]  Not including disks because,
[2055.76 --> 2057.66]  well, I frankly don't want to add up
[2057.66 --> 2059.82]  how much I've spent on hard drives over the years.
[2061.12 --> 2062.46]  And the Sligar case,
[2062.54 --> 2063.40]  if I had purchased that,
[2063.44 --> 2064.38]  would have been another $400.
[2064.84 --> 2066.28]  So very quickly,
[2066.60 --> 2069.50]  you're sort of adding up to well over $2,000.
[2070.02 --> 2071.56]  So you'd want to build this for something
[2071.56 --> 2074.26]  that could last four or five years,
[2074.32 --> 2075.52]  at least, maybe more.
[2075.84 --> 2076.10]  Yeah.
[2076.40 --> 2078.32]  And that's kind of the interesting thing for me.
[2078.32 --> 2081.56]  If you compare this build and this case
[2081.56 --> 2084.18]  directly to the HomeLab 15,
[2084.74 --> 2088.54]  and their price tag of $2,000,
[2088.76 --> 2090.36]  give or take, for the full build.
[2090.50 --> 2092.90]  I'm going to just say that they're both about $2,000
[2092.90 --> 2094.74]  because prices fluctuate,
[2094.78 --> 2095.52]  all that kind of stuff.
[2096.32 --> 2098.64]  What's interesting is that the HL15
[2098.64 --> 2099.86]  was a brand new build.
[2099.94 --> 2100.78]  So brand new parts,
[2100.96 --> 2102.00]  brand new Super Micro motherboard,
[2102.30 --> 2104.12]  so you get warranty.
[2104.76 --> 2106.10]  The parts that I purchased,
[2106.22 --> 2106.96]  the Epic parts,
[2106.96 --> 2109.24]  were from a Chinese eBay seller
[2109.24 --> 2111.96]  called TUGM something or other.
[2112.10 --> 2114.24]  There'll be a link to my YouTube video
[2114.24 --> 2116.30]  in which there's a link in the description
[2116.30 --> 2118.22]  to all of the components
[2118.22 --> 2119.14]  and all the rest of it
[2119.14 --> 2121.68]  for you to have a browse for.
[2122.22 --> 2122.66]  So, you know,
[2122.68 --> 2124.82]  it's not quite a direct comparison,
[2125.00 --> 2125.16]  you know,
[2125.20 --> 2126.46]  comparing a brand new product
[2126.46 --> 2127.52]  to used,
[2127.66 --> 2128.36]  you know,
[2128.42 --> 2129.20]  enterprise gear.
[2129.20 --> 2131.28]  But the reality is,
[2131.72 --> 2133.44]  one of the things we do in HomeLab world,
[2133.54 --> 2134.70]  the best, I think,
[2134.74 --> 2137.58]  is actually give these old servers
[2137.58 --> 2139.16]  a new lease of life.
[2139.54 --> 2142.38]  And is it the most responsible thing in the world
[2142.38 --> 2144.38]  to buy a brand new system?
[2144.52 --> 2146.70]  Particularly with the 45 dryer system,
[2146.88 --> 2148.52]  when the Xeon they send out with it,
[2148.56 --> 2149.62]  the 6-core Xeon is,
[2149.62 --> 2152.34]  it's kind of slow
[2152.34 --> 2153.26]  and not,
[2153.54 --> 2153.76]  you know,
[2153.76 --> 2154.98]  not the best CPU.
[2155.16 --> 2155.26]  I mean,
[2155.32 --> 2155.52]  yes,
[2155.54 --> 2156.30]  you can upgrade it,
[2156.34 --> 2157.46]  but that's extra cost.
[2157.60 --> 2157.66]  That's,
[2157.78 --> 2158.04]  you know.
[2158.52 --> 2160.64]  So I look at the two servers
[2160.64 --> 2160.98]  at,
[2161.04 --> 2161.22]  you know,
[2161.28 --> 2162.94]  the $2,000 price point
[2162.94 --> 2163.24]  and,
[2163.34 --> 2164.06]  well,
[2164.16 --> 2165.06]  there's no comparison.
[2165.56 --> 2165.62]  Yeah,
[2165.64 --> 2167.02]  and I wonder if the audience feels like
[2167.02 --> 2167.60]  $2,000
[2167.60 --> 2168.94]  is too much
[2168.94 --> 2170.28]  for a HomeLab box.
[2170.62 --> 2170.76]  I mean,
[2170.90 --> 2171.22]  I grant,
[2171.34 --> 2171.84]  not everybody,
[2172.08 --> 2172.54]  but I wonder,
[2173.54 --> 2174.48]  as you look at
[2174.48 --> 2176.08]  trying to build something
[2176.08 --> 2177.22]  that would last you
[2177.22 --> 2178.54]  two to four to five years,
[2178.54 --> 2180.26]  and I look at my storage consumption rate
[2180.26 --> 2181.30]  and I look at
[2181.30 --> 2183.42]  all of the applications I want,
[2183.48 --> 2184.40]  like I want to get Frigate
[2184.40 --> 2185.36]  going in the future,
[2185.56 --> 2187.68]  I want to get more local AI running,
[2188.26 --> 2190.06]  both for myself at home.
[2190.94 --> 2191.78]  My wife likes it
[2191.78 --> 2193.18]  for asking gardening questions
[2193.18 --> 2194.64]  and I want it here
[2194.64 --> 2196.74]  for summarizing JB show notes
[2196.74 --> 2197.28]  and chapters
[2197.28 --> 2198.90]  so we can inevitably
[2198.90 --> 2199.88]  have some sort of system
[2199.88 --> 2201.00]  where internally we can say,
[2201.14 --> 2202.04]  what show
[2202.04 --> 2203.94]  did Alex and I talk about
[2203.94 --> 2204.92]  his Epic server build?
[2205.12 --> 2205.38]  And,
[2205.46 --> 2205.54]  you know,
[2205.56 --> 2206.44]  you just query the system
[2206.44 --> 2207.28]  and it can tell us that.
[2207.52 --> 2207.54]  And,
[2207.54 --> 2208.76]  I want to experiment
[2208.76 --> 2209.54]  with those things
[2209.54 --> 2210.24]  internally
[2210.24 --> 2210.70]  and I just,
[2210.78 --> 2211.50]  all of these things
[2211.50 --> 2212.08]  are adding
[2212.08 --> 2213.76]  cost pressure
[2213.76 --> 2215.12]  and resource pressure
[2215.12 --> 2216.30]  and I feel like
[2216.30 --> 2217.86]  maybe $2,000
[2217.86 --> 2218.64]  these days,
[2219.90 --> 2221.14]  assuming one can afford it,
[2221.22 --> 2222.26]  is not unreasonable
[2222.26 --> 2223.80]  for a performance server
[2223.80 --> 2224.86]  that will have runway
[2224.86 --> 2227.00]  for multiple years.
[2227.62 --> 2227.86]  I mean,
[2227.88 --> 2228.26]  you're talking,
[2228.36 --> 2229.06]  you've got a system here
[2229.06 --> 2229.92]  where you can put in
[2229.92 --> 2231.02]  a lot more drives,
[2231.18 --> 2231.46]  you can,
[2231.54 --> 2232.12]  you've got,
[2232.58 --> 2233.52]  you can offload
[2233.52 --> 2234.14]  some of the tasks
[2234.14 --> 2235.06]  to that Arc card,
[2235.16 --> 2236.14]  which is phenomenal.
[2236.14 --> 2236.58]  Yeah.
[2237.20 --> 2237.42]  I mean,
[2237.52 --> 2238.64]  that's a system
[2238.64 --> 2239.10]  that's going to be
[2239.10 --> 2240.28]  hard to beat
[2240.28 --> 2241.44]  for a couple of years
[2241.44 --> 2241.96]  minimum
[2241.96 --> 2243.22]  and it's still going to
[2243.22 --> 2243.98]  work great for years
[2243.98 --> 2244.48]  after that.
[2244.56 --> 2245.06]  So I wonder,
[2245.24 --> 2245.88]  just my question is
[2245.88 --> 2246.48]  to the audience,
[2247.10 --> 2247.88]  boost in or go to
[2247.88 --> 2248.78]  the contact page,
[2249.48 --> 2250.88]  what is your price point
[2250.88 --> 2251.84]  for a Homelab server?
[2252.00 --> 2252.68]  I don't think we've ever
[2252.68 --> 2253.28]  asked the audience,
[2253.52 --> 2255.54]  I know it's not exactly
[2255.54 --> 2256.52]  something people like
[2256.52 --> 2256.94]  to talk about,
[2257.04 --> 2258.02]  but I'm really curious
[2258.02 --> 2259.12]  because I think I'm,
[2259.32 --> 2259.76]  not that I could
[2259.76 --> 2260.70]  necessarily buy it right now
[2260.70 --> 2261.26]  and pull the trigger,
[2261.86 --> 2262.68]  but I think I'm in the
[2262.68 --> 2263.76]  camp of $2,000
[2263.76 --> 2264.76]  for something that
[2264.76 --> 2265.56]  could have a lot of storage
[2265.56 --> 2266.46]  and some performance
[2266.46 --> 2267.20]  is pretty reasonable
[2267.20 --> 2267.72]  these days.
[2268.14 --> 2268.34]  I mean,
[2268.36 --> 2268.96]  if you look at it,
[2269.06 --> 2270.08]  the big advancement
[2270.08 --> 2271.70]  between the two systems,
[2271.80 --> 2273.08]  my old i5 system
[2273.08 --> 2274.28]  and this one
[2274.28 --> 2275.98]  is it's consumer grade
[2275.98 --> 2278.24]  versus server grade stuff.
[2278.72 --> 2278.94]  Right.
[2279.12 --> 2280.30]  The currency that I now
[2280.30 --> 2280.94]  deal in
[2280.94 --> 2282.80]  is PCIe slots
[2282.80 --> 2284.20]  rather than
[2284.20 --> 2285.62]  PCIe lanes
[2285.62 --> 2286.30]  and just,
[2286.62 --> 2286.84]  you know,
[2286.84 --> 2288.24]  I've got seven
[2288.24 --> 2289.76]  single slot cards
[2289.76 --> 2290.46]  I could essentially
[2290.46 --> 2291.48]  fit into that system.
[2291.48 --> 2292.84]  So if you were,
[2292.96 --> 2293.24]  for example,
[2293.24 --> 2293.90]  to take a look
[2293.90 --> 2296.36]  at the NVIDIA ATX A4000,
[2296.60 --> 2297.78]  RTX A4000,
[2297.88 --> 2298.06]  sorry,
[2298.72 --> 2299.94]  that is a single slot
[2299.94 --> 2300.68]  PCIe card
[2300.68 --> 2301.68]  that takes a single
[2301.68 --> 2302.92]  six pin power cable.
[2303.08 --> 2304.06]  So it's roughly
[2304.06 --> 2305.04]  150 watts
[2305.04 --> 2307.02]  plus the 75-ish
[2307.02 --> 2307.52]  it pulls from
[2307.52 --> 2308.36]  the socket itself.
[2309.22 --> 2309.94]  And I could essentially
[2309.94 --> 2310.98]  have five of those
[2310.98 --> 2311.72]  things in this box.
[2312.04 --> 2312.40]  First of all,
[2312.44 --> 2313.00]  that's a lot of heat
[2313.00 --> 2313.46]  to deal with,
[2313.48 --> 2314.24]  but that's a separate
[2314.24 --> 2314.64]  problem.
[2315.20 --> 2315.66]  But, you know,
[2315.72 --> 2316.54]  rather than buying
[2316.54 --> 2317.64]  a 3080 or something
[2317.64 --> 2318.16]  like that,
[2318.22 --> 2319.60]  that's got a two
[2319.60 --> 2320.48]  or a two and a half
[2320.48 --> 2321.30]  slot cooler,
[2321.48 --> 2322.78]  it's much more
[2322.78 --> 2323.44]  cost effective
[2323.44 --> 2324.90]  for doing these
[2324.90 --> 2325.50]  sort of machine
[2325.50 --> 2326.72]  learning AI type
[2326.72 --> 2327.22]  workloads.
[2327.22 --> 2328.36]  And I will be
[2328.36 --> 2329.38]  experimenting with
[2329.38 --> 2330.36]  Ollama over the
[2330.36 --> 2330.90]  coming weeks,
[2331.38 --> 2332.02]  in particular,
[2332.30 --> 2332.68]  locally,
[2332.68 --> 2333.50]  with a lot of this
[2333.50 --> 2334.82]  self-hosted LLM
[2334.82 --> 2335.16]  stuff,
[2335.80 --> 2337.24]  using an A4000,
[2337.32 --> 2337.78]  which I've got in
[2337.78 --> 2338.58]  the system as well.
[2339.24 --> 2339.64]  And it's,
[2339.72 --> 2339.94]  you know,
[2339.98 --> 2340.82]  it's fascinating,
[2340.82 --> 2341.42]  like you say,
[2341.54 --> 2341.76]  like,
[2342.70 --> 2343.60]  there's so much
[2343.60 --> 2344.56]  happening in the
[2344.56 --> 2345.70]  AI space at the
[2345.70 --> 2346.24]  moment that it
[2346.24 --> 2347.06]  almost behooves you
[2347.06 --> 2348.94]  to have a card
[2348.94 --> 2350.02]  like that in a
[2350.02 --> 2350.66]  system that you
[2350.66 --> 2351.34]  can have access
[2351.34 --> 2351.74]  to.
[2351.88 --> 2352.76]  Because I tried to
[2352.76 --> 2353.40]  run some of these
[2353.40 --> 2354.44]  models just CPU
[2354.44 --> 2355.06]  only.
[2355.52 --> 2356.38]  And then I threw
[2356.38 --> 2357.28]  it on the
[2357.28 --> 2358.64]  NVIDIA card and I
[2358.64 --> 2358.80]  went,
[2359.50 --> 2360.04]  oh,
[2360.60 --> 2361.52]  I see now.
[2362.10 --> 2362.96]  The other reality
[2362.96 --> 2364.82]  of the distribution
[2364.82 --> 2365.92]  of these AI
[2365.92 --> 2366.72]  projects right now
[2366.72 --> 2367.32]  is most of the
[2367.32 --> 2367.62]  time they're
[2367.62 --> 2369.08]  distributed as a
[2369.08 --> 2369.46]  container,
[2369.98 --> 2370.70]  sometimes as a
[2370.70 --> 2371.30]  setup script,
[2371.40 --> 2372.64]  and they expect a
[2372.64 --> 2373.34]  video card.
[2374.14 --> 2375.56]  And I'm always
[2375.56 --> 2376.34]  doing the math,
[2376.42 --> 2376.52]  like,
[2376.56 --> 2377.06]  should I do this
[2377.06 --> 2377.90]  one locally on
[2377.90 --> 2378.78]  my laptop or
[2378.78 --> 2379.38]  should I download
[2379.38 --> 2380.00]  this one and run
[2380.00 --> 2380.58]  this one on the
[2380.58 --> 2381.28]  server because it's
[2381.28 --> 2381.68]  going to use a
[2381.68 --> 2382.46]  web UI and we'd
[2382.46 --> 2383.08]  all like to have
[2383.08 --> 2383.90]  access to it.
[2384.52 --> 2385.90]  And I'm constantly
[2385.90 --> 2387.18]  trying to just do
[2387.18 --> 2387.84]  that math.
[2388.18 --> 2389.10]  And I think it
[2389.10 --> 2389.66]  makes a lot of
[2389.66 --> 2390.40]  sense to have one
[2390.40 --> 2391.02]  rig where I
[2391.02 --> 2391.58]  actually just would
[2391.58 --> 2392.36]  have that investment,
[2392.50 --> 2393.22]  have that setup.
[2393.50 --> 2395.34]  And because like 90%
[2395.34 --> 2396.20]  of these things are
[2396.20 --> 2397.38]  just web front ends,
[2397.42 --> 2397.92]  that's how you get
[2397.92 --> 2398.50]  the results,
[2398.90 --> 2399.60]  it makes a lot of
[2399.60 --> 2400.22]  sense to have one
[2400.22 --> 2400.62]  box.
[2400.94 --> 2401.40]  And then me,
[2401.96 --> 2402.40]  of course,
[2402.50 --> 2403.28]  I'd throw that app
[2403.28 --> 2404.00]  on my tail net,
[2404.12 --> 2404.54]  right?
[2404.60 --> 2405.72]  So then these AI
[2405.72 --> 2406.78]  services would just be
[2406.78 --> 2407.86]  put the name into
[2407.86 --> 2408.50]  your browser on
[2408.50 --> 2409.20]  every machine and
[2409.20 --> 2409.88]  they just pop right
[2409.88 --> 2410.08]  up.
[2410.16 --> 2411.42]  And having one box
[2411.42 --> 2411.82]  that has the
[2411.82 --> 2412.66]  hardware capabilities,
[2413.04 --> 2413.46]  for me,
[2413.54 --> 2413.68]  you know,
[2413.70 --> 2414.14]  a couple of
[2414.14 --> 2414.48]  people,
[2415.24 --> 2415.30]  and,
[2415.38 --> 2415.58]  you know,
[2415.68 --> 2416.52]  maybe us here at
[2416.52 --> 2416.74]  JB,
[2417.50 --> 2418.72]  seems like the way
[2418.72 --> 2419.10]  to go.
[2419.40 --> 2419.88]  Instead of all
[2419.88 --> 2420.78]  individual machines
[2420.78 --> 2421.54]  all having to
[2421.54 --> 2422.46]  have that power.
[2423.18 --> 2423.28]  Right.
[2423.42 --> 2424.72]  And power is going
[2424.72 --> 2426.04]  to be my next little
[2426.04 --> 2426.60]  topic here,
[2426.64 --> 2426.90]  actually.
[2427.44 --> 2428.92]  If I asked you
[2428.92 --> 2429.62]  how much you
[2429.62 --> 2431.22]  thought a 24-core
[2431.22 --> 2433.28]  monster CPU with
[2433.28 --> 2434.74]  half a, you know,
[2434.84 --> 2435.24]  quarter of a
[2435.24 --> 2436.00]  terabyte of RAM in
[2436.00 --> 2436.14]  it,
[2436.14 --> 2437.00]  how much are
[2437.00 --> 2437.26]  idle?
[2437.36 --> 2437.94]  Just CPU,
[2438.12 --> 2438.38]  motherboard,
[2438.58 --> 2439.64]  no PCI devices.
[2440.20 --> 2440.92]  What would be an
[2440.92 --> 2442.32]  acceptable idle
[2442.32 --> 2443.38]  power draw for you?
[2443.76 --> 2443.98]  Me?
[2444.36 --> 2444.74]  Well, that's
[2444.74 --> 2445.34]  different, but,
[2445.42 --> 2446.12]  I mean,
[2446.14 --> 2446.42]  you've got to
[2446.42 --> 2446.60]  figure.
[2447.28 --> 2448.10]  For most people,
[2448.20 --> 2448.62]  I think it's
[2448.62 --> 2449.14]  something in the
[2449.14 --> 2450.14]  light bulb,
[2450.22 --> 2450.44]  60,
[2450.52 --> 2451.24]  70 watts,
[2451.28 --> 2452.10]  80 watts would
[2452.10 --> 2453.76]  be fine.
[2453.98 --> 2454.08]  You know,
[2454.12 --> 2454.28]  you know,
[2454.32 --> 2454.86]  you see some
[2454.86 --> 2455.90]  light bulbs,
[2455.98 --> 2456.98]  maybe 110 watts
[2456.98 --> 2457.24]  for,
[2458.08 --> 2458.52]  I don't know.
[2458.78 --> 2458.88]  Because,
[2458.96 --> 2459.04]  I mean,
[2459.06 --> 2459.86]  if you go back a
[2459.86 --> 2460.18]  couple of
[2460.18 --> 2460.98]  generations to
[2460.98 --> 2462.14]  the LGA 2011
[2462.14 --> 2463.16]  build that I had
[2463.16 --> 2463.88]  before this,
[2463.88 --> 2464.52]  which was a,
[2464.86 --> 2465.86]  several years ago
[2465.86 --> 2466.08]  now,
[2466.12 --> 2466.50]  but it was a
[2466.50 --> 2467.54]  dual Zeon chip,
[2468.18 --> 2468.92]  and I had,
[2468.98 --> 2469.26]  I think,
[2469.68 --> 2470.52]  spread across two
[2470.52 --> 2471.10]  CPUs,
[2471.14 --> 2472.02]  I had 20 cores
[2472.02 --> 2472.88]  and 40 threads
[2472.88 --> 2474.84]  and 128 gigs of RAM
[2474.84 --> 2475.34]  when I was doing all
[2475.34 --> 2476.24]  that OpenShift stuff
[2476.24 --> 2476.74]  for Red Hat.
[2477.14 --> 2478.34]  This Epic system,
[2478.94 --> 2479.68]  from the wall,
[2480.06 --> 2481.60]  45 to 50 watts
[2481.60 --> 2482.00]  are idle.
[2482.00 --> 2482.90]  Wow.
[2483.94 --> 2484.30]  Yeah,
[2484.36 --> 2484.46]  I mean,
[2484.46 --> 2484.88]  I think my,
[2484.96 --> 2485.76]  I think my servers
[2485.76 --> 2487.00]  are hundreds of watts.
[2487.24 --> 2487.40]  Well,
[2487.44 --> 2488.24]  I'm used to those
[2488.24 --> 2488.52]  Zeons,
[2488.62 --> 2489.56]  and they were in
[2489.56 --> 2491.04]  the 150 to 200
[2491.04 --> 2491.64]  watt range,
[2491.72 --> 2493.34]  sat there doing
[2493.34 --> 2494.30]  Billy Bob nothing
[2494.30 --> 2494.80]  at all,
[2495.00 --> 2495.30]  you know?
[2495.36 --> 2495.52]  Yeah.
[2495.90 --> 2496.08]  Yeah,
[2496.08 --> 2496.60]  I think that's
[2496.60 --> 2497.12]  what mine is.
[2497.62 --> 2498.54]  That is really,
[2498.78 --> 2500.14]  that is a huge change.
[2500.52 --> 2501.08]  Big difference.
[2501.22 --> 2501.46]  Yeah,
[2501.56 --> 2501.70]  boy,
[2501.72 --> 2502.24]  I'm glad to hear that.
[2502.28 --> 2502.68]  And then you add
[2502.68 --> 2503.60]  in the Arc Pro card,
[2503.66 --> 2503.78]  I mean,
[2503.80 --> 2504.52]  I go through all
[2504.52 --> 2505.48]  the specifics
[2505.48 --> 2506.12]  in the video,
[2506.56 --> 2507.48]  but the Arc Pro card
[2507.48 --> 2508.32]  was about 10 watts
[2508.32 --> 2508.78]  at idle,
[2509.12 --> 2509.88]  the NVIDIA card
[2509.88 --> 2510.88]  was about 10 watts,
[2510.88 --> 2512.20]  the 10 gig networking
[2512.20 --> 2513.16]  SFP plus card
[2513.16 --> 2514.12]  was about 10 watts.
[2514.66 --> 2515.40]  By the time you add
[2515.40 --> 2516.30]  in all hard drives,
[2516.44 --> 2516.58]  you know,
[2516.66 --> 2516.98]  10,
[2518.00 --> 2518.66]  three and a half inch
[2518.66 --> 2519.22]  hard drives,
[2519.28 --> 2519.58]  that's sort of
[2519.58 --> 2520.38]  another 60 watts,
[2520.46 --> 2520.82]  give or take
[2520.82 --> 2521.80]  five or six watts each.
[2522.50 --> 2522.64]  You know,
[2522.70 --> 2523.76]  so I've got this whole
[2523.76 --> 2525.84]  super powerful box
[2525.84 --> 2526.90]  running in the basement
[2526.90 --> 2529.00]  for 175 watts.
[2529.12 --> 2529.28]  I mean,
[2529.30 --> 2530.14]  it just absolutely
[2530.14 --> 2531.10]  blows my mind
[2531.10 --> 2531.60]  that I can have
[2531.60 --> 2532.48]  that much power
[2532.48 --> 2533.22]  at my disposal
[2533.22 --> 2534.96]  for such a small
[2534.96 --> 2535.54]  power budget.
[2536.20 --> 2536.28]  Yeah,
[2536.46 --> 2537.70]  that's a big,
[2537.76 --> 2538.58]  big improvement.
[2539.10 --> 2539.70]  And yeah,
[2539.70 --> 2540.06]  you're right.
[2540.16 --> 2540.42]  It's,
[2540.42 --> 2540.86]  it would run
[2540.86 --> 2541.62]  circles around
[2541.62 --> 2542.10]  my system.
[2542.68 --> 2542.86]  Hmm,
[2543.30 --> 2543.70]  that's good.
[2543.74 --> 2544.14]  I'm really glad
[2544.14 --> 2544.48]  to hear that.
[2544.50 --> 2545.28]  It makes me kind of,
[2545.62 --> 2546.14]  kind of think
[2546.14 --> 2546.76]  this is a future
[2546.76 --> 2548.10]  direction for maybe
[2548.10 --> 2548.80]  systems here at the
[2548.80 --> 2549.58]  JB headquarters.
[2549.86 --> 2550.48]  The only thing
[2550.48 --> 2551.94]  really that would
[2551.94 --> 2553.14]  run circles around
[2553.14 --> 2553.58]  it in terms of
[2553.58 --> 2553.98]  power usage
[2553.98 --> 2554.84]  would be like a
[2554.84 --> 2555.88]  fleet of,
[2556.14 --> 2556.28]  you know,
[2556.34 --> 2557.22]  small form factor
[2557.22 --> 2558.00]  PCs or something
[2558.00 --> 2558.46]  like that.
[2558.54 --> 2558.64]  Sure,
[2558.98 --> 2559.18]  sure.
[2559.24 --> 2560.04]  But then you've
[2560.04 --> 2561.06]  got the complexity
[2561.06 --> 2562.04]  of managing
[2562.04 --> 2563.38]  10 or 15
[2563.38 --> 2564.10]  different power
[2564.10 --> 2564.62]  supplies
[2564.62 --> 2565.94]  and all the
[2565.94 --> 2566.86]  overhead of managing
[2566.86 --> 2567.54]  10 or 15
[2567.54 --> 2568.82]  different operating
[2568.82 --> 2569.86]  systems and yada,
[2569.96 --> 2570.12]  yada,
[2570.20 --> 2570.34]  yada,
[2570.34 --> 2570.52]  right?
[2570.58 --> 2571.10]  You get the
[2571.10 --> 2571.42]  idea.
[2571.62 --> 2571.74]  Yeah,
[2572.04 --> 2572.20]  yeah,
[2572.44 --> 2572.62]  yeah.
[2572.74 --> 2573.52]  Beowulf cluster is
[2573.52 --> 2574.02]  not always the
[2574.02 --> 2574.60]  answer anymore.
[2575.18 --> 2575.58]  But I really,
[2575.76 --> 2575.86]  you know,
[2575.88 --> 2576.32]  because I've been,
[2576.72 --> 2577.28]  as I've been looking
[2577.28 --> 2577.56]  at this,
[2577.60 --> 2578.06]  I'm thinking,
[2578.22 --> 2578.72]  what are we going
[2578.72 --> 2579.00]  to do?
[2579.02 --> 2579.50]  Are we going to put
[2579.50 --> 2580.36]  video cards in
[2580.36 --> 2580.80]  several of our
[2580.80 --> 2581.40]  machines and buy
[2581.40 --> 2582.14]  several video cards?
[2582.14 --> 2582.60]  That's just not
[2582.60 --> 2582.96]  very,
[2583.02 --> 2584.00]  that's just not very
[2584.00 --> 2584.94]  realistic from a
[2584.94 --> 2585.58]  budget standpoint.
[2585.90 --> 2586.48]  And I don't
[2586.48 --> 2587.24]  necessarily need that.
[2587.34 --> 2587.68]  And am I going to
[2587.68 --> 2587.92]  buy,
[2588.06 --> 2588.78]  and am I going to buy
[2588.78 --> 2589.50]  all my future
[2589.50 --> 2590.52]  laptops with dedicated
[2590.52 --> 2592.44]  graphics or only buy
[2592.44 --> 2593.28]  Macs with neural
[2593.28 --> 2593.58]  cores?
[2593.72 --> 2594.52]  I just don't think
[2594.52 --> 2595.28]  that's viable either.
[2595.28 --> 2595.86]  I'd like to have
[2595.86 --> 2597.00]  my laptops be lean,
[2597.12 --> 2597.26]  mean,
[2597.30 --> 2597.80]  and portable.
[2598.42 --> 2598.68]  So yeah,
[2598.70 --> 2599.22]  I think this is
[2599.22 --> 2599.70]  fantastic,
[2599.86 --> 2600.08]  Alex.
[2600.52 --> 2601.94]  This is a pretty
[2601.94 --> 2602.74]  epic build.
[2603.42 --> 2604.64]  I see what you did
[2604.64 --> 2604.92]  there.
[2604.92 --> 2609.10]  This week in
[2609.10 --> 2609.52]  Bitcoin.
[2609.72 --> 2610.56]  It's a new show in
[2610.56 --> 2611.70]  development inside the
[2611.70 --> 2612.66]  Jupiter Broadcasting
[2612.66 --> 2613.26]  Labs.
[2613.46 --> 2614.18]  And you're one of the
[2614.18 --> 2614.96]  very first to hear
[2614.96 --> 2615.34]  about it.
[2615.42 --> 2616.10]  Now you guys maybe
[2616.10 --> 2616.74]  know that I've been
[2616.74 --> 2617.42]  following Bitcoin
[2617.42 --> 2618.46]  since around 2012.
[2619.46 --> 2620.52]  But I think right now
[2620.52 --> 2621.08]  it's actually one of
[2621.08 --> 2621.74]  the most interesting
[2621.74 --> 2623.60]  time ever for Bitcoin.
[2624.48 --> 2625.40]  Definitely the launch
[2625.40 --> 2626.10]  of the ETFs.
[2626.12 --> 2626.58]  That's been kicking
[2626.58 --> 2627.50]  off a new phase in
[2627.50 --> 2628.24]  development investment.
[2628.64 --> 2629.54]  So starting in just
[2629.54 --> 2630.26]  the next few months,
[2630.26 --> 2630.74]  we're going to see
[2630.74 --> 2631.80]  new types of projects
[2631.80 --> 2632.50]  and new types of
[2632.50 --> 2633.20]  development happening
[2633.20 --> 2634.30]  on Bitcoin at a
[2634.30 --> 2634.90]  level we've never
[2634.90 --> 2635.76]  seen before.
[2636.52 --> 2637.48]  But maybe even more
[2637.48 --> 2639.16]  importantly, I think
[2639.16 --> 2640.34]  there's just a new
[2640.34 --> 2641.68]  interest ignited and a
[2641.68 --> 2642.70]  desire to understand
[2642.70 --> 2643.48]  what might be the
[2643.48 --> 2644.54]  hardest money mankind
[2644.54 --> 2645.56]  has ever known.
[2646.18 --> 2646.72]  And one of the most
[2646.72 --> 2647.58]  exciting things for me
[2647.58 --> 2648.20]  that the show will try
[2648.20 --> 2649.84]  to capture is that
[2649.84 --> 2650.86]  when you learn Bitcoin,
[2651.00 --> 2652.04]  it does reveal what
[2652.04 --> 2653.08]  is so broken about
[2653.08 --> 2654.12]  all the other systems
[2654.12 --> 2655.58]  and why an open
[2655.58 --> 2656.52]  source currency that
[2656.52 --> 2657.36]  is not tied to any
[2657.36 --> 2658.34]  particular state is
[2658.34 --> 2659.00]  going to be so
[2659.00 --> 2659.56]  important in our
[2659.56 --> 2659.86]  future.
[2660.42 --> 2661.34]  It really is a
[2661.34 --> 2662.26]  peaceful revolution by
[2662.26 --> 2663.30]  the people one sat
[2663.30 --> 2663.84]  at a time.
[2663.84 --> 2664.64]  And I'm going to
[2664.64 --> 2665.56]  cover it each week
[2665.56 --> 2666.24]  on This Week in
[2666.24 --> 2666.48]  Bitcoin.
[2666.90 --> 2667.66]  So go find the
[2667.66 --> 2671.16]  signal at www.thisweekinbitcoin.show.
[2671.86 --> 2673.42]  That's thisweekinbitcoin.show,
[2673.54 --> 2674.54]  a high signal Bitcoin
[2674.54 --> 2675.56]  news podcast in
[2675.56 --> 2676.52]  development right now
[2676.52 --> 2677.92]  focused on analysis
[2677.92 --> 2678.48]  that you'll find
[2678.48 --> 2678.90]  valuable.
[2679.78 --> 2681.10]  Thisweekinbitcoin.show.
[2681.28 --> 2682.46]  Go check it out and let
[2682.46 --> 2683.14]  me know what you think.
[2683.86 --> 2684.76]  We're on the ground
[2684.76 --> 2685.70]  floor and anybody that's
[2685.70 --> 2686.48]  interested in learning
[2686.48 --> 2687.76]  more is welcome.
[2688.42 --> 2689.26]  Go find it.
[2689.36 --> 2690.16]  Once more, it is
[2690.16 --> 2692.36]  thisweekinbitcoin.show.
[2692.36 --> 2694.14]  Give it a listen, send
[2694.14 --> 2695.00]  me your feedback and let
[2695.00 --> 2695.64]  me know what you think.
[2696.38 --> 2698.06]  Thisweekinbitcoin.show.
[2700.44 --> 2701.64]  Well, Kevin writes in,
[2701.72 --> 2702.58]  do you have any advice
[2702.58 --> 2703.52]  or suggestions for
[2703.52 --> 2704.58]  managing a huge
[2704.58 --> 2705.62]  Docker Compose file
[2705.62 --> 2706.48]  beyond just splitting
[2706.48 --> 2707.62]  it into smaller chunks?
[2708.28 --> 2709.08]  I do actually.
[2709.26 --> 2710.30]  Yes, for several years
[2710.30 --> 2711.76]  now, I have used a
[2711.76 --> 2713.26]  Ansible based Docker
[2713.26 --> 2714.14]  Compose generator.
[2714.30 --> 2714.88]  There'll be a link to it
[2714.88 --> 2715.68]  in the show notes down
[2715.68 --> 2716.00]  below.
[2716.48 --> 2717.64]  But more recently, I've
[2717.64 --> 2718.94]  actually taken not only
[2718.94 --> 2720.08]  to using the VS Code
[2720.08 --> 2722.02]  remote SSH plugin to
[2722.02 --> 2723.24]  manage Docker Compose
[2723.24 --> 2724.34]  files on my remote
[2724.34 --> 2724.78]  systems.
[2725.38 --> 2726.04]  But also, the
[2726.04 --> 2727.20]  Tailscale plugin for
[2727.20 --> 2728.38]  VS Code is pretty
[2728.38 --> 2730.52]  handy to just drop in,
[2731.00 --> 2731.74]  you know, particularly
[2731.74 --> 2732.34]  in those demo
[2732.34 --> 2733.12]  environments that I'm
[2733.12 --> 2733.82]  building all the time
[2733.82 --> 2734.62]  where I'm constantly
[2734.62 --> 2736.20]  just tweaking paths
[2736.20 --> 2737.82]  and settings and lots
[2737.82 --> 2738.82]  of little small tweaks
[2738.82 --> 2739.34]  and that kind of
[2739.34 --> 2739.60]  stuff.
[2740.14 --> 2741.00]  And then as I kind of
[2741.00 --> 2742.12]  productionize stuff and
[2742.12 --> 2742.72]  put it into my
[2742.72 --> 2744.28]  pseudo prod that's in
[2744.28 --> 2745.26]  my basement, you know,
[2745.64 --> 2746.70]  we all have that, I'm
[2746.70 --> 2747.48]  sure, listening to this
[2747.48 --> 2747.70]  show.
[2748.20 --> 2749.20]  Then I put it through
[2749.20 --> 2750.20]  the Ansible ringer and
[2750.20 --> 2751.22]  put it into the Docker
[2751.22 --> 2752.66]  Compose generator, which
[2752.66 --> 2754.36]  essentially just takes as
[2754.36 --> 2756.78]  an input a YAML dictionary
[2756.78 --> 2760.12]  of values and then using
[2760.12 --> 2761.44]  Ginger 2 templating under
[2761.44 --> 2762.92]  the hood spits out a
[2762.92 --> 2764.66]  formatted Docker Compose
[2764.66 --> 2764.98]  file.
[2765.48 --> 2766.86]  I went the route of kind
[2766.86 --> 2767.94]  of going in between,
[2768.16 --> 2769.34]  Kevin, and this is sort of
[2769.34 --> 2770.74]  the low tech, is I decided
[2770.74 --> 2772.48]  to split Docker Composes
[2772.48 --> 2774.10]  into general services group.
[2774.28 --> 2775.60]  So I have like a media
[2775.60 --> 2777.48]  Docker Compose and I have my
[2777.48 --> 2779.18]  notes and VS Code server
[2779.18 --> 2780.02]  and a few other things
[2780.02 --> 2780.64]  that are kind of in that
[2780.64 --> 2781.16]  category.
[2781.72 --> 2783.70]  And then I also have like
[2783.70 --> 2784.70]  piehole separate and stuff
[2784.70 --> 2785.14]  like that.
[2785.50 --> 2787.10]  And then what I do is just
[2787.10 --> 2788.00]  go into each individual
[2788.00 --> 2789.84]  category as its own
[2789.84 --> 2790.66]  individual server on the
[2790.66 --> 2791.14]  file.
[2791.76 --> 2792.78]  And then what I do is I
[2792.78 --> 2793.64]  just go into each
[2793.64 --> 2794.98]  directory where I have that
[2794.98 --> 2796.22]  individual stacks Docker
[2796.22 --> 2797.44]  Compose and I will just
[2797.44 --> 2798.14]  update those.
[2798.18 --> 2799.38]  And you could obviously do
[2799.38 --> 2800.28]  this a lot of different
[2800.28 --> 2800.52]  ways.
[2800.58 --> 2802.00]  But for me, instead of
[2802.00 --> 2803.26]  creating like 15 different
[2803.26 --> 2804.74]  Docker Composes, it means I
[2804.74 --> 2806.58]  have four different Docker
[2806.58 --> 2807.04]  Composes.
[2807.04 --> 2808.62]  And it's just broken down
[2808.62 --> 2809.20]  by category.
[2809.58 --> 2810.28]  But I'd love to hear other
[2810.28 --> 2810.92]  people's ideas.
[2811.44 --> 2812.48]  Feature request for Docker
[2812.48 --> 2814.22]  Compose for me would be some
[2814.22 --> 2815.44]  kind of higher level
[2815.44 --> 2817.42]  orchestration of those.
[2817.48 --> 2818.20]  I think they call them
[2818.20 --> 2819.22]  stacks underneath.
[2819.90 --> 2820.86]  It'd be great if I could
[2820.86 --> 2821.92]  just, you know, sit at my
[2821.92 --> 2823.10]  top level containers
[2823.10 --> 2825.18]  directory and have within it
[2825.18 --> 2826.48]  multiple, you know, media
[2826.48 --> 2829.92]  servers, administration, all
[2829.92 --> 2830.76]  that kind of other stuff,
[2830.84 --> 2831.78]  you know, underneath as
[2831.78 --> 2833.22]  separate directories with
[2833.22 --> 2834.58]  their own, you know, little
[2834.58 --> 2835.92]  fiefdoms within them.
[2835.92 --> 2837.36]  But then at that higher
[2837.36 --> 2838.76]  level, if I could just type
[2838.76 --> 2840.26]  something like Docker
[2840.26 --> 2842.16]  Compose, I don't know,
[2842.56 --> 2844.78]  stop all or something, and
[2844.78 --> 2846.08]  it would just traverse all
[2846.08 --> 2847.16]  of the Docker Compose files
[2847.16 --> 2848.78]  underneath, merge them into
[2848.78 --> 2849.94]  one massive file for me
[2849.94 --> 2850.80]  whenever I do that.
[2851.24 --> 2852.36]  So I can act on all the
[2852.36 --> 2854.06]  containers on my system all
[2854.06 --> 2854.46]  at once.
[2854.56 --> 2855.48]  That's the reason I've stuck
[2855.48 --> 2856.42]  with a single monolithic
[2856.42 --> 2858.28]  file broken up with Ansible
[2858.28 --> 2858.68]  underneath.
[2859.14 --> 2859.24]  Yeah.
[2859.40 --> 2860.98]  From your lips to some
[2860.98 --> 2862.00]  developers ears.
[2862.28 --> 2863.16]  I hope so.
[2863.20 --> 2864.10]  Maybe somebody knows how to
[2864.10 --> 2864.92]  do it and they can boost it
[2864.92 --> 2865.02]  in.
[2865.06 --> 2866.18]  We got some great boosts
[2866.18 --> 2866.72]  this week.
[2866.88 --> 2868.64]  And Aaron is our baller
[2868.64 --> 2871.10]  with 78,000 six sats.
[2871.26 --> 2872.80]  And he was following up on a
[2872.80 --> 2873.50]  boost from our previous
[2873.50 --> 2874.00]  episode.
[2874.64 --> 2875.60]  He said, I got the
[2875.60 --> 2876.88]  pronunciation wrong of his
[2876.88 --> 2877.50]  town in Texas.
[2877.70 --> 2878.76]  Surprise, surprise.
[2879.44 --> 2879.84]  Shocker.
[2880.26 --> 2881.16]  It's cute, too.
[2881.20 --> 2881.94]  It's called Bernie.
[2882.40 --> 2883.16]  The town of Barney.
[2883.70 --> 2884.42]  You know what?
[2884.92 --> 2885.20]  Bernie.
[2885.44 --> 2886.20]  Where are you from?
[2886.30 --> 2886.96]  Bernie, Texas.
[2887.64 --> 2888.00]  Barney.
[2888.92 --> 2889.32]  Barney.
[2889.42 --> 2890.22]  I would love that.
[2890.28 --> 2890.88]  I would love to be able to
[2890.88 --> 2891.26]  say that.
[2891.78 --> 2892.54]  He says, sorry about the
[2892.54 --> 2892.82]  confusion.
[2892.82 --> 2893.82]  No, it was all my fault.
[2893.92 --> 2895.22]  It's an area of Texas that has
[2895.22 --> 2896.34]  German heritage.
[2897.18 --> 2898.62]  He said, you'd be surprised about
[2898.62 --> 2899.72]  Thai food here in Texas, too.
[2899.82 --> 2900.86]  I doubt that.
[2901.04 --> 2902.32]  You see, that's what somebody who's
[2902.32 --> 2903.82]  lived in Texas says about Texas
[2903.82 --> 2904.34]  Thai food.
[2904.90 --> 2905.88]  If you've ever been to the
[2905.88 --> 2906.92]  Pacific Northwest, you'll
[2906.92 --> 2910.06]  understand the Pacific Rim is
[2910.06 --> 2911.30]  obviously where a lot of Asians
[2911.30 --> 2912.06]  land first.
[2912.22 --> 2914.42]  And so the food from Asia in the
[2914.42 --> 2916.78]  Pacific Rim, some of the best Thai
[2916.78 --> 2918.68]  food I've ever had has been in the
[2918.68 --> 2919.82]  Seattle general area.
[2919.82 --> 2921.20]  Top notch primo.
[2921.52 --> 2921.72]  Yeah.
[2921.80 --> 2922.20]  Top notch primo.
[2922.32 --> 2923.00]  It's pretty good.
[2923.54 --> 2924.96]  Yeah, it's pretty good.
[2925.86 --> 2927.20]  But he says they'd blow you away.
[2927.28 --> 2928.40]  So I'd be down to try it.
[2928.46 --> 2929.54]  Plus, I want to go to a town called
[2929.54 --> 2930.24]  Barney anyways.
[2930.46 --> 2932.18]  And hey, I used to think that
[2932.18 --> 2933.98]  barbecue I used to get in London was
[2933.98 --> 2935.32]  good until I went to Austin.
[2935.80 --> 2937.32]  So I know, you know, that actually
[2937.32 --> 2937.82]  wrecked me.
[2938.40 --> 2940.88]  I can confidently say that I have
[2940.88 --> 2943.06]  never had barbecue as good since.
[2943.18 --> 2944.68]  And it kind of wrecked me.
[2944.68 --> 2946.24]  And the local places around here
[2946.24 --> 2947.74]  very much disappoint.
[2947.74 --> 2949.98]  And I, much like you just
[2949.98 --> 2951.26]  mentioned, did not appreciate
[2951.26 --> 2951.70]  that.
[2952.28 --> 2954.26]  And I kind of wish, in a way, I
[2954.26 --> 2954.82]  didn't know.
[2955.12 --> 2955.38]  Yeah.
[2955.70 --> 2956.64]  But much like I probably did for
[2956.64 --> 2957.82]  you, it's kind of inspired me to
[2957.82 --> 2959.44]  maybe this summer really get into
[2959.44 --> 2960.40]  actually just making my own
[2960.40 --> 2960.92]  brisket again.
[2961.36 --> 2962.02]  Sometimes you got to do it
[2962.02 --> 2962.32]  yourself.
[2962.48 --> 2963.06]  Now I'm hungry.
[2963.16 --> 2963.62]  Thanks, Chris.
[2963.88 --> 2964.42]  I know, right?
[2964.48 --> 2965.60]  He says, yeah, it's lunchtime.
[2965.66 --> 2967.46]  He says, he finishes with, he
[2967.46 --> 2968.90]  appreciated the advice with
[2968.90 --> 2970.22]  jellyfin over tail scale.
[2970.76 --> 2970.90]  Yeah.
[2970.90 --> 2973.30]  You know, tail scale and all of my
[2973.30 --> 2975.52]  services are like peanut butter
[2975.52 --> 2976.02]  and jelly.
[2976.20 --> 2978.16]  But the jellyfin one solved
[2978.16 --> 2979.48]  sharing for me.
[2979.84 --> 2980.82]  I don't share it with as many
[2980.82 --> 2981.58]  people anymore.
[2982.26 --> 2984.46]  But my wife and I rarely these
[2984.46 --> 2985.56]  days, but every now and then
[2985.56 --> 2986.94]  there's this little burger place
[2986.94 --> 2988.02]  that's in like a train car.
[2988.52 --> 2989.56]  And they make some of the best
[2989.56 --> 2990.28]  burgers around.
[2990.44 --> 2991.66]  And we like to go out there and
[2991.66 --> 2992.94]  order, but sometimes it can take
[2992.94 --> 2993.32]  them a bit.
[2993.68 --> 2994.94]  And it's a great chance to watch
[2994.94 --> 2995.96]  an episode of like Who's the
[2995.96 --> 2996.36]  Boss?
[2997.24 --> 2998.58]  Or, you know, something like that.
[2998.86 --> 2999.80]  Maybe King of the Hill.
[3000.66 --> 3003.50]  And those are great shows because
[3003.50 --> 3004.52]  they're low res and they're easy
[3004.52 --> 3005.34]  to stream over cellular.
[3005.62 --> 3006.66]  And I was never, when we switched
[3006.66 --> 3007.76]  to jellyfin, I'd lost that.
[3008.10 --> 3009.88]  And then when I realized, hey,
[3009.94 --> 3011.08]  dummy, put it all on tail scale.
[3012.22 --> 3012.78]  Problem solved.
[3012.90 --> 3013.82]  Now we get to watch King of the
[3013.82 --> 3014.52]  Hill at the burger place.
[3014.86 --> 3016.14]  Well, dare I say, keep an eye out
[3016.14 --> 3017.60]  on the tail scale channels this
[3017.60 --> 3018.98]  week, maybe next week.
[3019.44 --> 3022.16]  I've got a video planned talking
[3022.16 --> 3024.14]  about how to do sharing of
[3024.14 --> 3026.04]  self-hosted services using custom
[3026.04 --> 3028.34]  domains, using caddy underneath.
[3028.34 --> 3030.42]  So if you don't want to rely on
[3030.42 --> 3033.40]  the TS.net stuff, that's your
[3033.40 --> 3033.76]  solution.
[3034.20 --> 3035.50]  Odin's Ride comes in with 5,000
[3035.50 --> 3035.80]  sats.
[3036.56 --> 3037.68]  I said, I was glad to hear a bit
[3037.68 --> 3038.68]  about Unraid on the show.
[3038.80 --> 3040.40]  As a fully capable sysadmin, I've
[3040.40 --> 3042.26]  been a long time happy Unraid user
[3042.26 --> 3043.58]  simply because it makes things so
[3043.58 --> 3043.96]  simple.
[3044.48 --> 3045.58]  It's a great solution for those of
[3045.58 --> 3047.04]  us who want to self-host but are
[3047.04 --> 3048.46]  just too busy to keep up with the
[3048.46 --> 3050.66]  nitty gritty technical details or
[3050.66 --> 3051.66]  don't want to spend a ton of time
[3051.66 --> 3052.68]  maintaining systems.
[3053.06 --> 3054.36]  Plus, it works great with tail
[3054.36 --> 3054.52]  scale.
[3056.34 --> 3057.92]  I'm feeling this one, Odin.
[3057.92 --> 3061.26]  My shame right now is my home
[3061.26 --> 3062.74]  assistant has gone kind of sideways
[3062.74 --> 3064.18]  on me in a weird way.
[3064.64 --> 3065.90]  Just certain things aren't working.
[3066.84 --> 3069.22]  I, for years, have used bedtime and
[3069.22 --> 3069.98]  good morning scripts.
[3070.64 --> 3071.84]  And, you know, I have it tied to
[3071.84 --> 3072.18]  buttons.
[3072.38 --> 3074.02]  It's a button on the dashboard.
[3074.86 --> 3075.56]  They just quit working.
[3076.44 --> 3078.48]  And I haven't touched the system for
[3078.48 --> 3079.82]  something like nearly 50 days.
[3079.98 --> 3081.04]  And this is part of the reason why
[3081.04 --> 3081.72]  things have gone sideways.
[3082.08 --> 3083.30]  I haven't done any updates.
[3083.50 --> 3084.90]  I haven't changed any configuration.
[3084.90 --> 3087.34]  I literally have, I've only rebooted
[3087.34 --> 3088.24]  it a couple of times.
[3088.82 --> 3090.22]  And things are just kind of not
[3090.22 --> 3090.76]  working.
[3091.54 --> 3093.04]  And I don't know if it's a bug or
[3093.04 --> 3093.42]  what.
[3093.62 --> 3094.86]  And I feel this right now.
[3094.92 --> 3096.54]  Like, I really haven't had time to
[3096.54 --> 3097.38]  get to my infrastructure.
[3097.68 --> 3098.40]  I've been so busy.
[3098.44 --> 3099.54]  And I'm only going to be busier with
[3099.54 --> 3100.32]  this travel season.
[3101.10 --> 3102.26]  Could really use something that just
[3102.26 --> 3103.34]  is an easy button for a little
[3103.34 --> 3103.62]  while.
[3103.72 --> 3105.52]  I wish I could just hit a button and
[3105.52 --> 3107.20]  everything is just fully self-
[3107.20 --> 3108.10]  automated for a while.
[3108.60 --> 3109.10]  That's the dream.
[3109.74 --> 3112.24]  BirdDad0234 comes in with 10,000
[3112.24 --> 3112.50]  sets.
[3112.50 --> 3113.66]  He'll be our last booster this
[3113.66 --> 3113.86]  week.
[3113.90 --> 3115.06]  And he says, I've been meaning to
[3115.06 --> 3116.26]  send this in so many times.
[3116.98 --> 3118.90]  To heal your ripping woes, I
[3118.90 --> 3120.94]  present ARM, the automatic
[3120.94 --> 3121.84]  ripping machine.
[3122.16 --> 3124.34]  Insert a disc, it finds it, and
[3124.34 --> 3125.30]  then it rips it appropriately.
[3125.84 --> 3127.28]  Go forth and rip, my dudes.
[3128.48 --> 3130.06]  Oh, so you mean my Windows Media
[3130.06 --> 3131.98]  center, or Windows Media player
[3131.98 --> 3133.84]  ripping wasn't the best way to do
[3133.84 --> 3134.18]  something.
[3134.36 --> 3135.80]  This might be a step up, Alex.
[3135.92 --> 3136.98]  This might be a step up.
[3137.12 --> 3137.48]  Likely.
[3138.32 --> 3139.62]  See, yeah, you just insert a
[3139.62 --> 3141.44]  Blu-ray, a DVD, or a music CD.
[3141.44 --> 3142.84]  It checks to see if it's audio,
[3142.98 --> 3144.48]  video, or whatever, and data, and
[3144.48 --> 3145.80]  then it just rips it.
[3146.66 --> 3148.40]  Man, just put a little Linux box
[3148.40 --> 3149.36]  somewhere with a drive?
[3149.82 --> 3150.44]  It just does it.
[3150.56 --> 3152.04]  It goes all sheer la boof and just
[3152.04 --> 3152.44]  does it.
[3153.10 --> 3153.84]  That's awesome.
[3153.92 --> 3154.66]  Yeah, just do it.
[3154.76 --> 3155.08]  Nice.
[3155.26 --> 3156.32]  Thank you, everybody, who boosted
[3156.32 --> 3156.38]  in.
[3156.40 --> 3157.22]  We had six boosters.
[3157.32 --> 3159.76]  We only stacked 98,228 sats,
[3159.84 --> 3159.98]  though.
[3160.18 --> 3161.48]  I think maybe that's in a
[3161.48 --> 3163.10]  commentary on the last episode,
[3163.20 --> 3164.18]  but we still appreciate everybody
[3164.18 --> 3164.98]  who did boost in.
[3165.30 --> 3166.70]  You can get a new podcast app and
[3166.70 --> 3168.34]  join the podcasting 2.0 revolution
[3168.34 --> 3169.28]  that is working to keep
[3169.28 --> 3171.20]  podcasting decentralized and
[3171.20 --> 3172.20]  making it possible for the
[3172.20 --> 3173.36]  audience to fund the podcast
[3173.36 --> 3174.96]  directly, keeping you the
[3174.96 --> 3176.20]  biggest customer and therefore
[3176.20 --> 3177.40]  the focus on the quality.
[3178.32 --> 3179.88]  Podcastapps.com and also a big
[3179.88 --> 3181.18]  thank you to our SREs.
[3181.70 --> 3182.82]  You can find out more at
[3182.82 --> 3184.62]  selfhosted.show.sre.
[3185.08 --> 3187.72]  There is a reasonably priced
[3187.72 --> 3189.46]  membership that gives you an
[3189.46 --> 3190.98]  ad-free version of the show with
[3190.98 --> 3192.46]  additional content, a post-show at
[3192.46 --> 3194.48]  the end as well, and it really
[3194.48 --> 3196.18]  helps us stay on the road these
[3196.18 --> 3196.32]  days.
[3196.38 --> 3197.66]  We have one official sponsor this
[3197.66 --> 3199.30]  week, and the other sponsor is
[3199.30 --> 3200.98]  really our members and our
[3200.98 --> 3202.04]  boosters who boost the individual
[3202.04 --> 3202.52]  production.
[3202.98 --> 3204.98]  Selfhosted.show.sre if you'd like
[3204.98 --> 3205.44]  to sign up.
[3205.92 --> 3206.76]  Don't forget, with conference
[3206.76 --> 3208.06]  season fast approaching,
[3208.26 --> 3210.10]  meetup.com slash jupiter
[3210.10 --> 3211.74]  broadcasting is the place to go
[3211.74 --> 3213.84]  to find out all of the real-time
[3213.84 --> 3216.18]  information about all the meetups
[3216.18 --> 3216.68]  that we're having.
[3216.94 --> 3218.20]  There'll also be various matrix
[3218.20 --> 3220.24]  rooms generally related to each
[3220.24 --> 3222.02]  event as well, so if you want to
[3222.02 --> 3223.04]  find out more information about
[3223.04 --> 3224.88]  that, meetup.com slash jupiter
[3224.88 --> 3225.30]  broadcasting.
[3225.30 --> 3227.20]  Yes, coming up very soon, even
[3227.20 --> 3228.94]  if you can't see us at scale,
[3229.12 --> 3229.98]  we'll have a couple events
[3229.98 --> 3231.26]  shortly after that, so maybe
[3231.26 --> 3232.92]  we'll get a chance to say hi.
[3233.56 --> 3235.68]  You can find me on Weapon X, I
[3235.68 --> 3236.86]  am at chrislas.
[3237.62 --> 3238.94]  Still doing the Weapon X thing,
[3239.02 --> 3239.16]  huh?
[3239.42 --> 3241.14]  As long as it's got that stupid
[3241.14 --> 3241.48]  name.
[3243.32 --> 3245.50]  I'm over at alex.ktz.me for all
[3245.50 --> 3246.68]  the various places that I'm on the
[3246.68 --> 3248.04]  internet, and thanks for listening
[3248.04 --> 3248.42]  everybody.
[3248.62 --> 3250.34]  That was selfhosted.show slash
[3250.34 --> 3251.16]  118.
[3251.16 --> 3253.22]  How to say xjilipea. Bolg
[3253.22 --> 3253.98]  Please stop ming for watching.
[3253.98 --> 3254.94]  Please stop ming for watching.
[3254.96 --> 3255.90]  I'm roadmellerizing
[3255.90 --> 3256.14]  because of the cosmetic
[3256.14 --> 3256.16]  incident.
[3256.16 --> 3256.94]  Orkonmyvil
[3256.94 --> 3257.02]  Is it aSS
[3257.02 --> 3257.40]  too much?
[3257.40 --> 3258.60]  All along,
[3258.60 --> 3259.22]  the reasonsπου
[3259.22 --> 3259.50]  are always
[3259.50 --> 3259.70]  modernized
[3259.70 --> 3260.16]  people
[3260.30 --> 3260.46]  who have
[3260.46 --> 3261.32]  tempered
[3261.32 --> 3261.40]  your
[3261.40 --> 3262.42] ijuana
[3262.42 --> 3262.52]  isn't
[3262.52 --> 3263.00]  upset.
[3263.00 --> 3263.32]  How to sound
[3263.94 --> 3264.66]  about
[3264.66 --> 3264.78]  the
[3264.78 --> 3265.48]  Va-da-da- Evangel
[3265.48 --> 3266.42]  event.
[3267.34 --> 3269.42]  And
[3269.52 --> 3270.84]  really
[3270.84 --> 3271.68]  can see
[3274.82 --> 3276.32]  other
[3276.40 --> 3277.30] .
