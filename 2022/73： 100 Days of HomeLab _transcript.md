[0.00 --> 6.44]  Well, welcome to episode 73, everybody. My usual co-host, Chris Fisher, is unfortunately out sick
[6.44 --> 11.92]  this week. We think he might have the rona. So please send him your best wishes. But joining me,
[11.98 --> 16.32]  I have a very special guest. I have Techno Tim. Hi, Tim. Hey, thanks for having me.
[16.58 --> 20.02]  Well, thank you. Absolutely. Last minute, I messaged Tim yesterday and said,
[20.84 --> 24.92]  yeah, Chris isn't feeling so good. Do you happen to be free tomorrow night? And
[24.92 --> 31.06]  serendipitously, he was. So here we are. So this episode, we're going to be talking about all
[31.06 --> 37.24]  things Homelab. Tim just passed 100,000 subscribers on YouTube. Congratulations.
[38.08 --> 39.70]  Thank you. Thank you. Yeah, it's crazy.
[40.02 --> 44.92]  And as part of that, I think you launched a 100 days of Homelab initiative, which we'll come to
[44.92 --> 50.00]  in just a minute. But before we get there, usual plugs for things like the Discord at selfhosted.show
[50.00 --> 54.90]  slash Discord. We've got over 4,000 people over there talking about all things self-hosted.
[54.92 --> 61.40]  Hosted, maker spaces, home assistant, all that kind of stuff. You all know as well that we've
[61.40 --> 68.04]  got a UK meetup coming up in August. The date did change due to some flight stuff with me. So
[68.04 --> 74.22]  the new date is provisionally August the 5th. We're still trying to find a venue. And now if you have
[74.22 --> 78.40]  any ideas about where we might host this thing in London, I've been ringing around a few places the
[78.40 --> 82.92]  last few days trying to find a pub with a big beer garden or something like that so that we don't have
[82.92 --> 89.04]  to hang out on like a village green or something, you know, the requirements are outdoors, has toilets,
[89.28 --> 94.70]  has beer. I think that's probably a pretty good recipe for a good meetup. So if you have any ideas
[94.70 --> 100.74]  about where we might do this in London general area, let me know. I'm on Twitter at ironicbadger.
[100.74 --> 108.36]  So remember, that's the provisional date is August the 5th. And I think that's about it. So it's
[108.36 --> 113.00]  probably about time we start talking about the 100 days of HomeLab. What madman came up with a
[113.00 --> 115.08]  100 day hour a day challenge?
[115.90 --> 121.78]  Yeah, me, I guess. You know, 100 days of HomeLab is something that I've been noodling on for,
[121.94 --> 127.52]  I'd say, about six months. You know, I'm a software developer and software developers have had a
[127.52 --> 132.74]  challenge for a while. It's the 100 days of code. And it pops up in my feed everywhere. And I think,
[132.82 --> 140.56]  what a great initiative. You know, you form a habit by doing something once a day for an hour a day
[140.56 --> 145.56]  with a goal in mind and march towards that goal for 100 days. And by the end of the 100 days,
[145.68 --> 150.76]  you'll learn something. Maybe you'll learn how to program. Maybe you build a website, whatever it is.
[151.24 --> 154.74]  Maybe you'll learn that actually you don't like the thing that you signed up to do quite as much as
[154.74 --> 159.14]  you thought you did. That is true, too. Yeah, very good point. Yeah, you might discover this is not
[159.14 --> 163.78]  for me. Like I thought programming wasn't for me in college, but now it's programming for me out of
[163.78 --> 169.34]  college. You know, I had that idea of, OK, how can I get people in the HomeLab community, one,
[169.44 --> 175.10]  together and motivated and excited about doing stuff? I'm excited. I know a lot of people are,
[175.20 --> 180.94]  but, you know, just kind of bringing people together. And the whole entire landscape of a HomeLab,
[180.94 --> 185.80]  if you think about it, it's gigantic. But, you know, I kind of think of it as networking,
[186.28 --> 192.00]  storage, infrastructure, automation, a little bit of DevOps, some hosting. You know, it's a lot of
[192.00 --> 197.40]  different things to a lot of different people. And, you know, that landscape is rapidly changing,
[197.64 --> 201.40]  you know, especially in the last couple of years, if you think of infrastructure as code or
[201.40 --> 206.82]  anything or storage, storage now in Kubernetes, storage everywhere. It's all changing,
[206.82 --> 212.82]  you know, software defined networks. And so I thought, hmm, I have 100K coming up and what can
[212.82 --> 217.24]  I do that has, you know, has as related to 100? And that's what I thought. I thought, well,
[217.34 --> 222.28]  maybe I'll launch something around then. I was six months out and I thought, you know what,
[222.36 --> 228.26]  I'm just going to do what I do best and procrastinate for six months until this, you know,
[228.72 --> 233.44]  this 100K subs if it ever comes. But it came pretty quick. So I had to get on the ball.
[233.44 --> 238.84]  Well, that's a nice problem to have. You know, I'm not sure if I've ever told this story on air,
[239.10 --> 243.98]  but I did a computer science master's. I was originally a trained musician and then did a
[243.98 --> 248.70]  few years at the Apple store and went and did a comp sci master's. One of the friends I made on
[248.70 --> 254.84]  that course went and did a PhD straight away afterwards. And his PhD was into defining DevOps.
[255.28 --> 259.84]  I don't know how he managed to swing that with his supervisor, but he did. And he got paid to do it.
[259.84 --> 267.58]  And I think this dude spent four years defining DevOps in his PhD thesis. Do you know what the
[267.58 --> 269.44]  outcome of the four years was? What's that?
[270.14 --> 272.78]  There isn't a definition. It's too nebulous.
[273.88 --> 275.38]  I like it. I like it.
[275.96 --> 279.94]  If only someone would pay me for four years to do absolutely nothing. I mean, sorry,
[280.08 --> 286.46]  sorry, Steve, if you're listening, but it's an interesting thing that you raise seriously,
[286.46 --> 293.70]  that DevOps in general means whatever you want it to mean. It really, truly it does. You know,
[293.74 --> 297.84]  to some people, it means that you're a cloud expert. To other people, it means that you can
[297.84 --> 302.00]  write Terraform code. To other people, it means that you know all about networking, right? It just
[302.00 --> 305.94]  depends on the problem that you happen to need to solve that's in front of you this week. It's
[305.94 --> 311.62]  almost like just like a buzzword, like a magic word that management don't have to hire specific
[311.62 --> 316.58]  people to do specific tasks. We want a generalist that knows a little bit about everything. And I
[316.58 --> 319.06]  think that's typically where DevOps comes in.
[319.40 --> 324.56]  Yeah, that's a good point. And it's, you know, it can be lumped as anything from getting code
[324.56 --> 330.04]  into production and whatever that means. It could be, you know, that's a huge chasm to cross.
[330.52 --> 335.60]  And it could be many different technologies. And yeah, it's a, you know, a jack of all trades type of
[335.60 --> 337.92]  role, but very needed.
[337.92 --> 341.88]  Oh, you've, you've used a database, have you? Okay. So that means you're a DBA now.
[342.04 --> 343.64]  That's right. That's right.
[344.16 --> 347.88]  So what kind of stuff have you got planned? I've seen you've done, you know, your launch video,
[347.98 --> 353.66]  your 100k subs video was pretty cool. You had 12 of the biggest home labbing YouTubers as a
[353.66 --> 358.10]  massive collaboration. You know, there's Wendell, friend of the show on there, a bunch of other
[358.10 --> 362.52]  people, Jeff from Craft Computing. What else do you have planned for the 100 days?
[363.06 --> 367.58]  I'm on day four today, you know, but for me, it was just to kind of get people
[367.58 --> 372.96]  motivated about, you know, getting into home lab, whether they are already doing it or rekindling
[372.96 --> 378.66]  that, you know, that passion they have for it. It was just kind of getting everybody on the same
[378.66 --> 384.22]  page, like created a hashtag for it. And what I'm realizing through this hashtag is, is, is that one,
[384.28 --> 388.36]  people are using it. My, my Twitter's never been so active. I don't have a lot of followers. So I'm
[388.36 --> 392.18]  like, whoa, this is how almost famous people feel.
[392.56 --> 393.26]  What is the hashtag?
[393.26 --> 398.32]  100 days of home lab. It's small, but people are using it. And what I'm discovering through this is,
[398.40 --> 403.62]  you know, these, these updates that people are giving are very similar to my daily standup to
[403.62 --> 408.02]  my scrum, you know, as a software developer, you, you know, if you do scrum, you stand up and say,
[408.18 --> 412.84]  you know, what did I do yesterday? What did I do today? And, you know, do I have any roadblocks? And
[412.84 --> 419.02]  it's, it's very awesome seeing everyone just kind of chiming in with what they're working on today,
[419.02 --> 424.32]  what challenges they're facing and then seeing other people join in and talk about how you could
[424.32 --> 429.48]  solve a particular problem or, Hey, how did that work out for you? It's just been very awesome.
[429.48 --> 435.36]  So I, I don't know what the long-term plan is. If I get to day 100 and someone is on day one,
[435.74 --> 441.30]  feel like that's a success. That means that, you know, this has gone longer than my hundred days
[441.30 --> 445.74]  and someone else's journey is starting now. And so, you know, there's a lot of people said,
[445.80 --> 448.86]  do I start with you? Don't I start with you? Start when you want. Like,
[449.02 --> 453.08]  you know, just because my train's leaving today doesn't mean your train's leaving today.
[453.22 --> 454.58]  Your train could be leaving next week.
[454.76 --> 455.16]  Choo-choo.
[455.54 --> 461.14]  That's right. That's right. And so, you know, I, I, if I get to day 100 and I see a day one,
[461.26 --> 465.84]  that means this whole thing was a success because it's, it's bigger than, than my hundred days.
[466.44 --> 471.14]  You must have some kind of an overarching goal because, you know, the time I think about when I
[471.14 --> 476.82]  was really probably the most active in terms of development over the last few years was just before I
[476.82 --> 480.82]  immigrated. Actually, I was, I was pretty stressed about the move coming up, you know,
[480.88 --> 486.38]  England to America and I just needed something to distract me. So I used, I spent hours writing
[486.38 --> 492.16]  Ansible playbooks to completely Ansible eyes the deployment of my server. And at the time it was
[492.16 --> 497.50]  mostly Ansible eyes, but I'd done it three or four years prior. So a lot of the stuff I'd learned,
[497.56 --> 501.92]  you know, as a consultant for a while, I'd learned some tips and tricks and I'd learned some new stuff.
[501.92 --> 507.62]  And I thought, right, I want to do it properly. And my goal was to do as much as I could through
[507.62 --> 512.14]  one or two commands to deploy the whole thing. Is there something like that at play for you here?
[512.64 --> 517.22]  Possibly. I mean, I, I've done some Ansible automation. I think just a couple of months ago,
[517.30 --> 522.36]  you know, I, I created an Ansible playbook to create a high availability Kubernetes cluster along
[522.36 --> 526.62]  with load balancers all in one, because I saw that as a pain point for a lot of the people that were
[526.62 --> 533.76]  using Kubernetes. So yes, it is. And so I, I found a whole bunch of forks that were left abandoned and
[533.76 --> 538.70]  I made them work. And so I, you know, automated a lot of that, but with this, you know, I'm,
[538.70 --> 544.06]  I'm not sure. I mean, for me, it was really supposed to be kind of a, you know, a celebration
[544.06 --> 549.48]  video and at the same time get people involved. But long-term, I, I honestly, I didn't think it was
[549.48 --> 553.66]  going to be, you know, turn into something as, as big as it is now.
[553.66 --> 557.52]  Well, you've got to stop coming on people's random podcasts and talking about it.
[557.52 --> 558.90]  Yeah. Stop promoting it.
[559.66 --> 564.66]  That's true. That's true. I mean, it, it, it's a great initiative. I mean, if, if, if there was
[564.66 --> 570.18]  ever, you know, some learning company that wanted to do something and, and help people and infrastructure
[570.18 --> 576.10]  do something, I'd be all for it. But, uh, honestly, no, no long-term plans. It was an idea that turned
[576.10 --> 582.26]  into a video. I got a lot of awesome people on YouTube to help me out. And that's where it stopped.
[582.26 --> 585.64]  For me, it's, it's, you know, it's, it's obviously still going.
[586.00 --> 591.44]  Sounds to me like you had this bright idea and you didn't think what happens when I release this
[591.44 --> 594.14]  into the world? Like, do I actually have to follow through on this thing?
[594.18 --> 594.62]  That's true.
[594.74 --> 598.88]  I've been, I've been, in fact, that's this show, you know, for me, I've, I'm living it, baby.
[599.10 --> 604.24]  That's right. I bet. I bet. Yeah. Like I didn't think how does this scale? What,
[604.40 --> 606.10]  you know, what's my long-term goal?
[606.34 --> 610.20]  Right. Which is ironic for someone who's as deep into Kubernetes as you are.
[610.20 --> 615.36]  Yeah. I mean, usually my, you know, my videos do okay over time, but this one did really good,
[615.44 --> 620.14]  really fast. And that's, that's not, you know, my typical, you know, release cycle for videos.
[620.34 --> 625.98]  I released a lot of videos on tutorials and how to set things up on deeper topics. So I get lots
[625.98 --> 631.60]  of views over time. Um, and you know, usually I'll get some tweets and, Hey, how did you do this? Or,
[631.94 --> 636.16]  you know, or someone on discord will ask, how do I fix this? And, you know, basically like
[636.16 --> 643.62]  async tech support. But with this one, it was like, no one needs my help. They're all doing it
[643.62 --> 648.68]  themselves. And, but at the same time, they're all joining in. So it's, it's, it's really unique
[648.68 --> 653.02]  from what I've done in the past. So at this point, I suppose it's worth kind of defining
[653.02 --> 659.56]  what a home lab is, and maybe you could tell the folks how you got into home labbing to start with
[659.56 --> 664.88]  and, you know, that kind of thing. Yeah, that's a, that's a huge topic. I even have a hard time
[664.88 --> 670.32]  describing home lab to people at work or anything else, because I think that, uh, you know, that the,
[670.32 --> 676.08]  the term has kind of evolved into a lot of things. The way I look at it is it's, uh, you know, when
[676.08 --> 681.38]  you think of, you know, you went to school, you had a computer lab there where maybe that computer lab,
[681.46 --> 686.26]  you were able to set up certain environments, um, and destroy those environments or build them up or do
[686.26 --> 690.80]  whatever you wanted to tinker in those environments. And that's kind of the idea I think behind home
[690.80 --> 695.54]  lab is that you can set up an environment, a safe place where you can set up an environment to,
[695.54 --> 702.88]  to tinker with tools or to explore new technologies or automate some, some infrastructure or geek out on
[702.88 --> 708.28]  storage and networking. It's even turned a lot into self-hosting stuff at home to people. You know,
[708.28 --> 713.52]  I, I say it too, they, they've kind of coalesced and sometimes I'll, you know, I'll say, Hey,
[713.52 --> 718.22]  yeah, I'm self like the website. I'm, I'm self hosting it in my home lab, but you know,
[718.28 --> 722.52]  it's more than a lab then at that point, you know, it's, it's, it's, it's borderline.
[722.76 --> 727.18]  Just make sure when you're tinkering, you don't take Plex down because the wife will come and find
[727.18 --> 731.20]  you. Oh yeah. Plex or DNS. Yep. That's I hear faster than my alerts.
[732.46 --> 735.46]  It's true. How do I know the wifi is off the kids are shouting?
[735.60 --> 738.04]  That's right. That's right. Oh, Plex must be done.
[738.96 --> 743.06]  Yeah. It's, it, it, it's so many things to so many different people. So it's really hard for me to,
[743.06 --> 747.66]  to kind of summarize it. Cause to me, it means something different, but, and to someone else,
[747.70 --> 751.64]  it means, you know, something different. But for me, for a long time, it's been just a place where
[751.64 --> 756.72]  I can spin up stuff and test stuff and tear it down without the fear of destroying, you know,
[756.74 --> 761.58]  the company's production. And a lot of times, if you work at a big company, you don't have access to
[761.58 --> 766.46]  a lot of this stuff, either security wise or physically, you don't have access to a lot of the
[766.46 --> 771.62]  tools. And then on top of that, a lot of the times the architecture is just, you know,
[771.62 --> 774.92]  decided before you get there. So you're just implementing stuff.
[775.64 --> 778.06]  Deleting a production VPC is a rite of passage though.
[778.14 --> 783.72]  That's right. Yeah. Yeah. Our work, sometimes Kafka accidentally gets deleted in our lower
[783.72 --> 784.20]  environments.
[784.44 --> 788.70]  But the worst thing I've ever done, I don't think I've ever said this on air, is I deleted a
[788.70 --> 789.70]  production load balancer.
[789.92 --> 790.54]  Oh yeah.
[790.62 --> 795.58]  And I didn't know what I'd done at the time. And then suddenly all the senior developers came
[795.58 --> 799.52]  out of the break room and were like, why are all of our alerts firing? I'm like,
[800.00 --> 804.18]  I was working on the load balancer. Oops.
[805.28 --> 809.80]  I've been there before where you're like, I did just make a change, but I hope it wasn't that.
[810.38 --> 816.50]  Yes. We made some changes to the CI process after that. So, I mean, you could say that Alex's screw
[816.50 --> 818.90]  up saved the company money in the long run.
[818.98 --> 821.76]  There you go. Yeah. Yeah. I'll take it. I'll take it.
[821.76 --> 826.96]  Yeah. No, I mean, you, you raise another good point. Like I think a home lab, it means different
[826.96 --> 832.08]  things to different people, much like DevOps does, I suppose. I mean, to me, a home lab
[832.08 --> 839.44]  is, I don't have a set, I mean, I suppose I do because I didn't sell the dual Xeon box
[839.44 --> 845.04]  I retired a year ago yet, but really a home lab should be separate from any kind of production
[845.04 --> 849.74]  services, you know, and I use the term production loosely at home. Although maybe it's not that
[849.74 --> 854.22]  loose because I have stuff like home assistant now and Plex, as we talked about, and a bunch
[854.22 --> 858.00]  of other stuff that I actually do rely on, you know, home assistant particularly to, to
[858.00 --> 864.18]  run multiple facets of, of my house. So a home lab to me at least is something, a space
[864.18 --> 870.80]  that I can just break stuff and it doesn't matter. And, uh, you can come all different
[870.80 --> 875.90]  shapes and sizes, right? I mean, I mentioned I had a dual Xeon box that I could use as mine.
[875.90 --> 881.22]  People use Raspberry Pis or other stuff. Oh, uh, anything. I mean, people are using old
[881.22 --> 886.86]  broken laptops without a screen. Uh, some people are using, uh, old PCs. My, my recommendation
[886.86 --> 892.36]  most of the time when people say, um, um, I want to build a home lab is, well, just upgrade
[892.36 --> 896.84]  your current PC. So you get an upgrade, you know, and on the machine you use the most and
[896.84 --> 900.30]  use the one that's sitting over there for your home lab, you know, have that be your first
[900.30 --> 903.80]  one. And you get two for one, you get two for one, you get an upgrade on your main machine.
[903.80 --> 908.08]  Then you get a pretty nice machine for your home lab. And that's probably going to outperform a lot
[908.08 --> 911.52]  of the things that you would, you would buy otherwise, you know, or spend a lot on.
[911.92 --> 917.56]  I was just thinking about upgrading, you know, consumer grade gear. And the thing that runs out
[917.56 --> 922.90]  first in a home lab scenario always is memory. You always run out of Ram first. And, you know,
[922.94 --> 927.34]  you think about using an old laptop because it's got a built-in screen, a built-in keyboard,
[927.46 --> 931.68]  a battery for as a UPS, that kind of stuff. But it can typically only have 16,
[931.68 --> 936.68]  maybe 24 gigs of Ram if you're lucky. Yeah. That's not enough to do a whole bunch with.
[936.96 --> 940.80]  Yeah, no. But a lot of people getting into it are just getting started. You know,
[940.84 --> 946.08]  it might be enough to run a hypervisor, you know, three, four Linux virtual machines and
[946.08 --> 950.42]  enough to kind of tinker with something else, you know, and not destroying their own production
[950.42 --> 956.82]  machine. But, you know, it spans the gamut. There's used enterprise gear. Some of my old PCs
[956.82 --> 961.96]  got converted into rack mount PCs and now they're in my server rack, you know, all the way to new
[961.96 --> 966.66]  enterprise, which I've even bought before. Super micro servers sometimes are pretty affordable.
[967.08 --> 970.98]  But then, yeah, all the way down to Raspberry Pis too. I have four or five of those. So it's,
[971.22 --> 978.40]  I, you know, I generally think it can be any computing device, I think, can be used mostly
[978.40 --> 985.92]  in a lot of the same ways. Now over at wiki.selfhosted.show, we have an SS8 guest storage
[985.92 --> 991.18]  leaderboard. At the top of the list, we've got Wendell with a petabyte who's clearly just showing
[991.18 --> 997.78]  off and nobody's going to touch that. But I have to ask you, Tim, how many terabytes do you have
[997.78 --> 1006.28]  on your LAN of raw storage? Oh, good question. I have a lot of RAM. My disk shelf alone has 40 terabytes.
[1006.28 --> 1010.16]  I forgot you had that disk shelf. I mean, there's one, there's one of your videos,
[1010.30 --> 1015.72]  goes back about a year or so now, I think, where you do an amazing job of taking us through all the
[1015.72 --> 1020.16]  different boxes you have in your rack. And you've even got some pretty cool LED lighting in that
[1020.16 --> 1024.50]  server room, if I recall. Yeah, yeah, yeah. It's, it's, it's, yeah, it's pretty wild. It's similar to,
[1024.58 --> 1029.70]  it's overkill, but it looks cool. Yeah, it is. It is. You know, when I first started making content,
[1029.84 --> 1033.30]  a lot of gamers were doing it. And I, you know, I play games too. And I thought,
[1033.30 --> 1037.64]  we can't let all the gamers have fun. People with servers can have fun too. And
[1037.64 --> 1041.92]  RGBs is how they have fun. No. Tim, it'll see any video game I need, baby.
[1042.14 --> 1048.96]  Yeah, that's right. That's right. Or the, uh, uh, Chrome, the, the dinosaur when you're offline.
[1050.24 --> 1054.78]  But, uh, yeah, I think I'll, I'll stick with 40 terabytes. I mean, I, I know I have, you know,
[1054.78 --> 1061.54]  a handful in desktops around here and Macs and laptops, but it's, I can account for 40 right off the
[1061.54 --> 1065.98]  top of my head. There's no way I'm getting close to a petabyte. I'm sure Geerling, Geerling is there
[1065.98 --> 1071.16]  now too as a petabyte. That's right. With this petabyte pie project. My goodness. That was a
[1071.16 --> 1075.28]  cool video. It was. Yeah. Incredible. Incredible. But yeah, I can't touch those.
[1077.50 --> 1083.52]  Linode.com slash SSH. Go there to get a $100 60 day credit on a new account and support the show.
[1084.30 --> 1087.82]  Linode has been rolling out upgrades to NVMe storage on their rigs recently,
[1087.82 --> 1093.08]  which offers much greater performance density or IOPS per gigabyte than traditional storage.
[1093.60 --> 1097.34]  If you're a performance hound or your application needs that level of storage throughput,
[1097.84 --> 1101.68]  Linode's team can help you sort through the possibilities for accessing the power of NVMe
[1101.68 --> 1105.20]  and arriving at the optimal storage configuration for your environment.
[1106.06 --> 1111.50]  The Linode support experience truly is one of the most remarkable things about Linode as a company.
[1111.82 --> 1116.46]  No matter what time, what day it is, you can open a ticket with Linode and know that they'll
[1116.46 --> 1120.42]  take care of you. No matter how silly you've been, whether you've decided to try and install
[1120.42 --> 1125.78]  your own custom operating system on one of their nodes that is not supported, they'll still try and
[1125.78 --> 1131.10]  help you. I can't imagine opening a ticket with some of the other big hyperscalers asking how I'd go
[1131.10 --> 1137.24]  ahead and install some random distro and actually get a coherent reply from a human. Linode's been doing
[1137.24 --> 1142.96]  this for a long time, 18 years in fact, and they just keep getting better. Go try it for real and
[1142.96 --> 1149.76]  see for yourself at linode.com slash SSH. Linode makes it simple, affordable and accessible to deploy and
[1149.76 --> 1155.64]  manage your customers' projects in the cloud. Linode also has an easy to use and powerful cloud dashboard
[1155.64 --> 1162.38]  with S3 compatible object storage, bare metal servers, cloud firewalls, DDoS protection and so much more.
[1163.04 --> 1169.04]  In fact, we use Nextcloud here at the network to run the backend for all of our show storage. So when our editors
[1169.04 --> 1173.74]  need our files, for example, they'll go and pull it down from Nextcloud. And that's backed by Linode's
[1173.74 --> 1179.80]  fantastic S3 object storage. It just means as an administrator of a Nextcloud server, I don't have
[1179.80 --> 1185.18]  to worry about how much disk space is free. I just know that Nextcloud can go and create a new object
[1185.18 --> 1191.22]  in the bucket and we're all good. And with pricing 30 to 50% cheaper than the other major cloud providers,
[1191.84 --> 1197.22]  Linode can be part of your multi-cloud strategy. Use our $100 credit to performance test your network
[1197.22 --> 1202.20]  so you can see just how good Linode is for yourself. Go and grab yourself that $100 credit
[1202.20 --> 1209.06]  and 60-day free trial over at linode.com slash SSH. That's linode.com slash SSH.
[1211.36 --> 1217.78]  Now, I think the thing that I found you for first was Kubernetes content. You were doing a bunch of
[1217.78 --> 1225.60]  stuff with Rancher, I think, at the time and K3S. As an OpenShift guy, you know, at work, obviously my
[1225.60 --> 1230.78]  propensity is to use OpenShifty type stuff. But actually, I do like to try and keep my skills
[1230.78 --> 1235.64]  in the real Kubernetes world without a lot of the OpenShift magic that goes on with the rooting layer
[1235.64 --> 1240.94]  and all that kind of stuff. And so that leads me down the path of looking at K3S. And I always,
[1241.08 --> 1246.90]  always, always find myself in this dichotomy of, I want to have something at home to learn on,
[1247.64 --> 1250.04]  but my goodness, is this complicated and overkill?
[1250.04 --> 1257.48]  So, you know, it is. Well, it could be. But I ask, you know, what is overkill? Is overkill 40 terabytes
[1257.48 --> 1263.74]  of storage? Is overkill a V8 engine in your car? Is overkill, you know, half a terabyte of RAM?
[1264.02 --> 1269.64]  You know, what is overkill? So, you know, yeah, I've made a lot of K3S content and you hit the nail
[1269.64 --> 1275.72]  on the head. Like when I built my Ansible playbook for K3S, it was to solve a lot of the complexity of
[1275.72 --> 1280.16]  setting it up because there's a lot of complexity in just setting it up, let alone everything you
[1280.16 --> 1286.80]  need to know about Kubernetes later on. But I think K3S is a, one, it's a fantastic product. It's an
[1286.80 --> 1292.88]  easy, lightweight way, air quotes on lightweight, way to run containers on the edge. You know, with it,
[1292.96 --> 1299.08]  you get a full, mostly full Kubernetes API. And, you know, for a lot of things, it might seem overkill.
[1299.08 --> 1305.94]  Hey, I'm running one container of everything in my, you know, my Docker stack or Portainer or
[1305.94 --> 1310.04]  whatever you're using to manage your Docker containers. But what happens if you want to run
[1310.04 --> 1315.14]  two? What happens if you want to make sure that they're always up? What happens if you want to
[1315.14 --> 1321.06]  do that declaratively and, you know, create YAML for all your deployments so it's repeatable?
[1321.28 --> 1326.18]  How do you handle storage, you know, on your single node? Single node's pretty easy,
[1326.18 --> 1331.96]  but, you know, how do you handle it if you have more than one? And so, you know, Kubernetes asks
[1331.96 --> 1336.92]  a lot of those questions of containers and you're left to kind of figure it out. But for the most part,
[1337.02 --> 1341.76]  once you get going with it, I think, you know, like, like me, when I caught the DevOps bug or
[1341.76 --> 1347.10]  engineering bug or software development bug, you know, it's something that you can go really deep on
[1347.10 --> 1352.42]  really fast and maybe never come back from. It definitely is a lot of fun, but it, it,
[1352.42 --> 1354.10]  there's a lot of learning involved.
[1354.10 --> 1359.24]  I always find myself thinking, right, I've got two or three Raspberry Pis sat in the drawer.
[1359.98 --> 1364.90]  And the whole purpose of doing this would be to have a highly available, I don't know,
[1365.26 --> 1370.20]  Git server, web server, whatever it is, basic services like that. I don't think I would do
[1370.20 --> 1375.14]  things like Home Assistant in, in Kubernetes because it's, it's best suited as its own VM.
[1375.36 --> 1380.88]  And we'll just, we'll forget about that. But there are certain services in the, in my
[1380.88 --> 1386.42]  overall kind of self-hosting world that would be pretty cool. It, you know, at the moment I run
[1386.42 --> 1391.58]  everything on my storage server. So if, if a disk fails, I have to take that thing out and, and
[1391.58 --> 1397.40]  shoot it in the, no, I don't do that. I take the disk out and the machine's offline for an hour or two,
[1397.44 --> 1403.26]  or maybe longer. If I'm doing some data transfer, I will actually stop all the containers on that box
[1403.26 --> 1406.52]  so that nothing's reading and writing to merger FS and doing all that kind of stuff.
[1406.52 --> 1414.42]  And I find myself thinking in those moments, which admittedly is only once a month for a few hours
[1414.42 --> 1420.78]  at most, I think, oh, I'd be great if this was self-healing and that web service had just moved
[1420.78 --> 1426.10]  over here and its underlying storage had also replicated and also done all, and it's just those,
[1426.40 --> 1430.70]  all those extra thoughts of, well, but then I need to solve this problem and then I need to solve
[1430.70 --> 1434.94]  that one. And then I need a load balancer and then I need to replicate the storage and all that
[1434.94 --> 1442.24]  kind of stuff. So what's the lowest barrier of entry to a highly available Kubernetes setup in a
[1442.24 --> 1447.18]  home lab scenario? Oh yeah, good question. So, I mean, you hit the nail on the head with all the
[1447.18 --> 1451.80]  challenges you'll start to face. Those are the known ones. There are a lot of ones you don't know
[1451.80 --> 1458.04]  until you get into it, but the lowest barrier of entry, I think the minimum available, there's a
[1458.04 --> 1463.20]  couple of ways you can do it. With K3S, you can use etcd for your, your, your Kubernetes database,
[1463.20 --> 1468.94]  or you can use a MySQL database, which is external. At the end of the day, you need at least three
[1468.94 --> 1473.60]  nodes for Quorum for them to vote. But if you're using the MySQL version, you don't need Quorum
[1473.60 --> 1480.44]  because the MySQL database acts as your database. So you nodes don't need to vote or it is the tiebreaker.
[1481.18 --> 1488.66]  So how does that work? etcd is explicitly designed for Kubernetes, or at least that's the way it feels.
[1488.66 --> 1493.06]  I know it wasn't originally, but it's very lightweight. It's very good at maintaining
[1493.06 --> 1498.38]  Quorum and the performance at scale is excellent. MySQL, not so much.
[1499.02 --> 1503.72]  Yeah, no, I, I totally agree. So if you choose the etcd route, it's going to be very chatty,
[1503.88 --> 1509.02]  but highly available. It's going to be replicating all of the data across all of those nodes.
[1509.28 --> 1515.14]  It will have some kind of performance impact if you're using Raspberry Pis with microSD cards,
[1515.14 --> 1520.88]  probably not the best storage for something that reads and writes often. But with MySQL,
[1521.20 --> 1527.12]  if you have it there, you can run that anywhere. It becomes your state for where these nodes go and
[1527.12 --> 1532.84]  look up their state. And then your database for everything in Kubernetes. But I think the performance
[1532.84 --> 1539.16]  is good enough, good enough for nodes and good enough for K3S. I think otherwise they wouldn't
[1539.16 --> 1545.20]  have chosen it. I suppose I get caught up sometimes in, you know, thinking about this from my day job
[1545.20 --> 1549.88]  and thinking that I must do things properly. I must do it with etcd when actually probably MySQL,
[1550.74 --> 1554.74]  certainly from your description there, sounds actually like in some cases it might be a decent
[1554.74 --> 1559.38]  choice. So what do you do? Do you put MySQL on its, you know, let's say you've got three Pis running
[1559.38 --> 1563.86]  K3S. Do you then have a fourth that's just dedicated as a single node for MySQL?
[1563.86 --> 1568.78]  Well, if you're doing MySQL, you could do two nodes with a MySQL database anywhere in the
[1568.78 --> 1571.92]  environment that it can communicate with. It doesn't even have to be a Kubernetes node.
[1572.12 --> 1576.36]  So you can have two Raspberry Pis and then your MySQL database wherever, anywhere else,
[1576.38 --> 1579.26]  as long as it can reach, you know, MySQL over TCP.
[1579.64 --> 1581.58]  And how's the complexity of setting up that replication?
[1582.28 --> 1585.60]  You don't have to do anything. There's nothing you need to do. With K3S,
[1585.72 --> 1591.64]  all of that is obfuscated from you in general, like with etcd or MySQL. You don't need to know
[1591.64 --> 1596.22]  how to do that or how to set it up. Not saying that, you know, you might not have to troubleshoot
[1596.22 --> 1602.50]  it sometimes, but for the most part, it's pretty solid. I'm a huge fan of the etcd way because,
[1603.14 --> 1607.72]  you know, you can spin up nodes, add nodes. And I mean, you could do that with the MySQL version.
[1608.22 --> 1612.74]  More industry standard too. So if we come back to one of the original goals of learning,
[1613.42 --> 1618.60]  right, if you're doing things at home in a very custom way, you could argue that certain
[1618.60 --> 1623.80]  businesses and certain shops will have a huge amount of custom code. Certainly older,
[1623.90 --> 1628.78]  more legacy shops from, let's say, more than 15 years old, let's say, before the cloud was really
[1628.78 --> 1633.00]  a thing. They'll have a lot of on-premise infrastructure that you'll go and you'll read
[1633.00 --> 1637.78]  the wiki if they have one and you'll scratch your head and be like, why did you do it that way?
[1638.42 --> 1641.06]  Because 20 years ago, there was no other way, mate. That's why.
[1641.78 --> 1642.64]  Yeah, exactly.
[1642.64 --> 1648.82]  So, you know, there is that to contend with. If you think about doing the MySQL route is it's not
[1648.82 --> 1654.84]  an industry standard way of doing things, whereas etcd is. So, you know, you've got a few pies now
[1654.84 --> 1658.40]  running K3S with, let's say, etcd as the backend. What next?
[1658.74 --> 1663.52]  So the next thing I highly recommend doing is going and figuring out storage. Well,
[1663.74 --> 1666.06]  there's two pieces. It's choose your own adventure.
[1666.20 --> 1669.52]  Remember I said the terminal is the only video game I need, baby. You see what I mean?
[1669.52 --> 1676.22]  Yeah. So those are the two things. And I recommend people like figure that out up front. I know most
[1676.22 --> 1681.20]  people when they build a cluster, they don't even have K3S in mind and maybe they do, but they're
[1681.20 --> 1686.20]  more focused on the service that they want to run. They want to run WordPress or Ghost or Plex maybe.
[1686.72 --> 1690.36]  And so they're really focused on that. And sometimes I have to remind people, okay,
[1690.64 --> 1694.70]  before you do that, figure out storage and load balancing, because that's, that's tough to figure
[1694.70 --> 1699.50]  out. I would probably say figure out storage too, because almost every stateful,
[1699.52 --> 1704.54]  stateful applications. So stateful applications in Kubernetes are ones that write state or keep
[1704.54 --> 1709.98]  state in memory. But for ones that write to a volume to disk, you need to figure out storage
[1709.98 --> 1715.66]  and you can do the, Hey, put it all in NFS, but then you're taking, you know, you're taking this
[1715.66 --> 1721.54]  highly available service K3S and making it, you know, putting in a single point of failure,
[1721.54 --> 1726.42]  which is probably your NFS. It's the same thing with MySQL too. And when we were talking about that
[1726.42 --> 1729.78]  earlier, the reason why I don't choose that is because you're just, you know, you're taking
[1729.78 --> 1733.12]  something that's highly available and all of a sudden you're making a single point of failure,
[1733.24 --> 1739.46]  be your MySQL server. And then you have to make your MySQL server HA to make that HA. And so it just
[1739.46 --> 1745.66]  grows exponentially. It depends on how, how, how rigid you are about making things highly available.
[1745.66 --> 1751.26]  And so you, you, you have a lot of choices, you know, but for storage, it's really going to be
[1751.26 --> 1755.72]  up to you. If you want to make it highly available, you could dump everything in NFS and that's fine.
[1755.82 --> 1760.82]  Or you could choose things like Rook, Seth or, or Longhorn there, there, there are options.
[1761.60 --> 1767.98]  Why, why didn't I take the blue pill? That's often what I end up thinking at 2am when I've started
[1767.98 --> 1775.68]  one of these ludicrous adventures down that particular rabbit hole. Yeah. So let's presuppose
[1775.68 --> 1782.18]  that, uh, we now have a running Kubernetes cluster with a load balancer, uh, with storage and
[1782.18 --> 1787.74]  everything's working. We've got a completely empty cluster. Now what, where do people find apps to
[1787.74 --> 1792.96]  actually run on this thing that are compatible with Kubernetes? Yeah, good question. So most, um,
[1793.02 --> 1797.80]  most, I'll say most, uh, air quotes, most containers that are, are built on Docker,
[1797.98 --> 1803.36]  um, are compatible with Kubernetes because Kubernetes under the covers is now using a
[1803.36 --> 1807.56]  different container runtime. It's not important, but it's compatible with Docker images and Docker
[1807.56 --> 1812.32]  containers. So one, anything you were previously running in Docker most likely is going to run in
[1812.32 --> 1816.82]  Kubernetes. I mean, that's how it was designed to work. Something you'll need to pay attention to.
[1816.84 --> 1821.90]  And I kind of hinted at it a little bit was, was, you know, stateful applications. You'll need to make
[1821.90 --> 1827.10]  sure that that application you have can scale. Everybody thinks like, Oh, you know, I'm running Plex.
[1827.10 --> 1832.22]  The way to make it highly available is spin the replicas up to three. It's not going to work.
[1832.94 --> 1837.76]  It's not going to work. Yeah. So if, if things weren't built to be stateless, you're not going
[1837.76 --> 1841.50]  to be able to scale them. You'll get some other benefits, like they could bounce around on nodes,
[1841.54 --> 1846.42]  but you can only run one. So it's almost a bit like raid in that regard, right? It's not designed
[1846.42 --> 1852.50]  to increase your resilience necessarily. It's designed to increase your uptime. That's right. So the whole
[1852.50 --> 1858.56]  sales pitch behind Kubernetes that kind of got me excited about it in the beginning was let's say
[1858.56 --> 1864.08]  you had a Plex instance running on node one and node two and three are just sat there chilling out,
[1864.16 --> 1869.80]  doing nothing. Node one has a hardware failure and Kubernetes is running a loop constantly checking
[1869.80 --> 1875.80]  the state of these things. And every time that loop executes, it's saying right on node one,
[1875.80 --> 1883.24]  this pod exists, Plex exists, and it matches the state declared in the YAML file that Alex put in
[1883.24 --> 1888.28]  place. Cool. Everything's hunky dory and it will carry on doing that loop. I don't know what the
[1888.28 --> 1894.62]  frequency is, but it's many times a minute that that typically happens. Now what happens when node
[1894.62 --> 1901.46]  one has a hardware failure or drops off the network or just crashes if the application crashes for some
[1901.46 --> 1905.98]  reason? Well, Kubernetes is going to come around and do its health checks and make sure that everything's
[1905.98 --> 1910.98]  tickety-boo and it's going to say, hang on a minute, the desired state over here doesn't match what I'm
[1910.98 --> 1916.64]  expecting. Well, what I'm going to do is I'm going to utilize a different node that matches the node
[1916.64 --> 1921.14]  selector rule that you've put in here. Let's say it's a node with quick sync for transcoding, for example.
[1922.00 --> 1927.94]  Not every node in your cluster might have a GPU available to do that. The loop will go around and it will
[1927.94 --> 1933.92]  say, hey, okay, well, out of the five nodes in this cluster, I can use these two. And now I'm going to
[1933.92 --> 1937.48]  take the Plex pod and I'm going to make sure it's destroyed over there, but I'm going to spin up a new
[1937.48 --> 1942.10]  one over here. And then I'm going to tell you that that happened in your log and alert you about it.
[1942.76 --> 1948.32]  That's generally speaking, the typical use case for a stateful application in Kubernetes. Like Tim was
[1948.32 --> 1954.82]  saying, it's not to have three copies of Plex running at the same time because the database writes.
[1954.82 --> 1959.82]  And like, if you think about how the data would flow in that transaction, you're coming in to
[1959.82 --> 1965.26]  watch video. Well, which version of the Plex runtime are you hitting? And then that version of the Plex
[1965.26 --> 1970.16]  runtime is probably got its fingers in the database somewhere. And how does the database know which one
[1970.16 --> 1976.34]  to listen to? And it can get very confusing very quickly, which is why a lot of dev shops have to
[1976.34 --> 1984.10]  architect things in a way called the 12 factor app. If you're interested, go and look at 12 factor app.net.
[1984.10 --> 1989.24]  I think that's the website. Hang on. Yeah. Yeah. Good site. Good reference to 12 factor.net is the
[1989.24 --> 1995.62]  website. There'll be a link in the show notes. There are a few different ways to run containers
[1995.62 --> 1999.98]  on Kubernetes. Like you were saying, OCI compliant containers. Typically that's mostly Docker containers.
[2000.34 --> 2006.58]  There are a few others under the covers as well. There is a project called Kubernetes at home,
[2006.64 --> 2011.22]  which there'll be a link to in the show notes, Kate's at home. And this is a fantastic resource.
[2011.22 --> 2016.34]  If you're not familiar with it, go check it out. You can go over there and download Helm charts and all
[2016.34 --> 2022.66]  sorts of other stuff to run applications on top of your Kubernetes cluster. And a lot of other smart
[2022.66 --> 2027.44]  people have done a lot of the legwork for you thinking about how do I run an application that
[2027.44 --> 2034.04]  wasn't designed for the Kubernetes world to make it run in the Kubernetes world, stuff like user
[2034.04 --> 2038.86]  management. You know, we're all familiar with the group and user ID stuff from a normal Linux
[2038.86 --> 2043.70]  Docker host. There's some tweaks you've got to make in the Kubernetes world to translate that
[2043.70 --> 2048.70]  stuff across multiple nodes because it's not just typical Linux permissions, right? There's a,
[2048.78 --> 2053.54]  there's an extra layer on top and there's, there's lots of other small gotchas like that. Like,
[2053.84 --> 2056.98]  you know, like Tim was saying, you know, there's plenty of stuff that you don't know what you don't
[2056.98 --> 2062.22]  know until you find out you don't know it. And it's a, it's a deep rabbit hole, but it's one that if
[2062.22 --> 2067.64]  you've got any interest in, I highly recommend you give a look to Tim's channel as well as the
[2067.64 --> 2072.94]  Kubernetes at home stuff that's linked in the show notes. Yeah. Like I've worked with
[2072.94 --> 2078.14]  Kubernetes at home folks, a couple of them there. I'm in their community. That's how I got bit by
[2078.14 --> 2083.52]  the flux bug, you know, and declaratively defining your whole entire Kubernetes cluster through
[2083.52 --> 2088.18]  manifest. Yeah. That's a great call out. The Kubernetes at home helm charge are fantastic,
[2088.36 --> 2093.02]  especially for people self-hosting because they went after a lot of the services that people are
[2093.02 --> 2097.70]  self-hosting. And if you just want normal, you know, I shouldn't say normal, but publicly available
[2097.70 --> 2102.96]  helm charts that, you know, for services like NGINX and, you know, all these enterprise services,
[2103.10 --> 2107.72]  those are out there. Those helm charts are out there. But what the Kates at home helm charts are,
[2107.84 --> 2111.94]  they're going after, they're going after Plex, they're going after, you know, Sonar, Radar,
[2112.04 --> 2116.62]  like all these services that people like to run at home and building charts for them. And if you even
[2116.62 --> 2122.20]  search some of the helm chart repository aggregators, they referenced their charts too. So yeah,
[2122.20 --> 2127.60]  they've been a huge help in getting me onto flux, which is a totally different topic, but it's
[2127.60 --> 2131.32]  pretty far down the rabbit hole. I got absolutely hooked by these guys when I found out I could run
[2131.32 --> 2136.42]  a Factorio server on my Kubernetes cluster. I just thought it was the coolest thing in the world.
[2136.86 --> 2141.64]  So talk to me a bit about GitOps and flux and that kind of thing. We've talked to, obviously,
[2141.74 --> 2146.22]  I rambled a lot a minute ago about, you know, declarative state and how there's this loop
[2146.22 --> 2152.00]  in Kubernetes that is constantly checking the state of things. GitOps takes that to another
[2152.00 --> 2159.38]  level, right? It does. So GitOps is a lot more defined, I guess, than DevOps. So GitOps is this
[2159.38 --> 2168.50]  idea that you define your cluster state or your environment state in manifest 100%. And the way
[2168.50 --> 2177.18]  that you influence the state of a cluster or infrastructure is by doing it through Git. So
[2177.18 --> 2183.24]  for example, I just went through this exercise, you know, I needed to get, let's just say an Nginx
[2183.24 --> 2191.24]  container, I would add an Nginx manifest, whether I'm using Helm or Kubernetes manifests, I would create
[2191.24 --> 2196.72]  that manifest, I would create that manifest, I would commit it to Git, and I would push it up. And then
[2196.72 --> 2202.74]  there are services within Kubernetes that say, hey, I just got this manifest, I'm looking at the current
[2202.74 --> 2208.28]  state, I'm looking at the desired state, and I will apply it. And so GitOps basically says that you,
[2208.60 --> 2214.40]  the only way you can influence state is really by influencing Git, but they say through a pull
[2214.40 --> 2222.02]  request could be anyway. But now my whole entire cluster at home is that way. And I think the benefit
[2222.02 --> 2228.16]  of that is that I can reproduce my whole entire Kubernetes cluster by just saying, you know,
[2228.16 --> 2234.14]  kubectl apply or use Flux to do it all over again, and rebuild my whole entire cluster. Now,
[2234.30 --> 2239.90]  data is a different story, I would have to do some restores on data to get those, those persistent
[2239.90 --> 2245.40]  volume claims back. But at the end of the day, I have my whole entire playbook for how to build my
[2245.40 --> 2250.18]  cluster. You know, if you're running your own cluster, you can do one offs and do all these weird
[2250.18 --> 2252.04]  stuff. You know, you know how it is to tinker.
[2252.04 --> 2257.30]  That's just it. That's just it. GitOps at home might seem like massive overkill,
[2257.56 --> 2261.20]  just like ansibilizing your server might seem massive overkill when it's just you.
[2261.34 --> 2261.80]  That's right.
[2261.84 --> 2266.48]  But if you take these principles into the workplace, I guarantee you it's going to make you more
[2266.48 --> 2272.16]  employable, you'll earn a bigger salary. But as a team, it just makes your life so much easier,
[2272.16 --> 2277.34]  because you're not like, who's done this to the load balancer? Alex, was it you? No, it's in Git.
[2277.40 --> 2280.42]  You can go and look at GitBlaim and you know that it was Tim that broke the load balancer,
[2280.42 --> 2286.08]  not Alex this week. Yeah, don't let him. Yeah. And it's nice because, you know,
[2286.14 --> 2291.48]  places I've worked at, sometimes developers have full access to Kubernetes, which is fine. That's
[2291.48 --> 2297.36]  a choice made by the company. But anyone can then go kubectl apply or kubectl delete everything,
[2297.36 --> 2302.36]  and then it's gone. You know, and so GitOps basically says no more of that. We're separating
[2302.36 --> 2306.50]  our concerns. You know, if you want to get things into Kubernetes, you do it through Git,
[2306.50 --> 2311.52]  and then you use, you know, a controller or service to apply those to Kubernetes. So it's,
[2311.88 --> 2315.76]  it's very interesting. It's very, it's very bleeding edge. And a couple of places are doing
[2315.76 --> 2320.72]  this now for a couple, you know, Flux is one, Argo CD is another. And I'm sure there's a handful
[2320.72 --> 2325.20]  of others that are coming up. Even GitLab themselves does it. Portainer does it for Docker. I mean,
[2325.50 --> 2329.94]  this is a hot topic, but it's, it's really awesome. But at the end of the day, now as a developer,
[2329.94 --> 2334.98]  I'm like, okay, I can't, I can't make changes to Kubernetes directly, which I'm fine with. I'm fine with
[2334.98 --> 2342.04]  process. It has upsides and downsides. The upside is like you say, everything is declarative and it
[2342.04 --> 2348.08]  makes rebuilding stuff really, really easy. The downside is you have to make every single change
[2348.08 --> 2354.42]  that way, no matter if it's a one character change to a config file and whatever your peer review
[2354.42 --> 2358.96]  process is, you know, in a home lab, it's likely to be you going, yes, yes, mash, mash, mash. Yes,
[2359.02 --> 2363.38]  yes, yes. Whereas at work, you know, you might have to get your team lead to approve it and,
[2363.38 --> 2367.62]  you know, explain why you miss the semicolon off the end of a line or whatever it might be,
[2368.14 --> 2372.54]  you know, that kind of thing. So it has its upsides and downsides. I think for me,
[2372.58 --> 2376.68]  the upsides do outweigh the downsides simply because of everything we've talked about.
[2377.44 --> 2383.24]  Yeah, I agree. I agree. My, my notes section that I used to have on how to reconfigure my
[2383.24 --> 2391.10]  Kubernetes cluster in the case of an event is gone. It used to be a long list of helm commands that I
[2391.10 --> 2397.60]  used to run kube control, you know, commands that I run along with manifest manifest. And now that's
[2397.60 --> 2403.10]  just gone. It's just no, my, my documentation is the code. And I, I hate it when people say that,
[2403.16 --> 2407.00]  but it's true. Now, now my code is the documentation and documentation is the code. There's,
[2407.12 --> 2411.38]  there's no other way to do it. Well, it's the source of truth. It's the most up-to-date version
[2411.38 --> 2417.12]  of what's in production. I mean, the only other more truthful source would be actually production,
[2417.12 --> 2421.30]  but if you've been doing it all through GitOps anyway, they should be the same.
[2421.68 --> 2426.76]  That's right. Yeah. Yeah. It's a, it's pretty strict principle, but I, I, I enjoy it. You know,
[2426.84 --> 2430.72]  Argo CD is another one that I I've been wanting to play with. It's, it's pretty cool. It's,
[2430.80 --> 2435.34]  it's a lot more visual, you know, even before I was doing give up GitOps, I would still deploy
[2435.34 --> 2441.74]  stuff through Kubernetes. I had still use CI CD, you know, pipelines, commit manifests,
[2441.74 --> 2446.92]  and then have, you know, a kube control apply during CI. This is a little bit different and it's,
[2446.92 --> 2449.32]  it's pretty awesome. Pretty awesome. It's fun to explore.
[2452.56 --> 2458.14]  Talescale.com slash self-hosted. Go there to get a free personal account for up to 20 devices and
[2458.14 --> 2463.20]  support the show. Talescale is one of my absolute favorite discoveries of the last 12 months. It's
[2463.20 --> 2469.18]  a zero config VPN. You can install it on any device in minutes and manage the firewall rules for you.
[2469.18 --> 2474.08]  And it works from anywhere. I've been able to close all the ports in my firewall, thanks to the
[2474.08 --> 2478.84]  outbound nap punching that Talescale does. And this means that no matter where I am in the world,
[2478.94 --> 2485.58]  I can connect to my LAN as if I'm sat in this chair. And it is so great. I can hardly explain
[2485.58 --> 2492.20]  to you guys. I can also, thanks to their amazing subnet router technology, connect to the Synology
[2492.20 --> 2496.54]  box running at my mom's house or the server I have running at my dad's house as if I'm on their
[2496.54 --> 2502.38]  LANs as well. For me, one of the best parts is every device on my network gets a stable IP and
[2502.38 --> 2508.06]  auto-assigned domain that stays consistent no matter what network the device is on. Devices
[2508.06 --> 2512.08]  only connect after signing in through your existing identity provider. This means you
[2512.08 --> 2517.24]  can more easily enforce multi-factor authentication and deauthorize those who you've shared things
[2517.24 --> 2522.38]  with who you perhaps wish you hadn't. You can try it for yourself for free for up to 20 machines
[2522.38 --> 2528.78]  at talescale.com slash self-hosted. And just imagine, what if this is how the internet worked?
[2528.78 --> 2535.46]  What if every machine had a static IP and a DNS name? And that address migrated around the world
[2535.46 --> 2540.94]  with you? And it was always encrypted? And you never had to worry about certificates? And all of
[2540.94 --> 2546.12]  this just happened automatically? That's Talescale. So go and try it out for yourself for free for up
[2546.12 --> 2549.46]  to 20 machines at talescale.com slash self-hosted.
[2549.46 --> 2557.04]  Jerry writes in, hey guys, in response to the Wi-Fi enabled e-ink device mentioned in episode 72,
[2557.20 --> 2563.10]  I thought you should check out pine64.org slash pine note. Hey, Jerry, I just want to say thanks
[2563.10 --> 2567.00]  for writing in with this one. I mean, I know the conclusion that Chris and I came to in the last
[2567.00 --> 2572.10]  episode was that for the most part, wherever you're going to want an e-ink display, there's going to be
[2572.10 --> 2579.34]  power and therefore a cheap tablet might make more sense. But if you really, really do want an e-ink
[2579.34 --> 2585.98]  display, you can go ahead and look at this pine note developer edition. It is $400. So what we were
[2585.98 --> 2591.84]  saying about e-ink displays being expensive definitely holds true with this device, but it does look cool.
[2591.94 --> 2597.96]  And obviously, you know, supporting the pine project is a noble endeavor. Those guys do great work over
[2597.96 --> 2602.60]  there. So you can go ahead and take a look at the link in the show notes to the pine note.
[2603.86 --> 2608.24]  And Joshua also writes in, I've been running Linux since high school and I've been self-hosting
[2608.24 --> 2613.46]  almost as long. I am currently getting my master's in cybersecurity engineering and I've been using the
[2613.46 --> 2619.54]  skills I learned to try and make my systems more secure. One tool I learned about recently is Linus.
[2619.88 --> 2626.12]  I think that's how you say it anyway. L-Y-N-I-S. This scans your configs and gives you suggestions to
[2626.12 --> 2631.64]  improve your security. Do either of you run any tools to help ensure you aren't making any obvious
[2631.64 --> 2637.00]  security mistakes? Now, Tim, I know that you do some stuff like this in your day job. I wondered if
[2637.00 --> 2642.26]  you had any suggestions for Josh. Yeah, great question. I was actually working on this today.
[2642.54 --> 2647.76]  There are a lot of tools you can use to do analysis on the things you use. For example,
[2648.32 --> 2654.84]  I was setting up container image scanning today to scan Docker containers to look for vulnerabilities,
[2654.84 --> 2662.14]  known vulnerabilities that are higher critical and if they were addressed or not. So there are lots of
[2662.14 --> 2667.14]  things you can do like that. You can scan them either at rest in a container registry or you can
[2667.14 --> 2672.76]  scan them even during runtime if they're in Kubernetes. And then if you are writing code, there's a lot of
[2672.76 --> 2679.22]  static code analysis tools you can use too as well to scan and look for vulnerabilities in either your
[2679.22 --> 2685.40]  code or dependencies that you're using for your code. Trivia is one that I was using today to set
[2685.40 --> 2691.34]  up and it's really, really awesome. And it's open source and they do a lot of scanning of a lot of
[2691.34 --> 2696.98]  different types. They're kind of an all-in-one now where they can scan code, dependencies, and containers.
[2697.52 --> 2700.64]  So now when we see a video come out from you in a few weeks' time on that, I'll be like,
[2700.64 --> 2706.54]  hey, you heard it here first. You know, I think for me, cybersecurity is one of those things. Like
[2706.54 --> 2712.50]  it's obviously a buzzword in certain areas, but just not being the tallest nail is the name of
[2712.50 --> 2717.44]  the game. Don't do silly things like open ports in your firewall you don't absolutely need. I mean,
[2717.54 --> 2722.88]  for me, since discovering Tailscale, I've actually been able to close every single port in my firewall.
[2723.06 --> 2726.66]  Like I don't have anything open anymore, not even WireGuard like I used to,
[2726.66 --> 2731.72]  because Tailscale does all the outbound nat punching that I need to get past my own firewall
[2731.72 --> 2737.00]  so I can connect to my LAN as if I'm, you know, here wherever I am in the world, which is just
[2737.00 --> 2741.70]  great. So stuff like that, you know, don't open ports in your firewall, I think is a super basic
[2741.70 --> 2747.66]  but really important principle. There's also stuff like using SSH keys or certificates if you want to,
[2747.80 --> 2753.12]  using TLS to make sure it is actually your website that you're connected to through Let's Encrypt.
[2753.12 --> 2758.18]  There's really no excuse these days not to. But I think beyond that, just don't be the tallest nail.
[2758.34 --> 2764.88]  Don't use a silly, stupid password like password123. At least make some basic effort. That kind of thing.
[2764.94 --> 2768.34]  Use a password manager, that kind of stuff. I think that's all you need to do, really.
[2769.40 --> 2770.50]  So Jackin writes,
[2770.50 --> 2785.18]  Jackin, I almost shed a tear on the last episode of Lass. I've got to be honest with you. I know Chris isn't here,
[2785.60 --> 2789.08]  but I was a huge fanboy of JB for many years before starting this show.
[2789.74 --> 2794.06]  And I owe a lot of what I can say and talk to about Linux, I think, to JB as a whole.
[2794.06 --> 2797.98]  So I feel you there, man. I feel you there. Now, he continues,
[2798.28 --> 2802.74]  on episode 71, a listener asked about thoughts on alternatives to the Raspberry Pi.
[2803.56 --> 2808.92]  I think the Orange Pi makes a decent low-cost board. They sell for around 24 bucks and you can
[2808.92 --> 2814.66]  get them directly from the manufacturer. Now, Tim, I know you're a bit of a pie fiend as well as I am
[2814.66 --> 2818.34]  and Chris too. Have you ever heard of these Orange Pies?
[2818.74 --> 2823.50]  You know, I've heard the name, but I can't tell you how they differ.
[2824.06 --> 2831.06]  I can't. Yeah, I have lots of Raspberry Pis. I even have a Turing Pi too. And the only
[2831.06 --> 2837.60]  non-Pi device I have is an NVIDIA Jetson. But I haven't heard of them. I need to look into them,
[2837.72 --> 2841.06]  especially if they have a better supply than Raspberry Pis right now.
[2841.34 --> 2845.74]  Well, that's just it, isn't it? Raspberry Pis are unobtainium. So no matter how much we might
[2845.74 --> 2851.50]  wax lyrical about them, if you can't find them, then it's pretty much no good to anybody. So
[2851.50 --> 2856.56]  yeah, maybe these Orange Pies are the way to go. They look like a pretty cool board. They're ARM64
[2856.56 --> 2862.04]  based, which is, you know, it can be a bit of a problem sometimes to find applications to run on
[2862.04 --> 2867.76]  these things. But for a small little headless box, maybe they'll do the trick. Who knows?
[2868.16 --> 2872.34]  If you have been running an Orange Pi in anger, please write in and let us know at
[2872.34 --> 2878.08]  selfhosted.show slash contact. Now, I want to say a huge thanks to Tim for stepping in at the last
[2878.08 --> 2880.62]  minute here to help me co-host the show. Thank you, Tim.
[2880.98 --> 2882.48]  Yeah, thanks for having me. Huge fan.
[2882.80 --> 2886.32]  Is there anywhere else you'd like to send people? I mean, I imagine you've got some channel on YouTube.
[2886.72 --> 2891.74]  Yeah, yeah. Channel on YouTube. Yeah. Just Google Techno Tim or use your favorite search
[2891.74 --> 2896.28]  engine and look for Techno Tim or just Techno Tim. Live. That's an easy way to get a hold of me.
[2896.78 --> 2898.96]  Well, very good. Thank you very much for joining us. Now,
[2898.96 --> 2903.76]  I want to say also a big thank you to our Site Reliability Engineers, our SRE subscribers. You
[2903.76 --> 2910.06]  make the show possible over at selfhosted.show slash SRE. You can also go and support the entire
[2910.06 --> 2915.64]  Jupiter Broadcasting Network over at Jupiter.party. Don't forget as well that we have the London
[2915.64 --> 2920.40]  Meetup coming up on August the 5th. More details to follow on that soon. And again,
[2920.46 --> 2925.82]  if you have a venue recommendation, please, I would love to hear it. As always, you can get in touch
[2925.82 --> 2930.36]  with us at selfhosted.show slash contact. That's the place to go to get in touch with us. And you
[2930.36 --> 2935.82]  can find me on Twitter at Ironic Badger. I'm at Techno Tim live on Twitter. Very good. And thanks
[2935.82 --> 2939.48]  for listening, everybody. That was selfhosted.show slash 73.
