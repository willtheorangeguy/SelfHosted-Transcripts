[0.00 → 3.14] Once again today we're joined by Brent. Hello Brent, how are you?
[3.40 → 5.04] Hey Alex, I'm good. How are you guys?
[5.38 → 9.40] Well we're fantastic now that you're here. It's always nice to have a little maple syrup flair.
[9.48 → 14.32] And you know what? I just got back from El Salvador and there was no maple syrup to be had.
[14.42 → 16.84] Except for at Wendy's. But you don't want their maple syrup.
[17.00 → 19.08] Makes sense. You made it back in one piece, huh?
[19.08 → 23.90] I did. I did. I'm feeling, towards the end of the trip I was actually feeling pretty good. Furthermore, I didn't really want to go.
[24.52 → 29.06] Just go figure, right? But that's just sort of how it goes sometimes.
[29.06 → 32.46] But I'm glad to be back because we've got a packed episode.
[32.74 → 36.48] Not only do we have a special guest coming up, the core developer behind Image.
[37.02 → 39.92] But Alex, you got some new gear in the Home Lab.
[40.26 → 44.72] It's been a veritable circus of UPS drivers the last couple of weeks.
[45.18 → 48.28] Not only did I get a new 3D printer, I got one of the Bamboo Lab ones.
[48.48 → 50.52] Which is awesome, by the way.
[50.80 → 56.64] I also got my 45 Home Lab server review unit sat on the desk here behind me.
[56.64 → 60.50] Big and chunky boy on the desk.
[60.68 → 62.44] It's like a 4U box.
[63.20 → 68.80] I'm trying to describe to you, you know, through the medium of audio, just how big this thing is.
[68.88 → 75.24] It's like one of those fractal, defined-sized cases just flipped on its side and kind of designed to go in a rack.
[75.88 → 80.46] They do ship rubber feet to go with this thing if you want to stand it upright vertically.
[80.46 → 85.76] One of the things I really like about it, actually, is on the front, there's a pair of captive thumb screws.
[86.14 → 89.02] So to get inside, they're on the front of the case.
[89.16 → 90.80] So imagine it's in a rack situation.
[91.04 → 93.38] You've got two captive thumb screws that you twiddle.
[94.94 → 98.58] And once they're loose, you just push the top of the case back a little bit and pop it up.
[98.62 → 101.00] And then you've got access to all the internals of the case.
[101.00 → 115.70] So they sent me the fully loaded unit, the one with the six-core Leon CPU in it, 32 gigs of RAM, one terabyte NVMe SSD, and also the 15 pre-wired drive bays, which is just fantastic.
[115.84 → 119.34] So this case, the build quality is the first thing that struck me, really.
[119.86 → 122.38] It is absolutely flawless.
[122.70 → 125.18] This thing is built like a tank, really thick.
[125.18 → 128.50] I assume steel, metal of some description, I assume it's steel.
[128.94 → 131.20] Really thick, good quality machining.
[131.64 → 132.54] No tool marks.
[132.64 → 134.32] The powder coat job is fabulous.
[135.46 → 140.80] It's up there with System76's build quality from when we took a tour of their factory a few years ago.
[141.08 → 143.24] I don't know about you, Chris, but I'm feeling all sorts of envy.
[143.60 → 143.92] I know.
[143.98 → 146.60] I'm thinking, boy, this sounds like a pretty nice rig.
[146.62 → 150.52] I actually do think I'd want to have it standing out on the table or something.
[150.60 → 151.72] Maybe I wouldn't want it in the rack.
[151.72 → 155.42] Like, within arm's reach, like Alex, you just give it a slap to prove it's actually there.
[155.42 → 156.54] Yeah, so you can give it a good smack.
[156.92 → 158.54] So that's the aesthetics of it.
[158.76 → 160.16] Have you taken it much further than that?
[160.26 → 161.80] Just first impressions, I assume, so far.
[162.16 → 170.34] Well, the CPU that's in there is a Leon 3204 from 2018 with a 1.8 or 1.9.
[170.50 → 173.56] The internet can't quite agree on the core base clock of this CPU.
[174.04 → 180.46] 32 gigs of RAM that's in there is ECC memory, and the one terabyte SSD is an NVMe one, as I mentioned.
[181.72 → 185.34] I find it fascinating that they went with a Leon CPU, and there's obviously some
[185.34 → 187.04] reasons why you would do that.
[187.30 → 192.24] If you look at the PCIe lanes that a Leon affords you, it basically enables them to put
[192.24 → 196.98] the HBA card directly onto the Supermicro motherboard that ships in this thing.
[197.08 → 199.50] It's an X11 SBH motherboard.
[199.50 → 203.66] I opted for the one with the SFP plus 10 gig a pair of Nix in it.
[203.80 → 208.16] They do make a standard RJ45 variant as well.
[208.16 → 211.04] Alex, I heard you say 2018 in there.
[211.42 → 213.64] Does that seem quite old these days?
[214.26 → 216.14] Yes, and there is no way around that.
[216.20 → 221.68] It's a six core CPU with no media encoding engines either, so there's no quick sync with
[221.68 → 222.12] this chip.
[222.72 → 228.46] That single decision led me down a bit of a path of thinking, who is this box for?
[228.86 → 233.22] Because when we had Doug and Mitch on a couple of weeks ago talking about how it's big, strong,
[233.22 → 239.82] fast, stable storage, all that kind of stuff, the performance for just storage is really
[239.82 → 240.30] good.
[241.60 → 246.82] But the minute I have a server on in my house 24-7, I'm looking at what else can it be
[246.82 → 247.14] doing?
[247.58 → 248.86] I want to be doing image.
[248.92 → 251.92] I want to be running image on it and doing a bunch of machine learning tasks on it.
[251.98 → 256.16] I want to be doing Jellyfin or Plex or whatever and doing a bunch of transcoding on it maybe
[256.16 → 259.64] for remote media streaming, that kind of stuff.
[259.64 → 266.48] And I find the choice of a six core CPU with a sub 2 gigahertz clock speed from five years
[266.48 → 268.54] ago peculiar.
[269.02 → 273.54] I understand that the choice of motherboard is probably what precipitated the choice of
[273.54 → 279.38] CPU because certain motherboards have certain features like HBA is built into them like this
[279.38 → 285.08] one does, and it supports up to 2 terabytes of RAM because it's a Leon chip, all this kind
[285.08 → 285.34] of stuff.
[285.34 → 289.08] There are a lot of very valid reasons for doing a Leon.
[289.64 → 294.44] However, if you're putting this in a home lab, it's in the name.
[294.58 → 296.40] It's probably going in my home.
[296.80 → 303.10] And for most people at home, you are using a box with 15 hard drive slots to store some
[303.10 → 303.92] kind of media.
[304.26 → 304.68] Probably.
[305.52 → 306.68] You might be a video editor.
[306.98 → 311.86] I can't imagine that's a huge use case, although certainly there will be a bunch of YouTubers
[311.86 → 316.38] that use this as their primary video editing storage system.
[316.38 → 322.58] But I've got to imagine that most people building these or using these cases to build servers
[322.58 → 328.24] are doing things like Unpaid and True NAS and perfect media servers, dare I say it, all that
[328.24 → 328.78] kind of stuff.
[329.22 → 334.56] And so why wouldn't you put a CPU in it that has hardware media encoding?
[334.56 → 340.22] It really confuses me as to the identity of the product a little bit.
[340.66 → 342.54] I bet it is predicated on the motherboard.
[343.14 → 348.94] And I wonder if just describing which motherboard and CPU are coming in the system sort of solves
[348.94 → 349.34] this problem.
[349.44 → 351.20] So then you just know before you pull the trigger here.
[352.12 → 354.36] And maybe some folks don't care about Quick Sync.
[354.86 → 355.80] I mean, that is a thing, right?
[355.84 → 360.66] You can just buy the chassis on its own, the case on its own, for about $800.
[360.98 → 365.10] So the fully loaded unit that they sent me, which, full disclosure, I did not pay for,
[365.60 → 367.02] the full unit is $2,000.
[367.42 → 370.52] They sell a version of just the case for about $900.
[370.52 → 373.92] And then the case and a power supply for $900.
[374.28 → 376.36] And then just the case is about $800.
[377.02 → 377.42] Right.
[377.62 → 380.70] So you could, I guess, get that one and put your own motherboard and CPU in.
[380.74 → 381.40] Absolutely, yeah.
[381.42 → 384.28] And if you look at what Wendell's up to on Level 1 Tech, that's exactly what
[384.28 → 384.76] he's doing.
[384.84 → 389.52] He's putting some like AMD Epic server chip in there and balls to the wall,
[389.64 → 391.66] fastest as NVMe it can possibly be.
[391.74 → 392.62] It's kind of nuts.
[393.24 → 394.04] I want that one.
[394.34 → 395.00] I want that one.
[395.30 → 401.50] But so this got me thinking about, you know, for $800, let's review just the chassis on its
[401.50 → 402.26] own for a second.
[402.40 → 405.22] For $800, what else could I buy?
[405.22 → 412.82] And the obvious choice for me, at least, is the Rosewall LSV4500U, which is a bit deeper
[412.82 → 413.56] and a bit longer.
[414.38 → 420.24] And it only has 12 drive bays with the hot swap loading out the front rather than out
[420.24 → 421.40] the top like this one.
[421.80 → 422.86] So, I mean, that's kind of a wash.
[422.94 → 426.06] Like if you want to load the hard drives in and out the front of the case without having
[426.06 → 429.42] to pull it in and out on rails, maybe you consider that a pro.
[429.84 → 435.52] If you like that kind of thing, then the 45 drives with 15 versus 12 is a pro for that
[435.52 → 435.72] one.
[435.72 → 440.10] So that's really a wash for me, the 12 versus 15 slots.
[440.56 → 441.08] I don't know.
[441.12 → 444.50] I think I'd probably rather have the 15 drives, and then I don't also have to put them in
[444.50 → 444.84] sleds.
[445.50 → 446.40] Yeah, that is a thing.
[446.48 → 450.60] I mean, the drive bays at the front of this thing are tool-less.
[451.02 → 451.82] So that's pretty cool.
[452.30 → 456.46] But, you know, the other thing I think about is five years ago when this CPU was birthed
[456.46 → 462.50] into the world, hard drive sizes were 8, 10, 12-ish terabytes.
[463.38 → 470.60] And so 15 slots back then was, air quotes, only 150 terabytes, which is still a hell of
[470.60 → 471.28] a lot of terabytes.
[472.48 → 477.66] Now, 20 terabyte hard drives are $300 a pop, which, okay, is not cheap.
[477.86 → 483.56] But in terms of a rational purchasing decision, you know, you could quite easily put 300 terabytes
[483.56 → 490.30] in this box now in that same density, which is, if you're using 300 terabytes at home,
[491.16 → 495.04] I'd love to know what for if it's a totally legal application.
[495.78 → 496.66] That's all I'll say.
[497.72 → 498.46] Oh, I could see it.
[498.70 → 499.44] I could see it.
[499.50 → 499.66] Yeah.
[499.74 → 504.26] These days, especially with large models and, you know, somebody wanted to bring all their
[504.26 → 506.28] media for a media production company.
[506.48 → 507.30] I could see it.
[507.74 → 513.46] I mean, again, you're talking, this is a device that lives between the consumer, like the
[513.46 → 516.30] NAS for consumers and the enterprise, right?
[516.46 → 519.04] This is a 15-drive bay system.
[519.34 → 522.40] And in the case with the fully loaded one, it comes with a 2018 processor.
[522.52 → 525.56] But that kind of makes sense if you're coming from an enterprise design standpoint.
[525.72 → 527.38] So it's for very serious folks.
[527.58 → 533.64] And an $800 starting entry point for just a chassis and the backplate for people that
[533.64 → 538.20] are pretty serious seems about right when you can put 15 drives in there, and you can put
[538.20 → 540.28] your own motherboard in there if you want and your own CPU.
[541.12 → 541.34] Yeah.
[541.40 → 542.88] I mean, that sounds kind of nice.
[543.82 → 546.52] It is a bit expensive, but it sounds really nice for people that are serious.
[547.16 → 550.10] It is absolutely a really nice bit of kit.
[550.26 → 551.76] It's a premium build quality.
[552.74 → 554.78] And I've got no complaints about it, really.
[554.90 → 560.64] I just wish that it was $500 or $600, not $800.
[560.84 → 561.30] Oh, yeah.
[561.30 → 566.64] And then it would be a totally different equation for me because at that price point, it becomes
[566.64 → 571.94] the de facto standard unit of deployment for home libbers and folks looking to build on
[571.94 → 573.94] RAID servers and that kind of thing.
[573.94 → 575.46] They came out with the HL12.
[576.46 → 578.86] You know, the HL12, 12 bays, $500.
[579.78 → 581.60] Because I don't really know if it's the slots you're after.
[581.76 → 583.76] It's you want something that's quality, right?
[583.86 → 585.12] You're going to put this in your home.
[585.20 → 585.48] Craftsmanship.
[585.48 → 586.82] It's going to have your home pictures on there.
[586.96 → 587.18] Right.
[587.54 → 587.86] Craftsmanship.
[587.86 → 587.98] Craftsmanship.
[589.04 → 590.16] I think that counts for something.
[590.72 → 594.84] It does, which leads me to a little bit of the software experience out of the box that
[594.84 → 596.52] I had some issues with too, unfortunately.
[597.04 → 600.46] So the image they shipped to me had Rocky Linux on the SSD.
[601.08 → 605.12] And the first thing I did was try to log in, as you can imagine.
[605.38 → 611.28] So first, I had to look for the PMI password, which was printed on a tiny little
[611.28 → 612.22] sticker on the motherboard.
[612.72 → 616.00] Their documentation, unfortunately, told me it would be printed on a white sticker on the
[616.00 → 617.68] side of the case that wasn't present.
[617.86 → 622.64] So I had to go spelunking on the internet and find that Supermicro motherboards, as of
[622.64 → 626.22] 2019, put this unique password on the motherboard.
[627.02 → 633.68] Then I spent a while trying to get that password in with the correct username of admin and then
[633.68 → 635.64] realizing that admin had to be all caps.
[636.78 → 637.82] It was case-sensitive.
[638.00 → 640.02] So it literally took me half an hour to turn it on.
[640.82 → 641.54] That's on me.
[641.72 → 644.24] Some of it, you know, but some of it's on the documentation too.
[645.08 → 650.30] Once I then got the system booted up, I was presented with a GNOME login screen.
[650.46 → 652.20] And I was like, oh, username 45 drives.
[652.28 → 657.72] So I look in the documentation for the Home Lab server, which is like 100 pages long.
[658.46 → 663.42] I had to get to page 61 before I found out what that username and password was.
[663.86 → 665.04] And it was wrong.
[665.04 → 668.54] It told me the username was root and the password was correct.
[668.92 → 672.30] But it was for the user 45 drives, not the user root.
[672.50 → 674.28] So, you know, some teething issues there.
[674.52 → 676.12] Nothing major.
[676.26 → 678.24] Just some small niggles to fix in the documentation.
[679.44 → 683.82] Then I loaded up the terminal once I got logged in and thought, cool, right, time to update
[683.82 → 687.34] packages as you do, like a reflex after you've used Linux for a long time.
[687.86 → 688.18] Absolutely.
[688.18 → 693.38] And I had to do dash skip broken dash fix something.
[693.54 → 698.20] I had to pass three different parameters to ignore all sorts of shenanigans that was going
[698.20 → 702.60] on with DNF in order to fix a bunch of outs of the box broken packages, which was a bit
[702.60 → 703.08] disappointing.
[703.84 → 704.10] Hmm.
[704.78 → 705.34] That is.
[706.46 → 710.78] I'm not, you know, I'm not sure if I'm actually even just thrilled with the choice of Rocky.
[710.94 → 711.26] I do.
[711.34 → 713.20] Again, I see it from the enterprise perspective.
[713.82 → 716.62] Well, I think they ship Rocky because they can do cockpit modules.
[716.62 → 722.52] And they've spent a bunch of time on their Houston UI, which is actually based on top
[722.52 → 723.14] of cockpit.
[723.36 → 727.20] And they've shipped some custom modules in there, which let you see which drive is in
[727.20 → 729.32] which physical slot on the system.
[730.16 → 733.44] Some proper system integrator level stuff, which is brilliant.
[733.58 → 735.42] That's exactly what I want to see at this price point.
[736.40 → 742.68] And then the only final niggle I had was I loaded up Firefox because it has a desktop.
[742.90 → 744.76] For some reason, this server comes pre-installed with a desktop.
[745.56 → 745.96] Whatever.
[745.96 → 746.50] That's fine.
[747.58 → 750.64] And Firefox had someone else's browser history in it.
[750.90 → 752.84] Presumably the tech that was setting up the server.
[753.18 → 757.26] Like it was looking at Supermicro fan control and a bunch of other stuff that they Googled
[757.26 → 759.52] and gone through the GitHub link and downloaded the script.
[759.70 → 765.60] And I was just thinking to myself, that cheapens it a little bit because I would have expected
[765.60 → 769.80] them to have a pre-made golden image with all of that stuff removed.
[769.80 → 774.40] And, you know, I come from the enterprise world with Red Hat for a long time when building
[774.40 → 779.86] those kinds of experiences, out-of-the-box experiences, is exactly what tools like Satellite and Ansible
[779.86 → 782.34] have been doing for years and years and years.
[782.40 → 785.34] And I just, I wonder why that wasn't done here.
[785.34 → 788.14] It was a custom-bespoke edition, Alex.
[788.46 → 789.46] Yeah, just for me.
[789.46 → 794.66] I would imagine, too, like that image is probably going to be something they're developing quite a bit.
[795.04 → 796.30] There'll be probably updates they're shipping.
[796.68 → 796.82] Yeah.
[796.82 → 800.22] But knowing you, I don't really see you wanting to run Rocky in production.
[800.34 → 802.26] Are you planning to keep Rocky installed on there?
[802.30 → 803.76] Or are you going to try going with something else?
[803.94 → 805.84] I want to try putting Nix on this bad boy.
[806.46 → 806.74] There you go.
[806.74 → 810.08] I actually want to do a full-on Nix OS server.
[810.44 → 816.92] One of the guys I work with has been showing me some really ninja-level stuff with Nix and
[816.92 → 822.64] System DN-Spawn containers and how he's configuring that with a helper script as part of his Flake setup.
[822.64 → 827.48] But I'll get in some details into that over the next few weeks, months, because it's pretty complicated
[827.48 → 829.02] and I'm still learning it myself.
[829.26 → 830.76] But it looks amazing.
[831.40 → 835.94] And isolated containers on the host as part of a Nix declarative config, Ada, Ada, Ada.
[836.56 → 836.76] Yeah.
[837.42 → 838.64] It's pretty cool stuff.
[838.86 → 839.28] I'm feeling it.
[839.34 → 842.12] That's why I want to do our server here at the studio as Nix.
[842.18 → 844.72] We almost went Proxmox, and then I started thinking about it.
[844.72 → 845.42] I'm like, wait a minute.
[845.64 → 847.28] We've missed the window, Chris.
[847.34 → 848.04] It's mid-November.
[848.14 → 849.30] We should have done Nix November.
[849.98 → 850.52] Yeah, I know.
[850.76 → 851.12] I know.
[851.56 → 852.02] I know.
[852.02 → 852.54] All right.
[852.64 → 853.66] Nix New Year, maybe.
[854.10 → 856.52] But so, I mean, really, you should have no problem, right?
[856.56 → 858.50] It's a standard PC.
[858.64 → 859.56] It's an x86 box.
[859.66 → 859.80] Yeah.
[859.96 → 861.24] Nix should just load right on there.
[861.36 → 865.88] It's just a Leon box with a CPU and memory, right?
[865.90 → 866.90] It's just a Linux box, right?
[867.02 → 867.68] At the end of the day.
[868.58 → 871.48] I know it's early, but I mark my words.
[871.48 → 879.44] In a couple of years, hardware vendors like 45 Drives and 45 Home Lab, and I also think IX Systems,
[879.44 → 887.56] they will realize that to achieve the level of quality and reliability they want, it will
[887.56 → 890.80] be in their best interest to ship this hardware with Nix OS.
[890.80 → 896.94] I had an absolutely fascinating conversation with an individual in El Salvador who's shipping hardware to stores.
[896.94 → 902.20] And by a process of elimination, they started with Debian and went through everything else.
[902.20 → 909.02] And by a process of elimination, they're now using Nix OS because of its quick ability to deploy, recover, and do all that stuff that they need.
[909.48 → 911.24] I think a lot of hardware vendors are going to get there.
[912.02 → 915.40] So, you know, you'll have to keep us updated on what it's like to run it on this machine.
[915.40 → 916.70] Well, I absolutely will.
[916.80 → 924.88] So I think the way I'm going to split my Home Lab up now is I'm going to keep my existing server with the i5-8500 CPU in it and Quick Sync.
[925.12 → 929.86] I'm going to keep that for all the mundane sort of media serving tasks that I have in the house.
[929.98 → 940.22] And then this one is going to be straight up like business suit and tie, you know, photo storage, Nextcloud, that kind of stuff that, you know,
[940.22 → 944.48] I'm going to throw a few hard drives in there and do ZFS, all that kind of stuff.
[944.64 → 951.06] So I think for me, it'd be nice to have that separation of duties as well between like a serious server and a fun server.
[951.48 → 952.32] Do I need it?
[952.42 → 955.14] No, but it is fun as hell.
[955.90 → 961.66] Alex, I often know when you're reviewing this kind of units, energy consumption comes to mind for you.
[961.74 → 962.60] Have you measured this yet?
[962.60 → 970.14] Now, whilst I don't have 15 hard drives to load this thing up with, what I can tell you is what the standby power consumption is,
[970.22 → 975.02] because this thing has a BMC built into it for proper PMI because it's a super micro server motherboard.
[975.88 → 980.66] So just turned off, plugged in with just the BMC on is 23 watts,
[981.50 → 987.24] which if you consider that is already more than most of those small form factor, like one litter PCs on its own.
[987.80 → 988.32] True.
[988.46 → 990.14] Gives you an idea of things.
[990.34 → 993.94] But better than those Dells that we have plugged in upstairs.
[995.00 → 999.18] Yeah, you can't throw two terabytes of RAM into a micro PC, can you?
[999.18 → 1009.20] I mean, the more we talk about it, I really see how this fits between like a one litter PC home lab machine and also like a huge used like super micro or old Dell or HP rack unit.
[1009.48 → 1014.64] Just powered at Rocky Linux, just at the desktop, no hard drives installed, nothing like that.
[1014.96 → 1016.74] Roughly, roughly 120 watts.
[1016.74 → 1024.00] It's a Leon at the end of the day, and that has some ramifications with energy usage.
[1024.14 → 1030.62] So if you compare that to like the i5-8500, for example, that's drawing 10 to 15 watts at idle.
[1030.82 → 1032.74] Okay, I've got a bunch of hard drives in that box too, but...
[1033.74 → 1038.06] That's again where it'd be really nice to have Quick Sync in that CPU, so you could throw a few more tasks at it.
[1038.06 → 1038.40] Yeah.
[1038.98 → 1041.88] Now, it's a server, so they've put server-grade fans in it.
[1042.10 → 1051.30] The CPU itself doesn't have any fans on the heat sink, so that should give you an idea of the level of noise that you can expect from the other fans in the chassis too.
[1052.04 → 1058.32] You could legitimately condition the air in your house with this thing if you put a HEPA filter on the front of it.
[1058.40 → 1059.52] The airflow is quite impressive.
[1059.52 → 1065.12] So a big thanks to 45 drives for sending that unit over for review, and you'll be hearing more about that in the upcoming episodes.
[1066.74 → 1068.72] Talescale.com slash self-hosted.
[1068.80 → 1071.52] Head on over there to get a free account for up to 100 devices.
[1071.70 → 1074.96] That's not a limited-time thing, and it's a great way to support the show.
[1075.02 → 1079.54] You get 100 devices, and you can see that Tale scale truly is simple and secure.
[1079.66 → 1081.76] And you know we love that it's built on WireGuard.
[1082.10 → 1083.68] It'll get up and running in just minutes.
[1084.22 → 1086.46] Tale scale's so great when you're travelling.
[1086.46 → 1094.54] I mean, it's fantastic if you just work from home, and you want to have a secure connection to maybe a VPS and something that's running on your local machine and a phone.
[1094.74 → 1098.52] You can kind of create your own mesh network across all those different networks.
[1098.60 → 1099.28] That's really handy.
[1100.00 → 1104.20] But man, oh man, when I'm travelling, oh boy, is it great.
[1105.04 → 1112.28] Knowing that every photo I was taking, every contact I was saving, everything was being synced securely over Tale scale to my next cloud box.
[1112.28 → 1119.72] That's a level of peace of mind that I just haven't really been able to describe before when I'm joining like an airport Wi-Fi in El Salvador.
[1120.72 → 1124.58] I just love knowing that all my information is protected by Tale scale.
[1124.84 → 1128.10] And Tale scale traversed double, gnat, like it's nothing.
[1128.60 → 1137.42] And when I'm switching between networks, going between weird cellular providers I've never heard of, and onto an Airbnb Wi-Fi, Tale scale never missed a beat.
[1137.42 → 1144.78] My connections between my servers, my computers, my mobile devices, even some of my appliances was just bulletproof.
[1144.88 → 1153.02] I was managing my power input on my Victory system using a subnet router on my LAN in my RV connected over cellular.
[1153.54 → 1156.24] And I'm doing it all from my phone while I'm travelling.
[1156.72 → 1159.62] It really is a great resource too for moving data back and forth.
[1159.72 → 1163.02] They have Tale scale send, which made it really easy to copy files back and forth.
[1163.02 → 1170.56] If you want to share resources with folks, you can either integrate it with your enterprise ACLs or if you're just an individual, some friends, they've got a system that works for you.
[1171.04 → 1174.98] It'll completely work when you're separated by firewalls and subnets.
[1175.08 → 1177.80] It's just, it really is the chef's kiss of networking.
[1178.22 → 1184.70] It's where I wanted to see WireGuard go when I first heard it get described way back in the day when it was just a twinkle in the colonel's eye.
[1184.70 → 1192.00] From arch servers to mobile devices, you've got to try it out, deploy it and see how fantastic it is to build your own private mesh network.
[1192.44 → 1194.98] Just go to talescale.com slash self-hosted.
[1195.10 → 1198.52] You can try it for free for up to 100 devices, really make sure it works for you.
[1198.92 → 1200.10] And it's a great way to support the show.
[1200.40 → 1203.50] So it's talescale.com slash self-hosted.
[1203.50 → 1210.14] Well, two weeks ago, we talked about the Verge cast and their big self-hosting podcast episode.
[1210.50 → 1214.94] And in that, they interviewed Alex, who is the lead developer for the Image project.
[1215.24 → 1221.34] Now, Image is ostensibly a Google Photos self-hosted replacement, or at least that's what it's trying to be.
[1221.74 → 1228.94] So Chris and I sat down with him to talk through the future of the project and the roadmap and also, you know, open source sustainability and that kind of thing.
[1228.94 → 1238.14] So we finally got Alex on the show, the developer of Image, and it's kind of great timing because version 1.8.6 just came out.
[1238.68 → 1240.52] And Alex, welcome to self-host.
[1240.70 → 1242.58] And sorry we haven't had you on the show before now.
[1242.94 → 1243.40] No worry.
[1243.52 → 1244.50] Thank you for having me.
[1244.58 → 1247.96] It's a pleasure to be here to talk to you guys and to talk about Image.
[1248.20 → 1251.24] Well, the new release came out just a couple of days ago as we record.
[1251.80 → 1255.12] It's got some nice features, I think specifically like around sharing, right?
[1255.22 → 1256.00] That is correct.
[1256.00 → 1262.70] Yeah, so this new release, we add the unified sharing for partners.
[1263.10 → 1266.96] So now if you have multiple partners, you can enable that option.
[1267.28 → 1271.00] So all the access of the partners is also showing on your timeline.
[1271.64 → 1276.34] And this makes browsing experience a lot better.
[1276.46 → 1282.04] So you don't have to switch to the sharing tab and then click on each partner to see the new media.
[1282.18 → 1283.78] But now just in your timeline.
[1283.78 → 1287.44] But there are a lot of caveats as this is the basic version.
[1288.04 → 1292.04] The searching is not including the partner media yet.
[1292.82 → 1300.24] And the only thing to share on that media is the location for now.
[1300.66 → 1305.36] That's fantastic because if you think about how most people actually use a photo solution, right?
[1305.40 → 1307.60] My wife is taking pictures of my kid.
[1307.60 → 1312.96] I'm taking pictures of my kid and we probably both want to see pictures of our kid, right?
[1313.04 → 1314.90] And so it's a family unit thing.
[1315.16 → 1324.68] And a lot of the self-hosted solutions to date don't really take that multi-user within a single household, a single family into account.
[1324.76 → 1326.68] So I'm absolutely thrilled to hear that you guys are.
[1326.68 → 1327.42] Thank you.
[1327.54 → 1332.42] And I think this is coming from a lot of my own use case as well.
[1333.42 → 1335.06] Scratch your own itch.
[1335.12 → 1337.40] That's the best way to develop software, in my opinion.
[1337.74 → 1337.86] Yeah.
[1337.92 → 1349.16] And then we add the new map tire server to moving away from using the free tire server from OpenStreetMap as their usage policy.
[1349.16 → 1357.58] I thought that was hilarious when I looked at it because you were like, well, when we were just a small scrappy project, we could get away with using it for free.
[1357.64 → 1359.02] But now we're kind of a big deal.
[1359.38 → 1362.14] So we kind of need to do this properly by the book.
[1362.14 → 1362.54] Yeah.
[1362.74 → 1374.18] The community, there are some concerned that asking us that we should move away as soon as possible to not overuse their free resources.
[1374.18 → 1379.48] And, yeah, we take this change, and we move away to a different map tire server.
[1380.44 → 1385.34] And it's also giving us the opportunity to build our own layers.
[1385.60 → 1391.20] So to make it look slicker on the dark and the light mode.
[1391.78 → 1392.42] I think it does.
[1392.62 → 1393.78] I think it does.
[1394.14 → 1402.10] So I want to talk about the audacity of the project for just a moment because the idea of trying to replace Google Photos kind of seems like an impossible task.
[1402.10 → 1410.54] And yet version 1.86, getting pretty far now with face recognition, sharing support, the location.
[1410.68 → 1413.80] When I was looking at my pictures from my trip, the new map stuff is really slick.
[1414.28 → 1418.78] So you are kind of in a transition phase now to a big project, right?
[1419.28 → 1420.54] Yeah, I would say so.
[1421.46 → 1430.12] Just to look at this core member because they kind of group the new user coming in by day.
[1430.12 → 1432.84] So when you look at it, you can see it grow.
[1433.92 → 1441.68] And when I first started this core, we might have one or two new people coming into the server every day.
[1441.78 → 1445.78] And now when you look at it, it can reach like 20, 40 people.
[1446.94 → 1455.02] And then the star on GitHub is also the indication of how the project getting more popular.
[1455.02 → 1463.68] And also I more often than I would admit that I would browse the Internet to see how people are talking about image.
[1464.08 → 1466.72] And yeah, we've seen a lot of chatting.
[1467.10 → 1471.90] And most of the crows are coming from words of mouth.
[1472.18 → 1473.86] Yeah, it's coming up online all the time now, though.
[1473.94 → 1480.52] I feel like I see it getting mentioned every week at least by some different group online saying they're using it to replace Google Photos.
[1480.52 → 1484.32] People are recognizing it for a genuine replacement.
[1484.66 → 1485.56] It's pretty exciting.
[1485.64 → 1486.64] I just wanted to say congratulations.
[1487.66 → 1488.00] Thank you.
[1488.32 → 1491.92] Yeah, one of my goals is to build something for myself.
[1492.64 → 1496.34] And funnily enough, image maybe what it is.
[1496.34 → 1507.10] You and I have crossed paths a couple of times on Reddit, I think, in the past and talked about your funding model in particular in terms of a sustainable model for an open source project.
[1507.20 → 1512.98] I mean, we've seen Home Assistant with Zebu Casa, for example, build a company around an open source project.
[1512.98 → 1525.48] I think we've also discussed in Cross Paths that something like this photo solution is so big in scope that you do almost need a company to support it.
[1525.60 → 1529.88] Like, you've obviously done amazing work, and you've got some fantastic contributors to date.
[1530.02 → 1537.56] But I wanted to ask you what the plans are for the future of image as a project and also as a sustainable project in open source.
[1537.56 → 1547.80] So I think there are one thing that I want to not pivot off is to not making it into some type of paywall.
[1548.16 → 1556.08] Like some of the open source projects starting out as open source, and then they got funding from outside investor.
[1556.30 → 1559.54] And then they got that money pressure to eventually have to make money.
[1559.66 → 1562.56] So they kind of pivot off the first original idea.
[1563.90 → 1567.44] So I don't want to do that for image at all.
[1567.44 → 1571.72] I want to make it as, you know, something good, something people enjoy using.
[1572.02 → 1575.84] So that is something that we would never like to move away from.
[1576.60 → 1582.62] The core team has talked about maybe eventually after the service, the app is more stable.
[1583.18 → 1589.30] We could think of building a hosting solution for other people.
[1589.30 → 1593.04] So people that would like to use image but don't want to host it themselves.
[1593.04 → 1603.42] So I think that is the this might be the only way right now to make it as a sustainable business.
[1603.42 → 1616.82] But by not making it as the main income source at home for all of us, I think that's making it as a sustainable project that keep growing.
[1616.96 → 1620.76] Because we don't have to depend on it for our livelihood, right?
[1620.84 → 1628.46] You still have your day job, and you still dedicated your time outside of job in order to build image.
[1628.46 → 1633.46] And it's a joy to do that as something.
[1634.28 → 1645.82] I think the whole core team really enjoy because we have such a nice group to chat about technology, code, and just how to beat Google.
[1645.82 → 1648.80] You love to hear that, right?
[1649.24 → 1657.90] And really, it's great that while you grow the project and get it to that point where it's stable enough that it could be a product that you do have the support and income of a day job.
[1658.46 → 1663.60] And maybe one day those two things merge and image becomes a bigger part of your income source.
[1663.60 → 1677.70] Yeah, and that's what I strive to achieve is when it gets to that point where I can replace the income source of image into my own, that I can support my family and the growth of my family.
[1677.86 → 1679.52] Then that would be fantastic, right?
[1679.62 → 1684.60] You got to work on something you love, you make good things for people, and then you also get to earn money from it.
[1684.90 → 1686.62] Yes, that would be absolutely fantastic.
[1686.86 → 1690.12] So how could people support the project today?
[1690.12 → 1701.92] So today there's only donation means to support the project besides testing and reporting bugs to help us develop the project better.
[1702.22 → 1713.20] So you can support the project financially from GitHub sponsor or from Liberapay or buy me a coffee.
[1713.34 → 1716.86] I drink a lot of coffee, so keep the coffee coming.
[1716.86 → 1727.26] Now, in the Verge cast interview that we talked about on the last Self-hosted episode, you're now a super famous big deal developer, right?
[1727.30 → 1729.34] And the big time on the Verge cast podcast.
[1729.48 → 1730.20] I wouldn't say so.
[1731.94 → 1739.62] You talked a little bit about your architectural decisions about splitting it out into microservices and a bunch of Docker containers and stuff like that.
[1740.50 → 1745.56] Is there anything you wish you'd done differently now or are there any big changes coming down the pike?
[1745.56 → 1763.68] Yeah, so the goal is to consolidate some of the services like the proxy container and a web container to put that into the server container to make it less scary when people are looking at the Docker Compose file because those can be done.
[1764.60 → 1769.84] But when I started it, it makes sense to split it up at that moment.
[1769.84 → 1784.06] And now we might have found a way just today to make the web not server-side rendering anymore while still keeping that really snappiness when using the app.
[1784.34 → 1790.38] So with microservice architectures, you have the potential for remote workers and stuff like that.
[1790.42 → 1790.68] Correct.
[1790.68 → 1795.30] I mean, I would love to see it where I could distribute the facial recognition, you know.
[1795.58 → 1805.08] So I just dumped, for example, like three or four terabytes worth of photos into Image in the last couple of months because you guys are awesome and added external library support, which is amazing.
[1805.50 → 1806.30] Chef's kiss.
[1806.50 → 1806.96] Thank you.
[1807.34 → 1813.14] But it took like two or three weeks for it to chew through all of those images that I had.
[1813.54 → 1815.20] I've got lots of CPUs in this house.
[1815.20 → 1819.86] It would have been great if I had an easy way to distribute that task throughout all my systems.
[1819.86 → 1830.32] Yeah, so actually the idea of breaking down microservices, different containers, handle different things is exactly to serve this use case.
[1830.78 → 1836.22] So as of now, you can run the machine learning on a completely different machine.
[1836.86 → 1842.72] And if you put a front-end upload balancing on it, then you can distribute it on multiple nodes.
[1842.72 → 1852.36] Because we are not accessing the file on that container, but you are sending the file to those containers.
[1852.56 → 1856.48] And then it would do the referencing and then sending back the data that it needs.
[1857.42 → 1865.54] The microservices is a little bit more involved because you would need to be able to see the file system,
[1865.90 → 1870.10] see similar to the server so that it can access and do the transcoding stuff.
[1870.10 → 1873.82] But if you have network mounted, you can also do that already.
[1874.34 → 1878.52] Pretty typical distributed network storage replication problem there.
[1878.66 → 1878.88] Yeah.
[1880.02 → 1887.04] But I think the architecture has been designed exactly for that purpose.
[1887.30 → 1889.98] And we have a lot of people that already do that.
[1890.14 → 1894.90] I think that will help you guys as you move towards eventually a hosted service.
[1895.26 → 1897.66] You'll be able to pick the cheapest VPS provider that week.
[1897.66 → 1898.02] Yeah.
[1898.52 → 1899.38] You know what, maybe?
[1900.10 → 1902.24] Yeah, we've got a great coupon code you can use.
[1904.32 → 1908.06] Well, I think for me and probably a lot of people listening, I know Alex too,
[1908.12 → 1915.18] this is one of the tools that has really been the key to googling so much of my private information.
[1916.20 → 1918.66] And so privacy and security is super important.
[1918.72 → 1925.26] I'm just kind of curious to know your thoughts around enabling sharing but keeping people's images safe and secure
[1925.26 → 1927.64] and how that kind of works from a back-end perspective.
[1927.64 → 1930.92] Is your question more about at home?
[1931.28 → 1931.38] Yeah.
[1931.46 → 1936.96] Like say if I wanted to share an image with somebody, would there maybe be like a back-end service,
[1937.10 → 1941.26] like down the road, some sort of intermediary that would be the go-between to share the image
[1941.26 → 1943.98] so I wouldn't have to expose, say, like my home machine or something?
[1944.48 → 1949.16] I'm trying to think of ways of sharing images where I don't link someone to my image instance.
[1949.16 → 1955.86] That sounds challenging at the moment, but anything might have a solution.
[1956.66 → 1962.12] We're on video chat with Alex, dear listeners, and I can see the cogs turning right now live as he's thinking,
[1962.36 → 1966.52] what if we had some kind of like remote cloud, you know?
[1966.76 → 1967.76] Yeah, that's what I'm wondering.
[1967.76 → 1970.40] Like VPS linked up or something, you know?
[1970.86 → 1971.90] That's a great idea, Chris.
[1972.22 → 1973.46] Feature request right there.
[1973.52 → 1978.58] Turkey Day is coming, and I'm thinking something that I could, like a page that would be generated
[1978.58 → 1980.92] that I could share with family, but I wouldn't have to link them.
[1981.58 → 1983.86] They wouldn't all be necessarily loading it from my direct server.
[1984.30 → 1984.62] I see.
[1984.62 → 1990.42] So in that page, you would talk to the image server at home, but that is abstracted in the background,
[1990.42 → 1996.44] and then it would use the image API in order to pull those, just like a proxy, right?
[1996.50 → 1997.62] Just like a proxy page.
[1998.18 → 2006.42] Eventually, this is something that we want is to build a plugin system for people to build things around image.
[2007.30 → 2011.32] The API is compatible with a lot of the languages.
[2011.32 → 2021.78] So we use OpenAI, so it can generate SDK for Python, for JavaScript, for Rust if you want,
[2021.92 → 2023.74] for anything that you could think of, right?
[2023.98 → 2028.86] And then they can use that in order to talk to their server, the image in instant.
[2029.58 → 2034.70] And now one of the we have one perfect tool I would like to mention here is called Image Go.
[2034.70 → 2036.76] It's from Simulate.
[2036.90 → 2039.16] It has Discord handle.
[2039.16 → 2042.64] It's a CLI tool.
[2042.92 → 2045.54] You point it to your Google tech out.
[2045.78 → 2049.16] You don't even have to extract all the zip file that you download.
[2050.02 → 2056.44] It unzips it, and then it parses all the metadata from that JSON file that Google gave you,
[2057.04 → 2063.70] and then upload everything into Image and create the album that come in your Google account.
[2064.08 → 2066.20] So it's just like one click, go.
[2066.20 → 2066.24] Wow.
[2067.20 → 2068.12] That's so neat.
[2068.90 → 2069.26] Yes.
[2069.60 → 2070.34] I love that.
[2070.46 → 2074.50] See, that plugin system, if that really extended, could be a solution because people could build
[2074.50 → 2075.04] things around that.
[2075.06 → 2078.92] Because that's, when I really A, B, what I miss from Google Photos is like a way to share
[2078.92 → 2083.56] photos, and I'm not like sharing any of my personal infra, but something down the road,
[2084.00 → 2086.28] like a plugin system, there are all kinds of ways to solve that.
[2086.28 → 2090.02] I'm thrilled to hear that you guys are thinking more about that, too.
[2090.34 → 2092.76] It's going to be an exciting future as an image user.
[2092.76 → 2094.20] It absolutely is.
[2094.50 → 2095.98] Now, I have another question for you, Alex.
[2096.56 → 2101.62] Ever since the beginning of the project, there's been a banner in your documentation and on
[2101.62 → 2106.96] your website that says, here be dragons, do not do anything serious with this project
[2106.96 → 2108.82] because it's still under very active development.
[2109.60 → 2114.18] Do you have any sense as a timescale as to how long before we can actually start to,
[2114.64 → 2116.70] air quotes, depend on Image?
[2116.70 → 2121.80] You know, in this court, we have a funny way of saying that it's the any ETA question
[2121.80 → 2124.32] is a prohibited question.
[2124.62 → 2126.34] We don't talk about that here.
[2127.52 → 2128.84] Yeah, that's fair enough.
[2129.02 → 2131.18] Don't commit to deadlines on air in particular.
[2131.40 → 2131.82] I get it.
[2132.32 → 2137.68] We put that because part of it is Image is very active in development, right?
[2137.68 → 2144.28] It's like just this last release, the first time ever, we pushed out the first release
[2144.28 → 2148.96] that if you don't, if you're not on the same version, you cannot access the instance from
[2148.96 → 2156.20] your phone at all because we changed the underground, the underlying API.
[2156.86 → 2161.94] That the only way to resolve the difference is to log out and log back in on the same version.
[2161.94 → 2168.54] Things like this could happen because we are striving to go to the industry standard for
[2168.54 → 2169.74] the code base.
[2169.84 → 2176.30] If anything that we see can be improved for the better future of Image, we will do that.
[2176.60 → 2182.72] And since there are many, many things that we still can improve, we don't want to prohibit
[2182.72 → 2187.08] us to backward compatibility at the moment.
[2187.08 → 2199.16] But people are striving to get to the point of feature freeze or when the core architecture
[2199.16 → 2204.40] is more stable, we would like to eventually remove that banner.
[2205.12 → 2208.70] I think we all just see the potential of the product and want to start using it.
[2209.24 → 2210.00] I say product.
[2210.14 → 2211.46] It's not a product, project.
[2211.46 → 2217.48] And we just want to start using it today because we're all fed up with the cloud nonsense and
[2217.48 → 2222.74] giving our, you know, machine learning overlord model, you know, so much data.
[2223.28 → 2227.56] So I think that's the only pressure really from us is that we kind of wish it already existed
[2227.56 → 2232.36] because the pressures that forced you to create it in the first place are quite powerful.
[2233.02 → 2233.80] Yeah, very tempting.
[2234.02 → 2235.42] They're tempting fruit, aren't they?
[2236.08 → 2238.78] Alex, I'm going to keep using it even with that banner on there.
[2238.78 → 2241.64] So there, and thank you so much for a career.
[2241.72 → 2244.28] And thank you to the entire team and everybody that works on it and contributes.
[2244.56 → 2244.80] Absolutely.
[2245.08 → 2248.18] I know a lot of us in the self-hosted community are just extremely grateful.
[2248.30 → 2250.08] Yeah, I would like to shout out to the team too.
[2250.42 → 2252.74] Everybody in the team is great.
[2253.00 → 2254.26] They're coming from different backgrounds.
[2254.40 → 2255.70] We have students from Europe.
[2255.88 → 2261.64] We have people working in application security, some 11x developer.
[2261.64 → 2264.88] So the whole team is great.
[2265.04 → 2270.24] And people are very, you know, welcoming and willing to teach each other.
[2270.94 → 2279.98] So I want to keep this mindset growing in order to attract more contributors and just to make it a good place to be,
[2280.20 → 2283.62] not just from using the application, but from developing the application as well.
[2283.62 → 2289.36] And so if you'd like to contribute, you can go to GitHub.com and image-app, I believe, is the place to go.
[2289.48 → 2291.16] You've got a couple of hundred contributors already.
[2291.36 → 2292.88] A few more wouldn't hurt, right?
[2293.70 → 2294.02] Yep.
[2295.20 → 2298.08] So a big thank you from me and Chris for joining us on the show today.
[2298.26 → 2301.58] And I'm sure this won't be the last time that you check in with us.
[2301.64 → 2303.52] But until next time, thank you very much.
[2303.66 → 2304.16] Thank you, guys.
[2304.28 → 2304.76] Thanks, Alex.
[2304.90 → 2305.48] Thanks, Chris.
[2305.56 → 2306.76] You guys have a wonderful night.
[2306.76 → 2310.30] Linode.com slash SSH.
[2310.46 → 2312.84] Linde is where we host everything in the cloud.
[2312.98 → 2316.30] And now Linde is part of Akamai, the Akamai.
[2316.40 → 2320.94] But with all the tooling, the UI that we like, the CLI that's super handy,
[2321.04 → 2326.34] all that stuff that you can use to build, deploy, and scale in the cloud, that's still there.
[2326.76 → 2330.06] It's just now they're combined with the power of Akamai's global reach.
[2330.06 → 2332.36] They are the premier network out there.
[2332.36 → 2337.74] And Akamai is expanding their cloud services, expanding tooling,
[2338.24 → 2343.72] but keeping things affordable, reliable, and scalable for users of any size,
[2343.80 → 2345.80] an enterprise or an individual project.
[2346.02 → 2349.40] And something we've taken advantage of in the last month is the expansion of the data centres.
[2349.54 → 2352.64] They're expanding worldwide to give us more access to more resources
[2352.64 → 2355.38] so you can grow your project or your business.
[2355.62 → 2356.18] So why wait?
[2356.30 → 2358.88] Go see why Linde is the only cloud provider we recommend.
[2359.06 → 2361.52] Experience the power of Linde, now Akamai.
[2361.52 → 2363.88] Go to linode.com slash SSH.
[2364.00 → 2368.10] That supports the show, and it gives you a $100 credit so you can really kick the tires.
[2368.46 → 2372.72] So go see how Linde, now Akamai, can help scale your applications from the cloud to the edge.
[2372.86 → 2375.62] That's linode.com slash SSH.
[2377.16 → 2378.52] Well, it's that time of year, Brent.
[2378.56 → 2381.22] You messaged me saying, I want to buy some hard drives.
[2381.36 → 2385.58] And I couldn't refuse the opportunity to sit down with you and discuss hard drives.
[2385.66 → 2388.58] It's literally my specialist favourite subject in the whole world.
[2388.58 → 2391.84] Once a year, you get all giddy about getting new hard drives.
[2391.88 → 2393.24] And I thought I'd join in this year.
[2393.94 → 2395.08] So here's part one.
[2395.56 → 2400.18] Brent and I sat down and recorded a few different segments to use over the holiday season,
[2400.40 → 2406.02] discussing his journey into buying hard drives, some purchasing considerations, all that kind of stuff.
[2406.44 → 2412.18] I'm going to put part two in today's post show, which I believe, Chris, we have a special offer for our members.
[2412.18 → 2415.24] It is the Black Friday season after all.
[2415.30 → 2418.48] So if you've been thinking about becoming a member and support the show, and you want to get that post show,
[2418.78 → 2425.22] use the promo code Black Friday, and you'll get $2 off a month for a whole year of the SRE membership.
[2425.62 → 2431.30] Just go to self-hosted. Show slash SRE, and it's promo code Black Friday, all one word.
[2431.58 → 2434.58] And then you get the post show, and you get a post show every single episode.
[2434.58 → 2446.58] So all the way back in 2019, October 2019, four years ago, Brent, you and I sat down with Antonio, the developer for Mergers.
[2447.00 → 2454.20] And you professed to me in that episode and public record, no less, that you wanted to take storage more seriously.
[2454.38 → 2455.54] And here we are four years later.
[2455.58 → 2459.10] And I think it's about time we cashed that check.
[2459.10 → 2459.42] Huh?
[2459.58 → 2461.52] No, it's long overdue, Alex.
[2461.64 → 2466.14] And I admit it had been on my mind for four years previous to that as well.
[2466.32 → 2468.96] So I am in bad shape.
[2469.02 → 2471.54] Because we were talking about this before we pressed record.
[2471.86 → 2477.48] And you said to me, I've been buying drives with ZFS in mind in pairs for like the last eight years.
[2478.12 → 2479.18] No more than that.
[2479.26 → 2487.06] Like since my photography career required it, which is, you know, I had been doing photography for 18.
[2487.06 → 2493.64] So I've got like paired one terabyte drives and paired 500 gig backup drives.
[2493.80 → 2496.66] Like basically anytime I'd buy drives, I would try to pair them.
[2497.00 → 2500.52] Because I knew one day I would be smart enough to actually do something about it.
[2501.40 → 2502.62] And that day is today, is it?
[2503.48 → 2504.70] Well, I'm hoping it is.
[2504.82 → 2509.38] But my level of success so far is challenging at best.
[2510.20 → 2511.82] Well, OK, let's start at the beginning.
[2512.16 → 2513.18] You mentioned photography.
[2513.18 → 2517.34] Now, I know that's a career path that was huge for you previously.
[2517.34 → 2525.94] But now, obviously, with your next cloud work, I would imagine your data generation is a little, you know, the velocity is a little slower on that side of things.
[2526.30 → 2530.00] What kinds of stuff are you looking to store at the moment?
[2530.86 → 2531.88] Yeah, it's a good question.
[2531.88 → 2539.18] I think most of my data, at least the big stuff at this point, is archival, to be honest.
[2539.54 → 2543.42] Like it can just sit there and won't get accessed very often.
[2543.60 → 2546.08] And it's a read only probably kind of scenario, if ever.
[2547.10 → 2548.68] OK, so that leads me into my next question.
[2548.98 → 2553.68] If it's archival, do you genuinely need it to be always on?
[2554.80 → 2555.62] Always accessible?
[2555.62 → 2556.34] Hmm.
[2556.78 → 2561.38] I hadn't even considered that because I had just pictured all of my storage being in one box.
[2561.86 → 2563.10] But tell me what you have in mind.
[2563.42 → 2571.56] If it's an archival situation, it's not beyond the realms of possibility that you've got a client ringing you up that you had on the books 10 years ago that says,
[2571.56 → 2573.50] you know that shoot you did in our mine?
[2574.24 → 2579.16] Could you find that particular, you know, shot of Fred or whatever?
[2579.38 → 2580.38] I've gotten those emails before.
[2580.64 → 2581.56] Yeah, I'm sure you have.
[2581.56 → 2587.56] And you think, right, well, if I just, you know, write down what's on each hard drive, external hard drive in a drawer, for example,
[2588.38 → 2591.30] that could be a legitimate filing system for that data.
[2591.94 → 2600.86] The issue with that is Bit Rot is a thing and that keeping those drives just sat in a hard drive, you know, they're not going to last forever.
[2601.70 → 2610.40] So you could explore something like Amazon's Glacier service, which is a cloud-based long-term archival situation.
[2610.40 → 2611.98] It's fairly cheap.
[2612.20 → 2614.60] They do kind of hit you on the retrieval fees.
[2614.72 → 2619.20] But if this is an archival situation only, maybe it's a decent option.
[2619.88 → 2623.18] I hadn't considered that at all as my primary source of storage.
[2623.32 → 2628.26] I had only considered Cloud Solutions as kind of off-site copy.
[2628.26 → 2635.78] I think mostly because I have, I don't know if I trust them with the primary data.
[2636.00 → 2637.26] Is that one way to look at it?
[2637.28 → 2641.46] But you're suggesting maybe I have drives in a drawer and also some data there.
[2641.56 → 2642.32] Is that what you're suggesting?
[2642.80 → 2643.56] It could be.
[2643.78 → 2648.04] I mean, the other option is you just have all of that data running all the time in your house.
[2648.04 → 2654.92] And it's always available on top of ZFS so that you've got all the checksumming and beautiful magic that ZFS gives you for data integrity.
[2655.74 → 2657.60] And then you back that up to Glacier.
[2657.84 → 2665.52] And the purpose for suggesting that is it would reduce the complexity for you somewhat in terms of having to have a box at a remote house with,
[2665.52 → 2677.88] as I found out fairly recently, having a remote box in a different country or a different side of the country even, even if it's in a family house, it's hard sometimes to get access to that.
[2678.30 → 2683.74] And, you know, the economics of something like rsync.net don't really work out.
[2683.90 → 2689.20] You know, seven or eight terabytes in rsync.net is $70 or $80 a month.
[2689.30 → 2690.22] Oh, I see what you're saying.
[2691.22 → 2695.30] Which pays for a remote backup server in no time at all.
[2696.20 → 2702.78] But Glacier is, from memory, it's $10 for a similar thing or less per month.
[2703.50 → 2706.08] Like I say, the way they get you is on the retrieval.
[2706.16 → 2717.20] So if you try and do an expedited retrieval, they'll charge you $10 for 1,000 API requests versus just a standard rate of $0.03 per 1,000 requests.
[2717.60 → 2718.86] Hence the name Glacier.
[2719.22 → 2723.76] Because it's like, only if the world is going wrong do you want to melt that thing.
[2723.76 → 2727.46] Yeah, they've never actually published what the underlying storage technology is.
[2727.56 → 2730.86] I suspect it's tape, but we don't actually know.
[2731.28 → 2742.98] And so it would make sense because I would, you know, I'd imagine they have those tapes in some kind of robot automation system that can actually move a physical piece of media in and out of a specific location.
[2742.98 → 2747.78] And if you're doing an expedited recovery, that probably means some S hit the fan somewhere.
[2748.40 → 2750.26] And you need that stuff back pretty quick.
[2750.74 → 2751.14] All right.
[2751.18 → 2757.18] So let's leave Glacier for a second and talk a little bit more about your local hardware desires.
[2757.18 → 2760.44] You send me a list of all the hard drives you've got.
[2760.50 → 2764.08] And let me just read this to the audience because it's quite glorious.
[2764.24 → 2765.24] I think you're going to enjoy this.
[2765.30 → 2765.76] Is it really?
[2766.10 → 2766.52] Yeah.
[2766.76 → 2767.70] I liked it.
[2768.26 → 2772.08] There is a Western Digital 8TB drive, brackets, shucked.
[2772.84 → 2775.30] A Western Digital Red 4TB drive.
[2775.70 → 2778.62] A Western Digital Caviar Black 2TB drive.
[2778.62 → 2781.92] Three Seagate 1.5TB drives.
[2782.56 → 2785.74] Two Western Digital Caviar 1TB drives.
[2786.26 → 2788.58] And two 500GB drives.
[2788.72 → 2789.56] How many is that?
[2789.68 → 2792.22] One, two, three, four, five, six, seven, eight, nine, ten.
[2792.48 → 2793.38] Ten drives, Brent.
[2793.68 → 2795.24] That's quite a lot.
[2795.42 → 2803.88] Unfortunately, this doesn't include any of the two and a half inch like external drives that I've been carrying on all my travels to do, you know, local backups as I go.
[2803.88 → 2805.36] So there are a couple more of those.
[2805.36 → 2808.86] So maybe we should throw in the mix, but they might not be useful in this setup.
[2809.00 → 2809.24] I don't know.
[2809.80 → 2817.40] And then the next line in our little chat exchange was, but there's data duplication, inefficiencies galore, etc.
[2817.62 → 2821.40] So really, I have no idea quite how much storage I have.
[2822.08 → 2827.84] So if we add all of that storage up, dear listeners, it comes to approximately 21.5TB.
[2827.84 → 2836.00] But your guesstimating on the use of that is somewhere between 8 and 13TB?
[2836.48 → 2836.98] Is that right?
[2837.70 → 2837.90] Yeah.
[2838.08 → 2845.24] I think part of the challenge here is that these drives were never all available at the same time.
[2845.24 → 2850.38] And so they ended up being generations of storage for me.
[2850.50 → 2856.28] You know, someone fill up, and then they would go on, let's call it long term storage and be replaced.
[2856.66 → 2863.82] And as they filled up, depending on how busy I was at the time or what, it would just kind of get slotted in.
[2863.82 → 2867.30] And so the data is not extremely well organized.
[2867.42 → 2870.58] You know, it's organized as well as I could muster along the way.
[2870.76 → 2878.04] But because of that drive swapping, there's also duplicates of stuff, especially with system backups and things like that.
[2878.14 → 2881.12] There are multiple, multiple copies of that kind of data.
[2881.66 → 2886.96] And photography projects, sometimes, you know, on one set of drives, there's a project that was half finished.
[2887.04 → 2890.38] And on the next set of drives, there's the whole project that was finished or something like that.
[2890.38 → 2899.46] So I think if, you know, we approach this intelligently and got rid of all those duplicates, I would imagine there's way less data than I think there is.
[2899.56 → 2902.68] But to be honest, I'm just human and I have no idea.
[2903.26 → 2905.36] You know, what's interesting is I think we've all been there.
[2905.46 → 2908.74] We've all found an old hard drive in a drawer and gone, hmm, you know what?
[2908.76 → 2909.72] I should back this up.
[2910.06 → 2912.44] And then a couple of years elapse.
[2912.58 → 2915.34] And then you find that same hard drive in a drawer, and you go, you know what?
[2915.36 → 2916.68] I should back this hard drive up.
[2916.68 → 2923.82] And before you know it, you have that hard drive in triplicate somewhere named slightly differently, you know, every time.
[2924.38 → 2930.46] Well, the thing for me is like this is just another iteration of my trying to get that great solution.
[2930.58 → 2933.10] I mean, you've got perfect media server, right?
[2933.18 → 2942.12] And I've had various versions of tons of hard drives in a box and various versions of having it be functional for me.
[2942.12 → 2953.64] But it never quite got to the point where I felt really comfortable about the data and that it was, you know, being checked for parity and that if a drive failed, that it wouldn't lose anything, etc., etc.
[2953.80 → 2960.18] So I still, despite my, you know, knowing better and my efforts, I have a long way to go, I feel like.
[2961.02 → 2962.32] Which is embarrassing, to be honest.
[2963.10 → 2966.92] Well, in that case, my suggestion is keep it simple.
[2966.92 → 2973.98] Do a pair of disks in a ZFS mirror and then never think about it again.
[2974.30 → 2976.16] I mean, obviously monitor them and all that kind of stuff.
[2976.22 → 2982.54] But what I mean in terms of you're worried about like checksumming and all that kind of stuff and parity and then data integrity.
[2983.18 → 2989.60] ZFS gives you all of that out of the box because it doesn't actually care about specific files.
[2989.60 → 3002.00] ZFS cares about the blocks, the data blocks, and it checks that if a specific block is read from disk and doesn't match the checksum it expects between the two mirrors, it will go away and figure out what the right one is.
[3002.06 → 3011.08] And then if it can't give you the fully integral data, it just won't give you that piece of data at all.
[3011.08 → 3019.26] Which sounds like a bug, but actually, if you ask me, it's a feature because it means that you're never going to get garbage out of a ZFS system.
[3020.28 → 3026.82] The other nice thing about doing a pair of drives like that is your unit of expansion becomes really simple.
[3026.82 → 3043.40] And these days you can buy 20 terabyte hard drives for $300 each, which isn't cheap, granted, but also for 20 terabytes of mirrored storage, effectively 40 terabytes of raw, 20 terabytes of usable.
[3044.02 → 3046.14] That's actually not a bad deal at all.
[3046.70 → 3050.62] The other thing about doing a pair is slot density matters.
[3050.62 → 3055.16] You know, you might have, let's say, four slots in a server.
[3056.34 → 3061.92] So let's put Brent in the shoes of five years in the future, Brent, and this 20 terabyte mirror is full.
[3062.60 → 3064.52] You think to yourself, well, what can I do here?
[3064.60 → 3071.06] Well, you could just go and buy another pair of drives of whatever the in vogue size is that year.
[3071.24 → 3073.76] Let's assume it's 40 terabytes in five years time.
[3073.76 → 3085.24] And then suddenly you've more than doubled your capacity, but all the old data is still there in its old format for you to, you know, move around between as you see fit.
[3085.44 → 3088.24] The mental model, it keeps it really simple to understand.
[3089.24 → 3096.74] You know, that leads me straight into the whole crux of the question that I have today, which feels like a bit of emergency.
[3096.74 → 3101.22] We're at Black Friday season and a bunch of drives are on sale.
[3101.38 → 3108.70] And if you look at them in Canadian dollars, I have a potential to save like $200 per drive or something with some of these sales.
[3109.24 → 3121.10] So my question was, you know, you're suggesting these get the massive most drive that I could possibly muster in my budget and throw those as a pair into, you know, the storage rack that I have here.
[3121.56 → 3124.48] But it gets me thinking about all these drives that I already have.
[3124.48 → 3126.76] You know, I've got an eight terabyte, for instance.
[3127.02 → 3130.04] Can I just buy an eight terabyte drive and combine it with that?
[3130.12 → 3140.16] Like, it seems like maybe that would be far cheaper and maybe that would get me far enough where I could wait a year or two and then get that massive pair later.
[3140.26 → 3142.98] What do you think about the now versus later question?
[3143.80 → 3144.78] The same logic applies.
[3145.02 → 3145.16] Yeah.
[3145.40 → 3150.44] Get the biggest hard drive your budget will permit to pair with the old one.
[3150.44 → 3159.52] So even if all you buy today is one 20 terabyte hard drive, for example, pair that with the eight that you've already got, the eight terabyte.
[3159.84 → 3162.30] So your mirror would be an eight and a 20.
[3162.72 → 3165.96] You'd be wasting 12 terabytes today, which sounds a bit stupid.
[3165.96 → 3174.32] But in six months time, when you come across another good deal and this just allows you to like do dollar cost averaging of hard drives, I guess.
[3174.62 → 3179.30] So you're buying a hard drive now, one to make the mirror.
[3179.56 → 3186.40] And then in six months time, all you do is swap out the eight terabyte for the new 20, for example, re-silver it.
[3186.42 → 3189.38] And suddenly then you've got the full 20 available to you.
[3189.38 → 3195.32] I had never even considered wasting 12 terabytes just for a couple of months.
[3195.52 → 3197.72] It's a bit of a first world opulent problem, isn't it?
[3198.04 → 3207.74] But when you put it that way, you know, when you're trying to balance budget and maybe drive slots and things like that, it actually, in a strange way, makes a lot of sense.
[3209.78 → 3213.30] But it doesn't make it easy to make a choice, does it?
[3213.30 → 3226.38] No. And the biggest knock against ZFS really versus something like Mergers, which you know I'm a great proponent of, is that with ZFS, you have to start with empty drives.
[3226.74 → 3230.54] So my question to you would be this eight terabyte drive.
[3230.88 → 3237.38] Do you have somewhere to put that eight terabytes whilst you build the new array, right?
[3237.42 → 3238.30] The new Z pool.
[3239.08 → 3240.64] It's a very good point.
[3240.64 → 3242.64] I will admit this eight terabyte.
[3242.82 → 3245.76] I also may have broke the connector on it.
[3245.88 → 3246.80] So it's a little fiddly.
[3246.80 → 3247.52] Yeah, it's easily done.
[3247.98 → 3248.66] It's easily done.
[3249.50 → 3250.60] So here's the other thing, right?
[3250.72 → 3256.06] We were talking about the data you wanted to store, and it's all kind of suit and tie business data, right?
[3256.12 → 3260.08] It's real data that cannot be replaced stuff.
[3260.64 → 3260.96] Yes.
[3260.96 → 3271.06] Why not use your existing fleet of mismatched hard drives to store some slightly more replaceable stuff instead using something like Mergers?
[3271.42 → 3272.90] Don't worry about the parity on that.
[3273.00 → 3284.20] And then have two different tiers of data stores within the same box using Mergers and that on one side for the media and then ZFS for the suit and tie data on the other.
[3284.20 → 3284.24] Yeah.
[3285.12 → 3287.14] I also hadn't considered that.
[3287.28 → 3288.74] I'm glad you're here with me.
[3288.74 → 3289.14] Yeah.
[3289.80 → 3290.28] Yeah.
[3290.36 → 3298.54] And I like the idea of the peace of mind of new drives because these drives, you know, have been around and just been sitting there as well.
[3298.54 → 3302.08] And they've travelled across the country in the back of a trailer, etc.
[3302.08 → 3308.08] So my confidence in these older drives is also surprisingly low.
[3308.80 → 3313.78] So the idea of buying new drives feels, I don't know, emotionally like a good thing.
[3314.84 → 3324.82] But I guess that brings me to another question of, you know, if you go somewhere like diskprices.com to see what the best deal might be, they just by default show you a bunch of used drives.
[3324.82 → 3329.44] And those seem to have great prices, and they seem like enterprise drives.
[3329.52 → 3336.12] And I'm just curious your opinion of, you know, if you shouldn't care about drives, they should just be replaceable.
[3336.12 → 3338.70] Then is that a reasonable avenue to go down?
[3339.36 → 3341.12] If you're running a data centre, yes.
[3342.32 → 3350.58] If you are a man with less than a dozen hard drives in his house, then each one actually matters.
[3351.44 → 3352.90] At least a little bit.
[3352.90 → 3357.40] You could argue that an off-site backup makes that argument a little bit less relevant.
[3358.36 → 3366.98] But for every time a drive fails, it's extra cost, it's extra cognitive load, it's extra time watching and resilvering and, you know, all that kind of stuff.
[3366.98 → 3375.34] So from my perspective, you're going to be saving probably 30 or 40% with a used drive versus a brand new one.
[3376.10 → 3377.76] But you just don't know its history.
[3378.76 → 3382.76] There's just no way to know how many times Linus Tech Tips has dropped that particular drive.
[3382.90 → 3383.32] Is there?
[3384.46 → 3385.66] Oh, local drives.
[3386.92 → 3388.06] Yeah, I guess you're right.
[3388.14 → 3388.86] The same applies.
[3389.10 → 3397.02] If I'm not comfortable with the history of the drives that I have in my own care, then I certainly shouldn't be comfortable with the drives that I know not the history.
[3397.02 → 3404.74] There are certain things in a computer that I will absolutely advocate buying used RAM, definitely, because you can check that really easily.
[3404.88 → 3405.08] Really?
[3405.20 → 3405.38] Yeah.
[3405.58 → 3405.82] Oh.
[3406.64 → 3410.00] CPUs, they almost, I've only ever had one go bad on me.
[3411.00 → 3415.50] Motherboards, again, they either typically work or they don't, as long as you check the CPU pins very carefully.
[3416.16 → 3422.72] Power supplies, you know, typically they're pretty reliable too, as long as they've got all the original modular cables with them.
[3422.96 → 3428.42] You don't swap them out with a different manufacturer because the pinouts can be wrong and then wrong voltages fry things.
[3428.42 → 3430.52] Obviously, a case as well.
[3430.62 → 3433.30] Obviously, that doesn't really matter if that's used or not.
[3433.98 → 3440.08] But hard drives are the one thing because they are so delicate and the tolerances are so small, and they're so fragile.
[3441.04 → 3442.54] I just don't mess about with them.
[3443.22 → 3443.24] Hmm.
[3444.06 → 3444.84] Well, that's great advice.
[3444.94 → 3445.36] Thank you, Alex.
[3445.40 → 3450.00] It feels like now I just got to open my wallet, see what I get shipped here this week.
[3450.00 → 3454.00] 45Homelab.com.
[3454.70 → 3456.06] The HL15 is here.
[3456.18 → 3457.24] It's available for purchase.
[3457.70 → 3463.96] You can get it in a bare-bones thing, or you can get it built up with a chassis and a backplate and the PSU ready to go, fully tested.
[3464.44 → 3465.60] It's really up to you.
[3465.72 → 3467.60] Big, strong, fast storage for the Home lab.
[3467.96 → 3475.24] Taking the enterprise mindset, the lessons learned that 45 Drives has taken from all their years in the enterprise and collaborating with the open source community.
[3475.74 → 3478.50] And now building something for the Homemaker.
[3478.50 → 3482.08] It comes with Rocky Linux, and you'll have the ability to install applications on it.
[3482.12 → 3485.70] Things like Image will run fantastic on the HL15.
[3486.48 → 3490.46] And from what I hear, Alex has one arriving soon or maybe already arrived, actually.
[3490.86 → 3494.64] I don't want to say too much, but chances are there's going to be a review on the show.
[3494.94 → 3501.08] I'm really excited because now we have something that I think meets the bar, and it takes this as seriously as we all do.
[3501.42 → 3502.26] So go try it out.
[3502.32 → 3506.44] I think this is the perfect unit for anybody that wants something robust that can grow with them.
[3506.44 → 3510.88] It's the HL15 and you can find it over at 45homelab.com.
[3510.96 → 3511.50] It's here.
[3511.86 → 3514.00] It's based on your feedback, and it's beautiful.
[3514.10 → 3516.64] Big, strong, and fast at 45homelab.com.
[3516.64 → 3520.04] Well, Alex, thanks so much for your insights.
[3520.26 → 3524.56] As always, I should just listen to what you say and just go and do it.
[3524.92 → 3526.02] So thank you for that.
[3526.22 → 3526.94] Oh, stop.
[3527.06 → 3529.44] But I bet you we've got a bunch of boosts we should go through.
[3530.20 → 3531.70] We have a nice batch this week.
[3531.72 → 3533.54] We can't always fit them all for runtime.
[3533.54 → 3542.00] But Bamham182 comes in with 34,567 SATs using Pod verse this week.
[3542.30 → 3546.14] And they write, I appreciated hearing about the backups as I'm building a backup server.
[3546.46 → 3551.70] I've got an Elite Desk 800 G3 SFF for $40 on eBay.
[3552.08 → 3552.54] $40?
[3553.10 → 3553.76] That's amazing.
[3553.76 → 3554.22] That's what I'm saying.
[3554.60 → 3557.10] That's what I keep saying about these one litter PCs, man.
[3557.18 → 3559.52] They are bargain of the century.
[3560.10 → 3563.06] And it has two 3.5 NVMe drives in it.
[3563.52 → 3567.44] I bought the Easy Stores, which will replace some drives in my main Pool.
[3567.92 → 3569.18] These will go into the Elite Desk.
[3569.50 → 3573.20] If all goes as planned, the box will go to a friend's house and is off all the time.
[3573.22 → 3577.82] But it'll turn on at night and sync the data through WireGuard and then turn back off.
[3577.94 → 3581.98] I switch from pfSense to Open Sense with all the WireGuard drama.
[3582.42 → 3586.96] And then from Open Sense to NixOS because I became more and more familiar with NixOS.
[3587.94 → 3589.32] Absolutely no regrets so far.
[3589.32 → 3593.10] I love having full control and not having things I don't need running 24-7.
[3593.54 → 3597.62] I recently wanted to swap out a Dell Wise I was using for a T740.
[3598.06 → 3601.10] I was able to get the T740 running with a very similar config,
[3601.40 → 3605.12] swapped the boxes in it without the family even realizing I had done it.
[3605.26 → 3606.22] Nice job, dude.
[3607.22 → 3608.90] I have a question here.
[3610.22 → 3613.00] Given these little one litter PCs, and they just sip power,
[3613.56 → 3616.00] why would you bother turning them on and off at night like that?
[3616.26 → 3617.54] It's probably not your power, Bill.
[3617.82 → 3618.76] It's not your power, right?
[3618.76 → 3620.36] So even a little bit still something, right?
[3621.00 → 3626.64] Yeah, but I just worry about, you know, mechanical hard drives spinning up, spinning down.
[3626.74 → 3629.84] Is that a consideration here or am I just, you know, worrying for no reason?
[3630.50 → 3631.30] It is a consideration.
[3631.62 → 3635.36] It adds significant complexity to all of your monitoring as well.
[3635.36 → 3641.62] Also, the exit conditions of the backup scripts itself, it becomes a consideration too.
[3641.62 → 3645.98] If the server's on all the time, you don't have to have any of those considerations.
[3646.22 → 3648.52] You just can assume it's always on.
[3649.20 → 3654.58] And if ZFS tries to do a replication, it will say, well, you're already doing a replication, dummy.
[3654.64 → 3655.70] Don't try and do another one.
[3655.70 → 3667.70] Whereas if it's in the middle of one, and it shuts the computer down and then, you know, let's say you're doing, let's say you just took a trip, hypothetical example, and you're dumping 100 gigs worth of pictures onto your local system.
[3667.70 → 3671.98] That could easily take a couple of days or more to upload to the remote site.
[3673.06 → 3680.02] And in that case, you've got to plan for that, okay, one-off eventuality, that unusual eventuality, but you've still got to plan for it.
[3680.08 → 3683.10] And it, like I say, it just adds complexity to the whole situation.
[3683.80 → 3693.68] And, you know, reading the rest of this comment, you're clearly a gentleman that appreciates the finer things in life by ditching any non-declarative OS, right?
[3693.84 → 3694.68] So, you know.
[3695.20 → 3696.18] Look at us, girl.
[3697.70 → 3699.58] I love it.
[3699.76 → 3700.12] That's right.
[3700.16 → 3700.94] The gentleman's OS.
[3701.86 → 3703.28] I think it's a pretty solid setup.
[3703.48 → 3709.46] I totally get turning it on and off to save power, although I have a similar setup here, right?
[3709.46 → 3713.64] I have my main workstation on a Zigbee smart plug.
[3714.86 → 3722.94] And when I arrive, I have an automation that turns on the smart plug and my BIOS is set to restore power when the power state comes back.
[3723.52 → 3725.54] And that's worked for six months.
[3725.54 → 3728.46] And then when I went on my trip and came back, the smart plug turned on.
[3728.78 → 3732.32] And now every other time, the PC doesn't restore power state.
[3732.64 → 3734.58] Just for some reason, still set in the BIOS.
[3735.20 → 3736.16] I haven't changed a thing.
[3736.24 → 3737.74] And it just doesn't restore power state.
[3737.82 → 3739.04] So that kind of thing can happen, too.
[3739.04 → 3750.78] Now, Alex, this gets me thinking about you sent me a photo a couple of days ago of something you 3D printed for your one litter PC, which to me on the surface seems ridiculous.
[3751.34 → 3751.96] Oh, yeah.
[3751.96 → 3754.78] But can you maybe give us more details?
[3755.28 → 3759.44] I 3D printed a rack mount, a 1U rack mount for these little systems.
[3759.68 → 3761.86] Chris, I'm going to be just, dear listeners, here we go.
[3763.06 → 3764.04] Oh, my goodness.
[3764.04 → 3765.00] This is amazing.
[3765.00 → 3770.48] So I've got one of these little Dell boxes, one of these little PCs in a rack mount system now.
[3771.36 → 3773.44] That is so cool.
[3774.02 → 3778.46] And then obviously a 3D printer can't fit 19 inches, which is a standard rack unit width.
[3778.66 → 3786.10] So you split it in half, put some screws in the middle, and suddenly you've got a 19-inch wide 1U unit for two of these things.
[3786.42 → 3788.12] You put two of them in there, one, yeah, in one.
[3788.28 → 3788.94] Oh, my gosh.
[3788.94 → 3795.54] There's quite a few if you look on like printable or thingies or something like that, there are quite a few people that sort of stack them on top of each other like this.
[3795.62 → 3798.42] And you can fit an 8 port switch in there as well.
[3798.46 → 3808.44] So you can actually literally have like a 5 or 6 half width U rack, you know, like a mini rack almost, like a desktop home lab rack, just 3D printing.
[3809.16 → 3809.98] I need that for the Droid.
[3810.34 → 3813.84] I have yet to find a case I'm fully satisfied with, with the Droid.
[3814.20 → 3817.04] And I just need a rack unit that the top is exposed.
[3817.60 → 3818.10] That's really great.
[3818.10 → 3820.96] Just buy a bamboo lab printer, dude, and be done with it and get it over with.
[3821.50 → 3821.78] All right.
[3822.64 → 3827.00] Johnny Castaway comes in with 26,235 stats using Pod verse.
[3827.26 → 3828.30] Johnny Castaway?
[3828.98 → 3829.70] Isn't that great?
[3830.22 → 3830.88] I know, it's a great name.
[3830.96 → 3831.86] He's a member.
[3832.02 → 3832.98] That brings me back.
[3833.12 → 3834.00] That brings me back.
[3834.00 → 3835.18] Long time listener.
[3835.84 → 3840.24] And he says, thank you for contributing to everybody who makes my 8-hour weekly commute bearable.
[3840.44 → 3840.66] Wow.
[3840.94 → 3842.50] We are the commuter's friend.
[3843.28 → 3844.90] He says, I was once at peace with Arch.
[3845.14 → 3846.34] Then I tried Nix-O-Us.
[3846.34 → 3846.94] Nix.
[3847.02 → 3848.32] Gave up many times.
[3848.44 → 3849.82] Returned to my old arch slippers.
[3850.12 → 3852.40] But Nix kept taunting me.
[3852.60 → 3854.52] Like a beast, Nix has been tamed now.
[3854.82 → 3855.84] And I think it's here to stay.
[3856.14 → 3858.68] He says, my next endeavour is Nix-OS on the Steam Deck.
[3858.82 → 3859.42] Any thoughts?
[3860.48 → 3860.84] Ooh.
[3860.98 → 3861.24] I don't know.
[3861.28 → 3862.50] Do you want to mess up a good thing?
[3862.78 → 3863.46] Oh, it's a UK.
[3863.66 → 3865.12] He also comes in from the UK.
[3865.12 → 3865.20] Right.
[3865.72 → 3865.92] Yeah.
[3865.94 → 3868.88] All the discerning people must do these days, of course.
[3869.00 → 3869.08] Right.
[3869.08 → 3869.14] Right.
[3870.22 → 3874.40] You know, it's funny because I was such a curmudgeon when it came to Nix as well.
[3874.56 → 3876.22] And Chris brought it up in the show.
[3876.68 → 3880.48] And I believe privately said to me, Alex, if you just listen sometimes.
[3880.48 → 3882.40] I identified Nix years ago.
[3882.78 → 3884.14] Why couldn't we have done this in self-defence?
[3884.34 → 3886.18] And I was like, yeah, but I just didn't see it.
[3886.34 → 3887.50] And it's just one of those things.
[3887.68 → 3891.90] Like, nobody can tell you how good Nix is.
[3891.96 → 3896.00] Nobody can tell you how it's going to change your life.
[3896.36 → 3898.06] You just have to experience it.
[3898.10 → 3900.22] And it just has to click for you.
[3900.46 → 3904.52] And it's like that moment as a teenager where your parents tell you, you just don't understand.
[3904.52 → 3912.94] And you're like, well, one day, eventually, with enough experience, you realize just how powerful that stuff can be.
[3913.98 → 3921.26] You know, in Linux Unplugged, sometimes we get a hard time because we're mentioning Nix OS far more this year than, well, we ever had.
[3922.08 → 3927.52] But it's just because it solves so many issues in a beautiful way.
[3927.80 → 3929.38] I mean, there's that learning curve, of course.
[3929.38 → 3937.62] But I have heard just this week alone, like five to six different people say, oh, yeah, thanks, guys.
[3937.76 → 3938.68] You made me try Nix OS.
[3938.80 → 3939.98] Now I can't use anything else.
[3940.84 → 3945.48] And so if you haven't tried it yet, I mean, I'm running it on this laptop in front of me.
[3945.52 → 3946.52] And I was a curmudgeon, too.
[3946.58 → 3947.66] It took me a while to come to it.
[3947.72 → 3949.92] And it's just like, it's just kind of nice.
[3950.24 → 3950.96] It's kind of nice.
[3951.04 → 3951.90] Another tool in the toolbox.
[3952.22 → 3955.14] I mean, you look at the wider ecosystem.
[3955.14 → 3959.76] I mean, the whole Flake's adoption situation is, frankly, it's just a mess.
[3960.34 → 3969.70] But you've got companies like Determinant Systems with Flake Hub coming along, pushing the agenda and taking the project by the scruff of the neck and saying, come on, boys, sort this out.
[3970.12 → 3971.34] And that's exactly what it needs.
[3971.56 → 3979.00] And for me, those signs are the green shoots that I needed to know that the project was going to be worth investing in the long term.
[3980.16 → 3981.02] Yep, I completely agree.
[3981.08 → 3984.02] Although I'll take the other side just to be fun and say, don't try it because it'll wreck you.
[3984.02 → 3985.02] Stick with your distro.
[3985.26 → 3985.52] Stick.
[3985.76 → 3986.34] Don't change it.
[3986.60 → 3987.50] You'll never be the same.
[3988.30 → 3993.30] The Bitcoin dad pod comes in with 24,444 SATs using Pod verse.
[3993.92 → 3997.32] He writes back, Blaze Cloud is another remote endpoint for backups.
[3997.44 → 3999.84] I use Rustic and their S3 encrypted object storage.
[4000.48 → 4003.72] My last bill was $4 for just two terabytes of storage.
[4003.98 → 4004.28] Whoa.
[4005.08 → 4005.92] That's attractive.
[4006.64 → 4006.92] Mm-hmm.
[4007.36 → 4007.76] Noted.
[4007.82 → 4010.88] He says, I've deployed tail scale at limited scale, and I find it amazing.
[4010.88 → 4016.50] That said, I'm concerned about relying on it as a third party now that it has visibility into my network.
[4016.62 → 4022.08] They also seem like an obvious point of regulation in a world of governments obsessed with surveillant private online activity.
[4022.26 → 4025.62] Has anyone ever tried to migrate a tail scale setup to head scale?
[4025.62 → 4027.78] What are your thoughts on the potential risks?
[4027.78 → 4033.74] Well, I can't speak to the migration to head scale because I completely trust the tail scale infrastructure.
[4034.44 → 4034.92] And here's why.
[4034.92 → 4041.24] If you know anything about public key infrastructure, you will know that that is what WireGuard is based on top of.
[4041.38 → 4050.08] So the idea that you provide a key, the remote server authenticates based on that kind of stuff, and it's very difficult to break that level of encryption.
[4051.54 → 4058.52] Any data that transits any tail scale asset is encrypted using that methodology.
[4058.52 → 4070.56] But the thing about tail scale that kind of makes it magic, and okay, yes, I work for them, corporate shill moment, hat on, is most of the connections happen through the magic sock.
[4070.64 → 4072.44] So they become peer-to-peer connections.
[4072.82 → 4077.60] So very little data actually traverses any tail scale owned infrastructure.
[4078.32 → 4082.92] At any point, you can look at tail scale status, look at all the nodes in your network.
[4082.92 → 4091.48] You can do tail scale net check, which prints an analysis of the local network conditions, like all the local DEEP servers, all that kind of stuff.
[4092.14 → 4103.92] So when you are connecting two tail scale nodes together, they initially connect and report back through the tail scale control server via this DEEP mechanism, D-E-R-P.
[4104.22 → 4107.90] The only thing that's identifiable on there is, you know, like an IP address, that kind of stuff.
[4107.90 → 4113.20] But frankly, that's identifiable across many other situations than just tail scale.
[4113.52 → 4120.60] The actual packets, the actual traffic, tail scale aren't interested in that because that would cost them money to transit through their servers, all that kind of stuff.
[4121.04 → 4132.58] And if you look at the free tier that tail scale offers too, those particular users that are on the free tier, you think to yourself, well, how can that possibly make sense from a business perspective for them to offer this thing for free?
[4132.58 → 4138.08] Well, it's because no data transits tail scale's network, unless you're using something like tail scale funnel or something like that.
[4138.14 → 4139.72] And then it's relayed through a TCP proxy.
[4140.18 → 4144.22] But that's for like hosting a very simple website as a developer or something like that.
[4144.74 → 4149.80] So, you know, in terms of trusting them, there isn't much trust I actually need to give tail scale.
[4149.96 → 4154.02] The only thing I need to give them is that they're going to continue to exchange my wire guard keys for me.
[4154.52 → 4155.18] And that's it, really.
[4155.22 → 4160.74] That's the only trust that I need to put in tail scale as a company and to continue to exist, of course.
[4160.74 → 4164.54] Yeah, and I also probably could have done more to play around with head scale.
[4164.84 → 4179.50] But part of the overall solution that I find super attractive is that the hosted component where they do that sort of deep discovery, I guess would be the term, which I love, is sort of the value added that I needed to actually start using it.
[4180.04 → 4186.66] I kept having one-off wire guard setups that I would have for six months or nine months at a time, maybe a year at most.
[4186.66 → 4191.64] Then I'd rebuild it and set it up differently, and I'd have a different way to, you know, maybe even try to manage it.
[4192.40 → 4195.34] And that just – that worked.
[4195.78 → 4203.78] But it was – it's like a – it's a – tail scale is a different level of a solution because it brings all my devices into one mesh network.
[4204.38 → 4209.74] And I was never going to get to that level with anything that I had to kind of self-set up like that.
[4209.80 → 4211.72] It just – I was never going to spend the time.
[4211.72 → 4216.28] And so that's kind of that extra value they brought there is what made me put it on everything.
[4216.72 → 4223.36] You could argue that switching solutions every six months is pretty secure because by the time any script kiddies are caught up with you, you're on to the next thing.
[4224.04 → 4224.54] Yeah, that's true.
[4224.64 → 4224.98] That's true.
[4225.32 → 4229.34] Now, we do have more boosts to make into the show because we had 10 total boosters this week.
[4229.40 → 4230.68] But we'll put a link to the Boost Barn.
[4231.18 → 4233.62] We do read all of them, and then we save them for posterity.
[4233.84 → 4235.56] So thank you, everybody who boosts in.
[4235.70 → 4239.54] We stacked 346,804 SATs this week.
[4240.00 → 4241.08] We really appreciate that.
[4241.08 → 4247.88] You can boost in by getting a podcast app at podcastapps.com like Pod verse and Automatic and Fountain.
[4247.96 → 4249.26] Those are really popular in our audience.
[4249.94 → 4251.82] And if you don't want to switch apps, we'll just get Alfie.
[4251.90 → 4252.68] Getalbie.com.
[4252.76 → 4255.28] You top it off and head over to the podcast index and boost in.
[4255.32 → 4256.48] We'll have links to that.
[4257.06 → 4258.14] And also thank you to our members.
[4258.24 → 4260.14] Once again, don't forget we got that Black Friday sale.
[4260.76 → 4262.76] Two bucks off a month for a year.
[4262.94 → 4264.16] We use promo code Black Friday.
[4265.42 → 4268.30] You can find me at alex.ktz.me.
[4268.30 → 4272.62] Got a bunch of links to the various places that I'm on the internet over there.
[4273.10 → 4275.18] One place you can find me is Linux Unplugged.
[4275.48 → 4276.38] Linuxunplugged.com.
[4277.18 → 4279.52] A bunch of shenanigans happening over there, too.
[4280.28 → 4281.24] Yeah, you can find me over there.
[4281.44 → 4281.84] Sometimes.
[4282.38 → 4283.30] Not every week, though.
[4283.42 → 4284.50] Sometimes it's Evil Chris.
[4284.64 → 4286.54] You just have to figure out if it's Good Chris or Evil Chris.
[4286.62 → 4287.88] But this is Good Chris for sure.
[4288.52 → 4290.12] Although if it was Evil Chris, I wouldn't tell you.
[4290.52 → 4292.74] But they're both tweeting at Christmas on Weapon X.
[4292.74 → 4296.26] And the show is also at Self-Hosted Show if you want to follow that over there.
[4296.90 → 4297.68] Thanks for listening, everybody.
[4297.86 → 4300.50] That was self-hosted. Show slash 110.
