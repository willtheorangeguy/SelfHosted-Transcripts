[0.00 --> 4.02]  One of the cornerstones of our collective worlds as self-hosters is storage.
[4.56 --> 6.66]  Hard drives, let's face it, are evil.
[7.20 --> 10.94]  So today, we have the CTO of Unraid, John Ponozzo, joining us.
[11.54 --> 13.76]  Unraid was my gateway to Linux back in 2012,
[14.18 --> 16.92]  and it's got an absolutely incredible community behind it,
[16.96 --> 20.60]  whilst also being one of the easiest ways to store and own your data.
[21.52 --> 23.94]  John takes us through the excitement of discovering Docker,
[24.40 --> 27.02]  what it was like to be featured online as Tech Tips,
[27.32 --> 29.14]  and the future of Unraid itself.
[29.84 --> 31.60]  First, though, a quick bit of housekeeping.
[32.40 --> 37.58]  Last episode, we mentioned a group buy for a DIY open-source open-hardware energy monitor
[37.58 --> 41.16]  for about $20, you know, the one based around the Raspberry Pi.
[42.28 --> 46.32]  We'll be doing a larger roundup of energy monitoring options in the next episode,
[46.52 --> 47.58]  that'll be number 26,
[47.98 --> 51.40]  but I wanted to let you know that the group buy looks like it's going to be going ahead.
[52.10 --> 56.40]  We've definitely got enough orders for the US and the EU, that includes the UK,
[56.40 --> 60.44]  and for our friends down under, unfortunately, we're not quite there yet.
[60.78 --> 66.14]  So if you are interested, please register using the Google Form link in the show notes.
[66.40 --> 69.96]  This also applies if you emailed us or posted on Twitter.
[70.50 --> 72.08]  The form is what we'll be using now,
[72.14 --> 75.06]  as the response was so much larger than anticipated,
[75.66 --> 78.88]  and it was spread across, I don't know, like five or six different places.
[78.88 --> 85.66]  So please, if you are in doubt, put your name in the form and we'll record you as being interested.
[86.34 --> 91.10]  We'll leave the form open until the end of August and then be in touch for the next steps in September.
[91.10 --> 95.56]  Let's get you to our interview with Unraid's John Panazzo.
[97.14 --> 98.86]  John, welcome to Self Hosted.
[98.88 --> 99.58]  It's good to have you here.
[99.94 --> 100.80]  Thanks. It's good to be here.
[101.10 --> 103.28]  So I know we have tons of questions for you.
[103.74 --> 108.04]  And just full disclosure, Alex is quite familiar with Unraid and I'm the noob.
[108.14 --> 112.04]  So I'll be playing the noob, as always, it seems these days on this episode.
[112.56 --> 116.52]  So let's just start with people who aren't familiar with what is Unraid and who would you say it's for?
[116.52 --> 121.16]  So Unraid is a server operating system that was built by LineTech back in 2005.
[121.82 --> 125.44]  And it's predominantly for personal home media enthusiasts,
[125.44 --> 131.70]  people that want to build their own home media server to store all their personal digital media amongst other content.
[132.36 --> 136.44]  And we've been basically building it out over the last several years.
[136.54 --> 139.72]  So originally it started off as just a NAS platform, pure storage play.
[139.98 --> 145.20]  And then with Unraid 6, we kind of completely modernized the OS and expanded its capability.
[145.20 --> 149.08]  So what used to be known as a NAS OS is now a full-blown server platform.
[149.24 --> 153.50]  And to us, the server platform really makes sense because storage is one aspect.
[153.96 --> 156.22]  The next aspect is running applications on that server.
[156.30 --> 157.66]  And the third is running virtual machines.
[157.76 --> 161.44]  So we pretty much have expanded it to be the full gamut of what a traditional server can do.
[162.04 --> 167.50]  I noticed your pricing structure is essentially tiered around the amount of attached storage.
[168.00 --> 171.14]  Do your customers tend to be either on the lower end or on the very extreme high end?
[171.16 --> 172.58]  Or is there a good in-between?
[172.98 --> 173.82]  You'd be surprised.
[173.82 --> 180.56]  You know, obviously there's a lot more people out there with six or less devices than there are with people that have 25.
[181.18 --> 182.42]  That's just logical.
[182.70 --> 185.22]  But we actually have a pretty good spread.
[185.70 --> 192.56]  And there are plenty of folks out there that just buy the top tier knowing that eventually I'm going to have that many storage devices.
[192.90 --> 196.98]  So, yeah, you'd be surprised how many people opt for Plus and Pro over Basic.
[196.98 --> 201.98]  I'm kind of curious how the forest fire that has been 2020 has affected Unrate.
[202.56 --> 204.48]  Has there been a notable change in business?
[204.66 --> 209.52]  And are you guys eyeballing maybe long-term something like a subscription model?
[209.52 --> 216.20]  So, I can definitely tell you that with everything going on with coronavirus and whatnot, believe it or not, that's not hurt us at all.
[217.02 --> 225.38]  I think, if anything, not that I'm happy that this has happened, but it has definitely helped business growth only because there's more people at home now.
[225.38 --> 229.28]  And what do you do as an IT person that's at home or somebody who's a tech enthusiast at home?
[229.36 --> 229.70]  You tinker.
[230.38 --> 233.94]  And very likely those people are going to somehow or another come across Unrate.
[234.12 --> 236.42]  So, we've not been negatively impacted.
[236.54 --> 238.38]  And we don't have, you know, brick-and-mortar offices.
[238.64 --> 241.58]  We're a completely remote team with people all over the world.
[241.82 --> 248.80]  So, if anything, it's kind of helped out because we've been able to hire some more people this year and help some people out in some bad situations.
[249.16 --> 251.14]  So, it's been great.
[251.14 --> 253.48]  I think 2020 is going to be a banner year for us.
[253.78 --> 254.68]  That's really great news.
[255.04 --> 260.84]  I'm not sure I fully appreciate the implications of being a nerd stuck at home means I tinker more.
[261.58 --> 262.56]  I mean, it's definitely true.
[263.36 --> 264.26]  Definitely true.
[264.40 --> 265.44]  Hey, I know I do.
[266.14 --> 266.36]  Yeah.
[266.50 --> 267.52]  No, it's totally true.
[267.60 --> 268.10]  It's a thing.
[268.58 --> 268.82]  So, yeah.
[268.88 --> 271.00]  I mean, it's always a tricky balance, isn't it?
[271.00 --> 281.00]  Building a sustainable business model on one-time license purchases versus, say, the Netflix model of, or more accurately, I suppose, the Adobe model.
[281.58 --> 284.16]  Of purchasing software over time.
[284.42 --> 290.98]  And particularly with Unraid, given that the lifespan of a license purchase could be a decade or two.
[291.70 --> 297.34]  You know, I pay my 60 bucks once and then that's it for, you know, LimeTech season doesn't see another dime of that.
[297.34 --> 303.32]  And just to reiterate Chris's question, I was wondering if there were any plans for subscriptions moving forward.
[303.78 --> 304.22]  Yes.
[304.36 --> 313.44]  I can't get into all the details on how that's going to work, but we have very much been looking into building other options that you can use with Unraid.
[313.44 --> 315.82]  So, there's two ways to look at that question.
[315.92 --> 319.64]  The one is, are we going to launch some kind of subscription service?
[319.76 --> 323.18]  And the second is, how does that affect the current licensing model?
[323.18 --> 327.70]  And so, we are working on options for both of those.
[327.70 --> 334.22]  So, one model would be something that you can pay to extend the value of Unraid.
[334.40 --> 339.26]  So, you still have your registration key or some type of license that validates your ownership of the product.
[339.66 --> 343.56]  But then we offer services that complement the product that are optional to purchase.
[344.18 --> 346.20]  The other is an online license key.
[346.20 --> 348.78]  And this is something that we've wanted to do for some time.
[349.00 --> 357.44]  When Unraid was started, when this whole business was started back in 05, you know, Tom Mortensen, our CEO, he built this as kind of a pet project.
[357.74 --> 359.34]  And it was nothing more than beer money.
[359.48 --> 360.98]  It was, hey, there's a problem.
[361.58 --> 362.68]  I can solve that problem.
[363.02 --> 366.98]  There's not a lot of people other than me that are looking or interested to solve that problem.
[367.08 --> 367.90]  So, I'll do it.
[367.96 --> 368.84]  And I'll release it.
[369.10 --> 369.68]  And we'll go.
[369.88 --> 374.64]  Literally, he just went to avsforum.com, created a post in there, said, hey, I'm a guy.
[374.72 --> 375.42]  I made something.
[375.42 --> 376.02]  Check it out.
[376.20 --> 379.42]  And just from that, the whole business kind of exploded.
[379.62 --> 382.76]  Now, for a very long time, it was still just a beer money business.
[382.90 --> 386.28]  And Tom was the only main employee, the only employee at all.
[386.92 --> 388.30]  But then it started to grow.
[388.48 --> 391.44]  And it got to the point where he wanted to do something major.
[391.44 --> 393.56]  And it happened to coincide with timing for me.
[393.64 --> 394.74]  That's how I joined the company.
[394.80 --> 395.76]  And I reached out to Tom.
[396.44 --> 400.78]  And we started having conversations about, you know, what could we do to really blow this thing up?
[401.26 --> 402.86]  And years later, here we are.
[402.94 --> 404.42]  And we're looking at, you know, sales.
[404.42 --> 405.78]  We're looking at how licensing works.
[405.78 --> 407.74]  And, you know, you hit the nail on the head.
[407.74 --> 416.80]  From a business model standpoint, it's untenable to not have any customer rebuys or repurchase or anything like that.
[417.12 --> 418.10]  But we've made it work.
[418.50 --> 419.20]  We've made it work.
[419.20 --> 420.98]  And we've grown doing it.
[421.04 --> 424.38]  Like, our monthly sales revenue is over 10x what it was several years ago.
[424.58 --> 427.48]  So we're doing great.
[427.58 --> 431.60]  But we know that there's a shelf life out there for how long that kind of model will last.
[431.60 --> 439.30]  So we are working on both of those options to give people another way to contribute back to Unraid and also get some more value out of it.
[439.74 --> 440.52]  That's a great story.
[440.82 --> 441.96]  I love that origin.
[441.96 --> 443.90]  I'm kind of curious right now.
[443.90 --> 451.86]  Do you see one of the big drivers of new business people discovering Unraid applications that they want to run on their LAN?
[452.06 --> 453.34]  Or is it storage?
[453.68 --> 459.00]  And the reason that I'm asking that is I wonder how cloud storage plays in this.
[459.12 --> 464.42]  Say somebody like Backblaze who can come along and offer reasonable rates for storage and Wasabi and others.
[464.42 --> 467.80]  Does that apply a certain kind of market pressure to you?
[468.06 --> 472.58]  Or is there an offset by people hosting applications like Plex?
[473.02 --> 475.96]  I don't think that any cloud storage has any pressure on us at all.
[476.10 --> 479.08]  I mean, people were saying, oh, Netflix is going to kill Unraid.
[479.24 --> 479.76]  And it's not.
[480.26 --> 483.38]  Like, there's the people out there that want an Unraid server.
[484.10 --> 486.32]  They don't care about any of those outside factors.
[486.48 --> 489.06]  And there's a lot of folks out there that, you know, cloud's great.
[489.22 --> 491.00]  I have nothing against cloud.
[491.10 --> 493.56]  I think it's a great technology for the right use cases.
[493.56 --> 496.62]  But there are plenty of use cases that cloud is not the right technology.
[497.26 --> 511.52]  And, you know, I'll tell you right now, when your power goes out or your internet goes out for any extended period of time, especially if your internet goes out for any extended period of time, you'll learn how quickly you miss DVDs or Blu-rays or any method of playing media content that doesn't require an internet connection.
[512.00 --> 512.30]  That's true.
[512.58 --> 513.18]  Very true.
[513.30 --> 515.94]  I've gone to a lot of lengths to solve that problem.
[516.16 --> 522.30]  And also, you can't beat, honestly, you just can't beat the cost difference between a lot of local storage versus the same amount in the cloud.
[522.30 --> 523.24]  Oh, of course not.
[523.24 --> 525.60]  I mean, we just went through a pricing model recently.
[525.80 --> 529.64]  We were kind of just looking at options for what we could do with cloud tech.
[529.72 --> 532.30]  And I'm like, well, what would it take to run an Unraid server in the cloud?
[532.82 --> 542.60]  And when I just did, I mean, granted, this is still a research project undergoing, but like with Amazon, oh, my God, I almost choked at how much money it would have cost to just run an instance in the cloud.
[542.60 --> 548.70]  Because it's not like, oh, well, my compute usage is low and I'm only going to have to spin that VM up when I need to access an application.
[548.86 --> 551.46]  No, if you're going to run it in the cloud, you've got to run it in the cloud.
[551.52 --> 554.22]  It has to be always on, always available, ready at the fingertip.
[554.22 --> 558.84]  And so that's a minimum amount of compute resource that you have to dedicate budget towards.
[559.28 --> 562.92]  And then when you look at storage costs in Amazon, I mean, don't get me wrong.
[562.98 --> 566.54]  If you're running a website or a business off the cloud, Amazon's great.
[566.90 --> 572.16]  But when you're as a consumer and you're thinking about, well, I need a media server or I need a home server, personal server.
[572.58 --> 574.48]  And I could run that in the cloud or I could run it on-prem.
[575.16 --> 576.28]  What's the difference in cost?
[576.28 --> 580.38]  You look at the hosting model and you're like, in less than a year, I can pay for this and build it in my house.
[580.74 --> 581.68]  It's those transit costs.
[581.80 --> 582.62]  That's how they get you.
[582.88 --> 585.28]  Yeah, it's bandwidth and storage.
[585.90 --> 586.80]  That's the real killer.
[586.92 --> 591.94]  The CPU, the compute resources and all that stuff, that does add up, but it's fixed, right?
[592.02 --> 593.08]  Like, you know, it's predictable.
[593.24 --> 593.56]  It's fixed.
[593.62 --> 594.34]  It's not going to grow.
[594.44 --> 595.16]  It's not going to change.
[595.22 --> 596.46]  It's pretty much going to remain the same.
[596.78 --> 599.36]  Your storage is always going to go up and your bandwidth is always going to go up.
[599.82 --> 603.48]  So it's just it's a matter of time before the price model just doesn't make sense.
[604.20 --> 604.90]  I agree totally.
[604.90 --> 613.26]  You know, I made that same calculation myself a couple of years ago when I emigrated and built a two and a half thousand dollar server.
[613.46 --> 615.94]  You know, you think, OK, well, that's a lot of Netflix.
[616.14 --> 620.54]  But at the same time, I've got full control over what's on this box in my basement.
[620.54 --> 622.12]  And I always will.
[622.44 --> 624.52]  So that's the rationale I go through.
[625.06 --> 626.18]  There's more to it than just that, too.
[626.26 --> 628.34]  Like, you know, all right, let's talk Google for a minute.
[628.88 --> 629.92]  So I'm a big Android guy.
[630.04 --> 632.46]  Like I my wife's an Apple person and I'm an Android person.
[632.46 --> 634.92]  So you can imagine the fun technology conversations we have at home.
[635.80 --> 639.08]  But and when she the best part about that is whenever she asked me for help, I'd be like, well, I don't know.
[639.14 --> 639.78]  I don't use Apple.
[640.24 --> 644.04]  So that's the one time I can play dumb as a tech person and be like, I think you might have to call Apple.
[644.56 --> 652.86]  But one of the things that I have noticed, and this applies to both of those platforms, definitely with my my Android phone, I guess maybe I have to verify with Apple.
[652.86 --> 658.88]  But with Android, for sure, when you take pictures on an Android device and they go to Google's cloud, you think, oh, that's great.
[658.96 --> 661.50]  Right. And I bought this really nice phone that's got this really nice camera.
[661.58 --> 663.30]  It's taking these really nice high fidelity pictures.
[663.90 --> 670.34]  Yet after a while, once it's no longer cached on your phone and you go back to look at that picture again, it's not quite as crisp, not quite as clear.
[670.40 --> 673.96]  And it's because they apply compression and they they lower the image quality.
[673.96 --> 679.24]  That really honestly, the first time I noticed that, it really pissed me off because as a customer, I feel cheated.
[679.36 --> 683.06]  I feel like I bought a device that was capable of taking really high quality pictures.
[683.70 --> 688.42]  And you gave me a service that complements that device to store those pictures online, which I think is great.
[688.96 --> 694.10]  But then without notifying me and without and whether you notify me or not, it doesn't really matter.
[694.18 --> 696.46]  You just you degraded the quality of those pictures.
[696.46 --> 697.36]  And I don't like that.
[697.56 --> 697.66]  Yeah.
[697.66 --> 703.92]  So having a local storage where you can protect protect the original quality and fidelity of the content that you're capturing.
[703.96 --> 709.84]  And creating, you know, it's one thing if it's a movie or a TV show or whatever, something that I download from the Internet.
[709.96 --> 710.52]  That's one thing.
[710.60 --> 716.62]  But when it's my kids pictures and I go look at it years later and it's all pixelated because Google applied some compression to it.
[716.70 --> 722.88]  And that's even worse when when it's years down the road and the camera that I originally used was already low quality.
[722.88 --> 724.84]  And now you're compressing it even for it.
[724.84 --> 726.72]  Just it makes for not a good experience.
[726.72 --> 732.44]  So having local storage to protect your stuff, I think that's actually going to become more and more important.
[732.44 --> 734.42]  You only get one chance at those photographs.
[734.74 --> 734.88]  Yes.
[734.96 --> 736.34]  Very, very important stuff.
[736.48 --> 736.66]  So.
[737.00 --> 737.54]  All right.
[737.54 --> 740.00]  Let's talk a little bit about the future.
[740.64 --> 744.80]  We're high up in the version six release cycle of Unraid now.
[745.48 --> 747.24]  It's your 15th birthday soon.
[747.48 --> 749.56]  Is version seven on the horizon?
[750.70 --> 753.40]  Can't get into any details about what seven might look like.
[753.40 --> 760.16]  I'll tell you right now that we've had maybe a handful of conversations, you know, speculating on what could seven be.
[760.24 --> 760.50]  OK.
[760.66 --> 761.10]  You know what?
[761.14 --> 762.40]  What could what could go in there?
[762.82 --> 765.46]  We're not yet actively developing version seven.
[765.62 --> 765.92]  All right.
[766.24 --> 769.24]  We're still we're still plenty of life left in the six tree.
[769.78 --> 771.42]  Six nine is about to go stable.
[771.64 --> 773.72]  You know, it's currently available for public testing.
[774.02 --> 774.80]  It's in beta.
[774.80 --> 779.64]  And and we already have a six ten roadmap that's that's being worked on.
[780.28 --> 784.10]  But beyond the six series, I can't really comment on what seven would be.
[784.24 --> 788.42]  But I can tell you that I definitely have things in my mind that I want.
[788.86 --> 791.60]  And eventually, I think we're going to get there.
[791.94 --> 792.56]  I think we're going to get there.
[792.64 --> 793.26]  I wish I could.
[793.32 --> 795.12]  I really like you can hear it in my voice.
[795.18 --> 796.22]  That's a pretty good tease.
[796.22 --> 800.58]  I really want to talk about what I'd love to have happen.
[801.02 --> 804.36]  But I you know, it's just too early to get into those details.
[804.66 --> 806.94]  And I don't want to get beat up over it.
[807.00 --> 808.48]  So that's cool, man.
[808.52 --> 809.12]  That's no problem.
[809.60 --> 811.84]  So what are you excited about in six?
[812.28 --> 814.20]  Was it six point eight or six point nine next?
[814.62 --> 816.72]  Six six nine is the next main release.
[816.72 --> 818.24]  And then after that, we have six ten.
[818.40 --> 819.94]  So six nine is going to be awesome.
[820.54 --> 824.42]  You know, multi-pool support has been something that we've been working on for a while now.
[824.42 --> 826.36]  And six nine is going to bring it to bear.
[827.26 --> 832.40]  And I just actually so this was it was perfect timing because Tom's like, hey, we're going to add this this new feature.
[832.50 --> 833.76]  It's going to be multiple cash pools.
[834.42 --> 837.20]  And we're going to roll it out in six nine.
[837.52 --> 843.78]  And right around the time that he started talking about doing that, my cash pool was actually filling up my personal system at home.
[844.12 --> 847.82]  And I'm like, you know, this is a great time to test out this new feature.
[847.82 --> 853.36]  So this last week, actually, I went through and created a new cash pool, put brand new SSDs in,
[853.36 --> 861.76]  got it formatted, and then I stopped all my services, stopped Docker, stopped VM manager and copied the bulk of my cash,
[862.20 --> 863.92]  my original cash onto the new pool.
[864.30 --> 870.50]  And then I did a new config operation so that I could make the new pool my default cash pool and just replace my old pool.
[870.90 --> 872.12]  John is an Unraid newbie.
[872.18 --> 874.08]  Can I ask you, what is a cash pool?
[874.38 --> 878.02]  So Unraid operates with two main storage pools in mind.
[878.14 --> 880.28]  The first is the array and the second is the cash.
[880.72 --> 882.86]  So the array, the idea is, is that's where you put your hard drives.
[882.86 --> 885.92]  So you have at least one, but you can have up to two parity disks.
[886.40 --> 889.22]  And then the remainder can be just standard data disks.
[889.62 --> 892.10]  And they can be of different sizes, speeds, brands, protocols.
[892.22 --> 894.26]  That's one of the big hallmarks of Unraid.
[895.06 --> 897.90]  And then that's where you put all of your long-term storage data, right?
[897.94 --> 899.90]  And that's where all your media content goes.
[900.12 --> 902.14]  Everything that you want to store long-term goes there.
[902.60 --> 905.62]  But the downside is that hard drives can be slow.
[906.50 --> 911.22]  You might not be able to fully saturate network performance using right operations to the array.
[911.22 --> 913.46]  So we created something called the cache.
[913.54 --> 919.96]  And the cache is nothing more than another grouping of devices that manages storage a little bit differently than the array.
[920.14 --> 924.64]  So the array, we have up to two dedicated parity disks, and the rest are data.
[925.36 --> 930.10]  And because of those dedicated parity disks, that means there's no striping happening across the data disks in the array.
[930.10 --> 934.28]  That has a performance impact, whereas the cache pool, we actually currently use ButterFS.
[934.88 --> 937.16]  We can talk about a new file system option there in a minute.
[938.00 --> 943.88]  And ButterFS allows you to group many different devices, also of different size, speeds, brands, protocols.
[944.64 --> 946.46]  But it does it in a RAID 1 formation.
[946.60 --> 952.36]  Now, it's not, you know, for anybody that hears RAID 1, they usually have a very fixed image in their head of what that means.
[952.44 --> 955.88]  But in ButterFS world, you can have more than two devices in a RAID 1.
[955.88 --> 962.96]  All it means is that every time a bit gets written to that disk pool, it's going to make sure that bit gets written to two different devices that are in the pool.
[963.14 --> 963.52]  That's all.
[964.02 --> 964.80]  Did you hear that, Chris?
[965.26 --> 966.64]  ButterFS? The ButterFS part?
[967.12 --> 969.20]  Yeah, Chris is all in on ButterFS these days.
[969.36 --> 971.04]  I do. I do like me some butter these days.
[971.44 --> 972.24]  ButterFS is great.
[972.78 --> 977.60]  You know, there's still some outlying issues with ButterFS that are sometimes a struggle.
[977.60 --> 980.14]  And it just feels like the project that never ends.
[980.96 --> 983.46]  But I still like it a lot.
[983.54 --> 986.02]  I just don't trust RAID 5 and 6 totally yet.
[986.62 --> 988.84]  But RAID 1 and 10 are great.
[989.54 --> 994.22]  And so for operating a cache pool, which, again, the purpose of the cache pool is to act as a cache,
[994.30 --> 998.24]  which for those that I would imagine most people that are listening know what that is.
[998.32 --> 1001.00]  But if they don't, it's just a temporary repository for data.
[1001.52 --> 1004.60]  And that's faster than your long-term storage repository.
[1004.60 --> 1008.68]  So when you write data to a share in Unraid, if the share is cache-enabled,
[1009.12 --> 1011.56]  then the data actually gets written to the cache pool first,
[1011.68 --> 1014.84]  and then it gets moved to the array on a schedule that you define.
[1015.00 --> 1017.26]  So right now it's by default at 3.40 a.m.
[1017.76 --> 1024.98]  So the cache is great because it can make real-time write operations appear to be a lot faster than what the array is capable of.
[1025.18 --> 1029.54]  Use the fast storage to receive the data and then write it in the background as time permits.
[1029.74 --> 1030.16]  Exactly.
[1030.16 --> 1038.16]  Yeah, I think that that new pooling or multiple pools opens up some interesting possibilities for different tiers of storage.
[1038.56 --> 1044.68]  So the next logical question from here is what about multiple arrays and stuff like that?
[1044.72 --> 1048.96]  Because, I mean, you want an SSD array, for example, backed by an SSD cache,
[1049.06 --> 1052.82]  and then you want a spinning array backed by an SSD cache.
[1053.00 --> 1055.78]  Like you could have different – do you see where I'm going?
[1055.90 --> 1057.00]  You could do different things with that.
[1057.00 --> 1057.76]  Yeah, I mean –
[1057.76 --> 1058.12]  Absolutely.
[1058.32 --> 1062.00]  There's – I will say that SSDs in the array are possible,
[1062.00 --> 1067.02]  but they add additional challenges based on how the devices do discard or trim operations.
[1067.86 --> 1070.98]  So it's a more complicated problem to solve.
[1071.34 --> 1074.82]  Now, one thing that I do want to test at some point in the future, I just –
[1074.82 --> 1077.06]  you know, there's so many ideas of what you can do with Unraid,
[1077.14 --> 1080.52]  but one really cool one that I want to mess around with at some point is building an array
[1080.52 --> 1085.92]  where the parity disks are NVMe, but the data disks are all SATA-based SSD.
[1086.64 --> 1091.56]  And the reason for this is that what happens when a write hits Unraid is that the system has to first decide
[1091.56 --> 1094.24]  which disk it's going to go to, right, where that write's going to go.
[1094.64 --> 1097.58]  Because, again, unlike traditional RAID, we don't stripe data.
[1097.72 --> 1099.70]  Every disk is formatted with its own file system.
[1099.78 --> 1102.04]  It operates independently of the other disks in the system.
[1102.04 --> 1107.94]  The only time they work in concert is when you are rebuilding a disk using parity.
[1108.46 --> 1111.40]  However, every time a disk gets a write, so does parity, right?
[1111.50 --> 1113.04]  So parity becomes a bottleneck.
[1113.14 --> 1116.92]  So let's say I'm writing three different files at the same time and they're each going to a different disk.
[1117.66 --> 1120.98]  Well, disk 1, 2, and 3 are each independently receiving a write,
[1121.10 --> 1125.62]  but then at the same time, those three writes are also hitting the parity disk all at the same time.
[1125.90 --> 1131.36]  But if you have a parity disk that has far more IO, far more IOPS available to it,
[1131.36 --> 1136.58]  than your data disks, then maybe you can kind of overcome that bottleneck limitation
[1136.58 --> 1139.26]  and get some really fast write speeds direct to the array.
[1139.62 --> 1140.80]  That is fascinating.
[1141.22 --> 1142.42]  I want to play around with that idea.
[1142.52 --> 1145.66]  It's one of those things where it's going to cost some money and take some time
[1145.66 --> 1147.14]  to really go through the testing on it.
[1147.54 --> 1149.12]  But I think that could be a really cool way to do it.
[1149.42 --> 1151.14]  Absolutely fascinating. Thank you, John.
[1151.14 --> 1154.76]  I was wondering if that was possible because for the longest time,
[1154.90 --> 1158.78]  that inherent having to make two writes at once performance imitation
[1158.78 --> 1163.28]  has been something that we've talked about in the Unray community for years
[1163.28 --> 1164.58]  as being a bottleneck.
[1164.74 --> 1166.64]  So it'd be interesting to solve that.
[1166.80 --> 1168.78]  So that leads me on to another...
[1170.00 --> 1172.80]  I guess it's an elephant in the room whenever you're talking about storage.
[1173.02 --> 1174.92]  It's kind of the juggernaut hiding in the corner.
[1175.54 --> 1176.64]  What about ZFS?
[1177.12 --> 1180.86]  So I love the European way, the Z.
[1181.60 --> 1182.76]  I'm going to start using that.
[1182.98 --> 1183.76]  Oh, I'm sorry, darling.
[1183.76 --> 1185.34]  Would you like ZFS?
[1185.64 --> 1186.80]  Is that better?
[1187.18 --> 1187.80]  No, no, no.
[1188.44 --> 1190.36]  ZFS it is.
[1190.46 --> 1191.78]  Okay, and we're going to go to the ZO.
[1191.92 --> 1192.76]  I just soak it up.
[1194.80 --> 1197.56]  So ZFS, so I like ZFS.
[1198.42 --> 1200.18]  So let's just go right through it.
[1200.30 --> 1204.38]  So have you seen the recent article that was this year from Linus Torvalds
[1204.38 --> 1205.64]  about ZFS on Linux?
[1205.92 --> 1206.92]  I'm assuming you had to have.
[1207.16 --> 1207.36]  Yeah.
[1207.36 --> 1215.08]  Okay, so Linus has got some pretty out there opinions on ZFS and why.
[1215.24 --> 1216.70]  No, that's not like Linus.
[1217.12 --> 1217.38]  Yeah.
[1217.84 --> 1220.36]  And when I say out there, I don't mean like out there like he's crazy,
[1220.46 --> 1224.10]  but like, no, he's got legitimate concerns as to what would happen
[1224.10 --> 1227.84]  if they just straight up merged ZFS into Linux.
[1228.28 --> 1230.98]  And all it would take is an email from Larry Ellison
[1230.98 --> 1233.72]  or any of the legal team at Oracle to make it happen.
[1233.90 --> 1236.30]  But they don't, and there's a reason they don't.
[1236.30 --> 1237.68]  So it's a licensing issue.
[1237.84 --> 1240.84]  At the end of the day, the reason that ZFS is not a part of Linux
[1240.84 --> 1242.14]  has nothing to do with technology.
[1242.26 --> 1243.46]  It has everything to do with licensing.
[1244.16 --> 1247.54]  And we think we might have a way to work around that issue.
[1248.14 --> 1251.82]  I know that there are other Linux distros that have already adopted it,
[1252.24 --> 1254.16]  and they're doing so at a risk.
[1254.54 --> 1257.00]  And because they have and nothing's happened yet,
[1257.04 --> 1258.08]  that gives us confidence.
[1258.54 --> 1261.60]  But all I can say is that ZFS has been something
[1261.60 --> 1263.08]  that we've been eyeing for a while.
[1263.08 --> 1267.12]  And part of the reason that multiple pools were put in
[1267.12 --> 1270.06]  is that it seemed like a pretty good feature to put in maybe before that.
[1270.56 --> 1271.04]  Yeah, absolutely.
[1271.24 --> 1275.52]  I can just imagine Unraid as the hypervisor using ZVols underneath.
[1275.94 --> 1277.04]  Oh, that would be so great.
[1277.30 --> 1278.72]  Yeah, the other thing you got to remember with ZFS,
[1279.14 --> 1281.78]  and this goes back to why we originally chose ButterFS,
[1282.42 --> 1285.82]  ButterFS was the perfect complement to Unraid.
[1286.24 --> 1286.66]  Perfect.
[1286.66 --> 1290.12]  Because from a user experience standpoint,
[1290.30 --> 1293.08]  in terms of how somebody goes about building an array,
[1293.34 --> 1294.08]  building their server,
[1294.28 --> 1296.08]  and then assigning all those storage devices,
[1296.78 --> 1299.16]  the rules about what you can do there,
[1299.34 --> 1300.32]  they work the same.
[1300.50 --> 1302.40]  That's the best part about ButterFS and Unraid,
[1302.76 --> 1305.54]  is they both let you use any kind of device you want.
[1305.78 --> 1306.78]  You can mix and match.
[1306.82 --> 1307.80]  You can use different sizes.
[1307.98 --> 1308.66]  It doesn't matter.
[1309.30 --> 1311.00]  And the best part is when you want to expand,
[1311.26 --> 1312.54]  you can just add another device,
[1312.68 --> 1313.46]  just like Unraid.
[1313.46 --> 1316.06]  Unraid, all of that goes away with ZFS.
[1316.26 --> 1316.84]  I almost said Z.
[1317.40 --> 1319.50]  All of that goes away with ZFS,
[1319.70 --> 1321.56]  because now you have to play by the ZFS rules.
[1321.64 --> 1322.70]  And I understand those rules,
[1323.14 --> 1324.02]  and they make sense,
[1324.46 --> 1326.46]  but to an average Unraid user,
[1327.02 --> 1328.00]  that might be frustrating.
[1328.62 --> 1329.82]  Let's say we did it as default.
[1329.94 --> 1330.80]  Let's just say, for example,
[1330.86 --> 1332.58]  that our cache pool was based on ZFS as default,
[1332.68 --> 1335.64]  and you created a two-device RAID 1 ZFS setup,
[1336.20 --> 1337.42]  and now you want to expand it.
[1337.92 --> 1339.66]  How easy is that compared to ButterFS?
[1340.32 --> 1341.28]  I mean, it's not terrible.
[1341.28 --> 1342.76]  With a two-device pool, it's not terrible.
[1342.76 --> 1344.38]  But imagine it's four or six,
[1344.58 --> 1347.36]  and now you have to add another four or six devices
[1347.36 --> 1349.82]  into a new Z pool in order to expand the existing.
[1350.18 --> 1351.38]  That's a huge cost.
[1351.52 --> 1353.52]  And sometimes it's not even realistic
[1353.52 --> 1355.60]  because the user doesn't have enough SATA ports available
[1355.60 --> 1357.80]  to add that much storage to the server they're dealing with.
[1357.88 --> 1359.36]  So let's face facts.
[1359.46 --> 1361.30]  ZFS was not built for home users.
[1361.34 --> 1362.62]  It was built for the enterprise.
[1363.22 --> 1366.10]  We're trying to kind of bend that enterprise tool
[1366.10 --> 1367.68]  to be valuable to consumers,
[1367.68 --> 1369.72]  and I'm totally on board with it
[1369.72 --> 1371.82]  because I think there are some very cool things
[1371.82 --> 1372.72]  that you can do with ZFS,
[1372.92 --> 1374.40]  and I know there's plenty of people out there
[1374.40 --> 1376.18]  that use FreeNAS, for example,
[1376.26 --> 1378.40]  which is entirely based on using ZFS.
[1378.78 --> 1381.84]  So yeah, I'm on board with bringing it in-house
[1381.84 --> 1382.72]  and using it.
[1383.18 --> 1385.24]  It's just going to take a little time
[1385.24 --> 1386.42]  for us to get it fully implemented,
[1386.72 --> 1389.08]  but it's something that we are actively working on.
[1389.24 --> 1390.66]  I actually think that's a pretty fair answer.
[1390.78 --> 1392.34]  I think Alex and I both really agree with you.
[1392.34 --> 1394.42]  It is truly an enterprise file system,
[1394.64 --> 1395.88]  and if you have an enterprise budget,
[1396.00 --> 1396.96]  it's very manageable.
[1397.72 --> 1400.78]  If you're a high-end home user,
[1400.96 --> 1401.72]  and you can make it work,
[1401.76 --> 1402.62]  I'm doing it right now,
[1402.70 --> 1404.42]  but I went out and got a super micro chassis
[1404.42 --> 1406.64]  to make it happen.
[1406.90 --> 1407.46]  And that's the reality.
[1407.54 --> 1408.78]  I mean, the majority of our customers,
[1409.22 --> 1410.16]  they're not doing that.
[1410.38 --> 1411.96]  They're taking an old PC,
[1412.38 --> 1414.84]  and they're repurposing it for the use as a server.
[1415.02 --> 1416.86]  And honestly, that's what I used to do
[1416.86 --> 1418.60]  when I was building PCs as a young'un.
[1418.70 --> 1420.32]  Like when I was first getting into technology,
[1420.92 --> 1422.02]  what was my first PC?
[1422.16 --> 1424.34]  It's a gaming PC, like most tech people, right?
[1424.68 --> 1426.38]  But then that gaming PC gets a little old,
[1426.48 --> 1427.16]  and you realize,
[1427.28 --> 1428.70]  well, I can't really upgrade it anymore.
[1428.90 --> 1429.82]  Time to build a new one.
[1430.16 --> 1431.14]  So you take the old one,
[1431.38 --> 1432.12]  and you make it your server.
[1432.48 --> 1433.40]  It's a good value.
[1433.54 --> 1434.78]  So John, along those lines,
[1434.84 --> 1436.12]  I guess my question is,
[1436.20 --> 1437.42]  you must see a lot of different builds
[1437.42 --> 1438.90]  just being inside the company
[1438.90 --> 1440.20]  and seeing different stuff online.
[1440.70 --> 1442.36]  Does one really stand out to you
[1442.36 --> 1444.30]  as a pretty amazing Unraid build?
[1444.30 --> 1445.02]  Oh, come on.
[1445.16 --> 1446.82]  Have you not seen any of the Linus videos
[1446.82 --> 1447.64]  from Linus Tech Tips?
[1447.82 --> 1448.18]  Come on.
[1448.46 --> 1450.16]  I thought that might be your answer.
[1450.32 --> 1451.66]  If I don't point my finger
[1451.66 --> 1453.64]  at at least nine of those builds,
[1453.78 --> 1454.44]  then yeah.
[1454.56 --> 1456.00]  I mean, those are the crazy.
[1456.44 --> 1459.12]  I remember that the craziest one
[1459.12 --> 1461.18]  had to be the seven gamers one.
[1461.26 --> 1463.16]  Not the nine, not the eight, but the seven.
[1463.56 --> 1465.10]  And the reason the seven was so crazy
[1465.10 --> 1466.88]  was because Linus calls us up,
[1467.56 --> 1468.30]  calls me up.
[1468.34 --> 1469.00]  He only calls me.
[1469.50 --> 1470.26]  And he says,
[1470.32 --> 1470.56]  hey,
[1471.38 --> 1471.56]  he says,
[1471.56 --> 1474.32]  I got seven of these AMD nano GPUs coming.
[1474.42 --> 1475.36]  As soon as he says AMD,
[1475.36 --> 1477.34]  my hairs on the back of my neck rise
[1477.34 --> 1480.42]  because I cannot stand AMD GPUs
[1480.42 --> 1481.48]  for one reason,
[1481.56 --> 1482.90]  and that's because VM pass-through
[1482.90 --> 1484.36]  with those is a royal pain.
[1484.82 --> 1485.06]  I just,
[1485.32 --> 1485.74]  NVIDIA,
[1485.96 --> 1487.86]  I know that there's a lot of Linux people
[1487.86 --> 1488.54]  that hate NVIDIA
[1488.54 --> 1489.74]  for how they handle open source,
[1489.82 --> 1491.06]  and I understand that.
[1491.14 --> 1491.82]  I totally get it.
[1491.86 --> 1493.10]  But when it comes down
[1493.10 --> 1494.42]  to what works and what doesn't,
[1494.86 --> 1496.64]  I've rarely had problems
[1496.64 --> 1498.08]  getting NVIDIA GPUs to pass-through.
[1498.24 --> 1500.04]  I always have problems with AMD.
[1500.20 --> 1500.52]  Okay.
[1500.76 --> 1501.02]  So he's like,
[1501.04 --> 1502.60]  I got these brand new,
[1503.12 --> 1505.98]  never before seen AMD GPUs.
[1506.30 --> 1506.46]  Oh,
[1506.48 --> 1507.12]  and by the way,
[1507.26 --> 1509.22]  I'm going to rip all of the coolers
[1509.22 --> 1510.28]  off these GPUs,
[1510.30 --> 1510.98]  and I'm going to have
[1510.98 --> 1512.22]  a cooler manufacturer
[1512.22 --> 1514.78]  make me a custom block,
[1515.06 --> 1516.44]  custom water cooling block
[1516.44 --> 1518.08]  that's going to be one block
[1518.08 --> 1519.90]  that's going to slide into this system
[1519.90 --> 1521.74]  and cool all seven of those cards
[1521.74 --> 1522.60]  at the same time.
[1522.60 --> 1524.50]  Can I go under the hood for a second?
[1524.62 --> 1525.70]  Because I know that this is something
[1525.70 --> 1527.98]  that you don't touch on a lot,
[1528.06 --> 1529.50]  but it's based on Slackware, right?
[1529.50 --> 1530.58]  That's our distribution.
[1530.70 --> 1530.80]  Yeah,
[1530.84 --> 1531.52]  that's the,
[1532.10 --> 1532.32]  yeah.
[1532.64 --> 1534.48]  Do you have any measurements on this?
[1534.58 --> 1535.76]  But as far as you know,
[1535.88 --> 1537.92]  are you perhaps the most widely spread
[1537.92 --> 1540.76]  Slackware Linux distribution in existence?
[1541.12 --> 1542.50]  It probably wouldn't surprise me.
[1542.70 --> 1543.56]  I don't know.
[1543.62 --> 1545.06]  I don't know for a fact,
[1545.12 --> 1545.40]  but I mean,
[1545.42 --> 1546.28]  let's face facts.
[1546.36 --> 1548.20]  When you think about Linux distributions,
[1548.88 --> 1550.32]  the top names that come to mind
[1550.32 --> 1550.90]  are probably,
[1551.04 --> 1551.34]  you know,
[1551.44 --> 1551.88]  Ubuntu,
[1552.10 --> 1552.68]  Fedora,
[1552.98 --> 1553.40]  Arch,
[1553.68 --> 1553.90]  you know,
[1553.96 --> 1554.76]  that group.
[1555.60 --> 1558.18]  Slackware is like the very last one
[1558.18 --> 1559.42]  that I think people think about
[1559.42 --> 1560.78]  because it's not really built
[1560.78 --> 1562.70]  for everyday Linux users.
[1562.70 --> 1564.56]  It's built for guys
[1564.56 --> 1565.70]  that are building platforms.
[1565.70 --> 1567.00]  It's built for people
[1567.00 --> 1568.20]  that want to really tinker
[1568.20 --> 1569.36]  or really want to rip
[1569.36 --> 1570.20]  the whole thing apart.
[1570.32 --> 1571.60]  Like what you can do
[1571.60 --> 1572.88]  with a Slackware distribution
[1572.88 --> 1573.52]  in terms of,
[1573.64 --> 1574.76]  from a developer's perspective,
[1574.76 --> 1577.20]  is so much more fine-tuned
[1577.20 --> 1578.54]  than what you do
[1578.54 --> 1579.62]  with traditional distros.
[1579.84 --> 1580.06]  Like,
[1580.40 --> 1581.48]  think about how small
[1581.48 --> 1582.76]  Unraid is as a release.
[1583.08 --> 1583.62]  I couldn't do that
[1583.62 --> 1584.00]  with Ubuntu.
[1584.76 --> 1584.92]  I could,
[1584.98 --> 1585.24]  I just,
[1585.34 --> 1585.50]  I mean,
[1585.56 --> 1586.48]  and by the time I,
[1586.60 --> 1587.16]  if I could,
[1587.40 --> 1588.42]  by the time I'd get there,
[1588.46 --> 1588.78]  I'd say,
[1588.84 --> 1588.96]  well,
[1589.04 --> 1589.84]  I could have done it
[1589.84 --> 1590.26]  a lot quicker
[1590.26 --> 1591.18]  using a different platform.
[1591.40 --> 1591.64]  So,
[1592.18 --> 1592.42]  yeah,
[1592.46 --> 1594.02]  we're probably the largest,
[1594.20 --> 1595.34]  I would think we're probably
[1595.34 --> 1596.62]  the largest Slackware distribution
[1596.62 --> 1597.00]  out there.
[1597.14 --> 1598.20]  I thought that might be the case,
[1598.24 --> 1599.10]  which is just something
[1599.10 --> 1600.10]  I don't think a lot of people
[1600.10 --> 1601.06]  have given a nod to
[1601.06 --> 1601.60]  or consideration
[1601.60 --> 1604.40]  because it's one of the originals.
[1604.60 --> 1604.68]  So,
[1604.74 --> 1605.66]  it's pretty great to see it
[1605.66 --> 1606.76]  in widespread use out there.
[1607.08 --> 1607.40]  Absolutely.
[1607.74 --> 1607.92]  I mean,
[1607.98 --> 1608.92]  we love Patrick,
[1609.12 --> 1610.20]  but I can never pronounce
[1610.20 --> 1610.80]  his last name.
[1611.52 --> 1611.88]  So,
[1612.00 --> 1612.50]  Patrick V,
[1612.58 --> 1613.62]  we're just going to say Patrick V.
[1613.62 --> 1614.06]  Yes.
[1614.46 --> 1614.72]  You know,
[1614.76 --> 1615.46]  we have great respect
[1615.46 --> 1616.52]  for the work that he's done
[1616.52 --> 1616.74]  and,
[1616.82 --> 1617.60]  you know,
[1617.76 --> 1619.42]  it's been a great platform.
[1619.52 --> 1620.00]  And the funny thing
[1620.00 --> 1620.80]  about Slackware
[1620.80 --> 1621.22]  is that like,
[1621.24 --> 1621.84]  because this conversation
[1621.84 --> 1622.74]  comes up about Slackware
[1622.74 --> 1623.96]  once in a blue moon,
[1624.08 --> 1625.54]  came up a lot years ago.
[1626.02 --> 1626.68]  We really haven't heard
[1626.68 --> 1627.36]  anything about it since.
[1627.44 --> 1628.04]  The reality is,
[1628.06 --> 1629.18]  is that Slackware,
[1629.34 --> 1629.54]  Arch,
[1629.62 --> 1630.60]  it really does not,
[1630.68 --> 1631.52]  for us as a company,
[1631.58 --> 1632.34]  it does not matter.
[1632.80 --> 1632.98]  Like,
[1633.12 --> 1634.40]  Linux is not about
[1634.40 --> 1635.24]  the distribution,
[1635.42 --> 1636.12]  it's about the kernel.
[1636.52 --> 1637.82]  It's about what can the kernel do.
[1638.08 --> 1639.50]  And all a distribution is,
[1639.52 --> 1641.26]  is a way to wrap up
[1641.26 --> 1642.36]  what the kernel can do
[1642.36 --> 1643.18]  into a more
[1643.18 --> 1644.26]  manageable way.
[1644.74 --> 1646.20]  And when it comes to us,
[1646.30 --> 1646.52]  you know,
[1646.60 --> 1646.84]  we've,
[1646.84 --> 1647.40]  we went through,
[1647.46 --> 1648.28]  we've always gone through
[1648.28 --> 1649.46]  discussions where we talk about,
[1649.54 --> 1649.66]  well,
[1649.66 --> 1650.26]  should we switch?
[1650.32 --> 1651.36]  Should we move to a different platform?
[1651.52 --> 1652.64]  And we might at some point,
[1652.68 --> 1653.04]  we might,
[1653.50 --> 1654.30]  but the reality is,
[1654.34 --> 1654.60]  is that,
[1654.70 --> 1656.44]  that one of the big value props
[1656.44 --> 1656.96]  that,
[1657.10 --> 1657.84]  that we have
[1657.84 --> 1659.24]  is the fact that Unraid runs
[1659.24 --> 1659.92]  as an appliance.
[1660.16 --> 1662.10]  It really is an appliance built OS.
[1662.10 --> 1663.36]  It's not Windows,
[1663.52 --> 1663.74]  right?
[1663.82 --> 1664.98]  Windows is a platform,
[1665.46 --> 1665.62]  right?
[1665.72 --> 1666.22]  Windows is,
[1666.22 --> 1666.52]  hey,
[1666.90 --> 1667.60]  you load Windows
[1667.60 --> 1668.36]  and then you load
[1668.36 --> 1669.12]  a bunch of other things
[1669.12 --> 1669.66]  into Windows
[1669.66 --> 1671.10]  and now it's an operating system.
[1671.24 --> 1671.96]  Now it has everything
[1671.96 --> 1672.42]  that it needs.
[1672.88 --> 1673.60]  We're an appliance.
[1673.70 --> 1674.36]  Everything that you need
[1674.36 --> 1674.70]  is in the,
[1674.70 --> 1675.42]  is in the stick.
[1675.88 --> 1676.62]  All in the stick.
[1676.74 --> 1676.82]  Your,
[1676.86 --> 1677.42]  your capabilities
[1677.42 --> 1678.08]  as a hypervisor,
[1678.26 --> 1678.44]  there.
[1678.58 --> 1678.84]  Docker,
[1679.06 --> 1679.20]  there.
[1679.34 --> 1680.10]  Management capability,
[1680.26 --> 1680.44]  there.
[1680.64 --> 1681.84]  Everything is built in.
[1682.22 --> 1683.36]  And what's great about Slackware
[1683.36 --> 1684.08]  is that we were able
[1684.08 --> 1684.94]  to kind of pull out
[1684.94 --> 1685.66]  all the nonsense
[1685.66 --> 1686.60]  that we didn't need
[1686.60 --> 1687.16]  in the kernel,
[1687.30 --> 1688.14]  everything we didn't need
[1688.14 --> 1688.76]  in the OS,
[1689.22 --> 1690.24]  and really get it down
[1690.24 --> 1691.72]  to a very minimalistic build.
[1692.32 --> 1692.54]  And that,
[1692.68 --> 1693.12]  I think that's,
[1693.42 --> 1693.66]  that's,
[1693.72 --> 1694.70]  honestly is one of my
[1694.70 --> 1695.58]  favorite things about Unraid
[1695.58 --> 1696.72]  is how minimalistic
[1696.72 --> 1697.90]  the OS really is.
[1698.32 --> 1699.26]  You hit the nail on the head.
[1699.62 --> 1700.90]  It was a few years ago,
[1701.02 --> 1701.36]  I think,
[1701.48 --> 1702.28]  sort of 2013,
[1702.64 --> 1704.16]  14 sort of period
[1704.16 --> 1705.08]  that I think you and I
[1705.08 --> 1706.04]  first crossed paths.
[1706.78 --> 1707.52]  And this was when
[1707.52 --> 1708.70]  Docker was being added
[1708.70 --> 1709.94]  for the very first time
[1709.94 --> 1710.52]  to Unraid.
[1711.06 --> 1711.80]  And round about
[1711.80 --> 1712.88]  that sort of time,
[1712.88 --> 1713.92]  we were running
[1713.92 --> 1715.30]  custom VMs
[1715.30 --> 1716.88]  to run media apps.
[1717.08 --> 1718.16]  And it was just
[1718.16 --> 1719.00]  this whole layer
[1719.00 --> 1719.64]  of abstraction
[1719.64 --> 1720.42]  and complexity
[1720.42 --> 1722.12]  which now
[1722.12 --> 1723.72]  with containers
[1723.72 --> 1724.48]  is just,
[1724.56 --> 1725.50]  it's not a problem.
[1725.74 --> 1727.02]  So the base OS
[1727.02 --> 1728.10]  just doesn't matter anymore.
[1728.20 --> 1729.56]  And I'm a strong believer
[1729.56 --> 1730.02]  of that
[1730.02 --> 1731.28]  as long as you can run
[1731.28 --> 1731.78]  a container,
[1731.98 --> 1732.54]  you can run
[1732.54 --> 1733.70]  whatever OS you want.
[1734.14 --> 1734.88]  That's exactly right.
[1735.04 --> 1735.36]  And I mean,
[1735.38 --> 1736.20]  the funny thing is,
[1736.22 --> 1736.70]  is that so
[1736.70 --> 1737.92]  when we were working
[1737.92 --> 1738.48]  on 6,
[1739.10 --> 1740.76]  the reason that VMs
[1740.76 --> 1741.36]  were initially
[1741.36 --> 1742.78]  like looked at
[1742.78 --> 1743.98]  was not because
[1743.98 --> 1744.46]  of something
[1744.46 --> 1745.74]  that Tom wanted originally.
[1745.74 --> 1746.38]  It was because
[1746.38 --> 1747.42]  of what people wanted,
[1747.68 --> 1748.72]  what our customers wanted,
[1748.80 --> 1749.76]  what our users were using.
[1749.76 --> 1750.54]  And so what we found
[1750.54 --> 1750.86]  was that
[1750.86 --> 1752.52]  the big calling card
[1752.52 --> 1752.94]  to Unraid
[1752.94 --> 1753.98]  in the five days
[1753.98 --> 1754.62]  were plugins.
[1755.30 --> 1756.30]  That was the,
[1756.30 --> 1757.06]  you know,
[1757.12 --> 1758.04]  cat's pajamas right there.
[1758.16 --> 1758.98]  Everybody was downloading
[1758.98 --> 1759.72]  the Plex plugin
[1759.72 --> 1761.22]  and, you know,
[1761.26 --> 1762.46]  that guy Faze
[1762.46 --> 1763.06]  in our community,
[1763.16 --> 1763.82]  he created all
[1763.82 --> 1764.48]  these different plugins
[1764.48 --> 1766.48]  and it just extended
[1766.48 --> 1767.18]  the value of Unraid.
[1767.32 --> 1767.40]  You know,
[1767.42 --> 1768.08]  you didn't have a feature
[1768.08 --> 1768.50]  that you wanted,
[1768.56 --> 1769.20]  you'd add a plugin.
[1769.86 --> 1770.36]  The problem,
[1770.46 --> 1771.38]  that's where Slackware's
[1771.38 --> 1772.50]  weakness was exposed though
[1772.50 --> 1773.04]  because in order
[1773.04 --> 1773.86]  to run these plugins,
[1774.44 --> 1775.10]  you'd have to be able
[1775.10 --> 1775.80]  to download
[1775.80 --> 1777.16]  these packages
[1777.16 --> 1778.16]  and install them
[1778.16 --> 1778.86]  that were built
[1778.86 --> 1779.80]  for Slackware
[1779.80 --> 1780.64]  and you'd find
[1780.64 --> 1781.08]  that there were
[1781.08 --> 1781.82]  plenty of packages
[1781.82 --> 1782.20]  out there
[1782.20 --> 1783.10]  that just weren't built.
[1783.46 --> 1784.34]  I was surprised
[1784.34 --> 1785.44]  when I joined the company
[1785.44 --> 1787.16]  that Plex actually
[1787.16 --> 1787.98]  had a build
[1787.98 --> 1789.20]  that they made
[1789.20 --> 1789.82]  that somebody
[1789.82 --> 1790.54]  didn't have to hack through.
[1790.64 --> 1791.08]  They made
[1791.08 --> 1791.78]  and they supported
[1791.78 --> 1792.60]  for Unraid,
[1792.72 --> 1793.12]  which tells you
[1793.12 --> 1794.14]  how big we must have been
[1794.14 --> 1795.00]  for their community.
[1795.62 --> 1795.88]  And so,
[1795.98 --> 1796.12]  yeah,
[1796.16 --> 1797.06]  we saw all these people
[1797.06 --> 1797.60]  using plugins
[1797.60 --> 1798.14]  and Tom's like,
[1798.18 --> 1798.32]  you know,
[1798.36 --> 1799.36]  this is just not manageable.
[1799.80 --> 1800.96]  So our choices are
[1800.96 --> 1802.12]  move to a platform
[1802.12 --> 1802.84]  where it is
[1802.84 --> 1803.44]  or find a way
[1803.44 --> 1803.94]  to make it work
[1803.94 --> 1804.68]  on what we have
[1804.68 --> 1805.74]  and VMs
[1805.74 --> 1806.84]  were the first foray
[1806.84 --> 1807.28]  into that.
[1807.36 --> 1807.82]  And I think you were
[1807.82 --> 1808.34]  involved in that
[1808.34 --> 1809.00]  a little bit, Alex,
[1809.06 --> 1810.12]  where Tom reached out
[1810.12 --> 1810.28]  to you
[1810.28 --> 1810.78]  and you were creating
[1810.78 --> 1811.66]  some VM templates
[1811.66 --> 1812.50]  and things like that.
[1813.04 --> 1813.76]  But then as we were
[1813.76 --> 1814.60]  going down that road,
[1814.66 --> 1815.12]  there was a couple
[1815.12 --> 1815.60]  different things
[1815.60 --> 1816.14]  that we discovered.
[1816.26 --> 1816.86]  The first was
[1816.86 --> 1817.60]  that we were originally
[1817.60 --> 1818.28]  using Zen
[1818.28 --> 1819.20]  as our hypervisor
[1819.20 --> 1819.74]  and Zen's,
[1820.12 --> 1821.56]  the reason that I like Zen
[1821.56 --> 1821.90]  so much
[1821.90 --> 1822.46]  is I actually come
[1822.46 --> 1823.30]  from the Citrix world
[1823.30 --> 1824.80]  prior to LimeTech
[1824.80 --> 1825.58]  and that was,
[1825.92 --> 1826.66]  Citrix's big thing
[1826.66 --> 1827.10]  was Zen
[1827.10 --> 1827.74]  and Zen server.
[1828.48 --> 1829.02]  And I thought,
[1829.14 --> 1829.26]  wow,
[1829.32 --> 1829.80]  this is great.
[1829.90 --> 1830.70]  It's a similar platform.
[1830.82 --> 1831.30]  Let's try it.
[1831.84 --> 1832.10]  You know,
[1832.10 --> 1833.02]  I like the way
[1833.02 --> 1834.18]  that the whole project
[1834.18 --> 1834.86]  was structured,
[1835.06 --> 1836.08]  but we had a lot
[1836.08 --> 1836.82]  of problems with Zen.
[1837.00 --> 1837.52]  And specifically
[1837.52 --> 1838.46]  with GPU pass-through,
[1838.50 --> 1838.88]  we had a lot
[1838.88 --> 1839.50]  of problems with Zen.
[1840.10 --> 1840.76]  And so then we looked
[1840.76 --> 1841.48]  into KVM
[1841.48 --> 1841.84]  and we're like,
[1841.88 --> 1842.04]  wow,
[1842.08 --> 1842.68]  this is going to solve
[1842.68 --> 1843.60]  all of our GPU pass-through
[1843.60 --> 1843.94]  problems.
[1844.04 --> 1845.50]  But then the question
[1845.50 --> 1845.88]  became,
[1845.98 --> 1846.10]  well,
[1846.10 --> 1846.48]  wait a minute.
[1846.86 --> 1847.64]  Do I really need
[1847.64 --> 1848.30]  a 10 gig
[1848.30 --> 1849.44]  or even a 1 gig
[1849.44 --> 1850.66]  size V disk
[1850.66 --> 1852.06]  to run Plex?
[1852.62 --> 1852.84]  Like,
[1852.88 --> 1854.18]  does that seem
[1854.18 --> 1855.30]  like a good trade-off
[1855.30 --> 1856.30]  and then the user
[1856.30 --> 1857.38]  has to manage that?
[1857.54 --> 1857.58]  Like,
[1857.62 --> 1858.28]  they can't just
[1858.28 --> 1858.78]  automatically,
[1859.02 --> 1859.60]  Plex isn't going
[1859.60 --> 1860.46]  to just auto-update.
[1860.64 --> 1860.70]  Like,
[1860.72 --> 1861.46]  you have to manage
[1861.46 --> 1861.96]  that VM
[1861.96 --> 1862.42]  and you have to
[1862.42 --> 1863.20]  manage the OS
[1863.20 --> 1863.68]  in that VM.
[1863.86 --> 1864.64]  And it just,
[1864.74 --> 1865.36]  there was so much
[1865.36 --> 1866.82]  additional stuff
[1866.82 --> 1868.02]  that came with VMs
[1868.02 --> 1869.06]  that didn't come
[1869.06 --> 1869.62]  with containers.
[1869.62 --> 1870.28]  And I remember
[1870.28 --> 1871.82]  a guy in our community
[1871.82 --> 1872.76]  by the name of Naz,
[1872.82 --> 1873.54]  that's his handle
[1873.54 --> 1874.10]  in our forum,
[1874.58 --> 1875.72]  had once posted
[1875.72 --> 1876.36]  a feature request
[1876.36 --> 1876.70]  and he just,
[1876.80 --> 1877.40]  real short,
[1877.50 --> 1877.62]  just,
[1877.72 --> 1877.90]  hey,
[1878.46 --> 1879.14]  there's this new thing,
[1879.22 --> 1879.46]  Docker.
[1879.92 --> 1880.72]  I think it looks
[1880.72 --> 1881.26]  pretty cool.
[1881.76 --> 1882.18]  You guys should
[1882.18 --> 1882.64]  check it out.
[1883.20 --> 1884.02]  And so Eric,
[1884.12 --> 1884.62]  our CTO,
[1884.82 --> 1885.32]  and myself,
[1885.42 --> 1886.30]  we started looking at it
[1886.30 --> 1886.70]  and I'm like,
[1887.42 --> 1888.60]  the first week
[1888.60 --> 1889.70]  I'm looking at Docker,
[1890.36 --> 1890.90]  I was just,
[1890.90 --> 1891.98]  I'm so confused.
[1892.08 --> 1892.62]  I'm looking at it
[1892.62 --> 1892.92]  and I'm like,
[1893.30 --> 1894.50]  this thing sounds great
[1894.50 --> 1895.86]  but it also is so confusing
[1895.86 --> 1896.82]  I don't understand it.
[1897.30 --> 1898.24]  And then we just built it.
[1898.36 --> 1899.98]  So Eric went into the dungeon
[1899.98 --> 1901.54]  and built a release of Unraid
[1901.54 --> 1902.28]  that supported Docker
[1902.28 --> 1903.20]  and Eric's like,
[1903.24 --> 1904.04]  I'm about to show you
[1904.04 --> 1904.78]  how great this is.
[1904.86 --> 1905.78]  Here's what I want you to type.
[1905.92 --> 1907.04]  Docker run space,
[1907.18 --> 1907.68]  blah, blah, blah, blah.
[1907.72 --> 1908.72]  I gave me a command to run.
[1909.36 --> 1909.92]  And I hit enter
[1909.92 --> 1910.22]  and I'm like,
[1910.26 --> 1910.74]  okay, now what?
[1910.78 --> 1911.00]  And he goes,
[1911.08 --> 1911.66]  that's it.
[1911.78 --> 1912.60]  You're running Plex.
[1912.90 --> 1913.18]  Yep.
[1913.32 --> 1913.58]  I'm like,
[1913.64 --> 1913.80]  what?
[1913.80 --> 1915.28]  And I type in the IP
[1915.28 --> 1915.76]  and sure shit,
[1915.86 --> 1916.38]  Plex is loading,
[1916.50 --> 1916.80]  it's running,
[1916.92 --> 1917.52]  it's doing its thing.
[1920.90 --> 1921.92]  That's where everything fell in.
[1921.98 --> 1923.32]  Like this is just this big,
[1923.82 --> 1925.32]  what's the meme out there?
[1925.40 --> 1926.46]  Nyan cat or whatever
[1926.46 --> 1927.76]  when the thing goes like,
[1928.12 --> 1928.70]  like it's like,
[1928.70 --> 1931.06]  the movie Limitless or whatever.
[1931.14 --> 1931.42]  All of a sudden
[1931.42 --> 1932.40]  you understand everything.
[1932.52 --> 1933.28]  Everything falls in a place.
[1933.36 --> 1933.94]  It's like the moment
[1933.94 --> 1934.82]  Doc Brown hits his head
[1934.82 --> 1935.30]  on the toilet
[1935.30 --> 1936.94]  and thinks of the flux capacity.
[1937.32 --> 1937.68]  Exactly.
[1938.22 --> 1939.86]  And so I remember calling Tom
[1939.86 --> 1941.02]  and I think,
[1941.14 --> 1942.24]  I honestly think it might've been
[1942.24 --> 1942.92]  in the middle of the night.
[1943.02 --> 1943.86]  It might've been like
[1943.86 --> 1944.72]  really late at night.
[1944.76 --> 1944.94]  I'm like,
[1944.98 --> 1945.26]  Tom.
[1945.62 --> 1946.22]  And he's like,
[1946.22 --> 1947.16]  John, what's up?
[1947.16 --> 1947.60]  And I'm like,
[1947.62 --> 1948.28]  this thing,
[1948.38 --> 1949.28]  you got to see it.
[1949.58 --> 1950.72]  So we got him the build
[1950.72 --> 1951.34]  and he's like,
[1951.38 --> 1951.52]  okay,
[1951.54 --> 1952.24]  now what I had,
[1952.32 --> 1953.26]  I literally was on the phone.
[1953.34 --> 1953.90]  I walked him through
[1953.90 --> 1954.12]  and I'm like,
[1954.18 --> 1955.54]  type this command run
[1955.54 --> 1955.94]  and he's,
[1956.08 --> 1956.96]  he gets it up and running
[1956.96 --> 1957.40]  and he's like,
[1957.58 --> 1957.74]  okay,
[1957.74 --> 1958.46]  now that was pretty cool.
[1958.64 --> 1958.94]  Yeah.
[1959.14 --> 1961.20]  And we all had this eyeopening moment
[1961.20 --> 1962.06]  of we got to do this.
[1962.10 --> 1963.90]  And so the funny thing about it too
[1963.90 --> 1964.32]  is that we,
[1964.58 --> 1965.38]  the first iteration
[1965.38 --> 1967.42]  of building a Docker management interface
[1967.42 --> 1968.84]  was nothing compared
[1968.84 --> 1969.52]  to what it is today.
[1969.54 --> 1969.82]  It was,
[1970.28 --> 1970.92]  it was honestly,
[1970.98 --> 1971.70]  it was pretty piss poor,
[1971.86 --> 1973.16]  but it did the job.
[1973.32 --> 1974.08]  It worked,
[1974.18 --> 1975.30]  but it required users
[1975.30 --> 1977.16]  to add these template repos
[1977.16 --> 1978.48]  and people would have to build
[1978.48 --> 1979.92]  their apps on GitHub
[1979.92 --> 1981.16]  and then link these repos
[1981.16 --> 1981.32]  and all.
[1981.88 --> 1982.96]  And just putting out
[1982.96 --> 1983.50]  like the first,
[1983.58 --> 1984.80]  I think the first beta releases
[1984.80 --> 1985.94]  that we had with this in there,
[1986.34 --> 1987.54]  the community just took it
[1987.54 --> 1988.28]  and ran with it.
[1988.34 --> 1988.92]  And that's how we have
[1988.92 --> 1989.96]  the community app store.
[1990.36 --> 1990.86]  That's how we have
[1990.86 --> 1992.02]  the new Docker manager
[1992.02 --> 1993.76]  that that's way more polished
[1993.76 --> 1994.70]  than what the old one was.
[1995.04 --> 1996.02]  It's just crazy
[1996.02 --> 1997.14]  how fast
[1997.14 --> 1999.60]  everything clicked into place
[1999.60 --> 2001.10]  after we put it out there.
[2001.22 --> 2001.36]  So,
[2001.46 --> 2001.60]  I mean,
[2001.66 --> 2002.24]  Docker is,
[2003.00 --> 2003.96]  Docker is awesome.
[2004.16 --> 2005.16]  I got no other way to put it.
[2005.16 --> 2005.72]  It's just awesome.
[2005.72 --> 2007.84]  I think my Doc Brown moment
[2007.84 --> 2010.28]  was when I set everything up
[2010.28 --> 2010.88]  and I really,
[2011.02 --> 2011.20]  you know,
[2011.26 --> 2012.60]  I had a good configuration.
[2013.16 --> 2014.90]  I tore the container down
[2014.90 --> 2016.54]  and then stood up
[2016.54 --> 2018.04]  a new version of the container
[2018.04 --> 2019.28]  and it just resumed
[2019.28 --> 2020.04]  and the data
[2020.04 --> 2021.28]  was completely separate
[2021.28 --> 2022.32]  from the application.
[2022.64 --> 2022.74]  Yep.
[2022.86 --> 2023.90]  And that was the moment
[2023.90 --> 2024.24]  I went,
[2024.46 --> 2024.78]  aha,
[2025.32 --> 2025.92]  I get it.
[2026.06 --> 2026.86]  This solves a problem
[2026.86 --> 2028.52]  I fought forever in IT.
[2028.76 --> 2028.92]  So,
[2029.06 --> 2030.04]  I love that story.
[2030.10 --> 2030.58]  It's sort of like
[2030.58 --> 2031.90]  the Docker origin story
[2031.90 --> 2032.54]  in Unraid.
[2032.80 --> 2032.82]  So,
[2032.82 --> 2034.30]  my last question
[2034.30 --> 2034.98]  is I kind of want
[2034.98 --> 2035.66]  to tease out of you
[2035.66 --> 2036.66]  anything you can give us
[2036.66 --> 2037.32]  about this
[2037.32 --> 2039.34]  soon.unraid.net
[2039.34 --> 2040.88]  which says
[2040.88 --> 2041.40]  the team has been
[2041.40 --> 2042.46]  working hard on something
[2042.46 --> 2043.70]  we're calling my servers
[2043.70 --> 2045.06]  to be released soon.
[2045.24 --> 2046.60]  What are you talking about?
[2046.74 --> 2048.14]  I have no idea
[2048.14 --> 2049.30]  what you're talking about.
[2049.52 --> 2049.96]  Hmm.
[2050.12 --> 2050.84]  Are you talking about
[2050.84 --> 2051.24]  the little,
[2051.48 --> 2051.84]  did you,
[2051.94 --> 2052.38]  okay now,
[2052.48 --> 2052.80]  hold on.
[2052.90 --> 2054.28]  Did you actually find
[2054.28 --> 2055.32]  the Easter egg
[2055.32 --> 2056.10]  or did somebody
[2056.10 --> 2056.86]  just tell you?
[2056.92 --> 2057.80]  Let's start with them.
[2058.08 --> 2059.58]  I may have informants.
[2059.80 --> 2060.94]  They may be named Alex,
[2061.06 --> 2061.56]  but I mean,
[2061.58 --> 2062.24]  we found this
[2062.24 --> 2063.02]  and I noticed
[2063.02 --> 2064.08]  it seems to be legit.
[2064.20 --> 2064.88]  The color scheme
[2064.88 --> 2065.56]  looks on point.
[2065.66 --> 2066.90]  It's SSL signed.
[2067.60 --> 2068.30]  It's legit.
[2068.66 --> 2069.06]  So,
[2069.12 --> 2070.34]  so if you're interested
[2070.34 --> 2071.68]  in getting involved
[2071.68 --> 2072.90]  in being able
[2072.90 --> 2074.20]  to test some new things
[2074.20 --> 2075.28]  that you want
[2075.28 --> 2075.68]  to get ahead
[2075.68 --> 2076.00]  of the rest
[2076.00 --> 2076.80]  of the community on,
[2077.24 --> 2077.64]  that's where
[2077.64 --> 2078.38]  to sign up for it.
[2078.74 --> 2079.62]  All I can say
[2079.62 --> 2080.36]  is that
[2080.36 --> 2081.80]  we have some
[2081.80 --> 2082.68]  pretty big plans
[2082.68 --> 2083.46]  to roll out
[2083.46 --> 2084.68]  some pretty nice services
[2084.68 --> 2085.74]  to complement the OS.
[2085.88 --> 2086.54]  We talked about this
[2086.54 --> 2087.10]  a little earlier
[2087.10 --> 2088.60]  and we are looking
[2088.60 --> 2089.84]  to get people in line
[2089.84 --> 2090.72]  that want to start
[2090.72 --> 2091.64]  testing that for us
[2091.64 --> 2092.42]  a little bit more
[2092.42 --> 2093.30]  rigorously.
[2093.58 --> 2094.44]  We've been personally
[2094.44 --> 2095.24]  testing it for
[2095.24 --> 2096.42]  all over a year now
[2096.42 --> 2097.72]  and we're pretty confident
[2097.72 --> 2098.48]  with what we've built.
[2098.92 --> 2099.26]  Obviously,
[2099.38 --> 2100.32]  as soon as you expand it
[2100.32 --> 2100.72]  beyond,
[2100.94 --> 2101.26]  you know,
[2101.44 --> 2102.28]  the size of a room,
[2102.60 --> 2103.72]  people are going to find
[2103.72 --> 2104.34]  chinks in the armor.
[2104.50 --> 2104.60]  So,
[2104.98 --> 2106.56]  it's a beta testing
[2106.56 --> 2107.42]  program sign up.
[2107.50 --> 2108.50]  That's the core of it.
[2108.82 --> 2109.26]  That sounds like
[2109.26 --> 2109.66]  a good thing.
[2109.72 --> 2109.80]  So,
[2109.86 --> 2110.26]  we'll put a link
[2110.26 --> 2111.06]  to that in the show notes
[2111.06 --> 2112.58]  soon.unraid.net.
[2112.94 --> 2113.18]  John,
[2113.22 --> 2113.80]  where else should we
[2113.80 --> 2114.56]  send people?
[2114.72 --> 2115.08]  You mentioned
[2115.08 --> 2116.26]  there's a community area,
[2116.36 --> 2116.86]  it sounds like.
[2116.86 --> 2118.22]  Our forums are where
[2118.22 --> 2118.84]  everybody goes,
[2119.02 --> 2120.02]  both new users,
[2120.18 --> 2120.78]  existing users,
[2120.78 --> 2121.40]  and people that are
[2121.40 --> 2121.90]  thinking about
[2121.90 --> 2122.56]  becoming users.
[2122.94 --> 2123.82]  The biggest thing
[2123.82 --> 2124.66]  that I can guide people
[2124.66 --> 2125.38]  about Unraid is,
[2125.52 --> 2125.68]  okay,
[2125.96 --> 2126.36]  first,
[2126.66 --> 2127.38]  go on YouTube
[2127.38 --> 2128.76]  and watch Space Invader
[2128.76 --> 2129.34]  1's videos
[2129.34 --> 2130.02]  if you haven't.
[2130.54 --> 2131.98]  Ed is just an amazing guy
[2131.98 --> 2133.52]  and he has created
[2133.52 --> 2134.42]  so much content
[2134.42 --> 2135.04]  around Unraid
[2135.04 --> 2136.54]  and going so much deeper
[2136.54 --> 2137.90]  than we ever would
[2137.90 --> 2138.58]  as a company
[2138.58 --> 2140.44]  to explain all the nuances
[2140.44 --> 2141.20]  to how to configure
[2141.20 --> 2142.46]  all the most advanced things.
[2142.82 --> 2142.90]  So,
[2142.94 --> 2143.58]  if you have any questions
[2143.58 --> 2144.30]  about Unraid OS,
[2144.40 --> 2145.10]  if you want someone
[2145.10 --> 2146.02]  that's going to walk you
[2146.02 --> 2146.28]  through it,
[2146.32 --> 2146.58]  give you,
[2146.90 --> 2147.14]  you know,
[2147.20 --> 2148.52]  a nice presentation on it,
[2148.88 --> 2150.06]  I highly recommend
[2150.06 --> 2150.72]  checking that out.
[2151.12 --> 2151.56]  The other thing
[2151.56 --> 2152.28]  I obviously recommend
[2152.28 --> 2152.70]  checking out
[2152.70 --> 2154.16]  is Linus Tech Tips.
[2154.66 --> 2155.50]  Linus Sebastian's
[2155.50 --> 2156.70]  a big friend of the show
[2156.70 --> 2157.22]  or a big friend
[2157.22 --> 2157.98]  of the company
[2157.98 --> 2159.14]  and we lean on him
[2159.14 --> 2159.70]  pretty heavily
[2159.70 --> 2160.94]  to help kind of
[2160.94 --> 2161.54]  push the limits
[2161.54 --> 2162.28]  of what we can do
[2162.28 --> 2162.90]  with the software
[2162.90 --> 2163.68]  and,
[2163.82 --> 2164.28]  or I should say,
[2164.36 --> 2165.10]  he pushes us.
[2166.18 --> 2167.40]  And the other thing
[2167.40 --> 2168.06]  that I would recommend
[2168.06 --> 2168.68]  is that if people
[2168.68 --> 2169.18]  are wondering,
[2169.32 --> 2169.44]  you know,
[2169.50 --> 2169.68]  well,
[2169.70 --> 2170.24]  I want to build
[2170.24 --> 2170.80]  an Unraid server,
[2170.84 --> 2171.22]  I'm not sure
[2171.22 --> 2171.86]  what hardware to use,
[2172.14 --> 2172.60]  the forums.
[2173.08 --> 2174.32]  Our forums are like,
[2174.38 --> 2174.96]  we get emails
[2174.96 --> 2176.26]  pretty often about,
[2176.26 --> 2176.42]  well,
[2176.42 --> 2177.52]  what hardware should I use?
[2177.58 --> 2178.54]  And the reality is
[2178.54 --> 2179.60]  that we're not a hardware company,
[2179.68 --> 2180.44]  we're a software company.
[2180.58 --> 2182.36]  So our hardware requirements
[2182.36 --> 2183.08]  are pretty basic.
[2183.20 --> 2183.50]  You've got to have
[2183.50 --> 2184.52]  a 64-bit processor,
[2184.90 --> 2185.54]  I'd recommend
[2185.54 --> 2186.66]  at least 4 gigs of RAM
[2186.66 --> 2188.96]  and a decent USB flash stick,
[2189.04 --> 2189.48]  that's it.
[2189.82 --> 2190.56]  But then if you want
[2190.56 --> 2191.32]  to do VMs,
[2191.42 --> 2192.34]  your processor's got
[2192.34 --> 2193.34]  to support virtualization,
[2193.44 --> 2194.04]  it's got to support
[2194.04 --> 2194.60]  pass-through,
[2194.96 --> 2195.48]  and there's ways
[2195.48 --> 2196.20]  to look that up
[2196.20 --> 2197.06]  easier with Intel
[2197.06 --> 2197.64]  than with AMD.
[2197.64 --> 2198.78]  But, you know,
[2198.84 --> 2199.50]  if you're wondering,
[2199.66 --> 2199.74]  well,
[2199.74 --> 2200.26]  am I going to run
[2200.26 --> 2200.84]  into problems
[2200.84 --> 2201.88]  or if I use this hardware,
[2202.00 --> 2202.80]  are there any limitations?
[2202.90 --> 2203.72]  Just post in our forum,
[2203.86 --> 2204.80]  there's a good chance
[2204.80 --> 2205.86]  somebody's already used it.
[2205.98 --> 2206.72]  That's a good resource
[2206.72 --> 2207.46]  because it is such
[2207.46 --> 2208.14]  a varied thing.
[2208.20 --> 2208.86]  You need a community
[2208.86 --> 2209.86]  to lean on.
[2210.36 --> 2210.92]  Well, John,
[2211.06 --> 2212.06]  thanks for coming on.
[2212.12 --> 2212.82]  Do keep us in the loop
[2212.82 --> 2213.76]  on future developments
[2213.76 --> 2214.42]  and stuff so we can
[2214.42 --> 2215.52]  keep our audience informed
[2215.52 --> 2217.22]  and send us little nudges
[2217.22 --> 2217.64]  here and there
[2217.64 --> 2218.30]  as things develop
[2218.30 --> 2219.48]  because I think
[2219.48 --> 2220.22]  we'll be following.
[2220.48 --> 2221.70]  I'm kind of scratching
[2221.70 --> 2222.12]  my head.
[2222.20 --> 2223.62]  I think I have a couple
[2223.62 --> 2224.12]  of excuses
[2224.12 --> 2225.14]  to try out Unraid.
[2225.42 --> 2226.12]  I might give it a go
[2226.12 --> 2226.56]  here soon
[2226.56 --> 2227.12]  and report back
[2227.12 --> 2227.54]  on the show.
[2227.88 --> 2228.46]  If you get tired
[2228.46 --> 2229.42]  of rolling your own
[2229.42 --> 2230.86]  and you want to just have
[2230.86 --> 2232.16]  a packaged OS
[2232.16 --> 2233.34]  that you don't have
[2233.34 --> 2233.74]  to tinker
[2233.74 --> 2234.28]  and you don't have
[2234.28 --> 2234.68]  to manage,
[2234.78 --> 2235.36]  you can just mess
[2235.36 --> 2235.94]  with the apps
[2235.94 --> 2236.70]  and the VMs
[2236.70 --> 2237.26]  and the storage
[2237.26 --> 2237.90]  and that's it,
[2238.18 --> 2238.84]  we're for you.
[2239.16 --> 2240.34]  We're 100% for you.
[2240.48 --> 2241.36]  That's the elevator pitch
[2241.36 --> 2241.74]  right there.
[2241.98 --> 2242.66]  Remind me what you said
[2242.66 --> 2243.46]  at the start though,
[2243.82 --> 2244.04]  John.
[2245.22 --> 2245.74]  Wait, what?
[2245.76 --> 2246.28]  Zed?
[2249.86 --> 2250.86]  Well, I hope you enjoyed
[2250.86 --> 2251.72]  that chat with John
[2251.72 --> 2252.72]  as much as I did.
[2252.96 --> 2253.42]  As ever,
[2253.52 --> 2254.30]  you can find more
[2254.30 --> 2255.04]  about the show
[2255.04 --> 2256.72]  at selfhosted.show
[2256.72 --> 2257.76]  We're on Twitter
[2257.76 --> 2259.22]  at selfhosted.show
[2259.22 --> 2260.74]  Chris is at
[2260.74 --> 2262.00]  ChrisLAS on Twitter.
[2262.26 --> 2262.78]  I'm at
[2262.78 --> 2263.54]  IronicBadger
[2263.54 --> 2264.48]  and that was
[2264.48 --> 2265.88]  selfhosted.25.
[2265.88 --> 2267.66]  IronicBadger
[2267.66 --> 2268.04]  and that was
[2268.04 --> 2268.30]  you
[2268.30 --> 2268.92]  haveagens
[2268.92 --> 2276.84]  to
[2280.84 --> 2281.22]  puking
[2281.22 --> 2281.38]  he dangers
[2281.38 --> 2281.44]  as much.
