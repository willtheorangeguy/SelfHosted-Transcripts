[0.00 --> 2.08]  Hello fellow self-hosters, Alex here.
[2.50 --> 5.24]  We've got a super exciting episode up our sleeves today.
[5.76 --> 7.90]  This is one I've been waiting to share with you for a little while.
[8.50 --> 13.30]  It's a pre-recorded interview with Elan, the CTO and co-founder of Plex.
[14.06 --> 17.40]  Chris and I got the chance to talk with Elan during the JB Sprint in August
[17.40 --> 19.48]  from his Hawaii home base.
[20.20 --> 24.64]  We cover lots of ground in this interview with him on topics ranging from electric cars
[24.64 --> 27.98]  to the motivations behind starting Plex in the first place
[27.98 --> 30.40]  and where the project is heading in the future.
[31.02 --> 34.26]  Be sure to stick around though as we have some exciting news
[34.26 --> 37.50]  about the ghost blogging platform's new release to share as well.
[37.90 --> 43.72]  So sit back, relax and enjoy our interview with Elan Feingold from Plex.
[44.46 --> 48.34]  You guys know this, Alex and I are both big Plex users
[48.34 --> 51.00]  and I challenged Alex before the show started
[51.00 --> 55.72]  to attempt an elevator pitch explanation of what Plex is.
[56.24 --> 57.10]  Okay, here we go.
[57.10 --> 62.94]  Plex organises audio and visual media from your personal media libraries
[62.94 --> 66.26]  and allows you to stream it to any playback device.
[66.86 --> 69.10]  And for me, Plex has been a huge gateway drug.
[69.66 --> 71.92]  I had a Synology NAS back in the day
[71.92 --> 76.72]  and now I have a huge server in my basement with 100 plus terabytes
[76.72 --> 80.46]  that has 20 cores and hundreds of gigabytes of RAM
[80.46 --> 84.26]  and I honestly owe an awful lot of that stuff to Plex.
[84.26 --> 90.32]  One of the other cool things that Plex does is that it does on-the-fly media transcoding.
[91.10 --> 96.24]  And why that's important is lots of different media devices support different codecs.
[96.76 --> 100.26]  You know, a web browser might not be able to support the same codecs as an iPhone, for example,
[100.42 --> 102.52]  or an Android TV box.
[102.52 --> 107.78]  And the single most magical feature of Plex is that if I press play on a device,
[107.86 --> 109.44]  there's no configuration required.
[109.86 --> 112.80]  It will just start playing my media as if by magic
[112.80 --> 117.48]  and transcode it from whatever source using FFmpeg to whatever target device.
[117.90 --> 119.54]  It just works and it's wonderful.
[120.04 --> 120.54]  That was pretty good.
[120.60 --> 121.10]  What did you think, Elon?
[121.42 --> 122.00]  I'm impressed.
[122.22 --> 125.94]  Are you looking for a position as our PR spokesperson?
[126.32 --> 127.04]  I love your accent.
[127.16 --> 128.22]  I love the way you can describe that.
[128.32 --> 128.92]  That's brilliant.
[129.10 --> 132.22]  Well, I got out of a speeding ticket with this accent a couple of weeks ago.
[133.40 --> 135.44]  Now, don't be sniping my co-host.
[135.52 --> 136.88]  I just got this thing off the ground.
[137.12 --> 137.44]  Damn it.
[138.60 --> 140.06]  Well, thank you for being here.
[140.66 --> 143.28]  We thought maybe we'd like to start with a few personal questions.
[143.50 --> 147.00]  Our crowd is a lot of a do-yourself-hosted kind of group
[147.00 --> 149.84]  and they love to know what people's setups are.
[150.36 --> 154.00]  And so we would like to ask, at what you consider to be home base,
[154.68 --> 157.16]  roughly how many computers would you say are in the home?
[157.86 --> 158.28]  Yeah, sure.
[159.34 --> 162.34]  I mean, I work personally off a Mac desktop.
[162.64 --> 163.64]  Right now it's a Mac Mini.
[164.70 --> 168.96]  I used to have the Trashcan Mac Pro, but that just got super long in the tooth,
[168.96 --> 172.12]  so I moved to one of the new Mac Minis.
[173.08 --> 175.96]  And then my wife and I both have MacBooks,
[175.96 --> 178.90]  because I really love the fact that they're super light and portable.
[179.24 --> 182.28]  And I don't do a lot of coding on that, mostly on the desktop with a bigger screen.
[182.66 --> 185.58]  And then as far as the media box,
[186.02 --> 192.74]  I have a 3U Norco box with a bunch of hard drives in it,
[192.86 --> 195.46]  probably around 100 terabytes.
[196.74 --> 200.56]  And that's running ZFS on top of Ubuntu,
[201.32 --> 205.40]  which is sort of what most of us at Plex have gravitated towards.
[205.40 --> 208.84]  We really like ZFS or ZFS, if you will.
[209.48 --> 213.96]  Although there are several people that use Unraid, but I tend to use that ZFS.
[214.64 --> 219.70]  And it was an older system, but I just upgraded recently.
[219.88 --> 223.88]  I guess Facebook and a bunch of other companies dumped a bunch of xenons on them,
[224.22 --> 225.62]  like that they were using in data centers.
[225.62 --> 233.10]  So I picked up a couple of eight core, 16 thread xenons for like 100 bucks each.
[233.28 --> 238.88]  So now it's got a total of 16 cores, 32 threads for 200 bucks, which is kind of unbeatable.
[239.58 --> 239.72]  Nice.
[239.94 --> 240.60]  No kidding.
[241.46 --> 244.60]  Now, I kind of got to know with all of that kind of storage and stuff,
[244.66 --> 247.80]  have you invested in a pretty fast local network?
[247.80 --> 252.62]  Well, yeah, when we got the place, we wired it for Cat 6.
[253.82 --> 258.64]  But sadly, I mean, there's Gigabit running to all the important places.
[258.86 --> 263.08]  And I experimented probably about a year ago with trying to go 10 gig,
[263.54 --> 267.72]  just between the Mac Mini, which as you know, like it's Ethernet ports, ports, 10 gig.
[267.72 --> 273.44]  And so I added one of these cheap $100 cards to the Linux system that also supported 10 gig.
[273.80 --> 275.38]  And it kind of worked for like a few days.
[275.58 --> 278.36]  And I would transfer an MKV file back and forth and be like,
[278.42 --> 280.08]  oh my God, 300 megabytes per second.
[280.18 --> 280.58]  That's incredible.
[280.76 --> 284.58]  And then it just like stopped working on the Linux side after a while.
[284.64 --> 287.40]  And I would get like, wouldn't be able to connect and I'd have to reboot.
[287.56 --> 289.20]  And I just was like, okay, fine.
[289.30 --> 292.02]  I'd prefer stable 1 gig over unstable 10 gig.
[292.42 --> 292.56]  Right.
[292.94 --> 293.14]  Yeah.
[293.14 --> 297.40]  I mean, you must have been around in a time where even 1 gigabit would be.
[297.72 --> 299.10]  Just a remarkable transfer rate.
[299.46 --> 299.78]  Oh yeah.
[299.94 --> 300.30]  Incredible.
[300.48 --> 305.50]  I mean, the thing that actually blows my mind nowadays is that with a good Wi-Fi connection,
[305.68 --> 309.50]  you can get up there in at least the hundreds of megabits per second.
[309.70 --> 310.96]  Like that is kind of mind blowing.
[311.10 --> 316.36]  Like I don't think wired is actually really kept up with the accelerating speed of wireless.
[316.86 --> 322.92]  Thank goodness, because it probably makes Plex much more of a real option for people in homes
[322.92 --> 325.40]  that don't have, you know, physical wiring.
[325.74 --> 326.12]  It is true.
[326.12 --> 331.34]  I mean, honestly, I think a technology that people don't give enough credit to is Powerline,
[331.84 --> 334.12]  which is also something that's progressed super fast.
[334.26 --> 340.36]  I had a thing in my living room that I wanted to also speed up with wired and I used Powerline
[340.36 --> 347.44]  and I was able to get about a gigabit, I think, just over Powerline, which is, again, kind of crazy.
[347.54 --> 348.52]  That used to be super flaky.
[348.70 --> 352.92]  It used to, you know, 10 megabits, five megabits, but that's gotten really good too.
[352.92 --> 357.26]  Speaking of power, I was doing a bit of research before the interview.
[357.96 --> 359.52]  How do you like your Tesla Model 3?
[359.84 --> 363.04]  That's some impressive, I'm like looking around for a spy cam now.
[364.56 --> 366.52]  There was some post on Medium that I found.
[367.44 --> 369.20]  Yeah, I love it.
[369.20 --> 373.08]  To me, it's like the future of cars.
[373.66 --> 377.58]  And I know that's a term that is thrown around fairly lightly.
[377.80 --> 386.52]  But I guess the feeling I have with it as it gets software updates and new features over the air is it, you know,
[386.52 --> 391.08]  like I feel like I'm living through the revolution on the way to self-driving cars.
[391.60 --> 394.82]  And I'm not, you know, like as bullish.
[395.38 --> 400.66]  The company is very bullish about full self-driving, end of the year, except for regulations.
[400.66 --> 403.82]  And like, you know, historically, that's always been a lot harder.
[403.82 --> 413.62]  But it's incredibly cool to sort of live through, in theory, have the hardware and just need the software and see the software take incremental steps.
[414.34 --> 416.64]  You know, like, hey, all of a sudden I recognize a stop sign.
[416.86 --> 418.58]  Hey, all of a sudden I know that I stop at a stop sign.
[418.72 --> 426.12]  Like that's, as a nerd geek kind of a guy, like that is an incredibly unique experience in a car, right?
[426.14 --> 428.82]  Usually you get a car, nothing gets updated ever.
[429.76 --> 431.30]  You sell it and get a new car.
[431.42 --> 432.30]  Maybe you get an upgrade.
[432.30 --> 436.38]  So it's really, it feels like a living piece of technology, essentially.
[437.42 --> 439.36]  Did you ever have an iPod back in the day?
[439.50 --> 444.68]  I remember that Apple had a similar kind of, you know, we're used to devices that never see updates.
[444.80 --> 446.34]  We never get new features.
[446.58 --> 450.78]  And I remember having that same kind of journey of discovery with my first iPod.
[451.58 --> 454.02]  I unfortunately came to iPod late.
[455.18 --> 459.78]  Instead, I had one of those creative Zune players, which was just utter crap.
[460.08 --> 460.40]  Oh, yeah.
[460.40 --> 465.52]  Like, no one had figured out back then that really all you needed to do was a simple hierarchy of artist album track.
[465.64 --> 471.52]  Like, no one had figured that out until Apple came along with the iPod and everyone was like, oh, yeah, artist album track.
[471.60 --> 472.54]  That makes total sense.
[472.54 --> 476.98]  But, yeah, I know Apple's always been really good about updates.
[477.50 --> 482.50]  Talking of user interfaces and stuff, the iPod revolutionized things with a click wheel.
[483.02 --> 490.54]  I test drove a Model 3 a few weeks ago, which is why when I saw it, I brought it up because I just wanted to get another person's input into why I should buy one.
[490.54 --> 492.90]  How are you finding the zero buttons thing?
[493.46 --> 494.48]  You should definitely buy one.
[494.90 --> 499.20]  But so I counted because before the Model 3, I had a Leaf.
[499.62 --> 500.82]  So I've been electric for a while.
[500.90 --> 503.30]  I had two successive Leaf leases.
[503.44 --> 504.38]  Say that two times fast.
[504.38 --> 508.34]  And I counted the number of buttons on my Leaf.
[508.48 --> 509.64]  And it was something ridiculous.
[510.00 --> 511.34]  Like, I'm not exaggerating here.
[511.38 --> 519.34]  I think it was something like 60 or 70 buttons in that sort of front hemisphere compared to the Tesla, which was like 10 or something like that.
[519.34 --> 522.94]  But I have slightly mixed feelings.
[523.50 --> 525.92]  For the most part, it works amazingly well.
[526.26 --> 536.78]  And, you know, the sort of the control surfaces that they do have with the D-pad things on your thumbs work super well for various aspects.
[536.78 --> 541.40]  But I do, there are a couple things like opening garage doors.
[542.18 --> 559.62]  And if you have to make adjustments to things, looking, having to look at the screen and hit a tap target while you're driving at 50 or 60 miles an hour is unquestionably less safe than, you know, like feeling from a mechanical switch or knowing where it is.
[559.62 --> 567.76]  So that's a bit, I think that's, but that's essentially just an aspect of, again, the hardware is a little bit ahead of the software, right?
[567.78 --> 569.50]  Like eventually we probably won't need the wheel.
[569.68 --> 574.26]  And eventually it'll be smart enough that I don't have to, you know, change the wiper speed.
[574.94 --> 581.58]  So the hope is that the software will eventually catch up and just make it less and less likely for you to have to touch anything.
[582.40 --> 585.34]  Yeah, if you're not the one driving, I guess it doesn't matter so much.
[585.34 --> 590.08]  So anyway, let's shift gears a little bit and get into some of the backstory behind Plex.
[590.94 --> 592.44]  It's been around a little while now.
[593.38 --> 594.98]  I forget what year it was founded.
[595.48 --> 600.34]  Like technically, I think we're coming up on the exact 10 year anniversary of the incorporation.
[601.08 --> 604.94]  But like we were around for a bit before that, before we were sort of a real company.
[605.52 --> 605.92]  Congratulations.
[606.42 --> 606.60]  Yeah.
[606.68 --> 607.02]  Thanks.
[607.24 --> 607.90]  Thanks so much.
[607.90 --> 611.88]  And I'm wondering what motivated you to create Plex in the first place?
[611.88 --> 615.58]  I mean, essentially the story is very simple.
[615.84 --> 618.90]  My wife left me alone near Christmas.
[619.26 --> 622.96]  I was bored and I was just wanted to play around with something.
[623.60 --> 626.40]  And I had, yeah, it never turns out well.
[626.94 --> 630.96]  I've been running the Xbox Media Center on a hacked Xbox.
[631.38 --> 638.46]  And we were just at that cusp where you were starting to see 720p HD video appear.
[638.46 --> 642.34]  And the Xbox was clearly struggling at this.
[642.92 --> 644.52]  And the Mac Mini was out.
[644.76 --> 648.96]  And that just seemed like an incredibly great form factor for, I mean, it was, you know,
[649.00 --> 652.22]  like a tenth of the size of one of those giant Xbox things.
[653.16 --> 655.24]  And super good horsepower.
[655.44 --> 657.14]  So it just seemed like an obvious target.
[657.56 --> 661.62]  And the Xfinity team had already been working on porting it to Linux.
[661.82 --> 665.10]  And as you know, like the underpinnings, Unix, same thing.
[665.16 --> 666.64]  I was like, how hard could this possibly be?
[666.68 --> 667.36]  Let me give it a try.
[667.36 --> 667.62]  Yeah.
[668.08 --> 669.02]  Famous last words.
[669.26 --> 669.48]  Yeah.
[669.64 --> 671.58]  It wasn't very easy.
[672.26 --> 674.32]  But that's how it all started, essentially.
[674.46 --> 677.34]  It was scratching an itch, which is probably how most projects start.
[677.96 --> 678.20]  Yeah.
[678.62 --> 682.34]  Now, I guess the 10-year marks are kind of a good opportunity to look back.
[682.92 --> 687.02]  If you had a time machine, would you go back and slip one bit of information to pass self
[687.02 --> 688.34]  to do something differently?
[688.34 --> 694.62]  I mean, there's definitely things we've done along the road that I would have done differently.
[696.76 --> 701.64]  But I don't know if there's any, if I can summarize it down to a single thing.
[701.72 --> 704.38]  Maybe like don't DDoS yourself as much.
[704.80 --> 706.84]  Do you mean your servers or yourself personally?
[706.84 --> 711.22]  Like our servers DDoSing our services.
[711.86 --> 716.08]  Because when you have millions of machines out there and you're like, okay, let's flip
[716.08 --> 716.74]  on this new thing.
[716.78 --> 718.32]  And they all start using it.
[718.56 --> 719.70]  You can melt yourself down.
[719.70 --> 725.78]  But no, I think there's definitely lots of lessons learned along the way.
[726.58 --> 732.30]  And one thing that has always been super important to me, as well as I know my co-founder and a
[732.30 --> 737.82]  lot of the other people at Plex, is we really do try to stay in contact with the community.
[738.06 --> 739.88]  Like I've just been in the forums, replying to posts.
[740.00 --> 743.14]  And I love that contact with users.
[743.14 --> 749.94]  And I think that having that contact, keeping that surface area, the surface contact area
[749.94 --> 754.46]  between yourself and your user base helps you on the right track.
[754.58 --> 757.38]  Like they will tell you very vocally when you're doing something wrong.
[757.88 --> 760.12]  And again, you might not always agree.
[760.26 --> 761.28]  And you might agree to disagree.
[761.46 --> 765.84]  You might take a slightly different turn or to quote what I think is actually not a Steve
[765.84 --> 766.54]  Jobs quote.
[766.66 --> 769.46]  Like you might give your customers what they want, not what they ask for.
[769.46 --> 777.36]  But in general, I think you ignore your customers and you lose that surface contact area with
[777.36 --> 778.78]  your customers at your own risk.
[778.94 --> 781.04]  Like that's the, I think one of the biggest lessons.
[781.94 --> 786.76]  It's a tight line because there's also the enthusiast trap where you get stuck always trying to
[786.76 --> 789.50]  serve your most vocal, most diehard fans.
[789.50 --> 791.66]  And it's harder to appeal to a wider audience.
[792.06 --> 793.38]  That is entirely true.
[793.38 --> 800.10]  And I know that I've watched Plex over the years expand into new integrations with podcasts
[800.10 --> 801.64]  and other online services.
[801.80 --> 807.12]  Have you seen pushback from the original diehard Plex community on those new services?
[807.88 --> 808.70]  How's that been?
[809.16 --> 809.64]  Absolutely.
[810.18 --> 810.82]  Yeah, absolutely.
[811.04 --> 816.34]  I mean, I think we used a joke like, you know, if we'd release an iOS update, the Android
[816.34 --> 817.04]  people will get angry.
[817.14 --> 819.80]  If we'd release an Android update, the iOS people will get angry.
[819.80 --> 825.58]  So I think Plex, one of the metaphors that we use internally to describe it is it's essentially
[825.58 --> 826.46]  a fractal, right?
[826.52 --> 830.18]  You can zoom in and maybe you're interested in Plex for music.
[830.34 --> 833.26]  So you're very zoomed into that part of our platform.
[833.44 --> 836.12]  Maybe use Plex for movies and you're very zoomed into that.
[836.58 --> 842.34]  And in a sense, like you're protective of the area that you are the most interested in,
[842.66 --> 843.74]  most vested in.
[843.94 --> 848.40]  And of course, that goes for, you know, what app you use, what streaming device you use or
[848.40 --> 849.00]  don't use.
[849.80 --> 853.92]  And I think there is also kind of just a sense of cheese being moved.
[854.08 --> 855.70]  You know, people are used to things a certain way.
[856.78 --> 862.90]  Our intent with podcasts, you know, for example, was to give people the opportunity to consume
[862.90 --> 867.64]  this content alongside their other content and maybe even relate it in a way so that,
[867.76 --> 872.84]  hey, if you like have Bob Dylan in your library, you know, like, and you have Plex everywhere,
[872.84 --> 873.60]  why not?
[873.86 --> 878.44]  Why shouldn't we say, hey, there's a really good podcast that where they're interviewing Bob
[878.44 --> 878.68]  Dylan.
[878.68 --> 882.52]  So if you like Bob Dylan, you have Bob Dylan in your library, maybe you want to check out
[882.52 --> 882.92]  this podcast.
[883.68 --> 885.62]  And we thought that would be super cool.
[886.08 --> 888.88]  And, you know, people would like that sort of integration.
[888.88 --> 893.96]  We haven't gotten along to that specifically yet.
[893.96 --> 896.16]  But that's along the lines of, you know, where we're thinking.
[896.28 --> 897.18]  You can see it with Tidal.
[898.28 --> 900.14]  There's been also pushback against Tidal.
[900.22 --> 901.06]  Some people don't like it.
[901.12 --> 906.58]  But I think the people that have music libraries that want to expand their musical horizons,
[906.58 --> 909.64]  to me, and that's, I count myself in that.
[910.30 --> 913.42]  To me, like, I think the Tidal integration is awesome.
[913.82 --> 920.78]  I have purchased more new music in the last year than I have in the previous five years
[920.78 --> 923.84]  because it's such a cool way to discover new music.
[923.84 --> 929.00]  Like, I mean, we, I know there's some detail here, but like we show you new album releases
[929.00 --> 931.66]  from artists that are in your library.
[931.66 --> 937.32]  And we let you play radios where we introduce new stuff that you haven't heard from Tidal.
[937.90 --> 940.36]  So there's all these kind of cool little integration features.
[940.60 --> 944.06]  So I think if you kind of zoom out and you're like, why is Plex doing Tidal?
[944.44 --> 945.30]  It might seem kind of weird.
[945.30 --> 948.86]  But if you are actually invested into the music ecosystem and you're a music lover,
[949.26 --> 954.36]  I think you'll find it's, there's no other solution that melds the two so seamlessly.
[954.82 --> 956.34]  I like seeing it as a podcaster.
[956.42 --> 957.78]  I like seeing those podcasts in there.
[957.78 --> 962.50]  And I noticed recently they seem to be matching more to what my movie library has.
[962.66 --> 964.42]  And I think that's a pretty clever strategy too.
[964.58 --> 968.70]  So I say as a podcaster, keep it up, but it's a bit self-serving.
[970.06 --> 973.34]  Yeah, no, I mean, you know, it's a big, it's a giant web of media, right?
[973.44 --> 976.48]  Like it's, these things are very interrelated.
[976.94 --> 978.38]  There's podcasts that relate to movies.
[978.50 --> 980.14]  There's podcasts that relate to TV shows.
[980.28 --> 983.68]  There's, there's all sorts of relationships between different types of media.
[983.68 --> 983.72]  Yeah.
[984.28 --> 988.96]  And it's nice to have fresh content without me having to do the work sometimes.
[989.84 --> 990.20]  Exactly.
[990.42 --> 993.82]  And that's, that's honestly, you know, that's, that's one of the other things that we like
[993.82 --> 999.04]  about it is, you know, the barriers to entry to Plex historically has been, hey, go get
[999.04 --> 999.48]  a server.
[1000.06 --> 1002.70]  Hey, go rip a bunch of CDs or DVDs or whatever.
[1003.22 --> 1004.04]  That's hard, right?
[1004.06 --> 1005.32]  You need a computer that's always on.
[1005.40 --> 1010.20]  It's clearly not for everyone, but with a podcast, you don't need a server.
[1010.20 --> 1014.18]  Um, so that, you know, makes it hopefully lowers the barrier to entry.
[1014.40 --> 1016.36]  So that's, uh, that's also a good thing.
[1017.18 --> 1020.98]  So I wanted to take a minute to just, uh, walk back a little bit.
[1021.34 --> 1028.00]  Um, the feedback, uh, from the, from the users, I think sometimes the subreddit in particular
[1028.00 --> 1029.16]  can be a little bit toxic.
[1030.10 --> 1034.62]  I noticed one of your posts earlier had, yeah, I've, I've turned off notifications for obvious
[1034.62 --> 1035.18]  reasons.
[1035.18 --> 1040.24]  I can only imagine how many times you get tagged a day, just on Reddit, but there was
[1040.24 --> 1041.10]  one piece of feedback.
[1041.26 --> 1047.36]  One of the users put, which I just wanted to get your, uh, response to really, which is
[1047.36 --> 1054.10]  most annoying to me is the fact that many bugs have gotten worse or have been unacknowledged.
[1054.64 --> 1059.18]  Yet Plex does nothing but introduce new features that I think the majority of users don't care
[1059.18 --> 1059.48]  about.
[1059.48 --> 1066.38]  I would rather no new features and a stable app instead of this feature, uh, waterfall.
[1067.04 --> 1071.80]  That seems pretty harsh to me having, you know, been a diehard Plex user myself for at
[1071.80 --> 1075.18]  least, I don't know, must be five plus years at this point.
[1075.64 --> 1079.46]  I've seen a few bugs and a few issues, but honestly, I don't see anything that makes me
[1079.46 --> 1080.88]  feel as strongly as this guy does.
[1081.00 --> 1086.30]  I just wanted to get your take on, on that kind of, uh, we would rather a stable app than
[1086.30 --> 1087.14]  no new features.
[1087.14 --> 1092.76]  I mean, I think generally building products, building software specifically, there's always
[1092.76 --> 1094.64]  a trade-off between new features and bugs.
[1094.98 --> 1096.28]  Software is never bug free.
[1096.70 --> 1101.26]  There's always going to be bugs and, you know, marketing and there's always a push for new
[1101.26 --> 1101.54]  features.
[1101.54 --> 1103.78]  So there's, there's always going to be a trade-off there.
[1104.42 --> 1110.22]  Um, but I think the, the trade-off that we make, we definitely, it's not like all of our
[1110.22 --> 1111.80]  engineers are working on new features.
[1111.80 --> 1115.02]  It's not like all of our engineers are working on fixing bugs.
[1115.02 --> 1121.56]  There's always a ratio of some doing new work, some doing bug work.
[1122.32 --> 1131.64]  So it's, um, it's just, it's, it's tricky because there are certainly bugs that have
[1131.64 --> 1134.78]  gone unaddressed for longer than I would personally like.
[1134.78 --> 1143.36]  There are definitely, um, you know, times when I wish we were faster at fixing bugs, but it's
[1143.36 --> 1144.58]  always the trade-off.
[1145.00 --> 1150.14]  And, um, you know, we, we definitely do try to address bugs.
[1150.32 --> 1155.42]  I think one of the things that, that the user is referencing and one of the things I've seen
[1155.42 --> 1159.20]  mentioned elsewhere is they would love it if we at least acknowledged bugs.
[1159.20 --> 1162.76]  And that's something that, again, we've tried to be better at.
[1162.90 --> 1164.16]  We try to respond in the forums.
[1164.42 --> 1169.14]  I've encouraged our engineers to, you know, spend more time in there and our support staff
[1169.14 --> 1171.08]  to say, Hey, this, we're working on this.
[1171.14 --> 1171.30]  Yep.
[1171.42 --> 1171.98]  No issue.
[1172.26 --> 1172.44]  Yep.
[1172.50 --> 1175.56]  We're working on it, but we're sort of outnumbered.
[1176.14 --> 1181.96]  And there's clearly times when we don't, um, we aren't able to acknowledge every single
[1181.96 --> 1182.28]  thing.
[1183.00 --> 1185.34]  And it's, there's a lot of balls in the air.
[1185.34 --> 1190.96]  Well, as a user, I must say, I've noticed over the last nine months or so that things
[1190.96 --> 1193.34]  have gotten significantly better on the messaging front.
[1193.86 --> 1197.84]  Um, the stability of the apps appears to have improved quite a bit.
[1198.12 --> 1202.20]  And, uh, the only thing that I've noticed that's changed quite a lot has been the UI.
[1202.64 --> 1205.70]  Uh, there's been quite a few different revisions of the UI this year.
[1205.72 --> 1209.66]  And I wondered, given you just rolled out a new version a couple of weeks ago, is this
[1209.66 --> 1211.58]  the final revision we're going to see for a while?
[1211.58 --> 1212.02]  Yeah.
[1212.24 --> 1212.76]  Yeah.
[1212.84 --> 1217.80]  I mean, that's a perfect example, I think, of, um, the feedback loop and listening to
[1217.80 --> 1223.32]  users because we were heading down, I think time flies and you're having fun.
[1223.40 --> 1230.78]  But last year we were heading up a particular direction with the UI and we got feedback on
[1230.78 --> 1230.96]  it.
[1230.96 --> 1235.88]  Um, and it, it really kind of missed the mark for what we were intending.
[1236.34 --> 1243.68]  And so we went back to the drawing board and, uh, that's when we came up with the UNO, the
[1243.68 --> 1246.16]  UI that we've termed called UNO.
[1246.80 --> 1250.70]  And the response to that has been overwhelmingly positive.
[1250.70 --> 1258.10]  And so what you've seen over the last few months is essentially just a coalescing, um, of all
[1258.10 --> 1260.10]  of our interfaces to go in that direction.
[1260.10 --> 1264.64]  Cause it seems to be one that our, our users like and appreciate the customizability of the
[1264.64 --> 1267.60]  home screen and, um, all that, all that kind of stuff.
[1267.60 --> 1270.46]  So essentially what you're seeing is just us converging on this.
[1270.58 --> 1274.30]  We feel that this UI will last us for a while.
[1274.30 --> 1275.80]  Like it's fairly scalable, right?
[1275.82 --> 1280.76]  It works in multiple different scenarios from all I want to see on my home screen is podcast
[1280.76 --> 1285.40]  entitled to, Hey, I have libraries from five different servers I want to have on my home
[1285.40 --> 1287.00]  screen and treat just as importantly.
[1287.42 --> 1290.78]  So I think it's the best UI I've ever seen rolled out from the project.
[1290.78 --> 1297.40]  And I can only imagine the, the incredible constraints that there must be in designing for
[1297.40 --> 1303.22]  all of the different types of set top TV appliance boxes from, from Apple TV down to the sticks
[1303.22 --> 1305.58]  of all different kinds and random Android devices.
[1305.78 --> 1308.18]  It must be a pretty large part of the business.
[1308.92 --> 1309.06]  Yeah.
[1309.22 --> 1317.14]  And definitely, I mean, as, as the tech guy, I really, um, like it when we can reuse code
[1317.14 --> 1318.66]  as much as possible all over the place.
[1319.16 --> 1320.48]  Um, but you're absolutely right.
[1320.50 --> 1325.98]  I mean, there, there's, there's a wide variety of, of platforms that we hit the shield is a
[1325.98 --> 1327.88]  very powerful Android platform.
[1328.04 --> 1330.06]  There are way less powerful Android platforms.
[1330.06 --> 1336.18]  There's the smart TVs that like have very, we call them potato devices sometimes just
[1336.18 --> 1338.62]  because they're, they're not super fast.
[1339.10 --> 1340.02]  That's pretty good.
[1340.66 --> 1342.94]  Do you mind if I, uh, mind if I borrow that?
[1343.00 --> 1343.70]  That's a good call.
[1344.62 --> 1345.02]  No.
[1345.12 --> 1349.18]  And in fact, just as I said it, I'm like, I wonder why potato like spud gun, like potato,
[1349.34 --> 1352.54]  I guess potatoes are slow, but no vegetables move.
[1352.64 --> 1354.14]  So I don't know why we're singling out a potato.
[1354.44 --> 1359.00]  There's always that science experiment from like a elementary school where somebody powers something
[1359.00 --> 1359.64]  with a potato.
[1359.64 --> 1360.94]  So it's like just enough power.
[1361.36 --> 1362.54]  Ah, thank you.
[1362.62 --> 1363.62]  That makes perfect sense.
[1363.70 --> 1363.88]  Now.
[1364.22 --> 1364.48]  Yeah.
[1364.62 --> 1365.46]  That's MacGyver.
[1365.66 --> 1366.50]  Yeah, exactly.
[1366.96 --> 1367.26]  Yeah.
[1367.38 --> 1372.52]  Well, I mean, I can only imagine the constraints just in shipping that software to on time to
[1372.52 --> 1373.18]  end users.
[1373.18 --> 1377.62]  We're having to go through different vendors and different app stores and all of that must
[1377.62 --> 1379.48]  be massively complex.
[1379.66 --> 1379.84]  Yeah.
[1380.34 --> 1381.16]  It's very hard.
[1381.72 --> 1381.96]  Yeah.
[1381.96 --> 1386.10]  I mean, there's definitely a, not a, not an insignificant fraction of time spent on
[1386.10 --> 1391.56]  the packaging and different release formats and processes and all of that for sure.
[1391.88 --> 1393.78]  I'm just still thinking about the 10 year mark.
[1393.78 --> 1396.32]  It's pretty significant to be joining us right around then.
[1396.88 --> 1399.86]  And, um, I'd kind of like to know about some future plans.
[1400.04 --> 1402.60]  There must be some stuff in the pipeline near term.
[1402.66 --> 1403.86]  Anything that you can share yet?
[1404.60 --> 1409.10]  One of the things that's near and dear to my own heart is the big upgrade of the music
[1409.10 --> 1409.52]  library.
[1410.42 --> 1418.16]  Um, as you may be aware of, we've been moving metadata sources, um, and we've kind of revamped
[1418.16 --> 1423.94]  and upgraded the music system and a bunch of our associated systems in the cloud.
[1423.94 --> 1425.22]  And we think it's really awesome.
[1425.22 --> 1432.80]  Um, so we continue to make, you know, huge advances in, um, the personal media space for
[1432.80 --> 1435.24]  that, um, media type.
[1435.24 --> 1439.08]  And we're also looking to do some other cool stuff with movies and TV shows that you're
[1439.08 --> 1439.82]  going to see here shortly.
[1440.56 --> 1445.28]  Um, so I think there's, there's kind of like the trinity of investments.
[1445.28 --> 1452.44]  You know, we, we definitely are, um, working on making the personal media features even
[1452.44 --> 1453.40]  more interesting.
[1454.22 --> 1462.18]  Um, and we're continue to look to make the players, the, the player space, um, for us.
[1462.18 --> 1466.58]  Like you kind of mentioned at the beginning, you said very nicely about how you can play
[1466.58 --> 1467.46]  anything anywhere.
[1467.72 --> 1471.72]  And that's kind of been our mantra for a while, but we've been investing kind of behind the
[1471.72 --> 1475.90]  scenes that it might not be completely visible, but in the actual player stacks of our platform.
[1475.90 --> 1480.80]  So Android TV, a couple of years ago, got the XO player based thing, which is an FFM peg
[1480.80 --> 1481.28]  based player.
[1481.40 --> 1485.98]  And then on Apple TV and iOS, we got the MPV based player, which again, that sounds like
[1485.98 --> 1488.26]  gobbledygook, which is probably why it's sort of hidden.
[1488.26 --> 1492.18]  But essentially we've no, our audience understands and boy, do we appreciate it.
[1492.26 --> 1492.40]  Yeah.
[1492.64 --> 1493.00]  Awesome.
[1493.08 --> 1494.06]  Well, I love your audience then.
[1494.16 --> 1494.28]  Yeah.
[1494.34 --> 1499.66]  So, I mean, that's, that's been a key for us because we, we want the media to play well.
[1499.74 --> 1501.02]  We want the media to play fast.
[1501.14 --> 1504.36]  We want it to, you know, the more you can direct play, the more energy efficient it is,
[1504.38 --> 1508.28]  the faster you can seek, the faster playback time you have.
[1508.36 --> 1515.38]  So we've, we've really been investing heavily in that core tech of player upgrades and we take
[1515.38 --> 1516.20]  it very seriously.
[1516.94 --> 1519.86]  And so that's sort of like another part, right?
[1519.92 --> 1524.76]  Because, you know, our platform playback is an incredibly huge part.
[1525.80 --> 1530.86]  And then on the third, third part is kind of where you've seen us play with podcasts and
[1530.86 --> 1535.74]  title and stuff like that, which is we happen to think that it's really cool to have access
[1535.74 --> 1540.48]  to an even larger catalog of content, some of which might not come from your own computer.
[1540.48 --> 1543.60]  Um, and we certainly don't want to force it on people.
[1543.82 --> 1549.04]  People can turn it off if they don't want it, but, um, we, we, we think it's, there's
[1549.04 --> 1554.90]  some really exciting opportunities for remixing your own content, uh, augmenting, we call it
[1554.90 --> 1555.26]  internally.
[1555.64 --> 1557.76]  Augmentation is kind of what, what the term we use.
[1558.18 --> 1561.56]  Um, and that's kind of what you're seeing with title.
[1561.60 --> 1562.82]  And I'll just give another example.
[1562.82 --> 1569.58]  Like if I go into Bob Dylan and I'm got my title account set up, if I have missing albums,
[1569.58 --> 1574.00]  if I'm missing any albums by Bob Dylan, they'll show up right alongside the albums that I own
[1574.00 --> 1575.68]  one click to play them.
[1576.34 --> 1577.98]  Um, that's pretty cool.
[1578.50 --> 1583.42]  Um, so, you know, that's, that's some of the, some of the innovation space we're playing
[1583.42 --> 1583.64]  in.
[1584.64 --> 1585.74]  Yeah, that's really nice.
[1585.74 --> 1591.24]  And it augments, you know, cloud services like Spotify quite nicely to have something
[1591.24 --> 1593.20]  like that available in high quality and everything.
[1593.58 --> 1598.24]  And I wanted to touch on the playback improvements that you talked about.
[1598.48 --> 1600.78]  This, this is a feature feature request from me.
[1600.84 --> 1601.10]  Really?
[1601.92 --> 1605.50]  Uh, I have a server that has about 10 or 12 people that use it regularly.
[1605.62 --> 1610.76]  And one thing I've noticed, I have gigabit upload here, so I'm not constrained with my
[1610.76 --> 1611.88]  pipe going out.
[1612.56 --> 1621.00]  I would love to be able to set an on the fly transcoding, um, preference, like prefer direct
[1621.00 --> 1624.74]  play over transcode or something like that instead of the current default.
[1624.98 --> 1625.60]  A server side?
[1625.78 --> 1625.94]  Yeah.
[1626.02 --> 1626.66]  Server side.
[1626.74 --> 1626.88]  Yeah.
[1627.56 --> 1628.98]  Like push it out to the clients.
[1629.40 --> 1634.70]  I mean, I, I guess, uh, wouldn't that, I mean, that would assume that your clients
[1634.70 --> 1638.68]  have the downstream bandwidth, right?
[1638.70 --> 1643.22]  Like there might be, let's say if someone has a, a five megabit download, they're not
[1643.22 --> 1646.74]  going to be able to direct play at 20 megabit.
[1646.86 --> 1647.46]  That's true.
[1647.46 --> 1650.82]  I would prefer to be able to push a direct play.
[1651.02 --> 1652.04]  I take your point though.
[1652.10 --> 1656.28]  I mean, you're trying to, um, aim at the, you know, the lowest common denominator, which
[1656.28 --> 1662.04]  is going to be probably the client's downlink bandwidth or my upload bandwidth, which I can
[1662.04 --> 1662.94]  control right now.
[1663.64 --> 1664.88]  Or heaven forbid somebody on mobile.
[1665.74 --> 1666.14]  Yeah.
[1666.34 --> 1666.64]  Yeah.
[1666.66 --> 1670.66]  I was going to say like, if someone's on an iPhone, they probably don't have 20 megabits
[1670.66 --> 1670.84]  either.
[1670.98 --> 1675.12]  I mean, you, what you've touched on there is, is some of the complexity that we were trying
[1675.12 --> 1681.00]  to, um, or that we have been trying to address with the streaming brain project that we have,
[1681.06 --> 1687.10]  where the, the server is trying to be very cognizant of all of those facts.
[1687.22 --> 1689.02]  How much upload bandwidth do I have?
[1689.16 --> 1691.36]  What's the, um, bandwidth of file?
[1691.54 --> 1693.70]  How loaded is the CPU right now?
[1694.06 --> 1698.80]  How much bandwidth is the client, you know, how fast is the client able to transfer and sort
[1698.80 --> 1700.60]  of magically making adjustments.
[1700.96 --> 1707.70]  So, you know, you'll see, um, cases where one, if you have, let's say 20 megabit upstream,
[1707.70 --> 1711.18]  you'll start with a transcode and you'll use that 15 megabits.
[1711.18 --> 1715.62]  And then when a new client comes on, like literally they would only have five megabits
[1715.62 --> 1716.04]  left.
[1716.16 --> 1719.30]  But what we do is we downshift so they can share more evenly the bandwidth.
[1719.70 --> 1724.08]  So there is a lot of magic going on behind the scenes right now to try to make it automatic.
[1724.08 --> 1728.72]  But that magic is essentially in, in the transcode, right?
[1728.78 --> 1732.20]  Cause that's where you have the volume knob essentially, you know, direct play.
[1732.30 --> 1733.94]  There's, there's no real volume knob on that.
[1734.54 --> 1739.28]  I actually am very impressed by how, how intelligent the entire backend is.
[1739.32 --> 1743.54]  So this, this kind of collection of tools is called the streaming brain.
[1743.54 --> 1744.08]  Did you say?
[1744.78 --> 1745.18]  Yeah.
[1745.22 --> 1748.34]  I'm not exactly sure why we decided to call it that, but that just was kind of what we
[1748.34 --> 1750.10]  ended up calling it internally, the streaming brain.
[1750.10 --> 1757.26]  And amusing side note, um, when we have meetings around it, there was one guy who, um, one of
[1757.26 --> 1762.04]  our project manager guys who loved to use emoji and he was trying to come up with emoji representation
[1762.04 --> 1762.92]  of streaming brain.
[1763.02 --> 1769.18]  And the best thing he could do is while streaming, he used the shower emoji and then brain, he
[1769.18 --> 1769.96]  used the robot.
[1770.10 --> 1771.82]  So it was like robot in a shower.
[1771.96 --> 1775.90]  And if you go to our online store, I think we actually sell a t-shirt.
[1776.04 --> 1778.06]  That's a robot taking a shower.
[1778.06 --> 1778.50]  Yeah.
[1778.96 --> 1784.16]  It's like the robot from, um, Oh, what was that old sci-fi movie with a hitchhiker's
[1784.16 --> 1784.38]  guide?
[1784.72 --> 1785.00]  No, no.
[1785.08 --> 1786.12]  The one with Leslie Nielsen in it.
[1786.18 --> 1788.12]  The, uh, Oh, it's such a, it's a classic.
[1788.22 --> 1789.38]  I can't believe I'm blanking on it.
[1789.42 --> 1791.82]  It's even when it's, it's in my Plex library.
[1792.00 --> 1795.36]  So I really, I really should know forbidden planet.
[1795.70 --> 1796.06]  Yes.
[1796.30 --> 1797.00]  Ah, yes.
[1797.16 --> 1799.70]  I'll put a link to the blog post that has a picture of it.
[1799.72 --> 1800.30]  It's so good.
[1800.42 --> 1801.42]  We'll have that in the show notes.
[1801.84 --> 1802.06]  Yeah.
[1802.16 --> 1803.54]  That's our illustrator, Craig.
[1803.54 --> 1806.56]  He is a brilliant, super talented guy.
[1806.96 --> 1809.24]  And, uh, yeah, you'll see a lot of his work on our t-shirts.
[1809.60 --> 1810.26]  That's awesome.
[1810.48 --> 1812.96]  We always joke about pivoting to, you know, clothing.
[1814.54 --> 1819.28]  You know, I'm saying if it all looked like that, that actually would be a, probably a lucrative
[1819.28 --> 1821.36]  side business, a little Plex side hustle.
[1821.64 --> 1822.98]  Move over threadless.
[1823.38 --> 1823.66]  Yeah.
[1823.66 --> 1827.02]  I thoroughly enjoyed that.
[1827.12 --> 1830.96]  And I hope we get an opportunity to chat with him in the future and just sort of check in
[1830.96 --> 1831.42]  on things.
[1831.42 --> 1834.42]  But you did promise we'd talk about ghost.
[1834.66 --> 1839.90]  Ghost is a blogging platform that has exploded over the last few years.
[1840.04 --> 1844.46]  Last week, 4,286 new sites were made with ghosts.
[1844.86 --> 1846.06]  And that's just last week.
[1846.16 --> 1847.70]  And they have a brand new release.
[1848.12 --> 1849.12]  I ain't afraid of no ghost.
[1849.80 --> 1851.24]  Oh, I can't believe you.
[1851.24 --> 1853.84]  I suppose it had to be done.
[1854.26 --> 1855.74]  It's one week away from Halloween.
[1855.88 --> 1857.22]  You've got to embrace my new country.
[1857.60 --> 1858.08]  That's right.
[1858.20 --> 1858.80]  Good for you.
[1859.34 --> 1859.48]  Yeah.
[1859.52 --> 1859.72]  Okay.
[1859.80 --> 1860.22]  Fair enough.
[1860.30 --> 1863.50]  We are talking about ghost near Halloween and somebody had to put it in there.
[1863.60 --> 1863.76]  Yeah.
[1863.88 --> 1865.30]  So you're a big fan though.
[1865.70 --> 1871.84]  I have daydreamed about using ghost, but never had enough reason to move off of WordPress.
[1872.38 --> 1875.42]  Another favorite of, you know, the open source community.
[1875.84 --> 1876.88]  But you, you did.
[1876.98 --> 1878.72]  You just says, nah, no WordPress for me.
[1878.72 --> 1883.66]  Well, it was when Linux server was in the early days and I was doing a lot of blogging over there.
[1884.02 --> 1899.08]  And it's just, I don't know, like WordPress is fine, but I always felt like it was an extremely big, heavyweight application for what I wanted to achieve, which was just write some text with a couple of images and a couple of categories and tags and that kind of thing.
[1899.08 --> 1900.56]  I don't need any of the CMS.
[1901.00 --> 1902.96]  I don't need any of the e-commerce type stuff.
[1903.84 --> 1905.78]  And ghost fitted that bill really, really well.
[1906.00 --> 1909.32]  It had a beautiful typography because fonts do matter.
[1910.68 --> 1914.38]  And the, uh, the writer's interface as well is super clean.
[1914.92 --> 1916.96]  So what do you consider notable about the new, what is it?
[1917.02 --> 1918.62]  3.0 release they just announced?
[1918.88 --> 1919.60]  There's a few things.
[1919.60 --> 1932.44]  So firstly is they are looking to give creators a way to receive money without relying on a third party middleman like Patreon or something like that.
[1932.84 --> 1937.86]  And what's particularly interesting about this is it doesn't require the ghost company to remain in business either.
[1937.86 --> 1944.16]  So there is a direct way for readers of a blog to contribute to the writer of a blog, which is really nice.
[1945.34 --> 1947.16]  The payments all go through Stripe.
[1947.30 --> 1951.24]  So, so long as Stripe stay in business, then this mechanism will continue to work just fine.
[1952.10 --> 1956.68]  There's another new feature in the release, which changes the way in which the sites are generated.
[1956.68 --> 1964.38]  And there's a lot more support now for static site generation frameworks for things like Gatsby, Next.js, et cetera, et cetera.
[1964.44 --> 1967.00]  There's dozens of, dozens of changes there around that stuff.
[1967.00 --> 1976.34]  And if you want proof of the pudding, the entire ghost.org website is actually a Gatsby.js app hosted on top of Ghost.
[1976.84 --> 1982.68]  The other change that I'm super excited about is the way in which themes used to be developed.
[1982.98 --> 1989.74]  So before this release, you had to upload themes as a zip file, apply the change, and then pray that it worked.
[1990.14 --> 1996.44]  Well, now with a combination of the Jamstack work that they have, you can actually combine that with GitHub Actions
[1996.44 --> 2001.50]  and then sync custom ghost themes to your live production site with each commit you make to Git.
[2001.80 --> 2003.70]  All right, I might give that a go in the future.
[2003.90 --> 2004.84]  You've tempted me, Alex.
[2005.12 --> 2008.92]  And so if you do, it's really easy to get started with a Docker Compose file.
[2008.92 --> 2020.24]  You can then couple that with an Nginx image from the Linux server guys and have a Let's Encrypt TLS HTTPS encrypted website.
[2020.24 --> 2025.68]  We'll put a link to a sample Docker Compose and Nginx config file in the show notes for you.
[2026.10 --> 2026.96]  Oh, you're a gentleman.
[2027.48 --> 2030.26]  Well, just a quick project off-grid update from me.
[2030.30 --> 2031.22]  I've ordered my cameras.
[2031.34 --> 2033.14]  I'll reveal which cameras here in the near future.
[2033.64 --> 2037.64]  And I can tell you and I are going to need to have a storage chat soon.
[2038.16 --> 2039.32]  We've got to talk some storage.
[2039.48 --> 2041.14]  I've got to sort my storage out.
[2041.30 --> 2043.14]  That sends shivers down my spine, Christopher.
[2043.14 --> 2046.22]  I love talking about storage, Alex.
[2047.38 --> 2054.54]  Head over to selfhosted.show to send us your feedback, comments, any other stuff that you think we should know about in this space.
[2054.90 --> 2059.94]  How I could do storage for multiple Raspberry Pis in a tiny network with low power requirements.
[2060.04 --> 2060.68]  I'd love to know that.
[2060.76 --> 2061.92]  Selfhosted.show slash contact.
[2062.44 --> 2065.26]  I am at Chris LAS on the Twitter.
[2065.36 --> 2066.52]  He's at Ironic Badger.
[2066.72 --> 2067.32]  Thanks for listening.
[2067.32 --> 2070.12]  That was selfhosted.show slash four.
[2073.14 --> 2103.12]  I am at Chris LAS on the Twitter.
