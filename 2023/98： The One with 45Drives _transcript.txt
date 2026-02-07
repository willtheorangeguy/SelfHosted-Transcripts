[0.00 --> 2.74]  Well, this piece of news started over in your neck of the woods over at Amazon.
[3.22 --> 6.98]  They're looking to discontinue celebrity voices for their lady cylinders.
[7.74 --> 9.04]  Even if you paid for them.
[9.32 --> 13.70]  If you bought them, if you bought Samuel L. Jackson's voice for your lady tube,
[14.62 --> 15.66]  they're taking it out.
[15.86 --> 17.20]  In the next few months, they're going to pull them.
[17.62 --> 19.98]  I can't even imagine the home assistant doing this kind of thing
[19.98 --> 21.18]  with their year of the voice,
[21.30 --> 27.84]  like somehow retroactively pulling Popey's voice out of the system.
[27.84 --> 30.16]  You know, I want my Popey forever.
[30.70 --> 31.72]  This is what made me think of it.
[32.06 --> 34.56]  Just as home assistant is doing the year of voice,
[34.70 --> 41.46]  it seems that Amazon is undercutting and underfunding their smart assistant division.
[41.78 --> 43.48]  All the celebrity voices are going away.
[44.12 --> 45.44]  No real reason has been given.
[45.76 --> 50.76]  If you want to go through the rigmarole of going to support and asking them for a refund,
[50.86 --> 51.72]  they'll do it for you.
[51.78 --> 54.54]  But they can't be bothered to automatically credit your account
[54.54 --> 56.04]  because there's just no way they could know.
[56.04 --> 58.18]  How could they know?
[58.82 --> 59.00]  You know?
[60.18 --> 63.54]  And then, you know, I heard this, Alex, and I thought,
[63.72 --> 66.84]  there is this kind of reoccurring theme that we see,
[67.04 --> 68.92]  especially with Amazon and these others.
[69.48 --> 72.62]  Google also just announced that they are discontinuing integration
[72.62 --> 74.64]  with many of the to-do services out there,
[74.88 --> 76.94]  like AnyDo and others for Google Assistant.
[77.26 --> 79.10]  They're just turning off the API access.
[79.36 --> 80.82]  You know, they're not really going to do that anymore.
[80.82 --> 86.44]  So if you use the Google Assistant to add to-dos to your list,
[86.50 --> 87.50]  you're not going to do that anymore.
[87.76 --> 89.14]  You can still use the Google apps, though.
[90.04 --> 92.82]  It's like they just keep changing the contract on us.
[93.26 --> 95.24]  Amazon also just had to pay out a lawsuit,
[95.82 --> 98.44]  quite a bit of money for Ring,
[98.86 --> 101.02]  sharing more than just what was authorized,
[101.24 --> 102.92]  but sharing all kinds of videos.
[103.86 --> 107.28]  Almost every week, we see something that makes me shake my head and go,
[107.28 --> 109.06]  this is why we got a self-host,
[109.14 --> 110.94]  and this is why I think I'm getting more excited
[110.94 --> 112.80]  about Home Assistant's ear of the voice
[112.80 --> 115.02]  and the work they're doing over there.
[115.64 --> 118.44]  There's a lot of things they could be spending time
[118.44 --> 119.78]  and energy scaling out on,
[119.98 --> 122.76]  and the little bit of experimentation I've done,
[122.82 --> 124.12]  I'm really glad this is it,
[124.40 --> 127.18]  because it's producing upstream projects
[127.18 --> 130.30]  that you can use for other stuff outside of Home Assistant as well.
[130.80 --> 131.76]  So it's like a double win.
[131.96 --> 133.52]  Well, it's not just Amazon
[133.52 --> 135.76]  that have been having a bit of a weird week
[135.76 --> 140.02]  with regards to doing DRM-type stuff,
[140.26 --> 141.44]  I suppose, or having issues.
[141.82 --> 145.12]  The MB project had a hack this week,
[145.44 --> 147.84]  so just a public safety announcement, really.
[148.24 --> 149.26]  If you're running an MB server,
[149.42 --> 152.04]  make sure that you are up to date on your patches.
[152.22 --> 154.22]  There was a remote code execution vulnerability
[154.22 --> 157.36]  combined with a proxy header vulnerability
[157.36 --> 159.84]  recently fixed in the beta channel,
[159.84 --> 161.14]  and this allowed an attacker
[161.14 --> 164.06]  to gain administrative access on such systems.
[164.06 --> 165.78]  Oh, not good, Alex.
[166.00 --> 166.92]  Not good at all.
[167.36 --> 167.94]  Good to know.
[168.56 --> 171.08]  Well, speaking of cleaning things up and purging,
[171.52 --> 174.48]  I was kind of curious about your habits
[174.48 --> 176.66]  in terms of going through your file server
[176.66 --> 178.90]  and determining if it's time to clean things up
[178.90 --> 180.14]  and where you draw the line.
[180.48 --> 181.44]  And of course, I'd be curious to know
[181.44 --> 182.62]  where the audience draws their line.
[182.88 --> 184.42]  I was looking at the file server,
[184.66 --> 187.46]  and I was getting down to 100 gigs free.
[187.62 --> 189.82]  And that's kind of my red line, right?
[189.82 --> 192.30]  That's like, because when you start getting low on space,
[192.48 --> 195.14]  it just becomes exponentially harder
[195.14 --> 196.42]  to migrate that data.
[196.68 --> 198.06]  It's always easier to do it
[198.06 --> 199.12]  before you run out of space.
[199.30 --> 201.22]  And so I started looking through there,
[201.28 --> 203.30]  and I was using various command line tools,
[203.36 --> 204.84]  because this is over in SSH connection,
[205.12 --> 208.88]  to try to suss out what is the most large,
[208.98 --> 210.06]  like what are the largest files,
[210.12 --> 212.20]  what's the most storage dedicated to.
[213.06 --> 215.28]  And one of the things I saw in there
[215.28 --> 217.38]  was my vlog source files.
[217.48 --> 219.04]  Because, you know, I did like 60 vlog episodes
[219.04 --> 220.44]  years ago on YouTube.
[221.92 --> 224.18]  And I kept all the source files
[224.18 --> 226.08]  because there's a lot of drone footage in there
[226.08 --> 228.56]  of our neighborhood and trips that we went on
[228.56 --> 230.02]  and locations all over the country.
[230.22 --> 231.50]  And Noah crushing it into a tree.
[231.88 --> 232.64]  Sure, yeah.
[232.88 --> 234.34]  And there's also probably clips of the kids
[234.34 --> 236.04]  being young and cute, just that kind of stuff.
[236.06 --> 237.66]  So I just decided to always keep it.
[237.94 --> 241.96]  But I've never once in years ever gone back to it.
[241.96 --> 242.82]  And looked at it.
[243.74 --> 245.18]  So then I started looking at it.
[245.20 --> 246.70]  And it's, you know, a couple of hundred gigs.
[246.80 --> 248.98]  Actually, I think it's like a terabyte worth of stuff.
[249.56 --> 251.82]  And it would be such a huge job to go through
[251.82 --> 254.40]  and extract those ginormous raw files anyways.
[255.24 --> 257.68]  And I have a lot of pictures from that time and era.
[257.84 --> 259.44]  Plus, I have the produced videos.
[260.06 --> 261.78]  Like, where do you draw the line
[261.78 --> 264.96]  on what you're going to clear out?
[265.12 --> 267.46]  Or do you just always plan to add more storage?
[267.52 --> 268.54]  Because that's what I've been debating.
[268.66 --> 270.18]  Like, should I really add more storage?
[270.18 --> 273.64]  Or could I go through and delete these 16 movies
[273.64 --> 276.44]  I'm never, ever, ever going to actually watch?
[276.68 --> 278.98]  And all these source files for these projects
[278.98 --> 280.96]  that I was doing years ago,
[281.10 --> 283.04]  video projects I was doing years ago,
[283.24 --> 285.00]  I'm never going to reopen those projects.
[285.08 --> 286.60]  I probably will never go through the source footage,
[286.60 --> 288.06]  even though I know there's stuff in there.
[288.82 --> 290.10]  Or do you hold it all,
[290.38 --> 291.62]  thinking like maybe one day
[291.62 --> 293.46]  some AI tool is going to come along,
[293.54 --> 295.40]  just scan it for you and categorize it for you
[295.40 --> 296.48]  and make it all retrievable?
[296.62 --> 297.62]  Like, I mean, I don't know.
[297.62 --> 298.40]  Like, what's your approach?
[298.72 --> 301.02]  Now there's an angle I hadn't considered for AI.
[301.02 --> 303.62]  Let's go through all my thousands of hours
[303.62 --> 305.02]  of drone footage that I took
[305.02 --> 307.06]  when I first got my first drone.
[307.56 --> 308.38]  Wouldn't, I mean, you know,
[308.40 --> 309.18]  as soon as you delete it,
[309.22 --> 309.78]  they're going to come out
[309.78 --> 311.20]  with some sort of project like that.
[311.28 --> 313.06]  That'll go through and auto-categorize,
[313.18 --> 314.50]  auto-tag, auto-locate.
[314.70 --> 316.86]  It's an interesting discussion, actually.
[317.16 --> 319.18]  And I think it speaks to a strategy
[319.18 --> 319.88]  that I adopted.
[319.88 --> 326.04]  So my storage is kind of divided into two halves.
[326.30 --> 327.90]  I've got an ephemeral area,
[328.06 --> 330.54]  which is typically what I use Merger FS for.
[330.86 --> 334.38]  And that is often for stuff which has been acquired,
[335.22 --> 336.50]  wink, wink, nudge, nudge.
[337.18 --> 338.00]  I don't know what you're talking about.
[338.10 --> 340.52]  And is very easily replaceable, you know?
[340.64 --> 343.86]  So commercially produced stuff, right?
[344.22 --> 346.46]  You could go buy that Blu-ray again
[346.46 --> 348.02]  and back it up again if you needed to.
[348.02 --> 348.80]  Yes, sir.
[349.34 --> 351.22]  I'm not talking about the drone footage
[351.22 --> 354.40]  of my trip to Croatia in 2016, for example,
[354.76 --> 357.20]  where I'm never going to be on that day again in history.
[357.82 --> 360.28]  And, you know, I think for me,
[360.36 --> 362.60]  anything that is completely irreplaceable,
[362.74 --> 366.30]  no matter how asinine it seems
[366.30 --> 368.58]  or how inconsequential it seems to you now,
[369.08 --> 371.76]  there may be some point in the future
[371.76 --> 372.88]  where you look back and think,
[372.96 --> 374.02]  oh, I wish I had the footage
[374.02 --> 376.82]  that I took in the car on the way from New York
[376.82 --> 378.84]  back to Washington when I went to the Ubuntu Summit,
[379.32 --> 381.40]  you know, eight years ago, whatever it was.
[382.02 --> 382.96]  Yeah, yeah, that's true.
[383.04 --> 384.34]  I would have a bunch of footage
[384.34 --> 385.40]  from that trip to New York.
[386.02 --> 386.38]  Yeah.
[386.54 --> 388.26]  And also, you know,
[388.26 --> 389.88]  if you get 20, 30 years down the road,
[389.98 --> 391.58]  that drone footage is a time capsule
[391.58 --> 394.34]  of an area that won't look anything like that anymore.
[394.80 --> 396.52]  And, you know, I think of it like this.
[396.52 --> 400.72]  So I put all of that data onto a ZFS mirror
[400.72 --> 402.72]  or an array of some kind.
[402.78 --> 404.20]  But in my case, I don't have more than,
[404.32 --> 406.24]  I've got a 14 terabyte ZFS mirror,
[406.50 --> 409.04]  which I then replicate to two different places.
[409.60 --> 411.74]  One in the closet next to me up here.
[411.86 --> 413.36]  So main server's in the basement,
[413.64 --> 414.94]  backup server is up here.
[415.32 --> 416.92]  And then I have my old UK server,
[416.98 --> 417.50]  as you probably know,
[417.54 --> 418.72]  if you've listened to the show for a while,
[419.16 --> 421.68]  where everything gets backed up to again.
[421.68 --> 424.54]  But I look at these files,
[424.84 --> 427.22]  I'm keeping them for myself, yes, on some level,
[427.36 --> 429.20]  because they're memories,
[429.50 --> 432.02]  they are moments in history, moments in time.
[433.30 --> 434.68]  But I look at photo albums
[434.68 --> 435.78]  when I go to my parents' houses
[435.78 --> 437.50]  and I look back at my parents
[437.50 --> 438.20]  when they were younger.
[439.20 --> 441.52]  And I see the way they look at each other,
[441.72 --> 443.04]  the clothes they're wearing,
[443.70 --> 445.08]  the vehicles they're driving,
[445.40 --> 446.60]  the locations they're at.
[446.82 --> 448.78]  And you can kind of piece together
[448.78 --> 450.34]  from the stuff you hear about your parents
[450.34 --> 451.70]  talking about over the years.
[452.54 --> 454.52]  You can piece together bits of their history
[454.52 --> 455.32]  that they've never,
[456.38 --> 457.64]  that they've either forgotten
[457.64 --> 459.92]  or just didn't have the time to tell you
[459.92 --> 461.18]  for whatever reason it might be.
[461.84 --> 462.44]  And so almost,
[462.56 --> 464.20]  I feel like I'm keeping some of those
[464.20 --> 467.22]  more unique memories,
[467.50 --> 468.58]  not for me,
[468.68 --> 469.86]  but for Kiddo,
[469.96 --> 470.92]  when she gets a bit older.
[472.08 --> 474.10]  Yeah, I could definitely see that
[474.10 --> 474.86]  with the vlog too,
[475.08 --> 476.44]  because there's a lot of footage of them
[476.44 --> 478.38]  and their home,
[478.64 --> 479.32]  their surroundings,
[479.32 --> 480.50]  all of that.
[481.04 --> 482.02]  The other aspect is,
[482.14 --> 483.06]  maybe she'll get,
[483.24 --> 483.58]  you know,
[483.62 --> 485.54]  the inevitable hand-me-down photo album,
[485.62 --> 486.12]  look at it and go,
[486.52 --> 487.56]  what the hell is this?
[487.70 --> 488.74]  And throw it in the bin.
[489.14 --> 490.36]  That seems equally as possible.
[490.44 --> 491.30]  But that's her decision.
[491.52 --> 491.68]  You know,
[491.72 --> 492.94]  at least she's then got the option.
[493.94 --> 494.12]  Yeah.
[494.40 --> 496.20]  So I decided to keep it for now.
[496.80 --> 498.26]  And I've gone through
[498.26 --> 500.06]  and just found other areas
[500.06 --> 501.08]  I can cut back.
[501.94 --> 502.12]  You know,
[502.12 --> 503.36]  one of the things that I discovered
[503.36 --> 505.90]  is when you have a lot of files,
[505.90 --> 507.66]  like Final Cut archives
[507.66 --> 509.22]  or a lot of media files
[509.22 --> 511.02]  or something like that,
[511.56 --> 514.38]  there aren't a lot of great command line tools
[514.38 --> 515.36]  to go through
[515.36 --> 516.96]  and analyze your usage
[516.96 --> 519.00]  and give you information quickly.
[519.54 --> 521.40]  I love NCDU.
[521.96 --> 523.78]  I've been using it for 200 years.
[523.98 --> 524.80]  I've been using it
[524.80 --> 526.18]  before your grandfather was born,
[526.40 --> 526.88]  but man,
[526.94 --> 527.44]  is it slow.
[527.58 --> 527.90]  I mean,
[528.50 --> 529.10]  so,
[529.36 --> 530.60]  so slow.
[530.68 --> 532.26]  To scan my file server here,
[532.26 --> 534.36]  it took 20 minutes.
[534.76 --> 535.34]  200 years,
[535.44 --> 535.58]  huh?
[535.80 --> 536.46]  200 years.
[536.60 --> 536.78]  Yeah.
[536.98 --> 537.20]  Yeah.
[537.28 --> 537.46]  Yeah.
[537.56 --> 537.76]  Yeah.
[537.76 --> 538.32]  Time traveler.
[539.00 --> 540.04]  So I went out
[540.04 --> 541.28]  and found a better tool.
[541.40 --> 542.08]  I found a better way.
[542.14 --> 543.08]  I believe it's a Rust app too.
[543.16 --> 543.84]  It's called Dua
[543.84 --> 545.92]  Disk Usage Analyzer
[545.92 --> 548.14]  and it did the same exact scan
[548.14 --> 549.22]  and I'm not even kidding
[549.22 --> 550.20]  in 15 seconds.
[550.50 --> 552.02]  It was way better.
[552.72 --> 553.16]  What?
[553.62 --> 554.02]  Yeah.
[554.20 --> 554.94]  Oh no.
[555.32 --> 555.58]  Yeah.
[555.62 --> 556.24]  It's way better.
[556.84 --> 558.26]  So it's called Dua
[558.26 --> 559.40]  the Disk Usage Analyzer
[559.40 --> 560.10]  and it's a tool
[560.10 --> 561.14]  to conveniently learn
[561.14 --> 562.56]  about the usage of your disk space
[562.56 --> 563.62]  and you can either
[563.62 --> 564.90]  just run it against a directory
[564.90 --> 566.08]  or you can put it
[566.08 --> 567.50]  in interactive mode
[567.50 --> 568.50]  and browse around
[568.50 --> 569.28]  the file system
[569.28 --> 570.54]  and get like actual
[570.54 --> 571.56]  bar graphs and stuff
[571.56 --> 572.30]  of the usage.
[572.86 --> 573.88]  And it works
[573.88 --> 574.72]  just like you would expect
[574.72 --> 575.74]  from a tool like this.
[576.08 --> 576.44]  Quick,
[576.90 --> 577.24]  easy.
[577.46 --> 577.98]  If you just want
[577.98 --> 578.70]  a command line output,
[578.78 --> 579.34]  you can get that
[579.34 --> 579.76]  or if you want
[579.76 --> 580.28]  the interactive
[580.28 --> 581.52]  kind of ncursus style.
[581.68 --> 582.04]  Of course,
[582.10 --> 582.76]  I was using this
[582.76 --> 583.94]  over an SSH connection
[583.94 --> 585.08]  and then
[585.08 --> 586.50]  the other thing it touts,
[586.56 --> 587.70]  I can't really testify
[587.70 --> 588.68]  either way,
[588.90 --> 589.40]  your honor,
[589.58 --> 590.70]  but the other thing
[590.70 --> 592.56]  that the defendant claims
[592.56 --> 594.32]  is that it also
[594.32 --> 595.42]  will delete faster
[595.42 --> 596.72]  than RM can delete
[596.72 --> 597.74]  large directories
[597.74 --> 598.48]  and large files.
[598.66 --> 599.60]  I will say
[599.60 --> 600.96]  they delete fast.
[601.18 --> 601.64]  I don't know
[601.64 --> 602.38]  if it deletes faster
[602.38 --> 602.92]  than RM,
[603.20 --> 604.08]  but it works,
[604.20 --> 605.50]  so I'm pleased with that.
[606.00 --> 606.82]  And I'll put a link
[606.82 --> 607.56]  to it in the show notes.
[607.68 --> 608.82]  It's a Rust tool,
[608.98 --> 609.84]  so it's available
[609.84 --> 610.40]  for Windows,
[610.60 --> 610.90]  Mac,
[611.42 --> 611.98]  and Linux.
[612.36 --> 612.88]  And if you want it
[612.88 --> 613.18]  on Linux,
[613.24 --> 613.64]  you can just like
[613.64 --> 614.30]  pull down the binary
[614.30 --> 614.92]  and just run it.
[615.28 --> 616.34]  It's also packaged up
[616.34 --> 616.98]  for Vue distros.
[617.66 --> 618.40]  Shouldn't you be saving
[618.40 --> 619.16]  the Rust tools
[619.16 --> 620.06]  for Linux Unplugged
[620.06 --> 621.20]  with your week of Rust
[621.20 --> 622.10]  that's going on?
[622.46 --> 622.92]  Dang it.
[623.34 --> 623.76]  Dang it.
[623.80 --> 624.00]  Well,
[624.08 --> 624.22]  yeah,
[624.22 --> 625.08]  I had to save the best one.
[625.12 --> 626.04]  This is really the best one
[626.04 --> 626.56]  of the bunch,
[626.62 --> 627.02]  I think.
[627.48 --> 627.76]  But you know,
[627.78 --> 629.26]  just managing this problem
[629.26 --> 630.58]  with my server,
[630.70 --> 632.16]  it does make me realize
[632.16 --> 633.08]  like there is
[633.08 --> 634.12]  a machine
[634.12 --> 635.24]  that has been missing
[635.24 --> 636.78]  from my life.
[636.78 --> 638.86]  And I have tried
[638.86 --> 639.72]  the Synologies,
[640.10 --> 640.52]  I have tried
[640.52 --> 641.38]  the QNAPs,
[641.50 --> 642.56]  I have tried
[642.56 --> 644.16]  using different NASs
[644.16 --> 645.04]  from like IX Systems,
[645.20 --> 645.60]  I've tried
[645.60 --> 647.02]  Intermediate Boxes,
[647.10 --> 647.98]  and then I've also done
[647.98 --> 648.84]  like Unix Surplus
[648.84 --> 649.80]  and bought old
[649.80 --> 651.70]  Big Towers
[651.70 --> 652.84]  and converted those
[652.84 --> 653.34]  into NASs,
[653.38 --> 653.72]  which are really
[653.72 --> 654.56]  Enterprise Systems.
[655.38 --> 655.88]  And so,
[656.02 --> 656.82]  we had a chance
[656.82 --> 657.36]  this week
[657.36 --> 658.60]  to chat with
[658.60 --> 659.10]  two gentlemen,
[659.26 --> 660.12]  Doug and Mitch
[660.12 --> 661.48]  from 45 Drives,
[661.52 --> 662.46]  who you're about to meet.
[662.90 --> 664.16]  And 45 Drives
[664.16 --> 665.08]  is setting off
[665.08 --> 666.30]  to develop a
[666.30 --> 667.06]  quote-unquote
[667.06 --> 668.46]  Homelab server
[668.46 --> 669.62]  that kind of sits
[669.62 --> 670.90]  in this area,
[670.96 --> 671.74]  that kind of bridges
[671.74 --> 672.92]  the gap between
[672.92 --> 674.36]  the Enterprise gear
[674.36 --> 676.28]  and the Consumer gear.
[676.60 --> 676.96]  You know,
[676.96 --> 677.96]  something that isn't
[677.96 --> 678.88]  $5,000,
[679.44 --> 680.36]  but something that isn't
[680.36 --> 680.84]  like $800,
[680.88 --> 681.30]  $900,
[682.02 --> 682.24]  right?
[682.54 --> 683.38]  Something you can afford
[683.38 --> 684.04]  for your Homelab,
[684.08 --> 685.24]  but it's a serious tool
[685.24 --> 686.60]  and something that
[686.60 --> 687.54]  obviously Alex and I
[687.54 --> 688.66]  would be very interested in.
[688.96 --> 689.76]  And so they joined us
[689.76 --> 690.16]  this week.
[690.16 --> 694.26]  tailscale.com
[694.26 --> 695.54]  slash self-hosted.
[695.62 --> 696.46]  Now you can get
[696.46 --> 698.44]  up to 100 devices
[698.44 --> 699.12]  for free
[699.12 --> 699.62]  when you go to
[699.62 --> 700.52]  tailscale.com
[700.52 --> 701.38]  slash self-hosted.
[701.64 --> 702.42]  It's a great way
[702.42 --> 703.10]  to support the show
[703.10 --> 704.00]  why you are checking out
[704.00 --> 704.90]  the best VPN
[704.90 --> 705.74]  in the business
[705.74 --> 706.20]  out there.
[706.56 --> 706.90]  Simple,
[707.22 --> 707.62]  secure,
[707.80 --> 708.72]  a flat mesh network
[708.72 --> 709.72]  built on top of
[709.72 --> 710.44]  WireGuard.
[710.80 --> 711.58]  And you can get it up
[711.58 --> 712.26]  in minutes.
[712.36 --> 713.02]  I know you don't have
[713.02 --> 713.66]  all day anymore
[713.66 --> 714.90]  to spend on these
[714.90 --> 715.60]  types of projects.
[715.72 --> 716.16]  I understand.
[716.36 --> 716.90]  I've been there.
[716.96 --> 717.32]  Of course,
[717.70 --> 718.50]  there's lots of ways
[718.50 --> 719.10]  you can do this,
[719.10 --> 720.20]  but tailscale is the
[720.20 --> 721.42]  ultimate accumulation
[721.42 --> 722.72]  of what we were hoping
[722.72 --> 724.46]  WireGuard would give us.
[724.54 --> 725.92]  It lets you easily
[725.92 --> 727.16]  manage your devices
[727.16 --> 727.54]  quickly.
[727.68 --> 728.38]  You got five minutes.
[728.44 --> 729.58]  You can get it on three systems.
[730.04 --> 731.30]  It'll set up a secure
[731.30 --> 732.60]  private mesh network
[732.60 --> 733.18]  where they connect
[733.18 --> 734.18]  directly to each other.
[734.30 --> 734.96]  And you can leave
[734.96 --> 735.68]  tailscale running
[735.68 --> 737.14]  persistently because
[737.14 --> 738.04]  it's intelligent enough
[738.04 --> 739.20]  what needs to route out
[739.20 --> 740.10]  to the tailscale network
[740.10 --> 740.86]  versus what should go
[740.86 --> 741.68]  to the public internet.
[742.12 --> 743.30]  That matters because
[743.30 --> 744.40]  leaving it on all the time
[744.40 --> 745.08]  means that network
[745.08 --> 745.90]  is all available
[745.90 --> 746.78]  all the time,
[747.08 --> 747.40]  always.
[747.74 --> 748.54]  So now you can start
[748.54 --> 749.64]  setting up your dashboards
[749.64 --> 751.08]  to use the tailscale IP
[751.08 --> 752.26]  or for home assistant,
[752.32 --> 752.88]  you can start using
[752.88 --> 753.66]  the tailscale IP
[753.66 --> 754.78]  instead of the internal IP.
[754.78 --> 755.72]  You could even start
[755.72 --> 756.52]  using DNS
[756.52 --> 757.52]  and tailscale support
[757.52 --> 758.00]  something called
[758.00 --> 759.08]  magic DNS as well.
[759.48 --> 760.14]  It starts getting
[760.14 --> 761.26]  ultimately powerful
[761.26 --> 762.66]  with up to 100 devices.
[762.96 --> 763.92]  You can start putting
[763.92 --> 764.94]  your containers in there,
[765.02 --> 765.92]  your VMs in there,
[765.98 --> 766.90]  every mobile device
[766.90 --> 767.22]  you've got.
[767.30 --> 767.98]  You can truly put
[767.98 --> 769.38]  every node on your tailnet
[769.38 --> 770.72]  and stop going over
[770.72 --> 771.34]  the public internet.
[771.50 --> 771.92]  I don't.
[772.34 --> 772.90]  I don't have any
[772.90 --> 774.12]  inbound firewall ports
[774.12 --> 775.32]  on any of my networks
[775.32 --> 776.80]  for any of my systems.
[776.98 --> 778.04]  It's all over tailscale.
[778.04 --> 779.42]  Now, even my phone syncing
[779.42 --> 780.58]  is over tailscale.
[780.74 --> 781.52]  I love WireGuard.
[781.60 --> 782.52]  I'm so happy to see this
[782.52 --> 782.96]  and they have lots
[782.96 --> 783.86]  of tooling too
[783.86 --> 785.48]  like tailscale send,
[786.38 --> 787.14]  tailscale SSH,
[787.20 --> 787.76]  all these tools
[787.76 --> 788.48]  that build on top
[788.48 --> 789.66]  of your tailnet
[789.66 --> 790.66]  to let you move
[790.66 --> 791.24]  things around
[791.24 --> 791.82]  and authenticate
[791.82 --> 792.64]  quickly and efficiently.
[792.76 --> 793.18]  And of course,
[793.26 --> 794.64]  there's ways to share
[794.64 --> 795.72]  with access controls
[795.72 --> 796.66]  that you can audit
[796.66 --> 797.98]  and there's integration
[797.98 --> 798.90]  with enterprise login
[798.90 --> 799.80]  systems that supports
[799.80 --> 800.84]  multi-factor authentication.
[800.84 --> 803.50]  It's really top notch.
[803.94 --> 804.78]  You've got to try it.
[805.12 --> 806.08]  It'll change the way
[806.08 --> 806.64]  you network
[806.64 --> 807.12]  and it's going
[807.12 --> 807.78]  to improve it.
[808.52 --> 809.46]  Tailscale.com
[809.46 --> 810.42]  slash self-hosted.
[810.58 --> 811.22]  Go there to support
[811.22 --> 811.60]  the show
[811.60 --> 812.54]  and try it for free
[812.54 --> 813.30]  forever
[813.30 --> 815.20]  for up to 100 devices.
[815.78 --> 816.56]  Tailscale.com
[816.56 --> 818.32]  slash self-hosted.
[819.92 --> 820.90]  Well, joining us
[820.90 --> 821.56]  on the show today,
[821.60 --> 822.32]  I'm really excited
[822.32 --> 823.50]  to welcome Doug
[823.50 --> 824.36]  and Mitch
[824.36 --> 825.76]  from 45 Drives.
[826.26 --> 827.36]  Doug is the president
[827.36 --> 828.46]  and co-founder
[828.46 --> 829.10]  and Mitch
[829.10 --> 830.72]  is the lead
[830.72 --> 831.42]  storage architect.
[831.92 --> 833.04]  Welcome to the show, guys.
[833.52 --> 834.24]  Thank you very much.
[834.66 --> 835.40]  Yeah, my pleasure.
[835.68 --> 836.28]  Happy to be here.
[836.28 --> 837.16]  And we thought
[837.16 --> 838.24]  we'd talk to you today.
[838.60 --> 838.90]  I mean,
[839.16 --> 840.32]  I probably like
[840.32 --> 841.08]  most of our audience
[841.08 --> 841.80]  spend probably
[841.80 --> 842.58]  a bit too much time
[842.58 --> 842.94]  on Reddit
[842.94 --> 844.76]  and I saw your post
[844.76 --> 845.68]  recently about
[845.68 --> 846.36]  the upcoming
[846.36 --> 847.28]  HomeLab server
[847.28 --> 847.80]  that you guys
[847.80 --> 848.50]  are working on.
[848.96 --> 849.44]  HomeLabs.
[850.00 --> 851.36]  So 45 Drives
[851.36 --> 851.88]  and, you know,
[852.20 --> 852.86]  some of your audience
[852.86 --> 853.56]  may know us
[853.56 --> 854.78]  and those that don't,
[854.88 --> 856.00]  we make big,
[856.18 --> 857.06]  strong, fast
[857.06 --> 858.78]  storage server systems.
[859.00 --> 859.96]  We do single servers
[859.96 --> 860.46]  clustered,
[860.62 --> 861.34]  but it's professional
[861.34 --> 862.22]  market stuff.
[862.64 --> 863.58]  It's enterprise.
[863.58 --> 864.96]  The company's
[864.96 --> 866.14]  been a great run.
[866.46 --> 867.30]  We do things differently.
[867.46 --> 867.84]  We call it
[867.84 --> 868.68]  new enterprise
[868.68 --> 869.52]  that we do.
[869.62 --> 870.22]  It's open source,
[870.28 --> 871.10]  open platform,
[871.52 --> 872.48]  no vendor lock-in,
[872.54 --> 873.42]  just a whole different thing.
[873.68 --> 873.80]  You know,
[873.80 --> 874.46]  buy what you want,
[874.52 --> 875.48]  get the services you want.
[875.56 --> 876.66]  We have full service
[876.66 --> 877.24]  if you want it,
[877.34 --> 878.50]  but we got a group
[878.50 --> 878.84]  of people
[878.84 --> 880.00]  who love computing
[880.00 --> 881.24]  and we love storage.
[881.36 --> 881.72]  We love
[881.72 --> 883.64]  big monster beasts
[883.64 --> 884.58]  and 19-inch
[884.58 --> 885.46]  rack-mount cabinets
[885.46 --> 886.18]  that, you know,
[886.20 --> 888.34]  weigh 140 pounds
[888.34 --> 889.06]  or something for,
[889.28 --> 889.48]  you know,
[889.60 --> 890.88]  they're fun to play with.
[890.88 --> 891.68]  Yeah,
[891.76 --> 893.20]  we got computing
[893.20 --> 893.84]  in our blood
[893.84 --> 895.44]  and the Home Labs world
[895.44 --> 896.46]  has always been,
[896.88 --> 897.12]  you know,
[897.16 --> 898.60]  it's been exciting for us
[898.60 --> 899.66]  and, you know,
[899.68 --> 901.00]  a lot of us are involved
[901.00 --> 901.80]  in that ourselves.
[902.50 --> 902.68]  You know,
[902.72 --> 903.90]  Mitch is hugely,
[903.90 --> 904.86]  I'm not so much anymore,
[905.02 --> 906.28]  I'm just getting a little bit older
[906.28 --> 907.98]  and to involve my entrepreneurship,
[908.20 --> 909.78]  but Mitch is deeply into it.
[910.14 --> 911.20]  So we have a bunch of fans
[911.20 --> 912.06]  of the Home Labs world
[912.06 --> 912.30]  and,
[912.74 --> 913.76]  but we've never really made
[913.76 --> 914.62]  a product for it.
[914.72 --> 915.54]  So that's,
[915.94 --> 917.04]  our heads have turned there.
[917.26 --> 918.12]  I've been familiar
[918.12 --> 918.72]  with your products
[918.72 --> 919.76]  for a very long time
[919.76 --> 920.96]  through various,
[921.04 --> 922.20]  very famous YouTubers,
[922.80 --> 923.52]  the Storinators,
[923.72 --> 924.58]  all that kind of stuff.
[924.68 --> 926.32]  And I've drooled over your gear
[926.32 --> 927.10]  for many years,
[927.52 --> 928.02]  but, you know,
[928.06 --> 928.84]  the price ranges
[928.84 --> 929.42]  of those products,
[929.50 --> 929.98]  they're not aimed
[929.98 --> 931.50]  at home users like me.
[931.56 --> 933.50]  So I am super duper excited
[933.50 --> 934.22]  that you guys
[934.22 --> 935.76]  are targeting this segment.
[936.28 --> 936.34]  Yeah,
[936.38 --> 938.32]  we've got a whole lot of fans
[938.32 --> 939.24]  that kind of have been
[939.24 --> 940.34]  homegrown over the years
[940.34 --> 942.48]  with a lot of our YouTube campaigns
[942.48 --> 943.46]  with a lot of the influencers
[943.46 --> 945.58]  and like all the techies,
[945.74 --> 946.72]  all the people that work here
[946.72 --> 947.50]  that are on the tech side
[947.50 --> 948.34]  are like me.
[948.34 --> 950.18]  We're all deeply ingrained
[950.18 --> 950.68]  in this stuff.
[950.82 --> 952.02]  Like it's not just a job,
[952.10 --> 953.14]  it's our life
[953.14 --> 954.74]  and our really passion,
[955.24 --> 955.38]  right?
[955.38 --> 956.74]  So I'm super excited
[956.74 --> 958.32]  about finally being able
[958.32 --> 959.88]  to start to offer something
[959.88 --> 961.78]  that I would be able
[961.78 --> 962.28]  to afford,
[962.44 --> 962.98]  you know what I mean,
[963.02 --> 964.78]  normally for something like this.
[964.82 --> 965.10]  So yeah,
[965.14 --> 966.60]  it's huge for me for sure
[966.60 --> 968.46]  and I'm very excited
[968.46 --> 969.22]  to roll this out.
[969.66 --> 970.36]  So I've been wondering,
[970.62 --> 971.62]  I kind of get the sense
[971.62 --> 973.00]  that you might be closer
[973.00 --> 973.64]  to market
[973.64 --> 975.22]  than the post
[975.22 --> 975.94]  on Reddit
[975.94 --> 977.06]  one month ago
[977.06 --> 978.66]  kind of implies.
[978.78 --> 979.66]  You were reaching out
[979.66 --> 980.16]  to the community
[980.16 --> 982.02]  and asking for input
[982.02 --> 983.20]  on what would be
[983.20 --> 983.90]  a great server
[983.90 --> 985.22]  that fits somewhere
[985.22 --> 987.36]  between the consumer NAS
[987.36 --> 988.22]  that you can buy,
[988.38 --> 989.78]  say at Best Buy right now
[989.78 --> 991.78]  and a massive
[991.78 --> 993.30]  multi-thousand dollar
[993.30 --> 995.00]  big enterprise system.
[995.16 --> 996.06]  And I don't know,
[996.14 --> 996.72]  I guess reading
[996.72 --> 997.50]  through this post,
[997.58 --> 998.84]  I kind of got the sense
[998.84 --> 999.84]  that you already
[999.84 --> 1001.76]  have a system in mind.
[1001.94 --> 1002.84]  You kind of have
[1002.84 --> 1004.08]  at least a target in mind.
[1004.08 --> 1005.48]  Can you share sort of
[1005.48 --> 1006.36]  what that vision is?
[1007.18 --> 1007.88]  Sort of.
[1008.48 --> 1009.72]  We do things very fast.
[1010.06 --> 1010.66]  Yeah, yeah.
[1010.84 --> 1012.20]  And so our development,
[1012.58 --> 1012.98]  yeah,
[1013.04 --> 1014.00]  will be really fast.
[1014.08 --> 1014.72]  We have a sister company
[1014.72 --> 1015.56]  called Protocase
[1015.56 --> 1018.14]  that's the fastest manufacturer
[1018.14 --> 1018.96]  in the world.
[1019.28 --> 1021.00]  Does metal
[1021.00 --> 1023.34]  and like surround electronics.
[1023.98 --> 1025.56]  It does electromechanical assembly
[1025.56 --> 1026.32]  and the like too.
[1026.78 --> 1027.62]  So we have that there
[1027.62 --> 1029.48]  and it's lightning fast to do it.
[1029.72 --> 1030.12]  But, you know,
[1030.16 --> 1030.86]  going to this market,
[1030.94 --> 1031.72]  we got to figure out
[1031.72 --> 1033.60]  exactly what we can build.
[1033.60 --> 1035.36]  If we use the analogy
[1035.36 --> 1036.36]  and say
[1036.36 --> 1038.78]  what we make
[1038.78 --> 1040.20]  in the professional
[1040.20 --> 1041.34]  and enterprise market
[1041.34 --> 1042.60]  is the,
[1042.88 --> 1043.14]  let's see,
[1043.20 --> 1043.92]  it's an 18-wheeler.
[1044.40 --> 1045.82]  So it's a big double trailer,
[1045.90 --> 1046.44]  18-wheeler
[1046.44 --> 1047.64]  and you got 800 horsepower
[1047.64 --> 1048.36]  turbo diesel
[1048.36 --> 1049.88]  and big stacks
[1049.88 --> 1051.30]  and incredible power to it.
[1051.66 --> 1052.00]  Great.
[1052.30 --> 1054.28]  But it's too expensive
[1054.28 --> 1055.84]  for home use
[1055.84 --> 1056.56]  and it won't fit
[1056.56 --> 1057.10]  in your driveway.
[1057.44 --> 1058.00]  Okay.
[1058.60 --> 1060.08]  And the other end of it,
[1060.28 --> 1060.48]  you know,
[1060.50 --> 1061.34]  we recognize
[1061.34 --> 1062.02]  that out there right now,
[1062.02 --> 1062.96]  if you just want NAS
[1062.96 --> 1064.36]  to put it on a home network,
[1065.06 --> 1065.24]  you know,
[1065.30 --> 1066.30]  and I say a home network,
[1066.38 --> 1067.26]  not a home lab network
[1067.26 --> 1068.44]  and you can go buy,
[1068.56 --> 1068.78]  I don't know,
[1068.84 --> 1069.30]  Synology
[1069.30 --> 1070.94]  or QNAP
[1070.94 --> 1071.52]  or something,
[1071.82 --> 1072.04]  whatever,
[1072.24 --> 1072.56]  you know,
[1072.62 --> 1073.48]  you know,
[1073.48 --> 1074.30]  get four bays
[1074.30 --> 1075.22]  for a couple hundred bucks
[1075.22 --> 1075.84]  to drive bay
[1075.84 --> 1077.66]  and an $800 device
[1077.66 --> 1079.02]  and they're good.
[1079.02 --> 1080.46]  but we'll call that
[1080.46 --> 1082.28]  the small car
[1082.28 --> 1083.08]  or the micro car
[1083.08 --> 1084.12]  with a little utility trailer
[1084.12 --> 1084.62]  behind it
[1084.62 --> 1085.90]  and then somewhere
[1085.90 --> 1086.30]  in the middle,
[1086.38 --> 1086.84]  there's something
[1086.84 --> 1087.80]  that probably looks
[1087.80 --> 1089.16]  like a heavy-duty pickup truck
[1089.16 --> 1090.32]  with a good-sized diesel
[1090.32 --> 1090.70]  in it
[1090.70 --> 1092.72]  and extra strong suspension.
[1093.10 --> 1094.02]  So if I use that analogy,
[1094.22 --> 1094.70]  like we know
[1094.70 --> 1095.38]  where we want to go
[1095.38 --> 1096.26]  position-wise
[1096.26 --> 1097.78]  and we went to Reddit,
[1097.96 --> 1098.70]  we're going really,
[1099.02 --> 1100.60]  what exactly is that?
[1101.04 --> 1101.78]  And, you know,
[1101.78 --> 1102.44]  a bunch of questions
[1102.44 --> 1103.66]  because we all know,
[1104.30 --> 1104.52]  you know,
[1104.58 --> 1105.46]  you can get that,
[1105.52 --> 1105.68]  you know,
[1105.68 --> 1106.32]  stars in the eyes
[1106.32 --> 1107.30]  of both the 18-wheeler
[1107.30 --> 1109.10]  and it's too much.
[1109.38 --> 1110.34]  So what is right?
[1110.42 --> 1111.26]  That really is our question.
[1111.36 --> 1112.52]  Once we get our hands,
[1112.98 --> 1113.78]  our minds wrapped
[1113.78 --> 1115.26]  around starting point,
[1115.32 --> 1115.42]  you know,
[1115.44 --> 1116.38]  there's going to be a line
[1116.38 --> 1117.70]  and let's get our minds
[1117.70 --> 1118.44]  around the starting point.
[1118.50 --> 1119.28]  It will be pretty quick
[1119.28 --> 1120.22]  by the time we get there,
[1120.42 --> 1120.96]  but we're still trying
[1120.96 --> 1121.34]  to figure out
[1121.34 --> 1122.42]  exactly what it is.
[1122.84 --> 1123.00]  I see.
[1123.06 --> 1123.68]  So there must be
[1123.68 --> 1125.42]  some kind of target applications
[1125.42 --> 1127.40]  that you want to make it possible
[1127.40 --> 1128.80]  for the end user to run.
[1128.88 --> 1129.58]  There must be some sort
[1129.58 --> 1130.10]  of workloads
[1130.10 --> 1131.00]  that you're thinking of
[1131.00 --> 1132.54]  and storage and applications
[1132.54 --> 1133.50]  are both part of that.
[1133.82 --> 1134.18]  Absolutely.
[1134.32 --> 1134.62]  Absolutely.
[1134.82 --> 1135.92]  So we take a look
[1135.92 --> 1137.40]  at like what I think
[1137.40 --> 1139.20]  the average home user would do
[1139.20 --> 1140.34]  or the home lab user would do
[1140.34 --> 1140.92]  and then we were like,
[1141.22 --> 1141.40]  okay,
[1141.42 --> 1142.00]  let's take a look
[1142.00 --> 1142.80]  at these things, right?
[1142.82 --> 1143.54]  Like a lot of people
[1143.54 --> 1144.50]  will run a hypervisor
[1144.50 --> 1146.38]  or some sort of compute.
[1146.74 --> 1147.34]  A lot of people
[1147.34 --> 1148.46]  are running media servers.
[1148.60 --> 1149.04]  A lot of people
[1149.04 --> 1149.60]  are running things
[1149.60 --> 1150.52]  like Nextcloud,
[1151.00 --> 1152.00]  VPNs,
[1152.10 --> 1153.34]  all those types of things, right?
[1153.54 --> 1154.36]  So we wanted to,
[1154.60 --> 1155.64]  rather than throw those
[1155.64 --> 1156.14]  out there though,
[1156.16 --> 1156.76]  we just wanted to say,
[1156.82 --> 1156.92]  hey,
[1157.02 --> 1158.18]  what are the top five,
[1158.42 --> 1159.24]  top 10 applications
[1159.24 --> 1160.54]  that you guys
[1160.54 --> 1161.40]  are interested in?
[1161.76 --> 1162.38]  And, you know,
[1162.38 --> 1163.92]  we really love the idea
[1163.92 --> 1164.92]  of having the ability
[1164.92 --> 1165.46]  of, you know,
[1165.52 --> 1166.38]  one-click containers
[1166.38 --> 1166.86]  to, you know,
[1166.86 --> 1168.14]  deploy a plaque server
[1168.14 --> 1169.12]  or a VPN
[1169.12 --> 1170.06]  or something like that.
[1170.32 --> 1171.62]  But we also want
[1171.62 --> 1172.76]  to leave the wires
[1172.76 --> 1173.22]  hanging out,
[1173.24 --> 1173.64]  so to speak,
[1173.68 --> 1175.04]  for the more advanced users
[1175.04 --> 1175.82]  that really want
[1175.82 --> 1176.76]  to get underneath the hood
[1176.76 --> 1178.72]  and do some custom,
[1178.86 --> 1179.58]  customizations
[1179.58 --> 1180.46]  on the Linux side.
[1180.88 --> 1181.90]  And that was a big part
[1181.90 --> 1183.06]  of when we developed Houston,
[1183.16 --> 1184.44]  which is our user interface
[1184.44 --> 1185.32]  or web user interface
[1185.32 --> 1186.58]  used to manage
[1186.58 --> 1187.46]  our storage servers.
[1187.92 --> 1188.82]  And that was a big part
[1188.82 --> 1189.42]  of that as well
[1189.42 --> 1190.46]  is we want to make it
[1190.46 --> 1191.30]  easy and simple
[1191.30 --> 1192.96]  for a lot of our users
[1192.96 --> 1193.62]  and our customers
[1193.62 --> 1194.88]  that aren't highly
[1194.88 --> 1196.16]  technical Linux users,
[1196.34 --> 1197.60]  but they need to be able
[1197.60 --> 1198.50]  to do everything
[1198.50 --> 1199.56]  that a very highly
[1199.56 --> 1200.90]  technical user can do.
[1201.10 --> 1202.26]  And so anything
[1202.26 --> 1203.02]  that you do
[1203.02 --> 1204.02]  in the command line
[1204.02 --> 1205.10]  doesn't get overridden
[1205.10 --> 1205.88]  by the UI
[1205.88 --> 1206.58]  and vice versa.
[1207.00 --> 1207.48]  And so we want
[1207.48 --> 1208.86]  to take that same approach
[1208.86 --> 1210.06]  to the home lab market
[1210.06 --> 1210.48]  as well
[1210.48 --> 1211.58]  and have it best
[1211.58 --> 1212.18]  of both worlds
[1212.18 --> 1213.32]  for both types of users.
[1213.60 --> 1214.56]  And if I could add
[1214.56 --> 1215.28]  in that too,
[1215.74 --> 1217.00]  there's a fundamental thing,
[1217.14 --> 1217.60]  you know,
[1217.60 --> 1218.22]  storage power.
[1218.30 --> 1219.04]  We take it for granted
[1219.04 --> 1219.52]  around here.
[1219.60 --> 1219.98]  We got our,
[1220.12 --> 1220.34]  you know,
[1220.38 --> 1220.96]  our group,
[1221.14 --> 1221.80]  the group that Mitch
[1221.80 --> 1222.72]  works in that does
[1222.72 --> 1224.12]  architecture configuration
[1224.12 --> 1225.32]  and service.
[1225.54 --> 1226.88]  And we get to move around
[1226.88 --> 1228.22]  massive amounts of data
[1228.22 --> 1229.56]  and get to move it
[1229.56 --> 1230.24]  very, very quickly.
[1230.58 --> 1231.34]  We love it.
[1231.42 --> 1231.84]  It's great.
[1231.92 --> 1233.80]  You put a huge machine
[1233.80 --> 1234.16]  together,
[1234.24 --> 1234.78]  you set up,
[1235.14 --> 1235.70]  you know,
[1235.78 --> 1236.58]  you got a bunch of data
[1236.58 --> 1236.96]  in there
[1236.96 --> 1238.54]  in well thought out
[1238.54 --> 1239.96]  arrays with redundancy,
[1240.30 --> 1241.78]  but parallelism in it.
[1242.06 --> 1242.46]  And,
[1242.56 --> 1242.88]  you know,
[1242.94 --> 1244.18]  and we help people,
[1244.48 --> 1244.68]  you know,
[1244.68 --> 1246.72]  do crazy transfer rates
[1246.72 --> 1247.64]  where we'll be getting,
[1247.72 --> 1247.86]  you know,
[1247.88 --> 1249.84]  five gigabytes per second
[1249.84 --> 1251.68]  flowing out of a single box.
[1252.36 --> 1252.46]  And,
[1252.52 --> 1252.78]  you know,
[1252.78 --> 1253.86]  doing single client transfers,
[1254.08 --> 1254.30]  you know,
[1254.36 --> 1255.68]  filling a 10 gigabit line
[1255.68 --> 1256.58]  and just the one transfer
[1256.58 --> 1257.12]  to one client.
[1257.46 --> 1258.06]  And it's fun
[1258.06 --> 1258.86]  and it's doable.
[1259.02 --> 1260.24]  Anybody who loves Linux,
[1260.44 --> 1260.62]  you know,
[1260.64 --> 1261.38]  we can teach people
[1261.38 --> 1262.52]  how to tune things up
[1262.52 --> 1263.78]  and do that kind of stuff.
[1264.04 --> 1264.40]  But,
[1264.56 --> 1264.92]  you know,
[1265.02 --> 1266.02]  question for us
[1266.02 --> 1267.12]  and what we do
[1267.12 --> 1267.52]  and what people
[1267.52 --> 1268.08]  are going to do with it
[1268.08 --> 1268.84]  is to what extent
[1268.84 --> 1270.14]  that heavy duty storage,
[1270.88 --> 1271.08]  you know,
[1271.12 --> 1271.98]  fun to play with.
[1272.24 --> 1272.58]  But,
[1272.94 --> 1273.34]  you know,
[1273.38 --> 1274.48]  do you have the network bandwidth
[1274.48 --> 1276.06]  and do you have any place
[1276.06 --> 1276.72]  for it to go?
[1277.04 --> 1277.80]  And we don't know
[1277.80 --> 1278.10]  because,
[1278.44 --> 1278.62]  you know,
[1278.68 --> 1279.92]  people do all kinds of things
[1279.92 --> 1280.64]  in the Homelab world,
[1280.70 --> 1280.88]  right?
[1280.96 --> 1282.54]  It's such an interesting
[1282.54 --> 1283.28]  group of people.
[1283.80 --> 1284.66]  I love to hear it
[1284.66 --> 1286.10]  and it sounds to me
[1286.10 --> 1287.02]  like you're going after
[1287.02 --> 1289.22]  that kind of yummy middle
[1289.22 --> 1291.08]  where Unraid users
[1291.08 --> 1292.74]  meet Proxmox users
[1292.74 --> 1294.86]  meet maybe ESXi users.
[1294.86 --> 1296.80]  that kind of middle ground
[1296.80 --> 1298.64]  where if I wanted to build
[1298.64 --> 1299.42]  a server capable
[1299.42 --> 1301.82]  of hosting enough VMs
[1301.82 --> 1302.96]  to make it worth my while,
[1303.04 --> 1303.70]  so let's say I'm playing around
[1303.70 --> 1304.12]  with Kubernetes
[1304.12 --> 1304.98]  or something at home,
[1305.70 --> 1306.70]  I want to put 64,
[1306.96 --> 1308.12]  maybe 128 gig
[1308.12 --> 1309.84]  or more worth of RAM in there.
[1310.28 --> 1311.16]  A lot of,
[1311.18 --> 1311.48]  you know,
[1311.60 --> 1312.92]  consumer grade motherboards
[1312.92 --> 1314.82]  just can't handle that.
[1314.86 --> 1315.60]  And then I think to myself,
[1315.66 --> 1315.74]  well,
[1315.76 --> 1316.30]  it's a server.
[1316.42 --> 1317.76]  I need IPMI in there.
[1318.32 --> 1318.90]  Wouldn't it be great
[1318.90 --> 1319.64]  if I could just buy
[1319.64 --> 1321.08]  an off-the-shelf power supply
[1321.08 --> 1321.44]  as well?
[1321.52 --> 1321.64]  So,
[1321.72 --> 1321.86]  I mean,
[1321.94 --> 1323.16]  how are you guys thinking
[1323.16 --> 1324.32]  about the actual hardware
[1324.32 --> 1325.16]  that's going into this?
[1325.22 --> 1325.90]  Are you going to use
[1325.90 --> 1326.84]  commodity stuff
[1326.84 --> 1327.72]  or are you just providing
[1327.72 --> 1328.18]  a chassis?
[1329.00 --> 1329.70]  You know what?
[1330.20 --> 1331.20]  It's price point,
[1331.72 --> 1332.00]  you know?
[1332.68 --> 1334.16]  It's like we can design
[1334.16 --> 1334.58]  whatever
[1334.58 --> 1335.66]  and ideally,
[1336.10 --> 1336.86]  the idea is just having
[1336.86 --> 1338.78]  a chassis as a base
[1338.78 --> 1340.56]  and then putting out
[1340.56 --> 1341.62]  some options for,
[1342.38 --> 1342.62]  you know,
[1342.64 --> 1343.28]  people want to put,
[1343.86 --> 1344.06]  you know,
[1344.76 --> 1345.58]  what we're designed
[1345.58 --> 1346.16]  to be compatible
[1346.16 --> 1346.86]  so you can put in
[1346.86 --> 1348.68]  a consumer grade power supply
[1348.68 --> 1349.20]  if you want
[1349.20 --> 1349.50]  or,
[1349.50 --> 1350.44]  you know,
[1350.78 --> 1351.50]  and the option
[1351.50 --> 1352.52]  to put your own motherboard in
[1352.52 --> 1353.98]  but we'll probably look
[1353.98 --> 1354.68]  at offering
[1354.68 --> 1355.58]  some professional,
[1355.80 --> 1356.78]  you know,
[1356.84 --> 1357.22]  grade,
[1357.36 --> 1358.40]  you know,
[1358.44 --> 1359.00]  motherboards
[1359.00 --> 1360.36]  that have all the features
[1360.36 --> 1360.66]  on it
[1360.66 --> 1360.78]  but,
[1360.88 --> 1361.00]  you know,
[1361.00 --> 1361.30]  it comes down
[1361.30 --> 1361.90]  to price point
[1361.90 --> 1362.36]  and it's a,
[1362.64 --> 1364.30]  we're a cost plus company,
[1364.42 --> 1364.66]  you know,
[1364.74 --> 1366.08]  and in the enterprise market,
[1366.24 --> 1367.30]  you know,
[1367.30 --> 1368.50]  our systems sell
[1368.50 --> 1370.24]  for quite dramatically
[1370.24 --> 1372.00]  lower than the legacy
[1372.00 --> 1372.92]  enterprise vendors.
[1373.42 --> 1373.60]  You know,
[1373.64 --> 1375.04]  we call it new enterprise.
[1375.48 --> 1375.60]  You know,
[1375.62 --> 1376.60]  we'll sell on the same thing.
[1376.74 --> 1378.22]  There's no big value pricing
[1378.22 --> 1379.84]  and making a grab off it.
[1379.96 --> 1379.98]  Well,
[1380.06 --> 1380.34]  you know,
[1380.34 --> 1381.00]  in the market,
[1381.26 --> 1382.52]  it isn't there
[1382.52 --> 1384.68]  but there's cost base
[1384.68 --> 1384.96]  in it,
[1385.00 --> 1385.18]  right?
[1385.44 --> 1386.22]  You want all the bells
[1386.22 --> 1386.72]  and whistles
[1386.72 --> 1387.72]  so the bells and whistles
[1387.72 --> 1389.48]  cost and it's got to flow through.
[1389.92 --> 1390.10]  So,
[1390.18 --> 1391.36]  what I'd really love to do,
[1391.42 --> 1391.54]  you know,
[1391.60 --> 1391.86]  look,
[1391.96 --> 1392.30]  what we do,
[1392.50 --> 1393.24]  here's the advantage
[1393.24 --> 1394.18]  we have as an organization.
[1394.68 --> 1396.06]  We are sort of
[1396.06 --> 1396.88]  on the cutting edge
[1396.88 --> 1398.32]  of low volume
[1398.32 --> 1400.08]  mass custom manufacturing
[1400.08 --> 1402.76]  and we can customize things
[1402.76 --> 1403.86]  better than anybody can
[1403.86 --> 1404.66]  and we're just going to
[1404.66 --> 1405.30]  really play with that
[1405.30 --> 1405.76]  and see what we can do
[1405.76 --> 1406.40]  in this market
[1406.40 --> 1407.80]  to see what we can do
[1407.80 --> 1408.84]  to get options out there.
[1408.98 --> 1409.12]  You know,
[1409.12 --> 1410.40]  and then the market will tell us,
[1410.64 --> 1410.76]  you know,
[1410.76 --> 1412.18]  we want these initial conversations.
[1412.72 --> 1413.30]  They're absolutely great
[1413.30 --> 1414.34]  to get us some starting points
[1414.34 --> 1415.84]  and then you put stuff out there
[1415.84 --> 1417.04]  and you see where people want to go,
[1417.34 --> 1417.52]  right?
[1417.60 --> 1418.94]  And what do they want to spend on,
[1419.00 --> 1419.16]  right?
[1419.64 --> 1419.96]  So,
[1420.08 --> 1421.20]  anybody listening to this
[1421.20 --> 1423.24]  who hasn't seen the posts on Reddit
[1423.24 --> 1424.96]  or anywhere else you've posted,
[1425.48 --> 1427.08]  what's the best avenue for them
[1427.08 --> 1429.16]  to direct their feedback to you?
[1429.68 --> 1431.44]  Info at 45drives.com,
[1431.48 --> 1432.10]  I think for now,
[1432.22 --> 1433.96]  is something that people can reach out to
[1433.96 --> 1435.06]  today right now.
[1435.50 --> 1437.22]  Something that we're working on right now
[1437.22 --> 1437.92]  in the background
[1437.92 --> 1440.04]  is bringing back the 45 drives form.
[1440.34 --> 1440.52]  So,
[1440.58 --> 1442.60]  we had a form many years ago
[1442.60 --> 1444.48]  and it kind of went away
[1444.48 --> 1446.16]  in lieu of our support page
[1446.16 --> 1447.12]  and the way we do support now.
[1447.14 --> 1448.22]  But we think that's really important
[1448.22 --> 1449.00]  to bring that back.
[1449.34 --> 1449.44]  So,
[1449.50 --> 1450.46]  that is definitely going to be
[1450.46 --> 1451.22]  another big thing
[1451.22 --> 1452.58]  that's coming down the pipe very soon.
[1452.94 --> 1453.86]  And we're hoping that's going to be
[1453.86 --> 1454.54]  kind of homegrown
[1454.54 --> 1455.86]  and everyone kind of helps each other,
[1455.92 --> 1456.70]  but we're also going to have
[1456.70 --> 1457.64]  our own service team
[1457.64 --> 1459.24]  that is going to be manning it daily.
[1459.82 --> 1461.00]  And one thing just quickly,
[1461.10 --> 1462.62]  what I wanted to just jump back on,
[1462.62 --> 1464.44]  on kind of what 45 drives
[1464.44 --> 1465.42]  we'll be offering in the home lab,
[1465.66 --> 1465.82]  you know,
[1465.82 --> 1467.76]  you look at what do we do right now
[1467.76 --> 1468.54]  with our storage servers
[1468.54 --> 1469.24]  that's unique.
[1469.36 --> 1471.18]  And I think of our density
[1471.18 --> 1472.96]  and also our PCB backplane
[1472.96 --> 1474.48]  and our no multiplexers.
[1474.84 --> 1474.94]  So,
[1475.00 --> 1475.78]  our PCB backplane
[1475.78 --> 1476.88]  is really freaking cool.
[1477.00 --> 1477.48]  I love it.
[1477.60 --> 1479.20]  It's a fantastic design
[1479.20 --> 1479.78]  that we've done
[1479.78 --> 1481.16]  and the fact that we don't use
[1481.16 --> 1482.02]  any multiplexers.
[1482.38 --> 1482.46]  So,
[1482.50 --> 1483.44]  I think those are going to be
[1483.44 --> 1484.34]  huge carryovers
[1484.34 --> 1485.52]  into the home lab.
[1485.98 --> 1487.22]  And I think it will be
[1487.22 --> 1488.52]  immensely important
[1488.52 --> 1489.48]  to have no motherboard
[1489.48 --> 1490.86]  as option as well.
[1490.86 --> 1491.70]  I was going to ask
[1491.70 --> 1492.20]  for those of us
[1492.20 --> 1492.86]  that aren't familiar
[1492.86 --> 1494.28]  with what a multiplexer is.
[1494.62 --> 1494.98]  So,
[1495.12 --> 1495.68]  when you get into
[1495.68 --> 1496.56]  large storage servers,
[1496.66 --> 1497.04]  one of the things
[1497.04 --> 1498.22]  that we do very differently
[1498.22 --> 1500.00]  to make it economical,
[1500.70 --> 1501.78]  to build a very large
[1501.78 --> 1502.48]  storage server,
[1502.80 --> 1503.96]  the Chinese made
[1503.96 --> 1505.00]  large storage servers,
[1505.42 --> 1506.46]  they'll plug hard drives
[1506.46 --> 1507.34]  together in five
[1507.34 --> 1508.76]  SATA drives.
[1509.24 --> 1509.56]  Typically,
[1509.68 --> 1510.40]  they're on SATA.
[1510.66 --> 1510.80]  Well,
[1510.86 --> 1512.04]  everything's in SATA
[1512.04 --> 1512.98]  and port multiplication.
[1513.64 --> 1513.84]  So,
[1514.10 --> 1514.54]  typically,
[1514.74 --> 1515.66]  five drives
[1515.66 --> 1517.60]  will share one SATA port.
[1517.98 --> 1518.78]  When you do that,
[1518.84 --> 1519.34]  you end up
[1519.34 --> 1519.94]  really,
[1520.06 --> 1520.28]  you know,
[1520.28 --> 1521.10]  a spinner,
[1521.76 --> 1522.02]  you know,
[1522.04 --> 1522.68]  we kind of use
[1522.68 --> 1525.42]  200 megabytes per second
[1525.42 --> 1526.44]  as its throughput.
[1526.76 --> 1526.92]  So,
[1527.18 --> 1527.36]  you know,
[1527.54 --> 1529.50]  a couple gigabits per second.
[1529.72 --> 1530.50]  It doesn't take too many
[1530.50 --> 1531.14]  of them before you
[1531.14 --> 1532.84]  completely plug up
[1532.84 --> 1533.68]  a SATA port.
[1534.06 --> 1534.82]  The multiplexing
[1534.82 --> 1535.58]  is,
[1536.18 --> 1536.34]  yeah,
[1536.40 --> 1536.78]  two of them,
[1536.86 --> 1537.10]  in fact.
[1537.42 --> 1537.58]  Yeah,
[1537.62 --> 1538.34]  so you lose bandwidth
[1538.34 --> 1538.80]  on it,
[1538.98 --> 1539.56]  and it's also,
[1539.72 --> 1540.78]  it's a pain in the butt
[1540.78 --> 1541.44]  driver-wise,
[1541.76 --> 1542.62]  and you try to operate
[1542.62 --> 1543.16]  these things,
[1543.38 --> 1544.24]  you bump into driver
[1544.24 --> 1544.56]  problems,
[1544.66 --> 1545.22]  driver problems.
[1545.54 --> 1545.72]  So,
[1545.82 --> 1546.34]  we did something,
[1546.52 --> 1546.64]  you know,
[1546.66 --> 1547.44]  we pioneered it
[1547.44 --> 1548.46]  a number of years ago
[1548.46 --> 1549.28]  in large storage servers.
[1549.28 --> 1550.20]  We call it direct wired.
[1550.20 --> 1550.86]  You know,
[1550.92 --> 1551.60]  direct lane
[1551.60 --> 1553.50]  from hard drive
[1553.50 --> 1554.70]  through to your
[1554.70 --> 1555.62]  HBA adapter,
[1555.76 --> 1556.44]  which has the ability
[1556.44 --> 1557.18]  to handle the bandwidth
[1557.18 --> 1559.06]  of all these drives.
[1559.76 --> 1559.78]  So,
[1560.06 --> 1560.56]  that's it.
[1560.64 --> 1560.72]  Yeah,
[1560.80 --> 1561.52]  multiplexing is,
[1562.16 --> 1562.30]  you know,
[1562.34 --> 1563.10]  multiplexing is good
[1563.10 --> 1563.56]  if you want to,
[1563.68 --> 1564.04]  you know,
[1564.04 --> 1565.50]  large archival servers
[1565.50 --> 1566.42]  and you want to make them
[1566.42 --> 1568.24]  at the very lowest dollar,
[1568.64 --> 1569.90]  but it's not us.
[1570.04 --> 1570.66]  It's not big,
[1570.74 --> 1570.96]  fast,
[1571.04 --> 1571.32]  strong.
[1571.82 --> 1572.22]  So,
[1572.34 --> 1573.22]  what sort of form factors
[1573.22 --> 1573.74]  are you thinking?
[1573.74 --> 1574.86]  A rack mount thing
[1574.86 --> 1575.42]  or something that sits
[1575.42 --> 1576.12]  on a shelf
[1576.12 --> 1576.76]  or what?
[1577.16 --> 1577.26]  So,
[1577.36 --> 1578.14]  the feedback
[1578.14 --> 1579.12]  that we got back
[1579.12 --> 1579.90]  and I think
[1579.90 --> 1580.84]  it's dead on
[1580.84 --> 1581.94]  is we got back
[1581.94 --> 1582.48]  for you,
[1582.58 --> 1583.04]  to you,
[1583.40 --> 1584.56]  are kind of the ones
[1584.56 --> 1585.06]  that we're shooting
[1585.06 --> 1585.80]  for right now.
[1586.10 --> 1586.76]  And then also,
[1586.76 --> 1587.76]  it's going to be rack bound,
[1587.84 --> 1588.48]  but with the ability
[1588.48 --> 1589.94]  to screw on some rubber feet
[1589.94 --> 1590.76]  and have something
[1590.76 --> 1591.44]  that's going to be pleasing
[1591.44 --> 1592.02]  to the eye
[1592.02 --> 1593.34]  that you can put on a desk
[1593.34 --> 1594.40]  and still be very nice
[1594.40 --> 1595.20]  and look good,
[1595.24 --> 1595.42]  right?
[1595.82 --> 1596.02]  So,
[1596.10 --> 1596.86]  I personally have a
[1596.86 --> 1597.70]  Stornator at home,
[1597.82 --> 1598.68]  one of our older versions.
[1598.96 --> 1599.74]  And I did something
[1599.74 --> 1600.18]  very similar
[1600.18 --> 1601.00]  to what you were talking about.
[1601.04 --> 1601.14]  Like,
[1601.20 --> 1602.08]  I put a regular
[1602.08 --> 1603.46]  ATX power supply in it.
[1603.46 --> 1604.30]  I put a couple
[1604.30 --> 1605.40]  Hyper 212 EVO
[1605.40 --> 1606.50]  Cooler Master Coolers,
[1606.84 --> 1607.78]  some Noctua fans,
[1607.84 --> 1608.52]  and now it's very,
[1608.62 --> 1609.16]  very quiet
[1609.16 --> 1610.14]  and just sits
[1610.14 --> 1611.26]  right in my rack
[1611.26 --> 1612.58]  and is just like
[1612.58 --> 1613.90]  a beautiful server for me.
[1613.96 --> 1614.40]  I've had it running
[1614.40 --> 1615.04]  for a few years.
[1615.14 --> 1615.32]  So,
[1615.78 --> 1616.52]  if we can translate
[1616.52 --> 1617.58]  that to the home lab,
[1617.80 --> 1618.86]  that'd be fantastic.
[1619.32 --> 1619.60]  I love it.
[1619.62 --> 1620.58]  When you talk to a vendor
[1620.58 --> 1621.88]  like you guys
[1621.88 --> 1622.66]  who clearly
[1622.66 --> 1623.94]  is actually passionate
[1623.94 --> 1624.56]  about what they're
[1624.56 --> 1625.04]  talking about
[1625.04 --> 1626.00]  and you jump in
[1626.00 --> 1626.30]  and say,
[1626.40 --> 1626.48]  oh,
[1626.50 --> 1627.52]  I had a Hyper 212
[1627.52 --> 1628.44]  EVO Cooler,
[1628.52 --> 1628.68]  like,
[1629.00 --> 1630.18]  you obviously are not
[1630.18 --> 1631.24]  trying to BS us.
[1631.30 --> 1632.32]  You definitely are
[1632.32 --> 1633.44]  talking the talk.
[1633.88 --> 1634.64]  And walk in the walk.
[1634.78 --> 1634.88]  So,
[1635.58 --> 1636.74]  what is the thing
[1636.74 --> 1637.30]  that's probably going
[1637.30 --> 1638.14]  to be the most challenging?
[1638.68 --> 1640.12]  We can build that 18-wheeler,
[1640.30 --> 1640.52]  that,
[1640.52 --> 1641.12]  you know,
[1641.16 --> 1642.30]  Australian road train
[1642.30 --> 1643.06]  with three trailers,
[1643.16 --> 1643.70]  the biggest engine
[1643.70 --> 1644.12]  you ever had.
[1644.18 --> 1644.74]  We can build it.
[1645.22 --> 1646.32]  It's finding
[1646.32 --> 1647.48]  what the market wants.
[1648.30 --> 1648.56]  You know,
[1648.76 --> 1650.22]  it's just a subtle matching
[1650.22 --> 1651.30]  between what the market wants
[1651.30 --> 1652.02]  and what makes sense
[1652.02 --> 1652.52]  for people
[1652.52 --> 1653.78]  and price point
[1653.78 --> 1656.44]  and trying to find that.
[1656.74 --> 1657.92]  Because if we just go crazy
[1657.92 --> 1658.72]  and put out something
[1658.72 --> 1659.28]  that has,
[1659.68 --> 1660.10]  you know,
[1660.10 --> 1661.10]  every bell and whistle
[1661.10 --> 1662.06]  and full horsepower
[1662.06 --> 1662.86]  and full size,
[1662.86 --> 1663.66]  it ends up being
[1663.66 --> 1664.42]  a professional line,
[1664.48 --> 1664.66]  right?
[1664.98 --> 1665.18]  So,
[1665.32 --> 1666.12]  we've got to figure out
[1666.12 --> 1666.54]  what works.
[1666.92 --> 1668.42]  The chassis is a great idea.
[1668.54 --> 1669.12]  We sell chassis,
[1669.28 --> 1670.66]  then people can let us know.
[1670.74 --> 1671.58]  We can watch what people
[1671.58 --> 1671.78]  are doing,
[1671.86 --> 1672.36]  getting feedback.
[1672.86 --> 1673.88]  What are they putting in
[1673.88 --> 1674.76]  for electronics?
[1675.28 --> 1675.42]  You know,
[1675.42 --> 1675.96]  what are they running
[1675.96 --> 1676.92]  on software-wise?
[1677.04 --> 1677.90]  Get a sense of that.
[1678.14 --> 1679.28]  We can tune into that.
[1679.66 --> 1680.16]  That's where you've got
[1680.16 --> 1680.70]  to get to on it.
[1680.86 --> 1681.92]  It's knowing the market.
[1682.32 --> 1683.30]  And when it comes down to,
[1683.36 --> 1683.60]  as I said,
[1683.64 --> 1684.42]  the other end of it
[1684.42 --> 1685.78]  is a place that,
[1685.94 --> 1686.08]  you know,
[1686.12 --> 1686.58]  challenging.
[1687.18 --> 1688.12]  We just know
[1688.12 --> 1688.96]  you've got to stay out of there.
[1689.10 --> 1689.26]  Look,
[1689.36 --> 1690.58]  we're North American design.
[1690.76 --> 1692.46]  We're North American manufactured
[1692.46 --> 1694.50]  and we do stuff
[1694.50 --> 1694.94]  and, you know,
[1694.96 --> 1696.44]  we mass custom manufacture it.
[1696.84 --> 1697.66]  If you want cheap,
[1698.04 --> 1698.68]  it's not us.
[1699.46 --> 1700.84]  We're not exotic price.
[1701.04 --> 1702.44]  We're not a Maserati,
[1703.10 --> 1704.28]  but neither are we
[1704.28 --> 1704.96]  or, you know,
[1705.02 --> 1706.96]  your entry-level automobile
[1706.96 --> 1707.80]  or whatever, right?
[1708.02 --> 1709.02]  It's not it, so.
[1709.20 --> 1710.06]  We talked about this
[1710.06 --> 1710.58]  the other day,
[1710.68 --> 1711.00]  you know,
[1711.26 --> 1713.32]  some of the big enterprise companies
[1713.32 --> 1714.84]  have to pay the steak dinner bill
[1714.84 --> 1715.84]  and they charge a lot
[1715.84 --> 1716.36]  for the service
[1716.36 --> 1716.92]  on the other end
[1716.92 --> 1717.54]  as a consequence.
[1719.02 --> 1719.28]  Yeah,
[1719.44 --> 1720.52]  you're paying for a triple,
[1720.64 --> 1721.34]  three times over
[1721.34 --> 1722.06]  on the back end.
[1722.32 --> 1722.86]  Right, exactly.
[1723.18 --> 1723.40]  Yeah,
[1723.40 --> 1724.26]  I love it.
[1724.32 --> 1724.42]  Yeah,
[1724.48 --> 1725.72]  that's enterprise sales.
[1725.84 --> 1726.50]  You go to buy something
[1726.50 --> 1727.06]  enterprise vendor,
[1727.14 --> 1727.84]  they take you to the best
[1727.84 --> 1728.78]  steakhouse in town,
[1728.88 --> 1729.58]  buy a steak dinner
[1729.58 --> 1730.52]  and you know
[1730.52 --> 1732.20]  your organization's paying
[1732.20 --> 1732.74]  for it
[1732.74 --> 1734.12]  after they buy it from them.
[1734.38 --> 1734.58]  Yeah,
[1734.66 --> 1735.46]  in the long run.
[1735.76 --> 1736.02]  Yeah.
[1736.68 --> 1737.02]  Well,
[1737.20 --> 1737.48]  Doug,
[1737.58 --> 1737.78]  Mitch,
[1737.80 --> 1738.76]  this is right up our alley.
[1738.84 --> 1739.60]  We look forward to seeing
[1739.60 --> 1740.56]  what you guys develop,
[1740.70 --> 1741.70]  so keep us posted
[1741.70 --> 1742.76]  on how things go.
[1742.98 --> 1743.62]  Just let us know
[1743.62 --> 1744.46]  when something's developed
[1744.46 --> 1745.32]  and keep us in the loop,
[1745.36 --> 1745.60]  okay?
[1746.14 --> 1747.72]  I would love to come back on
[1747.72 --> 1748.76]  when we have a couple more
[1748.76 --> 1749.80]  updates for us,
[1749.82 --> 1750.70]  maybe a month or two
[1750.70 --> 1751.30]  down the road
[1751.30 --> 1752.20]  and when we've got
[1752.20 --> 1752.94]  something a little closer.
[1753.08 --> 1753.16]  Yeah.
[1753.44 --> 1753.74]  Yeah,
[1753.78 --> 1754.44]  we're just into,
[1754.74 --> 1755.08]  you know,
[1755.10 --> 1755.46]  the feedback,
[1755.64 --> 1756.22]  digesting it,
[1756.26 --> 1758.48]  just into our creative meetings
[1758.48 --> 1759.12]  on it right now
[1759.12 --> 1760.86]  to see what we develop.
[1761.02 --> 1762.02]  Our development team
[1762.02 --> 1763.22]  is great fun for them.
[1763.58 --> 1764.56]  It's really a fun project
[1764.56 --> 1765.04]  for us,
[1765.12 --> 1767.14]  so we would love to share it.
[1767.26 --> 1768.34]  Our sense is it feels
[1768.34 --> 1769.28]  sort of like you guys
[1769.28 --> 1770.42]  are in the right direction.
[1770.82 --> 1771.32]  Sounds like you're
[1771.32 --> 1771.86]  building a product
[1771.86 --> 1773.28]  that Alex and myself
[1773.28 --> 1774.04]  and a lot of our audience
[1774.04 --> 1774.56]  would probably be
[1774.56 --> 1775.10]  interested in,
[1775.18 --> 1775.26]  so.
[1775.26 --> 1775.80]  I'll buy it.
[1775.80 --> 1776.12]  Yeah.
[1777.50 --> 1778.58]  We'll chat again soon.
[1778.62 --> 1779.26]  I'll hold you to that.
[1779.86 --> 1780.78]  Thanks for joining us,
[1780.82 --> 1781.00]  guys.
[1781.12 --> 1781.80]  Thank you very much.
[1781.80 --> 1782.18]  Thank you.
[1782.26 --> 1783.12]  Thank you for having us.
[1785.22 --> 1787.26]  Linode.com slash SSH.
[1787.34 --> 1788.70]  Go there for $100
[1788.70 --> 1790.38]  in 60-day credit.
[1790.62 --> 1791.68]  Really kick the tires
[1791.68 --> 1793.80]  and see the exciting news.
[1794.30 --> 1795.62]  Linode is now part of Akamai,
[1795.94 --> 1796.84]  all the developer-friendly
[1796.84 --> 1797.60]  tools you love,
[1797.64 --> 1798.48]  like their beautiful
[1798.48 --> 1799.26]  cloud manager
[1799.26 --> 1800.02]  that's well-designed,
[1800.12 --> 1801.56]  the API that's documented
[1801.56 --> 1802.68]  and has lots of libraries
[1802.68 --> 1803.80]  in your favorite language
[1803.80 --> 1805.26]  and the CLI I use
[1805.26 --> 1806.34]  to take quick snapshots
[1806.34 --> 1807.10]  or upload to their
[1807.10 --> 1807.78]  object storage.
[1808.00 --> 1808.96]  All that stuff
[1808.96 --> 1809.72]  that we enjoy,
[1809.92 --> 1811.90]  that really make it possible
[1811.90 --> 1813.06]  to build and deploy
[1813.06 --> 1814.76]  and even do it at scale,
[1814.88 --> 1815.68]  all that stuff,
[1815.74 --> 1816.42]  it's still available,
[1816.56 --> 1817.60]  but now it's combined
[1817.60 --> 1818.30]  with the power
[1818.30 --> 1819.40]  and the global reach
[1819.40 --> 1820.62]  of Akamai.
[1820.96 --> 1822.64]  And Akamai is investing big.
[1823.04 --> 1824.18]  They're expanding services
[1824.18 --> 1824.88]  to offer more
[1824.88 --> 1826.08]  cloud computing resources
[1826.08 --> 1827.52]  and the tooling we love
[1827.52 --> 1828.06]  while giving you
[1828.06 --> 1828.68]  that classic,
[1829.68 --> 1830.16]  reliable,
[1830.74 --> 1831.12]  affordable,
[1831.42 --> 1832.46]  and scalable solutions
[1832.46 --> 1833.70]  for individuals
[1833.70 --> 1834.36]  and businesses
[1834.36 --> 1835.82]  of all sizes.
[1835.98 --> 1836.92]  And as part of Akamai's
[1836.92 --> 1838.06]  global network of offerings,
[1838.32 --> 1838.88]  the data centers
[1838.88 --> 1840.52]  are expanding worldwide,
[1840.52 --> 1841.56]  all over the world,
[1841.64 --> 1842.08]  lots of them,
[1842.16 --> 1843.06]  they're going in big,
[1843.10 --> 1843.54]  you guys,
[1843.64 --> 1844.48]  and they're giving you
[1844.48 --> 1846.04]  access to even more resources
[1846.04 --> 1847.02]  to help you grow
[1847.02 --> 1847.62]  your project,
[1847.80 --> 1848.12]  your site,
[1848.22 --> 1848.70]  your business,
[1848.70 --> 1850.02]  and serve your customers.
[1850.40 --> 1851.18]  That's how we've been
[1851.18 --> 1852.10]  doing it for years now
[1852.10 --> 1853.20]  and we just wouldn't
[1853.20 --> 1854.06]  do it any other way.
[1854.40 --> 1855.14]  Nobody does it better,
[1855.22 --> 1855.78]  so why wait?
[1855.88 --> 1856.68]  Go experience the power
[1856.68 --> 1857.14]  of Linode,
[1857.72 --> 1858.38]  now Akamai.
[1858.94 --> 1860.04]  Go to linode.com
[1860.04 --> 1861.06]  slash SSH,
[1861.22 --> 1861.92]  learn how Linode,
[1861.92 --> 1863.08]  now Akamai can help you
[1863.08 --> 1863.94]  scale your applications
[1863.94 --> 1864.68]  from the cloud
[1864.68 --> 1865.60]  all the way out
[1865.60 --> 1866.92]  to the very edge.
[1867.06 --> 1867.96]  Linode.com
[1867.96 --> 1869.82]  slash SSH.
[1871.82 --> 1872.96]  We got a lot of feedback
[1872.96 --> 1874.22]  over the last couple of weeks
[1874.22 --> 1875.26]  about Obsidian,
[1875.50 --> 1877.20]  a couple of choice quotes
[1877.20 --> 1878.32]  from various listeners.
[1878.88 --> 1879.98]  Dimitri wrote in
[1879.98 --> 1881.00]  agreeing that Obsidian
[1881.00 --> 1882.84]  is truly the way
[1882.84 --> 1883.60]  and he suggests
[1883.60 --> 1885.04]  SyncThing for Android users.
[1885.46 --> 1886.72]  This is a popular one,
[1886.80 --> 1887.70]  not a great option
[1887.70 --> 1888.34]  for iOS,
[1888.76 --> 1889.66]  I have to underscore,
[1889.66 --> 1890.74]  but if you got
[1890.74 --> 1892.14]  SyncThing on your desktop
[1892.14 --> 1892.86]  or your server
[1892.86 --> 1893.64]  and you got SyncThing
[1893.64 --> 1894.80]  on your Android device,
[1895.00 --> 1896.22]  you can basically
[1896.22 --> 1897.62]  use Obsidian Sync,
[1897.94 --> 1898.24]  well,
[1898.40 --> 1899.46]  that for Sync
[1899.46 --> 1901.24]  and multiple people
[1901.24 --> 1901.78]  wrote in
[1901.78 --> 1902.44]  and boosted
[1902.44 --> 1903.18]  and saying it works.
[1903.70 --> 1904.70]  I, of course,
[1905.24 --> 1906.90]  because I'm a glutton
[1906.90 --> 1907.48]  for punishment,
[1907.80 --> 1909.68]  I have my primary use case
[1909.68 --> 1910.34]  is the desktop
[1910.34 --> 1912.20]  and my next use case
[1912.20 --> 1912.94]  would be my
[1912.94 --> 1913.66]  Pyzell 7
[1913.66 --> 1914.86]  because I'm an Android user now,
[1914.86 --> 1917.06]  but in the garage,
[1917.06 --> 1918.38]  I have an iPad
[1918.38 --> 1919.24]  with a keyboard
[1919.24 --> 1920.30]  that I want to use
[1920.30 --> 1920.92]  for notes
[1920.92 --> 1922.20]  while I'm working out there
[1922.20 --> 1923.86]  and so I have to be able
[1923.86 --> 1924.82]  to sync to iOS.
[1925.24 --> 1926.24]  So I did it, Alex.
[1926.34 --> 1927.68]  I bought Obsidian Sync.
[1928.30 --> 1929.60]  One of my favorite things
[1929.60 --> 1930.16]  and one of the things
[1930.16 --> 1931.02]  that really put me over,
[1931.26 --> 1931.90]  this is stupid,
[1933.26 --> 1934.40]  but when you told me
[1934.40 --> 1935.40]  that Obsidian Sync
[1935.40 --> 1936.58]  syncs themes
[1936.58 --> 1937.14]  and plugins
[1937.14 --> 1939.72]  and that they were per vault,
[1939.94 --> 1940.82]  I was in
[1940.82 --> 1943.62]  because then I could have vaults.
[1943.62 --> 1944.88]  So the wife and I
[1944.88 --> 1945.80]  are sharing a login,
[1946.04 --> 1946.62]  sorry Obsidian,
[1947.12 --> 1948.46]  and she just opens
[1948.46 --> 1949.60]  the vaults on her devices
[1949.60 --> 1950.28]  she cares about
[1950.28 --> 1951.80]  and it works perfectly
[1951.80 --> 1952.58]  and I have them
[1952.58 --> 1953.18]  like kind of more
[1953.18 --> 1953.98]  minimal plugins.
[1954.24 --> 1954.84]  I have a, you know,
[1954.86 --> 1955.88]  a nice theme for her.
[1956.42 --> 1957.18]  So far,
[1957.24 --> 1958.14]  that's working really,
[1958.26 --> 1958.84]  really well.
[1959.06 --> 1960.74]  I've also had to shift
[1960.74 --> 1963.00]  from like the Evernote
[1963.00 --> 1964.40]  philosophy of capture
[1964.40 --> 1965.22]  everything
[1965.22 --> 1966.68]  and then sort it out later
[1966.68 --> 1968.18]  to just
[1968.18 --> 1969.30]  with Obsidian,
[1969.38 --> 1970.18]  I think it works better
[1970.18 --> 1970.52]  if
[1970.52 --> 1972.56]  only capture the things
[1972.56 --> 1973.34]  you think you might need
[1973.34 --> 1973.62]  later
[1973.62 --> 1975.26]  and link to stuff
[1975.26 --> 1976.22]  and it's just,
[1976.32 --> 1977.24]  that's just a transition
[1977.24 --> 1977.92]  I have to make
[1977.92 --> 1978.64]  but I think it's one
[1978.64 --> 1979.62]  I'm going to get behind.
[1979.84 --> 1980.48]  It's really interesting
[1980.48 --> 1981.68]  for documentation though
[1981.68 --> 1982.14]  as well.
[1982.28 --> 1982.80]  Like if you,
[1983.44 --> 1983.74]  I mean,
[1983.76 --> 1984.96]  I don't typically use
[1984.96 --> 1986.04]  the graph view
[1986.04 --> 1987.06]  for very much at all
[1987.06 --> 1988.14]  but as I've been,
[1988.18 --> 1988.94]  you know,
[1989.00 --> 1989.92]  acquiring notes
[1989.92 --> 1990.82]  ahead of this track day
[1990.82 --> 1991.44]  I did at the weekend
[1991.44 --> 1992.06]  for the car,
[1992.18 --> 1992.34]  you know,
[1992.66 --> 1993.38]  what brake pads
[1993.38 --> 1993.90]  did I run
[1993.90 --> 1994.92]  and then even whilst
[1994.92 --> 1995.50]  I was at the event
[1995.50 --> 1996.14]  like what were my
[1996.14 --> 1996.68]  tire pressures
[1996.68 --> 1997.78]  after a certain session
[1997.78 --> 1998.12]  and just,
[1998.34 --> 1998.50]  Oh,
[1998.84 --> 1999.32]  interesting,
[1999.48 --> 1999.70]  yeah.
[2000.04 --> 2000.68]  You'll forget.
[2001.02 --> 2001.28]  Yeah,
[2001.46 --> 2001.80]  you know,
[2001.86 --> 2002.64]  it's important to keep
[2002.64 --> 2003.30]  a record of that stuff
[2003.30 --> 2004.18]  like ambient temperature
[2004.18 --> 2004.80]  was this
[2004.80 --> 2006.02]  and so my tires
[2006.02 --> 2006.72]  came in at the end
[2006.72 --> 2007.24]  of this session
[2007.24 --> 2008.46]  this temperature
[2008.46 --> 2009.50]  and with this pressure
[2009.50 --> 2009.82]  etc.
[2010.42 --> 2011.18]  Like normally
[2011.18 --> 2011.96]  that stuff would end up
[2011.96 --> 2012.76]  in a paper notebook
[2012.76 --> 2013.78]  and I'd have to physically
[2013.78 --> 2015.22]  go and get it
[2015.22 --> 2015.78]  and remember that
[2015.78 --> 2016.86]  it's linked in my mind
[2016.86 --> 2017.60]  to the car
[2017.60 --> 2018.16]  for example.
[2018.16 --> 2020.00]  But what I did
[2020.00 --> 2020.64]  was just quickly
[2020.64 --> 2021.14]  at the track
[2021.14 --> 2021.90]  I just did a
[2021.90 --> 2022.54]  bracket bracket
[2022.54 --> 2024.06]  2019 Golf R
[2024.06 --> 2024.66]  and then that linked
[2024.66 --> 2025.62]  that back to the
[2025.62 --> 2026.82]  the main page
[2026.82 --> 2027.40]  for the car
[2027.40 --> 2028.42]  and then I have
[2028.42 --> 2029.46]  a data view query
[2029.46 --> 2030.18]  that looks at
[2030.18 --> 2030.88]  every note
[2030.88 --> 2031.76]  that has that
[2031.76 --> 2032.58]  phrase in it
[2032.58 --> 2033.42]  or that backlink
[2033.42 --> 2033.82]  in it
[2033.82 --> 2034.98]  and then shows me
[2034.98 --> 2035.38]  it's almost like
[2035.38 --> 2036.20]  a table of contents
[2036.20 --> 2036.90]  for the car
[2036.90 --> 2037.80]  and then it goes
[2037.80 --> 2038.56]  to those sub notes
[2038.56 --> 2039.20]  underneath it
[2039.20 --> 2039.62]  and that's
[2039.62 --> 2041.22]  that kind of
[2041.22 --> 2042.26]  wiki style
[2042.26 --> 2042.94]  functionality
[2042.94 --> 2043.92]  in plain text
[2043.92 --> 2044.36]  notes
[2044.36 --> 2045.72]  I have no idea
[2045.72 --> 2046.94]  how they've done it
[2046.94 --> 2047.74]  but it is
[2047.74 --> 2048.80]  absolute magic.
[2050.42 --> 2051.44]  Yep the magic
[2051.44 --> 2052.16]  is in the linking.
[2052.70 --> 2053.66]  Lewis wrote in
[2053.66 --> 2054.18]  saying well
[2054.18 --> 2055.26]  he was perfectly
[2055.26 --> 2056.66]  happy with Joplin
[2056.66 --> 2058.12]  until the last
[2058.12 --> 2058.68]  episode of
[2058.68 --> 2059.28]  Self Hosted
[2059.28 --> 2059.82]  and now he's
[2059.82 --> 2060.98]  migrating to Obsidian.
[2061.88 --> 2062.38]  Yeah we had
[2062.38 --> 2063.08]  that sentiment
[2063.08 --> 2063.66]  come in
[2063.66 --> 2064.76]  across the various
[2064.76 --> 2065.20]  channels.
[2065.52 --> 2066.56]  I'm sorry about that.
[2066.92 --> 2067.46]  I hope you
[2067.46 --> 2068.58]  are suffering
[2068.58 --> 2069.48]  and I hope
[2069.48 --> 2069.96]  it's going
[2069.96 --> 2070.80]  horribly for you
[2070.80 --> 2071.34]  so that way
[2071.34 --> 2072.50]  you feel slightly
[2072.50 --> 2073.66]  just a little
[2073.66 --> 2074.18]  tiny bit
[2074.18 --> 2074.62]  of the pain
[2074.62 --> 2075.56]  that I've had
[2075.56 --> 2075.94]  to feel
[2075.94 --> 2076.72]  for the last
[2076.72 --> 2077.24]  few weeks
[2077.24 --> 2077.98]  and I hope
[2077.98 --> 2078.70]  you continue
[2078.70 --> 2079.96]  to endure it.
[2080.58 --> 2081.28]  No not really
[2081.28 --> 2082.46]  but a little bit.
[2082.98 --> 2084.04]  It's a good
[2084.04 --> 2085.32]  project I think
[2085.32 --> 2085.98]  and I know
[2085.98 --> 2086.60]  at this point
[2086.60 --> 2087.16]  we probably
[2087.16 --> 2087.92]  sound like Obsidian
[2087.92 --> 2088.82]  Shills or whatever
[2088.82 --> 2090.52]  but we've got
[2090.52 --> 2091.10]  no relationship
[2091.10 --> 2091.48]  to them.
[2091.54 --> 2091.98]  They're not even
[2091.98 --> 2092.86]  really technically
[2092.86 --> 2093.86]  a self-hosted
[2093.86 --> 2095.04]  app in the
[2095.04 --> 2095.84]  truest sense.
[2096.04 --> 2096.74]  They're not even
[2096.74 --> 2098.10]  really open source
[2098.10 --> 2098.60]  either.
[2099.18 --> 2099.86]  It's a bit of
[2099.86 --> 2100.66]  an awkward one
[2100.66 --> 2101.30]  to be talking
[2101.30 --> 2101.82]  about so much
[2101.82 --> 2102.32]  in the show
[2102.32 --> 2103.74]  but
[2103.74 --> 2104.72]  I think
[2104.72 --> 2105.26]  from a data
[2105.26 --> 2105.82]  sovereignty
[2105.82 --> 2106.64]  point of view
[2106.64 --> 2107.54]  that's where
[2107.54 --> 2108.06]  it absolutely
[2108.06 --> 2108.64]  wins out
[2108.64 --> 2109.26]  and that's
[2109.26 --> 2110.22]  always the
[2110.22 --> 2110.82]  balance we try
[2110.82 --> 2111.18]  and strike
[2111.18 --> 2111.76]  on this show
[2111.76 --> 2112.84]  is some
[2112.84 --> 2113.26]  kind of a
[2113.26 --> 2113.60]  pragmatic
[2113.60 --> 2114.22]  balance
[2114.22 --> 2114.74]  between
[2114.74 --> 2115.98]  the various
[2115.98 --> 2116.46]  principles
[2116.46 --> 2117.06]  and pillars
[2117.06 --> 2117.90]  of the
[2117.90 --> 2118.68]  different aspects
[2118.68 --> 2119.56]  of self-hosting
[2119.56 --> 2121.04]  and for me
[2121.04 --> 2121.68]  Obsidian really
[2121.68 --> 2122.20]  wins out
[2122.20 --> 2123.00]  because I
[2123.00 --> 2124.06]  own the
[2124.06 --> 2125.22]  data 100%
[2125.22 --> 2125.60]  you know
[2125.60 --> 2125.90]  they've got
[2125.90 --> 2126.32]  the local
[2126.32 --> 2127.02]  files on my
[2127.02 --> 2127.74]  on my disc
[2127.74 --> 2128.18]  right now
[2128.18 --> 2128.56]  in front of me
[2128.56 --> 2128.98]  I can open
[2128.98 --> 2129.62]  them in any
[2129.62 --> 2130.54]  editor I want
[2130.54 --> 2131.14]  not just
[2131.14 --> 2131.54]  Obsidian
[2131.54 --> 2132.84]  yeah for me
[2132.84 --> 2133.46]  that was
[2133.46 --> 2134.52]  the deal breaker
[2134.52 --> 2135.14]  was I had to
[2135.14 --> 2135.94]  have the files
[2135.94 --> 2136.46]  offline
[2136.46 --> 2137.36]  I wanted to
[2137.36 --> 2137.66]  have them
[2137.66 --> 2138.30]  locally in a
[2138.30 --> 2138.96]  standard format
[2138.96 --> 2139.50]  if I could
[2139.50 --> 2140.14]  mark down in
[2140.14 --> 2140.62]  this case
[2140.62 --> 2141.62]  and that's the
[2141.62 --> 2142.24]  way exactly
[2142.24 --> 2142.72]  that their
[2142.72 --> 2143.58]  sync tool works
[2143.58 --> 2144.28]  is it it
[2144.28 --> 2144.70]  syncs the
[2144.70 --> 2145.52]  files to
[2145.52 --> 2146.44]  your local
[2146.44 --> 2147.16]  file system
[2147.16 --> 2148.06]  and the fact
[2148.06 --> 2148.86]  that you can
[2148.86 --> 2149.52]  put something
[2149.52 --> 2151.10]  like sync
[2151.10 --> 2151.48]  thing in the
[2151.48 --> 2151.94]  back end
[2151.94 --> 2152.94]  or git
[2152.94 --> 2153.38]  or something
[2153.38 --> 2154.72]  else to move
[2154.72 --> 2155.22]  those files
[2155.22 --> 2155.82]  if you'd like
[2155.82 --> 2157.30]  I think
[2157.30 --> 2157.78]  gives me
[2157.78 --> 2158.22]  the option
[2158.22 --> 2158.56]  to say
[2158.56 --> 2159.04]  well okay
[2159.04 --> 2159.36]  I'm done
[2159.36 --> 2159.74]  with the
[2159.74 --> 2160.08]  sync thing
[2160.08 --> 2160.40]  service
[2160.40 --> 2160.88]  thanks so
[2160.88 --> 2161.16]  much
[2161.16 --> 2161.88]  see you
[2161.88 --> 2162.04]  later
[2162.04 --> 2162.58]  I'll do
[2162.58 --> 2163.20]  another way
[2163.20 --> 2163.58]  one day
[2163.58 --> 2164.18]  if I want
[2164.18 --> 2166.06]  so I was
[2166.06 --> 2166.62]  okay with it
[2166.62 --> 2167.34]  have you tried
[2167.34 --> 2167.90]  mixing and
[2167.90 --> 2168.60]  matching sync
[2168.60 --> 2169.30]  services yet
[2169.30 --> 2170.02]  I mean I know
[2170.02 --> 2170.56]  the Obsidian
[2170.56 --> 2171.18]  sync service
[2171.18 --> 2171.78]  works across
[2171.78 --> 2172.50]  all platforms
[2172.50 --> 2173.74]  but you know
[2173.74 --> 2174.08]  it's almost
[2174.08 --> 2174.70]  like a
[2174.70 --> 2175.68]  insurance policy
[2175.68 --> 2176.02]  like
[2176.02 --> 2177.22]  I was initially
[2177.22 --> 2178.00]  trying to do
[2178.00 --> 2178.18]  it over
[2178.18 --> 2178.76]  next cloud
[2178.76 --> 2179.34]  but then
[2179.34 --> 2179.98]  couldn't get
[2179.98 --> 2180.42]  real-time
[2180.42 --> 2181.04]  syncing to
[2181.04 --> 2181.30]  mobile
[2181.30 --> 2181.70]  which really
[2181.70 --> 2182.36]  kind of
[2182.36 --> 2182.72]  sealed the
[2182.72 --> 2182.86]  deal
[2182.86 --> 2183.12]  because the
[2183.12 --> 2183.44]  wife needs
[2183.44 --> 2183.72]  the full
[2183.72 --> 2184.00]  mobile
[2184.00 --> 2184.48]  experience
[2184.48 --> 2184.80]  Alex
[2184.80 --> 2185.38]  you know
[2185.38 --> 2185.64]  what I mean
[2185.64 --> 2186.40]  did your
[2186.40 --> 2186.68]  iPhone
[2186.68 --> 2187.24]  turn back
[2187.24 --> 2187.64]  on yet
[2187.64 --> 2188.50]  yeah it
[2188.50 --> 2189.02]  did actually
[2189.02 --> 2189.94]  after it
[2189.94 --> 2190.40]  sat for a
[2190.40 --> 2190.74]  couple of
[2190.74 --> 2191.18]  days I
[2191.18 --> 2191.42]  think it
[2191.42 --> 2192.12]  fully drained
[2192.12 --> 2193.32]  itself and
[2193.32 --> 2193.60]  then I
[2193.60 --> 2194.04]  plugged it
[2194.04 --> 2194.98]  in again
[2194.98 --> 2195.82]  and it
[2195.82 --> 2196.38]  booted up
[2196.38 --> 2196.54]  you know
[2196.54 --> 2196.72]  I had to
[2196.72 --> 2196.90]  do the
[2196.90 --> 2197.48]  full charge
[2197.48 --> 2198.18]  so I
[2198.18 --> 2198.50]  think maybe
[2198.50 --> 2198.72]  it was
[2198.72 --> 2199.20]  like locked
[2199.20 --> 2200.08]  up and
[2200.08 --> 2200.36]  it just
[2200.36 --> 2201.08]  wouldn't go
[2201.08 --> 2201.42]  anywhere until
[2201.42 --> 2201.72]  the phone
[2201.72 --> 2202.14]  died but I
[2202.14 --> 2202.58]  tried plugging
[2202.58 --> 2202.96]  that sucker
[2202.96 --> 2203.34]  into a
[2203.34 --> 2203.76]  Mac I
[2203.76 --> 2204.24]  tried plugging
[2204.24 --> 2204.64]  it into
[2204.64 --> 2205.08]  the wall
[2205.08 --> 2205.52]  outlet
[2205.52 --> 2206.50]  all the
[2206.50 --> 2207.14]  things you
[2207.14 --> 2207.32]  know I
[2207.32 --> 2207.62]  tried all
[2207.62 --> 2207.94]  the track
[2207.94 --> 2208.22]  I tried
[2208.22 --> 2208.58]  holding all
[2208.58 --> 2208.92]  the buttons
[2208.92 --> 2209.20]  you're supposed
[2209.20 --> 2209.70]  to hold
[2209.70 --> 2210.14]  I did the
[2210.14 --> 2210.76]  whole dance
[2210.76 --> 2211.84]  I feel like
[2211.84 --> 2212.46]  Apple's on a
[2212.46 --> 2213.18]  weird trajectory
[2213.18 --> 2213.70]  at the minute
[2213.70 --> 2214.56]  do you feel
[2214.56 --> 2214.98]  this too
[2214.98 --> 2216.28]  in was it
[2216.28 --> 2217.04]  Ventura the
[2217.04 --> 2217.82]  latest Mac OS
[2217.82 --> 2218.28]  this is going
[2218.28 --> 2218.50]  to be a
[2218.50 --> 2219.12]  complete tangent
[2219.12 --> 2219.66]  from the
[2219.66 --> 2220.68]  doc by the
[2220.68 --> 2221.26]  way but
[2221.26 --> 2222.10]  have you ever
[2222.10 --> 2222.56]  tried to set
[2222.56 --> 2222.96]  a static
[2222.96 --> 2223.94]  IP on the
[2223.94 --> 2224.36]  new version
[2224.36 --> 2224.90]  of Mac OS
[2224.90 --> 2225.62]  no I don't
[2225.62 --> 2225.96]  think so
[2225.96 --> 2227.36]  it's an
[2227.36 --> 2227.68]  absolute
[2227.68 --> 2228.12]  show
[2228.12 --> 2229.76]  it just
[2229.76 --> 2230.24]  doesn't do
[2230.24 --> 2230.48]  it
[2230.48 --> 2231.30]  so like a
[2231.30 --> 2231.86]  couple of
[2231.86 --> 2232.24]  months ago
[2232.24 --> 2232.68]  when I was
[2232.68 --> 2233.08]  doing all
[2233.08 --> 2233.60]  the networking
[2233.60 --> 2234.08]  stuff
[2234.08 --> 2234.50]  we never
[2234.50 --> 2234.88]  talked about
[2234.88 --> 2235.10]  this in
[2235.10 --> 2235.42]  the show
[2235.42 --> 2236.40]  but I
[2236.40 --> 2236.92]  was trying
[2236.92 --> 2237.64]  my damnedest
[2237.64 --> 2238.20]  to set
[2238.20 --> 2238.66]  a static
[2238.66 --> 2240.04]  IP on
[2240.04 --> 2240.42]  because I
[2240.42 --> 2240.98]  knew what
[2240.98 --> 2241.88]  the IP
[2241.88 --> 2242.44]  address of a
[2242.44 --> 2242.98]  certain thing
[2242.98 --> 2243.32]  was on the
[2243.32 --> 2243.58]  network
[2243.58 --> 2244.22]  the DHCP
[2244.22 --> 2244.82]  server was
[2244.82 --> 2245.02]  down
[2245.02 --> 2245.26]  I'm like
[2245.26 --> 2245.50]  right
[2245.50 --> 2246.16]  if I give
[2246.16 --> 2246.60]  my laptop
[2246.60 --> 2247.04]  a static
[2247.04 --> 2247.58]  IP I can
[2247.58 --> 2247.96]  get into
[2247.96 --> 2248.50]  OpenSense
[2248.50 --> 2248.94]  and turn
[2248.94 --> 2249.70]  the DHCP
[2249.70 --> 2250.34]  server back
[2250.34 --> 2250.68]  on again
[2250.68 --> 2251.12]  and everything
[2251.12 --> 2251.76]  will be fine
[2251.76 --> 2253.80]  but the
[2253.80 --> 2254.40]  new Mac OS
[2254.40 --> 2254.88]  nope
[2254.88 --> 2255.58]  you cannot
[2255.58 --> 2256.48]  manually do
[2256.48 --> 2256.80]  that
[2256.80 --> 2257.38]  no
[2257.38 --> 2258.66]  under certain
[2258.66 --> 2259.42]  circumstances
[2259.42 --> 2260.40]  which includes
[2260.40 --> 2261.48]  no internet
[2261.48 --> 2262.80]  no way
[2262.80 --> 2263.08]  dude
[2263.08 --> 2264.32]  no way
[2264.32 --> 2265.52]  no way
[2265.52 --> 2266.02]  you're telling
[2266.02 --> 2266.38]  me
[2266.38 --> 2267.30]  no way
[2267.30 --> 2267.60]  you're telling
[2267.60 --> 2267.86]  me when
[2267.86 --> 2268.36]  Mac OS
[2268.36 --> 2268.80]  doesn't have
[2268.80 --> 2269.18]  an internet
[2269.18 --> 2269.66]  connection
[2269.66 --> 2270.20]  it doesn't
[2270.20 --> 2270.68]  let you set
[2270.68 --> 2271.22]  a manual
[2271.22 --> 2271.56]  IP
[2271.56 --> 2273.48]  no way
[2273.48 --> 2273.86]  it's a
[2273.86 --> 2274.40]  feature now
[2274.40 --> 2275.50]  in Ventura
[2275.50 --> 2277.02]  that was
[2277.02 --> 2278.10]  it 11 point
[2278.10 --> 2278.86]  I don't even
[2278.86 --> 2279.10]  know what
[2279.10 --> 2279.66]  version numbers
[2279.66 --> 2280.18]  that's blowing
[2280.18 --> 2281.06]  my mind
[2281.06 --> 2281.76]  13 point
[2281.76 --> 2282.26]  I'm on
[2282.26 --> 2283.04]  13.4
[2283.04 --> 2283.48]  over here
[2283.48 --> 2283.80]  yep
[2283.80 --> 2284.72]  it's frustrating
[2284.72 --> 2285.30]  as all hell
[2285.30 --> 2286.76]  well at least
[2286.76 --> 2287.24]  the machines
[2287.24 --> 2287.98]  are $6,000
[2287.98 --> 2288.52]  when you
[2288.52 --> 2289.16]  properly spec
[2289.16 --> 2289.36]  them
[2289.36 --> 2290.24]  well it makes
[2290.24 --> 2290.88]  that framework
[2290.88 --> 2291.36]  that we talked
[2291.36 --> 2291.82]  about in the
[2291.82 --> 2292.18]  post show
[2292.18 --> 2292.74]  last week
[2292.74 --> 2294.00]  look smarter
[2294.00 --> 2294.66]  and smarter
[2294.66 --> 2295.12]  doesn't it
[2295.12 --> 2296.70]  I cancelled
[2296.70 --> 2297.26]  my pre-order
[2297.26 --> 2297.78]  for the
[2297.78 --> 2298.68]  AMD one
[2298.68 --> 2299.24]  by the way
[2299.24 --> 2299.68]  because we
[2299.68 --> 2300.10]  talked in the
[2300.10 --> 2300.38]  post show
[2300.38 --> 2300.78]  last week
[2300.78 --> 2301.52]  about quick sync
[2301.52 --> 2302.44]  and how if I'm
[2302.44 --> 2302.78]  going to use it
[2302.78 --> 2303.36]  as a server
[2303.36 --> 2304.34]  one day you
[2304.34 --> 2304.56]  might
[2304.56 --> 2304.96]  and the
[2304.96 --> 2305.38]  Thunderbolt
[2305.38 --> 2305.86]  stuff
[2305.86 --> 2306.92]  yeah so I've
[2306.92 --> 2307.38]  gone for the
[2307.38 --> 2307.94]  pre-order for
[2307.94 --> 2309.32]  the i5
[2309.32 --> 2309.86]  framework
[2309.86 --> 2310.48]  which will also
[2310.48 --> 2311.12]  be here in
[2311.12 --> 2311.82]  a month or
[2311.82 --> 2312.50]  two hopefully
[2312.50 --> 2313.46]  not six
[2313.46 --> 2314.94]  yeah that's
[2314.94 --> 2315.54]  also nice
[2315.54 --> 2316.56]  I'm still
[2316.56 --> 2317.64]  hopeful that
[2317.64 --> 2318.96]  that the
[2318.96 --> 2319.68]  Asahi project
[2319.68 --> 2321.30]  gets a really
[2321.30 --> 2322.74]  really competent
[2322.74 --> 2323.52]  headless
[2323.52 --> 2324.88]  Linux server
[2324.88 --> 2325.34]  setup
[2325.34 --> 2326.22]  so that way
[2326.22 --> 2326.78]  I can just
[2326.78 --> 2327.38]  use like an
[2327.38 --> 2328.12]  M1 Mac mini
[2328.12 --> 2329.68]  as a home
[2329.68 --> 2330.18]  server or
[2330.18 --> 2330.42]  something
[2330.42 --> 2331.04]  that's what
[2331.04 --> 2331.58]  my hope is
[2331.58 --> 2332.38]  I hope so
[2332.38 --> 2332.94]  too but
[2332.94 --> 2333.82]  let's be honest
[2333.82 --> 2334.30]  you're dreaming
[2334.30 --> 2334.82]  lad you're
[2334.82 --> 2335.12]  dreaming
[2335.12 --> 2337.24]  I'm dreaming
[2337.24 --> 2337.64]  about a
[2337.64 --> 2338.06]  Hunnigan who
[2338.06 --> 2338.52]  boosted in with
[2338.52 --> 2339.76]  40,000 sats
[2339.76 --> 2340.22]  just says
[2340.22 --> 2341.28]  great show
[2341.28 --> 2341.96]  thank you
[2341.96 --> 2342.40]  Hunnigan for
[2342.40 --> 2342.92]  sending in some
[2342.92 --> 2343.28]  value
[2343.28 --> 2344.14]  Active Shadow
[2344.14 --> 2344.90]  came in with
[2344.90 --> 2346.32]  30,000 sats
[2346.32 --> 2347.64]  sending in from
[2347.64 --> 2347.98]  Fountain
[2347.98 --> 2348.42]  just say I
[2348.42 --> 2348.82]  wanted to say
[2348.82 --> 2349.28]  thanks for the
[2349.28 --> 2349.66]  show I was
[2349.66 --> 2350.16]  curious if
[2350.16 --> 2350.94]  either of you
[2350.94 --> 2352.60]  have ever used
[2352.60 --> 2353.62]  the VS Code
[2353.62 --> 2354.50]  dev containers
[2354.50 --> 2355.56]  I live by them
[2355.56 --> 2356.28]  they keep my
[2356.28 --> 2357.20]  base Arch Linux
[2357.20 --> 2358.26]  with Hyperland
[2358.26 --> 2359.98]  install clean
[2359.98 --> 2361.04]  it allows different
[2361.04 --> 2361.80]  versions of languages
[2361.80 --> 2362.72]  for different projects
[2362.72 --> 2363.60]  and make sharing
[2363.60 --> 2364.12]  the development
[2364.12 --> 2365.50]  environment easy
[2365.50 --> 2366.52]  that's a really
[2366.52 --> 2367.16]  great idea
[2367.16 --> 2368.46]  I don't but I do
[2368.46 --> 2370.22]  use the VS Code
[2370.22 --> 2370.90]  web server
[2370.90 --> 2371.82]  I'm sure you must
[2371.82 --> 2372.62]  use that too Alex
[2372.62 --> 2374.34]  yeah I do love
[2374.34 --> 2375.82]  the VS Code
[2375.82 --> 2377.56]  in a container
[2377.56 --> 2378.44]  I actually use the
[2378.44 --> 2378.92]  heck out of it
[2378.92 --> 2379.48]  in Home Assistant
[2379.48 --> 2380.36]  it's kind of built
[2380.36 --> 2380.88]  in as one of the
[2380.88 --> 2381.20]  plugins
[2381.20 --> 2382.58]  I use the heck
[2382.58 --> 2382.96]  out of that
[2382.96 --> 2383.38]  over there
[2383.38 --> 2384.78]  but I don't know
[2384.78 --> 2385.08]  if you remember
[2385.08 --> 2385.70]  we talked about
[2385.70 --> 2386.22]  that I went to
[2386.22 --> 2386.84]  All Things Open
[2386.84 --> 2387.44]  in October
[2387.44 --> 2388.66]  and I went to
[2388.66 --> 2389.66]  a talk by a
[2389.66 --> 2390.16]  chap called
[2390.16 --> 2391.32]  Scott Hanselman
[2391.32 --> 2392.08]  who is a
[2392.08 --> 2392.54]  developer
[2392.54 --> 2393.50]  I think a
[2393.50 --> 2394.22]  developer advocate
[2394.22 --> 2394.80]  over at
[2394.80 --> 2395.18]  Microsoft
[2395.18 --> 2396.58]  if you've never
[2396.58 --> 2397.44]  heard Scott
[2397.44 --> 2398.10]  talk by the way
[2398.10 --> 2398.58]  and you see him
[2398.58 --> 2399.18]  on a conference
[2399.18 --> 2400.24]  schedule
[2400.24 --> 2402.20]  ignore all the
[2402.20 --> 2402.66]  other sessions
[2402.66 --> 2403.38]  that are clashing
[2403.38 --> 2403.72]  with him
[2403.72 --> 2404.30]  he is one of
[2404.30 --> 2405.08]  the most engaging
[2405.08 --> 2406.06]  speakers you will
[2406.06 --> 2406.74]  ever have the
[2406.74 --> 2407.28]  pleasure of going
[2407.28 --> 2408.84]  to listen to
[2408.84 --> 2409.92]  but he gave a
[2409.92 --> 2410.96]  presentation about
[2410.96 --> 2412.14]  VS Code and
[2412.14 --> 2413.00]  the dev containers
[2413.00 --> 2413.64]  that were in there
[2413.64 --> 2414.82]  I remember at the
[2414.82 --> 2415.44]  time thinking
[2415.44 --> 2416.36]  yeah these look
[2416.36 --> 2417.42]  amazing why am I
[2417.42 --> 2418.02]  using these
[2418.02 --> 2419.82]  and then got home
[2419.82 --> 2421.08]  and I don't know
[2421.08 --> 2422.06]  had to give Archie
[2422.06 --> 2422.82]  some scritches and
[2422.82 --> 2423.46]  forgot about it
[2423.46 --> 2424.98]  so thank you very
[2424.98 --> 2425.94]  much for writing in
[2425.94 --> 2427.04]  I will put this at
[2427.04 --> 2427.70]  the top of my list
[2427.70 --> 2428.50]  and give it another
[2428.50 --> 2428.82]  look
[2428.82 --> 2429.78]  it does look really
[2429.78 --> 2430.38]  fantastic I was
[2430.38 --> 2431.08]  just looking it up
[2431.08 --> 2432.06]  while you were
[2432.06 --> 2432.72]  talking and it does
[2432.72 --> 2433.22]  look great
[2433.22 --> 2434.50]  Kyocera comes in
[2434.50 --> 2435.48]  with a row of
[2435.48 --> 2436.04]  McDucks
[2436.04 --> 2437.88]  22,222 sats
[2437.88 --> 2439.00]  Chris asks about
[2439.00 --> 2439.68]  something like
[2439.68 --> 2440.56]  Fasten and would
[2440.56 --> 2441.12]  it work without
[2441.12 --> 2442.10]  insurance we were
[2442.10 --> 2442.70]  talking about that
[2442.70 --> 2443.76]  tool that lets you
[2443.76 --> 2444.18]  connect to your
[2444.18 --> 2444.94]  medical records
[2444.94 --> 2446.44]  easy the insurance
[2446.44 --> 2447.08]  provider isn't
[2447.08 --> 2447.88]  responsible for the
[2447.88 --> 2448.56]  health records the
[2448.56 --> 2449.64]  doctor's offices
[2449.64 --> 2451.88]  that's why it's huge
[2451.88 --> 2453.18]  and Apple Health
[2453.18 --> 2454.16]  doing this was also
[2454.16 --> 2454.96]  massive and the
[2454.96 --> 2455.78]  idea being that you
[2455.78 --> 2456.36]  could electronically
[2456.36 --> 2457.16]  connect it over an
[2457.16 --> 2458.42]  API get your
[2458.42 --> 2459.46]  medical records and
[2459.46 --> 2460.18]  store them yourself
[2460.18 --> 2460.98]  and then just have
[2460.98 --> 2462.18]  them next time you go
[2462.18 --> 2462.96]  to a doctor or a
[2462.96 --> 2464.04]  specialist what a
[2464.04 --> 2465.32]  concept what an
[2465.32 --> 2466.94]  idea when I read
[2466.94 --> 2468.16]  this this boost in
[2468.16 --> 2468.78]  the doc I actually
[2468.78 --> 2469.34]  went and looked on
[2469.34 --> 2470.58]  my iPhone and looked
[2470.58 --> 2471.84]  in the health app and
[2471.84 --> 2472.92]  it turns out I can
[2472.92 --> 2474.72]  also connect the
[2474.72 --> 2476.00]  Apple Health app into
[2476.00 --> 2476.92]  I think it's the
[2476.92 --> 2478.20]  my chart system that
[2478.20 --> 2480.30]  my my doctor's office
[2480.30 --> 2481.78]  uses and it works
[2481.78 --> 2482.60]  just as well as
[2482.60 --> 2484.34]  Fasten except I
[2484.34 --> 2486.24]  I assume the data is
[2486.24 --> 2487.24]  stored somewhere on
[2487.24 --> 2488.22]  Apple servers as well
[2488.22 --> 2489.98]  as my iPhone I I
[2489.98 --> 2491.12]  don't know I think it
[2491.12 --> 2492.10]  is stored locally
[2492.10 --> 2493.50]  in your health app
[2493.50 --> 2494.26]  but I think they
[2494.26 --> 2494.86]  encrypted in the
[2494.86 --> 2495.54]  backup to iCloud
[2495.54 --> 2496.66]  you could maybe open
[2496.66 --> 2497.40]  up the health app on
[2497.40 --> 2497.90]  another iCloud
[2497.90 --> 2498.62]  connected device and
[2498.62 --> 2499.10]  find out
[2499.10 --> 2500.36]  that's a good point
[2500.36 --> 2500.94]  maybe I should
[2500.94 --> 2501.58]  that's interesting
[2501.58 --> 2502.42]  okay I didn't know
[2502.42 --> 2503.10]  you could do that
[2503.10 --> 2504.86]  with I I do remember
[2504.86 --> 2507.36]  something about being
[2507.36 --> 2507.84]  able to pull in
[2507.84 --> 2509.72]  records but I I
[2509.72 --> 2510.32]  never really know how
[2510.32 --> 2511.00]  much to trust the
[2511.00 --> 2511.94]  Apple health app but
[2511.94 --> 2512.74]  I've never heard of
[2512.74 --> 2514.68]  anything leaking from
[2514.68 --> 2515.68]  it it's quite nice
[2515.68 --> 2516.34]  like you know the
[2516.34 --> 2517.06]  blood test I talked
[2517.06 --> 2517.72]  about in the last
[2517.72 --> 2518.62]  episode it showed me
[2518.62 --> 2519.58]  all the different you
[2519.58 --> 2521.30]  know ranges of things
[2521.30 --> 2522.72]  that I'm fine for and
[2522.72 --> 2523.42]  a couple of things I
[2523.42 --> 2524.22]  need to work on and
[2524.22 --> 2525.08]  that kind of stuff you
[2525.08 --> 2525.84]  know it pulled that
[2525.84 --> 2526.78]  data into the app and
[2526.78 --> 2528.20]  visualized it in in the
[2528.20 --> 2529.06]  Apple health app yeah
[2529.06 --> 2530.04]  as well as well as
[2530.04 --> 2531.34]  Fasten to Fasten did it
[2531.34 --> 2532.32]  as well it was great
[2532.32 --> 2534.60]  that's cool that's
[2534.60 --> 2535.76]  useful and if it truly
[2535.76 --> 2537.26]  is private that's that's
[2537.26 --> 2538.32]  really great legit
[2538.32 --> 2539.30]  salvage comes in with
[2539.30 --> 2541.66]  10,000 sets hearing you
[2541.66 --> 2542.44]  talk about your notes
[2542.44 --> 2543.40]  made me think are you
[2543.40 --> 2544.64]  talking about notes and
[2544.64 --> 2545.88]  document management as
[2545.88 --> 2547.62]  the same thing do you
[2547.62 --> 2548.60]  distinguish the two
[2548.60 --> 2549.88]  since I haven't found
[2549.88 --> 2550.44]  any open source
[2550.44 --> 2551.52]  solutions yet I don't
[2551.52 --> 2552.54]  have a good comparison
[2552.54 --> 2553.90]  closest I would think
[2553.90 --> 2555.12]  with the Microsoft world
[2555.12 --> 2555.74]  would be like using
[2555.74 --> 2557.36]  OneNote for notes
[2557.36 --> 2558.22]  versus SharePoint
[2558.22 --> 2559.62]  OneNote would be more
[2559.62 --> 2560.76]  creating data like
[2560.76 --> 2561.96]  grocery lists you know
[2561.96 --> 2562.96]  things like jotting
[2562.96 --> 2564.24]  down phone numbers
[2564.24 --> 2564.96]  other things and
[2564.96 --> 2566.32]  SharePoint would be the
[2566.32 --> 2567.66]  finished searchable
[2567.66 --> 2569.32]  product scan mail
[2569.32 --> 2571.20]  receipts warranties
[2571.20 --> 2572.92]  documents I currently use
[2572.92 --> 2573.56]  the notes app in
[2573.56 --> 2574.66]  next cloud it works but
[2574.66 --> 2576.38]  I'm not satisfied I'm
[2576.38 --> 2577.24]  also searching for the
[2577.24 --> 2578.04]  SharePoint replacement
[2578.04 --> 2579.28]  out there I want to
[2579.28 --> 2580.44]  pick up a nice document
[2580.44 --> 2581.72]  scanner to scan every
[2581.72 --> 2582.80]  piece of paper in my
[2582.80 --> 2583.88]  home and any documents
[2583.88 --> 2585.24]  going forward and make
[2585.24 --> 2586.46]  it searchable something
[2586.46 --> 2587.88]  like paperless Nginx
[2587.88 --> 2589.38]  perhaps I haven't tried
[2589.38 --> 2591.00]  it yet what are your
[2591.00 --> 2592.96]  thoughts well I've tried
[2592.96 --> 2593.92]  both of them a couple
[2593.92 --> 2595.16]  of years ago was it
[2595.16 --> 2596.08]  last summer we went
[2596.08 --> 2597.00]  back to England for my
[2597.00 --> 2598.52]  sister's wedding and my
[2598.52 --> 2599.58]  wife is a music teacher
[2599.58 --> 2601.62]  she teaches piano
[2601.62 --> 2602.56]  clarinet that kind of
[2602.56 --> 2603.38]  thing over the internet
[2603.38 --> 2604.68]  and on zoom to some
[2604.68 --> 2605.90]  people and some some
[2605.90 --> 2606.46]  people come to our
[2606.46 --> 2607.12]  house and that kind of
[2607.12 --> 2608.62]  thing and she wanted
[2608.62 --> 2609.86]  to scan in the sheet
[2609.86 --> 2610.82]  music and have it
[2610.82 --> 2612.62]  searchable with OCR for
[2612.62 --> 2613.68]  example for various
[2613.68 --> 2614.56]  different pieces of
[2614.56 --> 2615.36]  music rather than
[2615.36 --> 2617.30]  carrying 25 piano books
[2617.30 --> 2619.00]  across across the ocean
[2619.00 --> 2620.58]  yeah and we use
[2620.58 --> 2622.12]  paperless really heavily
[2622.12 --> 2623.14]  for that and I think
[2623.14 --> 2624.40]  she still uses it for
[2624.40 --> 2625.44]  for those particular
[2625.44 --> 2627.00]  books but there's no
[2627.00 --> 2628.34]  reason why I mean OCR is
[2628.34 --> 2630.10]  OCR is OCR really I
[2630.10 --> 2631.24]  mean there are different
[2631.24 --> 2633.62]  qualities of recognition I
[2633.62 --> 2635.90]  suppose but it's really up
[2635.90 --> 2636.86]  to you how you divide
[2636.86 --> 2637.96]  these things up I mean
[2637.96 --> 2641.42]  the context switching of
[2641.42 --> 2643.34]  documents versus notes
[2643.34 --> 2644.90]  that that line is a grey
[2644.90 --> 2645.90]  one and really only you
[2645.90 --> 2647.92]  can draw it and it it
[2647.92 --> 2648.96]  depends whether you want
[2648.96 --> 2650.02]  to have everything in one
[2650.02 --> 2651.74]  place or have like you
[2651.74 --> 2653.90]  say bills and receipts
[2653.90 --> 2654.74]  and that kind of stuff in
[2654.74 --> 2656.14]  one place and then your
[2656.14 --> 2657.34]  well like I talked about
[2657.34 --> 2658.20]  like tire pressures and
[2658.20 --> 2659.38]  stuff you know that kind
[2659.38 --> 2660.68]  of you know in the moment
[2660.68 --> 2661.80]  notes information
[2661.80 --> 2663.76]  somewhere else it's it's
[2663.76 --> 2665.02]  it's your knowledge base
[2665.02 --> 2666.06]  it's up to you I guess
[2666.06 --> 2667.64]  how you draw the lines
[2667.64 --> 2667.94]  in it
[2667.94 --> 2669.60]  been thinking about the
[2669.60 --> 2671.28]  same kind of questions
[2671.28 --> 2672.46]  I'd love to know your
[2672.46 --> 2673.60]  thoughts anyone out there
[2673.60 --> 2675.24]  listening or legit salvage
[2675.24 --> 2676.92]  which you come to it is
[2676.92 --> 2677.84]  useful to have all that
[2677.84 --> 2679.20]  stuff and as somebody who
[2679.20 --> 2680.50]  pictures themselves on the
[2680.50 --> 2681.72]  road for multiple months
[2681.72 --> 2682.68]  at a time you want to
[2682.68 --> 2684.00]  have a system for inbound
[2684.00 --> 2685.32]  mail and scanning it and
[2685.32 --> 2686.48]  you don't want to carry all
[2686.48 --> 2688.56]  that around so I'm always
[2688.56 --> 2689.50]  interested in people's
[2689.50 --> 2690.86]  thoughts there I want to
[2690.86 --> 2691.62]  say thank you everybody who
[2691.62 --> 2692.72]  boosted and we do that we
[2692.72 --> 2694.30]  do the top four boosts on
[2694.30 --> 2696.20]  the show Todd from
[2696.20 --> 2697.02]  Northern Virginia also
[2697.02 --> 2697.96]  came in with a row of
[2697.96 --> 2698.78]  McDucks but didn't have a
[2698.78 --> 2699.62]  message but just want to
[2699.62 --> 2700.74]  give him a shout out and
[2700.74 --> 2701.54]  thank you everybody else who
[2701.54 --> 2702.46]  boosted and we do read
[2702.46 --> 2703.08]  them there are some great
[2703.08 --> 2703.82]  ones in there and Gene
[2703.82 --> 2705.44]  beans gave me some tools to
[2705.44 --> 2707.10]  check out a few things to
[2707.10 --> 2708.36]  look at so thank you
[2708.36 --> 2709.26]  everybody if you'd like to
[2709.26 --> 2710.74]  boost in the show I say go
[2710.74 --> 2712.86]  get Albie get albie.com top
[2712.86 --> 2713.64]  it off with some little
[2713.64 --> 2714.80]  sats and then over to the
[2714.80 --> 2716.84]  podcast index we have it all
[2716.84 --> 2717.58]  linked to the show notes you
[2717.58 --> 2718.50]  can just boost right there from
[2718.50 --> 2720.10]  the website and of course
[2720.10 --> 2721.28]  you can also subscribe to
[2721.28 --> 2722.54]  the show via the membership
[2722.54 --> 2724.00]  program and you can support
[2724.00 --> 2724.86]  it with those fiat fun
[2724.86 --> 2725.96]  coupons we absolutely
[2725.96 --> 2727.02]  appreciate those members
[2727.02 --> 2728.76]  that is at self hosted dot
[2728.76 --> 2730.38]  show slash sre you get an
[2730.38 --> 2731.60]  ad free feed as a thank you
[2731.60 --> 2734.06]  and that post show Alex is
[2734.06 --> 2735.10]  referring to what post show
[2735.10 --> 2736.56]  yeah our members get a post
[2736.56 --> 2739.02]  show and it's just a way of
[2739.02 --> 2740.42]  saying thank you self hosted
[2740.42 --> 2742.66]  dot show slash sre fiat fun
[2742.66 --> 2744.22]  coupons with no debt ceiling
[2744.22 --> 2748.26]  limit hooray they print what
[2748.26 --> 2749.80]  you have to work for what could
[2749.80 --> 2751.26]  go wrong so if you want to
[2751.26 --> 2752.44]  find out more about the
[2752.44 --> 2753.52]  various different places I'm
[2753.52 --> 2754.50]  online you can go to blog
[2754.50 --> 2755.82]  dot katie's ed dot me and go
[2755.82 --> 2757.34]  to the about me page all my
[2757.34 --> 2758.86]  youtube twitter all that kind
[2758.86 --> 2760.40]  of stuff is linked over there
[2760.40 --> 2761.90]  if you want to write into the
[2761.90 --> 2762.80]  show you can go to self
[2762.80 --> 2764.30]  hosted dot show slash contact
[2764.30 --> 2766.06]  don't forget to let the 45
[2766.06 --> 2768.30]  drives guys know your feedback
[2768.30 --> 2769.54]  on their project as well I
[2769.54 --> 2770.98]  think they said info at 45
[2770.98 --> 2773.30]  drives yeah and show notes
[2773.30 --> 2775.06]  at self hosted dot show slash
[2775.06 --> 2776.86]  98 thanks for joining us
