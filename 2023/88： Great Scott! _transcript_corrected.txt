[0.00 → 6.40] Well, it does feel like we were only just in California, but you're making excuses to go back again. What's wrong with you?
[7.04 → 14.42] Excuses? Excuses? I'm being dragged back. Just when I thought I was out, Alex, they pull me back in.
[14.86 → 27.94] Traditionally in the springtime, that meant, for JB at least, Linux Fest Northwest. And it doesn't really look like that's going to be happening again this year, sadly. And you want to get your springtime conference on, don't you?
[27.94 → 49.46] Yeah. Scale calls. And it does feel like it's been a long time since we had an event to go to. There's a lot of good audiences and community members that are there. And it's an opportunity for the team to get together again. We're still working out all the details, but we wanted to get the word out kind of early because from like recording now, it's like 55 days out or something. It's March 10th-ish or something like that.
[49.70 → 51.50] That's not very long at all.
[51.50 → 75.30] No, I know. I know. Like we really got to. And it's been one of those things where we kind of hem and hawed a little bit because like you said, we were just in Pasadena. Like we were literally just there a few months ago. And if we could pick somewhere new to go, we'd rather because we want to go see folks we haven't had a chance to see for a while. Thankfully, the crew down at Scale and in the Scale area is really awesome. So, you know, it's going to be worth it.
[75.30 → 79.38] It was the end of September we were there. Somehow it's mid-January already.
[79.70 → 83.44] No, I know. It's wild. And get this, it's 2023 too.
[84.96 → 103.78] Yeah. So, Scale takes place March 9th through the 12th at the Pasadena Convention Centre in Pasadena, California. There are some hotels around, probably a little cheaper if you go further out. But it's traditionally been a pretty great event. I don't know if we'll be there all four days because I think at least Sunday I'm going to need to, you know, record like a podcast.
[103.78 → 105.44] Yeah. Work.
[107.34 → 111.80] I think Scale is like the North American equivalent of FOSDEM, isn't it?
[112.22 → 119.10] Yeah. Yeah, probably. Yeah. I think it's at least 5,000 people. Well, it was probably, you know, a couple of years ago. I don't know about now.
[119.32 → 121.22] Be interesting to see how it's recovered, you know?
[121.40 → 121.62] Yeah.
[121.92 → 127.20] Even in the before times, you go to a conference like that, and you just expect to pick up the conference crud, don't you?
[127.58 → 129.62] The con-crud, as we called it. Yeah.
[129.62 → 142.72] Yeah. I don't know how much of an effect it's had or will have on FOSDEM moving forward as well. Maybe one of these years we'll get you over to Europe and get you to go to FOSDEM. I know I keep pulling your chain to do that, but one of these days.
[143.08 → 146.64] I don't know about the winter. You know, that's my only thing. It doesn't seem like winter's time to go.
[146.66 → 150.90] Yeah. February in Belgium's a bit grim sometimes.
[151.06 → 155.64] Whereas, like, March in Pasadena is going to be lovely. It's going to be great.
[155.64 → 158.72] It's no contest at all. It's just no contest.
[159.14 → 168.16] No. It's actually, for me, it's like, it's going to be nice because I'll come from the Pacific Northwest where it's no doubt kind of just gray and dreary and go down to Pasadena and enjoy the sunshine.
[168.58 → 177.20] I think the plan is, is we're going to do a little bit of a community get together up in the Seattle area, north of Seattle, up in the Gnomish County area.
[177.20 → 186.14] Then we're going to do some work at the studio and then some of us are going to drive down to Pasadena and then some of us will fly into Pasadena.
[186.26 → 189.62] It's going to, you know, crew's going to get together. We'd love to see you down there if you can make it.
[189.68 → 191.82] We'll have meetups and stuff like that once we get it all figured out.
[191.88 → 194.24] But it's early days, and we just wanted to get the word out there.
[194.70 → 200.16] And I know, you know, coming, you know, a month or two, you know, 60 Danish, 50 Danish, really, let's be, let's be honest.
[200.16 → 205.62] You're going to need to get out, get some sunshine, Alex, because you've been going deep into Kubernetes.
[206.00 → 207.60] You're going to need a little away.
[208.06 → 208.92] I have this weekend.
[209.28 → 214.88] I decided, I think, I think I was doing some server maintenance or something.
[214.98 → 218.00] And my server was down for a couple of hours.
[218.40 → 219.06] I'll tell you what it was.
[219.12 → 221.64] And we'll come on to this later in the show, but my firewall went down.
[221.82 → 222.66] So like, oh yeah.
[222.90 → 224.98] And I needed to crimp a new Ethernet cable.
[224.98 → 229.78] And I know I have a wiki article about, you know, which standard I use.
[230.16 → 236.52] But the trouble is my wiki wasn't working because DNS was down because that's on the firewall.
[237.40 → 244.92] And then, so this got me thinking about, you know, because I've always thought to myself, Kubernetes at home is just too much.
[245.14 → 246.46] It's too much.
[246.56 → 247.34] I don't need it.
[247.40 → 248.32] It's busman's holiday.
[248.76 → 250.38] I could do it all day, every day at work.
[250.42 → 252.76] I don't need to be dealing with that complexity at home.
[252.76 → 259.96] But actually, sometimes there are some services, some critical services that would benefit from being highly available.
[260.16 → 262.84] DNS is probably one of them that I need to put behind.
[263.18 → 264.24] Maybe keep alive D.
[264.86 → 270.24] But then there are some basic application services like the wiki, maybe Home Assistant.
[270.46 → 272.80] If I can get that on Kubernetes, that'd be pretty cool.
[273.82 → 274.72] Don't know about that one.
[275.32 → 283.12] But certainly basic web services like a wiki, putting those on a small K3S cluster should be absolutely no problem whatsoever.
[283.12 → 287.88] And so I ended up going spelunking down the K3S rabbit hole this weekend.
[288.42 → 291.22] So K3S, can you tell me a little bit about that?
[291.36 → 292.88] I'm familiar with K8s.
[293.22 → 295.14] Yeah, well, K8s is just Kubernetes.
[295.46 → 300.98] The reason they put number eight is that there are eight characters between the K and the S, if you didn't know that.
[301.26 → 304.14] So what is K3 Kubernetes still, but smaller?
[304.14 → 305.92] It is.
[306.02 → 311.32] The idea is that Kubernetes is a small, lightweight distribution of Kubernetes.
[311.62 → 318.12] It trims out a lot of the more enterprise-y stuff that you just realistically, in a small deployment, do not need.
[318.60 → 321.42] They pick a lower number because it's smaller and lighter weight.
[321.92 → 322.90] Yeah, I like that.
[323.06 → 323.28] Okay.
[323.90 → 331.24] So it's a little, and you feel like this is probably responsible for you giving yourself permission to try this at home?
[331.24 → 335.46] Because I know you and I have talked about this before, and both of our takeaways have always been, eh, it's a bit too much.
[335.82 → 337.00] This is this what's changed?
[337.20 → 347.34] Well, it was this, and it was, I was updating the Perfect Media Server website, which is hosted on the same node as jupiterbroadcasting.com.
[347.42 → 352.76] And there's five or six pretty critical websites in my life, at least, that are hosted on this one node.
[352.76 → 362.92] And if I want to reboot it, or I want to upgrade Docker, or do anything on that node, it can take the websites down for a minute or five, depending on a reboot sometimes.
[363.86 → 372.32] And so I was actually thinking about eventually using this knowledge I gained locally on how to host the wiki and all that kind of stuff,
[372.32 → 380.42] to putting jupiterbroadcasting.com and my blog and, you know, all the other stuff into a hosted Kubernetes cluster on Linde,
[380.98 → 390.34] and then take all the server administration aspect out of the equation and literally just target it through something like a Flux Git Ops kind of scenario,
[390.34 → 398.26] where if you or I or Was or, you know, Brent or anybody on the crew pushes a small update to the website, it auto-deploys.
[398.26 → 403.76] And there's, I mean, we do that through GitHub Actions now, but there's no high availability.
[404.04 → 406.92] If that node goes down, the website goes down, and that's that.
[407.66 → 412.90] Actions is deploying the website, but wouldn't necessarily deploy the infrastructure necessary to run the website.
[413.14 → 414.02] No, absolutely not.
[414.16 → 423.30] So really, this is, for me at the moment, an academic exercise, just to try and learn a bit more about actually using Kubernetes locally,
[423.30 → 429.94] because I used it at work every day for a couple of years, probably about four or five years ago now.
[430.42 → 436.78] Ever since then, a lot of my stuff has been pretty much theoretical stuff, talking to customers, advising, you know,
[436.88 → 442.64] but I haven't had to do a lot of actual Kubernetes hands-on stuff recently.
[443.26 → 447.64] You know, I do a lot of infrastructure, like this is the best practice around etc,
[447.64 → 452.52] and how you, you know, make the right number of IOPS and all that kind of stuff for OpenShift.
[453.42 → 457.34] But actually, once the cluster's up and running, I kind of hand it off to someone else,
[457.38 → 458.68] and it's their problem to deal with.
[459.24 → 461.30] My problem is infrastructure and that kind of thing.
[461.86 → 465.64] And so for me, it's an academic exercise to learn a bit more about the inner workings of Kubernetes
[465.64 → 468.20] and just poke the dragon a little bit.
[468.20 → 475.12] And so the first hurdle I had to overcome was how do I automate the deployment of K3S?
[475.22 → 481.18] I didn't want to be treating this cluster like it was a, you know, Fabergé egg.
[481.56 → 488.08] I wanted to be able to go Duke Nuke on this thing and completely break it and rebuild it in 20 minutes.
[488.68 → 489.72] And you're all out of bubblegum.
[491.00 → 491.44] Indeed.
[492.40 → 496.20] And so I turned to my favourite tool in such a scenario, Terraform.
[496.20 → 498.00] You might have been thinking Ansible, but...
[498.00 → 498.78] I was.
[499.54 → 501.94] It's not the right tool for immutable infrastructure.
[502.18 → 510.90] Ansible is, it's more designed to configure traditional operating systems like Ubuntu or Fedora or those kinds of things.
[511.30 → 520.56] Whereas I'm running this on a small read-only OS rather than a traditional kind of like cattle versus pets is what I'm trying to explain here.
[520.66 → 523.04] I'm doing a poor job, but that's basically where I'm trying to go.
[523.04 → 529.84] And so what I ended up doing was using a Terraform provider from a chap called Tel mate on GitHub.
[530.00 → 532.02] There'll be a link to all of this stuff in the show notes.
[532.50 → 535.54] And this thing is, it talks to the Proxmox API.
[536.18 → 539.84] Once it does that, it can configure and provision different resources.
[539.84 → 541.56] So it can configure virtual machines.
[541.86 → 546.32] So essentially I have a template for the virtual machine that I'm deploying.
[546.32 → 552.00] It will then clone that virtual machine based on the parameters I have in my Terraform.
[552.50 → 557.88] So it will give it a certain size of disk for a master node and a certain size of disk for a worker node and all that kind of stuff.
[558.52 → 566.80] But where it got fascinating was I like to do static IP reservations through DHCP, which might sound a little weird.
[567.16 → 567.96] No, that's how I do it too.
[568.06 → 570.78] I do that MAC address based reservation stuff, right?
[570.92 → 572.14] So that's exactly how I do it.
[572.14 → 574.36] All my servers, my cameras, everything.
[574.36 → 576.48] Yeah, I find it works really, really well for me.
[576.68 → 577.72] You know, it has done for years.
[578.42 → 584.60] I could run a real DNS server that has an API that lets me do a proper IPAM, IP address management stuff.
[584.74 → 585.98] But I don't.
[586.38 → 589.58] I just use the built-in Open Sense one.
[590.04 → 593.46] And so what I needed to do was configure two pieces of information.
[594.08 → 595.80] One is the MAC address on a node.
[595.80 → 603.78] And also the second piece is the target Proxmox node in my Proxmox cluster that I wanted to deploy this VM onto.
[603.98 → 609.20] Because it's no good deploying all these VMs onto a single Proxmox host.
[609.60 → 613.88] Because if that host goes down, all the VMs go down, and I'm back to square one, right?
[613.96 → 618.04] So some of my worker nodes and some of my master nodes have to be distributed.
[618.04 → 625.90] So behind me, I have pulled out of the closet an old i5 system that's been gathering dust for a few years.
[625.98 → 628.54] It's running a Hollywood script behind me if you're on the live stream.
[629.24 → 632.28] I've also got my backup server running Proxmox.
[632.42 → 635.70] And I have my main server in the basement also running Proxmox.
[635.76 → 637.48] So I have a three-node Proxmox cluster.
[638.22 → 639.04] It's pretty cool.
[639.10 → 642.76] I'm not doing anything cool like live migration or anything like that.
[642.76 → 649.32] But I can, from a single Proxmox UI, see all the VMs in my house, see all the nodes in my house.
[649.56 → 653.52] And it just tickles the nerd in me, you know?
[653.92 → 654.44] No kidding.
[654.82 → 655.78] I have to ask.
[655.86 → 660.42] I mean, not to rabbit hole tangent to us here, but are you doing centralized storage?
[660.90 → 662.38] Are you thinking about centralized storage?
[662.48 → 665.26] Is each one of these Proxmox servers doing local storage?
[665.50 → 666.14] What are you doing there?
[666.52 → 669.08] Storage is local to the nodes at the moment.
[669.08 → 673.52] And so Proxmox storage is separate from Kubernetes storage in my world.
[674.12 → 678.54] I've always thought that doing Kubernetes at home was a bit silly because if, you know,
[678.60 → 684.60] let's say I wanted to run Jellyfin or Plex or something on Kubernetes and the node that
[684.60 → 691.54] has all the storage, all the media is down, well, then so is Plex or Jellyfin because the
[691.54 → 692.34] media isn't there.
[692.38 → 693.66] So what's the point in running the service?
[694.58 → 697.62] And that argument has held true for almost all of my services.
[697.62 → 702.00] But it was just that wiki thing that made me think, actually, there are a few things I
[702.00 → 704.90] wouldn't mind auto redeploying between different places.
[705.52 → 707.82] And things like a wiki are fairly stateless.
[708.24 → 714.56] So what I'm thinking of doing is using the Longhorn project, which is also from Rancher
[714.56 → 720.18] along with K3S, to synchronize small amounts of storage around the network.
[720.28 → 723.56] I'm not doing things like media files because that's just unnecessary.
[723.56 → 729.56] But a few hundred gigabytes, probably not even that, between different nodes using Longhorn.
[729.98 → 734.62] And then I'll be able to bring up a pod in any of those three Proxmox nodes as a VM.
[735.20 → 739.08] Well, I'll bring up a VM on the Proxmox node and then run a pod inside the VM.
[739.36 → 740.92] That should work.
[740.98 → 743.88] Although I haven't gotten to storage yet in my tinkering.
[744.34 → 745.80] That's for the next episode.
[745.80 → 746.20] Yeah.
[746.20 → 746.60] Yeah.
[747.80 → 749.52] I'd be curious to see where that goes.
[749.68 → 755.84] But this sounds like a really valuable project, just in the sense that the skills that you're
[755.84 → 758.32] picking up here are refreshing your day job stuff.
[758.32 → 763.10] Sounds like it could be useful for the JB infrastructure, for your own infrastructure.
[763.36 → 766.20] And man, are you making me really want to try Proxmox again?
[766.58 → 767.86] I almost did it with the Droid.
[767.86 → 774.40] I almost did Proxmox on there, but, you know, I still am high on the Nix juice.
[774.94 → 777.30] So I just went, you know, bare metal Nix OS.
[777.72 → 783.46] But, you know, it's the fact that Proxmox ships an Ubuntu kernel and I get ZFS out of the box.
[783.60 → 785.06] That really does it for me.
[785.24 → 786.08] Yeah, that's nice.
[786.28 → 786.48] Yeah.
[786.60 → 787.76] With a Debian user space.
[787.98 → 789.22] It really does it for me.
[789.48 → 790.36] That's a funky setup.
[790.66 → 791.98] So Debian user space.
[792.04 → 793.36] Well, I guess that's actually kind of Ubuntu.
[794.18 → 794.98] Pretty much.
[795.16 → 795.36] Yeah.
[795.36 → 795.66] Yeah.
[795.66 → 799.48] So I still got access to apt for all those packages.
[799.48 → 804.62] And it's a very familiar landing pad for me, except I've just got this.
[804.72 → 806.94] And I know I always say GUIs are unnecessary.
[806.94 → 807.80] They are.
[807.92 → 813.60] But I've got a nice single pane of glass GUI for all the VMs and crap running in my network.
[814.04 → 815.70] You don't need that junk for your containers.
[816.12 → 817.74] Not with Terraform, I don't.
[818.16 → 818.48] No.
[819.04 → 821.68] So just to finish the Terraform thought, because I don't think I quite did.
[822.02 → 822.28] Uh-huh.
[822.68 → 824.80] I needed the two pieces of information.
[824.80 → 829.90] I needed the IP address and I needed the MAC address and the target node to be deployed on.
[830.62 → 835.52] And so out of the box, Terraform doesn't support iterating over data structures like that.
[835.72 → 842.04] So some kind people in the Discord helped me figure out that if you use the for each command in Terraform,
[842.04 → 848.84] you can actually look up sub-elements of nested maps in this case and bring them out.
[849.06 → 858.60] And, you know, so I can have, you know, node master one, specific MAC, specific target node, node master two, et cetera, et cetera.
[858.60 → 863.16] And I can feed that stuff directly into Terraform.
[863.56 → 867.20] There's a link in the show notes to my GitHub where I figured all that stuff out.
[867.34 → 868.52] I don't know if you'll find it useful.
[868.72 → 869.08] You might.
[869.24 → 869.76] You might not.
[870.36 → 877.52] But Terraform is one of those tools that I think doesn't get enough love, but it quietly builds the infrastructure that runs the Internet.
[877.52 → 880.22] You know, it's just, it's awesome.
[881.88 → 883.84] Linode.com slash SSH.
[883.92 → 886.36] That's where you go to get $100 in 60-day credit.
[886.52 → 890.64] And it's a great way to support the show while you're checking out a cloud provider that is great for us self-hosted.
[891.00 → 898.24] I have a couple of different tricks that I can't believe Linde lets me do, but they've actually documented it for at least two different use cases now.
[898.24 → 907.34] I have found it necessary to deploy a Linde and then destroy the operating system, just get rid of the OS that's on there and deploy my own OS.
[907.44 → 913.30] Once for a VPN setup that I was doing that used a weird router on the other end, and they have their own weird Linux.
[914.10 → 916.08] And then another one is for JupyterLab.
[917.38 → 922.08] JupyterLab is a Nix box, and it, I think, started life as an Ubuntu box.
[922.08 → 928.24] But, you know, that's the kind of level of access that Linde gives you is you can change things like that.
[928.30 → 930.44] Now it's a Nix box, and it's great.
[931.26 → 934.64] It actually makes for a perfect Jupyter or a Peer Tube server, I should say.
[935.34 → 939.66] And Linde just lets you get in their like that, just lets you get in there and do that kind of stuff.
[939.70 → 943.38] And they've got perfect documentation to help you, a dashboard that makes it super approachable.
[943.54 → 947.72] So, you know, if you're just learning, you know, they've got a dashboard, you got this.
[948.10 → 950.20] If you're like a next level, you know, you've been doing this for 20 years.
[950.20 → 952.32] They've got an API you can take advantage of.
[952.58 → 954.68] Of course, they support infrastructure management tools.
[955.28 → 958.58] In fact, I'm going to put a link to their Understanding Kubernetes Guide.
[958.90 → 961.32] It is an instant download, no email required.
[961.52 → 962.34] You just go get it.
[962.66 → 965.04] It's a recently updated, like towards the end of last year.
[965.12 → 973.50] It's a comprehensive resource that covers everything from, like, fundamental concepts of Kubernetes to the individual components of a Kubernetes cluster, the network model implementations.
[973.50 → 980.64] And they just recently added sections on understanding the Kubernetes dashboard, the high availability control plane, and auto-scaling.
[981.14 → 983.50] Super great resource that they're giving away for free.
[984.08 → 986.22] And yeah, Linde works with all of those tools.
[986.34 → 990.22] So as, you know, you're learning this stuff, you can go use our $100 credit to try it.
[990.62 → 995.84] And as you're deploying this stuff, you'll find that Linde is fast enough and reliable that you can deploy it in production for millions of users.
[996.58 → 997.24] Millions of users.
[997.24 → 1000.90] I mean, I can actually say that from a source of experience.
[1001.04 → 1003.04] We run our website on Linde.
[1003.12 → 1006.00] We have tons of our back-end JB infrastructure runs on Linde.
[1006.64 → 1008.44] And our podcasts get millions of downloads.
[1008.66 → 1010.64] And they just keep on trucking right along.
[1010.76 → 1014.12] We've never had a problem in, I think, just about three years now.
[1014.52 → 1015.18] It's been really great.
[1015.26 → 1017.36] And, of course, I've got friends that have been using Linde for a decade.
[1017.70 → 1019.16] And they've been around for nearly 19 years.
[1019.46 → 1020.50] There's something you're going to love.
[1020.58 → 1023.60] They've got data centres near you with another dozen coming online this year.
[1024.08 → 1025.10] They are their own ISP.
[1025.20 → 1026.20] So the speeds are outrageous.
[1026.20 → 1027.34] The hardware is fantastic.
[1028.06 → 1030.52] I rave about it because it is legitimately the best.
[1030.94 → 1033.72] There are lots of options out there, but nobody checks all the boxes.
[1034.20 → 1036.68] So go grab that $100, kick the tires, and try it out.
[1037.24 → 1039.20] Linode.com slash SSH.
[1039.30 → 1042.14] That's Linode.com slash SSH.
[1043.74 → 1048.66] Well, in the last episode, I was bemoaning the fact we only had four entries for the hard drive giveaway.
[1049.12 → 1050.98] I'm glad to say that has changed this time.
[1051.28 → 1053.88] We had 15 or so totals.
[1054.38 → 1055.16] All right.
[1055.16 → 1055.68] 17.
[1055.68 → 1055.88] 17.
[1055.94 → 1059.02] 17 total entries into the giveaway contest.
[1059.48 → 1063.12] There will be a link in the show notes where you can go and vote for the winner.
[1063.12 → 1067.70] So all the different data loss stories I asked people to send in are now on GitHub.
[1068.14 → 1078.52] We discussed this in the Discord with a few folks about how to, you know, present this as a poll where, you know, you've got the text of the entry and then a voting system on the same page.
[1078.58 → 1082.64] And building something like this would have been a project in and of itself.
[1082.64 → 1085.32] So we just decided to take the easy route and go with GitHub.
[1085.96 → 1090.58] Now, if you react to this, or you upvote these posts somehow, not comment.
[1090.76 → 1093.40] I'm not interested in your comments, although you can make comments if you want to.
[1094.36 → 1098.02] The winner will be picked simply by the one with the most upvotes.
[1098.02 → 1099.02] Sob story.
[1099.02 → 1099.28] Oh, man.
[1100.38 → 1101.38] Oh, man.
[1101.82 → 1102.64] Oh, Geez.
[1102.74 → 1104.12] I'm reading a couple of these.
[1104.48 → 1106.74] So basically, you can go upvote the worst sob story.
[1107.16 → 1108.18] There are some good ones in there.
[1108.36 → 1111.64] I do implore you to doom scroll through a few of them.
[1112.10 → 1115.50] There are basically some lessons to be learned for sure.
[1115.72 → 1120.72] Some of these I could have seen myself making these mistakes.
[1121.42 → 1123.04] Yeah, we'll put a link to this in the show notes.
[1123.12 → 1123.30] All right.
[1123.38 → 1125.06] So go vote the worst sob story.
[1125.06 → 1128.54] I think I know the one I have to vote for, but I'll have to read them all first.
[1130.04 → 1130.44] Wow.
[1131.40 → 1132.06] Okay, Alex.
[1132.06 → 1136.88] Well, I have come across something very, very, very exciting.
[1137.02 → 1144.04] It was recommended to me by the developer of the Nebula Mesh VPN, which is also an awesome project.
[1144.76 → 1151.62] And it is a custom community firmware for the Waze 3 and Waze 2 cameras.
[1151.82 → 1153.82] Now, this is unlike anything we've talked about before.
[1153.90 → 1157.06] We have kind of talked about custom firmwares for these Waze cams before.
[1157.66 → 1158.74] This is a whole new thing, baby.
[1158.74 → 1163.44] And it is called WZ underscore mini hacks.
[1163.70 → 1166.14] It is an alternative entire firmware.
[1166.36 → 1167.60] It boots off the SD card.
[1167.70 → 1171.16] It doesn't touch the OS on your Waze cam.
[1171.36 → 1171.90] So that's nice.
[1172.20 → 1176.38] And it adds a couple of very, very nice features to these.
[1176.66 → 1179.96] Again, I'm going to say it $35 IP cameras.
[1180.86 → 1183.54] First and foremost, Ethernet support.
[1183.54 → 1193.06] So you can get a USB Ethernet dongle, and you can run the Waze cam over Ethernet, which is huge if you ask me.
[1193.22 → 1195.42] And you can do specifically even POE.
[1195.78 → 1196.48] So how does that work?
[1196.56 → 1198.18] Because they're just a USB connection, aren't they?
[1198.24 → 1198.48] Yeah.
[1198.58 → 1200.34] So you got to get an adapter.
[1200.92 → 1206.10] And there's several on Amazon that does micro USB instead of a regular like USB A.
[1206.10 → 1211.38] But you can get dongles that have micro USB and you can plug that into the Waze cam.
[1211.88 → 1218.46] This Linux environment adds support for several different types of Ethernet adapters.
[1218.58 → 1220.48] And some of them even support POE, Alex.
[1220.54 → 1222.34] You can do POE with the Waze cams.
[1222.64 → 1222.82] Really?
[1223.12 → 1223.40] Yeah.
[1223.88 → 1224.20] Yeah.
[1224.40 → 1225.56] It's huge, right?
[1225.60 → 1226.44] That's a huge change.
[1226.68 → 1227.28] Here's another one.
[1227.28 → 1230.22] This firmware comes with WireGuard pre-installed.
[1230.40 → 1236.22] All you have to do is update the config with your WireGuard information, and it'll do a WireGuard VPN right on the camera.
[1236.62 → 1237.06] Say what?
[1237.64 → 1237.90] Yep.
[1237.98 → 1239.04] WireGuard built right in.
[1239.50 → 1243.70] Because it's also a Linux box, you can SSH into it and upload your own binaries.
[1243.70 → 1253.64] So, for example, you could install Tail Scale or Nebula and just run it right on the box, right on the little teeny tiny camera.
[1253.76 → 1255.28] It has an RTSP server included.
[1255.58 → 1258.54] It has a webcam mode you can put it in just via the config file.
[1258.62 → 1261.02] You SSH into it and you can put it in a webcam mode.
[1261.52 → 1263.28] And then you can hook it up to your computer over USB.
[1263.62 → 1265.46] It also has RTMP streaming.
[1265.46 → 1279.30] So, not only could it be an RTSP camera feed that you could pull into different sources, like VLC or software like Shinobi, but it can also stream to something like YouTube Live, Twitch, those types of things.
[1279.34 → 1281.08] You can actually have it stream to an endpoint directly.
[1281.92 → 1288.24] It supports SIF, Samba, so you can have it mount a Samba share and save the recordings to a Samba share.
[1288.24 → 1295.20] So, NFS and they've added USB mass storage, like I mentioned, SSH login, where you get a user land, where you get a shell.
[1296.46 → 1297.20] It's so great.
[1297.40 → 1301.86] And Ryan, who I learned this from, tells me that he uses Ansible now to deploy his cameras.
[1302.12 → 1303.90] So, he's installed Ansible on these.
[1304.20 → 1304.64] You got me.
[1305.08 → 1306.80] What's the catch?
[1306.88 → 1307.84] Come on, there must be a catch.
[1307.90 → 1309.14] This sounds too good to be true.
[1309.54 → 1309.92] You're right.
[1310.04 → 1310.34] You're right.
[1310.40 → 1312.34] There is actually a bit of a catch, unfortunately.
[1312.34 → 1320.66] It seems like if you're on the absolute latest, I think, up-to-date version of the Waze firmware, this is broken and perhaps has been broken since the summer.
[1321.52 → 1323.38] You can't boot, because Waze kind of goes around.
[1323.96 → 1329.38] According to the project, what happens, Alex, does people try the firmware on their Waze camera.
[1329.90 → 1333.38] Then they go try to get support from Waze while they're running this firmware.
[1333.96 → 1336.08] Waze discovers this firmware is a thing.
[1336.36 → 1339.34] And then Waze makes patches, so that way they don't get support calls.
[1339.34 → 1342.22] It's not like they're actively trying to crush the project.
[1342.36 → 1343.90] They're just trying to crush support calls.
[1344.12 → 1349.94] So, the project has put a call-out asking people, don't contact Waze support when you're running the custom firmware.
[1350.16 → 1351.44] Don't go to the vendor for that.
[1351.90 → 1362.22] But the thing that I love about this is these $35 cameras have a tremendous, tremendous sensor that has incredible night vision.
[1362.32 → 1367.46] Like, you can have it even through a window looking at your backyard, and it still can make things out.
[1367.46 → 1377.30] But they've just recently, the firmware doesn't support this yet, but they just also, Waze, recently updated their Waze Pan 3 camera, which is outdoor and now moves around.
[1377.80 → 1387.92] And so, to be able to own a device like that, put your own firmware on there, run your own stuff, connect it directly to your WireGuard VPN, have it stream directly RTMP or RTSP.
[1387.92 → 1397.06] To be able to SSH into it, and it's $35 with a crazy great sensor, this, to me, just takes these devices to the next level.
[1397.38 → 1399.30] And I have to give it a strong recommendation.
[1399.64 → 1409.10] And one of the things that I really like about it, and again, super early days in my testing, but what I really liked about it is everything is configured through a single config file.
[1409.56 → 1411.52] So, you basically, you do a git checkout.
[1411.78 → 1412.78] You know, you pull down the repo.
[1412.88 → 1414.78] Okay, so I'm running Nix OS on my camera.
[1414.88 → 1415.78] That's what's happening, right?
[1415.78 → 1417.14] No, it's not Nix.
[1418.68 → 1420.34] You pull down the repo.
[1420.66 → 1423.16] It's got the SD card stuff that you drop on there.
[1423.24 → 1424.24] It's got the config file.
[1424.38 → 1425.34] It's really simple.
[1425.46 → 1426.14] It's well-documented.
[1426.56 → 1432.70] You just tweak the default settings as you like, turn on what you want, turn off what you don't, and everything is controlled through that single config file.
[1433.50 → 1434.10] And that's it.
[1434.58 → 1435.42] And then you boot it up.
[1435.90 → 1437.32] It'll get a DHCP address.
[1437.60 → 1438.18] You're off to the races.
[1438.18 → 1447.92] It turns out I have a Waze 3 camera literally behind my monitor here so I can check on the baby when she's running around making mayhem in this bonus room that I'm in.
[1448.66 → 1452.86] I've just grabbed a micro SD card, so I might be doing that whilst we're recording the rest of the show.
[1452.98 → 1454.26] This is very exciting, Chris.
[1454.34 → 1454.98] Very exciting.
[1454.98 → 1461.58] I think the other gotcha is I think it requires a minimum of a 256 gigabyte SD card because there is a whole OS on there.
[1462.14 → 1463.00] 256 gig?
[1463.36 → 1463.64] Yes.
[1463.88 → 1468.16] But the upside is you get like all of these external storage options.
[1468.98 → 1469.80] 256 Meg.
[1470.10 → 1470.64] Come on.
[1470.80 → 1471.04] Read.
[1471.14 → 1471.52] No, really?
[1471.78 → 1471.98] Yeah.
[1471.98 → 1472.30] Oh, okay.
[1472.36 → 1472.78] That's what it says.
[1473.14 → 1475.16] I just translated that to gigs in my head.
[1475.18 → 1477.30] I was going to say gigabytes and a micro SD.
[1477.52 → 1478.46] That's crazy.
[1478.50 → 1479.00] I mean, not really.
[1479.38 → 1479.80] Think about it.
[1479.80 → 1481.34] They got a whole Linux OS on there.
[1481.42 → 1483.76] They got all these different server pieces of software on there.
[1483.76 → 1484.54] I mean, yeah, you're right.
[1484.60 → 1485.32] It is still a lot.
[1485.52 → 1487.84] It's impressive that it is actually only 256 legs.
[1488.38 → 1494.08] But for me, the breakthrough thing that's going to be a game changer for my setup here, hands down, Ethernet support.
[1494.22 → 1499.64] I don't use Ethernet a lot in the RV, but the one spot I absolutely will with POE is the dash cam.
[1500.24 → 1504.66] Because the only thing that makes that thing kind of suck, the Is suck as a dash cam, is when you're going down the road.
[1505.40 → 1508.58] You can just have all this crazy Wi-Fi interference.
[1508.58 → 1513.64] And so I can drop frames just randomly, regardless of what's going on really with any of the hardware.
[1513.76 → 1516.72] Just by external random radio interference.
[1516.90 → 1525.04] So to just get that off of Wi-Fi altogether and to get that data load, which is streaming video constantly as I'm driving, and get that onto the Ethernet.
[1525.82 → 1526.68] Game changer.
[1527.00 → 1527.94] Fricking game changer.
[1528.18 → 1535.16] That is the worst thing about the Is cams to date anyway has been that they've been Wi-Fi limited, you know.
[1535.22 → 1539.18] And I've had some Wi-Fi issues going on in this house this week, actually.
[1539.18 → 1547.02] When I was screwing around with the Ada fruit display, which if you're on the live stream you can see behind me, that device only supported 2.4 gigahertz.
[1547.14 → 1551.18] So I just switched my IoT network into 2.4 only mode.
[1551.88 → 1552.98] My goodness me.
[1553.32 → 1555.94] So many devices on a 2.4 gig network.
[1556.06 → 1558.62] You forget how quickly that thing gets congested.
[1558.62 → 1563.32] I had Son off stop working Shelly stop working Google Displays.
[1563.70 → 1569.06] Stuff that's been reliable now for two or three years just f*** the bed completely.
[1569.44 → 1572.90] I flipped the 5 gig switch back on last night because I'd forgotten I'd turned it off.
[1573.02 → 1577.28] And I was like, oh, that's what you did, you plonker, you know.
[1577.70 → 1580.36] Yeah, you know, I've been doing channel analysis and stuff like that.
[1580.44 → 1582.40] I haven't gotten the SDR thing yet, but I want to.
[1582.40 → 1588.16] And of course, like all the neighbours are all stacked on a few, some of the channels, and it's just so gross.
[1588.24 → 1590.16] The setup is, it's so congested.
[1590.18 → 1597.48] And that's why I've, I've kind of slowed my excitement a little bit about Matter is it's 2.4 gigahertz as well.
[1597.56 → 1599.20] It's different channels, right?
[1599.24 → 1600.00] It's different frequencies.
[1600.50 → 1602.90] So they're not overlapping with Wi-Fi and stuff.
[1602.90 → 1614.84] But I am positive that if you have your home assistant device with your Matter radio sitting right next to your Wi-Fi access point, it will absolutely cause issues.
[1615.08 → 1616.76] Just like it does right now with Zigbee.
[1617.12 → 1620.90] The issue is, is there sometimes people have all that stuff crammed in one spot.
[1621.04 → 1626.26] You know, they have like a little electronics cabinet or electronic shelf or whatever, and they put all that stuff in one space.
[1626.34 → 1628.88] And 2.4 is just so slammed.
[1628.88 → 1632.28] So to have Ethernet, man, whoopee, I'm excited about that.
[1632.90 → 1635.64] So that is the downside is with the firmware stuff.
[1635.74 → 1637.24] They haven't fixed it with the latest firmware yet.
[1637.48 → 1639.80] That little disclaimer aside, I think you're going to love it, guys.
[1640.52 → 1641.80] I am literally doing it right now.
[1642.24 → 1642.56] Are you?
[1643.32 → 1643.68] Yeah.
[1643.84 → 1644.66] It looks real easy.
[1644.78 → 1648.52] Like you just copy the root of the SD card into the SD card directory.
[1648.98 → 1649.16] Yep.
[1649.36 → 1651.04] And then boot it up and then boot the camera up.
[1651.24 → 1654.60] I mean, I remember the Fang stuff was the right pain to do back in the day.
[1654.70 → 1655.74] This looks really easy.
[1656.34 → 1662.42] And if like you sounds like you do, like I do, I already have the Mac address reserved for an IP.
[1662.42 → 1664.70] So I know what IP it's going to get when it boots already.
[1664.92 → 1666.98] And I already have it assigned a domain name.
[1667.26 → 1668.62] It's just choice.
[1669.10 → 1671.24] It's really super easy when you have that all in place.
[1671.68 → 1678.20] I am running into the issue, though, where macOS at the moment, these SD cards were used in Raspberry Pis previously.
[1678.20 → 1689.40] And currently the partition table is picking up the first partition, which is the boot partition, which is 32 megabytes on a 16 gig SD card.
[1689.40 → 1693.28] I think it wants the whole thing just fat 32 or something.
[1693.70 → 1694.98] Just one big fat 32.
[1696.02 → 1703.34] Alex Scuba wrote in in regard to project donations, I think inspired by our chat around the Matrix project, saying they were struggling with funding.
[1703.34 → 1713.14] And really frustrating, too, by the way, after we did that episode, TechCrunch ran a feature piece on Matrix, and they ended the article talking about how much money they have.
[1713.36 → 1716.96] They totally missed the financial troubles that the Matrix Foundation is having.
[1717.02 → 1718.54] It was embarrassing for TechCrunch.
[1719.44 → 1720.56] But Scuba wrote, I wrote out.
[1720.68 → 1723.54] I reached out to the foundation for us individual supporters here.
[1723.62 → 1725.62] How they here's how they claim we should support them.
[1725.62 → 1728.80] Quote, thanks for reaching out and supporting Matrix.
[1729.24 → 1739.32] The best way to donate is through our Donor Box campaign at donorbox.org slash keep dash matrix dash exciting.
[1740.02 → 1741.98] Thanks again, Lisa.
[1742.72 → 1743.80] That's their answer.
[1744.32 → 1747.54] Well, I was thinking last time we recorded, what could we do as a network?
[1747.68 → 1750.60] We've been using the heck out of Matrix this year.
[1750.60 → 1764.04] And it's a super-duper important technology for the future of the web to have, you know, a chat system that isn't beholden like Discord to whatever Discord do next year or Slack or Microsoft Teams.
[1764.22 → 1769.80] I hate to even say it, but it's a thing, you know, and they're businesses.
[1770.08 → 1771.34] They have bottom lines.
[1771.48 → 1773.10] They have some of them shareholders.
[1773.30 → 1774.12] They have to keep happy.
[1774.12 → 1787.58] And those motives are going to be at best orthogonal to what we want from it, which is a simple, permanently available forevermore kind of open chat system.
[1788.50 → 1790.52] And on top of that, self-hostable.
[1791.02 → 1791.34] Right.
[1792.30 → 1799.14] And I know we still use the Discord, but we do also have for the last six months or so a self-hosted Matrix space.
[1799.14 → 1801.84] So if you want to go over there, go find us.
[1801.98 → 1804.44] It's part of the Jupiter Broadcasting overall space.
[1804.54 → 1805.12] It's in there.
[1805.20 → 1805.68] I'm in there.
[1806.36 → 1808.08] At Alex, I think.
[1808.42 → 1809.54] Or Ironic Badger.
[1809.72 → 1810.08] I forget.
[1810.20 → 1810.66] One of the two.
[1811.18 → 1814.28] Yeah, jupiterbroadcasting.com slash matrix for easy links and stuff.
[1814.56 → 1814.98] Exactly.
[1815.40 → 1827.86] What I was going to say, though, was in 2022, we generated about $1,000 worth of affiliate revenue from CloudFree.shop and MyLocalBytes, the two self-hosting companies.
[1827.86 → 1832.56] I actually found out the CloudFree.shop guy is now full-time running that shop.
[1832.64 → 1833.50] He's quit his day job.
[1833.84 → 1834.36] That's great.
[1834.54 → 1836.68] And he's now running that website full-time.
[1836.86 → 1838.16] So hats off to him.
[1838.38 → 1847.78] But I was thinking we could split this pool of money 50-50 between a couple of our favourite open source projects, give 50% to Matrix and 50% to maybe Jellyfin.
[1848.14 → 1848.78] You know what's funny?
[1848.84 → 1850.36] I was thinking Jellyfin, too.
[1851.00 → 1853.70] I was like, because, you know, I have a Plex Pass, a lifetime Plex Pass.
[1853.70 → 1861.38] And I thought, well, if I'm going to actually switch over to using Jellyfin, which we're going to talk about in a little bit, I thought, I better make sure they're going to stick around.
[1861.92 → 1865.06] Well, the reason I was thinking Matrix is that they were pleading poverty just last week.
[1865.52 → 1866.70] Yeah, I like that, too.
[1867.10 → 1867.50] Yeah, I don't.
[1867.50 → 1872.36] But my issue is I don't feel like Patreon is appropriate for what you and I want to do.
[1872.46 → 1875.78] They also haven't updated their Patreon page, and their goals are super out of date on there.
[1875.82 → 1878.16] They look like they've reached all their goals if you go by what they have on there.
[1878.48 → 1883.12] I don't feel like Patreon is the appropriate platform for a decentralized system like Matrix either.
[1883.20 → 1883.96] I have issues with that.
[1884.46 → 1888.50] And DonorBox.org, I haven't seen this anywhere on their site.
[1888.60 → 1891.86] I haven't seen, I haven't heard anything about this, and I've been following Matrix pretty closely.
[1892.50 → 1894.44] I'm just not comfortable with these options either.
[1894.44 → 1897.68] So, I don't know, maybe Donor Box is worth checking out.
[1897.88 → 1899.26] I'll give that a look, because I agree.
[1899.36 → 1902.00] Matrix is also another one of these critical ones that we should be supporting.
[1903.18 → 1904.94] So, a huge thank you to the audience, really.
[1905.24 → 1909.56] You know, every time you buy something from one of those two shops and use the coupon code self-hosted,
[1910.34 → 1913.38] you are inadvertently supporting open source software.
[1913.48 → 1915.96] You didn't know it at the time, but that's what we're going to do with the revenue.
[1916.42 → 1917.68] You know what?
[1917.70 → 1921.06] If these turds would get on the Lightning Network, I'd put them in for our boost splits.
[1921.36 → 1924.36] I've put in several projects in LAPS splits that we talk about.
[1924.44 → 1927.32] And, you know, they'll raise a couple of hundred bucks for being in there.
[1927.52 → 1928.68] That's not nothing.
[1929.30 → 1932.02] But, ah, why don't we talk about Jellyfin?
[1932.16 → 1934.32] Because it is Jellyfin January, after all.
[1934.34 → 1937.90] And we've got people that are also trying out Jellyfin right along with us.
[1938.10 → 1939.08] A bunch of people have jumped in.
[1939.62 → 1940.36] We're halfway through.
[1940.62 → 1941.44] How's it going for you?
[1941.48 → 1943.44] We talked about it a little bit in UP on Sunday.
[1944.02 → 1945.82] 4.92, link in the show notes.
[1946.02 → 1947.02] How's it going for you today?
[1947.02 → 1952.04] You know, in a way, it just got interesting a couple of days ago for me.
[1952.04 → 1958.70] Because when we first started, I couldn't get my hands on the Swift fin native Jellyfin app for Apple TV.
[1958.86 → 1959.92] So I stuck with Infuse.
[1960.88 → 1967.46] But as soon as it came out, as soon as I realized it was out, I should say, I installed it that evening.
[1967.46 → 1977.52] And I made the switch to Swift fin, which is their brand-new iOS Jellyfin client that, as you might guess, is based on Swift.
[1977.68 → 1979.06] They're Apple's programming language.
[1979.86 → 1982.40] Boy, I have a lot of thoughts.
[1982.56 → 1983.82] It's very early.
[1984.12 → 1985.08] It's very much a beta.
[1985.80 → 1989.76] And I'd say it's probably an MVP, a minimum viable product at that.
[1989.86 → 1992.32] But it does support live TV, which I was happy to see.
[1992.86 → 1995.14] The way I would initially describe it is fast.
[1995.14 → 1997.80] Swift fin launches instantaneously.
[1998.42 → 2005.10] Shows all my libraries what I was previously watching by the time it's on the screen, which is instantaneously.
[2005.62 → 2014.76] And then the other thing that blew me away was just how freaking amazing the Scrub Fast Forward Rewind is.
[2015.02 → 2019.06] Like, I would swear that file was on the SSD of the Apple TV.
[2019.38 → 2020.70] It was unbelievable.
[2021.00 → 2023.26] I've never had performance like that from Jellyfin.
[2023.36 → 2024.76] It was top-notch.
[2024.76 → 2027.90] And, of course, it was important because still no skip intro.
[2028.54 → 2041.44] And, Alex, we could not have picked a more trying time to do this Jellyfin challenge because, you see, on a personal moral level, I refuse to watch the Enterprise intro more than three times.
[2042.00 → 2044.06] And I'm in the middle of season three Enterprise.
[2044.06 → 2047.12] And so I'm having to precision fast-forward.
[2047.88 → 2053.84] And thankfully, Swift fin is much better at that than Infuse was.
[2054.32 → 2059.64] Is Enterprise the one that we watched in Pasadena, like Work?
[2059.84 → 2061.38] No, that's the next generation.
[2061.52 → 2062.26] Oh, Enterprise.
[2062.48 → 2064.04] Is that the ancient one then?
[2064.42 → 2065.22] Enterprise is, yeah.
[2065.22 → 2068.78] Basically, they did, you know, a sequel or a prequel.
[2069.00 → 2073.54] I should say they did a prequel style with Enterprise where they went 100 years before Kirk.
[2074.22 → 2078.76] It comes later in the Star Trek franchise in terms of like air date, right?
[2078.78 → 2079.36] It's early 2000s.
[2079.36 → 2079.92] 2000s.
[2080.48 → 2083.62] But they time it earlier in the Star Trek universe.
[2083.88 → 2090.36] And they went for a Rod Stewart Rocky intro instead of, you know, remember, like, in Star Trek The Next Generation, it's that.
[2091.36 → 2094.56] Dun, dun, DA-da-dun, dun.
[2094.56 → 2094.78] Whew.
[2095.56 → 2097.38] Dun, dun, dun, dun, dun.
[2097.46 → 2097.94] Yeah, right?
[2098.36 → 2101.58] But in Enterprise, it's more of a.
[2101.84 → 2104.28] It's been a long time.
[2105.00 → 2106.60] Getting from here.
[2106.60 → 2108.54] And he's like, nope, nope, nope.
[2109.04 → 2111.38] The no skipping intro, it's a hard rule.
[2111.48 → 2112.46] We have to skip that intro.
[2112.60 → 2113.82] So we've been doing the fast-forward.
[2113.94 → 2114.40] It's working.
[2114.74 → 2120.68] I'm really, really hoping they integrate intro skipping into the actual native client when it's ready.
[2121.24 → 2124.10] I should clarify, we have a question in the chat.
[2124.48 → 2128.44] I thought there was a plug-in for Jellyfin and intro skipping already.
[2128.98 → 2130.84] And does that not work for you?
[2131.26 → 2131.76] I've gotten.
[2131.94 → 2133.30] So there is one.
[2133.30 → 2136.94] There's a couple, actually, but the most popular one is the one I have installed.
[2137.44 → 2139.78] And it will work if you're using the web UI.
[2140.18 → 2144.00] You can even install a modified web UI that'll give you a button like you have on Plex.
[2144.82 → 2152.14] And you should be able to skip intros on the set-top clients when you turn on server-side skipping.
[2152.50 → 2155.16] This plug-in allows for server-side skipping, which is awesome.
[2155.78 → 2157.20] But it's also a hard switch.
[2157.34 → 2159.04] You have, it's, all intros are skipped.
[2159.04 → 2163.14] And it happens, the service, it just forwards the client the amount of time of the intro.
[2163.84 → 2165.08] No interaction required.
[2166.18 → 2169.98] That worked the last time I deployed Jellyfin using the Linux server IO container.
[2170.26 → 2174.38] I'm using the upstream Jellyfin container this time with their upstream Docker Compose.
[2174.90 → 2176.06] And it doesn't work.
[2176.18 → 2176.68] I don't know why.
[2176.94 → 2177.74] Nothing else is different.
[2178.38 → 2184.82] I can skip intro in the web player, but I cannot skip, it does not skip intros for me on any of the set-top box players.
[2184.82 → 2189.72] So I have a little cry every night, but outside of that, the Jellyfin client was good, if not rough.
[2190.14 → 2194.40] Like, I have videos in there that are like YouTube downloads that don't have the appropriate metadata.
[2195.58 → 2198.28] And it just totally doesn't know how to display those.
[2198.46 → 2199.92] It looks like a mess.
[2200.98 → 2205.16] Well, neither does Plex, to be fair, if we're comparing apples to oranges.
[2205.16 → 2217.70] But I think if you're a developer for Jellyfin, that's probably the only real hurdle that we've found so far this month that's been, I don't want to say unsolvable, because, you know, you've got the server side thing.
[2218.22 → 2227.12] But just the way Plex does it with the audio fingerprinting and the little button that pops up in all the clients, that's the way it should be.
[2227.50 → 2227.90] It's huge.
[2227.90 → 2236.56] I'd love to see a similar option for skip credits, too, because we've just started watching a Netflix series with the kiddo called Puffin Rock.
[2237.26 → 2241.36] And, you know, it's just little puffins flying around, which she likes watching the pictures.
[2242.00 → 2247.20] But the credits on Netflix, I don't know if you've ever actually watched a real Netflix show.
[2247.84 → 2252.90] At the end of the credits, you only see about five or ten seconds, and it takes you straight to the next episode.
[2252.90 → 2258.88] But at the end of those credits, it's just like 30 seconds of black and white, boring text silence.
[2259.54 → 2263.30] So what I'd love to see would be not only an intro skip, but also a credit skip somehow.
[2263.48 → 2265.08] I don't know if that would be possible.
[2265.38 → 2269.94] Yeah, or just forwarding to the next one, you know, ten seconds into the credits or something with a countdown.
[2270.66 → 2273.72] So is the automatic intro skipping server side working for you?
[2273.88 → 2278.78] I haven't actually tried it yet, because I haven't been binge-watching any shows where that's a big problem.
[2278.78 → 2283.68] Awesome. We got a bunch of boosts about the Jellyfin challenge, so I thought I'd throw them in here.
[2283.96 → 2286.70] On boosted in with 22,222 SATs.
[2287.26 → 2290.78] It says, Gents, I wanted to call out a handy app called JellyPlex Watched.
[2291.34 → 2292.18] It's available on GitHub.
[2292.56 → 2296.02] And it lets you sync your Plex and Jellyfin watch history to each other.
[2296.28 → 2299.30] I've been using it as I run both media servers alongside each other.
[2299.36 → 2301.76] Hopefully useful as you take the plunge into Jellyfin this month.
[2301.86 → 2303.58] Keep up the amazing work.
[2304.28 → 2304.96] On, thank you.
[2304.96 → 2308.56] I've been thinking about, I have a Plex server that I maintain for family.
[2309.76 → 2315.72] And I've been thinking, depending on how this challenge goes, I might move that over to Jellyfin as well.
[2316.02 → 2320.38] They have, like, so many shows and movies and stuff.
[2320.68 → 2321.60] You know, years.
[2321.80 → 2323.10] It's a multi-year Plex.
[2323.42 → 2326.68] So it's like, I have to sync all that watch to whatever I move them to.
[2327.28 → 2328.58] I know there are a couple scripts that do it.
[2328.58 → 2339.50] But you as a server admin now, you know, the benefit of that is that you can enable on a per-profile basis the video quality that that person receives.
[2339.60 → 2344.54] So you can guarantee that they'll always transcode, although they'll never transcode if that's what you prefer.
[2345.22 → 2346.44] That is really nice.
[2346.44 → 2352.00] And that is, for me, one of the absolute killer differences between Plex and Jellyfin.
[2352.50 → 2355.06] Jellyfin assumes that I know what I want.
[2355.94 → 2357.90] And Plex is almost like the apple of the space.
[2358.04 → 2360.08] Like, here are some decisions we've taken.
[2360.62 → 2361.66] You will like them.
[2361.66 → 2363.28] And this is the way it's going to be.
[2363.62 → 2366.36] Whereas Jellyfin is a lot more like Linux in a lot of ways.
[2366.58 → 2369.16] Like, it's, for the most part, it works pretty well.
[2369.28 → 2370.80] But if you want to get under the hood and tinker.
[2371.64 → 2375.66] And for me, I've been on perfectmediaserver.com.
[2376.54 → 2381.36] I've had Plex as my number one app for the last, I don't know, two years since I launched the site.
[2382.12 → 2384.38] This week, I put Jellyfin as my number one.
[2384.56 → 2385.66] I am absolutely.
[2385.98 → 2386.64] You think it's sticking?
[2386.98 → 2388.10] I love it, dude.
[2388.18 → 2390.48] It's just so fast and responsive.
[2390.48 → 2397.78] And the only thing is, though, neither one of us have travelled while we have Jellyfin.
[2398.26 → 2400.52] I mean, for me, Tail scale will solve that problem.
[2400.94 → 2405.26] But what about when you want to watch it, like, on a hotel set-top box?
[2405.36 → 2410.80] Like, the thing is, this is what I've come to before, is I've been in hotel rooms.
[2411.04 → 2412.96] They just have Plex apps installed a lot of times.
[2413.00 → 2413.98] Or, you know, we go to an Airbnb.
[2414.36 → 2416.02] They have a smart television that has a Plex app.
[2416.08 → 2417.80] And, you know, you and I sometimes check when we go to these.
[2417.86 → 2418.90] They don't have Jellyfin apps.
[2419.16 → 2420.08] Yeah, you have a point.
[2420.08 → 2422.70] So there's that complication that could make it a little...
[2422.70 → 2425.36] So we have to keep this challenge going until March, is what you're saying.
[2427.68 → 2428.04] Maybe.
[2428.54 → 2430.94] Eric boosted in with 6,789 sets.
[2431.40 → 2432.66] I'm excited about the Jellyfin challenge.
[2432.86 → 2435.58] I'm using Jellyfin on my little Intel NUC server via Docker.
[2435.72 → 2436.68] It performs really well.
[2437.16 → 2441.18] Last week, I put Cody on a Raspberry Pi Model 3 hooked up to my TV next to my treadmill
[2441.18 → 2443.54] so I can watch my local media while I'm exercising.
[2443.76 → 2444.50] Keep up the great work.
[2444.50 → 2446.40] That's a fascinating little setup.
[2447.02 → 2451.62] I kind of almost wonder if Jellyfin is a little more resource hungry than Plex, potentially.
[2452.12 → 2455.84] But I'm also just a .NET conspiracy theorist.
[2456.16 → 2458.62] So it could just be that my .NET bias is showing.
[2459.00 → 2461.84] Null Pointer isn't switching until we're all done with the challenge, he says.
[2462.06 → 2462.54] Fair enough.
[2462.88 → 2464.00] We'll try it so you don't have to.
[2464.00 → 2468.94] And Multicast of Versus is that he's been using Jellyfin for years, but he thinks part
[2468.94 → 2471.46] of the reason why it stuck is that he's never used Plex prior.
[2471.76 → 2473.00] And Was feels the same way.
[2473.44 → 2477.20] Alex joined us on Linux Unplugged this week, and we talked a little bit about the challenge
[2477.20 → 2477.60] over there.
[2478.04 → 2479.84] And, you know, like, Was never had intro skipping.
[2480.42 → 2481.64] So he doesn't miss it.
[2482.16 → 2483.72] He never got hooked on the good sauce.
[2484.02 → 2487.80] So he also says, Rustic says that Infuse has rocked.
[2487.98 → 2490.18] It was really the game changer that let them switch to Jellyfin.
[2491.04 → 2491.98] So I agree.
[2491.98 → 2495.62] Honestly, I think at the end of the challenge, I'll probably go back to Infuse if I stick
[2495.62 → 2496.14] with Jellyfin.
[2496.96 → 2502.88] It's just a more mature video player, and it's been around for years, you know, and
[2502.88 → 2503.52] it's been refined.
[2503.70 → 2505.70] There is a yearly subscription cost, though.
[2506.12 → 2507.86] So I could see Swift fin eventually.
[2508.08 → 2508.44] Well, that's it.
[2508.50 → 2509.32] That's just it, isn't it?
[2509.48 → 2514.58] It's a pretty exciting time to be looking into this stuff with Swift fin coming out and all
[2514.58 → 2519.90] the server-side changes they've made in the last year plus since we last properly
[2519.90 → 2520.50] checked it out.
[2520.50 → 2524.78] It's the perfect timing for me because, you know, I do have a shield still.
[2525.18 → 2529.02] I used to be all shields everywhere, and I've slowly been moving over Apple TVs because
[2529.02 → 2531.14] I just think they're better boxes.
[2532.56 → 2535.44] So it's like, if we'd done this a month ago, I wouldn't have this.
[2535.76 → 2537.18] But now you're not an iOS guy anymore.
[2537.36 → 2539.28] Does that not change the equation some?
[2539.28 → 2543.60] It does stink a little bit, but you know what I've done to make up for like all the
[2543.60 → 2549.08] nice integrated controls of the Apple TV with iOS is I have a Home Assistant media playback
[2549.08 → 2554.74] widget on like my second Android screen, and that controls the Apple TV.
[2555.12 → 2560.52] So I have essentially right there on my phone playback controls for the Apple TV like I had
[2560.52 → 2560.92] on iOS.
[2560.92 → 2565.10] I can't do like AirPlay and stuff, and it doesn't do Chromecast, obviously.
[2565.74 → 2571.62] But using Home Assistant as the intermediary, I can send stuff from my Android phone to the
[2571.62 → 2573.48] Apple TV and I can control the playback.
[2573.70 → 2574.42] So that's pretty great.
[2574.86 → 2575.82] That is so cool.
[2575.90 → 2580.06] I mean, I remember in the very early days of Jodi, there was an app called, I think it
[2580.06 → 2586.60] was Yankee, Y-A-T-S-E, that you could do a similar thing with Jodi, and it was XBMC, I
[2586.60 → 2591.16] suppose, back in those days, where you could send the media from the library that you were
[2591.16 → 2595.56] browsing on your phone and basically queue it up and send it to the screen a bit like
[2595.56 → 2597.52] a Chromecast, but better.
[2598.22 → 2602.42] I love that functionality that's built into the Jellyfin mobile clients.
[2602.52 → 2603.34] It's super cool.
[2603.98 → 2604.44] What are your thoughts?
[2604.72 → 2608.96] So Schmetzfeld, and I'll probably Schmetzfeld says that he thinks that it's one to two years
[2608.96 → 2609.66] behind Plex.
[2609.66 → 2615.42] In some ways, the server side, I'd say, is certainly in that ballpark.
[2615.64 → 2616.90] Pretty good now.
[2617.16 → 2617.34] Yeah.
[2617.48 → 2618.96] I don't know if I'd say one to two years.
[2619.38 → 2624.40] Well, the server side, maybe that's a little harsh, but on the client side, definitely,
[2624.60 → 2625.36] maybe even more.
[2626.10 → 2634.26] The Android TV experience is like 95% of the way there, but it doesn't feel as nice.
[2634.40 → 2638.84] It doesn't feel like it's the difference between running your hand over a nicely finished
[2638.84 → 2643.14] piece of furniture and a piece of cheap IKEA plastic furniture.
[2644.02 → 2646.02] It's a very subtle difference.
[2646.02 → 2649.76] And for most people, that piece of plastic furniture is good enough and gets the job
[2649.76 → 2650.06] done.
[2650.52 → 2654.44] But you can't beat a properly finished piece of real oil finished wood.
[2654.62 → 2656.78] You know, there's a difference.
[2657.16 → 2658.58] It's small, but there's a difference.
[2658.98 → 2664.46] I did eventually put my Jellyfin behind a Nginx proxy so I can do SSL termination so I can
[2664.46 → 2665.36] get Chromecast working.
[2665.36 → 2665.70] Nice.
[2665.84 → 2666.82] Makes a big difference.
[2666.94 → 2668.46] So Marcel was having problems with Chromecast.
[2668.56 → 2671.54] Marcel, you might look into getting SSL set up.
[2672.00 → 2675.22] Hybrid Sarcasm, though, came in with one that I thought was great with the Jellyfin challenge.
[2675.30 → 2677.60] 10,000 sass to say, you beautiful knuckleheads.
[2678.02 → 2681.70] Spousal approval for production changes requires Apple TV apps.
[2682.12 → 2687.82] Because of this episode, I found Swift in and the evaluation will commit soon, they write.
[2688.12 → 2691.88] I won't be taking part in the Jellyfin January, but you've gotten the attention of this Plex
[2691.88 → 2692.94] lifetime pass holder.
[2693.12 → 2694.24] Cheers and keep up the good work.
[2694.24 → 2696.16] I mean, that was the aim of the challenge, really.
[2696.26 → 2701.60] It was just to raise the profile of Jellyfin a bit and encourage folks who were maybe Jellyfin
[2701.60 → 2703.40] curious to kind of give it a try.
[2704.00 → 2706.80] Certainly, I've been pleasantly surprised.
[2706.90 → 2711.86] You know, in the last episode, my expectation was that it wasn't going to stick.
[2711.96 → 2714.12] I was going to skip off the atmosphere once more.
[2714.32 → 2718.24] But here I am two weeks in and so fast, so good.
[2718.38 → 2720.62] I mean, my wife's agreed to come on the next episode.
[2720.62 → 2724.38] She is the all-important decision maker for such things in the house.
[2725.02 → 2727.36] And talk about her experience with audio bookshelf.
[2727.52 → 2730.02] I've thrust down her throat instead of prologue.
[2730.38 → 2732.16] A bunch of other small things as well.
[2732.58 → 2735.54] So yeah, if you're curious about to hear what my good lady wife has to say, she's agreed
[2735.54 → 2737.04] to come on the next episode.
[2737.04 → 2745.60] Visit CrowdStrike.com slash LCE to ingest and view all of your logs in one beautiful place.
[2745.74 → 2748.06] This is CrowdStrike's Falcon Log Scale.
[2748.24 → 2752.14] It's a new centralized log management and observability tool from CrowdStrike.
[2752.28 → 2753.34] You may have heard of Humid.
[2753.74 → 2754.32] This is that.
[2754.40 → 2755.04] It's Log Scale.
[2755.12 → 2759.62] It's developed as an alternative to legacy logging solutions that are super expensive.
[2759.62 → 2765.26] I think one of the real beauties of Log Scale is it takes logs from any source.
[2765.60 → 2768.72] All the different formats, all the different types of logs that your systems produce, all
[2768.72 → 2770.78] the different services, hardware, etc.
[2770.98 → 2772.58] You don't have to massage the format.
[2772.92 → 2774.20] You don't need to provide it a schema.
[2774.58 → 2777.92] You pump them all into Log Scale, and it figures it out and puts it in the dashboard.
[2778.08 → 2780.62] It's got a fantastic platform for this.
[2780.96 → 2782.46] And it has an index-free architecture.
[2782.74 → 2785.14] So you can ingest over a petabyte of data per day.
[2785.24 → 2787.92] And then you get to search that with sub-second latency.
[2787.92 → 2789.88] Which is so funny, man.
[2790.14 → 2792.64] I remember building Oracle databases and did this stuff back in the day.
[2793.04 → 2797.28] It just is so much better, faster, and cheaper than things like Splunk or Elastic.
[2797.62 → 2801.04] And with the reduced computational footprint, it's actually legitimately an option.
[2801.60 → 2802.52] Here's the nice thing.
[2802.92 → 2805.02] They have a Log Scale Community Edition.
[2805.54 → 2808.90] This is the largest, no-cost data ingestion offering on the market.
[2809.44 → 2815.32] Log Scale Community Edition allows you to ingest up to 16 gigs per day of logs with a
[2815.32 → 2816.12] seven-day retention.
[2816.12 → 2818.50] No credit card, no trial.
[2818.70 → 2819.80] It's just for the long haul.
[2819.84 → 2820.12] It's yours.
[2820.84 → 2822.44] Just has that seven-day retention.
[2823.00 → 2825.50] And you can pump your logs in there when you're like in the middle of building a network
[2825.50 → 2826.94] or an issue or a project.
[2827.10 → 2829.84] Like when I was trying out Home Assistant on the yellow, I thought, you know, this is a
[2829.84 → 2833.06] great opportunity to actually throw some logs in there and see what it tells me as I'm
[2833.06 → 2834.06] setting stuff up.
[2834.58 → 2838.10] It's perfect for self-hosted who are setting things up.
[2838.22 → 2839.12] Maybe you're building a network.
[2839.22 → 2840.18] Maybe you're trying something.
[2840.26 → 2842.30] You want to have some observability on the whole thing.
[2843.04 → 2844.92] But it can't be like an eight-hour job.
[2844.92 → 2845.94] You just got to get it done.
[2846.72 → 2850.90] You can go over to CrowdStrike.ice, sign up, and then you can start sending your logs in
[2850.90 → 2852.46] there and then just go check that dashboard.
[2852.98 → 2853.68] You're going to love it.
[2854.14 → 2856.80] So it's CrowdStrike.com slash LCE.
[2857.16 → 2859.72] That stands for Log Scale Community Edition.
[2860.30 → 2862.46] CrowdStrike.com slash LCE.
[2862.46 → 2870.30] One of the nicks on my Open Sense box, as we alluded to earlier in the episode, was giving
[2870.30 → 2870.98] way this week.
[2871.70 → 2876.88] So one of the gigabit nicks, for some reason, it started negotiating at 100 instead of 1,000
[2876.88 → 2879.14] and then it just dropped out.
[2879.40 → 2883.20] And so I went down to the basement, unplugged, rep lugged, and it went back to gigabit.
[2883.24 → 2884.34] And I was like, oh, cool.
[2884.68 → 2885.14] Problem solved.
[2885.26 → 2885.84] Problem solved.
[2885.84 → 2889.06] Then it did the same thing the next day, overnight.
[2889.52 → 2890.82] And I thought, oh, okay, it's the cable.
[2891.12 → 2892.64] So I replaced the cable.
[2893.92 → 2894.66] Problem solved.
[2895.18 → 2897.40] Until it did the same thing about three days later.
[2897.58 → 2898.46] I was like, oh, crap.
[2898.66 → 2899.72] It's the port, isn't it?
[2899.76 → 2900.30] It's the port.
[2900.92 → 2901.94] That sucks, Alex.
[2902.44 → 2903.72] It's a perfectly good machine.
[2904.16 → 2907.10] I should say that when I switched the cable, I also switched the port on the switch.
[2907.20 → 2909.58] So I know it's the port on the motherboard.
[2909.58 → 2914.54] And so I sort of started doing my research into firewall appliances and stuff like that.
[2914.60 → 2917.72] And I thought the easiest thing to do would just be to replace the motherboard.
[2917.94 → 2920.88] It's an Intel DQ77KB motherboard.
[2921.34 → 2924.98] I've had it now for about four, maybe, yeah, four years or so.
[2925.38 → 2927.98] And it's just worked great, actually, up until now.
[2928.06 → 2929.74] It's got an i3 third gen in it.
[2930.06 → 2931.40] It doesn't draw much power.
[2931.64 → 2933.78] It just does what it needs to do for open sense.
[2934.24 → 2935.32] So you're thinking like a part swap?
[2935.56 → 2937.02] I was thinking just swap the motherboard over.
[2938.12 → 2939.34] Can I find a motherboard?
[2940.26 → 2942.32] Well, I could on eBay in England.
[2942.74 → 2944.24] So I bought one in England.
[2945.30 → 2950.02] And my sister's bringing it with her when she comes in a few weeks to come see us.
[2951.14 → 2960.84] But I couldn't wait that long because for now, I'm running my entire infrastructure in this house through a USB Ethernet gigabit adapter through open sense.
[2961.24 → 2961.56] Attaboy.
[2962.04 → 2967.96] I've got to say, I am very impressed with open sense and its ability to just, you know, a couple of lines of config change.
[2967.96 → 2975.06] And it just changed my LAN from being, you know, EN01 to being USB Ethernet one.
[2975.06 → 2977.52] And it just picked up and didn't miss a beat.
[2977.52 → 2981.82] But it doesn't give me the warm and fuzzier with the USB Ethernet adapter.
[2982.16 → 2984.82] It's working, but I don't know for how long.
[2985.36 → 2993.70] That's definitely not a comfortable position, especially when you don't want it to break in the middle of the day when you're working from home or the wife's working from home.
[2993.70 → 2994.70] I just don't want it to break.
[2995.18 → 2995.34] No.
[2996.08 → 3000.46] Broken internet is worse than many other things in a nerd's life.
[3002.48 → 3004.02] Unless you intentionally break it.
[3004.46 → 3011.80] And so our friends over at Serve the Home have a lovely set of articles about these passive firewalls that are coming out of China at the moment.
[3011.80 → 3018.70] And I picked up one of these N5105 based systems based around the Intel Celeron chips.
[3019.22 → 3026.36] And it's got a set of four 2.5 gig i226-V nicks in it.
[3026.62 → 3030.60] So I've got four 2.5 gig nicks in my firewall.
[3031.08 → 3033.98] Now, my pipe in and out the house is only gigabit.
[3034.22 → 3035.70] You know, gigabit down anyway.
[3036.40 → 3038.18] 30 Meg up, 1,000 down.
[3038.42 → 3039.24] Ugh, spectrum.
[3039.24 → 3043.40] So I don't really need it, but I figure it's a good level of future-proofing.
[3043.52 → 3044.74] This thing is pretty cool.
[3045.06 → 3046.84] It's a completely fanless chassis.
[3047.10 → 3049.66] So it's all like aluminum fins around the edge.
[3050.12 → 3053.88] A couple of heat spreaders to transfer the heat from the motherboard to the chassis.
[3054.72 → 3055.44] So I'm hopeful.
[3055.54 → 3057.18] I paid about 300 bucks for this thing.
[3057.30 → 3059.94] It's still on the airplane over from China at the moment.
[3060.04 → 3061.90] So I'll let you know how it goes when it arrives.
[3061.90 → 3072.08] I feel like this is the year of finding Intel-based solutions for things that might have gone to an ARM machine had the supply chains not gone totally sideways.
[3072.44 → 3072.80] Yeah, maybe.
[3073.12 → 3078.32] This is a really nice little alternative to an ARM board.
[3078.32 → 3081.36] And you don't have to worry about any of those compatibility issues.
[3081.54 → 3082.58] This is looking pretty cool.
[3082.62 → 3085.20] And I like this design where it's essentially the case is the heat sink.
[3085.68 → 3095.78] So going right the way back to the start of the episode, one of the reasons I started looking at K3S and Proxmox was because this system supports PCI pass-through.
[3095.78 → 3105.68] So I'm going to finally go back to virtualizing my firewall and then also host a small subset of the K3S services on this node as well.
[3105.80 → 3107.76] I wonder if it has quick sync.
[3108.98 → 3109.72] I don't know.
[3109.78 → 3110.10] Probably.
[3110.48 → 3110.78] Do you know?
[3111.02 → 3111.28] Do you know?
[3112.54 → 3113.72] That's where my mind goes.
[3113.82 → 3115.50] I mean, yeah, firewall is nice and all.
[3117.30 → 3118.28] Can it do quick sync?
[3119.02 → 3119.64] That's great.
[3119.94 → 3122.62] And when you get it in, you'll let us know how it goes.
[3122.68 → 3124.02] You'll give us a follow-up report.
[3124.02 → 3125.72] It does have quick sync.
[3126.42 → 3126.72] Oh, good.
[3127.18 → 3130.70] Well, I expect you to stream video from your firewall then, you know?
[3131.20 → 3131.88] Well, I'll tell you what.
[3131.96 → 3142.16] When I find that Ethernet HDMI streaming adapter dongle thing that I did that we talked about a couple of episodes ago, you can bet I'll be doing that.
[3144.66 → 3145.22] All right.
[3145.24 → 3145.88] It's just feedback.
[3146.02 → 3147.78] Rotten wood boosted in 50,000 SATs.
[3147.88 → 3148.44] Love the show.
[3148.64 → 3151.68] Always find the conversations interesting and love when you all have a third set in.
[3152.32 → 3153.26] Brent, Wendell, et cetera.
[3153.32 → 3154.22] That's actually good feedback.
[3154.22 → 3162.28] I always wonder if people like, you know, the 3Bs or if they're maybe they just like it when it's just Alex and me, nice and intimate.
[3163.06 → 3165.54] Linux Teamster boosting with 5,000 SATs.
[3166.08 → 3167.74] Thanks both of you for what you do.
[3167.90 → 3168.98] I'm not really technical.
[3169.24 → 3170.08] I'm a truck driver.
[3170.08 → 3175.34] But I've always loved Linux and I love the whole idea of self-hosting and data self-sovereignty.
[3176.00 → 3179.78] My journey started with your show, and I've mostly only used the Badger stack.
[3180.28 → 3180.98] That's awesome.
[3181.30 → 3183.26] Chris and the Badger is a great comfy shirt, by the way.
[3183.36 → 3187.94] At first, it was an Ubuntu server on a Pi 4, but quickly I built a 12th gen box mostly for SATA fun.
[3188.34 → 3189.40] Also, Jellyfin's been great.
[3190.12 → 3191.92] If I can do it, anyone can do it.
[3192.08 → 3193.32] Love you both.
[3193.32 → 3194.96] Well, thank you, Linux Teamster.
[3195.22 → 3197.94] He's a Badger stack fan, Alex, he says in there.
[3198.56 → 3204.34] He's a truck driver by trade, so he doesn't have a background, so he uses the Badger stack to get his systems up and going.
[3205.38 → 3205.92] That's great.
[3206.00 → 3207.44] I love that you played around with the Pi 4, too.
[3207.52 → 3208.08] Good for you.
[3209.44 → 3210.76] You're checking all the boxes, man.
[3210.88 → 3211.74] Yeah, you love to hear it.
[3212.12 → 3216.70] Okay, so noobs wanted to follow up about my TP-Link AP that I tried.
[3216.80 → 3217.06] Oh, yeah.
[3217.08 → 3217.58] How's that going?
[3218.30 → 3219.98] Well, I ended up retiring it.
[3220.32 → 3220.56] I don't know.
[3220.58 → 3221.36] I might try it again.
[3221.50 → 3222.18] I might try it again.
[3222.28 → 3222.60] I'm not sure.
[3223.04 → 3223.20] Yeah.
[3223.74 → 3230.32] I just kept having a problem where, ironically, the TP-Link smart plugs would drop off the most.
[3230.32 → 3237.22] And sometimes that meant our room wouldn't heat because my oil heater in my bedroom is actually running off of one of those.
[3237.66 → 3241.46] So I decided to go back, but I'm still really interested in what people are doing.
[3241.46 → 3249.98] And if they have a very congested 2.4 gigahertz space and if they have smart devices running on Wi-Fi, I'd like to know.
[3250.22 → 3251.94] Are you still all Unify, Alex?
[3252.32 → 3253.02] Would you do it again?
[3253.62 → 3254.32] Yeah, I think I would.
[3254.80 → 3256.92] You know, I've been looking at different switches and stuff.
[3257.78 → 3259.56] I'm still considering Unify.
[3259.78 → 3265.26] I know we've talked a bit about them as a company in this show and some of their ethical policies and decisions and stuff.
[3265.32 → 3266.02] People love the gear.
[3266.02 → 3271.24] I've got four, five different client sites, including family members.
[3271.76 → 3274.18] I've got four APs in this house.
[3274.34 → 3276.92] You know, it would be a lot of money to rip it out and replace it.
[3277.06 → 3283.08] So for the moment, it continues to work just fine and does what I need it to do.
[3283.22 → 3284.36] So, yeah, I probably would.
[3284.76 → 3286.32] I don't know if you and I have an answer for this bit.
[3286.32 → 3298.62] Bitcoin or social boosted in 3200 stats to ask if we knew of any way to track cardio performance and like heart rate, calories burned that wasn't on one of these privacy degrading cloud services like the Fitbit stuff.
[3298.86 → 3300.92] I've been thinking about this, too, because I sleep track.
[3301.10 → 3302.62] I track my steps.
[3302.94 → 3303.68] All of that.
[3303.78 → 3305.24] I use the Apple Watch right now.
[3305.84 → 3310.30] I imagine Apple Health is fairly secure, but I'd way rather just run something on my own server.
[3310.70 → 3312.34] I don't know of anything like that.
[3312.60 → 3314.24] Well, isn't Apple all about privacy, though?
[3314.24 → 3316.74] I mean, that's what their billboards would have you believe.
[3317.10 → 3318.78] Yeah, I would just like to have it on my own.
[3318.84 → 3319.18] I'd like it.
[3319.88 → 3324.94] If it was my own data, I could maybe use it as a home assistant sensor data point.
[3325.00 → 3325.96] I could have my own graphs.
[3325.98 → 3330.48] Just feels like it'd be better if it was a device reporting to my own systems.
[3330.48 → 3334.12] If anybody has any idea of anything doing that, let us know.
[3334.50 → 3335.56] And then our last boost.
[3336.12 → 3337.12] 21 is enough.
[3337.26 → 3339.38] Boosted in with 21000 stats.
[3339.56 → 3340.16] It's a nice one.
[3340.20 → 3340.96] That's a nice round.
[3341.10 → 3341.64] Perfect number.
[3342.16 → 3343.56] Love to hear about Alfie on the pod.
[3343.56 → 3344.54] Here are some stats for me.
[3344.60 → 3345.38] Also via Alfie.
[3345.56 → 3345.78] Cheers.
[3346.00 → 3346.26] Yes.
[3346.42 → 3349.24] So if you'd like if you hear about these boost things, you're like, what the hell is this?
[3349.30 → 3350.18] What are all these boosts?
[3350.74 → 3355.72] This is a decentralized peer to peer way to send in a message to the show and give us a little bit of value.
[3355.78 → 3356.62] That's what the stats are.
[3357.00 → 3361.68] Alfie is an open source browser client that communicates with the Lightning Network.
[3362.14 → 3367.86] So you grab Alfie, you go to the podcast index page, and you can boost right there from the website and send us a message and support the show.
[3367.86 → 3376.78] And I like you saw earlier in the show, folks are trying out the Jellyfin challenge, and they're reporting in via the boost as a little bit way to give back a little value to the show while we're all doing this together.
[3377.14 → 3378.16] It's a really nice thing.
[3378.36 → 3384.08] And of course, there's a million ways you can get a hold of us, including the Matrix room, the Discord room that we've talked about and email.
[3384.08 → 3386.02] So you go to self-host. Show slash contact.
[3386.18 → 3389.42] So you pick the medium that fits you best.
[3389.94 → 3391.12] We just like hearing from you.
[3391.34 → 3393.32] And a big thank you to our SRE subscribers.
[3393.52 → 3394.60] You make the show possible.
[3394.82 → 3397.44] And I'm going to have a little goodie for all our members.
[3397.66 → 3398.52] Just a little discount.
[3398.98 → 3401.98] Coder Radio just hit episode 500, Alex.
[3402.48 → 3403.46] We're going to do the robes again.
[3403.86 → 3404.76] We're going to do the robes.
[3404.92 → 3405.48] Oh, my God.
[3405.50 → 3406.40] You're a glutton for punishment.
[3406.68 → 3407.30] What can I say?
[3407.52 → 3408.12] The last run.
[3408.22 → 3409.68] And I'm going to do a promo code for the members.
[3409.86 → 3411.66] You get an ad free version of the show.
[3412.06 → 3413.86] And probably the best part, you get the post show.
[3414.96 → 3418.74] You can sign up at self-host. Show slash SRE or support all the network shows.
[3418.82 → 3420.96] Get them all ad free at jupyter.party.
[3421.72 → 3423.96] And I finally figured out my Mastodon handle.
[3424.36 → 3427.48] It's tech hub. Social slash at ironic badger.
[3427.92 → 3428.86] Very nice.
[3429.06 → 3430.90] I'm on, I think it's Linux Rocks.
[3431.64 → 3432.28] Is that one?
[3432.44 → 3433.38] I can't remember where I'm at.
[3433.42 → 3433.82] I don't know.
[3433.86 → 3434.10] Is it?
[3434.16 → 3434.70] You tell me.
[3434.80 → 3437.08] If I can figure it out, I'll put it in the show notes.
[3437.30 → 3438.50] I've been sending people to Matrix.
[3438.70 → 3442.76] Come say hi to me in the self-hosted Matrix, jupyterbroadcasting.com.
[3442.76 → 3444.26] Like we get feedback in there.
[3444.30 → 3447.28] So sometimes I'll grab a little bit of feedback for the show, and they're all do like a little
[3447.28 → 3449.52] announcement about the live stream and let people know.
[3449.72 → 3452.22] So it's just sort of a nice little community in there and still growing.
[3452.48 → 3454.18] And we self-host that Matrix server.
[3454.64 → 3455.06] Yes, we do.
[3455.58 → 3456.64] And thanks for listening, everybody.
[3456.64 → 3459.14] That was self-hosted. Show slash 88.
