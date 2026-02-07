[0.00 --> 3.96]  I think we have something like 70 people signed up for the East Coast meetup so far.
[5.18 --> 6.14]  69, baby.
[6.64 --> 6.98]  Nice.
[7.72 --> 11.62]  You know it's going to go up from there, too, because it always kind of goes up a few ticks in the last day.
[12.16 --> 15.98]  Now, the question that I have, is this barbecue place going to have enough meat?
[16.62 --> 19.74]  Well, I've been emailing them back and forth, and it's a little bit complicated.
[19.96 --> 23.68]  We don't want to have to charge everybody tickets and admission and that kind of thing.
[24.08 --> 28.98]  But, you know, a barbecue restaurant, they make a certain amount of food in the morning, well, the night before.
[28.98 --> 31.24]  And once it's gone, it's gone.
[31.58 --> 35.88]  So there are a couple of things that we can do to help kind of mitigate that.
[36.28 --> 37.82]  You can preorder on the website.
[38.24 --> 46.18]  So, you know, when you turn up to the spot, you can walk into the restaurant and they'll sort of carve your food while you wait in there without waiting in the normal line.
[46.98 --> 56.30]  The other thing that we were thinking about doing, but we're not sure of the logistics and how it would work, is giving them numbers beforehand so that we can actually make sure there's enough meat for everybody.
[56.48 --> 58.88]  Well, the way that would work is if people sign up on the meetup page.
[59.60 --> 59.70]  Yeah.
[59.76 --> 65.40]  So it is critical if you are coming, please make sure you sign up on the meetup page so we have a really accurate idea of numbers.
[65.56 --> 68.84]  And equally, if you aren't able to make it, please unsubscribe.
[69.22 --> 70.94]  Please say, no, you're not coming anymore.
[71.00 --> 71.96]  That's really important, too.
[72.62 --> 74.34]  I love that we're running into this problem.
[75.30 --> 77.26]  And this is just a great problem to have.
[77.36 --> 80.38]  We are thrilled to have this problem and we want it to be an even bigger problem.
[80.52 --> 88.86]  So if you can come hang out with us on April 9th in Raleigh, North Carolina, we have all the details at meetup.com slash Jupiter Broadcasting.
[88.86 --> 91.88]  and don't worry, we're going to bring some snacks too.
[92.82 --> 94.48]  And they're not going to be meat snacks.
[94.62 --> 97.20]  If you're not a meat eater, there will be something for you.
[97.66 --> 99.00]  Yeah, well, I think we're bringing Brent with us,
[99.04 --> 100.56]  so we've at least got to take care of him, right?
[101.18 --> 103.52]  Right, he'll be our vegan advocate, you know.
[103.66 --> 105.42]  He always stands up for the non-meat eaters
[105.42 --> 107.44]  because he's about the only one in our crowd.
[109.26 --> 112.26]  So I was browsing the old Hacker News the other day
[112.26 --> 114.94]  and I came across a Docker.com blog post
[114.94 --> 119.36]  about a speed boost achievement for Docker Desktop in 4.6.
[119.82 --> 121.40]  This is a fascinating story, Alex.
[121.90 --> 122.82]  Yeah, I think so too.
[122.98 --> 124.76]  And the performance of Docker Desktop,
[124.98 --> 128.68]  particularly on the M1 Silicon, Apple Silicon Macs,
[128.68 --> 134.58]  has been bad enough that I have literally stopped using Docker on my Mac
[134.58 --> 137.74]  and I just SSH into a server and use it there
[137.74 --> 139.20]  and do all my builds on a remote server.
[140.26 --> 140.34]  Yeah.
[141.18 --> 141.56]  Oof.
[141.78 --> 143.94]  Okay, so, you know, we're going to talk today
[143.94 --> 146.02]  about how I'm looking at ditching containers,
[146.02 --> 149.32]  so we thought we should probably have a little bit of container good news.
[150.18 --> 153.20]  And this is a neat little happenstance.
[153.20 --> 156.90]  There was a discovery by the Asahi Linux team,
[157.00 --> 160.64]  Hector Martin, who's trying to port Linux to the M1,
[161.46 --> 165.94]  discovered that Apple's NVMe drivers are really, really great
[165.94 --> 169.90]  except for a particular function called the fsync.
[169.90 --> 173.34]  And depending on how this is called and when it's called,
[173.80 --> 177.20]  it's horribly slow on macOS.
[178.06 --> 181.14]  So Hector discovered that, talked about it publicly.
[181.82 --> 184.84]  They've submitted code upstream to Linux kernel to solve it on Linux,
[185.06 --> 187.26]  but it isn't necessarily solved on the Mac.
[187.96 --> 190.22]  And so a Docker user noticed this.
[190.22 --> 192.20]  We'll have a link to the GitHub issue and said,
[192.28 --> 194.66]  hey, by the way, this might help performance.
[194.66 --> 199.02]  I've done some testing here, and I've noticed that if you use the same fix
[199.02 --> 201.82]  that Hector Martin found and you apply it,
[202.22 --> 204.86]  you're going to get this kind of expected performance increase.
[205.16 --> 207.66]  And, you know, just one of these great examples of community helping,
[208.50 --> 210.22]  you know, really improving a product like this.
[210.48 --> 212.52]  The Docker team took a look at the suggestion and said,
[212.58 --> 214.74]  yeah, you're right, let's implement it.
[214.82 --> 218.62]  And now they're saying some operations are like 98% faster.
[219.66 --> 220.90]  Well, they were pretty slow beforehand.
[221.16 --> 222.04]  So, I mean.
[222.80 --> 223.86]  They had room to go.
[223.86 --> 226.84]  They had plenty of headspace to improve that.
[227.00 --> 227.10]  Yeah.
[227.54 --> 227.80]  Yeah.
[228.02 --> 228.76]  It's interesting.
[228.94 --> 232.24]  And, you know, as we record, the Asahi Linux team just released,
[232.38 --> 235.32]  I think it was, you know, a few days ago, their first alpha.
[236.14 --> 236.54]  Right.
[237.36 --> 239.44]  And I'm going to give it a go this Sunday.
[239.74 --> 240.86]  By the time people are hearing this,
[240.88 --> 244.54]  it'll be just like probably the weekend this episode came out.
[244.94 --> 247.06]  But we tried it at first,
[247.06 --> 252.52]  and there's like some file system typical problems you'll fall into
[252.52 --> 254.20]  that just sort of trap you.
[254.36 --> 256.74]  It's like, I don't know if you ever played that game Pitfall.
[256.94 --> 259.92]  You know, you're running along and all of a sudden you just fall into a pit.
[260.30 --> 262.76]  That's what it's like right now trying to get Linux on the M1.
[262.86 --> 266.64]  But if you solve file system problems or you don't have any file system problems
[266.64 --> 271.82]  and you're trying it on an M1 Mac, like an Air or a Mini,
[271.82 --> 274.08]  it seems to be pretty straightforward.
[274.54 --> 279.04]  And early benchmarks are showing pretty good performance,
[279.10 --> 280.54]  as long as you're not hitting that GPU.
[281.54 --> 281.60]  Yeah.
[281.62 --> 285.02]  You know what's interesting is Jeff Geerling released a video this week
[285.02 --> 288.24]  talking about his experiences with the new Mac Studio.
[288.94 --> 291.58]  And in that video, he did some power comparisons
[291.58 --> 294.54]  between a recent Ryzen system that he built,
[294.74 --> 298.00]  a Linux gaming PC, compared to the Mac Studio.
[298.00 --> 301.94]  And I couldn't quite believe what I was seeing.
[302.04 --> 304.54]  But then at the same time, having used the M1 MacBook Air
[304.54 --> 309.36]  and my M1 Max MacBook Pro.
[309.66 --> 310.72]  God, that's such a stupid name.
[312.10 --> 313.88]  I just called the MacBook Max.
[314.60 --> 314.94]  Okay.
[315.16 --> 315.42]  Yeah.
[315.50 --> 316.56]  Well, it's still a stupid name.
[316.98 --> 320.30]  But who thought Max Mac was a good one?
[320.40 --> 320.66]  Anyway.
[321.46 --> 321.76]  I know.
[322.06 --> 324.16]  You know, there's just nobody to say no anymore, is there?
[324.60 --> 327.22]  Anyway, that's a bit of a segue, a bit of a tangent,
[327.22 --> 328.50]  a bit of a tangent there.
[329.36 --> 329.80]  Yeah.
[329.80 --> 331.42]  The power draw was a lot better, though.
[331.48 --> 331.78]  You're right.
[332.90 --> 335.22]  Wasn't the Ryzen something in the 40-watt neighborhood?
[335.56 --> 336.06]  That's right.
[336.16 --> 336.52]  Yeah, yeah.
[336.60 --> 339.28]  The Ryzen was about 38, 40 watts, something like that.
[339.34 --> 342.32]  And the Mac Studio idle was 6 watts.
[342.70 --> 343.88]  It's the same as a Raspberry Pi.
[344.48 --> 344.62]  Yeah.
[344.68 --> 346.80]  And in the context of Docker Desktop 2,
[346.90 --> 351.40]  you really got to figure the majority of the use case
[351.40 --> 353.00]  is for development testing.
[353.00 --> 358.56]  And so this fsync change doesn't really impact things much
[358.56 --> 360.08]  other than, you know, improves performance.
[360.22 --> 361.68]  I think, I'm not sure, Alex,
[361.72 --> 363.74]  but I think there's an argument to be made
[363.74 --> 365.76]  that it might be slightly less safe
[365.76 --> 368.24]  the way they've changed this operation.
[368.48 --> 371.10]  But it kind of feels like, you know, again,
[371.36 --> 373.32]  for a development Docker setup,
[373.48 --> 375.96]  it doesn't really matter if it's slightly less safe
[375.96 --> 379.22]  because you're not running your production server on this thing.
[379.22 --> 381.02]  Yeah, it's a similar type of operation
[381.02 --> 383.76]  to when you make a bunch of writes to a USB drive, right?
[384.12 --> 385.50]  After you've written some data,
[385.62 --> 388.02]  you need to sync it and make sure that those writes have occurred
[388.02 --> 389.94]  and the fast system tables have all been updated,
[390.06 --> 390.70]  that kind of thing.
[391.18 --> 394.08]  So as it turns out, macOS actually cheats, as you said, Chris.
[394.72 --> 397.72]  On Linux, fsync will both flush writes to the drive
[397.72 --> 401.14]  and ask it to flush its write cache to stable storage.
[401.66 --> 405.24]  But on macOS, fsync only flushes writes to the drive itself.
[405.24 --> 409.18]  Instead, they provide a ffulsync operation
[409.18 --> 411.02]  to do what fsync does on Linux.
[411.60 --> 415.58]  Ah, so you got fsync and you got fsync full sync.
[416.00 --> 416.34]  Yeah.
[417.12 --> 419.78]  Now on the laptops, I can see why they would do this, right?
[419.82 --> 422.44]  Because essentially the laptop has a built-in UPS.
[422.60 --> 424.18]  If you yank the power cord on a MacBook,
[424.54 --> 426.36]  it's going to keep on trucking, right?
[426.46 --> 427.24]  But on a Mac Studio...
[427.80 --> 428.92]  Same on the iPhone, right?
[428.96 --> 430.24]  Same on an iPhone, yeah, absolutely.
[430.64 --> 433.24]  But on a Mac Studio or some kind of other desktop,
[433.24 --> 436.24]  once you pull the power cord, you're toast.
[436.36 --> 438.76]  So this leads me to wonder what would happen to,
[438.76 --> 441.76]  you know, data integrity on a desktop Mac
[441.76 --> 443.32]  that doesn't have a built-in battery.
[444.46 --> 448.06]  Yeah, you got to figure Apple must have done the math,
[448.44 --> 451.02]  but there is that sort of cynical voice
[451.02 --> 452.28]  in the back of my head that goes,
[452.52 --> 454.90]  well, you know, they may have just designed this
[454.90 --> 458.56]  for mobile devices because that's their primary device now.
[458.62 --> 460.42]  And, you know, when they sell Macs,
[460.42 --> 463.18]  the number one Mac they sell are the laptops,
[463.30 --> 465.52]  so they're probably designing for that, you know?
[465.94 --> 467.96]  That's the voice in the back of my head when I hear that.
[468.02 --> 468.84]  And I think to myself,
[469.36 --> 471.56]  maybe APFS needs a few more years
[471.56 --> 473.92]  before I give it the old production grade
[473.92 --> 476.48]  for any kind of serious data storage.
[477.04 --> 477.88]  I mean, that said,
[478.14 --> 480.94]  I've experienced zero issues with APFS.
[480.94 --> 482.68]  And the migration was flawless.
[482.68 --> 486.68]  I really give them credit for the migration.
[486.98 --> 492.18]  I also give them credit for the really kind of low-key
[492.18 --> 495.84]  but consistent rollout they did over three versions of macOS
[495.84 --> 501.06]  to sort of slice and dice the way that volumes are managed on APFS.
[501.24 --> 503.36]  Like, they really executed well on that transition.
[503.48 --> 504.40]  I'll give them credit there.
[504.40 --> 507.48]  That doesn't change the fact, though,
[507.62 --> 513.30]  that we haven't seen a lot of production server-grade
[513.30 --> 516.16]  edge case uses out there for years, right?
[516.22 --> 518.74]  And I don't mean to be the old IT guy in the room,
[518.88 --> 519.62]  but for me,
[520.28 --> 522.48]  for a file system to really be production-grade,
[522.58 --> 523.94]  say, for, like, server data,
[523.94 --> 526.88]  I want to see other people banging on it
[526.88 --> 528.52]  for a few years in production
[528.52 --> 530.02]  in the way I'd be using it.
[530.04 --> 532.54]  So if it's containers or whatever it might be,
[532.54 --> 535.00]  you know, like, yeah, they've done well,
[535.32 --> 536.74]  and I think that sets the ground
[536.74 --> 539.10]  for a pretty good file system that I can trust,
[539.26 --> 540.24]  but it's still, like,
[540.38 --> 543.52]  for it to actually be considered safe in my brain,
[544.02 --> 546.38]  I've got to see people using it the way I'm using it,
[546.54 --> 548.18]  and I've got to see that working for a while.
[548.98 --> 550.08]  Yeah, so with all that in mind,
[550.08 --> 554.90]  I really hope that Asahi Linux works well
[554.90 --> 556.04]  in a couple of years' time.
[556.54 --> 558.68]  And, you know, the market is flooded
[558.68 --> 561.00]  with these cheap M1 Mac minis
[561.00 --> 563.12]  that are now obsolete from Apple software,
[563.36 --> 566.82]  and we can all run low-power Linux,
[567.18 --> 569.44]  Apple Silicon home servers.
[571.78 --> 574.16]  Linode.com slash SSH.
[574.22 --> 576.34]  Go there to get $100 in 60-day credit
[576.34 --> 577.22]  on a new account,
[577.42 --> 579.42]  and you go there to support this here show.
[579.92 --> 580.64]  Yeah, that's right.
[580.84 --> 582.12]  This here show is made possible
[582.12 --> 583.66]  by you taking advantage of our sponsor.
[583.84 --> 585.00]  When it comes time for you
[585.52 --> 586.74]  or someone you know
[586.74 --> 587.72]  or someone you're working with
[587.72 --> 588.58]  to deploy a server,
[589.22 --> 590.98]  go to linode.com slash SSH.
[590.98 --> 592.08]  It's what I use for anything
[592.08 --> 593.28]  that I deploy in the cloud
[593.28 --> 594.74]  for, like, the last two and a half years.
[595.12 --> 596.52]  And it's so much nicer
[596.52 --> 597.42]  than those hyperscalers
[597.42 --> 598.32]  that just want to lock into
[598.32 --> 600.34]  their crazy, complicated platforms.
[600.84 --> 602.52]  You know, Linode started in 2003,
[602.74 --> 604.62]  and they've just been moving it forward,
[604.84 --> 606.64]  iterating and making it better and better.
[606.82 --> 609.52]  And now, it's like nearly 19 years later.
[610.58 --> 611.34]  That's wild.
[611.64 --> 612.76]  Linode is old enough to vote.
[612.76 --> 613.44]  That's crazy.
[613.44 --> 615.56]  And they've really just iterated on
[615.56 --> 617.06]  and making something super great.
[617.24 --> 618.32]  And that's why they're willing
[618.32 --> 619.12]  to give you $100.
[620.10 --> 622.44]  $100 is like a confidence statement.
[622.82 --> 623.52]  They're saying,
[623.68 --> 624.76]  we trust that if we let you
[624.76 --> 626.34]  actually kick the tires with this thing,
[626.36 --> 627.38]  you're going to like what you see.
[627.62 --> 628.82]  And it's just such a great way
[628.82 --> 629.82]  to support the show, too.
[630.16 --> 631.80]  So it's linode.com slash SSH.
[631.88 --> 632.66]  Go deploy something.
[632.76 --> 633.62]  Go try something.
[634.16 --> 635.98]  Go see why they are the absolute best.
[636.10 --> 637.30]  They make cloud computing simple,
[637.50 --> 639.12]  affordable, and accessible to all.
[639.84 --> 642.22]  Linode.com slash SSH.
[643.44 --> 647.22]  Now, this is a Mixture Public Service announcement
[647.22 --> 649.00]  slash App Pick.
[649.14 --> 650.20]  I think we've mentioned Paperless
[650.20 --> 651.04]  on the show before.
[651.52 --> 653.48]  It's a document management system
[653.48 --> 655.84]  that helps you transform physical documents
[655.84 --> 658.12]  into a searchable online archive.
[658.60 --> 659.94]  And I've used this to great effect
[659.94 --> 660.80]  for my wife, actually,
[660.88 --> 662.68]  when we're traveling and stuff back to England.
[663.20 --> 666.46]  She does a lot of Skype and Zoom music teaching lessons.
[666.60 --> 667.30]  She's a music teacher.
[667.86 --> 669.16]  And what we actually did
[669.16 --> 671.30]  was scanned all of her students' music
[671.30 --> 672.56]  into Paperless.
[672.72 --> 674.84]  And then using the OCR that's in there,
[674.88 --> 675.66]  we can actually search
[675.66 --> 677.28]  for the specific bit of sheet music
[677.28 --> 677.90]  that we need
[677.90 --> 679.08]  when she's in England
[679.08 --> 680.22]  on my server back here,
[680.26 --> 682.50]  which is just super cool.
[682.74 --> 683.94]  So anyway, for the longest time,
[684.08 --> 686.66]  I've been using Paperless-NG.
[687.30 --> 689.46]  I think it stood for Paperless Next Gen.
[689.94 --> 691.46]  Not entirely sure, to be honest.
[692.00 --> 694.18]  I like to think the next generation.
[694.68 --> 696.02]  Yeah, like make it so.
[696.98 --> 697.88]  You got it.
[697.88 --> 701.34]  A chap called Jonas Winkler
[701.34 --> 703.86]  actually took over the original Paperless project,
[703.86 --> 705.36]  which itself had been abandoned.
[706.08 --> 707.62]  Now, in the last few weeks,
[707.86 --> 709.62]  there's been a new project come along
[709.62 --> 712.30]  called Paperless-NGX.
[712.74 --> 714.36]  Next Generation X?
[715.22 --> 716.50]  Something like that?
[717.18 --> 719.36]  And essentially what the community have done
[719.36 --> 722.56]  is the NG fork of the original code
[722.56 --> 724.36]  has seemed to go unmaintained.
[724.46 --> 725.36]  There's actually a GitHub issue,
[725.46 --> 726.62]  which we'll link to in the show notes,
[726.62 --> 729.06]  where there's a bunch of people talking about
[729.06 --> 730.74]  how much value they get from the software
[730.74 --> 732.74]  and also how much of a shame it is
[732.74 --> 733.86]  to see it kind of go to waste.
[734.44 --> 736.32]  But obviously, open source being open source,
[736.66 --> 738.58]  you know, this discussion thread went on
[738.58 --> 741.20]  for, you know, the best part of two, three weeks
[741.20 --> 743.58]  before eventually the community just went,
[744.02 --> 745.44]  okay, this Jonas guy,
[745.68 --> 748.06]  he seems to have fallen off the radar for now
[748.06 --> 748.92]  for whatever reason.
[749.40 --> 750.54]  So we're just going to fork this thing
[750.54 --> 751.48]  and call it NGX.
[752.32 --> 753.44]  Yeah, I sure hope he's okay.
[753.44 --> 755.38]  You know, I hope it's just a case of burnout.
[756.60 --> 758.76]  And it is good to see something like this.
[758.76 --> 760.38]  You wouldn't, this wouldn't happen
[760.38 --> 762.50]  with a commercial service, right?
[762.54 --> 764.42]  When a cloud company is shutting down
[764.42 --> 765.20]  for whatever reason,
[765.60 --> 767.16]  the product's just kind of gone.
[767.50 --> 768.82]  But when you have something
[768.82 --> 770.12]  that you can self-host,
[770.38 --> 771.80]  that's open source software,
[772.34 --> 775.56]  there can be a escape hatch
[775.56 --> 777.76]  when the project kind of starts to fade.
[778.08 --> 779.90]  Now, this first version doesn't seem
[779.90 --> 781.92]  like it's introduced a ton of new stuff.
[781.92 --> 784.92]  They dropped support for Python 3.7.
[785.02 --> 786.06]  So they're kind of moving that forward.
[786.18 --> 787.50]  They've updated a ton of the docs
[787.50 --> 788.94]  and the scripts and the containers
[788.94 --> 789.82]  and the branding.
[790.38 --> 791.68]  They also had to drop support
[791.68 --> 792.70]  for Ansible playbooks,
[792.74 --> 794.30]  which is definitely a bummer to see that.
[794.66 --> 796.42]  But they are hoping maybe somebody
[796.42 --> 798.34]  would want to help them support that.
[798.62 --> 800.04]  It seems like maybe it's just
[800.04 --> 802.16]  an issue of things getting out of date
[802.16 --> 804.14]  and the dev team not really having
[804.14 --> 805.38]  the skill set to manage it.
[806.16 --> 807.80]  So long as they continue to support Docker,
[808.18 --> 809.66]  you know, they've got my vote.
[809.66 --> 811.06]  But what's interesting, though,
[811.08 --> 813.66]  is if we look through the issues
[814.28 --> 814.96]  on their GitHub,
[815.24 --> 817.64]  there is one specifically talking around
[817.64 --> 821.18]  moving the organization in GitHub forward.
[821.90 --> 823.48]  And, you know, so right now
[823.48 --> 824.52]  is probably a really good time
[824.52 --> 825.64]  to get involved in the project
[825.64 --> 826.56]  if you're looking to do
[826.56 --> 828.70]  any kind of open source contributions.
[829.70 --> 830.70]  You know, clearly they're looking
[830.70 --> 832.58]  to improve the project.
[833.38 --> 835.76]  There is an issue in here, 1632,
[835.94 --> 836.68]  which again will be linked
[836.68 --> 838.02]  in the show notes where they're talking
[838.02 --> 840.62]  about how you can make
[840.62 --> 842.56]  your membership official of the project.
[843.40 --> 845.56]  It's 100% a community project
[845.56 --> 847.78]  and they will gladly welcome contributions
[847.78 --> 849.82]  from anybody, member or not.
[850.46 --> 852.48]  But, you know, if you're a member of it,
[852.54 --> 854.92]  you can start to have a bit more say
[854.92 --> 856.92]  over where the direction of the project goes
[856.92 --> 857.60]  and that kind of thing.
[858.26 --> 858.58]  Interesting.
[859.18 --> 861.12]  Yeah, I wish them the best, right?
[861.12 --> 862.64]  This is one of those projects
[862.64 --> 866.84]  that I think is probably not mentioned enough.
[867.38 --> 868.82]  If you look into it,
[868.90 --> 869.94]  it's such a no-brainer.
[870.72 --> 873.20]  I'm implementing this in the future,
[873.68 --> 874.60]  probably at the end of summer.
[875.30 --> 876.96]  I'm definitely putting this into action.
[877.30 --> 877.82]  It's amazing.
[878.20 --> 879.34]  There's just no way
[879.34 --> 881.06]  I'm going to do another year
[881.06 --> 881.86]  without this system.
[881.96 --> 883.78]  So Paperless NGX, go check it out.
[884.62 --> 887.20]  My plan is to have something set up
[887.20 --> 887.96]  by the end of summer.
[887.96 --> 890.18]  So that way, I know,
[890.38 --> 891.62]  I'm a big talker right now,
[892.10 --> 893.98]  but that way at the start of 2023,
[893.98 --> 895.60]  I could just use Paperless
[895.60 --> 896.56]  from the beginning of the year.
[896.96 --> 897.38]  We'll see.
[897.90 --> 899.52]  I'll tell you where it's really useful
[899.52 --> 900.62]  is tax season.
[901.06 --> 902.76]  You know, you get all these 1099s
[902.76 --> 903.82]  and W2 forms,
[903.94 --> 905.22]  all this kind of crap coming in,
[905.26 --> 907.26]  you know, from all over the place.
[907.42 --> 909.52]  You just take a picture on your smartphone
[909.52 --> 912.00]  with one of the scan apps
[912.00 --> 915.52]  and then you can share it from there
[915.52 --> 916.38]  with Paperless,
[916.38 --> 917.82]  you know, like through the share sheet
[917.82 --> 920.48]  on iOS or a similar thing on Android.
[921.00 --> 922.64]  That will basically then upload
[922.64 --> 924.08]  the file into Paperless
[924.08 --> 926.24]  and then it does its optical
[926.24 --> 927.84]  character recognition OCR
[927.84 --> 928.96]  on those files.
[929.46 --> 930.48]  And from there,
[930.70 --> 931.58]  all you need to do
[931.58 --> 932.96]  when it comes to tax time
[932.96 --> 935.44]  is search 1099 or tax
[935.44 --> 936.40]  or whatever it is
[936.40 --> 938.04]  and you'll just find all the forms.
[938.26 --> 938.82]  Boom, boom, boom, boom, boom.
[940.00 --> 941.58]  Even cooler than that, though,
[941.70 --> 942.96]  is you can set up a bunch
[942.96 --> 944.42]  of ingestion rules.
[944.42 --> 945.92]  So what we did for the sheet music,
[945.92 --> 946.52]  for example,
[946.92 --> 948.30]  was we look for certain keywords
[948.30 --> 949.52]  like bassoon or piano
[949.52 --> 950.44]  or that kind of thing
[950.44 --> 953.48]  and add certain tags to each file.
[953.90 --> 954.82]  So in our case,
[954.84 --> 956.32]  we added sheet music as a tag
[956.32 --> 957.68]  or anytime I get an email
[957.68 --> 960.48]  from Google with my Google Fi bill in it,
[960.80 --> 962.30]  I have that send the email,
[962.42 --> 963.36]  automatically forward it
[963.36 --> 965.14]  to an address
[965.14 --> 966.26]  that will put it
[966.26 --> 967.32]  into a specific folder
[967.32 --> 970.16]  and Paperless will scan that folder,
[970.38 --> 971.28]  ingest the file,
[971.46 --> 972.44]  automatically tag it.
[972.44 --> 973.92]  And so when I come to expense
[973.92 --> 975.68]  my cell phone bill through work,
[975.88 --> 976.86]  all I need to do
[976.86 --> 978.86]  is I don't need to log into Google Fi
[978.86 --> 979.72]  and then Spectrum
[979.72 --> 981.86]  and all these different systems.
[982.12 --> 983.24]  I log into Paperless,
[983.38 --> 984.98]  search for my little keyword
[984.98 --> 988.16]  to bring up my personal internet bills.
[988.72 --> 990.04]  Boom, just download the PDF.
[990.22 --> 990.40]  Done.
[991.36 --> 993.60]  That's so great.
[993.90 --> 994.50]  I love it.
[994.72 --> 996.54]  I really, really love it.
[997.14 --> 997.84]  I've been struggling
[997.84 --> 999.66]  with that very thing today.
[999.80 --> 1001.64]  That's what I was working on earlier today.
[1002.44 --> 1004.84]  It's just been one bad news after another,
[1004.98 --> 1006.30]  including the one
[1006.30 --> 1007.78]  that I probably heard from
[1007.78 --> 1009.94]  the most from the audience
[1009.94 --> 1011.20]  since our last episode,
[1011.20 --> 1012.88]  and that is that the Matter Group
[1012.88 --> 1015.22]  has announced a delay
[1015.22 --> 1016.94]  for the Matter Standard.
[1017.10 --> 1019.52]  Yes, that is the one announced in 2019
[1019.52 --> 1022.14]  by Amazon, Apple, Google, and Samsung.
[1023.14 --> 1024.96]  The idea is to take Zigbee
[1024.96 --> 1025.68]  and make something
[1025.68 --> 1027.26]  they could all use together
[1027.26 --> 1029.50]  that has a few base things
[1029.50 --> 1030.40]  they could all agree on.
[1030.48 --> 1031.54]  And of course, Alex,
[1031.54 --> 1035.02]  the industry is trying to spin this.
[1035.14 --> 1036.62]  Like the Nanoleaf CEO said,
[1036.72 --> 1036.90]  quote,
[1037.48 --> 1038.86]  I think the three-month delay
[1038.86 --> 1040.56]  might actually be a good thing.
[1040.96 --> 1041.76]  I feel that now
[1041.76 --> 1042.86]  that there's more certainty
[1042.86 --> 1043.70]  across the industry,
[1043.80 --> 1044.58]  we'll see unity
[1044.58 --> 1045.94]  at the time of launch.
[1046.18 --> 1046.78]  Yeah, it's a good thing
[1046.78 --> 1048.42]  because we can't get enough chips right now,
[1048.46 --> 1049.64]  so we'll just push it out
[1049.64 --> 1051.58]  and then sell the same amount anyway.
[1052.36 --> 1053.12]  Right, sure.
[1053.38 --> 1053.82]  Yeah, I mean,
[1053.86 --> 1054.52]  it's his job to say
[1054.52 --> 1055.28]  it's a good thing, right?
[1055.88 --> 1056.38]  I gotta say,
[1056.40 --> 1057.36]  I'm not too surprised.
[1057.36 --> 1059.66]  It really is funny, though,
[1059.68 --> 1061.90]  because anybody who doubts matter,
[1062.20 --> 1062.60]  it's like,
[1062.72 --> 1064.36]  they took this news, man,
[1064.48 --> 1067.22]  and they just run with it.
[1067.34 --> 1069.14]  They sent me the link.
[1070.40 --> 1072.26]  And I agree,
[1072.50 --> 1074.06]  my confidence is slipping,
[1074.06 --> 1075.92]  but it just,
[1076.32 --> 1078.16]  it's so obviously needed
[1078.16 --> 1080.52]  that I hope,
[1080.52 --> 1081.92]  I hope that this delay
[1081.92 --> 1084.72]  doesn't throw this whole thing off track.
[1084.84 --> 1085.90]  But it has sent me
[1085.90 --> 1089.80]  into a bit of a death spiral
[1089.80 --> 1091.58]  with my whole home setup now, Alex.
[1091.70 --> 1092.68]  It's just a disaster.
[1093.28 --> 1093.90]  I don't blame you.
[1093.96 --> 1094.82]  I mean, we had that feedback
[1094.82 --> 1095.94]  a couple of episodes ago
[1095.94 --> 1096.34]  saying,
[1096.48 --> 1097.84]  should I wait for Matter
[1097.84 --> 1099.60]  or should I get into Z-Wave
[1099.60 --> 1101.28]  or Zigbee or whatever right now?
[1101.48 --> 1102.66]  And if I recall,
[1102.72 --> 1103.34]  the advice was,
[1103.34 --> 1104.26]  if you need something now,
[1104.34 --> 1104.86]  buy it now.
[1104.92 --> 1105.94]  And I think that advice
[1105.94 --> 1108.52]  has just been proven right.
[1108.70 --> 1108.86]  You know,
[1108.92 --> 1109.84]  if you need
[1109.84 --> 1112.22]  a new smart home widget today,
[1112.80 --> 1114.76]  buy what's on the market today
[1114.76 --> 1116.24]  and hope for the best.
[1117.32 --> 1118.14]  Yeah, and for me,
[1118.28 --> 1119.52]  for me,
[1119.74 --> 1121.00]  it sends me
[1121.00 --> 1122.80]  into this whole spiral of,
[1123.16 --> 1123.28]  okay,
[1123.28 --> 1124.44]  now I've got a problem
[1124.44 --> 1126.28]  because I've got a network
[1126.28 --> 1127.04]  of, you know,
[1128.02 --> 1129.42]  30 Z-Wave devices
[1129.42 --> 1130.42]  devices
[1130.42 --> 1132.04]  and they are integrated
[1132.04 --> 1133.48]  throughout the automations
[1133.48 --> 1135.28]  and, you know,
[1135.34 --> 1136.04]  everything from
[1136.04 --> 1137.78]  temperature display widgets
[1137.78 --> 1141.74]  to scripts and automations.
[1142.06 --> 1143.88]  I have a Z-Wave device in there.
[1144.30 --> 1145.26]  And so the migration
[1145.26 --> 1146.08]  to Z-Wave JS,
[1146.34 --> 1147.34]  which I've tried in the past
[1147.34 --> 1147.74]  for me,
[1148.22 --> 1149.90]  went horribly bad.
[1150.30 --> 1150.86]  Nothing worked.
[1150.94 --> 1151.84]  I essentially had to just
[1151.84 --> 1153.38]  retouch everything
[1153.38 --> 1154.12]  in Home Assistant.
[1154.58 --> 1154.90]  And you know,
[1154.92 --> 1155.38]  one of those things
[1155.38 --> 1156.40]  where you load your dashboard
[1156.40 --> 1158.10]  and like everything's aired out
[1158.10 --> 1159.06]  and not working right.
[1159.70 --> 1160.10]  Oh, yeah.
[1160.68 --> 1162.40]  Yeah, that was my situation.
[1163.20 --> 1165.02]  And so my thought was,
[1165.14 --> 1165.54]  screw it.
[1165.60 --> 1166.46]  I'm not going to migrate
[1166.46 --> 1167.24]  to Z-Wave JS.
[1167.44 --> 1168.16]  I'm going to hold out
[1168.16 --> 1169.28]  and just move over to Matter
[1169.28 --> 1170.10]  and I'll just
[1170.10 --> 1172.68]  low-key replace the devices
[1172.68 --> 1173.34]  over a year
[1173.34 --> 1174.00]  and call it good.
[1174.66 --> 1176.40]  And that plan came crashing down
[1176.40 --> 1177.36]  a couple of months ago
[1177.36 --> 1178.08]  when I discovered
[1178.08 --> 1178.92]  or a month ago
[1178.92 --> 1179.56]  when I discovered
[1179.56 --> 1180.46]  that the next release,
[1180.56 --> 1181.48]  the one that comes out
[1181.48 --> 1183.52]  in really probably a few days
[1183.52 --> 1184.22]  from the release
[1184.22 --> 1184.86]  of this episode,
[1185.02 --> 1187.54]  will totally disable
[1187.54 --> 1188.66]  the Z-Wave integration
[1188.66 --> 1189.32]  that I'm using.
[1189.86 --> 1191.82]  So I'm kind of stuck in time
[1191.82 --> 1193.16]  with Home Assistant.
[1193.54 --> 1195.02]  And now that Matter is delayed,
[1195.18 --> 1196.10]  it's like a whole
[1196.10 --> 1197.44]  another complicating factor.
[1198.36 --> 1199.80]  And I've realized
[1199.80 --> 1200.96]  that if I'm going to do
[1200.96 --> 1202.52]  this Z-Wave JS migration,
[1203.06 --> 1204.34]  that it's going to end up
[1204.34 --> 1206.70]  being so much work
[1206.70 --> 1208.78]  that I might as well
[1208.78 --> 1209.62]  take this opportunity
[1209.62 --> 1210.96]  to just redo everything.
[1211.66 --> 1211.84]  You know,
[1211.96 --> 1213.04]  have you reached that point
[1213.04 --> 1213.36]  where you're like,
[1213.36 --> 1213.80]  yeah, okay,
[1213.88 --> 1215.80]  this one job
[1215.80 --> 1217.28]  is essentially so much work
[1217.28 --> 1218.14]  that just nuke
[1218.14 --> 1218.62]  and paving
[1218.62 --> 1220.14]  the entire infrastructure
[1220.14 --> 1221.94]  is only a minor part
[1221.94 --> 1222.96]  of the overall work.
[1224.18 --> 1224.70]  I feel that way
[1224.70 --> 1225.36]  every time I think
[1225.36 --> 1226.12]  about implementing
[1226.12 --> 1227.46]  a VLAN setup
[1227.46 --> 1228.10]  in my house.
[1228.22 --> 1228.70]  Like at the moment,
[1228.74 --> 1229.84]  I just run a flat network
[1229.84 --> 1231.80]  and I think,
[1231.92 --> 1232.48]  oh, it would be cool
[1232.48 --> 1233.22]  if my cameras
[1233.22 --> 1234.16]  were on their own VLAN
[1234.16 --> 1235.88]  and then all my IoT stuff
[1235.88 --> 1236.30]  was on its own.
[1236.32 --> 1236.90]  But you think,
[1237.12 --> 1239.00]  I'm going to have to touch
[1239.00 --> 1240.48]  every device here
[1240.48 --> 1242.20]  and I just can't be bothered.
[1242.20 --> 1243.48]  Let's just stick it
[1243.48 --> 1244.28]  in a slash 16
[1244.28 --> 1245.08]  and forget about it.
[1245.08 --> 1248.76]  tailscale.com
[1248.76 --> 1250.02]  slash self-hosted.
[1250.08 --> 1250.54]  Go there to get
[1250.54 --> 1251.40]  a free personal account
[1251.40 --> 1252.40]  for up to 20 devices
[1252.40 --> 1253.12]  and of course
[1253.12 --> 1253.98]  you support the show
[1253.98 --> 1254.82]  and you can sign up
[1254.82 --> 1255.50]  for tailscale.
[1255.64 --> 1256.70]  tailscale.com
[1256.70 --> 1257.90]  slash self-hosted.
[1257.94 --> 1260.26]  It is the Zero Config VPN.
[1260.46 --> 1261.88]  It installs on any device
[1261.88 --> 1262.32]  in minutes.
[1262.46 --> 1264.08]  You can manage firewall rules.
[1264.24 --> 1265.78]  You can work from anywhere.
[1266.28 --> 1268.18]  I have really taken things
[1268.18 --> 1268.90]  to the next level.
[1269.02 --> 1269.96]  I have recently started
[1269.96 --> 1272.04]  adding a couple of my VMs
[1272.04 --> 1273.58]  to my tailscale network.
[1273.86 --> 1275.34]  Now stick with me here
[1275.34 --> 1275.80]  for a second.
[1276.28 --> 1277.80]  Now I can SSH
[1277.80 --> 1278.58]  into the VMs
[1278.58 --> 1279.26]  I have running
[1279.26 --> 1280.00]  on my machines
[1280.00 --> 1280.60]  here in the studio
[1280.60 --> 1281.18]  where I'm working
[1281.18 --> 1282.64]  on projects from home.
[1282.82 --> 1285.20]  It's so great.
[1285.54 --> 1286.62]  It is so great.
[1286.86 --> 1287.34]  Also,
[1287.58 --> 1288.50]  I can confirm
[1288.50 --> 1289.92]  that it is
[1289.92 --> 1291.38]  stupid simple
[1291.38 --> 1292.58]  to set up tailscale
[1292.58 --> 1293.44]  on Nix OS.
[1293.76 --> 1294.76]  More details on that
[1294.76 --> 1295.36]  in a moment.
[1295.82 --> 1296.42]  And what I love
[1296.42 --> 1297.14]  about tailscale
[1297.14 --> 1297.80]  is it supports
[1297.80 --> 1298.96]  two-factor authentication,
[1299.54 --> 1300.50]  your single sign-on,
[1300.50 --> 1301.96]  and underneath all of it,
[1302.18 --> 1303.18]  they're using the stuff
[1303.18 --> 1304.38]  that just makes WireGuard
[1304.38 --> 1304.86]  so great,
[1304.92 --> 1305.70]  the noise protocol.
[1306.20 --> 1307.54]  And they do a mesh network
[1307.54 --> 1307.98]  so that way
[1307.98 --> 1308.92]  it's one flat network
[1308.92 --> 1310.22]  between all your machines.
[1310.70 --> 1311.60]  It's so simple
[1311.60 --> 1312.66]  to get started as well
[1312.66 --> 1314.58]  and they really have installers
[1314.58 --> 1315.86]  for like every distro,
[1315.98 --> 1317.52]  even ARM Linux distros,
[1317.68 --> 1318.52]  all that kind of stuff.
[1319.02 --> 1319.88]  You'd be amazed
[1319.88 --> 1320.74]  how fast you can build
[1320.74 --> 1322.00]  out a WireGuard network
[1322.00 --> 1322.64]  that's meshed
[1322.64 --> 1323.14]  peer-to-peer
[1323.14 --> 1324.84]  in just minutes.
[1325.74 --> 1326.52]  I love it.
[1326.98 --> 1327.22]  And you know,
[1327.26 --> 1328.08]  after you get everything
[1328.08 --> 1328.74]  signed up,
[1328.74 --> 1330.46]  they all have their own IP
[1330.46 --> 1331.82]  and so I've started
[1331.82 --> 1332.78]  setting bookmarks.
[1333.00 --> 1334.62]  I have a tailscale folder
[1334.62 --> 1335.50]  in my bookmark bar
[1335.50 --> 1337.22]  and all of the different
[1337.22 --> 1338.40]  web services that I hit
[1338.40 --> 1340.32]  that I have a tailscale IP
[1340.32 --> 1340.76]  for now.
[1341.40 --> 1341.66]  So from,
[1342.20 --> 1342.96]  and of course that syncs
[1342.96 --> 1344.16]  across all my Chrome instances,
[1344.34 --> 1345.62]  so from every machine
[1345.62 --> 1346.98]  I can get access
[1346.98 --> 1348.44]  to those web apps
[1348.44 --> 1349.62]  and it doesn't matter what,
[1349.74 --> 1350.50]  it could be Dylan
[1350.50 --> 1351.54]  at home,
[1351.66 --> 1352.30]  it could be something
[1352.30 --> 1352.80]  at the studio,
[1352.92 --> 1353.38]  it could be something
[1353.38 --> 1353.90]  in the RV,
[1354.02 --> 1354.48]  it could be something
[1354.48 --> 1355.02]  up on Linode.
[1355.08 --> 1357.08]  It's just super powerful.
[1357.60 --> 1358.68]  So go try it for yourself.
[1358.74 --> 1359.72]  Support the show
[1359.72 --> 1361.68]  and use it up to 20 machines
[1361.68 --> 1362.68]  for absolutely free
[1362.68 --> 1363.26]  by going to
[1363.26 --> 1364.54]  tailscale.com
[1364.54 --> 1365.22]  slash
[1365.22 --> 1366.36]  self-hosted.
[1368.50 --> 1369.64]  In the doc,
[1369.72 --> 1371.70]  I see a very tantalizing
[1371.70 --> 1372.78]  little sentence
[1372.78 --> 1373.40]  that says,
[1373.56 --> 1374.86]  I have a new direction
[1374.86 --> 1375.56]  for dupes,
[1375.80 --> 1377.34]  the no container theory.
[1377.72 --> 1378.70]  I cannot wait
[1378.70 --> 1379.76]  to hear your logic on this.
[1380.26 --> 1381.72]  I want more control
[1381.72 --> 1383.08]  with this next go around
[1383.08 --> 1384.08]  and I'm looking at
[1384.08 --> 1385.20]  what my options are
[1385.20 --> 1387.00]  with any kind of setup
[1387.00 --> 1387.76]  that I might redo
[1387.76 --> 1389.14]  and maybe to kind
[1389.14 --> 1389.66]  of help you understand,
[1389.74 --> 1390.20]  I should recap
[1390.20 --> 1390.86]  what I have now.
[1391.22 --> 1392.18]  So right now,
[1392.18 --> 1392.96]  I have a couple
[1392.96 --> 1394.18]  of Raspberry Pi 4s
[1394.18 --> 1394.58]  that are running
[1394.58 --> 1396.32]  Ubuntu 2004,
[1396.70 --> 1396.84]  right,
[1396.92 --> 1398.04]  the previous LTS
[1398.04 --> 1401.22]  and back when
[1401.22 --> 1402.00]  I set that up,
[1402.10 --> 1402.34]  Alex,
[1402.40 --> 1403.86]  you could still get
[1403.86 --> 1405.74]  a setup script
[1405.74 --> 1406.84]  for Home Assistant
[1406.84 --> 1408.38]  where you could install
[1408.38 --> 1409.90]  supervised Home Assistant
[1409.90 --> 1411.60]  on vanilla Ubuntu,
[1411.74 --> 1412.32]  which I don't think
[1412.32 --> 1413.52]  they actually support anymore.
[1413.52 --> 1415.34]  but in my world,
[1415.54 --> 1417.44]  this is the ideal setup
[1417.44 --> 1418.64]  because I have Home Assistant
[1418.64 --> 1419.70]  running in containers
[1419.70 --> 1421.42]  but a fully supervised setup
[1421.42 --> 1422.70]  so I have access
[1422.70 --> 1423.58]  to the add-ons,
[1423.66 --> 1424.66]  I can get the hack store,
[1424.78 --> 1425.40]  all that kind of stuff.
[1425.46 --> 1426.62]  I get the backup manager,
[1426.88 --> 1427.40]  snapshots,
[1427.52 --> 1427.76]  et cetera,
[1427.84 --> 1428.18]  et cetera,
[1428.80 --> 1429.92]  but it's on an OS
[1429.92 --> 1430.90]  that I manage
[1430.90 --> 1432.24]  that I update
[1432.24 --> 1432.90]  because that's how
[1432.90 --> 1433.92]  I prefer to do things.
[1434.74 --> 1436.16]  That is no longer
[1436.16 --> 1437.02]  a viable option
[1437.02 --> 1438.16]  and even now,
[1438.26 --> 1440.26]  it's kind of fiddly.
[1441.16 --> 1441.94]  Home Assistant
[1441.94 --> 1443.12]  will often say
[1443.12 --> 1444.78]  that I am in an unhealthy state
[1444.78 --> 1446.06]  and so it won't let me
[1446.06 --> 1447.04]  update add-ons
[1447.04 --> 1448.14]  or update the system
[1448.14 --> 1449.82]  and I have to reboot
[1449.82 --> 1451.50]  and then it's all of a sudden
[1451.50 --> 1452.90]  in a healthy state again
[1452.90 --> 1455.02]  and then I can go about
[1455.02 --> 1455.94]  updating things.
[1456.50 --> 1458.38]  So it's already not perfect
[1458.38 --> 1459.86]  and I don't want to go
[1459.86 --> 1461.36]  the direction of
[1461.36 --> 1462.38]  where I was trending,
[1462.62 --> 1464.18]  which is an x86 machine
[1464.18 --> 1465.60]  that would be more powerful,
[1466.74 --> 1467.90]  ideally like a laptop
[1467.90 --> 1469.00]  that supports QuickSync
[1469.00 --> 1471.04]  and then I would put
[1471.04 --> 1472.06]  Proxmox on that
[1472.06 --> 1474.12]  and I would run
[1474.12 --> 1474.68]  Home Assistant
[1474.68 --> 1475.94]  in its own dedicated
[1475.94 --> 1476.66]  virtual machine
[1476.66 --> 1477.58]  as just an appliance
[1477.58 --> 1478.98]  and I would just
[1478.98 --> 1480.18]  swallow the fact
[1480.18 --> 1481.24]  that I am running
[1481.24 --> 1481.90]  their OS
[1481.90 --> 1483.08]  and I don't really
[1483.08 --> 1483.88]  want to do that.
[1484.38 --> 1485.28]  But you know what?
[1485.74 --> 1486.60]  It's fine,
[1486.64 --> 1487.36]  I told myself.
[1488.52 --> 1490.12]  But as the Asahi Linux team
[1490.12 --> 1491.56]  started getting Linux
[1491.56 --> 1492.50]  on the M1
[1492.50 --> 1493.74]  closer to a reality
[1493.74 --> 1495.06]  and I started realizing
[1495.06 --> 1497.32]  that a headless
[1497.32 --> 1499.06]  Mac Mini M1
[1499.06 --> 1501.36]  running Linux
[1501.36 --> 1502.78]  could be a viable
[1502.78 --> 1503.50]  home server
[1503.50 --> 1506.66]  and maybe I don't
[1506.66 --> 1507.28]  want to go this
[1507.28 --> 1508.14]  Proxmox route.
[1508.74 --> 1509.66]  Maybe I want to go
[1509.66 --> 1511.74]  a Linux host
[1511.74 --> 1512.72]  that is running
[1512.72 --> 1513.46]  these applications.
[1514.74 --> 1516.12]  Then I started thinking
[1516.12 --> 1518.48]  what are my two main
[1518.48 --> 1519.54]  problems that I would
[1519.54 --> 1520.10]  like to solve
[1520.10 --> 1521.32]  with this next round?
[1521.46 --> 1521.74]  Like if I,
[1521.88 --> 1522.62]  besides performance
[1522.62 --> 1523.34]  because that's a given,
[1523.74 --> 1525.38]  if I were rebuilding
[1525.38 --> 1526.68]  my entire home setup
[1526.68 --> 1527.54]  and you got to think
[1527.54 --> 1528.12]  about this yourself
[1528.12 --> 1528.96]  probably sometimes,
[1529.56 --> 1531.70]  what problem would I
[1531.70 --> 1532.44]  really like to solve
[1532.44 --> 1532.94]  for myself?
[1533.60 --> 1535.02]  And I realized
[1535.02 --> 1536.88]  I would love to solve
[1536.88 --> 1538.40]  reproducibility
[1538.40 --> 1541.26]  because a year or two
[1541.26 --> 1541.90]  into this,
[1541.98 --> 1544.04]  I don't really remember
[1544.04 --> 1545.00]  how I have it set up.
[1545.06 --> 1545.82]  I have it set up
[1545.82 --> 1547.40]  in a way that it's
[1547.40 --> 1548.06]  pretty obvious
[1548.06 --> 1548.78]  to figure out
[1548.78 --> 1550.16]  and I do have
[1550.16 --> 1551.26]  some documentation
[1551.26 --> 1551.98]  although I haven't
[1551.98 --> 1552.98]  touched it in about a year.
[1553.74 --> 1555.54]  So I don't really have
[1555.54 --> 1556.56]  like a game plan
[1556.56 --> 1557.38]  to like rebuild
[1557.38 --> 1557.98]  this thing
[1557.98 --> 1559.36]  should a Raspberry Pi
[1559.36 --> 1559.96]  crap out.
[1560.26 --> 1560.40]  I mean,
[1560.42 --> 1561.10]  I could probably do it
[1561.10 --> 1561.84]  in a couple of days
[1561.84 --> 1563.60]  then the home assistant
[1563.60 --> 1564.48]  stuff would take longer
[1564.48 --> 1565.70]  but you know,
[1565.76 --> 1566.48]  it's not ideal.
[1567.62 --> 1568.66]  And I started thinking
[1568.66 --> 1569.68]  about what I could do
[1569.68 --> 1570.56]  to solve this problem
[1570.56 --> 1572.12]  and I started thinking
[1572.12 --> 1573.32]  about your favorite
[1573.32 --> 1573.88]  Ansible,
[1574.16 --> 1574.66]  of course.
[1575.46 --> 1576.08]  Perhaps like,
[1576.14 --> 1576.26]  you know,
[1576.28 --> 1577.14]  this was an opportunity
[1577.14 --> 1579.02]  and my moment in time
[1579.02 --> 1580.32]  to learn Ansible.
[1580.86 --> 1581.66]  I'm sure you think
[1581.66 --> 1582.62]  that's probably a great idea.
[1582.62 --> 1583.88]  Well,
[1583.92 --> 1584.44]  you're not going to hear
[1584.44 --> 1585.82]  anything bad
[1585.82 --> 1586.84]  about some kind
[1586.84 --> 1587.56]  of config management
[1587.56 --> 1588.02]  from me.
[1588.08 --> 1588.20]  No,
[1588.26 --> 1588.42]  no.
[1588.64 --> 1589.30]  I think Ansible
[1589.30 --> 1590.98]  is a laudable goal.
[1591.86 --> 1592.52]  So instead,
[1592.60 --> 1593.32]  I did a hard write
[1593.32 --> 1595.58]  and turned from that
[1595.58 --> 1596.68]  and went down
[1596.68 --> 1597.60]  the path of Nix.
[1598.76 --> 1599.68]  And the reason
[1599.68 --> 1600.64]  why I got to Nix
[1600.64 --> 1601.98]  is I wanted...
[1601.98 --> 1602.42]  God damn it.
[1602.44 --> 1603.20]  I wanted...
[1603.20 --> 1603.74]  I know,
[1603.78 --> 1604.08]  I'm sorry.
[1604.28 --> 1604.56]  I know.
[1604.64 --> 1605.44]  We're so close.
[1605.70 --> 1606.58]  I wanted something
[1606.58 --> 1609.24]  that was reproducible
[1609.24 --> 1609.96]  from the metal
[1609.96 --> 1611.78]  so I could essentially
[1611.78 --> 1612.76]  just recreate
[1612.76 --> 1614.28]  the same exact setup
[1614.28 --> 1615.70]  by just dropping
[1615.70 --> 1616.86]  in some config files
[1616.86 --> 1618.50]  and building the system.
[1619.20 --> 1621.28]  And that's what Nix provides.
[1621.98 --> 1622.98]  And then as I start
[1622.98 --> 1624.68]  to use Nix
[1624.68 --> 1625.24]  and Nix OS
[1625.24 --> 1626.94]  and I tried Nix OS
[1626.94 --> 1628.30]  versus just putting Nix
[1628.30 --> 1629.26]  on top of a distro
[1629.26 --> 1630.96]  and really it's just a...
[1631.92 --> 1632.96]  It's kind of like...
[1633.60 --> 1634.24]  It's a matter of
[1634.24 --> 1635.22]  how far do you want
[1635.22 --> 1636.06]  to be able to control
[1636.06 --> 1636.86]  the system, right?
[1636.86 --> 1637.62]  Are you good with
[1637.62 --> 1639.26]  setting up a base distro
[1639.26 --> 1640.54]  and keeping its package manager
[1640.54 --> 1641.68]  going and then putting
[1641.68 --> 1642.24]  Nix on there
[1642.24 --> 1643.36]  and then rebuilding everything?
[1643.52 --> 1644.40]  Or would you like to build
[1644.40 --> 1645.86]  everything from the ground up?
[1646.36 --> 1647.30]  User accounts,
[1647.46 --> 1648.36]  groups, permissions,
[1649.14 --> 1649.74]  everything,
[1650.24 --> 1651.06]  reproduce everything.
[1651.18 --> 1651.74]  And that's the route
[1651.74 --> 1652.32]  I want to go.
[1652.78 --> 1653.38]  And that's why
[1653.38 --> 1654.62]  I went more than just Nix
[1654.62 --> 1655.36]  the package manager.
[1655.48 --> 1656.24]  I went to Nix OS.
[1657.36 --> 1658.44]  And the Nix OS
[1658.44 --> 1659.66]  way of doing things
[1659.66 --> 1661.48]  is extremely compelling
[1661.48 --> 1662.92]  because you can...
[1662.92 --> 1664.38]  With very simple syntax,
[1664.66 --> 1665.28]  you can say,
[1665.40 --> 1666.42]  I want containers.
[1667.20 --> 1669.52]  And then you build the system
[1669.52 --> 1671.00]  and you can test it
[1671.00 --> 1672.02]  before you deploy it
[1672.02 --> 1673.04]  and it's reproducible
[1673.04 --> 1673.74]  and it's so great.
[1673.78 --> 1674.70]  But you build the system
[1674.70 --> 1675.82]  and if you tell it,
[1675.90 --> 1677.20]  I want containers,
[1678.22 --> 1679.78]  the Nix system
[1679.78 --> 1681.04]  figures it all out, man.
[1681.18 --> 1681.90]  It figures out
[1681.90 --> 1682.90]  the software dependencies,
[1683.12 --> 1683.64]  the services
[1683.64 --> 1684.62]  that need to be installed.
[1684.72 --> 1686.04]  You can make declarations
[1686.04 --> 1687.20]  in there for firewall stuff.
[1687.44 --> 1689.20]  It's a lot like Docker Compose,
[1689.42 --> 1691.90]  but for your entire OS.
[1692.74 --> 1695.26]  It's honestly how Linux should be.
[1695.26 --> 1696.14]  For a lot,
[1696.22 --> 1697.38]  for basically every use
[1697.38 --> 1698.22]  except for the desktop,
[1698.74 --> 1699.88]  this is how Linux should work.
[1700.08 --> 1701.52]  For every container,
[1701.94 --> 1702.86]  for every server,
[1703.26 --> 1704.86]  for every IoT device out there,
[1705.10 --> 1706.32]  for any system out there,
[1706.34 --> 1706.92]  and I'm telling you this
[1706.92 --> 1707.86]  as somebody who's used Linux
[1707.86 --> 1709.14]  for probably almost 25 years,
[1709.52 --> 1710.72]  this is how Linux
[1710.72 --> 1712.16]  should have worked forever.
[1712.58 --> 1713.42]  Now, Nix has actually been around
[1713.42 --> 1713.92]  for a little while.
[1714.04 --> 1714.88]  I'm just finally getting around
[1714.88 --> 1715.28]  to try it.
[1715.72 --> 1716.74]  And so what I have discovered,
[1716.88 --> 1717.04]  Alex,
[1717.04 --> 1717.84]  while using Nix
[1717.84 --> 1718.90]  is if you can use
[1718.90 --> 1720.10]  the Nix package manager
[1720.10 --> 1721.44]  to install stuff
[1721.44 --> 1722.28]  and manage stuff,
[1722.72 --> 1724.82]  you've essentially documented
[1724.82 --> 1725.66]  your entire system
[1725.66 --> 1726.58]  with the config file
[1726.58 --> 1727.74]  and made it reproducible.
[1727.94 --> 1728.78]  So anytime you could
[1728.78 --> 1729.96]  deploy Home Assistant
[1729.96 --> 1731.42]  through the config file
[1731.42 --> 1733.44]  or a sync thing
[1733.44 --> 1734.34]  or Plex
[1734.34 --> 1735.52]  or whatever,
[1736.12 --> 1736.86]  you can essentially
[1736.86 --> 1737.56]  run a command
[1737.56 --> 1738.66]  on another box
[1738.66 --> 1739.28]  and rebuild
[1739.28 --> 1739.72]  and recreate
[1739.72 --> 1740.66]  that entire system
[1740.66 --> 1742.64]  to exactly how you had it.
[1743.64 --> 1744.78]  And you can do that
[1744.78 --> 1745.78]  in a rolling way.
[1745.78 --> 1747.64]  So what happens
[1747.64 --> 1749.58]  when something isn't
[1749.58 --> 1751.36]  in the Nix way,
[1751.52 --> 1752.42]  the Nix ethos?
[1753.22 --> 1754.26]  Yeah, like an example
[1754.26 --> 1754.98]  of this actually
[1754.98 --> 1756.54]  is paperless NGX.
[1756.72 --> 1757.42]  Like I don't think
[1757.42 --> 1759.02]  that's been packaged up yet,
[1759.14 --> 1759.36]  right?
[1760.00 --> 1761.38]  You can totally do
[1761.38 --> 1762.26]  containers in Nix.
[1762.66 --> 1763.52]  Like totally.
[1763.74 --> 1764.78]  It is great for that.
[1764.86 --> 1766.30]  It's great as a container base
[1766.30 --> 1767.02]  and it is great
[1767.02 --> 1768.08]  as a container host.
[1769.04 --> 1770.74]  And you can do Podman
[1770.74 --> 1771.40]  and Docker
[1771.40 --> 1772.26]  on the same system
[1772.26 --> 1773.10]  at the same time.
[1773.24 --> 1774.42]  Like it's really powerful.
[1774.42 --> 1776.40]  And I think
[1776.40 --> 1777.02]  a lot of listeners
[1777.02 --> 1778.08]  that are hearing me
[1778.08 --> 1778.40]  right now
[1778.40 --> 1779.14]  are probably thinking,
[1779.28 --> 1779.64]  no, Chris,
[1779.72 --> 1781.06]  just run the container
[1781.06 --> 1781.80]  on Nix OS.
[1782.26 --> 1783.74]  It's so much easier.
[1784.06 --> 1785.16]  And that may actually
[1785.16 --> 1786.32]  ultimately be the way I go.
[1787.30 --> 1788.74]  I may still end up
[1788.74 --> 1789.60]  running a few things
[1789.60 --> 1790.16]  in containers,
[1790.16 --> 1791.66]  but what I have realized
[1791.66 --> 1794.16]  is the benefit
[1794.16 --> 1796.16]  of the way Nix
[1796.16 --> 1797.78]  manages everything
[1797.78 --> 1799.58]  is that I can come back
[1799.58 --> 1800.30]  to a system
[1800.30 --> 1802.34]  five years later
[1802.34 --> 1804.16]  and not only will it be
[1804.16 --> 1805.18]  fully up to date.
[1805.60 --> 1806.66]  But if it just has
[1806.66 --> 1807.38]  any problems,
[1807.74 --> 1809.04]  A, super easy to roll back
[1809.04 --> 1810.20]  and B, super easy
[1810.20 --> 1810.70]  to reproduce.
[1811.36 --> 1812.78]  Just like, done.
[1813.46 --> 1814.92]  How often do you do that though?
[1815.36 --> 1816.84]  Five years is your example.
[1817.72 --> 1818.06]  Often.
[1818.18 --> 1818.34]  I mean,
[1818.42 --> 1819.20]  usually I don't use hardware
[1819.20 --> 1820.14]  past that, right?
[1820.22 --> 1821.28]  So I'm touching on,
[1821.34 --> 1822.12]  I'm rebuilding stuff
[1822.12 --> 1823.46]  every few years, usually.
[1824.20 --> 1826.14]  I mean, speaking about myself,
[1826.46 --> 1829.58]  I prefer to change stuff
[1829.58 --> 1831.08]  every couple of years.
[1831.08 --> 1832.78]  So the chances of me
[1832.78 --> 1833.96]  sticking with the same system
[1833.96 --> 1835.42]  for five whole years
[1835.42 --> 1836.34]  is quite slim.
[1836.74 --> 1837.74]  Have you ever had
[1837.74 --> 1838.66]  like an Arch desktop
[1838.66 --> 1839.84]  that you install
[1839.84 --> 1841.50]  and then like three years later
[1841.50 --> 1842.86]  you realize it's the same install
[1842.86 --> 1843.44]  and you've just been
[1843.44 --> 1844.84]  reliably updating it?
[1845.24 --> 1846.52]  My Arch desktop actually
[1846.52 --> 1847.84]  is the one that I installed
[1847.84 --> 1848.28]  in London
[1848.28 --> 1849.70]  and it traveled across the ocean
[1849.70 --> 1850.70]  in a container, you know?
[1850.90 --> 1851.00]  So.
[1851.66 --> 1852.76]  I love it, right?
[1852.84 --> 1853.82]  And when you think about
[1853.82 --> 1855.72]  how like some desktop Linux users,
[1856.06 --> 1856.98]  especially Mint users,
[1857.10 --> 1858.62]  they actually like reinstall
[1858.62 --> 1859.38]  every major,
[1859.60 --> 1860.70]  for every major version.
[1860.82 --> 1861.14]  I know.
[1861.68 --> 1862.82]  It's crazy, right?
[1863.40 --> 1864.14]  Nix is that
[1864.14 --> 1865.60]  for everything to the next level
[1865.60 --> 1866.90]  and I can pin versions
[1866.90 --> 1867.62]  if I need to,
[1867.68 --> 1868.46]  I can roll back.
[1868.82 --> 1869.94]  It's the kind of distro
[1869.94 --> 1871.74]  that you can install it
[1871.74 --> 1873.70]  and you can actually
[1873.70 --> 1875.30]  reliably let it auto-update
[1875.30 --> 1876.96]  because it's so simple to recover.
[1878.30 --> 1879.70]  It's very compelling
[1879.70 --> 1882.08]  and I'm still kind of new to it
[1882.08 --> 1883.10]  so I'm struggling
[1883.10 --> 1884.80]  to really put all of it into words
[1884.80 --> 1886.16]  but it's got me excited
[1886.16 --> 1887.94]  in a way about deploying software
[1887.94 --> 1888.40]  on Linux
[1888.40 --> 1889.62]  that essentially
[1889.62 --> 1890.70]  Docker Compose did
[1890.70 --> 1891.38]  for containers
[1891.38 --> 1893.52]  and I really don't have
[1893.52 --> 1894.44]  a major problem
[1894.44 --> 1896.54]  with running these applications
[1896.54 --> 1897.20]  in containers
[1897.20 --> 1899.60]  but if I'm being totally honest,
[1900.60 --> 1902.40]  I do feel kind of weird
[1902.40 --> 1904.28]  about pulling down
[1904.28 --> 1905.58]  like essentially
[1905.58 --> 1906.74]  an entire software
[1906.74 --> 1908.20]  OS environment
[1908.20 --> 1909.18]  to run sync thing
[1909.18 --> 1910.68]  when it's just like,
[1910.78 --> 1911.12]  you know,
[1911.48 --> 1912.50]  some binaries
[1912.50 --> 1913.70]  and some config files
[1913.70 --> 1915.44]  and I don't really need
[1915.44 --> 1916.06]  to run all of that
[1916.06 --> 1916.52]  in a container.
[1916.52 --> 1917.36]  I don't need to manage
[1917.36 --> 1917.92]  the network.
[1918.04 --> 1918.52]  I don't need to have
[1918.52 --> 1920.16]  like these virtual network interfaces.
[1920.68 --> 1921.76]  I don't need any of that.
[1921.82 --> 1922.36]  I don't need to like
[1922.36 --> 1924.02]  mount storage volumes
[1924.02 --> 1925.20]  or any of that.
[1925.30 --> 1926.50]  I don't really need it
[1926.50 --> 1927.84]  if I can still get
[1927.84 --> 1929.30]  all of the manageability benefits
[1929.30 --> 1930.40]  that I got with the software
[1930.40 --> 1931.18]  as a container.
[1931.40 --> 1931.72]  You know,
[1931.72 --> 1933.00]  being able to pull down
[1933.00 --> 1934.00]  specific versions,
[1934.12 --> 1935.06]  being able to stay current,
[1935.14 --> 1936.24]  being able to roll back,
[1936.66 --> 1937.86]  being able to isolate data
[1937.86 --> 1939.02]  and application stuff.
[1939.02 --> 1939.24]  Like,
[1939.48 --> 1940.30]  I get all of that
[1940.30 --> 1940.66]  with Nix
[1940.66 --> 1941.46]  without actually having
[1941.46 --> 1942.30]  to have it in a container.
[1942.30 --> 1944.50]  That's compelling to me
[1944.50 --> 1945.80]  and it also means
[1945.80 --> 1946.36]  that I could probably
[1946.36 --> 1948.16]  really eek a lot of performance
[1948.16 --> 1948.94]  out of an M1
[1948.94 --> 1950.96]  and the great thing is
[1950.96 --> 1951.88]  is there's already people
[1951.88 --> 1952.94]  working to get Nix OS
[1952.94 --> 1954.28]  running on the M1 Mini.
[1954.60 --> 1955.00]  So like,
[1955.14 --> 1956.26]  by the time I'm ready
[1956.26 --> 1956.82]  to do this,
[1956.90 --> 1957.80]  the work's going to be done.
[1958.58 --> 1960.30]  Can I play devil's advocate now?
[1960.74 --> 1961.14]  Are you done?
[1961.74 --> 1962.14]  Yeah, yeah.
[1962.14 --> 1963.44]  Is your soapbox...
[1963.44 --> 1965.10]  So in summary,
[1965.90 --> 1966.74]  Boo containers.
[1967.06 --> 1967.68]  No, yeah, go ahead.
[1967.68 --> 1971.32]  Why learn
[1971.32 --> 1974.98]  a slightly unusual
[1974.98 --> 1976.48]  bespoke
[1976.48 --> 1979.76]  deployment configuration system,
[1980.14 --> 1981.52]  which is what Nix appears to use
[1981.52 --> 1982.54]  just from a quick glance.
[1982.60 --> 1982.90]  I'll be honest,
[1982.92 --> 1984.30]  I'm not super familiar with it.
[1984.94 --> 1985.56]  And I really,
[1985.74 --> 1985.96]  you know,
[1986.04 --> 1987.28]  I have no real opinions.
[1987.36 --> 1988.10]  Let me preface
[1988.10 --> 1988.98]  everything I'm about to say
[1988.98 --> 1990.00]  with no real opinions
[1990.00 --> 1991.00]  about Nix OS at all.
[1991.06 --> 1992.30]  I haven't looked at it
[1992.30 --> 1992.94]  super closely.
[1994.04 --> 1994.40]  But,
[1995.52 --> 1996.60]  devil's advocate time.
[1996.60 --> 1998.54]  If I am learning Ansible
[1998.54 --> 2000.96]  and I want to run it
[2000.96 --> 2001.64]  against Ubuntu
[2001.64 --> 2002.74]  or CentOS
[2002.74 --> 2003.80]  or Arch
[2003.80 --> 2005.66]  or macOS
[2005.66 --> 2008.28]  or any other system
[2008.28 --> 2009.80]  that Ansible supports,
[2010.38 --> 2012.06]  I've learned a skill
[2012.06 --> 2012.94]  that's transferable
[2012.94 --> 2013.82]  not only between
[2013.82 --> 2014.54]  multiple different
[2014.54 --> 2015.64]  operating systems,
[2015.92 --> 2018.60]  but also different jobs.
[2019.12 --> 2019.86]  And Ansible's been
[2019.86 --> 2020.56]  hugely powerful
[2020.56 --> 2021.40]  for my career,
[2021.60 --> 2021.78]  you know,
[2021.80 --> 2022.50]  as a springboard
[2022.50 --> 2022.98]  where I could
[2022.98 --> 2024.26]  start operating
[2024.26 --> 2024.82]  at a level
[2024.82 --> 2025.84]  that was much higher
[2025.84 --> 2026.84]  than actually
[2026.84 --> 2027.54]  if I'd just been
[2027.54 --> 2028.02]  doing everything
[2028.02 --> 2028.74]  like a caveman
[2028.74 --> 2029.82]  on the command line,
[2030.36 --> 2030.50]  right?
[2030.54 --> 2031.18]  Simply because
[2031.18 --> 2032.26]  people smarter than me
[2032.26 --> 2033.22]  had abstracted away
[2033.22 --> 2034.10]  a lot of the complexity.
[2035.30 --> 2036.56]  And so I look at Nix OS
[2036.56 --> 2037.50]  and I see their
[2037.50 --> 2038.38]  configuration language
[2038.38 --> 2040.18]  looks pretty easy
[2040.18 --> 2040.60]  to understand.
[2040.72 --> 2041.14]  It's, you know,
[2041.16 --> 2041.98]  it's just a standard
[2041.98 --> 2043.52]  sort of JSON type
[2043.52 --> 2044.66]  looking configuration
[2044.66 --> 2045.40]  thing, right?
[2046.58 --> 2047.48]  And some of the things
[2047.48 --> 2048.06]  you said, right?
[2048.10 --> 2049.64]  You wanted reproducibility.
[2050.16 --> 2050.32]  Okay,
[2050.40 --> 2050.86]  so Nix OS
[2050.86 --> 2052.42]  is clearly that
[2052.42 --> 2053.30]  because of the
[2053.30 --> 2054.32]  whole ethos
[2054.32 --> 2055.16]  of the project.
[2055.30 --> 2056.78]  But let's say
[2056.78 --> 2057.88]  you wanted in five years
[2057.88 --> 2059.52]  time to redeploy
[2059.52 --> 2060.68]  a specific version
[2060.68 --> 2061.26]  of Sync thing
[2061.26 --> 2062.24]  for whatever reason
[2062.24 --> 2062.74]  it might be.
[2063.90 --> 2065.00]  You could do that
[2065.00 --> 2066.00]  with a container
[2066.00 --> 2066.76]  on Ansible.
[2067.08 --> 2067.78]  You could go through
[2067.78 --> 2069.12]  your git commit history,
[2069.80 --> 2071.04]  look up what tag
[2071.04 --> 2071.56]  you are running
[2071.56 --> 2072.50]  five years ago,
[2073.06 --> 2073.72]  pull that down
[2073.72 --> 2074.42]  from Docker Hub,
[2074.82 --> 2076.12]  assuming it's still there,
[2076.12 --> 2076.86]  but the same was true
[2076.86 --> 2077.88]  of Nix OS, right?
[2078.28 --> 2079.06]  And then deploy
[2079.06 --> 2079.64]  that container
[2079.64 --> 2080.14]  and you've got
[2080.14 --> 2081.14]  everything as it was
[2081.14 --> 2081.96]  on that day in history
[2081.96 --> 2082.74]  five years ago.
[2082.98 --> 2083.82]  And it's all in git,
[2083.90 --> 2084.68]  so it's all version
[2084.68 --> 2085.54]  controlled and it's
[2085.54 --> 2086.28]  all reproducible.
[2087.20 --> 2087.86]  I wouldn't be surprised
[2087.86 --> 2088.62]  if the more common
[2088.62 --> 2089.76]  way of using Nix
[2089.76 --> 2091.44]  isn't Ansible
[2091.44 --> 2093.18]  deploying like a CentOS
[2093.18 --> 2094.12]  or a RHEL system
[2094.12 --> 2095.08]  or an Ubuntu system
[2095.08 --> 2095.96]  with the Nix package
[2095.96 --> 2096.98]  manager installed.
[2097.62 --> 2098.24]  Because I think
[2098.24 --> 2098.72]  the other thing you,
[2098.90 --> 2099.32]  I don't know if you
[2099.32 --> 2100.24]  mentioned it necessarily
[2100.24 --> 2100.54]  in there,
[2100.54 --> 2101.96]  but learning Ansible
[2101.96 --> 2102.74]  would also be a much
[2102.74 --> 2103.68]  more employable skill.
[2104.14 --> 2104.58]  You know,
[2104.62 --> 2105.12]  if you're ever looking
[2105.12 --> 2105.82]  for a job,
[2105.92 --> 2107.14]  it looks good on the resume.
[2107.88 --> 2108.28]  Um,
[2109.00 --> 2110.34]  so I actually don't think
[2110.34 --> 2111.36]  it precludes me
[2111.36 --> 2112.22]  from wanting to learn
[2112.22 --> 2113.20]  Ansible because I think
[2113.20 --> 2114.84]  that's still time
[2114.84 --> 2115.78]  that would be well spent.
[2116.48 --> 2117.08]  Yeah, I do.
[2117.58 --> 2118.68]  What I have kind of felt
[2118.68 --> 2120.48]  about using Nix is,
[2120.70 --> 2121.06]  um,
[2121.40 --> 2121.58]  okay,
[2121.68 --> 2122.20]  this is going to be
[2122.20 --> 2122.82]  kind of a controversial
[2122.82 --> 2123.24]  statement,
[2123.44 --> 2123.64]  but,
[2124.34 --> 2125.02]  uh,
[2125.20 --> 2126.04]  this is the future
[2126.04 --> 2126.56]  of Linux.
[2127.18 --> 2128.10]  And this,
[2128.22 --> 2128.86]  a lot of what
[2128.86 --> 2129.38]  they're solving,
[2129.50 --> 2130.38]  it just should be done
[2130.38 --> 2131.04]  at the OS
[2131.04 --> 2132.06]  anyways.
[2132.06 --> 2133.20]  And it doesn't
[2133.20 --> 2134.40]  necessarily mean
[2134.40 --> 2135.40]  you don't still also
[2135.40 --> 2136.02]  need something
[2136.02 --> 2136.92]  like Ansible.
[2137.38 --> 2138.16]  Maybe for some
[2138.16 --> 2139.52]  small scale things,
[2139.58 --> 2139.78]  you know,
[2139.82 --> 2140.92]  if you have a few boxes,
[2141.42 --> 2142.22]  maybe with something
[2142.22 --> 2142.70]  like Nix,
[2142.74 --> 2143.30]  you could get away
[2143.30 --> 2143.90]  without something
[2143.90 --> 2144.34]  centralized.
[2144.90 --> 2145.48]  But if you have
[2145.48 --> 2146.26]  any kind of scale,
[2146.52 --> 2147.10]  you're obviously
[2147.10 --> 2147.64]  going to need tools
[2147.64 --> 2148.26]  to manage that.
[2148.68 --> 2150.34]  But I honestly think
[2150.34 --> 2151.34]  when I use Nix,
[2151.86 --> 2152.42]  I look at what
[2152.42 --> 2153.02]  Rails is doing,
[2153.16 --> 2153.98]  and I don't know
[2153.98 --> 2154.40]  how they're going
[2154.40 --> 2154.84]  to get there,
[2155.38 --> 2156.30]  but they're ultimately
[2156.30 --> 2157.10]  going to end up here.
[2157.82 --> 2158.60]  And same with
[2158.60 --> 2159.30]  what Canonical
[2159.30 --> 2159.62]  needs to do
[2159.62 --> 2160.06]  with Ubuntu.
[2161.32 --> 2162.50]  And it's so,
[2162.62 --> 2163.22]  in some ways,
[2163.26 --> 2163.92]  I like using it
[2163.92 --> 2165.34]  because it's just,
[2166.48 --> 2167.72]  I think it's how
[2167.72 --> 2168.42]  I'm going to use
[2168.42 --> 2169.10]  Linux now
[2169.10 --> 2170.72]  for the future
[2170.72 --> 2172.08]  when I'm not
[2172.08 --> 2173.46]  deploying a desktop
[2173.46 --> 2173.88]  system.
[2173.98 --> 2174.56]  And I'm not even
[2174.56 --> 2175.92]  convinced it may
[2175.92 --> 2176.76]  actually ultimately
[2176.76 --> 2177.38]  end up using it
[2177.38 --> 2178.24]  for a desktop system
[2178.24 --> 2179.12]  as well.
[2179.46 --> 2180.22]  Especially like a
[2180.22 --> 2180.76]  system here in the
[2180.76 --> 2181.52]  studio that's pretty
[2181.52 --> 2182.04]  static.
[2183.00 --> 2183.32]  I think the
[2183.32 --> 2184.22]  counterpoint to that
[2184.22 --> 2185.86]  is what Red Hat,
[2185.98 --> 2186.46]  for example,
[2186.46 --> 2187.26]  I know it well,
[2187.34 --> 2188.00]  are doing with
[2188.00 --> 2189.36]  the Red Hat
[2189.36 --> 2190.74]  Core OS operating
[2190.74 --> 2191.34]  system at the
[2191.34 --> 2191.50]  minute,
[2191.64 --> 2192.56]  Fedora Core OS
[2192.56 --> 2192.96]  if you want to
[2192.96 --> 2193.48]  try out the
[2193.48 --> 2194.84]  upstream version.
[2195.52 --> 2196.22]  Everything is
[2196.22 --> 2197.78]  configured declaratively
[2197.78 --> 2198.86]  up front,
[2199.04 --> 2199.22]  right?
[2199.28 --> 2199.94]  So you say,
[2200.06 --> 2200.74]  I want this
[2200.74 --> 2201.60]  NIC to have
[2201.60 --> 2202.46]  this IP address.
[2202.94 --> 2203.74]  I want these
[2203.74 --> 2204.96]  storage disks to
[2204.96 --> 2205.88]  be configured to
[2205.88 --> 2206.56]  this mount point,
[2206.64 --> 2207.24]  that kind of thing.
[2208.08 --> 2209.04]  That's all done
[2209.04 --> 2209.56]  through an
[2209.56 --> 2210.26]  ignition config
[2210.26 --> 2210.66]  file.
[2210.90 --> 2211.90]  You supply that
[2211.90 --> 2212.70]  to the VM
[2212.70 --> 2213.52]  or to the
[2213.52 --> 2215.44]  machine when it
[2215.44 --> 2216.00]  boots up,
[2216.00 --> 2217.10]  and it then
[2217.10 --> 2218.32]  configures itself
[2218.32 --> 2219.52]  based on that
[2219.52 --> 2221.04]  instantiation kind
[2221.04 --> 2222.10]  of request.
[2223.06 --> 2224.00]  And it seems to
[2224.00 --> 2224.72]  me like NICS is
[2224.72 --> 2225.60]  operating in a
[2225.60 --> 2226.46]  similar space where
[2226.46 --> 2227.44]  the operating system
[2227.44 --> 2228.16]  is almost like
[2228.16 --> 2229.78]  read only and
[2229.78 --> 2230.44]  everything is kind
[2230.44 --> 2231.42]  of given to it.
[2231.50 --> 2232.12]  It's like this
[2232.12 --> 2233.90]  blank canvas onto
[2233.90 --> 2234.70]  which everything gets
[2234.70 --> 2236.08]  painted straight
[2236.08 --> 2236.42]  away.
[2237.06 --> 2237.84]  NICS OS itself
[2237.84 --> 2238.70]  managed to make
[2238.70 --> 2239.76]  base arch feel
[2239.76 --> 2240.08]  bloated.
[2240.20 --> 2240.78]  It's really
[2240.78 --> 2241.12]  nothing.
[2241.26 --> 2241.86]  There's not a lot
[2241.86 --> 2242.72]  going on there.
[2242.72 --> 2245.56]  So what happens
[2245.56 --> 2246.22]  when you need to
[2246.22 --> 2247.70]  do a rollback,
[2247.94 --> 2248.60]  for example,
[2248.60 --> 2249.34]  with my home
[2249.34 --> 2250.08]  assistant VM
[2250.08 --> 2251.34]  running on top
[2251.34 --> 2251.92]  of Proxmox,
[2252.16 --> 2253.42]  if an upgrade
[2253.42 --> 2254.16]  goes sideways,
[2254.72 --> 2256.06]  all I do is
[2256.06 --> 2257.02]  roll back a
[2257.02 --> 2257.82]  specific snapshot
[2257.82 --> 2258.96]  which on the
[2258.96 --> 2259.82]  ZFS backend
[2259.82 --> 2260.64]  storage that
[2260.64 --> 2261.70]  Proxmox uses
[2261.70 --> 2263.48]  is simple.
[2264.26 --> 2265.28]  How does that
[2265.28 --> 2265.82]  work in NICS?
[2265.88 --> 2266.56]  Do you know yet?
[2266.56 --> 2268.24]  See, you probably
[2268.24 --> 2269.70]  wouldn't quite go
[2269.70 --> 2270.20]  through the same
[2270.20 --> 2270.78]  scenario.
[2271.00 --> 2272.00]  So what I've run
[2272.00 --> 2273.46]  into so far is
[2273.46 --> 2274.68]  there's two ways.
[2274.84 --> 2276.16]  You can YOLO it
[2276.16 --> 2277.06]  and just build and
[2277.06 --> 2278.46]  deploy, but you
[2278.46 --> 2279.24]  can also do like a
[2279.24 --> 2280.62]  build dash dash
[2280.62 --> 2281.06]  test.
[2281.56 --> 2281.98]  And that does
[2281.98 --> 2282.74]  everything and
[2282.74 --> 2284.86]  that's where it'll
[2284.86 --> 2285.30]  fail out.
[2285.44 --> 2286.18]  So they have this
[2286.18 --> 2286.84]  sort of switch
[2286.84 --> 2287.48]  command that you
[2287.48 --> 2287.68]  add.
[2287.80 --> 2288.86]  So once you
[2288.86 --> 2289.62]  verify that
[2289.62 --> 2290.40]  everything's sane,
[2290.50 --> 2291.40]  the config works,
[2291.86 --> 2293.46]  and like software
[2293.46 --> 2294.22]  building, when it
[2294.22 --> 2294.82]  fails to build,
[2294.88 --> 2295.28]  it'll give you
[2295.28 --> 2295.86]  errors and it'll
[2295.86 --> 2296.48]  tell you where in
[2296.48 --> 2297.14]  the config file,
[2297.20 --> 2297.70]  there might be a
[2297.70 --> 2298.32]  problem and stuff
[2298.32 --> 2298.70]  like that.
[2299.42 --> 2300.12]  And then once
[2300.12 --> 2300.84]  you've resolved all
[2300.84 --> 2301.98]  that, you do the
[2301.98 --> 2303.28]  switch command and
[2303.28 --> 2303.98]  it actually then
[2303.98 --> 2304.84]  deploys that as
[2304.84 --> 2305.40]  your production
[2305.40 --> 2305.90]  system.
[2306.68 --> 2307.46]  But by the time
[2307.46 --> 2308.10]  you've deployed it,
[2308.16 --> 2308.60]  you already know
[2308.60 --> 2309.26]  everything works.
[2309.40 --> 2310.08]  So there's no,
[2310.92 --> 2311.72]  you can roll back,
[2311.84 --> 2312.20]  but there's,
[2313.02 --> 2313.38]  it doesn't really,
[2313.46 --> 2313.70]  you don't really
[2313.70 --> 2314.58]  need to because
[2314.58 --> 2315.40]  you just don't,
[2315.48 --> 2315.86]  it doesn't,
[2315.94 --> 2316.56]  it doesn't actually
[2316.56 --> 2317.70]  switch over unless
[2317.70 --> 2318.72]  it actually successfully
[2318.72 --> 2319.72]  everything works.
[2321.08 --> 2321.82]  I mean, that's
[2321.82 --> 2322.26]  interesting.
[2323.32 --> 2324.08]  Obviously there's a
[2324.08 --> 2325.22]  paradigm shift there
[2325.22 --> 2325.62]  that I,
[2325.62 --> 2326.94]  I and you and
[2326.94 --> 2327.82]  we perhaps as a,
[2327.82 --> 2328.66]  as a show need to
[2328.66 --> 2329.24]  go through and
[2329.24 --> 2330.02]  kind of figure out
[2330.02 --> 2331.62]  what the future
[2331.62 --> 2332.22]  looks like if
[2332.22 --> 2332.70]  Nix is,
[2332.78 --> 2333.44]  is the way to go
[2333.44 --> 2334.20]  because you're
[2334.20 --> 2334.56]  certainly,
[2335.04 --> 2335.46]  you're certainly
[2335.46 --> 2336.36]  peaking my interest
[2336.36 --> 2337.30]  as we talk about it.
[2337.76 --> 2338.70]  I think it is kind
[2338.70 --> 2339.28]  of, for me,
[2339.30 --> 2339.84]  it's a discovery
[2339.84 --> 2340.44]  thing too.
[2341.20 --> 2341.96]  I'm thinking about
[2341.96 --> 2343.16]  making a Nix chat
[2343.16 --> 2343.84]  room on the
[2343.84 --> 2344.34]  matrix server
[2344.34 --> 2344.80]  because I think we
[2344.80 --> 2345.28]  have some Nix
[2345.28 --> 2346.68]  nerds in the
[2346.68 --> 2347.06]  audience.
[2347.40 --> 2348.08]  Just to kind of
[2348.08 --> 2348.66]  wrap this up,
[2348.86 --> 2349.62]  Alex, what I was
[2349.62 --> 2350.72]  thinking is with
[2350.72 --> 2351.36]  using Nix, I
[2351.36 --> 2352.42]  would keep things
[2352.42 --> 2353.58]  under very tight
[2353.58 --> 2354.16]  control.
[2355.12 --> 2355.52]  And then I think
[2355.52 --> 2356.22]  I kind of want to,
[2356.50 --> 2357.08]  and maybe you can
[2357.08 --> 2357.64]  tell me if I'm on
[2357.64 --> 2358.18]  the right track
[2358.18 --> 2358.42]  here.
[2359.16 --> 2360.10]  I think maybe I
[2360.10 --> 2360.60]  might stick with
[2360.60 --> 2361.06]  Home Assistant
[2361.06 --> 2361.50]  core.
[2361.62 --> 2361.96]  So it's going to
[2361.96 --> 2362.40]  be a pretty
[2362.40 --> 2363.20]  minimal Home
[2363.20 --> 2363.50]  Assistant.
[2363.70 --> 2364.06]  I'm going to
[2364.06 --> 2364.54]  get like the
[2364.54 --> 2365.32]  minimum viable
[2365.32 --> 2365.88]  Home Assistant
[2365.88 --> 2366.44]  rebuilt.
[2367.62 --> 2369.10]  And I, I
[2369.10 --> 2369.70]  wonder if I
[2369.70 --> 2370.50]  shouldn't, and
[2370.50 --> 2370.90]  maybe you could
[2370.90 --> 2371.64]  talk me off this
[2371.64 --> 2372.78]  ledge, consider
[2372.78 --> 2373.78]  going with Node
[2373.78 --> 2375.40]  Red for my
[2375.40 --> 2375.82]  automation.
[2376.02 --> 2376.50]  So I'm doing
[2376.50 --> 2377.84]  all my automations
[2377.84 --> 2378.40]  in something
[2378.40 --> 2379.64]  separate, something
[2379.64 --> 2380.68]  else outside of
[2380.68 --> 2381.14]  Home Assistant.
[2381.14 --> 2382.02]  Again, kind of
[2382.02 --> 2383.28]  building these
[2383.28 --> 2384.04]  data silos.
[2384.76 --> 2385.46]  And I'm also
[2385.46 --> 2386.30]  thinking, and I
[2386.30 --> 2386.86]  don't know how I
[2386.86 --> 2387.36]  would even manage
[2387.36 --> 2387.90]  to pull all this
[2387.90 --> 2388.34]  off at this
[2388.34 --> 2389.30]  point, but this
[2389.30 --> 2389.78]  is really the
[2389.78 --> 2390.44]  time to transition
[2390.44 --> 2391.00]  everything to
[2391.00 --> 2391.58]  MQTT.
[2391.92 --> 2392.66]  Like anything I
[2392.66 --> 2393.10]  can get over
[2393.10 --> 2394.30]  MQTT, do it,
[2394.34 --> 2395.48]  including like
[2395.48 --> 2396.50]  Z-Wave JS to
[2396.50 --> 2397.66]  MQTT and all of
[2397.66 --> 2397.84]  it.
[2398.64 --> 2399.36]  So do you think
[2399.36 --> 2399.74]  I'm on the right
[2399.74 --> 2400.06]  track?
[2400.12 --> 2400.84]  Is Node Red too
[2400.84 --> 2401.26]  far?
[2401.76 --> 2402.48]  Or is it just
[2402.48 --> 2403.28]  like, I don't
[2403.28 --> 2403.76]  know, I'm just,
[2404.32 --> 2404.74]  if I'm going to
[2404.74 --> 2405.62]  redo all this again,
[2405.68 --> 2406.54]  I don't really want
[2406.54 --> 2407.12]  to have to do it
[2407.12 --> 2408.20]  a second time.
[2409.36 --> 2410.30]  Node Red is
[2410.30 --> 2411.82]  brilliant for
[2411.82 --> 2413.70]  extremely complex
[2413.70 --> 2415.08]  automations where
[2415.08 --> 2415.78]  there are lots
[2415.78 --> 2419.48]  of if this, then
[2419.48 --> 2420.54]  that, and if
[2420.54 --> 2421.30]  this condition is
[2421.30 --> 2422.08]  true, then do
[2422.08 --> 2422.56]  that, you know,
[2422.96 --> 2423.72]  all that kind of
[2423.72 --> 2424.54]  really complicated,
[2424.66 --> 2425.06]  almost like
[2425.06 --> 2425.94]  programming logic.
[2427.02 --> 2428.12]  Where it's, I
[2428.12 --> 2428.92]  think, complete
[2428.92 --> 2429.68]  overkill is just
[2429.68 --> 2430.56]  a simple turn
[2430.56 --> 2431.40]  light on at 6
[2431.40 --> 2432.64]  AM type thing,
[2432.78 --> 2433.42]  turn heater on
[2433.42 --> 2433.92]  at 6 AM,
[2434.00 --> 2434.40]  whatever it is.
[2434.40 --> 2434.72]  Sure, sure,
[2434.92 --> 2435.10]  yeah.
[2435.10 --> 2437.62]  And I tend to
[2437.62 --> 2438.48]  have in my mind,
[2438.60 --> 2439.44]  as soon as I go
[2439.44 --> 2440.46]  beyond like 3 or
[2440.46 --> 2441.48]  4 or 5 kind of
[2441.48 --> 2442.34]  steps in an
[2442.34 --> 2443.54]  automation, I
[2443.54 --> 2444.94]  find the Home
[2444.94 --> 2445.78]  Assistant YAML
[2445.78 --> 2446.48]  based or the
[2446.48 --> 2447.22]  interface based
[2447.22 --> 2447.98]  automations quite
[2447.98 --> 2448.62]  cumbersome, and
[2448.62 --> 2449.22]  that's when I
[2449.22 --> 2449.78]  reach for Node
[2449.78 --> 2449.98]  Red.
[2451.08 --> 2452.02]  I could see like
[2452.02 --> 2452.96]  80% of our
[2452.96 --> 2453.84]  automations wouldn't
[2453.84 --> 2455.18]  need that, but
[2455.18 --> 2456.62]  there is a niche
[2456.62 --> 2458.14]  there, like if so
[2458.14 --> 2458.96]  and so hasn't been
[2458.96 --> 2460.08]  home for so long
[2460.08 --> 2460.88]  and so and so is
[2460.88 --> 2461.96]  this far from here,
[2462.04 --> 2462.64]  then turn these
[2462.64 --> 2463.22]  things off.
[2463.22 --> 2464.16]  And then
[2464.16 --> 2466.26]  additionally, I
[2466.26 --> 2467.16]  hope at some
[2467.16 --> 2467.70]  point I'm going to
[2467.70 --> 2469.26]  have over MQTT
[2469.26 --> 2470.36]  all of my power
[2470.36 --> 2471.22]  information from the
[2471.22 --> 2471.98]  Victron system
[2471.98 --> 2472.70]  feeding in, and
[2472.70 --> 2473.10]  then I would be
[2473.10 --> 2473.78]  also looking at
[2473.78 --> 2475.66]  solar input and
[2475.66 --> 2476.80]  battery charge level
[2476.80 --> 2478.04]  and possibly doing
[2478.04 --> 2479.06]  automations based on
[2479.06 --> 2479.66]  that as well.
[2480.40 --> 2481.50]  MQTT is just so
[2481.50 --> 2483.30]  lightweight and it
[2483.30 --> 2484.30]  does all you need
[2484.30 --> 2485.00]  it to do in a
[2485.00 --> 2486.58]  really small little
[2486.58 --> 2487.36]  lightweight package.
[2487.72 --> 2488.30]  So I got an
[2488.30 --> 2488.56]  idea.
[2488.80 --> 2489.42]  So here's what we're
[2489.42 --> 2490.32]  going to do is you
[2490.32 --> 2491.16]  and Wes come out,
[2491.92 --> 2492.62]  we'll fly you out
[2492.62 --> 2493.62]  for episode 70
[2493.62 --> 2494.90]  and we'll do a
[2494.90 --> 2495.94]  bro build at the
[2495.94 --> 2496.28]  RV.
[2497.50 --> 2498.22]  We'll rebuild
[2498.22 --> 2499.06]  everything over the
[2499.06 --> 2499.42]  weekend.
[2499.42 --> 2500.34]  We'll record it for
[2500.34 --> 2500.74]  the show.
[2501.54 --> 2502.26]  You know, we'll go
[2502.26 --> 2503.14]  do some fancy
[2503.14 --> 2503.72]  driving.
[2504.16 --> 2504.96]  We'll make a whole
[2504.96 --> 2505.80]  thing out of it
[2505.80 --> 2506.72]  because I just don't
[2506.72 --> 2507.20]  know if I want to
[2507.20 --> 2507.86]  take all this on.
[2507.92 --> 2508.52]  Like we got to get
[2508.52 --> 2508.84]  Linux.
[2508.94 --> 2509.28]  We got to get
[2509.28 --> 2510.16]  Nix OS going on
[2510.16 --> 2510.68]  in M1.
[2510.88 --> 2512.36]  I got to get
[2512.36 --> 2513.42]  everything rebuilt.
[2513.52 --> 2514.04]  I got to get all
[2514.04 --> 2514.56]  of the individual
[2514.56 --> 2515.40]  Docker services
[2515.40 --> 2515.92]  restored.
[2516.02 --> 2516.68]  Got to migrate
[2516.68 --> 2517.48]  data.
[2517.94 --> 2518.70]  Then we got to get
[2518.70 --> 2519.22]  everything using
[2519.22 --> 2519.86]  MQTT.
[2520.00 --> 2520.30]  Got to get
[2520.30 --> 2521.30]  Node-red going.
[2521.30 --> 2522.72]  Should talk about
[2522.72 --> 2523.40]  my daily rate,
[2523.52 --> 2523.66]  huh?
[2524.30 --> 2524.60]  Yeah.
[2524.80 --> 2525.72]  I mean, you know,
[2525.96 --> 2527.70]  maybe I could pay it
[2527.70 --> 2528.30]  in like sandwiches,
[2528.80 --> 2529.60]  delicious burgers,
[2529.94 --> 2530.98]  roads in the Pacific
[2530.98 --> 2531.36]  Northwest.
[2531.88 --> 2532.28]  There's a little
[2532.28 --> 2533.24]  Asian place just
[2533.24 --> 2534.02]  across the road from
[2534.02 --> 2535.82]  the studio, which I
[2535.82 --> 2536.78]  love that place.
[2537.08 --> 2537.64]  It is good.
[2538.20 --> 2538.82]  That's when Noah
[2538.82 --> 2539.60]  comes in to visit.
[2539.70 --> 2540.14]  That's the first
[2540.14 --> 2541.22]  place he and I go.
[2541.32 --> 2541.74]  And if we don't
[2541.74 --> 2543.16]  have time, but I
[2543.16 --> 2543.70]  know he's coming,
[2543.80 --> 2545.02]  I'll order ahead for
[2545.02 --> 2545.24]  him.
[2545.24 --> 2546.42]  So I remember
[2546.42 --> 2547.84]  this is a very old
[2547.84 --> 2548.58]  Linux action show
[2548.58 --> 2549.34]  where he was waxing
[2549.34 --> 2549.92]  lyrical, I think,
[2549.96 --> 2550.84]  about Panda Express
[2550.84 --> 2551.48]  and you were like,
[2551.74 --> 2552.60]  dude, it's a chain.
[2553.94 --> 2554.92]  He does love his
[2554.92 --> 2555.76]  Chinese food, though.
[2556.14 --> 2556.46]  I don't know.
[2556.50 --> 2557.14]  We just think about it.
[2557.14 --> 2557.44]  We got to do
[2557.44 --> 2558.16]  something for episode
[2558.16 --> 2558.70]  70.
[2558.70 --> 2559.34]  And I'm just saying
[2559.34 --> 2560.10]  you come out here.
[2560.44 --> 2560.78]  I mean, you know,
[2560.80 --> 2561.64]  JB will put you up.
[2562.14 --> 2562.94]  It's not long, is it?
[2562.98 --> 2563.86]  It's probably what sort
[2563.86 --> 2564.70]  of May, June sort of
[2564.70 --> 2564.96]  time.
[2565.02 --> 2566.10]  Yeah, maybe we'll see.
[2566.70 --> 2567.46]  Watch this space.
[2568.10 --> 2569.12]  We need to issue a
[2569.12 --> 2569.98]  correction on the show.
[2570.40 --> 2571.64]  Samuel G writes in
[2571.64 --> 2572.88]  about the Argon Aeon
[2572.88 --> 2574.50]  4-Bay Raspberry Pi NAS
[2574.50 --> 2575.26]  case that we covered
[2575.26 --> 2576.00]  last episode.
[2576.56 --> 2576.98]  Hi, guys.
[2577.04 --> 2577.70]  I love the show.
[2577.82 --> 2578.60]  I think you might have
[2578.60 --> 2579.90]  read the Argon Aeon
[2579.90 --> 2580.94]  announcement wrong.
[2581.38 --> 2582.10]  You referred to the
[2582.10 --> 2583.48]  base model as $700,
[2584.14 --> 2585.10]  but I think that's
[2585.10 --> 2586.10]  actually an HK money.
[2586.90 --> 2588.66]  In US dollars, it's
[2588.66 --> 2590.04]  only about $120, which
[2590.04 --> 2591.60]  is a pretty good price
[2591.60 --> 2592.70]  if you look at it.
[2592.98 --> 2593.90]  So, yes, thank you
[2593.90 --> 2594.64]  for writing in and
[2594.64 --> 2595.54]  letting us know that
[2595.54 --> 2597.44]  we can't do currency
[2597.44 --> 2598.00]  conversions.
[2598.36 --> 2598.84]  No, you know what?
[2598.84 --> 2599.86]  It was my bad because
[2599.86 --> 2601.30]  I grabbed it and I
[2601.30 --> 2602.18]  put it in the dock,
[2602.18 --> 2603.56]  but I didn't note
[2603.56 --> 2604.12]  the currency.
[2604.90 --> 2605.78]  And so I just assumed
[2605.78 --> 2607.12]  it was US because it
[2607.12 --> 2607.58]  was like, you know,
[2607.62 --> 2608.12]  it had been a couple
[2608.12 --> 2608.80]  hours because I'm a
[2608.80 --> 2609.00]  dummy.
[2609.56 --> 2610.72]  Also, Samuel sent that
[2610.72 --> 2612.64]  in as a boost with a
[2612.64 --> 2614.10]  value for value podcast
[2614.10 --> 2614.36]  app.
[2614.84 --> 2615.70]  That's pretty cool.
[2616.06 --> 2616.48]  Very cool.
[2616.48 --> 2618.50]  And Gene sent, oh, I
[2618.50 --> 2619.26]  meant to bring it in the
[2619.26 --> 2620.20]  studio with me, Alex,
[2620.30 --> 2622.68]  but Gene heard about
[2622.68 --> 2623.88]  the temperature issues
[2623.88 --> 2624.92]  we've been having in
[2624.92 --> 2626.92]  the studio garage server
[2626.92 --> 2628.56]  room over the summer.
[2628.56 --> 2631.18]  and he built a Wi-Fi
[2631.18 --> 2632.62]  sensor for me to put
[2632.62 --> 2632.98]  in there.
[2633.12 --> 2634.30]  That is so cool.
[2634.36 --> 2634.86]  I meant to bring it
[2634.86 --> 2635.66]  down here for you.
[2636.46 --> 2637.36]  So that way you could
[2637.36 --> 2638.72]  look at his handiwork.
[2638.80 --> 2640.06]  So I'll show it to you
[2640.06 --> 2640.94]  after the show.
[2641.98 --> 2643.22]  But of course, it's
[2643.22 --> 2644.12]  using ESP home.
[2644.34 --> 2645.92]  So it should be no
[2645.92 --> 2647.64]  problem to get it
[2647.64 --> 2648.96]  working with home
[2648.96 --> 2649.72]  assistant here in the
[2649.72 --> 2649.98]  studio.
[2649.98 --> 2650.64]  And we'll be able to
[2650.64 --> 2651.94]  monitor the temperature
[2651.94 --> 2653.32]  out there, which I'm
[2653.32 --> 2653.70]  going to get this
[2653.70 --> 2654.60]  installed once we have
[2654.60 --> 2655.46]  the rack in its final
[2655.46 --> 2655.86]  position.
[2656.24 --> 2657.02]  So thank you, Gene,
[2657.08 --> 2657.70]  for sending that in.
[2657.74 --> 2658.38]  He sent that in a bit
[2658.38 --> 2660.28]  ago, and the plan is
[2660.28 --> 2661.22]  to deploy that soon.
[2662.24 --> 2663.00]  Yeah, I mean, if I
[2663.00 --> 2663.50]  come out there, we
[2663.50 --> 2664.68]  should do that and
[2664.68 --> 2666.58]  deploy a fleet of
[2666.58 --> 2667.62]  sensors, not just one.
[2667.94 --> 2668.52]  Oh, man, if you
[2668.52 --> 2669.46]  actually came out here,
[2669.62 --> 2671.08]  yeah, we'd have a lot.
[2671.18 --> 2672.02]  There's probably like a
[2672.02 --> 2672.94]  dozen things we could
[2672.94 --> 2673.18]  do.
[2674.02 --> 2675.60]  Bearded Tech sent in
[2675.60 --> 2677.70]  something so rad.
[2678.04 --> 2678.82]  And I say rad,
[2678.94 --> 2679.78]  ironically awesome.
[2680.38 --> 2681.54]  I got feedback that I
[2681.54 --> 2682.10]  should stop saying
[2682.10 --> 2682.38]  rad.
[2682.50 --> 2682.72]  No.
[2684.24 --> 2684.60]  No.
[2685.04 --> 2685.68]  I will not.
[2686.52 --> 2687.26]  Anyways, Bearded
[2687.26 --> 2689.14]  Tech has written this
[2689.14 --> 2690.34]  piece of software called
[2690.34 --> 2690.74]  Fever.
[2691.38 --> 2692.56]  And you got to look at
[2692.56 --> 2693.00]  this, Alex.
[2693.08 --> 2694.54]  Go look at his GitHub
[2694.54 --> 2695.16]  page there.
[2695.58 --> 2697.56]  It's a Frigate event
[2697.56 --> 2698.36]  video recorder.
[2698.46 --> 2699.12]  Have you seen this?
[2699.80 --> 2700.82]  Yeah, only because you
[2700.82 --> 2701.58]  put it in the doc, and
[2701.58 --> 2702.82]  it looks awesome.
[2703.10 --> 2705.22]  I am going to be adding
[2705.22 --> 2706.04]  this to my Frigate
[2706.04 --> 2706.86]  arsenal pretty soon.
[2707.24 --> 2707.48]  Yeah.
[2707.60 --> 2708.46]  So it lets you store
[2708.46 --> 2709.34]  video independently of
[2709.34 --> 2710.52]  Frigate, but it also has
[2710.52 --> 2711.18]  some Home Assistant
[2711.18 --> 2712.60]  integrations for
[2712.60 --> 2713.28]  notifications.
[2714.06 --> 2715.28]  You can get frames in
[2715.28 --> 2715.80]  Home Assistant.
[2716.48 --> 2717.38]  It makes browsing it
[2717.38 --> 2717.82]  really easy.
[2717.88 --> 2718.68]  He's been working on
[2718.68 --> 2719.56]  mobile support, so if
[2719.56 --> 2720.82]  you got one of them
[2720.82 --> 2722.18]  internet phones like Alex
[2722.18 --> 2723.64]  does, you can still look
[2723.64 --> 2723.92]  at it.
[2724.06 --> 2724.74]  You can look at your
[2724.74 --> 2725.98]  vidges in the web
[2725.98 --> 2726.56]  viewer.
[2726.56 --> 2729.46]  Like an internet phone is
[2729.46 --> 2730.50]  a special thing these
[2730.50 --> 2730.98]  days.
[2731.18 --> 2733.08]  I got to give you crap,
[2733.18 --> 2733.42]  I guess.
[2733.48 --> 2733.82]  I don't know.
[2735.38 --> 2736.20]  You know, have you seen
[2736.20 --> 2737.96]  the prices of the Coral,
[2738.08 --> 2739.42]  like the little AI kind of
[2739.42 --> 2741.38]  USB sticks that work really
[2741.38 --> 2741.60]  well?
[2741.74 --> 2741.98]  Are they crazy?
[2742.60 --> 2742.88]  Yeah.
[2742.98 --> 2744.44]  So I paid, I think, like
[2744.44 --> 2746.96]  $30 or $40 over MSRP.
[2747.16 --> 2748.38]  They're going for over $200.
[2749.00 --> 2749.88]  Oh my gosh.
[2749.98 --> 2750.84]  Like more than double.
[2751.00 --> 2752.10]  It's kind of crazy.
[2752.70 --> 2755.02]  So Bearded Tech has a
[2755.02 --> 2756.60]  GitHub page up with this
[2756.60 --> 2757.74]  Fever app on there, and
[2757.74 --> 2758.38]  it's super cool.
[2758.48 --> 2759.36]  He's also got a Docker
[2759.36 --> 2761.26]  Compose, if that's how
[2761.26 --> 2762.02]  you, you know, if you're
[2762.02 --> 2763.32]  still using containers.
[2764.70 --> 2766.00]  Like a caveman.
[2766.20 --> 2767.22]  I don't use containers
[2767.22 --> 2768.50]  anymore, but if you're
[2768.50 --> 2769.48]  still using containers,
[2769.58 --> 2770.14]  he's got a Docker
[2770.14 --> 2771.28]  Compose, good to go.
[2773.20 --> 2773.82]  You know, what's
[2773.82 --> 2774.74]  interesting is I see in
[2774.74 --> 2775.88]  his config file that he's
[2775.88 --> 2776.96]  got a whole tail scale
[2776.96 --> 2777.42]  section.
[2778.20 --> 2778.60]  Oh yeah?
[2778.60 --> 2781.14]  Yeah, he's been, he's
[2781.14 --> 2782.02]  been dropping me hints
[2782.02 --> 2782.90]  about stuff he's working
[2782.90 --> 2783.16]  on.
[2783.74 --> 2784.38]  It's really good.
[2784.44 --> 2785.34]  And it's GPL too.
[2785.86 --> 2786.08]  So.
[2786.32 --> 2786.68]  Nice.
[2786.78 --> 2787.16]  It's free.
[2787.48 --> 2787.72]  Yeah.
[2788.02 --> 2788.94]  So go check that out.
[2788.98 --> 2789.68]  We'll have a link to that
[2789.68 --> 2790.40]  in the show notes.
[2791.12 --> 2791.92]  Well, very good.
[2792.06 --> 2793.58]  I hope to see lots of
[2793.58 --> 2794.98]  you at our meetup on
[2794.98 --> 2796.18]  April the 9th in Raleigh.
[2796.96 --> 2798.18]  Like we said, please make
[2798.18 --> 2799.18]  sure if you are coming,
[2799.26 --> 2800.42]  you update the page so
[2800.42 --> 2801.66]  we can get an accurate
[2801.66 --> 2802.92]  idea of numbers so we
[2802.92 --> 2804.28]  don't order too much
[2804.28 --> 2806.96]  meat or too many other
[2806.96 --> 2807.76]  treats for you.
[2808.60 --> 2809.00]  Right.
[2809.28 --> 2810.12]  And I want to put the
[2810.12 --> 2811.06]  word out there, Alex.
[2811.12 --> 2811.92]  I'd like you all to join
[2811.92 --> 2813.36]  me, including you on
[2813.36 --> 2815.48]  March 31st at jblive.tv,
[2815.66 --> 2816.16]  4 p.m.
[2816.22 --> 2818.16]  Seattle time, 7 p.m.
[2818.22 --> 2820.18]  Alex time, 11 p.m.
[2820.22 --> 2820.58]  London.
[2821.18 --> 2822.90]  We're doing an AMA and
[2822.90 --> 2823.60]  any of the hosts are
[2823.60 --> 2823.88]  welcome.
[2824.00 --> 2824.80]  I know nobody's actually
[2824.80 --> 2825.56]  said they're showing up,
[2825.60 --> 2826.24]  but we're going to do an
[2826.24 --> 2826.54]  AMA.
[2826.64 --> 2827.28]  We're going to help people
[2827.28 --> 2828.28]  get set up on Matrix.
[2828.74 --> 2831.44]  And the big thing, I'm
[2831.44 --> 2832.36]  giving away some Bitcoin.
[2832.64 --> 2833.72]  I'm going to help you get
[2833.72 --> 2834.82]  your value for value
[2834.82 --> 2835.92]  podcasting app.
[2835.98 --> 2836.52]  So I've been talking
[2836.52 --> 2837.82]  about Fountain on some of
[2837.82 --> 2838.38]  the other shows.
[2838.60 --> 2839.72]  It has a little boost
[2839.72 --> 2840.70]  feature in there, but the
[2840.70 --> 2841.50]  hardest part is getting
[2841.50 --> 2841.98]  set up.
[2842.54 --> 2843.14]  So I'm going to give away
[2843.14 --> 2843.80]  some Bitcoin to help
[2843.80 --> 2844.84]  people get set up so that
[2844.84 --> 2846.98]  way they can try out
[2846.98 --> 2848.12]  boosting, boosting their
[2848.12 --> 2849.16]  favorite podcast creators
[2849.16 --> 2850.14]  out there and maybe one
[2850.14 --> 2851.22]  day free software projects
[2851.22 --> 2853.46]  because the bearded tech
[2853.46 --> 2855.40]  who's working on fever is
[2855.40 --> 2856.14]  integrating lightning
[2856.14 --> 2858.04]  payments so you can send a
[2858.04 --> 2859.00]  boost to his project to
[2859.00 --> 2859.38]  support it.
[2859.46 --> 2860.60]  I think that's so cool.
[2860.76 --> 2863.04]  So join me, AMA, Matrix
[2863.04 --> 2865.76]  Setup, Bitcoin giveaway, and I
[2865.76 --> 2866.96]  have a special guest joining
[2866.96 --> 2868.78]  me do a little interview on
[2868.78 --> 2869.32]  the live stream.
[2869.66 --> 2871.02]  So it's March 31st, 4pm
[2871.02 --> 2872.98]  Seattle, 7pm New York, 11pm
[2872.98 --> 2874.80]  London at jblav.tv.
[2875.58 --> 2876.28]  And for all the ways to get
[2876.28 --> 2877.40]  in touch with us, you can go
[2877.40 --> 2879.12]  to selfhosted.show slash
[2879.12 --> 2879.50]  contact.
[2879.84 --> 2881.48]  There's a form over there you
[2881.48 --> 2883.28]  can fill in and get your
[2883.28 --> 2883.92]  message on the show.
[2884.70 --> 2885.86]  Pew, pew, pew, pew.
[2886.18 --> 2887.74]  You can also hit us up on
[2887.74 --> 2888.08]  Discord.
[2888.60 --> 2889.72]  We got information about that
[2889.72 --> 2890.82]  at selfhosted.show slash
[2890.82 --> 2891.16]  Discord.
[2891.40 --> 2892.84]  And the self-hosted matrix
[2892.84 --> 2895.46]  rooms at colony.jupiterbroadcasting.com.
[2895.46 --> 2896.60]  And of course, this here
[2896.60 --> 2898.12]  podcast is at selfhosted
[2898.12 --> 2899.10]  show on Twitter.
[2900.22 --> 2901.58]  As always, thank you so
[2901.58 --> 2902.10]  much for listening,
[2902.22 --> 2902.50]  everybody.
[2902.66 --> 2903.92]  That was selfhosted.show
[2903.92 --> 2905.02]  slash 67.
