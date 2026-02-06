[0.00 → 2.24] Would I be a bad man if I ran Arch on the server?
[3.34 → 4.50] You can't do that.
[4.66 → 4.96] Why not?
[5.00 → 6.18] You don't really do that, do you?
[6.66 → 7.10] I might.
[7.58 → 10.00] No, I don't, but I have often considered it.
[10.08 → 12.04] I stream a lot of important things from that server.
[12.44 → 13.82] I have often considered it.
[13.88 → 15.42] No, I use Debian primarily.
[16.68 → 21.04] However, lately I switched out to Ubuntu for the ZFS stuff.
[22.40 → 25.18] And this was after coming to Linux Fest Northwest in April.
[25.18 → 28.86] I listened to Jim and Alan Jude, who are very persuasive gentlemen.
[29.06 → 29.22] They are.
[29.72 → 30.96] They really can convince you.
[31.20 → 37.20] Yeah, and Ubuntu has ZFS baked into the user space tool.
[37.44 → 39.32] All you need to install is a user space tool.
[39.56 → 42.44] And in future releases, it sounds like it's getting even easier.
[43.20 → 47.58] For me, though, you just can't beat the stability of a Debian or a CentOS or something like that.
[47.98 → 48.40] Yes.
[48.72 → 49.36] On the server.
[49.56 → 50.52] On the server, yeah.
[50.66 → 51.10] I agree.
[51.10 → 55.42] I think, actually, if I was going to pick one true OS to rule them all for my personal servers,
[55.62 → 56.62] I would pick Debian.
[57.18 → 57.38] Why?
[57.38 → 63.00] Because it is very much so, out of many of the distros, the most set it and forget it.
[63.10 → 64.68] Even more so, I think, than CentOS.
[64.68 → 67.14] It's just my personal opinion, though.
[67.84 → 69.46] I don't actually run Debian.
[69.82 → 72.74] I get a good sense of stability.
[72.74 → 79.10] Whenever I run apps update or apps upgrade on Debian, there's maybe a dozen packages a week that change, if that.
[79.10 → 79.14] Yeah.
[79.76 → 83.62] Well, I kind of feel like this question is sort of irrelevant, too, in a way.
[83.62 → 91.66] Because in the past, I would avoid using Debian because it was so slow moving that the packages would be horribly out of date.
[91.84 → 93.50] And so it was just not really a contender.
[93.62 → 95.70] That kind of moved me up to Ubuntu and things like that.
[95.70 → 101.92] But now I'm really, to be honest with you, of the opinion that it just doesn't matter.
[102.20 → 111.14] Whichever one you are comfortable managing, and what matters more is how you deploy and run the applications and how you secure them and how you manage all of that.
[111.20 → 113.12] That's like what I think matters a lot more.
[113.18 → 117.52] And then the OS is an implementation detail, and it just needs to be one you're comfortable with.
[117.80 → 118.88] Containers changed everything.
[118.88 → 119.86] Yeah, basically.
[120.00 → 120.94] Or VMs, too.
[121.06 → 122.60] But for me, it was containers, really.
[123.12 → 125.16] Because VMs, you still had to answer that server question.
[125.16 → 126.60] Because VMs, you've still got to pick an OS.
[126.80 → 132.20] Whereas a container, okay, the maintainer has picked a base image to base it off of.
[133.32 → 140.86] It could be an image based on Debian or Arch or Fedora or some other esoteric thing, Alpine or something.
[142.08 → 147.92] But when you're able to separate the application runtime from the base OS, you end up in a situation where, like you say,
[147.92 → 151.14] the base OS doesn't matter anymore.
[151.52 → 158.02] The only time it matters is when you want to have things like extra file system support, like Ubuntu's ZFS support.
[159.12 → 163.62] And, you know, Debian is still a bit old and crusty.
[163.90 → 166.52] And that's what makes it great, in a way.
[166.80 → 167.20] Well, okay.
[167.38 → 172.04] Just going to throw this out to Play Devil's Advocate, just to have a rounder conversation.
[172.92 → 174.16] What about Windows Server?
[174.98 → 175.66] Well, what about it?
[175.66 → 181.14] Well, you get disk management in the, you know, typical Windows disk management stuff.
[181.20 → 183.50] You get some decent features with NTFS.
[183.74 → 188.38] You get shadow copy volumes for your user's data to be safe, which is kind of a nice backup.
[188.78 → 191.26] You've got plentiful application availability.
[191.54 → 194.00] You've even got the capability of running containers.
[194.34 → 197.76] And Hyper-V isn't that bad of a virtualized if you want to run VMs.
[198.12 → 199.56] Containers in inverted commas.
[199.72 → 199.98] Yeah.
[199.98 → 202.30] They're still running a Linux kernel somewhere.
[202.52 → 203.74] I know, but it works.
[204.02 → 204.16] Yeah.
[204.34 → 207.30] So, I mean, what if Windows is the OS you're the most comfortable with?
[207.70 → 213.04] Because from where I've just positioned myself, I've kind of backed myself into that corner.
[213.18 → 216.66] Because if you're running the applications in a container, it doesn't really matter with the host OS.
[216.86 → 217.78] I was just that guy.
[218.04 → 218.56] To a point.
[218.94 → 220.10] Here's my counter to that.
[220.10 → 226.54] Learning Linux is an incredible enabler from a career standpoint.
[227.18 → 234.68] You're investing in yourself by learning these things, by learning about what SSH is, by learning about port forwarding and opening things in your firewall.
[235.24 → 247.26] You're doing stuff that is being done in the enterprise, that is being done in business, that you go to your next job interview, and you can be like, well, hey, I've done X, Y, and Z in my home lab.
[247.26 → 247.72] Mm-hmm.
[248.18 → 250.76] I run these services for my family.
[250.88 → 252.16] I run an Cloud instance.
[252.54 → 257.92] And then I had to set up a reverse proxy that means I don't have to open loads and loads of ports.
[258.02 → 262.48] I can just have a Let's Encrypt certificate that does this stuff automatically.
[262.60 → 265.00] And you can talk authoritatively in an interview on these topics.
[265.12 → 267.38] And that, for me, is the answer.
[268.34 → 270.96] Yeah, that was a big revelation I had not too long ago.
[270.96 → 279.20] I was using enterprise-grade production-deployed tools to run my home lab stuff.
[279.34 → 282.82] And I just thought for a second, it's been a long time since I've done that.
[283.30 → 286.48] That is very much what learning Linux felt like back in the day.
[287.04 → 287.70] So that's a great point.
[287.84 → 295.68] And I can't argue it because the skill set of the future, I made this point on the Linux Unplugged recently, is, quote, unquote, the cloud.
[295.68 → 299.70] When you look at open job searches right now, there'll be a couple of thousand for a traditional sysadmin.
[300.14 → 303.74] And then there'll be, like, 10,000 for a, quote, unquote, cloud admin.
[304.14 → 304.42] Cloud.
[304.66 → 305.94] Yeah, well, the cloud's made of Linux.
[306.28 → 307.60] It's just someone else's computer, you know.
[307.80 → 308.20] It is.
[308.28 → 310.94] Well, it can be your own computer in the case of our preference.
[311.08 → 312.26] This is something I wanted to ask you.
[312.42 → 314.36] Like, what does self-hosted mean to you?
[314.46 → 318.96] Like, for me, it's having something on a box that I control.
[318.96 → 327.80] I think that's kind of the root of it because I consider servers that I run on DigitalOcean to be my boxes.
[328.34 → 328.40] Yeah.
[328.84 → 335.72] Maybe that's not a safe illusion to be under because, in theory, they could just go in there and probably get access to that image.
[335.78 → 337.66] They have root access to the box they're all running on.
[338.82 → 340.00] So maybe I shouldn't feel that way.
[340.00 → 350.88] But I do right now, my current frame of thought is services I've implemented, data I'm responsible for, and applications and security that's totally under my control.
[351.36 → 351.46] Yeah.
[351.88 → 358.12] And there are a number of considerations you've got to make when deciding where to self-host a particular service.
[358.56 → 361.32] Do I host it in my garage or my basement or a closet?
[362.02 → 369.10] Or do I need more uptime than I can guarantee with that and put it on a droplet or an EC2 instance or something like that?
[369.10 → 375.24] And then, obviously, you've got cost considerations when you come on to cloud hosting versus local hosting.
[375.98 → 386.18] So local hosting, you're going to be spending a lot of money up front, probably at least $1,000 to build a system with half a dozen disks and multiple terabytes.
[386.88 → 396.60] Whereas the draw of something like a cloud service, what do you call it, a VPS, is that you can get started in, what, 35 seconds, 40 seconds?
[396.60 → 399.90] And maybe an entry price of $5 a month?
[400.08 → 400.30] Yeah.
[400.56 → 404.02] Which is much easier to eat than $1,000 up front.
[404.54 → 405.52] And there's no power bill?
[406.08 → 407.42] There's no heat considerations?
[408.02 → 412.12] Because I built a new server in September last year, and I have some regrets, you know.
[413.10 → 413.44] Really?
[413.76 → 414.02] Hmm.
[414.42 → 414.82] Hmm.
[414.82 → 425.86] I'd like to talk about that, because I went through a phase where I'm going to try to cloud all the things on boxes I run and have only dumb small appliances in the house.
[425.86 → 433.68] And now I'm swinging back to big rig, lots of disk, draws a lot of power, but also provides a lot of benefits.
[433.96 → 435.62] And I'm not having any regrets.
[436.62 → 438.56] Well, okay, so let me be more specific.
[438.96 → 442.16] I love having 100 terabytes on my LAN.
[442.38 → 442.60] Right.
[443.14 → 444.34] I love being able to...
[444.34 → 445.90] Just think of the cost to do that in the cloud.
[446.90 → 448.28] Well, but you wouldn't do that.
[448.28 → 450.14] It just takes it out as an option, basically.
[450.14 → 450.78] I wouldn't do that.
[450.90 → 454.00] I mean, I needed somewhere to store my drone footage, all of my photography stuff.
[454.38 → 454.70] Same.
[456.00 → 459.70] And I'm sure you've got production requirements for your storage as well.
[459.70 → 468.46] But for me, like, looking at my Power Bell every month, my server draws, it's a dual Leon E5-2690V2.
[468.64 → 470.06] So they're pretty powerful CPUs.
[470.10 → 473.14] They score, like, 15,000 on Pass Mark each.
[473.70 → 477.40] So that is the minimum you want for a 4K Plex transcode.
[477.86 → 482.26] And do you find that your CPUs stay fairly active, like you are using that much horsepower?
[482.38 → 487.58] Because sometimes people, you know, they overbuild, which then gets you down to overpower.
[487.58 → 489.92] And that's where I thought I could go all appliance space.
[490.10 → 493.46] I could have just little small boxes of Raspberry Pi here and NVIDIA Shield there,
[493.60 → 495.56] and then have all the horsepower up in the cloud.
[496.20 → 497.18] That was my dream.
[497.26 → 497.94] I mean, it's tempting.
[498.36 → 498.94] It was.
[499.02 → 501.20] I'm looking at my server load here, and it's currently sat at 11.
[501.96 → 507.34] So they're, you know, 40 thread, 20 core boxes, CPUs.
[507.62 → 510.52] So the work is kind of burst when those CPUs are actually in use?
[510.62 → 511.84] And otherwise, they're kind of sitting there idle.
[512.08 → 512.34] Yeah.
[512.34 → 516.46] Like, when a Plex transcode comes in, it'll burst the first 10 minutes,
[516.52 → 522.10] and then it'll just sort of blip, blip, blip every few seconds the next bit of transcoding.
[522.22 → 525.24] Well, that's a tough call, though, because you do want to overbuild at least a little.
[525.32 → 527.20] So it lasts a while and has plenty of headroom.
[527.40 → 528.58] Well, so here's what I found.
[528.58 → 536.14] Like, Plex has this wonderful offline sync feature where I can effectively download and transcode media
[536.14 → 543.38] from whatever format Plex sees it in to my iPad or to my phone at 8 to 10x speed on these CPUs.
[543.44 → 550.18] I used to have an Atom C2750, one of these old AS Rock boards, Atom 8 core things.
[550.32 → 550.54] Oh, yeah.
[550.60 → 551.16] That was wonderful.
[551.26 → 551.96] It sipped power.
[552.14 → 552.32] Yep.
[552.58 → 556.10] Had like a 30-watt kind of maximum power draw.
[556.32 → 556.46] Yep.
[556.46 → 559.02] And that worked great when it was just me doing Plex.
[560.12 → 562.04] But my new house, I have a gigabit upload.
[562.42 → 564.42] And so I was like, well, let's share the love a little bit.
[565.06 → 566.72] Let's let, you know, you have access.
[566.86 → 571.62] My parents, you know, in England and my uncle in Canada have access to this thing.
[571.88 → 577.46] And you think, well, I want to be able to do at least, let's say, 10 streams at once.
[577.48 → 581.88] And then when you start looking at that, there's a whole rabbit hole you could go down of doing hardware transcoding
[581.88 → 587.40] with this new NVIDIA stuff, NV-ENC, which has come popularized because of Twitch streaming and that kind of thing.
[587.52 → 588.64] But does have some limitations.
[589.42 → 589.68] Yes.
[590.40 → 595.08] NVIDIA arbitrarily limit their GPU drivers to two streams on consumer cards.
[595.32 → 597.12] Like a 1080 Ti, for crying out loud.
[597.54 → 600.82] That's capable of doing 20 or 30 streams, and they limit it to two.
[600.82 → 605.34] And really, not all codecs and bit rates are supported.
[605.80 → 608.70] So if you want something that's more flexible, you still end up on CPU.
[609.00 → 611.20] So you still need to account for that in your CPU build.
[611.48 → 611.60] Yeah.
[612.26 → 619.70] And so going back a bit to my power bill, I look at these dual Eons, and they idle at around,
[619.80 → 622.44] I mean, there are 15 hard drives in this box as well.
[622.80 → 623.02] Yeah.
[623.52 → 626.36] But they idle, that box idles at around 300 watts.
[626.36 → 631.02] And now some rough math that I use to calculate what that costs me.
[631.88 → 635.64] North Carolina, my power is about 11 cents per kilowatt-hour.
[636.14 → 642.12] And you can approximate that to roughly $1 per watt per year.
[642.76 → 646.62] So that server costs me approximately $300 a year to run.
[647.20 → 650.96] Now, if I was to look at what I could get in DigitalOcean or Amazon for that kind of money,
[651.32 → 652.12] it wouldn't come close.
[652.12 → 652.44] Yeah.
[652.44 → 656.68] Not in horsepower and not in storage.
[657.02 → 660.68] And also bear in mind that you're getting the benefit of raw metal performance,
[660.90 → 663.70] not a virtual machine up on a shared system.
[664.06 → 664.18] Mm-hmm.
[664.68 → 667.68] So I run Proxmox as my base OS, which is based on top of Debian.
[668.28 → 671.92] And then all of my application workloads are within an Ubuntu VM,
[672.12 → 676.10] which I use pass-through on to send a couple of disk controllers through.
[676.72 → 677.78] And that works great.
[677.78 → 680.32] And I don't notice any performance penalty for real on that.
[682.32 → 685.44] But I can't help escape this thing, particularly with this new Ry zen launch.
[685.74 → 688.92] I can't help escape the fact that I could build a system with similar performance
[688.92 → 691.80] that only drew 100 watts from the wall.
[693.02 → 697.02] And I've still got, you know, the new Ry zen 3 Zen 2 stuff.
[697.02 → 701.56] I could have the same performance for less than half the energy draw.
[702.64 → 705.00] Yeah, but there's no way that math works out price-wise.
[705.06 → 708.76] Since you've spent the money on the server, it would take you so long to make that up.
[709.32 → 709.58] Yeah.
[709.70 → 712.78] I mean, a Ry zen build is going to cost me at least, what, $1,000, $1,500?
[713.56 → 715.48] To be honest for you, it's probably going to be closer to $2,000.
[715.76 → 715.94] Yeah.
[715.94 → 716.26] Come on.
[716.34 → 716.88] You know yourself.
[716.88 → 723.22] Yeah, and, you know, there's another thing that this old enterprise gear has that you
[723.22 → 727.54] can't necessarily get cheaply on the AMD side right now, and that's PMI.
[727.82 → 728.12] Mm-hmm.
[728.44 → 734.12] So I could log into my pfSense box from here, bring up the PMI interface, and remotely see
[734.12 → 736.34] what is being output through the VGA port.
[736.58 → 737.20] You know, I'm in Seattle.
[737.28 → 738.76] My server's in Raleigh, North Carolina.
[739.14 → 741.92] And I can just bring up the display as if I was there.
[742.12 → 742.28] Yeah.
[742.92 → 743.76] KVM over IP.
[744.00 → 744.76] It's amazing.
[744.76 → 747.28] That is, especially when you have family members that are depending on it.
[747.54 → 748.96] That is really nice to have that.
[749.12 → 752.38] Well, we use the word depending on inverted commas as well, I think.
[752.90 → 754.72] The whole thing is a big math equation to me.
[755.22 → 757.56] I look at what I expect this box to do.
[757.72 → 761.92] How core to my, how, quote unquote, dependent am I on this?
[761.98 → 764.54] How core to my daily use of my network is it?
[765.06 → 766.82] I.e., is it doing DNS?
[767.02 → 768.22] Is it doing DHCP?
[768.48 → 771.32] Is it doing Samba or NFS, some kind of storage?
[771.32 → 774.44] So then how, how performant does that need to be?
[774.54 → 776.38] And how dependable does it need to be?
[776.56 → 781.18] And then from that, I try to derive how reliable I need the server hardware to be.
[781.18 → 789.34] And then the only other kind of two factors I have to, I have to figure there is how much CPU and disk.
[789.40 → 791.68] Because often the other things will drive the RAM requirements.
[792.06 → 800.62] And I often end up on a mix of X86, Leon hardware with 64 gigs of RAM was kind of like my standard build right now.
[800.76 → 801.94] And then a ton of disk.
[802.24 → 803.46] And it is the same thing.
[803.50 → 804.20] It's drawing around.
[804.40 → 805.64] I don't think it's drawing that much.
[805.72 → 807.20] I don't have, I don't have as many disks as you do.
[807.20 → 810.46] But it does, it does have a big cost.
[810.60 → 815.60] I look at it as a business expense since it is, you know, also file services for our team and whatnot.
[816.06 → 823.30] But it was a hard calculation to make because I did, I did really like when I could go lower power.
[823.44 → 829.26] Because I often went, that also meant less noise, less heat, less cost, less complexity.
[829.26 → 835.10] So I do, I do kind of want to encourage like when possible, don't, don't overbuild if possible.
[835.36 → 837.56] I've kind of gotten away with that so far in the RV.
[837.82 → 843.18] I don't have any, any hard work equipment that requires a fan or anything like that running in the RV.
[843.30 → 844.54] It's all appliance based so far.
[844.70 → 845.82] But I can feel it slipping.
[846.34 → 846.68] It's slipping.
[846.98 → 848.90] You're not tempted to put a pie in the, in the RV then?
[848.94 → 851.60] Oh, I got like an idea for like three different ones right now.
[851.60 → 858.58] The Raspberry Pi fits in a weird place in all of this because it's perfect to run small stuff that doesn't have much IO.
[859.26 → 866.28] But the minute you want to attach more than one SATA type disk to it, you have to have lots of USB converters.
[866.40 → 872.94] And maybe with the 4, we should do some testing maybe that, because they've separated out the, the Ethernet bus from the USB bus.
[873.24 → 873.60] Finally.
[873.60 → 873.88] Yep.
[874.02 → 877.08] The early benchmarking I've done shows it really makes a big difference.
[877.22 → 877.52] I'm sure.
[877.52 → 883.70] So I think the 4 is the first Raspberry Pi that's truly ready to be a home server.
[884.10 → 893.82] And I think so regardless of what hardware you pick and regardless of what OS, even though we, I think we both kind of recommend if you're starting out, people try out Debian or Ubuntu therefore.
[894.00 → 894.60] Well, there are others.
[894.90 → 895.06] Yep.
[895.22 → 896.70] Santos would be another good choice, I think.
[896.80 → 898.78] Well, we haven't mentioned Friends or Unpaid yet.
[899.32 → 902.26] Oh, I feel like we could have a whole conversation on those suckers.
[902.32 → 902.48] Right?
[902.74 → 902.98] Yeah.
[902.98 → 907.70] I mean, if you're just starting out, Unpaid, I would say is possibly the easiest thing around.
[908.04 → 908.16] Yeah.
[908.60 → 909.36] Is that good though?
[909.86 → 914.36] It's, it's a proprietary piece of software, which you have to pay a license for.
[914.90 → 919.34] So it's not completely free and open source like our Debian recommendation would be.
[919.34 → 929.60] And that's something that I struggle with quite often when speaking to people in Discord or on Reddit is, it's trying to gauge you as a person.
[929.74 → 934.04] Where do, what are you trying to get out of this purchase or this build?
[934.40 → 939.84] Are you trying to learn skills that will make you more marketable for a job?
[939.84 → 943.76] Or are you just trying to solve a problem, which is how do I stream media around my house?
[944.38 → 947.60] You could also be somebody who just likes to know how the things work.
[947.74 → 949.42] And so you want to build it yourself, put it together.
[949.74 → 951.34] You want to know all the parts of the recipe.
[952.06 → 953.58] You know, what is the right box for you?
[953.62 → 954.60] Is it a Synology maybe?
[955.56 → 959.68] Is, is learning Linux the right thing for you to do whatsoever?
[960.50 → 962.74] There are, there are so many options in this space.
[962.92 → 964.76] It can be bewildering as a new guy.
[964.76 → 972.12] It's like, like we need like some sort of show that has time to discuss and explore all these different options and help sort all of this out.
[972.24 → 973.28] Something to help you.
[973.78 → 974.48] Is that what this is?
[974.62 → 975.14] Yeah, maybe.
[975.36 → 976.40] Oh, okay.
[976.88 → 978.86] Maybe something to help you navigate those complexities.
[979.10 → 979.72] What a great idea.
[980.26 → 987.12] I think my other, my other like checklist, if you're considering self-hosting is you need to be willing to take on some personal responsibility for security.
[987.66 → 988.02] Absolutely.
[988.02 → 992.48] You know, be willing to use SSH key authentication whenever possible.
[992.74 → 994.60] Don't use passwords for any kind of login.
[994.76 → 1003.08] Be willing to explore isolating applications and services, either through VMs, through containers, whatever works for you.
[1003.60 → 1007.50] Also, where possible, restrict your file systems to read only.
[1008.26 → 1013.50] There's no reason, if you don't need to have write access or if you can easily enable write access to make a change, consider that.
[1014.00 → 1020.06] And also, stay tuned for future discussions on setting up reverse proxies because that's going to be a key part of this too.
[1020.12 → 1023.02] You've got to be willing to deep dive a little bit into a reverse proxy.
[1023.02 → 1035.14] And if you're willing to do those kinds of self-responsibility items that aren't related to the CPU or the hardware or the operating system, if you're willing to do those things in addition, I think you're probably a good candidate to self-host.
[1035.14 → 1047.36] But the other thing is, right, if you were to just buy an off-the-shelf Synology or a QNAP or any of the other kind of NAS in a box, like Drop maybe, you're still going to have to figure a lot of this stuff out.
[1047.46 → 1056.00] The minute you, for me, what woke my mind up to all this was five or six years ago, I bought a Drop, returned it because it was expensive.
[1056.00 → 1058.02] I've owned a couple of them.
[1058.24 → 1059.14] And then I bought a Synology.
[1059.56 → 1059.78] Yeah.
[1060.12 → 1060.26] Yeah.
[1060.68 → 1065.54] And then I sort of thought to myself, well, I've got this thing sat there with blink lights that's on.
[1066.02 → 1066.88] What else can I do with it?
[1066.94 → 1067.16] Right.
[1067.16 → 1074.42] And that single thought sparked my entire journey rabbit hole into, I guess, being sat here with you right now.
[1074.94 → 1075.20] You know?
[1076.08 → 1078.58] Was that before you worked for Red Hat or was that?
[1078.74 → 1079.38] Oh, a long time.
[1079.44 → 1079.60] Yeah.
[1079.94 → 1081.88] This was, I was still working at the Apple Store.
[1082.12 → 1082.56] Oh, okay.
[1082.82 → 1085.52] I was a genius on the genius bar at the Apple Store.
[1085.68 → 1086.30] You have that moment.
[1086.38 → 1088.14] You say to yourself, I want to solve this problem.
[1088.76 → 1089.26] What would it take?
[1089.26 → 1094.72] For me, it was a 1.5 terabyte Seagate hard drive, which are notorious now.
[1094.80 → 1095.64] They have a reputation.
[1096.44 → 1097.52] I woke up one morning.
[1097.58 → 1098.58] I'd powered my computer off.
[1098.70 → 1099.56] I was still running Windows.
[1100.26 → 1100.90] I'm sorry to say.
[1101.22 → 1103.06] No, Windows happens, man.
[1103.94 → 1104.74] We're okay with that.
[1104.78 → 1105.88] I was still running Windows.
[1106.02 → 1112.02] And I had a bunch of movies and TV shows on this 1.5 terabyte hard drive, which I'd ripped from DVDs I had.
[1112.18 → 1112.60] Oh, yeah.
[1112.74 → 1114.32] Oh, that's a labour of love.
[1114.54 → 1114.76] Yeah.
[1114.86 → 1116.46] And they were beautifully categorized.
[1116.54 → 1116.78] Of course.
[1116.78 → 1117.52] And catalogued.
[1117.60 → 1119.92] You had a nice naming scheme for each file and everything.
[1120.40 → 1122.78] And I woke up one morning, pushed a power button on my desktop.
[1123.82 → 1123.98] Sure.
[1123.98 → 1126.10] And that drive didn't show up.
[1126.16 → 1127.08] And I'm like, what the F?
[1127.64 → 1128.70] Where has this gone?
[1128.80 → 1129.78] It was fine last night.
[1129.92 → 1131.12] Double-click on old my computer.
[1131.28 → 1131.96] No D drive.
[1132.46 → 1133.38] And then you go in disk management.
[1133.54 → 1133.80] Nothing.
[1134.04 → 1134.98] And then you go into the BIOS.
[1135.32 → 1135.64] Nothing.
[1135.92 → 1136.24] Uh-oh.
[1136.24 → 1138.48] And when it doesn't show up in the BIOS, you're like, oh, crap.
[1140.00 → 1145.94] So I had a USB external hard drive, 3.5 hard drive.
[1146.50 → 1147.74] It can close your kind of thing.
[1147.86 → 1148.48] Mount thing.
[1148.56 → 1149.26] It was like a hot swap.
[1149.82 → 1151.16] I had one of those toasters.
[1151.60 → 1151.78] Yeah.
[1151.78 → 1152.64] It's like a USB toaster.
[1152.80 → 1154.82] You put this full-size drive in there.
[1155.12 → 1156.04] I love those things.
[1156.18 → 1156.44] Yeah.
[1156.44 → 1159.60] So they fulfill a use case that I wish I had.
[1159.88 → 1160.18] Right.
[1160.28 → 1160.44] Exactly.
[1160.44 → 1161.06] I just don't have it.
[1161.22 → 1161.68] Never used.
[1161.90 → 1165.64] I bought one at home, and I bought one here at the studio, and I thought, I'll synchronize
[1165.64 → 1166.12] my data that way.
[1166.12 → 1167.38] I use it all the time, but no.
[1167.54 → 1167.90] Nothing.
[1168.54 → 1175.20] So anyway, this 1.5 terabyte Seagate drive just had a hugely horrific failure rate.
[1175.84 → 1181.20] We're talking double-digit percentages, where the spindle one morning just decided, I'm
[1181.20 → 1181.82] not going to unlock.
[1182.06 → 1186.40] Back when IBM made this, I had a series of, we called them Death Stars.
[1186.62 → 1187.56] Same thing happened to me.
[1187.62 → 1189.82] In an array, like, several of them started popping.
[1190.04 → 1192.58] That name has stuck with the Desk Star forever.
[1192.84 → 1193.08] Mm-hmm.
[1193.58 → 1195.84] So I had a similar thing afflict me one time.
[1196.22 → 1199.04] And then you start thinking, well, what if that had been the other drive that had all
[1199.04 → 1199.78] my photos on it?
[1200.22 → 1200.42] Yeah.
[1200.98 → 1203.68] And then you think, well, okay, I need some redundancy here.
[1203.68 → 1208.54] Because one, the phrase in the backup industry is once is nonce.
[1209.34 → 1209.82] Right.
[1209.94 → 1211.06] One is none, actually.
[1211.22 → 1213.00] One copy is not a backup.
[1213.42 → 1214.04] One is none.
[1214.48 → 1215.66] Two is something.
[1216.20 → 1217.16] And then three is...
[1217.16 → 1217.74] A proper backup.
[1217.90 → 1218.74] Yeah, that's what you want.
[1219.06 → 1225.56] So nowadays, I have, for all of my photos, for example, I have a full copy in Google of
[1225.56 → 1227.00] everything, like Google Drive.
[1228.92 → 1233.52] I have a few drives at my dad's house, which I send everything remotely to him, encrypted
[1233.52 → 1237.20] using Duplicate across the internet to his house.
[1237.22 → 1237.76] Oh, how does that work?
[1239.58 → 1243.04] It has this wonderful way of doing, like, snapshots.
[1243.14 → 1245.10] So it does, like, incremental backups.
[1245.36 → 1246.76] It's a bit like ZFS Send, I believe.
[1246.86 → 1248.24] It only sends what's changed.
[1248.38 → 1252.56] But it works at the file level instead of ZFS's block level stuff.
[1253.10 → 1253.98] So in some ways, it's better.
[1254.04 → 1254.74] In some ways, it's worse.
[1255.24 → 1258.48] And do you go to the trouble of encrypting the data that you send up to Google Drive?
[1259.26 → 1259.92] Google, yes.
[1260.10 → 1260.26] Yeah.
[1260.54 → 1261.14] My dad's, no.
[1261.40 → 1261.76] Yeah, right.
[1261.88 → 1262.48] Sure, sure.
[1262.74 → 1267.14] Because in the event of a failure where I need to get that data, the risk of having
[1267.14 → 1271.52] to remember an encryption password on my dad's house might be the one thing that costs me
[1271.52 → 1271.90] that data.
[1272.04 → 1274.54] And it feels like if it's going to be safe somewhere, it's probably your dad's house.
[1275.92 → 1280.50] Does the encryption you use to go to Google Drive, does it support incremental file changes
[1280.50 → 1282.14] or is it whole files every time?
[1282.40 → 1283.96] I think it must be whole files every time.
[1283.96 → 1287.62] Yeah, that's something I think we could explore in the future, too, is how to leverage the cloud
[1287.62 → 1291.30] for your self-hosted solution that is still secure for backups.
[1291.58 → 1291.78] Yeah.
[1292.02 → 1292.56] You know, private.
[1292.86 → 1293.72] I think that'd be a big thing.
[1293.80 → 1296.16] There's a whole rabbit hole we could go into on just backups alone.
[1296.30 → 1296.72] Oh, man.
[1297.04 → 1297.32] Totally.
[1297.42 → 1298.96] We could have a total full conversation.
[1299.58 → 1300.54] I'd love suggestions, too.
[1300.58 → 1303.96] We have a new Twitter account, at SelfHostedShow, which you can tweet at.
[1304.04 → 1305.50] Alex and I will both be monitoring that.
[1305.84 → 1308.26] And if you have something you want to get in the show, that's probably the best way.
[1308.26 → 1314.50] Or hit us on Twitter or in the Telegram for Jupyter Broadcasting, hashtag Ask SSH.
[1314.62 → 1315.78] What does the S stand for?
[1315.86 → 1316.36] The extra S.
[1316.62 → 1317.62] The super self-hosted show.
[1317.78 → 1319.10] I think we should make the audience guess.
[1319.40 → 1323.88] Oh, they should give us suggestions by doing hashtag ask, because we just wanted to use SSH.
[1323.94 → 1326.16] And the winner will get a t-shirt with Ask SSH on it.
[1326.22 → 1326.98] Oh, great.
[1327.36 → 1327.56] Yeah?
[1328.20 → 1328.64] Sure.
[1329.08 → 1330.16] Let's just do that.
[1330.58 → 1334.78] And then if you have something longer form that you want to get over to us, self-hosted. Show
[1334.78 → 1340.34] slash contact, self-hosted. Show is going to be the landing page for this whole show.
[1340.44 → 1346.00] Anything like links or contact pages or our RSS feeds, subscribe links, all of that is
[1346.00 → 1347.42] at self-hosted.show.
[1347.98 → 1352.06] And so we're going to be focusing mostly on server stuff, like you've just heard.
[1352.24 → 1352.38] Yeah.
[1352.46 → 1355.16] Chris and I, we're building out infrastructure.
[1355.40 → 1356.14] We're infrastructure guys.
[1356.32 → 1356.46] Yeah.
[1356.50 → 1359.24] Like right now, I'm working on like a whole security camera system that's going to be
[1359.24 → 1359.76] tied into this.
[1359.78 → 1360.18] Right.
[1360.32 → 1360.60] Yes.
[1360.60 → 1360.98] Got to talk about that soon.
[1360.98 → 1362.00] I can't wait to hear about that.
[1362.00 → 1362.32] Yeah.
[1362.58 → 1364.74] I really, really, really like it so far.
[1364.78 → 1367.22] But we also have another show on the network called Choose Linux.
[1367.54 → 1367.72] Yep.
[1368.00 → 1369.60] Which complements this one really well.
[1369.70 → 1370.64] Yeah, on the desktop side.
[1370.76 → 1370.94] Yes.
[1370.96 → 1373.22] And they're trying out desktop applications and distributions.
[1373.66 → 1375.30] It's a great introduction to that.
[1375.72 → 1379.90] It's just a fun journey of discovering new things in open source and Linux.
[1380.26 → 1384.12] Just like we'll be doing on the server side, they do it on the desktop side.
[1384.18 → 1385.58] So it's sort of a companion show in a way.
[1385.86 → 1386.82] I like how that's worked out.
[1387.28 → 1389.58] It's almost like we planned it that way.
[1390.08 → 1390.48] Almost?
[1390.48 → 1390.76] Most?
[1390.98 → 1394.28] Hey, before we run, I've been watching something this week I want to tell you about.
[1394.36 → 1395.62] I think you might really like this channel.
[1395.72 → 1395.86] Okay.
[1396.12 → 1400.68] I came across it when I was doing research on security cameras.
[1401.22 → 1403.42] And have you heard of the Dufy Cam Ease?
[1403.94 → 1404.52] No, I have not.
[1404.82 → 1407.30] They're like a competitor to the Arlo camera system.
[1408.30 → 1409.96] And Dufy is a division of Anchor.
[1410.12 → 1411.22] People that make all the...
[1411.22 → 1412.62] My Robotic is by Dufy.
[1412.62 → 1412.86] Yeah.
[1413.16 → 1419.26] And so they've made some really nice cameras that are battery, wireless, the local recording,
[1419.48 → 1422.22] which is encrypted, and you still get remote access to it.
[1422.54 → 1424.92] And the channel is just great, where I watched the review.
[1425.10 → 1426.54] It's Undecided with Matt Farrell.
[1426.74 → 1429.54] And he has just a great, clean take on this stuff.
[1429.62 → 1430.38] Nice, level-headed.
[1430.96 → 1431.70] It's a good YouTube channel.
[1431.76 → 1433.86] So I subscribed, and I became a patron today.
[1433.92 → 1435.12] I really was that impressed.
[1435.24 → 1436.24] Look at those production values.
[1436.44 → 1437.44] This guy has good lighting.
[1437.54 → 1438.58] That's what I'm talking about.
[1438.58 → 1441.74] You can tell just in the first thumbnail how good a video is going to be.
[1441.74 → 1443.48] And he's really, he's well-spoken.
[1443.60 → 1446.28] He posts the script up on his website.
[1446.48 → 1447.80] He does a perfect evaluation.
[1448.48 → 1449.66] And I just want...
[1449.66 → 1451.84] So he's plugged these cameras into a Synology box, has he?
[1452.48 → 1452.84] I think.
[1452.92 → 1454.32] It's one of the many systems he has, yeah.
[1454.40 → 1454.82] That's great.
[1455.72 → 1456.28] Check it out.
[1456.36 → 1457.34] Undecided with Matt Farrell.
[1457.40 → 1461.24] We'll have a link in the show notes at self-hosted. Show slash one.
