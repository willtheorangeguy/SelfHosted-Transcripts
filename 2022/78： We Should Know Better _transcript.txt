[0.00 --> 2.58]  No Brent this week. He's finally left the building.
[3.16 --> 6.10]  I must feel a little like empty nest over there.
[6.26 --> 9.56]  Yeah, a little bit. We do miss our little baby Brent bird.
[9.74 --> 16.20]  Yeah, it's like having a pet Canadian around that cleans up after himself, makes food.
[16.46 --> 21.16]  Mostly, apart from his perennially dirty egg pan that's on the stove.
[21.54 --> 24.54]  Yeah, he'll have that and like a plate and a cup.
[24.74 --> 27.96]  It's impossible to explain to anybody that's never lived with a Brent.
[27.96 --> 31.22]  But the guy eats constantly.
[31.66 --> 34.86]  This is his vegan lifestyle because he doesn't have any serious protein in him.
[35.10 --> 42.08]  But to his credit, and I think you'd agree with me, this bastard can make a meal out of anything.
[42.38 --> 45.56]  Like I'll look in the fridge and I'll be like, we've got nothing to eat.
[45.68 --> 48.26]  And Brent will look up there and go, oh, we've got three days worth of food in here.
[48.44 --> 51.00]  And he'll put a bunch of stuff together that you'd never think would work.
[51.44 --> 53.54]  And it works. That's like his superpower.
[53.54 --> 58.12]  In his honor today, I am drinking a beverage which is new to me.
[58.22 --> 60.68]  This is the Canada Dry Ginger Ale.
[61.06 --> 62.04]  It's actually very tasty.
[62.40 --> 63.78]  Maybe they know what they're doing up there.
[64.08 --> 68.48]  So I know while he was at your place, he was deep diving into Plex.
[68.98 --> 73.20]  And he was also watching some content off of my Plex server while it was still up.
[73.20 --> 87.08]  And kind of ironically, today, as we're starting the show, we look at the headlines and we see Plex has suffered a massive compromise exposing usernames, emails and passwords, Alex.
[87.08 --> 88.96]  Yeah, this is not a good look, is it?
[89.04 --> 106.72]  For an app which is, well, was primarily designed for local media playback to suffer a compromise like this, where they say that yesterday we discovered suspicious activity on one of our databases.
[106.72 --> 114.18]  We immediately began an investigation and it does appear that a third party was able to access a limited subset of data.
[114.66 --> 119.16]  That includes emails, usernames and encrypted passwords.
[119.96 --> 131.76]  Now, what I find interesting about this statement is that there are conflicting reports online as to whether the passwords themselves were encrypted or whether they were just hashed with a salt.
[131.76 --> 140.68]  I think you touched on it there. I think why it stings so much is some of us have been using Plex and some of us have been a lifetime subscriber for a very, very, very long time.
[141.16 --> 146.52]  And it didn't necessarily have all of these hooks into the online Plex backend.
[146.92 --> 152.94]  In fact, I don't even recall it requiring logging into the Plex service to just access my local Plex library.
[153.12 --> 155.24]  I seem to recall that was something that came along later.
[155.24 --> 158.90]  And so they've sort of built and baked in this stuff as time has gone on.
[159.68 --> 166.80]  And it was something that initially started as kind of my off the radar stash of stuff.
[167.60 --> 170.44]  And now it's sort of integrated in with this whole service.
[170.44 --> 174.72]  And now my information's been leaked because, of course, my stuff's in there.
[175.04 --> 176.06]  It really stings.
[176.06 --> 180.36]  We know better, and I think that's going to be the theme of this episode, is that we know better.
[180.46 --> 186.24]  These companies that store our data in the cloud, be it Plex, be it Google, as we will touch on later.
[187.88 --> 192.12]  At some point, that information is going to become public domain.
[192.12 --> 214.94]  And I think no matter whether it's an encrypted library of some description of information, like, say, what's in your password manager, or whether it's a database of hashed password salts, or whatever it may well be, at some point, it is fair to say that that information will end up in the wrong hands somehow.
[216.44 --> 219.46]  You know, it's just a fact of life these days, unfortunately.
[219.46 --> 237.00]  So all of this, and I think, again, this will be a theme of this episode, has me questioning, yet again, why I'm relying on a closed source application which requires third-party authentication outside my LAN to watch a file which is sat in my basement.
[238.32 --> 248.04]  Jellyfin is the obvious choice, but I wondered, do you have any opinions on, I don't want to say Plex versus Jellyfin, but like the ecosystem of the two apps?
[248.04 --> 256.52]  Yeah, this is going to be tricky because maybe you and I, with our set-top boxes, could kind of make anything work.
[256.76 --> 262.10]  But there's also, like, listeners out there who are using Plex because it's built into their smart TV.
[262.54 --> 263.78]  They've got an app for it.
[264.52 --> 268.08]  And that is not necessarily the case with Jellyfin.
[268.16 --> 272.10]  You can get it on Android, you can get it on Apple TV, you can get it on the Roku, a Jellyfin app.
[272.10 --> 276.48]  So I imagine you can also sideload it or get it maybe from the store directly on the Firestick.
[276.60 --> 277.50]  I haven't checked in forever.
[277.98 --> 278.68]  But that's about it.
[279.30 --> 280.56]  That's where it drops off, right?
[280.72 --> 282.88]  And there's a lot of other devices out there.
[283.40 --> 284.06]  That's tricky.
[284.66 --> 290.04]  I know also I hear from the audience a lot there's a UI, you know, a UI gap between Jellyfin and Plex.
[290.04 --> 301.70]  And I also will, I know we're going to hear from people that will say, but hey, you know, Chris, hey, Alex, you could actually, for the most part, use Plex with only local network authentication.
[302.24 --> 304.52]  But here you hit the same issue you have with Jellyfin.
[305.38 --> 311.48]  When you go with only local authentication with Plex, you break about 80% of the Plex clients.
[311.66 --> 312.64]  They just don't work.
[312.64 --> 320.52]  And if you want to test, just disconnect your internet for an afternoon and see what devices in your house will play Plex and which ones won't.
[320.72 --> 322.02]  I think you'll be quite disappointed.
[322.44 --> 323.08]  Yeah, not many.
[323.38 --> 335.32]  And the thing is, like when I was on the plane coming back from England just last week, even my iPad, which I had deliberately cached terabytes worth of media to an external drive,
[335.32 --> 344.10]  decided when I loaded up the Plex app that it was going to sit there and spin for a minute or two, trying to connect, even though there was no network connection.
[344.78 --> 346.66]  And I'm like, what are you doing?
[346.66 --> 348.88]  I just want to play these local files.
[349.04 --> 350.24]  Please let me in.
[350.92 --> 356.72]  And it straws slowly, one by one by one, breaking the camel's back here with Plex.
[356.90 --> 359.92]  But I have a few apps that I rely on.
[360.26 --> 361.28]  I say rely.
[361.46 --> 362.64]  I use, OK?
[362.88 --> 363.78]  It's maybe not rely.
[363.92 --> 364.94]  It's too strong of a word.
[364.94 --> 373.38]  But things like Tautooli, and I don't know if I've said that name correctly, but essentially it's Plex server playback stats application.
[373.90 --> 383.14]  So it can track, you know, what my users have been watching, when they played, paused and stopped and started, and whether they transcoded and all these useful things,
[383.14 --> 389.32]  which I can look back in trends and say, well, which shows, because nobody watched for three years, well, I can go ahead and delete those.
[389.72 --> 390.72]  That kind of thing.
[390.94 --> 391.88]  Oh, that's an interesting idea.
[391.88 --> 396.04]  I'd never thought about actually using it for cleaning up library items you're no longer using.
[396.40 --> 401.50]  Did you happen to check and just, I don't know, review what Brent binged while you were gone?
[402.32 --> 404.84]  I think he was on a Better Call Saul binge whilst I was gone.
[404.94 --> 405.38]  Yeah, yeah.
[405.38 --> 406.86]  Mostly because we were.
[407.10 --> 409.72]  Which, by the way, I'm not going to spoil the ending, but it was fantastic.
[410.16 --> 412.38]  This is part of the ecosystem you're talking about, though.
[412.46 --> 413.00]  Yeah, absolutely.
[413.84 --> 415.28]  So Tautooli is one of them.
[415.58 --> 417.90]  There's a new one this week, which I just came across.
[417.98 --> 421.66]  I think you've been using it for a while from what you told me, called Overseer.
[421.66 --> 427.38]  Overseer is a class of application we don't talk a lot about on the show, sort of touching the third rail.
[427.78 --> 432.32]  But it is the ultimate evolution of that type of application.
[432.44 --> 438.08]  And these are those apps where you just say, hey, computer, I want this movie or this show.
[438.12 --> 438.86]  And it goes and gets it.
[438.88 --> 444.84]  But this takes it to the next level in helping you discover stuff that's trending and popular or well-rated.
[445.08 --> 447.22]  And it wraps it all up with such a great UI.
[447.52 --> 448.82]  That's what I absolutely love about it.
[448.82 --> 454.04]  So the thing that really seals the deal is it has a full Plex library integration.
[454.48 --> 460.44]  So if I'm saying to my family, well, let's say my mum was a big Elvis fan.
[460.70 --> 462.58]  And that new Elvis movie just came out.
[462.62 --> 465.40]  She was like, could you add it to Plex for me?
[465.60 --> 467.84]  And I'm like, well, I could.
[468.08 --> 468.90]  But you could do it yourself.
[469.82 --> 472.82]  And then she had the link with her three-tail scale, which is awesome.
[473.60 --> 475.16]  So there's nothing exposed on the internet.
[475.26 --> 477.58]  But it has a library integration with Plex.
[477.58 --> 482.70]  And so if I already had that movie in my library and she went to go and request it, for example,
[483.24 --> 486.34]  it would say, hey, dummy, this already exists.
[486.42 --> 486.96]  Go watch it.
[487.14 --> 490.36]  And it'd give you a direct link right the way through to Plex's UI.
[490.70 --> 495.32]  And there's nothing I would say that stops these kind of apps integrating with Jellyfin directly.
[495.74 --> 499.66]  It's just that Plex has been the tallest nail for a very long time now.
[499.66 --> 505.96]  And so if you are a developer targeting this space, it's only natural that you would target Plex first.
[506.32 --> 507.22]  Yeah, I suppose so.
[507.30 --> 512.52]  Plus, you know, Plex has the company you can interface with if you're another business.
[512.68 --> 518.82]  I think the other thing that they have going for them, obviously, is they have a really well-established API, really well-documented.
[519.04 --> 520.86]  And then they have that big user base.
[521.22 --> 522.36]  You just add all that stuff up.
[522.36 --> 524.38]  And I understand why people are building for it first.
[525.16 --> 530.22]  Overseer, though, which Overseer, by the way, is spelt Overseer.
[531.80 --> 533.28]  Is that what it is?
[533.34 --> 533.72]  Let me look.
[533.82 --> 535.16]  There'll be a link in the show notes, people.
[535.40 --> 535.50]  Yeah.
[535.84 --> 536.12]  Yeah.
[536.62 --> 541.20]  Overseer.dev, if you want to check it out.
[541.20 --> 550.76]  It does support local accounts, but then you lose one of the nice things that Overseer supports, which is it will integrate with your Plex user accounts.
[550.98 --> 556.22]  And it supports restricting media to certain users, which is really handy when you have kids.
[557.48 --> 559.30]  Again, it's part of that damn ecosystem.
[559.48 --> 564.32]  And I've been using this for several months, and it's just so easy to pull it up.
[564.90 --> 568.50]  So, again, they're not a sponsor on this show, but Tailscale on my phone, right?
[568.54 --> 569.66]  So I connect Tailscale.
[570.16 --> 572.90]  I pull this up in a web browser on my phone.
[573.12 --> 574.48]  It's perfectly formatted.
[574.78 --> 576.06]  I can hand it to my wife.
[576.50 --> 577.56]  She can type in what she wants.
[577.62 --> 579.32]  She can do her browsing, get it all set up.
[579.64 --> 580.56]  It's a real winner.
[581.14 --> 586.20]  And it's, I mean, it's not impossible to use it with Jellyfin, but it just wouldn't have that level of integration.
[586.72 --> 586.82]  Right.
[587.10 --> 590.14]  And we touched briefly on the third rail at the beginning of this.
[590.14 --> 592.56]  You don't have to use it in that context either.
[592.56 --> 600.42]  You could literally just use it as a wish list or a watch trending list as to what's available on various different services as well.
[600.52 --> 604.06]  So it's not limited to only people who wear pirate hats.
[606.52 --> 608.88]  Yeah, although it's, I mean, I think that is its core functionality.
[609.06 --> 609.76]  I'm not going to lie.
[609.92 --> 610.42]  Yeah, possibly.
[612.06 --> 613.16]  But you're right.
[613.22 --> 617.38]  You could also build a wish list, and it will help with some of those tracking services as well.
[617.56 --> 620.26]  And as you would expect, it's just like a container away.
[620.26 --> 623.84]  I didn't check the license on it, but I do think it's open source as well.
[624.12 --> 624.66]  Yeah, it's up on GitHub.
[624.86 --> 625.82]  Check it out over there.
[626.36 --> 627.34]  Overseer is a really good one.
[627.72 --> 631.86]  It's a Node.js app, and the source code is all on GitHub.
[633.56 --> 635.26]  Linode.com slash SSH.
[635.86 --> 640.80]  That's where you go to get $100 in 60-day credit on a new account, and it's just a great way to support the show.
[640.88 --> 644.40]  So it's Linode.com slash SSH.
[644.74 --> 646.02]  Linode is simple cloud hosting.
[646.02 --> 653.56]  When you want to put something up in the cloud, you want infrastructure you have under your control with root access that is super fast and affordable.
[654.22 --> 658.20]  Well, Linode is 30% to 50% cheaper than the major hyperscalers out there.
[658.68 --> 661.34]  And Linode can also be a fantastic platform to learn.
[661.48 --> 668.60]  I know I tell you guys about how we use it as our own lab, and it's also where we deploy all our stuff in production, like our new website's being built out, and we'll run from there.
[668.88 --> 671.10]  Just about anything we've built in the last two and a half, three years.
[671.10 --> 673.20]  But it's also where I go to learn.
[673.50 --> 677.94]  You know, they have Kali Linux on there right now, and cybersecurity is a huge field.
[678.34 --> 685.68]  And if you're going to get familiar with cybersecurity at all, you're going to be worth your salt at all, you've got to get Linux skills.
[685.90 --> 687.10]  You've got to train up.
[687.22 --> 691.06]  You just have to understand how these systems are built from the ground up.
[691.20 --> 694.26]  And why not just tear something down over and over again?
[694.38 --> 695.16]  Break and fix.
[695.26 --> 696.42]  Break and fix on Linode.
[696.84 --> 699.34]  It's so fast, you can get started in just seconds.
[699.34 --> 712.28]  And, you know, sure, you could, like, spin up a VM on your box, but there's no substitute for learning on an actual Linux machine that has really good performance, that installs packages in seconds, has a fantastic internet connection.
[713.02 --> 717.04]  Linode allows you to spin up and work with Linux servers with a distribution of your choice.
[717.12 --> 718.06]  They got all the good ones.
[718.46 --> 721.26]  Real compute power in a real data center.
[721.50 --> 729.28]  They regularly keep their software and their hardware as up-to-date as possible, run out MVME storage, 11 data centers around the world, AMD Epic.
[729.34 --> 730.04]  They have processors.
[731.18 --> 732.82]  And they have so many other great features, too.
[733.72 --> 736.08]  I use the crap out of the REST3 compatible object storage.
[736.82 --> 739.72]  Alex loves the fact that it's no problem to use things like Ansible.
[739.88 --> 741.88]  Of course, Terraform and Kubernetes support it as well.
[742.16 --> 744.02]  And they have the best support in the business.
[744.86 --> 745.94]  Sometimes that's really nice.
[746.00 --> 753.10]  If you, your friends, your family, or your business depend on it, it's nice to know you've got support 24-7, 365 with a real human being.
[753.88 --> 755.96]  So go get $100 and support the show.
[756.58 --> 757.34]  And try out Linode.
[758.06 --> 760.04]  Linode is just our host and provider of choice.
[760.14 --> 761.08]  They're a great place to go.
[761.18 --> 763.34]  My friends have been there for a decade.
[764.20 --> 766.66]  I'm a newbie compared to them, and I'm coming on three years.
[766.82 --> 768.04]  And I'm still extremely happy.
[768.48 --> 769.54]  So go try it out.
[769.86 --> 770.94]  Go see what you can do.
[771.04 --> 772.00]  Go see what you can learn.
[772.70 --> 773.62]  Go deploy something.
[774.20 --> 776.70]  Linode.com slash SSH.
[776.70 --> 791.82]  Now, picking back up on the theme of this episode of perhaps we should know better and not be surprised when big companies get hacked or do things with our data that we don't particularly like or agree with,
[792.36 --> 800.08]  there was an article in the New York Times this week about a gentleman whose young child, toddler, I think, had some kind of a medical issue.
[800.08 --> 818.58]  And as part of the telemedicine procedure that this father, worried parent, was doing, he uploaded some pictures of genitalia, of his child's genitalia, to his Android phone's Google automatic photos backup.
[819.22 --> 827.80]  And as a consequence, he ended up being flagged not only by Google, but by the police and law enforcement.
[827.80 --> 830.90]  Well, Google notified them automatically, so conveniently.
[831.08 --> 837.72]  Also sent them his entire Google account history, every search, all his location history, all of his text messages.
[838.30 --> 840.80]  They sent everything that he put in there since the early aughts.
[841.78 --> 843.40]  They sent it all over to the cops automatically.
[844.22 --> 846.20]  You know, the details of this are kind of interesting.
[846.66 --> 848.78]  So the wife took the pictures on her iPhone.
[850.02 --> 853.62]  She texted them to her husband because he was the one interfacing with the doctor.
[854.62 --> 857.78]  His Android automatically backed them up to Google Photos.
[857.80 --> 865.80]  Then Google's system detected these photos, flagged their child abuse team.
[866.24 --> 872.80]  They reviewed this guy's kid's crotch pictures, and then they sent it all off to the cops automatically.
[874.08 --> 880.30]  They, at that point, then disabled his Google account, which also disabled his Google Fi cell phone service.
[880.44 --> 884.40]  So then the police could no longer get a hold of him, which became an issue later.
[884.40 --> 887.16]  And they just presumed he was guilty.
[887.68 --> 896.90]  And I think the thing that I find disturbing about this is these are not pictures that are in an existing CSAM model database of known child pornography.
[896.90 --> 907.90]  These are brand new bespoke pictures that Google identified as child porn in this guy's Google photo database and then initiated this entire auto flag service.
[907.90 --> 910.90]  And he's this Mark.
[910.90 --> 912.54]  Mark, we only have his first name.
[913.00 --> 914.16]  He's not the only one.
[914.52 --> 924.44]  The New York Times article, which we'll link to in the show notes, talks about another dad that this happened to around the same time, because, of course, more people are using telemedicine now.
[925.58 --> 926.76]  And so it's happening more and more.
[926.76 --> 940.94]  And the other little detail in this story that's horrible, besides the fact that this guy's cell phone service was turned off, the police have notified Google that they've cleared him and Google refuses to turn his account back on.
[941.18 --> 942.74]  And this is true for the other ones as well.
[943.28 --> 946.06]  This is really what gets me going about this particular story.
[946.72 --> 956.10]  At what point did we as a society decide that Google were now the law, right?
[956.10 --> 970.92]  This guy, you know, the people that we have chosen as society to say, you are the one who decides whether someone has committed a crime or not, the police, detective, whatever it might be, FBI, whoever.
[972.06 --> 979.38]  At some point, Google, without really realizing it, probably have more power over you than that individual does.
[979.38 --> 993.20]  Because not only are you locked out of your cell service, you're also locked out of, was it 15 plus years worth of correspondence and PDF receipts and all the other stuff that ends up in everybody's Gmail inboxes?
[993.20 --> 1003.06]  Yeah. And the other dad who also got flagged was in the middle of a mortgage deal and was trying to like get papers to sign to buy his house and they were in his Gmail inbox.
[1003.22 --> 1012.72]  And because Gmail did this, because Gmail got turned off, he had to ask the broker to switch to a new email account, which then flagged him for fraud.
[1012.72 --> 1020.36]  And they thought that was suspicious, which then threw his entire mortgage back into review because his Gmail account got disabled.
[1020.36 --> 1030.16]  I think the saddest thing for me about this, and by this I mean sort of modern tech, Google, Apple, Facebook, or this kind of surveillance culture,
[1030.40 --> 1042.88]  is that we've ended up spiraling into this user manipulation, user surveillance space without, honestly, in autopilot, without really realizing that we were doing it.
[1042.88 --> 1049.60]  Piece by piece by piece, little by little, all of these little apps have eroded into our little worlds.
[1049.82 --> 1055.50]  And, you know, now Google Photos is a fundamental part of my personal photo backup strategy.
[1056.36 --> 1060.46]  I have a young child and, you know, I take pictures of her in the bath.
[1060.94 --> 1066.30]  At what point do I run the risk of Google flagging my images and having my stuff locked out?
[1066.38 --> 1069.26]  You know, it's not unlikely at this point.
[1069.26 --> 1073.68]  We also know that these classifiers and these models don't always get it right.
[1073.88 --> 1078.86]  Computer vision is still early, and everybody listening to this show knows that's a fact.
[1079.02 --> 1080.68]  Hot dog, not a hot dog.
[1081.32 --> 1081.62]  Right.
[1081.82 --> 1085.34]  And the reality is these things could get it wrong.
[1086.36 --> 1094.88]  And the best case scenario in that situation is that a team of people at Google are looking at whatever private pictures you have,
[1095.00 --> 1096.56]  and you never even know anything happened.
[1096.56 --> 1103.80]  But back in Google's headquarters, a group of human beings are looking at your private pictures because they've been flagged.
[1103.88 --> 1105.24]  That's the best case scenario.
[1105.64 --> 1105.82]  Right.
[1106.06 --> 1111.56]  And the worst case scenario is what's happened to Mark here, where everything got shut off,
[1111.74 --> 1116.76]  and then his entire account was downloaded and sent to the cops to review.
[1116.76 --> 1124.90]  Where if Mark, at any point in the last 15 years, had done something else illegal, it would be in there.
[1125.26 --> 1131.70]  Emails, text messages, photos, all of his location information, every place he ever went on Google Maps,
[1132.00 --> 1137.60]  every search request he's ever made into Google, every single Google Doc, every spreadsheet he's ever created,
[1137.60 --> 1139.32]  everything got sent to the cops.
[1139.66 --> 1140.80]  They could review that.
[1141.28 --> 1145.04]  And, you know, I mean, maybe some people will come out squeaky clean, and maybe others,
[1145.78 --> 1146.76]  there'd be something else in there.
[1146.82 --> 1149.68]  And I don't know what happens there, but I doubt it just gets deleted.
[1150.18 --> 1152.34]  You know, it's just, the precedent here is horrible.
[1152.34 --> 1157.38]  Around the time of Brexit, I remember having a discussion with a family member about,
[1157.88 --> 1161.16]  well, I've got nothing to hide, so I've got nothing to fear, right?
[1161.20 --> 1167.50]  And I think this is the insidious conclusion of that I've got nothing to hide.
[1167.70 --> 1172.62]  You know, this is a perfectly innocent, legitimate use case of taking a photograph like that.
[1173.08 --> 1174.86]  And it's landed this guy in a lot of trouble.
[1175.18 --> 1179.40]  I'm not totally familiar with wire-tapping laws on this side of the pond,
[1179.40 --> 1185.14]  but I do wonder if legislation needs to catch up with this kind of thing.
[1185.32 --> 1192.26]  Because as far as I'm aware, at least, it's a federal crime to wire-tap somebody without their permission or consent,
[1192.68 --> 1194.42]  without some kind of a court order.
[1194.94 --> 1201.70]  And I don't know if a EULA would really constitute a genuine admission of my consent to do this.
[1202.52 --> 1204.06]  Google will probably argue the opposite.
[1204.92 --> 1208.44]  But without some kind of a court order, this feels like a stretch to me.
[1208.44 --> 1212.92]  Yeah, so I know that the Fourth Amendment and those protections apply to anything the state does.
[1213.04 --> 1214.78]  The state would not be able to just do this.
[1214.98 --> 1220.02]  But we've privatized this now with Google and, of course, with all these other tech companies.
[1220.28 --> 1223.62]  And I do know that the lines there are a lot less clear.
[1224.26 --> 1230.00]  And so the beauty thing is, is there's this just not-my-problem-legal situation that Google's in
[1230.00 --> 1234.00]  and that the state is in, where Google can collect all the information and use it,
[1234.00 --> 1235.50]  infinitum, for their own value.
[1235.96 --> 1242.08]  And then they also have all the incentives in the world to share that data with law enforcement
[1242.08 --> 1246.10]  at the lowest friction way possible, in the most efficient way possible.
[1246.42 --> 1246.60]  Right?
[1246.66 --> 1248.98]  That's their incentive structure, for obvious reasons.
[1249.24 --> 1254.12]  And I don't think that's going to change because both parties involved,
[1254.12 --> 1258.84]  both the business and the state, are very satisfied with this arrangement.
[1258.84 --> 1259.70]  You know?
[1260.10 --> 1265.96]  Alex, it's been a long time since I have seen a tech story that actually genuinely gave me chills.
[1266.82 --> 1267.18]  Right?
[1267.28 --> 1269.50]  I mean, I've been like, oh, I've been outraged or whatever.
[1269.60 --> 1271.68]  But like, actually, like, oh, no.
[1272.98 --> 1273.40]  Uh-oh.
[1273.80 --> 1279.18]  Like, it's, we are already, all of us that are dads that have ever taken pictures of our kids
[1279.18 --> 1281.60]  in the bath or anything like that, we are all now at risk.
[1282.20 --> 1282.90]  All of us.
[1282.90 --> 1287.38]  And we just walked right into it, even though we've been talking about the risks for years.
[1287.90 --> 1289.16]  I've thought a lot about this.
[1289.24 --> 1294.92]  And I've realized the truth is these services have a lot of upside.
[1295.90 --> 1297.18]  They have a lot of it.
[1297.28 --> 1298.46]  They have a lot of reach.
[1298.72 --> 1299.92]  They have a lot of features.
[1300.70 --> 1302.58]  There's just a lot of upside to them.
[1302.92 --> 1306.52]  Google Photos is very, very tempting because they manage the storage.
[1306.52 --> 1310.74]  They manage the replication in their servers and their data centers.
[1310.74 --> 1312.62]  They manage the bandwidth.
[1313.70 --> 1315.38]  And they're kind of just doing it automatically.
[1315.54 --> 1316.82]  So you don't even have to think about it.
[1316.92 --> 1320.22]  And that, like, as a parent, like, the last thing you ever want to lose is your pictures.
[1320.94 --> 1323.92]  You know, if your whole house burned down, but you save nothing but your pictures, you'd
[1323.92 --> 1325.22]  say, well, at least I still have my pictures.
[1325.66 --> 1325.82]  Right?
[1325.88 --> 1326.84]  Like, that's, they're critical.
[1327.24 --> 1331.76]  You kind of just get pushed into it because it's the default, both on iOS and on Android.
[1332.30 --> 1334.98]  Because this is eventually going to be happening on iOS as well.
[1335.50 --> 1338.60]  You just set up the phone by default and all these things are on.
[1338.60 --> 1341.36]  And they're just kind of like, well, why not leave them on?
[1341.40 --> 1342.70]  Because my photos, they're important.
[1343.24 --> 1348.40]  One of the worst aspects of this, which we kind of already touched on, though, is that
[1348.40 --> 1353.72]  even though law enforcement said this chap was not guilty of committing a crime, he still
[1353.72 --> 1355.06]  doesn't have his Gmail account back.
[1355.38 --> 1358.88]  Google have told the New York Times they stand by these decisions.
[1359.36 --> 1362.64]  And this guy will be locked out, I presume, forever.
[1362.82 --> 1363.20]  That's it.
[1363.22 --> 1363.58]  He's done.
[1363.88 --> 1366.64]  Yeah, the response was just like, well, we find child porn to be abhorrent.
[1366.64 --> 1367.78]  And who could argue with that?
[1367.84 --> 1369.26]  That's a perfectly rational statement.
[1369.46 --> 1371.20]  Won't somebody think of the children?
[1372.20 --> 1373.50]  That's how it always starts, though.
[1373.98 --> 1379.92]  I think my baseline advice now is if you're going to use Google services, if you're going
[1379.92 --> 1385.00]  to be dependent on Google services, you have got to have a valid backup.
[1385.24 --> 1386.90]  Valid backup for anything that's important.
[1387.02 --> 1387.94]  Email, calendar.
[1388.68 --> 1389.62]  You've got to have it.
[1389.62 --> 1393.60]  You know, and I guess that's that's the bare minimum.
[1393.60 --> 1401.02]  But both in the case of Plex and in the case of Google Photos and all that, I am I feel
[1401.02 --> 1402.80]  like the math has just changed for me.
[1403.32 --> 1405.54]  I think it's time to give PhotoPRISM another try.
[1405.62 --> 1409.06]  I think it's time to really try to not use Google Photos at all.
[1409.18 --> 1412.28]  I took a break for a while and then I got back on and then I took a break for a while
[1412.28 --> 1413.28]  and then I got back on.
[1413.28 --> 1414.94]  But this is too far for me.
[1415.06 --> 1420.60]  This is if if if I don't pay attention to this red flag and then something happens to
[1420.60 --> 1420.86]  me.
[1421.82 --> 1423.58]  What kind of an idiot am I going to feel like?
[1423.76 --> 1427.76]  What kind of an ultimate idiot like this is like I've got to pay attention to these
[1427.76 --> 1432.26]  warning signs because the thing that seems to be clear and I'm curious to know if you
[1432.26 --> 1432.54]  agree.
[1433.76 --> 1436.48]  I'm not happy to say this, but it's getting worse.
[1437.48 --> 1440.90]  And the longer you participate and the more data you give it.
[1441.66 --> 1442.86]  The worse you make it.
[1442.86 --> 1449.54]  Like in the case of my Google account, I got a Gmail account within nine months of Gmail
[1449.54 --> 1450.20]  launching beta.
[1451.00 --> 1458.40]  I have Gmail chats with my ex-wife Angela when we were still like just meeting.
[1458.70 --> 1459.22]  Right.
[1459.36 --> 1459.86]  I mean.
[1460.72 --> 1467.88]  I have an entire relationship's worth of history in that Google chat and I feel like I got to
[1467.88 --> 1469.76]  I got to purge everything.
[1469.76 --> 1474.02]  I'm starting to feel a little more like Richard Stallman.
[1474.14 --> 1475.78]  Like I need to go off grid almost.
[1475.94 --> 1476.44]  And it's.
[1476.44 --> 1476.88]  Yeah.
[1477.18 --> 1477.38]  Yeah.
[1477.44 --> 1481.96]  You know, between because the other the other the other risk with Plex, Alex, and I think
[1481.96 --> 1484.64]  the real risk with Plex, they're going to get sold.
[1484.64 --> 1489.36]  They're going to get sold to a major entertainment company and then they're going to have all
[1489.36 --> 1493.28]  our metadata about what's on our servers, about what we're watching, about what our watch
[1493.28 --> 1495.10]  habits are, because, you know, they're collecting all of that.
[1495.98 --> 1496.40]  That's.
[1496.52 --> 1500.02]  And then with Google, the risk is that they're just going to get more invasive.
[1500.30 --> 1501.86]  They're going to do more things in your life.
[1501.86 --> 1505.66]  And then they just have that automatic pipeline to your local friendly authorities.
[1506.28 --> 1512.52]  And both are becoming more and more real, tangible risks to everyday people.
[1513.12 --> 1513.86]  Couldn't agree with you more.
[1514.04 --> 1518.54]  And it's got me looking for ways to back up my Gmail in the last few days.
[1518.54 --> 1524.54]  I actually put a thread in the self-hosted subreddit today as we record.
[1524.64 --> 1528.28]  It's Wednesday the day before or two days before this episode airs.
[1528.36 --> 1531.54]  So maybe there'll be some more answers to that thread in the meantime.
[1531.86 --> 1533.66]  I'll put a link to it in the show notes, of course.
[1534.36 --> 1537.26]  Lots of people suggest using Thunderbird as a backup.
[1537.50 --> 1544.02]  I I'm not sure if I agree with that as a backup per se, because it still requires some
[1544.02 --> 1548.78]  kind of a desktop environment in order for Thunderbird to run, as far as I'm aware.
[1549.08 --> 1550.26]  Yeah, you'd have to fire it up, right?
[1550.34 --> 1550.92]  And keep it going.
[1551.14 --> 1551.66]  Yeah, exactly.
[1552.04 --> 1553.12]  There are other options.
[1553.30 --> 1556.18]  Apparently, offline IMAP plus DoveCot is another one.
[1556.50 --> 1559.62]  And that will be usable with any mail software that uses SMTP.
[1560.74 --> 1564.02]  There's lots of other people talking about different ways to sync IMAP.
[1564.26 --> 1567.72]  Apparently, there is a Docker Thunderbird image, I'm told, in the chat as an option.
[1568.10 --> 1569.68]  So that will work quietly in the background.
[1570.34 --> 1573.60]  But one that a listener recommended to me in Discord this afternoon
[1573.60 --> 1578.76]  was one called Got Your Back from the GAM team, G-Y-B.
[1579.52 --> 1580.70]  Again, link in the show notes.
[1581.18 --> 1585.12]  This is a command line tool for backing up your Gmail messages to your computer
[1585.12 --> 1588.18]  using Gmail's API over HTTPS.
[1588.42 --> 1593.42]  So I had a quick spin of this before the show, just on my laptop, which is a MacBook.
[1594.72 --> 1596.82]  And it was a little fiddly to get set up.
[1596.94 --> 1600.52]  You know, if you've ever set up an API key for like Google Maps or anything like that
[1600.52 --> 1604.64]  and created a no-auth application with a client secret and a client token and what have you,
[1605.20 --> 1606.18]  it was a little bit fiddly.
[1606.40 --> 1607.94]  Probably took about 10 minutes to get it going.
[1608.60 --> 1611.54]  I put it on one of my lesser-known Gmail accounts.
[1611.62 --> 1613.44]  It only has about 10,000 emails in it.
[1613.50 --> 1615.50]  Not my primary one as the first try.
[1616.50 --> 1618.66]  And it works perfectly.
[1618.88 --> 1620.18]  Works exactly as advertised.
[1620.18 --> 1623.72]  All 10,000 messages were downloaded in .eml format.
[1624.20 --> 1629.92]  I was then able to open those with the mail client on Mac, view them in their full HTML glory,
[1630.54 --> 1631.36]  and it just worked.
[1632.06 --> 1635.48]  Hey, I like that it's command line, that it's basically a bash script,
[1635.60 --> 1636.84]  because then I could just cron that.
[1637.22 --> 1639.08]  That is something worth mentioning, actually.
[1639.24 --> 1642.56]  The project seems a little immature in some ways to me,
[1642.56 --> 1650.94]  because there's an issue in their GitHub where someone said that their wiki is open to public edits,
[1651.74 --> 1657.80]  and some insidious individual decided to change the download location of the binary
[1657.80 --> 1663.36]  or one of the scripts or something, so that it wasn't the official developer's script,
[1663.54 --> 1667.94]  and so some people had some unverified binaries being downloaded.
[1668.90 --> 1669.32]  Oh, no.
[1669.32 --> 1672.42]  And you never really know how many people got that and what's in there.
[1672.56 --> 1673.44]  That's too bad.
[1673.52 --> 1674.64]  Yeah, that's early day stuff.
[1675.28 --> 1678.68]  You know, if anybody out there in the audience knows of a way to do this,
[1679.18 --> 1681.94]  something you could automate, but just the whole account,
[1682.04 --> 1685.06]  like the Google Takeout functionality, boost in your answer,
[1685.12 --> 1689.54]  because I'd like to just back up everything, and then, I don't know,
[1690.00 --> 1692.30]  I'm on the edge of going over there and hitting delete.
[1692.54 --> 1693.80]  I am on the edge, man.
[1694.32 --> 1697.96]  If you've got the skills, you've got the infrastructure, you've got the tools,
[1697.96 --> 1699.30]  it's really a matter of time.
[1699.48 --> 1704.20]  So I think what I've got to do is figure out a weekend where this is,
[1704.26 --> 1706.98]  I just get it done, you know, and then I get everything set up,
[1707.02 --> 1708.36]  and then I go just delete it.
[1708.52 --> 1714.04]  And I hope, I hope to Linus that they actually truly delete it when I tell them to delete it,
[1714.04 --> 1715.48]  because who really knows?
[1715.84 --> 1716.52]  Who really knows?
[1716.88 --> 1717.58]  Who really knows?
[1718.22 --> 1719.72]  Now, this is another topic.
[1719.82 --> 1720.50]  This is photos.
[1720.70 --> 1723.60]  This is a little bit unrelated to Gmail itself,
[1723.60 --> 1727.00]  but obviously it's a fundamental part of the Google experience.
[1727.20 --> 1731.08]  There is a new self-hosted app on the scene called Image.
[1731.34 --> 1733.70]  Now, I haven't checked this out yet, actually, in person,
[1733.84 --> 1737.02]  because the developer states very clearly,
[1737.16 --> 1739.12]  this is not yet ready for production usage,
[1739.28 --> 1741.80]  and I don't really want to put my photos through it yet.
[1742.30 --> 1744.68]  However, every time I see this pop up on Reddit,
[1744.92 --> 1747.62]  it gets absolutely covered in praise.
[1748.30 --> 1750.54]  Everybody has nothing but good things to say about it.
[1750.54 --> 1752.52]  So I'm watching this project extremely closely.
[1753.26 --> 1755.40]  I've had several people mail in and tell me about it.
[1755.56 --> 1756.16]  Don't worry.
[1756.42 --> 1757.70]  It's on our radar.
[1757.88 --> 1758.62]  We will cover it,
[1758.68 --> 1761.32]  but once it goes into a, air quotes,
[1761.48 --> 1763.00]  production-ready state.
[1763.66 --> 1764.82]  Yeah, I'll keep an eye on it for sure.
[1765.38 --> 1765.62]  You know?
[1766.10 --> 1768.28]  Heck, I might even throw a few photos in there when it's in, you know,
[1768.30 --> 1768.96]  an earlier state.
[1769.10 --> 1771.14]  But yeah, I wouldn't want to switch the whole library over.
[1771.30 --> 1773.00]  But Image, I like the name.
[1773.66 --> 1774.94]  We'll have a link in the show notes.
[1777.34 --> 1780.10]  humio.com slash H-C-E.
[1780.54 --> 1783.90]  Go ingest all of your logs and view them in one place.
[1784.38 --> 1789.32]  Humio is a centralized log management and observability platform.
[1789.66 --> 1792.62]  The company was founded by developers in Denmark in 2016,
[1792.94 --> 1795.70]  and they've really been building something incredible since then.
[1795.98 --> 1797.42]  I think the real beauty of Humio,
[1797.50 --> 1798.70]  the thing they've really cracked,
[1798.76 --> 1801.54]  is they can take logs from any source and make them usable.
[1801.86 --> 1804.20]  You don't have to constantly massage the format.
[1804.54 --> 1805.74]  It doesn't need a schema.
[1805.74 --> 1807.98]  You just pump them all into Humio,
[1808.18 --> 1809.60]  and they're there when you need them,
[1809.76 --> 1811.80]  and the dashboard to review it all is great.
[1812.32 --> 1813.52]  Humio's platform is crazy.
[1814.08 --> 1818.20]  Their index-free architecture means you can ingest over a petabyte of data per day
[1818.20 --> 1820.06]  and search that with sub-second latency.
[1820.70 --> 1824.18]  And Humio's up to 80% cheaper than the competing platforms like Splunk or Elastic,
[1824.60 --> 1826.82]  thanks to its reduced hardware and computational footprint.
[1826.82 --> 1831.12]  I think the best way for our audience to get going is probably the community edition.
[1831.76 --> 1836.84]  Humio community edition is the largest no-cost data ingestion offering on the market today,
[1837.38 --> 1840.48]  allowing you to ingest up to 16 gigs per day,
[1841.02 --> 1842.38]  seven-day retention included.
[1842.48 --> 1843.56]  It's not a trial period.
[1844.02 --> 1845.18]  You get it for the long haul.
[1845.58 --> 1847.70]  This is perfect for us self-hosters because, yeah,
[1847.98 --> 1850.22]  you can put your home assistant logs in there.
[1850.38 --> 1852.06]  You can put your Nginx logs in there.
[1852.14 --> 1854.34]  Like I said earlier, you can put just about anything in there,
[1854.58 --> 1855.90]  and Humio knows what to do with it.
[1855.90 --> 1857.70]  It gives you the ability to bring all that stuff together,
[1858.24 --> 1861.20]  view it in one place, and that makes troubleshooting easier.
[1861.56 --> 1863.68]  It's so much better than having separate places to look
[1863.68 --> 1865.06]  when you need to figure out what went wrong.
[1865.38 --> 1866.34]  That's amateur stuff.
[1867.08 --> 1868.58]  Go get like a pro setup, right?
[1868.62 --> 1871.48]  Because when this is your home setup, it's your hobby,
[1872.06 --> 1873.50]  you don't want to have to fight with it.
[1873.60 --> 1874.60]  You just want the information.
[1874.82 --> 1876.00]  You want to be able to fix it quick.
[1876.32 --> 1877.10]  You want it easy.
[1877.26 --> 1877.92]  You want it usable.
[1878.12 --> 1879.80]  You don't want it to be another job.
[1880.16 --> 1882.44]  That's where Humio community edition could be perfect.
[1882.44 --> 1887.46]  So go get started for free at humio.com slash H-C-E.
[1887.60 --> 1892.40]  That's H-U-M-I-O dot com slash H-C-E.
[1892.40 --> 1896.44]  So you're all aboard the Zigbee train now.
[1896.52 --> 1898.30]  That seems to have left the station.
[1899.06 --> 1902.28]  Yeah, I was like trying so hard not to,
[1902.32 --> 1903.62]  because I already got a lot of Z-Wave,
[1903.98 --> 1905.44]  and I've already got Wi-Fi devices.
[1905.74 --> 1907.74]  Do I really need a third network, Alex?
[1907.80 --> 1908.44]  The answer is no.
[1909.10 --> 1909.32]  No.
[1909.64 --> 1910.26]  No, I do not.
[1910.78 --> 1912.22]  But yeah, that doesn't stop me anyways.
[1912.78 --> 1915.54]  This one really was because I'd tried everything else,
[1916.28 --> 1919.08]  and after last week's episode,
[1919.08 --> 1922.28]  I got a couple of notes almost immediately after the episode went out.
[1922.44 --> 1923.02]  They were just like,
[1923.78 --> 1926.16]  hey, you got to check out the Aquara temperature sensor.
[1926.72 --> 1928.90]  It's Zigbee, but it's battery powered,
[1929.04 --> 1931.04]  and it gives you real-time data.
[1931.38 --> 1934.26]  As the temperature changes, it sends in updates.
[1934.78 --> 1936.40]  You know, it's not this problem where it falls asleep
[1936.40 --> 1939.94]  and drops off the network like you had with the Shelly H&T.
[1940.64 --> 1942.50]  And so I thought, all right,
[1942.52 --> 1945.94]  I've been wanting to get, you know, on the Zigbee train and just try it.
[1945.98 --> 1947.64]  I knew eventually I wanted to give it a go,
[1947.64 --> 1950.04]  and I'm thinking about replacing my Z-Wave devices,
[1950.18 --> 1952.20]  and if Zigbee worked out, that'd probably be for the best.
[1952.68 --> 1955.28]  So I grabbed the Aquara temperature and humidity sensor
[1955.28 --> 1959.84]  and grabbed a Conbee Zigbee stick,
[1959.94 --> 1961.64]  which is like a German Zigbee stick,
[1961.92 --> 1964.24]  which just works out of the box with Home Assistant.
[1964.90 --> 1966.78]  And I got to say, Alex, this is the one.
[1967.46 --> 1968.74]  This is the one.
[1968.92 --> 1970.10]  I really like this.
[1970.16 --> 1972.74]  I think it's based on the same Yaome chipset
[1972.74 --> 1973.88]  that a lot of these are based on.
[1973.88 --> 1977.48]  And it has two years of battery life,
[1977.64 --> 1982.14]  which is outrageous because the things about the size of a bottle cap,
[1982.42 --> 1983.38]  you know, it's only square.
[1983.68 --> 1985.50]  It's super, super small.
[1985.62 --> 1987.46]  It's also the smallest temperature sensor
[1987.46 --> 1990.42]  of all of the ones that I've tried.
[1990.82 --> 1993.84]  It says on the box requires the Aquara hub.
[1994.04 --> 1996.88]  That just means it needs a Zigbee device to connect you.
[1996.88 --> 1998.54]  So once you put it on the Zigbee network,
[1998.62 --> 2000.50]  which takes about a millisecond,
[2000.58 --> 2003.02]  you just pull the battery, little plastic separator,
[2003.14 --> 2005.98]  and click the button when you're in discover mode in Zigbee,
[2006.10 --> 2007.90]  and it's connected immediately.
[2008.18 --> 2009.18]  What are you using for Zigbee?
[2009.42 --> 2010.42]  Are you using ZHA?
[2010.98 --> 2012.60]  Yeah, I'm using the built-in, yeah.
[2013.00 --> 2013.92]  And it's been fine.
[2014.02 --> 2017.42]  You know, it's cleaner and nicer than the Z-Wave stuff is.
[2017.48 --> 2019.00]  Of course, I'm using the older Z-Wave stuff.
[2019.68 --> 2021.38]  And Zigbee itself, I like.
[2021.38 --> 2024.80]  One of the things that I think is fantastic about it is
[2024.80 --> 2027.36]  when you add wired devices,
[2028.06 --> 2029.42]  you know, permanently powered devices,
[2029.64 --> 2031.00]  like a smart plug,
[2031.50 --> 2032.80]  just like Z-Wave,
[2033.04 --> 2035.40]  it builds the network out more.
[2035.52 --> 2037.28]  They become repeaters out there.
[2037.52 --> 2040.08]  It has about a 100-meter line-of-sight range.
[2040.30 --> 2041.82]  And, you know, you know how big the studio is.
[2042.02 --> 2042.98]  It's not that big.
[2043.32 --> 2046.74]  But the temperature sensor is in the far corner of the garage,
[2046.96 --> 2048.68]  and the home assistant blue
[2048.68 --> 2051.02]  is in the other far corner of the studio.
[2051.02 --> 2055.32]  So it's at the maximum separation you could get here in the studio,
[2055.44 --> 2057.62]  and it's still working pretty good.
[2057.70 --> 2060.22]  I think maybe I could slide a repeater in there
[2060.22 --> 2061.54]  and probably boost the signal a little bit,
[2061.62 --> 2063.58]  but it's getting the job done.
[2064.08 --> 2065.50]  Any permanently powered device,
[2065.58 --> 2066.70]  like a plug socket,
[2066.88 --> 2068.16]  like a smart plug,
[2068.60 --> 2069.76]  which is Zigbee ready,
[2069.88 --> 2070.98]  would be a great repeater,
[2071.02 --> 2071.84]  and I've got a couple of those.
[2072.44 --> 2076.64]  Also, light bulbs turn out to be really great Zigbee repeaters.
[2076.78 --> 2079.86]  Like all my Hue bulbs are connected to ZHA these days,
[2079.86 --> 2081.78]  and they're all permanently powered,
[2081.92 --> 2084.40]  and they all extend my Zigbee network.
[2085.02 --> 2087.96]  But I'm really glad that you're using this temperature sensor now,
[2088.00 --> 2089.08]  because I've had one since,
[2089.20 --> 2090.96]  I think, just before you came in April.
[2091.56 --> 2093.58]  There's one in my fridge, which works great,
[2093.80 --> 2097.04]  and I've got a couple in Ziploc freezer bags in the freezers,
[2097.04 --> 2101.32]  and they don't like minus 15 Celsius temperatures too much.
[2101.90 --> 2105.06]  The two-year battery life is more like two months,
[2105.50 --> 2106.62]  minus 15,
[2106.86 --> 2108.80]  but I must say the one in the fridge,
[2108.84 --> 2110.46]  which is typically around five Celsius,
[2110.98 --> 2113.90]  that's been on the original battery ever since I got it.
[2114.04 --> 2115.62]  So, so far, so good.
[2115.62 --> 2117.62]  I do think I'll be buying more of these,
[2117.70 --> 2118.52]  so that's good to know.
[2118.70 --> 2121.80]  I still have my Aotec Z-Wave in my freezer at home.
[2122.06 --> 2123.82]  On the original battery, I put it in there,
[2123.88 --> 2125.24]  which has been months now,
[2125.30 --> 2128.24]  but it's one of those bigger lithium Duracells.
[2128.96 --> 2129.56]  So I could see,
[2129.64 --> 2132.36]  because this is such a smaller battery in this guy,
[2132.40 --> 2133.72]  because it's such a tiny device.
[2134.02 --> 2136.34]  So this has the CR2032 battery in it,
[2136.36 --> 2137.70]  which is a lot smaller.
[2138.06 --> 2139.56]  It does also come in the box
[2139.56 --> 2141.62]  with a handy little circular double-sided tape,
[2141.94 --> 2143.78]  which fits perfectly on the back of the sensor,
[2143.78 --> 2145.18]  so you could just slap that on there
[2145.18 --> 2146.06]  and then you stick it anywhere.
[2146.70 --> 2148.46]  You are getting roasted in the chat, by the way.
[2148.56 --> 2148.96]  Oh, yeah?
[2149.18 --> 2150.24]  Yeah, you should go and see this.
[2150.66 --> 2152.08]  You know the little dog from Up,
[2152.32 --> 2152.72]  who's like,
[2152.88 --> 2153.90]  okay.
[2154.66 --> 2155.46]  Chris is like,
[2155.58 --> 2156.12]  new standard.
[2156.32 --> 2157.30]  Okay, I'm in.
[2157.40 --> 2158.42]  Yeah, I know.
[2158.60 --> 2159.46]  I know, it's true.
[2159.92 --> 2160.68]  It is true.
[2161.08 --> 2163.00]  Here's why I was okay going with Zigbee,
[2163.28 --> 2163.46]  right,
[2163.78 --> 2165.96]  is basically what Matter is.
[2166.48 --> 2168.32]  Matter is based on Zigbee,
[2168.64 --> 2170.12]  and it's an open source spec.
[2170.46 --> 2171.90]  It's going to be around forever.
[2171.90 --> 2172.90]  I mean, heck,
[2172.98 --> 2174.54]  the Mars rover is using Zigbee
[2174.54 --> 2175.58]  to communicate with the helicopter.
[2175.58 --> 2176.18]  I knew you were going to mention the Mars rover.
[2176.32 --> 2177.20]  Ding, ding, ding, ding, ding.
[2177.22 --> 2177.52]  You got to mention it.
[2178.94 --> 2180.20]  You got to mention it.
[2180.42 --> 2181.32]  It's so cool.
[2181.72 --> 2182.34]  And Z-Wave,
[2182.42 --> 2183.62]  Z-Wave's like end of life.
[2183.82 --> 2186.08]  So I think what I'm going to do is,
[2186.18 --> 2186.98]  although it sucks
[2186.98 --> 2188.54]  because I have so many Z-Wave devices,
[2189.06 --> 2190.92]  but I think over this next year,
[2191.06 --> 2191.38]  I don't know,
[2191.44 --> 2191.96]  maybe sooner,
[2192.46 --> 2193.36]  probably a lot sooner
[2193.36 --> 2194.96]  because I just want to get rid of
[2194.96 --> 2196.36]  my home assistant setup and start over.
[2196.68 --> 2198.50]  I think I'm going to just transition to Zigbee.
[2198.68 --> 2200.78]  So I'll have Zigbee and Wi-Fi devices,
[2200.78 --> 2201.98]  but honestly,
[2201.98 --> 2205.48]  I prefer not to have my IoT devices on Wi-Fi.
[2205.70 --> 2208.36]  It's heavy in terms of battery life
[2208.36 --> 2210.00]  and CPU and power,
[2210.14 --> 2212.96]  but also it's just not a great standard for it.
[2213.08 --> 2214.50]  It's a lot of chatter.
[2215.14 --> 2216.28]  And the more chatter,
[2216.38 --> 2217.34]  the worse the Wi-Fi network.
[2218.14 --> 2219.28]  Where like the Zigbee network,
[2220.00 --> 2221.04]  the individual devices
[2221.04 --> 2223.38]  can actually improve each other's signal
[2223.38 --> 2224.70]  and help route each other.
[2224.70 --> 2227.04]  And the more devices you add to a point,
[2227.20 --> 2227.96]  make it stronger.
[2228.38 --> 2230.48]  So it's clearly a better way to go
[2230.48 --> 2231.54]  for these types of devices.
[2231.86 --> 2234.40]  But it does suck having yet a third,
[2234.80 --> 2236.74]  a new wireless standard.
[2237.40 --> 2238.60]  That's why I resisted it,
[2238.82 --> 2240.72]  but it was the audience that convinced me to try it.
[2240.90 --> 2241.96]  And it is now my favorite.
[2242.36 --> 2243.78]  And it's nice to see the Zigbee integration
[2243.78 --> 2244.90]  work so well in home assistant.
[2245.36 --> 2246.24]  It makes me feel better.
[2246.62 --> 2248.84]  You'll be using the IKEA trad free buttons next.
[2249.14 --> 2249.76]  Just you wait.
[2249.76 --> 2250.48]  Oh man,
[2250.52 --> 2251.38]  I'm already on Alibaba
[2251.38 --> 2253.06]  and I'm already on Amazon
[2253.06 --> 2255.00]  just looking at all the possible Zigbee devices.
[2255.16 --> 2255.82]  In fact,
[2256.14 --> 2259.70]  I want to install LED lights
[2259.70 --> 2261.14]  in the wheel wells of jupes
[2261.14 --> 2262.46]  to help with rodents and stuff.
[2262.84 --> 2264.70]  And I don't want an LED light strip.
[2265.04 --> 2265.92]  I would like,
[2266.10 --> 2266.44]  you know,
[2266.64 --> 2268.02]  a big bright light
[2268.02 --> 2268.96]  that is Zigbee
[2268.96 --> 2270.90]  that's DC powered
[2270.90 --> 2272.10]  that I could mount in there
[2272.10 --> 2273.98]  and then home assistant could turn on
[2273.98 --> 2274.50]  in the evening
[2274.50 --> 2275.50]  and turn off in the morning
[2275.50 --> 2277.46]  and shine light down on the ground.
[2277.46 --> 2279.60]  And I've seen lots of light strips
[2279.60 --> 2283.64]  I can find lots of DC power Zigbee controllers,
[2284.10 --> 2286.58]  but I would like a mountable LED light.
[2286.80 --> 2287.62]  I haven't seen it.
[2287.66 --> 2288.00]  And of course,
[2288.02 --> 2289.54]  it'd have to be really weatherproof
[2289.54 --> 2290.78]  because it'd be in the wheel well.
[2291.24 --> 2292.92]  So you're going down the road with rain.
[2293.32 --> 2294.28]  But that's my next thing.
[2294.36 --> 2297.60]  I want to just kind of convert over.
[2297.96 --> 2299.56]  I'd like to get some Zigbee lighting.
[2300.12 --> 2301.82]  I got to replace some of my light strips.
[2302.24 --> 2302.38]  You know,
[2302.38 --> 2303.46]  I got to do some of that crap.
[2303.64 --> 2304.90]  There's some bulbs
[2304.90 --> 2306.62]  and some smart plugs
[2306.62 --> 2308.24]  and a lot of sensors.
[2308.24 --> 2310.50]  It does seem to work really well.
[2310.76 --> 2312.86]  And I was impressed with the performance
[2312.86 --> 2314.82]  and the fact that its battery life
[2314.82 --> 2316.44]  is supposedly pretty good
[2316.44 --> 2318.36]  and it's still giving me near real time data.
[2318.66 --> 2320.28]  As we're doing the show here,
[2320.62 --> 2321.80]  I'm watching the temperature
[2321.80 --> 2322.76]  in the studio garage
[2322.76 --> 2324.42]  just go up and up and up in real time.
[2324.62 --> 2325.30]  It's wonderful.
[2325.66 --> 2326.48]  Oh, that's fun.
[2326.60 --> 2327.14]  Yeah, useful.
[2327.30 --> 2328.04]  Isn't that great?
[2328.10 --> 2330.38]  Do you have also a Zigbee anxiety sensor
[2330.38 --> 2331.18]  to go with that?
[2331.58 --> 2332.70]  I will soon probably.
[2333.06 --> 2334.60]  I'm checking Alibaba every day now.
[2334.82 --> 2336.58]  There's all kinds of crazy Zigbee devices.
[2336.58 --> 2338.50]  So I think, yeah,
[2338.60 --> 2340.14]  wheel well lights would be my next thing.
[2340.30 --> 2340.98]  Temperature sensors,
[2341.10 --> 2342.04]  just getting them replaced,
[2342.36 --> 2344.18]  just phasing out the Z-Wave stuff.
[2344.28 --> 2345.42]  So if you got any tips out there,
[2345.84 --> 2346.50]  let me know.
[2346.84 --> 2348.02]  Of course, you can always tell us in person
[2348.02 --> 2349.28]  because the West Coast meetups
[2349.28 --> 2351.48]  are coming up soon too.
[2352.04 --> 2353.36]  Details at meetup.com
[2353.36 --> 2354.68]  slash Jupiter Broadcasting.
[2355.20 --> 2356.36]  We have a lot of events.
[2356.62 --> 2358.08]  We have a Southern Oregon event.
[2358.14 --> 2359.72]  We have a Northern California event.
[2359.78 --> 2361.44]  We have a Southern California event.
[2362.28 --> 2364.16]  We have random meetups we'll do
[2364.16 --> 2365.04]  called micro meetups
[2365.04 --> 2366.06]  as we're going down the road.
[2366.18 --> 2367.56]  And we have all of them listed out
[2367.56 --> 2368.92]  at meetup.com
[2368.92 --> 2370.16]  slash Jupiter Broadcasting.
[2370.70 --> 2372.30]  Finalizing the details right now,
[2372.36 --> 2373.62]  as Alex and I are recording,
[2374.28 --> 2375.74]  the wife lady is chatting
[2375.74 --> 2376.58]  with our insiders
[2376.58 --> 2378.90]  in our Matrix West Coast crew room,
[2379.20 --> 2381.36]  bit.ly slash West Coast crew.
[2381.82 --> 2383.72]  And they're in there chatting details.
[2384.14 --> 2385.62]  We were all set and ready
[2385.62 --> 2387.46]  to go to McMinimins in Portland.
[2387.92 --> 2389.06]  We have a listener that works there
[2389.06 --> 2389.82]  that invited us
[2389.82 --> 2391.44]  and even offered a spot for Jupes to park.
[2391.60 --> 2392.34]  Like, sweet, right?
[2392.34 --> 2393.66]  And we're like, awesome.
[2393.74 --> 2394.66]  This is going to be great.
[2395.24 --> 2396.20]  We'll get like, you know,
[2396.24 --> 2397.36]  the inside scoop
[2397.36 --> 2398.54]  because the guy works there.
[2398.96 --> 2400.58]  And then as they're figuring out details,
[2400.66 --> 2402.02]  we realize there's like
[2402.02 --> 2403.22]  a really well-known band
[2403.22 --> 2404.12]  coming in that night
[2404.12 --> 2405.34]  and the place is going to be
[2405.34 --> 2407.04]  absolutely slammed.
[2407.30 --> 2408.44]  And that's the kind of details
[2408.44 --> 2409.70]  we just wouldn't know
[2409.70 --> 2411.42]  unless we were talking to locals
[2411.42 --> 2413.04]  in that Matrix chat room.
[2413.32 --> 2414.60]  And so we caught that
[2414.60 --> 2415.56]  and we're pivoting
[2415.56 --> 2416.54]  and we're figuring that out.
[2416.56 --> 2417.94]  But those kinds of little details,
[2418.08 --> 2419.22]  they save the day.
[2419.22 --> 2420.74]  So if you're on the West Coast
[2420.74 --> 2421.88]  and you're going to be anywhere near
[2421.88 --> 2422.54]  where we're doing a meetup,
[2422.60 --> 2423.62]  we could use your brain.
[2423.94 --> 2425.82]  Bit.ly slash West Coast crew.
[2426.44 --> 2427.62]  I think the JPL,
[2427.80 --> 2428.88]  by the time we do the next episode,
[2428.96 --> 2430.22]  we'll have the JPL names too
[2430.22 --> 2431.74]  for folks that are making it.
[2431.88 --> 2432.42]  Alex will be there.
[2432.72 --> 2432.92]  Yeah.
[2433.20 --> 2434.30]  Yeah, you try and stop me.
[2434.50 --> 2435.90]  I think you'll be at the Southern meetup too
[2435.90 --> 2438.38]  that we have outside of the JPL event as well.
[2438.96 --> 2439.46]  Yeah, hopefully.
[2439.58 --> 2441.20]  I'm going to be trying to do,
[2441.34 --> 2442.44]  I think, three or four days
[2442.44 --> 2444.60]  in the LA, Pasadena area
[2444.60 --> 2446.14]  around the meetup.
[2446.52 --> 2448.36]  So really looking forward to it.
[2448.36 --> 2449.26]  Yeah, must be honest.
[2449.58 --> 2450.38]  It's going to be nerdy.
[2450.46 --> 2451.10]  It's going to be fun.
[2451.18 --> 2452.28]  It's going to be good to get together
[2452.28 --> 2454.60]  and hopefully it won't be so hot.
[2454.96 --> 2456.64]  I'm just taking a sip
[2456.64 --> 2459.06]  from my Pop! OS mug glass
[2459.06 --> 2461.16]  that I got on our last factory tour.
[2461.62 --> 2463.42]  I don't wish to poo-poo System 76
[2463.42 --> 2465.18]  because that was a really fun tour,
[2465.30 --> 2468.08]  but I think JPL might be slightly cooler.
[2468.38 --> 2469.06]  Just a little bit.
[2469.38 --> 2471.38]  It's going to be a real memory.
[2471.96 --> 2472.54]  They're both cool.
[2472.68 --> 2473.18]  Let's be fair.
[2473.82 --> 2475.60]  So I've reached into our boost bag
[2475.60 --> 2476.12]  and I've pulled out
[2476.12 --> 2477.36]  like our top five boosts this week.
[2477.36 --> 2478.20]  These aren't all of them,
[2478.26 --> 2480.72]  but we did 100% read all of them.
[2480.78 --> 2481.70]  So thank you, everybody,
[2481.70 --> 2482.74]  who boosted in.
[2483.12 --> 2483.70]  We're just going to pick
[2483.70 --> 2484.60]  a few of them this week
[2484.60 --> 2485.50]  to keep things moving.
[2485.66 --> 2486.48]  Prozac boosted in
[2486.48 --> 2487.26]  with a row of ducks,
[2487.38 --> 2489.42]  2,222 sats
[2489.42 --> 2490.58]  with his new podcast app.
[2490.62 --> 2490.84]  He says,
[2490.90 --> 2491.40]  Hello, guys.
[2491.82 --> 2493.36]  I'm listening to episode 77
[2493.36 --> 2494.80]  about the constant issues
[2494.80 --> 2495.64]  with Home Assistant.
[2496.14 --> 2497.76]  Have you considered moving
[2497.76 --> 2498.86]  to something like Hubitat?
[2499.54 --> 2501.10]  They sell an AIO hub
[2501.10 --> 2502.78]  with Z-Wave and Zigbee built in.
[2503.42 --> 2504.58]  It's a full device,
[2504.58 --> 2505.24]  ready to go.
[2505.24 --> 2506.28]  The platform has allowed me
[2506.28 --> 2507.92]  to focus on the automation aspects
[2507.92 --> 2509.90]  rather than managing Haas.
[2510.54 --> 2512.48]  And everything is locally processed.
[2513.16 --> 2513.70]  And I went and looked.
[2513.78 --> 2514.48]  They have a device
[2514.48 --> 2515.62]  like ready to go, Alex.
[2515.92 --> 2516.16]  I don't know.
[2516.20 --> 2517.18]  It doesn't seem like the solution for me.
[2517.24 --> 2518.38]  I like having my own hardware.
[2519.66 --> 2521.36]  But has the idea
[2521.36 --> 2522.66]  of switching away from Home Assistant
[2522.66 --> 2523.56]  crossed your mind at all?
[2523.60 --> 2524.74]  Or is that just not an area
[2524.74 --> 2525.54]  you're willing to go to?
[2526.08 --> 2526.82]  It's crossed my mind
[2526.82 --> 2528.28]  typically when I'm talking to you
[2528.28 --> 2530.38]  because you're a cranky old man
[2530.38 --> 2531.24]  about it these days.
[2531.24 --> 2533.58]  But I don't know.
[2533.66 --> 2534.96]  Maybe we should get some hardware
[2534.96 --> 2535.76]  in for testing, right?
[2535.84 --> 2538.56]  Maybe we should write it off
[2538.56 --> 2539.84]  as a tax write-off or something.
[2539.92 --> 2540.62]  Get it in for testing
[2540.62 --> 2541.36]  or something like that.
[2542.00 --> 2542.82]  Hubitat, reach out.
[2543.14 --> 2544.48]  I would give it a test.
[2545.20 --> 2546.06]  Kaspilin boosted in
[2546.06 --> 2547.86]  with 36,900 sats.
[2547.92 --> 2548.14]  He says,
[2548.22 --> 2549.68]  Hey, self-hosters.
[2550.14 --> 2550.90]  I need to confess.
[2550.98 --> 2552.04]  I'm one of the lizard people.
[2552.48 --> 2553.42]  I mean, it's a Seuss user.
[2554.08 --> 2555.92]  I found Linux when I was 15 years
[2555.92 --> 2556.92]  or something like that.
[2557.38 --> 2558.10]  You're old.
[2558.90 --> 2560.06]  I was at the Sea Scouts
[2560.06 --> 2561.02]  and my troop leader used
[2561.02 --> 2562.94]  Seuss version 9.2.
[2563.08 --> 2563.96]  That started my adventure
[2563.96 --> 2565.08]  and I never looked back.
[2565.24 --> 2566.84]  It was Windows XP days back then.
[2567.18 --> 2567.96]  I learned VMware,
[2568.34 --> 2569.02]  then Docker.
[2570.04 --> 2570.86]  And I know you guys these days
[2570.86 --> 2572.44]  talk a lot about NixOS and friends,
[2572.60 --> 2574.38]  but have you tried out Seuss
[2574.38 --> 2575.28]  and AutoYest?
[2575.62 --> 2576.68]  It's become my standard.
[2576.96 --> 2577.82]  Thanks for the work.
[2578.44 --> 2580.26]  Yeah, we actually got a lot of people
[2580.26 --> 2582.70]  who are Seuss fans in the audience.
[2582.84 --> 2583.66]  I guess people like it
[2583.66 --> 2584.34]  for their home labs
[2584.34 --> 2586.68]  because also Colin boosted
[2586.68 --> 2588.80]  with 5,436 sats
[2588.80 --> 2589.00]  says,
[2589.08 --> 2590.78]  I also wanted to give a big thumbs up
[2590.78 --> 2592.04]  for OpenSeuss.
[2592.38 --> 2594.30]  It's easy to use and powerful.
[2594.78 --> 2596.28]  It's been the center of my home lab
[2596.28 --> 2597.12]  and home automation.
[2598.26 --> 2598.44]  You know,
[2598.62 --> 2600.22]  Seuss was one of the early distros
[2600.22 --> 2601.98]  to let you like define
[2601.98 --> 2603.18]  how you wanted everything set up
[2603.18 --> 2604.00]  in that AutoYest.
[2604.32 --> 2605.58]  So I guess I kind of see
[2605.58 --> 2606.66]  why it could be a good home lab.
[2607.46 --> 2608.78]  It just feels like things have moved on,
[2608.88 --> 2609.02]  but.
[2609.58 --> 2611.60]  They must be very stable
[2611.60 --> 2612.66]  because you never hear
[2612.66 --> 2613.98]  any drama about Seuss,
[2614.04 --> 2614.32]  do you?
[2614.66 --> 2614.98]  Never.
[2615.22 --> 2615.96]  You don't hear people like,
[2616.04 --> 2617.06]  my Seuss machine died.
[2617.14 --> 2617.44]  You're right.
[2618.00 --> 2620.02]  Colin also gives a big plus one
[2620.02 --> 2621.80]  to the Aquara Zigbee temp sensors.
[2622.44 --> 2623.42]  He says he uses them
[2623.42 --> 2624.94]  and the batteries seem to last.
[2625.90 --> 2626.30]  So, okay.
[2627.04 --> 2627.66]  You like them.
[2628.12 --> 2628.88]  Colin likes them.
[2629.84 --> 2631.24]  I really wanted the Shelly one
[2631.24 --> 2632.50]  to work with the e-ink display.
[2632.88 --> 2634.10]  I really wanted that
[2634.10 --> 2635.14]  to be the one I use everywhere
[2635.14 --> 2636.90]  because I like having that display.
[2637.20 --> 2637.98]  I could almost,
[2638.10 --> 2638.20]  I mean,
[2638.22 --> 2639.18]  I bought a couple of them,
[2639.62 --> 2640.84]  so I could just use them for that.
[2640.84 --> 2642.58]  And then Purple Dog
[2642.58 --> 2644.66]  boosted in with our last boost,
[2644.84 --> 2646.08]  2,500 sats.
[2646.74 --> 2647.02]  He says,
[2647.24 --> 2647.46]  okay,
[2647.50 --> 2648.68]  I was listening to the section
[2648.68 --> 2650.20]  where you guys were talking about dying
[2650.20 --> 2651.72]  and leaving access to your loved ones
[2651.72 --> 2653.36]  while I was doing some housework.
[2653.66 --> 2654.86]  I slipped over
[2654.86 --> 2656.22]  and I narrowly avoided
[2656.22 --> 2658.34]  cracking my head on the freezer.
[2658.66 --> 2659.38]  So he decided
[2659.38 --> 2660.06]  it might be a sign
[2660.06 --> 2660.72]  he should boost in.
[2661.16 --> 2661.98]  Foreshadowing much?
[2663.24 --> 2664.34]  We got a row of ducks
[2664.34 --> 2665.30]  from user 604
[2665.30 --> 2666.24]  who recommended people
[2666.24 --> 2667.50]  check out Microtik routers,
[2667.56 --> 2668.60]  which he has been managing
[2668.60 --> 2669.34]  with Ansible.
[2669.66 --> 2672.00]  And then we got 1101 sats
[2672.00 --> 2673.98]  from a deck bot
[2673.98 --> 2674.74]  who suggested
[2674.74 --> 2677.58]  the Pi 4 compute module 4
[2677.58 --> 2680.26]  with OpenWrt installed on it
[2680.26 --> 2681.00]  for a router for me.
[2681.96 --> 2682.88]  That's kind of clever.
[2682.98 --> 2683.16]  He says,
[2683.20 --> 2683.78]  you get the GUI,
[2683.88 --> 2684.70]  you get the SSH,
[2684.88 --> 2685.76]  and you can actually configure
[2685.76 --> 2686.72]  with Ansible scripts too.
[2687.76 --> 2688.12]  Okay.
[2688.50 --> 2689.68]  I like the idea of using,
[2689.76 --> 2691.22]  because I bought the compute module 4
[2691.22 --> 2692.58]  and the carrier board
[2692.58 --> 2693.82]  specifically to be a router.
[2693.82 --> 2695.22]  I hadn't even thought
[2695.22 --> 2696.90]  about OpenWrt on there
[2696.90 --> 2697.62]  to be honest with you.
[2697.68 --> 2698.66]  And I'm sort of silly
[2698.66 --> 2699.38]  because I've actually had,
[2699.84 --> 2700.92]  I really liked it on that slate.
[2701.14 --> 2701.98]  I forgot it was even a thing,
[2702.10 --> 2703.46]  even though it's on that
[2703.46 --> 2705.06]  GL INET slate thing
[2705.06 --> 2706.06]  that I use as well.
[2706.16 --> 2706.80]  Which has been great.
[2707.46 --> 2708.48]  So, yeah.
[2708.88 --> 2709.66]  Hey, if it's good enough
[2709.66 --> 2710.26]  for Starlink.
[2710.52 --> 2710.86]  Right.
[2711.04 --> 2711.40]  It's true.
[2711.48 --> 2712.18]  They're using it on theirs.
[2713.26 --> 2713.70]  RusticCastiversa
[2713.70 --> 2715.46]  also boosted in 2600 sats.
[2716.02 --> 2716.96]  And it sounds like
[2716.96 --> 2718.16]  he's going to be clipping episodes
[2718.16 --> 2719.38]  for us from time to time.
[2719.40 --> 2720.26]  And he already has been
[2720.26 --> 2722.76]  whenever Fountain FM's
[2722.76 --> 2723.72]  transcription is working.
[2724.34 --> 2725.74]  So, he has clips
[2725.74 --> 2726.78]  from various JB shows
[2726.78 --> 2727.56]  and other podcasts.
[2727.70 --> 2728.32]  And I'll put a link
[2728.32 --> 2729.84]  to his Fountain FM profile
[2729.84 --> 2731.50]  for RusticCastiversa
[2731.50 --> 2732.40]  if you'd like to follow him
[2732.40 --> 2733.96]  and get clips from self-hosted
[2733.96 --> 2735.24]  and whatnots.
[2735.54 --> 2736.52]  Which I think is great.
[2736.60 --> 2737.60]  I think we need more of that
[2737.60 --> 2738.24]  in podcasts
[2738.24 --> 2739.16]  because I've been discovering
[2739.16 --> 2741.08]  a lot of shows via clips.
[2741.16 --> 2742.48]  A lot of these new podcast apps,
[2742.80 --> 2743.92]  newpodcastapps.com,
[2744.64 --> 2745.60]  support clips
[2745.60 --> 2746.44]  because that's part of the
[2746.44 --> 2747.70]  podcasting 2.0 standard.
[2748.02 --> 2749.72]  And I have a whole new
[2749.72 --> 2750.56]  batch of podcasts
[2750.56 --> 2751.38]  I'm listening to
[2751.38 --> 2753.38]  because I heard their clips first.
[2753.38 --> 2754.72]  So, thank you Rusticasta.
[2755.18 --> 2756.54]  If you want to get a new podcast app
[2756.54 --> 2757.00]  and boost in,
[2757.12 --> 2758.28]  newpodcastapps.com,
[2758.34 --> 2759.38]  just get one that supports boosts
[2760.06 --> 2760.72]  or try out
[2760.72 --> 2761.38]  Breeze,
[2762.04 --> 2764.06]  B-R-E-E-Z dot technology.
[2764.74 --> 2766.58]  Now, we've got a little sneak peek
[2766.58 --> 2767.56]  at what's coming up.
[2767.80 --> 2768.20]  That's right.
[2768.20 --> 2769.80]  I was lucky enough to get
[2769.80 --> 2771.70]  a notification just in time
[2771.70 --> 2772.94]  from Newegg this week
[2772.94 --> 2776.54]  that their Intel Arc GPU shipment,
[2776.72 --> 2778.36]  the ASRock A380s,
[2778.50 --> 2779.44]  was live.
[2779.54 --> 2780.64]  And I got in the pre-order queue
[2780.64 --> 2782.58]  and I was fast enough,
[2782.64 --> 2783.04]  I guess,
[2783.44 --> 2784.48]  because it shipped this morning.
[2785.04 --> 2785.06]  Wow.
[2785.22 --> 2786.56]  And it's now out of stock again.
[2786.82 --> 2787.12]  Yep.
[2787.24 --> 2787.60]  Already.
[2788.72 --> 2789.54]  That's great.
[2789.66 --> 2789.86]  Yeah.
[2789.92 --> 2791.02]  So, I pre-ordered one for the show.
[2791.10 --> 2791.74]  It's $140,
[2792.30 --> 2792.54]  you know,
[2792.58 --> 2793.02]  plus tax.
[2793.08 --> 2793.86]  I think it came to about
[2793.86 --> 2795.60]  155 shipped or something,
[2795.70 --> 2796.36]  which is not too bad.
[2797.02 --> 2798.34]  And I'll tell you why I'm excited
[2798.34 --> 2799.58]  about this self-hosters.
[2799.70 --> 2800.64]  It's because
[2800.64 --> 2803.38]  the Intel iGPU
[2803.38 --> 2805.18]  that is on my CPU
[2805.18 --> 2806.16]  is,
[2806.34 --> 2806.96]  with QuickSync,
[2807.18 --> 2809.20]  been such a game changer for me
[2809.20 --> 2811.04]  for hardware transcoding purposes.
[2811.84 --> 2812.08]  You know,
[2812.10 --> 2813.56]  I use it for my Blue Iris box.
[2813.96 --> 2815.64]  I use it for Plex and Jellyfin.
[2816.28 --> 2817.66]  Sometimes I even use it
[2817.66 --> 2818.88]  for batch transcoding jobs.
[2818.94 --> 2819.90]  Like before I got on the plane,
[2819.96 --> 2821.16]  I just queued up a bunch of stuff
[2821.16 --> 2822.04]  with FFmpeg
[2822.04 --> 2823.50]  and it just worked great.
[2824.68 --> 2825.28]  And I'll tell you why
[2825.28 --> 2826.02]  I'm super excited
[2826.02 --> 2827.90]  about these Intel Arc GPUs.
[2827.96 --> 2828.44]  It's because they have
[2828.44 --> 2830.12]  QuickSync hardware built into them,
[2830.72 --> 2832.10]  including the brand new
[2832.10 --> 2833.44]  AV1 codex.
[2834.16 --> 2834.70]  And so,
[2834.80 --> 2835.92]  I'm really looking forward
[2835.92 --> 2836.94]  to putting this through its paces.
[2837.06 --> 2837.60]  I'm hoping
[2837.60 --> 2838.72]  I'm going to be able
[2838.72 --> 2840.08]  to do some GPU pass-through
[2840.08 --> 2840.48]  with it
[2840.48 --> 2841.64]  and eventually get rid
[2841.64 --> 2843.40]  of my Blue Iris dedicated box
[2843.40 --> 2844.38]  and then just have
[2844.38 --> 2845.18]  the Windows VM
[2845.18 --> 2846.62]  with this GPU.
[2847.06 --> 2848.62]  And if it all works,
[2848.94 --> 2850.06]  you will hear all about it
[2850.06 --> 2850.58]  on the show
[2850.58 --> 2851.54]  and it will be coming up
[2851.54 --> 2852.90]  over the next few episodes.
[2853.42 --> 2854.04]  I hope we hear about it
[2854.04 --> 2855.26]  if it doesn't work, too.
[2855.40 --> 2855.64]  Well,
[2856.00 --> 2857.18]  with the state of the
[2857.18 --> 2858.28]  Intel Arc drivers,
[2858.36 --> 2858.96]  by all accounts,
[2859.00 --> 2860.10]  that's probably the likely
[2860.10 --> 2861.30]  scenario to start with.
[2862.20 --> 2862.60]  Wow,
[2862.68 --> 2862.96]  that's right.
[2862.96 --> 2863.68]  I'm really glad
[2863.68 --> 2864.68]  you were able to get one
[2864.68 --> 2866.44]  before they were out of stock again.
[2866.52 --> 2867.94]  That is so cool.
[2868.68 --> 2868.92]  Well,
[2869.10 --> 2870.50]  if you are listening
[2870.50 --> 2870.90]  and thinking,
[2871.00 --> 2872.06]  I hope they're not wrapping up,
[2872.16 --> 2872.32]  well,
[2872.36 --> 2873.34]  I've got bad news for you.
[2873.46 --> 2874.08]  We are,
[2874.26 --> 2875.08]  unless you're a member
[2875.08 --> 2875.98]  because our members
[2875.98 --> 2877.60]  get a bonus post show
[2877.60 --> 2878.66]  every single week
[2878.66 --> 2879.32]  as a thank you
[2879.32 --> 2880.80]  for being one of our SREs.
[2880.96 --> 2882.02]  You support the show,
[2882.44 --> 2883.62]  you get an ad-free feed
[2883.62 --> 2884.78]  as a little bit of a thank you
[2884.78 --> 2885.68]  with that post show,
[2885.88 --> 2887.12]  and you keep us going
[2887.12 --> 2888.14]  and keep us independent.
[2888.42 --> 2889.02]  You can sign up
[2889.02 --> 2890.10]  at selfhosted.show
[2890.10 --> 2890.94]  slash SRE
[2890.94 --> 2893.04]  or support all the shows
[2893.04 --> 2893.48]  on the network
[2893.48 --> 2894.02]  and get access
[2894.02 --> 2894.92]  to the special features
[2894.92 --> 2896.78]  for every single JB show,
[2897.04 --> 2898.56]  including every ad-free version
[2898.56 --> 2900.50]  at jupiter.party.
[2900.50 --> 2901.94]  And then don't forget
[2901.94 --> 2902.80]  those meetups
[2902.80 --> 2903.62]  on the West Coast,
[2904.22 --> 2904.92]  meetup.com
[2904.92 --> 2906.30]  slash jupiter broadcasting.
[2906.74 --> 2906.76]  Yeah,
[2906.80 --> 2907.54]  I very much look forward
[2907.54 --> 2908.44]  to seeing those of you
[2908.44 --> 2909.32]  that are down in LA.
[2909.60 --> 2909.84]  You know,
[2909.92 --> 2910.88]  I won't catch the guys
[2910.88 --> 2911.44]  up in the North,
[2911.56 --> 2913.26]  but maybe next time.
[2913.74 --> 2914.40]  As always,
[2914.48 --> 2914.96]  the place to go
[2914.96 --> 2915.78]  to get in touch with us
[2915.78 --> 2917.26]  is selfhosted.show
[2917.26 --> 2918.18]  slash contact.
[2918.58 --> 2919.04]  Or Twitter.
[2919.22 --> 2920.28]  You can always tweet the show
[2920.28 --> 2921.22]  at selfhostedshow
[2921.22 --> 2922.92]  and I'm at Chris LAS.
[2923.30 --> 2924.26]  And the show is over there
[2924.26 --> 2925.40]  at selfhostedshow.
[2925.64 --> 2926.32]  Thanks for listening,
[2926.42 --> 2926.70]  everybody.
[2926.70 --> 2928.28]  That was selfhosted.show
[2928.28 --> 2929.36]  slash 78.
[2930.50 --> 2960.48]  Listen to the show
