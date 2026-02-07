[0.00 → 1.48] Now, Reddit made me do this.
[1.70 → 4.38] I was browsing, I think it was r slash Linux the other day,
[4.48 → 8.42] and I became aware that you can actually configure TOP.
[8.52 → 9.12] Did you know this?
[9.70 → 11.30] I saw this post.
[11.64 → 15.74] I got to admit, I had no idea that TOP could expose somewhere this data.
[16.04 → 18.66] I feel a little embarrassed because I probably used TOP
[18.66 → 20.40] for longer than some of my kids have been alive.
[20.80 → 21.10] Right.
[22.12 → 23.70] So for those of you that don't know,
[24.20 → 28.26] TOP is the beautiful version of TOP, the process manager.
[28.26 → 29.86] It lets you look at all the running processes
[29.86 → 31.90] and sort them basically by CPU percentage.
[33.40 → 36.56] If you press F2, though, you can get into the setup screen
[36.56 → 39.20] and you can configure all sorts of goodies in there.
[39.28 → 42.48] Like you can show CPU frequency, CPU temperature.
[42.48 → 47.86] You can show disk IO, network, receive, transmit, all that kind of stuff.
[48.56 → 53.32] It's honestly one of those things that I've seen those little function row,
[53.40 → 56.72] that little function row on the bottom of TOP for the last 10 years.
[56.72 → 58.90] And I've just ignored it.
[59.50 → 61.30] But Reddit made me do it.
[61.66 → 65.58] I mean, I guess there is an upside to doom-scrolling Reddit from time to time.
[66.76 → 67.16] Occasionally.
[67.24 → 67.86] Those are the nuggets.
[68.10 → 68.98] This is why we scroll.
[69.54 → 72.36] You know, it's even gotten worse now because, you know, I'm an Android user now.
[72.46 → 73.52] Oh, yes, that's right.
[73.58 → 73.74] Yeah.
[73.90 → 74.14] Yeah.
[74.34 → 74.62] Right.
[74.76 → 74.94] Right.
[74.96 → 76.08] I'm an Android guy now.
[76.26 → 78.94] And I had to give me a decent Reddit app.
[78.94 → 82.06] So I got the Infinity app for Android.
[82.90 → 84.46] Legit recommend this Android app.
[84.52 → 86.86] This is a great Reddit client.
[87.48 → 89.68] But it has this feature called Lazy Mode.
[90.40 → 96.84] And by default, you turn on Lazy Mode and every 2.5 seconds, it just auto scrolls Reddit for you.
[96.84 → 102.10] So if you just want to, like, lay there on the couch with your phone up, it'll just auto scroll.
[102.36 → 104.10] And then if you tap into a post, it pauses.
[104.32 → 106.98] So you can, you know, doom scroll the comments for a bit.
[107.06 → 110.80] And then when you're ready to bail, and you go back, it just starts scrolling again.
[111.18 → 111.90] Oh, my God.
[112.36 → 112.72] Dude.
[113.60 → 114.72] You need help.
[116.08 → 117.16] Actually, you know what?
[118.00 → 119.62] It's good for RSI.
[119.92 → 121.08] Because that's swiping.
[121.60 → 123.26] You know, it wears the fingers down.
[123.42 → 125.06] It's not good for the fingers, Alex.
[125.06 → 125.22] Alex.
[125.66 → 127.52] It's not good for the mind either, Chris.
[129.68 → 133.22] Says the guy who started with a Reddit client or a Reddit topic.
[133.58 → 139.78] Anyway, I'll throw a link to Infinity for Reddit in the show notes, too, because I do give it actually a perfect big recommendation.
[139.94 → 140.90] It's a great little client.
[141.22 → 141.82] So there.
[142.26 → 143.08] So there.
[143.70 → 144.10] Unbelievable.
[144.68 → 149.98] Well, I have a little call-out I'd like to make before we start or a little request, I guess, for help.
[149.98 → 160.58] I'm I'm collecting input on what the audience does in general for I'm I'm coming home type notifications and automations.
[160.58 → 173.24] So when I was an iPhone user, Alex, when I used iOS like you, Alex, I took advantage of the iOS shortcuts, which is a brilliant tool in iOS now.
[173.24 → 181.58] And I had a little automation that would trigger, and it would send the wife a text message with a notification that I'm on my way home.
[181.66 → 184.80] It would look at my current location so I could trigger this anywhere.
[185.08 → 195.98] And then it would send her a time estimation for how long until I'm you know, I could tie this with triggering lights and doing other automations as well if I wanted to, which I may or may not ever need to.
[195.98 → 199.50] And so I'm wondering if people have a home assistant solution for this with Android.
[199.94 → 204.00] I've got those little NFC tags so I could easily scan an NFC tag.
[204.32 → 212.74] But one of the things I honestly don't really know how to do well in home assistant is actually how to send out notifications to external messaging platforms like, say, Telegram.
[212.84 → 214.72] I could send her a Telegram message, for example.
[214.92 → 216.26] I've never done that with home assistant.
[216.38 → 217.80] I'm not even sure if that's the right way.
[218.16 → 222.88] And I'm just wondering if people do something like this and what they've done and if they could share it with me.
[222.92 → 223.48] Have you done?
[224.36 → 225.72] Have you done anything like this?
[225.72 → 229.40] Do you let Kat know like any kind of automations for when you're travelling or stuff like that?
[229.82 → 235.28] I don't specifically send notifications from home assistant, but we've covered what I think will end up being your solution.
[235.72 → 236.78] Do you remember Apprise?
[237.40 → 238.44] No, no.
[238.66 → 238.96] Geez.
[239.26 → 241.66] Well, we covered this on the show back in episode 48.
[242.16 → 247.54] An Apprise is basically just a notification kind of consolidation framework.
[247.72 → 254.04] So rather than you having to integrate Home Assistant with three or four different notification services,
[254.04 → 260.92] you integrate with Apprise, and then they integrate with Telegram or Pushover or whatever it might be.
[261.58 → 266.10] And so you can just configure in Home Assistant using the Apprise URL that you have,
[266.52 → 271.36] send a notification containing this content, and you can do all the kind of interesting
[271.36 → 275.12] emulating state stuff you can do with Home Assistant's emulating language.
[275.36 → 280.96] You can configure that to be the notification, you know, with your current location and estimated time
[280.96 → 282.88] to come back, that kind of stuff.
[283.42 → 287.76] And then that way, if you ever want to dump Telegram for something else, a little more freedom
[287.76 → 290.48] respecting, that seems to be your current trajectory at the moment.
[291.14 → 295.42] You know, you can do that without having to completely rewrite everything in Home Assistant.
[295.42 → 298.80] This is exactly what I need to dig into, isn't it?
[299.36 → 300.78] I am so glad you remembered this.
[301.46 → 302.10] You're right.
[302.26 → 305.86] And I also could definitely see moving away from Telegram.
[306.04 → 309.00] I do not like the trajectory of Telegram in general.
[309.14 → 311.48] And I've been experimenting with Fluffy Chat.
[312.34 → 313.52] Yes, Fluffy Chat.
[313.90 → 316.64] That is a Silicon Valley whiteboard.
[317.12 → 318.30] I can just picture it right now.
[318.36 → 322.06] There's 15 different app names, and they've circled Fluffy Chat as the one.
[322.20 → 322.94] Oh, my God.
[322.94 → 326.74] But maybe the cute name will help with spousal approval factor.
[327.10 → 327.60] I don't know.
[327.70 → 331.84] Maybe it's an early days Telegram when the Telegram UI was a lot simpler.
[332.00 → 334.22] It looks a lot like that, but it's a front end to Matrix.
[334.94 → 339.02] So I'm hoping maybe I could move some family members that direction.
[339.58 → 345.54] Now, in terms of triggers on the Android side, I'm not sure quite what Graphene or Cali or
[345.54 → 347.34] wherever you're on this week supports.
[347.74 → 352.58] But what I'd probably be tempted to do is look into, are you familiar with Tasked?
[352.94 → 353.36] Yes.
[353.36 → 354.92] I used to use Tasked back in the day.
[355.22 → 355.34] Yeah.
[355.42 → 358.16] It's not the most user-friendly of applications.
[358.16 → 365.04] It does take quite a few batteries to be included before it is usable by humans, in my opinion.
[365.30 → 373.26] But for more complex automations and the stuff like you're talking about, Apple does the plumbing for you on shortcuts.
[373.26 → 379.44] On the Android side, obviously, you know, user build its own fiefdom instead.
[380.30 → 381.58] That's probably what you want to look at.
[381.64 → 382.40] Something like Tasked.
[382.44 → 383.28] There might be other options.
[383.38 → 390.48] And if you do happen to know any better options than Tasked these days, let us know at self-hosted. Show slash contact.
[390.48 → 394.26] Linode.com slash SSH.
[394.34 → 399.20] Go there to get $100 towards an account when you sign up, and it's a great way to support the show.
[399.72 → 402.54] Linde's how we host everything that we want to run in the cloud.
[402.80 → 405.62] It's a nice mix of power and control over a system.
[405.72 → 407.24] You can build it up from the ground up.
[407.32 → 409.18] I mean, that's how I've got Nix OS on there.
[409.18 → 415.84] Or you can go with one of their ready-to-go images, including like an Ubuntu or Debian stack with Docker pre-deployed.
[415.88 → 418.54] And then you just hit the button and get the image on there.
[418.56 → 421.02] It really kind of depends on what you are comfortable with.
[421.10 → 423.98] So it makes it really approachable for all types.
[424.08 → 430.00] People have been racking and stacking for 20 years and folks that are just spinning up their first server.
[430.12 → 432.54] And Linde makes it really easy to get going in a few clicks.
[432.58 → 436.46] And with that $100 while you're supporting the show, you can try out all kinds of features.
[436.46 → 442.12] Beyond just running a server, they have big, powerful CPUs, and they have big, powerful GPUs.
[442.16 → 446.76] And, of course, they've got superfast disk systems, and they've got a whole range, including anodes,
[446.82 → 452.58] which are great for just a blog or a gallery, maybe a landing page or a status page, or a VPN.
[452.78 → 458.56] In fact, I'll link in the show notes to a guide to set up your own self-hosted VPN on Linde in under 30 minutes.
[458.82 → 459.34] It's pretty nice.
[459.42 → 461.86] And I love Linde's S3-compatible object storage.
[461.94 → 464.58] I recommend you play around with that for your backups as well.
[464.58 → 469.28] It's a great way to get your data that's on-site on your LAN off-site somewhere.
[469.68 → 473.58] You encrypt it, send it up, put it on S3-compatible object storage on Linde.
[473.64 → 474.84] That's a great way to try out the $100.
[475.36 → 477.08] They have a powerful DNS manager.
[477.34 → 482.50] If you like to use orchestration management tools like Ansible, Terraform, Kubernetes, all that stuff,
[482.84 → 484.54] Linde has fantastic support for that.
[485.00 → 485.92] Super-fast networking.
[486.08 → 487.70] They've got 11 data centres around the world.
[487.78 → 490.76] That's one of the reasons I've chosen them is performance really matters.
[490.80 → 492.70] And they've got it in the compute area.
[492.70 → 494.24] They've got it in the disk IO area.
[494.54 → 496.96] They have 40 gigabit connections to the hypervisors.
[497.08 → 498.70] They are their own ISP.
[500.20 → 501.66] Have I mentioned that recently?
[501.72 → 502.42] That's a huge deal.
[502.64 → 505.48] And they're spinning up another dozen next year.
[505.72 → 510.56] So with pricing 30% to 50% cheaper than those big hyperscalers that want to lock you into their platform,
[510.92 → 512.70] with $100, you're getting free credit.
[513.14 → 514.22] And it's a great way to support the show.
[514.32 → 515.36] Why not go check them out?
[515.84 → 517.16] Their community support runs deep.
[517.26 → 519.04] Their commitment to these platforms runs deep.
[519.38 → 521.10] And they've been doing it for nearly 19 years.
[521.10 → 527.92] So go sign up today, support the show, and get $100 to try it out when you go to linode.com slash SSH.
[528.00 → 531.02] That's linode.com slash SSH.
[531.02 → 543.22] Now, talking of privacy respecting changes, this week I've made a change on my personal blog that I've been meaning to make for a year plus.
[543.60 → 549.16] The final nail in the coffin was I was at reinvent in Las Vegas last week or the week before.
[549.16 → 556.74] And I was browsing without an ad blocker for the first time, you know, in some time, to be honest with you.
[556.74 → 561.22] Because even when I'm out and about, I use Tail scale to route back through my home network, typically.
[561.98 → 565.22] And for whatever reason, my hotel Wi-Fi just didn't work with that.
[565.28 → 566.18] So I just turned it off.
[566.56 → 569.78] I went to my personal blog to put on the pictures of the desert that I took.
[570.00 → 573.02] And I was like, what are all these adverts in my website?
[573.22 → 574.36] I didn't put them there.
[574.36 → 590.34] And it turns out Disgust, the commenting engine that I've been using, injects tons of really gross adverts into my content, into my website, without me really being aware of it.
[590.94 → 592.88] Well, I had missed this entire thing.
[592.94 → 598.76] And that is extremely frustrating because, like you, I probably would not notice it because I also often run with an ad blocker.
[598.76 → 602.02] And I run with an ad blocker at the network level as well.
[602.24 → 603.86] So it's across all my systems.
[605.20 → 609.46] And by the way, I do pay for memberships for many sites that offer them.
[609.58 → 613.44] Like I just renewed for Pharynx and LWN just this week.
[613.92 → 617.76] But for me, it's a matter of saving bandwidth because I'm on an LTE connection.
[617.76 → 620.98] And I just do not want to download that crap over an LTE connection.
[621.22 → 623.12] So I prefer to block it at the network level.
[623.42 → 631.58] So I guess you were probably a little, I would say, disappointed when you came across this and probably spurred you into action.
[631.58 → 639.50] I was actually really quite angry to the point where I've been putting this project off, and I was like, right, I'm sat in my hotel room with nothing better to do tonight.
[639.96 → 641.30] I'm going to get this done.
[641.30 → 646.76] And so I found this project called Discus, G-I-S-C-U-S.
[646.76 → 653.62] And this uses GitHub notifications to track interactions and comments with your content.
[653.62 → 660.06] So rather than having some third party database I've got to maintain or anything like that, this relies on GitHub.
[660.58 → 668.60] So it means that commenters to my website, you know, being a largely technical kind of blog, need a GitHub account.
[668.78 → 670.36] So I didn't think that was too much of a problem.
[670.36 → 677.50] It means that GitHub takes care of spammers for me as well, which is a huge problem with self-hosted commenting systems.
[678.22 → 690.70] A lot of spammers target Discuss because it's used all over the Internet, whereas Discus is largely a nerd level project and not that many people use it, which I see as a feature.
[690.70 → 694.82] So for me, I was actually thought, right, this ticks all the boxes.
[695.22 → 702.42] I can have a nice self-hosted comment system that integrates with a third party that I trust, GitHub, Microsoft.
[703.54 → 708.68] But I've got, you know, seven, eight years worth of comments on some of these posts.
[708.76 → 711.28] And some of them have had tens of thousands of views.
[711.32 → 715.42] And I thought it would be a shame to lose that context on some of these posts.
[715.42 → 723.58] And so I had to find a way to export the comments from Discuss, which luckily they do provide as a CSV file.
[723.84 → 724.96] Or is it a JSON? I forget.
[725.54 → 729.44] There is a script to export it from the Discuss admin console.
[729.76 → 734.54] Then once I'd exported it, I used a script which I linked to in the blog post, which will be in the show notes,
[734.74 → 744.58] which basically traverses this file and goes through and uses the GitHub API to automatically create a GitHub discussion per post.
[744.58 → 746.28] And import each comment.
[746.82 → 754.02] Now, the downside to this is there isn't a one-to-one mapping between comments on GitHub and comments in Discuss.
[754.70 → 758.06] And the reason for that is because different people have different usernames.
[758.64 → 763.98] And so if you think to yourself, right, well, I'm called Ironic Badger over here, and I'm called Fred28 over there.
[764.48 → 767.90] How is this script possibly going to know who is who?
[767.90 → 775.26] So what it does is it uses my avatar to import all of these comments and say original commenter name was Fred28.
[775.84 → 779.10] And the date and time of the comment was this.
[779.22 → 780.96] And then it shows the text of the original comment.
[781.04 → 782.72] And it's very clear in when it does that.
[783.12 → 785.36] I did run into a couple of API rate limits.
[785.50 → 788.18] It probably took me about an hour to import all of my comments.
[788.18 → 793.88] And I had to try five or six times before I got the API to play nice with everything I was doing.
[793.88 → 797.88] But after that sort of 30 to 60-minute window, it was all good.
[798.46 → 802.28] So what was the process of actually getting the backend software up and running?
[802.34 → 807.02] Because it looks like you don't actually even have to self-host it if you don't necessarily want to.
[807.08 → 808.46] But I assume you probably went that route.
[809.16 → 812.86] So a couple of years ago, I forked the default Ghost Casper theme.
[813.42 → 818.14] And then I used a GitHub action to auto-deploy that theme to my blog using the Ghost API.
[818.14 → 826.00] So whenever I make a change to the theme on GitHub, it automatically pushes those changes to my blog on the internet.
[826.72 → 831.66] And so it was just a case of modifying, because I'm using the Ghost blogging engine,
[832.16 → 836.90] it was just a case of modifying maybe five to ten lines with a script snippet,
[837.02 → 840.94] replacing the Discuss snippet with the Discuss snippet.
[841.24 → 842.98] And it deployed the theme.
[843.20 → 844.22] I refreshed the page.
[844.38 → 845.90] And that was that.
[846.66 → 847.88] I'm just picturing you.
[848.14 → 853.12] So I'm picturing you like dark hotel room, maybe the TV's on.
[853.34 → 854.58] It's Vegas, right?
[854.74 → 858.14] You got like a bright laptop going, and you're hacking away at this.
[858.24 → 861.16] Are you doing like some Uber Eats while you're doing this?
[861.30 → 863.62] I think I might have ordered room service that night, yeah.
[863.64 → 864.02] Okay.
[864.52 → 866.52] And I was watching the World Cup on my iPad,
[866.78 → 869.54] which, by the way, I should probably talk about at some point in this episode,
[869.54 → 875.06] because HD Home Run and Plex has been a godsend throughout the World Cup.
[875.32 → 876.86] But let's finish this topic first.
[876.86 → 878.32] So we'll come back to that one.
[879.12 → 884.34] So what are your thoughts about its obvious dependency on GitHub?
[884.84 → 889.12] Because, I mean, clearly there is a bit of a compromise there, although, I mean, it's checking all the boxes.
[889.38 → 890.78] The compromises make sense.
[890.96 → 894.96] But, you know, that's going to probably be one of the number one red flags in the audience.
[894.96 → 900.96] If you're truly trying to self-host something like this, well, you're just building a dependency on GitHub here.
[901.50 → 905.26] Well, the alternative for me, honestly, because I don't want to turn myself into a content moderator,
[905.26 → 909.38] because our lord and saviour Elon Musk has shown us just how easy that is,
[909.48 → 911.72] is to just not have comments at all.
[911.72 → 913.98] That would honestly be my alternative.
[914.40 → 917.00] My purpose with this blog is to get information out there.
[917.02 → 919.18] And it's the same reason we use Discord in this show.
[919.46 → 922.58] It's the same reason that I'm using GitHub on these comments,
[922.58 → 928.16] is because being a pragmatist at heart, I just want to get s*** done.
[928.58 → 931.08] And sometimes that means making some compromises.
[931.44 → 935.20] And, you know, I give my rationale for why I make certain compromises.
[935.20 → 938.32] And in this case, it's that I don't want to manage spammers.
[939.12 → 940.22] Yeah, I would totally be the same way.
[940.32 → 941.60] I'd just rather not have comments.
[942.90 → 948.36] If I could plug some bot into GitHub and have matrix comment moderation automatically be done,
[948.60 → 950.86] I'd take that dependency right now.
[951.24 → 953.44] It's just such a pain in the neck, and it's such a problem.
[953.56 → 957.82] And the issue is the more scale you have, the better you are at managing it,
[957.82 → 959.30] because the more data points you have.
[959.46 → 961.88] So it just kind of makes sense to centralize that too.
[961.98 → 962.52] I don't love it.
[962.98 → 963.74] I don't love it.
[963.74 → 968.24] But GitHub feels like a fairly safe place, though, certainly for my audience,
[968.38 → 971.16] because most of the people on there have a reputation.
[971.34 → 973.20] They want to kind of uphold at least a little bit.
[973.76 → 976.48] And if they don't, it's very easy to moderate stuff.
[976.70 → 978.94] You know, the one or two bad apples that might come along.
[979.84 → 981.70] Like anything, it's a balancing act.
[981.84 → 986.50] And you have to draw that line yourself and decide where you fall, really.
[987.22 → 990.16] And there are other solutions out there, including just not having comments.
[991.20 → 993.46] Fred 28 for president in the chat, by the way.
[994.28 → 995.62] I don't know where that name came from.
[995.78 → 996.42] I'll vote for Fred.
[997.82 → 999.32] So, yeah, that seems smart.
[999.98 → 1001.06] You know, we do the show live.
[1001.14 → 1003.12] We should mention this from time to time in the actual pod.
[1003.62 → 1008.54] We do the show every other week, Wednesday evenings over at Jupiter.tube.
[1008.60 → 1010.06] That's our self-hosted Peer Tube instance.
[1010.16 → 1011.88] You can actually play back the recordings, too.
[1011.88 → 1016.44] We have the live times at jupiterbroadcasting.com slash calendar.
[1016.66 → 1021.56] But basically, it's 4.30 Pacific, 7.30 Eastern is when we do it every other Wednesday.
[1022.08 → 1026.64] Usually once my little one's in bed, and I've got time to actually think, do the show.
[1027.00 → 1027.64] That helps.
[1027.92 → 1028.08] Yeah.
[1028.48 → 1028.70] Yeah.
[1028.96 → 1029.16] Yeah.
[1029.16 → 1032.88] So I mentioned I teased a little bit about HD Home Run and Plex just now.
[1033.52 → 1036.56] I know we'll get some questions, so I'll just address it right now.
[1037.34 → 1043.14] My old UK server that I've talked about on this show a few times is running an i5-8500.
[1043.64 → 1049.32] So it has a very capable quick sync chip built into the CPU.
[1050.12 → 1052.80] It's the same chip that I use in my server in my basement.
[1052.94 → 1054.14] So I actually have the same motherboard.
[1054.32 → 1058.14] We've talked about this, but I have the same motherboard in the basement here as I do
[1058.14 → 1060.34] at my mother-in-law's house in England.
[1060.94 → 1064.58] And she just recently got fibre to the premises, which is amazing.
[1064.58 → 1068.16] So she's got like 600 Meg upload or something like that.
[1068.34 → 1070.86] It's honestly, it's beautiful.
[1074.16 → 1080.20] So for my purposes, what I did a few weeks before the World Cup was I bought, I used to
[1080.20 → 1083.86] have one, but it got lost in my parents' moves at some point.
[1084.08 → 1088.56] I bought a brand new Squadron HD Home Run device.
[1089.48 → 1094.50] This is, if you're not familiar, an over-the-air network TV tuner.
[1094.58 → 1100.56] That can tune into up to four different TV stations, TV channels, all at once.
[1101.36 → 1103.18] And Plex just picks this up.
[1103.38 → 1108.70] It does some kind of magic DNS, local DNS discovery on the network.
[1108.80 → 1110.18] Oh, that's nice.
[1110.30 → 1113.14] And you go into your admin portal for that particular server.
[1113.66 → 1115.62] And it says, hey, I've picked up this HD Home Run.
[1115.70 → 1117.48] Do you want to add it to your Plex server?
[1117.86 → 1118.78] What's your postcode?
[1118.78 → 1121.32] So that I can pull down the correct EPG data.
[1122.16 → 1126.32] And you're off to the races, maybe within 10 or 15 minutes.
[1126.50 → 1127.64] It's really slick.
[1128.18 → 1131.28] Do you get a fair amount of stations from your place?
[1131.62 → 1134.12] It's Free view in the UK, as what we call it.
[1134.42 → 1137.28] Are you having a family member install this and hook it up for you?
[1137.28 → 1141.90] Well, yes, because it's a network tuner, actually, it worked out really beautifully.
[1142.04 → 1143.62] I know my mother-in-law's house pretty well.
[1143.66 → 1147.76] And she's got this, like, antenna booster thing in the attic.
[1148.14 → 1155.82] And it happens to be right next to where I ran the Ethernet cable for the Wi-Fi that I put in one of the under-eaves areas of her house.
[1156.32 → 1158.34] And so there was a spare Ethernet port.
[1158.46 → 1163.88] And there was a spare power plug and a spare antenna jack all right next to each other.
[1163.88 → 1164.90] Oh, my gosh.
[1165.02 → 1166.76] She was having some renovations done.
[1167.10 → 1171.18] And she's been using this handyman for the last several years.
[1171.26 → 1172.36] So they're on pretty good terms.
[1172.48 → 1176.42] And she just said, hey, Matthew, could you install this for my son-in-law?
[1177.76 → 1180.22] It took him about half an hour, by all accounts.
[1180.84 → 1184.40] Once the signal was in, it came up and said antenna signal strength 100%.
[1184.40 → 1186.54] And it was just good to go.
[1186.70 → 1188.62] So I've been watching the World Cup.
[1188.80 → 1189.98] I've been doing DVR.
[1190.36 → 1192.40] Plex is pretty good at DVR stuff these days.
[1192.40 → 1196.40] You know, you can say record just this episode, record all shows.
[1196.52 → 1199.78] It will do the com skip stuff, if you remember that, from back in the day.
[1200.50 → 1202.26] It's pretty slick, to be honest with you.
[1202.72 → 1210.40] But I just had one of these wow moments where I was in the airport on the way to reinvent in Vegas
[1210.40 → 1214.16] with my iPad on Plex on the airport Wi-Fi,
[1214.62 → 1220.68] watching BBC Live football match on completely self-hosted infrastructure.
[1220.68 → 1222.66] And I'm like, this is awesome.
[1222.84 → 1223.96] This is why we do it.
[1224.48 → 1225.02] That is slick.
[1225.40 → 1226.66] You're kind of making me want one.
[1226.72 → 1230.32] Even though I have no idea how many channels I'd receive, I do like the local news.
[1230.48 → 1232.04] And this would be a great way to get the local news.
[1232.10 → 1236.42] And then I could cancel my, I don't know, it's almost like 70 bucks a month I've been
[1236.42 → 1238.38] conned into to pay for YouTube TV.
[1239.56 → 1243.32] You know if I could get local news, I could drop that.
[1243.52 → 1245.34] I could be happy with that.
[1245.34 → 1249.42] Well, I've got one in the closet behind me that I use for when there's a storm blowing
[1249.42 → 1250.68] through here or something like that.
[1251.56 → 1252.44] Highly recommend it.
[1252.74 → 1253.04] No wonder.
[1253.52 → 1253.82] I wonder.
[1253.90 → 1254.22] All right.
[1254.44 → 1255.56] So we'll put a link to that too.
[1255.64 → 1256.58] I wonder where I'd put it.
[1256.62 → 1257.94] Would I want to install it in the RV?
[1258.12 → 1259.96] Would I want to install it in the studio and stream it?
[1260.44 → 1261.64] It seems like it'd be fun to play with.
[1261.72 → 1267.42] Although it means I'm also kind of like getting more and more hooked into Plex, I guess.
[1267.80 → 1268.18] Is that right?
[1268.18 → 1271.80] Well, you could run a TV headed as well that you don't have to use Plex.
[1271.90 → 1274.50] There are other TV backends available.
[1275.28 → 1280.02] So TV headed is one that I used to use a few years ago with a TV tuner card, a PCI card.
[1280.48 → 1285.06] But the beauty of this HD Home Run box is you don't have to have a dedicated computer, really.
[1285.64 → 1290.02] If you're on your LAN, there are clients available for Android TV.
[1290.32 → 1294.72] I don't know about Apple TV, but certainly for iOS and Android, you just install the app
[1294.72 → 1296.04] and it just comes up straight away.
[1296.04 → 1298.92] I've got something neat for you.
[1299.00 → 1305.02] Go to CrowdStrike.com slash LCE and you can ingest and view all of your logs in one place.
[1305.30 → 1307.50] So this is CrowdStrike Falcon Log Scale.
[1307.68 → 1312.44] This is CrowdStrike's new centralized log management and observability tool, formerly known as Humid.
[1312.78 → 1318.02] So Log Scale has been developed as an alternative to legacy logging solutions that really make
[1318.02 → 1322.16] it cost prohibitive to ingest and search data volumes that you just kind of get if you've
[1322.16 → 1326.14] got some infrastructure, you know, more than a few systems.
[1326.50 → 1328.20] They just generate a ton of logs.
[1328.36 → 1332.66] And the beauty of Log Scale is that it can take logs from any of those sources and make
[1332.66 → 1333.16] them usable.
[1333.72 → 1335.54] You don't need to constantly massage the format.
[1335.80 → 1337.18] Oh, man, I spend time doing that.
[1337.22 → 1338.00] It doesn't need a schema.
[1338.20 → 1338.68] Oh, yep.
[1338.74 → 1339.10] Been there.
[1339.54 → 1342.42] You just pump them all in there, and then you got them when you need them.
[1342.68 → 1343.24] And the dashboard.
[1343.72 → 1343.90] Yep.
[1344.14 → 1344.58] It's great.
[1344.64 → 1345.20] Goes for days.
[1345.56 → 1346.54] This platform is crazy.
[1346.54 → 1352.10] It has an index free architecture, which means you can ingest over a petabyte of data per
[1352.10 → 1357.40] day and search that with sub second latency, not hours, sub second latency.
[1358.12 → 1363.86] And Log Scale is a lot cheaper because that architecture means they don't have a whole big old
[1363.86 → 1364.72] hardware footprint.
[1365.70 → 1366.14] Right.
[1366.76 → 1369.44] They're a lot better than platforms like Splunk or Elastic.
[1369.56 → 1370.06] Thanks to that.
[1370.14 → 1371.24] A lot better for you to run.
[1371.34 → 1372.08] A lot easier, a lot simpler.
[1372.08 → 1376.18] And they also have a community edition that they host.
[1376.18 → 1379.14] Now, the reason why I like to mention this is there are a lot of ways you can do this.
[1379.30 → 1383.46] You know, but I think one of the nice things about a platform like Log Scale is if you're
[1383.46 → 1386.78] going through a period where you're building out your infrastructure, maybe you're troubleshooting
[1386.78 → 1391.34] something, you could pump those logs into Log Scale Community Edition.
[1392.04 → 1396.72] That is the largest no cost data ingestion offering on the market.
[1397.02 → 1397.42] Right.
[1397.96 → 1403.12] Because Log Scale Community Edition allows you to ingest up to 16 gigabytes a day, and you get
[1403.12 → 1404.04] seven days of retention.
[1404.04 → 1405.92] So you can really watch what's going on.
[1405.92 → 1407.72] There's no credit card required, no trial period.
[1408.08 → 1408.80] You get that.
[1409.08 → 1413.80] So you can try that, pump your logs into there, do your troubleshooting, build your infra,
[1414.02 → 1416.60] fix your problems, get it all in one spot on a dashboard.
[1416.98 → 1419.26] It's just great for self-hosted who have a day job.
[1420.20 → 1421.62] And you want to get this stuff fixed.
[1421.68 → 1422.36] You want to enjoy it.
[1422.36 → 1425.32] You want to experiment with this, but you don't want a second job.
[1426.16 → 1427.20] So go try it out.
[1427.24 → 1428.40] It's a great way to support the show too.
[1428.40 → 1434.28] Get started with Log Scale Community Edition for free at CrowdStrike.com slash LCE.
[1434.48 → 1438.20] That's CrowdStrike.com slash LCE.
[1438.20 → 1440.94] All right.
[1440.94 → 1448.76] So I think I came across what might be the ultimate home network PMI kind of HDMI solution
[1448.76 → 1449.32] this week.
[1449.32 → 1454.88] When I looked at all the links in the notes, this is the one that really got my attention
[1454.88 → 1456.92] because this is something I could see some use in.
[1457.00 → 1462.80] So am I understanding that you are now transmitting HDMI signal over your LAN?
[1463.38 → 1464.40] Well, I want to be.
[1464.40 → 1467.22] I can't yet because they're all completely out of stock.
[1467.40 → 1468.56] Oh, okay.
[1468.64 → 1473.24] However, there is a link in the show notes to a YouTube video where I discovered this.
[1473.48 → 1478.66] And essentially, I used to use what were called balloon, I think, connectors back in the day
[1478.66 → 1483.90] where you could run a 1080p signal over a pair of Cat5e cables.
[1484.16 → 1488.52] And you used to have dedicated cables between point A and point B.
[1488.52 → 1497.00] The magic of this is that it just hooks into your normal IP-based network and broadcasts
[1497.00 → 1498.70] traffic over multicast.
[1499.30 → 1501.34] Yeah, that does seem really sweet.
[1502.32 → 1505.82] Do you think if, I mean, if you're using this a lot, do you think you have a sense of how
[1505.82 → 1507.14] much data load it is?
[1507.60 → 1509.10] Well, in the video, he does cover that.
[1509.36 → 1515.78] And it seems to be anywhere from sort of two or three to 10 Meg, depending on the various
[1515.78 → 1516.88] thing that he's watching.
[1516.88 → 1518.38] There is some compression.
[1518.90 → 1524.92] So if you're using this, I mean, he's using it to game on, which I'm not sure about that
[1524.92 → 1525.40] personally.
[1525.84 → 1528.28] But hey, 1080p gaming is a thing for some people.
[1528.46 → 1531.86] I've been using on 4K and what have you, because I play Factor.
[1532.02 → 1533.60] You fancy boy.
[1533.78 → 1534.48] You're so fancy.
[1534.76 → 1536.42] I've been playing so much Dwarf Fortress lately.
[1536.86 → 1543.52] I'm over here gaming on my portable little deck, you know, which I think is a 720p screen.
[1543.76 → 1544.44] Is it even that?
[1544.88 → 1546.56] I think it might be 720p.
[1546.88 → 1548.62] I'm sensitive to compression artifacts.
[1548.88 → 1549.20] I don't know.
[1549.26 → 1552.94] I just, you know, there are things in audio that you probably hear that most people don't
[1552.94 → 1553.10] hear.
[1553.18 → 1555.80] For some reason, I'm sensitive to video compression artifacts.
[1555.92 → 1556.74] No, that's fair.
[1556.78 → 1557.60] It is what it is.
[1558.04 → 1563.54] But essentially, this thing, you've got to have a solid network because multicast itself
[1563.54 → 1565.44] can be a network killer.
[1565.44 → 1571.52] So certain switches have the ability to turn on and off multicast support for various different
[1571.52 → 1571.98] ports.
[1572.50 → 1577.20] That may or may not be a requirement depending on how many devices you're throwing into the
[1577.20 → 1577.66] mix here.
[1577.66 → 1583.00] So, you know, until I get one of these things in my hands, I'm not going to be able to really
[1583.00 → 1585.54] give you a proper review on it.
[1585.88 → 1589.84] However, I'll give you a quick overview on why I think it's the ultimate KVM solution.
[1590.56 → 1595.08] So these devices can pass through the HID, so a keyboard and mouse input.
[1595.08 → 1598.26] They have a transmit box and a reception box.
[1598.78 → 1604.88] So I'm picturing down in my basement, I put the transmit box on my server and a second one
[1604.88 → 1607.00] on my Open Sense router.
[1607.84 → 1609.60] So I've got two down there in the basement.
[1610.04 → 1613.90] And then up here, I've got a screen over in the corner where I can have the reception
[1613.90 → 1616.64] module and over the Ethernet.
[1617.04 → 1623.28] So these two transmit boxes transmit on channel one and channel two across the entire network.
[1623.28 → 1629.76] So wherever I want to plug into these systems, all I have to do is have a receiver and change
[1629.76 → 1631.16] the channel on the receiver.
[1631.92 → 1635.20] And then suddenly I can view channel one, channel two, three.
[1635.46 → 1641.22] I think it supports up to 13 source devices and up to 253 receivers.
[1641.44 → 1645.86] That'd be kind of a fun thing to set up around the house and pipe your video around.
[1646.06 → 1648.26] I'm thinking for Blue Iris or something like that.
[1648.30 → 1650.86] You could have the screen up there and then just, oh, right.
[1650.88 → 1652.84] I actually want to go and check my server right now.
[1652.84 → 1653.70] Book, change.
[1654.12 → 1654.24] Yeah.
[1654.32 → 1656.20] Or a dashboard, perhaps.
[1656.28 → 1659.56] You want to bring a dashboard onto a screen in your bedroom or something like that.
[1659.62 → 1660.68] That could be really awesome.
[1661.46 → 1662.88] You would say in the bedroom.
[1663.36 → 1664.08] Oh, yeah.
[1664.52 → 1664.76] You know?
[1665.08 → 1666.82] No, you want to turn on.
[1667.06 → 1667.82] So what was that?
[1667.86 → 1669.82] You turn on the TV, and it's already there.
[1669.90 → 1671.30] It's already the input on the TV.
[1671.56 → 1672.94] Hades is a lucky lady.
[1672.94 → 1676.56] I know.
[1676.88 → 1677.44] It's true.
[1677.54 → 1678.74] That was my first thought.
[1679.22 → 1680.24] I just could find that super useful.
[1680.36 → 1682.48] But also the context of a studio.
[1683.02 → 1689.28] You know, how great would it be if I could pull in an HDMI source into OBS from a computer that's upstairs or something or vice versa?
[1690.10 → 1695.22] Or maybe somebody upstairs could have the HDMI out from OBS, the monitor, the live monitor.
[1695.90 → 1697.90] Or in the living room, even.
[1698.12 → 1699.64] Wouldn't it be great to be able to send the live?
[1699.64 → 1701.24] We used to actually do that physically.
[1701.36 → 1702.94] We used to have a really long HDMI cable.
[1702.94 → 1707.00] So I opened some ports over UDP as well as doing the multicast thing.
[1707.44 → 1711.84] And I will warn you that multicast will take down your network in a heartbeat if you don't know what you're doing.
[1712.20 → 1713.38] So just be prepared for that.
[1713.56 → 1715.26] Some adventures with that.
[1715.76 → 1718.14] But, I mean, this just looks like a fascinating solution.
[1718.36 → 1727.82] It looks like it's going to be around about $100, $130 for a receiver and a transmitter with some small discounts if you add more devices.
[1727.82 → 1739.88] If you compare that to building a Pi KVM, which the only thing this can't do is the remote power on, power off situation, which, let's be fair, is quite a rare use case.
[1740.20 → 1742.18] Very useful when you need it, but quite rare.
[1742.88 → 1753.08] This will do 90% of what the Pi KVM or any kind of other, you know, self-built KVM solution will do for the same money or less.
[1753.08 → 1757.82] And with the Raspberry Pi being an Titanium these days, I can't wait for these to come back in stock.
[1757.88 → 1761.72] As soon as I see that in-stock button, I'm just going to buy one just to try it out.
[1762.04 → 1763.90] Yeah, right on.
[1764.24 → 1765.44] Well, good, because I'd love to know.
[1765.58 → 1768.36] I could definitely – I fantasized about something like that for years.
[1768.44 → 1770.56] So I definitely want you to follow up on that.
[1771.28 → 1771.98] All right, what do you say?
[1772.04 → 1773.86] Should we do some feedback?
[1774.30 → 1779.50] Yeah, before we do, I would like to just talk about a small little giveaway that I'm going to do.
[1779.54 → 1780.40] Oh, yeah, right.
[1780.40 → 1789.92] It was Black Friday a couple of weeks ago, so obviously I bought a new hard drive as part of my annual ritual of buying hard drives on cheap hard drive weekend.
[1790.52 → 1796.12] So I got myself a 14-terabyte hard drive for about $196, which I was very pleased with.
[1796.74 → 1801.22] What this means is I've gone ahead and done the ZFS Resilver and the Scrub and all that,
[1801.22 → 1807.26] and I have on my desk in front of me a spare 10-terabyte hard drive.
[1807.26 → 1813.20] It's about four, four and a half years old, in perfect working condition.
[1813.66 → 1819.50] The only reason I've retired it is that I don't like things getting much beyond four or five years in age,
[1819.70 → 1825.74] and so I replace a drive or two every year, and that keeps me nicely up-to-date on new drives.
[1826.76 → 1831.70] So what I was thinking was I could sell this, you know, for, I don't know, 50, 60 bucks.
[1831.86 → 1832.60] Who knows?
[1832.60 → 1838.30] What I thought it would be good to do, though, is given it's the holidays and Christmas, why don't we do a giveaway, which we haven't done before?
[1839.32 → 1848.44] I was hoping for some needy college students or somebody who has absolutely no backup strategy or somebody that needs it, right?
[1848.84 → 1856.70] Maybe somebody, what about somebody building their first media server, Christmas movies for the family, for the holiday, you know, some sob story, basically.
[1856.70 → 1859.32] Yeah, we need a Simon Cowell grade sob story.
[1860.04 → 1865.42] I want somebody to write in, and we will put these to an audience vote over the next few weeks,
[1865.62 → 1872.92] with your worst data loss story, okay, or your worst I didn't have a backup story,
[1872.92 → 1880.26] and then we'll put all these into a document, a paste bin or something like that, one of our self-hosted paste situations,
[1880.60 → 1886.60] and we'll get the audience to vote, and then the winner will receive this 10 terabyte hard drive.
[1887.26 → 1895.36] Couple of caveats, lower 48 states or UK only, because I can get my sister to bring this back with her at the end of January to the UK
[1895.36 → 1901.32] and post it to the UK nice and cheaply, or I can post it in the US, obviously, from my house.
[1901.32 → 1908.76] So those are the terms and conditions, such as they are, and yeah, self-hosted. Show slash contact.
[1909.22 → 1914.28] Yep, there you go, send it in, and co-hosts do not qualify, unfortunately.
[1914.82 → 1917.44] How many hard drives do you have just sat in a box, be honest?
[1917.60 → 1921.64] I mean, now if you count ones that are like 2 terabytes, it could be dozens.
[1922.26 → 1922.72] It could be.
[1923.22 → 1926.72] Ones that are like 10 terabytes, it goes probably to none.
[1926.72 → 1939.24] But, oh, actually, I have a stack of like 128 and 256 and maybe a couple of 512 SSDs that I took out of a bunch of dead, like a dozen dead laptops,
[1939.44 → 1940.94] and I just went out and took out all the storage.
[1941.46 → 1944.02] It's just, it's a lot.
[1944.22 → 1945.02] It's a lot.
[1945.82 → 1950.98] All right, so Beau went over to self-hosted. Show slash contact and sent in some thoughts on note-taking.
[1951.22 → 1952.66] I've been on a journey right now.
[1952.66 → 1957.56] I have like a stand-in solution for the moment, but Beau writes, here's a plus one for Obsidian.
[1957.70 → 1958.66] I heart MK Docs.
[1959.58 → 1964.82] In fact, I rebuilt my hospital's internal medicine handbook with it, which is at vimbook.org, apparently.
[1965.22 → 1967.16] But also fell in love with Hugo.
[1967.34 → 1968.32] Well, yeah, of course.
[1968.44 → 1972.60] Yeah, Hugo is, Hugo can be used as a publishing tool for Obsidian.
[1972.86 → 1979.48] It supports all the essential features, superfast builds, and of course, it's open source, self-hostable, and GitHub Actions deployable.
[1979.48 → 1985.32] Like you, I'm still migrating many of my notes from elsewhere to .md files and Obsidian.
[1985.60 → 1990.06] So my own instance is rather bare, but if you're interested, and he gives it to us here,
[1990.70 → 1993.80] and he says on iOS, there's this app called Working Copy.
[1994.22 → 1998.12] That's an amazing Git app that plays nicely with GitHub and has good markdown.
[1998.58 → 2001.40] So you don't have to pay for the Obsidian app if you don't want to.
[2001.94 → 2004.02] I haven't found an equivalent yet on Android.
[2004.14 → 2005.90] I just used the GitHub web UI.
[2005.90 → 2010.86] A lot of people wrote in to say Obsidian, so thank you, everybody.
[2010.98 → 2014.60] I think I'm going to try it and maybe try using Nextcloud to do the syncing.
[2014.70 → 2015.92] I don't know if I'm way off base there.
[2016.08 → 2018.16] That's what I've been using for a while on the LAN.
[2018.96 → 2022.46] It's backed by Git as well, and there are a few conflicts every now and again,
[2022.68 → 2025.14] but I just ignore them, and it seems to be fine.
[2025.78 → 2028.72] But it doesn't do picture text recognition, right?
[2029.14 → 2029.82] It can.
[2030.38 → 2032.02] It can with a plugin or something?
[2032.52 → 2032.78] Yeah.
[2032.98 → 2033.24] Okay.
[2033.42 → 2034.12] Well, I'll give it a go.
[2034.12 → 2034.98] You know what?
[2035.04 → 2035.98] I'll give it a gosh darn go.
[2036.52 → 2039.98] A lot of people also have been giving me some tips on my Android journey,
[2040.04 → 2041.52] because, you know, I'm an Android guy now, Alex.
[2041.86 → 2042.66] Switch to Android.
[2043.20 → 2045.58] This is like the new CrossFit or veganism, isn't it?
[2045.86 → 2046.04] Yeah.
[2048.06 → 2051.50] Yeah, I use Graphene OS, by the way.
[2053.58 → 2055.04] Of course, it's the new Arch.
[2055.34 → 2055.68] Yeah.
[2055.68 → 2059.06] So people have been telling me to check out NewPipe.
[2059.54 → 2060.98] And you know what?
[2061.30 → 2065.30] I've heard about NewPipe for years, so I went in with expectations blazon'.
[2065.30 → 2069.02] And, man, have I been disappointed with NewPipe.
[2069.22 → 2071.88] First, I appreciate getting out of the YouTube app.
[2071.94 → 2073.34] So I do get where you all are coming from.
[2073.42 → 2074.24] Like, that part I get.
[2074.28 → 2075.40] It downloads real good.
[2075.48 → 2076.20] It does in the background.
[2076.32 → 2077.34] Multi-threaded download.
[2077.34 → 2079.82] It sends it out to your preferred video player.
[2079.96 → 2081.48] I like all of that a lot about NewPipe.
[2082.28 → 2085.10] And I like that, you know, I can have my own subscription list in there.
[2085.42 → 2088.90] But you know what is ridiculous about NewPipe, otherwise a decent app?
[2089.32 → 2091.54] It doesn't show you live streams.
[2091.86 → 2093.76] Like, if you go to a channel that's live.
[2094.38 → 2095.70] Sorry for my ignorant question.
[2095.82 → 2096.64] What is NewPipe?
[2097.04 → 2097.58] What does it do?
[2098.42 → 2101.40] Sorry, I got all worked up, because, man, did I get inundated with NewPipe.
[2101.90 → 2104.22] I had all this NewPipe in my face.
[2104.22 → 2112.30] It is an alternative YouTube client that's, like, lean, mean, customized machine.
[2112.92 → 2116.58] It's great if you have, like, a list of subscriptions or YouTubers that you want to follow.
[2116.82 → 2118.10] You pop them all in there.
[2118.24 → 2119.72] It does perfect downloads.
[2119.86 → 2123.92] It'll just do, like, you know, two or three threaded downloads superfast.
[2124.18 → 2125.42] It's great for all that.
[2125.58 → 2127.34] But it does not support live streams.
[2127.56 → 2130.30] And it does not support timestamps and videos.
[2130.90 → 2131.42] Well, that stinks.
[2131.90 → 2133.92] That just, it's a non-starter.
[2134.76 → 2137.96] Particularly these days, where every Tom, Dick, and Harry has a YouTube channel.
[2138.40 → 2142.46] And, you know, like, it's almost like anybody can just make content and put it on the internet for free.
[2142.60 → 2143.16] Yeah, yeah.
[2143.22 → 2145.10] And people will listen to it, you know.
[2146.80 → 2149.92] You really need those chapter markers in some YouTubers.
[2150.24 → 2151.24] You really, really do.
[2151.66 → 2153.76] And I'm already paying Goods for the premium.
[2154.54 → 2158.94] So I get the download in the YouTube app, which is actually better on Android than it is on iOS.
[2158.94 → 2160.20] The download in the background stuff.
[2160.32 → 2162.78] Turns out stuff can just run in the background perpetually and download.
[2163.40 → 2164.12] For better or for worse.
[2164.22 → 2165.38] But thank you, everybody.
[2165.80 → 2167.00] Keep sending in your suggestions.
[2167.26 → 2169.94] And if you'd like to boost in, I got a hot tip for you, Alex.
[2170.48 → 2172.70] But I figured we'd do this in the show.
[2172.92 → 2175.04] So that way people can see how this works.
[2175.04 → 2179.80] With the boosts, they have this mechanism called the split.
[2180.70 → 2183.64] And the split is what it sounds like.
[2183.68 → 2187.66] You can say 30% of the boost goes to Chris.
[2187.80 → 2189.82] 30% of the boost goes to Alex.
[2189.88 → 2193.64] And, like, 70% or whatever it is, you know, goes to the network.
[2193.70 → 2195.56] Or 40%, depending on how many hosts it is.
[2195.56 → 2196.70] You know, you could do different splits.
[2196.74 → 2197.20] You could do 20.
[2197.20 → 2198.08] All the way around.
[2198.92 → 2202.56] And to participate in that, you need to have a lightning address.
[2203.10 → 2211.10] And for, you know, until, like, I don't know, four months ago, you had to run a full node to get that address.
[2211.10 → 2220.74] But now, the group over at Alfie, which makes a browser extension that I like, I've had some meetings with them, and I think they're good folks.
[2221.66 → 2224.78] They have integrated with the whole podcasting 2.0 stuff.
[2224.96 → 2231.00] And when you go sign up at Alfie, they can generate you a value block code that you can give to me.
[2231.34 → 2233.28] And I can put in the splits for you.
[2233.54 → 2235.64] And you don't have to have a self-hosted node at all.
[2235.64 → 2243.40] Now, you're letting them host it, which is not necessarily great security practice, but we're not talking, like, thousands of dollars here, right?
[2244.02 → 2247.10] And then they manage all the lightning liquidity stuff for you.
[2247.32 → 2253.54] And then if you want, you can then plug in another app they've created called Saturn, Sat Earn.
[2254.08 → 2258.70] And that will give you the live boost dashboard so you can get the boosts as they come in live.
[2259.22 → 2264.36] And so I mention this because the audience could also go set up an Alfie account and get a lightning address.
[2264.36 → 2266.94] And could also participate in the boosts.
[2266.98 → 2272.58] If they send us a good question, we could put their lightning address in, and they could be involved in the split, stuff like that.
[2272.68 → 2275.38] So I'm mentioning it on air so that way everybody knows how this works.
[2275.72 → 2284.32] The great thing about Alfie, too, is later on, if you did want to host your own node, if you want to do the self-hosted route, you can actually plug Alfie into the self-hosted node later.
[2284.46 → 2287.56] So you can switch to a self-hosted solution, which is really cool.
[2287.62 → 2288.42] So I will put links.
[2288.78 → 2290.10] It's getalbie.com.
[2290.64 → 2291.52] You go there.
[2291.62 → 2293.20] That'll get you the value block code.
[2293.20 → 2295.46] In Alex's case, he gives that to me.
[2295.76 → 2297.12] Then I'll put that in our feeds.
[2297.24 → 2300.18] And then when people boost, your split will go to your Alfie wallet.
[2300.46 → 2303.94] And then you just go to Alfie and you can see all the boosts that have come in.
[2304.00 → 2306.90] And then you go to Sat Earn and you can read the boost messages.
[2307.60 → 2308.30] Does that make sense?
[2308.62 → 2310.14] Yeah, I think it's a fascinating concept.
[2310.64 → 2313.36] You know, I've been a little lukewarm.
[2313.58 → 2317.00] Might be an accurate description to some of the boost stuff in the past.
[2317.00 → 2320.74] But, you know, it's making a real difference on UP.
[2321.04 → 2326.74] You know, we're seeing in the lightning charts on Podcasting 2.0 some real benefits from exposure.
[2327.14 → 2331.06] You know, I can't remember the numbers specifically, but you were talking.
[2331.06 → 2333.26] I was listening to this podcast whilst I'm in Vegas.
[2333.40 → 2339.22] So in my head, I've got some Eiffel Tower going past in my head as I'm picturing listening to you talk about this.
[2339.70 → 2344.64] But we were in the top charts for several days because some of the boosts that people sent in.
[2344.88 → 2346.72] And that's all down to the listeners.
[2346.84 → 2351.56] That's a really great way of sharing the love and spreading JB around, you know.
[2351.56 → 2356.28] And I think if you start getting the histograms, I think it'll start clicking immediately.
[2357.02 → 2364.56] Because once you start getting the messages, and they come in on this dashboard, and they have some value attached to it and then there's that message.
[2364.96 → 2368.88] And it's in real time as they're listening to the episodes, you can see what episode they're listening.
[2369.02 → 2373.24] You could even, there are even some tools that can, some apps will tell you when, most of them don't.
[2373.28 → 2375.26] But you can even like to get that information in some cases.
[2375.42 → 2378.42] And it's a it's a really, it's, it's as close.
[2379.20 → 2381.36] I think you'll know what I'm, what I'm saying when I say this.
[2381.36 → 2386.74] It's as close to meeting the audience in person that I've ever come doing this in 15 years, right?
[2386.78 → 2394.22] It's not as good as meeting them in person in terms of connection, but it's just like a step removed.
[2394.64 → 2402.60] It's, it has made me more passionate about the audience and my connection to the community and more involved than I have been in years.
[2402.60 → 2405.16] It's like, it's a powerful thing for creators.
[2405.16 → 2409.92] So I think when you, if you do sign up, and then you do the histogram stuff on, on, on a Saturn,
[2409.92 → 2411.96] I think you'll see what I'm saying.
[2412.04 → 2412.78] It's so cool.
[2413.44 → 2415.06] And it's all decentralized, right?
[2415.10 → 2416.32] It's all self-hosted.
[2416.90 → 2418.94] And that is all part of it.
[2418.98 → 2419.98] It checks my boxes too.
[2420.08 → 2421.48] So love all of that.
[2421.76 → 2424.36] So with all that said, I'll also mention.
[2425.14 → 2428.88] You can boost into the show now without having to get a new podcast app.
[2428.88 → 2439.02] If you get that Alfie extension I mentioned, and you pull up the self-hosted shows page on the podcast index, which I will link in the show notes, you can just boost right from the webpage.
[2439.48 → 2442.62] No new podcast app required makes it a lot simpler.
[2442.84 → 2450.74] And Alfie also just added the ability to top off SATs in the Alfie app itself using moon pay as a service.
[2450.74 → 2456.40] So you can now add SATs directly to Alfie if you like, which we were experimenting with earlier today.
[2457.16 → 2471.36] So with that said, let's get to our first boost this week because it came in from the helpful idiot, and he took me to task, but he did it for 555,556 SATs, which is that's a big boost.
[2471.50 → 2472.20] Thank you, sir.
[2472.22 → 2475.86] And he says, but guys, I boosted in over 300,000 SATs and I didn't get a mention.
[2475.86 → 2478.94] That guy from late night Linux was the poor man's Alex.
[2481.14 → 2482.00] I love that.
[2482.24 → 2482.82] You know what?
[2482.94 → 2484.94] Even the poor man's Alex is still decent.
[2485.54 → 2486.48] Oh, he's talking about Joe.
[2486.64 → 2487.20] I see.
[2487.52 → 2487.72] Yes.
[2487.88 → 2489.50] Thank you to Joe for filling in for me, by the way.
[2489.52 → 2493.76] I don't think I said thank you last episode and I felt bad about it whilst I had the Rona.
[2494.34 → 2494.98] Thank you, Joe.
[2495.34 → 2497.52] I looked helpful idiot and I don't see it.
[2497.60 → 2502.72] And I think I had liquidity issues around that time, which is the downside of me self-hosting it.
[2502.72 → 2505.96] Like where Alfie manages that because I self-host mine.
[2506.28 → 2510.36] If I get the liquidity mixed up and the boost is big, sometimes it won't come in.
[2510.58 → 2511.62] It's fixed now, though.
[2511.72 → 2512.64] So that boost came in.
[2512.98 → 2519.74] You missed one very important comment that he made is that GIF equals GIF, which is a luck joke.
[2519.90 → 2522.34] I think I was just trying to avoid that whole thing.
[2522.52 → 2524.56] I don't want it to infect the next show.
[2525.04 → 2527.50] Oh, the pronunciation thing is a rabbit hole.
[2527.56 → 2529.14] Alex is a rabbit hole.
[2529.26 → 2530.56] I mean, I think it's GIF.
[2530.56 → 2531.76] I also think it's Debian.
[2534.26 → 2536.00] Well, of course, it's Debian Ian.
[2536.58 → 2539.66] Nomadic Coder boosts in with 3,110 SATs.
[2540.32 → 2545.46] He says, I don't take knowledge-based notes on my phone, only memos, which I can sync with my desktop.
[2545.92 → 2547.44] I follow Michael Bails.
[2547.56 → 2548.06] Is it Brazil?
[2548.18 → 2552.92] I think I follow his recommendation and use standard notes for privacy because they encrypt locally.
[2553.22 → 2556.38] I'm on the free plan, and it suffices for knowledge-based work.
[2556.38 → 2562.28] I use Settler on my desktop and I use Zettelkasten, I guess.
[2562.86 → 2563.26] Zettelkasten.
[2563.68 → 2564.56] Okay, Zettelkasten.
[2564.74 → 2565.34] All right, thank you.
[2565.74 → 2569.62] And then he puts all that up onto a Git repository, and he syncs that to GitLab.
[2570.28 → 2571.84] Yeah, that's a workflow with notes.
[2571.90 → 2574.64] It's just something in front of GitLab or GitHub.
[2574.64 → 2582.42] The whole Zettelkasten thing is why these Roam Research and Obsidian and Log Sec, and that's why all these tools have become so big.
[2582.50 → 2593.58] It's this linking your thinking kind of approach where you put backlinks within certain documents which then reference other documents, and you end up with, you know, index cards essentially of a topic.
[2594.10 → 2596.88] So, you know, let's say you're writing a blog post about ZFS, for example.
[2596.96 → 2598.24] You're taking notes about ZFS.
[2598.70 → 2602.22] Well, you don't need to put anything about what ZFS is in that note.
[2602.22 → 2613.62] You can have that linked somewhere else in a note dedicated to what ZFS is, and then you can have the short, you know, the short, I don't know, index of what you're thinking of that moment.
[2613.86 → 2621.40] And it creates some pretty complex connections, and it's an idea that I love as a concept.
[2621.40 → 2624.80] It's just not something I've ever actually made work in practice.
[2624.80 → 2636.74] And it's one of those things that I'm using on the daily already with my self-hosted Obsidian MK Docs, you know, internal home wiki.
[2637.72 → 2641.16] But if it went away tomorrow, I probably wouldn't miss it all that much.
[2641.40 → 2651.12] You know, I'm pretty good at searching and storing information in certain ways because I've trained myself because computers used to suck, and now they suck a little bit less in some ways, but more in others.
[2651.12 → 2654.62] But you can still fall back on that ways that used to suck.
[2654.76 → 2656.00] You know, you can still let it still work.
[2656.18 → 2656.32] Yeah.
[2656.46 → 2656.86] Okay.
[2657.02 → 2666.16] My wife and I were just having this chat the other day about how can computers now be so good and simultaneously still not able to print a single sheet of A4?
[2666.72 → 2667.02] Yeah.
[2667.16 → 2673.32] I mean, I had this experience when we came across an old Mac, the first Macintosh, the black and white all-in-one.
[2673.32 → 2685.02] And I fired up Clarín Works and fired up a card game and kind of had this moment where I was like, Geez, this thing's doing like 80% of what people need to do today.
[2685.12 → 2688.88] If you could get an email client on this thing and a messenger, you'd probably be good to go.
[2689.24 → 2691.14] But it would take 15 minutes to boot up, though.
[2691.50 → 2693.10] Well, there was that if you boot it off a disk.
[2693.10 → 2698.30] But you see, this had a premium external SCSI hard drive upgrade.
[2698.70 → 2700.54] Or I don't know if it was SCSI back then, but it was true.
[2700.54 → 2702.52] Oh, you fancy bitch, you.
[2702.72 → 2704.68] It was a big 20 megabyte hard drive.
[2704.90 → 2705.02] Yeah.
[2705.44 → 2706.64] So that was a little bit faster.
[2706.98 → 2707.16] Amazing.
[2707.86 → 2712.76] Stan Smith has our last boost this week for 600 SATs and just said, I wanted to send some good boost.
[2712.90 → 2713.54] Love your way.
[2714.18 → 2716.44] Love the show and all your Linux talk and self-hosted support.
[2716.60 → 2717.36] Keep up the good work.
[2717.44 → 2718.52] Well, thank you, Stan Smith.
[2718.52 → 2724.18] We also got 5,555 SATs from Radius, who just said, appreciate what you do.
[2724.42 → 2730.02] And 100 SATs from MTBDude641, his very first boost.
[2730.34 → 2730.70] Congratulations.
[2731.64 → 2735.76] You can get a new podcast app at newpodcastapps.com and send a boost in.
[2735.88 → 2739.76] Or I'll just have our page on the podcast index-linked in the show notes.
[2740.24 → 2742.40] Load up Alfie, go over there, get her done.
[2742.86 → 2745.62] And also, Alex, we should take a moment and thank our SRE subscribers.
[2745.62 → 2749.56] They help by making the ongoing production of the show possible.
[2749.84 → 2754.80] And they get an ad-free version of the show with a special post-show recorded just for them.
[2755.18 → 2758.12] You guys mean that we don't need to submit to an algorithm.
[2758.62 → 2760.44] And I cannot thank you enough for that.
[2760.78 → 2762.52] Jeff Killing is a perfect example, right?
[2762.62 → 2767.80] Poor guy is going through some incredibly bad health issues and some surgery stuff right now.
[2767.86 → 2770.22] So I'm sending you my best wishes, Jeff, if you're listening.
[2770.22 → 2775.72] But he had to put a note on his YouTube channel saying, right, this is going to hurt my algorithm.
[2775.92 → 2777.62] Please don't unsubscribe from my channel.
[2777.82 → 2782.66] Like, there's a real fear there from YouTubers that if they upset the algorithm for any reason,
[2782.76 → 2786.54] that they stop uploading regularly or anything like that.
[2787.06 → 2788.80] We just don't have to worry about that stuff.
[2788.90 → 2790.18] Yes, we've got a couple of sponsors.
[2790.74 → 2792.04] But that's it, you know.
[2792.04 → 2797.80] And compared to so much of the online content you see these days, I mean, you want to watch a three or four minute drum cover.
[2797.90 → 2803.14] You have to sit through a one-minute advert of somebody telling you about, I don't know, weed killer or something.
[2803.36 → 2803.66] I don't know.
[2803.78 → 2805.14] Well, and it's not just that, too.
[2805.26 → 2811.90] It's the system also forces them to do all the please like, subscribe, hit the bell.
[2812.28 → 2814.52] And then pull the silly faces in the thumbnails, too.
[2814.60 → 2817.22] You don't have to look at our faces unless you watch the live stream, of course.
[2817.22 → 2827.06] And it also kind of encourages them to do things to cause people to comment because even people raging in the comments still is seen as engagement by the algorithm.
[2827.58 → 2832.40] And so that's a common tactic that you just really, really just takes down the experience.
[2832.52 → 2833.50] So, yeah, thank you very much.
[2833.60 → 2836.26] And as a thank you, we do make that post show available.
[2837.04 → 2840.96] If you haven't signed up yet, you can sign up just for this show at self-hosted.show.SRE.
[2840.96 → 2852.08] But because we are spinning down the network Patreon, I have a special sale going for the Jupiter. Party membership, which gets you all the shows ad free, including this one with the post show.
[2852.32 → 2861.26] And if you use the promo code 2022, it'll take two bucks a month off the ongoing membership for the lifetime of the membership, which is outrageously a great deal.
[2861.26 → 2864.34] But it's as a thank you for people that are transitioning from my Patreon.
[2864.46 → 2865.22] And I've made it available.
[2865.42 → 2871.14] If you're an SRE and you want to upgrade, I also made it available as an upgrade membership promo code as well.
[2871.62 → 2877.48] And I think this week we're going to talk about the Raspberry Pi hoopla and the witch hunt that went on over there, maybe.
[2878.60 → 2878.96] Yes.
[2879.32 → 2880.48] You and I both have thoughts.
[2881.04 → 2884.28] And, of course, the Raspberry Pi has a pretty important role in the self-hosting community.
[2885.36 → 2887.68] It used to, if you could still buy one.
[2888.76 → 2890.40] But more on that later, perhaps.
[2890.40 → 2890.62] Yeah.
[2891.66 → 2896.12] So you all know by now, the place to go to get in touch with us is self-hosted. Show slash contact.
[2896.24 → 2898.04] Or, of course, you can boost into the show as well.
[2898.78 → 2902.60] You can find me over on Elon's Twitter these days, at Ironic Badger.
[2902.70 → 2903.56] I'm also on Mastodon.
[2903.80 → 2906.46] I'll put a link to my Mastodon in the show notes.
[2906.64 → 2910.36] I still don't quite fully understand how to send people where I am.
[2911.20 → 2911.56] Yeah.
[2911.68 → 2911.92] Okay.
[2912.22 → 2912.50] Okay.
[2913.12 → 2913.62] Oh, you know what?
[2913.62 → 2914.46] I'll plug the Matrix.
[2914.98 → 2916.96] You can find me in the Matrix Federation.
[2917.22 → 2920.58] Just go to jupiterbroadcasting.com slash matrix.
[2920.58 → 2921.02] Matrix.
[2921.22 → 2922.06] Knock, knock, Neo.
[2924.20 → 2925.28] Thanks for listening, everyone.
[2925.44 → 2927.56] That was soulphosted. Show slash 86.
[2927.56 → 2928.32] Six.
[2928.54 → 2928.68] Boom.
[2929.04 → 2929.34] Boom.
[2929.34 → 2929.84] Boom.
[2949.90 → 2950.46] Boom.
[2950.46 → 2951.34] Boom.
[2951.40 → 2952.30] Boom.
