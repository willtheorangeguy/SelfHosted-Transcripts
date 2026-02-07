[0.00 --> 2.32]  Welcome into episode 128, everybody.
[2.78 --> 4.06]  Question for you, Chris.
[4.54 --> 6.84]  Are automated updates evil?
[7.52 --> 12.18]  I personally think that you should be able to have your automated updates and your stability too.
[12.68 --> 14.02]  But it depends on the system.
[14.44 --> 17.30]  Of course, you're inferring about the CrowdStrike sensor update
[17.30 --> 21.64]  that blue-screened lots of Windows machines that use CrowdStrike Falcon.
[22.26 --> 26.64]  In that particular case, I don't like the way those antivirus things auto-update.
[26.74 --> 27.86]  I think that's awful.
[27.86 --> 31.20]  And it's, of course, the value prop, actually, of the product.
[31.84 --> 35.00]  But on OSs and systems that you manage and deploy,
[35.08 --> 39.12]  where you have to do a build check first and make sure things check out and then you deploy,
[39.32 --> 42.90]  I think there can be room, especially if it's a highly sensitive system
[42.90 --> 47.24]  exposed to particularly intense kinds of scrutiny and attack.
[48.06 --> 52.44]  By this point, we are not the bearers of bad news, I'm certain, on this particular issue.
[52.90 --> 57.20]  CrowdStrike, of course, knocked out 8.5 million PCs worldwide
[57.20 --> 60.78]  over the last week or so with a faulty update.
[61.42 --> 61.54]  Yeah.
[63.04 --> 63.40]  Yeah.
[63.76 --> 68.68]  And it was, of course, also in combination with a few other things that went wrong
[68.68 --> 71.08]  and testing that wasn't properly done.
[71.26 --> 72.54]  Of course, now CrowdStrike has...
[73.18 --> 76.36]  Well, they've not only offered everybody that was affected an Uber Eats gift card
[76.36 --> 77.38]  for like 15 bucks.
[77.46 --> 78.28]  So that's good.
[78.62 --> 79.54]  I thought that was a meme.
[79.60 --> 80.22]  Is that true?
[80.22 --> 81.70]  I think it's actually true.
[81.80 --> 82.72]  Oh, goodness me.
[83.14 --> 86.88]  CloudStrike says they also plan to stagger future deployments of updates
[86.88 --> 90.06]  so that way they can be tested by the public in piecemeal.
[90.64 --> 91.02]  Crikey.
[91.10 --> 92.18]  Amazing that wasn't already that way.
[92.24 --> 92.44]  Yeah.
[92.56 --> 95.36]  I mean, we were doing this stuff when I was fresh out of university.
[95.82 --> 98.30]  I mean, it's just basic, basic stuff.
[98.82 --> 98.96]  Yeah.
[98.96 --> 101.24]  Especially if you're going to do the live patching.
[101.24 --> 105.96]  You think you would just, by default, do a rollout that,
[106.36 --> 109.26]  even if it was just phased by a few hours,
[109.42 --> 111.08]  it would be better than what they did.
[111.86 --> 115.32]  I saw some commentary that actually stated this is effectively what would happen
[115.32 --> 117.62]  in a real cyber warfare situation.
[118.48 --> 121.06]  And as we speak, it's almost a week after the event,
[121.40 --> 125.98]  and Delta are still cancelling hundreds of flights every day to recover from this
[125.98 --> 129.48]  because equipment's in the wrong place, crews are in the wrong place,
[129.48 --> 131.20]  booking systems are still down.
[131.64 --> 133.74]  It's just absolute chaos out there.
[134.20 --> 138.08]  Lenart Pottering said very correctly that these commercial operating systems
[138.08 --> 140.76]  at this point should have a failed boot count system
[140.76 --> 142.64]  and then an auto rollback system.
[143.14 --> 144.84]  And that's all it would really take to solve this,
[144.96 --> 147.52]  is if Windows detected, oh, I've had multiple boot failures,
[148.12 --> 150.78]  let me boot into the previous image.
[151.22 --> 152.74]  Of course, you'd have to have that capability,
[152.92 --> 155.08]  but if you had that capability, problem solved.
[155.66 --> 157.00]  And see, that's where I start thinking,
[157.00 --> 159.64]  something that lets you roll back,
[159.84 --> 162.86]  combined with a system that checks the build before it deploys,
[163.52 --> 166.18]  you could actually have a successful auto deployment system.
[166.44 --> 170.04]  And on my two kids' Nix OS, I have two Nix OS kid laptops.
[170.28 --> 170.74]  There it is.
[170.96 --> 173.88]  And on these two machines, I have auto updates turned on.
[174.44 --> 176.96]  And they probably auto update two or three times a week
[176.96 --> 178.18]  because they're just using the computer,
[178.32 --> 180.06]  and the next time they boot the machine,
[180.16 --> 181.58]  it just boots into that new image.
[182.02 --> 183.00]  It doesn't even impact them.
[183.00 --> 186.24]  They're literally sitting there playing Minecraft or whatever they're playing,
[186.68 --> 189.34]  and the system's building a new version and checking it in the background
[189.34 --> 190.34]  and then deploying it.
[190.66 --> 192.24]  And then when they reboot, they go into that new image.
[192.28 --> 193.10]  And if it doesn't work,
[193.62 --> 195.92]  they just hit the down arrow at the boot menu
[195.92 --> 197.20]  and select the previous image.
[197.28 --> 197.60]  Absolutely.
[198.10 --> 200.04]  I was wondering how long it would take you to work Nix in there.
[200.44 --> 201.34]  Was that three minutes?
[201.52 --> 202.60]  Well, it really would help.
[203.02 --> 204.44]  I was thinking, should I say Ansible?
[204.58 --> 205.62]  But no, I was going to be honest.
[206.14 --> 206.88]  I was going to be honest.
[206.88 --> 211.18]  And I think this is also an example of maybe Windows isn't really up to this task.
[211.80 --> 213.36]  And this is something Microsoft could take on.
[213.44 --> 214.78]  This isn't necessarily their fault,
[215.32 --> 217.50]  although the brittleness of Windows, you could argue, is their fault.
[217.88 --> 219.80]  But how it handles these crash scenarios,
[220.46 --> 222.76]  it's acceptable for how we did things in 1997.
[223.60 --> 225.82]  But it's not acceptable how we do things in 2024.
[226.38 --> 227.76]  And with the mass deployment they have,
[227.86 --> 230.24]  even at 1% of Windows systems being taken out,
[230.30 --> 232.68]  it still is a massive impact around the world.
[232.78 --> 235.26]  It was breaking national news here in the States.
[235.26 --> 238.70]  They broke into everyday programming to go on the air
[238.70 --> 241.10]  about Windows Blue screening all over the world.
[242.18 --> 245.54]  Yeah, Windows 95 reveal, eat your heart out on this one, I think.
[247.06 --> 250.34]  Also, another maybe tip to the people out there
[250.34 --> 252.60]  is if they just had their computers off overnight,
[253.06 --> 254.40]  it wouldn't have received this auto-update
[254.40 --> 257.26]  because I think by something like 4 or 5 in the morning,
[258.42 --> 260.46]  they'd realized something had gone wrong.
[261.28 --> 263.34]  So if you say you came in at 8 a.m.
[263.34 --> 265.58]  and you turned your machine on at that point,
[266.00 --> 267.06]  you didn't have this problem.
[267.64 --> 269.30]  It's only the machines that were left on overnight,
[269.40 --> 271.28]  so mostly servers are always on displays
[271.28 --> 273.12]  or workstations that get kept on.
[273.84 --> 275.60]  It's all the folks that had to climb ladders
[275.60 --> 278.12]  to get to POS systems or displays
[278.12 --> 279.80]  that were 90 feet up in the air
[279.80 --> 281.78]  that I really felt for.
[282.36 --> 283.00]  No kidding.
[283.40 --> 285.16]  Or all the folks that had to work through the weekend.
[285.78 --> 286.78]  Yeah, yeah, yeah.
[286.86 --> 289.06]  I mean, that was another thing with this whole thing, right,
[289.10 --> 290.60]  is it was pushed on a Friday.
[290.60 --> 293.40]  And I was on the road at the time.
[293.58 --> 296.16]  And it's very rare,
[296.24 --> 297.92]  but it does happen that when I'm on a trip,
[298.66 --> 299.66]  big news breaks.
[299.96 --> 301.38]  And this is one of those events
[301.38 --> 304.84]  where I'm driving for five hours minimum maybe,
[305.32 --> 306.54]  maybe a little bit more,
[307.08 --> 309.92]  and I stop every now and then for a break,
[310.06 --> 311.68]  mostly so that way the wife can take a break.
[312.14 --> 313.24]  Maybe I have signal.
[313.50 --> 314.28]  Maybe I don't.
[314.38 --> 315.36]  Often I don't.
[315.48 --> 316.82]  And so when I did,
[316.90 --> 318.02]  and I got my phone open,
[318.02 --> 320.18]  and then I looked at it and I saw what was going on,
[320.48 --> 322.20]  I couldn't really process it at first.
[322.26 --> 323.94]  I'm like, what is happening?
[324.38 --> 326.14]  And I had to actually go over to Weapon X
[326.14 --> 327.10]  to put it all together
[327.10 --> 329.36]  to get like on the ground reports
[329.36 --> 330.86]  of people that were like kvetching
[330.86 --> 332.84]  about their systems being crashed
[332.84 --> 335.12]  to really kind of understand the magnitude of it.
[335.18 --> 336.78]  It was really, really something.
[336.92 --> 338.42]  And then I turned on the old TV
[338.42 --> 340.44]  to see if the news had it.
[340.50 --> 341.02]  And sure enough,
[341.08 --> 343.20]  they were doing like an emergency broadcast.
[343.76 --> 344.92]  It was quite the thing.
[344.92 --> 347.44]  And when you're offline
[347.44 --> 348.76]  and you come back
[348.76 --> 349.76]  and you see something like that,
[349.78 --> 349.96]  you're like,
[350.02 --> 351.72]  what the hell is going on out there?
[352.40 --> 354.44]  So how did 90 Jeep survive the heat wave?
[354.98 --> 356.64]  Oh man, I'm such a dummy, Alex.
[357.38 --> 359.08]  I drove her right into the heat,
[359.22 --> 360.40]  right into the heat.
[360.62 --> 361.60]  And it was hot.
[361.70 --> 363.10]  You know, we had days well above 100.
[364.10 --> 365.88]  But I kind of have the system down now.
[365.88 --> 369.90]  I really desperately need to install permanent cooling
[369.90 --> 373.74]  for my solar lithium inverter system.
[374.42 --> 375.84]  Because when you're really inverting,
[375.92 --> 378.24]  like say 2,800 watts to run AC,
[379.14 --> 380.58]  it just generates so much heat
[380.58 --> 382.20]  to discharge and invert that.
[382.36 --> 383.52]  Or if you're bringing in a lot of solar,
[383.58 --> 385.26]  if you're bringing in like 2,000 watts of solar,
[385.44 --> 388.04]  that actually generates a lot of heat in the system.
[388.50 --> 390.68]  And so I can't really run high loads
[390.68 --> 391.42]  while I'm driving.
[392.10 --> 393.40]  And I've got to figure out a way
[393.40 --> 394.42]  to bring in cool air
[394.42 --> 395.66]  and shoot out the hot air
[395.66 --> 397.38]  because that's a serious problem.
[397.38 --> 400.90]  And then also where all of my server gear is
[400.90 --> 402.42]  got really hot again,
[402.46 --> 405.52]  over 100 degrees in that little booth.
[406.38 --> 407.90]  And everything kept running,
[408.12 --> 410.02]  but I don't like running it
[410.02 --> 411.58]  at above 100 degree temperatures.
[411.74 --> 413.54]  So I've really got to wrap my head around
[413.54 --> 414.72]  how I'm going to solve these problems
[414.72 --> 415.30]  in the future.
[415.80 --> 417.14]  Everything held together though.
[417.62 --> 418.90]  So thankfully that bit worked.
[419.46 --> 421.40]  What I have slipped on,
[421.76 --> 423.18]  and I didn't realize it
[423.18 --> 424.28]  because I've had Starlink,
[424.36 --> 426.12]  so I've had connectivity in more locations
[426.12 --> 427.14]  than I ever have before,
[427.38 --> 429.32]  but I have slipped
[429.32 --> 431.68]  on my everything works offline mandate
[431.68 --> 432.76]  that I set up years ago.
[433.36 --> 434.38]  It's an interesting side effect
[434.38 --> 435.96]  of having internet everywhere with Starlink
[435.96 --> 436.96]  that you wouldn't consider.
[437.62 --> 438.56]  Yeah, and it wasn't until
[438.56 --> 439.68]  I'm going through the passes
[439.68 --> 441.60]  and we're covered in trees or whatnot
[441.60 --> 443.24]  and there's just no Starlink available.
[443.32 --> 444.64]  I can't get a clear shot to the sky.
[444.74 --> 446.08]  We don't have any cell signal at all.
[446.48 --> 447.72]  And we did this for a few days.
[447.84 --> 449.28]  It wasn't until then that I realized
[449.28 --> 451.34]  I've built a lot of things
[451.34 --> 454.12]  using a public DNS
[454.12 --> 456.88]  that points at tail net IPs.
[457.94 --> 460.52]  And so I could,
[460.84 --> 463.04]  everything is technically online,
[463.46 --> 465.78]  but I simply cannot resolve
[465.78 --> 467.24]  that public DNS
[467.24 --> 469.40]  that just points to an internal system.
[469.80 --> 470.80]  And that's when I realized
[470.80 --> 471.76]  I'd really screwed up
[471.76 --> 473.42]  because I'd set up Jellyfin that way.
[473.50 --> 475.48]  I'd set up Ersatz TV that way.
[475.60 --> 476.22]  Oh, yeah.
[476.34 --> 477.52]  Yeah, and so those things,
[477.58 --> 478.78]  like I went to sit down and watch TV
[478.78 --> 479.08]  and I'm like,
[479.12 --> 480.26]  oh, this is going to work great.
[480.88 --> 481.74]  Dad fail moment.
[481.74 --> 483.00]  I'm like, let's watch some TV.
[483.10 --> 483.52]  And the kids are like,
[483.58 --> 485.08]  but dad, we can't watch TV.
[485.16 --> 486.06]  We don't have any internet.
[486.44 --> 487.78]  Honest to God conversation.
[488.08 --> 488.82]  And I said,
[489.10 --> 490.48]  oh, don't worry, son.
[491.66 --> 493.18]  I've got everything offline.
[493.48 --> 493.86]  Watch.
[493.90 --> 494.62]  And I hit the button
[494.62 --> 496.02]  and nothing happens
[496.02 --> 499.88]  because Jellyfin was using a public DNS.
[499.88 --> 502.12]  And I guess that tells me
[502.12 --> 504.76]  I need to set up resolution
[504.76 --> 505.70]  for that domain
[505.70 --> 507.54]  on my internal pie hole or something.
[508.16 --> 509.32]  Yeah, some kind of local
[509.32 --> 511.06]  authoritative entry would do the trick.
[511.06 --> 513.70]  Yeah, but I think my primary DNS server
[513.70 --> 515.30]  is also on the tail net,
[515.40 --> 516.12]  which is on Linode.
[516.68 --> 518.22]  So I got to rethink that too
[518.22 --> 519.64]  and maybe move that back to the RV.
[520.44 --> 521.26]  Easy done though.
[521.42 --> 522.94]  I mean, use a bit of split DNS magic
[522.94 --> 523.92]  and you're off to the races.
[524.40 --> 525.34]  Yeah, I wanted to play around.
[525.46 --> 526.24]  I wanted to hear actually
[526.24 --> 527.16]  what the audience suggested.
[527.28 --> 528.04]  I was going to say boost in
[528.04 --> 529.08]  and tell me what you would use
[529.08 --> 529.70]  for this setup.
[530.16 --> 531.70]  I just need a fast local DNS.
[531.80 --> 532.56]  I've been using pie hole,
[532.62 --> 533.50]  pretty happy with it.
[533.92 --> 536.00]  But I'd be open to restructuring this
[536.00 --> 537.06]  to make this work better.
[537.88 --> 538.84]  And then I think also
[538.84 --> 540.06]  the other idea I'd love to hear
[540.06 --> 541.66]  from maybe you and also the audiences.
[543.34 --> 544.48]  Is there a simple
[544.48 --> 546.62]  offline messaging system we could use?
[546.94 --> 547.96]  I want something simple.
[548.02 --> 548.92]  It's not like a huge deal,
[549.04 --> 550.32]  but when you're totally offline,
[550.78 --> 552.96]  it's nice to be able to send messages
[552.96 --> 553.90]  to each other still,
[553.98 --> 554.92]  just as like reminders.
[555.70 --> 556.72]  This is something I guess maybe,
[556.80 --> 557.78]  I don't know if your family does this,
[557.84 --> 558.70]  but we'll set,
[558.76 --> 559.62]  we have like a thread
[559.62 --> 561.26]  set aside in Telegram
[561.26 --> 562.72]  and we'll pop in there
[562.72 --> 563.16]  and be like,
[563.60 --> 563.86]  oh yeah,
[563.86 --> 564.56]  we need to remember
[564.56 --> 567.04]  to call the suspension shop
[567.04 --> 567.94]  and book an appointment
[567.94 --> 568.94]  in September.
[569.70 --> 570.90]  And we'll just put that in there
[570.90 --> 572.10]  so that way when we're both,
[572.20 --> 573.32]  when we get back to civilization
[573.32 --> 574.58]  and we're not on our trip anymore,
[574.68 --> 575.36]  we'll look at that thread
[575.36 --> 575.54]  and go,
[575.58 --> 575.80]  oh yeah,
[575.82 --> 576.62]  we need to do these things.
[577.30 --> 578.72]  And so we built a routine around that.
[579.12 --> 580.22]  But when you're totally offline,
[580.32 --> 581.52]  you don't have any of that stuff.
[581.60 --> 582.72]  There's no way to send messages
[582.72 --> 583.76]  to each other when you're offline,
[583.90 --> 584.46]  even if you're all
[584.46 --> 585.54]  on the same Wi-Fi network.
[586.04 --> 587.44]  There's this revolutionary thing.
[587.58 --> 588.28]  You're going to love it.
[588.28 --> 591.20]  It's made from trees
[591.20 --> 593.38]  and they bind it together
[593.38 --> 595.32]  with glue along what's called,
[595.38 --> 595.62]  I think,
[595.64 --> 596.16]  a spine.
[596.62 --> 598.20]  And it has lots of pages.
[598.88 --> 598.90]  Man,
[598.92 --> 600.32]  this sounds like some caveman stuff.
[600.64 --> 601.88]  You can just write
[601.88 --> 603.78]  on this thing called paper
[603.78 --> 604.90]  and make a list.
[605.06 --> 606.08]  Now you sound like my wife.
[606.16 --> 606.32]  She's like,
[606.36 --> 606.58]  well look,
[606.64 --> 609.02]  I'll make a whiteboard right here
[609.02 --> 610.16]  and we'll just write it all down.
[610.30 --> 610.68]  And I'm like,
[610.86 --> 611.16]  yeah,
[611.18 --> 611.90]  that's fine.
[612.28 --> 612.68]  But like,
[612.72 --> 613.86]  I'm out working on something
[613.86 --> 616.10]  and something crosses my mind.
[616.38 --> 617.64]  I want to be able to just
[617.64 --> 619.08]  bark it into my phone real quick
[619.08 --> 619.90]  and send it off.
[620.16 --> 620.46]  You know,
[620.58 --> 620.82]  it's,
[621.06 --> 622.02]  I don't know.
[622.56 --> 623.92]  There's a few things like that.
[624.04 --> 625.92]  A couple of like my URL bookmarks too
[625.92 --> 627.06]  are all using public DNS
[627.06 --> 627.60]  or something.
[628.12 --> 629.50]  So a few things broke,
[629.62 --> 631.10]  but it wasn't,
[631.10 --> 631.74]  it wasn't anything
[631.74 --> 632.46]  I couldn't work around.
[632.56 --> 634.24]  Like I reconfigured Jellyfin
[634.24 --> 635.62]  to use the internal IPs
[635.62 --> 636.48]  and that just worked fine
[636.48 --> 637.36]  and all that kind of stuff.
[637.46 --> 637.58]  But,
[638.32 --> 639.00]  you know,
[639.00 --> 640.18]  I thought I was still building
[640.18 --> 641.74]  this system to work fully offline
[641.74 --> 642.94]  because all of the resources
[642.94 --> 644.14]  are on the same land.
[644.84 --> 646.56]  But it really shows me that,
[646.56 --> 647.56]  and I remember this
[647.56 --> 648.18]  from the first time
[648.18 --> 648.96]  I built this
[648.96 --> 650.90]  and documented this on the show,
[651.62 --> 652.22]  I've really,
[652.32 --> 653.70]  I've got to go somewhere
[653.70 --> 654.68]  that has no internet
[654.68 --> 655.90]  and actually test it.
[656.00 --> 657.32]  You actually have to test it
[657.32 --> 658.90]  because you can build something
[658.90 --> 659.42]  in a network
[659.42 --> 660.22]  and a whole system
[660.22 --> 661.72]  to try to work
[661.72 --> 663.06]  as if it's your own
[663.06 --> 664.26]  internal intranet
[664.26 --> 666.00]  with no external connection
[666.00 --> 667.08]  and everything continues on.
[667.18 --> 668.54]  But until you actually test it
[668.54 --> 669.90]  and disconnect the internet,
[670.38 --> 671.68]  you'll be surprised
[671.68 --> 672.52]  how many little things
[672.52 --> 673.14]  still leak out
[673.14 --> 674.00]  and still connect out
[674.00 --> 674.76]  to the bigger,
[674.92 --> 675.34]  wider world.
[675.34 --> 676.38]  It is amazing,
[676.48 --> 677.28]  even in this house,
[677.40 --> 677.86]  which is,
[677.98 --> 678.20]  you know,
[678.48 --> 679.40]  it's not mobile,
[679.56 --> 679.96]  of course.
[680.84 --> 682.34]  When the internet goes out,
[682.48 --> 683.98]  the number of little things
[683.98 --> 685.16]  that don't work,
[685.28 --> 686.02]  and most of my,
[686.14 --> 687.72]  I've got a pie hole locally
[687.72 --> 689.48]  that is the authoritative DNS server,
[689.60 --> 690.34]  which uses Cloudflare
[690.88 --> 691.84]  as the upstream DNS.
[692.66 --> 694.84]  I have DHCP local,
[695.00 --> 695.46]  of course.
[695.80 --> 697.50]  Most of the critical devices
[697.50 --> 698.74]  are statically IP'd.
[699.06 --> 700.34]  But if the firewall goes out
[700.34 --> 701.16]  or the internet
[701.16 --> 702.42]  in particular goes out,
[702.42 --> 704.32]  there's just a bunch
[704.32 --> 705.40]  of small things
[705.40 --> 706.44]  that don't work anymore.
[706.58 --> 707.00]  And I'm like,
[707.82 --> 708.26]  oh,
[708.74 --> 708.96]  well,
[709.02 --> 710.46]  that's sad,
[710.70 --> 711.16]  isn't it?
[711.92 --> 712.82]  One of the most annoying
[712.82 --> 714.90]  was my NVIDIA Shield
[714.90 --> 716.52]  would not connect
[716.52 --> 717.54]  to the Wi-Fi network
[717.54 --> 718.48]  at first
[718.48 --> 719.82]  just because it couldn't
[719.82 --> 720.18]  ping out
[720.18 --> 721.20]  to the broader internet.
[722.10 --> 722.52]  And again,
[722.62 --> 722.74]  like,
[722.78 --> 723.88]  everything's on my LAN.
[724.06 --> 724.94]  I don't need
[724.94 --> 726.74]  a routable internet connection
[726.74 --> 727.80]  for you to stream something
[727.80 --> 728.52]  from Jellyfin.
[729.48 --> 731.40]  And I've had several devices
[731.40 --> 732.18]  that do this.
[733.10 --> 734.22]  Maybe it was the Chromecast,
[734.36 --> 735.20]  but another device
[735.20 --> 736.78]  that just won't join the Wi-Fi.
[737.36 --> 738.72]  And like all the Google Home
[738.72 --> 740.32]  little screeny devices,
[740.50 --> 740.66]  you know,
[741.22 --> 741.76]  none of them,
[741.82 --> 742.00]  of course,
[742.04 --> 742.76]  I suppose they don't work anyways,
[742.80 --> 743.68]  but they just won't,
[743.68 --> 744.56]  they won't even talk
[744.56 --> 745.50]  to that Wi-Fi network.
[746.44 --> 747.24]  And to me,
[747.34 --> 747.76]  it made me,
[747.82 --> 748.46]  and I bet you
[748.46 --> 749.14]  there's a way to do this.
[749.16 --> 750.16]  I just haven't given it much thought,
[750.24 --> 751.68]  but I would like
[751.68 --> 753.26]  to fake this out somehow.
[753.58 --> 754.84]  I would like to have
[754.84 --> 755.52]  whatever they're doing,
[755.64 --> 756.36]  pinging or whatever,
[756.48 --> 757.82]  they're doing an HTTP request,
[757.82 --> 759.26]  I would like to fake it out
[759.26 --> 760.58]  and make it think
[760.58 --> 761.16]  it has internet.
[761.78 --> 762.66]  There's got to be a way
[762.66 --> 763.30]  to do that
[763.30 --> 764.28]  because these devices
[764.28 --> 765.84]  are a pain in my butt
[765.84 --> 766.70]  and I don't want to have
[766.70 --> 767.14]  to go into, say,
[767.20 --> 768.00]  like the Nvidia Shield
[768.00 --> 769.84]  and tell it to,
[769.94 --> 770.58]  no, actually,
[770.68 --> 771.50]  go connect to the Wi-Fi.
[771.60 --> 772.16]  Yes, actually,
[772.26 --> 772.78]  this Wi-Fi.
[772.98 --> 774.58]  Yes, I know it doesn't
[774.58 --> 774.96]  have internet.
[775.12 --> 775.94]  Please try again.
[776.36 --> 777.30]  And because each stage
[777.30 --> 778.06]  is like scanning
[778.06 --> 778.66]  and detecting,
[778.78 --> 780.08]  it takes you like five minutes.
[780.56 --> 780.76]  Right.
[781.08 --> 782.60]  And then, you know,
[782.66 --> 783.48]  then only discover
[783.48 --> 784.04]  another problem.
[784.18 --> 785.00]  So there's got to be a way
[785.00 --> 787.10]  to trick these appliances
[787.10 --> 788.44]  into thinking they have internet
[788.44 --> 789.84]  even when there isn't internet.
[790.32 --> 791.78]  These things get too clever
[791.78 --> 792.94]  for their own good sometimes.
[793.64 --> 794.60]  Our robot, VAC,
[794.70 --> 796.22]  died whilst we were in England.
[797.12 --> 798.06]  And so we bought a new one
[798.06 --> 798.72]  on Prime Day
[798.72 --> 799.64]  and it arrived
[799.64 --> 800.48]  and I'm sat there
[800.48 --> 801.70]  with my iOS phone
[801.70 --> 802.90]  trying to get this thing
[802.90 --> 805.48]  to connect to the 2.4 gigahertz Wi-Fi
[805.48 --> 807.24]  because it only supports 2.4 gig.
[807.48 --> 807.92]  Go figure.
[808.76 --> 808.96]  Yeah.
[809.68 --> 810.52]  And it just doesn't work.
[810.56 --> 812.36]  And I spend maybe 20 minutes
[812.36 --> 813.08]  with iOS.
[813.08 --> 813.74]  I then think,
[813.82 --> 814.40]  right, screw this.
[814.50 --> 815.66]  I went and got my OnePlus 7
[815.66 --> 816.54]  that's been in a drawer,
[816.72 --> 817.72]  7T,
[817.82 --> 818.52]  OnePlus 7T
[818.52 --> 819.38]  that's been in a drawer
[819.38 --> 821.48]  since I last used it
[821.48 --> 822.38]  a couple of years ago.
[823.22 --> 824.40]  And sure enough,
[824.44 --> 825.52]  I installed the Robo Rock app
[825.52 --> 826.22]  and boom,
[826.30 --> 826.58]  Android,
[826.68 --> 827.16]  I was up and running
[827.16 --> 827.82]  in two minutes.
[828.04 --> 829.62]  It's like there was something
[829.62 --> 830.90]  going on on iOS
[830.90 --> 831.56]  that was just,
[832.06 --> 833.28]  when it wanted to change
[833.28 --> 834.16]  Wi-Fi networks
[834.16 --> 835.58]  and try and inject credentials,
[835.72 --> 836.00]  I'm like,
[836.80 --> 838.44]  whoever tested this
[838.44 --> 840.36]  did not anticipate
[840.36 --> 842.00]  whatever problem.
[842.00 --> 843.06]  I looked in,
[843.10 --> 843.26]  you know,
[843.32 --> 844.16]  my pihole logs,
[844.24 --> 845.30]  there was no ad blocking
[845.30 --> 846.56]  or anything causing an issue.
[846.68 --> 847.42]  It's just...
[847.42 --> 848.52]  Can I suggest an idea
[848.52 --> 850.06]  and I wonder if you know?
[850.38 --> 851.08]  I'd love to know.
[851.18 --> 852.50]  With my doorbell that I got,
[852.62 --> 853.46]  same problem,
[853.68 --> 854.82]  exact same problem,
[855.08 --> 856.10]  if my AP
[856.10 --> 857.94]  had a 2.4
[857.94 --> 859.08]  and a 5 gigahertz
[859.08 --> 860.34]  that had the same names.
[860.68 --> 861.70]  So I heard that segment
[861.70 --> 862.54]  and I tried that
[862.54 --> 863.40]  based on the advice
[863.40 --> 864.22]  of Mr. Fisher
[864.22 --> 864.96]  and unfortunately
[864.96 --> 866.12]  didn't do the trick.
[866.20 --> 866.36]  Okay.
[866.78 --> 867.40]  I'm wondering though,
[867.44 --> 867.98]  does your OnePlus
[867.98 --> 869.46]  maybe only do 2.4?
[869.80 --> 870.04]  No,
[870.08 --> 870.70]  I don't think so.
[870.70 --> 871.90]  I think that's a 5 as well.
[871.98 --> 872.14]  Okay.
[872.86 --> 873.06]  Yeah,
[873.12 --> 874.42]  I've also though
[874.42 --> 875.74]  experienced situations
[875.74 --> 877.50]  where I start
[877.50 --> 879.18]  to pair some Wi-Fi device
[879.18 --> 879.72]  with iOS
[879.72 --> 880.68]  and have to bail
[880.68 --> 881.62]  and go get the Pixel
[881.62 --> 882.48]  and you know,
[882.52 --> 883.08]  the other thing
[883.08 --> 883.88]  I've also noticed,
[884.02 --> 884.20]  Alex,
[884.30 --> 885.72]  is more and more,
[885.86 --> 887.18]  which is great,
[887.34 --> 887.88]  I guess,
[887.98 --> 888.80]  for HomeKit users,
[888.92 --> 889.86]  but more and more,
[890.84 --> 891.20]  iOS,
[891.44 --> 892.20]  when you get
[892.20 --> 893.68]  that device on the Wi-Fi,
[893.78 --> 894.78]  it immediately starts
[894.78 --> 895.88]  enrolling it in HomeKit
[895.88 --> 896.96]  and associates with it.
[896.96 --> 897.72]  And once you associate
[897.72 --> 898.20]  with HomeKit,
[898.20 --> 899.98]  it's like SIM card lock.
[900.32 --> 901.68]  You're locked to HomeKit now.
[902.24 --> 904.62]  And it just starts that process
[904.62 --> 906.38]  the moment the iOS app
[906.38 --> 907.56]  gets the thing on Wi-Fi.
[908.06 --> 909.58]  And then it can be very hard
[909.58 --> 910.44]  to get it to work
[910.44 --> 911.16]  with Home Assistant
[911.16 --> 912.08]  unless you use
[912.08 --> 913.46]  HomeKit integration
[913.46 --> 914.16]  on Home Assistant,
[914.72 --> 915.28]  which I'd prefer
[915.28 --> 916.54]  to just have direct communication
[916.54 --> 917.22]  with the device.
[917.64 --> 918.40]  And so I often
[918.40 --> 919.04]  will go the route
[919.04 --> 920.72]  of now just using Android anyway,
[920.86 --> 922.14]  so I may have optionality
[922.14 --> 922.72]  down the road
[922.72 --> 923.64]  to use Home Assistant.
[924.26 --> 924.76]  You just kind of have
[924.76 --> 925.32]  to roll the dice.
[925.32 --> 927.12]  Now, speaking of Prime Day,
[927.22 --> 927.92]  I picked up a couple
[927.92 --> 930.02]  of 4TB NVMe SSDs.
[930.08 --> 931.58]  They were on a rather good offer
[931.58 --> 933.46]  of about $250 each.
[934.22 --> 935.66]  Typically, they're well over $300,
[935.80 --> 936.82]  so I was quite pleased with that.
[937.12 --> 938.20]  And I went to install it
[938.20 --> 939.88]  into my Epic build
[939.88 --> 941.82]  that I did in March,
[941.94 --> 942.76]  April sort of time.
[943.14 --> 944.06]  Talked about it on the show.
[944.62 --> 945.44]  Made a YouTube video
[945.44 --> 946.10]  about it, of course.
[946.70 --> 947.50]  And I noticed
[947.50 --> 948.28]  that the inside
[948.28 --> 949.48]  of the Sligar case
[949.48 --> 951.74]  wasn't full,
[951.74 --> 953.08]  but there were more
[953.08 --> 955.14]  fruit fly little carcasses
[955.14 --> 956.06]  in that case
[956.06 --> 957.30]  than I was comfortable with.
[957.68 --> 958.34]  Oh, they must have found
[958.34 --> 959.40]  a nice little cozy spot
[959.40 --> 959.96]  to hang out.
[960.54 --> 961.46]  Yeah, yeah.
[961.54 --> 961.98]  I mean, we're talking
[961.98 --> 962.66]  about the tiny,
[962.78 --> 963.76]  tiny little black,
[964.06 --> 965.76]  like, gnat-sized flies.
[965.90 --> 966.66]  I don't know if they're
[966.66 --> 967.48]  fruit flies or whatever,
[967.52 --> 968.00]  but the tiny,
[968.12 --> 968.64]  tiny little ones.
[968.66 --> 969.30]  You know the ones, right?
[969.54 --> 970.12]  Yeah, I do.
[971.30 --> 972.50]  So this Sligar case,
[972.58 --> 973.74]  the CX4712
[974.44 --> 975.54]  is the one that I have,
[976.08 --> 977.14]  doesn't come with
[977.14 --> 978.20]  a dust filter
[978.20 --> 979.06]  on the front of it.
[979.14 --> 980.22]  So I looked around
[980.22 --> 980.66]  on the internet
[980.66 --> 981.42]  for some solutions
[981.42 --> 982.52]  and apparently Sligar
[982.52 --> 983.58]  make one that they
[983.58 --> 984.74]  should ship with the case
[984.74 --> 986.00]  sometimes or if you contact it.
[986.32 --> 986.96]  I couldn't be bothered
[986.96 --> 987.48]  with all that.
[987.84 --> 988.38]  I went on Amazon
[988.38 --> 990.58]  and got a $12 kit
[990.58 --> 991.52]  of magnetic,
[992.26 --> 993.02]  what do you call this,
[993.14 --> 994.22]  filter material,
[994.36 --> 995.62]  like metallic filter material.
[996.10 --> 996.96]  Oh, yeah, like a mesh.
[997.04 --> 998.10]  Yeah, and then I just,
[998.20 --> 998.42]  you know,
[998.44 --> 999.10]  used a pair of scissors
[999.10 --> 999.78]  to cut it
[999.78 --> 1000.98]  and Bob's your uncle.
[1001.10 --> 1002.06]  It took me about 10 minutes
[1002.06 --> 1002.86]  and cost me $12
[1002.86 --> 1004.22]  and I now have a filter
[1004.22 --> 1004.76]  on the case.
[1004.94 --> 1006.14]  A custom filter
[1006.14 --> 1007.50]  that just matches.
[1007.68 --> 1008.02]  That's great.
[1008.10 --> 1008.28]  You know,
[1008.36 --> 1009.08]  this looks like something
[1009.08 --> 1009.52]  I could use
[1009.52 --> 1010.30]  if I ever do make
[1010.30 --> 1010.98]  my own ventilation
[1010.98 --> 1012.10]  from my battery bay.
[1012.60 --> 1013.26]  I should put something
[1013.26 --> 1013.98]  like this on there
[1013.98 --> 1014.68]  and it's magnetic.
[1014.94 --> 1015.92]  So does it come with a frame?
[1016.18 --> 1016.96]  Is that part magnetic?
[1017.54 --> 1019.06]  So it comes with a piece
[1019.06 --> 1020.52]  of sort of mesh fabric,
[1020.66 --> 1021.56]  metal mesh fabric
[1021.56 --> 1022.74]  coated in that kind
[1022.74 --> 1023.62]  of like plastic.
[1024.62 --> 1025.80]  If you touched it,
[1025.86 --> 1027.26]  you felt this texture
[1027.26 --> 1027.98]  a million times
[1027.98 --> 1028.74]  before in your life
[1028.74 --> 1029.78]  and then it just comes
[1029.78 --> 1031.64]  with some pre-adhesive
[1031.64 --> 1033.24]  backed strips
[1033.24 --> 1035.56]  of magnetic tape,
[1035.84 --> 1036.30]  I suppose.
[1036.96 --> 1037.70]  You just cut them
[1037.70 --> 1038.16]  to length
[1038.16 --> 1039.34]  and use the adhesive
[1039.34 --> 1040.00]  on the mesh
[1040.00 --> 1041.38]  and it just magnetizes
[1041.38 --> 1042.66]  itself to the steel
[1042.66 --> 1043.18]  of the case.
[1043.82 --> 1044.60]  That's a nice little tip.
[1044.84 --> 1045.38]  Put a link to that
[1045.38 --> 1045.88]  in the show notes.
[1046.00 --> 1046.42]  Now, Alex,
[1046.46 --> 1047.16]  you had a chance
[1047.16 --> 1048.32]  to sit down
[1048.32 --> 1049.62]  with a developer
[1049.62 --> 1050.70]  of ESP Home.
[1051.14 --> 1051.36]  Yeah,
[1051.38 --> 1052.14]  we got in a little bit
[1052.14 --> 1052.70]  of hot water
[1052.70 --> 1053.70]  after the last episode
[1053.70 --> 1054.88]  by suggesting
[1054.88 --> 1056.20]  that people don't update
[1056.20 --> 1057.64]  their ESP Home devices.
[1057.64 --> 1058.64]  So I thought
[1058.64 --> 1059.78]  I'd set the record straight
[1059.78 --> 1060.52]  and reached out
[1060.52 --> 1061.54]  to Frank over
[1061.54 --> 1062.44]  at the Home Assistant Project
[1062.44 --> 1063.28]  who put me in touch
[1063.28 --> 1063.80]  with Keith
[1063.80 --> 1065.60]  who works on ESP Home
[1065.60 --> 1066.50]  every single day.
[1066.88 --> 1067.46]  After the break,
[1067.50 --> 1068.06]  you can join us
[1068.06 --> 1068.86]  for an interview
[1068.86 --> 1069.56]  with Keith.
[1070.98 --> 1072.02]  Unraid.net
[1072.02 --> 1073.36]  slash self-hosted.
[1073.60 --> 1074.82]  Unleash your hardware
[1074.82 --> 1076.12]  and Unraid 7's
[1076.12 --> 1076.78]  public beta
[1076.78 --> 1078.42]  is out now
[1078.42 --> 1079.26]  and it is
[1079.26 --> 1080.10]  packed
[1080.10 --> 1080.94]  with game-changing
[1080.94 --> 1081.58]  new features
[1081.58 --> 1082.12]  and improvements
[1082.12 --> 1083.30]  that will redefine
[1083.30 --> 1084.54]  what you can achieve
[1084.54 --> 1085.58]  in your home lab.
[1086.10 --> 1086.52]  I mean, really,
[1086.60 --> 1087.18]  this beta release
[1087.18 --> 1088.54]  has something for everyone
[1088.54 --> 1089.46]  from a sleek,
[1089.64 --> 1090.86]  revamped new dashboard,
[1091.06 --> 1091.88]  improved navigation
[1091.88 --> 1093.06]  and monitoring stats
[1093.06 --> 1094.42]  to full hybrid
[1094.42 --> 1095.66]  ZFS sub-pools
[1095.66 --> 1096.22]  implemented,
[1096.82 --> 1097.82]  huge VM manager
[1097.82 --> 1098.26]  improvements
[1098.26 --> 1099.24]  and a lot more.
[1099.86 --> 1101.36]  Unraid 7 really rounds out
[1101.36 --> 1102.74]  ZFS's full capabilities
[1102.74 --> 1103.78]  with full integration
[1103.78 --> 1105.66]  of those hybrid ZFS pools
[1105.66 --> 1106.94]  that support a wide range
[1106.94 --> 1108.08]  of special VDEV types
[1108.08 --> 1109.16]  and with this beta
[1109.16 --> 1109.90]  you can now skip
[1109.90 --> 1110.70]  using the traditional
[1110.70 --> 1111.34]  Unraid array
[1111.34 --> 1112.24]  all together
[1112.24 --> 1114.70]  and run your own storage
[1114.70 --> 1115.78]  as pools
[1115.78 --> 1117.44]  with many new
[1117.44 --> 1118.60]  all-SSD platforms too.
[1118.72 --> 1118.82]  Like,
[1119.42 --> 1120.30]  the way you could make
[1120.30 --> 1120.86]  that work now
[1120.86 --> 1121.78]  with no limitations
[1121.78 --> 1123.80]  is mind-bending fast.
[1124.00 --> 1124.44]  So what are you
[1124.44 --> 1124.94]  going to build?
[1125.52 --> 1126.50]  Unraid is a powerful
[1126.50 --> 1127.88]  easy-to-use operating system
[1127.88 --> 1128.66]  for the self-hoster
[1128.66 --> 1129.20]  out there
[1129.20 --> 1130.76]  that has some disk
[1130.76 --> 1131.68]  and wants a network
[1131.68 --> 1132.28]  attached storage.
[1132.42 --> 1133.46]  You can run some applications.
[1134.12 --> 1134.76]  You can make it into
[1134.76 --> 1136.14]  anything you might dream of.
[1136.42 --> 1137.94]  It can be your VM machine
[1137.94 --> 1138.40]  if you like.
[1138.46 --> 1139.28]  So go make the most
[1139.28 --> 1140.08]  out of your hardware
[1140.08 --> 1141.44]  no matter what you have
[1141.44 --> 1141.90]  on hand.
[1142.34 --> 1143.22]  Different size drives
[1143.22 --> 1143.84]  and manufacturers
[1143.84 --> 1145.10]  is no problem at all.
[1145.20 --> 1146.22]  Unraid works with it all.
[1146.60 --> 1147.38]  So go check it out
[1147.38 --> 1148.10]  and support the show.
[1148.20 --> 1148.68]  You know, Unraid,
[1148.68 --> 1150.72]  it's built to last too.
[1151.14 --> 1151.82]  It's been around
[1151.82 --> 1153.00]  in one form or another
[1153.00 --> 1154.36]  since the early 2000s
[1154.36 --> 1155.34]  and it just keeps going
[1155.34 --> 1156.54]  from strength to strength.
[1157.14 --> 1157.74]  And the new
[1157.74 --> 1158.90]  Unraid 7 beta
[1158.90 --> 1160.36]  is amazing.
[1160.96 --> 1161.40]  Check it out
[1161.40 --> 1162.56]  at unraid.net
[1162.56 --> 1163.52]  slash self-hosted.
[1163.58 --> 1163.70]  Yeah,
[1163.86 --> 1164.66]  the Unraid
[1164.66 --> 1165.66]  and the new
[1165.66 --> 1166.82]  7 beta is out.
[1166.96 --> 1167.82]  Unraid.net
[1167.82 --> 1168.44]  slash
[1168.44 --> 1169.60]  self-hosted.
[1170.90 --> 1171.54]  All right,
[1171.58 --> 1173.14]  so in last week's episode,
[1173.32 --> 1173.76]  Chris and I
[1173.76 --> 1174.52]  talked a little bit
[1174.52 --> 1175.88]  about ESP Home
[1175.88 --> 1177.00]  and updates
[1177.00 --> 1178.38]  and things like that.
[1178.86 --> 1179.32]  And joining us
[1179.32 --> 1179.96]  on the show today
[1179.96 --> 1181.18]  is Just Keith
[1181.18 --> 1182.36]  from Nabu Casa.
[1182.68 --> 1183.50]  Hi, Just Keith.
[1183.60 --> 1184.04]  How are you?
[1184.42 --> 1185.36]  I am Just Keith.
[1185.92 --> 1187.24]  Yes, I am quite,
[1187.38 --> 1187.80]  quite good.
[1187.92 --> 1188.32]  Quite good.
[1188.40 --> 1189.06]  Thanks for having me.
[1189.66 --> 1190.30]  And what is it
[1190.30 --> 1191.62]  you do at Nabu Casa?
[1192.16 --> 1193.58]  So Nabu Casa,
[1193.80 --> 1195.00]  I've been there
[1195.00 --> 1196.04]  a little over a year now
[1196.04 --> 1197.40]  and I'm working on
[1197.40 --> 1198.12]  both hardware
[1198.12 --> 1198.66]  and software,
[1199.14 --> 1200.36]  primarily developing
[1200.36 --> 1201.26]  on ESP Home
[1201.26 --> 1202.20]  at the moment.
[1202.66 --> 1203.44]  I'm working with
[1203.44 --> 1204.30]  Jesse Hills
[1204.30 --> 1205.46]  who is in New Zealand
[1205.46 --> 1207.04]  and he is
[1207.04 --> 1208.20]  the kind of
[1208.20 --> 1209.14]  ESP Home lead,
[1209.36 --> 1210.10]  a project lead
[1210.10 --> 1210.78]  at this point.
[1211.32 --> 1213.00]  But I help him out
[1213.00 --> 1214.18]  as much as I'm able
[1214.18 --> 1215.40]  and also tinker
[1215.40 --> 1216.20]  in some other things,
[1216.24 --> 1216.64]  like I said,
[1216.70 --> 1217.80]  in some hardware stuff
[1217.80 --> 1219.58]  and testing things
[1219.58 --> 1220.22]  and everything
[1220.22 --> 1222.46]  from reviewing PRs
[1222.46 --> 1223.56]  to making sure
[1223.56 --> 1224.38]  stuff works
[1224.38 --> 1225.50]  to occasionally
[1225.50 --> 1226.42]  updating websites
[1226.42 --> 1227.14]  and documentation.
[1227.66 --> 1228.20]  So I'm kind of
[1228.20 --> 1228.88]  all over the board.
[1229.56 --> 1230.30]  So you'd be a good man
[1230.30 --> 1231.12]  to ask about
[1231.12 --> 1232.06]  update cadences
[1232.06 --> 1232.88]  for something like
[1232.88 --> 1233.82]  ESP Home then, huh?
[1233.96 --> 1234.82]  Yeah, we could talk
[1234.82 --> 1235.32]  about that.
[1235.80 --> 1236.34]  All right, well,
[1236.70 --> 1237.42]  for those people
[1237.42 --> 1238.44]  that aren't totally
[1238.44 --> 1239.60]  familiar with ESP Home,
[1239.64 --> 1240.44]  and we do talk about it
[1240.44 --> 1241.70]  a fair amount in the show,
[1241.88 --> 1243.40]  but let's just go back
[1243.40 --> 1244.30]  to ground zero
[1244.30 --> 1244.76]  for a minute.
[1244.96 --> 1245.74]  What is it?
[1246.22 --> 1247.52]  Oh, putting me
[1247.52 --> 1248.20]  on the spot.
[1248.80 --> 1249.50]  You know what?
[1249.74 --> 1250.76]  I'm kind of laughing
[1250.76 --> 1252.16]  because this is a question
[1252.16 --> 1253.18]  that surfaces
[1253.18 --> 1254.28]  somewhat regularly
[1254.28 --> 1256.34]  and we've had
[1256.34 --> 1257.16]  entire discussions
[1257.16 --> 1258.04]  about what exactly
[1258.04 --> 1259.02]  is ESP Home.
[1260.08 --> 1260.94]  So it's an interesting
[1260.94 --> 1261.44]  question.
[1262.20 --> 1263.08]  Probably the easiest
[1263.08 --> 1264.22]  way to express it
[1264.22 --> 1266.34]  is sort of
[1266.34 --> 1267.32]  a platform
[1267.32 --> 1267.98]  or a framework
[1267.98 --> 1269.10]  for building
[1269.10 --> 1272.32]  IoT devices,
[1272.48 --> 1273.30]  embedded devices,
[1273.54 --> 1274.48]  small devices,
[1274.76 --> 1275.86]  things, you know,
[1275.86 --> 1276.34]  where you might
[1276.34 --> 1277.26]  control something
[1277.26 --> 1277.96]  like a, you know,
[1277.96 --> 1278.48]  light bulb
[1278.48 --> 1279.04]  or a lamp
[1279.04 --> 1280.50]  that maybe
[1280.50 --> 1281.20]  changes colors
[1281.20 --> 1281.74]  and is connected
[1281.74 --> 1282.42]  to Wi-Fi
[1282.42 --> 1284.54]  or a thermostat
[1284.54 --> 1285.98]  or something
[1285.98 --> 1286.98]  to water your plants
[1286.98 --> 1287.64]  or your garden,
[1288.18 --> 1288.84]  little devices
[1288.84 --> 1289.32]  like that.
[1289.40 --> 1290.04]  ESP Home
[1290.04 --> 1291.98]  provides a
[1291.98 --> 1293.20]  kind of a foundation
[1293.20 --> 1294.98]  for building
[1294.98 --> 1296.46]  the firmware,
[1297.16 --> 1298.42]  which is essentially
[1298.42 --> 1298.92]  just software
[1298.92 --> 1299.82]  to run on these
[1299.82 --> 1301.10]  small embedded processors,
[1301.74 --> 1302.16]  primarily
[1302.16 --> 1303.84]  expressive devices
[1303.84 --> 1305.46]  that ESP32s
[1305.46 --> 1306.52]  and 8266,
[1306.60 --> 1307.02]  which I think
[1307.02 --> 1307.50]  most people
[1307.50 --> 1308.52]  are familiar with
[1308.52 --> 1310.16]  who've paid attention
[1310.16 --> 1310.88]  to the stuff at all.
[1311.28 --> 1312.04]  You may have heard
[1312.04 --> 1312.38]  of those,
[1312.52 --> 1313.24]  but yeah,
[1313.32 --> 1314.42]  the goal of ESP Home
[1314.42 --> 1315.28]  is to make it easy
[1315.28 --> 1316.86]  to build code
[1316.86 --> 1318.38]  that runs on those devices
[1318.38 --> 1320.94]  so that you can have,
[1321.04 --> 1321.42]  you know,
[1321.44 --> 1322.78]  kind of a custom application
[1322.78 --> 1324.32]  or, you know,
[1324.38 --> 1325.64]  usually you have a problem
[1325.64 --> 1326.24]  you want to solve
[1326.24 --> 1326.94]  and so this is
[1326.94 --> 1328.58]  one way to do that.
[1329.38 --> 1329.50]  Right.
[1329.64 --> 1330.48]  So a bunch of
[1330.48 --> 1331.92]  modular building blocks
[1331.92 --> 1333.14]  of, well,
[1333.16 --> 1333.60]  in your case,
[1333.66 --> 1334.24]  YAML code
[1334.24 --> 1335.46]  that you put into a text file
[1335.46 --> 1336.38]  and it spits out
[1336.38 --> 1337.14]  the binary
[1337.14 --> 1337.92]  that you need
[1337.92 --> 1338.82]  to put onto your
[1338.82 --> 1339.80]  microcontroller.
[1339.96 --> 1340.14]  Yep.
[1340.22 --> 1340.98]  That's a good
[1340.98 --> 1343.20]  kind of 30,000 foot view
[1343.20 --> 1343.78]  of, yep.
[1345.06 --> 1346.60]  I think it clicked for me
[1346.60 --> 1348.06]  I used to compile
[1348.06 --> 1349.48]  things in Arduino
[1349.48 --> 1350.90]  so there were two projects
[1350.90 --> 1351.90]  really that kind of
[1351.90 --> 1353.16]  changed the game
[1353.16 --> 1354.16]  for ESP devices.
[1354.32 --> 1355.10]  One was WLED
[1355.10 --> 1355.84]  and of course
[1355.84 --> 1356.36]  the other one
[1356.36 --> 1357.34]  was ESP Home.
[1357.56 --> 1358.40]  Maybe TAS Motor
[1358.40 --> 1358.78]  I should probably
[1358.78 --> 1359.72]  throw that one in there too
[1359.72 --> 1360.64]  maybe there's three
[1360.64 --> 1362.64]  but ESP Home
[1362.64 --> 1363.50]  is particularly cool
[1363.50 --> 1364.32]  because you guys
[1364.32 --> 1365.50]  support pretty much
[1365.50 --> 1366.56]  every sensor,
[1366.82 --> 1367.98]  every little widget
[1367.98 --> 1369.18]  that you can find
[1369.18 --> 1371.02]  AliExpress,
[1371.24 --> 1371.54]  you know,
[1371.66 --> 1372.06]  or
[1372.06 --> 1374.20]  what's the name
[1374.20 --> 1374.92]  of that little website
[1374.92 --> 1375.88]  where you buy parts?
[1375.88 --> 1377.96]  It totally escaped my mind.
[1378.68 --> 1379.82]  Oh, there's a bunch.
[1380.02 --> 1381.50]  AliExpress is certainly popular.
[1382.00 --> 1383.52]  You can get stuff on Amazon,
[1384.52 --> 1384.84]  you know,
[1385.12 --> 1386.16]  Adafruit SparkFun.
[1386.30 --> 1386.78]  Adafruit,
[1386.86 --> 1387.44]  that's the one.
[1387.54 --> 1387.94]  Thank you.
[1388.08 --> 1388.26]  Yeah.
[1388.80 --> 1390.28]  Yeah, there's lots of places
[1390.28 --> 1391.00]  to get these things.
[1391.72 --> 1392.84]  Yeah, ESP Home
[1392.84 --> 1394.38]  has gained a good bit
[1394.38 --> 1394.86]  of traction
[1394.86 --> 1396.42]  and I think
[1396.42 --> 1398.76]  because of its modularity
[1398.76 --> 1400.28]  and its, you know,
[1400.38 --> 1401.28]  customizability,
[1401.28 --> 1402.60]  it's easy to
[1402.60 --> 1404.00]  make something
[1404.00 --> 1404.82]  as small and simple
[1404.82 --> 1405.28]  as you want
[1405.28 --> 1405.88]  if you just want
[1405.88 --> 1406.64]  to measure temperature
[1406.64 --> 1407.16]  in a room.
[1408.24 --> 1409.48]  It's pretty straightforward
[1409.48 --> 1410.16]  to do that,
[1410.26 --> 1410.64]  honestly,
[1410.84 --> 1411.50]  about as straightforward
[1411.50 --> 1412.18]  as it can get.
[1412.40 --> 1412.60]  Cheap.
[1412.82 --> 1413.52]  And it is,
[1413.56 --> 1414.14]  it's very cheap.
[1414.22 --> 1414.74]  The parts
[1414.74 --> 1416.00]  are dirt cheap.
[1416.16 --> 1416.30]  You know,
[1416.34 --> 1417.66]  you can get a three-pack
[1417.66 --> 1419.34]  of ESP32s on Amazon,
[1419.92 --> 1420.08]  you know,
[1420.12 --> 1420.36]  the little,
[1420.46 --> 1421.50]  just the little breakout boards
[1421.50 --> 1422.34]  with all the little pins
[1422.34 --> 1423.42]  and it's like,
[1423.50 --> 1423.72]  you know,
[1423.78 --> 1424.46]  $10 or $11.
[1425.30 --> 1425.66]  So,
[1425.76 --> 1426.44]  it's quite nice.
[1426.88 --> 1427.96]  It's really not that often
[1427.96 --> 1429.48]  in the smart home world
[1429.48 --> 1429.84]  at least
[1429.84 --> 1431.20]  where we can build something
[1431.20 --> 1433.02]  fully open source,
[1434.04 --> 1434.44]  cheaper,
[1435.06 --> 1436.04]  and hackable
[1436.04 --> 1438.10]  than we can buy some,
[1438.22 --> 1438.56]  you know,
[1438.78 --> 1440.10]  pre-made thing on Amazon.
[1440.44 --> 1441.86]  I really love
[1441.86 --> 1442.38]  and value
[1442.38 --> 1443.86]  the ESP Home project
[1443.86 --> 1444.62]  quite dearly.
[1444.74 --> 1445.24]  Temperature sensors
[1445.24 --> 1446.32]  all around my house
[1446.32 --> 1447.52]  are powered by it.
[1447.56 --> 1448.78]  My garage door openers
[1448.78 --> 1449.66]  are powered by it.
[1449.70 --> 1450.48]  All sorts of stuff.
[1450.62 --> 1450.72]  Yep.
[1451.24 --> 1452.38]  Which leads me to,
[1452.66 --> 1452.90]  nicely,
[1453.08 --> 1454.14]  the update question.
[1454.40 --> 1454.58]  So,
[1454.68 --> 1455.48]  some of these things
[1455.48 --> 1457.16]  I have inside walls
[1457.16 --> 1459.06]  on top of my garage door opener
[1459.06 --> 1459.94]  so I have to get up a ladder
[1459.94 --> 1460.98]  to go and reset it
[1460.98 --> 1461.82]  which actually,
[1461.94 --> 1462.66]  now I think about it,
[1462.82 --> 1463.12]  thankfully,
[1463.20 --> 1464.08]  I've never had to do.
[1464.52 --> 1467.02]  But what is the source of truth?
[1467.16 --> 1469.06]  What is your proper opinion
[1469.06 --> 1470.24]  on how often people
[1470.24 --> 1471.34]  should update these things?
[1471.40 --> 1472.14]  What's the life cycle
[1472.14 --> 1472.84]  of the firmware?
[1473.44 --> 1473.68]  So,
[1474.00 --> 1474.32]  yeah,
[1474.50 --> 1475.50]  you're definitely not
[1475.50 --> 1476.82]  the first person to ask this
[1476.82 --> 1478.24]  and it comes up
[1478.24 --> 1478.88]  on the Discord
[1478.88 --> 1480.22]  and community forums a lot.
[1480.90 --> 1482.26]  I think to answer that
[1482.26 --> 1483.52]  in a way that
[1483.52 --> 1484.66]  the audience
[1484.66 --> 1485.52]  will appreciate,
[1485.52 --> 1486.68]  we need to
[1486.68 --> 1487.78]  look
[1487.78 --> 1489.28]  a little bit
[1489.28 --> 1490.30]  into how ESPHome
[1490.30 --> 1491.26]  actually works.
[1491.84 --> 1492.24]  And I'm just
[1492.24 --> 1493.12]  getting kind of
[1493.12 --> 1494.22]  from a high level here.
[1494.66 --> 1495.60]  I don't want to go
[1495.60 --> 1496.60]  into gruesome detail
[1496.60 --> 1497.72]  because we just don't need to.
[1497.92 --> 1498.08]  But,
[1498.62 --> 1499.52]  understand that
[1499.52 --> 1500.72]  ESPHome,
[1501.06 --> 1501.96]  when you create
[1501.96 --> 1502.96]  a YAML file,
[1503.64 --> 1504.86]  you are describing
[1504.86 --> 1506.44]  the bits,
[1507.54 --> 1508.08]  portions
[1508.08 --> 1509.62]  of ESPHome
[1509.62 --> 1510.92]  that you want to use
[1510.92 --> 1512.50]  on your device.
[1512.50 --> 1513.34]  So,
[1513.54 --> 1513.98]  for example,
[1514.28 --> 1515.22]  I have an infrared,
[1515.54 --> 1516.78]  just an IR blaster
[1516.78 --> 1517.66]  in my living room
[1517.66 --> 1518.88]  to control my television,
[1519.46 --> 1520.14]  AV system,
[1520.22 --> 1520.92]  and air conditioner.
[1521.70 --> 1522.50]  That means,
[1522.60 --> 1523.52]  so on that device,
[1523.94 --> 1524.42]  of course,
[1524.48 --> 1525.46]  there's the kind of
[1525.46 --> 1526.36]  foundational stuff,
[1526.52 --> 1527.50]  the Wi-Fi stack,
[1527.58 --> 1528.24]  the network stack,
[1529.10 --> 1531.74]  the API logger,
[1532.00 --> 1533.16]  and the infrared component
[1533.16 --> 1534.12]  that actually generates
[1534.12 --> 1535.10]  the codes and transmits them.
[1535.56 --> 1536.52]  But I understand that
[1536.52 --> 1537.78]  as I've built this device,
[1537.78 --> 1539.84]  I'm not using
[1539.84 --> 1541.02]  the entirety
[1541.02 --> 1541.94]  of everything
[1541.94 --> 1542.82]  in ESPHome.
[1542.94 --> 1543.56]  I'm using
[1543.56 --> 1544.58]  specific components.
[1545.52 --> 1545.88]  And so,
[1546.04 --> 1546.78]  when you consider
[1546.78 --> 1547.92]  that there's a new release
[1547.92 --> 1549.54]  on this device,
[1549.88 --> 1551.64]  if parts of ESPHome
[1551.64 --> 1552.28]  have changed
[1552.28 --> 1553.36]  that aren't irrelevant
[1553.36 --> 1555.04]  to what I'm actually
[1555.04 --> 1556.28]  running on this device,
[1556.80 --> 1558.36]  then updating it
[1558.36 --> 1559.42]  might actually
[1559.42 --> 1560.54]  really just
[1560.54 --> 1561.66]  not do anything
[1561.66 --> 1562.60]  other than change
[1562.60 --> 1563.70]  the compilation date.
[1564.12 --> 1564.56]  So,
[1564.94 --> 1566.08]  it's important
[1566.08 --> 1566.90]  to consider that.
[1567.00 --> 1567.18]  You know,
[1567.24 --> 1567.98]  we kind of
[1567.98 --> 1568.60]  nudge people,
[1568.72 --> 1568.82]  you know,
[1568.84 --> 1569.38]  you should read
[1569.38 --> 1569.94]  the release notes,
[1570.04 --> 1570.80]  read the change logs.
[1570.90 --> 1571.98]  But if you really
[1571.98 --> 1572.62]  want to know
[1572.62 --> 1573.04]  if you need
[1573.04 --> 1574.22]  to update a device,
[1574.82 --> 1575.72]  you need to do that
[1575.72 --> 1576.30]  in this case.
[1576.30 --> 1577.64]  Because it's quite possible
[1577.64 --> 1580.04]  that parts of ESPHome
[1580.04 --> 1581.88]  from release to release,
[1581.98 --> 1582.56]  especially like
[1582.56 --> 1583.14]  the underlying
[1583.14 --> 1584.10]  the foundational stuff
[1584.10 --> 1585.40]  like the Wi-Fi driver,
[1585.90 --> 1587.00]  the network stack,
[1587.30 --> 1587.78]  the API,
[1588.02 --> 1588.96]  that's not changing
[1588.96 --> 1589.78]  in every release.
[1590.20 --> 1590.48]  And so,
[1590.58 --> 1591.74]  if you rebuild your code,
[1592.24 --> 1592.54]  again,
[1592.66 --> 1593.82]  you may not be
[1593.82 --> 1594.74]  getting anything for that.
[1595.22 --> 1595.48]  So,
[1595.48 --> 1596.90]  should you update
[1596.90 --> 1597.68]  every release?
[1598.66 --> 1600.22]  And you probably
[1600.22 --> 1601.86]  actually don't need to.
[1602.08 --> 1602.22]  Now,
[1602.34 --> 1603.38]  I will admit,
[1604.12 --> 1604.96]  as having been
[1604.96 --> 1605.50]  a sysadmin
[1605.50 --> 1606.70]  for 15-something years,
[1606.74 --> 1607.44]  I get the pattern
[1607.44 --> 1607.74]  of like,
[1607.78 --> 1608.34]  we want to update
[1608.34 --> 1608.82]  all the things
[1608.82 --> 1609.66]  as quickly as possible.
[1609.76 --> 1610.36]  We want to patch,
[1610.42 --> 1610.92]  we want to make sure
[1610.92 --> 1611.82]  there's no vulnerabilities
[1611.82 --> 1612.92]  and so on and so forth.
[1613.00 --> 1614.56]  And I completely get that.
[1614.64 --> 1615.32]  I've dealt with,
[1615.44 --> 1615.78]  you know,
[1615.84 --> 1616.66]  compliance issues,
[1616.80 --> 1617.52]  business policies,
[1617.66 --> 1619.00]  things like PCI compliance.
[1619.18 --> 1619.32]  And so,
[1619.36 --> 1620.04]  so I get like
[1620.04 --> 1621.36]  why we want to patch.
[1622.48 --> 1623.74]  These are embedded devices.
[1624.00 --> 1624.76]  And so consequently,
[1624.76 --> 1626.44]  the behavior,
[1626.56 --> 1627.22]  the patterns
[1627.22 --> 1628.34]  are at least
[1628.34 --> 1629.06]  a little bit different.
[1629.50 --> 1630.28]  And so,
[1630.96 --> 1631.96]  updating every month,
[1632.10 --> 1632.98]  patching every month,
[1633.72 --> 1636.08]  you could very well
[1636.08 --> 1636.84]  be in a situation
[1636.84 --> 1637.94]  where other than
[1637.94 --> 1638.74]  rebuilding the code,
[1638.80 --> 1639.36]  you're not actually
[1639.36 --> 1640.20]  changing anything.
[1640.68 --> 1641.16]  So,
[1642.46 --> 1642.90]  the end,
[1643.04 --> 1644.42]  the classic engineering answer,
[1644.50 --> 1644.92]  should you update
[1644.92 --> 1645.32]  every month?
[1645.40 --> 1645.56]  Well,
[1645.58 --> 1646.04]  it depends.
[1646.04 --> 1647.20]  Yeah,
[1647.42 --> 1647.98]  fantastic.
[1648.24 --> 1649.18]  I was kind of hoping
[1649.18 --> 1649.74]  you'd say that,
[1649.80 --> 1650.22]  to be honest.
[1651.06 --> 1651.64]  But it's interesting
[1651.64 --> 1652.64]  what you say about,
[1652.84 --> 1653.16]  you know,
[1653.20 --> 1654.06]  different portions
[1654.06 --> 1655.44]  of the code base changing.
[1656.40 --> 1656.80]  Potentially,
[1656.96 --> 1658.08]  it would still recompile
[1658.08 --> 1658.64]  and still show
[1658.64 --> 1659.54]  as an update pending
[1659.54 --> 1661.22]  in the ESP home integration
[1661.22 --> 1661.82]  in Home Assistant,
[1661.98 --> 1662.44]  for example.
[1662.62 --> 1662.78]  Yes.
[1663.90 --> 1665.12]  Would there ever be
[1665.12 --> 1665.84]  a future
[1665.84 --> 1666.78]  where you guys
[1666.78 --> 1667.40]  would have
[1667.40 --> 1669.14]  smaller Delta updates
[1669.14 --> 1670.02]  that are a bit smarter
[1670.02 --> 1670.52]  about this?
[1670.52 --> 1671.04]  Yeah,
[1671.20 --> 1671.68]  we've actually,
[1671.88 --> 1672.90]  there's been some
[1672.90 --> 1673.70]  kind of on and off
[1673.70 --> 1674.68]  conversation about
[1674.68 --> 1675.84]  how could we better
[1675.84 --> 1676.86]  deal with that?
[1677.54 --> 1677.94]  And so,
[1678.16 --> 1679.56]  I don't want to say
[1679.56 --> 1680.76]  that there's a solution
[1680.76 --> 1682.44]  or a specific idea
[1682.44 --> 1682.98]  in the works
[1682.98 --> 1683.78]  to address that,
[1683.98 --> 1685.82]  but it is something
[1685.82 --> 1686.66]  that's on the radar
[1686.66 --> 1687.26]  where,
[1687.50 --> 1687.92]  you know,
[1688.00 --> 1689.56]  we have maybe
[1689.56 --> 1690.68]  the ESP home dashboard
[1690.68 --> 1691.66]  or some part
[1691.66 --> 1692.26]  of Home Assistant.
[1692.44 --> 1693.46]  I'm not really sure
[1693.46 --> 1694.52]  exactly where that would lie,
[1694.60 --> 1695.76]  but there would be
[1695.76 --> 1696.64]  some part of it
[1696.64 --> 1697.92]  that understands
[1697.92 --> 1699.34]  which components
[1699.34 --> 1700.14]  you've used
[1700.14 --> 1702.26]  as a part of configuration
[1702.26 --> 1703.28]  for which devices
[1703.28 --> 1704.90]  and just flag updates
[1704.90 --> 1706.42]  based on what's used
[1706.42 --> 1706.94]  and where.
[1708.12 --> 1708.86]  That's probably
[1708.86 --> 1709.64]  a little ways off,
[1709.78 --> 1710.28]  but again,
[1710.36 --> 1711.26]  it is something
[1711.26 --> 1712.10]  that we've had
[1712.10 --> 1712.60]  on the radar
[1712.60 --> 1713.74]  and it surfaces
[1713.74 --> 1714.28]  now and then.
[1714.66 --> 1715.16]  It's good to know
[1715.16 --> 1715.88]  you're thinking about it,
[1715.92 --> 1716.10]  though.
[1716.42 --> 1716.92]  And I'll tell you,
[1717.02 --> 1717.70]  one of the things
[1717.70 --> 1718.40]  that occurs to me,
[1718.50 --> 1719.64]  particularly with those devices
[1719.64 --> 1720.98]  that I put inside a wall,
[1721.64 --> 1723.30]  I know that flash storage
[1723.30 --> 1724.94]  has a finite lifespan.
[1725.22 --> 1726.06]  It does, yeah.
[1726.32 --> 1728.10]  Am I killing my ESP devices
[1728.10 --> 1729.30]  by updating them every week?
[1729.38 --> 1729.62]  Yeah,
[1729.62 --> 1730.56]  so that's another
[1730.56 --> 1731.24]  great question
[1731.24 --> 1732.92]  and definitely another one
[1732.92 --> 1733.80]  that I've seen
[1733.80 --> 1734.50]  serviced before.
[1735.40 --> 1735.66]  You know,
[1735.84 --> 1736.66]  a write is a write,
[1737.16 --> 1737.74]  especially some
[1737.74 --> 1738.60]  of the newer ESPs
[1738.60 --> 1739.86]  have a larger quantity
[1739.86 --> 1740.60]  of flash memory.
[1740.74 --> 1741.18]  It used to be
[1741.18 --> 1741.76]  that they shipped
[1741.76 --> 1742.18]  with, you know,
[1742.24 --> 1743.20]  half a megabyte
[1743.20 --> 1743.94]  or one megabyte
[1743.94 --> 1744.46]  like you'd see
[1744.46 --> 1745.98]  in a lot of the 8266s,
[1746.34 --> 1747.12]  maybe two megabytes.
[1747.66 --> 1748.50]  Some of the newer ones
[1748.50 --> 1750.38]  like the newer ESP32 modules
[1750.38 --> 1751.40]  and there are the S3s,
[1751.44 --> 1752.22]  some of these are shipping
[1752.22 --> 1752.80]  with, you know,
[1752.90 --> 1755.10]  1632 megabytes of flash.
[1755.26 --> 1756.26]  Whoa, slow down.
[1756.26 --> 1757.02]  I know, right?
[1757.14 --> 1757.48]  Huge.
[1757.48 --> 1758.94]  It's crazy time.
[1758.98 --> 1760.22]  Where's my NVMe, right?
[1760.64 --> 1762.10]  But point being,
[1762.20 --> 1763.08]  if you're only writing
[1763.08 --> 1764.08]  code on there,
[1764.28 --> 1764.46]  you know,
[1764.48 --> 1765.38]  if you're only using,
[1765.38 --> 1766.32]  you know,
[1766.34 --> 1767.46]  one or two megabytes,
[1767.58 --> 1769.34]  then some of that can be,
[1769.42 --> 1770.62]  because these things
[1770.62 --> 1771.76]  do do, you know,
[1771.82 --> 1772.84]  techniques like wear leveling
[1772.84 --> 1773.36]  and so on.
[1773.40 --> 1775.22]  And so there can be
[1775.22 --> 1775.82]  some distribution
[1775.82 --> 1776.72]  of those writes
[1776.72 --> 1778.20]  over the larger memory area.
[1778.20 --> 1780.36]  And if you are,
[1780.62 --> 1781.64]  unless you have
[1781.64 --> 1782.90]  deliberately created
[1782.90 --> 1784.00]  some code
[1784.00 --> 1785.62]  that is rewriting
[1785.62 --> 1786.38]  the flash
[1786.38 --> 1787.62]  every second
[1787.62 --> 1788.64]  of every minute
[1788.64 --> 1789.42]  of every hour
[1789.42 --> 1790.24]  of every day,
[1790.36 --> 1791.36]  they actually tend
[1791.36 --> 1792.34]  to last quite a while.
[1792.92 --> 1794.14]  Certainly updating them
[1794.14 --> 1795.14]  once or twice a month,
[1795.30 --> 1796.64]  the thing is still
[1796.64 --> 1797.44]  going to run for,
[1797.60 --> 1797.76]  you know,
[1797.80 --> 1799.06]  probably tens of years
[1799.06 --> 1800.08]  before you exhaust
[1800.08 --> 1801.16]  all the write cycles.
[1801.80 --> 1801.92]  You know,
[1801.94 --> 1803.02]  another thing to consider
[1803.02 --> 1805.36]  is some people
[1805.36 --> 1807.84]  use these in devices
[1807.84 --> 1808.58]  like lamps
[1808.58 --> 1809.48]  or thermostats
[1809.48 --> 1810.66]  where this state
[1810.66 --> 1811.78]  changes periodically,
[1811.78 --> 1813.76]  but they want
[1813.76 --> 1814.18]  this state
[1814.18 --> 1815.00]  to be restored
[1815.00 --> 1816.72]  after a power cycle
[1816.72 --> 1817.40]  or a reboot
[1817.40 --> 1818.06]  or a crash,
[1818.16 --> 1818.42]  whatever.
[1818.96 --> 1819.76]  And so there's a,
[1819.76 --> 1820.00]  you know,
[1820.04 --> 1821.04]  a portion of the memory
[1821.04 --> 1821.58]  that's used
[1821.58 --> 1822.30]  as essentially
[1822.30 --> 1823.46]  just non-volatile storage
[1823.46 --> 1824.72]  for data,
[1824.90 --> 1826.38]  not just a program code.
[1827.14 --> 1829.24]  And so that can be rewritten.
[1830.60 --> 1831.04]  There's,
[1831.12 --> 1831.96]  I think the default
[1831.96 --> 1832.76]  is one minute,
[1832.90 --> 1835.16]  but it only writes changes.
[1835.60 --> 1836.50]  So if something
[1836.50 --> 1837.36]  hasn't changed,
[1837.88 --> 1838.04]  you know,
[1838.08 --> 1838.48]  for example,
[1838.60 --> 1838.90]  so let's say
[1838.90 --> 1839.50]  I have a light bulb
[1839.50 --> 1840.32]  and I turn it on,
[1840.68 --> 1842.14]  it will write
[1842.14 --> 1843.10]  that new state
[1843.10 --> 1844.26]  at, you know,
[1844.30 --> 1844.92]  once a minute.
[1844.92 --> 1845.50]  But the thing is,
[1845.50 --> 1846.06]  is it only writes it
[1846.06 --> 1846.44]  when it changes.
[1846.54 --> 1847.14]  So if I only turn
[1847.14 --> 1847.82]  the light bulb on
[1847.82 --> 1849.02]  and off three times a day,
[1849.14 --> 1850.22]  it's only going to do
[1850.22 --> 1850.94]  six writes
[1850.94 --> 1851.84]  over the course
[1851.84 --> 1852.78]  of the entire day.
[1852.92 --> 1853.72]  It's not like you're
[1853.72 --> 1854.62]  rewriting everything
[1854.62 --> 1855.38]  every minute
[1855.38 --> 1856.60]  or whatever you set
[1856.60 --> 1857.40]  that interval to.
[1857.60 --> 1858.72]  So the flash longevity
[1858.72 --> 1859.34]  is pretty good.
[1859.42 --> 1859.82]  And I'll give you
[1859.82 --> 1860.44]  one more example.
[1861.26 --> 1863.36]  I've got some ESP32 boards
[1863.36 --> 1864.38]  that I use for development.
[1865.36 --> 1867.56]  Sometimes I nuke them
[1867.56 --> 1868.28]  and rewrite them,
[1868.42 --> 1868.64]  you know,
[1868.70 --> 1869.84]  dozens of times a day.
[1870.00 --> 1871.32]  This can sometimes go on
[1871.32 --> 1871.98]  for two,
[1872.10 --> 1872.26]  three,
[1872.38 --> 1873.32]  four weeks at a time.
[1873.50 --> 1874.74]  When you're really
[1874.74 --> 1875.64]  actively developing
[1875.64 --> 1876.88]  something and testing it,
[1877.04 --> 1877.76]  you're going to be,
[1877.82 --> 1878.02]  you know,
[1878.08 --> 1878.38]  writing,
[1878.54 --> 1878.78]  changing,
[1878.90 --> 1879.08]  writing,
[1879.22 --> 1879.48]  changing,
[1879.56 --> 1880.72]  and testing and so on.
[1880.72 --> 1881.82]  I bought them
[1881.82 --> 1883.18]  four or five years ago.
[1883.30 --> 1884.26]  They still work fine today.
[1885.18 --> 1886.78]  So even as a,
[1886.84 --> 1888.18]  doing a little more
[1888.18 --> 1889.04]  aggressive development,
[1889.84 --> 1890.58]  flash,
[1890.92 --> 1891.84]  wearing out the flash
[1891.84 --> 1893.14]  is probably not something
[1893.14 --> 1894.32]  you need to be concerned about.
[1894.84 --> 1895.26]  Well, very good.
[1895.40 --> 1895.60]  Now,
[1895.72 --> 1896.62]  I've got a question for you
[1896.62 --> 1897.34]  about the future
[1897.34 --> 1898.26]  and what things look like.
[1898.32 --> 1898.56]  Obviously,
[1899.02 --> 1900.28]  in the last couple of years,
[1900.62 --> 1902.22]  the ESP home project
[1902.22 --> 1903.16]  was subsumed
[1903.16 --> 1904.06]  or was it,
[1904.06 --> 1905.18]  was it technically acquired?
[1905.30 --> 1906.76]  What was the correct word
[1906.76 --> 1907.36]  to use there
[1907.36 --> 1908.66]  by the Home Assistant project?
[1908.66 --> 1910.56]  Acquired is the term
[1910.56 --> 1911.42]  that's been used.
[1911.56 --> 1911.76]  Yes.
[1911.96 --> 1912.78]  The original creator
[1912.78 --> 1913.50]  of ESP home,
[1913.76 --> 1913.98]  Otto,
[1914.66 --> 1915.98]  he started the project
[1915.98 --> 1916.78]  while he was in school
[1916.78 --> 1919.24]  and he seems to have
[1919.24 --> 1921.42]  moved on to other things
[1921.42 --> 1922.72]  as people do sometimes.
[1923.12 --> 1924.90]  And the project sort of
[1924.90 --> 1927.78]  was laying around
[1927.78 --> 1928.74]  on life support
[1928.74 --> 1929.52]  for a little while.
[1929.82 --> 1931.14]  And I think,
[1931.14 --> 1931.92]  I think Paulus
[1931.92 --> 1932.72]  and some of the other folks
[1932.72 --> 1933.80]  at Nabucasa realized
[1933.80 --> 1934.32]  that like,
[1934.64 --> 1935.68]  ESP home is really great
[1935.68 --> 1937.28]  and we don't want
[1937.28 --> 1938.16]  to just let it die.
[1938.16 --> 1939.50]  We don't want to fork it.
[1939.72 --> 1941.12]  And so they were able
[1941.12 --> 1942.10]  to get in touch with Otto
[1942.10 --> 1944.70]  and they acquired it.
[1944.80 --> 1946.78]  And so now Nabucasa
[1946.78 --> 1948.04]  is managing it
[1948.04 --> 1949.20]  alongside Home Assistant
[1949.20 --> 1951.00]  and a couple of other projects too.
[1951.56 --> 1952.60]  Me and Jesse
[1952.60 --> 1954.10]  are lucky enough
[1954.10 --> 1955.76]  to be working on it full time.
[1956.28 --> 1957.42]  Nabucasa has a number
[1957.42 --> 1958.02]  of other people
[1958.02 --> 1959.62]  that work on Home Assistant
[1959.62 --> 1960.98]  and various aspects of it.
[1961.04 --> 1962.38]  And we are able to do that
[1962.38 --> 1963.50]  entirely due to the support
[1963.50 --> 1964.08]  of the community.
[1964.44 --> 1965.26]  What a gift to humanity.
[1965.66 --> 1966.88]  And I genuinely mean that.
[1966.88 --> 1967.32]  It,
[1967.44 --> 1967.64]  no,
[1967.74 --> 1968.24]  it is.
[1968.34 --> 1968.84]  And like,
[1968.94 --> 1970.10]  we're appreciative
[1970.10 --> 1971.16]  to be able to do that.
[1971.26 --> 1971.84]  And I think
[1971.84 --> 1973.46]  for any listeners
[1973.46 --> 1974.98]  who aren't aware,
[1975.54 --> 1976.84]  Nabucasa exists
[1976.84 --> 1978.42]  because this project
[1978.42 --> 1980.32]  became so big
[1980.32 --> 1981.94]  that a couple of people
[1981.94 --> 1982.58]  working on it
[1982.58 --> 1983.44]  a couple nights a week
[1983.44 --> 1984.00]  after work
[1984.00 --> 1985.00]  for a couple of hours,
[1985.12 --> 1985.38]  just,
[1985.48 --> 1986.18]  it wasn't enough
[1986.18 --> 1987.04]  to keep it going.
[1987.04 --> 1988.82]  And so we needed
[1988.82 --> 1991.16]  a larger group of people
[1991.16 --> 1992.22]  who could really focus
[1992.22 --> 1993.22]  on it full time.
[1994.00 --> 1995.36]  And that is where
[1995.36 --> 1996.50]  Nabucasa came in.
[1996.82 --> 1996.84]  So,
[1996.84 --> 1998.26]  so Paulus and Pascal
[1998.26 --> 2000.06]  started Nabucasa,
[2001.06 --> 2001.40]  what,
[2001.50 --> 2002.20]  going to be
[2002.20 --> 2003.60]  about six years ago
[2003.60 --> 2003.94]  now,
[2004.00 --> 2004.40]  I believe.
[2004.68 --> 2006.32]  And if you subscribe
[2006.32 --> 2008.14]  to the cloud services,
[2008.26 --> 2009.48]  Nabucasa Home Assistant Cloud,
[2009.80 --> 2011.42]  that goes directly to us
[2011.42 --> 2012.60]  to pay us to work on it.
[2012.92 --> 2013.80]  So they found a way
[2013.80 --> 2015.16]  to monetize open source
[2015.16 --> 2017.44]  and all credit to them
[2017.44 --> 2018.16]  for doing so.
[2018.52 --> 2018.96]  Genuinely,
[2019.20 --> 2020.20]  it's not an easy
[2020.20 --> 2020.74]  nut to crack.
[2020.84 --> 2020.98]  I mean,
[2021.00 --> 2022.16]  we've seen just this week
[2022.16 --> 2022.94]  with the Image Project
[2022.94 --> 2025.12]  announcing air quotes licenses
[2025.12 --> 2025.82]  and being,
[2025.88 --> 2026.10]  you know,
[2026.12 --> 2027.14]  acquired by Futo.
[2027.44 --> 2028.40]  And it's,
[2028.40 --> 2029.04]  it's not,
[2029.46 --> 2030.70]  it's not an easy road
[2030.70 --> 2032.08]  to tread at all.
[2032.08 --> 2034.20]  And the Nabucasa project
[2034.20 --> 2034.74]  seems to be doing
[2034.74 --> 2035.36]  a pretty good job
[2035.36 --> 2036.12]  with that subscription.
[2036.54 --> 2038.16]  So let me ask you this,
[2038.30 --> 2039.22]  what's the feature
[2039.22 --> 2039.86]  on the roadmap
[2039.86 --> 2040.50]  that's got you
[2040.50 --> 2041.42]  the most excited?
[2042.60 --> 2044.90]  That's a good question there.
[2045.04 --> 2045.30]  You know,
[2045.36 --> 2047.06]  there's been a lot of work
[2047.06 --> 2049.22]  on voice stuff in general.
[2049.74 --> 2051.38]  And that has been
[2051.38 --> 2053.04]  really exciting
[2053.04 --> 2054.22]  and interesting to watch.
[2055.10 --> 2055.78]  I'm not sure that
[2055.78 --> 2056.74]  that would have happened.
[2056.86 --> 2057.00]  You know,
[2057.04 --> 2057.24]  there's,
[2057.32 --> 2058.54]  there's other projects
[2058.54 --> 2059.38]  who are experimenting
[2059.38 --> 2060.28]  with voice
[2060.28 --> 2061.42]  in any number of ways.
[2062.36 --> 2064.44]  The interesting part,
[2064.52 --> 2064.88]  I think,
[2065.04 --> 2066.72]  is that a home assistant
[2066.72 --> 2069.24]  is a great application
[2069.24 --> 2070.40]  of something like that.
[2070.44 --> 2071.12]  It's one thing
[2071.12 --> 2072.72]  to build an environment,
[2072.90 --> 2073.06]  you know,
[2073.10 --> 2073.22]  with,
[2073.28 --> 2074.08]  we have things
[2074.08 --> 2075.00]  now certainly like
[2075.00 --> 2075.60]  ChatGPT
[2075.60 --> 2076.64]  and these large language models.
[2076.64 --> 2077.76]  And it's one thing
[2077.76 --> 2078.30]  to have something
[2078.30 --> 2079.08]  that you can talk to
[2079.08 --> 2080.30]  or chat with,
[2080.40 --> 2081.02]  but it's,
[2081.14 --> 2082.08]  it kind of takes it
[2082.08 --> 2082.80]  to the next level
[2082.80 --> 2083.96]  to wire that in,
[2084.00 --> 2084.66]  so to speak,
[2084.66 --> 2085.96]  to something like
[2085.96 --> 2086.54]  home assistant
[2086.54 --> 2087.88]  where now there's
[2087.88 --> 2088.84]  a specific application.
[2088.84 --> 2089.52]  I can ask it
[2089.52 --> 2090.38]  to turn on a light
[2090.38 --> 2091.08]  or I can ask it
[2091.08 --> 2092.16]  to turn down the heat.
[2092.66 --> 2092.82]  You know,
[2092.86 --> 2093.48]  I can ask it
[2093.48 --> 2094.50]  to turn on a fan.
[2094.84 --> 2096.02]  It's cool to see that.
[2096.10 --> 2096.56]  And so I've,
[2096.56 --> 2097.08]  I've enjoyed
[2097.08 --> 2098.40]  kind of watching that.
[2098.40 --> 2099.34]  And admittedly,
[2099.34 --> 2101.22]  I don't do anywhere
[2101.22 --> 2101.86]  near as much.
[2101.96 --> 2102.06]  We,
[2102.18 --> 2102.98]  like we have a couple
[2102.98 --> 2103.30]  people,
[2103.38 --> 2104.14]  Mike and Kevin now
[2104.14 --> 2104.60]  who are working
[2104.60 --> 2105.26]  on the boys stuff
[2105.26 --> 2105.96]  really full time.
[2106.52 --> 2107.60]  Jesse had already
[2107.60 --> 2108.44]  written a lot of it
[2108.44 --> 2109.78]  when I,
[2109.96 --> 2110.54]  at least the ESP
[2110.54 --> 2111.30]  home side of it
[2111.30 --> 2112.22]  when I joined
[2112.22 --> 2113.88]  Nabucasa last year.
[2114.46 --> 2115.62]  So I've been a little
[2115.62 --> 2117.34]  bit more on the sidelines,
[2117.46 --> 2117.88]  if you will,
[2118.00 --> 2118.82]  kind of watching.
[2118.94 --> 2120.20]  I jump in where I can,
[2120.34 --> 2121.84]  but that's been
[2121.84 --> 2122.82]  really cool to watch.
[2123.24 --> 2124.42]  Other things coming up.
[2124.48 --> 2125.70]  We did something cool
[2125.70 --> 2126.98]  just in the last release
[2126.98 --> 2128.20]  with the update entities.
[2129.24 --> 2130.46]  Updating ESP home
[2130.46 --> 2132.12]  used to mean
[2132.12 --> 2133.16]  compiling source
[2133.16 --> 2133.68]  on your,
[2133.78 --> 2134.82]  your local machine
[2134.82 --> 2135.60]  and that machine
[2135.60 --> 2136.16]  being your,
[2136.38 --> 2136.56]  you know,
[2136.60 --> 2137.28]  whatever your home
[2137.28 --> 2137.88]  assistant instance
[2137.88 --> 2138.72]  is running on
[2138.72 --> 2139.08]  or,
[2139.68 --> 2139.96]  you know,
[2139.96 --> 2140.52]  maybe a laptop
[2140.52 --> 2141.44]  or desktop system
[2141.44 --> 2141.92]  if you have it
[2141.92 --> 2142.62]  set up that way.
[2142.62 --> 2143.30]  But it meant
[2143.30 --> 2144.08]  compiling the source
[2144.08 --> 2144.88]  on your local machine
[2144.88 --> 2145.72]  and then pushing it
[2145.72 --> 2147.26]  to the ESP,
[2147.60 --> 2147.98]  you know,
[2148.04 --> 2148.62]  over the air,
[2148.72 --> 2149.62]  OTA as we say.
[2150.36 --> 2152.78]  And in this last release,
[2153.06 --> 2153.98]  we had a contributor
[2153.98 --> 2156.40]  who created a PR
[2156.40 --> 2157.96]  to allow an ESP device
[2157.96 --> 2159.32]  to pull an update.
[2159.86 --> 2160.96]  So now there's a mechanism
[2160.96 --> 2161.60]  or an action
[2161.60 --> 2162.52]  that you can trigger
[2162.52 --> 2164.34]  within ESP home
[2164.34 --> 2166.22]  that you give it
[2166.22 --> 2167.00]  the,
[2167.00 --> 2167.76]  a URL
[2167.76 --> 2168.86]  or web address
[2168.86 --> 2170.78]  of a firmware image
[2170.78 --> 2171.92]  and it will then
[2171.92 --> 2172.52]  download that
[2172.52 --> 2173.02]  and install it.
[2173.08 --> 2173.54]  It works similar
[2173.54 --> 2174.82]  to how WLED does
[2174.82 --> 2176.58]  where you can give it
[2176.58 --> 2177.78]  the address of the file
[2177.78 --> 2178.48]  and it will pull it
[2178.48 --> 2178.76]  and then,
[2178.80 --> 2178.94]  you know,
[2178.96 --> 2179.90]  essentially install it
[2179.90 --> 2180.52]  on its own.
[2181.12 --> 2181.72]  So now we have
[2181.72 --> 2182.32]  that capability
[2182.32 --> 2183.50]  in ESP home as well.
[2183.98 --> 2184.62]  And then we took it
[2184.62 --> 2185.32]  even a step further
[2185.32 --> 2186.04]  and integrated it
[2186.04 --> 2187.00]  with update entities
[2187.00 --> 2188.92]  in Home Assistant
[2188.92 --> 2192.16]  so that now
[2192.16 --> 2194.42]  if there is an update
[2194.42 --> 2196.34]  available for your device
[2196.34 --> 2197.52]  from the publisher,
[2197.66 --> 2197.96]  let's say,
[2198.02 --> 2198.42]  for example,
[2198.42 --> 2199.64]  you bought a light bulb
[2199.64 --> 2200.58]  that has ESP home
[2200.58 --> 2201.48]  pre-installed on it,
[2202.18 --> 2203.48]  the manufacturer,
[2203.64 --> 2204.60]  developer of that device
[2204.60 --> 2205.74]  can just publish an update
[2205.74 --> 2206.90]  and then you'll just get
[2206.90 --> 2207.66]  an update button
[2207.66 --> 2208.46]  in Home Assistant
[2208.46 --> 2209.22]  and it will actually
[2209.22 --> 2209.92]  pull the update
[2209.92 --> 2210.72]  and it takes,
[2210.84 --> 2211.06]  you know,
[2211.30 --> 2211.46]  10,
[2211.54 --> 2212.20]  20 seconds
[2212.20 --> 2213.14]  as opposed to
[2213.14 --> 2214.30]  potentially an hour
[2214.30 --> 2214.84]  or more
[2214.84 --> 2216.78]  trying to compile source.
[2217.26 --> 2218.06]  I see a lot of people
[2218.06 --> 2219.12]  trying to build source code
[2219.12 --> 2220.22]  for these devices
[2220.22 --> 2220.72]  on, you know,
[2220.72 --> 2221.86]  something like a Raspberry Pi
[2221.86 --> 2222.66]  or these Odroids
[2222.66 --> 2225.06]  and you can do it
[2225.06 --> 2226.68]  but I can't wait an hour
[2226.68 --> 2227.70]  for my source to build
[2227.70 --> 2228.82]  for a single ESP.
[2229.06 --> 2229.84]  I need it to happen
[2229.84 --> 2230.62]  and, you know,
[2231.14 --> 2232.14]  sub one minute
[2232.14 --> 2232.80]  and so that's,
[2232.94 --> 2234.38]  I tend to build everything
[2234.38 --> 2234.94]  on my MacBook
[2234.94 --> 2236.46]  but regardless,
[2237.24 --> 2238.16]  this is another way
[2238.16 --> 2238.94]  to update devices
[2238.94 --> 2239.92]  and I think that's
[2239.92 --> 2240.80]  pretty cool
[2240.80 --> 2241.58]  because it can make
[2241.58 --> 2242.18]  managing things
[2242.18 --> 2242.72]  a lot easier
[2242.72 --> 2243.78]  and certainly speed things up
[2243.78 --> 2244.46]  for people
[2244.46 --> 2245.80]  who just want to go
[2245.80 --> 2246.46]  and play
[2246.46 --> 2248.38]  and not build
[2248.38 --> 2248.92]  and go through
[2248.92 --> 2249.72]  that whole process
[2249.72 --> 2252.82]  so it's cool to see that.
[2254.02 --> 2254.34]  And then,
[2254.44 --> 2255.54]  yeah,
[2255.62 --> 2256.90]  there's voice stuff ongoing
[2256.90 --> 2258.28]  so we'll have some more
[2258.28 --> 2258.88]  to talk about
[2258.88 --> 2259.90]  I think later this year
[2259.90 --> 2260.74]  and in that regard,
[2260.84 --> 2262.10]  I don't want to spoil
[2262.10 --> 2262.94]  any big surprises
[2262.94 --> 2263.42]  or anything
[2263.42 --> 2266.10]  but there's some cool stuff.
[2266.42 --> 2266.70]  Oh,
[2266.90 --> 2267.70]  I was hoping we'd get
[2267.70 --> 2268.02]  something.
[2268.02 --> 2268.42]  Yeah,
[2269.44 --> 2270.44]  I know how it goes.
[2270.56 --> 2270.74]  Anyway,
[2271.06 --> 2271.88]  we can ask people
[2271.88 --> 2272.72]  to tune into
[2272.72 --> 2274.12]  the monthly live streams
[2274.12 --> 2274.92]  that you and the rest
[2274.92 --> 2275.86]  of the Nabucasa project
[2275.86 --> 2276.70]  do every time
[2276.70 --> 2277.74]  there's a Home Assistant release.
[2278.02 --> 2279.30]  The Home Assistant project
[2279.30 --> 2280.24]  and ESP Home release
[2280.24 --> 2281.26]  is a kind of lockstep
[2281.26 --> 2281.98]  these days, right?
[2282.42 --> 2282.70]  Yeah,
[2282.78 --> 2284.42]  so the Home Assistant releases
[2284.42 --> 2285.92]  are at the top of the month.
[2286.44 --> 2287.26]  I believe they're doing
[2287.26 --> 2287.90]  the first Wednesday
[2287.90 --> 2288.26]  of the month
[2288.26 --> 2288.86]  is the release
[2288.86 --> 2290.96]  and ESP Home
[2290.96 --> 2292.24]  is offset by two weeks
[2292.24 --> 2293.32]  so we're doing
[2293.32 --> 2294.12]  the middle of the month
[2294.12 --> 2295.18]  I think the third Wednesday
[2295.18 --> 2296.66]  is when we release
[2296.66 --> 2298.52]  so that's the schedule
[2298.52 --> 2299.88]  that we try very hard
[2299.88 --> 2300.46]  to stick to
[2300.46 --> 2302.04]  and I think so far
[2302.04 --> 2302.68]  we've been able to
[2302.68 --> 2303.50]  to keep that.
[2304.38 --> 2305.18]  Well, good deal.
[2305.50 --> 2305.62]  Yeah.
[2305.70 --> 2306.22]  I want to say thank you
[2306.22 --> 2307.18]  very much for joining us
[2307.18 --> 2307.88]  just Keith
[2307.88 --> 2308.76]  from Nabucasa.
[2310.36 --> 2311.18]  It's been a pleasure
[2311.18 --> 2312.96]  and if ever you have
[2312.96 --> 2313.64]  anything exciting
[2313.64 --> 2314.42]  please let us know
[2314.42 --> 2315.40]  and we'll be happy
[2315.40 --> 2316.10]  to talk to you again.
[2316.58 --> 2316.96]  Absolutely.
[2317.76 --> 2318.56]  Thanks for coming on.
[2318.68 --> 2319.16]  Have a great day.
[2321.40 --> 2322.50]  Getgrist.com
[2322.50 --> 2323.50]  slash self-hosted
[2323.50 --> 2325.54]  that's getgrist.com
[2325.54 --> 2326.46]  slash self-hosted.
[2326.56 --> 2326.88]  Grist
[2326.88 --> 2328.30]  is the open source
[2328.30 --> 2329.44]  alternative to Airtable
[2329.44 --> 2330.28]  and Google Sheets.
[2330.62 --> 2331.80]  There are a lot
[2331.80 --> 2332.78]  of no-code tools
[2332.78 --> 2333.28]  out there
[2333.28 --> 2334.78]  but spreadsheets
[2334.78 --> 2336.24]  are the original
[2336.24 --> 2337.68]  low-code app, right?
[2338.38 --> 2339.34]  I could definitely
[2339.34 --> 2339.98]  attest to that
[2339.98 --> 2340.74]  and people have been
[2340.74 --> 2341.80]  building CRMs
[2341.80 --> 2342.48]  and payroll,
[2342.98 --> 2343.74]  event management,
[2343.96 --> 2344.30]  sales,
[2344.46 --> 2344.92]  all of it
[2344.92 --> 2346.08]  inside spreadsheets
[2346.08 --> 2347.20]  for decades
[2347.20 --> 2349.02]  despite the awkward
[2349.02 --> 2350.14]  and limited formulas,
[2350.44 --> 2351.58]  the bad format for it.
[2352.22 --> 2353.64]  What's really smart
[2353.64 --> 2354.64]  about Grist's approach
[2354.64 --> 2356.16]  to the no-code
[2356.16 --> 2357.30]  or low-code app building
[2357.30 --> 2358.60]  it takes what people
[2358.60 --> 2359.44]  already know
[2359.44 --> 2360.70]  and like about spreadsheets
[2360.70 --> 2361.36]  and it connects it
[2361.36 --> 2362.18]  to what people like
[2362.18 --> 2363.44]  more about
[2363.44 --> 2364.44]  robust software.
[2365.08 --> 2365.78]  The collaboration,
[2366.00 --> 2366.90]  the granular access,
[2367.06 --> 2367.56]  APIs,
[2368.16 --> 2369.24]  non-tabular data views
[2369.24 --> 2370.84]  it also raises
[2370.84 --> 2371.48]  the ceiling,
[2371.90 --> 2372.88]  letting advanced users
[2372.88 --> 2373.62]  work with data
[2373.62 --> 2374.34]  using something like
[2374.34 --> 2375.70]  Python or custom widgets
[2375.70 --> 2376.58]  as needed.
[2377.24 --> 2378.22]  I know it's true.
[2378.66 --> 2379.48]  You've probably got
[2379.48 --> 2380.44]  a load-bearing spreadsheet
[2380.44 --> 2381.18]  in your company
[2381.18 --> 2382.26]  or maybe even in your home.
[2382.36 --> 2382.98]  It happens.
[2383.26 --> 2384.32]  The best of us do it.
[2384.86 --> 2385.72]  They become impossible
[2385.72 --> 2386.36]  to maintain
[2386.36 --> 2387.60]  and they're too important
[2387.60 --> 2388.00]  to fail.
[2388.32 --> 2388.94]  Everyone ends up
[2388.94 --> 2389.92]  relying on one of these.
[2390.44 --> 2391.26]  So go try Grist.
[2391.30 --> 2392.40]  It's easy to integrate with.
[2392.48 --> 2393.24]  It's open source.
[2393.34 --> 2394.28]  You can self-host it.
[2394.56 --> 2395.70]  It's run by the French government
[2395.70 --> 2396.82]  who actively contributes
[2396.82 --> 2397.72]  back to the project.
[2397.72 --> 2399.14]  They tried the others
[2399.14 --> 2400.36]  and Grist is the best.
[2400.96 --> 2401.42]  I think you're going
[2401.42 --> 2401.94]  to love it too.
[2402.24 --> 2402.54]  Grist,
[2402.74 --> 2404.08]  the open source alternative
[2404.08 --> 2405.04]  that you can host.
[2405.38 --> 2406.02]  Go try it out
[2406.02 --> 2406.64]  and support the show.
[2406.76 --> 2408.64]  Go to getgrist.com
[2408.64 --> 2409.98]  slash self-hosted.
[2410.10 --> 2412.44]  That's getgrist.com
[2412.44 --> 2414.16]  slash self-hosted.
[2415.60 --> 2416.54]  Everybody's favorite
[2416.54 --> 2418.18]  self-hosted photo software
[2418.18 --> 2419.52]  was in the news this week.
[2419.68 --> 2420.54]  They've announced
[2420.54 --> 2421.16]  that they're going
[2421.16 --> 2423.06]  to start putting a license
[2423.06 --> 2424.46]  or so they called it
[2424.46 --> 2425.56]  in the beginning at least
[2425.56 --> 2427.36]  in front of image.
[2427.56 --> 2428.68]  This is an optional way
[2428.68 --> 2429.44]  for you to support
[2429.44 --> 2430.48]  the project starting
[2430.48 --> 2433.08]  at $25 for an individual license
[2433.08 --> 2435.82]  or $100 for an entire server.
[2436.48 --> 2437.16]  Yeah, and that would be
[2437.16 --> 2438.42]  multiple users essentially.
[2438.58 --> 2439.42]  So if you're an only
[2439.42 --> 2441.28]  one user image instance,
[2441.40 --> 2442.40]  you get a little bit
[2442.40 --> 2443.20]  more of a discount
[2443.20 --> 2445.70]  at $24.99 for lifetime.
[2445.94 --> 2446.48]  But if you have
[2446.48 --> 2447.28]  multiple users,
[2447.28 --> 2447.98]  then you're going
[2447.98 --> 2448.50]  to be kicking up
[2448.50 --> 2449.60]  to $99.99.
[2450.06 --> 2450.94]  Again, that is
[2450.94 --> 2453.24]  a lifetime purchase.
[2453.24 --> 2453.86]  And so they're going
[2453.86 --> 2456.82]  from license to product key.
[2456.94 --> 2457.80]  So instead of a license key,
[2457.84 --> 2458.14]  you're going to have
[2458.14 --> 2458.68]  a product key.
[2459.50 --> 2459.82]  Yeah, well,
[2459.92 --> 2460.82]  when I first saw
[2460.82 --> 2461.78]  this initial announcement
[2461.78 --> 2462.24]  come out
[2462.24 --> 2463.92]  and I saw the word license,
[2464.32 --> 2465.96]  my spidey senses.
[2466.18 --> 2467.00]  I mean, we've been
[2467.00 --> 2467.94]  in the open source community
[2467.94 --> 2468.38]  long enough,
[2468.46 --> 2468.82]  you and I,
[2468.86 --> 2469.42]  to know that
[2469.42 --> 2471.26]  that is a charged word
[2471.26 --> 2472.64]  if ever there was one.
[2473.26 --> 2474.68]  And so a couple of days later,
[2474.82 --> 2475.92]  Alex from the Image Project
[2475.92 --> 2477.42]  came out with a clarification
[2477.42 --> 2479.04]  around the wording
[2479.04 --> 2481.00]  used for purchasing image.
[2481.16 --> 2481.94]  And as Chris says,
[2481.94 --> 2483.20]  they've now changed
[2483.20 --> 2484.00]  the word licensed
[2484.00 --> 2486.54]  to purchase.
[2487.16 --> 2487.60]  Yeah.
[2488.10 --> 2490.12]  With a buy image button now
[2490.12 --> 2491.66]  and then a never show again
[2491.66 --> 2492.74]  and remind me in 30 days.
[2492.80 --> 2494.40]  Now you don't have to buy it,
[2494.46 --> 2494.82]  I guess.
[2494.90 --> 2496.10]  That's the other thing is...
[2496.10 --> 2496.26]  Right.
[2496.32 --> 2498.16]  This is all totally optional.
[2498.32 --> 2499.66]  This is just a way for you
[2499.66 --> 2501.66]  to give some greenbacks
[2501.66 --> 2503.06]  to the Image Project
[2503.06 --> 2504.06]  to support them.
[2504.48 --> 2505.80]  Now, I think we kind of
[2505.80 --> 2506.92]  had a fair warning
[2506.92 --> 2507.72]  this was coming.
[2507.84 --> 2508.54]  When they got
[2508.54 --> 2509.54]  full-time employment
[2509.54 --> 2510.04]  by Fudo,
[2510.22 --> 2510.92]  they talked about
[2510.92 --> 2511.76]  how they believe
[2511.76 --> 2512.58]  that good software
[2512.58 --> 2513.30]  should get paid,
[2513.50 --> 2513.68]  you know,
[2513.72 --> 2514.38]  keep it free,
[2514.48 --> 2515.48]  but you should also pay for it
[2515.48 --> 2516.42]  to make it self-hosted,
[2516.46 --> 2516.84]  but you should be able
[2516.84 --> 2517.46]  to pay for it.
[2518.30 --> 2519.52]  And I think you and I
[2519.52 --> 2520.22]  both agreed
[2520.22 --> 2521.10]  with that assertion.
[2521.34 --> 2522.26]  But now we have
[2522.26 --> 2523.14]  the actual pricing.
[2524.28 --> 2525.00]  $99.99
[2525.00 --> 2526.58]  would be the price I pay
[2526.58 --> 2527.82]  because I want my wife
[2527.82 --> 2528.60]  on this as well.
[2528.98 --> 2529.46]  But, you know,
[2529.50 --> 2530.08]  for some folks,
[2530.14 --> 2531.08]  it's only $24.99
[2531.08 --> 2532.96]  for lifetime licenses.
[2533.04 --> 2533.44]  How do you feel
[2533.44 --> 2534.10]  about that price?
[2534.46 --> 2535.60]  I think it's fine.
[2535.78 --> 2536.08]  I mean,
[2536.16 --> 2537.52]  the amount of money,
[2537.60 --> 2537.84]  actually,
[2537.84 --> 2538.70]  I don't think
[2538.70 --> 2540.16]  is necessarily the issue here.
[2540.16 --> 2541.34]  For me,
[2541.44 --> 2541.96]  it's the fact
[2541.96 --> 2543.32]  that it's a one-time deal.
[2543.92 --> 2545.48]  I would have expected
[2545.48 --> 2546.74]  in this modern world
[2546.74 --> 2548.18]  of subscriptions everywhere
[2548.18 --> 2549.50]  that they would give you
[2549.50 --> 2550.30]  a way to be like,
[2550.36 --> 2550.50]  right,
[2550.56 --> 2551.72]  you can support the project
[2551.72 --> 2553.08]  and get something
[2553.08 --> 2555.02]  that the free people don't
[2555.02 --> 2556.94]  for a certain amount of time,
[2557.08 --> 2557.88]  whether it's,
[2558.00 --> 2558.42]  you know,
[2558.46 --> 2559.52]  you're three months ahead
[2559.52 --> 2560.82]  of the free tier
[2560.82 --> 2562.70]  or something like that.
[2562.72 --> 2564.34]  I don't really quite know
[2564.34 --> 2565.04]  what to suggest
[2565.04 --> 2566.18]  because the last thing
[2566.18 --> 2567.02]  I really want to see
[2567.02 --> 2570.02]  is locking things
[2570.02 --> 2570.82]  behind a paywall
[2570.82 --> 2571.48]  with this project.
[2571.64 --> 2572.38]  And Alex has actually
[2572.38 --> 2572.88]  gone on record
[2572.88 --> 2573.72]  in the GitHub issues,
[2573.80 --> 2574.30]  which will be linked
[2574.30 --> 2574.88]  in the show notes
[2574.88 --> 2575.94]  if you'd like to read them.
[2576.70 --> 2577.42]  He's gone on record
[2577.42 --> 2578.00]  just to say
[2578.00 --> 2578.72]  that we're not going
[2578.72 --> 2579.60]  to add paywalls
[2579.60 --> 2580.12]  to the project
[2580.12 --> 2580.94]  and this purchase
[2580.94 --> 2581.96]  will not grant you
[2581.96 --> 2583.02]  any additional features
[2583.02 --> 2583.62]  in Image.
[2584.26 --> 2585.30]  It just simply says
[2585.30 --> 2586.24]  we rely on users
[2586.24 --> 2586.76]  like you
[2586.76 --> 2587.74]  to support Image's
[2587.74 --> 2588.74]  ongoing development.
[2589.22 --> 2590.30]  And if that's the case,
[2590.52 --> 2592.36]  a single one-time purchase
[2592.36 --> 2594.56]  doesn't seem like
[2594.56 --> 2596.30]  the most sustainable way
[2596.30 --> 2597.38]  to go about doing that.
[2597.98 --> 2598.70]  That's exactly
[2598.70 --> 2599.40]  what I was going to say.
[2600.08 --> 2600.56]  Exactly.
[2600.86 --> 2602.96]  I think $99.99
[2602.96 --> 2605.10]  is a fair chunk of money,
[2605.30 --> 2606.54]  but it's not enough
[2606.54 --> 2607.22]  for a lifetime.
[2607.82 --> 2608.72]  A year or two
[2608.72 --> 2609.90]  or three, maybe.
[2610.04 --> 2610.56]  I don't know,
[2610.74 --> 2611.96]  but definitely not a lifetime
[2611.96 --> 2612.90]  for a piece of software
[2612.90 --> 2613.62]  this complex
[2613.62 --> 2614.64]  that has this much work
[2614.64 --> 2615.30]  getting done on it
[2615.30 --> 2616.24]  that has maybe
[2616.24 --> 2617.06]  a couple of people
[2617.06 --> 2617.76]  now working on it
[2617.76 --> 2618.24]  full-time.
[2618.48 --> 2620.68]  So I don't really get it.
[2620.78 --> 2621.56]  And I know a lot of people
[2621.56 --> 2622.44]  are shocked at first
[2622.44 --> 2624.56]  at $99.99 U.S. greenbacks,
[2625.06 --> 2625.86]  but let's be real
[2625.86 --> 2627.08]  about a developer's salary,
[2627.20 --> 2629.76]  especially a really great developer
[2629.76 --> 2630.72]  who's working
[2630.72 --> 2631.40]  with cutting-edge
[2631.40 --> 2632.24]  web technologies,
[2632.44 --> 2632.82]  cutting-edge
[2632.82 --> 2633.98]  machine learning technologies,
[2634.16 --> 2634.52]  cutting-edge
[2634.52 --> 2635.90]  photo storage technologies,
[2636.44 --> 2637.98]  and mobile clients
[2637.98 --> 2640.02]  for both iOS and Android,
[2640.48 --> 2641.50]  as well as doing
[2641.50 --> 2642.34]  all of this in a way
[2642.34 --> 2643.14]  that can be distributed
[2643.14 --> 2644.42]  to tens of thousands
[2644.42 --> 2645.62]  of self-hosted users.
[2646.22 --> 2648.26]  That's top-tier
[2648.26 --> 2649.62]  development skill.
[2650.02 --> 2650.78]  That's top-tier.
[2651.56 --> 2652.18]  I mean,
[2652.60 --> 2654.92]  and I don't know,
[2655.04 --> 2655.26]  you know,
[2655.32 --> 2656.44]  I don't know
[2656.44 --> 2657.58]  if I'd actually go
[2657.58 --> 2658.28]  and just throw them
[2658.28 --> 2659.22]  another $99.99
[2659.22 --> 2660.06]  every now and then.
[2660.24 --> 2661.02]  Maybe I will.
[2662.96 --> 2664.04]  It gets kind of expensive.
[2664.16 --> 2664.36]  I just,
[2664.48 --> 2665.26]  I wish there was something
[2665.26 --> 2666.04]  in between here,
[2666.12 --> 2668.16]  maybe like $15 a year.
[2668.30 --> 2668.74]  I don't know.
[2669.40 --> 2669.50]  Right.
[2669.86 --> 2670.24]  I mean,
[2670.26 --> 2670.68]  if we were getting
[2670.68 --> 2671.48]  some extra features
[2671.48 --> 2672.22]  for the money,
[2672.52 --> 2673.24]  in a way,
[2673.32 --> 2674.06]  that becomes easier
[2674.06 --> 2674.52]  to stomach.
[2675.22 --> 2676.08]  This is just
[2676.08 --> 2677.24]  a way for us
[2677.24 --> 2677.64]  to say,
[2677.92 --> 2678.16]  yes,
[2678.18 --> 2678.68]  we're going to put
[2678.68 --> 2679.02]  our money
[2679.02 --> 2679.86]  where our mouth is
[2679.86 --> 2680.82]  in terms of supporting
[2680.82 --> 2681.92]  an open source project.
[2682.48 --> 2682.90]  Okay,
[2682.94 --> 2683.44]  here's an idea.
[2684.44 --> 2685.48]  You don't have to,
[2685.48 --> 2687.18]  you don't have to paywall
[2687.18 --> 2688.02]  any of the features
[2688.02 --> 2689.40]  in the application,
[2689.74 --> 2691.62]  but what about
[2691.62 --> 2693.56]  if you pay $15.95
[2693.56 --> 2693.98]  or,
[2694.06 --> 2694.22]  you know,
[2694.28 --> 2695.56]  $35.95 a year,
[2695.62 --> 2696.30]  whatever it is,
[2696.62 --> 2698.40]  you get cloud storage backup,
[2698.56 --> 2699.02]  secure,
[2699.46 --> 2699.78]  guaranteed,
[2699.92 --> 2700.30]  encrypted,
[2700.76 --> 2701.66]  cloud storage backup
[2701.66 --> 2702.20]  for all your photos.
[2702.20 --> 2703.24]  Because right now,
[2703.90 --> 2705.02]  that's what I'm doing.
[2705.14 --> 2706.10]  I'm rolling my own
[2706.10 --> 2706.80]  backup solution
[2706.80 --> 2708.26]  for my image backup
[2708.26 --> 2709.26]  and I'm eating
[2709.26 --> 2710.88]  terabytes of storage
[2710.88 --> 2711.54]  up in the cloud.
[2712.26 --> 2713.72]  I could take that fee
[2713.72 --> 2714.12]  that I'm paying
[2714.12 --> 2714.90]  for that cloud storage
[2714.90 --> 2715.84]  and put it towards image.
[2716.26 --> 2716.36]  Yeah,
[2716.40 --> 2717.22]  that could be an interesting
[2717.22 --> 2718.40]  way to go.
[2719.06 --> 2719.68]  I think also
[2719.68 --> 2721.82]  there is some merit
[2721.82 --> 2722.48]  in the fact
[2722.48 --> 2723.10]  that they've actually
[2723.10 --> 2724.30]  taken the steps
[2724.30 --> 2725.40]  to do this really
[2725.40 --> 2726.02]  and say,
[2726.32 --> 2726.48]  right,
[2726.60 --> 2728.32]  we know that financially
[2728.32 --> 2729.26]  we've got the backing
[2729.26 --> 2729.72]  of Futo,
[2729.72 --> 2731.10]  but we're also going
[2731.10 --> 2731.96]  to look to the community
[2731.96 --> 2734.46]  to set up a new model
[2734.46 --> 2735.40]  for this kind of software.
[2736.22 --> 2736.96]  We've seen
[2736.96 --> 2738.06]  countless times
[2738.06 --> 2739.12]  over the last decade
[2739.12 --> 2740.18]  free and open source
[2740.18 --> 2742.02]  projects come along,
[2742.48 --> 2743.32]  free in beer
[2743.32 --> 2744.70]  as well as licensing,
[2745.42 --> 2746.02]  come along
[2746.02 --> 2746.82]  and fade away
[2746.82 --> 2747.62]  because the developers
[2747.62 --> 2748.42]  lose interest
[2748.42 --> 2749.16]  because obviously
[2749.16 --> 2750.12]  they've got day jobs
[2750.12 --> 2750.70]  or families
[2750.70 --> 2751.80]  or whatever else it is
[2751.80 --> 2752.90]  to take care of.
[2753.06 --> 2754.34]  Sometimes we see them
[2754.34 --> 2755.04]  implode even,
[2755.18 --> 2755.60]  like they don't,
[2755.76 --> 2756.96]  it's not just a slow burnout
[2756.96 --> 2757.78]  but we have seen some
[2757.78 --> 2758.86]  like music server projects
[2758.86 --> 2759.16]  and whatnot
[2759.16 --> 2760.08]  that just explode
[2760.08 --> 2760.66]  or implode.
[2760.98 --> 2761.88]  And so this is a hugely
[2761.88 --> 2762.78]  positive step
[2762.78 --> 2763.92]  for the overall longevity
[2763.92 --> 2765.04]  of the image project,
[2765.14 --> 2765.60]  I think.
[2766.18 --> 2766.70]  But the only thing
[2766.70 --> 2767.44]  I think I would question
[2767.44 --> 2768.30]  is just the single
[2768.30 --> 2769.24]  one-time purchase.
[2769.86 --> 2769.98]  Yeah,
[2770.26 --> 2771.90]  I think we're in agreement there.
[2772.20 --> 2772.80]  Maybe we'll hear
[2772.80 --> 2773.56]  more thoughts from them.
[2773.90 --> 2775.18]  So we are cooking
[2775.18 --> 2776.62]  on the back end.
[2776.80 --> 2778.78]  We are looking at ways
[2778.78 --> 2779.58]  of restructuring
[2779.58 --> 2781.20]  the JB infrastructure
[2781.20 --> 2782.50]  just as it has grown
[2782.50 --> 2784.46]  and that,
[2784.76 --> 2784.94]  of course,
[2784.98 --> 2785.78]  gets more costly
[2785.78 --> 2786.58]  as it grows
[2786.58 --> 2787.52]  and it doesn't necessarily
[2787.52 --> 2788.24]  need to have
[2788.24 --> 2788.98]  as many nodes
[2788.98 --> 2790.76]  and different systems
[2790.76 --> 2791.66]  running what it does
[2791.66 --> 2792.20]  at the moment.
[2792.30 --> 2792.84]  So we've been looking
[2792.84 --> 2793.50]  at kind of ways
[2793.50 --> 2794.22]  to restructure
[2794.22 --> 2796.02]  and when we just look
[2796.02 --> 2796.94]  at the storage amounts
[2796.94 --> 2797.64]  and the kind of compute
[2797.64 --> 2798.24]  required,
[2798.94 --> 2799.36]  it seems like,
[2799.48 --> 2799.58]  Alex,
[2799.66 --> 2800.82]  we kept coming
[2800.82 --> 2802.52]  to maybe we need
[2802.52 --> 2803.26]  to colo
[2803.26 --> 2805.04]  and not use a VPS,
[2805.26 --> 2806.04]  not use AWS,
[2806.36 --> 2807.92]  but go old school
[2807.92 --> 2808.50]  and put something
[2808.50 --> 2809.12]  in a rack.
[2809.42 --> 2809.52]  Yeah,
[2809.58 --> 2810.00]  why not?
[2810.04 --> 2810.66]  What could go wrong
[2810.66 --> 2810.98]  with running
[2810.98 --> 2811.56]  your own hardware,
[2811.72 --> 2811.80]  huh?
[2811.90 --> 2812.10]  Yeah,
[2812.60 --> 2812.90]  I mean,
[2812.90 --> 2813.36]  I don't know,
[2813.44 --> 2814.34]  like I'm kind of
[2814.34 --> 2815.24]  nostalgic about it.
[2815.46 --> 2815.94]  So we're running
[2815.94 --> 2817.02]  a bunch of core services
[2817.02 --> 2817.64]  for the network
[2817.64 --> 2818.32]  on this thing,
[2818.48 --> 2819.60]  potentially the website,
[2819.74 --> 2820.68]  although we might keep
[2820.68 --> 2821.68]  that specifically
[2821.68 --> 2822.44]  on a VPS,
[2822.58 --> 2823.96]  we're not totally sure yet.
[2824.44 --> 2825.40]  But we're talking primarily
[2825.40 --> 2826.20]  about things like
[2826.20 --> 2827.52]  production assets,
[2827.90 --> 2828.04]  you know,
[2828.16 --> 2829.48]  our production next cloud
[2829.48 --> 2830.22]  where we get files
[2830.22 --> 2831.04]  to and from Drew,
[2831.16 --> 2831.68]  our editor,
[2832.42 --> 2833.28]  a bunch of other,
[2833.34 --> 2833.60]  you know,
[2833.86 --> 2834.52]  assets and things
[2834.52 --> 2835.06]  for the network,
[2835.18 --> 2836.14]  but also things
[2836.14 --> 2837.26]  like our matrix server
[2837.26 --> 2837.96]  that takes up
[2837.96 --> 2838.96]  a huge amount
[2838.96 --> 2840.10]  of CPU cycles
[2840.10 --> 2841.44]  on Linode right now
[2841.44 --> 2842.64]  and is on a very
[2842.64 --> 2843.56]  expensive box.
[2843.56 --> 2844.58]  It's just not sustainable
[2844.58 --> 2845.54]  for us to keep it there
[2845.54 --> 2846.44]  really financially.
[2847.68 --> 2848.40]  We've got a few
[2848.40 --> 2849.28]  other services up there
[2849.28 --> 2849.54]  too,
[2849.60 --> 2850.54]  which we may or may
[2850.54 --> 2851.32]  knock on the head.
[2851.40 --> 2851.80]  I don't know if you want
[2851.80 --> 2852.74]  to touch on those at all.
[2853.50 --> 2853.66]  Yeah,
[2853.80 --> 2855.36]  there's just some decisions
[2855.36 --> 2856.28]  we have to make.
[2856.44 --> 2857.06]  I think PeerTube
[2857.06 --> 2858.66]  is probably number one
[2858.66 --> 2859.86]  on the list of possible
[2859.86 --> 2860.50]  things we're going to
[2860.50 --> 2861.40]  roll back for a bit
[2861.40 --> 2862.90]  and maybe look to the
[2862.90 --> 2863.86]  community to host that
[2863.86 --> 2864.28]  or something.
[2865.10 --> 2865.74]  And then there's things
[2865.74 --> 2866.50]  that we also want to
[2866.50 --> 2867.50]  add down the road
[2867.50 --> 2869.02]  that get really costly
[2869.02 --> 2869.66]  in the cloud
[2869.66 --> 2870.52]  and that would be like
[2870.52 --> 2871.44]  GPU accelerated
[2871.44 --> 2872.82]  transcription for the shows.
[2872.82 --> 2873.38]  Yeah,
[2873.48 --> 2874.44]  we do that through
[2874.44 --> 2875.46]  services at the moment
[2875.46 --> 2876.20]  for some of our shows,
[2876.28 --> 2876.92]  but we'd love to start
[2876.92 --> 2877.82]  doing that for everything
[2877.82 --> 2878.40]  in-house.
[2878.68 --> 2879.36]  And then of course
[2879.36 --> 2880.16]  we would have that data
[2880.16 --> 2881.08]  that we could use for
[2881.08 --> 2882.00]  things like the
[2882.00 --> 2884.10]  notes.jupiterbroadcasting.com
[2884.10 --> 2884.68]  site and whatnot.
[2884.82 --> 2885.72]  So we really kind of
[2885.72 --> 2886.56]  want to be able to add
[2886.56 --> 2887.16]  some of that stuff
[2887.16 --> 2887.98]  and that gets crazy
[2887.98 --> 2888.50]  in the cloud.
[2888.88 --> 2889.70]  So it's removable.
[2889.90 --> 2891.00]  It's removing some things
[2891.00 --> 2892.22]  and adding some things.
[2892.64 --> 2893.34]  It also gives us
[2893.34 --> 2894.16]  a bit of a playground.
[2894.36 --> 2895.10]  So I'm considering
[2895.10 --> 2896.08]  trying to convince Chris
[2896.08 --> 2896.56]  that we should put
[2896.56 --> 2897.68]  Proxmox on this thing
[2897.68 --> 2899.18]  just so that we can
[2899.18 --> 2899.80]  have an OS
[2899.80 --> 2900.74]  that we can spin up
[2900.74 --> 2901.38]  virtual machines
[2901.38 --> 2902.32]  and spin them down
[2902.32 --> 2903.10]  and do backups
[2903.10 --> 2903.68]  and, you know,
[2903.72 --> 2904.94]  if we need two migrations
[2904.94 --> 2905.80]  and that kind of thing.
[2906.70 --> 2908.08]  But you, I know,
[2908.16 --> 2908.98]  have a couple of
[2908.98 --> 2910.00]  reservations about
[2910.00 --> 2910.90]  going that route.
[2911.40 --> 2912.38]  Yeah, I suppose.
[2913.28 --> 2914.08]  Although this seems
[2914.08 --> 2915.32]  like the right use case
[2915.32 --> 2916.58]  to be honest with you,
[2916.66 --> 2916.80]  right?
[2916.86 --> 2917.54]  Because before
[2917.54 --> 2918.92]  when I was going
[2918.92 --> 2919.84]  all in on Proxmox
[2919.84 --> 2920.56]  with the servers
[2920.56 --> 2921.22]  here in the studio
[2921.22 --> 2922.64]  and then we got
[2922.64 --> 2923.48]  finally deployed
[2923.48 --> 2923.98]  and I'm like,
[2924.18 --> 2924.68]  oh, this isn't
[2924.68 --> 2925.40]  what I want at all
[2925.40 --> 2925.78]  actually.
[2926.78 --> 2928.18]  That's a different use case.
[2928.96 --> 2929.64]  That's a different
[2929.64 --> 2930.44]  class of system.
[2930.96 --> 2931.54]  Yeah, this is a
[2931.54 --> 2932.60]  shared resource, right?
[2932.66 --> 2933.30]  Where you, me,
[2933.44 --> 2933.98]  Wes, Brent,
[2934.34 --> 2935.04]  maybe a couple of
[2935.04 --> 2935.56]  others will have
[2935.56 --> 2936.32]  access to it.
[2936.86 --> 2937.70]  And if we need to
[2937.70 --> 2938.54]  spin up a specific
[2938.54 --> 2939.66]  distro for the show
[2939.66 --> 2940.24]  and have it in a
[2940.24 --> 2941.00]  remote location
[2941.00 --> 2942.12]  for testing purposes
[2942.12 --> 2942.54]  or whatever
[2942.54 --> 2943.42]  with a different IP,
[2943.90 --> 2944.60]  this will give us
[2944.60 --> 2946.26]  the option to do that.
[2946.96 --> 2947.36]  Yeah, and that's
[2947.36 --> 2947.84]  actually something
[2947.84 --> 2949.10]  that is fairly common
[2949.10 --> 2950.38]  that we'd use a VPS
[2950.38 --> 2951.08]  for in the past.
[2951.46 --> 2951.66]  Yeah.
[2952.12 --> 2952.84]  I also just have
[2952.84 --> 2953.34]  this vision.
[2953.46 --> 2953.88]  You mentioned the
[2953.88 --> 2954.88]  GPU side of things.
[2954.96 --> 2955.50]  I have this vision
[2955.50 --> 2956.86]  of Wes creating
[2956.86 --> 2957.42]  some elaborate
[2957.42 --> 2958.18]  house of cards
[2958.18 --> 2959.50]  where Drew drops
[2959.50 --> 2960.30]  a file into a
[2960.30 --> 2961.06]  specific directory
[2961.06 --> 2961.56]  and the whole
[2961.56 --> 2962.68]  publishing process,
[2962.98 --> 2963.82]  all the encodes,
[2964.26 --> 2965.26]  all the transcriptions
[2965.26 --> 2965.54]  and everything
[2965.54 --> 2966.50]  happens on this box
[2966.50 --> 2966.94]  and then it just
[2966.94 --> 2968.42]  automatically trickles
[2968.42 --> 2969.10]  out to the internet.
[2969.48 --> 2969.92]  I think that's
[2969.92 --> 2970.48]  what ultimately
[2970.48 --> 2971.14]  we'll have to do
[2971.14 --> 2972.10]  because we do that
[2972.10 --> 2973.34]  with a system
[2973.34 --> 2973.70]  that we call
[2973.70 --> 2974.36]  CastaBlaster
[2974.36 --> 2975.58]  on Linode right now
[2975.58 --> 2976.58]  and it's a web form
[2976.58 --> 2977.76]  that Drew uploads to
[2977.76 --> 2979.36]  and then the system
[2979.36 --> 2980.02]  kicks off
[2980.02 --> 2981.34]  and that's the system
[2981.34 --> 2982.04]  that will be extended
[2982.04 --> 2983.22]  to do the transcription
[2983.22 --> 2985.02]  because it's got
[2985.02 --> 2985.48]  the audio
[2985.48 --> 2985.90]  and flax
[2985.90 --> 2986.66]  but more than that
[2986.66 --> 2987.86]  we'll also have
[2987.86 --> 2988.40]  the capabilities
[2988.40 --> 2989.30]  if we want to
[2989.30 --> 2990.64]  where Drew could
[2990.64 --> 2992.08]  upload the individual
[2992.08 --> 2993.14]  stems or individual
[2993.14 --> 2995.26]  tracks of each of us
[2995.26 --> 2995.84]  so it would be
[2995.84 --> 2996.48]  named Chris
[2996.48 --> 2997.06]  this one would be
[2997.06 --> 2997.68]  named Alex
[2997.68 --> 2999.76]  so then the
[2999.76 --> 3000.76]  transcription's aware
[3000.76 --> 3001.82]  of who the individual
[3001.82 --> 3002.28]  host is
[3002.28 --> 3004.22]  but also it's only
[3004.22 --> 3005.16]  that person speaking
[3005.16 --> 3006.18]  so it's much easier
[3006.18 --> 3006.82]  it's much cleaner
[3006.82 --> 3007.60]  for an automated
[3007.60 --> 3008.12]  transcription
[3008.12 --> 3009.36]  and we could only
[3009.36 --> 3010.00]  do that
[3010.00 --> 3011.16]  if it's integrated
[3011.16 --> 3012.14]  into the encoding
[3012.14 --> 3012.58]  pipeline
[3012.58 --> 3013.20]  and so those are
[3013.20 --> 3013.78]  tools that we've
[3013.78 --> 3014.82]  already begun building
[3014.82 --> 3016.14]  in different
[3016.14 --> 3016.88]  phases
[3016.88 --> 3017.78]  and of course
[3017.78 --> 3018.44]  the cast of last
[3018.44 --> 3019.26]  encoding pipelines
[3019.26 --> 3020.20]  existed for years
[3020.20 --> 3020.42]  now
[3020.42 --> 3022.20]  and we just have
[3022.20 --> 3022.78]  kind of a powerful
[3022.78 --> 3023.56]  box on Linode
[3023.56 --> 3024.08]  that does that
[3024.08 --> 3024.56]  crunching
[3024.56 --> 3025.66]  but you know
[3025.66 --> 3026.86]  we're not talking
[3026.86 --> 3027.80]  like major stuff
[3027.80 --> 3027.92]  here
[3027.92 --> 3028.72]  it's totally doable
[3028.72 --> 3029.56]  on a colo box
[3029.56 --> 3030.56]  yeah we're talking
[3030.56 --> 3031.18]  about the difference
[3031.18 --> 3032.08]  here between a
[3032.08 --> 3034.00]  VPS to CPU rig
[3034.00 --> 3035.64]  and the Xeon
[3035.64 --> 3037.38]  Silver 4214
[3037.38 --> 3038.26]  that's in the
[3038.26 --> 3039.64]  server that we're
[3039.64 --> 3040.30]  going to put into
[3040.30 --> 3041.66]  the colo near
[3041.66 --> 3042.82]  Toronto in Canada
[3042.82 --> 3044.02]  now I was going
[3044.02 --> 3044.58]  to offer up
[3044.58 --> 3045.14]  the audience
[3045.14 --> 3045.96]  to boost in
[3045.96 --> 3046.84]  and give us
[3046.84 --> 3047.42]  some naming
[3047.42 --> 3048.42]  suggestions for
[3048.42 --> 3048.94]  this server
[3048.94 --> 3049.78]  at the risk
[3049.78 --> 3050.50]  of ending up
[3050.50 --> 3050.98]  with a server
[3050.98 --> 3051.48]  name like
[3051.48 --> 3052.54]  server McServer
[3052.54 --> 3052.92]  face
[3052.92 --> 3053.26]  you know
[3053.26 --> 3053.90]  like Boaty
[3053.90 --> 3054.74]  McBoat face
[3054.74 --> 3055.58]  do we get to
[3055.58 --> 3057.22]  do we get to
[3057.22 --> 3058.10]  like veto
[3058.10 --> 3058.76]  any of them
[3058.76 --> 3060.40]  it's your
[3060.40 --> 3061.42]  network dude
[3061.42 --> 3062.28]  you make the
[3062.28 --> 3062.68]  rules
[3062.68 --> 3063.84]  I guess it depends
[3063.84 --> 3064.20]  on how big
[3064.20 --> 3064.82]  the boost is
[3064.82 --> 3066.12]  right
[3066.12 --> 3066.60]  yeah
[3066.60 --> 3067.20]  yeah
[3067.20 --> 3068.10]  so I think
[3068.10 --> 3068.52]  we'll do the
[3068.52 --> 3069.26]  Proxmox thing
[3069.26 --> 3069.68]  I think you're
[3069.68 --> 3070.04]  right I think
[3070.04 --> 3070.48]  it's the right
[3070.48 --> 3070.98]  use case
[3070.98 --> 3071.44]  it does make
[3071.44 --> 3071.82]  me a little
[3071.82 --> 3072.12]  nervous
[3072.12 --> 3072.54]  but you know
[3072.54 --> 3073.26]  honestly I just
[3073.26 --> 3074.22]  bet most of
[3074.22 --> 3074.72]  the VMs I'm going
[3074.72 --> 3075.10]  to spin up are
[3075.10 --> 3075.46]  just going to be
[3075.46 --> 3075.88]  Nick's ones
[3075.88 --> 3076.26]  and that'll be
[3076.26 --> 3077.24]  fine and that'll
[3077.24 --> 3077.78]  work we'll still
[3077.78 --> 3078.18]  get it done
[3078.18 --> 3078.62]  exactly
[3078.62 --> 3079.30]  and I think
[3079.30 --> 3079.82]  then we'll have
[3079.82 --> 3080.16]  some of that
[3080.16 --> 3080.88]  optionality to
[3080.88 --> 3081.70]  move VMs around
[3081.70 --> 3082.12]  if we need
[3082.12 --> 3082.42]  we'll have some
[3082.42 --> 3082.92]  of that DR
[3082.92 --> 3084.36]  stuff and we'll
[3084.36 --> 3084.90]  also have a
[3084.90 --> 3085.50]  common interface
[3085.50 --> 3086.44]  where any one
[3086.44 --> 3087.08]  of us can log
[3087.08 --> 3087.70]  in and look at
[3087.70 --> 3088.44]  systems and status
[3088.44 --> 3089.06]  and spin up
[3089.06 --> 3089.56]  and spin down
[3089.56 --> 3090.46]  so it's going to
[3090.46 --> 3091.06]  be a good thing
[3091.06 --> 3092.00]  and I'm going to
[3092.00 --> 3092.66]  be totally happy
[3092.66 --> 3093.22]  and I'm not going
[3093.22 --> 3093.78]  to complain at
[3093.78 --> 3094.36]  all about it
[3094.36 --> 3095.38]  press X to
[3095.38 --> 3102.00]  go try it out
[3102.00 --> 3102.62]  right now for
[3102.62 --> 3103.34]  up to 100
[3103.34 --> 3104.16]  devices and
[3104.16 --> 3105.12]  three users for
[3105.12 --> 3105.70]  free while you
[3105.70 --> 3106.42]  support the show
[3106.42 --> 3108.24]  at tailscale.com
[3108.24 --> 3109.60]  slash self
[3109.60 --> 3110.70]  hosted that's not
[3110.70 --> 3111.32]  a limited time
[3111.32 --> 3111.86]  deal either it's
[3111.86 --> 3112.58]  the plan I'm still
[3112.58 --> 3113.78]  on also something
[3113.78 --> 3114.52]  that the enterprises
[3114.52 --> 3116.00]  can try everyone
[3116.00 --> 3116.72]  these days is
[3116.72 --> 3117.48]  played around with
[3117.48 --> 3118.20]  some kind of VPN
[3118.20 --> 3119.04]  I swear every
[3119.04 --> 3120.12]  content creator has
[3120.12 --> 3121.18]  a VPN sponsor
[3121.18 --> 3122.38]  tailscale isn't
[3122.38 --> 3123.60]  like those it's
[3123.60 --> 3124.24]  not about hiding
[3124.24 --> 3124.76]  your browsing
[3124.76 --> 3125.36]  habits from a
[3125.36 --> 3126.20]  coffee shop owner
[3126.20 --> 3127.60]  or watching Netflix
[3127.60 --> 3128.16]  from some other
[3128.16 --> 3128.78]  location although
[3128.78 --> 3129.36]  you could kind of
[3129.36 --> 3129.82]  pull that off
[3129.82 --> 3130.88]  with tailscale it's
[3130.88 --> 3132.08]  really a VPN for
[3132.08 --> 3132.68]  connecting your
[3132.68 --> 3133.56]  devices to each
[3133.56 --> 3134.20]  other directly
[3134.20 --> 3135.64]  securely it's
[3135.64 --> 3136.32]  great for self
[3136.32 --> 3136.80]  hosters and
[3136.80 --> 3137.54]  home labbers it's
[3137.54 --> 3138.34]  great for companies
[3138.34 --> 3139.02]  because it gives
[3139.02 --> 3139.90]  you secure remote
[3139.90 --> 3140.90]  access to
[3140.90 --> 3141.84]  production to
[3141.84 --> 3143.08]  your databases to
[3143.08 --> 3144.02]  your servers to
[3144.02 --> 3144.48]  your Kubernetes
[3144.48 --> 3145.84]  cluster whatever it
[3145.84 --> 3146.66]  might be and it's
[3146.66 --> 3148.28]  fast really really
[3148.28 --> 3148.94]  fast you get
[3148.94 --> 3149.98]  privacy for everyone
[3149.98 --> 3151.52]  and every organization
[3151.52 --> 3152.86]  your devices show up
[3152.86 --> 3154.36]  on a flat mesh
[3154.36 --> 3154.90]  network protected
[3155.36 --> 3156.14]  by the noise
[3156.14 --> 3156.78]  protocol and
[3156.78 --> 3157.88]  wire guard and
[3157.88 --> 3158.48]  you can build a
[3158.48 --> 3159.18]  simple network
[3159.18 --> 3160.08]  across complex
[3160.08 --> 3161.62]  infrastructure bridge
[3161.62 --> 3162.90]  multiple different
[3162.90 --> 3164.06]  data centers or
[3164.06 --> 3165.04]  connect from home
[3165.04 --> 3165.90]  back to your work
[3165.90 --> 3167.40]  machines I put in
[3167.40 --> 3169.08]  my VMs I add I
[3169.08 --> 3169.80]  add it to all of my
[3169.80 --> 3170.52]  Docker container
[3170.52 --> 3171.16]  setups too so that
[3171.16 --> 3171.70]  way my Docker
[3171.70 --> 3172.28]  containers go
[3172.28 --> 3173.38]  directly onto my
[3173.38 --> 3174.68]  tail net and you
[3174.68 --> 3175.80]  can authenticate using
[3175.80 --> 3176.70]  tailscale app
[3176.70 --> 3177.90]  connectors so you can
[3177.90 --> 3178.24]  actually have
[3178.24 --> 3179.14]  applications that can
[3179.14 --> 3180.80]  authenticate to your
[3180.80 --> 3181.68]  tail net I do this
[3181.68 --> 3182.66]  actually with my SSH
[3182.66 --> 3184.16]  connections every SSH
[3184.16 --> 3184.94]  connection is actually
[3184.94 --> 3186.28]  authenticated by my
[3186.28 --> 3187.70]  tail net and it is
[3187.70 --> 3188.62]  really great because I
[3188.62 --> 3189.38]  can use all machine
[3189.38 --> 3190.20]  names I don't have to
[3190.20 --> 3191.92]  move keys around so go
[3191.92 --> 3192.96]  try it out personal
[3192.96 --> 3193.80]  plans always going to
[3193.80 --> 3194.90]  be free you can get it
[3194.90 --> 3196.76]  for 100 devices three
[3196.76 --> 3198.34]  users try it out no
[3198.34 --> 3199.66]  credit card required and
[3199.66 --> 3200.44]  you can support the
[3200.44 --> 3201.36]  show when you go to
[3201.36 --> 3203.04]  tailscale.com slash
[3203.04 --> 3204.70]  self hosted of course
[3204.70 --> 3205.42]  you could try it and if
[3205.42 --> 3206.10]  you want to recommend it
[3206.10 --> 3207.36]  at work to absolutely
[3207.36 --> 3208.90]  go to tailscale.com slash
[3208.90 --> 3209.68]  self hosted to get
[3209.68 --> 3211.36]  started 100 devices and
[3211.36 --> 3212.52]  three users for free
[3212.52 --> 3214.56]  forever that seems like
[3214.56 --> 3216.08]  a pretty good deal I
[3216.08 --> 3217.20]  love it no inbound
[3217.20 --> 3218.06]  ports on any of my
[3218.06 --> 3219.14]  firewalls you're gonna
[3219.14 --> 3220.42]  love it tailscale.com
[3220.42 --> 3224.10]  slash self hosted we got
[3224.10 --> 3225.34]  some boost into the show
[3225.34 --> 3226.64]  this week and Jordan
[3226.64 --> 3229.68]  Bravo comes in with 6,969
[3230.32 --> 3232.70]  sats he says I'm excited
[3232.70 --> 3233.94]  to try image on my home
[3233.94 --> 3234.84]  server once it's available
[3234.84 --> 3236.52]  on Nix OS on a slightly
[3236.52 --> 3237.82]  different topic I'd like to
[3237.82 --> 3239.34]  put Nix OS on my cloud
[3239.34 --> 3241.64]  VPS which currently uses
[3241.64 --> 3243.06]  Ubuntu does anyone have
[3243.06 --> 3244.14]  experience with this I've
[3244.14 --> 3245.10]  eyeballed the docs for
[3245.10 --> 3246.80]  Nix OS anywhere but I'm
[3246.80 --> 3248.02]  not sure where the best
[3248.02 --> 3249.90]  place to start is well
[3249.90 --> 3251.22]  Jordan I'll put a link in
[3251.22 --> 3252.40]  the show notes for you our
[3252.40 --> 3254.06]  good friend Wes over on
[3254.06 --> 3255.22]  Linux Unplugged gave a
[3255.22 --> 3256.38]  talk at this year's Linux
[3256.38 --> 3258.18]  Fest Northwest talking
[3258.18 --> 3259.52]  about deploying Nix OS
[3259.52 --> 3261.94]  literally anywhere and in
[3261.94 --> 3262.82]  this video which will be
[3262.82 --> 3263.82]  linked in the show notes he
[3263.82 --> 3264.94]  gave an exploration of
[3264.94 --> 3266.04]  booting and installing
[3266.04 --> 3268.70]  Nix OS there are also some
[3268.70 --> 3269.68]  other projects you might
[3269.68 --> 3271.20]  find useful one of them is
[3271.20 --> 3274.18]  called Nix Infect yes
[3274.18 --> 3276.56]  right yeah that is Nix OS
[3276.56 --> 3278.00]  anywhere and Nix Infect
[3278.00 --> 3280.46]  both really great it's so fun
[3280.46 --> 3282.70]  to take over a VPS do
[3282.70 --> 3284.70]  recommend Gene Bean came in
[3284.70 --> 3287.06]  with 8,888 sats he sent us
[3287.06 --> 3288.22]  a few boosts but for time I'm
[3288.22 --> 3289.54]  just going to get to one here
[3289.54 --> 3291.60]  and he says I migrated to
[3291.60 --> 3293.36]  the Nix module base next cloud
[3293.36 --> 3294.70]  with a few tweaks from y'all
[3294.70 --> 3296.10]  and other places and I'm quite
[3296.10 --> 3297.70]  happy with it that's our
[3297.70 --> 3298.60]  third or fourth boost from
[3298.60 --> 3299.62]  somebody that switched to
[3299.62 --> 3301.16]  the Nix module for next cloud
[3301.16 --> 3302.56]  seems like it's working for
[3302.56 --> 3304.76]  folks makes me want to redo
[3304.76 --> 3306.04]  it on my home system really
[3306.04 --> 3307.26]  bad except for it's just all
[3307.26 --> 3309.26]  working so well right now it's
[3309.26 --> 3312.12]  in the Docker container and it's
[3312.12 --> 3313.16]  I mean it could be a little
[3313.16 --> 3315.56]  faster for sure but you know
[3315.56 --> 3317.76]  it's not broke it's one of the
[3317.76 --> 3319.10]  few apps that I think almost
[3319.10 --> 3320.18]  everybody that's into self
[3320.18 --> 3322.12]  hosting actually hosts I think
[3322.12 --> 3323.10]  there's probably a handful of
[3323.10 --> 3324.78]  things like Plex or Jellyfin or
[3324.78 --> 3326.26]  some kind of media server
[3326.26 --> 3328.28]  another one would be next cloud
[3328.28 --> 3328.98]  I'm trying to think of
[3328.98 --> 3329.80]  anything else that's going to
[3329.80 --> 3331.20]  be quite as universal as those
[3331.20 --> 3332.92]  two I'm having a hard time
[3332.92 --> 3334.64]  yeah it's got to be yeah
[3334.64 --> 3337.32]  rare the rington comes in with
[3337.32 --> 3338.88]  5,000 sats I got a question for
[3338.88 --> 3340.46]  Chris in graphene west do you
[3340.46 --> 3341.84]  have the sandbox Google play
[3341.84 --> 3343.00]  services set up on the same
[3343.00 --> 3344.24]  profile as all your other apps
[3344.24 --> 3345.46]  or a separate profile and if it's
[3345.46 --> 3346.56]  a separate profile how do you
[3346.56 --> 3348.34]  get notifications and other
[3348.34 --> 3352.06]  profiles to work I do not I'm a
[3352.06 --> 3355.26]  bad security boy and I just have
[3355.26 --> 3357.60]  the play sandboxed as my regular
[3357.60 --> 3359.44]  user we need the Wilhelm scream
[3359.44 --> 3362.04]  at this point please I don't do a
[3362.04 --> 3363.16]  lot of apps for the play store I
[3363.16 --> 3364.96]  only do a like the ones like
[3364.96 --> 3366.26]  banking or something or Google
[3366.26 --> 3368.92]  Maps but F droid and obtainium are
[3368.92 --> 3371.06]  my other go-tos for that what was
[3371.06 --> 3372.16]  the name of the OS by the way it
[3372.16 --> 3374.92]  was a giraffe in a giraffe in OS I
[3374.92 --> 3376.62]  think yeah yeah that's what you said
[3376.62 --> 3378.52]  I've been enjoying it I've been
[3378.52 --> 3379.74]  enjoying it and thanks to our buddy
[3379.74 --> 3381.56]  Brent I got the Garmin watch
[3381.56 --> 3384.28]  and I so now I've got a watch
[3384.28 --> 3386.04]  that isn't the Apple watch but it
[3386.04 --> 3387.56]  does payments because you can't do
[3387.56 --> 3389.84]  like Google pay tap to pay with
[3389.84 --> 3391.26]  graphene OS but you can with the
[3391.26 --> 3393.98]  Garmin watch pew pew pew so that's
[3393.98 --> 3397.48]  great Bronson wig has a alternative
[3397.48 --> 3399.84]  option for blue bubbles users that's
[3399.84 --> 3401.78]  the service I've been using on an old
[3401.78 --> 3404.32]  Mac laptop to get iMessage on Android
[3404.32 --> 3407.02]  and they wanted me to know about
[3407.02 --> 3410.10]  Docker OS 10 it's a Mac VM in a
[3410.10 --> 3413.44]  Docker container it supposedly works and
[3413.44 --> 3414.52]  there might be some risk your Apple
[3414.52 --> 3416.32]  IDs who use it your own risk I looked
[3416.32 --> 3418.20]  at this I gotta check this out more
[3418.20 --> 3421.72]  it's so cool that is so cool I had
[3421.72 --> 3423.44]  never I should have known that people
[3423.44 --> 3424.64]  are there's a container there's a
[3424.64 --> 3427.26]  Docker container for Mac OS this is
[3427.26 --> 3429.52]  Jeff Goldblum speaking they they
[3429.52 --> 3430.78]  didn't they were so obsessed with
[3430.78 --> 3432.64]  whether they could they didn't stop to
[3432.64 --> 3434.88]  think with whether they should yeah I
[3434.88 --> 3436.16]  mean I love the idea of putting this
[3436.16 --> 3437.24]  on a server and just running it
[3437.24 --> 3439.50]  headless maybe even a VPS to be honest
[3439.50 --> 3441.00]  with you and just have it running
[3441.00 --> 3442.66]  blue bubbles headless and I could
[3442.66 --> 3445.00]  VNC into it when it set it up and
[3445.00 --> 3446.54]  then just let that run forever he
[3446.54 --> 3448.80]  sent a vehicle recommendation for
[3448.80 --> 3450.24]  Brentley you think we should pass it on
[3450.24 --> 3453.54]  to him yeah what did he send a Toyota
[3453.54 --> 3457.86]  Tundra 2017 no smarts reliable V8 so
[3457.86 --> 3460.14]  that sounds nice yeah the only the
[3460.14 --> 3461.76]  only bad thing I hear about those sort
[3461.76 --> 3463.46]  of slightly older Tundras is they're a
[3463.46 --> 3465.24]  little bit thirsty but other than that
[3465.24 --> 3467.46]  very reliable they also got a Garmin
[3467.46 --> 3471.34]  because of Brent that's great all
[3471.34 --> 3473.62]  right our last boost around us out
[3473.62 --> 3476.92]  comes from Iraq with 4400 sats for
[3476.92 --> 3478.66]  email alerts he's been using Amazon
[3478.66 --> 3480.76]  SES since he doesn't want to have to
[3480.76 --> 3483.02]  mess with an SMTP server and and then
[3483.02 --> 3484.12]  he answered a couple of your questions
[3484.12 --> 3486.32]  Alex he says I incorporate nifty
[3486.32 --> 3490.26]  NTF wire notify with uptime kuma to
[3490.26 --> 3492.40]  set different urgencies part of my
[3492.40 --> 3495.50]  reason to use notify or NTF Y is its
[3495.50 --> 3497.38]  unified push capability for apps like
[3497.38 --> 3501.62]  most it on element squid'll cast to run
[3501.62 --> 3505.24]  its own notifications huh those aren't
[3505.24 --> 3507.38]  real application names are they how is
[3507.38 --> 3509.56]  moshy don it's got to be a master on
[3509.56 --> 3512.22]  client right moshy don for master's on
[3512.22 --> 3515.00]  yeah there you go and shlitty shlitty
[3515.00 --> 3517.76]  chat yeah shlitty chat feature rich
[3517.76 --> 3520.44]  messenger for matrix there you go oh I
[3520.44 --> 3521.96]  all right I'll check that out that's
[3521.96 --> 3525.30]  that rings my bell sweet yeah that's
[3525.30 --> 3526.60]  nice that it all works with notify and
[3526.60 --> 3528.24]  that you can have different urgencies
[3528.24 --> 3529.90]  okay and the topic of game servers to
[3529.90 --> 3532.08]  round us out I'm running the unofficial
[3532.08 --> 3534.66]  docker packaged version of amp with the
[3534.66 --> 3536.42]  advanced license I got for the lulls a
[3536.42 --> 3538.72]  while back for land game streaming Alex
[3538.72 --> 3540.80]  I stream from my windows maybe bad
[3540.80 --> 3543.40]  light soon desktop using sunshine on the
[3543.40 --> 3545.90]  tower as the server and then moonlight as
[3545.90 --> 3547.44]  the client everywhere else it works
[3547.44 --> 3550.00]  enough but has some quirks getting things
[3550.00 --> 3551.90]  configured correctly to end sessions when
[3551.90 --> 3553.56]  quitting a game I ended up having some
[3553.56 --> 3555.30]  issues with bazite this week which led
[3555.30 --> 3558.80]  me to replacing it with windows this is
[3558.80 --> 3562.88]  another Wilhelm scream moment a couple of
[3562.88 --> 3564.96]  things conspired against me one of them
[3564.96 --> 3569.72]  is that the rx for the rx 560 that was in
[3569.72 --> 3571.82]  there is so old it was having some issues
[3571.82 --> 3575.56]  with game stream or something whatever the
[3575.56 --> 3577.40]  name of the game scope I think is what it
[3577.40 --> 3579.70]  is yeah and it wasn't booting into steam
[3579.70 --> 3581.34]  as you recall in the last episode I
[3581.34 --> 3582.32]  talked about having to enter my
[3582.32 --> 3584.68]  credentials every time a couple of guys
[3584.68 --> 3587.26]  on discord jumped in team linux was one
[3587.26 --> 3588.82]  of them and sort of helped me with some of
[3588.82 --> 3590.56]  the things that were going wrong and it
[3590.56 --> 3593.66]  turns out the the graphics card drivers
[3593.66 --> 3597.32]  don't support that new version so I bought
[3597.32 --> 3602.90]  myself an rx 6800 xt or 6700 xt I can't
[3602.90 --> 3605.20]  remember the model number about 250 bucks
[3605.20 --> 3609.90]  off of ebay and that resolved a lot of my
[3609.90 --> 3611.90]  issues I could run red dead redemption 2
[3611.90 --> 3614.78]  at 1080p at 60fps which was my benchmark
[3614.78 --> 3617.82]  for performance at just fine all day long
[3617.82 --> 3622.46]  but there were the real issue came when it
[3622.46 --> 3624.78]  went to sleep overnight or something and
[3624.78 --> 3626.88]  then the resolution after it came back from
[3626.88 --> 3629.54]  sleep set itself to 4k and so everything
[3629.54 --> 3632.42]  was absolutely tiny and then the final nail
[3632.42 --> 3634.30]  in the coffin besides the fact the audio
[3634.30 --> 3636.80]  device reset itself to the default audio
[3636.80 --> 3638.92]  device instead of HDMI audio every time
[3638.92 --> 3642.30]  the final nail in the coffin was that one
[3642.30 --> 3644.52]  morning my wife and I had a few minutes
[3644.52 --> 3646.24]  before we dropped out of school before
[3646.24 --> 3647.60]  work and we're like right let's play some
[3647.60 --> 3649.40]  we've been playing a lot of overcooked 2
[3649.40 --> 3652.68]  lately and I just couldn't get it to come
[3652.68 --> 3655.42]  out of 680 by 480 no matter what I did I
[3655.42 --> 3657.62]  disconnected the HDMI I reconnected it I
[3657.62 --> 3660.92]  rebooted the server the gaming box I
[3660.92 --> 3662.88]  turned it off like fully and unplugged it
[3662.88 --> 3664.50]  and tried to reset any I don't know
[3664.50 --> 3667.62]  nv ram that was persisting rebooted the
[3667.62 --> 3670.40]  tv even as well as the avr like everything
[3670.40 --> 3673.64]  in that stack and it was just locked at 680
[3673.64 --> 3676.50]  by 480 no matter what I did I even tried
[3676.50 --> 3678.08]  two or three different versions of bazite
[3678.08 --> 3679.64]  rolling back to different versions and what
[3679.64 --> 3681.56]  have you and in the end I just want this
[3681.56 --> 3683.68]  to be a set it and forget it you know
[3683.68 --> 3686.22]  stupid simple gaming box so I yeah we're
[3686.22 --> 3689.28]  back to windows absolutely understand I
[3689.28 --> 3691.54]  can tell you that with the steam deck
[3691.54 --> 3694.52]  I've experienced the toggling to 4k after
[3694.52 --> 3697.28]  sleep and always choosing the HDMI audio
[3697.28 --> 3699.96]  issues as well and having to disrupt that
[3699.96 --> 3701.60]  hey we got a couple of minutes let's sit
[3701.60 --> 3704.44]  down and play a video game and it happened
[3704.44 --> 3707.14]  enough that I after about a year of using
[3707.14 --> 3709.34]  it I disconnected my steam deck from the
[3709.34 --> 3710.78]  television and hooked the Nintendo switch
[3710.78 --> 3714.22]  back up I think in time bazite is going
[3714.22 --> 3716.12]  to be good enough but I mean ultimately
[3716.12 --> 3717.98]  there are just some issues that you can't
[3717.98 --> 3722.48]  overcome without some upstream stuff you
[3722.48 --> 3724.76]  know anti anti cheat is the one that comes
[3724.76 --> 3727.54]  to mind yes first of all yeah yeah you can
[3727.54 --> 3729.18]  solve a lot of performance issues with
[3729.18 --> 3731.38]  moonlight and sunlight and that sunshine and
[3731.38 --> 3734.12]  that kind of thing but my gaming desktop is
[3734.12 --> 3737.46]  connected to I think the aspect ratio is
[3737.46 --> 3740.06]  something like 64 by 7 or something stupid
[3740.06 --> 3742.82]  it's it's one of these ultra wide monitors
[3742.82 --> 3746.86]  but it's 5k 2k monitor it's a Dell 40 inch
[3746.86 --> 3748.52]  something I don't remember the model number
[3748.52 --> 3752.22]  but when I but when I try and do game stream
[3752.22 --> 3755.56]  from this computer to a 4k 16 by 9 aspect
[3755.56 --> 3760.42]  ratio TV it just it never works properly so
[3760.42 --> 3764.10]  okay yeah yeah I flirt with the idea of putting
[3764.10 --> 3766.00]  the graphics card actually in a server and
[3766.00 --> 3769.66]  virtualizing it of course but you know that
[3769.66 --> 3771.46]  kind of gets away from the I've got five
[3771.46 --> 3773.76]  minutes I just play a few games this is how
[3773.76 --> 3776.02]  you end up with a Nintendo switch yeah I
[3776.02 --> 3779.00]  just want to say super quickly that using
[3779.00 --> 3782.10]  the switch did show me like oh I do miss
[3782.10 --> 3784.40]  the openness of the steam deck like not
[3784.40 --> 3785.96]  being able to use any controller I want and
[3785.96 --> 3787.70]  a few other things so there's a lot of
[3787.70 --> 3788.98]  nice things about the steam deck too it's
[3788.98 --> 3791.90]  not all bad shout out to to VT52 who
[3791.90 --> 3794.70]  suggested send grid and a row of ducks
[3794.70 --> 3797.10]  from caveman f16 suggesting that he uses
[3797.10 --> 3798.78]  his proton mail account that works well
[3798.78 --> 3802.16]  and fire glow center firely go sent us a
[3802.16 --> 3804.66]  1000 sat boost as a first-time booster so
[3804.66 --> 3808.58]  we had 13 boosters total we stacked 43,146
[3808.58 --> 3810.06]  sets not our best show but we had some
[3810.06 --> 3811.36]  great messages in there in fact there's
[3811.36 --> 3813.34]  even more boosts we can't fit them all in
[3813.34 --> 3815.84]  for time but we link to the boost barn where
[3815.84 --> 3817.28]  you can read those that didn't make it onto
[3817.28 --> 3818.94]  the air and we keep them in our show notes
[3818.94 --> 3821.42]  as well now if you'd like to jump in it's
[3821.42 --> 3823.08]  never been easier with fountain and
[3823.08 --> 3824.30]  strikes strikes now available in more
[3824.30 --> 3826.02]  than 100 countries including just
[3826.02 --> 3827.98]  recently the UK you can integrate it
[3827.98 --> 3829.88]  with fountain FM you don't have to hold
[3829.88 --> 3831.64]  sats you don't have to like be a
[3831.64 --> 3833.88]  bitcoiner you just connect it all up
[3833.88 --> 3835.76]  fund the wallet and boost the show with
[3835.76 --> 3837.20]  a message it's a great way to support
[3837.20 --> 3838.92]  the show but not only us it supports the
[3838.92 --> 3841.10]  developers who create the apps they get
[3841.10 --> 3843.12]  a percentage and a small percentage goes
[3843.12 --> 3844.88]  to the index to keep that alive to keep
[3844.88 --> 3847.00]  everything going without having to load
[3847.00 --> 3848.94]  it up with ads or corporate sponsors or
[3848.94 --> 3850.78]  whatever it might be like subscription
[3850.78 --> 3852.70]  plans it's a really slick system you're
[3852.70 --> 3855.32]  supporting us here at the network and of
[3855.32 --> 3856.42]  course the people that create the apps
[3856.42 --> 3858.10]  and it's a great way to get your message
[3858.10 --> 3860.06]  on here podcast apps dot com and
[3860.06 --> 3862.04]  fountain dot FM for that now if you'd
[3862.04 --> 3863.60]  like to support us a bit more directly
[3863.60 --> 3865.98]  you can go to self hosted dot show slash
[3865.98 --> 3869.30]  sre to get an ad free feed with a post
[3869.30 --> 3870.66]  show and I believe today we're going to
[3870.66 --> 3872.56]  be talking a great deal about the latest
[3872.56 --> 3875.30]  home assistant release it's hard to it's
[3875.30 --> 3877.12]  hard to bite my tongue but we're going to
[3877.12 --> 3879.56]  save it for the members we had some
[3879.56 --> 3881.14]  meetups coming up in fact Brent has one
[3881.14 --> 3882.92]  coming up in a few weeks those are at
[3882.92 --> 3884.62]  meetup dot com slash Jupiter broadcasting
[3884.62 --> 3886.76]  we just had one in Spokane shout out to
[3886.76 --> 3888.80]  the self hosted listeners who made it
[3888.80 --> 3890.62]  for that meetup it was hot and I was
[3890.62 --> 3892.08]  impressed how many people still showed
[3892.08 --> 3893.24]  up even though it was like a hundred
[3893.24 --> 3895.10]  degrees outside maybe it's because they
[3895.10 --> 3896.74]  knew the venue had air conditioning but
[3896.74 --> 3898.06]  it was nice to see you all and tip of
[3898.06 --> 3899.82]  the hat to those out there that listen
[3899.82 --> 3901.34]  to the self hosted pod if you want to
[3901.34 --> 3902.66]  find more of me on the internet you can
[3902.66 --> 3905.16]  go to alex dot katie's end dot me come
[3905.16 --> 3906.94]  hang out in the Nostra universe it's
[3906.94 --> 3909.48]  weird chris las dot com thanks
[3909.48 --> 3910.40]  for listening everyone that was
[3910.40 --> 3912.80]  self hosted dot show slash one two eight
[3912.80 --> 3914.54]  you
[3914.54 --> 3916.54]  you
[3916.54 --> 3918.54]  you
[3918.54 --> 3920.54]  you
[3920.54 --> 3922.54]  you
[3922.54 --> 3924.54]  you
[3924.54 --> 3926.54]  you
[3926.54 --> 3928.54]  you
[3928.54 --> 3930.54]  you
[3930.54 --> 3932.54]  you
[3932.54 --> 3934.54]  you
[3934.54 --> 3936.54]  you
[3936.54 --> 3938.54]  you
