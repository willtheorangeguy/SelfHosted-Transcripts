[0.00 --> 8.42]  Since our last episode, I have been just every single night building something new, trying something new for my home server setup.
[8.42 --> 12.52]  I feel like I've really rebounded from the death of my Raspberry Pi.
[13.08 --> 15.76]  And now I'm just like trying out different setups.
[15.92 --> 21.16]  I'm really just going out, having fun, living life, experiencing different things.
[21.30 --> 24.78]  I'm not getting committed to any serious configurations or setups.
[24.98 --> 29.10]  I'm just dabbling and experimenting and really enjoying myself.
[29.10 --> 32.38]  But sowing your seed in the field of Linux, I take it.
[33.26 --> 33.66]  Absolutely.
[34.06 --> 36.54]  And things were just going really great.
[38.22 --> 39.22]  Until last night.
[39.50 --> 40.06]  Uh-oh.
[40.36 --> 41.22]  But we'll get to that.
[41.28 --> 42.14]  We'll get to that in the show.
[42.22 --> 45.44]  There's so much to get into today that I want to save it for a little bit.
[45.56 --> 47.58]  Because I know you've been at an event recently.
[48.08 --> 56.14]  We also have been thinking about doing a little shout out to the community, trying to get somebody who might be a Discord bot wizard to help us come up with a title bot for the show.
[56.52 --> 57.98]  So there's a lot to cover today.
[57.98 --> 61.92]  Plus, towards the end of the show, we've got some great feedback, some good questions.
[62.14 --> 63.94]  I've got some new hardware updates.
[64.70 --> 66.10]  So I'll tell you about it later, okay?
[66.66 --> 68.02]  Oh, it's such a tease.
[68.32 --> 71.08]  I think I'll stick around and see what's been happening.
[71.26 --> 72.54]  Stay tuned and find out, Alex.
[73.20 --> 73.60]  Exactly.
[73.60 --> 76.94]  Well, very quickly, let's just cover the title bot first, shall we?
[77.62 --> 78.82]  Very simple requirements.
[78.94 --> 83.88]  We want something that you type, you know, bang, you know, exclamation mark, start show.
[84.22 --> 85.90]  And that starts the timer running.
[85.90 --> 94.24]  And then ideally publishes any bang suggest titles to a little web page, which we can rank by the number of votes.
[94.58 --> 95.44]  Yeah, an upvote or something.
[96.44 --> 99.64]  If you've been with JB for a while, you remember jbtitles.com.
[99.92 --> 106.92]  Something like that that we used to have in IRC, but for the modern age in Discord would be bang tidy.
[106.92 --> 111.96]  Yeah, because we've been live streaming now for weeks over at jupyter.tube every other Wednesday.
[112.34 --> 113.66]  And we put our Discord up there.
[114.28 --> 116.62]  We've got a live chat room in our Discord.
[117.58 --> 123.70]  And the thing is, we've been podcasting for so long, our title-making happeners are broken.
[124.20 --> 125.92]  And we just cannot title these things.
[125.96 --> 127.30]  So we need to crowdsource that.
[127.66 --> 130.04]  And it gives people a chance to participate live and come up with a title.
[130.14 --> 131.98]  If you want to help us build a bot, reach out and let us know.
[132.16 --> 136.24]  Yeah, if it was up to me, every episode would be called Linux and stuff.
[136.92 --> 140.24]  We can do our buddy Joe's approach and just drop titles altogether.
[140.74 --> 142.64]  He convinced me to do that with Linux Action News.
[143.14 --> 143.80]  Best thing ever.
[144.18 --> 147.00]  Yeah, well, news is kind of, yeah, it's different.
[147.64 --> 148.22]  Yeah, yeah, yeah.
[148.60 --> 149.88]  All right, so I'm a little jelly.
[150.30 --> 152.04]  You've been at all things open today.
[152.28 --> 154.42]  I have, right on my doorstep.
[154.60 --> 160.04]  A great big open source, 4,000, 5,000 person open source conference right on my doorstep.
[160.58 --> 162.10]  4,000 to 5,000?
[162.44 --> 163.74]  Yeah, that's what I've been told, yeah.
[163.74 --> 163.78]  Yeah.
[164.32 --> 167.38]  I kind of almost feel like maybe this is the new Linux Fest.
[167.88 --> 168.40]  Am I right?
[168.54 --> 169.60]  Is it worth going to?
[169.68 --> 170.74]  Should I travel to this?
[170.82 --> 171.40]  Give me your take.
[171.62 --> 174.38]  Well, it's a sort of semi-commercial conference.
[174.68 --> 176.50]  It's in a bit of a weird spot, if you ask me.
[176.58 --> 182.28]  It's not like Linux Fest Northwest, which is completely hippie and free open source love
[182.28 --> 182.58]  fest.
[182.58 --> 187.88]  And it's not something like KubeCon, which is just almost entirely sales pitches.
[188.10 --> 194.32]  It seems to be to be somewhere in the middle, like it's mostly commercial sponsored stuff.
[194.54 --> 197.22]  And there's a handful of talks given by real people.
[197.60 --> 202.14]  And the rest are given by employees of companies who would like you to go and use their service
[202.14 --> 205.24]  mesh implementation, for example, or whatever it might be.
[205.24 --> 208.94]  But on the whole, the quality of the sessions was okay.
[209.56 --> 215.18]  I think probably about half of the sessions I went to were good, and the other half were
[215.18 --> 216.46]  really not good.
[216.96 --> 218.30]  What made them really not good?
[218.80 --> 219.84]  Were they sales pitches?
[220.60 --> 222.00]  Yeah, a mixture of stuff like that.
[222.20 --> 229.94]  Like it was clearly just, I mean, a 45-minute long infomercial, or the presenter was an intern
[229.94 --> 234.90]  and had never spoken to an audience before, or, you know, those kinds of things, really.
[235.38 --> 238.86]  So maybe the bar was a little low on who was accepted to speak?
[239.58 --> 239.86]  Yeah.
[240.00 --> 243.82]  Well, I mean, the reason I was interested in going was because Jim Salter was down to talk
[243.82 --> 248.48]  about ZFS, and who doesn't want to go and listen to Jim say how bad every other fire
[248.48 --> 250.42]  system in the world except ZFS is, right?
[251.32 --> 254.22]  Poor guy wasn't feeling terribly well, though, so he pulled out at the last minute.
[254.64 --> 257.58]  And we were left hanging, unfortunately.
[257.74 --> 259.60]  No Jim Salter ZFS love fest.
[259.60 --> 262.10]  You got to get your updated ZFS talking points.
[262.20 --> 262.80]  What are you going to do?
[263.20 --> 263.94]  Yeah, I know.
[264.18 --> 266.80]  Well, what I could do instead is talk about WSL2.
[267.38 --> 272.42]  Scott Hanselman, who is a Microsoft employee, I have to say was probably the best presenter
[272.42 --> 273.36]  that was at the conference.
[273.72 --> 280.80]  And he just had this wonderful way with him where he was funny and actually engaging and
[280.80 --> 284.22]  obviously clearly knew the subject he was talking about extremely well.
[284.22 --> 292.42]  And he did a very slick demo of how WSL2 and GitHub and VS Code and Windows are actually
[292.42 --> 295.78]  the perfect developer platform these days.
[296.72 --> 297.90]  And who would have thought?
[297.98 --> 306.12]  Who had on their bingo card 10 years ago, Microsoft would nail the developer experience on Linux,
[306.36 --> 309.72]  on Windows, and just make it all work seamlessly together?
[309.72 --> 311.66]  I mean, mind blown.
[312.22 --> 314.86]  Well, yes and no.
[315.18 --> 320.46]  I mean, they have, I think actually to give credit where credit is due, I think Microsoft's
[320.46 --> 327.88]  pivot to focus on Linux open source and I would say broader development tools and development
[327.88 --> 329.92]  platforms, which I think is really what they've done.
[329.92 --> 332.86]  That has been very impressive.
[333.48 --> 334.78]  They deserve all the credit.
[334.96 --> 342.40]  You very rarely see these empires, these massive corporations make these huge pivots.
[343.02 --> 349.18]  A lot of times companies just get locked into a way of doing business and they just only
[349.18 --> 352.70]  have tunnel vision and they fight everything else to try to protect that business model.
[353.54 --> 358.42]  Microsoft figured out that they had to sacrifice a little bit of Windows and adopt and embrace
[358.42 --> 361.08]  a little bit more Linux open source and things like that.
[361.18 --> 364.76]  To that end, I give them total and absolute compliments.
[364.88 --> 368.38]  I think they've done very well and I think it's legitimate in a lot of ways.
[369.04 --> 372.86]  But I think the Achilles heel to this dream fantasy that they're saying where you can have
[372.86 --> 376.98]  Windows with your compatibility and your corporate integration and you have WSL and you're just
[376.98 --> 380.76]  using GitHub and VS Code and everything's great because Edge is based on Chrome.
[380.88 --> 381.72]  So let's have fun.
[381.72 --> 385.88]  The problem is it's still Windows.
[386.22 --> 387.72]  It's still got the registry.
[387.96 --> 389.66]  It's still using NTFS.
[389.84 --> 395.14]  It still has an onion layered approach to the control panel and all the legacy stuff that comes
[395.14 --> 395.50]  in there.
[395.60 --> 398.68]  It still does all of the things that Windows does.
[398.80 --> 405.62]  It's still absolutely subject to the corporate tax strategy of Microsoft and whatever thing
[405.62 --> 408.28]  they're pursuing for that particular release cycle.
[408.28 --> 411.18]  Windows is absolutely still influenced by it.
[411.28 --> 415.16]  And as a user, you have to put up with it and wait for the next fad so they can swap it
[415.16 --> 416.36]  out and put the other thing in there.
[416.66 --> 417.72]  I mean, like right now, right?
[417.74 --> 422.52]  They're bundling in Teams or the bundle in Cortana or they'll put ads in the start menu.
[422.52 --> 427.08]  It just doesn't matter because they're always doing something else because one of the fiefdoms
[427.08 --> 431.52]  and Microsoft has finally gotten their chance, their moment, and they're going to get the
[431.52 --> 433.24]  numbers and they get something built into Windows.
[433.34 --> 439.02]  And you will always, always have to put up with that corporate strategy tax with a Windows
[439.02 --> 439.66]  workstation.
[440.14 --> 443.84]  And despite what they say, the driver model on Windows still blows.
[444.02 --> 446.78]  The printing subsystem on Windows still blows.
[446.96 --> 450.00]  The disk IO subsystem on Windows still blows.
[450.00 --> 455.88]  The Windows UI is still bloated, old, and has lots of legacy if you go just one layer below
[455.88 --> 456.96]  their new lacquer.
[457.58 --> 462.20]  And so, yeah, you can run a Linux kernel in a really great hyper-virtualized environment.
[462.32 --> 462.94]  Good for you.
[463.26 --> 464.72]  And VS Code's a pretty good product.
[465.08 --> 466.66]  But I could run VS Code on Linux.
[467.00 --> 471.82]  I could have a real Linux subsystem with a real Linux kernel that has real file systems
[471.82 --> 474.40]  and doesn't have all that Windows legacy bullcrap.
[474.90 --> 476.16]  And so it's close.
[476.52 --> 478.28]  Yeah, but your audio wouldn't work though.
[478.28 --> 479.14]  Yeah, yeah, right.
[479.54 --> 480.32]  I mean, you're right.
[480.44 --> 484.70]  And there are, absolutely, there are situations where, like, Linux doesn't cut it.
[485.08 --> 486.24]  And I acknowledge that.
[486.78 --> 490.16]  And that's why I think it is really great that WSL is as good as it is.
[490.70 --> 492.62]  Because there are people that just have no choice, too.
[493.34 --> 494.52]  And they have to use Windows.
[494.94 --> 496.44]  And for them, the subsystem's there.
[496.74 --> 500.42]  Well, if I want to run Flight Sim, there is no other way for me to run Flight Sim than
[500.42 --> 500.92]  to run Windows.
[501.10 --> 504.86]  Yeah, and there's, you know, like, I can't remember the name of it, but there's some game
[504.86 --> 506.06]  that my son Dylan loves.
[506.06 --> 510.18]  And so he's, you know, he's snuck in a dual boot into Windows now.
[510.44 --> 511.90]  So that way he can play that one game.
[511.94 --> 512.82]  And it kills me.
[513.00 --> 517.42]  But I have to acknowledge, like, if you want to run that application, you got to have Windows.
[517.50 --> 518.88]  So it absolutely has its place.
[519.18 --> 524.66]  But this utopia that they're painting for developers, you know, I just can't, I can't,
[524.66 --> 525.60]  I can't subscribe to it.
[525.60 --> 527.46]  I can't say as I disagree with anything you said.
[527.88 --> 535.36]  But they have solved an absolutely huge problem, which is encapsulated development environment.
[535.68 --> 540.66]  So Scott, in his talk, showed us something called development containers.
[541.20 --> 545.92]  And these essentially are a JSON manifest of all the requirements you need to develop a
[545.92 --> 546.88]  specific project.
[546.88 --> 555.36]  In his example, it was an oh my posh PowerShell kind of candy looking terminal pretty fire thing.
[556.56 --> 559.72]  And he downloaded the, he cloned the Git repo.
[560.28 --> 564.46]  VS Code automatically picked up the JSON file that was stored in the correct folder.
[564.46 --> 569.68]  It pre-installed all the dependencies in a container, a Docker container on Windows running in the
[569.68 --> 572.86]  Linux subsystem for Windows or whatever the hell it's called.
[573.90 --> 578.50]  And within, you know, a minute of cloning this repo, he was working.
[578.78 --> 581.32]  Well, hypothetically, presentation working.
[581.60 --> 581.96]  You know what I mean?
[582.20 --> 583.52]  That does sound really slick.
[583.88 --> 584.30]  I got it, mate.
[584.38 --> 585.40]  I mean, that does sound slick.
[585.56 --> 589.56]  I mean, a good part of my master's degree sort of five, six, seven years ago was trying
[589.56 --> 592.40]  to solve this encapsulated development environment thing.
[592.40 --> 595.18]  And that was what led me to Docker containers back then.
[595.40 --> 600.78]  And, you know, we were looking at Packer VMs and, you know, sending QCow2 images around
[600.78 --> 606.76]  to people and having like a special university version of Linux just for this computer science
[606.76 --> 607.18]  course.
[607.38 --> 610.38]  And God damn it, Microsoft went and figured it out.
[610.98 --> 611.42]  Microsoft.
[612.00 --> 612.82]  It's crazy.
[613.02 --> 613.32]  They did.
[614.22 --> 615.32]  It's pretty legit.
[615.48 --> 619.00]  And I have to say, too, like they recognize they needed a better terminal.
[619.26 --> 620.26]  They absolutely did.
[620.30 --> 621.46]  They created the Windows terminal.
[621.46 --> 622.88]  They made it an open source project.
[623.00 --> 626.74]  And it seems like it's a pretty good terminal, like direct text accelerated terminal.
[626.98 --> 628.38]  I mean, it's crazy.
[628.76 --> 628.92]  Yeah.
[629.78 --> 630.68]  So funny.
[630.96 --> 632.42]  It really it truly is.
[632.46 --> 636.62]  It's I have to mention that this is something my buddy Michael Dominick and I have been talking
[636.62 --> 640.00]  about for a while on Coder Radio because we often talk about the tooling for development
[640.00 --> 640.70]  workstations.
[640.70 --> 643.30]  And he's kind of been through this whole journey.
[643.92 --> 645.56]  Mac to Windows.
[645.56 --> 650.48]  WSL and like the Mecca that that opened up for him.
[650.48 --> 655.34]  And also, of course, VS Code and also integration with Azure and just like he went all in for
[655.34 --> 655.64]  a bit.
[655.84 --> 659.66]  And now he's actually back on Linux as his primary development workstation.
[659.78 --> 664.76]  And so the whole journey, I think, has been really interesting at Coder.show if you are
[664.76 --> 665.24]  interested.
[665.74 --> 667.24]  But I want to hear about the meetup.
[667.34 --> 670.20]  I know you had a chance to go say hi to some audience members.
[670.66 --> 672.54]  You guys coordinated in the Matrix chat.
[672.78 --> 673.88]  It sounded like it went pretty well.
[674.60 --> 674.92]  Absolutely.
[675.16 --> 675.32]  Yeah.
[675.36 --> 680.66]  Well, I bumped into a couple of listeners throughout the day who somehow recognized me from my
[680.66 --> 683.80]  voice like it's distinctive in a room full of Americans for some reason.
[683.88 --> 684.20]  Who knows?
[685.88 --> 689.52]  So we've got a little clip from a couple of listeners that we met up with for lunch.
[689.90 --> 692.60]  So I'm here at All Things Open with Reid and John.
[692.66 --> 694.28]  How are you liking the conference so far, John?
[694.64 --> 695.60]  It's been pretty good.
[695.82 --> 696.70]  Learned a lot.
[696.70 --> 704.24]  Been to a bunch of different sessions and gotten to meet some cool people and meet up
[704.24 --> 706.40]  with the JB crowd here.
[707.06 --> 707.22]  Yeah.
[707.34 --> 713.04]  And we use the element to JB Matrix to kind of have a little mini meetup in the lobby of
[713.04 --> 713.96]  the conference, didn't we?
[714.52 --> 716.20]  And Reid, I know you've been listening for a little while.
[716.26 --> 717.60]  How are you liking the conference as well?
[718.08 --> 718.70]  Oh, it's great.
[718.70 --> 718.96]  Yeah.
[718.96 --> 729.80]  A very wide range of people here from community to corporate and lots to learn, lots to see
[729.80 --> 730.98]  and lots of great people to meet.
[731.44 --> 733.78]  Any standout sessions for either of you?
[734.74 --> 743.90]  There was a beer brewing with IoT and JavaScript that I knew almost nothing about any of those
[743.90 --> 744.22]  subjects.
[744.22 --> 746.86]  And now I know a little bit about all of those subjects.
[747.30 --> 749.72]  You're at the Dunning-Kruger effect style moment, right?
[749.74 --> 751.58]  Where you don't realize how little you actually know.
[751.92 --> 753.24]  You feel vaguely competent.
[753.56 --> 754.00]  Completely.
[754.20 --> 754.92]  How about you, John?
[755.42 --> 759.82]  There was a great, it was half of a two for one that was on burnout.
[760.14 --> 767.14]  And it was a really good just kind of think about not burning out and ways to kind of handle
[767.14 --> 769.58]  that stress and take breaks and things like that.
[769.58 --> 770.78]  Yeah, very good.
[771.16 --> 776.22]  I've certainly been, I've certainly found burnout myself at times can be quite challenging
[776.22 --> 778.72]  to deal with, particularly during the last couple of years.
[778.88 --> 780.02]  So it's very good.
[780.10 --> 781.82]  Well, I wish you all the best for the rest of the afternoon.
[781.96 --> 783.34]  I hope you enjoy the rest of the conference.
[783.82 --> 784.18]  Thank you.
[785.46 --> 789.86]  I do hear what you're saying in there, though, that it's a pretty wide range that All Things
[789.86 --> 790.76]  Open is trying to cover.
[791.04 --> 794.18]  Although I like the idea about having sessions on burnout.
[794.18 --> 800.68]  And who doesn't like a session about automating beer brewing with Linux and open source technologies,
[800.82 --> 800.92]  huh?
[801.50 --> 806.72]  So the nice thing was, you know, the Raleigh downtown is a pretty small little place if
[806.72 --> 807.34]  you've never been.
[807.96 --> 813.48]  And Red Hat Tower, as we call it, The Tower, is only two blocks from the convention center,
[814.02 --> 815.28]  a short five minute walk.
[815.34 --> 820.34]  So I was able to meet up with these listeners, Reed and John, and take them to lunch at The
[820.34 --> 823.44]  Tower today, which as we record is Wednesday.
[824.18 --> 824.66]  Oh, good.
[824.68 --> 826.58]  Did you get more sauce while you were there?
[827.30 --> 830.24]  Alex likes to pick up a little extra sauce while he's at the Red Hat Tower.
[830.96 --> 836.16]  So I think what Chris is referring to there is Boar's Head, you know, the sandwich company.
[836.28 --> 838.26]  You think, you know what I'm referring to.
[838.36 --> 844.50]  Make this absolutely delicious gourmet, spicy mayonnaise, chipotle mayonnaise style thing.
[844.92 --> 845.52]  No, it's great.
[845.70 --> 848.96]  And I cannot get enough of it on turkey and provolone sandwiches when I'm at home during
[848.96 --> 849.32]  the day.
[849.92 --> 853.74]  So what I used to do at The Tower before COVID was anytime I went in The Tower, I used to go
[853.74 --> 858.26]  in and buy a bottle of this sauce off the vendor for, I don't know, like 10 bucks.
[858.72 --> 865.74]  Like, to put it in context, a tiny little tub of this stuff from the supermarket is five bucks.
[866.10 --> 871.62]  But a commercial catering size bottle of this sauce he gave me for 10 bucks a time.
[872.02 --> 876.06]  So I used to just slather this stuff on, whereas now I have to treat it like gold dust because
[876.06 --> 878.00]  we've got different vendors now after COVID.
[879.44 --> 880.20]  That's a bummer.
[880.20 --> 880.52]  Okay.
[880.66 --> 880.98]  All right.
[881.38 --> 882.32]  So lunch at The Tower.
[882.42 --> 883.26]  That's awfully nice.
[883.74 --> 884.54]  That sounds great.
[884.64 --> 885.12]  Yeah, we're nice.
[885.36 --> 887.40]  We also met up with Jay from LearnNixTV.
[887.92 --> 889.94]  Not going to mess up the creative process.
[890.90 --> 893.00]  I'm here with Jay from LearnNixTV.
[893.24 --> 893.68]  Hello, Jay.
[893.72 --> 894.16]  How are you?
[894.34 --> 894.72]  Doing well.
[894.76 --> 895.16]  How are you?
[895.62 --> 895.84]  Yeah.
[895.86 --> 902.26]  I went to your talk yesterday on RetroPie and how you're saving retro gaming from Oblivion.
[903.08 --> 903.32]  Yeah.
[903.46 --> 909.50]  So basically my setup is such that sync thing syncs all of my RetroPies together.
[909.50 --> 914.42]  So if I'm on my handheld RetroPie or the one on the TV, I could play a game, save the game,
[914.76 --> 917.00]  then go to the couch and it's the same save file.
[917.12 --> 918.88]  The ROMs and everything all sync to each other.
[919.10 --> 922.60]  So it's just like this thing where my save files just follow me around.
[922.70 --> 926.68]  It's just one of the amazing things that you could do with technology that you might not
[926.68 --> 928.10]  think about right off the top of your head.
[928.10 --> 930.78]  But if you put your mind to it, a little bit of creativity, you'd be surprised what you
[930.78 --> 931.50]  could come up with.
[932.12 --> 934.26]  Turns out if you try hard enough, you can, huh?
[934.50 --> 934.68]  Yeah.
[934.74 --> 939.38]  You're one of the few people on planet Earth that's got their hands on the CM4 module, right?
[939.60 --> 940.62]  How's that working out for you?
[940.62 --> 941.40]  What are you using that for?
[942.18 --> 943.94]  So actually I have a Turing Pi.
[944.10 --> 945.56]  So I have four of those in there.
[945.66 --> 948.02]  And then I have one in the handheld RetroPie.
[948.18 --> 950.62]  So it's actually working out really well.
[950.74 --> 954.60]  And the one that I have in the RetroPie, if it wasn't for Jeff Geerling, I wouldn't have
[954.60 --> 957.88]  it because he actually messaged me on Twitter like, hey, they have inventory
[957.88 --> 958.44]  over here.
[958.60 --> 960.42]  So if it wasn't for him, I wouldn't have it.
[960.44 --> 962.66]  I actually got the first ones before they got hard to find.
[962.72 --> 964.96]  And then later on, like right now, what are they going for?
[965.04 --> 966.14]  Like some crazy amount of money?
[967.20 --> 972.80]  I dread to think I haven't looked, but it's more than double, I think, MSRP.
[973.46 --> 974.18]  It's ridiculous.
[974.42 --> 978.14]  Like, especially the people that just want to have fun, set up something in their home
[978.14 --> 978.40]  lab.
[978.48 --> 982.40]  They have to navigate scalpers and everything just to work on the fun projects that they
[982.40 --> 982.96]  want to work on.
[982.96 --> 983.76]  I think that's terrible.
[983.76 --> 985.34]  Like, we just want to have fun with our technology.
[985.34 --> 987.32]  So how are you finding all things open?
[987.40 --> 988.18]  Is this your first one?
[989.14 --> 989.96]  Very first one.
[990.10 --> 991.56]  So it is very fun.
[991.76 --> 993.36]  We have a lot of cool people here.
[994.00 --> 995.28]  System 76 is here.
[995.52 --> 998.86]  Red Hat, Alma Linux, like a bunch of open source projects.
[999.02 --> 1001.18]  There's GitLab, Moodle, like countless others.
[1001.30 --> 1005.22]  It's just so much fun to, you know, just network with people, especially you.
[1005.30 --> 1008.24]  I haven't met you in person until this time, you know, until this event too.
[1008.36 --> 1009.90]  So I'm meeting really cool people.
[1009.90 --> 1011.68]  And I wouldn't trade it for anything.
[1012.36 --> 1014.54]  Yeah, there's something special about an open source conference, is there?
[1014.60 --> 1015.82]  Well, thank you very much, Jay.
[1015.98 --> 1017.24]  And enjoy the rest of your conference.
[1017.90 --> 1019.46]  I agree with Jay.
[1020.12 --> 1021.48]  Sync thing for the win.
[1021.86 --> 1022.26]  Absolutely.
[1022.54 --> 1025.90]  One of the MVPs of the last few years for me has been sync thing.
[1026.32 --> 1030.04]  Just my background ambient file system sync.
[1030.46 --> 1031.54]  I have Dropbox.
[1031.62 --> 1032.46]  You know, I have Nextcloud.
[1032.54 --> 1033.60]  I've tried these different things.
[1033.60 --> 1037.82]  I think of that as active, persistent syncing.
[1038.16 --> 1038.96]  You see it.
[1039.04 --> 1039.86]  It's got a status.
[1040.10 --> 1040.90]  You know it's happening.
[1041.52 --> 1042.86]  You can bring up the app.
[1042.94 --> 1043.84]  You can look at what's synced.
[1044.36 --> 1045.60]  I kind of look at sync thing.
[1045.66 --> 1047.48]  You can do all those things with sync thing.
[1047.60 --> 1049.48]  There's even system tray icons you can get.
[1049.54 --> 1054.04]  But I kind of think of sync thing as like this ambient background sync that's actually
[1054.04 --> 1055.60]  syncing file systems around.
[1056.32 --> 1059.40]  And it doesn't care where you store something.
[1059.48 --> 1063.00]  It doesn't have to be like in a particular directory like Nextcloud or Dropbox does.
[1063.00 --> 1066.08]  It can be anything, anywhere on your file system.
[1066.42 --> 1066.84]  It's pretty cool.
[1066.92 --> 1073.74]  And Jay was using it to sync his Steam Deck emulator progress with his RetroPie TV emulator
[1073.74 --> 1075.00]  progress.
[1075.22 --> 1078.80]  So that no matter where he was, his retro games were in sync, which is pretty cool.
[1079.32 --> 1079.96]  That's a great idea.
[1080.72 --> 1085.38]  That's a great idea because, you know, you don't want to lose progress when you move between
[1085.38 --> 1085.90]  devices.
[1086.24 --> 1088.54]  So maybe next year I'll see you at All Things Open.
[1088.54 --> 1093.80]  And in the meantime, keep an eye on the Meetup page at meetup.com slash Jupyter Broadcasting.
[1095.96 --> 1098.20]  Linode.com slash SSH.
[1098.26 --> 1101.40]  That's where you go to get $100 on a new account and support the show.
[1101.54 --> 1103.60]  Linode.com slash SSH.
[1103.62 --> 1104.98]  We were just talking about events.
[1105.38 --> 1106.90]  That's how I discovered Linode.
[1107.22 --> 1111.56]  It was at a Texas Linux Fest many years ago in the before times.
[1111.56 --> 1118.78]  And I could tell Texas Linux Fest was special because it was small, but the signal was very
[1118.78 --> 1119.30]  strong.
[1119.46 --> 1120.06]  You know what I mean?
[1120.10 --> 1123.62]  Like the talks were by like heavy hitters who knew their stuff.
[1123.66 --> 1127.92]  They were passionate about their projects, but the vendors weren't taking it very seriously.
[1129.26 --> 1130.24]  Except for Linode.
[1131.52 --> 1133.72]  Linode had a real serious setup.
[1133.90 --> 1134.56]  They were clearly participating.
[1135.40 --> 1139.16]  They were also, they would swap so somebody could be at the booth while somebody could actually
[1139.16 --> 1139.92]  attend the sessions.
[1139.92 --> 1141.44]  Like you could tell they were into it.
[1142.08 --> 1143.80]  And that's, that's when I made a mental note.
[1143.80 --> 1146.22]  Like I need to check out Linode.
[1147.08 --> 1148.90]  You know, that's like almost four years ago now.
[1149.56 --> 1150.80]  And now here they are, right?
[1150.82 --> 1155.72]  They've been sponsoring the self-hosted podcast from the get-go because it's just the perfect
[1155.72 --> 1159.36]  combination of performance, features, price.
[1159.44 --> 1162.62]  I mean, 30 to 50% cheaper than all the hyperscalers out there.
[1162.72 --> 1166.70]  And if you like to go to events, and I know you might, if you're going to go to the web summit,
[1166.70 --> 1169.24]  November 1st through the 4th, Linode's going to be there.
[1169.24 --> 1173.18]  Or IT Nation Connect in Orlando, Florida, the 9th through the 11th, Linode's going to be
[1173.18 --> 1173.38]  there.
[1173.68 --> 1177.56]  There's actually a whole list of events that Linode's going to.
[1177.96 --> 1178.62]  But try it out.
[1178.76 --> 1181.56]  Even if you're not going to an event, try it out because it's great performance.
[1181.70 --> 1186.92]  They have systems with super fast CPUs, MVME hard drives, 40 gigabit connections.
[1187.48 --> 1190.10]  And they're spinning up like a dozen new data centers next year.
[1190.24 --> 1191.92]  So there's just going to be more and more choice.
[1191.92 --> 1198.46]  So go get the $100 and actually kick the tires because with that $100, you can actually try it.
[1198.68 --> 1200.84]  You can really see what works and what doesn't work.
[1201.10 --> 1203.54]  Like you really can try any feature you want with that $100.
[1204.28 --> 1205.58]  So go, well, just about, I would imagine.
[1205.92 --> 1206.46]  I don't know.
[1206.80 --> 1209.76]  If you're Alex, you could probably come up with a way to spend that $100 in like one day.
[1209.94 --> 1212.56]  But you could also stretch it out for like 60 days.
[1212.56 --> 1217.22]  So go to Linode.com slash SSH, sign up, try it out and support the show.
[1217.62 --> 1219.86]  Linode.com slash SSH.
[1221.62 --> 1225.58]  Prima has it that the HA Yellow is in production.
[1226.48 --> 1227.60]  It's here, Alex.
[1227.88 --> 1228.46]  It's here.
[1228.70 --> 1230.64]  It's live and it's glorious.
[1231.54 --> 1236.70]  The Home Assistant Yellow finally arrived about a year after I crowdfunded it.
[1236.98 --> 1242.38]  I decided when I saw that it was shipping, I decided to order an MVME drive for it.
[1243.46 --> 1245.76]  Mine came with a CM4.
[1246.22 --> 1250.90]  I could have sworn I ordered it without a CM4, a Compute Module 4.
[1251.30 --> 1253.44]  But it came with one, which is okay.
[1254.00 --> 1257.06]  My CM4s have eight gigs of RAM, but whatever.
[1258.58 --> 1260.68]  So this one only has four, but that's fine.
[1260.72 --> 1261.18]  Or maybe two.
[1261.26 --> 1262.30]  I don't know what it is.
[1262.34 --> 1264.16]  It's not enough, but we're getting by.
[1264.72 --> 1265.16]  I hit that.
[1265.16 --> 1267.64]  The first thing I did is I put that MVME disk in there.
[1268.08 --> 1278.12]  I powered the thing up and discovered very quickly that it was just running off of the built-in EMMC and wasn't using my MVME disk.
[1278.72 --> 1282.90]  And I thought, well, now, what am I supposed to do with this?
[1283.08 --> 1284.12]  Just throw it in the garbage.
[1284.64 --> 1284.76]  You know.
[1284.80 --> 1285.82]  Yeah, get rid of it.
[1286.02 --> 1286.30]  Bye-bye.
[1286.52 --> 1290.28]  And I was digging through the system settings and I go in the storage area.
[1290.60 --> 1293.28]  And in the hamburger menu, there's like this migrate option.
[1293.28 --> 1297.80]  So I hit that and it says, we're going to move your data over to another disk.
[1297.86 --> 1298.96]  What disk would you like to use?
[1299.26 --> 1303.36]  And the only disk I had available was the new MVME, about a terabyte.
[1304.54 --> 1310.10]  It says, okay, well, this will take about 15 minutes and then we're going to reboot and we'll see you then.
[1310.46 --> 1313.04]  So I say, okay, go ahead.
[1313.52 --> 1314.42]  I hit that button.
[1315.40 --> 1316.30]  Little thing starts spinning.
[1317.46 --> 1318.98]  And I just couldn't watch it.
[1319.42 --> 1320.10]  I couldn't.
[1320.44 --> 1322.18]  It was too stressful because I didn't know what it was doing.
[1322.18 --> 1327.30]  Because, again, when it's all like web UI and their own OS, I have no idea what's happening.
[1327.72 --> 1338.10]  If they told me to go like, you know, repartition a disk and format it, mount it, and then update your configuration file to point to the new mount point, I'd feel like really solid.
[1338.26 --> 1339.38]  Like, okay.
[1339.68 --> 1340.14]  All right.
[1340.14 --> 1340.82]  I know I'm done.
[1341.18 --> 1343.22]  But, you know, that's not going to work for most people.
[1343.32 --> 1344.80]  They want to make it all a GUI option.
[1344.90 --> 1345.70]  So, okay, I'll try it.
[1346.38 --> 1352.10]  So I go to bed and I wake up the next morning and I go to the storage area.
[1352.18 --> 1352.98]  In the settings.
[1353.34 --> 1354.46]  Everything's working, by the way.
[1354.74 --> 1358.50]  I go to the storage area in the settings and now it just says like 900 gigs free.
[1359.50 --> 1364.76]  I think it moved everything off of the EMMC and it moved everything to the MVME.
[1366.14 --> 1370.64]  I'm not sure exactly what happened because it's kind of, it's all kind of abstracted for me.
[1370.64 --> 1376.48]  But the performance is so much better.
[1376.70 --> 1381.14]  And I have to say, I am very happy with the results.
[1381.34 --> 1383.20]  I could not ask for anything better.
[1383.38 --> 1385.48]  And I also decided to just start fresh.
[1385.76 --> 1386.32]  I went clean.
[1386.44 --> 1387.76]  I did not restore my backups.
[1388.32 --> 1390.46]  I didn't try to import my old settings.
[1390.46 --> 1396.16]  I just said, I'm going to burn three or four days straight and I'm just going to reset it up.
[1396.48 --> 1400.16]  And I literally probably spent three days resetting it up.
[1400.74 --> 1404.56]  There is a good argument to, you know, nuke and paving systems every now and again.
[1404.68 --> 1412.50]  Like I remember back in the day, I used to nuke and pave windows every six weeks sometimes, you know, because it was just that crusty.
[1413.12 --> 1413.78]  You still have to.
[1414.04 --> 1414.70]  Hasn't changed.
[1414.70 --> 1420.84]  And then, you know, when I get a new phone these days, still out of force of habit, I'll start from scratch with a new phone.
[1421.60 --> 1427.64]  But I don't know, like my MacBook here has got the same install on it as when it came with it.
[1427.70 --> 1430.26]  Like I don't feel the need to do that anymore.
[1430.50 --> 1437.00]  But Home Assistant, there's so much stuff in there that I've painstakingly created.
[1437.38 --> 1438.64]  I don't think I could do it.
[1438.86 --> 1439.64]  I don't think I could do it.
[1440.00 --> 1442.56]  I had a couple of moments, I think, that saved me.
[1442.56 --> 1449.98]  One was I downloaded my old backup from the Raspberry Pi that died and I extracted it manually.
[1450.46 --> 1461.70]  And I opened up my configuration YAML and I kind of grabbed a few key things that I knew I wanted, like my generic thermostat stuff, all of my integrations for my cameras.
[1462.26 --> 1463.82]  I just grabbed that stuff.
[1464.06 --> 1469.42]  So I didn't take the whole config file, but I just took the bits that I didn't want to have to recreate from whole cloth.
[1469.42 --> 1474.18]  That was one thing that I think helped a lot is I still used my old config file quite a bit.
[1474.98 --> 1476.30]  But the other thing was.
[1477.34 --> 1480.58]  The Z-Wave migration turned out to be a lot easier than I expected.
[1481.22 --> 1484.72]  The Z-Wave controller had everything on the network paired to it.
[1485.48 --> 1487.08]  And so when I took that USB dongle.
[1487.08 --> 1491.18]  And I plugged it into the new Home Assistant yellow.
[1492.96 --> 1495.88]  All of the nodes were still paired to that controller.
[1496.88 --> 1500.26]  They all showed up as brand new devices to Home Assistant.
[1501.06 --> 1503.14]  But all of the networking was already done.
[1503.24 --> 1506.88]  All the node order, all of that was already done.
[1506.88 --> 1514.78]  And so Home Assistant, just using the new integration, just said, oh, look at all these Z-Wave devices you have.
[1515.76 --> 1516.92]  This is incredible.
[1518.00 --> 1522.40]  And so the only part that was a pain in the butt was I did have to sit there.
[1522.40 --> 1529.04]  And this was one of like the seriously labor intensive tasks and rename every entity, every device entry.
[1529.38 --> 1532.40]  Just sit there and rename them because it just generates these stupid ass names.
[1532.80 --> 1533.86]  You know what would be really great?
[1533.86 --> 1542.60]  Like, imagine if Home Assistant had this like paper clip in the corner that popped up and said, hey, I noticed you've got some new devices.
[1542.88 --> 1543.90]  Do you want to set those up?
[1544.62 --> 1545.70]  I mean, super helpful.
[1545.92 --> 1547.60]  I don't think anyone's done that before.
[1547.60 --> 1551.44]  Just something that said, hey, would you like to just say what you want to call it now?
[1551.96 --> 1554.90]  So that way you don't spend the next two days renaming all these things.
[1554.90 --> 1561.80]  Because, of course, like my sensors, every single one of my sensors has like eight different entities that it puts in there.
[1561.80 --> 1562.00]  Right.
[1562.00 --> 1566.52]  All of my power switches have like three or four different entities that they put into there.
[1566.60 --> 1569.38]  So it's just so, so many items.
[1569.58 --> 1570.08]  That's a good point.
[1570.16 --> 1574.12]  The onboarding workflow of a new device, I think, could actually use some work in that respect.
[1574.62 --> 1576.90]  Some kind of a wizard or something.
[1577.32 --> 1578.00]  I should say.
[1578.42 --> 1579.38]  So that's my criticism.
[1579.58 --> 1580.50]  But I should say.
[1581.44 --> 1581.92]  Wow.
[1582.14 --> 1585.64]  It has gotten so much easier to set up Home Assistant.
[1585.64 --> 1589.86]  There's so many more UI options for stuff now.
[1590.86 --> 1591.82]  Like scripts.
[1591.90 --> 1593.78]  When you're writing a script, you know, the script thing.
[1593.92 --> 1595.52]  You can just reorder items now.
[1595.90 --> 1596.50]  Oh, God.
[1596.76 --> 1600.48]  I used to have to rewrite the script or I'll do it in YAML in the past.
[1600.80 --> 1602.24]  Now you can just reorder items.
[1602.24 --> 1609.18]  It's incredible the stuff that just the friction that they over time have smoothed out.
[1609.18 --> 1616.24]  It reminded me of like if you've been playing an MMO since it launched, like say Star Trek Online, and you've been playing it for like 10 years.
[1616.24 --> 1620.34]  And so like you're just at the end game and you've been at the end game for years.
[1620.50 --> 1627.74]  And then you decide to go create an alt account and you start over from the beginning and you realize they've completely redone the beginning of the game.
[1627.82 --> 1629.22]  A totally new tutorial.
[1629.48 --> 1631.24]  A totally new introduction to the game.
[1631.34 --> 1632.68]  A whole new story arc.
[1632.76 --> 1636.90]  And you're like, wow, this is so much better than when I tried this years ago.
[1637.26 --> 1639.00]  That's where Home Assistant is at now.
[1639.08 --> 1641.40]  It is so much easier to set up.
[1641.80 --> 1641.90]  Interesting.
[1641.90 --> 1646.68]  Well, maybe I should do and you can pave just in the interests of science and the show and stuff like that.
[1646.86 --> 1648.70]  I feel like it was a lot simpler.
[1649.14 --> 1650.64]  I mean, yeah, I had to go through the whole rename thing.
[1651.18 --> 1653.04]  Here's the other thing that's been a lot easier this time around.
[1653.88 --> 1657.22]  As of right now, I don't have a single automation.
[1657.50 --> 1658.42]  You look smug about that.
[1658.50 --> 1659.64]  Why do you look smug about that?
[1659.70 --> 1660.32]  Oh, I don't know.
[1660.34 --> 1662.72]  My last box, I probably had like 15 automations.
[1663.02 --> 1664.92]  And now I don't have a single automation.
[1665.20 --> 1667.48]  And I mean, if you think about it, I'm sure I will.
[1667.58 --> 1668.22]  I have one eventually.
[1668.76 --> 1670.10]  It's so much simpler.
[1670.10 --> 1684.70]  So I have used the scheduler card custom component that lets me schedule things in a UI that is so much more intuitive than using an automation that controls the lights and the outdoor stuff so much simpler.
[1684.94 --> 1687.48]  And then I've gone all in on thermostats.
[1687.60 --> 1692.12]  So I use the generic thermostat, which combines a temperature sensor with a smart plug.
[1692.12 --> 1699.12]  So the temperature sensor is used as the thermostat data and the smart plug gets toggled on and off.
[1699.20 --> 1703.12]  And I just set the temperatures using generic thermostats now.
[1704.02 --> 1705.62]  It's so much easier.
[1705.90 --> 1708.70]  My first pass, they didn't have generic thermostats.
[1709.02 --> 1713.42]  And so I was doing automations based on temperature ranges and sensor data.
[1713.64 --> 1714.84]  And it was all manual.
[1715.06 --> 1717.20]  And now it's just so smooth.
[1717.20 --> 1725.74]  And so that made it a lot easier to not having to like rebuild my automations was a huge time saver.
[1725.92 --> 1729.56]  And so using the scheduler card, which I will link in.
[1729.74 --> 1731.04]  It's not the scheduler integration.
[1731.26 --> 1732.08]  That's something different.
[1732.38 --> 1733.66]  You want the scheduler card.
[1733.84 --> 1736.50]  I'll have a link to that in the show notes and the generic thermostat.
[1736.50 --> 1738.40]  That is just something built into Home Assistant.
[1738.76 --> 1741.92]  Those two things together save me a ton of ache.
[1741.92 --> 1753.26]  And because the scheduler card allows for things like presence detection, sunset information, those types of things, I was able to avoid creating automations for things that I used to do all the time.
[1754.14 --> 1754.42]  Yeah.
[1754.92 --> 1755.76]  Oh, it's so great.
[1755.90 --> 1756.40]  It's so great.
[1756.46 --> 1757.84]  And it's so fast, Alex.
[1758.18 --> 1761.44]  Well, that's what happens when you have real storage, like an NVMe disk.
[1761.44 --> 1772.68]  You know, Home Assistant is making a lot of, you know, little transactions, which an SD card or even something hanging off the USB bus just isn't optimized for.
[1773.04 --> 1774.12]  It didn't feel like a problem.
[1774.76 --> 1780.26]  But now it's so fast that like, you know, have you ever had that thing where you accidentally like double tap or something like that?
[1780.34 --> 1785.64]  Like you just kind of like have a finger spasm and you tap twice when you mean to tap once or something like that.
[1785.96 --> 1786.14]  Yes.
[1786.22 --> 1788.88]  It's so fast that like it'll hit it.
[1788.98 --> 1789.62]  It'll boom, boom.
[1789.62 --> 1794.04]  Like when I double do that double tap spasm, light on, light off, just boom, boom.
[1794.16 --> 1795.38]  It's it's incredible.
[1795.50 --> 1798.64]  There's just there's literally no delay at all.
[1798.84 --> 1802.98]  And I am so happy with the Home Assistant Yellow using NVMe storage.
[1804.32 --> 1807.54]  I don't even mind that it's running its own operating system.
[1807.66 --> 1808.52]  I'm all in right now.
[1808.56 --> 1811.66]  And it's been funny watching my snapshots as I've configured this thing.
[1811.82 --> 1817.54]  When I first started like a 300 kilobyte snapshot and then a megabyte and then two megabytes.
[1817.54 --> 1820.08]  And now my snapshots are like 60 megabytes.
[1820.08 --> 1820.34]  Right.
[1820.42 --> 1824.90]  It's just as I keep building the system out, like the backups keep getting bigger and bigger.
[1825.16 --> 1825.64]  I love it.
[1825.84 --> 1826.94]  But you are such a nerd.
[1827.36 --> 1831.22]  On my old Pi, I think like the Home Assistant backups were like 1.2 gigabytes.
[1831.22 --> 1835.42]  And now they're like 70, 80 megabytes or something around there.
[1835.46 --> 1838.34]  They're just totally it's a totally leaner, meaner system.
[1838.80 --> 1840.14]  There's a lot of advantages to that.
[1840.26 --> 1844.92]  And I had to take some remedial action with one of my Shelleys this week.
[1845.48 --> 1853.66]  My Shelleys 2.5 that Brent, the wonderful Brent helped me install whilst he was here, that controls my outdoor rear floodlights.
[1853.66 --> 1856.76]  We were down at the fire pit and I had the lights on the back of the house.
[1856.84 --> 1858.36]  So it was lighting up the yard a little bit.
[1859.12 --> 1865.86]  Every 30 to 60 seconds, they would just turn off for a second and then turn back on for 30 seconds.
[1866.70 --> 1869.32]  And then turn off and then turn back on.
[1869.34 --> 1870.56]  And I'm like, what are you doing?
[1870.78 --> 1871.38]  That's not good.
[1871.80 --> 1871.98]  No.
[1872.18 --> 1876.44]  So I go in the Shelleys app and then for some reason the device is rebooting and resetting itself.
[1876.44 --> 1887.26]  So I have to catch the Shelleys app just at the right time where the device is on the network to even get network connectivity to get it to load in the app properly before it resets itself.
[1888.10 --> 1891.44]  Turns out it only did that when it was under load with the lights on.
[1891.52 --> 1897.36]  So my guess is there was some kind of a threshold of maybe temperature, I don't know, being met.
[1898.66 --> 1904.06]  So I did a bit of research and this led me to something I've done in the past on a couple of my other Shelleys,
[1904.06 --> 1913.74]  which is replace the stock firmware, the Mongoose OS that comes on the Shelleys with one of the more open firmwares, TAS Motor or an ESP Home.
[1914.30 --> 1917.60]  There's a link in the show notes, but essentially the gist is this.
[1918.22 --> 1925.00]  The Shelleys ship with non-standard DuPont pin sized, I don't know what you call it, jumper pins.
[1925.64 --> 1932.86]  So you can connect them over USB with a serial device and reprogram the Shelleys that way and manually flash the firmware onto them that way.
[1932.86 --> 1941.68]  But this Shelleys already in my wall neatly tucked away and I don't want to be pulling it out and doing that kind of thing really if I can avoid it.
[1941.88 --> 1944.94]  So I thought I'd try and find a way that does it over the air.
[1945.60 --> 1949.84]  And in the linked blog post there is a tool called MG2X.
[1951.20 --> 1959.32]  And this thing allows you to put TAS Motor directly onto the Shelleys just by using an over the air firmware upload.
[1959.32 --> 1967.16]  And within about 45 seconds, I'd replace the default OS with a single command in my browser.
[1967.78 --> 1968.24]  That's great.
[1968.28 --> 1971.48]  Is it using a built-in tool or is it an exploit?
[1971.98 --> 1972.84]  I think it must be.
[1972.90 --> 1981.94]  There's no, you know, we've talked about 2-year convert in the past, which basically created a man in the middle for these third-party updating things,
[1982.02 --> 1984.32]  which then spoofed the update server.
[1984.76 --> 1987.76]  None of that stuff is needed because the Shelleys are a lot more open than that.
[1987.76 --> 1995.20]  So I think all it was doing was just providing through, you know, when you go to a website and you have like the question mark and then a few parameters after the question mark.
[1995.90 --> 2008.10]  Essentially what it was doing was providing the URL for the update to this custom firmware, minimal firmware to the over the air URL update feature built directly into the web server of the existing Shelleys.
[2008.22 --> 2012.02]  So no weirdness, no hackery going on.
[2012.06 --> 2013.98]  It's just a really cool project.
[2013.98 --> 2017.14]  I see the Shelle plug S is supported.
[2017.56 --> 2026.04]  I actually wasn't really planning to say this, but I have noticed my least reliable device in my new setup right now is my Shelleys smart plug.
[2026.40 --> 2028.66]  I've just had it go offline a couple of times.
[2029.16 --> 2030.64]  None of my other devices have done that.
[2031.28 --> 2034.48]  And I wonder if it isn't the OS because the hardware seems pretty solid.
[2034.48 --> 2038.52]  Well, I thought I'd put TAS motor on there because it has temperature monitoring.
[2038.62 --> 2048.06]  And that was, you know, where my mind went to originally was, well, is this device resetting because there's a temperature limit set in the Mongoose OS that Shelleys ship on these things?
[2048.54 --> 2050.58]  Uh-oh, is my house about to catch fire and burn down?
[2050.80 --> 2051.22]  Yeah.
[2051.56 --> 2052.52]  Don't ignore this.
[2052.52 --> 2060.64]  And when I, you know, throw both the light switches on and put all the juice through this thing, the maximum temperature it gets to is about 50 Celsius.
[2060.98 --> 2062.24]  So it's totally fine.
[2062.68 --> 2065.06]  It's nothing to worry about from what I can tell.
[2065.50 --> 2068.82]  I don't really have anything negative to say about TAS motor on this thing.
[2068.86 --> 2072.44]  I think my original goal was to actually put ESP home on the Shelleys.
[2072.64 --> 2074.36]  But I like TAS motor so much.
[2074.40 --> 2075.22]  I'm just going to leave it there.
[2075.70 --> 2076.12]  Yeah, why not?
[2076.18 --> 2076.36]  Right.
[2076.40 --> 2076.90]  If it works.
[2077.42 --> 2078.36]  Sometimes you compromise.
[2078.56 --> 2079.06]  I did that.
[2079.06 --> 2085.30]  There was one device that I completely forgot about this, but it did happen.
[2085.40 --> 2087.22]  There was one device I just had to toss out.
[2087.64 --> 2088.86]  It was a HomeKit device.
[2089.26 --> 2092.52]  It was an LED light strip I bought that worked with HomeKit.
[2092.64 --> 2095.52]  But, you know, what the issue was is I lost the HomeKit pairing code.
[2096.28 --> 2104.54]  Not only did I lose the HomeKit pairing code, but I cannot figure out for the life of me how to get this thing to try to, like, reintroduce itself to the HomeKit network.
[2104.54 --> 2110.36]  And I just, I didn't want Wi-Fi, Zigbee, Z-Wave, and HomeKit, right?
[2110.44 --> 2111.80]  Like, I just don't need all of it.
[2112.16 --> 2121.06]  And so I went over to Amazon and I picked up the Zenglid Zigbee Smart LED light strip.
[2122.04 --> 2125.12]  It's a 16.4 foot smart light strip.
[2125.12 --> 2136.18]  Now, I know, guys, I know, I know there are ways you can build Z-Wave or Zigbee devices for pennies on the dollar compared to this.
[2136.30 --> 2137.14]  I understand that.
[2137.74 --> 2138.82]  Here's the situation.
[2139.98 --> 2150.30]  I deployed my new system and the kitchen light strip, this is the one that my wife uses while she's cooking to get a little extra light, wasn't working because it's a HomeKit one.
[2150.30 --> 2153.56]  And she wanted something fast.
[2153.76 --> 2157.38]  And the wife approval factor was declining with the new server quickly.
[2157.88 --> 2162.92]  So I snapped up this Zenglid Zigbee Smart LED strip.
[2163.00 --> 2163.80]  I don't know if I'm saying it right.
[2164.12 --> 2166.28]  It's got LEDs in it and it's got smarts in it.
[2166.46 --> 2168.32]  And it says it's for Alexa and Google.
[2168.48 --> 2171.44]  It's just a Zigbee device.
[2171.44 --> 2180.76]  And so you just, if you have a Zigbee controller, you just get it, you know, doing the Zigbee thing and you can control it immediately with Home Assistant.
[2180.94 --> 2181.60]  It picks it up.
[2181.88 --> 2183.96]  You can control the colors, the brightness.
[2184.66 --> 2185.60]  Everything works.
[2185.94 --> 2187.08]  Talks to it natively.
[2187.42 --> 2189.02]  It's 60 bucks from Amazon.
[2189.36 --> 2194.64]  But it is one of these things that you can just buy and pair immediately natively to Home Assistant.
[2194.82 --> 2197.02]  And we got it up and running in 15 minutes.
[2197.72 --> 2199.42]  And man, did that solve the problem.
[2199.42 --> 2201.94]  And now she's 100% in on the new system.
[2202.38 --> 2203.98]  So I just wanted to give that a plug.
[2204.10 --> 2210.62]  If you're looking for an LED light strip that you can hook to a Zigbee network that works with Home Assistant, I can vouch for this guy.
[2210.74 --> 2211.80]  And I'll put a link in the show notes.
[2212.26 --> 2218.72]  It also comes with a remote, which I have not tried yet, but I believe is also a Zigbee device.
[2218.74 --> 2220.56]  It's just an on and off in brightness.
[2220.70 --> 2222.84]  So it's a little physical remote that you can mount anywhere.
[2223.36 --> 2226.72]  And I would imagine once you tie it to Home Assistant, it could control anything.
[2226.72 --> 2229.66]  And the kit I got from Amazon for 60 bucks includes that.
[2229.74 --> 2232.48]  It also includes a Zigbee hub, which I do not need.
[2233.44 --> 2236.34]  Well, tell me about your jellyfin exploits this week.
[2236.40 --> 2237.18]  You've been a busy boy.
[2237.60 --> 2238.22]  Oh, geez.
[2238.64 --> 2239.04]  Oh, geez.
[2239.06 --> 2240.10]  You want to hear about this?
[2240.52 --> 2241.56]  I mean, I don't know.
[2241.58 --> 2241.88]  Do we?
[2242.22 --> 2242.78]  You tell me.
[2242.84 --> 2243.38]  You tell us.
[2243.50 --> 2244.74]  Let the audience be your guide.
[2245.14 --> 2245.48]  All right.
[2245.48 --> 2246.56]  So it was going real well.
[2247.08 --> 2249.42]  I mean, I thought to myself, here's what I'm going to do.
[2249.68 --> 2251.60]  I got this whole no container theory.
[2251.80 --> 2253.74]  I think this is going to work really well.
[2254.12 --> 2256.98]  I'm going to just install everything natively on Nix.
[2257.24 --> 2260.56]  I'm going to use the Nix package manager to manage everything.
[2261.12 --> 2266.10]  And I wanted to get a sense of what this would be like before I actually deployed it on my Odroid,
[2266.10 --> 2272.02]  because I was waiting for an SSD hard drive and a power cable for that hard drive,
[2272.14 --> 2273.72]  which was a custom order piece.
[2274.42 --> 2279.20]  So I thought, in the meantime, I'll deploy it on my HP Dev 1, which already runs Nix OS,
[2279.20 --> 2285.26]  and I'll just start reconfiguring that Dev 1 like I would configure a home server.
[2285.78 --> 2292.52]  So I took an external SSD that I had from the old Raspberry Pi, and I connected that,
[2292.68 --> 2295.50]  so that way I'd have some storage to work with for a little bit, because it's just an experiment.
[2295.50 --> 2300.32]  And I got that all mounted, set up with ButterFS like a gentleman,
[2301.28 --> 2306.98]  and set up Jellyfin on Nix OS, set up Infuse on the Apple TV,
[2307.58 --> 2310.98]  and I was really, really in a good spot.
[2311.40 --> 2313.34]  I tried out Infuse this week because of you.
[2313.84 --> 2314.24]  Oh, yeah.
[2314.64 --> 2319.12]  We went to the mountains last weekend, and LNE did a bit of entertainment in the car on the way.
[2319.18 --> 2321.94]  So I thought, oh, well, Chris recommended Infuse on iOS.
[2321.94 --> 2327.12]  So I downloaded a few YouTube videos and copied a few files across.
[2327.94 --> 2329.20]  Infuse is great.
[2329.76 --> 2331.12]  Oh, you like it. Good.
[2331.22 --> 2333.74]  I really like it. Yeah, it's nice.
[2334.08 --> 2337.64]  It is so nice. And for me, it was a big, I felt like this was a,
[2338.08 --> 2340.14]  this was my best shot for a Jellyfin adoption,
[2340.14 --> 2345.32]  because we're using Infuse on Apple TV for Plex.
[2346.26 --> 2348.96]  And so if I just change the back end out to Jellyfin,
[2349.30 --> 2351.44]  it's the same exact UI for the family members.
[2351.54 --> 2353.06]  Like, nobody would probably notice, right?
[2353.22 --> 2354.88]  And now I could be using Jellyfin, right?
[2355.04 --> 2356.42]  Ooh, you're a smart cookie.
[2356.86 --> 2358.22]  I set it all up on the Nix box.
[2358.30 --> 2359.60]  I got it all working with Infuse.
[2360.38 --> 2361.10]  It was great.
[2361.10 --> 2366.52]  Then one night, we spent one night out in the woods just recently,
[2366.66 --> 2367.80]  just like a couple of days ago.
[2367.88 --> 2370.40]  We had one night to spend out, just the wife and I in the woods,
[2370.52 --> 2372.64]  between Halloween and other things going on.
[2373.48 --> 2374.58]  And we get it all set up.
[2375.64 --> 2376.40]  Candles are lit.
[2376.84 --> 2377.94]  We had an excellent dinner.
[2378.86 --> 2379.92]  Shared a bottle of wine.
[2380.80 --> 2384.08]  We go back in the bedroom, turn on the television,
[2385.02 --> 2386.22]  decide to watch a little TV.
[2386.22 --> 2390.34]  I launch the Jellyfin app, and it auto-discovers,
[2390.66 --> 2392.38]  like it has on all my other devices,
[2392.56 --> 2394.38]  auto-discovers my Jellyfin instance.
[2394.84 --> 2396.44]  I select the Jellyfin instance.
[2397.04 --> 2398.36]  The wife looks over at me,
[2398.94 --> 2401.48]  appreciating my hard work on setting all this up,
[2401.98 --> 2403.08]  thinking how great I am.
[2403.50 --> 2405.08]  I say, select that server,
[2405.36 --> 2407.34]  and I get back in error message that says,
[2407.96 --> 2409.34]  incompatible server version.
[2410.24 --> 2412.46]  Now, I'm in the woods where there's really no cell signal,
[2412.52 --> 2413.26]  so there's no streaming.
[2413.26 --> 2416.38]  I've got the room in romantic mode.
[2416.46 --> 2417.22]  The wife's back there.
[2417.28 --> 2418.50]  She's thinking I've done great,
[2418.58 --> 2419.66]  getting this whole system rebuilt,
[2419.84 --> 2421.72]  and I cannot get anything to play.
[2422.06 --> 2423.66]  And the Jellyfin app just says,
[2423.84 --> 2425.44]  go screw yourself.
[2425.58 --> 2426.54]  Your server is out of date.
[2426.64 --> 2427.20]  Oh, no.
[2427.26 --> 2428.18]  Because, of course,
[2429.04 --> 2430.28]  and this happens every now and then,
[2430.38 --> 2433.04]  Nix is really pretty much a bleeding edge,
[2433.24 --> 2434.74]  rolling distribution,
[2435.12 --> 2437.26]  but it depends on maintainers.
[2438.08 --> 2441.58]  And Jellyfin is just currently out of date on NixOS.
[2441.58 --> 2441.78]  NixOS.
[2442.82 --> 2444.48]  It's close to getting updated.
[2444.70 --> 2446.74]  They have the next version in testing right now.
[2446.76 --> 2447.64]  As of two days ago,
[2447.70 --> 2448.70]  it's really close.
[2448.78 --> 2451.34]  I could technically install it if I wanted to right now.
[2452.04 --> 2452.78]  But, you know,
[2452.94 --> 2456.02]  if I want to start playing with goodies like skip intro,
[2456.92 --> 2458.22]  well, I'm going to have to play with plugins
[2458.22 --> 2462.36]  because Infuse may not even support it if I do,
[2462.46 --> 2464.88]  but Jellyfin doesn't seem to really have native support.
[2464.88 --> 2466.28]  So, like, I'm going to have to, like,
[2466.58 --> 2468.56]  get a plugin that does intro detection
[2468.56 --> 2470.76]  and then automatically skips its server side
[2470.76 --> 2472.78]  and then just streams that to Infuse.
[2472.86 --> 2473.86]  Like, I got to, like,
[2474.18 --> 2475.60]  hack it around to get it all working.
[2475.84 --> 2476.70]  And to do that,
[2476.74 --> 2479.00]  I also need their fork of FFmpeg.
[2479.26 --> 2482.04]  And I also need everything to be the absolute latest version.
[2482.18 --> 2482.64]  All of a sudden,
[2482.68 --> 2484.30]  I'm pretty much just looking at, like,
[2484.34 --> 2486.10]  the Linux server IO Jellyfin container
[2486.10 --> 2486.56]  and thinking,
[2486.76 --> 2488.10]  why don't I just deploy that?
[2488.14 --> 2490.00]  I'm right back at the container situation.
[2490.72 --> 2492.36]  I'm right back where I began.
[2492.36 --> 2493.86]  And then on top of that,
[2493.98 --> 2495.52]  I kind of miss Plex.
[2495.88 --> 2497.42]  Like, the skip intro stuff?
[2497.78 --> 2498.52]  Huge for me.
[2498.80 --> 2500.66]  I'm watching Star Trek Enterprise right now
[2500.66 --> 2501.58]  and I refuse.
[2502.10 --> 2505.02]  I refuse to watch that intro.
[2505.18 --> 2507.00]  I will never watch that intro again.
[2507.70 --> 2508.12]  Ever.
[2508.64 --> 2510.16]  I've watched it twice in my life.
[2510.60 --> 2511.30]  When it premiered
[2511.30 --> 2513.10]  and when I played it for my wife.
[2513.64 --> 2514.50]  And after that,
[2514.56 --> 2515.90]  I will never watch that intro again.
[2516.00 --> 2516.42]  I refuse.
[2516.68 --> 2517.76]  And the third time
[2517.76 --> 2519.18]  when you loaded up Jellyfin
[2519.18 --> 2520.60]  and there wasn't this skip intro button.
[2520.62 --> 2521.12]  Oh my God.
[2521.24 --> 2522.94]  I came running across the room
[2522.94 --> 2523.48]  for the remote.
[2523.58 --> 2523.78]  I'm like,
[2524.10 --> 2524.72]  no.
[2525.80 --> 2526.20]  Yeah.
[2526.38 --> 2527.90]  And I had to fast forward like an animal.
[2528.44 --> 2528.86]  And so,
[2528.94 --> 2529.14]  like,
[2529.16 --> 2529.70]  I miss that.
[2529.82 --> 2530.04]  Also,
[2530.14 --> 2531.54]  if you're using the native apps,
[2532.32 --> 2533.02]  and I think you'll agree,
[2533.12 --> 2533.34]  Alex,
[2534.14 --> 2534.78]  the Plex app
[2534.78 --> 2535.74]  is way better.
[2536.04 --> 2536.82]  It's not perfect,
[2536.94 --> 2537.28]  but yeah,
[2537.38 --> 2538.82]  it is better.
[2539.16 --> 2540.20]  Just the layout's better,
[2540.34 --> 2540.88]  the design,
[2541.08 --> 2541.42]  everything.
[2542.16 --> 2542.90]  It's a shame.
[2542.90 --> 2543.90]  If you're using Infuse,
[2543.96 --> 2544.88]  it's exactly the same.
[2545.52 --> 2545.60]  But,
[2545.72 --> 2546.18]  yeah.
[2546.30 --> 2546.42]  So,
[2546.54 --> 2546.72]  you know,
[2547.00 --> 2549.04]  I realized that this Nix OS package
[2549.04 --> 2550.18]  is going to get updated,
[2550.40 --> 2552.32]  and this won't be an issue for much longer.
[2552.86 --> 2554.60]  But it could be an issue again,
[2555.16 --> 2555.76]  and
[2555.76 --> 2558.52]  sometimes the TV breaks
[2558.52 --> 2559.80]  at absolutely
[2559.80 --> 2561.04]  the worst
[2561.04 --> 2561.90]  moment
[2561.90 --> 2562.68]  possible.
[2563.02 --> 2564.06]  And that's what happened to me.
[2564.66 --> 2564.90]  You know?
[2564.90 --> 2565.54]  You know,
[2565.58 --> 2566.20]  and that's why
[2566.20 --> 2567.58]  I adopted Plex
[2567.58 --> 2568.66]  and the NVIDIA Shield
[2568.66 --> 2569.22]  as kind of like
[2569.22 --> 2569.92]  the default
[2569.92 --> 2571.30]  media setup
[2571.30 --> 2571.98]  in the house.
[2574.08 --> 2575.30]  Most of the time,
[2575.86 --> 2576.60]  and I would say
[2576.60 --> 2578.06]  more than 95%
[2578.06 --> 2578.68]  of the time,
[2579.76 --> 2580.88]  Plex and the NVIDIA Shield
[2580.88 --> 2581.98]  just get the job done
[2581.98 --> 2582.76]  reliably.
[2583.56 --> 2584.52]  I am enjoying
[2584.52 --> 2586.04]  the real-time updates
[2586.04 --> 2587.04]  of Hia's face
[2587.04 --> 2588.38]  in the
[2588.38 --> 2589.52]  Discord chat.
[2589.52 --> 2589.84]  I know.
[2589.88 --> 2590.72]  Are you enjoying that too?
[2590.80 --> 2591.84]  They're having a good time,
[2591.92 --> 2592.36]  aren't they?
[2592.36 --> 2594.30]  For the listeners,
[2594.46 --> 2595.44]  there's a picture of a lady.
[2595.72 --> 2596.50]  It's not Hedia,
[2597.00 --> 2597.88]  but we're just pulling
[2597.88 --> 2600.02]  a completely straight face
[2600.02 --> 2600.96]  of,
[2601.24 --> 2602.66]  I ask him to put on Netflix.
[2602.98 --> 2603.84]  He glances at me
[2603.84 --> 2604.70]  and starts fumbling
[2604.70 --> 2605.76]  with some weird cable
[2605.76 --> 2606.94]  on his TV and laptop.
[2607.42 --> 2608.28]  We sit there
[2608.28 --> 2609.66]  while he does something
[2609.66 --> 2610.28]  on his laptop
[2610.28 --> 2611.68]  with a trembling finger
[2611.68 --> 2612.70]  and mumbles something
[2612.70 --> 2614.04]  about Torrance.
[2614.82 --> 2615.78]  This one's hitting
[2615.78 --> 2616.54]  close to home.
[2617.36 --> 2618.22]  Yes, it is.
[2618.44 --> 2618.78]  Yeah.
[2618.92 --> 2619.32]  Yeah.
[2619.82 --> 2620.50]  Oh, man.
[2620.50 --> 2621.82]  Yeah, so, you know,
[2621.88 --> 2622.80]  the ironic thing is,
[2622.86 --> 2623.50]  I mean, I do follow
[2623.50 --> 2624.00]  what you're saying,
[2624.14 --> 2625.48]  but the ironic thing is
[2625.48 --> 2626.46]  if we were watching
[2626.46 --> 2627.22]  on the Apple TV
[2627.22 --> 2627.90]  with Infuse,
[2628.06 --> 2628.70]  it wouldn't have been
[2628.70 --> 2629.12]  a problem.
[2629.12 --> 2629.84]  But because we are
[2629.84 --> 2631.26]  on the NVIDIA Shield
[2631.26 --> 2632.84]  and it had auto-updated
[2632.84 --> 2633.58]  the Jellyfin app,
[2634.04 --> 2635.24]  I just got this
[2635.24 --> 2635.98]  incompatible error.
[2636.90 --> 2637.66]  But I will say,
[2637.84 --> 2639.62]  every time I try
[2639.62 --> 2640.54]  Jellyfin,
[2640.70 --> 2642.22]  it gets a little bit better.
[2642.36 --> 2642.62]  Of course,
[2642.72 --> 2643.48]  Plex is moving on
[2643.48 --> 2644.38]  as well at the same time,
[2644.40 --> 2645.08]  which doesn't help.
[2645.58 --> 2646.42]  But, you know,
[2646.48 --> 2647.62]  I think in the next
[2647.62 --> 2648.46]  year or two,
[2649.12 --> 2649.84]  the tipping point
[2649.84 --> 2650.24]  will come.
[2650.66 --> 2651.86]  We're really close
[2651.86 --> 2652.56]  to where Jellyfin
[2652.56 --> 2653.62]  will be good enough
[2653.62 --> 2655.28]  to have that Chrome,
[2655.40 --> 2655.56]  you know,
[2655.58 --> 2656.34]  like skip intro
[2656.34 --> 2656.74]  that, you know,
[2656.76 --> 2657.48]  there's little things
[2657.48 --> 2659.18]  that I really value.
[2659.70 --> 2660.64]  And once we're there,
[2660.70 --> 2661.48]  I won't look back
[2661.48 --> 2662.08]  when I switch,
[2662.46 --> 2662.70]  you know.
[2662.86 --> 2663.64]  When it's ready,
[2663.80 --> 2665.26]  it's going to be amazing.
[2666.12 --> 2666.80]  I think it's there
[2666.80 --> 2667.54]  for me now
[2667.54 --> 2668.68]  using Infuse.
[2668.88 --> 2669.86]  And so my plan
[2669.86 --> 2671.48]  is to absolutely
[2671.48 --> 2672.84]  deploy it at home
[2672.84 --> 2674.58]  and then keep
[2674.58 --> 2675.52]  Plex at the studio.
[2675.68 --> 2676.12]  So I'm like
[2676.12 --> 2677.14]  not giving up Plex.
[2677.38 --> 2678.10]  I'm going to have Plex
[2678.10 --> 2679.22]  running here at the studio
[2679.22 --> 2680.10]  on the studio server
[2680.10 --> 2680.96]  where we have like
[2680.96 --> 2682.38]  JB Media,
[2682.72 --> 2683.84]  my archived media.
[2684.32 --> 2685.38]  We share it with people
[2685.38 --> 2685.96]  like that'll be
[2685.96 --> 2686.90]  the core Plex setup.
[2686.98 --> 2688.10]  But then at my home setup,
[2688.40 --> 2689.50]  that I'm going to keep
[2689.50 --> 2690.10]  with Jellyfin.
[2690.64 --> 2692.32]  And I haven't tried it yet,
[2692.34 --> 2693.66]  but there is a plugin
[2693.66 --> 2695.70]  that lets you scan
[2695.70 --> 2697.72]  and skip intros.
[2697.82 --> 2698.32]  It has a couple
[2698.32 --> 2698.92]  of limitations,
[2699.20 --> 2700.10]  but I think it makes sense.
[2700.16 --> 2701.10]  The intro has to be
[2701.10 --> 2703.02]  within the first 25%
[2703.02 --> 2704.54]  of an episode
[2704.54 --> 2705.50]  or the first 10 minutes.
[2705.50 --> 2706.92]  And the intro
[2706.92 --> 2707.62]  has to be between
[2707.62 --> 2709.60]  15 and 2 minutes long.
[2709.72 --> 2710.38]  15 seconds
[2710.38 --> 2711.40]  and 2 minutes long.
[2711.88 --> 2712.38]  And if it meets
[2712.38 --> 2712.94]  those criteria,
[2713.10 --> 2714.20]  supposedly it can detect it
[2714.20 --> 2714.84]  and then mark it.
[2715.34 --> 2715.92]  And then on
[2715.92 --> 2717.86]  the setting side,
[2717.96 --> 2718.96]  you can just tell
[2718.96 --> 2721.16]  the Jellyfin server
[2721.16 --> 2722.58]  automatically just skip it.
[2722.80 --> 2723.80]  Don't even ask the client,
[2723.94 --> 2725.02]  just skip the intro.
[2725.46 --> 2726.62]  And I think that'll be fine.
[2726.82 --> 2727.72]  That'll work for me.
[2728.28 --> 2729.62]  And if that's the case,
[2729.66 --> 2730.02]  then overall,
[2730.16 --> 2731.12]  I'm very happy
[2731.12 --> 2731.66]  with Jellyfin.
[2731.66 --> 2732.72]  I think it'll be good.
[2732.72 --> 2733.62]  I think it'll be good.
[2734.12 --> 2734.60]  A lot of the work
[2734.60 --> 2735.34]  that Plex did
[2735.34 --> 2737.42]  with their sonic fingerprinting
[2737.42 --> 2739.22]  and all that kind of stuff
[2739.22 --> 2740.22]  to detect the intros
[2740.22 --> 2741.98]  was extremely impressive.
[2742.50 --> 2743.60]  But I think,
[2743.78 --> 2745.20]  just given a bit more time,
[2745.72 --> 2746.48]  and Jellyfin is not
[2746.48 --> 2747.26]  a commercial project
[2747.26 --> 2748.26]  like Plex, of course,
[2748.36 --> 2749.34]  so they are going to be
[2749.34 --> 2750.46]  in a different class
[2750.46 --> 2752.38]  of speed of development
[2752.38 --> 2753.14]  and polish
[2753.14 --> 2753.98]  and all that kind of stuff.
[2754.30 --> 2755.56]  I'm willing to accept
[2755.56 --> 2756.50]  those compromises
[2756.50 --> 2759.64]  for my media library
[2759.64 --> 2761.24]  being air quotes free.
[2762.04 --> 2762.48]  And perhaps
[2762.48 --> 2763.42]  not monitored.
[2763.70 --> 2765.12]  I mean, I can't make that claim.
[2765.20 --> 2765.84]  I don't know if Plex
[2765.84 --> 2766.32]  is going to monitor,
[2766.42 --> 2766.96]  but I could see
[2766.96 --> 2767.84]  how commercial interests
[2767.84 --> 2768.66]  would persuade them to.
[2768.74 --> 2769.34]  But also,
[2769.86 --> 2770.68]  just that aside,
[2771.78 --> 2772.86]  Jellyfin works a little better
[2772.86 --> 2773.96]  offline than Plex does.
[2774.12 --> 2775.54]  And I am ultimately
[2775.54 --> 2776.56]  always trying to build
[2776.56 --> 2777.78]  this system to operate
[2777.78 --> 2780.20]  as seamlessly as possible
[2780.20 --> 2781.80]  with no internet connection.
[2782.08 --> 2783.16]  And with Plex,
[2783.40 --> 2784.78]  that sometimes falls down.
[2785.28 --> 2785.92]  Well, like we talked about
[2785.92 --> 2786.88]  with Rune last week,
[2787.34 --> 2787.50]  you know,
[2787.68 --> 2788.50]  for you,
[2789.48 --> 2790.76]  where your internet connectivity
[2790.76 --> 2791.64]  comes and goes,
[2791.64 --> 2792.12]  you know,
[2792.12 --> 2792.82]  something like Rune
[2792.82 --> 2794.62]  where it just has zero minutes
[2794.62 --> 2795.54]  of guaranteed offline
[2795.54 --> 2797.38]  playback is just
[2797.38 --> 2798.98]  not an option.
[2799.58 --> 2800.96]  I didn't renew my Rune.
[2801.12 --> 2802.40]  I didn't buy Rune
[2802.40 --> 2803.22]  after my free trial,
[2803.26 --> 2803.68]  by the way,
[2804.10 --> 2805.02]  in case anybody was interested.
[2805.02 --> 2806.32]  I thought about it long
[2806.32 --> 2807.36]  and hard after the episode,
[2807.48 --> 2808.64]  but in the end,
[2808.66 --> 2809.40]  I just couldn't do it.
[2810.12 --> 2811.22]  Yeah, Jellyfin is just that.
[2811.44 --> 2812.12]  It's like,
[2812.20 --> 2813.20]  what was it?
[2813.24 --> 2814.32]  Cody, XBMC.
[2814.44 --> 2815.90]  It's like what that project
[2815.90 --> 2816.98]  could have been,
[2817.44 --> 2817.76]  you know,
[2817.84 --> 2818.52]  turned into.
[2818.64 --> 2819.70]  It's like the modern version
[2819.70 --> 2820.06]  of that.
[2820.14 --> 2821.18]  And I'm so happy to see
[2821.18 --> 2822.20]  it's moving from strength
[2822.20 --> 2822.68]  to strength.
[2822.68 --> 2824.20]  jupiter.party.
[2824.20 --> 2825.30]  If you'd like to support
[2825.30 --> 2826.20]  the entire network,
[2826.82 --> 2828.10]  invest in the ongoing
[2828.10 --> 2829.10]  content creation
[2829.10 --> 2830.20]  and get the shows
[2830.20 --> 2830.92]  ad-free,
[2831.40 --> 2832.74]  you can get every single
[2832.74 --> 2834.10]  jupiter broadcasting production
[2834.10 --> 2836.04]  at jupiter.party.
[2836.14 --> 2836.74]  Become a member
[2836.74 --> 2838.04]  and get the shows ad-free
[2838.04 --> 2839.56]  like self-hosted,
[2839.72 --> 2840.22]  including
[2840.22 --> 2842.06]  the self-hosted post show
[2842.06 --> 2843.14]  only available
[2843.14 --> 2843.86]  to our members
[2843.86 --> 2845.52]  at jupiter.party
[2845.52 --> 2846.30]  and of course,
[2846.90 --> 2848.46]  our self-hosted SREs.
[2848.84 --> 2849.48]  All right,
[2849.56 --> 2850.40]  time for some feedback,
[2850.52 --> 2850.90]  I think.
[2851.46 --> 2852.64]  Julian F. writes in
[2852.64 --> 2853.32]  Via Matrix,
[2853.60 --> 2854.74]  I was excited to hear
[2854.74 --> 2856.38]  about the Mycroft Mark II,
[2856.72 --> 2857.70]  but then discovered
[2857.70 --> 2859.70]  Mycroft STT service
[2859.70 --> 2860.74]  is a proxy for
[2860.74 --> 2862.32]  Google's STT.
[2862.42 --> 2862.86]  I think that means
[2862.86 --> 2863.72]  speech to text.
[2864.54 --> 2865.50]  Has anyone found
[2865.50 --> 2866.16]  a comparison
[2866.16 --> 2867.42]  of various home assistants
[2867.42 --> 2869.18]  and how relatively good
[2869.18 --> 2870.02]  and private
[2870.02 --> 2871.04]  each system is?
[2871.48 --> 2872.12]  I noticed there's
[2872.12 --> 2873.26]  a Mycroft integration
[2873.26 --> 2874.06]  for home assistant,
[2874.38 --> 2875.38]  but is it any
[2875.38 --> 2875.72]  good?
[2876.10 --> 2877.28]  This is a tough problem.
[2878.26 --> 2879.74]  The voice assistant
[2879.74 --> 2881.60]  stuff is
[2881.60 --> 2883.94]  kind of necessary
[2883.94 --> 2884.58]  in my house.
[2885.04 --> 2885.44]  Like, that's how
[2885.44 --> 2886.14]  my kids prefer
[2886.14 --> 2886.70]  to interact
[2886.70 --> 2887.62]  with home assistant
[2887.62 --> 2888.46]  and honestly,
[2889.00 --> 2889.86]  I'd say my wife
[2889.86 --> 2891.10]  probably 50%
[2891.10 --> 2892.96]  of the time-ish,
[2893.22 --> 2894.02]  somewhere in that range,
[2894.44 --> 2895.36]  she likes to interact
[2895.36 --> 2896.24]  with home assistant
[2896.24 --> 2897.10]  through voice.
[2897.74 --> 2898.34]  You guys know
[2898.34 --> 2898.90]  my solution
[2898.90 --> 2899.76]  has been the HomePod.
[2900.34 --> 2901.28]  The downside there
[2901.28 --> 2902.12]  is
[2902.12 --> 2903.68]  HomePods require
[2903.68 --> 2904.14]  internet
[2904.14 --> 2905.44]  to do the voice
[2905.44 --> 2905.94]  transcription
[2905.94 --> 2906.62]  and they're doing
[2906.62 --> 2907.94]  it on Apple servers.
[2908.90 --> 2910.36]  The upside
[2910.36 --> 2911.66]  is that once
[2911.66 --> 2912.24]  it figures out
[2912.24 --> 2912.98]  what you're saying,
[2913.28 --> 2914.16]  it executes that
[2914.16 --> 2914.96]  over the LAN,
[2915.20 --> 2915.90]  where some devices
[2915.90 --> 2916.88]  use like an API
[2916.88 --> 2918.06]  and a cloud system
[2918.06 --> 2918.52]  and all that.
[2919.04 --> 2919.72]  I don't know
[2919.72 --> 2920.16]  if that's the same
[2920.16 --> 2920.90]  for Mycroft,
[2920.98 --> 2921.74]  other than it sounds
[2921.74 --> 2922.24]  like they're using
[2922.24 --> 2923.22]  Google speech to text,
[2923.30 --> 2924.32]  which that's not ideal.
[2924.54 --> 2925.04]  Do you have a sense
[2925.04 --> 2925.66]  of this one, Alex?
[2925.66 --> 2927.06]  There are zero
[2927.06 --> 2927.96]  voice assistants
[2927.96 --> 2928.90]  deployed in production
[2928.90 --> 2929.56]  in this house
[2929.56 --> 2929.88]  because,
[2930.14 --> 2930.56]  as we've talked
[2930.56 --> 2931.48]  about several times,
[2932.12 --> 2933.44]  they are just getting
[2933.44 --> 2935.00]  worse and more annoying
[2935.00 --> 2936.10]  and more naggy
[2936.10 --> 2936.80]  and, hey,
[2936.90 --> 2937.42]  by the way,
[2937.48 --> 2938.08]  did you know that you,
[2938.20 --> 2938.72]  no, no,
[2938.78 --> 2939.46]  shut up.
[2939.58 --> 2940.42]  I just want to know
[2940.42 --> 2941.08]  what the weather is
[2941.08 --> 2943.26]  or I'm not interested,
[2943.54 --> 2943.82]  okay?
[2944.18 --> 2944.78]  I've never really
[2944.78 --> 2945.48]  played around with it
[2945.48 --> 2946.26]  until just this
[2946.26 --> 2947.10]  most recent build,
[2947.46 --> 2949.42]  but when you subscribe
[2949.42 --> 2950.86]  to Nebukasa Cloud
[2950.86 --> 2951.62]  for Home Assistant,
[2951.62 --> 2953.44]  one of the features
[2953.44 --> 2954.96]  you get is their
[2954.96 --> 2956.94]  text-to-speech service.
[2957.68 --> 2958.22]  I don't know
[2958.22 --> 2958.90]  if you've tried it,
[2959.22 --> 2960.40]  but it sounds
[2960.40 --> 2961.58]  better than Google's.
[2961.98 --> 2962.60]  I did a little
[2962.60 --> 2963.54]  A-B comparison
[2963.54 --> 2964.32]  and had the family
[2964.32 --> 2964.86]  say which one
[2964.86 --> 2965.40]  they liked better.
[2965.82 --> 2966.56]  They all picked
[2966.56 --> 2967.16]  the Nebukasa
[2967.16 --> 2968.32]  text-to-speech service
[2968.32 --> 2969.48]  and, I mean,
[2969.50 --> 2970.36]  it's on their servers,
[2970.66 --> 2971.36]  so I don't know how,
[2971.48 --> 2971.84]  I don't know,
[2971.88 --> 2972.30]  maybe they're just
[2972.30 --> 2973.40]  proxying somebody else,
[2973.66 --> 2975.08]  but I've been using that.
[2975.20 --> 2977.04]  So I have nighttime scripts
[2977.04 --> 2977.78]  like we've talked about
[2977.78 --> 2978.44]  in the show before
[2978.44 --> 2979.56]  and now,
[2979.70 --> 2981.06]  when the script kicks off,
[2981.62 --> 2983.00]  it uses the Nebukasa
[2983.00 --> 2985.04]  text-to-speech service
[2985.04 --> 2987.56]  to play on all the HomePods
[2987.56 --> 2988.36]  that, like,
[2988.42 --> 2989.10]  the bedtime mode
[2989.10 --> 2989.42]  is starting
[2989.42 --> 2990.02]  and everybody's got,
[2990.12 --> 2990.66]  like, 15 minutes
[2990.66 --> 2991.50]  to get their ass to bed.
[2992.08 --> 2993.24]  And it sounds great,
[2993.62 --> 2994.78]  but it's not local.
[2995.22 --> 2997.02]  I imagine it's more private
[2997.02 --> 2998.20]  than using the Google one,
[2998.28 --> 2999.08]  but it's not local.
[2999.54 --> 3000.94]  I'd love something local.
[3001.40 --> 3002.06]  It's something that
[3002.06 --> 3003.30]  could tie into a speaker.
[3003.52 --> 3004.14]  I don't care if I have
[3004.14 --> 3005.24]  to build the device for it,
[3005.64 --> 3006.38]  a little microphone.
[3007.24 --> 3007.82]  In fact, in a way,
[3007.86 --> 3009.18]  I'd prefer to build
[3009.18 --> 3009.68]  my own device
[3009.68 --> 3010.32]  because I could build it
[3010.32 --> 3011.38]  with badass microphones
[3011.38 --> 3012.10]  positioned right where
[3012.10 --> 3012.56]  I need them.
[3013.00 --> 3013.74]  That's the key, isn't it?
[3013.92 --> 3015.60]  Local, local, local.
[3015.88 --> 3016.56]  Yeah, absolutely.
[3017.06 --> 3018.64]  We did link to the
[3018.64 --> 3020.38]  integration for Mycroft
[3020.38 --> 3023.06]  that Julian also included.
[3023.40 --> 3024.06]  If you know,
[3024.44 --> 3025.04]  let us know.
[3025.22 --> 3026.84]  If you've seen a comparison
[3026.84 --> 3027.92]  of Home Assistants,
[3028.60 --> 3029.98]  if you have a little bit
[3029.98 --> 3030.90]  of experience you've done,
[3031.02 --> 3032.22]  or if you have a Mycroft
[3032.22 --> 3032.92]  that you've tried
[3032.92 --> 3033.84]  with Home Assistant,
[3034.58 --> 3035.30]  let us know.
[3035.30 --> 3036.92]  selfhosted.show
[3036.92 --> 3037.46]  contact,
[3037.76 --> 3038.96]  or you can send us a boost
[3038.96 --> 3040.08]  with a new podcast app.
[3040.22 --> 3042.48]  And speaking of boosts,
[3042.56 --> 3043.88]  Gene Bean came in this week
[3043.88 --> 3044.90]  with a really generous
[3044.90 --> 3048.00]  20,480 sats.
[3048.52 --> 3049.54]  And Gene has a question.
[3050.36 --> 3051.38]  How do y'all back up
[3051.38 --> 3052.04]  your Nextcloud?
[3052.24 --> 3054.12]  I'm running the Snap version
[3054.12 --> 3055.34]  on Debian for now.
[3055.54 --> 3056.26]  It's just simplicity.
[3056.64 --> 3058.32]  But I'm totally game to change it
[3058.32 --> 3059.66]  as I have to migrate servers
[3059.66 --> 3060.60]  at some point anyways.
[3061.22 --> 3061.90]  So how do you back up
[3061.90 --> 3062.32]  your Nextcloud?
[3062.32 --> 3063.74]  Well, all of my containers,
[3063.92 --> 3064.66]  and I run Nextcloud
[3064.66 --> 3065.32]  in a container,
[3065.72 --> 3066.48]  of course,
[3066.72 --> 3068.50]  is they're all backed,
[3068.62 --> 3069.68]  all of their app data,
[3069.86 --> 3070.40]  which is what I call
[3070.40 --> 3071.82]  the kind of persistent data
[3071.82 --> 3072.56]  of these containers,
[3073.30 --> 3074.94]  they're all ZFS volumes.
[3075.22 --> 3076.12]  And then I just replicate
[3076.12 --> 3077.54]  those across the world
[3077.54 --> 3078.66]  to various different servers
[3078.66 --> 3079.06]  that I have.
[3079.10 --> 3080.50]  I've got one upstairs.
[3080.72 --> 3081.66]  So my main server's
[3081.66 --> 3082.20]  in the basement.
[3082.96 --> 3084.12]  I use ZFS Send,
[3084.40 --> 3085.56]  which is wrapped in
[3085.56 --> 3086.56]  Jim Salter's
[3086.56 --> 3088.24]  Sanoid and Syncoid tooling
[3088.24 --> 3090.54]  to send it to a box
[3090.54 --> 3091.42]  that I have under my desk
[3091.42 --> 3091.82]  up here,
[3091.82 --> 3092.72]  which has just got
[3092.72 --> 3093.92]  a couple of 10 terabyte drives
[3093.92 --> 3096.24]  in it as a full ZFS replication
[3096.24 --> 3097.16]  of what's in the basement
[3097.16 --> 3099.32]  in case of a pipe burst
[3099.32 --> 3100.06]  or something.
[3100.56 --> 3101.52]  And then I don't have to rely
[3101.52 --> 3102.20]  on the internet
[3102.20 --> 3103.32]  to get that data back.
[3103.80 --> 3105.52]  If this house blows down
[3105.52 --> 3106.50]  for whatever reason,
[3106.74 --> 3107.42]  then I've got stuff
[3107.42 --> 3107.94]  on the other side
[3107.94 --> 3108.50]  of the Atlantic
[3108.50 --> 3109.72]  that I can recover from.
[3110.12 --> 3112.18]  And then as a third prong
[3112.18 --> 3113.34]  to that backup strategy,
[3113.90 --> 3116.08]  I use AutoRestick
[3116.08 --> 3117.54]  as a wrapper around Restick
[3117.54 --> 3118.72]  to send my stuff over
[3118.72 --> 3120.06]  to a Synology as well.
[3120.06 --> 3121.94]  And that does all the app data
[3121.94 --> 3123.04]  on a file level
[3123.04 --> 3124.36]  as opposed to ZFS's
[3124.36 --> 3125.00]  block level.
[3125.10 --> 3125.72]  So I've got kind of
[3125.72 --> 3127.82]  a two-prong approach
[3127.82 --> 3129.80]  to how I backup that data.
[3130.54 --> 3131.72]  I'm wondering what people do
[3131.72 --> 3132.70]  when they want to back up
[3132.70 --> 3135.54]  like 25 terabytes of data.
[3136.12 --> 3136.94]  Well, the only option
[3136.94 --> 3137.82]  realistically
[3137.82 --> 3139.74]  is to either pay
[3139.74 --> 3140.44]  through the nose
[3140.44 --> 3141.22]  for Glacier
[3141.22 --> 3142.04]  or something like that
[3142.04 --> 3142.54]  with AWS
[3142.54 --> 3144.92]  or to build a server
[3144.92 --> 3145.38]  and stick it
[3145.38 --> 3146.10]  at a friend's house.
[3146.10 --> 3147.50]  I mean, once you're getting
[3147.50 --> 3148.28]  above the sort of
[3148.28 --> 3151.58]  20, 50, 100 terabyte numbers,
[3152.16 --> 3153.04]  the monthly payments
[3153.04 --> 3153.76]  on that would pay
[3153.76 --> 3154.38]  for a server
[3154.38 --> 3154.86]  somewhere else
[3154.86 --> 3155.78]  pretty quickly.
[3156.16 --> 3156.68]  I think you're right.
[3157.06 --> 3157.54]  I think you're right.
[3158.20 --> 3158.96]  Gene Bean also sent
[3158.96 --> 3160.20]  another 2048 SaaS
[3160.20 --> 3160.96]  just to say that he's
[3160.96 --> 3161.60]  really been enjoying
[3161.60 --> 3162.74]  the random live feeds
[3162.74 --> 3164.24]  over at Jupyter.tube
[3164.24 --> 3165.64]  and he's looking forward
[3165.64 --> 3166.88]  to deets on the Odroid.
[3167.50 --> 3168.12]  We don't mention it
[3168.12 --> 3168.56]  all the time.
[3169.14 --> 3169.96]  I hope we've mentioned
[3169.96 --> 3170.74]  it frequently,
[3170.98 --> 3172.06]  but if you don't know,
[3172.14 --> 3173.12]  we have been live streaming
[3173.12 --> 3174.20]  over at Jupyter.tube,
[3174.20 --> 3176.32]  which is our own JB
[3176.32 --> 3177.94]  self-hosted instance
[3177.94 --> 3178.58]  of PeerTube,
[3178.74 --> 3179.58]  which is like a YouTube
[3179.58 --> 3180.22]  in a box.
[3180.56 --> 3181.88]  We mostly just use it
[3181.88 --> 3183.00]  to just record
[3183.00 --> 3184.96]  how we make the live show
[3184.96 --> 3186.12]  or how we record the shows
[3186.12 --> 3186.94]  live and all that,
[3187.02 --> 3187.82]  but, you know,
[3188.32 --> 3189.18]  you could use it
[3189.18 --> 3190.60]  if you are an open source project
[3190.60 --> 3191.94]  or a church
[3191.94 --> 3193.70]  or like a city council
[3193.70 --> 3195.10]  or a school district,
[3195.30 --> 3196.22]  you could use it
[3196.22 --> 3196.96]  as your own private
[3196.96 --> 3197.82]  YouTube instance
[3197.82 --> 3198.92]  with playlists
[3198.92 --> 3199.42]  and accounts
[3199.42 --> 3200.34]  and all that kind of stuff.
[3201.48 --> 3203.22]  User 9014,
[3203.46 --> 3204.04]  using Fountain,
[3204.20 --> 3205.24]  hasn't set their username,
[3205.76 --> 3207.14]  boosted in with 1200 sets.
[3207.34 --> 3208.54]  Tinkers will be Tinkers.
[3209.06 --> 3209.82]  I'm trying to boost
[3209.82 --> 3210.74]  the thing with the Fountain app.
[3211.10 --> 3211.54]  So far,
[3211.62 --> 3212.58]  I'm not really a fan of the app.
[3212.66 --> 3213.48]  I love the concept
[3213.48 --> 3214.32]  of value for value,
[3214.70 --> 3215.48]  but the app coming
[3215.48 --> 3216.54]  from Pocket Casts,
[3216.60 --> 3216.86]  to me,
[3216.90 --> 3217.72]  it's just not the same.
[3218.14 --> 3218.78]  Maybe it's just me
[3218.78 --> 3219.48]  being an asshole
[3219.48 --> 3220.38]  Android developer.
[3220.98 --> 3221.50]  I'll keep trying
[3221.50 --> 3222.38]  the other 2.0 apps.
[3223.12 --> 3224.04]  Thanks for the shows, though.
[3224.14 --> 3224.76]  I love them all.
[3224.94 --> 3226.46]  Sending love from Spain.
[3226.68 --> 3227.84]  Una cerveza, por favor.
[3227.84 --> 3230.06]  I agree.
[3230.06 --> 3232.38]  It's an uphill adoption.
[3232.54 --> 3233.38]  I'm not going to lie to you.
[3233.82 --> 3235.26]  It took me a solid month
[3235.26 --> 3236.22]  to wrap my head
[3236.22 --> 3236.76]  around Fountain.
[3237.54 --> 3237.94]  Really,
[3238.06 --> 3238.86]  what made Fountain stick
[3238.86 --> 3239.46]  for me is I started
[3239.46 --> 3241.28]  discovering new podcasts
[3241.28 --> 3242.22]  through their clips feature.
[3242.78 --> 3243.24]  And then I was like,
[3243.30 --> 3244.00]  I was on board.
[3244.62 --> 3245.50]  But I've been hearing
[3245.50 --> 3246.04]  from some people,
[3246.12 --> 3246.60]  they'll stick with
[3246.60 --> 3247.20]  their favorite app
[3247.20 --> 3247.68]  and they'll use
[3247.68 --> 3249.00]  Podverse.fm,
[3249.06 --> 3249.56]  the web app,
[3250.02 --> 3250.96]  to boost into the show.
[3251.38 --> 3252.90]  User 1692 wrote in
[3252.90 --> 3254.20]  with 1500 sats.
[3254.38 --> 3255.38]  I just wanted to let you know
[3255.38 --> 3256.84]  that the Rune Lifetime
[3256.84 --> 3259.22]  used to only be $499.
[3260.08 --> 3261.34]  The CEO has threatened
[3261.34 --> 3262.42]  to pull it at some point
[3262.42 --> 3263.40]  as it's not sustainable
[3263.40 --> 3264.96]  and so I buckled
[3264.96 --> 3265.92]  and bought the Lifetime.
[3266.56 --> 3267.70]  A one-off purchase for me
[3267.70 --> 3268.58]  is way better than
[3268.58 --> 3269.40]  $10 a month.
[3269.94 --> 3270.36]  I just thought
[3270.36 --> 3270.88]  you'd like to know.
[3271.56 --> 3272.70]  I'm a bit more inclined
[3272.70 --> 3273.66]  for that kind of thing, too.
[3273.74 --> 3274.86]  I mean, $499 is a little
[3274.86 --> 3275.74]  rich for my blood.
[3276.04 --> 3277.44]  Well, it's $699 now.
[3277.66 --> 3278.40]  Yeah, and sometimes
[3278.40 --> 3279.02]  every now and then
[3279.02 --> 3279.58]  those things have
[3279.58 --> 3280.62]  like a Black Friday sale.
[3280.62 --> 3281.44]  Probably not Rune,
[3281.94 --> 3284.54]  but $500 for a lifetime,
[3284.68 --> 3285.60]  I'd have to use it.
[3285.90 --> 3286.84]  I'd have to use it
[3286.84 --> 3288.52]  for at least five years
[3288.52 --> 3289.52]  consistently for me
[3289.52 --> 3290.08]  to start to admit,
[3290.20 --> 3290.70]  at least.
[3291.36 --> 3291.98]  In the time since
[3291.98 --> 3292.84]  the last episode,
[3293.54 --> 3294.90]  my free trial has expired,
[3294.98 --> 3295.58]  as I mentioned,
[3295.90 --> 3299.46]  but the feature voting section
[3299.46 --> 3301.24]  of the Rune forum,
[3302.28 --> 3305.48]  re-enabling offline grace period
[3305.48 --> 3306.18]  for the server
[3306.18 --> 3307.36]  has become their most
[3307.36 --> 3308.78]  requested feature ever
[3308.78 --> 3310.14]  in the space of a week,
[3310.14 --> 3311.00]  which I just think
[3311.00 --> 3311.56]  is amazing.
[3311.82 --> 3312.66]  That tells you something,
[3312.78 --> 3313.24]  doesn't it?
[3313.36 --> 3313.88]  It does,
[3313.98 --> 3314.48]  and it will be
[3314.48 --> 3315.20]  really interesting
[3315.20 --> 3315.90]  to see whether
[3315.90 --> 3316.90]  they listen or not,
[3317.00 --> 3318.14]  and that will dictate,
[3318.74 --> 3319.06]  for me,
[3319.14 --> 3320.22]  the posture of the company
[3320.22 --> 3320.78]  and the product
[3320.78 --> 3321.46]  moving forward.
[3321.70 --> 3322.30]  Huge signal.
[3322.42 --> 3323.12]  Depending on how
[3323.12 --> 3323.90]  they react to this
[3323.90 --> 3324.60]  will depend as to
[3324.60 --> 3325.08]  whether I become
[3325.08 --> 3325.82]  a customer or not.
[3326.42 --> 3327.20]  Yeah, you're right.
[3327.26 --> 3328.88]  This is a defining
[3328.88 --> 3329.58]  moment for them.
[3329.78 --> 3330.54]  It really is, yeah.
[3331.10 --> 3332.04]  I'm really grateful
[3332.04 --> 3332.98]  Dexword boosted in
[3332.98 --> 3333.92]  with 901 sats
[3333.92 --> 3334.84]  because I probably
[3334.84 --> 3335.36]  heard about this
[3335.36 --> 3336.54]  five times in this
[3336.54 --> 3337.40]  last week since I
[3337.40 --> 3338.04]  started talking about
[3338.04 --> 3338.58]  the Odroid.
[3338.74 --> 3338.90]  He says,
[3338.96 --> 3339.44]  have you guys
[3339.44 --> 3340.12]  looked at the
[3340.12 --> 3340.92]  Zimra board?
[3341.30 --> 3342.00]  I've been tempted
[3342.00 --> 3342.76]  to get one instead
[3342.76 --> 3343.56]  of a Raspberry Pi.
[3344.24 --> 3345.14]  I think we've talked
[3345.14 --> 3345.84]  about this on the show
[3345.84 --> 3346.72]  before, Alex.
[3346.94 --> 3347.86]  We've had some feedback
[3347.86 --> 3348.68]  about it, definitely.
[3349.02 --> 3350.46]  It's one of those
[3350.46 --> 3351.44]  boards that just
[3351.44 --> 3352.40]  looks really cool,
[3352.56 --> 3353.52]  but I don't
[3353.52 --> 3354.46]  personally have a
[3354.46 --> 3355.74]  use case for it,
[3355.74 --> 3356.64]  so I haven't bought
[3356.64 --> 3358.88]  one, but the more
[3358.88 --> 3360.40]  of you become SREs,
[3360.48 --> 3362.12]  maybe we can think
[3362.12 --> 3362.82]  about buying one.
[3363.14 --> 3363.84]  How about that
[3363.84 --> 3364.38]  for a plug?
[3364.70 --> 3365.30]  There you go.
[3365.42 --> 3366.60]  I am just too
[3366.60 --> 3368.46]  skeptical to spend
[3368.46 --> 3369.78]  my own hard-earned
[3369.78 --> 3371.90]  money on this thing.
[3372.20 --> 3372.86]  I don't know.
[3372.92 --> 3373.30]  I think I've been
[3373.30 --> 3374.26]  burned too many times.
[3374.82 --> 3377.48]  It is an Intel
[3377.48 --> 3379.10]  quad-core based system
[3379.10 --> 3380.90]  that is wrapped
[3380.90 --> 3384.16]  inside a, like it
[3384.16 --> 3384.86]  looks like it's a
[3384.86 --> 3387.14]  ruggedized case
[3387.14 --> 3387.96]  that has a heat
[3387.96 --> 3388.86]  sink that's built
[3388.86 --> 3390.06]  into it, and so
[3390.06 --> 3390.68]  it's almost something
[3390.68 --> 3391.50]  like you could install
[3391.50 --> 3392.22]  in a vehicle, which
[3392.22 --> 3392.96]  I think is one of the
[3392.96 --> 3393.76]  reasons why people
[3393.76 --> 3395.00]  have hit me up so
[3395.00 --> 3395.60]  much about it, because
[3395.60 --> 3396.46]  it looks like it's
[3396.46 --> 3397.50]  meant to be installed
[3397.50 --> 3399.62]  in a vehicle, because
[3399.62 --> 3400.42]  it's so ruggedized.
[3401.02 --> 3401.94]  So a company like
[3401.94 --> 3403.12]  Odroid has a track
[3403.12 --> 3404.44]  record, but the
[3404.44 --> 3406.04]  Zima people, Z-I-M-A,
[3406.36 --> 3406.94]  I don't know anything
[3406.94 --> 3407.50]  about them.
[3407.64 --> 3408.08]  I don't know if they're
[3408.08 --> 3408.62]  going to be around.
[3408.88 --> 3409.64]  It doesn't seem like
[3409.64 --> 3410.66]  many people have this,
[3410.70 --> 3411.24]  and if this thing
[3411.24 --> 3413.10]  isn't successful, does
[3413.10 --> 3414.24]  the company begin and
[3414.24 --> 3415.10]  end right here?
[3415.44 --> 3416.10]  Like, I have so many
[3416.10 --> 3416.94]  questions about this
[3416.94 --> 3417.88]  device, too, in terms
[3417.88 --> 3418.88]  of performance and
[3418.88 --> 3420.38]  storage, and I just
[3420.38 --> 3421.84]  don't trust it enough
[3421.84 --> 3422.42]  to spend my own
[3422.42 --> 3423.24]  money to try it.
[3423.96 --> 3425.18]  I agree, it looks
[3425.18 --> 3426.02]  perfect for somebody
[3426.02 --> 3427.22]  like me, and it does
[3427.22 --> 3428.66]  have a PCI slot, which
[3428.66 --> 3430.64]  I would love.
[3431.02 --> 3432.26]  It's really strange,
[3432.30 --> 3432.54]  isn't it?
[3432.58 --> 3434.86]  So it's got a PCI 2.0
[3434.86 --> 3438.44]  X4 PCIe slot, and two
[3438.44 --> 3440.32]  SATA ports, and two
[3440.32 --> 3441.50]  gigabit LAN ports.
[3441.54 --> 3442.24]  Yeah, it looks really
[3442.24 --> 3442.52]  good.
[3442.60 --> 3443.28]  So it would make a
[3443.28 --> 3444.76]  pretty good NAS kind
[3444.76 --> 3445.98]  of, like, brain.
[3446.28 --> 3446.96]  I agree.
[3447.74 --> 3448.56]  It's just that the
[3448.56 --> 3449.62]  Odroid looks like a
[3449.62 --> 3450.66]  complete solution that's
[3450.66 --> 3451.56]  ready to go, and to
[3451.56 --> 3452.40]  this, this just looks
[3452.40 --> 3453.32]  like it's a Kickstarter,
[3453.52 --> 3454.24]  but I know it's not.
[3454.34 --> 3454.94]  Well, it was.
[3455.56 --> 3456.56]  Yeah, it was.
[3456.80 --> 3458.02]  It was, but it's been
[3458.02 --> 3459.26]  fulfilled now, I think,
[3459.42 --> 3460.36]  which is, you know,
[3460.40 --> 3461.06]  it's not a guarantee
[3461.06 --> 3462.08]  with Kickstarter, is it?
[3462.32 --> 3463.20]  I've just been burned
[3463.20 --> 3464.34]  so many times to spend
[3464.34 --> 3465.52]  120 bucks on something
[3465.52 --> 3467.46]  like this, but I really
[3467.46 --> 3468.36]  like the look of it.
[3468.36 --> 3470.98]  If the Odroid wasn't a
[3470.98 --> 3472.64]  thing, I may be
[3472.64 --> 3472.90]  tempted.
[3473.08 --> 3474.20]  It is close to that.
[3474.78 --> 3475.68]  But now it's like, it
[3475.68 --> 3476.44]  just feels silly.
[3476.72 --> 3478.00]  I don't need it, and
[3478.00 --> 3478.56]  yeah.
[3478.64 --> 3481.34]  I mean, with a PCIe 4X
[3481.34 --> 3482.28]  slot, you could do quite
[3482.28 --> 3482.90]  a lot with this thing.
[3482.98 --> 3484.12]  You could stick extra,
[3484.32 --> 3485.92]  you know, a couple of
[3485.92 --> 3487.18]  extra SSDs in there.
[3487.28 --> 3488.36]  You could put, I
[3488.36 --> 3489.14]  don't know, a 10 gig
[3489.14 --> 3490.48]  ethernet in there.
[3490.64 --> 3491.24]  I mean, you could do a
[3491.24 --> 3492.14]  lot of cool stuff with it.
[3492.86 --> 3493.72]  It's a bit of a weird
[3493.72 --> 3494.62]  form factor as well.
[3494.68 --> 3495.30]  It's kind of like got a
[3495.30 --> 3496.44]  heatsink built into it,
[3496.46 --> 3497.54]  and then the PCI slots
[3497.54 --> 3498.74]  hanging off the side,
[3498.90 --> 3501.10]  and yeah, like, what
[3501.10 --> 3502.16]  form factor is this
[3502.16 --> 3502.78]  designed for?
[3502.92 --> 3504.86]  It looks a little bit
[3504.86 --> 3507.06]  odd in that respect,
[3507.34 --> 3509.06]  but it's certainly
[3509.06 --> 3509.58]  something I'm keeping
[3509.58 --> 3509.98]  an eye on.
[3510.40 --> 3510.84]  All right, I'm going to
[3510.84 --> 3511.60]  try to move fast,
[3511.82 --> 3512.32]  because we've got some
[3512.32 --> 3513.58]  great ones, but I want
[3513.58 --> 3514.64]  to give a mention to
[3514.64 --> 3516.36]  MG boosted in a row of
[3516.36 --> 3518.12]  ducks, 222 sats.
[3518.70 --> 3519.24]  Says, I've been very
[3519.24 --> 3520.48]  happy with LMS and
[3520.48 --> 3521.90]  Squeeze Lite running on
[3521.90 --> 3523.28]  Pies, so there's some
[3523.28 --> 3524.16]  more feedback there.
[3524.78 --> 3525.86]  J-Cube sent their first
[3525.86 --> 3526.66]  boost this week, and
[3526.66 --> 3527.38]  they just started the
[3527.38 --> 3528.60]  show at episode 73.
[3529.28 --> 3530.30]  That's amazing.
[3531.00 --> 3533.04]  Nev came in with 2004
[3533.04 --> 3533.56]  sats.
[3533.68 --> 3535.10]  2004 is the year of
[3535.10 --> 3535.72]  NGINX.
[3535.90 --> 3536.38]  That's when it was
[3536.38 --> 3536.66]  created.
[3537.34 --> 3538.54]  Ubuntu's first release.
[3539.22 --> 3540.04]  I didn't realize those
[3540.04 --> 3540.48]  two things.
[3541.22 --> 3542.20]  Gen 2 was not for
[3542.20 --> 3543.10]  weirdos at the time.
[3543.40 --> 3544.76]  That was the year Nev's
[3544.76 --> 3546.46]  car was built, and the
[3546.46 --> 3547.48]  first time they ever saw
[3547.48 --> 3548.94]  a terminal emulator, and
[3548.94 --> 3549.68]  they just wanted to
[3549.68 --> 3549.92]  share.
[3549.92 --> 3552.30]  And then Acorn wanted
[3552.30 --> 3553.30]  to know your favorite
[3553.30 --> 3554.22]  terminal app.
[3554.30 --> 3555.00]  They say they like
[3555.00 --> 3557.24]  lazy Docker project, Htop,
[3557.54 --> 3558.34]  those types of things.
[3558.42 --> 3559.20]  Do you have a terminal
[3559.20 --> 3560.82]  app that's like one of
[3560.82 --> 3562.50]  your go-tos, besides the
[3562.50 --> 3563.18]  obvious Emacs?
[3563.30 --> 3564.38]  I think it must be
[3564.38 --> 3564.78]  Hollywood.
[3565.24 --> 3566.38]  You know, that kind of
[3566.38 --> 3568.06]  one that makes me look
[3568.06 --> 3569.80]  like a legit hacker in
[3569.80 --> 3570.58]  the background with some
[3570.58 --> 3571.36]  of my live streams.
[3571.98 --> 3573.06]  That's a great answer.
[3573.18 --> 3573.78]  We've got to put a link
[3573.78 --> 3574.10]  to that.
[3574.34 --> 3575.00]  Hollywood snap.
[3575.24 --> 3576.30]  I'll put a note right
[3576.30 --> 3576.58]  there.
[3577.30 --> 3577.92]  Check it out.
[3577.92 --> 3578.88]  There's a snap for it
[3578.88 --> 3579.60]  that makes your computer
[3579.60 --> 3580.42]  look like it's doing
[3580.42 --> 3581.64]  amazing things.
[3581.74 --> 3582.74]  That's a great answer.
[3583.18 --> 3585.02]  Bashtop is also a really
[3585.02 --> 3586.62]  great one, just in terms
[3586.62 --> 3588.08]  of just visualizations and
[3588.08 --> 3588.42]  whatnot.
[3589.08 --> 3590.20]  And then Thumbs comes in
[3590.20 --> 3591.20]  with our last boost,
[3591.30 --> 3592.34]  10,000 sets.
[3593.18 --> 3593.94]  Do you guys ever have
[3593.94 --> 3596.30]  memories of what you
[3596.30 --> 3597.92]  were listening to at a
[3597.92 --> 3598.70]  specific place?
[3599.16 --> 3600.52]  I just pulled into a
[3600.52 --> 3601.94]  parking lot I haven't been
[3601.94 --> 3602.98]  to in a couple of years,
[3603.14 --> 3605.02]  and I was taken back to
[3605.02 --> 3606.00]  the moment I was listening
[3606.00 --> 3607.40]  to episode two with
[3607.40 --> 3607.80]  Wendell.
[3608.36 --> 3609.30]  Thanks for the years of
[3609.30 --> 3610.40]  memories and great content.
[3610.86 --> 3611.64]  I'm a network member,
[3611.74 --> 3612.46]  but I thought you deserve
[3612.46 --> 3613.88]  some extra value for that
[3613.88 --> 3614.20]  memory.
[3614.66 --> 3615.52]  You know, for me, I can
[3615.52 --> 3616.68]  think of a JB memory.
[3617.04 --> 3617.82]  This was when I was doing
[3617.82 --> 3618.76]  my computer science
[3618.76 --> 3621.00]  masters back in 2015,
[3621.54 --> 3623.16]  13, 14 period.
[3623.66 --> 3624.60]  And I was listening to
[3624.60 --> 3625.76]  you and Mike on Coder
[3625.76 --> 3627.32]  talk about whatever
[3627.32 --> 3628.32]  nonsense it was you were
[3628.32 --> 3629.02]  talking about at the
[3629.02 --> 3629.32]  time.
[3629.76 --> 3631.34]  And I thought, you know
[3631.34 --> 3631.56]  what?
[3631.60 --> 3632.42]  I actually know a little
[3632.42 --> 3633.16]  bit about this stuff.
[3633.24 --> 3633.92]  Maybe I should get a
[3633.92 --> 3634.40]  career in it.
[3634.90 --> 3635.36]  The funny thing about
[3635.36 --> 3636.34]  Coder, that might have
[3636.34 --> 3638.10]  been around the time we
[3638.10 --> 3639.16]  were interviewing the two
[3639.16 --> 3640.16]  co-founders of Docker
[3640.16 --> 3640.84]  before it was called
[3640.84 --> 3641.22]  Docker.
[3641.38 --> 3642.00]  I remember, yeah.
[3642.12 --> 3643.88]  And that is an old, if
[3643.88 --> 3644.56]  somebody can find that in
[3644.56 --> 3645.20]  the archive, that's a
[3645.20 --> 3646.50]  great, that's a really
[3646.50 --> 3647.16]  great old interview.
[3647.28 --> 3648.20]  Before it was even
[3648.20 --> 3649.14]  called Docker, I forget
[3649.14 --> 3649.90]  the name right now.
[3649.92 --> 3650.12]  Yeah.
[3650.36 --> 3651.14]  Mike always remembers.
[3651.68 --> 3652.82]  So that's my job is just
[3652.82 --> 3653.56]  to remember that we did
[3653.56 --> 3654.28]  the interview and then he
[3654.28 --> 3654.94]  remembers what they
[3654.94 --> 3655.38]  called it.
[3655.56 --> 3656.22]  But they didn't start
[3656.22 --> 3656.70]  with Docker.
[3657.56 --> 3658.70]  It's fascinating too,
[3658.76 --> 3659.38]  because, you know, we
[3659.38 --> 3659.92]  asked them a little bit
[3659.92 --> 3661.00]  about their business ideas.
[3661.50 --> 3662.30]  People are still asking
[3662.30 --> 3663.20]  some of the questions we
[3663.20 --> 3663.74]  asked them in that
[3663.74 --> 3664.04]  interview.
[3664.04 --> 3666.80]  Thank you to
[3666.80 --> 3667.74]  Honigan or
[3667.74 --> 3669.14]  Honanega?
[3669.80 --> 3670.10]  Don't know.
[3670.52 --> 3672.36]  Sent 3,000 sats, 5,000
[3672.36 --> 3673.46]  sats from Ninja Mort.
[3673.54 --> 3674.52]  No messages with those.
[3674.58 --> 3675.20]  They just sent them in
[3675.20 --> 3675.78]  when they were listening.
[3676.18 --> 3676.98]  We also got a few other
[3676.98 --> 3677.50]  boosts in there that
[3677.50 --> 3678.14]  didn't quite make it to
[3678.14 --> 3679.06]  the show because we got to
[3679.06 --> 3679.54]  keep it tighter.
[3679.94 --> 3680.60]  But I just want to say
[3680.60 --> 3681.28]  thank you, everybody.
[3681.78 --> 3682.68]  It's a big motivator.
[3682.82 --> 3684.10]  It really is a nice, like,
[3684.18 --> 3684.70]  boost to morale.
[3685.26 --> 3686.64]  And it's also a great way
[3686.64 --> 3687.10]  to show value.
[3687.18 --> 3688.26]  Go get a new podcast app
[3688.26 --> 3690.04]  at newpodcastapps.com
[3690.04 --> 3691.62]  or become a member.
[3692.14 --> 3692.56]  You can go to
[3692.56 --> 3693.38]  selfhosted.show
[3693.38 --> 3694.34]  slash sre
[3694.34 --> 3696.24]  and invest in the
[3696.24 --> 3697.10]  ongoing production.
[3697.24 --> 3698.06]  A boost is a great way
[3698.06 --> 3698.96]  to say good job
[3698.96 --> 3699.92]  or get a message on the
[3699.92 --> 3700.24]  show.
[3700.80 --> 3701.76]  And the membership
[3701.76 --> 3702.52]  is a great way to
[3702.52 --> 3703.38]  invest in ongoing
[3703.38 --> 3703.96]  production.
[3704.18 --> 3705.02]  Selfhosted.show
[3705.02 --> 3706.20]  slash sre.
[3707.04 --> 3707.72]  We should probably
[3707.72 --> 3708.36]  mention the Matrix.
[3708.52 --> 3709.22]  I mean, we do have a
[3709.22 --> 3709.80]  Discord, too.
[3709.90 --> 3710.80]  That's been rocking the
[3710.80 --> 3711.68]  whole episode at
[3711.68 --> 3712.42]  selfhosted.show
[3712.42 --> 3713.02]  slash Discord.
[3713.02 --> 3714.14]  But maybe honorable
[3714.14 --> 3715.14]  mention for the Matrix
[3715.14 --> 3716.12]  because it was
[3716.12 --> 3717.58]  useful for the meetup.
[3718.92 --> 3719.78]  Jupyterbroadcasting.com
[3719.78 --> 3720.46]  slash Matrix
[3720.46 --> 3722.26]  for deets on that.
[3723.16 --> 3724.18]  Thank you, Alex,
[3724.44 --> 3725.36]  because I know
[3725.36 --> 3726.12]  early this morning
[3726.12 --> 3728.40]  when the OpenSSL
[3728.40 --> 3729.58]  patches went out,
[3730.02 --> 3730.58]  you got up
[3730.58 --> 3731.70]  and got the JB
[3731.70 --> 3732.56]  infrastructure all
[3732.56 --> 3733.00]  updated.
[3733.10 --> 3733.74]  So thank you for
[3733.74 --> 3734.54]  doing that for us.
[3734.62 --> 3735.28]  By the time this comes
[3735.28 --> 3736.00]  out, people know
[3736.00 --> 3736.48]  about that.
[3737.00 --> 3737.16]  Yeah.
[3737.16 --> 3738.04]  Well, there was a big
[3738.04 --> 3738.90]  vulnerability release
[3738.90 --> 3741.06]  this morning in OpenSSL.
[3741.16 --> 3742.26]  Only the second ever,
[3742.38 --> 3742.84]  I think,
[3743.40 --> 3744.84]  critical marked
[3744.84 --> 3745.64]  CVE,
[3746.00 --> 3746.68]  something to do
[3746.68 --> 3747.28]  with remote code
[3747.28 --> 3747.82]  execution.
[3748.66 --> 3749.46]  Actually, it turned out
[3749.46 --> 3750.00]  I didn't have to do
[3750.00 --> 3750.90]  a whole bunch because
[3750.90 --> 3752.06]  I had already set up
[3752.06 --> 3752.96]  unattended upgrades
[3752.96 --> 3753.72]  in all of our Ubuntu
[3753.72 --> 3754.76]  boxes that we use.
[3755.38 --> 3756.14]  So by the time I'd
[3756.14 --> 3756.82]  logged in, it had
[3756.82 --> 3757.86]  already gone and done
[3757.86 --> 3759.32]  the unattended upgrade
[3759.32 --> 3759.96]  for the security
[3759.96 --> 3760.42]  patches.
[3761.16 --> 3761.94]  It was just an example,
[3762.12 --> 3763.24]  I suppose, of good
[3763.24 --> 3764.26]  sysadmining.
[3764.64 --> 3765.46]  But, you know, I went
[3765.46 --> 3766.18]  on to check anyway,
[3766.30 --> 3766.84]  just in case.
[3767.18 --> 3767.64]  You heard it here.
[3768.06 --> 3768.74]  You heard it here,
[3768.82 --> 3769.14]  everybody.
[3769.62 --> 3770.64]  Alex recommends using
[3770.64 --> 3771.82]  Ubuntu systems with
[3771.82 --> 3772.58]  auto-updates.
[3774.84 --> 3775.32]  Yeah.
[3777.32 --> 3777.82]  All right.
[3777.86 --> 3778.42]  Well, it's still good
[3778.42 --> 3779.00]  to have it done.
[3779.14 --> 3779.84]  So thank you.
[3780.46 --> 3781.22]  If you'd like to send
[3781.22 --> 3781.72]  us your feedback,
[3781.82 --> 3782.16]  like I said,
[3782.22 --> 3782.96]  new podcast app
[3782.96 --> 3783.90]  or self-hosted
[3783.90 --> 3785.02]  dot show slash
[3785.02 --> 3786.00]  contact.
[3786.54 --> 3787.06]  And you can go and
[3787.06 --> 3788.02]  find me over on
[3788.02 --> 3789.24]  Elon's latest play
[3789.24 --> 3790.02]  thing at Twitter.
[3790.48 --> 3791.40]  I am at
[3791.40 --> 3792.18]  ironic badger.
[3792.36 --> 3793.04]  I'm over there
[3793.04 --> 3794.44]  at Chris LAS.
[3794.68 --> 3795.96]  And the podcast
[3795.96 --> 3797.20]  is at self-hosted
[3797.20 --> 3797.44]  show.
[3797.80 --> 3799.30]  44 billion dollars
[3799.30 --> 3800.10]  for a toy.
[3800.64 --> 3801.24]  Can you imagine?
[3801.56 --> 3802.90]  For a pain in the neck.
[3802.90 --> 3803.34]  Yeah.
[3803.92 --> 3804.32]  Crazy.
[3804.96 --> 3805.70]  Anyway, thanks for
[3805.70 --> 3806.26]  listening, everybody.
[3806.52 --> 3807.32]  That was self-hosted
[3807.32 --> 3808.76]  dot show slash 83.
