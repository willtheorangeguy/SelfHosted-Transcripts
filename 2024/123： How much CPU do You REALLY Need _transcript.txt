[0.00 --> 12.06]  We've both been traveling, and I've never been quite happy with self-hosted tools around trip planning, maps, or anything that really is just better than a good paper map, Alex.
[12.16 --> 17.16]  You know, sometimes when you're traveling, especially on a road trip, it's really hard to beat the paper map.
[17.54 --> 20.50]  Or hard to beat Google Maps. Let's just be honest about it.
[20.86 --> 21.62]  That's the other problem.
[22.38 --> 28.70]  And I don't know if I'm there yet, but I have been playing around with something called FaciliMap, and I'll put a link to this in the show notes.
[29.70 --> 33.68]  It's what they say, a privacy-friendly, open-source, versatile online map.
[34.68 --> 44.56]  And what it does is it pulls in a bunch of different services that are based on OpenStreetMap and allows you to find things and visualize things in ways that Google Maps never does.
[44.56 --> 53.16]  And there's a couple of terrain options in here that just make it – well, you should go look at Washington State on a couple of these different terrain modes.
[53.26 --> 56.86]  It really helps you understand, like, where the mountains are at, where the peak elevations are at.
[56.86 --> 59.00]  But also you can then set waypoints.
[59.40 --> 62.88]  You can bring in GPX files and then lay them over this.
[63.16 --> 64.90]  You can, of course, then recall those things later on.
[64.96 --> 67.40]  You can run it through a simple Docker Compose, too.
[67.46 --> 69.12]  So it's pretty easy to get up and going.
[69.58 --> 72.42]  It gets a little more complicated if you want to put a pretty big database behind it.
[72.46 --> 74.74]  But small instance, it's not too bad.
[74.74 --> 77.40]  I always forget how good OpenStreetMap is.
[77.58 --> 79.36]  I've just pulled it up now whilst we're recording.
[80.12 --> 81.52]  And there's a whole bunch of information.
[81.70 --> 83.58]  I'm pretty familiar with the area where I live in.
[83.60 --> 84.88]  I've been here five or six years now.
[85.46 --> 89.76]  I know what the area around me looks like on Google Maps and Apple Maps in particular.
[90.62 --> 96.42]  But, you know, this has just dropped me off where my ISP spits me out in my browser as opposed to where I actually live.
[96.42 --> 100.04]  And I'm looking at this OpenStreetMap overlay.
[100.98 --> 102.80]  It's at facilemap.org.
[102.88 --> 103.86]  There'll be a link in the show notes.
[104.32 --> 108.16]  I just love the way that OpenStreetMap presents its data.
[108.52 --> 112.14]  It's not quite as good as a good ordnance survey map.
[112.52 --> 115.98]  I have a bit of a penchant for a good ordnance survey map.
[116.16 --> 119.58]  But, you know, this is a pretty good digital alternative.
[120.16 --> 125.06]  The one that I thought was kind of interesting is to go look like at a destination and then turn on the hiking trails overlay.
[125.06 --> 127.06]  And they have biking trails as well.
[127.14 --> 128.28]  Oh, that's a good spot to hike.
[128.68 --> 131.34]  And I looked and there's some massive great hiking spots near me.
[131.46 --> 132.94]  So I forgot all about that.
[133.22 --> 136.04]  It's neat and it has all kinds of different filters and features.
[136.32 --> 137.48]  And you can host it yourself.
[138.06 --> 144.20]  That and also a shout out to GPX Pod and GPX Edit, which are two different apps for your NextCloud instance.
[145.06 --> 147.06]  And these let you, say, import your Garmin nav.
[147.70 --> 150.74]  Maybe you've saved favorite spots in there and then you can view them inside NextCloud.
[151.18 --> 152.46]  So there's a couple of ways to do this.
[152.46 --> 161.42]  And I'd also be curious how anyone out there listening has solved their own self-hosted map, POI, you know, save the spot for the future type tool.
[161.98 --> 166.30]  For many years, my solution to that problem has been drop a star on Google Maps.
[166.48 --> 171.98]  I would love to get that brought in-house and own that particular data mine.
[172.70 --> 172.86]  Yeah.
[173.04 --> 173.24]  Yeah.
[173.26 --> 173.88]  That's what I'm thinking.
[174.34 --> 175.18]  There's got to be a way.
[175.18 --> 179.54]  GetGrist.com slash self-hosted.
[179.60 --> 183.14]  Grist is the open source alternative to Airtable and Google Sheets.
[183.54 --> 184.40]  No shame here.
[184.48 --> 190.54]  But if your company has one of those load-bearing spreadsheets, I swear just about every company has one of these.
[190.62 --> 194.62]  They become impossible to maintain over time, but they're too important to fail.
[195.20 --> 196.78]  Everyone seems to rely on one of these.
[196.88 --> 199.44]  And inevitably, it's like one person owns it.
[199.50 --> 200.74]  And then what happens if they go?
[200.74 --> 204.52]  Or, like, what happens if their bad data hygiene practices make its way into its spreadsheet?
[205.34 --> 215.62]  What you really want is something that is easy to use as a spreadsheet by all users, but is reliable, accessible, maybe as portable as an actual database.
[216.34 --> 218.58]  And it makes sense that people get trapped in the spreadsheet world.
[218.70 --> 219.22]  I've seen it.
[219.28 --> 219.82]  I understand.
[220.22 --> 221.34]  You've got to check out Grist.
[221.38 --> 225.82]  It's really good at combining why people like spreadsheets with why databases make sense.
[226.14 --> 230.02]  And the user doesn't need to know that it's a relational database underneath all of it.
[230.02 --> 231.30]  They just get to build.
[231.30 --> 241.70]  And if you've ever looked at something like a database and thought, hmm, I wish others could access this with a GUI and then maybe not have to learn SQL or something like that, Grist fits in really well.
[242.22 --> 245.86]  Grist is a fully integrated spreadsheet UI built on top of a portal SQLite file.
[246.40 --> 249.54]  Non-technical users can add and analyze data like a spreadsheet.
[250.14 --> 255.86]  But everything is relational and managed within a sophisticated set of access rules, even down to the table.
[255.86 --> 259.44]  So Grist works so well with your existing authentication infrastructure.
[259.72 --> 265.38]  And it's easy to integrate because of a REST API and there's lots of popular integrations ready to go right now.
[265.80 --> 274.40]  And as a listener of this show, I bet you're going to appreciate that Grist is open source and receives active code contributions from the community like the French government who uses Grist for thousands of their employees.
[275.08 --> 279.74]  Grist is the open source alternative you can host yourself with a portable file that makes sense.
[280.04 --> 281.44]  Go try it out and support the show.
[281.44 --> 284.52]  It's getgrist.com slash self-hosted.
[284.64 --> 286.96]  Stop worrying about the technology and use the best.
[287.12 --> 289.84]  Getgrist.com slash self-hosted.
[291.44 --> 295.42]  Another episode of Self-Hosted and here we are talking about Image yet again.
[295.74 --> 303.64]  The day after we recorded the last episode, some news about Image dropped, which we probably should cover in this episode.
[304.58 --> 309.72]  Image is joining forces with an organization known as FUTO.
[309.72 --> 313.28]  Yeah, and now the core team is going to go full time as a result of this.
[313.46 --> 320.42]  FUTO may ring a bell because they have funded other open source projects, although this seems like quite the commitment.
[320.92 --> 324.14]  It's a really interesting situation we find ourselves in here.
[324.66 --> 331.80]  Essentially, the gentleman behind FUTO, I believe he made some money with WhatsApp at some point in the past.
[331.80 --> 339.66]  And as such, he kind of got a little bit burnt out with Silicon Valley and some of the VC skullduggery that goes on.
[340.32 --> 346.84]  And essentially, his mission in life now seems to be to stick a middle finger up at big tech.
[347.44 --> 348.58]  At least that's how I read it.
[348.58 --> 356.62]  Yeah, or at least try to make an environment where certain types of development that might otherwise not be sustainable can be sustainable.
[356.78 --> 358.72]  That's the more PC way to put it, yes.
[359.20 --> 361.52]  Well, it does mean there are some transactions here, right?
[361.62 --> 368.58]  So FUTO does now technically own the trademarks and the source code, although the project will remain AGPL.
[369.62 --> 372.52]  So I suppose if things went sideways, the source code is still available.
[372.52 --> 374.44]  So the core team stays in place.
[374.52 --> 377.34]  This is just going to be their full-time job right now, which is huge.
[377.42 --> 379.46]  I mean, you can't really understate that.
[379.52 --> 383.80]  And the core team seems to be providing the direction and the feature set.
[384.40 --> 393.44]  With the only real request that I can see that FUTO has made is that, you know, build this whole thing so that way we can make a cloud service out of it one day, which I think the image team was already going to do.
[394.20 --> 394.30]  Right.
[394.70 --> 397.82]  As I understood it, I've been talking to Alex Tran.
[397.94 --> 402.24]  We've had him on the show before, but I've been talking to him a lot in the last couple of weeks about this news.
[402.52 --> 406.02]  You know, trying to make sure that everybody's happy with it.
[406.22 --> 413.38]  The reaction to this has been pretty interesting because I will certainly admit my heart dropped when I read that first sentence.
[414.52 --> 416.98]  Initially thinking, oh, God, image has been bought out.
[417.32 --> 420.88]  But as you just said, Chris, the source code remains AGPL.
[420.88 --> 438.62]  I think that alone, that single fact alone gives me huge peace of mind that even if we need to rename image because of the trademark situation in a few years, for whatever reason, even if that needs to happen, the source code and all the effort that's being put in here is not going to go to waste.
[438.62 --> 441.88]  It does seem like one of those situations where the benefits are pretty clear.
[442.24 --> 447.08]  You know, the team that's been setting the direction is going to be the same team that continues to set the direction.
[447.60 --> 450.18]  They're not going to change anything dramatically about the project.
[450.32 --> 451.56]  It's going to remain AGPL.
[451.68 --> 456.90]  Those things, those are obviously palatable benefits, let alone getting the dev team hired.
[457.02 --> 457.78]  That's just, that's huge.
[458.04 --> 458.16]  Yeah.
[458.30 --> 460.32]  And the downsides are all kind of what ifs.
[460.34 --> 463.56]  Like, well, what if in five years, like they don't see eye to eye?
[463.66 --> 465.72]  Like those are all the downsides are like what ifs.
[465.72 --> 468.22]  And those are things that we could always pivot, tuck and roll.
[468.54 --> 470.48]  I mean, it's a legitimate concern.
[471.02 --> 479.24]  This gentleman who's behind Futo, for example, what if he gets bored and decides to do a Russ Hanneman and drive off with Tres Comas into the distance?
[479.24 --> 482.62]  You know, it's like what's going to happen to the project in that situation?
[482.62 --> 494.34]  But I think also it speaks to the fact of how little trust we have in tech in general that most people's first reaction to this is negative.
[494.34 --> 497.06]  Yeah, I think, you know, people fool me once.
[497.38 --> 501.22]  How do you think people will react when they do put a price tag on it?
[501.28 --> 506.36]  I think that's the goal here is Futo is going to say, hey, if you use this, why not pay for it?
[506.38 --> 507.10]  Like it's still free.
[507.34 --> 508.28]  You can still get it.
[508.30 --> 509.44]  You can still self-host it.
[509.64 --> 512.94]  But if you'd like to send us 10 bucks, you can send us 10 bucks.
[513.38 --> 514.72]  How do you think that's going to go over?
[514.72 --> 520.62]  I think if you listen to their live stream, they cover this speculation outright and they just say, yeah.
[521.40 --> 537.98]  Why is it OK for open source software to be expected to be free if it's going to be of high quality and a commercial alternative, a genuine commercial alternative to something like Google Photos or iCloud Photos or whatever you use?
[537.98 --> 551.46]  And why should the expectation that the fact that the software is free as in open versus free as in cost, that expectation isn't based in the capitalistic societies that we actually live in?
[551.50 --> 555.74]  I mean, the very fact that we have open source software at all is a minor miracle.
[555.74 --> 559.86]  Why is it not OK to have these people be paid to eat?
[560.00 --> 561.08]  That's how I take it anyway.
[561.46 --> 562.10]  I hope they do.
[562.16 --> 565.54]  And I hope it's pay what you want, because if you ask me, I think image is worth 100 bucks.
[566.16 --> 568.16]  You know, I think every major version could be worth 100 bucks.
[568.24 --> 570.30]  That's what we would have paid back in the day for software like this.
[570.30 --> 572.06]  Well, I actually asked Alex this question directly.
[572.16 --> 574.90]  I said, you know, what is the monetization strategy?
[574.90 --> 580.78]  And he said, yeah, we're probably going to charge a license fee or some kind of a fee, a small amount of money.
[580.78 --> 582.34]  He said, I don't know what that actually means.
[582.44 --> 583.50]  It could be 100 bucks.
[583.54 --> 584.02]  It could be $10.
[584.42 --> 584.94]  Who knows?
[585.74 --> 590.64]  But I think they're going to look at charging some kind of a fee to use image as a one time thing.
[591.16 --> 595.54]  I don't know whether it's going to be a semantic version or like a major version fee.
[595.64 --> 597.94]  Like every time they rev the major version, you pay again.
[598.44 --> 602.50]  To me, that would seem to make the most sense in terms of making the project sustainable.
[602.50 --> 607.98]  And that's certainly what if you look at commercial platforms like iOS apps love to do.
[608.10 --> 609.44]  And Blue Irish does this as well.
[609.50 --> 611.52]  Like every year you pay for updates and stuff.
[611.52 --> 617.24]  I'd certainly pay $30, $40, $50 without even thinking for something like image.
[617.24 --> 623.36]  If it's of as good a quality as it is now or better in a couple of years time, sure.
[623.62 --> 623.76]  Yeah.
[623.76 --> 626.30]  I didn't get the impression of a licensing scheme.
[626.40 --> 630.82]  I got more of an impression that you could go, you know, just do a Docker poll and get it all up and running.
[630.90 --> 633.02]  But if you wanted to go to the website, there'd be a pay button.
[633.66 --> 637.94]  I think that really is the right – it's essentially value for value is what it is.
[638.02 --> 639.06]  They're just not calling it that.
[639.12 --> 641.58]  It's let people show up and contribute the value they think it's worth.
[641.58 --> 645.58]  And, you know, good software, good self-hosted software is worth paying for.
[646.24 --> 651.88]  And I think the model where it's all free, it's all available up like on Docker Hub or GitHub or wherever they want to host it.
[651.94 --> 655.00]  And you can go deploy it and play with it, learn to love it.
[655.38 --> 660.54]  Then it's worth a lot more to you all of a sudden than it was like if you were going to – if you had to pay before you could even try it.
[660.64 --> 660.86]  Yep.
[661.10 --> 661.40]  All right.
[661.46 --> 662.10]  I'll give it $5.
[662.38 --> 662.68]  Okay.
[662.78 --> 663.66]  I've heard good things.
[663.90 --> 665.60]  You know, I heard Alex and Chris talk about this.
[665.64 --> 666.64]  I'll throw $5 at it.
[667.10 --> 668.80]  But now I've used it for more than a year.
[668.80 --> 672.24]  I'm like, yeah, I think things like worth $100 to me, you know, like –
[672.24 --> 673.36]  Yeah, exactly.
[673.62 --> 674.76]  I think it could be a good model.
[675.02 --> 680.92]  Short-term charging for the software, a bit like Ubuntu tried to with their download slider, I think is the goal.
[681.00 --> 684.90]  And then long-term as some kind of a hosted service would seem to be the way to go, yeah.
[685.20 --> 686.18]  Would you consider that?
[686.58 --> 694.86]  You know, like if it was secure, if you were comfortable that it was private, would you consider using an image-hosted service?
[694.86 --> 697.14]  Because then, you know, you're getting things off-site.
[697.14 --> 700.74]  But I'm probably not the target market for that service.
[700.88 --> 704.36]  But I could see people like me buying it for family members.
[704.60 --> 704.98]  Absolutely.
[706.70 --> 708.34]  Yeah, I'm always a little tight on space.
[708.44 --> 712.48]  I've got a maximum of 8 terabyte I'm working with on my home system.
[712.62 --> 712.82]  Right.
[713.06 --> 716.34]  And I could always try to add more solid state.
[716.98 --> 721.96]  Or I try to reduce how much I – so I don't keep like my full media library on there.
[721.96 --> 723.86]  I keep like an abbreviated version of it.
[724.16 --> 726.74]  But I do keep my whole photo library on there.
[727.36 --> 730.18]  And so that's eating up the bulk of the space.
[730.60 --> 735.86]  And I could see myself just saying, I'll just put that all up on the image cloud.
[736.12 --> 737.74]  If, say, I trusted the storage.
[738.20 --> 743.36]  Going back to something that – some other backup method that doesn't eat that storage space on my Odroid.
[743.48 --> 746.74]  I could see myself maybe being a customer just because storage space is tight.
[746.74 --> 748.58]  Or definitely for family members.
[749.56 --> 753.96]  And if the storage plans were reasonable and secure, I'd probably pay a fee for that.
[754.40 --> 756.60]  Would you pay as much as Google or iCloud charge?
[756.88 --> 761.48]  That's trickier because in theory you're getting a lot more for that cloud membership, right?
[761.50 --> 762.42]  There's a lot of other services.
[763.04 --> 766.10]  I mean iCloud for 2 terabytes is $10 a month.
[766.48 --> 766.66]  Yeah.
[767.02 --> 770.10]  I just don't think 2 terabytes would quite cut it for me.
[770.26 --> 770.40]  Yeah.
[770.78 --> 774.74]  And it seems tricky because they can't really do a lot of mass deduplication.
[774.74 --> 777.54]  So they're really – it's probably a high storage cost.
[777.94 --> 781.50]  Well, particularly if they're encrypting it in any kind of meaningful way, yeah.
[781.74 --> 782.84]  They can't do any really.
[783.72 --> 789.88]  I also understand that this is going to allow the image team to accelerate plans for a stable release on their roadmap.
[790.48 --> 792.34]  Oh, ha, ha, ha, ha, ha, ha.
[793.16 --> 794.30]  That's great news.
[794.86 --> 796.38]  Yeah, I'm all for that.
[796.50 --> 802.90]  I think too that getting the software kind of nailed down, you would think like if you want to make a cloud service out of this,
[802.90 --> 808.66]  even the next couple of years, going to want to get to a stable version and then begin optimizing the back end for that
[808.66 --> 812.12]  because you're going to have to run this thing at scale so you better start fixing some of these problems.
[812.24 --> 812.46]  Right.
[812.84 --> 813.02]  Yeah.
[813.14 --> 817.82]  So I could see sort of a business driver need for that but also just the user base probably really appreciate.
[817.82 --> 825.32]  I think the other thing that Futo is going to give them is the runway to hire people who have done that kind of mass service build out before,
[825.72 --> 832.54]  access to the correct developers that have the right cloud experience and caching and scaling things.
[832.78 --> 839.70]  You know, it's not a simple ask to just take what should be a system that runs on your local server
[839.70 --> 842.34]  and put it in the cloud and open it up to tens of thousands of people.
[842.34 --> 852.32]  There's going to be some pain as they do that and I think one of the things that I'm sort of hearing from Alex is that that's going to be possible now with this collaboration with Futo.
[852.90 --> 855.90]  I think calling it a collaboration is fairly reasonable too.
[856.08 --> 866.18]  I mean, so far we've been given no reason other than just general tinfoil hatness to think that Futo is anything other than altruistic.
[866.18 --> 875.34]  They have a pretty long live stream that you can find on YouTube and they go into some of their motivations there and I watch that and I buy it.
[875.76 --> 882.58]  I mean, I think the main guy behind this seems like he's got big ambitions and has seen a few things.
[882.72 --> 889.84]  He also worked at Yahoo in the Yahoo Gaming area and he has seen a few cycles and he's made all the money he needs to make
[889.84 --> 894.94]  and he's got enough that he can set aside to kind of fund this thing for multiple years before it even begins to pay for itself.
[894.94 --> 899.54]  I mean, I'd like to think if I was a billionaire, that's something I'd do.
[899.62 --> 900.14]  I don't know though.
[900.74 --> 902.24]  Desert Island sounds pretty appealing.
[902.56 --> 908.62]  Yeah, well, after you get your Desert Island and your jet and, you know, your condo and every major city that you enjoy,
[908.78 --> 912.10]  then you set aside a few bill to fund your favorite open source projects.
[912.54 --> 913.48]  You might, you just might.
[913.64 --> 914.02]  Absolutely.
[914.02 --> 920.70]  Now, another thing that popped up in this whole news cycle was Greyjay, which is an app from Lewis Rossman,
[920.90 --> 929.00]  who is involved with Futo opening some kind of a, it's almost like a maker space, like a repair space for the community in Austin.
[929.36 --> 933.66]  And Lewis, as you know, is big into Right to Repair and all that kind of stuff.
[934.08 --> 942.42]  And Greyjay is basically a way of following individual creators that transcends a specific platform.
[942.42 --> 952.14]  And the example I think that Lewis gave when he launched the app was Eli the Computer Guy on YouTube still uploads videos to other platforms,
[952.30 --> 958.04]  but because he was deplatformed by YouTube, lost a bunch of people and people don't know where to find him anymore.
[958.14 --> 960.52]  And I think Greyjay tries to solve that.
[961.26 --> 967.70]  Now, one of the problems that they ran into was that people accused them of not understanding what open source meant.
[967.70 --> 976.92]  And the reason why was because Greyjay was released with a license that prohibited commercial redistribution, as I understand it,
[977.34 --> 985.96]  because they wanted to try and make sure that there weren't a bunch of grey market clones of Greyjay appearing in Google Play and app stores and stuff like that
[985.96 --> 989.70]  to circumvent some of the stuff they were trying to protect against.
[989.70 --> 997.76]  And I don't know, like, I feel like the people who are saying that Futo simply doesn't understand open source licensing are a little wide of the mark.
[998.18 --> 1002.12]  But it's just something to be aware of that they've got some skin in this game already.
[1002.56 --> 1008.10]  Yeah, I guess I should have been paying attention a little bit before now, but I'm definitely paying attention at this point.
[1008.78 --> 1011.40]  I'm wondering now what other projects they're going to go after.
[1011.40 --> 1015.86]  I mean, you look at they've got a video project with Greyjay.
[1016.06 --> 1029.02]  They've got another photo sharing feed thing called Circles, which maybe it's a little bit like Facebook slash Instagram, a little bit like it's it's photo related.
[1029.56 --> 1039.04]  But they say it's built with the security model of Signal in mind and a bunch of other stuff to do with like voice inputs and other privacy respecting things.
[1039.04 --> 1044.18]  So it's going to be fascinating to see what Futo does in the next one, two, three years.
[1045.68 --> 1053.78]  About eight months ago, I set out to answer the question, what is the perfect media server CPU, if such a thing could possibly exist?
[1054.52 --> 1064.90]  And I wrote a benchmark script in conjunction with my good friend Morgan to find out, because as you probably know from listening to the show, I'm a bit of a fanboy when it comes to Intel's quick sync technology.
[1064.90 --> 1078.68]  This is a piece of hardware circuitry that's built into pretty much every Intel graphics card, iGPU that's built into your CPU since 2014, 15 sort of era.
[1078.76 --> 1080.38]  So it's been around for a long time.
[1080.38 --> 1094.84]  But what's particularly interesting in a media server context is that this hardware transcoding uses five to 10 watts to transcode multiple 4K streams faster than you can do it in software.
[1094.84 --> 1112.10]  And so what I wanted to do was figure out what is the difference between, let's say, a 7th or 8th gen Intel processor and some of the more modern 12th, 13th, 14th gen processors compared to the super low power N100 type stuff.
[1112.72 --> 1113.64]  And so that's what we've done.
[1114.30 --> 1114.34]  Okay.
[1114.70 --> 1120.32]  Kind of looking for maybe the best performance to price to power usage sweet spot.
[1120.54 --> 1120.80]  Yeah.
[1120.94 --> 1123.06]  Proper it depends answer coming up.
[1123.06 --> 1123.80]  So be warned.
[1123.80 --> 1124.56]  Okay.
[1124.96 --> 1126.62]  Reddit didn't like it at the weekend.
[1127.08 --> 1133.62]  There was one particular guy that decided to reply to my Reddit thread with, conclusion, well, it depends.
[1133.76 --> 1135.92]  And he goes, well, what was the point in the entire test then?
[1135.96 --> 1137.86]  I'm like, well, did you even read the article, dude?
[1138.26 --> 1139.12]  No, probably not.
[1139.68 --> 1149.88]  So the conclusion, we'll jump straight to that, is that you might find that this month an 11th gen Intel CPU and motherboard combo is the best one you can find on eBay.
[1149.88 --> 1152.30]  Next month it might be 8th gen.
[1152.36 --> 1159.32]  And the month after it might, you might decide, well, actually I want DDR5 or something like that, in which case you can only go 13th gen or newer.
[1159.32 --> 1163.32]  Or you might say to yourself, well, I don't want to upgrade my motherboard and CPU.
[1163.46 --> 1164.82]  What about Arc GPUs?
[1165.16 --> 1167.20]  So let's get into some of the results.
[1167.20 --> 1173.40]  Now, one of my wonderful contributors to this QuickSync calc repo.
[1173.84 --> 1175.98]  So I mentioned Morgan helped me write the script.
[1176.38 --> 1178.50]  And there was another user called Alissimo.
[1179.04 --> 1180.10]  I hope I got that right.
[1180.10 --> 1185.28]  Alissimo, Alissimo, who shared a wonderful script which helped visualize some of this data.
[1185.60 --> 1190.62]  So make sure you check out the show notes because there'll be a link to the blog post where all of this stuff gets unpacked.
[1190.70 --> 1193.24]  There's graphs in there, charts, all that kind of stuff.
[1193.70 --> 1200.40]  But he wrote a visualization tool in Python which helped kind of give us a pretty good idea of the spread across generations.
[1200.40 --> 1210.52]  So what's interesting about QuickSync, if you look at some of the older chips, so let's take a Skylake chip which is Intel 6th gen.
[1211.22 --> 1215.26]  That has H.264 hardware decoding in it.
[1215.70 --> 1222.24]  But 5th and 4th and 3rd and so on, they don't really have very much in the way of hardware encoding whatsoever.
[1222.50 --> 1225.80]  I mean, they've got some basic MPEG-2 hardware stuff, AVC.
[1225.80 --> 1232.70]  There's a fantastic graphic on Wikipedia, actually, which shows you how over the years they've added new codecs.
[1232.92 --> 1237.28]  And stuff like the 13th gen has AV1 support, for example.
[1237.34 --> 1240.32]  So if you want the most modern codec support, buy a new chip.
[1240.44 --> 1249.26]  Because the downside of it being a hardware encoder is it's a very specialized piece of circuitry, like an ASIC, that can only do one thing.
[1249.76 --> 1251.60]  And it won't do anything else.
[1251.60 --> 1255.60]  You can't add AV1 support in hardware to a chip from five years ago.
[1255.96 --> 1258.12]  Yeah, it's what it ships with is what it's always going to support.
[1258.42 --> 1258.86]  Exactly.
[1259.62 --> 1263.04]  Now, QuickSync is great, as I mentioned, because of its power efficiency.
[1263.32 --> 1270.42]  So, you know, you're doing multiple 4K streams at sort of 5 to 10 watts of power consumption to encode a 4K file.
[1271.12 --> 1279.54]  Sometimes at more than 1x speed with some of the 10-bit HEVC files, the H.265 stuff, which is almost unheard of, to be honest.
[1280.22 --> 1283.32]  But let's jump into some of the results specifically.
[1283.32 --> 1288.16]  So if we want to look at, say, there's a chart in the blog post linked, as I mentioned.
[1288.56 --> 1298.28]  If we want to compare, say, an Intel i5-8500, which just happens to be the CPU that's been in my primary media server for the last three, four years, something like that,
[1298.28 --> 1309.26]  to an Intel 13th gen, so an i5-13600K, which also just so happens to be the CPU I've just thrown into my primary media server downstairs in the last couple of weeks,
[1309.26 --> 1314.12]  you would think there would be an absolutely enormous difference between these chips.
[1314.40 --> 1317.72]  An i5-8500 was released in 2018.
[1318.52 --> 1320.66]  A 13th gen was released last year.
[1320.80 --> 1321.96]  So what's that, four years?
[1322.50 --> 1326.52]  Four, yeah, four years, five years, six years even, of CPU progress.
[1326.52 --> 1336.62]  So you would think that transcoding something like a 1080p file, an H.264 1080p file, would be orders of magnitude different, wouldn't you?
[1336.88 --> 1337.16]  Sure.
[1337.54 --> 1340.74]  Well, when it comes to CPU encodes, that is the case.
[1340.90 --> 1348.28]  So with a 13th gen, you're looking at about 30 seconds to encode this specific file that I include as part of the benchmark.
[1348.96 --> 1352.02]  And with the 8th gen, it's about 60 seconds.
[1352.02 --> 1359.46]  So the grunt of the software encode, so there's no hardware encoding involved, the new CPUs are a lot faster,
[1359.72 --> 1363.84]  and they use about the same amount of energy to encode that file as well as they do it.
[1364.12 --> 1366.72]  So if you're doing software encodes, well, it's a no-brainer.
[1366.88 --> 1375.90]  But if we jump straight into the hardware H.264 1080p encode, this thing, it maybe has a two-second difference.
[1375.90 --> 1385.64]  They haven't touched the H.264 encoders whatsoever since 2018, is what we can extrapolate from that.
[1385.86 --> 1387.14]  They got it working? Good enough.
[1387.44 --> 1387.88]  Exactly.
[1388.78 --> 1391.00]  I mean, things are a little bit different when you get to 4K.
[1391.12 --> 1394.30]  The gap goes from being one or two seconds to being five or six seconds.
[1394.80 --> 1399.62]  But it's still, in H.264 land, it doesn't matter what CPU you get.
[1399.70 --> 1402.96]  As long as it's 7th or 8th gen or newer, the performance is the same.
[1402.96 --> 1406.36]  Even despite the fact that they have completely different graphics chips.
[1406.54 --> 1414.52]  So the 8th gen has HD630 graphics, whereas the 13th has UHD770 with different clock speeds and all the rest of it.
[1414.62 --> 1419.84]  But as we discussed, the hardware circuitry is set in stone when it leaves the factory.
[1420.62 --> 1424.88]  And it looks like the H.264 circuit has been set in stone since 2018.
[1425.60 --> 1428.96]  Now, let's jump into H.265 territory, HEVC.
[1428.96 --> 1435.78]  You would think, again, that there would be a huge gulf between the 8th and 13th gen chips.
[1435.88 --> 1437.30]  But it's just not the case.
[1437.74 --> 1444.12]  So the 8th gen CPU takes about 45 seconds to encode the H.265 file in 8-bit.
[1444.66 --> 1451.98]  Whereas the 13th gen took 40 seconds, 39 seconds, I think, was the average result in the tests.
[1452.48 --> 1456.98]  Things do get a little different, though, when you jump up to the 10-bit 4K file.
[1456.98 --> 1460.50]  This is the file that really sorts the men from the boys.
[1460.62 --> 1463.16]  This is the one that makes everything come to its knees.
[1463.88 --> 1469.12]  Now, the 8th gen CPU takes nearly 180 seconds to encode this file.
[1469.50 --> 1477.48]  Whereas the 13th gen takes 130 seconds or so, just a little bit over two minutes versus nearly three minutes with the other chip.
[1477.48 --> 1484.64]  So there is a big difference with specifically 4K 10-bit H.265 files.
[1485.08 --> 1488.84]  But in every other test that I ran, it didn't really matter.
[1489.56 --> 1497.68]  Again, so if you're doing really the latest, like we're talking H.265 4K 10-bit video, then it's going to make a difference if you're doing a lot of that.
[1497.68 --> 1501.94]  But outside of that, these encoders are basically pretty much set in stone.
[1502.20 --> 1512.32]  And kind of to your earlier conclusion, it would make sense that the most latest codec with the most latest video technology, that's going to have the best support in the most latest CPU.
[1512.48 --> 1518.42]  But once they, in theory, nail H.265 4K, probably not going to change much for quite a while.
[1518.42 --> 1521.96]  No. You know, these platforms are quite different.
[1522.46 --> 1525.44]  The 13th gen supports PCIe Gen 5.
[1525.56 --> 1530.64]  It has DDR5 memory, which is a lot faster than DDR4 of the 8th gen chips.
[1531.18 --> 1538.64]  And I'm deliberately comparing these 8th versus the 13th because everything in between is sort of a sliding scale, just to give you all an idea.
[1539.44 --> 1542.48]  You would think that the speed of the memory in the system would make...
[1542.48 --> 1543.92]  Yeah, just more I.O. bandwidth.
[1544.04 --> 1545.26]  Yeah, more of a difference.
[1545.26 --> 1550.76]  It's like maybe there's more, you know, L2, L3, I don't know, cash on the chip or something that makes it different.
[1550.88 --> 1552.38]  But no, it doesn't seem to matter.
[1552.66 --> 1555.72]  It's like these little encoder accelerator chips are just little factories.
[1556.10 --> 1557.96]  And the factory staff remain the same.
[1558.08 --> 1559.58]  And the capacity remains the same.
[1559.76 --> 1561.50]  And the world goes on around them.
[1561.84 --> 1568.90]  Now, of course, most of us are running these sorts of chips in an environment where we're doing things like a bunch of containers.
[1569.26 --> 1571.84]  We're doing a bunch of VMs, maybe, on these systems.
[1571.84 --> 1576.76]  That's where you'll start to notice more pep in the system with a newer chip and stuff like that.
[1576.76 --> 1583.40]  Again, down to the things like more modern memory bandwidth and more M.2 lanes and all that kind of stuff.
[1583.40 --> 1591.22]  But if all you're doing is a bog standard, super simple media server that's just serving a few files for Jellyfin with the odd transcode here or there,
[1591.60 --> 1596.32]  I don't see any reason to go for anything other than sort of 7th, 8th, 8th gen, to be honest with you.
[1596.32 --> 1600.30]  Now, we do need to talk a little bit about Intel Arc whilst we're here.
[1600.52 --> 1609.64]  Because I was lucky enough, one of the podcast listeners, I am Spartacus, he goes by, sold me an Arc Pro A40 GPU.
[1609.86 --> 1611.16]  It's an OEM-only card.
[1611.22 --> 1613.20]  You can't buy it on the market, so to speak.
[1613.28 --> 1616.10]  It's sort of a system integrators-only card.
[1616.42 --> 1618.14]  This thing is an absolute monster.
[1618.66 --> 1623.86]  So you remember how I said the 8th gen chip took nearly 180 seconds to encode that 10-bit 4K file?
[1623.86 --> 1624.26]  Yeah.
[1624.48 --> 1626.86]  This thing took about 38 seconds.
[1627.30 --> 1630.08]  Oh, that's encouraging.
[1630.96 --> 1637.62]  Now, we've got to temper your excitement a little bit because it used 65 watts whilst it did it, not 5 to 10 watts.
[1637.72 --> 1638.64]  Oh, right, of course.
[1639.22 --> 1639.80]  Right, of course.
[1639.94 --> 1640.54]  But-
[1640.54 --> 1642.74]  Well, it just depends on what you're optimizing for, I suppose.
[1642.84 --> 1643.62]  Yeah, exactly.
[1643.70 --> 1645.12]  It's like when you're running in the rain.
[1645.20 --> 1647.44]  Do you get wetter when you run in the rain or walk in the rain?
[1647.44 --> 1659.42]  If I'm running a task for 38 seconds instead of 3 minutes, am I cumulatively using more energy, even though it's six times the amount of energy being used or less?
[1659.80 --> 1665.86]  Is it better to have that heat dumped into the box in one short burst or have it spread out over 3 minutes?
[1666.18 --> 1667.92]  Really, only you can answer that question.
[1668.50 --> 1671.46]  I just thought it was really interesting to have an Arc card to be able to test.
[1671.46 --> 1683.08]  It was also pretty interesting as well because the HL15 that 45Drive sent me a few months ago had what I can only describe as a potato CPU, and it had the Xeon Bronze chip.
[1683.18 --> 1688.96]  The model number escapes me, but it was like a 2.2 gigahertz 2018 sort of chip.
[1689.00 --> 1689.82]  It was not fast.
[1689.92 --> 1691.28]  It didn't have very many cores.
[1691.84 --> 1697.52]  So with that Xeon Bronze 3204 CPU, which ran at 1.9 gigahertz, I must correct myself,
[1697.52 --> 1704.80]  the Arc Pro ran at, it took 140 seconds to do that 4K 10-bit encode.
[1705.12 --> 1711.26]  When I threw the Arc Pro into my Epic 7402 build that I did recently, that dropped to 39 seconds.
[1711.58 --> 1715.74]  So 101 seconds quicker just because of the CPU.
[1716.48 --> 1716.66]  Yeah.
[1717.20 --> 1717.60]  Wow.
[1718.26 --> 1719.40]  So it does make a big difference.
[1719.82 --> 1725.86]  Yeah, and I could see if you're in a situation where you get your hands on an Arc GPU and you don't mind the power use,
[1725.86 --> 1734.22]  it's still cheaper as far as, I guess, energy usage than probably like systems that we were building 5, 10 years ago
[1734.22 --> 1737.80]  that were probably pulling 500, 600 watts from the wall continuously.
[1738.54 --> 1738.86]  Easy.
[1739.02 --> 1743.38]  So in the grand scheme of things, 60 watts isn't horrible compared to what we used to do,
[1743.46 --> 1747.16]  especially if your workload is enough where something like that would actually be beneficial.
[1747.56 --> 1752.14]  What I would love to do is pull in some experts to get NV, Inc. benchmarked in there,
[1752.18 --> 1755.30]  as well as some of the AMD APUs that exist as well.
[1755.30 --> 1761.24]  So if that floats your boat, again, there'll be a link in the show notes to the repo where you can contribute
[1761.24 --> 1764.82]  to the little bit janky bash script that Morgan and I threw together.
[1766.98 --> 1769.12]  Unraid.net slash self-hosted.
[1769.20 --> 1769.96]  Go check it out.
[1770.44 --> 1772.46]  Unraid is powerful and flexible.
[1772.76 --> 1777.80]  From a local file storage system, maybe a gaming rig, content creation, and everything in between,
[1778.50 --> 1782.74]  Unraid allows you to get the most out of your home lab and self-host all your important data
[1782.74 --> 1784.52]  and your important services.
[1785.12 --> 1789.94]  It's a network-attached operating system that lets you mix and match.
[1790.16 --> 1791.74]  You got a closet full of old drives?
[1791.92 --> 1793.00]  Say no more, my friend.
[1793.26 --> 1797.24]  You can take those, mix and match those drives, and securely store and share your data,
[1797.44 --> 1802.50]  manage your VMs and your Docker applications, all from one nice web-based interface.
[1802.50 --> 1810.26]  One of the features we love is Unraid lets you easily pass through a graphics card to enable gaming or accelerated VM or container.
[1810.40 --> 1812.00]  Maybe you want a video edit on your Unraid.
[1812.28 --> 1813.54]  It is that flexible.
[1814.10 --> 1822.92]  And Unraid's UI is so simple that managing an entire stack of Docker containers is simple, straightforward, and easy to figure out.
[1822.92 --> 1827.84]  And they have new applications from hundreds of user-created templates in the community app section all the time,
[1827.92 --> 1829.22]  something you should always be checking out.
[1829.50 --> 1832.56]  It makes it really easy to tuck and roll, depending on your expertise level,
[1832.56 --> 1836.36]  from total beginner to expert who wants the most from their system.
[1836.70 --> 1839.50]  It's a powerful, user-friendly operating system for home servers.
[1839.90 --> 1843.34]  Go build the perfect storage solution with the hardware you already have.
[1843.68 --> 1844.74]  Use Unraid OS.
[1845.12 --> 1849.06]  Just support the show by going to unraid.net slash self-hosted.
[1849.06 --> 1857.38]  That's unraid.net slash self-hosted, and go check out Unraid, a powerful, easy-to-use operating system for servers, for storage, and for your applications.
[1857.74 --> 1860.42]  Maximize your hardware with unmatched flexibility.
[1860.80 --> 1863.98]  And go say goodbye to that closet full of mismatched drives.
[1864.04 --> 1864.70]  We've all got it.
[1865.26 --> 1867.60]  No shame, but Unraid is the solution.
[1868.20 --> 1869.74]  Check it out and support the show.
[1870.04 --> 1872.50]  Go to unraid.net slash self-hosted.
[1872.50 --> 1881.04]  So if we're okay accepting that anything newer than a sort of a 7th or 8th gen CPU is the future,
[1881.64 --> 1883.72]  for media servers specifically,
[1884.30 --> 1886.94]  we've got to look at the rest of the ecosystem around the chips,
[1887.00 --> 1888.44]  because it's all very well and good saying,
[1888.44 --> 1893.26]  yes, I can buy an 8th gen i5-8500 for $60 on eBay,
[1893.46 --> 1895.34]  but it's no good if you can't find a motherboard.
[1896.24 --> 1899.14]  And these chips are not spring chickens,
[1899.14 --> 1902.82]  and by extension that means the motherboards have gone the same way too.
[1902.96 --> 1908.18]  So it can be quite tricky to piece together an entire system.
[1908.36 --> 1911.64]  So you've got to find, I mean, DDR4 RAM, I mean, that's been around for a decade,
[1912.34 --> 1915.72]  and its performance characteristics are pretty well understood at this point.
[1916.04 --> 1917.26]  So that's not really a concern.
[1917.38 --> 1920.96]  DDR4 memory is, you know, a commodity at this point, and it's cheap.
[1921.82 --> 1925.32]  DDR5 is about twice the price still, which is unfortunate.
[1925.32 --> 1928.24]  But let's say you want to find an 8th gen motherboard.
[1928.76 --> 1932.26]  You can find a lot of used, like, gaming-grade motherboards,
[1932.46 --> 1934.50]  and for some people that's totally fine.
[1934.90 --> 1938.50]  Pair that with a Pi KVM, and you get all pretty much the same features
[1938.50 --> 1941.88]  as a built-in BMC chip would give you on a, you know,
[1941.92 --> 1945.40]  a more server-grade motherboard, for want of a better word.
[1945.60 --> 1947.76]  But the trouble is, those server-grade boards,
[1948.18 --> 1952.34]  the BMC integration, for the most part, is just that little bit more reliable.
[1952.34 --> 1956.32]  And for me, as you well know, I've got my backup server in the UK
[1956.32 --> 1957.38]  on the other side of the ocean.
[1957.62 --> 1961.68]  I can't deal with anything other than perfect reliability on that box, really.
[1962.32 --> 1964.52]  And the IPMI has bailed me out a couple of times
[1964.52 --> 1967.92]  after, like, power outages in the remote country and stuff like that.
[1968.00 --> 1971.02]  So as much as I love advocating for Pi KVMs
[1971.02 --> 1974.48]  when you can go down to your basement and physically touch the box
[1974.48 --> 1976.12]  and finagle it back to life again,
[1976.58 --> 1980.42]  when it's a remote deployment or you don't have easy access to be hands-on,
[1980.42 --> 1983.00]  I'll still advocate for the BMC stuff.
[1983.06 --> 1984.96]  And that's where things start to get a little bit more tricky.
[1985.22 --> 1989.94]  So to give you an example, the LGA 1151 socket,
[1990.16 --> 1992.46]  which is the one that the 8th-gen Intel CPUs use,
[1992.94 --> 1994.64]  if you want to find a motherboard with BMC,
[1994.70 --> 1998.28]  the cheapest I could find was sort of in that $200 to $300 range on eBay,
[1999.16 --> 2002.64]  which, you know, some of the advantages of a cheap CPU
[2002.64 --> 2004.22]  start to evaporate at that point.
[2004.22 --> 2008.72]  Yeah, although, you know, if you factor in the cost of Pi KVM,
[2008.80 --> 2011.18]  which is probably about $100 and something, it's not so bad.
[2011.38 --> 2012.90]  You know, you start to think about it.
[2012.94 --> 2015.26]  If you were going to put a Pi KVM on there, it's $120.
[2016.08 --> 2016.72]  That's true.
[2016.92 --> 2018.40]  Yeah, actually, I hadn't considered that.
[2018.48 --> 2021.90]  Because, I mean, in my mind, the Pi KVM is a sunk cost,
[2021.98 --> 2023.68]  but that's not fair to assume that at all, is it?
[2023.68 --> 2026.38]  Because you might be buying a new one for this.
[2026.44 --> 2026.68]  Right.
[2026.78 --> 2027.72]  Yeah, that's a good point.
[2027.94 --> 2029.92]  I am a big fan of Pi KVM.
[2029.92 --> 2034.58]  I have used it, you know, remotely in anger and been, you know, perfectly happy with it.
[2034.66 --> 2037.80]  But I also agree that if you can have built-in management tools as well,
[2038.28 --> 2041.48]  in a situation where it really matters, you're going to be a lot better off.
[2042.00 --> 2045.30]  Although, you know, I wonder, what about, okay, Alex, just going down this route,
[2045.36 --> 2046.78]  what about having, like, two machines?
[2047.14 --> 2051.82]  And one of them is just like a little one-liter PC that's a remote box that you can do support from.
[2051.94 --> 2052.54]  Great question.
[2053.10 --> 2054.26]  Well, I covered a little bit.
[2054.32 --> 2058.18]  There were some test results that came in with the N100 chip, which is a...
[2058.18 --> 2058.34]  Yeah.
[2058.34 --> 2062.90]  It's basically the efficiency cores of an Intel 12th Gen only.
[2063.76 --> 2067.38]  So for those of you that aren't familiar, Intel in the, I think it was 12th Gen,
[2067.44 --> 2069.90]  introduced their new P and E core architecture.
[2070.44 --> 2073.42]  And they released this really interesting chip called the N100.
[2073.74 --> 2076.34]  There's also a slightly bigger brother called the N305,
[2076.56 --> 2079.50]  which is just a slightly beefier version,
[2079.96 --> 2082.84]  as being like the ultimate conclusion of their Atom series.
[2083.42 --> 2086.88]  So this thing, the N100 sips, absolutely sips power.
[2086.88 --> 2092.30]  It uses about six watts idle for the entire system, which is quite something.
[2092.58 --> 2096.92]  The downside is, of course, it's a bit of a potato when it comes to doing anything processor intensive.
[2097.72 --> 2102.64]  So you start thinking to yourself, well, why don't I look at these small form factor PCs,
[2103.24 --> 2106.74]  ignoring the fact that N100 motherboards are difficult to get hold of,
[2106.82 --> 2108.42]  often don't have enough SATA ports,
[2108.42 --> 2113.48]  and sometimes you end up having to do weird stuff to get things like 10 gig on them and stuff like that,
[2113.52 --> 2116.62]  because they just don't have enough PCIe lanes to be useful.
[2116.74 --> 2120.86]  I think they have about nine lanes to go around the entire system, which just isn't enough.
[2120.86 --> 2123.72]  So you think to yourself, well, why don't I use a small form factor PC,
[2123.84 --> 2126.22]  like some of those Dell ones that you talk about all the time, Alex?
[2126.22 --> 2127.94]  And it's a great point.
[2128.32 --> 2132.42]  If you have a big honking storage box that you're happy with,
[2133.02 --> 2136.50]  you'll probably be in the red for quite a long time.
[2136.90 --> 2140.10]  Energy efficiency wise, you know, if you want to buy a new system,
[2140.38 --> 2144.80]  it's hard to justify the ROI on buying a new system versus,
[2145.70 --> 2149.36]  you know, you look at some of the sales that Dell has on these boxes.
[2149.36 --> 2153.94]  An i5 6600T box I picked up for $138.
[2154.50 --> 2154.78]  Wow.
[2154.84 --> 2157.88]  With 8 gigs of RAM and 128 gig SSD, for example.
[2158.32 --> 2159.94]  Hmm. That's not bad.
[2160.06 --> 2160.82]  And they have QuickSync.
[2161.56 --> 2162.90]  Yeah. A little QuickSync box.
[2163.12 --> 2167.00]  These T processors, I never really liked them.
[2167.40 --> 2169.16]  A lot of people go, oh, but they're low power.
[2169.58 --> 2170.56]  They're not low power.
[2170.66 --> 2172.76]  They're just capped at a certain TDP.
[2173.20 --> 2179.30]  So at the lower end, you've got all the same grunt for the most part as a desktop class,
[2179.36 --> 2181.14]  chip without the T designation.
[2181.76 --> 2184.82]  But all T does is it just cuts it off at the kneecaps.
[2184.96 --> 2186.98]  And it says, ha ha, you can't go any further than this.
[2187.36 --> 2188.84]  The T stands for cap TDP.
[2189.08 --> 2190.18]  Is that what it stands for?
[2190.56 --> 2192.92]  T stands for totally annoying.
[2193.64 --> 2196.04]  Because they're often more expensive to buy.
[2196.22 --> 2197.76]  Because they're more desirable.
[2197.76 --> 2199.94]  Because people think they're a low power chip.
[2200.32 --> 2202.46]  Even though at idle, they're exactly the same.
[2203.10 --> 2205.32]  These small form factor builds, they make sense.
[2205.32 --> 2208.94]  Because there's only so much heat you can get out of a little one liter box, for example.
[2209.36 --> 2215.00]  But if people are buying them to put in a full-size chassis with a proper cooler situation and stuff,
[2215.14 --> 2217.26]  I've never really understood the benefit.
[2218.04 --> 2219.28]  Yeah, I guess that makes sense.
[2219.76 --> 2221.20]  I could see that as a line.
[2221.68 --> 2226.72]  I do think, too, at that price, though, you could almost afford to have a backup one in a drawer.
[2226.96 --> 2229.44]  And then you could throw these things in just the worst conditions.
[2229.68 --> 2229.96]  Yeah.
[2229.96 --> 2235.26]  And if they burn themselves out, you just pull it out and pop in the replacement that's in the drawer.
[2235.34 --> 2236.80]  It's kind of the Raspberry Pi strategy.
[2236.88 --> 2239.76]  I was going to say, you said the same thing about a Raspberry Pi five years ago.
[2240.26 --> 2240.50]  Yeah.
[2240.64 --> 2241.94]  I mean, I think that's where we're at now.
[2242.90 --> 2245.36]  That's assuming, though, that you have storage somewhere else, I suppose.
[2246.40 --> 2246.76]  Yeah.
[2246.96 --> 2250.46]  I mean, you can get an 8-terabyte, 2.5-inch SSD if you want.
[2251.02 --> 2252.88]  I mean, that's a lot of Rick and Morty right there.
[2252.88 --> 2258.48]  That's what I do in my little home Odroid setup, right, is I'm hanging an 8-terabyte SSD off the thing.
[2258.96 --> 2268.58]  Or I think it was Jeff Geerling this week just highlighted that you can get these carrier boards now for the Raspberry Pi 5 that have four M.2 slots on them.
[2269.12 --> 2273.10]  There's a bunch of other small, low-powered NAS boxes that are flash-only.
[2274.28 --> 2282.48]  And since the last time we had a discussion like this, the landscape has changed in terms of flash prices versus spinning rust.
[2282.48 --> 2292.30]  Like, yes, 20-terabyte drives exist now, but so do 4-terabyte M.2 drives at a reasonable price if you can wait for a sale, you know.
[2292.40 --> 2295.00]  So where does this leave us, Chris?
[2296.02 --> 2301.78]  Well, I'll tell you what I like about the Intel stuff, either the QuickSync or using the ARC card.
[2302.30 --> 2310.28]  I guess unless I'm wrong, it seems like it's probably a little simpler than any of the other GPU vendors because it's all just really built into Linux now.
[2310.46 --> 2310.68]  Yeah.
[2310.68 --> 2312.70]  Maybe with the AMD exception.
[2312.94 --> 2322.98]  But I would imagine you're just passing a device path through in a Docker Compose that points to, like, the DRI device or something, and then the applications in the container just see that?
[2323.10 --> 2326.06]  Is that how it works from, like, a practical standpoint to use the ARC video card?
[2326.48 --> 2327.32]  Yeah, same thing.
[2327.42 --> 2338.84]  So the QuickSync stuff built into the CPU shows up as slash dev slash DRI slash render D128, and the ARC GPU shows up as D129.
[2338.84 --> 2340.58]  Ah, okay.
[2340.94 --> 2346.26]  And then so you could just map that to the device in the container or maybe just pass them all through, I suppose.
[2346.52 --> 2346.84]  Absolutely.
[2347.44 --> 2349.54]  And then you could use – could you use both simultaneously?
[2350.36 --> 2351.70]  I haven't tried that.
[2352.08 --> 2353.18]  I imagine it would be fine.
[2353.18 --> 2359.02]  But it would be up to the app, I suppose, to have some way of scheduling those jobs on different places.
[2359.44 --> 2359.58]  Yeah.
[2359.94 --> 2360.12]  Yeah.
[2360.24 --> 2361.20]  That would probably be the trick.
[2361.28 --> 2380.18]  What would be ideal – and this would go for a small form factor like farm – would be if something like Jellyfin – I know this kind of exists for Plex, although I never got it working – was some kind of, like, Kubernetes-based transcoding remote worker situation.
[2380.18 --> 2387.66]  So you could spin up pods, for example, and have Jellyfin point at those pods to do processing.
[2387.76 --> 2391.28]  A little bit like we talked about in the last episode with image and the machine learning stuff.
[2391.70 --> 2395.68]  If you could point at a remote endpoint and say, here is your compute.
[2395.80 --> 2397.32]  Go load balance yourself.
[2397.88 --> 2399.12]  Maybe that would be a way to do it.
[2399.12 --> 2408.78]  That really should be the way – that is the solution to getting, like, on-premises LLMs that can work at scale and things like that.
[2408.84 --> 2417.90]  If you could somehow have – sort of, like, take the Wyoming protocol that Home Assistant has created for voice assistants to be able to remotely communicate with processing endpoints.
[2417.90 --> 2434.28]  If you could extend that to all sort of jobs of that, like, encode jobs or compute jobs that could be approachable by folks like us, that maybe you just run an application in a Docker container that points at a hardware device and has a listening port.
[2434.94 --> 2439.02]  And then, you know, they use some sort of auto-discover DNS protocol.
[2439.18 --> 2441.20]  They find each other and you can just submit jobs to it.
[2441.44 --> 2441.96]  Would be nice, huh?
[2441.96 --> 2444.90]  You could see something that really is large at scale.
[2445.36 --> 2448.56]  And it's never going to happen, but you know who could do this is Apple.
[2449.08 --> 2457.56]  Apple could just build this into all their devices with all of their neural processors and you could just run a local LLM that just runs across all your iDevices at once.
[2458.40 --> 2460.78]  They'll never do it, but if anybody could, they could.
[2461.20 --> 2461.58]  Indeed.
[2462.40 --> 2463.72]  Yeah, so there you go, folks.
[2463.72 --> 2469.36]  That is – the perfect media server CPU is up to you, really.
[2469.36 --> 2476.36]  I know that's such a cop-out to not pick one, but it really does depend on what's on eBay this month.
[2476.84 --> 2477.98]  I think you're being too hard on yourself.
[2478.06 --> 2478.56]  I don't know.
[2478.80 --> 2480.42]  Because I think it's actually really good information.
[2480.70 --> 2485.58]  If you start with the 8th gen, you're going to be okay, and anything later, the better.
[2485.86 --> 2486.26]  It's true.
[2486.50 --> 2488.66]  Nothing like this existed publicly for many years.
[2488.66 --> 2496.30]  And I actually pitched this article to Ars Technica sort of three or four years whenever I did that Google Photos thing for them, and they weren't interested.
[2496.48 --> 2498.64]  So it's been on my mind for a very long time, this.
[2499.22 --> 2503.10]  And a huge thanks to the community that offered up their hardware to run these tests.
[2503.18 --> 2508.40]  I haven't counted how many, but it's got to be approaching 100 or so as a sample size.
[2508.40 --> 2513.96]  Feel free to, if you haven't done it already, just download the Git repo.
[2514.12 --> 2514.70]  It runs a script.
[2514.84 --> 2517.74]  It pulls down some stuff from Linode's S3 storage.
[2518.38 --> 2523.54]  It takes about five minutes to run the tests and then submit the results to the GIST.
[2523.98 --> 2531.76]  I have a GitHub action that automatically updates the graphs based on those GIST results every – I think I've set it to run every week.
[2531.76 --> 2536.82]  So by all means, I know I've drawn some conclusions today, but the results, you can just keep them coming.
[2539.60 --> 2541.96]  Tailscale.com slash self-hosted.
[2542.02 --> 2543.94]  Go get 100 devices for free.
[2543.94 --> 2547.26]  I have Tailscale on every single system.
[2547.48 --> 2557.32]  My mobile devices, my set-top boxes, my family's computers, my containers even have individual Tailnet nodes, and I'm still not using all 100 devices.
[2557.88 --> 2564.58]  Tailscale is the easiest way to connect your devices and your services to each other directly wherever they are.
[2564.72 --> 2565.50]  That's the idea.
[2565.66 --> 2570.96]  It's secure remote access to your systems when you need them, even if they don't have the Tailscale client on them.
[2570.96 --> 2572.16]  And it's fast.
[2572.54 --> 2574.24]  Like, really, really fast.
[2574.94 --> 2577.98]  And Android users, today is your day.
[2578.48 --> 2581.28]  Tailscale is relaunching the app for Android.
[2581.40 --> 2586.00]  Redesigned from the ground up for a better look and feel, faster performance, and even more features.
[2586.00 --> 2589.10]  You can find out the details at Tailscale.com slash blog.
[2589.40 --> 2590.66]  That's super nice to see.
[2590.78 --> 2596.50]  I will also give a mention for the Tailscale Apple TV app, which is a game changer.
[2596.70 --> 2607.32]  It's absolutely mind-blowingly awesome to have Tailscale on the Apple TV, even as just like a node on the network, but also then to get access into a private network of content and media that I have.
[2607.64 --> 2611.40]  And when I move that Apple TV physically, it still has the same Tailnet IP.
[2611.84 --> 2613.56]  It can still access the same content.
[2613.56 --> 2615.78]  And it's an extremely powerful idea.
[2616.16 --> 2617.74]  I put everything on my Tailnet now.
[2617.84 --> 2625.32]  So I have no inbound ports on my firewall, and everything can find each other on my Tailnet network, including I even have a DNS server on there.
[2625.42 --> 2628.36]  And I'm pinging and talking to everything by name these days.
[2629.06 --> 2631.40]  It's like my own genuine little internet that I've built.
[2631.40 --> 2638.86]  And it's all protected by WireGuard, zero config, no fuss, machine to machine, talking directly to each other.
[2639.16 --> 2640.46]  And it's perfect in enterprises.
[2640.68 --> 2642.66]  You can cut down that complex infrastructure.
[2643.12 --> 2650.68]  They have ACL policies to securely control access to devices and services with next-gen access controls, a dashboard that now supports dark mode.
[2650.68 --> 2655.94]  And they have all the tooling you'd need to integrate with your existing authentication infrastructure.
[2656.42 --> 2659.70]  So for a home labber, you know, the 100 devices, that might just cover you.
[2659.82 --> 2661.76]  Go to tailscale.com slash self-hosted.
[2662.10 --> 2667.56]  Then if you want to take it to work one day, they have got solutions that make this work and sing in the enterprise.
[2667.56 --> 2672.84]  Simple secure networks for a team or an individual of any size built on top of WireGuard.
[2673.12 --> 2676.30]  Now with a brand new rebuilt Android app.
[2676.72 --> 2684.24]  Try it today, support the show, and get it for free on 100 devices and three users at tailscale.com slash self-hosted.
[2685.72 --> 2688.00]  I thought we weren't into dashboards.
[2688.12 --> 2692.84]  I thought we decided that dashboards were crufty and pointless and old hat.
[2692.98 --> 2693.16]  No?
[2693.86 --> 2696.20]  Definitely not into dashboards, Alex.
[2696.20 --> 2697.34]  Definitely not.
[2697.56 --> 2701.84]  But I have been kind of glancing at this Maffle dashboard.
[2701.96 --> 2703.00]  I don't actually know how you say it.
[2703.08 --> 2704.14]  M-A-F-L.
[2704.92 --> 2709.54]  And it's supposed to be a really simple, you know, a couple of lines of YAML.
[2709.64 --> 2714.88]  You got yourself a dashboard where you can track services, get links to things, keep it all local.
[2715.38 --> 2720.52]  I'm putting this out there because here's what I realized while traveling I would have liked to have had.
[2720.52 --> 2729.32]  I would like to just open up my browser and have a homepage that has, A, links to, I have services on, you know, multiple lands.
[2730.10 --> 2731.70]  Well, just on my tail net.
[2731.70 --> 2734.64]  And I would like to kind of know what things are up or down.
[2734.92 --> 2736.14]  Just red light, green light.
[2736.14 --> 2740.06]  That's all I want is like a logo, red light, green light.
[2740.12 --> 2741.80]  And if I click it, it takes me to the thing.
[2741.96 --> 2747.48]  And maybe I can have sections so I can have it by location, studio, you know, jupes, cloud stuff.
[2747.56 --> 2747.92]  I don't know.
[2747.92 --> 2751.32]  And I think I'm getting close with this.
[2752.00 --> 2755.76]  I'm not looking for something that's going to be like the thing I go share on Reddit with screenshots.
[2755.76 --> 2759.00]  And I don't want it to have like all this crazy information.
[2759.00 --> 2761.24]  I just want something that will load fast.
[2762.02 --> 2763.28]  I can put on my tail net.
[2763.62 --> 2768.04]  And then I kind of get a once overview of everything that is like my, you know, backend stuff.
[2768.72 --> 2772.66]  What about the entropy that we discussed last time we brought up dashboards?
[2772.88 --> 2774.54]  How are you going to keep it up to date?
[2774.98 --> 2775.64]  I don't know.
[2775.64 --> 2779.34]  So this is, I feel like this is where it's always going to fall down.
[2779.70 --> 2787.38]  And I don't know why these, like these dashboards often don't let you edit their config inside the dashboard, which seems like a quick way.
[2787.42 --> 2788.08]  It's like, I'm there.
[2788.60 --> 2791.16]  I'll just go edit this really quick here and save it.
[2791.58 --> 2793.10]  No, no, you got to SSH in.
[2793.18 --> 2793.94]  You got to go to the file.
[2794.04 --> 2795.02]  You know, it's like, come on.
[2795.10 --> 2795.90]  It makes it take forever.
[2795.90 --> 2798.40]  There was a version of another dashboard.
[2798.58 --> 2805.40]  I think it was called Flame that let you do a dashboard like this in a similar way to you did traffic.
[2805.64 --> 2810.46]  So you put labels in your compose file and it generated the dashboard from there.
[2811.22 --> 2817.34]  It kind of made my compose file a bit messy because it needed three or four or five labels per container or something.
[2817.50 --> 2819.30]  But maybe that's the way to do it.
[2819.78 --> 2821.24]  I'd also like to hear what the audience has to say.
[2821.26 --> 2821.78]  Yeah, me too.
[2821.92 --> 2823.66]  Boost in or email in and let us know.
[2824.46 --> 2829.66]  Speaking of a boost, A-A-Ron came in with 100,000 sats.
[2829.74 --> 2830.72]  You're our baller this week.
[2830.78 --> 2831.28]  That's for sure.
[2831.36 --> 2833.24]  Thank you very, very much.
[2833.24 --> 2834.28]  And they wrote,
[2834.44 --> 2839.22]  I just got offered a job that's a big step in my career and I wanted to share the love and say thank you.
[2839.60 --> 2845.26]  This new position will be DevOps engineering and a large part of that DevOps knowledge and interest is because of this podcast.
[2845.88 --> 2850.02]  I wouldn't have found my love of automation if I didn't discover Jupyter Broadcasting from the bottom of my heart.
[2850.30 --> 2850.82]  Thanks, guys.
[2850.82 --> 2853.04]  Well, thank you very much, A-Ron.
[2853.34 --> 2865.30]  You know what's funny about this boost is that I'm pretty sure I sent you, Chris, a very similar email five, six, seven years ago before I was involved with JB saying thank you for all the shows.
[2865.46 --> 2871.42]  So I really appreciate messages like this because it's, you know, paying it forward and it's just nice to hear that.
[2872.14 --> 2877.66]  We heard it from several people at conferences as well and I'm feeling pretty recharged from the audience lately.
[2878.18 --> 2879.30]  So big thanks, guys.
[2879.30 --> 2881.60]  It is one of the nicest messages you can get.
[2882.20 --> 2882.72]  Thank you.
[2882.80 --> 2884.38]  And also congratulations, A-Ron.
[2884.78 --> 2885.04]  Yeah.
[2885.34 --> 2885.92]  That's really great.
[2886.30 --> 2888.24]  Shaft and Spanner came in with 20,000 sats.
[2888.52 --> 2889.32]  Redis has changed.
[2889.38 --> 2889.98]  You like that?
[2890.40 --> 2891.44]  That's a funny name.
[2891.60 --> 2892.28]  It is a good one.
[2892.28 --> 2892.68]  Shaft and Spanner.
[2892.68 --> 2893.20]  I like it too.
[2893.84 --> 2896.02]  Redis changed their license in March, they write.
[2896.18 --> 2901.04]  Home Assistant is now owned by the Open Home Foundation and Image has transferred its ownership to FUTO.
[2901.56 --> 2906.26]  Is this worthy of an episode to discuss ownership, licensing and the long-term survivability of FOSS?
[2906.26 --> 2912.40]  As we discussed about FUTO earlier, they are not touching the license of Image specifically.
[2912.40 --> 2919.78]  So even if they turn out to be bad actors, and as we discussed, we don't necessarily have any reason to believe that they will yet.
[2920.42 --> 2921.52]  The code's going to be fine.
[2921.66 --> 2922.62]  The project's going to be fine.
[2923.00 --> 2928.28]  I think Home Assistant is another good example of it's all fine as far as I can tell right now.
[2928.28 --> 2930.86]  The proof will be in the pudding.
[2931.04 --> 2934.56]  The only juror that we can trust is time here.
[2935.34 --> 2945.00]  But the fact that both of these projects have made these moves, Home Assistant in particular, being the founders of this Open Home Foundation, hats off.
[2945.32 --> 2947.42]  You know, it's big picture thinking.
[2947.62 --> 2952.14]  It's thinking about how do I make these projects sustainable in the long term?
[2952.14 --> 2956.72]  Like, I'm sure Paulus one day will get bored of Home Assistant, hopefully not in the near future.
[2956.72 --> 2959.76]  But one day, like, the guy's going to want to retire or something, I'm sure.
[2960.34 --> 2965.88]  And how do these people make sure that these projects transcend themselves in the long term?
[2966.04 --> 2972.68]  For these projects that are hopefully going to be around for the rest of our lives, like Home Assistant, I think it's really important.
[2972.68 --> 2974.40]  Yeah, plus one to all of that.
[2974.46 --> 2975.12]  I completely agree.
[2975.38 --> 2977.46]  We are obviously keeping our eye on it, though, Shaft.
[2977.52 --> 2982.00]  So if anything does look a little funky or smells a little weird, we'll be on it.
[2982.06 --> 2982.36]  Yeah.
[2982.46 --> 2982.84]  But we're watching.
[2983.00 --> 2987.48]  The Redis situation and the Terraform situation, I think, are different.
[2987.84 --> 2994.96]  Primarily, maybe not Redis, but they're both primarily commercial tools that were built on open source and then were rug pulled.
[2995.28 --> 3001.26]  So I think they are perhaps worthy of a different discussion, but I wouldn't lump them in with Home Assistant and Image, personally.
[3001.26 --> 3003.56]  Simon comes in with 5,500 sats.
[3003.76 --> 3007.06]  I wanted to tell you about another image alternative called Ante.io.
[3007.18 --> 3008.84]  It's E-N-T-E dot I-O.
[3009.46 --> 3012.36]  It's end-to-end encrypted and privacy-preserving photo storage app.
[3012.72 --> 3016.64]  I've been using their hosted servers for quite some time now, and I think it's pretty great.
[3017.06 --> 3020.46]  Their clients have always been open source, and they recently open sourced their server, too.
[3020.70 --> 3021.56]  Greetings from Germany.
[3021.96 --> 3023.56]  They have some pretty nice pricing plans.
[3023.76 --> 3030.86]  So I was speaking with Alex, who is the lead developer of Image, and I know this is on their roadmap for some indeterminate point in the future.
[3030.86 --> 3033.32]  Some hosted version of Image.
[3033.52 --> 3036.02]  That's going to be their business model, I believe, moving forward.
[3036.74 --> 3044.68]  But the Ante stuff, you can buy storage like you would buy iCloud storage, and you don't need to worry about hosting it yourself.
[3044.86 --> 3054.30]  So as long as you trust where this data is living, and I haven't dug into where it lives, I'll be honest, but as long as you trust where it's living, go for it.
[3054.92 --> 3058.38]  WotC comes in with 17,345 sats.
[3058.50 --> 3063.42]  Have you guys thought of self-hosting a Bitwarden instance and then back-ending it with Tailscale so it's available everywhere?
[3064.12 --> 3069.48]  Enterprise licenses are a bit expensive, but you could also do it with six free family accounts with each license.
[3069.48 --> 3078.82]  Yes, I have, and for much the same reason as I don't run Headscale, there are just a couple of things in my infrastructure that are so critical that I can't afford for them to go down.
[3078.90 --> 3085.04]  Like, if my Bitwarden disappeared, I would be... I should probably back that up somehow.
[3085.58 --> 3087.28]  Now I'm talking about it in the episode.
[3087.98 --> 3088.12]  Yeah.
[3088.72 --> 3091.92]  Vaultwarden, I think. Didn't they just rename themselves again to something else?
[3091.92 --> 3096.46]  But yeah, Vaultwarden is the self-hosted version of Bitwarden, and I believe it's a Rust app.
[3096.86 --> 3110.40]  You can absolutely run this thing locally, and I'm sure that many of us listening have the skill set to do it, but it's that what happens when all systems are down moment, and I need that password to get back into everything.
[3110.96 --> 3117.68]  Something, I mean, particularly with Bitwarden only being $10 a year for the hosted service, you know, it's... that's a value trade-off I'm willing to make.
[3117.68 --> 3130.94]  That's where I sit with it mostly as well. I do think I need to probably develop a better practice about backing up and exporting my database, and then maybe having a Vaultwarden instance somewhere on my tail net that I restore into from time to time.
[3131.02 --> 3132.02]  You and me both, I think.
[3132.48 --> 3136.56]  Yeah, I'll give some thought to that. I think it's an interesting... that's an interesting idea.
[3136.78 --> 3143.66]  I wonder if you could do it the other way around. If you could treat the Vaultwarden as the primary, and then Bitwarden as the cold storage, so to speak.
[3143.72 --> 3143.90]  Maybe.
[3144.26 --> 3145.28]  I'd be down for trying that.
[3145.28 --> 3153.40]  It does make it easier with everything just being on tail scale. There's just always, yeah, there's always a lot of layers to think of there. But thank you, Watsi. Appreciate that.
[3154.22 --> 3168.08]  Mascot NR comes in with 2,000 sats. The last show is my first boost, so let's make it two. The NR at the end of my name is a UK postcode, which Alex may recognize as being from Norfolk. Do you recognize that from being from Norfolk there, Alex?
[3168.08 --> 3186.60]  Yes, I do. The postcodes over there, NR16 and NR... I think the one I lived in Norwich was NR2. Was it NR4? Something like that. Anyway, yes, I do. I love Norfolk. That's where I did my master's at UEA, and my wife's from Norwich. A very big soft spot for that part of the world.
[3186.60 --> 3204.28]  Oh. He writes, so a JB meetup in Norwich is something I'm hoping for, and we'll keep an eye on the meetup page. Also, Unraid 100% gave me everything I needed for now with my self-hosted journey, so I'm pleased they're a sponsor. Although I said in my last boost I listen to all the shows, I only understand about 1% of them. It's that upbeat attitude I'm here for.
[3204.28 --> 3234.12]  Yeah, well, I was talking to, I think Joe over on Late Night Linux was talking about doing a meetup in June, which happens to be the sort of time I'm going to be in England, and I was talking with Wimpy and Popey as well about them coming along and trying to do something. I don't know if we'll manage to make the schedules all work with everybody, but I'm considering doing something in Norwich for the folks out east or Cambridge area, because there's a few folks out that way that I talk to quite often, and maybe something in the sort of Reading, Basingstoke,
[3234.28 --> 3253.74]  sort of area, rather than London itself, because I know that we did it in London proper last time. It really depends on where we can find events to do it. It could be small, low-key, just find a Riverside pub. In fact, in Norwich, I know the perfect one, so we'll probably do one in Norwich. And then in the Basingstoke area, I don't know, we'll find something. Keep an eye on the page.
[3254.28 --> 3254.66]  There you go.
[3255.70 --> 3261.86]  MSC0135 comes in with our last boost that's going to make it in the show this week. It's 2,560 sats. They write,
[3261.86 --> 3291.54]  Yes, but probably not...
[3291.86 --> 3300.14]  To the point of, you know, I don't know, like tinfoil hatting this particular solution. There's probably other parts of your life that the NSA are much more interested in.
[3300.36 --> 3301.88]  Yes, like your credit card, your debit card.
[3302.02 --> 3302.34]  Yeah.
[3302.86 --> 3314.82]  Whatever telemetry your car reports. Those things they love. Your phone account. Your service provider is selling them everything. But also, if you're using Matrix, that could be SSL already in there. Home Assistant as well.
[3314.82 --> 3325.96]  What you could do, this is something I've sort of been experimenting about making a video for for work, is run TailScale on a VPS somewhere and run TailScale inside your LAN.
[3325.96 --> 3338.28]  Connect the two together over the TailNet and you run the reverse proxy on the Cloud VPS. And then that way you can publicly expose that to the public internet like you're doing with CloudFlare tunnels.
[3338.28 --> 3347.62]  But you control the TLS, you control the DNS, like you're in charge of everything, including making sure it's secure because it's on the public internet too, of course.
[3347.62 --> 3357.08]  So with CloudFlare, you do get nice stuff like DDoS protection and all the rest of it. But if you want to own the chain more, run it on a VPS.
[3357.58 --> 3360.74]  Thank you very much for the boost. And it's a good question. Let us know what you decided to do, Emacy.
[3361.20 --> 3362.08]  Yeah, I'd love to know.
[3362.22 --> 3377.32]  We had 10 total boosters, so that means there is a couple of boosts in the boost bar that we'll have linked in the show notes. And we stacked 166,831 sats with no middleman, nobody in between, just an open source peer-to-peer protocol sent directly to us to support the show.
[3377.32 --> 3388.30]  If you'd like to send a boost with a message and some value, get a new podcast app at newpodcastapps.com. So many great ones to choose from, GPL, different models for each type, each individual, each type of person.
[3388.38 --> 3396.78]  It's like the distros back in the day where each one really stood out as having its own unique proposition. That's where we're at with the 2.0 apps. Check it out at newpodcastapps.com.
[3397.14 --> 3406.66]  And don't forget self-hosted.show slash SRE if you would prefer to pay in fiat fund coupons. You can support the show over there when you get an ad-free feed along with our post show.
[3406.66 --> 3417.30]  Yeah, a little extra content to say thank you for our members. We really appreciate you. You can find that linked at the website. There's a website, self-hosted.show. Do you know about that? It's got links.
[3417.72 --> 3419.46]  Yeah, it's a pretty cool website, huh?
[3420.00 --> 3422.60]  Yeah, it's easy. Like one spot, you can just link to stuff.
[3422.60 --> 3433.28]  Now, if you'd like to come see your favourite fat bearded Englishman in England, meetup.com slash Jupiter Broadcasting. Keep an eye on that page for all the info regarding meetups.
[3433.56 --> 3436.94]  You can also find me on the internet at alex.ktz.me.
[3437.46 --> 3439.50]  You can find me at chrislas.com.
[3439.94 --> 3444.06]  And until next time, thanks for listening. That was self-hosted.show slash 123.
[3444.06 --> 3444.94]  ...
[3444.94 --> 3445.88]  ...
[3445.88 --> 3447.36]  ...
[3447.36 --> 3447.88]  ...
[3447.88 --> 3447.96]  ...
[3447.96 --> 3449.78]  ...
[3454.32 --> 3454.98]  ...
