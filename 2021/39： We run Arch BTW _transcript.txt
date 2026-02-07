[0.00 --> 3.52]  Coming up on today's show, we cover our favourite LastPass alternative,
[4.14 --> 7.50]  we talk about why more boxes might be better than one,
[7.72 --> 10.98]  and we confess our undying love for Arch.
[11.86 --> 12.46]  I'm Alex.
[12.76 --> 15.28]  And I'm Chris, and this is Self-Hosted 39.
[30.00 --> 45.44]  I, too, I, too, Alex, have been worshipping at the altar of Arch recently.
[45.58 --> 47.84]  After experimenting with various different distributions,
[48.52 --> 50.80]  I like that I can set up a minimal system,
[50.80 --> 56.46]  and I actually have been enjoying using Arch as my base application server.
[56.84 --> 58.42]  I don't run apps directly on Arch,
[58.42 --> 61.96]  but in containers or VMs, I find it to be a fantastic platform.
[62.06 --> 63.04]  I've been doing it for a while now.
[63.64 --> 66.16]  This comes hot off the heels of this week's Linux Unplugged,
[66.24 --> 70.40]  where I think it's fair to say you got in your soapbox and preached the Arch gospel.
[70.74 --> 71.70]  I don't know.
[71.94 --> 75.22]  I think what I got in my soapbox about was
[75.22 --> 77.96]  it's become kind of a joke or a meme,
[77.96 --> 82.26]  oh, Arch users, people are just trying to flex and talk about how elite they are,
[82.76 --> 85.14]  when the reality is that's not it at all.
[85.14 --> 89.42]  I simply just want something that makes it really quick to get software deployed or up and running,
[89.54 --> 92.96]  and maybe have the most minimal Linux install before I run an application.
[93.14 --> 96.96]  And I find it great for that, without sort of all of the upfront work
[96.96 --> 99.62]  that something like Gen 2 or Linux from scratch takes.
[100.08 --> 100.88]  Hey, bro, bro, bro.
[101.50 --> 102.52]  I run Arch, by the way.
[103.02 --> 103.40]  Yeah.
[103.74 --> 105.16]  Well, that's kind of how it started.
[105.60 --> 109.18]  And then it became, it kind of grew from there, didn't it?
[109.32 --> 109.72]  It did.
[109.72 --> 111.50]  Yeah, I definitely feel the shame.
[111.50 --> 114.22]  Like, when you say to people, I run Arch,
[114.32 --> 118.34]  it's not because you want to flex, or at least I don't want to flex.
[118.76 --> 121.74]  It's because I just love it so gosh darn much,
[121.74 --> 124.78]  and I think other people would too if they just gave it a chance.
[125.14 --> 126.04]  Well, why is that?
[126.08 --> 128.36]  I think we should talk about, maybe just really briefly,
[128.52 --> 129.88]  why it is you love it so much.
[129.90 --> 132.02]  Because it's not the forms, right?
[132.04 --> 134.94]  It's not the Arch user base, necessarily.
[135.14 --> 136.96]  It's the practicality of it, right?
[137.38 --> 137.78]  It is.
[137.78 --> 142.88]  I am one command away from pretty much any piece of software that I want.
[143.72 --> 146.28]  Yay-S, everything, literally.
[147.16 --> 150.44]  You know, the AUR is Arch's secret sauce.
[151.08 --> 151.98]  Think of anything.
[152.14 --> 153.06]  Think of a custom kernel.
[153.36 --> 156.86]  You know, VFIO stuff is pretty complex to get into.
[157.46 --> 159.46]  There is a custom kernel already compiled,
[159.68 --> 163.16]  or there's a package build to compile a custom kernel already there for you,
[163.18 --> 163.66]  ready to go.
[164.36 --> 167.00]  You want some esoteric piece of software that,
[167.00 --> 168.96]  on Ubuntu would be a PPA,
[169.30 --> 171.26]  or on Fedora would be a copper repo.
[171.78 --> 173.32]  I don't have to worry about any of that.
[173.38 --> 175.28]  It's just yay-s install,
[175.56 --> 176.56]  and off you go.
[177.54 --> 180.34]  And besides that, you know, as a new user,
[180.46 --> 183.06]  when I was getting into Linux in 2013,
[183.38 --> 184.64]  14 sort of time period,
[185.46 --> 186.38]  the Arch documentation
[186.38 --> 189.48]  is just the best around,
[189.48 --> 191.82]  and it's crowdsourced.
[192.02 --> 193.98]  It's not always completely accurate
[193.98 --> 195.80]  and always completely totally up to date,
[195.86 --> 196.82]  but it's good enough
[196.82 --> 200.24]  that even an idiot like me can pick it up
[200.24 --> 200.96]  and get going
[200.96 --> 202.94]  when I knew basically nothing.
[203.60 --> 204.36]  And at that point,
[204.40 --> 206.50]  that was when Arch had just transitioned to Systemd.
[206.50 --> 210.52]  So I kind of credit Arch and Systemd and Docker
[210.52 --> 212.44]  as being the three kind of pillars
[212.44 --> 213.84]  of what got me into Linux
[213.84 --> 216.82]  and being able to get me over that initial new user
[216.82 --> 218.58]  not knowing what I'm doing hump.
[218.84 --> 220.26]  Those three things together,
[220.46 --> 223.24]  for me, were just game-changing.
[223.84 --> 225.22]  There really is a Linux for every type.
[225.34 --> 227.02]  Obviously, there's benefits
[227.02 --> 228.54]  to running something like Debian
[228.54 --> 232.46]  or CentOS or Ubuntu LTS on a server
[232.46 --> 234.40]  that make just a ton of sense for most people.
[234.92 --> 235.94]  I'm the type of user,
[236.04 --> 238.16]  I don't mind logging in at least once a week,
[238.78 --> 240.02]  doing a package update
[240.02 --> 242.90]  and seeing what needs to be installed.
[243.38 --> 245.62]  I don't always have time for that.
[245.62 --> 247.68]  I don't always get to do it weekly,
[247.86 --> 249.38]  but I generally am able to do it
[249.38 --> 250.46]  at least once a month,
[250.50 --> 251.40]  if not twice a month.
[251.40 --> 254.00]  And that seems to be all it's taken for me
[254.00 --> 255.60]  to keep these systems up and running.
[255.66 --> 256.78]  And the benefit that I get
[256.78 --> 258.52]  from a self-hosting standpoint
[258.52 --> 261.72]  is my operating system is continuously updated.
[261.84 --> 264.08]  I don't have this event
[264.08 --> 265.80]  that comes up every few years
[265.80 --> 267.80]  where I kind of brace myself
[267.80 --> 270.42]  and do this massive upgrade.
[271.10 --> 272.54]  Instead, I take my medicine
[272.54 --> 274.10]  kind of on a weekly basis
[274.10 --> 276.78]  and it kind of stretches out the changes
[276.78 --> 278.00]  so that they're just more minor.
[278.12 --> 278.70]  They're more frequent,
[278.86 --> 280.06]  but they're more minor.
[280.06 --> 281.44]  I prefer that.
[281.44 --> 282.64]  And then when you add something
[282.64 --> 283.36]  like Alex was saying,
[283.46 --> 283.94]  the AUR,
[284.32 --> 286.42]  with the package management system,
[286.60 --> 289.40]  I can get something up and running
[289.40 --> 291.68]  in moments on Arch
[291.68 --> 294.38]  that would take a bit of fiddling around,
[294.48 --> 295.44]  maybe adding a package repository,
[296.36 --> 298.14]  following a guide to add the keys
[298.14 --> 299.24]  and all that kind of stuff
[299.24 --> 300.50]  to a machine.
[300.62 --> 302.08]  And then I have the joy
[302.08 --> 303.76]  of watching that repo go by
[303.76 --> 305.30]  every time I do an apt update
[305.30 --> 306.38]  or a DNF update.
[306.50 --> 308.44]  And I'm not a huge fan of that system.
[308.44 --> 308.90]  It works.
[309.54 --> 310.78]  And for some people,
[310.82 --> 311.46]  it works really well.
[311.60 --> 312.82]  For me, I just like to have it
[312.82 --> 314.66]  all integrated with a single package manager,
[315.22 --> 316.80]  single set of updates that I do.
[317.08 --> 319.60]  And it's always guaranteed to be
[319.60 --> 320.94]  at least close to guaranteed,
[321.06 --> 321.62]  I should say,
[321.88 --> 322.74]  the latest version
[322.74 --> 323.62]  when I install something.
[323.82 --> 325.18]  So I know the security stuff's
[325.18 --> 325.68]  taken care of,
[325.72 --> 326.36]  the feature stuff
[326.36 --> 327.36]  that I've been reading about online,
[327.40 --> 328.58]  I know it's already landed.
[329.12 --> 330.86]  And then anything that's more complex
[330.86 --> 332.78]  than a basic system level tool,
[333.02 --> 335.44]  I'm already loading in a container anyways.
[335.44 --> 337.68]  Anyways, and those are often based on Alpine
[337.68 --> 338.98]  or Ubuntu, et cetera.
[339.12 --> 340.56]  And it kind of doesn't really matter
[340.56 --> 341.72]  what the host OS is running
[341.72 --> 343.30]  as long as it's secure and up to date.
[343.64 --> 345.88]  I kind of view Arch a little bit like
[345.88 --> 347.42]  stock Android.
[347.96 --> 349.86]  You know, like on a Pixel phone
[349.86 --> 351.48]  or, well, not OnePlus anymore,
[351.76 --> 353.10]  but definitely on the Pixel phones.
[353.28 --> 355.10]  Like, it has no opinion.
[355.42 --> 356.68]  There's no opinionation really
[356.68 --> 357.54]  in how it does stuff.
[357.60 --> 358.62]  It just gives you stuff
[358.62 --> 360.08]  and lets you figure it out by yourself.
[360.72 --> 361.86]  And for that reason,
[361.98 --> 363.58]  it makes a really great
[363.58 --> 364.66]  minimum viable server.
[365.38 --> 366.32]  It also makes
[366.32 --> 367.94]  a really great workstation.
[368.36 --> 370.70]  It could make a great cloud box
[370.70 --> 371.82]  because you can only install
[371.82 --> 373.48]  very, very minimal numbers of packages.
[373.74 --> 375.08]  So from a security perspective,
[375.72 --> 377.40]  there's a smaller attack surface.
[378.16 --> 380.44]  The downside is that the industry,
[380.64 --> 382.40]  and I use air quotes around industry,
[383.32 --> 384.20]  in the cloud at least,
[384.36 --> 386.52]  does seem to be settling on Ubuntu.
[386.52 --> 387.84]  Like if you look at market share
[387.84 --> 388.68]  and stuff like that.
[389.20 --> 391.00]  So you are kind of
[391.00 --> 393.20]  trailblazing your own path
[393.20 --> 394.28]  by going with Arch.
[394.48 --> 397.06]  But I would argue that
[397.06 --> 398.22]  what distro you run
[398.22 --> 399.56]  doesn't really matter
[399.56 --> 400.38]  that much anymore.
[400.74 --> 402.36]  I mean, I do feel pretty strongly
[402.36 --> 403.02]  that, you know,
[403.06 --> 404.50]  all my systems will just run Arch.
[405.28 --> 406.38]  You know, if it's a laptop
[406.38 --> 407.30]  or a desktop or whatever.
[407.46 --> 408.22]  But if it's a server,
[408.94 --> 410.32]  I'll probably put Ubuntu on it.
[410.88 --> 412.22]  Even though everything
[412.22 --> 412.98]  we've just said,
[413.10 --> 416.08]  because it has canonical behind it
[416.08 --> 417.12]  doing a bunch of testing,
[417.58 --> 418.80]  especially when it comes to ZFS
[418.80 --> 420.08]  and the licensing there.
[420.34 --> 421.20]  That's a tricky one,
[421.20 --> 421.96]  even on Arch.
[422.48 --> 423.44]  Just a bunch of stuff,
[423.52 --> 424.04]  a bunch of testing
[424.04 --> 425.04]  and things like that
[425.04 --> 427.04]  mean that I don't run Arch
[427.04 --> 428.16]  absolutely everywhere,
[428.68 --> 429.60]  just most places.
[430.08 --> 431.28]  I have found that for the cloud,
[431.40 --> 433.06]  I'm sticking with Ubuntu LTS
[433.06 --> 434.12]  for the most part.
[434.32 --> 435.54]  I find that works really well.
[435.88 --> 437.06]  And for my Raspberry Pis
[437.06 --> 438.66]  that are at the RV
[438.66 --> 440.44]  on an LTE connection,
[440.84 --> 442.98]  I'm also running Ubuntu LTS there
[442.98 --> 444.48]  in part because they've done
[444.48 --> 445.56]  a really good job
[445.56 --> 447.48]  with their Pi support.
[447.48 --> 450.16]  But also, less updates
[450.16 --> 451.74]  is a feature when you're on cellular.
[452.26 --> 452.66]  Yeah.
[453.02 --> 454.34]  And I'm already updating
[454.34 --> 455.70]  my laptop enough as it is.
[456.18 --> 457.72]  So there's those elements of it.
[457.86 --> 459.24]  But when I have an opportunity
[459.24 --> 460.58]  to run local physical hardware,
[460.66 --> 461.72]  like I do here at the studio,
[461.80 --> 462.38]  it's all Arch.
[462.80 --> 463.80]  It works fantastic.
[464.24 --> 465.72]  I do have one Arch box
[465.72 --> 466.56]  up in the cloud
[466.56 --> 468.22]  that is like an example
[468.22 --> 469.72]  of Arch in the cloud gone wrong,
[469.86 --> 473.02]  where the vendor tried to pin
[473.02 --> 474.72]  to a certain version of the kernel.
[474.82 --> 475.14]  And of course,
[475.16 --> 475.76]  that just doesn't work
[475.76 --> 476.44]  very well with Arch.
[476.86 --> 478.14]  So I think it is a little trickier
[478.14 --> 478.54]  in the cloud.
[478.60 --> 479.84]  And it's not a 100% solution.
[480.42 --> 481.86]  And what I was just advocating
[481.86 --> 482.92]  now, I guess, here
[482.92 --> 483.66]  and in that episode
[483.66 --> 484.68]  of Linux Unplugged
[484.68 --> 487.90]  is let's not mock people
[487.90 --> 489.06]  for their choice of distribution.
[489.24 --> 489.96]  There's functionality
[489.96 --> 491.34]  behind everything
[491.34 --> 493.38]  and like perfectly good reasons
[493.38 --> 494.44]  to run SUSE as well.
[494.96 --> 496.54]  My buddy on Coda Radio, Mike,
[496.92 --> 498.30]  that's what he prefers to run.
[498.40 --> 499.86]  He likes SUSE in the enterprise.
[500.08 --> 501.70]  He runs Pop! OS on his desktop
[501.70 --> 503.42]  and SUSE in the rack.
[503.60 --> 504.96]  And that works really well for him.
[505.40 --> 506.46]  It's not like we're trying
[506.46 --> 507.38]  to create a
[507.38 --> 509.08]  this distribution is better debate.
[509.36 --> 510.46]  What we're trying to say is
[510.46 --> 511.84]  let's include everybody
[511.84 --> 512.72]  in the conversation
[512.72 --> 513.76]  and not mock people
[513.76 --> 515.58]  for their choice of distribution.
[516.00 --> 517.26]  And as a couple
[517.26 --> 518.28]  of counter-narrative guys,
[518.36 --> 519.74]  I guess we happen to find Arch
[519.74 --> 520.70]  actually works pretty well
[520.70 --> 521.88]  if you're willing to maintain it.
[523.62 --> 525.94]  Linode.com slash SSH.
[526.04 --> 527.14]  Go there to get a $100
[527.14 --> 528.14]  60-day credit
[528.14 --> 528.88]  towards a new account.
[529.00 --> 530.86]  Yeah, $100 in credit
[530.86 --> 531.38]  to play with.
[531.72 --> 532.12]  And of course,
[532.12 --> 533.08]  you're supporting the show
[533.08 --> 535.50]  by going to linode.com slash SSH.
[535.70 --> 536.70]  That's where we set up
[536.70 --> 537.58]  all of our infrastructure
[537.58 --> 538.68]  for JB 3.0.
[538.80 --> 539.62]  If we're playing around
[539.62 --> 541.22]  for something like SSH,
[541.30 --> 542.52]  like segment work or something,
[542.94 --> 544.54]  yeah, we do that up on Linode.
[544.64 --> 545.84]  And speaking of Arch,
[545.88 --> 546.74]  one of the great things
[546.74 --> 547.46]  about Linode
[547.46 --> 548.48]  is they let you pick
[548.48 --> 549.40]  just about any distribution
[549.40 --> 549.92]  you want.
[549.98 --> 550.56]  They have Arch.
[550.94 --> 551.52]  They got, I mean,
[551.52 --> 552.04]  they got everything.
[552.16 --> 553.18]  Alpine, Debian,
[554.08 --> 554.86]  CentOS, SUSE,
[555.30 --> 556.18]  Ubuntu's, of course.
[556.46 --> 557.08]  I mean, they got like
[557.08 --> 558.06]  everything up there.
[558.44 --> 559.52]  Even some Fedora
[559.52 --> 561.02]  for you crazy kids out there.
[561.14 --> 562.58]  You can run it up on Linode.
[562.66 --> 563.66]  They've been in this game
[563.66 --> 564.70]  since 2003.
[564.88 --> 566.32]  They've learned what works
[566.32 --> 567.40]  and they've learned
[567.40 --> 568.34]  what doesn't work.
[568.38 --> 569.40]  And they were doing that
[569.40 --> 571.10]  years before everybody else.
[571.26 --> 572.58]  And they've really managed
[572.58 --> 573.44]  to modernize it
[573.44 --> 575.30]  with a beautiful cloud dashboard
[575.30 --> 576.22]  that makes it approachable
[576.22 --> 576.60]  to somebody
[576.60 --> 577.88]  who's brand new to servers
[577.88 --> 579.56]  or maybe you're like
[579.56 --> 580.28]  a longtime pro.
[580.68 --> 581.22]  You're going to love
[581.22 --> 582.40]  the way this dashboard works.
[582.52 --> 582.76]  Of course,
[582.80 --> 584.44]  they have native SSD storage,
[584.54 --> 585.48]  40 gigabit connections
[585.48 --> 586.56]  coming into the machines.
[586.96 --> 588.30]  It's all super fast.
[588.56 --> 589.38]  And because they've been around
[589.38 --> 590.34]  since 2003,
[590.52 --> 592.46]  they've got some great locations.
[592.62 --> 593.72]  Like, think about that, right?
[593.74 --> 594.50]  They can leverage
[594.50 --> 595.28]  their experience,
[595.40 --> 596.08]  their relationships
[596.08 --> 597.94]  in a way that nobody else can
[597.94 --> 598.82]  because they've been
[598.82 --> 599.62]  in cloud computing
[599.62 --> 600.94]  before it was cloud computing.
[601.20 --> 602.10]  11 data centers
[602.10 --> 602.88]  around the world.
[603.12 --> 603.76]  We got an email
[603.76 --> 604.88]  into the show from James.
[605.76 --> 606.10]  He said,
[606.16 --> 606.92]  I wanted to set up
[606.92 --> 608.56]  an SMTP relay
[608.56 --> 610.08]  at my previous
[610.08 --> 611.70]  VPS provider,
[612.30 --> 614.20]  but because they were
[614.20 --> 615.28]  kind of, you know,
[615.48 --> 617.00]  trying to be competitive
[617.00 --> 617.58]  in the market,
[617.72 --> 618.78]  they ended up
[618.78 --> 619.66]  with not the best
[619.66 --> 620.66]  IP reputation
[620.66 --> 621.76]  and they ended up
[621.76 --> 622.28]  getting blocked
[622.28 --> 622.92]  by Microsoft.
[623.20 --> 624.10]  And so then he spun up
[624.10 --> 625.60]  another box on their system
[625.60 --> 626.68]  and that also got blocked
[626.68 --> 627.42]  by Microsoft.
[629.12 --> 629.62]  He's like,
[629.64 --> 630.54]  I couldn't even find them
[630.54 --> 631.58]  on any public blacklist.
[631.64 --> 632.88]  Yet Microsoft just started
[632.88 --> 634.78]  blacklisting all of these IPs.
[634.78 --> 635.70]  So I decided I'd go over
[635.70 --> 636.24]  to Linode
[636.24 --> 638.44]  and try a Linode over there
[638.44 --> 639.14]  and support the show.
[639.22 --> 639.88]  So he goes to
[639.88 --> 641.56]  linode.com slash SSH.
[641.70 --> 642.94]  He spins up a system
[642.94 --> 643.34]  on Linode
[643.34 --> 643.86]  and he discovers,
[644.06 --> 644.34]  oh,
[644.34 --> 646.44]  Linode has a policy
[646.44 --> 647.16]  where they block
[647.16 --> 648.66]  all SMTP related ports
[648.66 --> 649.32]  by default.
[649.46 --> 650.06]  Oh, well,
[650.36 --> 651.20]  I guess I'll email support
[651.20 --> 652.14]  and see what they say.
[652.28 --> 652.92]  So he sends off
[652.92 --> 653.88]  a quick email to support.
[654.06 --> 655.48]  He gets a prompt response
[655.48 --> 656.06]  later
[656.06 --> 657.66]  and they open up the ports
[657.66 --> 658.52]  and everything
[658.52 --> 659.80]  is working perfectly.
[660.42 --> 660.86]  He goes,
[661.44 --> 663.04]  then a few days later,
[663.04 --> 664.18]  I finally got a response
[664.18 --> 665.38]  from my original provider
[665.38 --> 666.54]  with some canned email
[666.54 --> 667.52]  that didn't help it at all.
[667.58 --> 668.38]  I reply to that.
[668.58 --> 670.46]  I got another canned email response
[670.46 --> 671.44]  and that was it.
[671.44 --> 672.24]  I just gave up
[672.24 --> 673.32]  and I'm moving everything
[673.32 --> 674.18]  over to Linode.
[674.44 --> 676.14]  They're genuinely just great
[676.14 --> 678.34]  and I've gotten so many notes
[678.34 --> 678.68]  into the show
[678.68 --> 679.80]  that talk about Linode support.
[679.96 --> 680.50]  It's not an aspect
[680.50 --> 681.32]  I touch on a lot
[681.32 --> 682.32]  but it really matters
[682.32 --> 683.24]  once you get up and running,
[683.38 --> 684.72]  especially if you've got
[684.72 --> 685.66]  some important infrastructure
[685.66 --> 686.08]  on there.
[686.34 --> 686.98]  So go check them out.
[687.08 --> 689.16]  Linode.com slash SSH.
[689.16 --> 692.22]  Now I know you covered
[692.22 --> 693.58]  some stuff about LastPass
[693.58 --> 695.24]  in Linux Unplugged.
[695.28 --> 697.60]  This is like Linux Unplugged Plus
[697.60 --> 698.58]  this episode, isn't it?
[699.68 --> 701.60]  But LastPass have been doing
[701.60 --> 702.52]  some shenanigans
[702.52 --> 704.28]  with their free tiers and stuff.
[704.40 --> 705.76]  I think we've all been expecting this
[705.76 --> 706.80]  for quite a long time
[706.80 --> 709.16]  since they were acquired.
[709.82 --> 711.46]  Now they are limiting
[711.46 --> 713.84]  the access
[713.84 --> 715.90]  to unlimited devices
[715.90 --> 716.86]  of one type.
[717.36 --> 718.72]  So to clarify what that means
[718.72 --> 720.26]  is you can access
[720.26 --> 721.36]  LastPass free
[721.36 --> 723.30]  on an unlimited number
[723.30 --> 723.98]  of computers
[723.98 --> 725.74]  or an unlimited number
[725.74 --> 727.00]  of mobile devices
[727.00 --> 728.20]  but not both
[728.20 --> 729.14]  on their free tier.
[729.86 --> 730.72]  I say enough.
[731.04 --> 732.14]  I say that stinks.
[732.44 --> 733.50]  And we have a recommendation
[733.50 --> 734.14]  for you.
[734.64 --> 735.00]  I agree.
[735.20 --> 736.12]  I mean the price right now
[736.12 --> 737.06]  is kind of reasonable.
[737.30 --> 738.04]  It's like what?
[738.20 --> 739.04]  Four bucks a year
[739.04 --> 739.60]  or something?
[740.16 --> 741.16]  It's not outrageous
[741.16 --> 742.70]  for a year.
[742.92 --> 743.18]  I mean
[743.18 --> 744.72]  but it stinks
[744.72 --> 745.80]  the way it's going about.
[746.54 --> 747.14]  And I agree.
[747.38 --> 748.40]  It's time to look
[748.40 --> 749.04]  at an alternative
[749.04 --> 749.94]  and this is
[749.94 --> 751.04]  the self-hosted podcast
[751.04 --> 752.98]  and I think both of us
[752.98 --> 754.52]  landed on Bitwarden
[754.52 --> 755.38]  pretty quickly.
[755.96 --> 757.36]  I have some trepidation
[757.36 --> 757.82]  here though.
[757.82 --> 758.52]  Hold on a minute.
[758.64 --> 759.50]  I think LastPass
[759.50 --> 761.08]  is $27 a year.
[761.74 --> 763.76]  It's $2.25 a month
[763.76 --> 764.54]  billed annually.
[765.46 --> 766.38]  Oh you're kidding me.
[766.72 --> 766.86]  Yeah.
[767.08 --> 767.88]  Oh jeez.
[767.98 --> 768.18]  Okay.
[769.20 --> 771.02]  Ah yeah you're right.
[771.12 --> 771.46]  So that's
[771.46 --> 772.36]  that's not nearly
[772.36 --> 773.34]  the deal I thought it was.
[773.40 --> 774.06]  That's a bad deal.
[774.06 --> 775.84]  Especially when
[775.84 --> 776.94]  Bitwarden is only
[776.94 --> 778.28]  $10 a year.
[778.52 --> 779.06]  That's if you
[779.06 --> 780.38]  buy an annual plan.
[781.08 --> 781.90]  But if you don't
[781.90 --> 783.00]  even want to do that
[783.00 --> 784.86]  you can self-host
[784.86 --> 785.98]  the Bitwarden
[785.98 --> 786.76]  server
[786.76 --> 787.78]  which is just
[787.78 --> 788.96]  so cool.
[789.38 --> 789.56]  Yeah.
[789.70 --> 791.20]  I really love seeing this
[791.20 --> 791.72]  and
[791.72 --> 793.08]  I know it's a little
[793.08 --> 793.94]  complicated.
[794.22 --> 795.12]  I think it requires
[795.12 --> 795.60]  SQL
[795.60 --> 796.98]  among other things.
[797.14 --> 798.10]  So the community
[798.10 --> 798.68]  has come up
[798.68 --> 799.46]  with an alternative.
[799.46 --> 800.58]  Yeah there's a project
[800.58 --> 801.94]  called Bitwarden RS
[801.94 --> 803.42]  which is written in Rust.
[804.42 --> 805.10]  Where's Wes
[805.10 --> 805.68]  when you need him?
[806.98 --> 808.44]  And this is a
[808.44 --> 810.50]  Bitwarden server
[810.50 --> 811.04]  that can run
[811.04 --> 811.66]  in a container
[811.66 --> 813.16]  that will essentially
[813.16 --> 815.06]  perform the same role
[815.06 --> 816.34]  as the $10 a year
[816.34 --> 817.80]  hosted service.
[818.04 --> 818.94]  The difference being
[818.94 --> 819.62]  is you own
[819.62 --> 820.26]  all the data
[820.26 --> 821.48]  it remains
[821.48 --> 822.40]  on your servers
[822.40 --> 823.18]  or your VPS
[823.18 --> 823.60]  or whatever.
[824.18 --> 824.74]  So there's a couple
[824.74 --> 825.32]  of ways you could
[825.32 --> 826.14]  go about doing this.
[826.38 --> 827.38]  The first and most
[827.38 --> 828.28]  obvious way is to
[828.28 --> 829.04]  spin up a Linode
[829.04 --> 829.96]  or something like that
[829.96 --> 831.14]  and throw Bitwarden
[831.14 --> 831.58]  on there
[831.58 --> 833.58]  and just call it good.
[833.84 --> 834.54]  And because it's
[834.54 --> 835.58]  your password manager
[835.58 --> 836.42]  I would probably
[836.42 --> 837.82]  caution against
[837.82 --> 839.14]  running this
[839.14 --> 840.16]  on a shared
[840.16 --> 841.36]  cloud VPS.
[841.56 --> 842.18]  You know if you're
[842.18 --> 843.34]  hosting a ton of websites
[843.34 --> 844.98]  and it's a very
[844.98 --> 845.50]  public
[845.50 --> 846.96]  you know VPS
[846.96 --> 848.02]  I probably wouldn't
[848.02 --> 848.96]  put your password manager
[848.96 --> 850.08]  on that same system.
[850.36 --> 851.04]  I would put it
[851.04 --> 852.14]  on a separate system
[852.14 --> 853.28]  just so you're
[853.28 --> 854.20]  reducing the blast
[854.20 --> 855.32]  radius of any bots
[855.32 --> 855.74]  or anything
[855.74 --> 856.68]  doing something crazy
[856.68 --> 857.92]  with the web servers.
[857.92 --> 859.36]  The other thing
[859.36 --> 860.00]  you can do
[860.00 --> 860.98]  is run it
[860.98 --> 861.90]  on your LAN
[861.90 --> 862.48]  and I think
[862.48 --> 863.58]  the running
[863.58 --> 864.18]  it on a separate
[864.18 --> 864.88]  system becomes
[864.88 --> 865.70]  less important
[865.70 --> 866.24]  when it's on
[866.24 --> 867.46]  your network.
[868.08 --> 868.82]  And the idea
[868.82 --> 869.80]  of running it
[869.80 --> 870.58]  on your LAN
[870.58 --> 871.08]  of course
[871.08 --> 872.58]  is that your data
[872.58 --> 873.48]  never leaves
[873.48 --> 874.36]  your house
[874.36 --> 875.00]  right?
[875.18 --> 875.84]  And that will
[875.84 --> 876.20]  hopefully
[876.20 --> 877.64]  reduce
[877.64 --> 878.50]  the risk
[878.50 --> 879.16]  even further.
[879.66 --> 880.56]  Now the downside
[880.56 --> 881.70]  of running your own
[881.70 --> 882.46]  password manager
[882.46 --> 882.86]  backend
[882.86 --> 883.68]  is you've got to
[883.68 --> 884.54]  configure secure
[884.54 --> 885.34]  access to it.
[885.34 --> 886.50]  So that could be
[886.50 --> 887.46]  using WireGuard
[887.46 --> 889.10]  or some other
[889.10 --> 890.08]  kind of authentication
[890.08 --> 890.84]  through SSH
[890.84 --> 891.70]  or something like that.
[892.04 --> 892.72]  But ultimately
[892.72 --> 893.18]  you're going to want
[893.18 --> 893.92]  to be really careful
[893.92 --> 894.74]  and really sure
[894.74 --> 895.28]  you know what you're
[895.28 --> 896.18]  doing from a security
[896.18 --> 896.74]  perspective
[896.74 --> 898.00]  before you start
[898.00 --> 898.70]  going and storing
[898.70 --> 899.32]  all your passwords
[899.32 --> 900.80]  on a public system.
[901.50 --> 901.82]  That's where you
[901.82 --> 902.56]  could make the argument
[902.56 --> 903.36]  that it could just
[903.36 --> 904.12]  be worth paying
[904.12 --> 904.82]  for their
[904.82 --> 906.18]  hosted service.
[906.92 --> 907.82]  And this is where
[907.82 --> 908.82]  I'm currently
[908.82 --> 909.76]  experiencing my
[909.76 --> 910.32]  trepidation.
[910.52 --> 912.44]  I 100% know
[912.44 --> 913.66]  I could self-host it.
[913.66 --> 914.90]  And the nice thing
[914.90 --> 915.54]  about this Rust
[915.54 --> 916.38]  version of their
[916.38 --> 917.00]  server is
[917.00 --> 918.32]  really minimal
[918.32 --> 918.84]  resources.
[918.84 --> 919.40]  So you could
[919.40 --> 919.90]  really run it
[919.90 --> 920.66]  on anything.
[920.82 --> 921.62]  So I could run
[921.62 --> 922.56]  it on my Raspberry Pi
[922.56 --> 923.30]  or I could run it
[923.30 --> 924.00]  easily here on the
[924.00 --> 924.70]  server at the studio.
[925.22 --> 926.84]  But I'm not sure
[926.84 --> 927.78]  I want to.
[928.30 --> 928.44]  You know,
[928.48 --> 928.96]  there's something
[928.96 --> 930.02]  about the
[930.02 --> 931.26]  master password
[931.26 --> 931.70]  vault.
[932.06 --> 932.80]  It's such a
[932.80 --> 934.00]  sacred responsibility
[934.00 --> 936.76]  that I almost
[936.76 --> 937.40]  trust an
[937.40 --> 938.18]  organization like
[938.18 --> 939.58]  Bitwarden to be
[939.58 --> 940.58]  more focused on
[940.58 --> 941.12]  securing that
[941.12 --> 942.10]  platform than I am.
[942.18 --> 943.28]  Not that I really
[943.28 --> 944.06]  have no concerns
[944.06 --> 944.76]  about our security.
[945.00 --> 945.42]  Really?
[946.30 --> 946.78]  But there's
[946.78 --> 947.52]  something that
[947.52 --> 948.18]  still gives me
[948.18 --> 948.70]  pause.
[949.12 --> 949.48]  They've got one
[949.48 --> 950.28]  job to do.
[950.42 --> 951.60]  And I've actually
[951.60 --> 952.50]  paid Bitwarden
[952.50 --> 953.44]  the $10 a year
[953.44 --> 954.68]  for two or three,
[954.82 --> 955.48]  maybe four years
[955.48 --> 955.94]  at this point.
[956.38 --> 956.94]  I've been very,
[957.06 --> 957.44]  very happy.
[957.64 --> 958.50]  It just does the
[958.50 --> 958.78]  job.
[958.94 --> 959.62]  I never have to
[959.62 --> 960.36]  think about it.
[960.68 --> 961.06]  All of the
[961.06 --> 962.10]  autofill stuff on
[962.10 --> 962.88]  Android and iOS
[962.88 --> 963.50]  just works
[963.50 --> 964.58]  fantastically well.
[965.34 --> 965.58]  You know,
[965.64 --> 966.88]  $10 is that kind
[966.88 --> 968.34]  of screw it
[968.34 --> 969.36]  amount of money
[969.36 --> 969.92]  when it's spread
[969.92 --> 970.86]  over an entire year.
[971.00 --> 971.14]  You know,
[971.18 --> 971.68]  it's less than a
[971.68 --> 972.28]  dollar a month.
[972.28 --> 973.72]  And to just
[973.72 --> 974.56]  not have to worry
[974.56 --> 975.20]  about it and to
[975.20 --> 975.74]  just not have to
[975.74 --> 976.48]  think about it for
[976.48 --> 978.00]  what, 80, 90 cents
[978.00 --> 978.44]  a month,
[978.88 --> 979.82]  that's worth it for me.
[980.06 --> 981.22]  It reminds me of
[981.22 --> 982.20]  why I kind of like
[982.20 --> 983.74]  supporting Nebukasa
[983.74 --> 985.14]  and how supporting
[985.14 --> 986.66]  Nebukasa goes into
[986.66 --> 987.10]  home assistant
[987.10 --> 987.62]  development and
[987.62 --> 988.22]  makes home assistant
[988.22 --> 988.56]  better.
[988.88 --> 990.16]  By subscribing to
[990.16 --> 990.90]  Bitwarden, you're
[990.90 --> 991.88]  helping them come up
[991.88 --> 992.40]  with a sustainable
[992.40 --> 993.38]  business model that
[993.38 --> 994.36]  encourages them to
[994.36 --> 995.00]  make the password
[995.00 --> 996.16]  manager better and
[996.16 --> 996.92]  keep their service
[996.92 --> 997.32]  secure.
[997.32 --> 999.14]  So it incentivizes
[999.14 --> 1000.14]  the right things
[1000.14 --> 1001.56]  and on top of that
[1001.56 --> 1002.02]  it means I don't
[1002.02 --> 1002.56]  have to host it
[1002.56 --> 1002.86]  myself.
[1003.04 --> 1003.56]  I haven't actually
[1003.56 --> 1004.40]  made my decision
[1004.40 --> 1006.24]  because I have
[1006.24 --> 1007.40]  kept a lot of
[1007.40 --> 1008.38]  business stuff in
[1008.38 --> 1009.30]  LastPass for a
[1009.30 --> 1009.52]  while.
[1009.66 --> 1010.16]  I know I like
[1010.16 --> 1010.88]  Bitwarden so I've
[1010.88 --> 1011.46]  always thought that's
[1011.46 --> 1012.08]  what I would jump
[1012.08 --> 1012.36]  to.
[1013.20 --> 1013.74]  And so I went over
[1013.74 --> 1015.18]  to their subscription
[1015.18 --> 1016.50]  pricing page and
[1016.50 --> 1017.26]  they also offer
[1017.26 --> 1018.80]  team plans for as
[1018.80 --> 1019.46]  little as like $3
[1019.46 --> 1020.58]  per user and that's
[1020.58 --> 1021.74]  still pretty reasonable.
[1022.54 --> 1023.22]  So I think that might
[1023.22 --> 1023.96]  be the direction I
[1023.96 --> 1024.50]  end up going.
[1024.70 --> 1025.28]  I'm going to research
[1025.28 --> 1025.96]  more about how
[1025.96 --> 1026.92]  they host it first
[1026.92 --> 1029.08]  because I know a
[1029.08 --> 1030.24]  big use case for me
[1030.24 --> 1031.52]  a really big use
[1031.52 --> 1032.06]  case for me is
[1032.06 --> 1032.82]  mobile access.
[1033.40 --> 1034.08]  It's such a
[1034.08 --> 1034.84]  crapshoot with me.
[1034.96 --> 1035.88]  I don't just connect
[1035.88 --> 1036.96]  from one machine.
[1037.20 --> 1038.28]  It's just ridiculous
[1038.28 --> 1039.00]  especially when you
[1039.00 --> 1040.04]  bring in like
[1040.04 --> 1041.38]  traveling or setting
[1041.38 --> 1042.08]  up family member
[1042.08 --> 1042.80]  systems or.
[1043.18 --> 1043.64]  And hosts.
[1043.98 --> 1044.62]  Yeah it's just
[1044.62 --> 1045.34]  it's ridiculous.
[1045.62 --> 1047.56]  So I kind of like
[1047.56 --> 1048.40]  the idea of something
[1048.40 --> 1048.94]  where I'm not
[1048.94 --> 1050.06]  handing out WireGuard
[1050.06 --> 1051.18]  connections to 15
[1051.18 --> 1052.02]  different people so
[1052.02 --> 1052.58]  that way they can
[1052.58 --> 1053.38]  access the central
[1053.38 --> 1054.34]  password database.
[1054.34 --> 1055.80]  And don't forget
[1055.80 --> 1056.48]  as well generally
[1056.48 --> 1057.28]  the time when you
[1057.28 --> 1058.22]  need Bitwarden the
[1058.22 --> 1059.00]  most is when your
[1059.00 --> 1060.08]  device is completely
[1060.08 --> 1061.50]  brand new or empty.
[1062.16 --> 1062.26]  Right.
[1062.66 --> 1063.48]  And so you've always
[1063.48 --> 1064.26]  got that awkward
[1064.26 --> 1065.30]  first 10 minutes
[1065.30 --> 1065.88]  where you're getting
[1065.88 --> 1066.94]  you know your two
[1066.94 --> 1067.96]  factor auth set up
[1067.96 --> 1068.86]  again and your
[1068.86 --> 1069.86]  Bitwarden whatever
[1069.86 --> 1070.60]  set up again.
[1071.18 --> 1071.74]  And once you've got
[1071.74 --> 1072.40]  those two things
[1072.40 --> 1072.98]  you're good to go
[1072.98 --> 1074.54]  generally but yeah I
[1074.54 --> 1075.08]  can see you don't
[1075.08 --> 1075.50]  want to be handing
[1075.50 --> 1076.50]  that out to randos.
[1077.04 --> 1077.50]  If you do want to
[1077.50 --> 1078.06]  self host it though
[1078.06 --> 1079.22]  Alex like somebody
[1079.22 --> 1079.86]  in our audience who
[1079.86 --> 1080.36]  may have a different
[1080.36 --> 1081.74]  use case it's easier
[1081.74 --> 1082.70]  than ever now because
[1082.70 --> 1083.74]  the Bitwarden
[1083.74 --> 1084.80]  Rust server has a
[1084.80 --> 1086.12]  Docker image fully
[1086.12 --> 1087.64]  up to date as of
[1087.64 --> 1088.82]  like 19 hours ago as
[1088.82 --> 1089.50]  we record this.
[1089.98 --> 1091.16]  It's like the old
[1091.16 --> 1092.52]  proverb if something
[1092.52 --> 1093.56]  isn't Dockerized at
[1093.56 --> 1094.20]  this point does it
[1094.20 --> 1094.82]  even exist?
[1095.78 --> 1096.74]  Now another nice
[1096.74 --> 1097.60]  thing that I do with
[1097.60 --> 1098.30]  Bitwarden is I
[1098.30 --> 1098.72]  actually share
[1098.72 --> 1099.54]  passwords with my
[1099.54 --> 1099.84]  wife.
[1100.06 --> 1100.92]  She has a Bitwarden.
[1101.30 --> 1101.80]  I don't think she
[1101.80 --> 1102.64]  pays the premium I
[1102.64 --> 1103.30]  think she just has the
[1103.30 --> 1104.94]  basic free account but
[1104.94 --> 1105.64]  we created an
[1105.64 --> 1107.14]  organization and when
[1107.14 --> 1107.86]  you create a
[1107.86 --> 1109.26]  particular login you
[1109.26 --> 1110.52]  can assign that login
[1110.52 --> 1111.72]  to an organization and
[1111.72 --> 1112.52]  share it with that
[1112.52 --> 1113.14]  organization.
[1113.92 --> 1114.90]  So certain passwords
[1114.90 --> 1115.94]  for us like Amazon,
[1116.44 --> 1117.88]  eBay, you know stuff
[1117.88 --> 1118.36]  that you want to
[1118.36 --> 1120.10]  share goes into that
[1120.10 --> 1122.04]  shared area if you
[1122.04 --> 1122.64]  like that shared
[1122.64 --> 1123.52]  organization and we've
[1123.52 --> 1124.58]  both got access to it.
[1124.70 --> 1125.38]  I find that really
[1125.38 --> 1125.74]  useful.
[1126.24 --> 1126.86]  There's of course other
[1126.86 --> 1127.72]  solutions out there.
[1127.84 --> 1128.70]  Another beloved one in
[1128.70 --> 1129.38]  the audience is
[1129.38 --> 1130.70]  KeePass and KeePassX
[1130.70 --> 1132.36]  and there's several
[1132.36 --> 1134.06]  solutions to this but
[1134.06 --> 1135.08]  Bitwarden is the one we
[1135.08 --> 1136.10]  both landed on I think
[1136.10 --> 1137.60]  in part because of the
[1137.60 --> 1138.56]  UI, the browser
[1138.56 --> 1140.24]  integration, the ability
[1140.24 --> 1142.12]  to self-host and the
[1142.12 --> 1143.00]  quality of the mobile
[1143.00 --> 1144.20]  apps all kind of come
[1144.20 --> 1145.02]  together to make it our
[1145.02 --> 1145.62]  favorite choice.
[1146.16 --> 1146.80]  So whilst we're sort of
[1146.80 --> 1147.86]  kind of on the topic of
[1147.86 --> 1149.44]  security, why don't we
[1149.44 --> 1151.70]  discuss the Plex hoopla
[1151.70 --> 1152.68]  that's been going on as
[1152.68 --> 1155.42]  well about this botnet
[1155.42 --> 1156.26]  thing that's been
[1156.26 --> 1157.70]  amplifying stuff across
[1157.70 --> 1158.16]  the internet?
[1158.16 --> 1159.50]  It just stinks because
[1159.50 --> 1160.86]  you know you got a Plex
[1160.86 --> 1162.28]  server going, you've
[1162.28 --> 1163.02]  opened it up to the
[1163.02 --> 1163.74]  internet so that way you
[1163.74 --> 1164.40]  can share it.
[1164.78 --> 1165.94]  Some scanner finds your
[1165.94 --> 1167.74]  server, indexes it and
[1167.74 --> 1168.84]  then some botnet author
[1168.84 --> 1170.88]  figures out a way to
[1170.88 --> 1171.78]  take advantage of a
[1171.78 --> 1172.98]  vulnerability in Plex to
[1172.98 --> 1174.86]  amplify by a factor of
[1174.86 --> 1177.28]  five their DDoS traffic.
[1177.50 --> 1179.48]  They kind of corral all of
[1179.48 --> 1180.36]  these different Plex
[1180.36 --> 1182.54]  installs together to kind
[1182.54 --> 1183.90]  of do this amplified
[1183.90 --> 1185.30]  attack against a single
[1185.30 --> 1186.64]  source and just happened
[1186.64 --> 1187.50]  the last week as we're
[1187.50 --> 1188.20]  recording this.
[1188.60 --> 1189.90]  NetScout said that there
[1189.90 --> 1191.02]  was a DDoS for hire
[1191.02 --> 1192.62]  service that recently
[1192.62 --> 1194.16]  turned misconfigured Plex
[1194.16 --> 1195.34]  media servers into
[1195.34 --> 1196.74]  amplifying attack servers.
[1196.74 --> 1198.72]  Rut roll.
[1199.20 --> 1200.26]  Yeah, not only does it
[1200.26 --> 1201.20]  suck up all of your
[1201.20 --> 1202.40]  bandwidth and attack
[1202.40 --> 1203.50]  somebody but it also
[1203.50 --> 1204.64]  runs your server like
[1204.64 --> 1205.06]  crazy.
[1205.38 --> 1206.50]  It's just bad.
[1206.98 --> 1207.90]  Yeah, what really kind
[1207.90 --> 1209.30]  of, I don't want to use
[1209.30 --> 1210.90]  the word scared me, but
[1210.90 --> 1212.06]  I suppose so, you know,
[1212.26 --> 1213.38]  gave me cause for a
[1213.38 --> 1215.80]  concern at least was just
[1215.80 --> 1218.78]  opening port 32400,
[1218.96 --> 1222.52]  32400 on TCP, just
[1222.52 --> 1224.26]  opening that port alone is
[1224.26 --> 1225.58]  enough to be vulnerable
[1225.58 --> 1226.30]  because it's such a
[1226.30 --> 1226.94]  common port.
[1227.64 --> 1228.68]  People will scan it and
[1228.68 --> 1229.58]  find it and then be like,
[1229.64 --> 1230.34]  oh, this guy's running
[1230.34 --> 1230.74]  Plex.
[1231.10 --> 1231.24]  Yeah.
[1231.48 --> 1233.14]  So what I've done since
[1233.14 --> 1234.38]  this vulnerability to
[1234.38 --> 1235.62]  kind of remove myself
[1235.62 --> 1239.06]  from the risk factor is
[1239.06 --> 1239.96]  I've closed that port in
[1239.96 --> 1241.10]  my firewall and I have
[1241.10 --> 1242.74]  started to define a
[1242.74 --> 1244.66]  custom server URL in my
[1244.66 --> 1245.68]  Plex server settings.
[1245.68 --> 1248.04]  And I set a DNS entry in
[1248.04 --> 1248.56]  Cloudflare.
[1249.24 --> 1251.00]  That then points to my
[1251.00 --> 1251.64]  WAN IP.
[1252.60 --> 1254.20]  From there, that then
[1254.20 --> 1256.00]  points to a traffic
[1256.00 --> 1257.12]  instance that's running on
[1257.12 --> 1257.94]  the same server as
[1257.94 --> 1258.28]  Plex.
[1259.00 --> 1260.22]  And from there, it does a
[1260.22 --> 1261.72]  standard reverse proxy
[1261.72 --> 1263.54]  thing and just does the
[1263.54 --> 1265.32]  remote access as if I was
[1265.32 --> 1267.16]  going through port 32400
[1267.16 --> 1269.08]  like I was last month.
[1269.56 --> 1271.78]  Very easy fix and I highly
[1271.78 --> 1272.76]  recommend you take a look
[1272.76 --> 1273.16]  into that.
[1273.16 --> 1274.06]  That's a great idea
[1274.06 --> 1275.36]  because Netscout said that
[1275.36 --> 1276.30]  after a scan they
[1276.30 --> 1277.20]  conducted, they found
[1277.20 --> 1279.26]  about 27,000 servers on
[1279.26 --> 1280.06]  the internet that can be
[1280.06 --> 1281.08]  abused this way.
[1281.80 --> 1283.16]  So it doesn't mean you
[1283.16 --> 1284.00]  have to shut off remote
[1284.00 --> 1286.46]  Plex, but it does mean
[1286.46 --> 1287.18]  you should probably take
[1287.18 --> 1287.96]  some steps to protect
[1287.96 --> 1288.30]  yourself.
[1288.72 --> 1289.50]  Yeah, just put it behind
[1289.50 --> 1290.24]  a reverse proxy.
[1290.40 --> 1291.00]  I mean, it doesn't have
[1291.00 --> 1291.46]  to be traffic.
[1291.62 --> 1292.28]  It could be Nginx.
[1292.38 --> 1292.84]  It could be whatever.
[1293.22 --> 1296.02]  But just don't open any
[1296.02 --> 1296.84]  ports in your firewall.
[1296.96 --> 1297.96]  You absolutely don't
[1297.96 --> 1298.44]  need to.
[1298.92 --> 1300.18]  Which actually brings me
[1300.18 --> 1301.62]  very nicely onto a very,
[1301.76 --> 1302.48]  very quick bit of
[1302.48 --> 1303.14]  follow up about the
[1303.14 --> 1304.36]  WireGuard rant I had
[1304.36 --> 1306.08]  last week on OpenSense.
[1307.24 --> 1308.94]  Turns out, like an
[1308.94 --> 1312.02]  idiot, I set a slash 16
[1312.02 --> 1313.96]  subnet in my DHCP server.
[1314.82 --> 1315.48]  Now for those that don't
[1315.48 --> 1316.60]  know, what that means is
[1316.60 --> 1319.96]  every address from 192.168.0
[1319.96 --> 1323.70]  all the way up to 192.168.255
[1323.70 --> 1326.56]  was within my DHCP range.
[1326.70 --> 1328.74]  So I had 65,000 or whatever
[1328.74 --> 1330.24]  DHCP addresses available.
[1331.24 --> 1332.92]  The upshot of that was when
[1332.92 --> 1334.24]  I was trying to route through
[1334.24 --> 1337.50]  WireGuard, I was doing a 192.168.13
[1337.50 --> 1338.54]  subnet.
[1339.16 --> 1341.54]  And so the remote servers were
[1341.54 --> 1343.64]  hearing that were receiving the
[1343.64 --> 1344.88]  commands from my laptop or my
[1344.88 --> 1345.42]  phone or whatever.
[1345.92 --> 1347.66]  But they didn't know how to route
[1347.66 --> 1349.68]  back to the client device because
[1349.68 --> 1351.14]  as far as they were concerned, the
[1351.14 --> 1352.70]  slash 16 overrode everything and
[1352.70 --> 1353.72]  it just thought everything was on
[1353.72 --> 1354.08]  the LAN.
[1354.08 --> 1357.02]  So what I did was I changed the
[1357.02 --> 1360.12]  subnet of the WireGuard VPN to a
[1360.12 --> 1361.12]  10.something.
[1361.74 --> 1362.94]  So it was a completely different
[1362.94 --> 1365.14]  subnet and I reduced my slash 16
[1365.14 --> 1367.14]  down to a more manageable slash 20.
[1367.62 --> 1368.92]  So I've only got a few thousand, like
[1368.92 --> 1370.98]  4,000 addresses now instead of
[1370.98 --> 1371.96]  65,000.
[1372.08 --> 1373.38]  I think that should tie me over for a
[1373.38 --> 1373.72]  bit, right?
[1374.08 --> 1374.60]  Nicely done.
[1375.02 --> 1376.58]  I definitely always suggest if
[1376.58 --> 1379.30]  people can, different subnets for
[1379.30 --> 1381.68]  the different VPN endpoints makes it
[1381.68 --> 1383.90]  so much simpler, you know, and I've
[1383.90 --> 1385.40]  tried, I've tried to do that myself
[1385.40 --> 1387.84]  so many times because it can solve
[1387.84 --> 1390.76]  you just a few simple problems and
[1390.76 --> 1392.74]  keeps it a little clear in your
[1392.74 --> 1393.02]  head.
[1393.18 --> 1396.12]  Like I know that the studio is .4
[1396.12 --> 1399.84]  and home is .7 and the WireGuard
[1399.84 --> 1401.42]  network is actually a .10 network.
[1401.54 --> 1402.50]  It's all separated out.
[1402.86 --> 1402.96]  Yeah.
[1403.02 --> 1404.20]  So I just wanted to be absolutely
[1404.20 --> 1406.16]  clear that the problem was the user
[1406.16 --> 1408.50]  not OpenSense or WireGuard.
[1408.60 --> 1409.80]  It was totally my fault.
[1409.80 --> 1412.92]  And I owe a huge debt of gratitude to
[1412.92 --> 1414.18]  one of our listeners who reached out
[1414.18 --> 1418.04]  to me on Discord and did a screen
[1418.04 --> 1419.16]  share with me and walked me through
[1419.16 --> 1420.40]  it for half an hour because he works
[1420.40 --> 1423.32]  in security down in Charlotte in
[1423.32 --> 1423.88]  North Carolina.
[1424.56 --> 1426.12]  And he sort of taught me some new
[1426.12 --> 1427.88]  stuff about, you know, networking and
[1427.88 --> 1428.88]  triage and that kind of stuff.
[1428.94 --> 1429.56]  So that was pretty cool.
[1429.62 --> 1431.70]  So huge thank you to that listener.
[1432.24 --> 1434.06]  Sounds like somebody we should buy a
[1434.06 --> 1436.78]  beer for when community events happen
[1436.78 --> 1437.10]  again.
[1437.44 --> 1437.88]  One day.
[1438.68 --> 1439.08]  Yeah.
[1439.80 --> 1442.06]  Well, if you'd like to learn
[1442.06 --> 1444.18]  networking or anything else, ACG has
[1444.18 --> 1447.16]  20% off annual plans right now.
[1447.28 --> 1448.56]  We'll have a link in the show notes
[1448.56 --> 1450.10]  or just go to cloudguru.com.
[1450.16 --> 1451.80]  And when you sign up, use the promo
[1451.80 --> 1454.00]  code springintocloud21.
[1454.24 --> 1455.86]  You know that cloud is growing.
[1455.96 --> 1457.48]  There's lots of new services and
[1457.48 --> 1459.62]  systems more every day, it seems.
[1459.98 --> 1461.50]  And that also means the demand for
[1461.50 --> 1463.16]  skilled cloud professionals is growing
[1463.16 --> 1463.48]  too.
[1463.84 --> 1465.98]  82% of hiring managers say a cloud
[1465.98 --> 1468.30]  certification makes a candidate more
[1468.30 --> 1468.80]  attractive.
[1468.80 --> 1471.36]  So go grow your skills with hands-on
[1471.36 --> 1472.08]  labs and learning.
[1472.42 --> 1473.72]  Keep up with change and develop the
[1473.72 --> 1475.38]  skills you need with a cloud guru.
[1475.62 --> 1478.32]  To get that 20% off, sign up for an
[1478.32 --> 1480.22]  annual plan and use that promo code
[1480.22 --> 1482.54]  springintocloud21.
[1482.54 --> 1485.32]  95% of learners say that a cloud guru's
[1485.32 --> 1487.08]  tools and content directly help them
[1487.08 --> 1488.22]  advance their careers.
[1488.54 --> 1489.72]  Spring into cloud21.
[1489.90 --> 1490.82]  Link in the show notes or go to
[1490.82 --> 1492.20]  cloudguru.com.
[1494.48 --> 1496.98]  Ryan writes in with an IGPU question.
[1497.46 --> 1498.00]  Hey there, friends.
[1498.08 --> 1499.12]  I'm a big fan of the show.
[1499.72 --> 1501.50]  I currently am in the process of building
[1501.50 --> 1503.10]  an off-grid house in New Zealand.
[1503.42 --> 1504.88]  Oh, that's the dream.
[1504.88 --> 1505.44]  I know.
[1506.00 --> 1506.40]  Right?
[1506.66 --> 1507.04]  Amazing.
[1507.32 --> 1508.10]  Can we come visit?
[1509.06 --> 1510.26]  Self-hosted on tour.
[1511.08 --> 1513.32]  Power consumption is key, so I want a
[1513.32 --> 1514.82]  small box to run basically everything
[1514.82 --> 1516.62]  I need, which thankfully isn't going to
[1516.62 --> 1517.36]  be that much.
[1517.80 --> 1520.24]  My question is, is it possible to run a
[1520.24 --> 1522.44]  Linux server and pass through an IGPU to
[1522.44 --> 1525.42]  a Windows VM for Blue Iris, while still
[1525.42 --> 1527.32]  using the IGPU for containerized
[1527.32 --> 1528.60]  applications like Plex?
[1529.24 --> 1531.26]  I can't seem to see any problem with
[1531.26 --> 1533.08]  this in theory, but wonder if you have
[1533.08 --> 1533.72]  any ideas.
[1534.16 --> 1534.92]  Love your work.
[1535.22 --> 1535.58]  Ryan.
[1536.62 --> 1537.88]  What do you think about this one?
[1537.98 --> 1539.90]  I have also contemplated, is there a
[1539.90 --> 1541.52]  way I can have my cake and eat it too
[1541.52 --> 1544.10]  when it comes to an IGPU and a low
[1544.10 --> 1544.66]  power system?
[1545.08 --> 1546.58]  I thought I'd solve this problem.
[1546.64 --> 1547.94]  I thought I had the answer.
[1548.46 --> 1551.50]  And it was a technology called GVT-G,
[1551.50 --> 1555.20]  which is a virtual graphics card kind
[1555.20 --> 1557.84]  of slicing thing that basically lets you
[1557.84 --> 1561.58]  take an Intel GPU built into your CPU
[1561.58 --> 1564.62]  and slice it up into two slices and give
[1564.62 --> 1566.14]  one to one VM and one to another.
[1566.34 --> 1569.04]  So the obvious use case for that is to
[1569.04 --> 1571.66]  give one slice to a Windows VM for Blue
[1571.66 --> 1574.14]  Iris and then give the other slice to
[1574.14 --> 1576.84]  another Linux VM for Plex and then keep
[1576.84 --> 1578.06]  the host as clean as possible.
[1578.72 --> 1578.78]  Yeah.
[1579.30 --> 1581.58]  However, and I've written a blog post about
[1581.58 --> 1582.36]  this this week.
[1583.22 --> 1586.54]  Unfortunately, the performance of GVT-G is
[1586.54 --> 1587.78]  horrible.
[1589.58 --> 1593.38]  I found it to be anywhere from 58 to 82%
[1593.38 --> 1595.56]  slower than Quicksync being run natively
[1595.56 --> 1596.54]  on the bare metal host.
[1597.16 --> 1598.16]  Holy smokes.
[1598.46 --> 1599.92]  I did not expect that at all.
[1600.34 --> 1600.46]  Yeah.
[1600.52 --> 1602.12]  So my test that I did was it was pretty
[1602.12 --> 1604.54]  unscientific, but it was a very real
[1604.54 --> 1605.56]  world use case for me.
[1605.56 --> 1608.76]  So I used the Plex sync for offline
[1608.76 --> 1612.22]  playback feature and I chose a high bit
[1612.22 --> 1612.50]  rate.
[1612.62 --> 1615.78]  So about a 38 megabyte a second.
[1616.44 --> 1617.54]  Was it megabit?
[1617.62 --> 1618.52]  I always get confused.
[1618.96 --> 1622.62]  Video file encoded with MPEG-4 and H.264
[1622.62 --> 1626.52]  with a DTS master audio soundtrack.
[1626.92 --> 1631.04]  And I used the four megabytes a second 720p
[1631.04 --> 1634.00]  sync for offline playback option within Plex.
[1634.00 --> 1636.36]  And I did that on an iPad.
[1636.90 --> 1637.90]  You know, that was the client.
[1638.02 --> 1639.48]  I don't think that bit really mattered too
[1639.48 --> 1641.56]  much, but I did a few different tests.
[1641.68 --> 1642.86]  So I did a software render.
[1643.04 --> 1647.76]  So this is using the Intel i5-8500 CPU.
[1648.24 --> 1650.20]  I picked that up for about a hundred dollars
[1650.20 --> 1650.88]  used on eBay.
[1651.04 --> 1652.32]  So it's a pretty good value.
[1652.68 --> 1653.44]  Four gigahertz.
[1653.54 --> 1656.44]  I think 4.1 gigahertz, six core CPU.
[1657.20 --> 1661.60]  With CPU rendering only, I saw a 1.1 times
[1661.60 --> 1662.32]  speed.
[1662.32 --> 1665.96]  The best I saw running it natively in QuickSync
[1665.96 --> 1668.00]  on the host was 10.2.
[1668.52 --> 1671.22]  And then on a sliding scale between those two
[1671.22 --> 1676.86]  numbers of 1 times and 10 times, with the GVTG stuff set
[1676.86 --> 1682.78]  into two slice mode, I saw only about a 1.8, 1.9 times.
[1683.32 --> 1687.68]  So it was faster than CPU software encoding, you know, twice as fast
[1687.68 --> 1695.28]  actually, but it was 80, what, something, 82% slower than running it on the
[1695.28 --> 1695.96]  bare metal host.
[1695.96 --> 1702.70]  So the other problem that I ran into, besides, you know, leaving 80 plus percent performance
[1702.70 --> 1705.44]  on the table, was stability.
[1705.86 --> 1708.76]  Unfortunately, that wasn't a great story either.
[1709.18 --> 1715.52]  The problems I ran into were, so I was running Proxmox as the base OS because the Proxmox
[1715.52 --> 1720.86]  wiki actually has a really great entry about enabling GVTG and QuickSync and pass through
[1720.86 --> 1721.64]  and all that kind of stuff.
[1721.64 --> 1723.58]  And it was really painless to get going.
[1723.68 --> 1726.52]  It only took me an hour or so to figure it all out and get it going.
[1727.38 --> 1729.50]  But the stability was just not there.
[1730.02 --> 1731.92]  My evidence is only anecdotal, though.
[1732.34 --> 1736.12]  Because of the instability, I couldn't really get the log files that I needed
[1736.12 --> 1741.68]  because the system either had to be hard reset or it was just hanging and processes were just
[1741.68 --> 1743.48]  hanging or I was getting kernel panics.
[1743.48 --> 1745.24]  It was just a mess.
[1745.80 --> 1748.32]  And, you know, at the end of the day...
[1748.32 --> 1751.92]  Just not something you could just let run and just not have to think about it.
[1752.06 --> 1753.70]  No, unfortunately, it wasn't.
[1753.80 --> 1759.76]  And, you know, things worked fine until I powered on the Windows VM that was running Blue Iris.
[1760.00 --> 1763.54]  And that system has six 4K cameras going into it.
[1763.58 --> 1765.38]  So it's got a decent amount of load.
[1765.38 --> 1772.26]  Now, I know for a fact that the i5 CPU can handle that load because it's been running in my HP 290 Slim
[1772.26 --> 1776.72]  for six months just fine, handling everything perfectly.
[1777.24 --> 1784.86]  But for some reason, when it's in the GVTG mode, it just, I guess, because the performance is so poor
[1784.86 --> 1791.04]  with the emulation, whatever they're doing to slice the GPU up, however they're doing it in the Intel drivers,
[1791.04 --> 1799.72]  it just meant that as soon as I powered up Blue Iris, within 30 minutes, the whole Proxmox system was just unhappy.
[1800.06 --> 1804.30]  You know, like the web UI wouldn't load sometimes or you actually go and reboot the system
[1804.30 --> 1810.78]  and you'll see SystemD printing out waiting on Kimu guest to shut down for like 30 minutes.
[1811.32 --> 1815.62]  So it wasn't just guest stability issues, but the entire host.
[1815.82 --> 1816.14]  Uh-huh.
[1817.06 --> 1817.90]  Ooh, yeah.
[1818.18 --> 1819.56]  Well, that's just a deal breaker.
[1819.56 --> 1822.18]  Oh, man, Alex.
[1822.36 --> 1824.98]  At the end of the day, you want it to be on and functional.
[1825.24 --> 1831.26]  And yes, this is a hobby, and I do enjoy messing about with servers, but there comes a point.
[1831.34 --> 1832.34]  It's not a full-time job.
[1832.50 --> 1833.24]  No, exactly.
[1833.58 --> 1837.70]  There comes a point where you're like, this S just needs to work now.
[1838.04 --> 1838.26]  Yeah.
[1838.64 --> 1839.98]  And it just didn't, unfortunately.
[1840.26 --> 1844.58]  I think you crossed the threshold of devoting more time to this than most folks quite a while ago.
[1844.58 --> 1848.36]  I mean, even taking a pass at the different encoding options, that's good insight.
[1848.36 --> 1854.76]  And it really shows you that you're, I mean, yeah, it's almost twice as fast if you use GVT.
[1854.76 --> 1860.42]  When you consider the stability issues, I would rather just use CPU encoding.
[1860.42 --> 1869.42]  CPU encoding with QuickSync, because that's only pulling down about 10 watts when it's doing a full 1080p stream, and it's running at 10x real time.
[1869.92 --> 1874.70]  So it actually, you know, in terms of performance per watt is the best thing out there.
[1874.94 --> 1879.18]  I actually also, just for giggles, use my 1080 Ti to run one of these transcodes.
[1879.76 --> 1881.62]  So QuickSync is running at 10x.
[1882.02 --> 1888.02]  A 1080 Ti, which is pulling down 18 times the amount of power, is running at 17 times.
[1888.20 --> 1889.98]  So 10x versus 17x.
[1890.08 --> 1890.50]  Wow.
[1890.70 --> 1897.44]  It's a good way to see the performance discrepancy between Intel's GPU and the NVIDIA GPU right there, isn't it?
[1897.46 --> 1897.96]  You can really.
[1898.28 --> 1900.82]  And then, of course, CPU with its measly 1.1x.
[1901.24 --> 1901.40]  Yeah.
[1902.02 --> 1905.70]  Performance per watt of the NVIDIA card was just hilariously bad.
[1906.06 --> 1906.58]  Well, sure.
[1906.98 --> 1907.30]  Sure.
[1907.30 --> 1914.94]  So what I've ended up doing, actually, and this is to go back to Ryan's question now, is I've ended up splitting things back out into physical boxes.
[1915.56 --> 1920.04]  The Blue Iris box is an HP290 Slim that I already had.
[1920.44 --> 1927.58]  I've put the i5 back into there, and I bought another i5 to put into my server, so I have two now, which is a shame, but hey-ho.
[1928.06 --> 1932.36]  I was doing some testing on the HP290 for average power usage.
[1932.36 --> 1938.12]  When I say idle, what I mean by that is Blue Iris is running with its normal sort of load.
[1938.30 --> 1945.72]  So an average sort of power usage I see on that box is anywhere from sort of 10 to 25 watts, depending on what it's doing.
[1945.72 --> 1951.08]  Which, for the performance I'm getting, you know, that kind of power usage is fantastic, really.
[1951.82 --> 1960.20]  And then my main server is pulling it anywhere with, you know, it's got, I think, 12 hard drives in it, anywhere from 40 to 80 watts at idle.
[1960.20 --> 1967.36]  So, you know, it's all pretty good, pretty low, you know, to have all that performance for under 100 watts at idle is, I'm pretty happy with that.
[1967.90 --> 1969.64]  Yeah, thanks for sharing the details with us.
[1969.68 --> 1970.86]  You mentioned the blog in there.
[1970.96 --> 1973.38]  Well, Sam actually writes in with our next question.
[1973.46 --> 1981.38]  He's a new listener, and he says, I'd love to hear more about what Alex uses for building his blog, and if you've experimented with any other options and what you thought.
[1981.56 --> 1982.24]  Thanks for the great show.
[1982.24 --> 1995.84]  Well, several years ago, when I was launching LinuxServer.io, I actually had a personal blog, blog.katz.me, that got turned into LinuxServer's blog and eventually the LinuxServer website, and that kind of took over and became its own thing.
[1996.26 --> 2004.84]  So we used to use WordPress, and then we moved to Ghost on LinuxServer, and this would be, I dread to think how long ago, like five years ago?
[2004.84 --> 2013.84]  We moved to Ghost, and it's been so solid, I then ended up spinning up Ghost for my own personal blog to do, like, travel writing and all that kind of stuff as well.
[2014.58 --> 2022.22]  So I use Ghost almost exclusively for blogging, and then the Perfect Media Server website is written in mkdocs.
[2022.70 --> 2024.66]  I live vicariously through you on Ghost.
[2024.90 --> 2032.26]  That was the route I thought I might go if I were going to set up a blog again, and I'm going to put a link to that in the show notes because I think that's worth checking out.
[2032.26 --> 2035.50]  Although they've changed their model a lot since I first originally found them.
[2035.54 --> 2041.38]  Now they seem like they're really focused on them hosting the blog, but you can still self-host and all that?
[2041.78 --> 2050.02]  Self-host out of a container, yeah, and I've actually got a custom theme, so I spent quite a bit of time before the Perfect Media Server 2020 edition came out,
[2050.02 --> 2058.02]  making sure that my blog had search and a few other different, you know, like fav icons and social media icons, all that kind of crap.
[2058.02 --> 2064.52]  So you can customize the theme relatively easily, and all of that stuff is open source in GitHub.
[2064.80 --> 2067.60]  So, you know, I have no complaints about Ghost at all.
[2067.66 --> 2069.02]  It just does exactly what I need.
[2069.20 --> 2073.60]  It looks pretty good, and you see it all over the place on the internet, really.
[2073.80 --> 2077.14]  So I think that's kind of, you know, proof is in the pudding.
[2077.40 --> 2080.38]  How many blogs do you see that are in Ghost?
[2080.72 --> 2081.46]  Quite a few.
[2081.56 --> 2082.72]  So yeah, it must be okay.
[2082.72 --> 2088.10]  All right, so I think our final question for today, Tamo writes in about user account management.
[2088.90 --> 2091.92]  Hi guys, I'm a new listener, and this show is perfect for me.
[2091.98 --> 2093.18]  I started at episode one.
[2093.36 --> 2093.88]  Well, thank you.
[2094.58 --> 2099.44]  I was wondering if you have done a podcast about how you manage different servers and user accounts.
[2099.62 --> 2102.74]  Do you have LDAP or some kind of centralized authentication?
[2103.70 --> 2110.68]  I'm finding creating unique user accounts for every server and saving their credentials every time to be a bit of a pain in the bum.
[2110.68 --> 2113.14]  I was wondering if you have any thoughts.
[2113.66 --> 2116.42]  Looking through the episode descriptions, I didn't find anything about this.
[2116.64 --> 2117.92]  Thanks, Tamo.
[2118.24 --> 2120.92]  Good question, because it's been on my mind a lot.
[2121.58 --> 2128.86]  Recently, Linux distributions like Fedora and Ubuntu added checkbox Active Directory support to their installers.
[2129.66 --> 2137.60]  And that got me thinking, yeah, almost wouldn't mind having like an Active Directory setup here on the LAN,
[2137.60 --> 2142.56]  either actual Active Directory or some Samba Frankenstein version of it.
[2142.78 --> 2148.06]  But truthfully, what I have landed on is standardized accounts.
[2148.16 --> 2152.38]  So we have a standardized Studio account, and I have an account on all the systems.
[2153.06 --> 2156.76]  And the people who work here at the Studio, we know those logins.
[2156.76 --> 2159.68]  And then for our server logins, we use SSH keys.
[2160.36 --> 2169.94]  But I do long term have my eye on Systemd HomeD as a potential way to solve this, at least here on the LAN at the studio.
[2170.68 --> 2172.42]  And I'll have a link to that in the show notes.
[2172.50 --> 2179.16]  But essentially, it takes your home directory and all of your user information and puts it into JSON.
[2179.16 --> 2185.72]  And then you can drop this home directory bundle into a Systemd HomeD enabled system.
[2186.06 --> 2191.94]  And not only does your home directory show up there, but you also then become a user on the system.
[2192.56 --> 2195.82]  That's obviously me giving you the short version.
[2196.06 --> 2197.28]  But it has some potential.
[2197.52 --> 2202.68]  So you could see here in the studio where perhaps we'd keep our master HomeD directories on the server
[2202.68 --> 2208.72]  and then R-sync them down to the studio machines in my workstation, I don't know, every hour, every 24 hours.
[2208.80 --> 2209.16]  I don't know.
[2209.48 --> 2210.48]  I haven't really looked into it yet.
[2210.94 --> 2213.84]  But if we did that, it would also sync down our user credentials.
[2214.50 --> 2219.26]  Early days, just something that's on my horizon, kind of keeping on my radar as a possibility
[2219.26 --> 2221.42]  because I don't need something too advanced.
[2221.72 --> 2226.10]  I've managed large LDAP single sign-on installations in the past as part of my job.
[2226.10 --> 2228.90]  And it worked surprisingly well for a long time.
[2228.94 --> 2230.88]  And I just don't really have an interest in doing that anymore.
[2230.88 --> 2233.18]  I mean, you could spin up LDAP.
[2233.26 --> 2234.40]  You could do free IPA.
[2234.48 --> 2235.54]  You could do a lot of things.
[2235.90 --> 2236.90]  You could do Active Directory.
[2237.08 --> 2238.28]  It sounds kind of fun.
[2238.32 --> 2238.66]  I don't know.
[2239.36 --> 2239.76]  Yeah.
[2239.94 --> 2245.72]  But I don't know about you, but I've got to the point over the last decade where I'm managing so many different systems.
[2246.02 --> 2249.54]  Some of them are in different houses or different cloud providers or stuff like that,
[2249.62 --> 2256.72]  that having them sync back to a central authentication would just be so complicated.
[2256.72 --> 2263.14]  I've kind of got, I feel like, half-decent context switching between the different servers and knowing,
[2263.28 --> 2266.32]  oh, right, I don't have that particular setup on this one.
[2266.42 --> 2271.92]  And any files I do need to sync between various things, I have my NAS, and I just mount that via Samba.
[2272.82 --> 2275.44]  And I don't really worry too much about the home directory.
[2275.54 --> 2278.72]  Anything that's in there, in my opinion at least, is ephemeral.
[2279.36 --> 2282.30]  It goes in Git or it goes in Samba or it gets lost.
[2282.42 --> 2283.52]  That's kind of how I treat it.
[2283.52 --> 2284.00]  Yeah.
[2284.40 --> 2294.16]  I think in part it's because I have, in full disclosure, I've accepted a security practice on the LAN of the studio that probably you shouldn't do,
[2294.24 --> 2299.00]  and that is we don't rotate passwords very often, maybe once every couple of years.
[2299.18 --> 2300.00]  But then again…
[2300.00 --> 2300.46]  It's convenient.
[2300.74 --> 2301.34]  I'll give you that.
[2301.62 --> 2301.82]  Yeah.
[2301.86 --> 2305.24]  And as far as physical access goes, it's a real small handful of people.
[2305.70 --> 2308.92]  It's not like an organization with an office of 20 here.
[2308.92 --> 2318.34]  And then for the servers, it's pretty much all down to SSH keys, and all remote login is usually done with that.
[2318.46 --> 2322.80]  Any access to the LAN is done with WireGuard, and that has its own set of keys.
[2323.20 --> 2324.74]  So there's some layers there.
[2325.24 --> 2327.66]  Every now and then, I still think it's a fair question.
[2327.74 --> 2331.16]  I still think to myself, I could do this a little better.
[2331.16 --> 2339.02]  And I do fantasize about a future where I deploy everything pragmatically, and then everything has central sign-on and central storage.
[2339.72 --> 2343.04]  But I think I'd have to clone myself to get there.
[2344.08 --> 2345.94]  But this goes back to the point at the beginning, right?
[2346.02 --> 2348.56]  You use Arch because you just want to get stuff done.
[2348.78 --> 2354.20]  And I think we don't use a central authentication system because we just want to get stuff done.
[2354.20 --> 2364.50]  We don't want to spend the week or two figuring it out and setting it up, and then every time we reinstall a box, attaching it to a domain controller or whatever it is.
[2364.82 --> 2364.94]  Right.
[2365.34 --> 2368.84]  I think it's just pragmatism, isn't it, that means we're lazy and don't do it.
[2370.32 --> 2371.40]  Maybe that's a bit of it.
[2371.66 --> 2372.54]  We've gotten old.
[2372.74 --> 2378.12]  What we need is a young SSH intern to come into the studio and whip us together and get a single sign-on going.
[2378.52 --> 2379.72]  Yeah, maybe, maybe.
[2379.72 --> 2385.10]  Thank you to our members over at selfhosted.show.sre.
[2385.22 --> 2386.40]  Thank you for supporting the show.
[2386.58 --> 2394.36]  As a thank you, we supply you a limited ad version of the show, and you also in that feed get extra content the post show.
[2394.52 --> 2397.80]  Thank you very much to our members at selfhosted.show.sre.
[2398.28 --> 2402.86]  We're going to have a little bit of a 3D printing hoedown in the post show today, I think.
[2403.24 --> 2407.00]  Yeah, I look forward to that, and I also have a bit of a confession to make.
[2407.00 --> 2409.20]  Just a little bit of business before we go.
[2409.20 --> 2412.04]  Everything we talk about is over at selfhosted.show.
[2412.18 --> 2416.28]  As always, you can go to selfhosted.show.com for all the ways to get in touch with us.
[2416.72 --> 2418.84]  And you can find me on Twitter at Ironic Badger.
[2419.04 --> 2423.50]  I'm there too, at Chris Elias, and the show at selfhosted.show.
[2423.84 --> 2426.18]  On Discord, I'm at AlexKTZ.
[2426.72 --> 2427.46]  Thanks for listening.
[2427.74 --> 2429.10]  That was selfhosted.show.com.
[2429.10 --> 2430.02]  Slash 39.
[2430.02 --> 2430.10]  Slash 39.
