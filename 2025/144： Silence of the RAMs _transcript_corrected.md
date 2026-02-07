[0.00 → 9.32] Welcome into episode 144. That number divisible by 12, right? That's a special number, at least to younger Alex.
[9.42 → 14.84] Anyway, there's something weird about 144 that I found fascinating. How are you doing, Chris?
[15.94 → 22.90] Well, I'm not quite as interested in 144, but it does feel like a nice milestone because I was looking at the doc template,
[22.90 → 29.82] which we updated at episode 100, and so we've done 44 episodes since the last iteration on the template.
[30.00 → 33.90] We always tweak every episode anyway, but I thought that was kind of noteworthy.
[34.08 → 36.88] Yeah. We're creeping up on 150 now, huh?
[37.08 → 41.50] I feel like all the small talk is to avoid the disastrous week that you've had.
[41.62 → 43.82] Oh, it's been bad.
[44.28 → 47.32] Yeah, I just see hints, and I feel like there's a story here.
[47.68 → 54.04] Well, if I told you it ended up with a dash to micro centre in Charlotte because my server died,
[54.86 → 58.76] that would give you some idea of the seriousness of the situation.
[58.76 → 64.52] Oh, no. Oh, no. That's never good, too, because you're always going with what they have in stock.
[65.16 → 68.22] Actually, that turned out to be... We'll get to that.
[68.48 → 69.52] Okay. Okay, good. Okay.
[70.04 → 76.16] Late last week, I was filming a video for work, and I was talking about self-hosted AI stacks.
[76.16 → 82.18] So, you know, Llama running local models with open web UI, like we talked about in the last episode on this show.
[82.88 → 85.38] And I thought to myself, you know what would be really nice?
[85.76 → 91.74] Is if on camera, if I had a prop in my hand of the GPU that I'm talking about.
[91.98 → 96.88] You know what I'm going to do? I'm just going to run down to the basement, power off the server, pull the graphics card,
[97.30 → 101.92] run back up, film a segment, put the graphics card back in, bad bing, bad boom.
[101.92 → 103.08] No big deal.
[103.62 → 104.46] Yeah. What could go wrong?
[105.60 → 107.34] Yeah, the server didn't turn back on again.
[108.16 → 108.90] Oh, no.
[109.82 → 111.92] All I did was pull the graphics card.
[112.10 → 116.54] Like, I've pulled PCIe cards 8,000 times in my life.
[117.06 → 119.72] I didn't do anything wrong or anything different.
[120.14 → 123.78] Let me ask you, did you rub your feet on the carpet before you touched the machine?
[124.78 → 126.28] I mean, like, what do you think happened?
[126.80 → 128.22] Just died? Do you think what?
[128.22 → 128.40] What?
[128.70 → 134.70] Well, after, so it was a real pickle of an issue to try and diagnose at first.
[135.10 → 138.54] Because I've got PMI for this box, you know, because it's a super micro motherboard.
[138.70 → 139.86] It is an Epic server.
[140.34 → 144.36] So it's the one I made a YouTube video about a year ago.
[144.52 → 145.92] You know, it's a monster.
[146.04 → 154.90] It's got a 7402 Epic chip in it, 256 gigs of RAM, tons of NVMe storage, you know, the works really.
[154.90 → 160.30] And I thought, right, I'm just going to log into the PMI and power it on that way.
[160.34 → 164.56] Because I thought to myself, I pushed the power button before I came back upstairs, didn't I?
[165.42 → 166.16] Yeah, I did.
[166.26 → 167.02] It's like one of those things.
[167.08 → 167.90] Did I lock the car?
[168.70 → 168.84] Yeah.
[169.26 → 170.24] Did I leave the stove on?
[170.42 → 173.80] And I'm back at my desk waiting for it to come back up in the Proxmox cluster.
[173.86 → 176.78] And I'm like, where are you?
[176.92 → 177.50] Where are you, bud?
[178.02 → 180.28] Yeah, I mean, I know it takes a while to post, but come on.
[180.34 → 180.78] Let's go.
[180.78 → 186.12] So then I pulled up KVM, and I'm like, there's nothing there.
[186.52 → 187.08] Dead signal.
[187.36 → 188.62] No VGA output.
[188.82 → 190.50] And I'm like, uh-oh.
[190.96 → 196.94] So at that point, I'm like, okay, I've probably mis plugged something in, or I didn't push the power button or whatever.
[197.78 → 202.06] PMI, and then I logged into the PMI of the box itself, not just KVM.
[202.88 → 205.38] Wasn't reading any sensors or anything.
[205.38 → 209.52] I could still log in, but it wasn't initialized properly.
[209.52 → 212.38] So I'm like, huh, that's weird.
[212.52 → 213.52] Never seen that before.
[214.42 → 216.46] So then I headed down to the basement, had a look.
[216.54 → 218.50] The fans were spinning, sure enough, powered on.
[218.58 → 222.38] So I'm like, right, and pull it out of the rack, get it on top of the rack and have a look at it.
[222.44 → 228.54] And there was a little LED blinking on the motherboard called, it's named M1LED.
[229.62 → 236.06] So I tapped that into Google and had a little look and came across, there was a link in the show notes,
[236.06 → 238.42] to a serve-the-home thread.
[239.10 → 243.64] It may as well be called serve-the-home of Alex's server is dead.
[244.58 → 245.86] Serve-the-home death.
[246.52 → 246.60] Yeah.
[246.60 → 255.68] Yeah, it turns out that there is, I have the revision 1.1 of this H12SSL-I motherboard.
[256.26 → 256.54] Okay.
[256.82 → 263.92] And it turns out that the area right underneath where all the PCIe cards, you know how the shape of a PCIe card,
[264.00 → 270.20] you've got the slot on the board and then there's a gap between the plastic slot and the back of the motherboard.
[270.70 → 271.12] Yeah, sure.
[271.12 → 277.00] There's sometimes some chips in there, you know, like audio chips and things like that they just use that dead space for.
[278.04 → 281.98] Well, on this motherboard, that's where the BMC and all of its dubbins lives.
[282.56 → 293.42] And it turns out it's extremely sensitive to any kind of overheating or any kind of PCIe devices knocking capacitors off the board, that kind of thing.
[293.44 → 295.54] That's what this thread was kind of pointing me towards.
[295.54 → 297.16] And you've been doing both, right?
[297.20 → 301.80] I mean, this thing's been cooking on AI tasks and, you know, pulling it in and out.
[302.32 → 303.34] Anything could have happened in there.
[303.34 → 303.52] Yeah.
[303.78 → 309.50] So I got my camera out and took some really high-res pictures because, you know, my eyes are getting old, and I can't see.
[310.32 → 311.74] And had a good look.
[311.84 → 316.80] And so far as I can tell, I've done absolutely nothing physical to the board.
[316.80 → 323.52] So when you start looking deeper in the thread, there are a bunch of guys getting multimeters out and measuring capacitance and resistance.
[323.90 → 326.18] And they're just like, oh, I just can't.
[326.28 → 331.52] I just, because these are tiny, tiny, tiny little, like, they're smaller than a grain of rice.
[331.92 → 334.72] Some of the SM, the surface mount components on this board.
[335.76 → 337.06] So, yeah, she's dead, Jim.
[337.32 → 341.86] The Epic server, the motherboard, super micro, piece of garbage is dead.
[341.86 → 346.46] And, man, you hate to see something like that take out a whole system, right?
[346.48 → 348.12] It's such a simple design mistake.
[348.90 → 350.92] I know that, I know space is tight on those boards.
[351.28 → 357.88] But those PCI cards, I mean, what kind of PCI card are you putting in a server that probably isn't getting hot?
[358.02 → 358.26] Yeah.
[358.56 → 358.80] Right?
[358.92 → 363.18] And it's going to be, the reason why those slots are there is that people take things in and out.
[363.32 → 363.54] It's just.
[363.84 → 370.98] You see people in this thread, they put captain tape over the top of the chips that are there and foam and all sorts of stuff.
[370.98 → 373.04] And I'm just like, man.
[373.24 → 377.82] There are some people in the thread, too, that have actually had super micro RMA the board successfully.
[378.44 → 384.00] But I'm not sure if I'm going to have much luck with that, given I bought it 13 months ago from a Chinese eBay seller.
[384.78 → 384.94] You know?
[386.66 → 387.96] Yeah, I suppose not.
[388.70 → 391.78] You've got a dead system, and you've figured out it's probably this.
[392.16 → 394.84] So, this is where I imagine the trip to the store comes in.
[395.50 → 395.96] Well, yeah.
[396.20 → 398.26] I mean, I'm not one to waste a crisis.
[398.54 → 399.04] You know what I mean?
[399.04 → 402.38] Like, it's a chance for an upgrade, of course.
[403.02 → 419.60] I mean, actually, funnily enough, I was talking with Stephen, you know, the guy up in Toronto, talking about how a few weeks ago that I was finding the Epic 7402 single thread performance a little bit slow for things like Windows Virtual Machines and what have you.
[419.60 → 423.20] Just the single thread performance just wasn't quite where I wanted it.
[423.26 → 429.06] And I was kind of looking around on eBay going, oh, maybe I could spend a little bit and get a faster CPU.
[429.54 → 431.72] And, nah, the one I've got works just fine.
[431.86 → 433.24] And kind of put that one on ice.
[433.24 → 442.88] And then I said to myself, right, once the attic is done, and you can film it properly, you can make a proper content series out of it, you're allowed to spend some money.
[443.60 → 445.96] Until then, just sit on it.
[446.60 → 446.78] Yeah.
[446.86 → 448.04] So, that kind of went out the window.
[448.14 → 449.24] The attic's still not done.
[449.24 → 452.20] They've painted it, at least, up there.
[452.30 → 453.92] But we don't have any carpet yet.
[454.32 → 456.74] Don't have any AC or HVAC up there yet.
[456.92 → 458.44] So, you know, progress in progress.
[459.26 → 462.24] So, I sort of looked around at the options I've got.
[462.54 → 466.06] And Epic chips, the newer ones, still look fantastic.
[466.68 → 476.70] But, again, the single core performance of an Epic chip is, well, they're designed to be multicore, multi-thread workload chips.
[476.70 → 484.34] They're not designed to be, like, desktop, you know, they're just not fast, single-thread performance systems.
[484.88 → 484.96] Sure.
[485.44 → 496.20] So, I thought, well, what about if I went for, like, a modern Ry zen, like an AM5, like a 9950X or something like that, that's got loads of threads, can run at 5 gigahertz, take lots of RAM, all the rest of it.
[497.24 → 501.20] Trouble is, they just don't have enough PCIe lanes from what I'm wanting to do.
[501.82 → 504.42] Like, I've got a pair of U.2 NVMe SSDs.
[504.42 → 512.92] I've got, I think, about six M.2 SSDs in there for things like caches as I'm doing video editing off the server over the network.
[513.66 → 515.66] You know, app data for all my containers.
[516.08 → 518.02] And just a bunch of stuff going on in there.
[518.14 → 524.96] Not to mention an NVIDIA GPU and the Intel Arc Pro GPU and a 10 gig SFP Plus network card.
[524.96 → 527.24] So, there's a lot going on in there.
[527.68 → 530.38] Yeah, you legitimately need to be thinking about the PCIe lanes.
[530.76 → 537.18] So, I sort of went to Perplexity and Claude and sort of said, you know, what are my options and how many lanes do I actually need?
[537.28 → 543.42] And we're, you know, just trying to talk it through with someone, you know, AI doing whatever it's doing.
[543.42 → 549.78] And I didn't expect this really from Perplexity, but it came out with, well, why don't you look at Thread ripper?
[550.26 → 551.32] And I'm like, Thread ripper?
[551.42 → 551.92] I've heard of that.
[552.06 → 553.30] I've heard Wendell talk about Thread ripper.
[553.42 → 554.56] Maybe I should look at Thread ripper.
[555.02 → 555.48] Right, sure.
[556.16 → 566.56] It turns out its kind of this nice middle ground between an AM5 desktop chip and the epic kind of massively multithreaded server-grade chip.
[566.56 → 570.96] It's basically a high-end desktop workstation chip.
[571.72 → 573.30] And I assume it's got the lanes you need?
[573.66 → 574.38] It does indeed.
[574.50 → 579.54] So, the Thread ripper Pro 5955WX is what I ended up going with.
[580.18 → 590.24] And in the end, I ended up picking that because Micro Centre had it in stock in Charlotte, which is a two-and-a-half-hour drive for me, you know?
[590.70 → 592.76] So, that's 16 cores, 4 gigahertz?
[592.76 → 599.94] Yeah, 16 cores, 32 threads, supports up to 2 terabytes of DDR4 memory.
[600.18 → 600.76] Oh, all right.
[600.88 → 601.58] That's another thing.
[602.02 → 610.66] I could reuse the existing memory from my Epic build with the Thread ripper Pro because it's still using DDR4.
[611.48 → 616.88] And then I thought, right, well, what's the use of having a CPU without a motherboard?
[616.98 → 618.46] I've got to find a motherboard in stock.
[619.70 → 621.30] Micro Centre carried that, too.
[621.62 → 621.84] Ah.
[621.84 → 623.56] There's an Asus.
[623.74 → 625.00] What's the model number of this thing?
[626.50 → 630.58] WRX80 Sage Pro Wi-Fi 2 motherboard.
[630.98 → 631.92] Sounds like a Subaru.
[632.22 → 633.72] Oh, dude, have you seen this thing?
[634.66 → 635.48] Yeah, this is.
[635.62 → 636.94] It looks like a tank.
[637.08 → 638.50] I mean, it is slick looking.
[638.62 → 639.96] Just beautiful.
[640.54 → 644.84] It's what motherboards all wish they were.
[645.26 → 647.16] This is like a tactical motherboard is what it is.
[647.22 → 647.48] Yeah, okay.
[647.56 → 650.70] So, let me read off the specs because this thing, it's packing some heat.
[650.70 → 654.46] First, it takes the Thread ripper Pro CPU.
[654.82 → 660.28] It's an extended ATX or EAT motherboard with dual 10 gigabits LAN.
[660.28 → 667.34] We're talking RJ45, not SFP+, unfortunately, but I'll take what I can get.
[667.42 → 668.04] It's built in.
[668.94 → 673.42] Loads of USB 3.2 Gen 2x2 Type-C ports.
[673.62 → 676.40] God, I wish they'd fix the naming of USB, really.
[676.40 → 681.08] And here's where it starts to get really tasty.
[681.86 → 686.60] Seven Gen 4 x 16 PCIe slots.
[687.22 → 687.66] There you go.
[687.72 → 688.04] Seven.
[688.44 → 689.14] Seven of them.
[689.98 → 690.40] Seven.
[692.08 → 693.00] That's nice.
[693.00 → 697.08] And they can all be individually bifurcated.
[698.08 → 704.80] Which means, because this board ships with one of the Asus Hyper M.2 cards,
[705.04 → 708.02] that means theoretically, dear listener,
[708.46 → 715.76] I could put seven times four M.2 cards in those PCIe slots
[715.76 → 725.84] and have 28 M.2 SSDs, NVMe SSDs, running at full bandwidth.
[726.98 → 728.58] I mean, this sounds like a YouTube video.
[728.80 → 729.32] I mean, come on.
[729.94 → 730.20] Right?
[730.26 → 731.02] There's got to be a reason.
[731.32 → 732.54] Yeah, if I'm made of money.
[732.66 → 732.98] Yeah, right.
[733.80 → 734.82] That's pretty nice.
[734.82 → 737.92] A pair of U.2 connectors on board,
[738.12 → 743.42] as well as three on board M.2 Gen 4 slots as well.
[744.64 → 751.42] And a built-in Asus ASM B9 KVM for remote management.
[751.80 → 752.24] Exactly.
[752.58 → 755.28] Yeah, it's got an KVM built right in.
[755.82 → 759.80] Not that I, I don't know, I don't really need it with Pi KVM these days,
[759.90 → 761.52] but it sure is nice to have.
[761.52 → 763.64] It is, especially like when you're, you know,
[763.68 → 765.00] in the situation you were just in.
[765.08 → 767.24] It's nice to have that one other thing to be able to check in on.
[767.44 → 767.82] Absolutely.
[768.60 → 771.32] I mean, it's packing so many PCIe slots
[771.32 → 774.98] that it's got two six-pin auxiliary power inputs
[774.98 → 779.18] to make sure that those seven slots have enough juice to,
[779.72 → 782.88] because I think the slots can each provide 75 watts
[782.88 → 785.94] and then the cards have extra cables that go into them
[785.94 → 786.86] to give them more power.
[786.86 → 792.94] But it's just a ridiculous motherboard, honestly.
[793.10 → 796.04] It's by far the nicest motherboard I have ever owned.
[796.24 → 797.22] Ever, ever owned.
[797.48 → 799.24] It's beautiful.
[799.92 → 801.68] It'd be interesting to know how long this one lasts.
[802.32 → 804.28] You know, because this could last a long time.
[804.60 → 805.64] Funny you should say that,
[805.86 → 807.50] because the guy at Micro Centre
[807.50 → 810.12] actually managed to successfully upsell me
[810.12 → 811.40] on their service plan.
[811.40 → 814.80] You got the service plan?
[814.96 → 815.70] Yeah, dude.
[815.76 → 816.48] Okay, let me explain.
[816.70 → 816.98] Let me explain.
[817.02 → 817.28] All right.
[817.42 → 817.64] Okay.
[817.78 → 818.78] So, okay.
[819.26 → 820.68] There's no easy way to say this,
[820.78 → 822.16] but the motherboard was $900.
[823.00 → 824.78] Yeah, it is an expensive motherboard.
[825.10 → 825.24] Yeah.
[825.38 → 826.78] The CPU was $1,000.
[827.60 → 827.78] Yeah.
[828.14 → 830.64] My budget for this upgrade was $2,000.
[831.00 → 832.32] So I'm like, okay.
[833.14 → 833.76] All right.
[833.78 → 835.14] Because I can reuse the RAM.
[835.76 → 835.92] Yeah.
[836.56 → 837.62] Begrudgingly, of course,
[837.62 → 839.72] I mean, deep down inside,
[839.88 → 841.04] 17-year-old me is going,
[841.20 → 842.24] ha, look at this thing.
[842.30 → 842.90] It's amazing.
[843.54 → 845.74] Whilst my credit card's quivering in fear
[845.74 → 846.70] in my back pocket.
[850.48 → 853.02] Unraid.net slash self-hosted.
[853.10 → 854.62] Now is the time to check it out.
[854.70 → 856.20] The new Unpaid 7 is out,
[856.72 → 858.76] and Unpaid is a trusted, powerful,
[858.96 → 860.44] easy-to-use operating system
[860.44 → 861.96] for self-hosted servers
[861.96 → 863.84] and for anyone who just needs to solve
[863.84 → 865.02] network-attached storage.
[865.36 → 866.48] Like most of you out there,
[866.48 → 868.60] you've probably got stuff on hand already,
[868.68 → 869.84] maybe different size drives
[869.84 → 870.84] or different manufacturers.
[871.34 → 872.86] Unpaid can handle that.
[873.24 → 874.40] And with Unpaid 7,
[874.70 → 875.80] they've now rounded out
[875.80 → 877.24] all the ZFS capabilities.
[877.34 → 878.56] I'm talking full capabilities
[878.56 → 879.48] with full integration,
[880.12 → 881.22] hybrid ZFS pools
[881.22 → 882.30] that support a wide range
[882.30 → 883.44] of special VDE types,
[883.90 → 885.06] great VM management
[885.06 → 886.54] that snaps in with all of that.
[886.94 → 889.44] And Unpaid has integrated tail scale,
[889.54 → 890.96] so you can now natively install it
[890.96 → 892.74] along with different Docker applications,
[893.20 → 894.14] so you can put the container
[894.14 → 895.20] directly on your tail net.
[895.20 → 898.46] It's packed with game-changing new features
[898.46 → 899.54] that just make it easier
[899.54 → 900.14] to get started
[900.14 → 901.20] and improve
[901.20 → 902.78] and really refine
[902.78 → 904.70] what's already been there.
[905.08 → 906.00] You hear us talk about
[906.00 → 907.20] so many cool projects,
[907.38 → 909.00] and I know all of us,
[909.12 → 910.66] our privacy is a priority,
[910.78 → 911.24] especially people
[911.24 → 912.00] that listen to this show,
[912.36 → 914.74] but these things require time
[914.74 → 915.32] and a commitment.
[916.04 → 917.88] Unpaid can be your secret tool,
[918.00 → 919.28] your weapon to get started
[919.28 → 920.06] and get going.
[920.56 → 921.46] You know, sometimes for me,
[921.46 → 923.34] like an impending trip
[923.34 → 925.18] just gets that last a bit of,
[925.42 → 925.86] oh my gosh,
[925.88 → 926.70] I got to get this done
[926.70 → 927.48] over the hurdle
[927.48 → 928.40] kind of thing for me.
[928.82 → 929.20] And, you know,
[929.26 → 930.40] Unpaid can be a tool
[930.40 → 932.46] that can let you get going right away
[932.46 → 933.08] with the stuff
[933.08 → 935.08] you already have on hand.
[935.54 → 936.82] And with the new Unpaid 7,
[936.90 → 938.26] it's time to take a look again
[938.26 → 940.44] because things are just really,
[940.68 → 941.60] really humming over there.
[941.92 → 942.28] And, you know,
[942.30 → 943.60] I don't even talk about this very often,
[943.70 → 944.82] but like there's just been
[944.82 → 946.10] a lot of small improvements
[946.10 → 946.60] under the hood
[946.60 → 948.10] to like the Samba file services
[948.10 → 948.90] and NFS
[948.90 → 949.40] and of course,
[949.78 → 951.32] just to the UI to the dashboard.
[951.98 → 953.28] So it's worth a new look
[953.28 → 954.10] if you've already checked out
[954.10 → 954.70] Unpaid before.
[955.12 → 955.60] And if you're ready
[955.60 → 956.60] to get started on a project,
[957.18 → 958.58] take advantage of the data security
[958.58 → 959.00] it offers.
[959.48 → 960.00] Support the show
[960.00 → 961.44] by going to unraid.net
[961.44 → 962.90] slash self-hosted.
[963.30 → 964.40] That's unraid.net
[964.40 → 965.88] slash self-hosted.
[967.60 → 968.58] Because I was buying
[968.58 → 969.88] a CPU cooler as well,
[969.96 → 971.22] which, by the way,
[971.34 → 973.42] Micro Centre carry a CPU cooler
[973.42 → 974.72] in stock
[974.72 → 977.24] to go with a random esoteric
[977.24 → 978.54] Thread ripper Pro CPU.
[979.22 → 981.06] Like, they are just god tier
[981.06 → 981.76] as a store.
[981.96 → 982.88] I mean, if you've never been
[982.88 → 983.64] to a Micro Centre,
[983.82 → 984.84] it's just like,
[985.62 → 986.52] for someone like me,
[986.58 → 987.32] it's like going to
[987.32 → 988.68] Willy Wonka's Chocolate Factory.
[988.84 → 990.58] They've got 3D printers
[990.58 → 992.04] out on the shop floor running.
[992.38 → 995.38] They've got Unify switches
[995.38 → 996.62] and Wi-Fi access points
[996.62 → 998.34] you can literally buy in the store.
[998.82 → 1000.96] They've got all of their PC cases out
[1000.96 → 1002.42] and you can literally look at them
[1002.42 → 1003.20] outside the packaging
[1003.20 → 1003.68] and be like,
[1004.06 → 1005.50] huh, I don't like the way
[1005.50 → 1006.56] that that thumbscrew,
[1007.04 → 1007.20] whatever,
[1007.28 → 1007.92] you can touch it
[1007.92 → 1009.36] and feel it
[1009.36 → 1010.98] and see it in 3D space.
[1011.38 → 1012.34] So you're making me jealous.
[1012.58 → 1013.74] We don't have one in Washington.
[1013.94 → 1015.42] Oh, if you ever get the chance,
[1015.50 → 1016.54] if you're ever in the neighbourhood
[1016.54 → 1017.32] of a Micro Centre,
[1017.94 → 1019.34] it's well worth going.
[1019.76 → 1022.06] It's just great.
[1022.12 → 1022.96] It was a great experience.
[1023.44 → 1023.68] But anyway,
[1023.88 → 1025.32] the sales associate
[1025.32 → 1026.16] that I spoke to
[1026.16 → 1026.54] was like,
[1027.10 → 1028.58] you're buying most of the parts
[1028.58 → 1030.20] for a build here.
[1030.24 → 1031.12] Because I also picked up
[1031.12 → 1032.36] a new power supply
[1032.36 → 1033.00] because I'm like,
[1033.06 → 1033.32] well,
[1033.94 → 1034.86] the Threadrepper Pro
[1034.86 → 1036.98] can pull a bit of extra juice
[1036.98 → 1038.22] compared to that Epic chip.
[1038.32 → 1039.78] So I upgraded from an 850
[1039.78 → 1041.26] to a 1200 watt power supply
[1041.26 → 1042.16] in the process too.
[1042.88 → 1043.30] And he was like,
[1043.34 → 1043.48] right,
[1043.54 → 1044.42] so you're buying a cooler,
[1044.62 → 1045.32] a power supply,
[1045.46 → 1046.52] a motherboard and a CPU.
[1047.06 → 1047.78] That's basically
[1047.78 → 1048.62] most of a build,
[1048.70 → 1048.96] isn't it?
[1048.96 → 1050.08] So he called his manager over
[1050.08 → 1050.48] and was like,
[1050.62 → 1051.68] can we sell this guy
[1051.68 → 1052.62] the desktop plan?
[1053.52 → 1054.34] And I'm like,
[1054.52 → 1055.60] what's the desktop plan?
[1056.78 → 1058.24] From Putty in his hand
[1058.24 → 1058.76] at this point.
[1059.32 → 1059.94] And he goes,
[1060.02 → 1060.16] well,
[1060.20 → 1060.96] if you wanted to cover
[1060.96 → 1061.86] just the motherboard
[1061.86 → 1062.16] for,
[1062.36 → 1064.84] I think it was three years,
[1065.20 → 1066.88] it's like $270.
[1067.60 → 1068.20] And I'm like,
[1068.28 → 1069.82] not interested.
[1070.56 → 1071.02] And then he goes,
[1071.08 → 1071.22] well,
[1071.28 → 1072.36] on the desktop plan,
[1072.72 → 1073.44] and this would cover
[1073.44 → 1074.72] everything you're buying here,
[1074.84 → 1075.50] not anything,
[1075.62 → 1075.84] you know,
[1075.88 → 1076.58] that you already have,
[1076.64 → 1077.30] but anything you buy
[1077.30 → 1078.06] from us today
[1078.06 → 1081.42] is 300, and I think
[1081.42 → 1082.86] $350 or something.
[1082.92 → 1083.32] And I'm like,
[1083.72 → 1084.68] all right,
[1084.88 → 1085.16] okay,
[1085.22 → 1085.34] well,
[1085.38 → 1086.22] tell me what does it cover?
[1087.08 → 1087.60] And apparently,
[1087.60 → 1089.50] it covers accidental damage.
[1089.90 → 1093.32] It covers manufacturing defects.
[1093.66 → 1095.00] It covers literally everything
[1095.00 → 1095.98] that could go wrong with it,
[1096.02 → 1096.48] bar theft,
[1096.54 → 1096.88] I think.
[1098.14 → 1099.96] And so to claim on this thing,
[1100.02 → 1101.06] all you do is take it back
[1101.06 → 1101.60] to the store,
[1101.68 → 1101.90] which,
[1102.52 → 1102.76] you know,
[1102.80 → 1103.16] for me,
[1103.32 → 1104.50] microcentre's two and a half hours
[1104.50 → 1105.10] down the road.
[1105.26 → 1105.44] Okay,
[1105.48 → 1106.30] that kind of sucks,
[1106.42 → 1107.56] but it could be worse.
[1108.40 → 1108.84] And he said,
[1108.90 → 1109.06] well,
[1109.14 → 1110.42] so let's say hypothetically
[1110.42 → 1111.46] in two and a half years,
[1111.88 → 1113.14] something happens
[1113.14 → 1114.62] and you bend a pin in the socket
[1114.62 → 1116.12] or one of the RAM slots
[1116.12 → 1116.76] stopped working
[1116.76 → 1117.26] or whatever.
[1117.60 → 1119.60] you can bring it back to us,
[1119.90 → 1120.78] anything that you've bought
[1120.78 → 1121.34] on the table
[1121.34 → 1123.72] and we'll give you store credit
[1123.72 → 1124.94] for the full value
[1124.94 → 1126.18] of what you've paid today,
[1126.20 → 1127.68] not what it would be worth,
[1127.82 → 1127.98] you know,
[1128.00 → 1129.18] if you resold it or whatever.
[1130.14 → 1130.86] So I'm like,
[1131.06 → 1131.28] oh,
[1131.94 → 1132.22] okay,
[1132.26 → 1132.36] well,
[1132.38 → 1133.16] that seems actually like
[1133.16 → 1133.92] quite a worthwhile
[1133.92 → 1134.82] insurance policy.
[1135.52 → 1135.54] Yeah,
[1135.56 → 1136.02] I could see it,
[1136.08 → 1137.02] especially after the experience
[1137.02 → 1137.68] you just went through,
[1137.90 → 1138.14] right?
[1138.54 → 1138.90] Yeah,
[1139.14 → 1140.40] I'm still bruised
[1140.40 → 1141.56] and he's offering me a way out.
[1141.64 → 1141.86] I'm like,
[1142.08 → 1144.66] do you sell this for eBay purchases too?
[1145.50 → 1145.80] Well,
[1145.86 → 1146.36] and like if something,
[1146.46 → 1147.62] not that it's likely to,
[1147.70 → 1149.02] but if something did go wrong,
[1149.06 → 1149.24] you're like,
[1149.26 → 1149.34] well,
[1149.34 → 1151.24] then I'm at another two grand again.
[1153.88 → 1154.20] Well,
[1154.30 → 1154.52] I'm not,
[1154.52 → 1155.22] I'm not suggesting
[1155.22 → 1156.12] I'm actually going to do this,
[1156.18 → 1157.12] but it'd be an awful shame
[1157.12 → 1157.80] if that motherboard
[1157.80 → 1158.38] stopped working
[1158.38 → 1159.22] in two and a half years,
[1159.26 → 1159.64] wouldn't it?
[1159.84 → 1160.20] Yeah,
[1160.40 → 1161.36] something just happens.
[1161.58 → 1161.78] Just,
[1161.96 → 1162.22] you know,
[1162.30 → 1162.82] I don't know,
[1163.30 → 1164.42] pipe burst or something.
[1164.50 → 1164.62] God,
[1164.66 → 1165.38] that would be awful.
[1166.04 → 1166.24] Yeah,
[1166.36 → 1167.68] probably design defect
[1167.68 → 1168.84] just caught up with it eventually.
[1169.22 → 1169.54] So,
[1170.00 → 1170.28] I,
[1170.42 → 1172.12] I purchased all this stuff
[1172.12 → 1173.40] and I didn't fancy driving
[1173.40 → 1174.78] all the way back to Raleigh
[1174.78 → 1176.28] just to find out
[1176.28 → 1177.74] that something was DOA.
[1178.56 → 1178.96] So,
[1179.42 → 1179.76] me,
[1179.94 → 1180.24] wife,
[1180.40 → 1180.64] kid,
[1180.84 → 1181.12] we,
[1181.18 → 1183.42] we made a weekend trip out of it.
[1183.50 → 1184.82] Ella got a hotel sleepover
[1184.82 → 1187.02] and then Catherine and me,
[1187.32 → 1188.50] we sat in the other half
[1188.50 → 1189.14] of the hotel room
[1189.14 → 1189.98] because we got one of those
[1189.98 → 1191.10] that has like two rooms,
[1191.20 → 1192.66] like a Hilton Home 2 or something.
[1193.22 → 1193.38] Oh,
[1193.42 → 1193.66] nice.
[1193.90 → 1194.34] And,
[1194.68 → 1196.38] I built the computer
[1196.38 → 1197.34] in the hotel room.
[1197.34 → 1199.24] You know what?
[1199.30 → 1200.38] That's not a bad idea.
[1200.44 → 1201.58] I never would have thought of that.
[1201.96 → 1202.60] Would you imagine?
[1202.76 → 1202.92] Yeah,
[1202.96 → 1203.84] like if you had gotten home
[1203.84 → 1204.58] and it didn't work?
[1204.74 → 1205.06] Yeah,
[1205.06 → 1206.00] I would have been pissed.
[1206.34 → 1206.50] Yeah,
[1206.58 → 1207.86] but the best part was
[1207.86 → 1209.00] I had my old server
[1209.00 → 1209.68] in a suitcase.
[1210.62 → 1210.92] Ah,
[1210.92 → 1211.32] ah,
[1211.66 → 1213.62] walking past the check-in desk
[1213.62 → 1215.20] with this massive suitcase
[1215.20 → 1216.14] full of a server.
[1216.66 → 1217.74] They think it's closed
[1217.74 → 1218.36] and you're on a trip.
[1218.56 → 1218.78] Right,
[1218.90 → 1219.64] and then I just,
[1219.78 → 1220.08] you know,
[1220.30 → 1221.24] get to my hotel room
[1221.24 → 1222.96] and I whip out this epic server
[1222.96 → 1223.22] with,
[1223.38 → 1223.50] you know,
[1223.60 → 1224.90] because I could just reuse the RAM
[1224.90 → 1225.20] and what have you.
[1225.20 → 1225.30] So,
[1225.38 → 1226.30] you brought like screens
[1226.30 → 1226.90] and keyboards
[1226.90 → 1227.34] and everything?
[1227.58 → 1227.68] No,
[1227.84 → 1228.02] no,
[1228.12 → 1228.30] no,
[1228.44 → 1229.34] you see,
[1229.54 → 1230.66] this is where it gets interesting.
[1231.12 → 1231.42] Uh-huh.
[1231.54 → 1233.48] I have an HDMI capture device
[1233.48 → 1234.42] over USB-C,
[1234.50 → 1234.80] don't I?
[1235.10 → 1235.92] For all the recordings
[1235.92 → 1236.68] I do for work.
[1236.84 → 1237.02] Sure,
[1237.12 → 1237.28] sure.
[1237.28 → 1237.30] So,
[1237.30 → 1237.38] I just,
[1237.38 → 1239.32] just brought my Cam Link 4K
[1239.32 → 1240.04] and used that.
[1240.04 → 1241.24] And just used a laptop screen
[1241.24 → 1242.38] as like a pass-through screen.
[1242.48 → 1242.60] Yeah,
[1242.64 → 1243.16] with OBS,
[1243.24 → 1243.40] yeah.
[1243.66 → 1243.82] Yeah.
[1246.16 → 1247.08] And he thinks you don't have
[1247.08 → 1247.90] to pack a screen,
[1247.98 → 1248.18] right?
[1249.82 → 1250.42] I mean,
[1251.30 → 1253.94] I mean,
[1254.02 → 1254.88] if it works,
[1254.94 → 1255.58] it ain't stupid,
[1255.70 → 1255.90] right?
[1256.90 → 1257.34] Obviously,
[1257.62 → 1258.20] you got it done.
[1258.58 → 1258.78] So,
[1258.82 → 1259.30] there we go.
[1259.78 → 1260.14] Currently,
[1260.24 → 1260.62] the server,
[1260.74 → 1261.90] I haven't actually touched it
[1261.90 → 1262.62] since we got home.
[1262.74 → 1262.90] It's,
[1262.96 → 1263.64] as we record,
[1264.02 → 1264.80] it's Monday evening,
[1264.80 → 1266.24] we got back yesterday on Sunday
[1266.24 → 1268.64] and I've just been so busy
[1268.64 → 1269.20] at work today.
[1269.28 → 1269.40] Like,
[1269.42 → 1270.64] I want to record a video
[1270.64 → 1271.96] of actually swapping the guts
[1271.96 → 1273.00] over and all the rest of it
[1273.00 → 1275.34] for my YouTube channel
[1275.34 → 1276.66] and I just haven't gotten to it yet.
[1276.80 → 1276.94] So,
[1277.34 → 1277.64] currently,
[1277.86 → 1279.16] I dashed all the way to Charlotte
[1279.16 → 1281.34] to get it over the weekend
[1281.34 → 1283.22] whilst I had a window of time
[1283.22 → 1284.18] before we go to scale
[1284.18 → 1285.10] and all the rest of it
[1285.10 → 1287.10] and it's still sat there
[1287.10 → 1287.58] and I haven't really,
[1287.92 → 1288.06] I mean,
[1288.16 → 1290.52] it posted in the hotel room
[1290.52 → 1291.04] successfully.
[1291.50 → 1291.88] So,
[1291.98 → 1292.96] I know it works
[1292.96 → 1294.94] but currently,
[1295.06 → 1295.82] the server's offline
[1295.82 → 1296.46] still.
[1296.46 → 1299.28] tailscale.com
[1299.28 → 1299.90] slash
[1299.90 → 1301.08] self-hosted.
[1301.16 → 1302.02] You have to go there,
[1302.10 → 1302.54] check it out,
[1302.62 → 1303.18] support the show
[1303.18 → 1303.84] and get it for free
[1303.84 → 1305.10] for up to 100 devices,
[1306.08 → 1306.78] three users
[1306.78 → 1308.78] and no credit card required.
[1309.18 → 1310.60] Tail scale is modern networking
[1310.60 → 1311.94] that connects your devices
[1311.94 → 1312.94] and your applications
[1312.94 → 1314.08] directly to each other.
[1314.34 → 1315.12] It's great for companies
[1315.12 → 1315.94] and it is great
[1315.94 → 1317.34] for self-hosted as well.
[1317.60 → 1319.06] I'm talking secure remote access
[1319.06 → 1320.14] to whatever it might be
[1320.14 → 1320.94] that you need
[1320.94 → 1322.22] and it's really fast
[1322.22 → 1323.82] and it's protected by WireGuard.
[1323.82 → 1325.50] When I'm travelling
[1325.50 → 1327.46] and I bring tail scale with me,
[1327.68 → 1328.60] it's like I bring
[1328.60 → 1329.96] my entire LAN with me.
[1330.20 → 1331.22] I've preloaded
[1331.22 → 1332.88] a little Apple TV set-top box
[1332.88 → 1334.12] that has a fantastic
[1334.12 → 1334.94] tail scale app
[1334.94 → 1336.26] that's connected
[1336.26 → 1336.98] to my tail net
[1336.98 → 1338.14] and when I get
[1338.14 → 1338.90] to the Airbnb,
[1339.40 → 1340.32] I'm going to plug it
[1340.32 → 1341.26] into the HDMI port
[1341.26 → 1341.78] on the TV,
[1342.02 → 1343.24] power up the Apple TV
[1343.24 → 1344.56] and I'll be streaming
[1344.56 → 1345.66] everything just like
[1345.66 → 1346.84] it was in my living room.
[1347.06 → 1348.48] Literally like the Apple TV
[1348.48 → 1350.68] was in my living room
[1350.68 → 1351.48] and I'm going to be
[1351.48 → 1351.90] in an Airbnb
[1351.90 → 1352.76] in California.
[1353.32 → 1354.68] I'm talking easy deploy,
[1354.84 → 1356.08] I'm talking zero config,
[1356.28 → 1357.82] I'm talking no fuss VPN
[1357.82 → 1359.44] that puts all your nodes
[1359.44 → 1360.74] on a flat mesh network
[1360.74 → 1361.58] and then you have
[1361.58 → 1362.46] the power to control that
[1362.46 → 1363.68] with things like ACLs
[1363.68 → 1364.82] and user authorization
[1364.82 → 1365.78] and you can tie it in
[1365.78 → 1366.34] with your corporate
[1366.34 → 1368.04] authorization system as well.
[1368.66 → 1369.76] You have to play with this
[1369.76 → 1370.94] because it will change your game.
[1371.04 → 1371.72] I literally have
[1371.72 → 1372.68] no inbound ports
[1372.68 → 1374.04] on any of our production
[1374.04 → 1374.88] corporate systems
[1374.88 → 1376.42] or my personal systems.
[1377.00 → 1377.54] It's the way
[1377.54 → 1378.34] it really should be
[1378.34 → 1379.52] and when you go
[1379.52 → 1380.62] to tailscale.com
[1380.62 → 1381.70] slash self-hosted
[1381.70 → 1383.38] you get the 100 devices
[1383.38 → 1384.14] for free forever
[1384.14 → 1384.90] for three users.
[1385.38 → 1386.24] You can take it further
[1386.24 → 1386.78] if you want
[1386.78 → 1387.42] but you might find
[1387.42 → 1388.14] that's a great plan
[1388.14 → 1388.68] just for you
[1388.68 → 1390.34] and thousands of companies
[1390.34 → 1391.12] like Instacart,
[1391.46 → 1392.06] Hugging Face,
[1392.42 → 1392.86] Duolingo,
[1393.26 → 1394.28] and Jupyter Broadcasting
[1394.28 → 1395.30] have switched to using
[1395.30 → 1396.26] Tail scale as well.
[1396.60 → 1397.28] Business plans,
[1397.46 → 1398.02] personal plans,
[1398.12 → 1398.72] and that free
[1398.72 → 1399.72] 100 device plan.
[1400.38 → 1401.10] All you have to do
[1401.10 → 1401.64] is gone to
[1401.64 → 1402.80] tailscale.com
[1402.80 → 1403.66] slash self-hosted.
[1403.98 → 1404.62] Go see why
[1404.62 → 1405.56] I've been raving about it.
[1405.66 → 1406.14] I love it
[1406.14 → 1406.80] and it's changed
[1406.80 → 1407.74] how I do networking.
[1407.74 → 1409.12] Much, much better.
[1409.54 → 1410.44] tailscale.com
[1410.44 → 1411.90] slash self-hosted.
[1413.26 → 1414.32] You seem to be
[1414.32 → 1415.52] on a crusade
[1415.52 → 1416.78] for sensors
[1416.78 → 1418.60] and smart home upgrades.
[1418.70 → 1419.48] What's driving this
[1419.48 → 1420.20] at the minute for you?
[1420.96 → 1421.24] You know,
[1421.30 → 1421.78] this winter
[1421.78 → 1422.58] I decided to get
[1422.58 → 1423.24] a diesel heater.
[1423.38 → 1423.44] Well,
[1423.50 → 1425.14] I finally got it installed.
[1426.10 → 1427.26] They're wonderful machines,
[1427.36 → 1427.68] actually,
[1428.20 → 1429.80] and they produce
[1429.80 → 1430.86] an incredible amount of heat.
[1431.62 → 1431.96] But, you know,
[1431.98 → 1432.60] I always thought,
[1433.28 → 1433.50] well,
[1433.60 → 1434.32] if this thing's,
[1434.32 → 1434.70] you know,
[1434.72 → 1435.90] got a combustion chamber,
[1435.90 → 1437.16] is there a possibility
[1437.16 → 1438.32] of CO2 leakage
[1438.32 → 1439.20] or something like that?
[1439.94 → 1441.24] And we also use propane
[1441.24 → 1441.58] to cook.
[1441.72 → 1441.84] You know,
[1441.84 → 1442.40] we have a propane
[1442.40 → 1442.96] stove top.
[1443.92 → 1444.58] And I've always wanted
[1444.58 → 1445.36] to kind of keep an eye
[1445.36 → 1445.76] on this.
[1445.84 → 1446.64] And I have a lot
[1446.64 → 1448.48] of these Z-Wave sensors
[1448.48 → 1449.12] throughout the house,
[1449.18 → 1449.82] but the one thing
[1449.82 → 1450.64] they don't do
[1450.64 → 1452.92] is CO2 detection.
[1453.08 → 1453.58] They do, like,
[1453.84 → 1454.54] everything else,
[1454.64 → 1456.00] but they don't do CO2.
[1456.52 → 1457.34] And when you look
[1457.34 → 1458.68] into specific CO2 sensors,
[1458.74 → 1459.22] and we'll talk about
[1459.22 → 1460.02] some more options
[1460.02 → 1460.94] in a little bit,
[1461.70 → 1462.68] you know,
[1462.70 → 1463.74] they can range from
[1463.74 → 1464.48] you build it
[1464.48 → 1466.04] with an ESP yourself
[1466.04 → 1468.12] for $10, $15 tops
[1468.12 → 1471.24] to $120, $130 devices,
[1471.36 → 1471.78] depending on what
[1471.78 → 1472.34] you look at.
[1474.14 → 1475.16] And so I was looking
[1475.16 → 1475.64] for something
[1475.64 → 1476.48] that was pre-built,
[1477.62 → 1478.68] and something I could
[1478.68 → 1479.58] buy a few of
[1479.58 → 1480.62] so it wouldn't
[1480.62 → 1481.32] break the bank.
[1482.84 → 1483.84] And I ended up
[1483.84 → 1484.96] getting one of these
[1484.96 → 1486.04] First Alert Z-Wave
[1486.04 → 1486.84] smoke detectors
[1486.84 → 1488.86] that is just a
[1488.86 → 1490.38] really rather
[1490.38 → 1492.22] innocuous-looking
[1492.22 → 1492.96] smoke detector.
[1492.96 → 1493.74] You could put it up
[1493.74 → 1494.22] on your wall
[1494.22 → 1495.10] and never use
[1495.10 → 1496.22] any of the smart features,
[1496.40 → 1497.98] and it has a great
[1497.98 → 1499.58] CO2 sensor built into it.
[1499.88 → 1501.10] $40 right off Amazon.
[1501.62 → 1501.88] I mean,
[1502.02 → 1502.68] I'm looking at the
[1502.68 → 1503.50] packaging for this thing.
[1503.90 → 1504.82] If this was on the
[1504.82 → 1505.62] shelf at Home Depot,
[1505.78 → 1506.54] I wouldn't be
[1506.54 → 1507.84] any the wiser
[1507.84 → 1508.92] that it had Z-Wave in it.
[1509.12 → 1509.26] No.
[1509.52 → 1510.66] And you'd never have
[1510.66 → 1511.04] to hook it up
[1511.04 → 1511.88] if you don't want to.
[1512.02 → 1512.80] It just looks like
[1512.80 → 1513.58] a bog-standard
[1513.58 → 1514.24] smoke detector.
[1514.88 → 1515.08] Yeah.
[1515.26 → 1515.60] Nice.
[1516.24 → 1517.34] And what is great
[1517.34 → 1518.30] is when you do
[1518.30 → 1519.54] connect it over Z-Wave,
[1519.70 → 1520.14] Home Assistant
[1520.14 → 1520.94] picks it right up
[1520.94 → 1521.74] when you put the thing
[1521.74 → 1522.44] in pairing mode,
[1522.60 → 1524.26] and all the
[1524.26 → 1524.86] sensor data
[1524.86 → 1526.06] now comes into
[1526.06 → 1526.60] Home Assistant,
[1526.98 → 1528.02] which is great
[1528.02 → 1528.42] because,
[1528.92 → 1529.62] you know,
[1529.66 → 1530.32] then you can do
[1530.32 → 1531.04] things like
[1531.04 → 1532.24] generate alerts
[1532.24 → 1533.86] because perhaps
[1533.86 → 1534.72] there's a CO2 leak
[1534.72 → 1535.42] when I'm not home.
[1535.68 → 1536.46] Very possible.
[1537.84 → 1538.72] Or, you know,
[1539.16 → 1540.08] maybe I'm out in the yard
[1540.08 → 1540.88] or something like that.
[1541.14 → 1541.92] So I wanted
[1541.92 → 1543.64] a way to notify myself
[1543.64 → 1544.58] when there was a CO2 leak,
[1544.62 → 1545.28] and that's why I wanted
[1545.28 → 1546.24] it to be on Z-Wave
[1546.24 → 1546.62] so that way
[1546.62 → 1547.84] I could get notifications
[1547.84 → 1548.92] and be aware of it
[1548.92 → 1549.68] even when I'm not there.
[1549.68 → 1551.56] So how does Z-Wave work?
[1551.66 → 1553.88] This is a battery-powered device,
[1554.02 → 1554.18] right?
[1554.42 → 1555.22] Does it work
[1555.22 → 1556.04] similarly
[1556.04 → 1557.60] to Zigbee
[1557.60 → 1558.52] where it's a mesh
[1558.52 → 1559.28] that has, like,
[1559.46 → 1560.60] routers and repeaters
[1560.60 → 1563.10] with hard line wire,
[1563.22 → 1563.46] like,
[1564.16 → 1565.26] light switches and stuff?
[1565.36 → 1565.54] Like,
[1565.70 → 1566.32] how does that work?
[1567.18 → 1567.68] I'm not sure
[1567.68 → 1569.32] about the exact architecture.
[1569.64 → 1570.20] I do think
[1570.20 → 1571.78] you have similar setup
[1571.78 → 1572.60] where you have, like,
[1572.92 → 1574.44] AC devices on Z-Wave
[1574.44 → 1576.40] are essentially repeaters
[1576.40 → 1577.40] and strengthen the network
[1577.40 → 1579.34] and then battery devices.
[1579.72 → 1581.12] They're generally more consumers
[1581.12 → 1582.08] of the Z-Wave network,
[1582.08 → 1583.04] and this is just
[1583.04 → 1583.92] AA batteries.
[1584.52 → 1585.34] And it does say
[1585.34 → 1586.06] it'll last a year.
[1586.14 → 1586.52] We'll see.
[1587.52 → 1587.92] Thankfully,
[1588.10 → 1588.92] the battery status
[1588.92 → 1590.08] and low warning level
[1590.08 → 1590.90] also comes through
[1590.90 → 1591.48] to Home Assistant.
[1591.90 → 1592.14] Nice.
[1592.30 → 1592.76] That's what you mean.
[1592.76 → 1592.84] Yeah,
[1593.26 → 1593.78] that is.
[1594.38 → 1595.58] So the nice thing
[1595.58 → 1596.66] I think about Z-Wave
[1596.66 → 1597.48] is that it's,
[1597.48 → 1598.66] just in my experience,
[1599.50 → 1600.26] been really,
[1600.38 → 1601.32] really rock solid, right?
[1601.34 → 1602.78] It's running at 900 megahertz.
[1602.96 → 1604.06] I don't really have anything else
[1604.06 → 1605.42] running at 900 megahertz,
[1605.42 → 1607.26] and it just has been
[1607.26 → 1608.04] the absolute,
[1608.24 → 1608.44] like,
[1608.52 → 1609.20] most reliable.
[1609.28 → 1610.36] I use it to control
[1610.36 → 1611.86] all of my heating,
[1612.36 → 1613.00] even the stuff
[1613.00 → 1613.98] that's down in my water bays
[1613.98 → 1614.86] that prevents our water
[1614.86 → 1615.42] from freezing
[1615.42 → 1616.34] all through winter.
[1616.50 → 1617.76] I trust that to Z-Wave
[1617.76 → 1619.14] and it's been rock solid.
[1619.68 → 1620.94] So I felt pretty good.
[1621.00 → 1621.14] Plus,
[1621.20 → 1621.80] this thing also
[1621.80 → 1622.80] obviously makes
[1622.80 → 1624.80] a blaring,
[1625.02 → 1625.48] audible,
[1626.12 → 1628.08] 85 dB alarm.
[1628.48 → 1629.38] It has a built-in,
[1629.50 → 1630.30] it's a smoke detector,
[1630.46 → 1630.66] you know,
[1630.70 → 1632.08] so it'll also beep itself.
[1632.08 → 1632.60] Right,
[1632.72 → 1634.10] you'd hope it would make a fuss
[1634.10 → 1636.26] when S hits the fan,
[1636.46 → 1636.82] so to speak.
[1636.86 → 1637.00] Yeah.
[1637.56 → 1638.78] I thought not good enough,
[1638.84 → 1639.00] though.
[1639.44 → 1640.50] I wanted a system
[1640.50 → 1641.36] that would escalate.
[1641.40 → 1642.32] So the first thing that happens
[1642.32 → 1643.14] when the smoke detector
[1643.14 → 1643.60] gets triggered,
[1643.68 → 1644.84] either smoke or CO2,
[1646.02 → 1647.40] push notifications go out.
[1647.50 → 1647.66] Like,
[1647.70 → 1648.26] that happens
[1648.26 → 1649.54] to any of my devices
[1649.54 → 1650.62] that have the Home Assistant app.
[1650.78 → 1651.90] Push notification goes out.
[1652.92 → 1653.80] After a minute,
[1654.32 → 1656.66] if the alarm isn't silenced,
[1657.24 → 1658.72] I then trigger
[1658.72 → 1659.82] all the sirens
[1659.82 → 1661.18] in Lady Joop's.
[1661.70 → 1663.34] And every Waze camera,
[1663.50 → 1664.96] every ring stick-up camera
[1664.96 → 1666.92] has a siren built into it.
[1667.22 → 1668.14] So it makes
[1668.14 → 1669.54] a real ruckus
[1669.54 → 1670.10] because, you know,
[1670.18 → 1670.62] collectively,
[1670.80 → 1671.38] there's like eight
[1671.38 → 1672.36] of these things all together.
[1673.18 → 1674.04] And Home Assistant
[1674.04 → 1675.22] can fire all those off.
[1675.96 → 1676.54] And then,
[1676.90 → 1679.84] because why not,
[1680.08 → 1681.24] I went all the way
[1681.24 → 1681.92] and I went and got
[1681.92 → 1682.68] a 100 dB,
[1683.36 → 1684.58] this is a Zigbee siren,
[1685.00 → 1685.70] it just plugs
[1685.70 → 1686.84] right into an AC outlet
[1686.84 → 1688.92] and it just has
[1688.92 → 1690.54] nothing but noise.
[1690.64 → 1690.78] Like,
[1690.82 → 1692.72] it just blasts
[1692.72 → 1693.10] different,
[1693.18 → 1693.94] eight different types
[1693.94 → 1694.42] of alarms.
[1695.06 → 1696.52] And this I have
[1696.52 → 1697.60] on the outside
[1697.60 → 1698.54] of Lady Joop's.
[1698.96 → 1699.76] And the idea is
[1699.76 → 1701.12] that after a period of time,
[1701.68 → 1702.74] if there is some sort
[1702.74 → 1703.90] of emergency situation
[1703.90 → 1704.78] inside the RV
[1704.78 → 1706.80] and nobody has taken action
[1706.80 → 1707.22] to say,
[1707.30 → 1708.48] situation under control,
[1708.72 → 1709.74] it starts blaring
[1709.74 → 1710.70] the outside siren
[1710.70 → 1711.10] because,
[1711.52 → 1711.92] honestly,
[1712.02 → 1712.80] if there's a fire
[1712.80 → 1714.14] or something like that,
[1714.52 → 1715.80] maybe a battery situation,
[1715.80 → 1716.90] people need to get away
[1716.90 → 1717.58] from the RV.
[1718.64 → 1720.12] So I want them to know,
[1720.44 → 1720.66] hey,
[1720.72 → 1721.70] there's a situation here.
[1721.76 → 1722.56] So I have one
[1722.56 → 1723.76] in an outside bay
[1723.76 → 1725.26] that will blare
[1725.26 → 1726.66] after a period of time
[1726.66 → 1727.42] outside as well.
[1727.46 → 1728.56] And I can also trigger that
[1728.56 → 1729.20] anytime I want,
[1729.48 → 1729.72] you know,
[1729.74 → 1730.84] right now I could trigger it.
[1730.92 → 1731.04] So,
[1731.86 → 1732.02] you know,
[1732.02 → 1733.22] if I got a notification
[1733.22 → 1734.56] someone's creeping on the RV,
[1734.66 → 1735.48] I could fire that sucker
[1735.48 → 1736.16] off right now.
[1736.16 → 1736.94] Or if I needed to get
[1736.94 → 1737.68] the kids' attention
[1737.68 → 1738.34] and they're not answering
[1738.34 → 1738.94] the damn phone.
[1739.98 → 1740.60] I've got an idea
[1740.60 → 1741.86] for an extension activity
[1741.86 → 1743.66] for this escalation
[1743.66 → 1744.84] of alarms for you.
[1745.42 → 1745.62] Yeah.
[1745.80 → 1746.16] Well,
[1746.24 → 1747.94] when the external one triggers,
[1748.04 → 1748.94] you should probably also
[1748.94 → 1750.32] allow Levi to leave
[1750.32 → 1751.18] the building too,
[1751.36 → 1751.64] somehow.
[1752.16 → 1752.66] You're right.
[1752.90 → 1753.56] Pop the door,
[1753.82 → 1754.04] Levi,
[1754.20 → 1754.48] exit.
[1754.66 → 1755.30] Something like that,
[1755.32 → 1755.52] yeah.
[1755.78 → 1756.08] Mm-hmm.
[1756.72 → 1758.24] I need a Levi detection sensor.
[1758.82 → 1759.74] So I will link
[1759.74 → 1760.80] a couple of sirens,
[1761.40 → 1762.30] the cheap one,
[1762.38 → 1762.92] and then there's like
[1762.92 → 1763.78] an $80 one.
[1763.90 → 1765.24] The $80 one is nice
[1765.24 → 1767.96] because it has a whole
[1767.96 → 1769.24] bunch of more tonal range.
[1769.36 → 1770.36] So you could also use it
[1770.36 → 1770.92] as just like
[1770.92 → 1772.14] a moderately
[1772.14 → 1774.52] nice sounding doorbell
[1774.52 → 1775.44] that isn't crazy loud.
[1775.56 → 1775.92] Like you could,
[1776.50 → 1777.28] anything you can plug
[1777.28 → 1777.96] into Home Assistant,
[1778.20 → 1779.12] you could have this thing
[1779.12 → 1780.46] ping different noises.
[1780.88 → 1782.42] It also has a built-in battery.
[1782.86 → 1784.28] So if you lose AC power,
[1784.36 → 1784.94] this thing can run
[1784.94 → 1785.44] for a while,
[1785.52 → 1786.20] for four hours,
[1786.40 → 1787.72] which is kind of nice.
[1787.84 → 1788.48] That's pretty good.
[1789.08 → 1789.24] Yeah.
[1789.62 → 1790.06] And it's,
[1790.26 → 1790.58] you know,
[1790.62 → 1791.22] having sirens
[1791.22 → 1792.16] has been kind of nice,
[1792.22 → 1793.00] but tying it into the
[1793.00 → 1793.66] smoke detector
[1793.66 → 1794.64] and CO2 detector,
[1794.76 → 1795.56] I feel like was,
[1796.22 → 1796.58] was,
[1796.68 → 1797.82] was probably
[1797.82 → 1799.58] an obvious next step,
[1799.62 → 1800.12] but something that
[1800.12 → 1801.00] I just had not connected.
[1801.00 → 1802.94] And the one thing
[1802.94 → 1803.52] I couldn't
[1803.52 → 1805.54] really nail,
[1806.28 → 1806.94] and maybe you know,
[1806.98 → 1808.18] or maybe people listening know,
[1808.32 → 1811.10] is I looked up ways
[1811.10 → 1811.34] to,
[1811.38 → 1812.64] to mark the notifications
[1812.64 → 1813.52] in Home Assistant
[1813.52 → 1814.56] as time critical.
[1814.56 → 1815.64] So that way it would bust
[1815.64 → 1816.80] through like a do not disturb
[1816.80 → 1817.64] both on Android
[1817.64 → 1818.36] and on iOS,
[1818.64 → 1819.52] different kind of
[1819.52 → 1820.42] like little things,
[1820.66 → 1821.12] you know,
[1821.14 → 1822.32] critical colon one
[1822.32 → 1822.94] is what you put in there
[1822.94 → 1824.06] for iOS or something like that.
[1824.36 → 1825.34] In the data field
[1825.34 → 1826.16] of the push notification,
[1826.16 → 1827.46] you can add these things,
[1828.00 → 1828.86] these little descriptors,
[1828.86 → 1829.82] and then supposedly
[1829.82 → 1831.04] supposed to tell the OS,
[1832.02 → 1833.72] this is a very urgent notification.
[1834.34 → 1834.36] Well,
[1834.38 → 1835.08] we talked about this
[1835.08 → 1835.56] a little bit
[1835.56 → 1836.74] in the last episode
[1836.74 → 1837.60] when we were using
[1837.60 → 1838.28] phone calls
[1838.28 → 1838.98] to break through
[1838.98 → 1840.04] do not disturb modes
[1840.04 → 1840.82] and all the rest of it.
[1841.48 → 1842.32] And Michael Hennessy
[1842.32 → 1843.30] actually wrote in saying,
[1843.40 → 1843.68] hey guys,
[1843.70 → 1844.62] I'm a long time listener.
[1845.10 → 1845.38] And Chris,
[1845.42 → 1845.94] I actually bought
[1845.94 → 1847.14] your old Synology off you
[1847.14 → 1848.04] a couple of years back.
[1848.14 → 1849.02] Still going strong.
[1849.12 → 1849.26] Oh,
[1849.30 → 1849.58] awesome.
[1850.06 → 1850.34] Good.
[1850.76 → 1851.08] He said,
[1851.12 → 1852.86] listening to the last episode,
[1853.32 → 1854.46] the guy who makes calls
[1854.46 → 1855.64] to bypass quiet mode,
[1855.72 → 1855.96] he goes,
[1855.96 → 1856.26] well,
[1856.34 → 1857.14] this is okay,
[1857.34 → 1858.96] but I use pushover.
[1859.82 → 1860.32] for this.
[1860.72 → 1862.34] It has different alert types
[1862.34 → 1863.58] as part of the notifications
[1863.58 → 1865.40] and the emergency alert
[1865.40 → 1866.94] can be set to make noise
[1866.94 → 1868.42] until you acknowledge it.
[1868.54 → 1869.44] It's really great.
[1869.64 → 1870.02] I like that.
[1870.18 → 1870.38] Okay.
[1870.52 → 1871.62] And I use it so much
[1871.62 → 1873.06] at work with the on-call team
[1873.06 → 1874.48] so they don't have any excuse
[1874.48 → 1875.70] for missing major alerts.
[1875.86 → 1876.78] Just my two cents.
[1877.46 → 1877.82] All right.
[1877.84 → 1878.62] I'm going to look into that.
[1879.28 → 1879.80] That seems like
[1879.80 → 1880.68] that could be the way to go
[1880.68 → 1882.72] because that's my one concern
[1882.72 → 1884.04] is that some sort of emergency
[1884.04 → 1884.84] is happening at home
[1884.84 → 1886.12] and I'm just sitting here
[1886.12 → 1886.30] with,
[1886.40 → 1887.44] because when I do a show,
[1887.44 → 1888.56] I always put it in,
[1888.86 → 1889.36] you know,
[1889.40 → 1890.16] do not disturb mode.
[1890.36 → 1891.30] So that would be pushover
[1891.30 → 1892.30] at pushover.net,
[1892.38 → 1892.80] I imagine,
[1893.06 → 1894.98] which is what I've used myself
[1894.98 → 1896.68] for like alerting
[1896.68 → 1898.66] all sorts of stuff for years.
[1898.72 → 1899.96] They've got a very generous free tier
[1899.96 → 1900.90] and I certainly used to.
[1901.42 → 1901.68] So yeah,
[1901.68 → 1902.28] take a look at it.
[1902.84 → 1903.84] I've definitely heard of it before.
[1903.96 → 1904.26] I will.
[1904.82 → 1906.00] So does all of this stuff
[1906.00 → 1907.86] natively work with Home Assistant then?
[1907.96 → 1909.22] Is it plug and play?
[1909.80 → 1910.60] That's what's great.
[1910.88 → 1911.02] Yeah,
[1911.04 → 1911.56] it all does.
[1911.76 → 1912.26] You don't even,
[1912.26 → 1913.22] you don't even need
[1913.22 → 1914.24] any kind of like hacks,
[1914.48 → 1915.30] special installation.
[1915.30 → 1915.78] Wonderful.
[1916.50 → 1916.70] Yeah,
[1916.76 → 1918.24] it all just plugs right in
[1918.24 → 1919.44] either using the Zigbee integration
[1919.44 → 1920.42] or the Z-Wave integration.
[1921.04 → 1922.28] And now I've been thinking,
[1923.40 → 1923.78] I've got,
[1923.84 → 1924.32] so I've got,
[1924.40 → 1925.82] I've got sensors everywhere.
[1925.94 → 1927.02] I've got cameras everywhere.
[1927.34 → 1928.72] I've got door sensors.
[1928.98 → 1929.98] I've got sirens.
[1931.02 → 1933.14] I have everything I need
[1933.14 → 1934.78] to have an alarm system.
[1935.08 → 1935.52] Oh,
[1935.60 → 1936.28] here we go.
[1936.68 → 1937.06] Right?
[1937.26 → 1937.40] Now,
[1937.40 → 1938.54] I don't know if this is a good idea
[1938.54 → 1939.00] or not,
[1939.12 → 1940.76] but I was looking at Alarm,
[1940.94 → 1943.26] which is an easy to use
[1943.26 → 1944.56] alarm system integration
[1944.56 → 1945.44] for Home Assistant.
[1946.56 → 1948.38] And it gives you a user interface
[1948.38 → 1950.24] for setting up your own alarm system
[1950.24 → 1952.10] completely right there
[1952.10 → 1953.44] in the Home Assistant dashboard.
[1954.80 → 1957.14] And it consists of three components.
[1957.28 → 1958.30] You have the Alarm component,
[1958.42 → 1959.82] which is the custom component
[1959.82 → 1960.54] that you have to install.
[1961.30 → 1962.62] You have the panel,
[1962.74 → 1963.26] which is a GUI
[1963.26 → 1964.28] for configuring the settings
[1964.28 → 1964.80] in your alarm,
[1964.94 → 1965.24] sensors,
[1965.38 → 1965.66] delays,
[1965.74 → 1966.34] and stuff like that.
[1966.34 → 1967.70] And then an Alarm card,
[1968.40 → 1969.64] which is a custom card
[1969.64 → 1970.82] you could put up like on a tablet
[1970.82 → 1971.42] or something,
[1971.92 → 1972.60] which is essentially
[1972.60 → 1973.52] for just arming
[1973.52 → 1974.48] and disarming the alarm
[1974.48 → 1976.24] like any kind of alarm pad would be.
[1976.96 → 1977.82] So that presupposes,
[1977.98 → 1978.60] I guess,
[1978.66 → 1980.98] that you've got some kind of keypad
[1980.98 → 1981.68] by the door.
[1981.78 → 1982.00] I mean,
[1982.18 → 1983.18] you've obviously got the
[1983.18 → 1984.86] Home Assistant Lovelace card,
[1984.98 → 1986.34] but could that link up
[1986.34 → 1987.32] with yet another piece
[1987.32 → 1988.58] of like physical hardware?
[1988.92 → 1988.98] Physical?
[1989.36 → 1989.62] Yeah,
[1989.66 → 1990.20] that'd be nice.
[1990.30 → 1991.28] Like a physical keypad.
[1991.78 → 1991.90] Yeah,
[1991.92 → 1992.08] maybe,
[1992.22 → 1992.72] I don't know,
[1993.00 → 1994.86] can you reach USB
[1994.86 → 1996.14] from your Home Assistant
[1996.14 → 1997.60] device from there?
[1998.22 → 1999.74] You can just put like a jumped
[1999.74 → 2000.22] by the door.
[2000.22 → 2000.48] Or blue,
[2000.48 → 2000.68] yeah,
[2000.78 → 2001.20] blue teeth,
[2001.32 → 2001.88] jumped maybe.
[2002.00 → 2002.66] Blue teeth.
[2003.12 → 2003.38] You know,
[2003.46 → 2004.10] that could work.
[2004.50 → 2004.70] Yeah.
[2005.62 → 2006.02] Also,
[2006.10 → 2007.40] it supports multiple users
[2007.40 → 2008.46] with individual pin codes
[2008.46 → 2009.08] so like the kids
[2009.08 → 2010.24] could have their own codes
[2010.24 → 2010.82] and stuff.
[2011.18 → 2011.78] Like that's,
[2011.90 → 2013.60] it's kind of everything I'd want,
[2013.96 → 2014.66] especially if,
[2014.96 → 2015.44] you know,
[2015.44 → 2017.14] if I get the urgent notification
[2017.14 → 2018.20] stuff worked out.
[2018.68 → 2019.48] I think get the kids
[2019.48 → 2020.50] to clock in and clock out
[2020.50 → 2021.38] as they do their chores,
[2021.50 → 2021.80] you know.
[2021.88 → 2022.16] Right.
[2022.32 → 2022.84] There you go.
[2023.20 → 2023.62] I'm sorry,
[2023.70 → 2023.86] Dylan,
[2023.94 → 2024.88] you were three minutes late.
[2025.10 → 2026.28] No iPad time for you,
[2026.36 → 2026.50] son.
[2027.18 → 2027.58] Also,
[2027.80 → 2029.20] it does support different zones.
[2029.34 → 2029.98] Like in the sense
[2029.98 → 2030.54] of the RV,
[2030.88 → 2031.82] you could see the house
[2031.82 → 2032.70] would be one zone
[2032.70 → 2034.18] and then the storage bays
[2034.18 → 2035.36] could all be a separate zone
[2035.36 → 2035.82] if I had,
[2035.96 → 2036.82] if I went as far as
[2036.82 → 2037.62] putting door sensors
[2037.62 → 2038.36] on the storage bays,
[2038.40 → 2039.12] which I have not done,
[2039.92 → 2040.64] but have considered.
[2041.44 → 2041.84] You know,
[2041.88 → 2042.44] you could even have,
[2042.58 → 2043.54] so you could have the house
[2043.54 → 2044.44] unarmed,
[2044.56 → 2045.00] but you could have
[2045.00 → 2046.08] the storage bays armed,
[2046.14 → 2046.76] which is great,
[2046.82 → 2047.84] like when we're at a campground.
[2048.00 → 2048.44] Oh yeah.
[2048.58 → 2049.78] Or a rest stop or something.
[2049.78 → 2050.18] Yep.
[2050.42 → 2050.68] Yep.
[2050.78 → 2051.02] Yep.
[2051.02 → 2051.10] Yep.
[2051.10 → 2051.34] Yep.
[2052.34 → 2052.54] Yeah.
[2052.54 → 2052.90] I don't know.
[2053.06 → 2054.54] I'm considering it.
[2054.78 → 2055.02] You know,
[2055.06 → 2055.82] obviously I'm travelling
[2055.82 → 2057.32] as this episode comes out,
[2057.36 → 2058.22] I'm travelling to scale
[2058.22 → 2058.82] and Alex,
[2058.88 → 2059.42] you're going to be at scale,
[2059.48 → 2059.72] right?
[2060.46 → 2060.82] Yeah.
[2061.14 → 2061.36] Yeah.
[2061.44 → 2062.20] So I've got a talk
[2062.20 → 2062.74] on the Saturday.
[2063.30 → 2063.54] Yeah.
[2063.84 → 2064.16] And,
[2064.24 → 2065.48] and so we're probably,
[2065.58 → 2066.06] that's where we're at
[2066.06 → 2066.44] right now,
[2066.48 → 2067.04] probably as people
[2067.04 → 2067.52] are listening to this,
[2067.56 → 2068.46] we're probably at your talk
[2068.46 → 2069.26] right now.
[2069.36 → 2069.88] Think about that.
[2070.52 → 2071.82] Wish I haven't written yet.
[2072.48 → 2072.98] Oh man.
[2073.68 → 2074.88] So if anybody has
[2074.88 → 2075.92] any experience with Alarm
[2075.92 → 2077.56] or any thoughts
[2077.56 → 2078.36] on this process
[2078.36 → 2079.06] that I'm considering,
[2079.52 → 2081.12] I've also seen folks
[2081.12 → 2081.94] on YouTube.
[2082.54 → 2083.08] I'm not going to go
[2083.08 → 2083.78] down this route yet,
[2083.88 → 2084.30] so I'm just going
[2084.30 → 2085.06] to save people time.
[2085.50 → 2085.70] Yes,
[2085.72 → 2086.46] I've seen the people
[2086.46 → 2088.14] that go gets the alarm systems
[2088.14 → 2088.96] from the 90s,
[2089.20 → 2089.88] like the one I actually
[2089.88 → 2090.54] have in the studio.
[2090.88 → 2091.72] And you can make
[2091.72 → 2092.56] all of that work
[2092.56 → 2093.14] with Home Assistant.
[2093.24 → 2093.86] No way.
[2094.18 → 2094.50] Yeah,
[2094.66 → 2094.94] yeah,
[2095.10 → 2095.42] yeah.
[2096.14 → 2097.04] That is gross.
[2097.66 → 2098.38] It's weird,
[2098.80 → 2099.52] but then it's like,
[2099.82 → 2099.98] it's,
[2100.06 → 2100.22] you know,
[2100.24 → 2101.38] the door sensor technology
[2101.38 → 2101.88] is magnets,
[2102.02 → 2102.16] right?
[2102.18 → 2102.98] It hasn't changed much.
[2102.98 → 2103.46] I suppose.
[2103.68 → 2104.38] Motion sensors,
[2104.50 → 2105.10] and then you get
[2105.10 → 2106.72] a physical pad,
[2107.20 → 2107.54] you know?
[2107.62 → 2109.22] It's time to get physical.
[2109.82 → 2110.12] Yeah.
[2110.74 → 2111.50] So there's that.
[2111.50 → 2112.14] Also,
[2112.42 → 2114.60] in just the news
[2114.60 → 2115.54] of sensors,
[2115.90 → 2117.46] there's some good news
[2117.46 → 2118.42] about the Apollo
[2118.42 → 2119.56] automation folks
[2119.56 → 2120.92] and joining the
[2120.92 → 2122.04] Works with Home Assistant
[2122.04 → 2122.50] program.
[2123.34 → 2123.46] Yeah,
[2123.58 → 2124.48] Apollo Automation,
[2124.62 → 2126.22] they're a fairly new
[2126.22 → 2127.56] smart home company,
[2127.76 → 2128.98] but they are building
[2128.98 → 2130.74] a really great reputation
[2130.74 → 2131.32] for themselves,
[2131.32 → 2132.56] and they are now
[2132.56 → 2133.20] officially
[2133.20 → 2134.58] the first
[2134.58 → 2135.90] made-for-ESP
[2135.90 → 2136.42] home,
[2136.72 → 2138.12] works-with-home assistant,
[2138.34 → 2139.08] certified
[2139.08 → 2140.44] automation,
[2140.68 → 2141.66] home automation partner.
[2141.66 → 2142.96] This is great.
[2143.34 → 2144.08] This is like made,
[2144.18 → 2144.58] this is,
[2144.64 → 2145.58] this is perfect
[2145.58 → 2146.60] for guys like us.
[2146.66 → 2147.02] I don't,
[2147.48 → 2148.10] I don't need to build
[2148.10 → 2148.84] all my own sensors,
[2148.98 → 2149.94] but I'd love it to be built
[2149.94 → 2150.94] on this technology
[2150.94 → 2152.22] that I know is solid
[2152.22 → 2153.10] and works great
[2153.10 → 2154.06] with the system I have.
[2154.06 → 2155.44] They have a range
[2155.44 → 2156.00] of sensors,
[2156.00 → 2157.72] from air quality sensors
[2157.72 → 2159.10] to millimetre wave sensors,
[2159.26 → 2160.14] radar sensors,
[2160.74 → 2162.36] plant watering sensors,
[2162.74 → 2163.28] and also...
[2163.28 → 2163.96] CO2 sensors?
[2164.24 → 2164.62] Yeah,
[2164.94 → 2166.48] garage parking assistant,
[2166.62 → 2167.22] like radar,
[2167.22 → 2168.70] so you could pull
[2168.70 → 2169.32] into your garage
[2169.32 → 2169.80] and think,
[2170.16 → 2171.42] how much further forward
[2171.42 → 2172.12] should I be pulling
[2172.12 → 2173.30] and have like an LED
[2173.30 → 2174.30] traffic light system,
[2174.38 → 2175.06] that'd be pretty cool.
[2175.46 → 2176.56] That's not a bad idea at all.
[2176.68 → 2177.74] Little LED
[2177.74 → 2178.24] that just book,
[2178.24 → 2178.66] book, book, book, book.
[2178.98 → 2179.22] Yeah,
[2179.56 → 2180.52] and they've just released
[2180.52 → 2182.02] a temperature probe
[2182.02 → 2183.42] called the Temp1,
[2183.66 → 2184.40] and this thing
[2184.40 → 2185.48] can actually withstand
[2185.48 → 2186.78] all sorts of
[2186.78 → 2187.80] ridiculous temperatures
[2187.80 → 2188.38] that you can put it
[2188.38 → 2189.20] inside an oven
[2189.20 → 2190.42] and it will measure
[2190.42 → 2192.48] up to 190 degrees Fahrenheit.
[2193.40 → 2194.96] A bunch of other stuff too,
[2195.08 → 2195.58] like it's,
[2195.62 → 2196.92] it's really cool.
[2196.92 → 2197.92] So if you're smoking
[2197.92 → 2198.88] those meats or whatever,
[2199.38 → 2200.24] you can actually use this
[2200.24 → 2201.06] inside your brisket
[2201.06 → 2203.36] to be a Temp probe.
[2204.18 → 2204.72] Could you imagine
[2204.72 → 2206.54] checking the home assistant chart
[2206.54 → 2207.84] for your brisket smoker?
[2208.42 → 2208.76] Yes.
[2208.86 → 2209.78] Actually, yes, yes,
[2209.78 → 2209.84] you can.
[2209.84 → 2210.42] Yes, I can.
[2213.68 → 2214.28] So anyway,
[2214.30 → 2215.18] we've got a couple of products
[2215.18 → 2215.82] on the bench.
[2216.32 → 2216.56] I was,
[2216.94 → 2217.96] I haven't,
[2218.22 → 2219.18] I just haven't gotten around
[2219.18 → 2220.04] to reviewing them yet
[2220.04 → 2222.66] because the attic's
[2222.66 → 2223.30] still not done yet.
[2223.48 → 2223.86] When I,
[2223.90 → 2224.16] when I,
[2224.32 → 2225.10] when I'm done up there,
[2225.12 → 2226.06] I want the lighting
[2226.06 → 2227.02] to be controlled.
[2227.82 → 2228.04] Well,
[2228.14 → 2228.80] first,
[2228.80 → 2229.72] I wanted to turn on
[2229.72 → 2231.08] through a PIR sensor
[2231.08 → 2232.72] because the response time
[2232.72 → 2233.66] for PIR is supposed
[2233.66 → 2234.10] to be better
[2234.10 → 2235.00] than millimetre wave.
[2235.42 → 2236.48] So I use PIR
[2236.48 → 2237.76] to turn the lights on
[2237.76 → 2238.82] and then I'll use
[2238.82 → 2239.72] millimetre wave
[2239.72 → 2240.44] and I've got a couple
[2240.44 → 2241.08] of their sensors
[2241.08 → 2241.92] ready to go
[2241.92 → 2243.72] for when the attic's done.
[2243.90 → 2245.18] So watch this space,
[2245.30 → 2245.72] but you know,
[2245.74 → 2246.60] I just wanted to highlight
[2246.60 → 2247.52] that Apollo automation
[2247.52 → 2249.18] have been accepted
[2249.18 → 2250.18] into the works
[2250.18 → 2251.32] with home assistant program
[2251.32 → 2252.62] and that ensures
[2252.62 → 2253.80] that certified devices
[2253.80 → 2255.26] are thoroughly tested,
[2255.58 → 2256.42] they're compatible
[2256.42 → 2257.48] and will receive
[2257.48 → 2258.34] ongoing support
[2258.34 → 2258.86] and updates
[2258.86 → 2260.48] to the standard
[2260.48 → 2261.28] that home assistant
[2261.28 → 2262.72] requires being a member
[2262.72 → 2263.30] of this program.
[2263.96 → 2264.58] So really,
[2264.64 → 2265.52] it's just a good way
[2265.52 → 2266.32] for users to know
[2266.32 → 2267.24] that they're getting,
[2267.40 → 2268.06] I suppose,
[2268.18 → 2268.76] well-supported
[2268.76 → 2270.22] and reliable products.
[2270.22 → 2274.02] keeb.io slash self-hosted,
[2274.10 → 2276.52] K-E-E-B.io slash self-hosted.
[2276.56 → 2277.18] Head on over there,
[2277.30 → 2277.94] sign up for the newsletter
[2277.94 → 2279.18] and get 5% off
[2279.18 → 2279.90] your next order.
[2280.36 → 2281.10] Let's face it,
[2281.68 → 2282.60] your keyboard might be
[2282.60 → 2283.44] one of the most important
[2283.44 → 2284.44] things you own.
[2284.82 → 2285.50] It took me a while
[2285.50 → 2286.46] to appreciate that,
[2286.58 → 2287.06] but I mean,
[2287.10 → 2288.02] I'm interfacing with it
[2288.02 → 2288.88] every day,
[2289.08 → 2290.26] most of the day.
[2290.70 → 2292.14] It's the primary interface
[2292.14 → 2292.90] to my computer
[2292.90 → 2294.26] and there's a lot
[2294.26 → 2295.08] of options out there,
[2295.20 → 2296.44] but I'm kind of somebody
[2296.44 → 2297.74] that likes a fancy keyboard now.
[2297.80 → 2298.72] I wasn't always this way,
[2298.72 → 2300.26] but I've seen the light.
[2300.84 → 2301.20] Kib.io,
[2301.34 → 2302.46] they range from regular keyboards
[2302.46 → 2303.86] and they really specialize
[2303.86 → 2305.70] in those cool split keyboards
[2305.70 → 2307.00] and the keyboards,
[2307.16 → 2308.22] they'll come fully built,
[2308.58 → 2309.22] ready to use
[2309.22 → 2310.18] if that's how you like it,
[2310.22 → 2310.92] out of the box
[2310.92 → 2312.38] or you can get it as a kit
[2312.38 → 2313.58] and assemble it,
[2313.64 → 2314.34] do some hot swapping.
[2314.82 → 2315.72] There's no soldering
[2315.72 → 2316.28] for those parts,
[2316.38 → 2317.48] so it might be a fun project
[2317.48 → 2318.16] for home too
[2318.16 → 2319.20] or, you know,
[2319.24 → 2320.02] if you just want to get started,
[2320.10 → 2320.52] you can get one
[2320.52 → 2321.12] that's fully built.
[2321.42 → 2322.06] The other thing
[2322.06 → 2323.12] that I think you should look at
[2323.12 → 2324.08] and you could kind of
[2324.08 → 2325.48] up your game a little bit
[2325.48 → 2326.90] is their macro pads.
[2327.10 → 2328.58] With those 9 to 16 keys,
[2328.58 → 2329.12] you can use them
[2329.12 → 2330.02] for all kinds of things.
[2330.12 → 2331.24] You can put phrases on there
[2331.24 → 2331.96] and have it connected
[2331.96 → 2333.38] to something like Bit Focus.
[2334.36 → 2335.92] You could have it control OBS.
[2336.72 → 2336.96] You know,
[2337.04 → 2337.92] there's probably a way
[2337.92 → 2339.00] using the Stream Deck software
[2339.00 → 2339.66] to tie it in
[2339.66 → 2340.72] with Home Assistant as well
[2340.72 → 2341.94] or maybe it's a nice way
[2341.94 → 2343.34] to control your home media PC.
[2344.08 → 2344.30] They just,
[2344.40 → 2345.50] I think those are so handy.
[2345.58 → 2346.24] We have a couple of them
[2346.24 → 2346.84] right here in the studio.
[2346.88 → 2347.12] In fact,
[2348.08 → 2348.46] I've got,
[2348.68 → 2349.02] look at this,
[2349.08 → 2350.56] I've got one right here.
[2351.36 → 2352.62] I love these little,
[2352.70 → 2353.42] this little thing,
[2353.52 → 2354.10] little side thing,
[2354.16 → 2354.26] you know,
[2354.26 → 2355.02] hook it up over USB.
[2355.20 → 2355.92] It's pretty great.
[2355.92 → 2357.56] I think people normally
[2357.56 → 2358.74] think of mechanical keyboards
[2358.74 → 2359.90] as loud and cliquey
[2359.90 → 2361.62] and those do exist,
[2361.78 → 2362.86] but they also have
[2362.86 → 2363.40] the versions
[2363.40 → 2364.78] with silent switches
[2364.78 → 2365.94] to keep things quiet
[2365.94 → 2366.42] and low-key
[2366.42 → 2367.04] in the office
[2367.04 → 2367.70] or at home,
[2367.90 → 2368.14] you know.
[2368.14 → 2370.42] I lack my loud typing.
[2370.64 → 2371.70] I'll be honest with you guys,
[2371.84 → 2373.82] but not everybody does
[2373.82 → 2374.82] or sometimes the people
[2374.82 → 2376.22] around you don't.
[2376.84 → 2378.34] They stock lots of DIY parts
[2378.34 → 2379.42] and microcontrollers
[2379.42 → 2381.12] and they're big supporters
[2381.12 → 2381.74] of open source.
[2381.82 → 2383.48] They publish the 3D print case parts
[2383.48 → 2384.88] and they're also part
[2384.88 → 2386.70] of the core QMK team
[2386.70 → 2387.74] for the firmware
[2387.74 → 2388.88] and all their boards
[2388.88 → 2390.12] use the QMK firmware.
[2390.52 → 2392.12] I love that.
[2392.78 → 2394.28] You deserve a great keyboard.
[2394.28 → 2394.94] Check them out
[2394.94 → 2395.86] and support the show.
[2395.86 → 2398.38] Go to keeb.io
[2398.38 → 2399.50] slash self-hosted.
[2399.58 → 2401.30] That's keeb.io
[2401.30 → 2402.98] slash self-hosted.
[2403.98 → 2406.22] So I was on these here YouTube's
[2406.22 → 2407.32] and I came across
[2407.32 → 2409.02] a Network Chuck video
[2409.02 → 2410.16] about a project
[2410.16 → 2411.26] called Ex
[2411.26 → 2413.10] and then the home
[2413.10 → 2414.42] wrote in saying,
[2414.64 → 2415.00] hey guys,
[2415.06 → 2416.06] have you seen this?
[2416.70 → 2417.52] GitHub.com
[2417.52 → 2419.08] slash Ex Explore.
[2419.20 → 2419.64] There'll be a link
[2419.64 → 2420.28] in the show notes.
[2420.28 → 2421.74] You can unify
[2421.74 → 2423.22] your existing devices
[2423.22 → 2424.80] into a single
[2424.80 → 2426.28] powerful GPU.
[2426.78 → 2428.24] It allows for the distribution
[2428.24 → 2429.32] of a model,
[2429.60 → 2430.50] an LLM model,
[2430.94 → 2432.08] across multiple
[2432.08 → 2433.36] physical devices.
[2433.94 → 2435.42] Yeah, EX.
[2435.56 → 2436.92] And I have seen this
[2436.92 → 2438.40] and this is right
[2438.40 → 2439.60] up my alley.
[2439.76 → 2440.90] I have always had
[2440.90 → 2441.92] such a soft spot
[2441.92 → 2443.24] for distributed compute
[2443.24 → 2444.86] and nothing's going
[2444.86 → 2445.34] to make you feel
[2445.34 → 2446.00] like you need to upgrade
[2446.00 → 2447.08] all of your stuff,
[2447.14 → 2447.66] your storage,
[2447.80 → 2448.24] your network,
[2448.38 → 2449.62] everything like Ex will.
[2449.62 → 2451.12] Yeah, absolutely.
[2451.64 → 2452.60] Because you can basically
[2452.60 → 2453.62] give your house
[2453.62 → 2455.26] a score ranging
[2455.26 → 2456.52] from GPU poor
[2456.52 → 2457.78] to GPU rich
[2457.78 → 2459.04] on the Ex dashboard.
[2459.60 → 2461.20] Yeah, yeah, yeah.
[2461.28 → 2461.98] What's cool though
[2461.98 → 2463.46] is it creates this
[2463.46 → 2465.44] kind of like picture
[2465.44 → 2466.50] of your infrastructure
[2466.50 → 2466.98] and says,
[2467.34 → 2467.58] you know,
[2467.64 → 2468.56] your Linux box
[2468.56 → 2469.82] runs at so many
[2469.82 → 2470.44] teraflops
[2470.44 → 2472.02] and your MacBook Pro
[2472.02 → 2473.48] runs at so many
[2473.48 → 2474.18] teraflops
[2474.18 → 2474.72] and it's like
[2474.72 → 2475.66] your Raspberry Pi
[2475.66 → 2477.54] runs at whatever
[2477.54 → 2477.94] the equivalent
[2477.94 → 2479.04] of a microflop is.
[2479.62 → 2480.34] And it's also,
[2480.66 → 2480.88] I mean,
[2480.98 → 2482.54] I haven't tried
[2482.54 → 2483.18] this extensively
[2483.18 → 2484.12] because I have
[2484.12 → 2484.90] very limited options,
[2485.06 → 2487.24] but my understanding
[2487.24 → 2488.40] is it's also pretty good
[2488.40 → 2489.30] at seeing which
[2489.30 → 2490.12] network interfaces,
[2490.54 → 2491.32] if you have multiple
[2491.32 → 2492.18] options and multiple
[2492.18 → 2492.56] routes,
[2492.68 → 2493.72] are communicating the
[2493.72 → 2494.66] fastest amongst the
[2494.66 → 2495.58] machines and then
[2495.58 → 2497.20] picking that for the
[2497.20 → 2498.06] transmission of like,
[2498.12 → 2498.28] you know,
[2498.32 → 2498.98] loading the model
[2498.98 → 2499.70] and things like that.
[2500.48 → 2501.02] Yeah, I haven't actually
[2501.02 → 2502.12] had a chance to use this
[2502.12 → 2502.96] yet thanks to my
[2502.96 → 2503.62] server shenanigans
[2503.62 → 2504.32] this weekend.
[2504.58 → 2505.74] I'd actually plan to
[2505.74 → 2506.78] look at this weekend
[2506.78 → 2507.56] and, you know,
[2507.70 → 2508.16] c'est la vie.
[2508.16 → 2509.28] Yeah, I think we could
[2509.28 → 2509.94] come back to this
[2509.94 → 2511.40] because this is like
[2511.40 → 2512.22] right up our alley.
[2512.40 → 2513.26] Yeah, for sure.
[2513.60 → 2514.84] What I'd like to test
[2514.84 → 2517.56] is how good does the
[2517.56 → 2518.58] network link between
[2518.58 → 2519.98] those boxes need to be?
[2520.36 → 2521.48] And let's say there was
[2521.48 → 2523.10] a GPU in the data
[2523.10 → 2524.12] centre in Toronto
[2524.12 → 2525.94] and a GPU in Chris's
[2525.94 → 2527.74] proverbial basement
[2527.74 → 2528.62] and one in my,
[2528.70 → 2529.86] like, could we link all
[2529.86 → 2530.72] of those three together
[2530.72 → 2531.78] or do you need to be
[2531.78 → 2532.10] local?
[2532.10 → 2534.20] And is it that initial
[2534.20 → 2535.42] load is maybe really
[2535.42 → 2536.30] long and painful
[2536.30 → 2537.32] but then after that
[2537.32 → 2538.40] it's smaller updates
[2538.40 → 2539.48] so it's actually
[2539.48 → 2539.94] functional?
[2540.22 → 2540.52] Yeah.
[2541.20 → 2542.30] Yeah, I'm just curious
[2542.30 → 2543.14] to answer that question
[2543.14 → 2543.82] really and then like
[2543.82 → 2545.00] how distributed can we
[2545.00 → 2545.66] actually be?
[2546.36 → 2546.58] Yeah.
[2547.08 → 2547.28] Yeah.
[2548.16 → 2548.78] Scott wrote in,
[2548.82 → 2549.46] I'm currently looking
[2549.46 → 2550.82] for a suggestion about
[2550.82 → 2552.20] Open Sense versus the
[2552.20 → 2552.90] Ubiquity firewall.
[2553.42 → 2554.02] I listen to all your
[2554.02 → 2554.64] shows and I can't
[2554.64 → 2555.32] remember which one you
[2555.32 → 2556.06] described your newest
[2556.06 → 2556.52] home setup.
[2556.52 → 2557.66] I moved to a new
[2557.66 → 2560.16] Pro Max 24 POE when my
[2560.16 → 2562.18] trusty ICE 6610 started
[2562.18 → 2562.64] dying.
[2563.10 → 2564.34] Now I'm trying to
[2564.34 → 2566.26] decide if I go full UI
[2566.26 → 2568.10] or stay with Open Sense.
[2568.32 → 2569.12] Thanks for your time
[2569.12 → 2569.96] and the great content.
[2570.56 → 2571.82] Well I made the switch
[2571.82 → 2573.28] to a what's it, a
[2573.28 → 2575.56] UDM Pro something or
[2575.56 → 2577.90] other probably about two
[2577.90 → 2578.74] or three months ago.
[2579.52 → 2581.68] I kind of love it after a
[2581.68 → 2582.28] bit of time.
[2582.74 → 2583.24] Yeah, okay.
[2583.42 → 2584.74] Mostly for VLAN
[2584.74 → 2585.20] management.
[2585.20 → 2587.64] I upgraded to it
[2587.64 → 2588.38] because I thought it
[2588.38 → 2588.84] would be nice.
[2588.92 → 2590.42] I've got Unify switches
[2590.42 → 2591.98] and access points.
[2592.08 → 2592.98] It would be nice if I
[2592.98 → 2594.32] just had like a
[2594.32 → 2595.54] dashboard that could
[2595.54 → 2596.62] understand and speak
[2596.62 → 2598.12] that language for all
[2598.12 → 2599.08] the data that those
[2599.08 → 2599.90] switches are collecting
[2599.90 → 2600.94] and present it to me in
[2600.94 → 2601.42] one place.
[2602.30 → 2603.70] But over the last few
[2603.70 → 2604.62] months, you know, I
[2604.62 → 2606.32] co-located Shane's
[2606.32 → 2607.32] server in my basement
[2607.32 → 2608.34] from a few episodes
[2608.34 → 2608.68] ago.
[2609.18 → 2610.08] So he's got his own
[2610.08 → 2611.24] VLAN and I can just,
[2611.40 → 2612.18] you know, from the
[2612.18 → 2613.02] Unify dashboard,
[2613.50 → 2614.04] book, book, book,
[2614.04 → 2615.14] map a couple of
[2615.14 → 2617.24] ports to his VLAN
[2617.24 → 2618.06] physical ports.
[2618.06 → 2618.90] So he doesn't need to
[2618.90 → 2619.88] do any tagging on the
[2619.88 → 2620.42] interfaces.
[2621.74 → 2623.08] It's got Unified
[2623.08 → 2624.40] Protect built in for
[2624.40 → 2624.92] cameras.
[2625.02 → 2625.74] I just throw a hard
[2625.74 → 2626.58] drive in there and it
[2626.58 → 2628.24] just works even with
[2628.24 → 2630.16] third-party cameras now
[2630.16 → 2631.06] using Aviv.
[2632.18 → 2633.24] That is nice.
[2633.46 → 2634.62] It is really nice.
[2634.94 → 2636.44] The one real bug
[2636.44 → 2637.58] bear, like the biggest
[2637.58 → 2638.72] difference for me of
[2638.72 → 2641.38] as an end user, of
[2641.38 → 2642.46] course, Open Sense is a
[2642.46 → 2644.32] BSD-based thing and
[2644.32 → 2645.58] Ubiquity firewalls
[2645.58 → 2646.56] actually underneath run
[2646.56 → 2647.96] Debian, I think.
[2650.10 → 2651.04] So I'm sort of thinking
[2651.04 → 2651.88] to myself, well, I can
[2651.88 → 2652.78] put Tail scale on the
[2652.78 → 2653.66] UDM, can't I?
[2653.82 → 2655.88] Well, technically, yes,
[2655.92 → 2657.64] you can, but every time
[2657.64 → 2658.68] you upgrade the
[2658.68 → 2659.72] firmware, it gets
[2659.72 → 2660.50] wiped, and you have to
[2660.50 → 2661.20] do it again.
[2661.60 → 2661.92] Right.
[2661.92 → 2664.74] So the DMS do support
[2664.74 → 2666.36] native WireGuard.
[2667.50 → 2668.52] So if you want to do a
[2668.52 → 2669.88] site-to-site VPN, they
[2669.88 → 2670.98] also have their own
[2670.98 → 2673.72] proprietary Unify VPN
[2673.72 → 2674.80] stuff that does that,
[2674.86 → 2675.48] which makes it very
[2675.48 → 2675.78] nice.
[2675.84 → 2677.14] So like, if you're all
[2677.14 → 2678.16] in on the Unify
[2678.16 → 2679.52] ecosystem, and you have a
[2679.52 → 2680.32] bunch of switches,
[2681.14 → 2682.36] absolutely go for it
[2682.36 → 2683.10] because it just makes
[2683.10 → 2684.22] managing the whole
[2684.22 → 2686.36] network a piece of
[2686.36 → 2686.68] cake.
[2687.06 → 2688.32] It's just a fabulous
[2688.32 → 2689.04] experience.
[2689.04 → 2691.98] And apart from the
[2691.98 → 2693.12] price, really, for what
[2693.12 → 2694.48] it is, you know, the
[2694.48 → 2695.74] Open Sense stuff, you'll
[2695.74 → 2696.98] pay for it in time
[2696.98 → 2699.60] configuring Plans and
[2699.60 → 2700.58] DHCP this.
[2700.86 → 2702.82] And I do love...
[2702.82 → 2703.42] Sounds like it kind of
[2703.42 → 2703.88] comes down to, does
[2703.88 → 2704.44] you want to be part of
[2704.44 → 2705.74] the Unify ecosystem?
[2706.20 → 2706.84] And is it going to
[2706.84 → 2708.08] have other products and
[2708.08 → 2708.64] things in that
[2708.64 → 2709.10] ecosystem?
[2709.34 → 2710.52] Or is this a one-off?
[2710.70 → 2711.34] Kind of what it sounds
[2711.34 → 2712.02] like it comes down to.
[2712.36 → 2712.72] Exactly.
[2712.98 → 2713.16] Yeah.
[2713.26 → 2713.74] I couldn't have said it
[2713.74 → 2713.96] better.
[2715.04 → 2715.88] Well, let us know what
[2715.88 → 2716.20] you do.
[2716.50 → 2717.18] I mean, this is
[2717.18 → 2718.06] something I'm also
[2718.06 → 2718.84] kind of considering
[2718.84 → 2719.48] for the studio.
[2719.68 → 2720.38] I'm, you know, I'm
[2720.38 → 2721.20] thinking everything from
[2721.20 → 2723.20] like a tiny SBC Nix box
[2723.20 → 2724.86] that is a really basic
[2724.86 → 2726.02] router because my
[2726.02 → 2726.66] firewall doesn't do
[2726.66 → 2728.54] much anymore to all
[2728.54 → 2729.04] the way up to something
[2729.04 → 2730.22] like the Unify system
[2730.22 → 2731.02] with the idea of then
[2731.02 → 2732.38] eventually that'll be
[2732.38 → 2733.12] the switch in the
[2733.12 → 2733.92] studio and then
[2733.92 → 2734.54] eventually that'll be
[2734.54 → 2735.32] the cameras in the
[2735.32 → 2735.58] studio.
[2735.72 → 2736.62] But, you know, just do
[2736.62 → 2737.28] it over time.
[2737.82 → 2738.50] And I haven't made my
[2738.50 → 2739.26] mind up yet, but I am
[2739.26 → 2739.98] kind of leaning that
[2739.98 → 2740.68] direction and then
[2740.68 → 2741.96] starting with the edge
[2741.96 → 2742.90] and then kind of
[2742.90 → 2744.08] building on the other
[2744.08 → 2744.80] devices from there.
[2744.90 → 2745.58] So let me know what
[2745.58 → 2745.90] you do.
[2746.98 → 2747.94] Unify just gets
[2747.94 → 2750.16] increasingly better
[2750.16 → 2751.14] the more you have,
[2751.20 → 2751.76] unfortunately.
[2752.70 → 2753.26] It's one of those
[2753.26 → 2754.66] types of things you
[2754.66 → 2755.28] think, oh, well, I
[2755.28 → 2755.98] could just get a
[2755.98 → 2757.22] bog-standard, simple,
[2757.90 → 2759.22] unmanaged switch for my
[2759.22 → 2763.22] desk, or I could get
[2763.22 → 2763.96] one where I could tag
[2763.96 → 2764.94] the ports and all the
[2764.94 → 2765.32] rest of it.
[2765.38 → 2765.58] And you're like,
[2765.66 → 2768.50] well, I'm in this far
[2768.50 → 2769.18] and may as well keep
[2769.18 → 2769.62] going.
[2769.78 → 2770.48] It's like a Costco
[2770.48 → 2771.40] membership, you know.
[2771.40 → 2774.22] Now we are recording
[2774.22 → 2775.28] early this week.
[2775.44 → 2776.24] In fact, if you're
[2776.24 → 2778.02] listening right as it
[2778.02 → 2778.76] comes out, you still
[2778.76 → 2779.46] have a chance to come
[2779.46 → 2780.08] say hi at our
[2780.08 → 2781.60] Saturday dinner at
[2781.60 → 2782.02] scale.
[2782.28 → 2783.20] It'll be on March
[2783.20 → 2784.40] 8th at 7 p.m.
[2784.40 → 2785.86] We have details at
[2785.86 → 2786.86] meetup.com slash
[2786.86 → 2787.82] Jupiter Broadcasting.
[2788.20 → 2789.12] And we'd love it if you
[2789.12 → 2790.18] came and said hi.
[2790.52 → 2792.00] But as I was just
[2792.00 → 2792.92] kind of collecting some
[2792.92 → 2794.20] links, I saw a boost
[2794.20 → 2795.66] from Adversary 17 came
[2795.66 → 2796.80] in for 17,000 SATs,
[2796.88 → 2798.18] like literally at just
[2798.18 → 2798.72] the right moment.
[2798.72 → 2799.92] And he has a good
[2799.92 → 2801.04] question that I think
[2801.04 → 2801.78] I would want to know
[2801.78 → 2802.00] too.
[2802.44 → 2803.26] He says, a few weeks
[2803.26 → 2804.48] ago, I mentioned I
[2804.48 → 2805.64] might get a Brusa
[2805.64 → 2806.50] Core 1.
[2807.02 → 2807.72] Well, I have.
[2807.84 → 2808.40] All right.
[2808.78 → 2809.18] Congratulations.
[2809.82 → 2811.50] He says, it should
[2811.50 → 2812.40] ship this month, but
[2812.40 → 2813.04] now I've been going
[2813.04 → 2813.90] down the rabbit hole
[2813.90 → 2814.64] of filaments.
[2815.16 → 2815.92] Alex, what do you
[2815.92 → 2816.84] primarily print with?
[2816.90 → 2817.88] Any good brands,
[2818.04 → 2818.86] places to get it,
[2818.96 → 2819.62] things to look out
[2819.62 → 2819.90] for?
[2820.36 → 2821.46] Any tips for, quote,
[2821.50 → 2822.36] I wish I knew this
[2822.36 → 2823.16] before I'd done
[2823.16 → 2824.08] something advice type
[2824.08 → 2824.32] thing?
[2824.58 → 2825.46] I'm a total noob,
[2825.76 → 2826.62] so any and all help
[2826.62 → 2827.24] would be appreciated.
[2827.68 → 2828.26] Well, this is a
[2828.26 → 2829.26] really great question
[2829.26 → 2830.48] because there is,
[2831.76 → 2832.50] nothing beats
[2832.50 → 2833.16] experience.
[2833.40 → 2834.36] At least that's what
[2834.36 → 2835.12] my old man used to
[2835.12 → 2835.52] tell me.
[2835.76 → 2836.60] Look at these grey
[2836.60 → 2837.30] hairs, each one
[2837.30 → 2838.34] represents something I
[2838.34 → 2838.78] did wrong.
[2839.40 → 2840.38] That's why my beard
[2840.38 → 2841.24] is basically full of
[2841.24 → 2841.96] grey hairs these
[2841.96 → 2842.20] days.
[2843.62 → 2845.12] So I primarily print
[2845.12 → 2846.00] with a mixture of
[2846.00 → 2848.12] PLA and PET
[2848.12 → 2848.62] filaments.
[2849.10 → 2851.02] And actually, for the
[2851.02 → 2852.40] most part, PLA, to be
[2852.40 → 2852.66] honest.
[2853.30 → 2854.50] I pick out whatever
[2854.50 → 2855.30] happens to be the
[2855.30 → 2856.58] the cheapest rolls on
[2856.58 → 2856.92] Amazon.
[2857.16 → 2857.86] And I just go with a
[2857.86 → 2858.84] bog-standard boring
[2858.84 → 2859.78] black filament for
[2859.78 → 2861.20] most things, like the
[2861.20 → 2862.18] infinity pots that
[2862.18 → 2863.04] I've printed eight
[2863.04 → 2863.96] bazillion of.
[2864.42 → 2865.20] I think you can get a
[2865.20 → 2866.54] roll of Elegy filament
[2866.54 → 2868.22] for about $13 or $14
[2868.22 → 2869.98] now for a kilo, which
[2869.98 → 2871.52] isn't too bad.
[2872.16 → 2873.58] You can go more exotic
[2873.58 → 2874.46] with like Proto
[2874.46 → 2876.90] Pastas and there's all
[2876.90 → 2877.58] sorts of brands.
[2877.72 → 2878.72] I mean, Printed Solid is
[2878.72 → 2880.02] the local now US
[2880.02 → 2880.74] distributor of
[2880.74 → 2883.32] Rosemont and all of
[2883.32 → 2884.34] these different things.
[2884.34 → 2885.58] But I've never really
[2885.58 → 2886.70] found that much
[2886.70 → 2888.16] benefit from going
[2888.16 → 2891.16] with a premium
[2891.16 → 2892.22] supplier of filament
[2892.22 → 2893.94] versus a more entry
[2893.94 → 2895.32] level, like just the
[2895.32 → 2896.14] the cheapest ones you can
[2896.14 → 2896.38] get.
[2897.04 → 2897.82] A lot of the
[2897.82 → 2899.90] manufacturers like to
[2899.90 → 2902.54] use, I don't want to
[2902.54 → 2903.08] accuse them of
[2903.08 → 2905.50] marketing their own
[2905.50 → 2906.50] stuff when that's
[2906.50 → 2907.04] exactly what they're
[2907.04 → 2907.64] doing, I suppose.
[2907.74 → 2908.68] But they talk about
[2908.68 → 2909.54] like dimensional
[2909.54 → 2910.74] accuracy of the
[2910.74 → 2911.72] filament being important
[2911.72 → 2913.34] as it's extruded
[2913.34 → 2914.86] through the nozzle
[2914.86 → 2915.60] and all the rest of
[2915.60 → 2915.68] it.
[2915.74 → 2916.62] And of course, that
[2916.62 → 2918.32] stuff does matter to
[2918.32 → 2918.90] a point.
[2919.16 → 2920.16] But really, you've got
[2920.16 → 2920.84] to ask yourself the
[2920.84 → 2922.22] question of like, how
[2922.22 → 2923.54] much do I actually
[2923.54 → 2926.08] care about the most
[2926.08 → 2927.36] perfect print, the
[2927.36 → 2928.34] most perfect model?
[2928.46 → 2930.10] Because the reality is
[2930.10 → 2931.08] with FDM printing,
[2931.60 → 2932.58] which is what the
[2932.58 → 2933.84] Core 1 is doing and
[2933.84 → 2935.28] every, you know,
[2936.40 → 2937.20] sort of bed slinger
[2937.20 → 2938.20] before it was doing
[2938.20 → 2940.64] too, you're not going
[2940.64 → 2942.48] to get prints that
[2942.48 → 2944.04] are actually perfect.
[2944.16 → 2944.84] If you want that,
[2944.96 → 2945.40] you've got to go
[2945.40 → 2946.24] resin, really.
[2946.92 → 2947.88] You can do a lot to
[2947.88 → 2949.04] like sand and smooth
[2949.04 → 2950.62] prints with acetone and
[2950.62 → 2951.58] paint them and fill
[2951.58 → 2952.72] them with like bond
[2952.72 → 2953.80] and filler and all the
[2953.80 → 2954.22] rest of it.
[2954.32 → 2956.22] But for the most part,
[2956.26 → 2957.12] I like to just print
[2957.12 → 2958.82] things in PLA and just
[2958.82 → 2959.50] keep it simple.
[2960.14 → 2961.64] The downside of PLA is
[2961.64 → 2962.52] it doesn't like getting
[2962.52 → 2964.14] warm at all.
[2964.20 → 2964.74] So like if you're going
[2964.74 → 2965.42] to print something to
[2965.42 → 2966.44] go inside your car,
[2967.32 → 2968.96] PLA will soften and go
[2968.96 → 2969.54] through what's called
[2969.54 → 2970.56] the glass transition
[2970.56 → 2971.92] temperature at about
[2971.92 → 2974.18] 45 Celsius, which
[2974.18 → 2975.48] means it becomes soft
[2975.48 → 2976.68] like warm chocolate.
[2977.08 → 2978.08] It's not actually
[2978.08 → 2978.60] melting.
[2979.06 → 2980.14] It just goes really
[2980.14 → 2980.64] soft.
[2980.76 → 2981.34] You know, when you've
[2981.34 → 2982.04] picked up a chocolate
[2982.04 → 2982.68] bar that's melted,
[2982.78 → 2983.52] you know exactly what I
[2983.52 → 2983.74] mean.
[2984.54 → 2987.06] Whereas PET, it can be
[2987.06 → 2988.74] a little more forgiving.
[2988.92 → 2989.74] It's got a little bit
[2989.74 → 2990.50] of flex to it.
[2990.56 → 2991.42] It can handle higher
[2991.42 → 2992.38] temperatures before it
[2992.38 → 2992.86] transitions.
[2992.86 → 2994.26] And, you know, if
[2994.26 → 2994.66] you're going to make
[2994.66 → 2995.38] something that's going
[2995.38 → 2997.66] to take some, that's
[2997.66 → 2998.52] going to need some give
[2998.52 → 2999.62] us some flex to it, then
[2999.62 → 3001.12] PET is the way to go.
[3002.18 → 3004.10] I've printed with ABS a
[3004.10 → 3005.98] few times, and it is the
[3005.98 → 3007.98] most picky, most
[3007.98 → 3009.88] difficult, most stinky,
[3010.10 → 3011.70] horrible stuff in the
[3011.70 → 3012.16] world.
[3012.88 → 3014.48] So, yeah, would not
[3014.48 → 3015.54] recommend ABS.
[3016.06 → 3017.14] Beyond that, just
[3017.14 → 3018.78] immerse yourself and have
[3018.78 → 3019.08] fun.
[3019.62 → 3020.94] You've bought an amazing
[3020.94 → 3022.16] machine with the Core 1,
[3022.20 → 3022.96] I'm sure of it.
[3023.54 → 3024.92] Brusa's got a reputation
[3024.92 → 3025.78] for a reason.
[3026.74 → 3027.86] And, yeah, thanks for
[3027.86 → 3029.60] writing in and have fun.
[3030.22 → 3031.08] Enjoy your replicator
[3031.08 → 3031.56] adversaries.
[3031.80 → 3033.14] And thank you everybody
[3033.14 → 3033.88] else who does support the
[3033.88 → 3034.58] show with a boost.
[3034.94 → 3036.02] We will be reading those
[3036.02 → 3036.90] when we get back to our
[3036.90 → 3037.86] regular schedule.
[3038.58 → 3041.18] And also, I just want to
[3041.18 → 3043.04] say a huge thank you
[3043.04 → 3043.52] to our members.
[3043.64 → 3044.12] You are like the
[3044.12 → 3044.84] foundation out there.
[3044.88 → 3045.56] That's why we call you
[3045.56 → 3046.38] our site reliability
[3046.38 → 3046.86] engineers.
[3047.38 → 3048.02] Thank you for your
[3048.02 → 3048.70] support as well.
[3049.26 → 3050.32] We have details at
[3050.32 → 3052.14] self-hosted.show.SRE.
[3052.14 → 3053.28] You support the show
[3053.28 → 3054.14] and as a thank you,
[3054.56 → 3055.68] you get an ad-free feed
[3055.68 → 3056.64] and a little extra
[3056.64 → 3057.04] content.
[3057.18 → 3058.40] We put a post show on
[3058.40 → 3059.36] every episode for our
[3059.36 → 3059.64] members.
[3060.04 → 3062.40] Again, self-hosted.show.SRE.
[3062.80 → 3063.84] One of those sort of
[3063.84 → 3065.06] behind-the-scenes chats
[3065.06 → 3067.40] where Chris and I have a
[3067.40 → 3069.26] radio-polished segment
[3069.26 → 3070.72] in the main show.
[3071.28 → 3072.48] The post show gets what
[3072.48 → 3073.52] we actually think.
[3075.26 → 3076.18] Yeah, well, because
[3076.18 → 3076.92] you're like the lower
[3076.92 → 3077.52] stakes, man.
[3077.58 → 3078.26] Not as many people are
[3078.26 → 3078.96] listening, right?
[3080.00 → 3080.44] Right.
[3080.56 → 3081.30] Something like that.
[3081.30 → 3082.36] Something like that.
[3082.56 → 3082.80] Yeah.
[3083.26 → 3083.62] You can go to
[3083.62 → 3084.74] meetup.com slash
[3084.74 → 3085.64] Jupiter Broadcasting
[3085.64 → 3086.78] for details of all of
[3086.78 → 3087.78] our upcoming meetups
[3087.78 → 3089.34] like this week's
[3089.34 → 3090.94] At Scale in Pasadena.
[3091.78 → 3092.12] Yes.
[3092.22 → 3093.02] And of course, we love
[3093.02 → 3093.80] hearing from you.
[3093.92 → 3094.86] You can do that at our
[3094.86 → 3095.26] website.
[3095.42 → 3096.36] Lots of links over there.
[3096.48 → 3097.54] Self-hosted. Show slash
[3097.54 → 3098.78] contact is the place to
[3098.78 → 3099.64] go to get in touch and
[3099.64 → 3101.00] drop us a note.
[3101.36 → 3102.24] And you can find me on
[3102.24 → 3102.98] the internet at
[3102.98 → 3104.40] alex.ktz.me.
[3104.48 → 3104.90] That's where my
[3104.90 → 3106.14] self-hosted link tree
[3106.14 → 3106.56] lives.
[3107.26 → 3107.88] Oh, I like it.
[3107.94 → 3109.30] I'm just living the
[3109.30 → 3110.34] wild side over at
[3110.34 → 3111.66] chrislas.com.
[3111.88 → 3114.42] And I also respond on
[3114.42 → 3115.06] Weapon X at
[3115.06 → 3116.26] chrislas.com as well.
[3117.06 → 3118.36] That place is getting
[3118.36 → 3120.08] increasingly worse and
[3120.08 → 3120.52] worse.
[3121.66 → 3122.52] One of these days,
[3122.60 → 3123.60] Chris, we'll kick the
[3123.60 → 3124.56] X habit for you.
[3125.78 → 3126.74] You know, it's I don't
[3126.74 → 3127.66] mind if you just go to
[3127.66 → 3128.96] I have my bookmark goes
[3128.96 → 3129.72] right to my replies.
[3129.86 → 3130.48] It's not so bad.
[3130.76 → 3131.30] Oh, OK.
[3131.60 → 3132.76] Just ignore the main
[3132.76 → 3133.38] benefit of the
[3133.38 → 3133.52] play.
[3133.52 → 3133.76] Anyway.
[3134.98 → 3135.70] Thanks for listening,
[3135.80 → 3136.08] everybody.
[3136.28 → 3137.16] That was self-hosted
[3137.16 → 3138.02] dot show slash
[3138.02 → 3138.82] 144.
[3140.92 → 3141.06] Thank you.
[3141.06 → 3141.28] Thank you.
[3141.28 → 3141.56] Thanks for listening.
[3141.56 → 3141.90] Thank you.
[3141.90 → 3142.02] Thank you.
[3142.80 → 3143.04] So, if you stop
[3143.04 → 3144.26] for relying on
[3144.26 → 3144.46] information,
[3144.64 → 3145.60] tell us a little bit
[3145.60 → 3146.72] of a visit to
[3146.72 → 3146.78] The
[3146.78 → 3146.90] English
[3146.90 → 3147.80] opportunity.
[3147.80 → 3147.82] Thank you.
[3148.16 → 3149.44] We'll be GO' GE
[3149.44 → 3150.54] sting a few
[3150.54 → 3150.68] home now um
[3150.68 → 3152.14] and make sure
[3152.14 → 3152.60] some of the
[3152.60 → 3153.28] fullpleaanite
[3153.28 → 3153.86] of Liquid
[3153.86 → 3154.24] of Liquid
[3154.24 → 3154.32] easily.
[3154.32 → 3155.00] 먹고
[3155.00 → 3156.10] 하다
[3156.10 → 3157.14] Also,
[3157.14 → 3158.08] hit the
[3158.08 → 3158.52] temperature
[3158.52 → 3159.08] of Corner
[3159.08 → 3159.76] naught
[3159.76 → 3160.24] number
[3160.24 → 3160.58] an
[3160.58 → 3160.80] even
[3160.80 → 3161.78] zip
