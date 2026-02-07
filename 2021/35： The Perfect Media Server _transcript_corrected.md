[0.08 → 2.50] Today's episode is a really exciting one for me.
[3.06 → 5.70] It's the culmination of five years' work.
[6.00 → 9.66] The perfect media server is now, well, I'll save it for the show.
[10.06 → 11.68] We also respond to a ton of your feedback.
[11.96 → 13.50] This is Self-Hosted 35.
[15.00 → 17.50] Well, Alex, I'll admit it right here on the show,
[17.66 → 20.66] I set up yet another Synching server this weekend.
[21.00 → 23.54] You thought you'd leave 2020 behind in style, hey?
[24.10 → 25.86] I wanted more speed, Alex.
[25.92 → 29.58] Actually, it really came down to me doing the math and realizing,
[29.58 → 33.92] hey, you know, when I switch networks, it kind of slows the syncing down.
[34.28 → 37.02] But if I can pull from multiple Sync servers,
[37.62 → 40.64] it kind of makes up for it and goes even faster in ideal situations.
[40.80 → 44.58] So I thought, why not set up a Synching server on Linde
[44.58 → 47.80] and just sync a small select stuff that I really want to move fast?
[48.56 → 51.10] And it legit works. It's really nice.
[51.76 → 54.52] It's like doubles the amount of files that can be transferred at once, too,
[55.02 → 56.88] from what I can tell in my brief testing.
[56.88 → 59.64] I'll be honest, I haven't continued with Synching
[59.64 → 61.62] after we talked about it a couple of episodes ago.
[61.96 → 62.80] It just doesn't work for me.
[62.88 → 64.58] It just doesn't do it, I'm afraid.
[64.84 → 66.16] But I'm glad it's working for you.
[66.54 → 67.86] You're a hater. I understand.
[68.30 → 69.46] I understand. I understand.
[69.64 → 71.16] I love it.
[71.52 → 80.10] I think 2020 is the year that I stepped into a long-term relationship with Synching.
[80.10 → 84.18] And it's not like I'm working on files super quick
[84.18 → 85.54] and I want to move it between machines
[85.54 → 88.42] and I want to edit a file upstairs and then walk down into the studio
[88.42 → 90.06] and have that file on my desktop.
[90.68 → 94.26] It may be able to serve that function, but I've learned not to expect that.
[94.58 → 97.28] The one caveat I do have with Synching
[97.28 → 99.94] is you've got to let it go at its own pace.
[100.22 → 101.46] You've got to let it go at its own pace.
[101.96 → 103.56] And that's why I love online learning, too.
[103.62 → 106.04] And this episode is brought to you by the all-new A Cloud Guru,
[106.04 → 109.82] the leader in learning for cloud Linux and other modern tech skills.
[110.16 → 112.62] Hundreds of courses, thousands of hands-on labs.
[112.72 → 116.48] Get certified, get hired, get learning at acloudguru.com.
[117.02 → 119.14] Well, Alex, I think we should start the show today by,
[119.38 → 121.34] well, maybe we started by talking about Synching,
[121.44 → 125.76] but now we should start talking about a project in various forms, at least,
[125.82 → 127.96] you've been working on for about five years.
[128.16 → 132.92] And I think, if I'm not wrong, it's like about to reach its ultimate form.
[133.32 → 134.06] Perhaps, yeah.
[134.06 → 136.58] Well, I mean, as we record, it's still 2020,
[136.90 → 139.58] but I think this is going to come out on New Year's morning.
[139.76 → 141.34] So Happy New Year, everybody.
[141.78 → 142.74] Welcome to 2021.
[143.20 → 146.12] Hopefully, it's more prosperous than the last one was.
[146.62 → 149.02] We're talking about my perfect media server project.
[149.26 → 152.64] So this was something that, when I was involved with linuxserver.io,
[152.80 → 159.12] that actually helped me kind of form the direction for that site
[159.12 → 160.60] and the blog and stuff like that.
[160.60 → 169.48] So on the 2nd of February 2016, I wrote a post about what I called the perfect media server,
[169.66 → 171.56] for want of a better name, and it's kind of stuck now.
[171.96 → 174.70] It's bold, but now you've kind of become the perfect media server guy.
[174.94 → 176.08] Yeah, I guess so.
[176.92 → 179.06] You know, I've toyed with changing the name a few times,
[179.18 → 181.18] but enough people have seen it.
[181.44 → 182.64] And, you know, I've looked at the analytics,
[182.64 → 185.88] and a lot of people have read that post over the years.
[187.16 → 189.16] In fact, funnily enough, when I moved to Raleigh,
[189.22 → 191.54] one of my closest friends now, who's also called Alex,
[192.16 → 194.92] he joined Linux server originally.
[195.14 → 196.52] He's now one of the Linux server devs.
[196.74 → 200.36] He joined that website because he read my perfect media server post.
[200.90 → 203.62] And so when I came to town, like, he met up with me,
[203.66 → 205.90] and we had a few beers and stuff like that.
[205.90 → 209.22] And he was so excited to tell me that he'd built one as well around,
[209.30 → 213.68] you know, Docker and Snap Raid and Merger FS and all this kind of stuff.
[213.82 → 217.72] So it's been a really cool thing to share with the world.
[218.26 → 221.88] Well, you also got a great domain name for it, perfectmediaserver.com.
[221.98 → 222.78] Is that new?
[223.12 → 223.96] Brand new, yes.
[224.30 → 228.98] I, well, when I say brand new, I mean, I bought it in June.
[228.98 → 238.52] I've been promising a 2020 version of this article for rather longer than I would like.
[238.82 → 243.58] So I released one in 2016, another one in 17, and another one in 19.
[244.06 → 246.66] And, you know, when you start thinking about what can I write about
[246.66 → 249.70] with these perfect media servers,
[249.96 → 253.72] when everything is just so reliable and just works,
[254.78 → 256.46] there comes a limit when you think,
[256.46 → 260.10] well, I can't really rehash the same thing again and again.
[261.38 → 264.78] And so this time I was looking at the three posts.
[265.08 → 267.74] And since I'm no longer involved with Linux server,
[267.92 → 271.06] I don't have access to edit those blog posts easily anymore.
[271.22 → 273.48] I mean, I can ask the team to fix things and stuff,
[273.64 → 276.32] but invariably information goes out of date.
[276.66 → 280.18] And I am a huge advocate of open source
[280.18 → 284.56] and community contributions and wikis and all that kind of stuff.
[284.56 → 288.18] And so I just thought that this would make much more sense
[288.18 → 293.38] as a kind of wiki type website with first class search categories,
[293.72 → 296.22] walking people through how to do things,
[296.28 → 298.10] you know, in a step-by-step kind of fashion,
[298.38 → 302.30] and then leave the blog posts as kind of like an annual opinion piece
[302.30 → 305.50] alongside this more kind of dry,
[305.68 → 309.80] technical wiki style website at perfectmediaserver.com.
[309.80 → 311.18] Okay, that makes a lot of sense.
[311.74 → 315.86] And I think probably the real value for people to understand is
[315.86 → 318.64] you're telling people there are a lot of options out there,
[318.74 → 320.82] but maybe this is a great stack to use.
[320.88 → 321.78] You can use this stack.
[321.88 → 322.60] I've tested this.
[322.68 → 329.54] I've refined it over the years to do really a beyond just okay media setup,
[329.58 → 330.74] but a great home media setup.
[330.96 → 333.76] And instead of saying, oh, there's so many use cases
[333.76 → 336.54] or the answer, which is frequently it depends,
[336.98 → 338.60] you make some opinionated decisions
[338.60 → 341.12] and kind of point people in a direction
[341.12 → 342.34] and then lay out how to do it.
[342.66 → 345.88] And I think that's maybe, for me, the real value of the site.
[345.88 → 348.98] I think as well, a lot of people come to Linux,
[349.04 → 350.34] and I've said this before on the show,
[350.94 → 353.70] a lot of people come to Linux not through the desktop,
[354.14 → 356.34] but through Plex,
[356.62 → 358.90] through running headless apps on a Synology
[358.90 → 360.88] or a Raspberry Pi or something like that.
[360.88 → 364.54] And once you start having a box in your house
[364.54 → 367.46] that does everything 24 hours a day,
[367.62 → 369.16] that is on 24 hours a day,
[369.58 → 370.82] you think, what else could I do with it?
[371.04 → 374.04] And that single spark is a huge rabbit hole.
[374.20 → 377.12] And I think one of my primary goals with the site
[377.12 → 379.38] is to equip those newer people
[379.38 → 383.74] with the skills that they need to install Ubuntu,
[384.82 → 385.94] set up Mergers,
[386.48 → 388.16] figure out what an FS tab is,
[388.16 → 391.02] and not be intimidated by, you know,
[391.22 → 396.10] wading through lots of different disparate documentation
[396.10 → 397.94] across different places on the internet.
[398.04 → 399.22] It's just all in one place.
[399.88 → 402.78] And if you want to have multiple hard drives
[402.78 → 405.32] in a single box that are of mismatched sizes
[405.32 → 406.80] with different file systems,
[407.24 → 408.58] well, here's a solution for you.
[409.10 → 410.70] You've already got data on these drives.
[410.78 → 411.88] You don't want to do RAID.
[412.22 → 413.04] Great, cool.
[413.14 → 414.66] Come along and join the party.
[414.66 → 416.62] Yeah, and honestly,
[416.92 → 418.98] it's a lot of the stack that we talk about frequently.
[419.34 → 420.58] You talk about Docker,
[420.76 → 422.34] kind of some of the background in there,
[422.40 → 423.02] how to get it going.
[423.34 → 425.12] And you work your way up through
[425.12 → 426.76] how to manage multiple disks
[426.76 → 427.88] of different sizes, like you say.
[427.96 → 428.54] But then also,
[429.08 → 430.32] if you want to go ZFS,
[430.70 → 433.78] and here's also a Proxmox layer you should consider,
[434.68 → 436.44] any one of those could be broken out
[436.44 → 438.42] and really have nothing to do
[438.42 → 440.30] with building a media server.
[440.64 → 442.28] So it's kind of valuable in that way too, I suppose.
[442.28 → 444.00] So I mentioned that just for the audience
[444.00 → 446.02] who's not interested in building a media server,
[446.16 → 449.04] but does want to learn more about Docker
[449.04 → 452.36] or Mergers or Snap Rate or ZFS or Proxmox
[452.36 → 454.88] or hardware, any of that kind of stack,
[454.96 → 456.24] stuff we talk about on this show
[456.24 → 458.16] and you want to read something from Alex on it,
[458.68 → 459.52] you can find it there too.
[459.66 → 462.42] And I could totally have seen a guy like me,
[463.24 → 465.10] maybe if I was building my media server setup
[465.10 → 465.90] for the first time,
[466.22 → 467.18] I'd be thinking, okay,
[467.24 → 468.52] I know I want to use containers,
[468.70 → 470.00] but I don't quite know how
[470.00 → 472.60] and in what way to use them to do this right.
[473.24 → 474.52] I know about Mergers,
[474.80 → 476.42] but I don't know how to deploy it.
[476.52 → 478.62] And so having you write something,
[479.52 → 481.04] having used this stuff in production
[481.04 → 482.16] for five years now,
[482.70 → 484.16] there's value to that.
[484.46 → 486.08] So you should be the perfect media server guy.
[486.56 → 487.88] I think that's, I said good on you.
[488.20 → 490.02] You be the perfect media server guy
[490.02 → 492.84] because I endorse this media server build here.
[492.94 → 494.80] You are, Chris, and you support this message.
[495.04 → 496.08] I wonder what the cost is.
[496.12 → 496.92] Have you thought about that?
[496.92 → 499.44] Have you thought about like what the cost would be
[499.44 → 502.38] for a minimal build of something from this guide?
[502.64 → 503.58] Well, in terms of hardware?
[504.60 → 505.58] Yeah, in terms of hardware.
[506.00 → 507.66] I think Quick Sync now for me
[507.66 → 509.50] is a minimum price of entry
[509.50 → 511.54] after everything we talked about in the last episode.
[512.24 → 515.04] So a hundred bucks for a CPU.
[515.76 → 517.32] You can probably find a used motherboard
[517.32 → 518.82] that will do the trick for a hundred dollars.
[519.02 → 520.74] Again, RAM is about a hundred.
[521.44 → 522.66] And then hard drives.
[522.74 → 524.00] For an eight terabyte hard drive now,
[524.00 → 525.30] you can go to Best Buy and pick one up
[525.30 → 528.14] for around 130, 140.
[528.58 → 529.86] So I don't know.
[529.92 → 531.86] Let's say 140.
[532.88 → 533.42] What's that?
[533.50 → 537.14] It's like $1,100 or so for hard drives.
[538.06 → 538.86] I don't know, $1,500.
[539.60 → 541.44] I think all in would get you
[541.44 → 543.58] five, eight terabyte drives
[543.58 → 545.00] of 40 terabytes of storage
[545.00 → 548.28] for $1,500 all in.
[548.28 → 550.92] And you own it forever.
[551.68 → 552.54] It's, you know, you're not,
[553.40 → 555.10] I mean, Synology make a great product.
[555.20 → 557.68] So do QNAP and Unpaid's also great,
[557.78 → 558.82] but it's not open source.
[559.68 → 562.50] Free NAS requires learning ZFS,
[563.16 → 565.72] which I know I talk about in Perfect Media Server,
[565.82 → 569.94] but it's kind of orthogonal to the main content.
[570.06 → 571.82] It's not required learning.
[571.98 → 574.44] Whereas with a True NAS or a Free NAS product,
[574.66 → 575.24] it is.
[575.24 → 578.50] It's just the most flexible thing for most people.
[578.64 → 581.32] And I think when you start looking at
[581.32 → 582.86] putting together one of these servers,
[583.00 → 585.80] $1,500 isn't a small upfront investment.
[586.00 → 586.50] And you think, right,
[586.56 → 587.84] well, where can I cut some costs?
[587.94 → 590.64] And the obvious answer is the hard drives.
[591.06 → 592.60] You know, rather than buying five,
[592.70 → 594.58] let's only buy a couple, right?
[594.60 → 596.90] And then I'll add the other three
[596.90 → 598.12] over the next year or two.
[598.90 → 600.20] Mergers lets me do that.
[600.28 → 603.40] It lets me add drives as my collection grows
[603.40 → 607.60] without having to re-silver a ZFS array
[607.60 → 611.40] or rebuild a RAID setup or anything like that.
[611.44 → 613.36] It just grows as I do,
[613.42 → 614.66] and it changes and matures.
[615.00 → 616.66] And because it's just Linux,
[617.00 → 620.16] it's open, and I can go and tinker
[620.16 → 621.52] as deep as I want under the hood.
[621.90 → 623.40] Or again, because it's Linux,
[623.56 → 624.96] it will just work.
[625.04 → 625.76] It's just reliable.
[626.02 → 628.16] It's battle-tested and hardened everywhere.
[628.16 → 632.58] So I really do think that if you're willing
[632.58 → 636.34] to put the time in and learn a little bit of this stuff
[636.34 → 638.92] with the information that's provided here for you,
[639.12 → 640.10] for free, I might add,
[640.14 → 641.76] I don't make a penny off of this stuff.
[642.20 → 643.62] Anyway, I never have.
[643.68 → 644.90] I just wanted to give this information
[644.90 → 645.90] back to the community.
[646.76 → 648.72] I don't think there's a better solution, really,
[648.80 → 650.12] if you're willing to put the effort in.
[650.92 → 652.44] And I'll just give one more mention,
[652.76 → 654.14] because as you were talking there,
[654.14 → 656.30] I was just also reviewing your Quick Sync
[656.30 → 657.68] and Proxmox page.
[658.18 → 659.98] And damn, you put some work into this.
[660.46 → 662.38] But I also, I think it's pretty clever
[662.38 → 665.18] that you embedded the relevant JB content
[665.18 → 667.42] where we've talked about a lot of this stuff in depth
[667.42 → 668.96] when it still holds up.
[669.04 → 671.76] So not only do you get a lot of the written stuff
[671.76 → 672.72] and the visual examples,
[672.88 → 675.26] but you've got a video from Wendell in here too.
[675.44 → 678.14] And so you add the supplemental media content.
[678.94 → 682.48] I could see us linking this to a lot of people
[682.48 → 684.16] that write into the show and ask questions
[684.16 → 684.96] about this stuff.
[685.78 → 687.58] If I were going to contribute one area,
[687.68 → 688.68] I just thought to troll you,
[688.74 → 690.40] I'd probably contribute using Butters.
[690.96 → 693.96] Because literally everything you just said
[693.96 → 696.44] about Mergers is why I use Butters.
[698.14 → 699.50] Seriously, like word for word.
[699.76 → 702.62] So on the ZFS page,
[702.76 → 705.28] there's a whole section about what about Butters.
[706.72 → 708.20] Okay, good.
[708.24 → 709.24] You've addressed it, I can see.
[709.76 → 711.12] Well, a little bit.
[711.12 → 714.14] And my conclusion was that using Butters
[714.14 → 717.06] would probably be easier than ZFS
[717.06 → 720.08] simply because it's shipped as part of the Linux kernel.
[720.34 → 724.02] But I've invested in ZFS mentally,
[724.20 → 727.32] but also I've synced six,
[727.46 → 730.82] seven terabytes worth of data across the ocean to the UK.
[731.36 → 733.14] And I don't want to have to spend another
[733.14 → 736.58] six or seven weeks doing that again if I switch.
[736.92 → 738.80] Well, ironically, it's more about
[738.80 → 740.48] it's more about how you use Mergers.
[741.00 → 742.92] However, I think, you know, both are gray.
[743.02 → 744.72] And if Mergers is working for you,
[745.52 → 747.16] I'm not, I will really not, I'm just more teasing.
[747.64 → 749.22] But it did strike me
[749.22 → 752.08] that being able to join mismatched disks
[752.08 → 753.66] and add them as it grows
[753.66 → 755.06] and be able to remove them easily
[755.06 → 757.74] is why I switched to using Butters
[757.74 → 759.26] on my Raspberry Pi media servers.
[759.26 → 760.36] Because I needed something
[760.36 → 762.54] that essentially was no cost.
[762.54 → 764.74] Since Butters is built into the kernel
[764.74 → 767.18] and it also doesn't have a high,
[767.28 → 768.86] it's a very efficient file system.
[768.94 → 770.10] There's not a big performance penalty.
[770.24 → 771.24] I don't need a lot of RAM.
[771.94 → 773.04] It meant that I didn't have to install
[773.04 → 775.28] any additional software at all.
[775.62 → 778.50] And actually no additional config files or anything.
[778.74 → 779.40] There's no config.
[779.50 → 781.86] It's just, it's all just with volume management
[781.86 → 782.74] on the command line.
[782.82 → 783.72] And it's very simple.
[783.84 → 785.92] It's like Butters add volume
[785.92 → 786.86] and you give it the path
[786.86 → 788.16] and you tell it what volume to add to
[788.16 → 789.02] and boom, you're done.
[789.22 → 789.76] And then remove.
[789.76 → 790.90] And as long as you have enough space,
[790.98 → 791.80] it sinks everything off
[791.80 → 792.56] and you can remove it.
[792.76 → 794.68] And I actually have not tested that.
[794.80 → 796.14] I could imagine it being tricky.
[796.66 → 797.66] But I think, you know,
[797.76 → 799.60] it's, there are different ways
[799.60 → 800.56] to solve all of these.
[800.72 → 802.36] And what you've done here with this
[802.36 → 803.66] is said, well, these are ways
[803.66 → 807.36] that not only are very sensible solutions,
[807.36 → 808.32] but ones that I've tested.
[808.74 → 810.04] And that's the value again.
[810.12 → 811.24] Like, yeah, I could add something
[811.24 → 811.84] about Butters,
[812.18 → 815.12] but there's limited value in it.
[815.22 → 816.44] You know, it's my experience.
[816.98 → 817.80] And this is something
[817.80 → 819.16] that you've worked at for a long time.
[819.16 → 820.70] So I think it's, yeah,
[820.88 → 822.20] I think Murders is a great solution
[822.20 → 823.00] for that kind of stuff.
[823.12 → 824.68] And, you know, things like ZFS
[824.68 → 825.44] and Snap Raid,
[825.54 → 827.12] depending on what your needs are,
[827.16 → 828.84] also can be appropriate solutions.
[829.44 → 830.30] So I've built this site
[830.30 → 831.16] around MK Docs,
[831.74 → 834.02] which happens to be the same project
[834.02 → 835.02] that we're using
[835.02 → 836.14] for the self-hosted wiki,
[836.26 → 837.56] which I've also put some work
[837.56 → 838.36] into this week
[838.36 → 840.06] over the Christmas break.
[840.48 → 841.66] So please go ahead
[841.66 → 843.34] and contribute to the self-hosted wiki
[843.34 → 845.14] at wiki.self-hosted.show
[845.14 → 846.92] because we're crying out
[846.92 → 847.94] for content over there.
[847.94 → 850.14] But MK Docs,
[850.20 → 851.04] I'll tell you what, Chris,
[851.16 → 854.70] has become a hell of a wiki software,
[855.02 → 855.32] you know?
[855.64 → 856.16] So I don't know
[856.16 → 857.02] when you're browsing this,
[857.08 → 858.16] but I don't know if you noticed
[858.16 → 859.30] it has a keyboard shortcut.
[859.58 → 860.38] And they don't tell you this,
[860.44 → 860.62] obviously,
[860.72 → 862.00] but it's the same as Vim.
[862.40 → 864.80] So you can press the forward slash key,
[865.00 → 866.38] which brings up search,
[866.52 → 867.50] and then you can search
[867.50 → 869.00] for any string in any page.
[869.18 → 870.06] And it will just,
[870.30 → 870.98] in real time,
[871.06 → 872.12] and then use the arrow keys.
[872.28 → 873.08] Oh, yes.
[873.08 → 874.58] And it will just take you straight
[874.58 → 876.10] to the section of that page.
[876.22 → 877.36] Just that feature alone
[877.36 → 878.64] had me sold.
[878.88 → 879.02] Huh.
[879.64 → 880.16] That's great.
[880.22 → 881.02] But they've added dozens
[881.02 → 881.88] of other features,
[882.30 → 882.52] you know,
[882.60 → 884.04] like they've got little tool tips,
[884.50 → 885.62] little info boxes,
[885.62 → 887.42] and stuff that breaks up the content.
[888.06 → 889.76] The code formatting,
[890.02 → 890.44] highlighting,
[890.84 → 892.04] is just brilliant.
[892.82 → 894.22] It's fully customizable.
[894.22 → 896.00] So, you know,
[896.26 → 898.30] it was using the COBOL wiki
[898.30 → 899.82] for the Helios 64 review,
[899.98 → 900.86] which finally got me
[900.86 → 903.58] to really take MK Docs seriously
[903.58 → 905.82] and really went through
[905.82 → 906.34] the documentation
[906.34 → 907.66] with a fine tooth comb.
[907.84 → 908.80] And I've enabled
[908.80 → 909.96] all the features that I want.
[910.16 → 910.84] And the only thing
[910.84 → 912.16] I haven't done yet is comments,
[912.38 → 913.94] which I might do.
[914.02 → 914.48] I might not.
[914.56 → 915.46] I haven't decided yet.
[915.98 → 918.24] But the material theme
[918.24 → 920.72] for MK Docs really is stunning.
[921.08 → 923.36] And I don't think at the moment
[923.36 → 924.74] there's a better open source
[924.74 → 926.88] documentation platform.
[927.48 → 928.04] Yeah, I will say
[928.04 → 929.26] that just the presentation,
[929.54 → 930.52] so not even commenting
[930.52 → 931.04] on what it's like
[931.04 → 932.62] to actually write on it,
[932.66 → 933.28] but the presentation
[933.28 → 935.48] is extremely readable.
[936.26 → 936.82] You know, documentation,
[937.14 → 938.32] especially something
[938.32 → 939.86] as extensive as a topic like this,
[939.92 → 941.08] can be just a chore
[941.08 → 941.76] to get through.
[942.18 → 943.40] But the way it lays out,
[943.46 → 943.90] like you said,
[943.94 → 944.44] the way it does
[944.44 → 945.42] some of the different quoting
[945.42 → 946.92] and code blocks
[946.92 → 948.14] and all of it,
[948.26 → 950.02] just all of it is really,
[950.10 → 950.40] it's just,
[950.50 → 951.42] it makes me want to use it
[951.42 → 951.94] for my stuff.
[951.94 → 953.02] So I was going to ask you,
[953.02 → 953.66] I was going to talk to you
[953.66 → 954.24] about MK Docs
[954.24 → 954.86] and see what you thought
[954.86 → 956.70] because, yeah,
[956.78 → 957.72] it really seems impressive
[957.72 → 960.86] and probably the perfect solution
[960.86 → 963.88] for just JB internal documentation.
[964.38 → 964.66] Yeah, I mean,
[964.80 → 965.28] it's all,
[965.50 → 966.68] everything's written in Markdown.
[967.52 → 968.96] So if in the future
[968.96 → 969.80] you decided to use
[969.80 → 970.64] a different solution
[970.64 → 971.34] for some reason,
[972.14 → 973.24] it's just plain text.
[973.34 → 974.94] It's not in a CMS somewhere.
[975.46 → 976.40] It lives in a Git repo.
[976.90 → 978.14] You can just copy and paste
[978.14 → 978.70] and job done.
[979.08 → 979.84] That's pretty nice.
[980.22 → 981.94] Well, so as we record right now,
[981.94 → 983.64] this isn't live.
[983.90 → 985.26] So what's your plan?
[985.30 → 985.86] I assume you're going to try
[985.86 → 986.36] to get it out
[986.36 → 987.62] when the show goes live.
[988.12 → 989.06] If you look at my GitHub
[989.06 → 990.42] commit history this week,
[990.42 → 991.90] it's going to be bright green.
[992.30 → 992.70] Yeah.
[993.42 → 994.92] I'm working away feverishly
[994.92 → 995.66] on this to get it done
[995.66 → 996.42] by the end of 2020.
[996.84 → 998.12] So I'm aiming
[998.12 → 999.46] for a New Year's Eve launch.
[999.56 → 1000.34] So by the time you listen
[1000.34 → 1000.98] to this episode,
[1001.06 → 1001.86] it should be live.
[1002.58 → 1003.38] PerfectMediaServer.com.
[1003.50 → 1004.32] Let me know what you think
[1004.32 → 1005.74] at Ironic Badger on Twitter.
[1005.74 → 1007.96] I would love to hear
[1007.96 → 1008.38] what you think
[1008.38 → 1009.58] because I've put a lot of time,
[1010.04 → 1011.20] probably several hundred hours
[1011.20 → 1012.60] into this site
[1012.60 → 1013.24] by the end of it,
[1013.42 → 1014.14] all told.
[1014.76 → 1016.08] I'd also accept PRs
[1016.08 → 1016.84] on the GitHub repo.
[1016.98 → 1017.86] So if you want to open an issue,
[1017.94 → 1018.72] if you find a mistake
[1018.72 → 1019.82] or something,
[1019.96 → 1021.08] which is highly likely
[1021.08 → 1021.54] at the pace
[1021.54 → 1022.44] I'm working right now,
[1023.18 → 1023.62] let me know
[1023.62 → 1024.46] through a GitHub issue
[1024.46 → 1025.44] or open a pull request
[1025.44 → 1025.80] or something.
[1025.88 → 1026.78] I would love to hear from you.
[1026.78 → 1027.18] Okay.
[1027.58 → 1032.42] Needs more Butters documentation.
[1033.20 → 1033.64] Serious.
[1033.64 → 1034.52] Seriously.
[1035.26 → 1035.74] Jeez.
[1037.88 → 1038.74] You, sir,
[1038.86 → 1040.54] are a grade A troll.
[1040.74 → 1041.18] Thank you.
[1043.56 → 1044.66] Linode.com
[1044.66 → 1045.86] slash SSH.
[1045.96 → 1046.24] Go there
[1046.24 → 1047.50] to get a $100
[1047.50 → 1048.90] 60-day credit
[1048.90 → 1049.68] towards a new account
[1049.68 → 1050.76] and go there
[1050.76 → 1051.54] to support the show.
[1051.94 → 1052.68] Linde is our
[1052.68 → 1053.78] cloud hosting provider
[1053.78 → 1054.84] and because the price
[1054.84 → 1055.32] is so great,
[1055.44 → 1056.40] they can make it possible
[1056.40 → 1058.24] for you to use Linde
[1058.24 → 1059.60] even for a small deployment
[1059.60 → 1061.06] or for a large deployment.
[1061.68 → 1062.44] Jeff used Linde
[1062.44 → 1063.26] to test migrate
[1063.26 → 1063.82] his important
[1063.82 → 1064.72] Nextcloud setup.
[1065.10 → 1066.04] He just took things
[1066.04 → 1067.24] one step at a time
[1067.24 → 1068.26] using different guides
[1068.26 → 1068.74] on Linde
[1068.74 → 1069.24] to make sure
[1069.24 → 1070.10] everything was right
[1070.10 → 1071.48] and he says
[1071.48 → 1072.36] eventually after about
[1072.36 → 1073.32] three pages of notes
[1073.32 → 1074.80] he did a completed
[1074.80 → 1076.26] successful migration
[1076.26 → 1077.46] and then he was able
[1077.46 → 1078.84] to take that knowledge,
[1079.52 → 1080.76] take that hands-on experience
[1080.76 → 1083.62] and go actually implement it
[1083.62 → 1084.28] on his production
[1084.28 → 1085.12] Nextcloud instance.
[1085.50 → 1085.70] He said,
[1085.78 → 1086.36] but in the testing
[1086.36 → 1087.32] he noticed that
[1087.32 → 1090.26] even their smaller Li nodes
[1090.26 → 1091.98] were still faster
[1091.98 → 1092.68] than his local
[1092.68 → 1093.30] quad-core
[1093.30 → 1094.12] 16-gigabyte
[1094.12 → 1094.86] local machine.
[1096.14 → 1098.14] So he's looking at
[1098.14 → 1098.92] maybe just hosting it
[1098.92 → 1099.92] on Linode.com
[1099.92 → 1100.94] And Alex,
[1101.04 → 1102.06] I know that you're using
[1102.06 → 1102.52] Linde for
[1102.52 → 1103.86] the perfectmediaserver.com
[1103.86 → 1105.10] I sure am, yeah.
[1105.32 → 1106.64] Same node as
[1106.64 → 1107.54] is doing the wiki
[1107.54 → 1109.94] and gallery.self-hosted.show
[1109.94 → 1111.18] is doing
[1111.18 → 1112.74] perfectmediaserver.com
[1112.74 → 1114.40] So you can really squeeze
[1114.40 → 1114.92] quite a lot
[1114.92 → 1115.84] out of these little things.
[1115.84 → 1116.94] I love hearing
[1116.94 → 1118.02] how people are using
[1118.02 → 1118.58] Linde.
[1118.72 → 1119.56] So do let me know
[1119.56 → 1120.82] either at the contact
[1120.82 → 1121.98] forum or at Chris Lass
[1121.98 → 1122.62] on Twitter
[1122.62 → 1124.08] because with $5
[1124.08 → 1125.14] a month rigs
[1125.14 → 1125.96] you can do a lot
[1125.96 → 1127.56] but they also have
[1127.56 → 1129.60] dedicated CPU systems
[1129.60 → 1130.30] or machines
[1130.30 → 1131.30] with tons of RAM
[1131.30 → 1132.44] or lots of GPU
[1132.44 → 1133.72] so go experiment
[1133.72 → 1134.50] with that $100
[1134.50 → 1135.56] 60-day credit.
[1135.98 → 1136.66] They also offer
[1136.66 → 1138.14] S3 object storage.
[1138.50 → 1139.42] This is a great way
[1139.42 → 1140.18] to store things
[1140.18 → 1140.84] in the cloud
[1140.84 → 1142.00] that don't need
[1142.00 → 1142.48] a Linde
[1142.48 → 1142.94] or a server
[1142.94 → 1143.70] sitting in front of them.
[1143.76 → 1144.34] You can just generate
[1144.34 → 1145.00] a public URL
[1145.00 → 1145.72] for that asset.
[1146.24 → 1146.74] I do this
[1146.74 → 1147.66] for soundboard clips
[1147.66 → 1148.66] you can do this
[1148.66 → 1149.22] for websites
[1149.22 → 1150.04] it's a great way
[1150.04 → 1151.00] to get a superfast
[1151.00 → 1151.60] portfolio
[1151.60 → 1152.60] where everything's
[1152.60 → 1153.30] stored statically
[1153.30 → 1154.16] in object storage
[1154.16 → 1155.06] and their prices
[1155.06 → 1155.52] are great.
[1155.80 → 1156.22] They also have
[1156.22 → 1156.96] load balancers
[1156.96 → 1157.26] and they have
[1157.26 → 1157.82] data centres
[1157.82 → 1159.00] in 11 locations
[1159.00 → 1159.76] around the world.
[1160.48 → 1160.88] So you're going to
[1160.88 → 1161.38] find something
[1161.38 → 1161.90] close to you
[1161.90 → 1163.30] or close to your client.
[1163.86 → 1164.18] So go to
[1164.18 → 1165.08] linode.com
[1165.08 → 1166.32] slash SSH
[1166.32 → 1167.06] go there
[1167.06 → 1168.00] get that $100
[1168.00 → 1169.00] 60-day credit
[1169.00 → 1169.94] apply that towards
[1169.94 → 1170.44] a new account
[1170.44 → 1171.56] and go there
[1171.56 → 1172.30] to support the show.
[1172.82 → 1173.92] You help make
[1173.92 → 1175.08] independent content
[1175.08 → 1175.58] like this
[1175.58 → 1175.86] free
[1175.86 → 1176.68] when you go to
[1176.68 → 1177.44] linode.com
[1177.44 → 1178.86] slash SSH.
[1178.86 → 1181.96] I can't quite believe
[1181.96 → 1182.64] just how many
[1182.64 → 1183.48] power line emails
[1183.48 → 1184.30] we had this week
[1184.30 → 1184.86] though can you?
[1185.68 → 1186.74] Alex it was
[1186.74 → 1187.62] wild.
[1187.88 → 1188.66] So I responded
[1188.66 → 1189.74] to several of them
[1189.74 → 1190.16] directly.
[1190.32 → 1190.96] I figured we respond
[1190.96 → 1191.56] to a couple here
[1191.56 → 1192.14] in the show
[1192.14 → 1193.34] when we had a few
[1193.34 → 1193.88] people write in
[1193.88 → 1194.60] about this stuff.
[1194.60 → 1196.24] I kind of suspected
[1196.24 → 1197.04] that power line
[1197.04 → 1197.64] networking was
[1197.64 → 1198.44] probably something
[1198.44 → 1200.88] that got more
[1200.88 → 1202.62] use and deployments
[1202.62 → 1205.28] than kind of
[1205.28 → 1206.32] gets representation
[1206.32 → 1207.16] because there's so
[1207.16 → 1208.06] many scenarios
[1208.06 → 1209.60] where Wi-Fi
[1209.60 → 1210.64] just doesn't work
[1210.64 → 1212.36] especially older
[1212.36 → 1213.08] style Wi-Fi
[1213.08 → 1213.98] non-mesh Wi-Fi
[1213.98 → 1214.90] where like
[1214.90 → 1215.90] either a house
[1215.90 → 1217.48] construction materials
[1217.48 → 1218.08] involved
[1218.08 → 1219.30] or distance
[1219.30 → 1220.98] or all kinds
[1220.98 → 1221.64] of weird things.
[1221.64 → 1223.58] I have a family
[1223.58 → 1224.28] member who's
[1224.28 → 1225.04] next to an airport
[1225.04 → 1226.32] and their
[1226.32 → 1227.22] radio signal
[1227.22 → 1228.12] situation is just
[1228.12 → 1228.50] crazy.
[1229.02 → 1229.48] It's just
[1229.48 → 1230.82] unusable.
[1231.58 → 1231.98] So I
[1231.98 → 1233.14] suspected
[1233.14 → 1234.00] we would hear
[1234.00 → 1234.90] a lot about this
[1234.90 → 1236.86] but JT wrote in
[1236.86 → 1237.50] to say that he's
[1237.50 → 1238.02] been using
[1238.02 → 1238.82] power line adapters
[1238.82 → 1239.76] for a couple of years.
[1240.38 → 1241.26] He currently has
[1241.26 → 1241.94] three of the
[1241.94 → 1243.34] TP-Link AV1000s
[1243.34 → 1243.88] which is the kit
[1243.88 → 1244.28] I bought
[1244.28 → 1246.06] with two different kits
[1246.06 → 1246.84] and he's using them
[1246.84 → 1247.50] without any issues.
[1247.62 → 1247.90] So he bought
[1247.90 → 1248.74] two of the kits
[1248.74 → 1249.70] two of what I have
[1249.70 → 1250.40] and they all
[1250.40 → 1251.00] link together.
[1251.00 → 1251.90] He says I do
[1251.90 → 1252.32] have a problem
[1252.32 → 1252.78] with one of the
[1252.78 → 1253.36] rooms though
[1253.36 → 1254.34] where one adapter
[1254.34 → 1255.00] normally gets about
[1255.00 → 1256.16] 120 megabits
[1256.16 → 1257.64] and then it gets
[1257.64 → 1258.18] out of sync
[1258.18 → 1258.84] and it starts
[1258.84 → 1259.80] dropping packets
[1259.80 → 1260.42] like mad
[1260.42 → 1261.16] dropping the
[1261.16 → 1261.98] bandwidth next to
[1261.98 → 1262.40] nothing
[1262.40 → 1263.06] sometimes even
[1263.06 → 1263.54] less than a
[1263.54 → 1263.98] megabit
[1263.98 → 1264.78] but if I
[1264.78 → 1265.22] unplug and
[1265.22 → 1265.72] rep lug them
[1265.72 → 1266.14] back in
[1266.14 → 1266.62] it seems to
[1266.62 → 1267.00] fix it.
[1267.36 → 1268.12] It happens
[1268.12 → 1268.46] from time
[1268.46 → 1268.94] to time
[1268.94 → 1270.12] but also
[1270.12 → 1270.60] I wanted to
[1270.60 → 1270.96] give just a
[1270.96 → 1271.52] quick shout out
[1271.52 → 1272.68] to cloudfree.shop
[1272.68 → 1273.38] one of our
[1273.38 → 1274.14] official unofficial
[1274.14 → 1274.86] sponsors here
[1274.86 → 1276.06] of the self-hosted
[1276.06 → 1276.54] podcast.
[1277.00 → 1277.38] Coupon code
[1277.38 → 1278.04] self-hosted.
[1278.32 → 1278.54] He said
[1278.54 → 1279.42] cloudfree.shop
[1279.42 → 1281.02] finally gave him
[1281.02 → 1281.88] the kick in the
[1281.88 → 1282.56] butt he needed
[1282.56 → 1283.48] to begin automating
[1283.48 → 1283.92] his home.
[1284.44 → 1284.64] He says
[1284.64 → 1285.10] I never want
[1285.10 → 1285.52] anything really
[1285.52 → 1286.04] connected to the
[1286.04 → 1286.56] cloud and with
[1286.56 → 1287.20] smart plugs from
[1287.20 → 1288.16] cloud free and
[1288.16 → 1288.68] home assistant
[1288.68 → 1289.66] I felt like I
[1289.66 → 1290.22] could finally get
[1290.22 → 1290.56] started.
[1291.06 → 1291.68] The first thing
[1291.68 → 1292.42] that I automated
[1292.42 → 1293.64] was my bearded
[1293.64 → 1294.50] dragon's cage
[1294.50 → 1294.84] lights.
[1295.38 → 1295.62] Yep.
[1295.74 → 1296.24] One of the first
[1296.24 → 1296.80] things I automated
[1296.80 → 1297.32] here in the studio
[1297.32 → 1298.22] was my fish tank
[1298.22 → 1299.16] lights so totally
[1299.16 → 1299.86] totally with you
[1299.86 → 1300.16] JT.
[1300.58 → 1301.08] He says
[1301.08 → 1302.22] which got rid of
[1302.22 → 1302.80] a terrible
[1302.80 → 1303.84] constantly clicking
[1303.84 → 1304.70] analog timer that
[1304.70 → 1305.40] I used to use.
[1305.40 → 1306.68] I also bought a
[1306.68 → 1308.76] D1 mini ESP8266
[1308.76 → 1310.02] Wi-Fi board and
[1310.02 → 1311.54] a BME280 temperature
[1311.54 → 1312.44] pressure and
[1312.44 → 1313.86] humidity sensor and
[1313.86 → 1314.70] combined them into
[1314.70 → 1315.98] an MQTT based
[1315.98 → 1316.80] sensor that home
[1316.80 → 1317.78] assistant uses to
[1317.78 → 1318.48] control the heat
[1318.48 → 1319.40] lamp in the cage.
[1319.50 → 1320.62] Heck yeah he did.
[1321.88 → 1322.68] That's great.
[1322.72 → 1323.42] That's next level.
[1323.82 → 1324.74] Talk about like you
[1324.74 → 1327.30] want a backup no
[1327.30 → 1328.14] fail state for that
[1328.14 → 1328.36] thing.
[1328.76 → 1329.42] He says the
[1329.42 → 1330.36] spousal approval
[1330.36 → 1331.98] factor was very high
[1331.98 → 1333.00] on these purchases
[1333.00 → 1334.46] and the time I
[1334.46 → 1335.48] spent learning to
[1335.48 → 1336.22] solder.
[1337.06 → 1337.66] That's great.
[1337.74 → 1338.26] Says thanks for the
[1338.26 → 1338.92] shows looking forward
[1338.92 → 1339.52] to the next one.
[1339.90 → 1340.60] Good to hear that
[1340.60 → 1340.96] JT.
[1341.06 → 1341.62] I love it when it
[1341.62 → 1342.76] works out and yeah
[1342.76 → 1343.80] for those of you who
[1343.80 → 1344.54] are new to the show
[1344.54 → 1346.28] cloudfree.shop is a
[1346.28 → 1347.20] community built store
[1347.20 → 1349.50] and we're official
[1349.50 → 1350.40] unofficial official
[1350.40 → 1351.52] sponsors, or they are
[1351.52 → 1353.06] we just love them and
[1353.06 → 1354.26] we worked out a deal
[1354.26 → 1355.24] when you use the
[1355.24 → 1356.42] promo code and you
[1356.42 → 1357.34] get devices that
[1357.34 → 1358.84] don't have like the
[1358.84 → 1359.74] cloud connected stuff
[1359.74 → 1360.16] on there.
[1360.64 → 1361.34] You know sometimes I
[1361.34 → 1362.02] like a little cloud
[1362.02 → 1362.70] like I put a sync
[1362.70 → 1363.34] things over up in
[1363.34 → 1364.30] the cloud made
[1364.30 → 1365.68] stuff faster but
[1365.68 → 1366.84] the smart plug that
[1366.84 → 1367.76] controls the old fish
[1367.76 → 1368.70] tank I don't want any
[1368.70 → 1369.40] cloud involved with
[1369.40 → 1370.34] that you know it's
[1370.34 → 1371.66] just how it goes.
[1372.68 → 1373.16] And you also don't
[1373.16 → 1373.68] have to wait
[1373.68 → 1374.42] necessarily on the
[1374.42 → 1375.02] slow boat from
[1375.02 → 1376.16] China sometimes for
[1376.16 → 1376.68] these things to
[1376.68 → 1377.38] arrive so.
[1377.66 → 1378.42] True.
[1378.66 → 1379.52] It is nice that they
[1379.52 → 1380.56] are stateside as well.
[1380.90 → 1381.86] Yeah that's good
[1381.86 → 1382.50] that's a good point.
[1383.78 → 1385.22] Row rote in about
[1385.22 → 1386.48] Power line Finicky and
[1386.48 → 1387.22] I think the reason I
[1387.22 → 1388.40] included his email is
[1388.40 → 1389.30] because he referred to
[1389.30 → 1390.80] us as Chris and the
[1390.80 → 1392.68] Badger which I
[1392.70 → 1395.00] which gave me like
[1395.00 → 1398.50] this morning AM or
[1398.50 → 1400.36] FM radio vibe and I
[1400.36 → 1401.14] just pictured you and
[1401.14 → 1402.42] I'm doing a morning
[1402.42 → 1405.44] WAX Chris and the
[1405.44 → 1406.48] Badger yeah I can I
[1406.48 → 1407.14] can hear it now.
[1407.34 → 1407.80] It's Chris and the
[1407.80 → 1408.16] Badger.
[1409.76 → 1410.64] Welcome to Chris and
[1410.64 → 1411.04] the Badger.
[1411.18 → 1411.68] Chris and the Badger.
[1411.76 → 1412.10] Chris and the Badger.
[1412.18 → 1412.96] It's the Badger.
[1413.68 → 1415.42] Yeah I could see that.
[1416.62 → 1418.06] I want a listener now to
[1418.06 → 1418.98] try and make us a jingle
[1418.98 → 1419.76] Chris and the Badger
[1419.76 → 1420.12] please.
[1420.36 → 1420.92] That would be fun.
[1422.20 → 1423.30] Chris and the Badger in
[1423.30 → 1423.74] the morning.
[1424.46 → 1425.48] He says Chris I was
[1425.48 → 1426.20] surprised to hear about
[1426.20 → 1426.82] your experiences with
[1426.82 → 1427.24] Power line.
[1427.34 → 1427.92] I've been using the
[1427.92 → 1428.74] TP-Link Power line
[1428.74 → 1429.36] products for several
[1429.36 → 1430.82] years now, and I've had
[1430.82 → 1431.78] mixed results and my
[1431.78 → 1433.06] experience it works but
[1433.06 → 1434.20] sometimes it has some
[1434.20 → 1434.92] problems that make it
[1434.92 → 1436.92] hard to really recommend
[1436.92 → 1438.74] and he tells me about
[1438.74 → 1439.76] different products that
[1439.76 → 1440.32] he's tried and
[1440.32 → 1441.42] troubleshooting and he
[1441.42 → 1442.74] has a pretty solid
[1442.74 → 1443.76] looking house layout.
[1444.00 → 1444.32] You know there's
[1444.32 → 1445.36] nothing too crazy about
[1445.36 → 1445.92] his electrical.
[1445.92 → 1447.48] It's a modern house
[1447.48 → 1450.76] and it's shorter than
[1450.76 → 1451.78] 300 meters and all of
[1451.78 → 1452.48] that kind of stuff that
[1452.48 → 1453.04] you'd look at.
[1453.62 → 1454.62] But he says Power line
[1454.62 → 1455.56] works, but it's
[1455.56 → 1456.64] definitely nowhere as
[1456.64 → 1457.86] fast as wired Ethernet.
[1458.46 → 1459.38] In fact it isn't even
[1459.38 → 1460.56] as fast as some of the
[1460.56 → 1462.58] mesh Wi-Fi that he's
[1462.58 → 1462.88] tested.
[1462.98 → 1463.60] So he did several
[1463.60 → 1464.28] different kind of speed
[1464.28 → 1465.16] tests for us and said
[1465.16 → 1467.80] in all he is able to
[1467.80 → 1469.06] get better performance on
[1469.06 → 1471.32] mesh Wi-Fi but in some
[1471.32 → 1473.00] situations where Wi-Fi
[1473.00 → 1473.74] didn't reach or there
[1473.74 → 1475.38] was other issues he was
[1475.38 → 1476.30] still able to get
[1476.30 → 1477.70] around 100, 150
[1477.70 → 1478.92] megabits with his
[1478.92 → 1479.84] Power line adapters.
[1480.58 → 1481.54] In one case depending
[1481.54 → 1482.44] on a product he tried he
[1482.44 → 1483.38] was able to get 300
[1483.38 → 1485.22] megabits which that's
[1485.22 → 1485.88] pretty respectable.
[1486.12 → 1486.76] That's really all I'd
[1486.76 → 1487.52] want over Power line.
[1487.70 → 1488.50] I'm not expecting
[1488.50 → 1489.00] gigabit.
[1489.46 → 1490.14] I mean if all you're
[1490.14 → 1492.28] doing is streaming you
[1492.28 → 1493.50] know on Cody or
[1493.50 → 1494.44] something like that you
[1494.44 → 1495.00] know that's all you
[1495.00 → 1495.38] need.
[1495.58 → 1496.58] He points out, and it's
[1496.58 → 1497.14] a great thing to
[1497.14 → 1498.82] consider is a little
[1498.82 → 1501.26] play of words that
[1501.26 → 1502.60] these manufacturers use.
[1502.84 → 1503.20] Yes.
[1503.38 → 1504.06] And I haven't verified
[1504.06 → 1504.92] this but according to
[1504.92 → 1506.30] him he says when they
[1506.30 → 1507.28] say it's a gigabit
[1507.28 → 1508.74] they mean it's a
[1508.74 → 1509.44] gigabit when you
[1509.44 → 1510.52] combine to send and
[1510.52 → 1510.94] the reception.
[1511.52 → 1512.86] It's actually half a
[1512.86 → 1514.68] gigabit in both
[1514.68 → 1515.24] directions.
[1515.62 → 1516.68] In a perfect world
[1516.68 → 1517.86] when there is no wind
[1517.86 → 1518.46] outside.
[1519.14 → 1519.32] Right.
[1519.56 → 1520.56] They're about one
[1520.56 → 1521.54] centimetre apart
[1521.54 → 1522.44] probably yes.
[1522.92 → 1523.96] So if you get a two
[1523.96 → 1525.34] gigabit model which
[1525.34 → 1526.30] there are two gigabit
[1526.30 → 1527.30] units then it's one
[1527.30 → 1528.22] gigabit send one
[1528.22 → 1529.24] gigabit receive, and it's
[1529.24 → 1531.16] actually a one gigabit
[1531.16 → 1532.22] unit the way we think of
[1532.22 → 1532.92] it in terms of like
[1532.92 → 1533.76] Ethernet adapters.
[1534.40 → 1535.12] So that's a little
[1535.12 → 1536.08] trick of rookies that
[1536.08 → 1537.40] they like to pull that
[1537.40 → 1537.92] when they're quoting
[1537.92 → 1539.00] speeds they're quoting
[1539.00 → 1540.74] just a Sand or receive.
[1541.76 → 1542.70] But we got lots of
[1542.70 → 1543.10] other feedback.
[1543.22 → 1544.02] Some people thought that
[1544.02 → 1545.04] it was that maybe I'd
[1545.04 → 1545.84] have better performance
[1545.84 → 1546.58] if I didn't have solar
[1546.58 → 1549.80] panels on the RV that
[1549.80 → 1550.50] they thought maybe that
[1550.50 → 1551.78] was causing some high
[1551.78 → 1552.80] degree of interference
[1552.80 → 1553.82] just because of you know
[1553.82 → 1554.70] the intensity of that.
[1554.86 → 1556.34] But those systems are
[1556.34 → 1557.02] totally separate.
[1557.36 → 1559.14] The house power doesn't
[1559.14 → 1560.26] connect to like the
[1560.26 → 1562.14] charge controller or the
[1562.14 → 1562.90] batteries directly.
[1563.30 → 1564.16] Yeah because a lot of
[1564.16 → 1565.54] folks wrote in and said
[1565.54 → 1567.34] that if you have coaxed in
[1567.34 → 1567.94] your walls you can
[1567.94 → 1569.66] actually get power line
[1569.66 → 1572.72] over coax adapters and
[1572.72 → 1573.50] because they're not
[1573.50 → 1575.12] carrying any signal in
[1575.12 → 1576.58] modern houses generally
[1576.58 → 1578.68] speaking any more you can
[1578.68 → 1579.70] actually get away with
[1579.70 → 1581.80] you know running Ethernet
[1581.80 → 1583.90] over those, and they're a
[1583.90 → 1585.06] very clean signal so you
[1585.06 → 1585.80] get better performance
[1585.80 → 1586.20] that way.
[1586.58 → 1587.32] That could be worth
[1587.32 → 1587.90] looking into.
[1588.20 → 1590.26] You know I got a couple
[1590.26 → 1591.54] of spots that have coaxed
[1591.54 → 1592.10] pre-run.
[1593.00 → 1593.82] That's interesting.
[1594.14 → 1594.32] Hmm.
[1594.66 → 1594.94] Hmm.
[1595.06 → 1595.78] I don't know Alex.
[1595.86 → 1597.80] Maybe one day in the
[1597.80 → 1598.42] future.
[1599.24 → 1600.90] Brad wrote in about a
[1600.90 → 1603.54] killer MOB with Quick Sync.
[1603.54 → 1604.68] Yeah he's found the
[1604.68 → 1608.16] AS Rock J5040 IT board.
[1608.50 → 1609.74] It's a mini IT form
[1609.74 → 1611.00] factor with a quad-core
[1611.00 → 1613.92] Pentium chip, and it has
[1613.92 → 1615.54] Quick Sync version 605.
[1615.54 → 1617.96] Now he wrote in about
[1617.96 → 1619.70] this one because of
[1619.70 → 1620.50] energy usage.
[1620.64 → 1621.96] This one idles he says
[1621.96 → 1624.48] between 10 and 15 watts
[1624.48 → 1624.86] only.
[1625.42 → 1627.40] But it also has four
[1627.40 → 1628.50] SATA ports which I
[1628.50 → 1630.56] thought hmm this would
[1630.56 → 1632.38] make a really nice sort
[1632.38 → 1633.54] of NAS motherboard
[1633.54 → 1634.54] potentially because you
[1634.54 → 1635.60] know four hard drives
[1635.60 → 1637.74] a small enclosure low
[1637.74 → 1639.58] power draw Quick Sync.
[1640.40 → 1641.08] You know you're pushing
[1641.08 → 1642.24] my buttons here Brad.
[1642.60 → 1643.16] Yeah really.
[1643.16 → 1643.96] Me too.
[1644.32 → 1645.06] It looks like a really
[1645.06 → 1645.74] nice motherboard.
[1645.88 → 1649.66] Yeah this AS Rock J5040
[1649.66 → 1650.16] IT.
[1650.96 → 1651.74] We'll put a link in the
[1651.74 → 1653.72] in the show notes.
[1654.02 → 1655.30] But that hardware
[1655.30 → 1656.16] acceleration that
[1656.78 → 1658.00] Quick Sync boy that
[1658.00 → 1658.84] is looking perfect.
[1658.96 → 1660.02] And this you could
[1660.02 → 1661.28] totally build I bet you
[1661.28 → 1662.76] for if you had the
[1662.76 → 1665.16] storage I bet two
[1665.70 → 1666.40] three hundred dollars
[1666.40 → 1667.64] to build a nice system
[1667.64 → 1668.30] with a decent little
[1668.30 → 1668.70] case.
[1668.88 → 1669.82] There's some memory
[1669.82 → 1670.64] around this thing.
[1671.06 → 1672.82] It's a passive CPU as
[1672.82 → 1674.80] well so it takes it
[1674.80 → 1675.70] doesn't need a fan on
[1675.70 → 1676.18] the CPU.
[1676.92 → 1678.06] Also it takes a
[1678.06 → 1679.50] laptop style SO
[1679.50 → 1680.58] DIM memory.
[1681.32 → 1682.22] So this thing is tiny.
[1682.34 → 1682.86] It's got a couple of
[1682.86 → 1684.46] M2 slots on there for
[1684.46 → 1685.36] Wi-Fi if you want.
[1686.10 → 1687.50] So yeah yeah go
[1687.50 → 1688.10] ahead and check that
[1688.10 → 1688.36] one out.
[1688.42 → 1688.90] That looks like a
[1688.90 → 1689.96] really, really useful
[1689.96 → 1690.50] little build.
[1690.96 → 1691.80] Stefan wrote in to tell
[1691.80 → 1692.72] us about some benchmarks
[1692.72 → 1693.80] in German that show
[1693.80 → 1694.72] that the latest AMD
[1694.72 → 1696.70] desktop Apus are
[1696.70 → 1698.10] getting idle power well
[1698.10 → 1700.22] below 10 watts and
[1700.22 → 1700.72] depending on the
[1700.72 → 1701.70] motherboard as low
[1701.70 → 1702.52] as six or seven
[1702.52 → 1702.92] watts.
[1703.44 → 1704.16] So it seems like
[1704.16 → 1704.72] there's something to
[1704.72 → 1705.42] watch there too.
[1705.86 → 1706.72] Oh I'm trying to
[1706.72 → 1707.88] avoid buying a Ry zen
[1707.88 → 1708.46] 5000.
[1709.12 → 1710.04] I'm really trying to
[1710.04 → 1711.74] avoid it but stuff
[1711.74 → 1713.06] like that makes me
[1713.06 → 1713.96] want to buy one.
[1715.86 → 1716.68] Hey while we're doing
[1716.68 → 1717.30] feedback I want to
[1717.30 → 1717.92] take a moment and
[1717.92 → 1719.38] mention that a cloud
[1719.38 → 1720.86] guru has a Python 3
[1720.86 → 1722.18] scripting course for
[1722.18 → 1723.08] system administrators
[1723.08 → 1724.50] where you can develop
[1724.50 → 1725.24] the skills you need to
[1725.24 → 1725.98] write effective and
[1725.98 → 1727.32] powerful scripts and
[1727.32 → 1728.46] create command line
[1728.46 → 1730.56] tools using Python 3.
[1730.56 → 1731.18] So in the course
[1731.18 → 1731.46] you're going to
[1731.46 → 1732.02] develop skills you
[1732.02 → 1732.36] need to write
[1732.36 → 1732.88] effective and
[1732.88 → 1733.54] powerful Python
[1733.54 → 1734.90] scripts, and it's
[1734.90 → 1736.00] it's a big one.
[1736.10 → 1736.50] So beyond the
[1736.50 → 1737.24] language itself you'll
[1737.24 → 1737.88] go through the full
[1737.88 → 1738.62] development process
[1738.62 → 1739.36] including project
[1739.36 → 1740.12] setup, planning,
[1740.74 → 1741.78] automated testing to
[1741.78 → 1742.30] build two different
[1742.30 → 1743.10] command line tools and
[1743.10 → 1743.34] more.
[1743.82 → 1744.46] So check out the link
[1744.46 → 1745.20] we'll have in the
[1745.20 → 1746.16] show notes for the
[1746.16 → 1747.22] Python 3 scripting for
[1747.22 → 1748.02] system administrators
[1748.02 → 1749.52] at cloudguru.com.
[1750.90 → 1751.94] Hey so I'm sat here
[1751.94 → 1752.34] whilst we were
[1752.34 → 1753.30] recording and thought
[1753.30 → 1754.22] my feet are cold.
[1754.64 → 1755.20] So whilst you were
[1755.20 → 1756.28] reading that ad spot
[1756.28 → 1757.56] I logged into my
[1757.56 → 1758.20] home assistant and
[1758.20 → 1758.86] just bumped up the
[1758.86 → 1759.76] thermostat a little bit.
[1760.56 → 1762.94] It's nice, isn't it?
[1763.56 → 1764.42] Yep, yep.
[1764.64 → 1765.54] I think my favourite
[1765.54 → 1767.66] still is because of
[1767.66 → 1768.10] the HomeKit
[1768.10 → 1769.76] integration when I'm
[1769.76 → 1771.14] driving home I just
[1771.14 → 1771.84] push a button on the
[1771.84 → 1772.96] steering wheel and I
[1772.96 → 1775.10] tell the computer just
[1775.10 → 1776.26] to turn on you know
[1776.26 → 1777.04] the heaters to extra
[1777.04 → 1777.24] heat.
[1777.44 → 1778.00] We have an extra heat
[1778.00 → 1778.52] mode that kind of
[1778.52 → 1779.06] brings up the
[1779.06 → 1780.22] temperature more a
[1780.22 → 1781.48] little quicker and
[1781.48 → 1782.28] so when I buy the
[1782.28 → 1782.84] and turn on the
[1782.84 → 1783.10] lights.
[1783.44 → 1783.96] So when I get home
[1783.96 → 1784.78] all the lights are on
[1784.78 → 1786.06] place is nice and
[1786.06 → 1786.34] toasty.
[1786.34 → 1788.68] Oh I've been
[1788.68 → 1789.32] thinking about like
[1789.32 → 1790.42] an NFC tag on the
[1790.42 → 1791.16] dashboard or something
[1791.16 → 1791.82] that I could just
[1791.82 → 1792.62] tap with my phone
[1792.62 → 1792.96] maybe.
[1793.66 → 1794.68] I haven't done it but
[1794.68 → 1795.22] I've been thinking
[1795.22 → 1795.70] about it.
[1796.18 → 1796.58] I've been thinking
[1796.58 → 1797.14] about that too.
[1797.20 → 1797.84] I actually have an
[1797.84 → 1798.70] NFC tag at the
[1798.70 → 1800.06] door out the
[1800.06 → 1800.78] studio so on my
[1800.78 → 1801.28] way out the
[1801.28 → 1802.36] studio I can tap it
[1802.36 → 1803.10] and right now it
[1803.10 → 1803.70] just kind of sends
[1803.70 → 1804.40] like an alert to the
[1804.40 → 1805.86] wife with an ETA
[1805.86 → 1807.04] and all of that kind
[1807.04 → 1807.98] of stuff you know
[1807.98 → 1808.82] based on my location
[1808.82 → 1810.28] and her location but
[1810.28 → 1810.96] I have been thinking
[1810.96 → 1811.58] man it'd be pretty
[1811.58 → 1812.98] great to tie that in
[1812.98 → 1814.22] with the heating and
[1814.22 → 1815.12] the lighting check to
[1815.12 → 1815.72] see if it's on or
[1815.72 → 1815.98] not.
[1816.54 → 1817.80] NFC tags and all of
[1817.80 → 1819.06] that is probably still
[1819.06 → 1820.28] the most underutilized
[1820.28 → 1821.62] area because on iOS
[1821.62 → 1823.78] it kind of sucks and I
[1823.78 → 1824.48] think it's similar on
[1824.48 → 1825.22] Android but not quite
[1825.22 → 1825.88] the same where on
[1825.88 → 1827.26] iOS it just brings up
[1827.26 → 1827.74] as far as I
[1827.74 → 1828.62] understand it a
[1828.62 → 1829.68] notification prompt
[1829.68 → 1830.34] that you then have to
[1830.34 → 1832.64] tap to execute the
[1832.64 → 1834.46] NFC automation and
[1834.46 → 1835.12] that just sounds like
[1835.12 → 1835.52] garbage.
[1836.04 → 1837.00] Not true on Android I
[1837.00 → 1838.06] just tap the tag and
[1838.06 → 1839.02] my garage door opens
[1839.02 → 1839.58] it's amazing.
[1840.26 → 1840.94] That's what I want.
[1841.34 → 1842.32] I can kind of see
[1842.32 → 1843.52] maybe why Apple did it
[1843.52 → 1844.30] this way for
[1844.30 → 1846.02] novices who you
[1846.02 → 1846.76] know they don't they
[1846.76 → 1847.46] don't want to execute
[1847.46 → 1848.30] stuff randomly on
[1848.30 → 1850.44] their phone but man
[1850.44 → 1852.22] I totally appreciate
[1852.22 → 1853.24] that, but I just would
[1853.24 → 1854.16] love a setting to say
[1854.16 → 1855.28] don't require user
[1855.28 → 1855.78] interaction.
[1856.12 → 1856.22] Yeah.
[1856.34 → 1857.38] It just sort of kills
[1857.38 → 1857.78] the usefulness.
[1857.90 → 1859.02] I have also here on
[1859.02 → 1860.42] the studio mixer I
[1860.42 → 1861.94] have an NFC tag because
[1861.94 → 1862.74] for some reason
[1862.74 → 1863.60] Behringer thought it'd
[1863.60 → 1864.42] be a great idea to put
[1864.42 → 1865.70] a like a phone holder
[1865.70 → 1866.74] on the mixer because
[1866.74 → 1867.46] the ideas are going to
[1867.46 → 1867.84] use like their
[1867.84 → 1868.78] touchscreen app on your
[1868.78 → 1870.94] phone, and so I have a
[1870.94 → 1871.58] spot where my phone
[1871.58 → 1873.88] sits and I just put an
[1873.88 → 1874.80] NFC tag in that spot
[1874.80 → 1875.86] just set my phone to
[1875.86 → 1877.32] D&D and turn on the
[1877.32 → 1878.24] studio lights which are
[1878.24 → 1879.14] on home assistant and
[1879.14 → 1879.66] all that.
[1880.66 → 1881.44] Old wrote into the
[1881.44 → 1882.44] holiday mailbag and
[1882.44 → 1883.16] said I'm a long time
[1883.16 → 1883.98] listener occasional
[1883.98 → 1885.22] disc order from Norway
[1885.22 → 1886.88] and we talk about
[1886.88 → 1887.58] storage setups on the
[1887.58 → 1888.46] show a little bit but
[1888.46 → 1889.14] I'd love you to go into
[1889.14 → 1890.46] some details with
[1890.46 → 1891.88] setups ranging from
[1891.88 → 1892.70] smaller setups to
[1892.70 → 1893.26] bigger setups.
[1893.74 → 1894.10] Do you have any
[1894.10 → 1895.18] strategies deciding on
[1895.18 → 1896.66] what you invest in?
[1897.30 → 1898.28] My backups are going to
[1898.28 → 1899.44] back blaze, but I'm
[1899.44 → 1900.48] rethinking things a little
[1900.48 → 1901.18] bit and I think I want
[1901.18 → 1901.88] more sane local
[1901.88 → 1903.16] storage, but I'm a
[1903.16 → 1903.84] little put off at the
[1903.84 → 1904.18] price.
[1905.20 → 1905.80] What would be a sweet
[1905.80 → 1906.56] spot in terms of
[1906.56 → 1908.00] discs and storage for
[1908.00 → 1909.18] about an 8 terabyte
[1909.18 → 1910.42] media collection as
[1910.42 → 1910.94] well as some more
[1910.94 → 1912.00] personal media like
[1912.00 → 1913.26] photos that I just
[1913.26 → 1914.02] don't want to lose?
[1914.42 → 1915.02] Any links would be
[1915.02 → 1915.44] great too.
[1915.84 → 1916.78] Man this question was
[1916.78 → 1917.76] made for me, wasn't it?
[1917.88 → 1919.00] It really was.
[1919.34 → 1921.74] So perfectmediaserver.com
[1921.74 → 1923.84] first I think is
[1923.84 → 1925.14] where I will send you in
[1925.14 → 1926.96] the first instance to
[1926.96 → 1927.52] look at the software
[1927.52 → 1928.20] side of things.
[1928.80 → 1930.06] I will be building up the
[1930.06 → 1931.04] hardware recommendations
[1931.04 → 1932.12] section of that site
[1932.12 → 1932.80] over the next few
[1932.80 → 1935.06] months but really I
[1935.06 → 1935.86] would just take a look
[1935.86 → 1937.06] at serverbuilds.net.
[1937.38 → 1938.82] They have some amazing
[1938.82 → 1940.84] used enterprise gear and
[1940.84 → 1942.06] I know it's quite a US
[1942.06 → 1944.28] centric website but you
[1944.28 → 1945.16] can still get a lot of
[1945.16 → 1946.26] good ideas about what to
[1946.26 → 1947.34] use like Quick Sync for
[1947.34 → 1949.08] example that that came
[1949.08 → 1950.42] from JDM the guy behind
[1950.42 → 1951.40] that site who we've had on
[1951.40 → 1953.32] the show before and just
[1953.32 → 1953.98] take a look at what
[1953.98 → 1954.86] they're doing and the
[1954.86 → 1956.12] trends and the way the
[1956.12 → 1957.34] industry is going with
[1957.34 → 1958.48] what those guys are doing
[1958.48 → 1959.26] over there at server
[1959.26 → 1961.32] builds and I think you
[1961.32 → 1961.96] can probably get away
[1961.96 → 1963.56] with a fairly minimal
[1963.56 → 1964.38] kind of setup.
[1964.54 → 1965.06] So you've got 8
[1965.06 → 1966.16] terabytes worth of stuff
[1966.16 → 1967.78] you want to store, so I
[1967.78 → 1969.16] would buy a hard drive
[1969.16 → 1971.46] that is at least 8
[1971.46 → 1972.78] probably 10 or 12
[1972.78 → 1973.74] terabytes so you've got a
[1973.74 → 1975.58] bit of headroom and buy
[1975.58 → 1976.74] a pair of them so that
[1976.74 → 1978.64] you know can have
[1978.64 → 1980.24] full redundancy.
[1981.12 → 1981.92] You're already using
[1981.92 → 1983.48] Back blaze so you know
[1983.48 → 1985.48] raid is not backup is a
[1985.48 → 1986.70] very common phrase that
[1986.70 → 1987.60] you'll hear people say.
[1987.60 → 1989.60] Make sure that you have
[1989.60 → 1991.96] everything duplicated in
[1991.96 → 1993.82] at least two different
[1993.82 → 1994.82] physical locations.
[1995.50 → 1996.56] So even if that just
[1996.56 → 1998.84] takes the form of you
[1998.84 → 1999.88] know a USB hard drive
[1999.88 → 2000.48] that you leave at your
[2000.48 → 2001.28] parents house when you
[2001.28 → 2002.84] go and see them one day
[2002.84 → 2005.38] in the future who knows
[2005.38 → 2007.92] you know the world is so
[2007.92 → 2009.00] different right now but
[2009.00 → 2011.46] if it's just a USB hard
[2011.46 → 2012.76] drive in a drawer at a
[2012.76 → 2014.02] parents house then that
[2014.02 → 2015.08] will do the trick as well
[2015.08 → 2015.78] you know in a lot of
[2015.78 → 2016.96] situations unless you
[2016.96 → 2019.10] have lots of media being
[2019.10 → 2019.98] added all the time but
[2019.98 → 2020.66] I don't think that's the
[2020.66 → 2021.58] use case for a lot of
[2021.58 → 2021.80] people.
[2021.98 → 2023.68] I think most people those
[2023.68 → 2024.98] kind of periodical backups
[2024.98 → 2026.90] every three to six
[2026.90 → 2028.04] months is probably
[2028.04 → 2028.70] sufficient.
[2029.78 → 2032.52] So build yourself you
[2032.52 → 2035.42] know a small mini IT
[2035.42 → 2037.80] couple of bay box and
[2037.80 → 2039.62] you know stick the
[2039.62 → 2040.82] perfect media server stack
[2040.82 → 2041.60] on there, and you'll be
[2041.60 → 2042.02] good to go.
[2042.02 → 2043.94] Yeah thankfully eight
[2043.94 → 2045.02] terabytes is a really
[2045.02 → 2046.86] pretty, pretty doable
[2046.86 → 2047.64] problem to solve.
[2048.14 → 2048.86] So you know of course
[2048.86 → 2049.60] you want more than that
[2049.60 → 2050.34] you're gonna you know at
[2050.34 → 2051.70] least at least I'd say go
[2051.70 → 2053.28] 12 terabytes if not more
[2053.28 → 2054.74] if you already are using
[2054.74 → 2056.34] eight terabytes and you
[2056.34 → 2056.90] could probably even
[2056.90 → 2058.84] justify a bit more than
[2058.84 → 2059.06] that.
[2059.48 → 2060.54] That's some great strategy
[2060.54 → 2061.70] advice right there and
[2061.70 → 2062.74] perfect timing for the
[2062.74 → 2064.54] show too so best of
[2064.54 → 2064.78] luck.
[2065.12 → 2066.20] I would take a look at
[2066.20 → 2069.04] amazon.de quite often
[2069.04 → 2070.94] have the Western Digital
[2070.94 → 2072.28] what are they called
[2072.28 → 2072.68] over there?
[2072.98 → 2073.80] They're not easy stores
[2073.80 → 2074.62] because they're Best Buy
[2074.62 → 2075.74] like US centric ones
[2075.74 → 2077.66] they're called My Books I
[2077.66 → 2078.74] think in Europe.
[2079.30 → 2080.66] You can quite often get
[2080.66 → 2082.50] those for a know 10
[2082.50 → 2084.06] 12 14 terabyte hard drive
[2084.06 → 2086.34] in the 200 250 euro
[2086.34 → 2088.16] range so that would be a
[2088.16 → 2089.14] good place to start it's
[2089.14 → 2089.72] not going to be super
[2089.72 → 2090.08] cheap.
[2090.74 → 2092.76] My philosophy with regards
[2092.76 → 2094.84] to how much local storage
[2094.84 → 2096.58] do I need versus cloud is
[2096.58 → 2099.36] it's up to you right it's
[2099.36 → 2101.42] it's your personal risk
[2101.42 → 2103.28] profile or and how
[2103.28 → 2104.84] important is this data to
[2104.84 → 2105.14] you?
[2106.04 → 2106.82] Are you going to be upset
[2106.82 → 2108.44] if is back blaze and I
[2108.44 → 2108.86] don't know if they're
[2108.86 → 2110.28] going to but if they turn
[2110.28 → 2111.60] around next week and you
[2111.60 → 2112.76] know triple their prices
[2112.76 → 2113.36] what are you going to do
[2113.36 → 2114.02] if that happens?
[2115.02 → 2116.16] If you have a hard drive
[2116.16 → 2118.54] in your closet you know
[2118.54 → 2120.40] up front what that cost is
[2120.40 → 2121.20] going to be what the total
[2121.20 → 2122.22] cost of ownership for that
[2122.22 → 2124.10] that storage is going to be
[2124.10 → 2125.04] and there 's'll be no
[2125.04 → 2126.10] surprises or anything like
[2126.10 → 2127.72] that, so I mean you're
[2127.72 → 2128.38] talking to a guy that's got
[2128.38 → 2129.36] 100 terabytes in his
[2129.36 → 2130.42] basement, so maybe I'm not
[2130.42 → 2132.26] the right guy to speak to
[2132.26 → 2132.88] you know.
[2133.14 → 2134.12] And the other guy who's
[2134.12 → 2134.84] like I need to get more
[2134.84 → 2135.88] disk as fast as possible
[2135.88 → 2136.96] I've only got 12 terabytes
[2136.96 → 2138.94] free right now like yeah
[2138.94 → 2141.46] yeah but really there's so
[2141.46 → 2143.56] many ways to solve it but
[2143.56 → 2144.58] I'd love to hear what you
[2144.58 → 2145.78] do so go to self-hosted
[2145.78 → 2146.90] dot show slash contact to
[2146.90 → 2148.50] update us and then Scott
[2148.50 → 2149.32] wrote in with another
[2149.32 → 2150.90] another question I have a
[2150.90 → 2152.14] sense the audience may have
[2152.14 → 2153.30] a few answers for us so
[2153.30 → 2154.42] keep that contact link in
[2154.42 → 2155.88] mind he says I was hoping
[2155.88 → 2156.52] you could make a
[2156.52 → 2158.00] recommendation for self-hosted
[2158.00 → 2160.60] online cookbook my mother
[2160.60 → 2162.34] has a huge cookbook full of
[2162.34 → 2164.48] old family recipes which I
[2164.48 → 2165.52] would like to digitalize
[2165.52 → 2168.16] ideally with OCR and the
[2168.16 → 2169.44] ability to take and search
[2169.44 → 2170.48] the recipes as well as
[2170.48 → 2172.00] preserving original image of
[2172.00 → 2173.36] the old handwritten family
[2173.36 → 2175.60] recipe Scott I love this
[2175.60 → 2177.32] idea what do you think
[2177.32 → 2178.70] Alex has anything come to
[2178.70 → 2180.12] mind for you well we
[2180.12 → 2181.68] covered chow down a little
[2181.68 → 2183.40] while ago as a self-hosted
[2183.40 → 2185.26] recipes app there is another
[2185.26 → 2186.98] one which whilst we're doing
[2186.98 → 2188.44] this segment I will try and
[2188.44 → 2190.02] find which I can't remember
[2190.02 → 2191.86] right now but there is also
[2191.86 → 2194.22] an old JB project isn't it
[2194.22 → 2196.26] yeah that's true that is true
[2196.26 → 2198.56] there is the open your
[2198.56 → 2200.30] mouth recipes which we
[2200.30 → 2201.56] actually used GitHub and
[2201.56 → 2203.30] Markdown for those I was
[2203.30 → 2204.18] thinking you know Scott could
[2204.18 → 2206.54] get started with even out any
[2206.54 → 2207.96] without any software selected
[2207.96 → 2209.36] yet by just getting good
[2209.36 → 2212.26] quality captures of those cards
[2212.26 → 2213.84] and he's going to want probably
[2213.84 → 2214.98] something he can take over to
[2214.98 → 2216.90] grandma's house or mom's house
[2216.90 → 2219.98] or whoever the
[2219.98 → 2220.70] family members you want to
[2220.70 → 2221.60] capture these from because why
[2221.60 → 2223.14] not get them all right you
[2223.14 → 2224.50] could probably get away with
[2224.50 → 2226.56] something like scan bot or the
[2226.56 → 2229.16] other available scanning apps on
[2229.16 → 2230.02] your phone, but you might look
[2230.02 → 2231.10] into scanner options too and
[2231.10 → 2232.80] just start there start getting the
[2232.80 → 2234.86] high quality images from there and
[2234.86 → 2237.06] then the software will come I
[2237.06 → 2238.60] found it okay it's called
[2238.60 → 2243.70] vapeen 1111 slash recipes what a
[2243.70 → 2245.68] catchy name huh it's a Django
[2245.68 → 2247.26] application designed for managing
[2247.26 → 2249.96] recipes, and it's a web app, so I
[2249.96 → 2251.56] would imagine it runs out of a
[2251.56 → 2253.52] container, but it's got a search
[2253.52 → 2256.26] built on top of Django's trigram
[2256.26 → 2259.24] similarity search engine and it
[2259.24 → 2260.72] allows you to create and search for
[2260.72 → 2263.28] tags and assign them in batches to
[2263.28 → 2264.64] certain files matching certain
[2264.64 → 2266.90] criteria it will sync with both
[2266.90 → 2269.80] Dropbox and next cloud with more
[2269.80 → 2271.62] support being added every
[2271.62 → 2273.96] week, and you can import lots of
[2273.96 → 2275.72] recipes from different websites
[2275.72 → 2278.14] with JSON objects and stuff like
[2278.14 → 2279.94] that and there are also apps for
[2279.94 → 2281.52] mobile devices like phones and
[2281.52 → 2283.96] tablets so yeah lots and lots of
[2283.96 → 2285.80] stuff in their runs in a docker
[2285.80 → 2289.38] this is what the Reddit collective
[2289.38 → 2292.98] thought recommends at the moment so I
[2292.98 → 2294.56] haven't tried this one I just
[2294.56 → 2295.72] haven't got to it, but it's on my
[2295.72 → 2297.00] short list so go and take a look at
[2297.00 → 2299.10] that link in the show notes I also
[2299.10 → 2302.16] recall that groceries had a bit of a
[2302.16 → 2304.12] recipe manager I don't recall how
[2304.12 → 2306.76] extensive it was but that's a past
[2306.76 → 2308.92] pick too so we'll put links to all of
[2308.92 → 2310.06] these the one that Alex just talked
[2310.06 → 2312.02] about you could see the example of
[2312.02 → 2313.34] how we used open your mouth on
[2313.34 → 2315.08] GitHub and just made it a community
[2315.08 → 2316.30] project so you could have multiple
[2316.30 → 2317.78] family members that contribute that
[2317.78 → 2320.02] way or perhaps somebody out there will
[2320.02 → 2322.34] know a great software project that we
[2322.34 → 2323.86] haven't mentioned and inform us all
[2323.86 → 2325.40] itself posted that show slash contact
[2325.40 → 2327.58] the last one in our holiday
[2327.58 → 2329.82] extravaganza mailbag here is a Asia
[2329.82 → 2332.90] writes in regarding thoughts that were
[2332.90 → 2334.84] inspired by self-hosted episode 33
[2334.84 → 2337.58] triggered by the hello 64 discussion he
[2337.58 → 2338.92] says hey guys I was listening to your
[2338.92 → 2340.82] review of the hello 64 with some
[2340.82 → 2342.38] interest since I am the owner of their
[2342.38 → 2344.86] previous product the Helios for I
[2345.56 → 2346.92] believe the points you make about
[2346.92 → 2348.84] software are quite valid, yet I'd like to
[2348.84 → 2350.46] point out that there's a really hard
[2350.46 → 2353.02] problem to solve I work personally with
[2353.02 → 2355.40] a company in Israel that makes SBCs and
[2355.40 → 2358.62] Some mostly with ARM based system on
[2358.62 → 2361.06] chips it's my job to make Debian
[2361.06 → 2362.76] available for each product to their
[2362.76 → 2365.62] customers long ago when I started I
[2365.62 → 2367.12] really wanted to do this the right way
[2367.12 → 2369.14] I submitted bug reports and patches to
[2369.14 → 2370.50] the Debian project for enabling all
[2370.50 → 2373.04] kinds of small things a kernel.config for
[2373.04 → 2374.68] a driver here a customized boot script
[2374.68 → 2377.12] there enabling open GL ES backends and
[2377.12 → 2379.88] shared libraries and continuously watching
[2379.88 → 2382.42] and testing the distributions for things
[2382.42 → 2385.04] that break turns out I never got to the
[2385.04 → 2386.78] point where I could give customers a
[2386.78 → 2388.64] pure Debian system there's always
[2388.64 → 2390.54] another tweak that I had to carry out
[2390.54 → 2392.78] of tree so to this day I'm creating
[2392.78 → 2394.54] block device images with custom kernel
[2394.54 → 2397.54] packages integrated binary blobs and
[2397.54 → 2398.96] maybe a system service for loading
[2398.96 → 2401.12] Bluetooth firmware and even patch parts
[2401.12 → 2404.06] of X or Wayland so why do I tell you
[2404.06 → 2406.10] all of this well the reason being for a
[2406.10 → 2407.74] new product it takes time and
[2407.74 → 2410.10] continued effort for mainlining all the
[2410.10 → 2411.94] things and the experience can differ
[2411.94 → 2414.38] largely by a particular SoC in your
[2414.38 → 2416.64] hands, and you'll find that despite even
[2416.64 → 2417.84] when the vendor does everything right
[2417.84 → 2420.14] it's still not perfect to really solve
[2420.14 → 2421.48] this problem there has to be a way for
[2421.48 → 2423.14] hardware makers who are both capable and
[2423.14 → 2424.76] willing to do the work to achieve
[2424.76 → 2426.26] something greater than what I was able
[2426.26 → 2429.18] to do in my job in his opinion it's just
[2429.18 → 2430.74] not there, yet he says Alex that the
[2430.74 → 2433.64] ecosystem just can't support the kind of
[2433.64 → 2435.64] rapid support that the hardware needs at
[2435.64 → 2437.38] this stage, and you know after reading
[2437.38 → 2439.46] this I was thinking look at the
[2439.46 → 2441.98] Raspberry Pi it's been around forever
[2441.98 → 2443.34] and of course they've had iterations
[2443.34 → 2445.26] that have changed things but you really
[2445.26 → 2447.82] still even there you kind of have to get
[2447.82 → 2451.38] an image that's at least been tested
[2451.38 → 2453.58] for the Raspberry Pi you can now get the
[2453.58 → 2455.68] Ubuntu ARM image, and it will boot on the
[2455.68 → 2457.98] Raspberry Pi, but that's only just recently
[2457.98 → 2459.96] it's, and it's really not there with all
[2459.96 → 2462.10] distros yeah you make a good point I
[2462.10 → 2464.76] mean the Ubuntu image for the Pi 4 has
[2464.76 → 2466.96] made a big difference for me to the
[2466.96 → 2468.94] overall kind of feel of it being a real
[2468.94 → 2472.34] air quotes a real device, and it's now in
[2472.34 → 2474.22] production for me, I'm using it as Pi KVM
[2474.22 → 2476.76] which ironically runs on Arch but anyway
[2476.76 → 2479.56] yeah I agree with you, I mean I ended up
[2479.56 → 2481.50] getting ZFS working on the Helios 64
[2481.50 → 2484.66] after the review in the end it was a few
[2484.66 → 2486.56] days it was a kernel update and DKMS
[2486.56 → 2489.50] started working again but yeah I just
[2489.50 → 2492.50] don't know how without you know an
[2492.50 → 2494.58] Apple level of control over both the
[2494.58 → 2496.54] hardware and software you could ever hope
[2496.54 → 2499.98] to solve this problem fully slow but
[2499.98 → 2501.82] steady there are standards like server
[2501.82 → 2505.38] ready that try to solve this more for the
[2505.38 → 2507.40] data centre, but those lessons could be
[2507.40 → 2508.94] learned in the consumer devices but
[2508.94 → 2511.30] there's just not necessarily the vendor
[2511.30 → 2513.42] buy-in and there's not necessarily the
[2513.42 → 2515.26] vendor buy-in to support the development
[2515.26 → 2516.66] right that's an area where they could
[2516.66 → 2518.58] apply a little bit of leverage they could
[2518.58 → 2520.50] hire people to just write the code and
[2520.50 → 2522.12] contribute it more and participate in
[2522.12 → 2525.34] these projects, but it's only it's only so
[2525.34 → 2528.40] scalable, and it's really not a problem we
[2528.40 → 2531.76] have on the x86 side of things we're so
[2531.76 → 2534.70] kind of swept up by the power usage of arm
[2534.70 → 2538.06] or the small size form factor or the price
[2538.06 → 2540.84] point I think we forget some of the
[2540.84 → 2542.68] luxuries that we've gained over the years
[2542.68 → 2545.04] with the x86 platform it just works you
[2545.04 → 2546.24] don't have to think about it, you don't
[2546.24 → 2550.18] have to grab a special version of a Linux
[2550.18 → 2553.12] distro or windows or whatever it is to
[2553.12 → 2556.46] to run on it and with apple changing to
[2556.46 → 2560.16] arm you know based CPUs it is that's the
[2560.16 → 2561.84] first real departure that mainstream
[2561.84 → 2565.72] computing has seen from x86 instruction
[2565.72 → 2568.78] sets for 15 years yep, and I think that's
[2568.78 → 2572.36] going to influence hopefully in five years
[2572.36 → 2574.82] time or so the rest of the industry will
[2574.82 → 2576.60] will be in a similar position to where
[2576.60 → 2578.30] apple are now with that kind of level of
[2578.30 → 2580.82] integration of course apple will be five
[2580.82 → 2582.44] years further down the road by then so
[2582.44 → 2584.42] who knows maybe they'll never catch up
[2584.42 → 2587.32] but it's a fascinating time for
[2587.32 → 2590.08] sure and I really want to support these
[2590.08 → 2593.20] guys doing these projects like
[2593.20 → 2596.06] COBOL you know they're a small team you
[2596.06 → 2597.24] know they're not they're not doing this
[2597.24 → 2599.04] to become millionaires overnight you know
[2599.04 → 2600.70] it's their doing it for the love I'm
[2600.70 → 2603.22] sure, and they made a really great
[2603.22 → 2605.10] product it just missed in a few key areas
[2605.10 → 2607.22] so I wanted to let some of the listeners
[2607.22 → 2611.36] know that I will be selling my Helios 64
[2611.36 → 2613.50] so if you're interested in the market just
[2613.50 → 2615.82] let me know via Twitter you know you'd
[2615.82 → 2616.88] have to wait for it to ship or anything
[2616.88 → 2618.78] for the next batch we'll sort something
[2618.78 → 2620.32] out just leave a little stink on it when
[2620.32 → 2621.58] you ship it out let's make it real
[2621.58 → 2623.84] special okay get a little bit of your
[2623.84 → 2626.00] stink on there I'll sign the inside in
[2626.00 → 2629.90] Tipped or something how about that I want
[2629.90 → 2631.56] to say also a special thank you to our
[2631.56 → 2633.90] members at self-hosted dot show slash SRE
[2633.90 → 2635.74] you can become a site reliability engineer
[2635.74 → 2638.22] for this show you get a limited ad feed
[2638.22 → 2640.68] and you get extra content you get a post
[2640.68 → 2642.56] show I think it's going to be a boozy
[2642.56 → 2646.10] today so thank you to our SRE team you
[2646.10 → 2648.76] keep this show up and running you are our
[2648.76 → 2650.94] reliability engineers I want to mention
[2650.94 → 2653.22] that you can find our sponsor a cloud guru
[2653.22 → 2655.56] on social media it's just slashed the cloud guru
[2655.56 → 2657.12] on any of the major platforms so like
[2657.12 → 2659.88] YouTube.com slash a cloud guru and go
[2659.88 → 2661.54] find them there now I know that you all
[2661.54 → 2664.06] know how to find this with the gargantuan
[2664.06 → 2665.74] amounts of feedback we've had I mean we
[2665.74 → 2667.46] really only got to a small portion of it
[2667.46 → 2669.92] this episode, but please do keep sending
[2669.92 → 2672.00] it in because it keeps us vitalized and
[2672.00 → 2674.02] connected with you guys and particularly
[2674.02 → 2676.70] in these present times hearing from you
[2676.70 → 2679.36] helps us keep the show focused on what
[2679.36 → 2681.70] you guys want to hear about, so self-hosted
[2681.70 → 2683.70] dot show slash contact is the place to go to
[2683.70 → 2686.06] get in touch with us, you can find me on
[2686.06 → 2687.86] twitter at ironic badger, and I'm there
[2687.86 → 2689.86] too at Chris last and the show is at
[2689.86 → 2691.46] self-hosted show and don't forget the
[2691.46 → 2693.70] network at Jupiter signal thanks for
[2693.70 → 2695.44] listening everybody that was self-hosted
[2695.44 → 2697.08] dot show slash 35
[2697.08 → 2699.68] you
