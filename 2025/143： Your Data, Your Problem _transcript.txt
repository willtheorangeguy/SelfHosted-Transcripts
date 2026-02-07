[0.00 --> 8.22]  Welcome to episode 143 of the Self-Hosted Podcast, and this week, our very own Alex is out and about.
[8.30 --> 9.18]  Where are you right now, Alex?
[9.52 --> 13.70]  We're time zone buddies. I am overlooking San Francisco Bay right now.
[14.02 --> 18.86]  The streets are paved with gold or something, and I'm in Silicon Valley, baby.
[19.64 --> 25.24]  Yeah, you've got a great view. You sent me a picture from your room, and you can see the Golden Gate Bridge in the distance and the hills.
[25.48 --> 26.68]  That's a real looker.
[27.16 --> 29.32]  And Alcatraz, just in case things get a bit rowdy.
[29.32 --> 30.90]  Was there Alcatraz in there, too?
[31.12 --> 32.46]  Yeah, just in the foreground.
[32.84 --> 34.98]  Oh, yeah, you're right. Oh, that's cool.
[35.04 --> 36.88]  Yeah, because I'm over on the Oakland side.
[37.12 --> 39.90]  That's so weird. Oh, look at that. It's so creepy.
[40.48 --> 49.58]  It does feel weird. Like, coming in from the airport, the first thing I notice is just how every single billboard out of SFO is a tech company. Every single one.
[49.98 --> 52.04]  Yeah, you're in the heart of the beast right now.
[52.28 --> 53.60]  Yeah, that's true.
[53.92 --> 55.22]  You're like in the lungs, I guess.
[55.22 --> 64.94]  So I had a listener write to me on Discord, selfhosted.show slash Discord, if you want to join the conversation, asking a pretty sort of meta question, saying,
[65.20 --> 71.56]  Hey, Alex, I've heard that self-hosting gives you more control, but I'm not sure exactly what that means.
[71.56 --> 77.56]  What are the benefits of self-hosting over something like a managed service or a managed hosting option?
[78.98 --> 85.66]  It's a good question. Like, what's the real value it's giving me versus, you know, trusting some company to manage it for me?
[85.76 --> 88.26]  Because then, you know, it saves you some gray hairs, I suppose.
[88.74 --> 91.06]  But you get to manage all your own downtime, I suppose.
[91.40 --> 91.76]  Yeah.
[91.76 --> 92.96]  That's a plus point.
[93.58 --> 94.24]  I guess so.
[94.66 --> 96.84]  Gosh, there's so many angles to answer this.
[96.96 --> 100.50]  And it really, I hate to say it, but it feels like, well, it depends on your situation.
[100.66 --> 109.34]  Because you might be somebody who just wants to learn how these things work, and maybe you feel better understanding how all of the different pieces work together.
[109.52 --> 110.76]  So that could be enough reason.
[111.14 --> 116.98]  Or, I mean, don't you think somebody might just be like a privacy-focused person, and so they want all of their data locally?
[116.98 --> 125.98]  Or, you know, maybe you're like me, Alex, and you want to be able to take your home off-grid from time to time in an RV, and you want to have essentially full functionality without internet.
[126.74 --> 127.94]  I think all those things apply.
[128.26 --> 132.38]  There are probably a couple of vectors that people come into self-hosting through these days.
[132.86 --> 139.12]  And I think the media hosting angle has been the strongest entry point for a number of years now.
[139.22 --> 141.16]  You know, the plexes, jelly fins, that kind of stuff.
[141.26 --> 141.92]  Media acquisition.
[142.30 --> 143.28]  We all know what I'm talking about.
[143.88 --> 146.72]  The other one now is home automation.
[146.98 --> 148.12]  As being another one.
[148.32 --> 160.44]  And, you know, in both of those camps, there are situations where you gain functionality, you gain features and control that you just wouldn't have by relying on third-party vendors.
[160.44 --> 168.98]  So, you know, you've got control over disparate smart home ecosystems from one place with Home Assistant, for example.
[168.98 --> 178.88]  So, from that perspective, it's a question of it does more than the proprietary options would let you.
[179.44 --> 180.46]  There's definitely that.
[180.58 --> 181.60]  You get to tinker more.
[181.86 --> 183.06]  You get to have more control.
[183.06 --> 184.94]  You know, as you were talking about it, too.
[185.02 --> 198.94]  I was thinking I've also been hearing from listeners who are beginning to explore LAMA and other LLMs that they can run locally because they want to do some of the things that you see people using CLOD and Perplexity and ChatGPT for.
[199.06 --> 202.08]  But they want to use sensitive data and they want it all to be local.
[202.08 --> 211.12]  And so I've seen a couple of listeners that are getting into the self-hosting route for their businesses or at home just to also experiment with large language models locally.
[212.00 --> 212.02]  Yeah.
[212.22 --> 216.66]  I mean, the privacy implications of keeping everything local I think are fairly obvious.
[217.08 --> 228.82]  You know, you're not sending off, you know, every request to Google or to Anthropic or to OpenAI that you're making to all of these different search chat, you know, systems.
[228.82 --> 237.94]  You know that that data is going into a bank somewhere and being fed in to train the next version of the model that comes out and all that kind of stuff.
[238.14 --> 251.72]  And if that doesn't interest you whatsoever, the ability to just run things fully locally, fully offline and agnostic of any kind of business model, I think is a huge advantage to self-hosting, too.
[252.56 --> 252.58]  Yeah.
[252.62 --> 257.36]  And I think you could just kind of there's a couple of table stakes that come along with self-hosting.
[257.36 --> 263.88]  It's arguably going to be a lot more private, especially if you don't have any, like, inbound ports on your firewall.
[264.02 --> 265.20]  You're not putting stuff on the Internet.
[265.88 --> 272.56]  You don't have third-party risk of a company offering you a product, a service, something like that.
[272.64 --> 278.28]  You know, the worst case being a device that's connected to a back-end service that eventually goes away.
[278.28 --> 282.74]  Companies are – maybe they're not in this for 10 to 15 years.
[282.90 --> 291.22]  But when you're building something that your family uses or yourself and you want to build something on top of that for a long time, you might want a product that lasts 10 to 15 years.
[291.32 --> 294.44]  That is achievable when you self-host.
[295.14 --> 300.16]  It is – it's never – I've never seen it achievable when you use any of the commercial proprietary services and platforms.
[300.16 --> 303.06]  I've never seen anything that's lasted that long.
[303.66 --> 308.44]  And, you know, it really sucks when it comes to, like, your IoT devices and whatnot.
[308.82 --> 323.36]  But then also I think we as – and I'm going to go here – a society, Alex, have lost how great it is to just take a little bit of time and have some craftsmanship with something.
[323.36 --> 325.52]  You know, it's not something you have to do for work.
[326.12 --> 330.24]  It's not something that's outside your comfort zone necessarily, maybe slightly outside.
[330.84 --> 336.70]  But you have an opportunity to build something with real craftsmanship and do it right and stack a W.
[337.74 --> 347.46]  And it's such a cool field because you will inevitably improve your quality of life, like things like a media stack or home assistant or solving your family's photo backups.
[347.46 --> 356.12]  There's an actual appreciable quality of life improvement and you can do it with craftsmanship and care and you can stack a W.
[356.82 --> 362.50]  And sometimes the jobs suck in or sometimes things aren't great with somebody, but you can still have this outlet.
[362.70 --> 365.28]  And for me, it's more enjoyable than gaming.
[365.90 --> 373.58]  I love gaming, but what I really get a lot of enjoyment from is building these systems that improve, you know, our day-to-day lives.
[373.58 --> 377.46]  The Linux terminal is the only video game that either of us truly need.
[378.44 --> 378.88]  Right?
[379.04 --> 381.16]  But I think it also goes a step further than that.
[381.22 --> 384.82]  You know, the education, the skills that you learn along the way.
[385.16 --> 400.30]  I can tell you pretty confidently that I wouldn't be sat in this chair right now without learning this stuff at home and having a home lab and experimenting and breaking stuff 8 million times at home before I finally figured out what worked for me.
[400.30 --> 404.40]  And then I go into work and I start saying, hey, this Terraform thing's pretty cool.
[404.48 --> 407.26]  We should look at this or, you know, this Ansible thing's pretty interesting.
[407.38 --> 408.12]  We should look at that.
[408.28 --> 411.14]  And what about containers and all the rest of it?
[411.30 --> 417.78]  Like that stuff, I mean, the old phrase of education isn't free comes to mind.
[417.78 --> 423.88]  I've paid for that educational piece with my own time, blood, sweat, frustration, tears, all the rest of it.
[424.40 --> 426.14]  Some people go to school to do that instead.
[426.30 --> 436.30]  But I think nothing can really beat as a practitioner in the IT space, the DevOps space, the, you know, you know what I'm talking about, like developer space.
[436.30 --> 445.10]  Nothing beats just solving and scratching your own itch and then being able to take those skills to a job interview or to work or something like that.
[445.26 --> 452.72]  And that for me has been, it's like an unspoken truth about self-hosting that we don't speak about too much.
[452.86 --> 457.22]  But it's been really powerful for me and my sort of personal career journey.
[457.94 --> 459.32]  Yeah, I think that's a great point.
[459.32 --> 463.98]  And then just to kind of finish it with one practical example, we'll put a link in the show notes.
[464.30 --> 466.56]  You know, there's the example of Amazon pulling e-books.
[467.46 --> 475.82]  My current like soapbox argument for why self-hosting media when I was kind of backing off and saying, well, I could just use streaming services.
[475.94 --> 477.52]  I don't need to burn all this hard drive space.
[478.28 --> 481.70]  And then some of my shows that I watched started getting pulled from streaming services.
[481.70 --> 490.66]  In fact, one of them just got pulled immediately before I was even done finishing the season because they decided they weren't going to have another season of the show and they didn't want to pay any royalties.
[490.78 --> 495.84]  So they just ripped the entire show right as I was in the middle of it, right off the streaming service.
[496.38 --> 497.84]  And that was Paramount Plus.
[498.86 --> 499.92]  And it happens all the time.
[500.40 --> 502.32]  This kind of stuff just gets yanked from you all the time.
[502.42 --> 505.28]  And so by taking matters into my own hands, it never happens again.
[505.52 --> 508.02]  And I have stuff that I, you know, don't have to stream.
[508.02 --> 511.72]  And we saw just this week Amazon pull the rug on.
[512.62 --> 515.88]  They're doing some licensing changes to Kindle books, right?
[516.24 --> 516.38]  Yeah.
[516.46 --> 521.36]  And I'm, you know, I've kind of bailed on the whole Kindle ecosystem as a result of this.
[521.66 --> 524.52]  But you're not you don't own the book.
[525.18 --> 527.96]  And they're making sure you understand that you're licensing it.
[528.04 --> 531.78]  They say by clicking on the above button, you agree to Amazon's Kindle store terms of use.
[531.78 --> 539.30]  And when you go in there, by placing your order, you're purchasing a license to the content and agree to the Kindle store terms of use.
[540.04 --> 543.48]  Imagine imagine Amazon knocking on your door and asking you to give them a book back.
[545.06 --> 547.86]  A paper book, you know, it's just never going to happen.
[547.98 --> 550.02]  But with the e-book system, it's no problem.
[550.34 --> 550.80]  It's easy.
[550.80 --> 559.42]  That said, it is an order of magnitude easier to share and or pirate an e-book than it is a paper copy.
[560.32 --> 563.14]  However, you know, physical books are pretty much worthless.
[563.42 --> 571.28]  And, you know, you can argue that by just looking at the network of little free libraries that exist around the country right now.
[571.50 --> 571.70]  Yeah.
[572.08 --> 573.44]  Those adorable little libraries.
[573.68 --> 575.46]  Physical books are actually worthless.
[575.46 --> 583.42]  And that license that you purchase for your e-book, once you've given the money to the author and the publisher, I mean, it's worthless.
[583.60 --> 585.02]  Why do they need to revoke it?
[585.66 --> 591.58]  Now, OK, now we've made a big stink about self-hosting and, you know, taking control of your stuff and how great it is.
[592.60 --> 597.02]  But I see here in the doc that you've been getting into Zigbee stuff.
[598.22 --> 601.24]  Yeah, nobody ever does that when things are running tickety-boo, do they?
[601.24 --> 604.96]  No, and it's usually, you know, it's funny how it's never Z-Wave in the doc.
[605.06 --> 605.70]  It's always Zigbee.
[606.16 --> 607.92]  Well, I don't have any Z-Wave devices.
[608.20 --> 611.08]  So that might be why I don't put any in.
[611.32 --> 619.96]  But actually, this post, which will be linked in the show notes at meshstack.de, talks about Zigbee table routing.
[619.96 --> 637.36]  And this is a really interesting topic that actually I had no idea was, you know, one of the trade-offs between using ZHA, which is the kind of prettier and easier to use plugin or integration for Home Assistant for Zigbee control versus Zigbee to MQTT.
[637.36 --> 649.42]  It turns out, you know, you read a lot of conjecture on forums and things about people saying Zigbee to MQTT is more stable and that ZHA is a little bit flaky and all this kind of stuff.
[649.50 --> 654.52]  It turns out that ZHA has table routing enabled by default.
[655.18 --> 661.46]  So the blog post goes into great detail talking about the two routing methods available for Zigbee.
[661.72 --> 663.94]  So you've got table routing and source routing.
[663.94 --> 678.36]  Table routing uses pre-configured tables, which creates a predefined table where each node knows all of the possible routes, ensuring, I guess, like a deterministic routing algorithm with a pretty low overhead.
[678.98 --> 688.68]  The trouble is it can cause higher latency and potential bandwidth issues due to redundant routes of nodes that have dropped offline or are no longer powered up or that kind of thing.
[688.68 --> 695.02]  Whereas source routing allows devices to determine their own path on the fly.
[695.16 --> 701.76]  And this offers more flexibility and efficient routing parameters for more dynamic environments.
[701.76 --> 715.36]  So in practice, what this means is in Home Assistant, ZHA, you can create a one line config change of source underscore routing equals true under your ZHA config.
[716.08 --> 725.36]  And I've noticed a significant performance increase by doing just this one one line change across my entire Zigbee network.
[725.36 --> 725.92]  Huh.
[725.92 --> 726.08]  Huh.
[726.08 --> 726.28]  Huh.
[727.28 --> 729.38]  I would be interested in trying this.
[729.52 --> 736.42]  You know, I've got a button we press, which kicks off a script that does the good night stuff and the good morning stuff.
[736.46 --> 744.96]  And there's always one LED light strip that just seems like it's not responding very quickly, sometimes like 20, 30 seconds before it actually fires.
[745.28 --> 745.68]  Oh, goodness.
[745.84 --> 746.02]  Yeah.
[746.22 --> 746.48]  No.
[746.48 --> 752.86]  I had a similar situation as part of my bedtime routine, which basically spams every single device in the house.
[752.96 --> 757.40]  When I push this little Zigbee button on my bedside table, everything shuts off.
[757.70 --> 760.60]  All the lights that are Zigbee get pinged.
[760.68 --> 763.88]  All of the blinds and shades get pinged, like everything.
[764.24 --> 767.58]  So the Zigbee network is about as congested as it could possibly be.
[767.58 --> 784.92]  And I know that when I push that button, it takes about 10 to 15 seconds in order for that loop to complete before my bedside light, which is the last thing I configured in the entire sequence deliberately, goes into its, you know, pre two minute countdown, like 5% mode.
[785.00 --> 788.60]  So I know that things, you know, a couple of minutes just to plug my phone in, all that kind of stuff.
[788.60 --> 797.06]  I pushed the button a couple of nights ago and before my arm had got back to my side, the entire routine had completed.
[797.60 --> 798.00]  Ah.
[798.44 --> 801.32]  So we're talking 15 seconds down to less than one.
[801.64 --> 802.32]  Oh, okay.
[802.66 --> 802.82]  Yeah.
[802.84 --> 803.02]  Okay.
[803.20 --> 804.28]  I'm going to try this too then.
[804.78 --> 805.60]  This could be nice.
[805.76 --> 807.50]  It's not a huge deal, but it's been annoying.
[807.70 --> 810.18]  I also have like a button panel by the couch.
[810.18 --> 815.96]  So when I'm watching a movie, I can hit a button and it turns off the lights and that stinking light always stays on long enough.
[815.96 --> 819.56]  Every time where the wife always says, is that going to turn off?
[821.10 --> 821.96]  Every time.
[822.40 --> 823.32]  And then it turns off.
[824.96 --> 828.04]  Now I did see there would be a link to a Reddit thread too.
[828.30 --> 831.40]  It was someone asking, are there any real downsides to source routing?
[831.76 --> 835.86]  And if source routing is so superior, why isn't it just the default for ZHA?
[836.58 --> 843.28]  And potentially the answer comes in that ZHA is shipped as a first class integration by Home Assistant.
[843.28 --> 855.34]  That means that it is targeting the Home Assistant yellow and green and the low power Home Assistant machines for which many people is what they run Home Assistant on.
[855.96 --> 861.72]  So sometimes the processing overhead can be higher on the host you're running it on.
[861.72 --> 863.08]  So that's something to bear in mind.
[863.62 --> 866.74]  But to be honest, I haven't really found a downside.
[866.90 --> 867.52]  I haven't noticed.
[867.58 --> 869.00]  I mean, I'm running it on an x86.
[869.56 --> 870.04]  What is it?
[870.08 --> 872.38]  An i5-6600T based.
[872.56 --> 874.74]  But it's not a powerful system by any stretch.
[875.12 --> 876.96]  But I haven't noticed any downsides whatsoever.
[877.22 --> 878.10]  So go ahead.
[878.18 --> 878.72]  Give it a try.
[878.86 --> 880.82]  Let us know how it goes for you.
[880.82 --> 885.62]  Tailscale.com slash self-hosted.
[885.72 --> 890.84]  Tailscale is the easiest way to connect your devices and services to each other wherever they are.
[890.92 --> 892.30]  It is modern networking.
[892.82 --> 899.00]  And if you go to Tailscale.com slash self-hosted, you'll get up to 100 devices and three users for free.
[899.34 --> 900.48]  No credit card required.
[900.48 --> 901.62]  And you can support the show.
[901.72 --> 904.42]  That's Tailscale.com slash self-hosted.
[904.42 --> 907.90]  A few things I love because I've been using it for quite a while now, a few years.
[908.22 --> 909.00]  It's fast.
[909.14 --> 910.74]  It just runs transparently.
[911.18 --> 919.84]  You really have no sense in terms of performance if you're talking over your tail net or through just like a clear text TCP connection over the internet.
[920.02 --> 924.78]  But what you do get is every device logically thinks it's on the same LAN.
[925.20 --> 926.74]  So you could have servers on a VPS.
[927.06 --> 928.80]  You could have a data center full of systems.
[929.02 --> 930.18]  You could have your mobile devices.
[930.38 --> 931.56]  You could have your admin team.
[931.66 --> 935.34]  You could have your production systems that have their own web tail net.
[935.34 --> 942.66]  And they all feel like no matter where they're at across diverse networks, they're on the same flat wire guard protected plane.
[942.66 --> 948.78]  And thousands of companies and many, many, many listeners of this show love Tailscale.
[948.78 --> 948.86]  Tailscale.
[949.06 --> 952.66]  The reality is everyone has heard of a VPN.
[953.56 --> 956.40]  But Tailscale isn't like any of those other VPNs.
[957.20 --> 963.74]  Tailscale is a secure mesh network that you can use to remotely access production systems like databases, servers, your Kubernetes cluster.
[963.74 --> 965.84]  And it's really secure.
[966.10 --> 967.36]  It's easy to deploy.
[967.66 --> 969.22]  And it's zero config.
[969.70 --> 970.82]  It's really simple.
[970.88 --> 974.62]  If you've got five minutes, you can probably get it up and going on three systems.
[974.82 --> 979.52]  And then once you have something set up, you can take that flat mesh network and build on top of it.
[979.84 --> 980.06]  Right?
[980.06 --> 985.58]  They have user ACL policies so you can securely control devices and services and what could access.
[985.96 --> 988.04]  They have things like Tailscale Funnel.
[988.18 --> 989.72]  And they have the Tailscale Send.
[989.82 --> 996.32]  And they have systems that allow you to use Tailscale to log in all your devices using your Tailscale credentials so you don't have to copy SSH keys everywhere.
[996.32 --> 1008.14]  And, of course, the ability to put applications directly on your Tailnet means that things like Visual Studio Code Editor for me, the web version, are available to any system on my Tailnet, which is all of my systems.
[1008.14 --> 1015.52]  Because I have no inbound ports anymore anywhere on any firewall for Jupyter Broadcasting or for myself personally.
[1015.76 --> 1021.46]  I just use Tailscale whenever I'm accessing any of my internal or syncing any of my external devices.
[1021.94 --> 1022.64]  It's great.
[1022.64 --> 1030.48]  So support the show and get it free for up to 100 devices and three users when you go to Tailscale.com slash self-hosted.
[1030.68 --> 1033.76]  That's Tailscale.com slash self-hosted.
[1035.72 --> 1038.68]  Have I ever talked to you about OpenWebUI before?
[1039.30 --> 1040.48]  Maybe off air.
[1040.92 --> 1043.34]  Maybe we've mentioned on the show briefly, but not much.
[1043.68 --> 1044.62]  Are you familiar with it then?
[1045.02 --> 1045.50]  Just a bit.
[1045.56 --> 1046.76]  I ran it shortly.
[1047.14 --> 1049.00]  And I have been thinking about giving it a go again.
[1049.06 --> 1050.56]  So it's fascinating that you're bringing it up.
[1050.56 --> 1057.34]  Well, it was actually a conversation over lunch at the, you know, I'm off site with work this week.
[1057.82 --> 1067.36]  A conversation over lunch with somebody talking about how to access multiple different, I suppose, ChatGPT and Claude and Gemini all in one place.
[1067.40 --> 1074.30]  And I'm like, ah, yes, but also you could access your self-hosted DeepSeek and Ollama and all the rest of it in one place too.
[1074.30 --> 1077.34]  So enter the project OpenWebUI.
[1077.92 --> 1084.26]  It's an extensible self-hosted AI interface that adapts to your workflows while operating entirely offline.
[1085.52 --> 1086.08]  Yes.
[1086.26 --> 1089.76]  I think I hear a Rick and Morty character yes click in there.
[1090.66 --> 1091.06]  Yes.
[1091.40 --> 1092.34]  That's what we want.
[1092.70 --> 1098.26]  So it's a little bit, the interface is a little busy, right?
[1098.50 --> 1098.68]  Yeah.
[1098.68 --> 1103.00]  I think mostly because it's trying to accommodate an awful lot of complexity under the scenes.
[1103.24 --> 1110.58]  So once you get past that, you're able to engage with multiple models from a single chat interface.
[1111.44 --> 1117.12]  That seems to be one of the killer features, especially if you have API keys across multiple services.
[1117.12 --> 1127.20]  And you also could, for example, by default, use your own local Llama instance or DeepSeek instance and then kick out to one of these external ones if you needed to.
[1127.66 --> 1129.44]  So that to me seems like, that's boom.
[1129.58 --> 1133.36]  Feature number one is it kind of brings them all together under one hood.
[1133.44 --> 1139.32]  Now, I have not really had the experience to say it does a great job of that, like when, say, formatting code output.
[1139.46 --> 1140.48]  But people tell me it does.
[1140.48 --> 1149.58]  Well, I think it's more about trying to reduce the cost of all of these multiple models that you can speak to.
[1149.76 --> 1156.22]  So let's just presuppose you wanted a subscription to Claude and a subscription to ChatGPT.
[1156.82 --> 1164.12]  The cheapest that you can do that by using the web-based subscription alone is, I think, 20 bucks a month for each platform.
[1164.60 --> 1164.76]  Yeah.
[1164.76 --> 1175.50]  Whereas OpenWebUI speaks the API calls that are required in order to just use API tokens instead of having to have a flat fee subscription.
[1175.86 --> 1181.06]  So it's a pay-as-you-go model versus an all-you-can-eat-and-then-you-get-throttled type model.
[1181.46 --> 1189.70]  It's a better way to go than using their web interfaces anyways because you're going to, if you really use these systems, you're going to inevitably need to pay for API credits.
[1190.18 --> 1191.84]  This happened to me when I installed Hoarder.
[1191.84 --> 1196.86]  I had to go get some OpenAI API credits even though I pay for ChatGPT Pro.
[1196.98 --> 1201.30]  So I'm paying for their damn ChatGPT Pro per month, and I'm also buying API credits.
[1201.42 --> 1202.56]  Claude works the same way.
[1202.88 --> 1209.26]  So just skip the web thing, skip the monthly, and just buy a handful of credits, and then you plug OpenWeb UI into that.
[1209.34 --> 1211.84]  You save a bunch of money, and you still get tons of good functionality.
[1212.64 --> 1212.68]  Yeah.
[1212.68 --> 1223.28]  It also supports all of the goodies like image generation integration, so you can plug in things like stable diffusion, Comfy UI, OpenAI's DALI.
[1224.04 --> 1225.50]  Now, have you tried this much?
[1225.70 --> 1228.08]  Didn't you have an instance running on one of your GPUs?
[1228.40 --> 1229.16]  I do, yes.
[1229.16 --> 1235.62]  I have an NVIDIA A4000 sat in the basement in my Epic server, and it's running on top of Nix.
[1236.08 --> 1247.84]  And the GPU is essentially running Ollama, and all I have OpenWeb UI do is reach out over tailscale to that GPU from wherever I am,
[1247.84 --> 1255.60]  and it just connects to the back end of Ollama, port 11434, and just works like a champ, honestly.
[1256.00 --> 1256.46]  That's cool.
[1256.84 --> 1257.54]  That is really neat.
[1257.62 --> 1265.38]  Now, have you, because what I wanted to know is, and I think this is what I would use a lot, is I know it supports adding documents to your chat,
[1265.44 --> 1267.68]  and then it can work on those and review those.
[1267.72 --> 1268.54]  Have you tried that much?
[1269.48 --> 1274.10]  I haven't done much rag with it, so that's retrieval augmented generation support,
[1274.10 --> 1279.94]  which means essentially you can load documents, as you were saying, into the chat interface.
[1280.96 --> 1286.02]  So from a privacy perspective, you know we were talking at the beginning of the show about privacy
[1286.02 --> 1291.80]  and how uploading random documents to ChatGPT might not be in your interest.
[1291.80 --> 1301.14]  If you are a company and you want to be able to do rag against any number of data sets without sending that information off who knows where,
[1301.72 --> 1303.78]  this is exactly the sort of tool you should be looking at.
[1304.10 --> 1311.06]  OpenWebUI plugged and backed up by Ollama, which then you can download pretty much any model from HuggingFace.
[1311.56 --> 1319.18]  And if you're not familiar with those terms, Ollama is just like a self-hosted server for running LLMs locally.
[1319.62 --> 1327.28]  And then HuggingFace is a little bit like Docker Hub is for containers, but it does the same job for AI models.
[1327.28 --> 1331.16]  There are so many neat ones on there, and it's a great way to discover new ones that have been published.
[1331.88 --> 1338.00]  And there are certain desktop tools, like LocalLM and others, that will actually just integrate HuggingFace,
[1338.12 --> 1339.32]  and it's a great way to play with it too.
[1339.74 --> 1346.74]  But I cannot tell you how useful this retrieval augmented generation support is.
[1346.74 --> 1357.68]  I have been finding it massively beneficial for research assistants, reviewing bills that have been coming out from different states and from the federal government,
[1357.78 --> 1362.04]  and then also contracts and just all kinds of little details.
[1362.04 --> 1372.20]  You can essentially interrogate a PDF and have it compare multiple types of language across multiple versions of a PDF and pull out different kinds of things.
[1372.40 --> 1377.32]  And it's just so incredibly useful when processing large amounts of documentation.
[1377.78 --> 1378.78]  Or, or, or, or.
[1379.40 --> 1380.00]  This is a good one.
[1380.00 --> 1386.80]  Last week, I took, like, a hundred emails from the Linux kernel mailing list, fed them all in there,
[1386.86 --> 1394.06]  and then I was able to essentially, you know, Q&A this mailing list and discussion and answer my questions and fill out my coverage.
[1394.18 --> 1395.84]  It's crazy how useful it is.
[1395.90 --> 1398.18]  So this is something I think I would use every day.
[1398.70 --> 1405.78]  Yeah, in terms of, like, the researching and digging through contracts and terms of service and, as you say, mailing lists,
[1405.78 --> 1409.48]  I think we'll get on to probably after the break with BeatCashFS.
[1410.00 --> 1422.48]  It's just, it takes hours out of your day of just trawling through incessant, you know, legal speak or random posts.
[1422.82 --> 1428.44]  It also supports, as of, I think about two weeks ago, they added a new feature called Code Interpreter.
[1428.76 --> 1435.66]  So this now allows models to dynamically execute code in real time to refine their own answers dynamically.
[1436.58 --> 1437.46]  Isn't that cool?
[1437.84 --> 1438.88]  That is great.
[1438.88 --> 1446.18]  I think it's also worth mentioning that Open Web UI supports web searches, which not all of these LLMs do right now.
[1446.28 --> 1447.40]  Some of them do, but not all.
[1447.86 --> 1447.96]  Right.
[1448.04 --> 1450.62]  So if you're a budding up-and-coming podcaster and you think to people,
[1451.16 --> 1455.78]  hmm, I want to summarize this massive long article into a digestible podcast segment,
[1456.42 --> 1459.86]  throw in the URL, and it will give you some bullet-pointed outputs to talk about.
[1460.16 --> 1462.88]  Yeah, or, you know, maybe you're in a meeting and you need to look smart real quick.
[1462.98 --> 1463.48]  Boop, boop, boop.
[1463.48 --> 1464.12]  Yeah.
[1466.44 --> 1467.10]  Yeah, maybe.
[1468.54 --> 1474.54]  I just think the features, you know, it's going to be, fasten your seatbelts, right?
[1474.54 --> 1477.24]  It's going to be bumpy with all the AI stuff that's coming along.
[1477.24 --> 1485.52]  And I think if, again, speaking to what we talked about at the top of the show, staying curious and educating yourself on what some of these self-hosted alternatives can do,
[1486.14 --> 1491.60]  you know, there will be companies that don't want anything to do with the cloud AI things that are happening right now.
[1491.66 --> 1494.82]  They'll want to keep it all on-premise and do everything locally.
[1494.82 --> 1503.02]  Now, you can argue to the blue in the face about the capabilities of, you know, Claude Sonnet versus Llama 3.3, whatever,
[1503.52 --> 1505.58]  and how much GPUs cost and all the rest of it.
[1505.68 --> 1511.24]  But for some people, regulatory things mean they have no other option than to do things on-premise.
[1511.42 --> 1513.12]  So keep yourself up to date.
[1513.30 --> 1514.34]  Take a look at OpenWeb UI.
[1514.50 --> 1516.98]  It's really just a fantastic tool.
[1517.22 --> 1521.46]  And the fact that it exists at all, I think, is a minor miracle.
[1521.88 --> 1523.80]  So check out the link in the show notes.
[1524.82 --> 1528.88]  Unraid.net slash self-hosted.
[1528.94 --> 1531.10]  So many great things are going on from Unraid.
[1531.18 --> 1535.66]  And I have heard from so many of you that have gotten to work now using Unraid 7.
[1535.96 --> 1537.18]  It just recently came out.
[1537.56 --> 1540.58]  Lots of nice improvements to ZFS and storage around there.
[1540.66 --> 1542.46]  Of course, the GUI tools got a nice refresh.
[1543.00 --> 1545.98]  The VM manager is sparkling great, as I say.
[1546.30 --> 1549.82]  And the Docker management is chef's kiss.
[1549.82 --> 1552.82]  The tail scale integration with your containers is...
[1552.82 --> 1556.72]  It's like I've always been doing for myself, but now they've just built it in.
[1556.88 --> 1558.58]  I've heard from some of you that just love that, too.
[1558.82 --> 1562.48]  The thing that I think is great about Unraid, and it just takes it to the next level with Unraid 7,
[1562.60 --> 1566.26]  is you can get started today with the hardware you have, the system you already have,
[1566.30 --> 1567.30]  and the disks that are in your closet.
[1567.36 --> 1568.84]  They don't necessarily have to match up.
[1569.20 --> 1570.40]  And you can start building out now.
[1570.40 --> 1575.60]  And they make it easy to get started with a lot of the applications and self-hosted things that we talk about right here in the podcast.
[1575.78 --> 1577.06]  You can get running on Unraid.
[1577.26 --> 1579.68]  Instead of taking months, it can take you a weekend.
[1580.26 --> 1582.88]  And, of course, we hear all the time that you want to have a solid home backup.
[1583.26 --> 1589.76]  And those of you that run macOS will probably appreciate that Unraid has excellent time machine support now,
[1590.24 --> 1592.02]  which is so convenient.
[1592.02 --> 1597.08]  If you have multiple Macs on your network, you can have them all backup to your Unraid system, and it works great.
[1597.66 --> 1599.22]  There's lots to love, really.
[1599.34 --> 1601.66]  And Unraid 7 just blows it out of the park.
[1602.00 --> 1604.48]  It's a fantastic release with lots of great features.
[1605.02 --> 1608.52]  And now with that tailscall integration with Docker 2, I just, oh, man.
[1609.04 --> 1612.36]  If I were building today, I'd go to unraid.net slash self-hosted.
[1612.42 --> 1614.16]  Check it out and support the show.
[1614.54 --> 1616.68]  Unraid.net slash self-hosted.
[1616.68 --> 1622.92]  So I was listening to another podcast the other day that goes by the name of Linux Unplugged
[1622.92 --> 1628.36]  that was talking about BcacheFS and sort of ZFS and ButterFS.
[1628.70 --> 1633.56]  And there's just this melange of server-grade file systems at the moment.
[1634.32 --> 1641.52]  And I heard on the Great Vine some drama has been, I don't really know how to phrase it, to be honest with you,
[1641.52 --> 1646.88]  but there's been some drama with Kent Overstreet, who is the main developer of BcacheFS.
[1647.70 --> 1650.86]  And I just, I thought maybe you'd break it down for us, Chris.
[1651.36 --> 1653.08]  Yeah, there are a lot of choices right now.
[1653.18 --> 1655.22]  I mean, obviously, we love ZFS.
[1655.80 --> 1663.06]  And I've been a ButterFS user for four or five years now on my, like, Raspberry Pi and Odroid-type systems,
[1663.12 --> 1664.68]  and then on my bigger x86 boxes.
[1664.68 --> 1667.46]  I've tended to go ZFS.
[1667.78 --> 1671.70]  But there is a challenger in development, like you said, called BcacheFS.
[1672.52 --> 1675.98]  But it's under active development.
[1676.24 --> 1678.26]  It's only recently been added to the Linux kernel.
[1678.84 --> 1685.40]  And there has been some hoopla around code of conduct and, you know, language
[1685.40 --> 1689.88]  and not groveling enough and apologizing enough.
[1690.10 --> 1692.98]  Kent apologized, but he literally did not apologize enough.
[1692.98 --> 1696.50]  And so they did suspend him from one cycle of the kernel.
[1697.18 --> 1698.04]  That's been reviewed.
[1698.18 --> 1700.80]  You know, they felt like, okay, you know, his penance has been paid.
[1700.88 --> 1704.00]  And so now he's actively contributing to the Linux kernel again.
[1704.22 --> 1707.60]  But there was also some hoopla from the Debian community.
[1708.46 --> 1712.12]  And I think this got picked up by some folks out there, like ours and whatnot,
[1712.30 --> 1715.80]  because he questioned the long-term supportability, the Debian maintainer,
[1715.90 --> 1719.78]  questioned the long-term supportability of BcacheFS tools.
[1719.78 --> 1724.46]  Jonathan Carter said that he sees several key issues.
[1724.60 --> 1728.44]  He thinks the development cycle of BcacheFS is too fast for Debian.
[1729.34 --> 1731.58]  Dependency management doesn't work the way he likes it.
[1731.70 --> 1734.40]  Works the way some other projects do, but doesn't work the way he likes it.
[1734.76 --> 1739.38]  It requires Rust dependencies, which, you know, that's tough for Debian.
[1739.68 --> 1740.56]  Rust is tough for Debian.
[1740.56 --> 1746.46]  And it's incompatible with certain upstream packaging policies of Debian.
[1746.52 --> 1748.90]  What makes Rust tough for Debian?
[1749.04 --> 1750.24]  Is it just the pace of development?
[1750.64 --> 1751.44]  Yeah, it's new.
[1751.72 --> 1756.94]  You know, if you were talking Arch or Gen 2 or Nix, it's a non-issue, right?
[1757.00 --> 1758.30]  But you're talking Debian here.
[1758.34 --> 1760.46]  You're essentially talking like getting the stuff into RHEL.
[1760.46 --> 1761.46]  Hmm.
[1761.72 --> 1762.02]  Yes.
[1762.10 --> 1768.16]  I mean, all of these things seem to honestly stem from Rust being added to the kernel.
[1768.92 --> 1770.54]  Either, what's your opinion?
[1770.70 --> 1773.38]  Was it too early or was it not early?
[1773.58 --> 1777.42]  Like, was it should have been added years ago or what?
[1777.54 --> 1781.10]  Well, if you wanted it in Debian today, it would have had to have been added years ago.
[1781.52 --> 1783.08]  But I kind of look at it like this.
[1783.08 --> 1784.86]  Like, it's got a LAN at some point.
[1784.86 --> 1788.00]  And so it's, you know, 6.12, 6.13, and 6.14.
[1788.16 --> 1789.98]  We're seeing a lot of active development here.
[1790.70 --> 1797.48]  But it'll take a couple of years for that to make its way downstream to Red Hat Enterprise Linux or Debian.
[1797.68 --> 1799.38]  And that's just kind of the natural process.
[1799.74 --> 1804.04]  The problem is, is that there's so much interest in BcacheFS.
[1804.24 --> 1805.34]  And we can get into why here in a moment.
[1805.40 --> 1809.66]  But there's so much interest in BcacheFS that users are pushing Debian.
[1810.04 --> 1812.30]  And they're trying to run it on their Debian systems.
[1812.30 --> 1814.16]  And they're doing custom builds and whatnot.
[1814.16 --> 1816.96]  Because there is so much demand for BcacheFS.
[1817.24 --> 1822.08]  And so it's creating tension in Debian earlier than it probably organically would have.
[1822.18 --> 1825.36]  If people just waited for Debian to get around to packaging and all this stuff.
[1825.72 --> 1829.86]  And as more things land upstream in the Linux kernel, it makes it easier for Debian.
[1830.96 --> 1834.30]  You know, so it won't be an issue forever.
[1834.60 --> 1839.74]  But it is the exact kind of issue that's going to have the most contention with Debian and projects like it.
[1840.20 --> 1843.10]  You want slow and stable, you get slow and stable.
[1843.36 --> 1843.44]  Right.
[1843.44 --> 1845.26]  That's the Debian mantra.
[1845.50 --> 1847.90]  And remember, Bcache isn't even officially released yet.
[1847.94 --> 1848.72]  It's still in development.
[1849.22 --> 1849.54]  Right.
[1849.86 --> 1850.06]  Yeah.
[1850.12 --> 1851.16]  So what's the alternative then?
[1851.36 --> 1856.38]  You know, don't use Debian with BcacheFS or just hack together your own implementation?
[1856.92 --> 1857.32]  Yeah.
[1857.68 --> 1857.98]  Yeah.
[1858.12 --> 1858.66]  Maybe that.
[1859.42 --> 1860.00]  I don't know.
[1860.58 --> 1861.86]  It's crazy to say.
[1861.96 --> 1865.26]  Some people have over 100 terabytes in production using BcacheFS.
[1865.62 --> 1867.00]  It's remarkable.
[1867.00 --> 1871.26]  There's very large setups out there in very big institutions running BcacheFS.
[1871.26 --> 1873.02]  So people are doing it.
[1873.58 --> 1876.88]  I don't personally think I want to put my important data on it yet.
[1877.00 --> 1878.70]  I'd run it as a file system for my laptop.
[1879.00 --> 1882.14]  But, you know, not my really long-term data I want to store just yet.
[1882.70 --> 1885.58]  Is it just one guy maintaining this thing right now?
[1886.18 --> 1886.46]  No, no.
[1886.54 --> 1887.16]  No, it's a team.
[1887.42 --> 1888.84]  It's definitely a whole team of folks.
[1889.20 --> 1891.72]  It was a passion project of Kent's for a long time.
[1891.72 --> 1896.20]  But it's sort of blossomed into a whole group of people and a big testing crew as well.
[1896.20 --> 1905.76]  So I wonder, like, for those people that are deep into the ZFS ecosystem, like myself, what would be some of the pros and cons of using one over the other?
[1905.98 --> 1911.06]  So you've got to start with the fact that BcacheFS is brand new, right?
[1911.16 --> 1916.60]  And it's designed using modern lessons learned from ZFS's design, right?
[1916.68 --> 1918.50]  And ButterFS and Extended 4.
[1918.76 --> 1923.48]  It's a new generation file system that's taking all the previous lessons learned, even from ZFS.
[1923.48 --> 1927.22]  And, of course, it's designed to be fully integrated into Linux kernel.
[1927.88 --> 1930.32]  So unlike ZFS, it won't face licensing issues.
[1930.84 --> 1935.56]  And that means one day better compatibility across all Linux distributions.
[1936.28 --> 1948.62]  Isn't it ironic that we seem to have faced more turbulence in the last six months from BcacheFS and Rust than we have from ZFS in the last few years?
[1949.30 --> 1950.76]  Yeah, or really ButterFS, too.
[1950.86 --> 1952.38]  ButterFS has just sort of been heads down.
[1952.78 --> 1953.18]  True.
[1953.48 --> 1954.66]  Trucking right along, you know?
[1954.78 --> 1957.64]  It's just one improvement after another with each kernel release.
[1958.24 --> 1960.20]  The thing is there's excitement about BcacheFS.
[1960.48 --> 1963.84]  You know, it allows granular control over data placement and replication.
[1964.68 --> 1967.80]  It can be configured for right through, right back, and right around caching.
[1968.60 --> 1972.10]  A lot of specialized setups for caching work great with BcacheFS.
[1972.34 --> 1975.32]  That's one of the reasons why there's some large production uses out there already.
[1976.46 --> 1980.62]  BcacheFS tracks device latency to automatically issue read requests to the faster device.
[1980.62 --> 1985.46]  And it's really kind of useful for people that have, like, mixed drive setups.
[1985.88 --> 1986.30]  Hint, hint.
[1986.56 --> 1986.92]  You know?
[1987.46 --> 1987.80]  Oh.
[1988.04 --> 1988.88]  Yeah, it's nice.
[1989.12 --> 1994.72]  Well, so if I have, like, an SSD cache, you know, in front of some spinners, that kind of thing.
[1994.72 --> 2003.52]  Yeah, or, you know, maybe you're using Unraid and you've got a bunch of mix-matched discs and brands, and a couple of them are stinkers and a couple of them are better performers.
[2003.94 --> 2006.26]  It'll sort of sort that out and compensate and figure it out.
[2006.72 --> 2007.08]  Okay.
[2007.08 --> 2007.78]  That sounds pretty neat.
[2007.78 --> 2009.82]  That sounds pretty cool, actually.
[2010.22 --> 2016.26]  And it's really efficient with system resources, especially compared to ZFS, but even ButterFS.
[2016.50 --> 2017.46]  I mean, it's a real fighter.
[2017.72 --> 2028.58]  So you could, you know, it's something that could scale from a Pi, a Pi 3 or a Pi 2, all the way up to, you know, like Netflix in production grade that's happening right now.
[2028.58 --> 2032.16]  And it's, they're looking forward already, right?
[2032.18 --> 2036.22]  So they're designing it for use cases that you can see from 2025 and beyond today.
[2036.96 --> 2042.68]  And I think that really matters because every time we can iterate on lessons learned, you know, you get something better.
[2042.82 --> 2047.68]  And the name, bcacheFS, it's a btree implementation, which is known to be high performance.
[2048.04 --> 2050.38]  Sort of like that's another reason why ButterFS went that way.
[2050.64 --> 2052.82]  It uses a key value store foundation.
[2052.82 --> 2055.02]  So it sits on stop of a key value store.
[2055.02 --> 2066.24]  And so operations are represented as keys that are inserted into various btrees, which I know that sounds complicated, but it actually simplifies complex operations and makes things faster.
[2066.42 --> 2069.08]  It has a sophisticated transaction model.
[2069.70 --> 2078.16]  And, of course, it has all the things you'd expect, like journaling, snapshot, like I mentioned earlier, encryption and tooling to recover data.
[2078.16 --> 2088.86]  So one of the big things that ZFS does so well is it operates at the block level, which means it's completely agnostic to the file system that sits atop it, really.
[2089.42 --> 2089.64]  Yeah.
[2089.88 --> 2091.72]  Does bcache do the same thing?
[2092.04 --> 2093.72]  I believe it's correct to say it does.
[2094.24 --> 2098.72]  It's controlling the disk and then it's controlling the abstractions that sit on top of the disk.
[2099.44 --> 2101.98]  And then, of course, you're formatting the file system with bcacheFS.
[2101.98 --> 2102.42]  Interesting.
[2103.64 --> 2103.88]  Yeah.
[2104.26 --> 2109.82]  So I'm thinking about some of the use cases there with, you know, mismatched drive sizes and all that kind of stuff.
[2109.92 --> 2111.22]  That's fascinating stuff.
[2111.60 --> 2122.92]  So I think, you know, going back to our Debian conversation, if Debian isn't the right target for bcache, people that want to experiment, like what is, in your opinion?
[2123.32 --> 2123.52]  Hmm.
[2124.20 --> 2129.28]  You know, I would have to imagine anything that's using a pretty recent Linux kernel.
[2129.28 --> 2136.54]  And then, of course, we at JB have tested it on Nix and we have it running on a couple of Nix systems.
[2136.86 --> 2138.28]  We need a Nix soundbite.
[2139.24 --> 2140.16]  Yeah, we do.
[2140.38 --> 2141.58]  A Nix jingle for real.
[2142.60 --> 2154.04]  And it's, you know, what is nice and different about these things, but you have to appreciate the difference here, is when something is fully integrated into Linux kernel and the Linux user space,
[2154.04 --> 2165.82]  it means you can use things like FSCK and all the standard commands you're used to, and they will all understand and be able to use bcacheFS, right?
[2165.90 --> 2171.46]  Now, there will be bcacheFS tools that are separate, but that's a big deal.
[2172.26 --> 2173.38]  Is the future bright, though?
[2173.48 --> 2179.04]  Like, are we at risk of some of this drama spilling over and bcache being kicked out of the kernel?
[2179.04 --> 2180.88]  No, no, I don't.
[2180.94 --> 2181.42]  I don't.
[2181.44 --> 2182.22]  I don't think so.
[2182.32 --> 2194.60]  I think, you know, there is a real – the Linux kernel, if you were to take it at stock, right, not modified, and then having the ZFS module plugged into it,
[2195.10 --> 2203.76]  if you were to take the stock Linux kernel, which ships on IoT devices and Android and everywhere that, you know, builds on top of Linux, they're using the stock kernel,
[2203.76 --> 2209.16]  it is very uncompetitive when it comes to file systems.
[2209.70 --> 2210.72]  XFS is pretty good.
[2211.40 --> 2212.28]  It's no ZFS.
[2212.80 --> 2216.46]  ButterFS is pretty great, but let's be honest, the reputation has been kind of damaged.
[2217.06 --> 2218.20]  People don't really trust it.
[2219.80 --> 2226.22]  Like, Apple – your iPhone has a better file system than the file systems that Linux offers by default.
[2226.22 --> 2234.98]  Now, APFS is a better file system than Linux offers by default if, you know – I mean, you could argue ButterFS, but –
[2234.98 --> 2235.72]  Why did you say that?
[2236.88 --> 2242.88]  Well, snapshots, volumes, encryption, all these things that we expect – Extended 4 doesn't do that.
[2243.30 --> 2245.40]  XFS doesn't do that, right?
[2245.40 --> 2250.02]  The stuff built into Linux kernel that most people are deploying by default, with the exception of ButterFS,
[2250.70 --> 2255.78]  doesn't support features that Windows has had for years and Apple's had for years.
[2256.30 --> 2262.24]  And so when you think about, you know, routers and IoT devices that could benefit from snapshots and things like that,
[2262.66 --> 2267.38]  having something like BcacheFS built in means all those things inherit that feature set.
[2267.38 --> 2272.20]  And they can run it on those minimal devices all the way up to massive enterprise-grade servers.
[2272.52 --> 2273.86]  They don't have to have a separate module.
[2274.18 --> 2278.78]  And all the tooling that you know, like FSEK and other things, work with this file system.
[2278.90 --> 2282.04]  So you don't have to learn new stuff to take advantage of it right away.
[2282.54 --> 2290.16]  Do you think we would have seen the rise of the immutable distro in quite the same way we have in the last couple of years
[2290.16 --> 2293.60]  if something like Bcache had been around sooner?
[2293.60 --> 2299.30]  You know, it's a good question because I was just trying GhostBSD for Linux Unplugged last week,
[2299.54 --> 2300.68]  and it's BSD, right?
[2300.78 --> 2305.82]  So ZFS baked in, no problem at all, no licensing issues there at all because they don't use GPL.
[2306.58 --> 2311.50]  And so GhostBSD, with its very basic package manager,
[2312.40 --> 2316.76]  automatically builds new boot environments for you after you do a system update.
[2316.76 --> 2323.76]  Like, this is like a minimal desktop with Mate and tooling that looks like it's Synaptic from, you know,
[2323.94 --> 2328.94]  2005 on the Linux desktop to install packages, and they can do boot environments.
[2329.26 --> 2335.60]  Because once it's in there by default, once it's built in, once it's like an API call away, if you will,
[2336.00 --> 2340.02]  then developers can just start building on top of it knowing it's there.
[2340.02 --> 2344.14]  But until it's baked in, it's never going to be like that.
[2344.20 --> 2347.24]  And that's the fundamental problem with ZFS and Linux.
[2347.32 --> 2353.64]  And while ZFS is great, you're never going to have all of the rest of the ecosystem build on top of Linux
[2353.64 --> 2356.00]  and just assume ZFS is there and they can do things.
[2356.04 --> 2356.68]  They just can't.
[2357.34 --> 2357.44]  Yeah.
[2357.80 --> 2360.26]  So what's the current state of the project then?
[2360.66 --> 2362.48]  What's been happening lately?
[2363.04 --> 2368.48]  The absolute most recent kernels that are in development are getting a lot of good stuff.
[2368.48 --> 2371.94]  I mean, Kent has really been knocking out of the park.
[2372.12 --> 2374.10]  The team that's testing stuff finds stuff.
[2374.30 --> 2376.30]  He's got a good core set of contributors.
[2377.10 --> 2383.54]  Online repair and scrub completes are landing, and that's huge.
[2384.16 --> 2387.56]  It might be like Linux 6.15 until really everything's there.
[2388.24 --> 2391.94]  I don't want to tell people it's ready yet, but, you know, it could be this year.
[2392.34 --> 2394.20]  And for a file system, that's a huge deal.
[2394.28 --> 2396.30]  These things take a very long time.
[2396.30 --> 2397.82]  This is a decade of development.
[2398.48 --> 2400.86]  That we're seeing kind of come together now.
[2401.28 --> 2404.10]  And all of it has been in the open.
[2404.20 --> 2408.98]  And I think that's something else to understand is ZFS, for the first five years,
[2409.22 --> 2411.40]  was held internally at Sun Microsystem.
[2411.58 --> 2415.82]  It was not made public until the Open Solaris project in 2005.
[2416.68 --> 2419.30]  And then, you know, we started seeing the process.
[2419.62 --> 2424.30]  But Bcash FS has been getting bike-shedded from the very beginning in the public light.
[2424.30 --> 2434.92]  And so every little, you know, argument and issue or bug has been analyzed and discussed and talked about for the last decade.
[2434.92 --> 2440.70]  And ZFS had the luxury of hiding for the first five years when it was probably in its most fragile state.
[2441.54 --> 2449.84]  And so, you know, and then it hasn't had the drama of having to contend to fight its way into mainstream Linux kernel,
[2449.84 --> 2454.08]  which is a process, as it should be.
[2454.56 --> 2456.98]  And, you know, and that's very public, too.
[2457.16 --> 2458.40]  ZFS has never had to do that.
[2458.40 --> 2465.96]  I wonder, like, shipping something as fundamental as a file system and tying it to the kernel release schedule,
[2466.84 --> 2470.14]  you know, that could potentially mean if you're on a, you know, Ubuntu or something,
[2470.32 --> 2474.58]  and you are on an LTS, you're not going to get a new kernel very often,
[2475.24 --> 2477.40]  which might mean that you are waiting.
[2478.04 --> 2479.70]  This goes back to Debian a little bit, too.
[2479.80 --> 2484.92]  But you're waiting for the new kernel before you can get a file system update.
[2484.92 --> 2488.28]  Is there any way to decouple, sensibly in your opinion,
[2489.06 --> 2494.66]  this development cycle of the file system from the kernel and yet maintain all those benefits?
[2495.30 --> 2499.42]  I wonder if you do it in part with feature flags like ZFS does today.
[2499.70 --> 2502.90]  You know, that's one way you could maintain a certain level of backwards compatibility.
[2503.62 --> 2507.44]  Of course, you could also update the user space tools separately.
[2508.12 --> 2510.22]  But this is kind of true for all file systems.
[2510.38 --> 2512.34]  True for anything that ships in the kernel, I suppose.
[2512.34 --> 2514.42]  Yeah, or a kernel module has to ship with the kernel.
[2514.42 --> 2514.68]  Yeah.
[2514.92 --> 2515.10]  Yeah.
[2516.12 --> 2520.44]  It probably, I think what you're touching on probably means early adopters of BcacheFS
[2520.44 --> 2526.68]  are probably not going to be best served by longer update cycle distros, at least at first.
[2526.90 --> 2528.94]  Unless, you know, maybe the 1.0 is really solid.
[2529.20 --> 2530.58]  I run Arch, by the way.
[2532.68 --> 2534.68]  Keeb.io slash self-hosted.
[2534.76 --> 2537.20]  K-E-E-B dot I-O slash self-hosted.
[2537.24 --> 2540.56]  Head on over there, sign up for the newsletter, and get 5% off your next order.
[2540.56 --> 2541.78]  Let's face it.
[2542.14 --> 2545.10]  Your keyboard might be one of the most important things you own.
[2545.50 --> 2547.14]  It took me a while to appreciate that.
[2547.24 --> 2550.92]  But, I mean, I'm interfacing with it every day, most of the day.
[2551.38 --> 2553.58]  It's the primary interface to my computer.
[2553.96 --> 2558.40]  And there's a lot of options out there, but I'm kind of somebody that likes a fancy keyboard now.
[2558.48 --> 2560.92]  I wasn't always this way, but I've seen the light.
[2561.50 --> 2566.36]  Keeb.io, they range from regular keyboards, and they really specialize in those cool split keyboards.
[2566.94 --> 2571.58]  And the keyboards, they'll come fully built, ready to use if that's how you like it, out of the box.
[2571.98 --> 2575.00]  Or you can get it as a kit and assemble it, do some hot swapping.
[2575.48 --> 2576.94]  There's no soldering for those parts.
[2577.02 --> 2578.82]  So it might be a fun project for home, too.
[2579.28 --> 2581.80]  Or, you know, if you just want to get started, you can get one that's fully built.
[2581.80 --> 2587.56]  The other thing that I think you should look at, and you could kind of up your game a little bit, is their macro pads.
[2587.80 --> 2590.68]  With those 9 to 16 keys, you can use them for all kinds of things.
[2590.78 --> 2594.04]  You can put phrases on there and have it connected to something like BitFocus.
[2595.02 --> 2596.58]  You could have it control OBS.
[2597.38 --> 2601.36]  You know, there's probably a way, using the Stream Deck software, to tie it in with Home Assistant as well.
[2601.62 --> 2604.02]  Or maybe it's a nice way to control your home media PC.
[2604.76 --> 2606.16]  I think those are so handy.
[2606.24 --> 2607.50]  We have a couple of them right here in the studio.
[2607.50 --> 2611.20]  In fact, I've got, look at this, I've got one right here.
[2611.80 --> 2615.70]  I love these little side things, you know, hook it up over USB.
[2615.86 --> 2616.58]  It's pretty great.
[2617.08 --> 2622.30]  I think people normally think of mechanical keyboards as loud and clicky, and those do exist.
[2622.70 --> 2628.80]  But they also have the versions with silent switches to keep things quiet and low-key in the office or at home, you know.
[2629.74 --> 2631.10]  I lack my loud typing.
[2631.30 --> 2632.36]  I'll be honest with you guys.
[2632.36 --> 2636.88]  But not everybody does, or sometimes the people around you don't.
[2637.52 --> 2640.08]  They stock lots of DIY parts and microcontrollers.
[2640.08 --> 2642.40]  And they're big supporters of open source.
[2642.48 --> 2644.16]  They publish the 3D print case parts.
[2644.42 --> 2648.42]  And they're also part of the core QMK team for the firmware.
[2648.62 --> 2650.76]  And all their boards use the QMK firmware.
[2651.34 --> 2652.78]  I love that.
[2653.44 --> 2654.94]  You deserve a great keyboard.
[2655.10 --> 2656.52]  Check them out and support the show.
[2656.90 --> 2660.18]  Go to keeb.io slash self-hosted.
[2660.26 --> 2663.62]  That's keeb.io slash self-hosted.
[2663.62 --> 2666.72]  All right, well, it's time for some feedback.
[2667.04 --> 2671.18]  Tom's Home Assistant tip, trick, or question came in through email, and he said,
[2671.60 --> 2679.66]  I thought I had a common solution to a common problem, but it looks like only about five people on the Home Assistant forums are using it.
[2679.78 --> 2681.00]  This is nuts to me.
[2681.00 --> 2682.66]  I hate when I see that.
[2682.78 --> 2693.22]  When I'm very much dependent on some integration or something, and I go to see the active user count integration on Home Assistant's page, and it says five people, it's like, oh, crap.
[2693.22 --> 2700.98]  He goes on, we've all discussed notifications before, but what about emergency notifications?
[2701.68 --> 2706.18]  Alerts so critical that they should interrupt anything, including sleep.
[2706.46 --> 2712.42]  Think smoke, freezes, floods, gas detection, intrusion, that kind of thing.
[2712.52 --> 2717.80]  Stuff that you need to know immediately, even when you're not physically present or asleep.
[2717.80 --> 2723.90]  Ideally, this should notify even non-tech-savvy folks, family or neighbors, as appropriate.
[2724.56 --> 2728.76]  My solution has been to adopt voice calls for this.
[2728.96 --> 2738.94]  It seems like a perfect, especially from an identification number perspective, solution to this problem that can break through the do-not-disturb modes on modern phones.
[2739.58 --> 2743.42]  So I've been using Twilio and Twilio Call to solve this problem.
[2743.42 --> 2744.44]  I see.
[2744.52 --> 2748.56]  And then he whitelists the Twilio phone number so it bypasses do-not-disturb.
[2749.00 --> 2753.96]  This is interesting, and where I could see it being useful is, like, the family or neighbors.
[2754.60 --> 2759.14]  I wouldn't want a phone call, but I'm curious what you do for urgent notifications.
[2759.42 --> 2762.82]  I have a couple set up now, and I'm wondering if you do.
[2763.42 --> 2763.94]  No.
[2764.26 --> 2765.72]  I'm thinking maybe I should.
[2765.94 --> 2766.20]  Yeah.
[2766.20 --> 2773.06]  I'm just wondering, like, I always think of your house as being so fragile.
[2773.54 --> 2782.50]  Like, you're exposed to the last two or three weeks the full force of atmospheric rivers and arctic blasts and snow and all this.
[2782.84 --> 2786.58]  Whereas I'm in my house, like, I don't really care too much what the weather's doing outside.
[2786.84 --> 2787.56]  It's fine.
[2787.70 --> 2791.20]  But maybe I should have a flood sensor or a leak detection thing.
[2791.20 --> 2800.72]  Yeah, you know, like a couple under a few sinks and one by the water heater or the, you know, washer and dryer is not, you know, it's not bad because you can catch stuff before it gets really bad.
[2800.80 --> 2809.98]  So I do this with my leak sensors, and I do use an automation that does send an urgent notification to all my devices.
[2810.42 --> 2812.56]  And I believe it does break through my do-not-disturb.
[2812.60 --> 2813.76]  I don't recall how I did that.
[2813.76 --> 2820.24]  And what has been universally the most beneficial has been the notification that makes it to my watch.
[2820.36 --> 2824.42]  Every time that has been the notification I have seen about a leak.
[2825.28 --> 2831.84]  So I am not a huge fan of depending on just communication via the phone.
[2832.96 --> 2842.54]  So another thing that I think what's important is you can change colors of lights, and there are Z-Wave and Zigbee sirens.
[2842.54 --> 2846.46]  And you can get some of them that are very loud.
[2846.80 --> 2857.32]  And so I have one outside the RV in an outside bay that if there is a significant flood in the RV, it will sound the siren so our neighbor knows too.
[2857.36 --> 2859.38]  So they could come over and turn off the water or something like that.
[2859.46 --> 2863.68]  So I went the siren route, and they just work great with Home Assistant.
[2863.68 --> 2863.72]  Awesome.
[2864.30 --> 2865.64]  That's a good plan.
[2866.24 --> 2876.68]  I've been thinking about this for the attic, notifications and things like that, because I'm going to be behind two doors acoustically detached from the rest of the house by design.
[2877.48 --> 2877.64]  Yeah.
[2877.84 --> 2884.54]  So I'm going to need some way of notifying me that, I don't know, dinner's ready or there's somebody at the front door or something like that.
[2884.64 --> 2884.78]  Yeah.
[2885.00 --> 2885.24]  Yeah.
[2885.24 --> 2885.76]  It's a good point.
[2886.20 --> 2887.12]  The Alex light.
[2887.34 --> 2887.44]  Yeah.
[2887.44 --> 2890.50]  So red means I need your attention now.
[2890.92 --> 2892.26]  Yellow means when you're available.
[2892.76 --> 2893.88]  And blue means it's food time.
[2894.62 --> 2894.94]  Ooh.
[2895.18 --> 2895.52]  Yeah.
[2896.50 --> 2897.00]  All right.
[2897.06 --> 2898.58]  Well, Joel wanted to send us a warning.
[2898.76 --> 2904.24]  He wrote in via email and says, hey, guys, a while ago you talked enthusiastically about the Nano KVM.
[2904.76 --> 2905.74]  Well, I picked one up myself.
[2905.74 --> 2907.98]  So much so that I bought a five pack.
[2908.64 --> 2909.52]  Oh, I should do that.
[2909.88 --> 2913.02]  He says, I never got around to using it, and now I'm kind of glad I didn't.
[2913.50 --> 2916.12]  Turns out the Nano KVM has serious issues.
[2916.24 --> 2918.86]  At best, poor security, but possibly something even worse.
[2919.24 --> 2921.48]  Check out the video, which we'll link in the show notes.
[2922.26 --> 2922.62]  Yes.
[2923.22 --> 2923.78]  AP...
[2923.78 --> 2925.68]  I never know how to say this guy's name.
[2926.42 --> 2926.90]  Apalardi?
[2929.42 --> 2934.00]  Apalardi's Adventures on YouTube went into great detail,
[2934.00 --> 2941.68]  talking about how this Nano KVM device exhibits several security issues in ranging severity.
[2942.38 --> 2947.52]  First of all is that they're using closed source software, making it difficult to verify their security.
[2948.50 --> 2953.02]  Next is that they download insecure binary libraries from the Internet
[2953.02 --> 2958.12]  and also use a weak encryption algorithm and plain text password storage.
[2958.88 --> 2959.06]  Yeah.
[2959.60 --> 2961.88]  I mean, those are definitely not best practices, that's for sure.
[2961.88 --> 2965.92]  I don't know if they're implicit security weaknesses, but they're not great security practices.
[2966.34 --> 2970.88]  And then on top of that, they have hard-coded DNS addresses, which bypasses any...
[2971.88 --> 2976.72]  I wouldn't say any network DNS security measures, but it bypasses quite a few,
[2976.88 --> 2977.80]  unless you know what you're doing.
[2978.72 --> 2983.48]  And they also enable unnecessary network communication, potentially exposing user data.
[2983.48 --> 2991.62]  Yeah, I hate this kind of stuff because it's really hard to know, is this intentional or is it just, you know,
[2992.16 --> 2993.14]  they don't know what they're doing.
[2994.04 --> 2994.88]  What's the phrase?
[2995.04 --> 2996.48]  Never attribute to...
[2996.48 --> 2997.48]  Malice, what could be...
[2998.10 --> 3000.90]  Incompetence, what can be attributed to stupidity or something.
[3000.90 --> 3001.02]  Yeah, okay.
[3001.46 --> 3003.96]  Never attribute malice, what could be attributed to stupidity.
[3004.04 --> 3004.60]  Yeah, that might be something.
[3005.32 --> 3006.60]  That might be what's happening here.
[3007.16 --> 3007.84]  Yeah, who knows?
[3007.84 --> 3011.48]  I mean, as far as we know, it's their first rodeo creating this kind of a device.
[3011.94 --> 3015.30]  And I want to give them the benefit of the doubt that they're going to fix this stuff over time,
[3015.36 --> 3019.14]  particularly given that some of the larger YouTubers are picking this up now.
[3019.74 --> 3020.90]  And plus, I suppose.
[3022.14 --> 3024.66]  It's been a golden year for IP KVMs.
[3024.76 --> 3025.94]  We've had the Nano KVM.
[3026.02 --> 3027.70]  Well, it started, of course, with the Pi KVM.
[3028.14 --> 3030.96]  But the trouble with that is it's a bit expensive to get involved with.
[3031.04 --> 3033.38]  You know, you want to buy the productized version, it's $300 or $400.
[3033.38 --> 3038.78]  The other option in that space is, well, it was the Nano KVM.
[3038.84 --> 3042.80]  They had the first mover advantage of being the cheap one, you know, $50 or less.
[3043.52 --> 3047.92]  Also now is the Jet KVM, which just landed on my desk just last week.
[3048.02 --> 3051.10]  So we will be doing a review of that in an upcoming episode as well.
[3052.24 --> 3058.96]  Now, I just want to say, if they wanted to alleviate a lot of our concerns,
[3059.32 --> 3061.52]  they could just open source the firmware.
[3061.52 --> 3065.26]  I know they'd probably be worried about competition, but competition's coming anyways.
[3065.78 --> 3070.44]  You could just open source everything that's the chips on the thing and solve a lot of these problems.
[3071.58 --> 3072.18]  Just saying.
[3072.76 --> 3077.10]  One of the other issues linked in the description of the YouTube video is that Nano KVM bundles
[3077.10 --> 3081.46]  an outdated and sci-ped hosted version of Tailscale.
[3081.62 --> 3083.98]  So yes, maybe I should get on top of that one.
[3084.46 --> 3085.70]  Jeez, thanks, guys.
[3085.70 --> 3087.38]  All right, another email.
[3087.88 --> 3093.84]  WH-20-250 is deep in the Home Assistant rabbit hole.
[3094.38 --> 3098.32]  It says, I was blown away when Home Assistant instantly found all the devices on my LAN,
[3098.42 --> 3099.98]  pulling them into one interface.
[3100.46 --> 3104.98]  No more remembering which device was on Google or Amazon or Control 4.
[3105.20 --> 3107.00]  And they all, of course, had their own apps.
[3107.00 --> 3113.02]  Then I discovered Hacks and the add-on store, opening up even more possibilities,
[3113.32 --> 3117.02]  which has definitely led me down the self-hosting rabbit hole and your podcast.
[3117.48 --> 3120.34]  So now we fast forward to today.
[3120.70 --> 3128.26]  He's got a VM setup on Unraid on a Dell PowerEdge R730XD with 128 gigs of RAM.
[3128.26 --> 3130.12]  He's got PFSense and a VM.
[3130.66 --> 3134.84]  And he's got a few Docker containers, including Image.
[3135.24 --> 3135.70]  Yes.
[3136.28 --> 3136.92]  Jellyfin.
[3137.32 --> 3137.68]  Yes.
[3138.16 --> 3138.76]  Nextcloud.
[3139.10 --> 3139.60]  Righteous.
[3139.86 --> 3140.82]  And Matrix.
[3141.30 --> 3147.00]  And he's expanding his LAN storage from 1.5 terabytes to 32.5 terabytes.
[3147.18 --> 3148.10]  That's a modest upgrade.
[3148.42 --> 3151.02]  I love it.
[3151.54 --> 3156.64]  So now he's thinking about maybe a low power failover PFSense box or OpenSense box,
[3156.64 --> 3157.80]  if you have any suggestions.
[3158.26 --> 3162.76]  And he's resisting the urge to build an even bigger server in the HL15 case.
[3162.82 --> 3164.18]  So he might like your perspective there.
[3164.80 --> 3168.08]  He says, if I cave, I'll send the Dell box to my oldest daughter as an off-site backup.
[3168.28 --> 3170.82]  Oh, he's already getting the justification ready, Alex.
[3171.20 --> 3171.70]  I love it.
[3171.90 --> 3172.10]  Yep.
[3172.54 --> 3172.82]  Yep.
[3174.28 --> 3175.52]  I think he's on the right track.
[3175.58 --> 3176.42]  I say go for it.
[3176.90 --> 3177.06]  Yeah.
[3177.08 --> 3181.56]  That email was actually the one that we talked about with the 20,000 SAT boost in the last episode.
[3181.90 --> 3183.80]  So I'm very glad that that got sent through.
[3183.80 --> 3189.74]  And I think, you know, from an OpenSense perspective, I've written a post on my blog,
[3189.80 --> 3194.60]  which I'll put a link to in the show notes, talking about like a very low frills OpenSense build.
[3195.26 --> 3201.62]  But to be honest with you, as long as the device has a pair of Intel Nix at the speed that you want,
[3201.62 --> 3205.70]  so at least gigabit depends on your WAN connection these days, you might need two and a half.
[3206.26 --> 3211.86]  As long as it has a pair of Intel Nix, you should be good to go for pretty much anything with PFSense or OpenSense these days.
[3212.42 --> 3212.60]  Yeah.
[3213.20 --> 3219.74]  You know, I'd say, you know, just take your time and maybe do consider going with the larger system as well.
[3219.74 --> 3224.80]  Because, I mean, just think of everything you've learned since you started this journey.
[3225.62 --> 3236.16]  I mean, you went from Google and Amazon controlling all your stuff to now look at you with your image and your jellyfin, your NixCloud and your matrix.
[3236.82 --> 3238.08]  And backups at your daughter's house.
[3238.26 --> 3238.46]  Yeah.
[3238.82 --> 3239.14]  Love it.
[3239.46 --> 3240.96]  This is some real progress.
[3241.14 --> 3242.90]  And so I think you should be proud of that.
[3242.92 --> 3243.82]  And thanks for sharing it with us.
[3243.82 --> 3250.14]  My favorite part of the email is, I'm not sure if I should thank you for all I've learned or blame you for my addiction.
[3250.98 --> 3251.38]  Yeah.
[3251.58 --> 3251.92]  Okay.
[3252.06 --> 3252.32]  Fair enough.
[3252.32 --> 3253.60]  Either way, keep doing what you're doing.
[3253.72 --> 3254.98]  Well, thanks for writing in, good sir.
[3255.38 --> 3257.76]  And keep up the good work, right?
[3258.38 --> 3259.14]  Yeah, exactly.
[3259.74 --> 3266.14]  Gene Bean comes in with 7,570 sats for our top four boosts this week.
[3266.18 --> 3267.28]  And he kicks it off.
[3267.28 --> 3271.34]  He says, did you guys look at the EcoWits Wit Boy?
[3271.44 --> 3273.10]  I'm just curious over the Tempest.
[3273.10 --> 3274.40]  I did not.
[3274.50 --> 3276.00]  But looking at it now, it looks pretty great.
[3276.80 --> 3279.42]  Well, since the last episode, I actually went ahead and purchased the Tempest.
[3279.60 --> 3280.62]  And I'm going to say it.
[3280.70 --> 3282.16]  I love this thing.
[3282.54 --> 3285.30]  But the Wit Boy also looks pretty cool.
[3285.40 --> 3289.44]  It comes with this sort of e-ink looking external tablet display thing.
[3289.68 --> 3290.22]  Yeah, that's nice.
[3290.74 --> 3291.14]  Yeah.
[3291.92 --> 3296.34]  But what I will say about the Tempest is that the installation was a piece of cake.
[3296.64 --> 3298.14]  Exactly like Chris described.
[3298.14 --> 3307.20]  You know, it just opens up a UDP port and Home Assistant picked it up with the Weather Tempest or Weather something integration.
[3307.62 --> 3308.22]  Piece of cake.
[3308.92 --> 3314.06]  But it looks like this other device, the Wit Boy, has the haptic rain sensor as well as an ultrasonic wind sensor.
[3314.44 --> 3316.22]  It looks very similar, to be honest with you.
[3316.42 --> 3316.54]  Yep.
[3316.54 --> 3318.18]  And 900 megahertz back to the base.
[3318.46 --> 3322.70]  But their base, I guess, has an Ethernet port, which that'd be kind of nice.
[3322.94 --> 3323.52]  Oh, no.
[3323.68 --> 3330.26]  Now, and also, the Tempest guys had a President's Day sale literally two days after mine arrived.
[3330.26 --> 3331.96]  With like 50 bucks off.
[3332.38 --> 3336.04]  So the nice thing about Wit Boy is that it would appear to be a little bit cheaper.
[3336.34 --> 3339.96]  The Tempest is in the $330 range, standard MSRP.
[3340.42 --> 3348.86]  Whereas this one appears to be in the $200-ish range, depending on a bunch of frequency stuff, depending on which country you live in.
[3349.00 --> 3351.18]  So it's a little bit cheaper.
[3351.32 --> 3355.54]  And it comes with a display tablet, too, which could be nice for you.
[3355.54 --> 3360.64]  He also points us to Shelf Player, which is an audiobook shelf client for iOS.
[3361.04 --> 3364.80]  And it looks really, really good.
[3365.58 --> 3367.84]  I mean, just a great UI design in general.
[3368.36 --> 3375.58]  I think if you're on iOS, I just, I think on iOS, because I don't use it as much anymore, my audiobook shelf beta app just expired as well.
[3376.00 --> 3378.28]  So Gene literally could not launch it this week.
[3378.36 --> 3381.16]  So it's called Shelf Player, and I'll put a link in the show notes.
[3381.16 --> 3391.00]  Yeah, it's worth noting it's $4.99 in the App Store as well, but plugs in with audiobook shelf and looks really nice.
[3391.12 --> 3391.82]  Yeah, like Chris said.
[3392.24 --> 3392.60]  Interesting.
[3392.84 --> 3394.08]  Interesting that it's five bucks.
[3394.74 --> 3395.04]  Huh.
[3395.42 --> 3400.30]  You know, I just, I didn't expect that because it's a Mozilla public licensed app.
[3400.42 --> 3402.86]  But I guess there's really no way to distribute it for iOS.
[3403.20 --> 3405.40]  So if you want to buy it on the App Store, they can charge.
[3406.38 --> 3406.98]  That's great.
[3407.34 --> 3409.24]  It's open source, but what are they going to do, right?
[3409.24 --> 3417.58]  But also Gene pointed out, oh my God, Gene, I can't believe you found this, that I actually have multiple Mastodon profiles.
[3418.20 --> 3423.74]  I guess I have one on LinuxRocks.online that I set up on May 14th of 2017.
[3424.84 --> 3428.10]  So I don't use it much.
[3428.82 --> 3434.46]  Of all the people that listen to this show, Gene Bean, you are a gentleman and a scholar for finding that.
[3434.58 --> 3435.18]  Good job, sir.
[3435.32 --> 3435.90]  Thank you, Gene.
[3435.90 --> 3439.96]  AlexMorass82 came in with 5,000 sats.
[3440.20 --> 3441.12]  Loving Pangolin.
[3441.48 --> 3443.90]  I got it and I created a Home Assistant add-on.
[3444.80 --> 3449.94]  He created it so that I could share the remote access to the family and reuse and use it over tailscale.
[3450.04 --> 3451.58]  It's available at github.com.
[3451.64 --> 3452.10]  He puts his ad.
[3452.14 --> 3453.28]  I'll put it in the link in the show notes.
[3453.86 --> 3457.30]  But it's a hash-addon-newt, N-E-W-T.
[3458.16 --> 3458.52]  Wow.
[3458.58 --> 3458.98]  How about that?
[3459.00 --> 3459.60]  He made that.
[3459.60 --> 3460.16]  Yeah.
[3460.46 --> 3468.78]  Well, one thing we didn't talk about at all with Pangolin in the last episode, we just ran out of time, was that the links can actually be authenticated as well.
[3468.88 --> 3477.74]  So you can create your own different types of auth for your own self-hosted Cloudflare tunnel alternative, which is what Pangolin ostensibly does.
[3477.74 --> 3485.72]  And adding that into Home Assistant seems like a completely logical next step for family members that refuse to use tailscale for whatever reason.
[3486.48 --> 3487.60]  So great job there, Alex.
[3487.92 --> 3488.30]  Yeah, really.
[3489.04 --> 3494.88]  Brad came in with a shout-out from Team Toronto, the group up there in Toronto, feels like it was forever ago.
[3495.00 --> 3497.66]  He says he's loving Docker Compose Generator.
[3497.66 --> 3498.94]  Oh, very good.
[3499.06 --> 3508.24]  Yes, that's an Ansible repo that I maintain that takes in a bunch of YAML files and spits out a formatted Docker Compose file.
[3508.84 --> 3510.14]  I hope everything is okay up there in Toronto.
[3510.26 --> 3511.84]  I know you guys had a lot of snow this week.
[3512.10 --> 3514.44]  We're talking feet worth of snow, apparently.
[3514.86 --> 3515.04]  Yeah.
[3515.26 --> 3517.74]  And you have planes landing upside down, so we're thinking of you.
[3518.48 --> 3518.90]  Too soon.
[3519.24 --> 3519.54]  I know.
[3520.00 --> 3523.94]  And our last one to round out the top four is Bronzewing came in with a row of ducks to say,
[3524.08 --> 3526.26]  I remember the dash cams came up recently.
[3526.26 --> 3531.78]  I had to get some strike funds to settle, but I wanted to recommend Vortex Radar on YouTube.
[3532.10 --> 3536.32]  They've been a great source of info on dash cams and primarily radar detectors.
[3537.34 --> 3539.08]  That's Vortex Radar on YouTube.
[3539.68 --> 3540.56]  Yeah, that's a great channel.
[3540.74 --> 3541.26]  Great recommendation.
[3541.56 --> 3541.88]  Thank you.
[3542.52 --> 3543.30]  So thank you, everybody.
[3543.52 --> 3545.70]  Our SAT streamers really did a heavy lift this week.
[3545.80 --> 3551.14]  38 of you streamed those SATs as you listened and stacked 58,748 SATs.
[3551.14 --> 3557.18]  And you combine that with our boosters, the show's stacked 105,762 SATs.
[3557.56 --> 3558.30]  We really appreciate it.
[3558.58 --> 3562.58]  Everybody's boost is read and saved, and we will link them all in the Boost Barn in the
[3562.58 --> 3563.98]  show notes if you'd like to read through them.
[3564.40 --> 3565.28]  It's really easy to boost.
[3565.34 --> 3568.44]  You just get some SATs with something like Strike or Bitcoin Well or River.
[3568.76 --> 3569.28]  I don't care.
[3569.28 --> 3571.12]  And then you boost it with something like Fountain.
[3571.48 --> 3575.10]  And then you get your message on the show, and you support us all using self-hosted
[3575.10 --> 3575.56]  infrastructure.
[3575.84 --> 3576.62]  Thank you, everybody.
[3577.04 --> 3577.86]  We really appreciate it.
[3578.36 --> 3582.56]  We also need to say a big thank you to our site reliability subscribers, our SREs.
[3582.94 --> 3586.10]  You make the show possible as well with your fiat fund coupons.
[3586.52 --> 3590.16]  You can go to self-hosted.show slash SRE and support the show.
[3590.40 --> 3595.52]  We also do an ad-free feed for those of you that are members with an additional post show
[3595.52 --> 3595.86]  as well.
[3596.16 --> 3598.02]  A little extra content to say thank you for the members.
[3598.02 --> 3599.16]  You really are our foundation.
[3599.70 --> 3605.50]  You can find me over at chrislas.com if you want to try out the wild side or, I don't
[3605.50 --> 3606.82]  know, maybe you want to try out Matrix.
[3607.08 --> 3609.06]  We've got some self-hosted chat rooms over there, too.
[3609.12 --> 3612.66]  We have details for our Matrix at jupiterbroadcasting.com slash Matrix.
[3613.48 --> 3615.24]  Oh, look at you with the chrislas.com.
[3615.66 --> 3617.36]  Yeah, you know, I just pointed at stuff.
[3618.04 --> 3620.40]  We need to get your self-hosted link tree up there, my boy.
[3620.42 --> 3621.12]  Yeah, you should, huh?
[3621.42 --> 3622.54]  Yeah, I might.
[3622.80 --> 3626.20]  And you can find my self-hosted link tree at alex.ktz.me.
[3626.56 --> 3628.92]  And until the next episode, thank you very much for listening.
[3628.92 --> 3632.14]  That was self-hosted.show slash 143.
[3632.14 --> 3632.62]  Here we go.
[3632.62 --> 3634.64]  Okay, let's dive in.
[3634.64 --> 3634.82]  Everybody.
[3635.02 --> 3635.74]  Here we go.
[3635.96 --> 3636.30]  Let's dive in.
[3644.56 --> 3644.92]  What?
