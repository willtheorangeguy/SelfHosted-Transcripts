[0.00 --> 5.68]  Coming up on Self-Hosted 14, Wendell's back. He joins us and we talk about the perfect low-power
[5.68 --> 12.64]  home server, some great ideas for a firewall, and why Alex has orange knobs all over his office.
[13.08 --> 13.48]  I'm Chris.
[13.90 --> 16.02]  And I'm Alex, and this is Self-Hosted 14.
[17.34 --> 21.22]  Welcome back to Self-Hosted. It's great to be here with episode 14, and Alex,
[21.28 --> 22.30]  we have a special one today.
[22.62 --> 23.20]  Another one.
[23.34 --> 23.76]  I know.
[23.98 --> 26.98]  Another special episode. I feel like every episode's special.
[26.98 --> 30.06]  It's like I used to say every show was a big show, but now they're not as long,
[30.16 --> 35.12]  so now they're just special shows. But this one really is because Wendell is joining us. He was
[35.12 --> 38.62]  on episode one, and we knew we'd want to have him back. So, Wendell, welcome back to the Self-Hosted
[38.62 --> 38.94]  Podcast.
[39.82 --> 44.28]  How's it going? I've been following the show, and there are so many people that are like,
[44.94 --> 46.44]  yes, Self-Hosted.
[48.16 --> 52.12]  Before we start, Alex, we had something we had to cut from last week's episode.
[52.78 --> 56.96]  Do you want to just maybe start with that, a little tip you had with, I think it was SSH Shuttle?
[56.98 --> 64.48]  SSH Shuttle is one of those tools. I've used it for several years now, and obviously this
[64.48 --> 71.86]  predates WireGuard being a thing, and it lets me tunnel traffic over SSH and essentially creates
[71.86 --> 78.22]  a poor man's VPN over SSH. So, I used to use it a lot when I worked in a bank, and they had a very
[78.22 --> 85.94]  restrictive outbound SSH policy. So, I used to use that in conjunction with Corkscrew out on port 443
[85.94 --> 93.72]  to make all my traffic look like what was SSL traffic, and then I could route all my DNS through
[93.72 --> 100.08]  that tunnel as well and get to any website I wanted. The point for me being was that I could
[100.08 --> 105.52]  actually get to my homeland very easily that way. I wasn't really too worried about going to silly
[105.52 --> 112.46]  sites at work. But yeah, it's a tool that I've used for many years, and I've had a blog post sat in
[112.46 --> 118.46]  drafts for what must be four years at this point, and I looked at it. I sat at Nashville Airport last
[118.46 --> 123.20]  week, and I thought, you know what? I need to publish this post. So, here we go.
[123.46 --> 128.52]  Good. We'll link that up in the old show notes. That's a great tool. I might actually play around
[128.52 --> 129.88]  with that myself. So, thank you.
[129.88 --> 135.72]  It's really nice. I use it a lot for Red Hat stuff. We have an internal VPN that we have to
[135.72 --> 140.84]  connect to, and I have a droplet that's running that's perma-connected to that VPN. And so,
[140.88 --> 147.36]  when I want to route traffic through the internal VPN to view the intranet or whatever, I have a
[147.36 --> 152.90]  bash alias that routes all my traffic for those few minutes through the tunnel and then through the
[152.90 --> 155.14]  droplet into Red Hat, and it works really nicely.
[155.14 --> 159.92]  That's a great tip. That's something I'm going to check out. Now, I had a realization this week
[159.92 --> 165.42]  that I wanted to share with you guys. Curious if this happens to you. So, at home, I have several
[165.42 --> 169.28]  Raspberry Pi 4s that I set up doing various different jobs. I think I've talked about it quite a bit on
[169.28 --> 176.16]  the show. But I had a realization that the details of how I set it all up are already beginning to fade.
[176.78 --> 180.66]  Do you have this happen where you just, you go all out on something? It's like a passion project,
[180.66 --> 181.98]  and then the details fade away?
[183.16 --> 187.00]  I'll give you one better. You go all out on a passion project, and then you're like,
[187.52 --> 192.54]  oh, wait. And then this just random thought occurs to you, and then it's like, I know,
[192.82 --> 197.22]  instead of putting this in the wiring closet with everything else, I'll put it here. And then you
[197.22 --> 200.58]  open up that cabinet, and there's already one there. And it's like, did I already do this and forget?
[200.58 --> 209.42]  I don't think that's ever happened to me that I've forgotten a piece of hardware exists. But I could,
[209.72 --> 213.74]  you know, having been to your place, I can imagine that's happened once or twice.
[214.24 --> 218.28]  Yeah, it's sort of a reminder that you're kind of predictable in a sense, because I've also done
[218.28 --> 222.12]  that with, like, oh, I need to save something on the computer, and I'll download a PDF, and I'll go
[222.12 --> 225.86]  to put it in a very specific place, so that way I can get to it later. And I'll open the directory,
[226.32 --> 230.12]  and the PDF is already there. And I've already done it. I just completely forgot that.
[230.12 --> 236.28]  Yeah, that's where I'm at. And I did do some documentation. So I'm not totally out in the
[236.28 --> 241.40]  woods. But I'm looking at it now, and I'm thinking, I wish I would have done this through
[241.40 --> 247.30]  some sort of automated deployment. Because the scenario I now fear is I've become super dependent
[247.30 --> 252.94]  on this hardware. And I'm just concerned about hardware failure. And if there's a hardware failure,
[253.34 --> 259.52]  because they are Raspberry Pis, they are swappable. So in theory, I could just take a dead one out,
[259.52 --> 264.86]  put a fully, who even cares what's wrong, right? Just buy an extra one, swap out the dead one,
[265.06 --> 271.76]  put in a good one, and then have something reset it up completely, as per some system. And I just
[271.76 --> 273.18]  haven't done that. And now I'm regretting it.
[273.64 --> 278.32]  Yeah, that's where that's where I am right now. I've got the four gig Raspberry Pi with the POE hat
[278.32 --> 283.78]  with the fixed USB-C power, and all of that. And it's like, yes, finally. And I've been experimenting
[283.78 --> 289.38]  with the Watchdog thing for about the last six months or so, like six or eight months. And the
[289.38 --> 296.14]  Watchdog thing works really well. But you can also Ethernet boot the Raspberry Pi. And so it's like,
[296.48 --> 300.62]  do I even need storage for the Raspberry Pi at this point? Because that's another point of failure.
[300.74 --> 306.00]  And maybe I can just be like, no, this Mac address boots and has this hat attached to it. And I can just
[306.00 --> 307.02]  sort of go from there.
[307.02 --> 311.04]  Do you still need the SD card for that, though? Even for Pixie booting?
[311.52 --> 316.74]  You might, just for like the bootloader or whatever. There's nothing actually stored,
[316.92 --> 321.86]  like you wouldn't need to do anything. Although it may be able to load from the EEPROM,
[322.36 --> 326.60]  because some of the documentation online is like, oh, there's an EEPROM that blah, blah, blah. And
[326.60 --> 329.06]  it's like, does that actually work? I don't know. I haven't gotten there yet.
[329.44 --> 332.08]  Can I trace back a little bit? What's the Watchdog thing?
[332.08 --> 337.94]  On the Raspberry Pi, you can load a kernel module that if you don't poke the Watchdog every 10
[337.94 --> 342.62]  seconds, it will hard reset the Raspberry Pi. So if the Raspberry Pi locks up or has some sort of
[342.62 --> 347.16]  hardware failure or overheats or something, it will just reset itself.
[347.32 --> 351.02]  And that's not going to cause any issues with the SD card corrupting itself or?
[351.34 --> 352.54]  Well, that's why I want a PXE boot.
[352.86 --> 354.08]  Ah, yes. Yep.
[354.32 --> 358.90]  If not PXE boot, the SD card should be completely read-only, maybe mechanically read-only,
[358.90 --> 363.30]  and just a super, super, super minimal boot environment. Although there's the security
[363.30 --> 368.02]  consideration with that, but I'd rather just completely raw boot and deal with it from there.
[368.76 --> 372.70]  Right. And then you could just have another SD card standing by if that one were to die for
[372.70 --> 375.92]  some reason. Just if it's such a minimal boot environment, it doesn't need to do much.
[376.68 --> 382.78]  But how do I do all of this? Like, what is too much for a home project? I don't want to create
[382.78 --> 386.72]  another monster that within six months, I'll forget how it's set up. That's what I'm worried about.
[386.72 --> 391.02]  And that's where I am too, because it's like, I don't know. For me, most of the Raspberry Pi stuff
[391.02 --> 395.94]  is just information logging and monitoring and a tiny, tiny little bit of control. So like,
[396.02 --> 399.58]  you know, the amazing Grafana dashboard that's like, this is what the boiler is doing. This
[399.58 --> 402.64]  is the pressure and this is the thing over time. And this is the other stuff that's happening.
[402.96 --> 404.96]  Yeah. Yeah. It's not the end of the world if you lose it.
[405.58 --> 410.06]  What do you guys tend to use for that kind of thing? Like config management, you know,
[410.06 --> 416.62]  my personal flavor is Ansible and mixed with a bit of Terraform sometimes. What do you use?
[417.02 --> 425.96]  Ansible mostly, although there are a few scripts that are just a bash script piped into SSH with
[425.96 --> 426.38]  keys.
[426.84 --> 428.72]  That's my setup. That's me over here.
[429.10 --> 433.42]  I don't think there's anything wrong with that, really. I mean, if you're being a super elite
[433.42 --> 438.38]  hacker, like Popey last week was giving me a hard time that I'm an elite hacker because I like IRC.
[440.06 --> 444.48]  No, I don't think that's true, but I think bash scripts do have their place. And coming back to
[444.48 --> 449.26]  your point, Chris, sometimes if you build a complex house of cards that you don't fully understand,
[449.42 --> 457.00]  you then don't touch it. So the magic bullet to making config management work for me is that you
[457.00 --> 463.44]  have to ensure every change you make to a system is made through that config management tool. So if
[463.44 --> 467.86]  you want to install just one package, you add that to your dictionary of packages or whatever,
[467.86 --> 472.76]  run Ansible and it goes and installs that one package. I'm going to explain Ansible very
[472.76 --> 481.60]  briefly for those that aren't familiar with it. It's an SSH based tool that is a declarative state
[481.60 --> 487.62]  type tool. So you say, I want my system to look like this. I want it to have these packages. I want
[487.62 --> 494.50]  Samba config to look like this, et cetera. You run the Ansible playbook command. It SSHs out to all of
[494.50 --> 499.08]  your different hosts and does all of the stuff based on what's in the playbooks. Once the playbooks
[499.08 --> 504.46]  have executed, the host state should match what is declared in the playbook, hence the declarative
[504.46 --> 513.12]  state name. And so if you let that config drift on those nodes from the declared state in the
[513.12 --> 518.66]  infrastructure as code type playbooks that you've written, you end up with this config drift between
[518.66 --> 524.08]  the two and it becomes really hard quite quickly to reconcile those differences unless you're quite
[524.08 --> 530.92]  strict about it. Even things like just minor point upgrades to the underlying distro can cause a
[530.92 --> 534.16]  problem. And then it's like, Oh, I didn't really want to spend three hours troubleshooting this today.
[534.62 --> 538.32]  Yeah. That's the thing. That's that happens. So what are you thinking, Chris? You want to do that
[538.32 --> 543.96]  for your pies now? Yeah. Although I am worried that's a bit much, but is it? So here's what my
[543.96 --> 549.34]  alternative is, is like an image based approach. Once a month, I pull out the SD cards and it's
[549.34 --> 552.84]  very manual. So it's very unlikely, isn't it? I mean, even just saying it out loud, I started to
[552.84 --> 558.60]  think it's a bad idea, but that's what I was thinking was just images and then duplicati gets
[558.60 --> 566.16]  the config data offsite and the actual large data is stored on a spinning disc or actually it's a solid
[566.16 --> 573.52]  state disc, not an SD card. So the OS really just has to get back to base. Then I could pull down the
[573.52 --> 579.88]  latest containers, restore the configs with duplicati, but it's a lot of manual work.
[579.96 --> 585.62]  That's probably a good couple of hours. And that's it for me. Like containers have changed how
[585.62 --> 590.88]  disposable my hosts are. I don't really care if my, if my host dies because all my data lives on
[590.88 --> 595.48]  some persistent storage somewhere else and the application is separated from it. So.
[596.04 --> 601.76]  Yeah. I almost, yeah. I don't know. And I don't know what point I should pull the eject
[601.76 --> 606.06]  lever and just say, okay, I have to go to some massive management system or if I just.
[606.36 --> 609.28]  Ansible's not a massive management system. I think if you've never used it before,
[609.28 --> 611.46]  there is this kind of fog. Yeah.
[611.70 --> 615.70]  But it's, it's like half a day's effort, I think to, you know, de-mist the fog.
[616.10 --> 618.56]  Oh really? Yeah. I'll give you some help.
[619.02 --> 621.88]  All right. Then that might be the route I want to go. If you think it's not,
[622.04 --> 624.70]  see, that's kind of, I just didn't want to have to bite off like a whole new thing,
[624.70 --> 627.70]  but I actually don't mind picking up something new really. It's, it's not,
[627.70 --> 633.50]  if it's not so bad, I can do it. Now let's talk about hardware whilst we have Mr. Wendell with us.
[634.36 --> 638.94]  One of your recent videos was all about the new Fractal case. They've gone in a really
[638.94 --> 644.96]  interesting way, really interesting direction. Yeah. Um, well it's the, it's the Fractal Define
[644.96 --> 652.32]  7 XL and the 7 and the 7 XL, I wasn't expecting to like it. It's just a giant tower case. I wasn't
[652.32 --> 657.00]  expecting to like it as much as I did, but it was like, man, this case would be perfect if it had wheels.
[657.00 --> 660.76]  And it's like, is there a wheels option? And they're like, no. And it's like, wait,
[660.90 --> 667.76]  I have a 3d printer. I can fix this. So I 3d printed my own adapters for the feet. And so I
[667.76 --> 672.24]  went through a couple iterations. Like this is like an early iteration, but it's sort of,
[672.48 --> 676.56]  it sort of centers the wheel actually on the screw. Um, cause I thought that would be a little,
[676.66 --> 681.32]  a little mechanically stronger, but it turns out like sort of sort of this like saddle thing
[681.32 --> 686.82]  is a better approach. And then I ended up 3d printing a, uh, a donut shaped hole.
[686.82 --> 691.84]  In the foot so that you can feed a zip tie through it. And the whole thing will go inside the case
[691.84 --> 699.38]  and you can screw and zip tie the foot to the case. And then you've got the wheel that will go in like
[699.38 --> 704.74]  this. And so you can have a really nice case on wheels. That just looks like an office chair
[704.74 --> 709.96]  caster, like a roller blade wheel or something. Yeah. That's literally, uh, this is, uh, this like,
[709.98 --> 713.62]  you can order these on Amazon. So like, if you have hardwood floors, you're not supposed to use
[713.62 --> 717.12]  office chair casters on harbor floors. Cause it'll wear a hole in it. You get, you get these
[717.12 --> 723.82]  and that's literally what this is. It's just an office chair caster that goes in there. And then
[723.82 --> 728.34]  this screws into the bottom of the fractal case. And then you have a pretty nice full tower case.
[728.34 --> 732.40]  That's really heavy and we'll roll around. Now, is there a way you could figure out
[732.40 --> 739.10]  a reason to charge $400 for those wheels? Because I knew you were going to go there.
[739.36 --> 745.34]  No, it's like $35 on Amazon and like a dollar of plastic. So. Hmm. Okay.
[746.74 --> 754.58]  Also 3d printed a, uh, an M.2 hot swap. So like not really hot swap, but like for like a U.2 device.
[754.58 --> 759.46]  And so you just zip tie the connector in the end here. And then the U.2, two and a half inch
[759.46 --> 764.38]  NVMe SSD just slides in. And so I've got these laying in the bottom of the case as well.
[765.02 --> 768.74]  And, uh, so it's like, Oh, I need to, you know, pop in a different Linux distro or whatever. I'll
[768.74 --> 772.98]  just pop out my main hard drive and pop in a new hard drive and it's PCIe connected and it's out of
[772.98 --> 779.40]  the way and it's nice. That is great. These are those wonderful Intel, what four terabyte SSDs
[779.40 --> 784.02]  that you found. Yeah. They're on eBay, right? Yeah. I bought a few of those. They're hard to get now,
[784.02 --> 789.32]  but, uh, yeah, yeah, it turns out they're, they're kind of nice. And this has got standard two and a
[789.32 --> 795.62]  half inch drive, uh, like screw holes in it. So you just screw this in the same way that you would
[795.62 --> 799.72]  a two and a half inch drive. And it's a lot taller, obviously. Doesn't that look like a tie fighter to
[799.72 --> 804.00]  you, Chris? Yeah. I could, you could, that's a good way to describe it. Yeah. Visualize a tie
[804.00 --> 807.70]  fighter folks. And that's kind of what it looks like. That's a great idea. I got to get one.
[807.70 --> 814.08]  Yeah. I think zip ties are really underrated in, in kind of low, low budget things like this.
[814.28 --> 819.00]  I use them for all my drones and stuff. They're a major mechanical component of the Prusa 3d printers.
[819.32 --> 825.78]  Yes, they are. Yeah. Yeah. I have two sat behind me. I have one of the minis and the i3. I love it.
[825.98 --> 829.34]  Yeah. That's what these were printed on. It works. It works really well for, for what it is.
[829.54 --> 835.34]  So, um, slight tangent about 3d printing for a moment. How, uh, how did you get into 3d printing?
[835.76 --> 841.94]  Uh, I needed to make things that didn't exist when I got a 3d printer. It was like very early in the
[841.94 --> 845.40]  maker bot days when they were open source and you could kind of get it out of like the laser cut wood.
[845.66 --> 848.74]  And the first 3d printer that I had was basically made out of laser printer parts.
[848.74 --> 853.56]  Cause it was like, Oh, step promoters laser printer. Yeah. I thought that I would be doing
[853.56 --> 857.32]  a lot more creative stuff with it because I was pretty good with AutoCAD in terms of like,
[857.40 --> 859.24]  cause I'd had some experience with CNC machining.
[859.40 --> 861.04]  You still using AutoCAD now?
[861.36 --> 867.00]  No, no. Uh, I made these with just Tinkercad, which is infuriating because it doesn't give you
[867.00 --> 872.06]  a CLI interface. Like with AutoCAD, it sort of taught me to just not even use the mouse to just
[872.06 --> 876.64]  visualize the part that I wanted to build and start typing coordinates. And, uh, cause like using the
[876.64 --> 880.38]  calipers and doing the CNC thing. And that works brilliantly with, with AutoCAD when you're going
[880.38 --> 885.82]  to do that. But if you, you know, need to use the mouse and it's not, not good. 90% of what I make
[885.82 --> 893.20]  in the 3d printer is parts for something that I've lost or something to fix something. So like I've
[893.20 --> 897.50]  got a bookshelf, I've got a bunch of bookshelves that have adjustable shelves. And sometimes I'll
[897.50 --> 900.54]  put tall things in and so I'll take a shelf out and then I'll rearrange. And then it's like, okay,
[900.54 --> 904.42]  I need to put that shelf back in and a little plastic things are gone. And they're not just pegs.
[904.42 --> 908.92]  They're like the ones that like the shelf snaps into it. And so I have about seven different
[908.92 --> 913.36]  models of those and it's like, Oh, time to rearrange the shelf. I'll just go and 3d print
[913.36 --> 919.38]  some more clips. And that's just what I do. Right next to me here. I have a pair of Ikea
[919.38 --> 924.58]  lack tables. I'm going to point them on the webcam to you both. And they are stacked together
[924.58 --> 929.52]  with two or no, well, obviously four, one for each leg, 3d printed things with a couple
[929.52 --> 934.14]  of screws. And it is brilliant. And then my 3d printer station behind me, like you can see
[934.14 --> 939.30]  all the orange, everything orange is, is 3d printed and designed in ID. I use fusion
[939.30 --> 942.40]  360, which Oh yeah. The hobby license for that is nice.
[942.54 --> 947.22]  The hobby license only lasts a year. It's the education license that's in perpetuity.
[947.42 --> 951.26]  So you've got to be careful with that, but it's annoying because it tethers me to windows
[951.26 --> 957.58]  and I've got Adobe stuff and fusion 360 that tethers me to windows, which gives me an excuse
[957.58 --> 964.04]  to do PCI pass through, but I'd really rather not have to. And you know, it could be worse.
[964.54 --> 971.36]  Yeah. At least it works, Alex for the most part. It's funny. You say anything orange was 3d printed.
[971.44 --> 976.22]  There's just your whole office is covered in orange little things everywhere. You put it all together.
[976.74 --> 977.86]  Yep. Kind of is.
[977.86 --> 984.12]  I've got a few videos that are coming out. And the first one is on, uh, something called, uh,
[984.32 --> 989.58]  the iron fireman. And I think I'm going to take an old thermostat cause it's, it's literally,
[989.58 --> 993.94]  it's a coal loader for the boiler, but the thermostat part of it still works, but it's mercury
[993.94 --> 999.68]  switch on a spring. So it's not super sensitive. I think I'm going to retrofit that. Did you see the,
[999.68 --> 1005.30]  uh, the hackaday mod that was the rotary dial cell phone. I'm going to try to take a raspberry pie
[1005.30 --> 1011.92]  W and shove it inside this thermostat and modernize it and 3d print all the stuff to make it actually
[1011.92 --> 1020.64]  kind of nice. But, um, there's a tiny, tiny little OLED, um, SPI screen that is just about as wide as
[1020.64 --> 1026.10]  the thermostat. And it is, it is taking every fiber of my being to resist having some kind of a thing
[1026.10 --> 1031.44]  to where when you get close, there's a proximity or something. And a servo causes the screen to lift
[1031.44 --> 1035.72]  out of the thermostat. Like I really want it, but it's so anachronistic because it's, you know,
[1035.72 --> 1040.56]  just a brass cover with some knobs for setting day and night temperature, but it's like, you get
[1040.56 --> 1045.42]  close to it and I want an OLED screen to like, just pop up out of it, you know, and then powered
[1045.42 --> 1050.88]  from a piece of cat six or something. And that'd be amazing. It would be really great. I want that too.
[1051.06 --> 1058.06]  Yeah. That does sound awesome. I want that. Well, I kind of have a, I have a hardware question.
[1058.06 --> 1062.46]  One that's a bit of a conundrum. So maybe I could pick both your brains on this one.
[1063.04 --> 1068.82]  Uh, I think my next, my next piece of hardware for my home setup, it's gotta be my edge device,
[1068.90 --> 1073.96]  my firewall. So right now I have that GL, what's it called? The GL net, those little tiny
[1073.96 --> 1076.36]  routers, Alex, that we've talked about before on the show.
[1076.80 --> 1081.64]  Yeah. The new version that we mentioned, I forget what episode it was like two or three or something.
[1081.70 --> 1082.34]  The slates.
[1082.34 --> 1088.90]  Yes. Yes. The slates. That's it. Which I really like because it has a great UI that lets you switch
[1088.90 --> 1095.14]  between multiple upstream network options. So my five, wifi, cat five, whatever. You can just switch
[1095.14 --> 1098.38]  between them through their GUI. But if you don't like that, you can drop under the hood and it's
[1098.38 --> 1103.80]  got a nice Linux command line and it works pretty well, but it's, it's very, um, appliance based.
[1103.80 --> 1110.12]  It's not very flexible. And the number one issue I have with it is, although it touts some level
[1110.12 --> 1115.44]  of wire guard support, there doesn't seem to be quite what I want. So I'm thinking about building,
[1115.66 --> 1120.62]  I don't know anymore if I should go with open sense or PF sense, but I'm thinking about building
[1120.62 --> 1126.72]  a new edge device that also has wire guard support that would allow me to select multiple networks
[1126.72 --> 1131.86]  from different options at different times. Uh, but let me keep all of the devices behind the LAN.
[1132.62 --> 1137.20]  You know, they stay the same, their IPs don't stay, their IPs don't change. And that the edge
[1137.20 --> 1141.22]  device needs to provide DNS for the LAN. So I can resolve all the LAN devices by name,
[1141.60 --> 1147.72]  those basic kinds of things. So obviously DHCP DNS, uh, I'd even like to provide NTP for the home
[1147.72 --> 1154.42]  network, but some of the key things I'd want is low power. If possible, low noise is requirement.
[1154.42 --> 1161.90]  And even fanless would be ideal. Is this a thing that exists? I would probably, it's not fanless,
[1161.90 --> 1167.56]  but it's a lot of horsepower. I'd probably go with, um, like the Ryzen embedded, which is probably
[1167.56 --> 1173.80]  like way, way, way extreme maximum overkill for your needs, but you can spin up micro containers
[1173.80 --> 1178.50]  and microservices. Like you can start with PF sense, but then you can expand that into a full free,
[1178.60 --> 1183.68]  free BSD installation, but maintain the PF sense GUI because that will give you containers. And then
[1183.68 --> 1188.44]  you can start running jails and then inside the jail, you can start running Docker and stuff like that.
[1188.44 --> 1193.16]  Cause I've been experimenting with modifying PF sense to be able to better support things like
[1193.16 --> 1201.32]  land cache for steam caching. Yes. So like I did this, this work with, uh, uh, Dr. Uh, Ian Cutras at,
[1201.32 --> 1208.70]  um, Anantech and, um, the Chinese servers. And so like the, these are, you know, sort of the forbidden
[1208.70 --> 1213.38]  technology. It's like, this is, you know, don't do business with these companies, blah, blah, blah. But
[1213.38 --> 1218.12]  it's like, I must explore the technology. And so, uh, that's on a secure network. And the way that
[1218.12 --> 1224.66]  that works is there's a PF sense machine that has a VPN connection and all of the traffic is tunneled,
[1224.66 --> 1229.82]  but it's also logged. So like every packet in and out is logged and it doesn't matter what protocol
[1229.82 --> 1234.06]  it is because sometimes you can hide things in non IP protocol stuff because people always forget
[1234.06 --> 1239.00]  about that. Or, you know, like weird, like, Oh, this looks like a, one of those really weird,
[1239.00 --> 1243.42]  you know, like IGMP packets. And it's completely benign. And it's like, Oh no, this is actually a way
[1243.42 --> 1248.72]  to exfiltrate data. Yeah. It's like, yeah, it's not good. So I've got a fairly elaborate setup on
[1248.72 --> 1254.58]  PF sense where it has, you know, the LAN interface and then it has like the red zone. And then it has,
[1254.64 --> 1259.58]  you know, a bunch of other interfaces and a couple of VLANs. And there's more stuff running
[1259.58 --> 1266.78]  on PF sense than you normally would for things like packet capture and analysis and IDS. And those
[1266.78 --> 1274.24]  things chew up a fair bit of, of horsepower, really super inexpensive option are those ultra small
[1274.24 --> 1278.82]  form factor Dells. Like you can get, you know, a Haswell or Ivy bridge. I mean, Intel mitigations
[1278.82 --> 1283.98]  aside, but you can get Intel, you can get like the Ivy bridge or Haswell micro form factor Dells down for
[1283.98 --> 1289.60]  like a hundred bucks and throw in eight or 16 gigs of RAM in those. And they're not fanless, but they're
[1289.60 --> 1295.00]  whisper quiet, at least until one of the fans die, throw in a quad port Nick. And you can do a lot with
[1295.00 --> 1299.44]  that. That's a great suggestion. Yeah. As long as it's fairly quiet, really, that's probably fine.
[1299.72 --> 1303.64]  And you can also just, you know, roll straight Linux on it if you want. That's an option.
[1304.08 --> 1309.16]  And not bother with the whole PF sense stuff. Yeah. That has also crossed my mind is just do a Linux
[1309.16 --> 1317.24]  box and then just roll bind, do wire guard by hand, set up DHCP. It's in fact, roll Linux box and maybe
[1317.24 --> 1322.24]  put pie hole on there to just make a few things easy in a container. Yeah. Like having the whole thing,
[1322.24 --> 1325.50]  that's, that's where I'm going is like not even doing very much on the host at all.
[1325.92 --> 1333.48]  Literally everything is container. Everything is, uh, you know, Docker compose or Ansible or whatever.
[1333.98 --> 1338.52]  And if those containers all live on one machine, great. And if those containers need to be split
[1338.52 --> 1343.28]  up across a couple of different machines, great, but all of it sort of works together because like
[1343.28 --> 1350.08]  the, the pie hole and the land cache for steam game caching and other game caching and all of that,
[1350.08 --> 1354.76]  all of that magic depends on DNS. Plus you also want the DNS experience to be like the most amazing
[1354.76 --> 1358.94]  thing ever. Cause if your local DNS resolver is garbage, your whole internet experience is going
[1358.94 --> 1363.84]  to feel like garbage. So you want that to be as good and fast as possible. And then maybe it's
[1363.84 --> 1368.46]  worth having a premium device for that. That is very good point. Can you talk a little more about
[1368.46 --> 1373.24]  the steam cache aspect and how it requires DNS? Because that's something I definitely want to get set up.
[1373.44 --> 1377.84]  It's been on my to-do list for a long time. And so I'm curious what I'll need to accommodate
[1377.84 --> 1383.70]  DNS wise to enable it. There's a, a GitHub repository for land cache that sort of goes
[1383.70 --> 1390.84]  into detail with everything, but steam will do a DNS lookup for a record that is expected to be
[1390.84 --> 1395.00]  rewritten by your ISP or local provider or whatever. And you can just do it yourself.
[1395.40 --> 1402.16]  And it does not depend on HTTPS. There's no encryption, nothing like that. And so if you
[1402.16 --> 1407.46]  rewrite that DNS request and you have a corresponding web server that can proxy requests,
[1407.46 --> 1413.20]  then steam is designed to work with a caching system. It's just normally it's like your ISP
[1413.20 --> 1416.06]  that's going to be doing the caching. But in this case, it's you that's going to be doing the caching.
[1416.62 --> 1420.66]  And generally that's true with blizzard and Activision and a bunch of other games.
[1421.28 --> 1427.30]  Sometimes HTTPS becomes a problem because they'll forget and they'll enable required HTTPS. And so
[1427.30 --> 1433.14]  any HTTPS traffic that you have is, is proxied, but not cached because it's encrypted. And that
[1433.14 --> 1437.66]  encryption is sort of temporal. So it might be able to cache it. But then if it goes to play back
[1437.66 --> 1441.30]  the cache later, it's sort of nonsensical at that point in time. So the fact that it was
[1441.30 --> 1447.76]  cached encrypted data doesn't really help you. But most game providers will let you do that.
[1447.82 --> 1452.82]  And Windows Update is the same way. It manages its own integrity checking. So it doesn't need HTTPS.
[1452.82 --> 1456.60]  And so you can get your Windows updates if you have Windows machines on your network or your family
[1456.60 --> 1462.62]  has Windows machines or whatever. Same thing with repositories. So our local, the same container
[1462.62 --> 1469.84]  that is doing Steam caching, also with DNS magic, we're caching Debian and Fedora. And so it's just
[1469.84 --> 1473.42]  completely transparent. And it's like, it's going to download the package and it's going to do its
[1473.42 --> 1478.06]  own integrity checking on the package, even though the connection is not encrypted. But because the
[1478.06 --> 1483.46]  connection is not encrypted, I can have that local cache. And so it's like, oh, it's time to update Debian.
[1483.46 --> 1486.40]  Oh, that's happening at a gigabit per second. That's nice.
[1486.80 --> 1490.98]  Yeah, really? Have you tried it with Ubuntu? Or is it just Debian proper?
[1491.44 --> 1495.34]  No, yeah, no, you can totally do it with Ubuntu. You can totally do it with any other distro where
[1495.34 --> 1503.00]  you can set up an HTTP non-S mirror. And then that URL will be cached if you do some DNS magic.
[1503.44 --> 1507.76]  Guys, that sounds nice. Yeah, I definitely want to do the Steam cache one. Because there are times
[1507.76 --> 1512.90]  when I'm on a MiFi. It's just so brutal. It's so bad. And I just think to myself,
[1512.90 --> 1517.28]  why haven't I set that Steam cache up yet? And that would be a good reason to have an edge
[1517.28 --> 1519.92]  device with a little more horsepower is to do kind of that stuff.
[1520.36 --> 1529.18]  Asrock has a, it's like the Desk Mini A320, I think. It's an APU, but it's got two three and a half
[1529.18 --> 1536.90]  inch bays. And I really, really want to add an M.2 SSD and two four terabyte mechanical hard drives to
[1536.90 --> 1541.68]  that so that it's like a cheap system. And that could be my travel cache system because I find myself in the
[1541.68 --> 1546.12]  same situation a lot of the time where I'm somewhere and like, maybe I'm going to go to
[1546.12 --> 1550.46]  Computex and maybe I want to do hardware testing like in my hotel room, but the hotel room connection
[1550.46 --> 1555.16]  is garbage. And I need, you know, terabytes of terabytes of Firestrike and games and crap like
[1555.16 --> 1559.76]  that. What if I could plug the hardware or laptop or whatever it is I'm testing in with a local
[1559.76 --> 1565.10]  connection? And I've got my little six inch cube of information basically. And it's just shoving all of
[1565.10 --> 1569.80]  the information that I could possibly ever need onto the machine to be tested at wire speed. And then I
[1569.80 --> 1574.52]  don't have to worry about it. That's glorious. I love that idea. I got, I'm making a project
[1574.52 --> 1579.34]  list over here, Alex. I got like a list of stuff I'm writing down over here. All right, I'm going
[1579.34 --> 1585.42]  to do that. You can add that to the pile of shame. Yeah. The things I'll do one day.
[1586.68 --> 1590.82]  I was watching a video. I think it was Jay's two cents. We went behind the scenes at one of these
[1590.82 --> 1596.44]  massive LAN parties where he was, he was talking with the networking team about how they ran fiber to
[1596.44 --> 1602.84]  each row of people doing LAN and they had the, the LAN cache there. And that was really interesting
[1602.84 --> 1608.50]  because he was talking about, I think it was Origin that uses HTTPS, which meant that they couldn't
[1608.50 --> 1613.42]  cache that one particular vendor. And there've been a lot of complaints for that. Uh, as I think it was,
[1613.42 --> 1618.20]  that was Kane and Max CFM and those guys for like dream because Kane does a lot of work for,
[1618.26 --> 1626.12]  for dream hack and they get the world record on, um, the LAN cache speed. It was, uh, 45 or 55,
[1626.12 --> 1631.54]  five gigabytes per second, I think, or was it gigabit? Might've been gigabit. It was fast.
[1631.80 --> 1637.98]  It was insanely fast. Even Linus's mega, you know, crazy super SSD server might struggle
[1637.98 --> 1642.44]  going much faster than that. Wendell, you said something in there earlier that I thought
[1642.44 --> 1647.00]  would be worth touching on. Sounds like you're doing sort of my approach of minimum viable Linux
[1647.00 --> 1653.02]  for the host OS. It's just a really base install for your, for your system. And then everything's
[1653.02 --> 1657.78]  either VM or containers. Yeah. Because repeatability and ain't nobody got time for that.
[1658.08 --> 1664.44]  Yeah. No kidding. Right. I know. Well, and also it's just, it's less to update. It's less to break.
[1664.50 --> 1668.22]  It's less security attack surface. It's a, there's a lot of benefits to it.
[1668.22 --> 1672.12]  The one thing that drives me insane about Docker containers is they never have good
[1672.12 --> 1678.24]  internal log management and you will need that for incident response. So I usually have things that
[1678.24 --> 1682.76]  like in the Docker for the, on the Docker side of it for Docker compose, it's like, okay, I'm just
[1682.76 --> 1686.92]  going to go ahead and map those directories to the host, but I'm also actually going to bother with
[1686.92 --> 1692.56]  log shipping to a machine on the network. That's super hardened just so that there's a logging device.
[1692.80 --> 1697.48]  And then it's like, Hey, I'm not getting a heartbeat from this machine. Then I started getting emails
[1697.48 --> 1702.10]  like something may, and it's, you know, a lot of the time it's just that machine locked up or the power
[1702.10 --> 1706.50]  went out and the battery on the other thing is lasting a little bit longer, but that's a great thing to do
[1706.50 --> 1712.94]  with the raspberry PI as well, because it's not x86. So like the, the script kitty binary exploit is
[1712.94 --> 1719.38]  like, Oh, it's raspberry PI. You can't just, you know, upload a binary and elf binary to it and,
[1719.42 --> 1724.94]  and have it actually work correctly. Right. And the fact that you can, you know, store the logs or
[1724.94 --> 1729.60]  export the logs or send it to something else, or just have it stored there on that device. Then it's
[1729.60 --> 1734.44]  like, it's nice because it's just right there on a separate device. And it's hard to sort of compromise
[1734.44 --> 1739.70]  that and everything else. So let's get to a little bit of feedback. I have an email here from Ian.
[1739.70 --> 1746.40]  Thanks for writing in Ian at ask SSH. Um, it's to do with hardware and he would like to know
[1746.40 --> 1751.74]  with all the AMD hardware releases right now, it's kind of hard to keep track of what is good
[1751.74 --> 1759.28]  for a low power server. What would you recommend as the best bang for budget AMD based system right now
[1759.28 --> 1766.98]  for a 24 seven based system? Best bang for the buck is probably the rise in 1600 AF. If you can find it,
[1767.04 --> 1775.08]  it's like 89 bucks and it's technically a 2600 because the 1600 on the old process sold so well,
[1775.12 --> 1781.12]  they're like, we'll call it 1600 AF. And, uh, it's a little slower than a 2600. So it didn't,
[1781.12 --> 1788.08]  it didn't quite make the cut for a 2600, but it is essentially 2600. And that CPU is incredible and
[1788.08 --> 1792.80]  incredible, you know, bang for the buck. Uh, cause it's basically a 2000 series rising.
[1793.54 --> 1798.96]  Where does that fit? Broadly speaking, I I'm fairly familiar with the Intel lineup. What's the
[1798.96 --> 1805.00]  Intel kind of comparative chip there? Probably one of the Xeon E3s, but it's actually going to be
[1805.00 --> 1809.72]  faster than just about all of the Xeon E3s that are available. Is that in single or multi-thread?
[1810.02 --> 1815.76]  Single thread is going to be close. Uh, it might slightly favor Intel. If you want to beat Intel
[1815.76 --> 1821.90]  in single thread with that Xeon E3, you could go with the Ryzen five 3600 and that's going to be a
[1821.90 --> 1829.48]  six core. And, uh, that will handily outperform any Xeon E3 available today. Coming back to Ian's
[1829.48 --> 1835.74]  question. He's, he's talking about the 24 by seven piece. What's the sort of idle energy draw on these
[1835.74 --> 1840.88]  things? It depends on the motherboard and it depends on the implementation. Um, if you go like super,
[1840.98 --> 1845.38]  super, super low power, which actually is a little tricky to do on Ryzen because you have to have a
[1845.38 --> 1850.94]  power supply that properly supports C6 and some power supplies that advertise the C6 deep sleep
[1850.94 --> 1856.60]  don't actually support the C6 deep sleep. And some power supplies implement the C6 deep sleep as
[1856.60 --> 1862.02]  turn on this big old bank of resistors just to keep things ready in case the system wakes up,
[1862.10 --> 1866.74]  which generates heat. So it doesn't actually consume less power. You gotta, you gotta really
[1866.74 --> 1870.88]  look at the power graph because those it's like, Oh, it's 80 plus gold or it's 80 plus bronze or it's 80
[1870.88 --> 1876.54]  plus platinum. When you start playing with the 1% power utilization, that power efficiency goes to
[1876.54 --> 1882.52]  like 50% or 30%. So like literally half the energy that you're burning, uh, just goes to,
[1882.52 --> 1887.94]  to idle DC to DC converters. In that case might actually be a better choice. Like one of the micro
[1887.94 --> 1893.06]  power supplies, if you really, really want to be super frugal on the power, but it also depends a lot
[1893.06 --> 1898.98]  on the motherboard in terms of like the actual CPU itself. It's on the order of like one or two
[1898.98 --> 1904.92]  watts per core while on the 3000 series plus whatever the IO die is using. So like the CPU
[1904.92 --> 1909.90]  itself in its lowest power state can be around like four or five watts, maybe less than that,
[1909.90 --> 1915.00]  but it really depends on the rest of the system. Wow. That's like Raspberry Pi level.
[1915.48 --> 1917.14]  Yeah. Well, it's not doing anything. So, I mean,
[1917.60 --> 1922.92]  yeah, no, but my Zeons downstairs are doing nothing and they're sucking down 150 watts each.
[1922.98 --> 1923.68]  Thank you very much.
[1924.12 --> 1928.48]  Your power usage is not going to be five watts at the wall, no matter what you do. It's just that the
[1928.48 --> 1933.88]  power usage is going to be dominated by everything else in the system other than the CPU. Sure. So
[1933.88 --> 1937.28]  just keeping the NVMe on standby is going to be five watts.
[1937.86 --> 1942.64]  Oh, that's good to know. I didn't know that. Um, and now a logical question to follow that. And
[1942.64 --> 1947.72]  this one's from me, what sort of motherboards would we be looking at? Is there anything with IPMI?
[1948.42 --> 1956.74]  Yes. Asrock, Asrock rack. Thank you. They have an X470 and X570 board. The X470 board has dual Intel 10 gig
[1956.74 --> 1962.40]  optional and you don't really pay that much more like the board plus a 10 gig card, you know,
[1962.46 --> 1969.22]  is like 350, 300, 350, something like that. And so three to $400 for that board. It's great. It's got a,
[1969.32 --> 1976.04]  it's got the AST 2500, same exact thing that you'd have in a server, full RAM, full VGA implementation.
[1976.04 --> 1981.48]  And with the American Megatrends flavored, uh, implementation of the IPMI, it's got all the
[1981.48 --> 1989.18]  features, the watchdog SSH access command line, the whole nine yards, but it's an AM four platform.
[1989.18 --> 1993.34]  And they just came out with the X570 version, but I haven't been able to source it. I think it's a
[1993.34 --> 1997.44]  little more. I think it's like on the order of $600. And I think that's just an availability issue,
[1997.44 --> 2004.18]  not like an actual expected end user cost. But the, uh, the 470 version is totally fine unless you need
[2004.18 --> 2010.64]  PCIe for, or even more PCIe bandwidth. So I assume those boards require DDR4, do they?
[2010.96 --> 2017.54]  Yeah. Yep. Yep. Yep. Okay. Good to know. So what a total system is going to cost you 400 for the board,
[2017.68 --> 2022.38]  a hundred ish for the CPU, and then what? 150 for 32 gigs of RAM.
[2022.62 --> 2029.16]  You can get unbuffered UDIMs. So I mean, I probably budget closer to 200 for the RAM and get unbuffered ECC.
[2029.70 --> 2033.18]  Okay. That's not bad though. That's a lot of performance for that money.
[2033.18 --> 2034.66]  And that would be a solid box.
[2035.16 --> 2038.28]  Yeah. And I think your idle current consumption on that, if you've got a good power supply,
[2038.34 --> 2039.84]  would probably be around 65 Watts.
[2040.26 --> 2041.30]  That's not bad at all.
[2041.54 --> 2042.68]  Very good. Yeah.
[2043.20 --> 2045.26]  All right. I want to go build one of those. So that's good.
[2045.60 --> 2046.40]  Add that to the pile.
[2047.14 --> 2049.04]  Yeah. Add that to the list of shame.
[2050.64 --> 2058.50]  I can give you a poor man's IPMI and that is a serial port. So here's the project for you. Maybe
[2058.50 --> 2061.72]  we can do a video on this because I already got all the stuff to do this. I just got to document it.
[2061.72 --> 2062.28]  Okay.
[2062.58 --> 2071.68]  It's a Raspberry Pi zero or regular Raspberry Pi if you want. The GPIO pin is wired into reset.
[2072.82 --> 2081.34]  RS-232 is connected to the RS-232 on the host machine. The Raspberry Pi is available on a separate
[2081.34 --> 2086.14]  network or the same network, depending on whatever you want to do. So the Raspberry Pi has enough
[2086.14 --> 2092.98]  wherewithal to reset the machine and it will at least get you to grub. So you can get grub on the
[2092.98 --> 2097.90]  serial terminal and do whatever you need to do as far as manipulating or booting the machine.
[2098.44 --> 2102.88]  That's a really great idea. Can you mount ISOs that way? Is that a thing you can do?
[2103.14 --> 2108.40]  If you wanted to do ISOs, you can't do ISOs over the serial port. What you do there is you put a USB
[2108.40 --> 2113.18]  stick in your computer that already has everything that you need to recover. Or if your motherboard has
[2113.18 --> 2120.30]  one of those onboard micro SD cards, not bootable, or bootable if you want, but you put that in there
[2120.30 --> 2128.00]  that has that stuff that you need on it already. And then you hardwire the BIOS to only boot from the
[2128.00 --> 2133.48]  built-in hard drive and not consider other options. And then from the grub prompt, you can specify the
[2133.48 --> 2136.68]  other partition on the USB stick and use that as a recovery.
[2136.68 --> 2143.10]  I can see it now. I'm ringing my wife when I'm at work. Hey, wife, I've forgotten to plug my USB
[2143.10 --> 2146.42]  stick in. Please go and plug it in. Thank you.
[2146.82 --> 2151.44]  Yeah. It's not as good as an ASP 2500, but for $15, it's not bad.
[2151.72 --> 2154.56]  And it retrofits to any board with a serial port.
[2154.92 --> 2155.14]  Yeah.
[2155.52 --> 2159.06]  Yeah. You should do a video on that. I think people would love that. That's a great idea.
[2159.68 --> 2161.20]  Alex, is there anything else on our list today?
[2161.20 --> 2165.26]  Well, when we went to see you, Wendell, I swear you talked a little bit about a Bluetooth
[2165.26 --> 2168.22]  low energy presence detection beacon.
[2168.46 --> 2171.68]  I finished that. There's a write-up of that on the forum and I haven't released the video,
[2171.80 --> 2176.66]  but probably by the time this is out, I will have released it. Forgetfulness is the only reason that
[2176.66 --> 2180.42]  I haven't released it, but that's on the Linux channel. And there's a write-up on the forum.
[2181.22 --> 2185.56]  It's Bluetooth low energy presence detection for like your house or whatever. And this is really
[2185.56 --> 2190.54]  the only internet of things stuff that I get into that is like genuinely like super useful.
[2190.54 --> 2195.16]  Because it's like, okay, if I'm in the workshop, I want some certain things to happen automatically.
[2195.16 --> 2200.14]  And if I go, well, if I leave the workshop and go into the house, whatever, and the wifi
[2200.14 --> 2204.42]  is not good enough. And wifi also is like, oh, I'm outside. And it's like, you're inside. It's
[2204.42 --> 2209.54]  like, I'm really not, but okay, that's fine. So, um, it would be nice if when I'm outside,
[2209.64 --> 2214.10]  the outside lights are on. And if I'm inside, it doesn't care about the state of the outside
[2214.10 --> 2219.46]  lights. So the logic there is very simple. It's like if outside and outside lights are not on,
[2219.46 --> 2224.94]  turn on outside lights. But if inside don't care about outside lights, if they're on, leave them
[2224.94 --> 2229.36]  on. If they're off, turn them off, but, or, you know, leave them off, but don't mess with the state
[2229.36 --> 2235.82]  of it. If I transition from, uh, inside to outside, turn them on. If I transition from not there to
[2235.82 --> 2242.06]  outside, turn them on. If I transition from, uh, not there to inside, it's probably fine to leave them
[2242.06 --> 2249.18]  alone. So Bluetooth long energy works better for that in my experience than wifi and pretty much
[2249.18 --> 2253.04]  every other technology that I've tried. And so are you just carrying your phone in your pocket
[2253.04 --> 2257.28]  and it's picking that up or do you carry a special, no, just, there's no special tiles or anything you
[2257.28 --> 2261.62]  need to carry. No, you can do the tiles do actually work a little better than the phone because the
[2261.62 --> 2267.18]  sometimes, sometimes the phone puts the Bluetooth thing to sleep to save power, but generally, um,
[2267.18 --> 2271.28]  the phone works fine. They do track people going through shopping centers and shopping malls and
[2271.28 --> 2276.34]  stuff using this, these Bluetooth beacons, uh, cruise ships use a lot of them as well, airports.
[2276.60 --> 2280.56]  So, um, this stuff is being used commercially. So we may as well make use of it at home. Hey.
[2280.98 --> 2285.90]  Yeah. You can, and you can combine stuff like that. I love the idea of it being Bluetooth LE
[2285.90 --> 2289.66]  because you're right. That is going to work better than wifi and you can put all around your house.
[2289.66 --> 2294.32]  The other thing that I've done around the studio, I've got one that you guys, I'll show it to you
[2294.32 --> 2301.82]  guys. It's right here. I have a, these little NFC tags around the studio. And, um, when I, when I
[2301.82 --> 2306.68]  go into an area, I put my phone on that NFC tag and then it triggers a home assistant automation
[2306.68 --> 2311.92]  for me for that area. I like the idea of supplementing location awareness, uh, from
[2311.92 --> 2316.40]  Bluetooth with these tags too, for manual overrides and whatnot. I just want to put one in my mailbox
[2316.40 --> 2321.40]  to know when the mailman comes. When you start to think in terms of like Bluetooth low energy tags,
[2321.40 --> 2326.26]  or even just QR codes, like printed QR codes, suppose that you had like, there was no effort
[2326.26 --> 2329.96]  at all involved. It's like, I'm in the kitchen. It's like, Oh, it's grocery shopping day. What
[2329.96 --> 2333.62]  all do I need? You just open the pantry and there's a sticker on the inside of the door.
[2333.82 --> 2339.80]  If you can effortlessly take out your phone, Hey phone, it's grocery store day, but the abbreviated
[2339.80 --> 2344.10]  way to say, Hey phone, it's grocery store day, not even tapping an icon or like finding the app
[2344.10 --> 2348.88]  among the thousands and thousands of apps on the phone with the completely stupid user interface
[2348.88 --> 2352.98]  of like, you know, scroll, scroll, scroll, scroll, scroll. It's just like, I've opened the pantry
[2352.98 --> 2357.96]  phone. Look at this. It's like, Oh, it must be grocery day. Correct phone. Let's go down a
[2357.96 --> 2364.62]  checklist of things that I usually buy. Yeah. The one that I just did recently is on my exit out the
[2364.62 --> 2371.04]  studio. I tap that with the phone and it sends a text message to the wife with an estimated time of
[2371.04 --> 2376.62]  arrival. And then it waits five minutes and then it brings up ways and my podcast player. And that's
[2376.62 --> 2381.32]  just all, you know, so that way I'm down the road and I'm clear of the wifi network. So I don't have
[2381.32 --> 2385.64]  to wait for the phone to figure out the wifi network versus LTE network. I'm clear of that.
[2385.64 --> 2389.58]  And then those other apps open up and they have a data connection and it kicks off just fine.
[2390.10 --> 2393.54]  Imagine a Bluetooth low energy beacon when you're like sitting at your couch in front of your big
[2393.54 --> 2397.88]  screen TV. And like, you just, you know, touch your phone to the thing and then you're in Plex.
[2397.98 --> 2402.34]  And it's like, not only are you in Plex, but you're in Plex controlling the giant TV. Like you didn't
[2402.34 --> 2406.90]  have to fiddle with finding the app and cast to this and the other thing. It literally is just,
[2406.98 --> 2414.00]  it knows. Damn you Wendell. I haven't done that. I've tried to set that up and it turns out that's
[2414.00 --> 2418.62]  actually kind of a hard problem, but that's because we're using rocks and sticks to try to bang out
[2418.62 --> 2424.12]  these, you know, human interfaces. And we really need somebody to come along and just like, just
[2424.12 --> 2430.42]  set all this garbage on fire and start over. Yeah. It does feel a lot like a stone age sometimes.
[2430.42 --> 2437.78]  Like we humans are still the critical translation layer and sometimes not so perfect. I, although
[2437.78 --> 2441.72]  think we have a theme here, gentlemen, it's essentially automate whatever you can really.
[2441.86 --> 2445.60]  That's what the theme is here. Yeah. How's been throughout the show, I guess, isn't it?
[2445.70 --> 2451.24]  The subtext of that for me is, can you do this in such a way that it is unlikely to bother you
[2451.24 --> 2457.76]  at least for years and years into the future? Like, can I set this thing up so that it works and
[2457.76 --> 2464.28]  is largely automated and I just don't have to worry about it anymore. And, you know, I could see at
[2464.28 --> 2469.38]  some point because the Amazon grocery delivery thing in my area has gotten to the point where
[2469.38 --> 2477.06]  I really want to take some time off and build an interface for like a Kroger, Walmart and Meijer
[2477.06 --> 2483.34]  and Amazon and just have them all fighting with each other for my API grocery list. And I don't want to
[2483.34 --> 2487.92]  buy everything from the API because I really do like to walk around the produce section and the
[2487.92 --> 2493.90]  bakery and, you know, like handpick a few things. But in terms of like grocery procurement, I would
[2493.90 --> 2500.90]  really like to have an application that is, hey, if you buy, you know, two extra cartons of Charmin this
[2500.90 --> 2507.06]  week, it's going to be 15% less overall. And it's like, great, make it so AI that's handling that for me.
[2507.06 --> 2509.10]  Yes, I would love that.
[2509.38 --> 2513.62]  Yeah, I just have all of that be handled. But the fact that you have, you know, three different
[2513.62 --> 2518.20]  grocery APIs that you can interface with, you literally can leverage that. And if enough people
[2518.20 --> 2522.14]  do that, it's going to be a race to the bottom and it's going to be glorious in terms of pricing,
[2522.36 --> 2526.80]  probably bad in terms of local businesses, but probably good in terms of consumer pricing.
[2527.50 --> 2529.62]  Should we approve Wendell's time off request for that?
[2530.12 --> 2532.88]  Yeah, I'll prove that. Yeah, I'll stamp that as long as we get early access.
[2532.88 --> 2537.92]  Well, that's probably it for us today, isn't it, Alex?
[2538.28 --> 2542.76]  Yeah, I think so. So thanks very much for listening. You can find us on Twitter at SelfHostedShow.
[2543.08 --> 2548.06]  And of course, SelfHosted.Show is the website, SelfHosted.Show slash subscribe for all the
[2548.06 --> 2552.14]  ways to get new episodes. And Wendell, give the people a way to catch what you do.
[2552.46 --> 2559.14]  YouTube.com slash LevelOneText or LevelOneText.com. And, you know, definitely if you, if I'm looking
[2559.14 --> 2564.72]  for volunteers to build the AI hotel from Altered Carbon, I've got, you know, two Tesla V100s we
[2564.72 --> 2568.62]  can load into that AI. And so it's just start doing all this stuff for us. And it's like,
[2568.70 --> 2569.96]  great, sounds good. Let's do it.
[2570.42 --> 2573.08]  Of course you are. Why wouldn't you be looking to do that?
[2573.48 --> 2574.52]  I think it's a great idea.
[2576.18 --> 2582.14]  Yeah, do go and check those forums out over on the LevelOneText site. They are a font of wonderful,
[2582.34 --> 2583.14]  wonderful information.
[2583.62 --> 2587.72]  And if nothing else, you can 3D print feet that you can't use on anything except fractal cases.
[2587.72 --> 2591.78]  And so thanks for listening. That was SelfHosted episode 14.
