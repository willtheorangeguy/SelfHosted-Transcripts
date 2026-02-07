[0.00 → 4.64] Well, somehow the last episode of Self-Hosted is here, episode 150.
[5.36 → 10.08] And to celebrate, if that's the right word, to celebrate the occasion, to mark the occasion,
[10.58 → 14.30] I'm joined by some longtime friends of the network.
[14.78 → 18.34] We've got Was, Brent, Drew, and of course Chris here today.
[18.42 → 18.94] Hello, folks.
[19.26 → 19.52] Hello.
[20.30 → 21.28] And goodbye.
[21.86 → 22.70] Well, hi.
[23.20 → 23.58] Hello.
[24.16 → 24.64] Hi, gentlemen.
[24.90 → 26.12] Nice to have you here for the last one.
[26.12 → 30.92] And Drew is one of those unsung heroes that we mention our editor quite often behind the scenes,
[31.00 → 32.94] but truly he is one of the best in the business.
[33.86 → 36.34] And I thought, I mean, he's been on the show before.
[36.44 → 38.62] I think he came on and talked about 3D printing a while ago.
[38.98 → 39.76] That sounds right.
[39.98 → 42.44] And of course, we all know Brent and Was from Linux Unplugged.
[42.62 → 43.20] Oh, hi.
[43.84 → 44.66] Hello again.
[44.96 → 48.52] And Brent's, you know, he's almost the third co-host of the Self-Hosted podcast.
[48.74 → 49.14] He's been on some of the episodes.
[49.14 → 49.98] By this point, yeah.
[49.98 → 52.84] Am I the most guested, you know, guest there is?
[52.84 → 53.16] I bet.
[53.72 → 54.16] You are.
[54.16 → 58.82] I had a listener send me in a bunch of stats that they'd used AI to trawl our RSS feed.
[59.32 → 59.64] Excellent.
[59.82 → 64.06] And you were like three times in the lead as being the most guested.
[64.16 → 65.52] When the show started, that was my goal.
[66.00 → 66.24] Ha ha.
[66.58 → 66.94] Was ha.
[67.72 → 71.06] I swear, actually, when the show started, your goal was to build a home server.
[71.14 → 72.12] How did that turn out?
[72.12 → 75.96] Oh, you know, somehow in this episode, I was hoping you wouldn't ask me that question.
[76.34 → 78.36] I think it's in perpetual building mode.
[78.46 → 79.96] I think that's just how I like it.
[80.48 → 82.62] But to be honest, there are a couple servers.
[82.62 → 94.00] I mean, now this whole van bus purchasing adventure that we've been tracking on Linux and Plugged and throughout the network means that I've got a little tiny studio in a vehicle on wheels.
[94.22 → 96.40] Thanks to Chris inspiring me for years.
[96.66 → 98.28] You finally have to learn to self-host.
[98.38 → 99.12] You're forced into it.
[99.18 → 99.66] It's bizarre.
[100.22 → 100.60] It's weird.
[100.60 → 101.68] I don't know if I like this, guys.
[102.76 → 106.90] And then this server that we've talked about here a couple of times.
[106.96 → 110.78] Alex is actually some of your old hardware thrown in a little box here in my cabin.
[111.54 → 112.62] That thing's been kicking.
[112.90 → 113.66] It's been doing great.
[114.00 → 118.78] I haven't lived here for, what, like two months now since we've been travelling so much.
[118.82 → 124.56] And it's just been going the whole time, just sucking in some of my data, doing all the things, doing backups and stuff.
[124.56 → 127.16] So I would say it's going pretty good.
[127.26 → 129.40] As self-hosting goes, it could always be better.
[129.52 → 132.06] There are projects on the list, but it's been reliable.
[132.32 → 134.18] So it's better than it's ever been.
[135.42 → 141.02] Well, I feel remiss that we didn't cover this right off the bat, but I believe it's your birthday today, isn't it?
[141.28 → 143.32] It happens to be my birthday as we record.
[143.42 → 143.60] Yes.
[143.82 → 143.98] Thank you.
[143.98 → 144.66] As we record.
[144.76 → 145.42] Happy birthday.
[145.70 → 146.48] Oh, thanks.
[147.02 → 147.56] Happy birthday.
[147.78 → 148.36] Thank you, gents.
[148.36 → 152.22] For your birthday, we got you the last episode of Self-Hosted.
[152.38 → 152.58] Oh.
[153.18 → 153.80] Can I have more?
[155.68 → 157.14] Don't listen to it all in one place.
[158.82 → 161.28] Yeah, 0.5 speed this time, 0.5.
[161.68 → 161.84] Yeah.
[161.84 → 170.90] Yeah, I think throughout the show, I was going through and kind of like recounting some of the bigger migrations I made.
[170.90 → 179.00] And I think two that stand out for me was migrating my main server at home from Ubuntu LTS to Nix OS.
[180.08 → 189.72] And going from a Home Assistant early on in the show, going from a Home Assistant core installation to a full Home Assistant OS with a supervised installation.
[189.72 → 194.78] And kind of rebuilding, choosing not to import, but to rebuild my Home Assistant from scratch.
[194.78 → 203.84] Which, that was like really early, and I still now have that same install running on that yellow from whatever episode we covered that, you know, years ago now.
[203.92 → 204.94] Four years ago, probably.
[206.02 → 208.46] Whenever the green first shipped, like that week.
[209.16 → 210.18] And it's still up to the task?
[210.24 → 211.06] Are you itching for an upgrade?
[211.18 → 214.02] Well, I am feeling like it's getting a little tight on RAM.
[214.36 → 216.10] You know, the thing only has two gigs of RAM.
[216.10 → 216.42] Ooh.
[216.64 → 221.26] And Brent set up a luxurious eight gig RAM unit in his van, and I really started to get a little jealous.
[221.26 → 230.68] But practically speaking, it works, except for when I'm doing ESP builds, and I'm building like the new update for my ESP home devices.
[231.92 → 238.40] It generally runs out of RAM, and the builds fail, unless you go into the configuration and say, only one build thread at a time.
[239.02 → 240.02] Keep it real low-key.
[240.56 → 241.56] No parallelism for you.
[241.66 → 242.24] Yeah, exactly.
[242.54 → 245.00] And then it manages to successfully do it.
[245.02 → 245.74] It's just really slow.
[246.62 → 249.98] You know, back when we started the show, you were Mr. Raspberry Pi almost.
[249.98 → 253.40] I mean, how many – I swear you were running like half a dozen at some point.
[254.14 → 254.80] Yeah, it really was.
[254.90 → 257.46] And they were Ubuntu, and that was for me.
[257.96 → 269.68] When you could take regular standard industry Ubuntu or whatever you wanted, and you could deploy it on a Raspberry Pi, and the 4 came along, and you had the CM4 module and all of that.
[269.78 → 274.74] Like, it really was a new world of low power, but enough horsepower.
[275.62 → 279.30] And that was perfect for my off-grid needs, running off battery power whenever I could.
[279.30 → 280.30] And it's kind of interesting.
[280.72 → 282.88] In a way, like, things swapped for you, right?
[282.94 → 288.72] Like, you started using some of the ARM systems that Apple came out with during the run of the show.
[289.22 → 294.54] But on the flip side, x86 got competitive at the low end, where you could swap the Pies to x86.
[294.76 → 294.90] Yeah.
[295.08 → 296.10] And I think I went – you're right.
[296.10 → 301.12] I think I had, like, in total all over the place, six Raspberry Pis in production at the peak.
[301.32 → 303.68] Then in my home RV, I had four.
[304.34 → 307.50] And now I have one real Pi left.
[307.56 → 310.52] And then if you count the Pi KVM, I have two Pis in production still.
[310.80 → 314.76] Didn't you have enough Pis in your RV that you actually had thermal issues?
[315.02 → 315.30] Yeah.
[315.44 → 315.64] Yeah.
[316.94 → 319.34] It was also just hot in the RV, but it was a problem.
[319.82 → 320.24] It was.
[320.24 → 327.04] But the thing I loved about it is I had another Pi ready to go in the same case, everything with the same – you know, the connection layouts.
[327.68 → 336.60] And so if I popped a Pi, you just disconnect all the storage and the accessories, mount the new Pi in and reconnect everything, and you're right back where you – so I loved that.
[336.70 → 338.26] Pretty low cost to have a hot swap there.
[338.26 → 338.46] Yeah.
[338.60 → 338.84] Yeah.
[338.84 → 345.94] But ultimately, I was able to use one Droid H3 to do the work that all those Pis did and still have a headroom.
[346.76 → 346.90] So.
[348.08 → 349.68] I think that's what changed, really.
[350.00 → 362.68] There was a glut of used x86 machines, small form factor Dell boxes, Lenovo boxes, came on the used market during the pandemic because nobody was in the office anymore.
[362.68 → 370.52] And then people realized how awesome and how low power those – and powerful those boxes were, as well as things like the Droid, whatever you got, the H3, I think.
[371.54 → 381.32] And Quick Sync obviously became a real workhorse during that period, too, for some of the – you know, some of the stuff we needed horsepower for, we no longer did.
[381.56 → 384.68] And it just meant that you could put everything into one place.
[384.68 → 397.30] I would imagine that's going to change here in a bit with all these, like, AI requirements because even small tasks that are being required in various projects require more than those can offer.
[397.76 → 399.46] So do you guys think?
[399.50 → 399.84] I think.
[399.94 → 404.34] But do you guys think there will be some shift now where the requirements will just take a big hop?
[405.08 → 406.90] Can you tell Brent's just back from Red Hat Summit?
[407.68 → 408.24] I guess.
[408.24 → 411.66] Well, local AI is a bit of a weird one.
[412.22 → 417.04] And obviously that's been the trend of the last, what, 12 to 18 months or so.
[417.88 → 421.46] Llama's come along with a bunch of local models.
[422.18 → 423.70] But you still need something to run them on.
[423.94 → 425.52] And there are a couple of ways you can do that.
[425.52 → 433.42] One is to have a CPU-based model, which if you've ever tried to run Llama on CPU only, it's not very good.
[434.80 → 437.12] You could then use, like, an NVIDIA GPU.
[437.12 → 441.82] You know, I've got an A4000 in my server, which I share with a few people over Tail scale.
[442.34 → 445.98] And they can all come in and sort of share one GPU amongst a few friends.
[446.24 → 450.32] And with a decent internet connection, that works pretty well because it's all API-driven anyway.
[451.14 → 457.04] Or you could buy a Mac Mini or a Mac Studio or something and load that up with a unified memory.
[457.40 → 465.10] And then suddenly you've got a neural processor that can have 64, 128 gigs worth of RAM at its disposal.
[465.10 → 470.42] The downside, of course, is that you have to run macOS as a server, which can be a bit of a challenge.
[471.12 → 474.50] To your question, Brent, I think it's going to depend on a lot of use cases.
[474.88 → 477.80] There's a ton of people out there that are never going to be interested in local AI.
[478.18 → 481.36] And I don't think it's going to be an issue for them.
[481.46 → 485.22] But for people that do want to experiment with it, it is moving up the requirements.
[485.88 → 489.38] My next system, I'm probably going to try to make sure it has a GPU in it.
[489.38 → 498.30] Even just for show production, stuff like whisper transcriptions, when you want to have diarized transcriptions of the shows, stuff like that.
[499.04 → 501.24] That stuff loves GPUs.
[501.48 → 503.30] It's not just AI that we can use it for.
[503.50 → 504.80] Like transcoding is one thing.
[505.30 → 506.46] AI inference is another.
[506.66 → 508.64] But there are other things we can use it for, too.
[509.48 → 514.04] Speaking of Red Hat, they do kind of have an interesting project for this problem.
[514.04 → 517.16] They have something that they are calling LLMD.
[517.94 → 526.18] And if you think about the way things are named on Linux, calling something LLMD is a really bold statement about the ambition and the scope of this project.
[527.00 → 535.86] And you could think of it as playing a role in helping distribute the back-end inference to the best-suited technology.
[535.86 → 544.48] So you could have an AI job on your LAN that maybe isn't that complicated and could run on a LLMD on a consumer-grade system.
[544.72 → 548.48] And so LLMD can help distribute to that local system.
[549.26 → 551.64] And then you have another job that's a little more serious.
[551.76 → 557.10] And based on the inference work and some instructions, it realizes, actually, I need to go spin this up on OpenAI.
[557.42 → 561.70] Or I need to go spin this up on whatever Azure's API endpoint is.
[561.70 → 567.00] And so you have, as a user, one common local interface and language.
[567.42 → 573.06] And then on the back-end, LLMD is doing some of the inference decision to decide where it should distribute that workload.
[573.54 → 581.96] And so you could kind of see a future where maybe 80%, 90% of your quote-unquote LLM AI jobs are done locally.
[582.10 → 583.20] Maybe it's speech recognition.
[583.48 → 585.04] It's commanding to your home assistant.
[585.20 → 587.20] It's real basic stuff that's already pre-cached.
[587.26 → 588.24] That's always staying local.
[588.24 → 596.20] But then something that's a little bit more complicated or requires an outside data source, like weather data or something like that, maybe then that gets distributed off to the cloud.
[596.84 → 599.34] And so you could have this system where it's a little bit of both.
[599.90 → 605.62] Yeah, I mean, I've been using a bunch of Open Router and some local stuff already just with things like OpenWebUI.
[605.80 → 607.00] So I bet that continues.
[607.00 → 620.94] I think I've seen a lot of folks in our community and more generally setting up tools like OpenWebUI just because even if you're just a casual user at this point, you're already hitting the subscription fatigue of just trying to use two AI services seriously.
[621.60 → 621.90] Yeah.
[622.00 → 633.38] I think the orchestration idea of really orchestrating out your LLM decisions is a fascinating and good direction to take the industry.
[633.38 → 652.80] Now, in honour of this being our final episode, I still don't like saying that, to be honest, but we can send people over to JupiterGarage.com where there is some limited edition merch available, a T-shirt, a dad hat, posters, you know, with all the episode titles, all that kind of stuff.
[653.54 → 655.42] Head over there whilst it's still available.
[656.32 → 657.52] Limited time only.
[657.52 → 664.94] That's right, Was, paying for a limited time only, which we don't really know how limited, but I imagine until supplies run out, which could be any day now.
[666.46 → 668.32] Yeah, who knows with the state of the world.
[669.14 → 675.62] One thing that definitely does have a limited supply, though, is the stuff in my personal garage sale.
[675.66 → 679.22] I mentioned in the last episode that we're selling the house, moving back to the UK.
[679.22 → 683.00] So everything in this house pretty much must go.
[683.10 → 691.44] That includes the surrounding desks, the chair I'm sat on, my bike in the basement, for example, my car even is going.
[691.68 → 702.54] So on June the 7th in Raleigh at my house at 1pm, we are going to be having a blowout, mega bonanza, super-duper, what other superlatives can I think of?
[702.98 → 706.28] Garage slash yard slash estate sale.
[707.02 → 707.38] Ultimate.
[707.38 → 707.58] Ultimate.
[708.52 → 710.20] Now, there are lots of details.
[712.78 → 713.46] Shush you.
[714.14 → 714.58] Extravaganza.
[714.96 → 715.98] Trying to do a show over here.
[716.04 → 716.46] Stop it.
[717.48 → 717.92] Outrageous.
[718.32 → 719.90] Crazy Alex is going crazy.
[720.00 → 720.80] The sale's now.
[722.18 → 724.12] Yeah, if you don't have one of those crazy.
[724.12 → 725.90] Waking waving inflatable arm flailing tube.
[725.90 → 728.38] Yeah, inflatable guys, you're doing it wrong.
[729.14 → 730.86] What's the interdimensional cable?
[730.98 → 731.82] Ants in your eyes.
[732.02 → 732.78] Terry or something?
[735.78 → 736.34] Yes.
[737.38 → 741.10] That's what this episode has turned into, is interdimensional cable.
[741.10 → 750.24] Anyway, you can go to self-hosted. Show slash discord and there is a channel over there, hashtag Badgers Garage Sale.
[750.64 → 751.88] Bunch of info in there.
[751.98 → 753.54] People jostling over some items.
[753.54 → 758.06] I am operating a very strict first come, first served policy.
[758.06 → 760.52] So 1pm, we're not going to sell anything before 1pm.
[760.86 → 764.78] You can come a little bit earlier if you like and browse and have a look and sort of take your pick.
[765.24 → 769.62] But I think just to be fair to everybody, we're just going to, you know, first come, first served.
[769.62 → 774.84] Do you have like an auctioneer there to do your selling?
[775.06 → 775.82] I'd like to hear this.
[775.94 → 777.94] Can we get some live audio or something?
[778.28 → 778.78] It's funny.
[778.92 → 784.86] Certain items, I've had messages from people like the 3D printers have sold 15 times over, for example.
[785.04 → 789.56] But there is a bunch of other stuff that I do need to get rid of as well.
[789.56 → 796.44] So I'm pricing it very competitively, I think, like probably below market rates for a lot of this stuff.
[796.54 → 797.66] So like come grab a bargain.
[798.22 → 801.58] I'm at the just take it off my hands price phase.
[801.90 → 805.52] So, you know, grab a bargain, I guess.
[805.94 → 808.82] What's the thing that's going to hurt the most to let go of?
[809.54 → 810.06] It's funny.
[810.16 → 813.30] Brent asked me this last week, and it's definitely the drum set.
[813.74 → 814.60] Still the drum set?
[814.80 → 815.06] All right.
[815.86 → 819.24] Yeah, drum set, maybe the car, but I can always buy another car.
[819.56 → 821.30] You can always buy another drum set, to be honest.
[821.52 → 821.74] But yeah.
[822.08 → 824.22] Okay, what if we restrict it to tech items then?
[824.26 → 826.62] Because those two make sense and those are, you know, they touch the heart there.
[827.12 → 828.90] What about the more tool aspect things?
[829.66 → 832.50] I don't know as I'm that attached to anything particularly.
[832.84 → 840.00] It's so easy in our modern world to replace anything that, you know, we emigrated once and we came this way.
[840.22 → 843.98] And everything I've got in my house, I acquired in the last seven years.
[843.98 → 847.72] So like it's not that difficult to buy new stuff.
[847.72 → 851.82] And tech in particular is very ephemeral.
[852.80 → 856.42] And, you know, you do enjoy a good server setup, and you have your playbooks ready.
[856.78 → 856.80] So.
[857.26 → 863.28] Is this your whole cattle versus pets just put onto your life items?
[863.88 → 864.56] That's what it sounds like to me.
[864.56 → 865.00] I suppose it is.
[865.06 → 865.22] Yeah.
[865.28 → 866.80] It's like the acid test of my.
[867.44 → 871.24] So Steven, producer Steven is hosting a server for me up in Toronto.
[871.24 → 872.62] So I'm going to send one up his way.
[872.86 → 880.58] So I am keeping one server with like media files and my actual like source of truth of photos and that kind of stuff on that.
[880.66 → 881.24] That will stay.
[881.60 → 883.48] But everything else.
[883.58 → 886.02] I mean, there's a Mac studio in the list.
[886.56 → 891.88] All of my media, my old media server is going like, yeah, I'm not really that attached to any of it.
[891.94 → 894.40] Turns out like I thought it'd be really hard to write this list.
[894.40 → 897.66] But the further down I got, the more gun ho I got.
[897.74 → 899.02] And I'm just like, you know what?
[899.32 → 900.32] It's time to reset.
[900.84 → 901.74] Dibs on the chair.
[902.62 → 904.38] We'll just call you Alex Condo now.
[904.78 → 911.58] Next time you can build a drum set that has like 40 pieces and really lean into the Neil Pert of it all.
[912.50 → 913.76] Yeah, I guess so.
[914.08 → 918.04] We are going to spend a year in a bus driving around America before we go back to England.
[918.22 → 922.40] So we've kind of got like two or three different categories of stuff going on right now.
[922.40 → 923.96] We've got the garage sale pile.
[924.28 → 926.02] We've got the bus pile.
[926.30 → 929.40] And then we've got the put in storage until it goes back to England pile.
[929.72 → 934.14] And we're trying to make each of those keep piles as small as possible.
[936.18 → 938.42] Talescale.com slash self-hosted.
[938.52 → 946.00] Tale scale is the easiest way to connect your devices and services to each other wherever they are over a flat mesh network protected by Wirecard.
[946.16 → 950.24] And a huge thank you to Tale scale for their long support of the self-hosted podcast.
[950.24 → 956.30] It's really changed the way I do networking, the way I do Home lab, and now the way I do networking security for Jupyter Broadcasting.
[957.12 → 962.98] I get secure remote access to my systems, my production systems, all over my tail net.
[963.24 → 965.96] Every device is on my tail net as one flat land.
[966.02 → 972.14] It doesn't matter if they're across multiple providers, across multiple data centres, mobile networks, behind carrier grade NAT.
[972.32 → 973.22] It doesn't matter.
[973.22 → 978.62] And what's been really awesome to see over the last couple of years is all the integrations with Tale scale.
[978.72 → 981.90] Now, you can just run applications and put that application directly on your tail net.
[981.98 → 984.48] So, for example, VS Code, the web version.
[984.84 → 990.26] I just go to code.mydomain.com, and it pulls right up in my browser on my tail net.
[990.36 → 992.30] Just that one container is right there.
[992.74 → 993.82] It's so powerful.
[993.82 → 999.18] And when you go to Talescale.com slash self-hosted, and you try it out, you'll be blown away with how simple it is to set up.
[999.60 → 1001.48] It's the two really come together.
[1001.68 → 1007.28] And you can get it up for free on 100 devices and three users when you go to Talescale.com slash self-hosted.
[1007.56 → 1008.76] No credit card required.
[1009.14 → 1015.36] See why we rave about it, why so many in our audience use it, and thousands of companies like Instacart, Hugging Face, and Duolingo.
[1015.62 → 1017.14] They've all switched to Tale scale.
[1017.32 → 1020.50] So go try it out for yourself or for your business and see how great it is.
[1020.50 → 1026.54] I have no inbound ports on my firewall, and Tale scale is one of our longtime running sponsors.
[1026.98 → 1030.62] You can give them a good thank-you over at Talescale.com slash self-hosted.
[1030.76 → 1035.14] The easiest way to connect your devices and services to each other wherever they are.
[1035.32 → 1037.98] Talescale.com slash self-hosted.
[1039.90 → 1044.66] So if I know you, Chris, you took a trip to Boston for Red Hat Summit last week.
[1044.74 → 1047.38] That means you did a bunch of updates before you went.
[1047.38 → 1052.34] It means that you put a bunch of stuff onto hard drives and transferred a bunch of files around.
[1053.10 → 1054.08] Yep, you got me.
[1054.32 → 1055.50] I did all that.
[1055.86 → 1059.28] First, you don't want to go out of town without your systems up to date, right?
[1060.12 → 1061.22] And this one bit me.
[1061.58 → 1065.12] I am often, often I'm taking the systems with me.
[1065.12 → 1067.82] So this approach makes a little more sense.
[1067.90 → 1069.86] But this time I was updating the systems and leaving.
[1070.68 → 1073.48] And the one thing that broke is the integration with my Victory.
[1073.88 → 1075.90] It was actually not any of the updates I did.
[1075.94 → 1079.32] It's just the Victory needed to be rebooted after I upgraded the Home Assistant system.
[1080.00 → 1083.34] And so the whole time I was gone, I didn't have power monitoring, which really drove me crazy.
[1083.34 → 1085.10] So it did bite me in the butt a little bit.
[1085.10 → 1095.02] But I always view this as an opportunity, Alex, to review the latest in local file sharing applications.
[1095.02 → 1099.12] Because one of the things that we haven't really talked a lot about over the run of the show,
[1099.20 → 1107.46] but it is surprisingly a true statement, is this is a very popular category where there are constantly new applications being developed.
[1107.96 → 1114.46] This, I want to create an airdrop replacement all the way up to enterprise-grade file sharing applications.
[1114.46 → 1119.92] It's one of those things people have the problem, a little decision fatigue at this point, because there are so many options.
[1120.04 → 1123.88] And it's small enough that a dev can say, oh, I can probably write that in a weekend.
[1124.14 → 1129.36] And there are a lot of technologies built in the browser to enable file sharing, just like with WebRTC and whatnot.
[1129.48 → 1132.62] So a lot of the stuff is there plumbing-wise to build these.
[1132.62 → 1133.42] You got the bones.
[1133.60 → 1133.88] Yeah.
[1134.14 → 1135.86] I just need a little Python and the right vibe.
[1136.54 → 1139.10] What I hear you going to here is you vibe-coded your own, right?
[1139.16 → 1139.88] That's what you're about to do.
[1139.88 → 1140.48] No, no.
[1140.84 → 1142.06] No, I like to peruse.
[1142.06 → 1144.00] So he needs to learn how to vibe-code, Brent.
[1144.00 → 1145.80] Yeah, you got to study that.
[1145.88 → 1146.50] You got to read a book.
[1146.92 → 1147.84] You can't just vibe-code.
[1148.84 → 1150.24] Coming soon from Jupyter Press.
[1150.44 → 1150.66] Yeah.
[1151.14 → 1156.88] No, I like to peruse because this is a popular category that frequently has updates.
[1157.06 → 1164.16] And so this is a problem I try to solve because iOS is a bit of a pain in the neck when it comes to transferring remote network files.
[1164.24 → 1165.42] There are lots of ways to do it.
[1165.48 → 1166.28] None of them are great.
[1167.28 → 1172.38] And I was going to use an iPad because it's a six-hour flight, and I wanted to watch some TV and some movies.
[1172.38 → 1178.24] So I looked at two this time because they're relatively recent ones, and I thought, let's go in with some new stuff.
[1178.46 → 1185.44] The first one is Teardrop, which is the most AirDrop-like of the two I'm going to talk about here.
[1185.50 → 1186.46] It's GPL3.
[1186.46 → 1190.52] It lets you send images, documents, or text, and it does a peer-to-peer connection.
[1190.82 → 1194.76] So two different devices on the same LAN open up the web page.
[1195.00 → 1197.92] They see each other, and then you can transfer files.
[1198.46 → 1200.90] Works on any device with a modern web application.
[1202.12 → 1203.06] Simple, easy.
[1204.24 → 1204.98] How do you host it?
[1205.42 → 1206.54] It's just a Docker container.
[1206.96 → 1207.68] Yeah, both of these.
[1208.02 → 1209.58] I mean, there are lots of ways you can do it, right?
[1210.04 → 1210.80] It's just in Docker.
[1210.80 → 1216.20] This one is probably the most general user-friendly.
[1216.46 → 1219.90] Am I right here going to the site that you can also just use it from there hosted?
[1219.94 → 1220.46] Yes, you can.
[1220.68 → 1221.02] Yeah, you can.
[1221.04 → 1221.72] That's kind of neat, too.
[1221.92 → 1225.48] Yeah, you can just go to PearDrop.net on both of them and just use it in there.
[1225.58 → 1227.52] But you can also self-host it real easy.
[1228.04 → 1233.20] I assume it's a peer-to-peer connection it establishes, even if it's on their own infrastructure.
[1233.76 → 1233.92] Yeah.
[1233.92 → 1239.52] Now, that's all great and all, but I wanted something a little more robust.
[1240.08 → 1241.48] Yeah, that one sounds a little tedious.
[1241.62 → 1244.60] If you're doing it at scale, you've got 10, 12, 20 movies you're trying to get over.
[1244.64 → 1245.38] Yeah, or a season.
[1245.64 → 1245.98] Uh-huh.
[1246.50 → 1248.92] So let me guess, you installed Nextcloud and...
[1248.92 → 1249.92] Just kidding.
[1250.28 → 1252.02] That is a method I've tried once before.
[1252.68 → 1258.82] You know, it all started really with Pleasant, and since then I've had to come up with other solutions.
[1258.84 → 1259.60] Just come off the rails.
[1259.60 → 1259.80] Oh, God.
[1260.28 → 1261.32] What a weak Plex had.
[1261.48 → 1263.50] We should get to that later, but my goodness.
[1263.50 → 1264.20] Yeah, yeah, yeah.
[1264.32 → 1265.64] They've been some naughty boys again.
[1266.16 → 1274.48] So my ultimate travel solution, which works 100% of the time so far, does I install Infuse on an iPad.
[1274.72 → 1280.82] I don't have it sync with iCloud, so it's just a local Infuse app, and then I just have it look at the file system on the iPad.
[1281.74 → 1284.44] And before I leave, I have it download all the metadata.
[1284.94 → 1288.48] So it's a very Jellyfin Plex-like experience.
[1288.70 → 1293.28] You have the season descriptions, the episode, the thumbnails, the layout you expect.
[1293.50 → 1295.46] But it's all 100% offline.
[1296.22 → 1299.00] And the spousal approval, she doesn't even know.
[1299.42 → 1300.78] She doesn't even know, right?
[1301.24 → 1302.40] It's really fantastic.
[1302.48 → 1305.38] But you've got to get the files on the iPad.
[1305.94 → 1307.92] And so this is where Quick Share came in.
[1308.44 → 1311.80] It bills itself as quick and simple file sharing between different devices.
[1311.80 → 1313.54] It's a Go app that you run in Docker.
[1314.02 → 1315.56] It's LGPL 3.0.
[1316.48 → 1321.58] Now, what it did that I really liked is it supported resuming, uploading, and downloading files.
[1321.92 → 1329.68] So if your darn iOS device, your mobile device goes to sleep, you can pick back up where you left off so you're not having to redownload the entire season when you got 8 out of the 10 episodes.
[1330.00 → 1330.72] That's pretty fancy.
[1330.88 → 1331.08] Yeah.
[1331.08 → 1335.24] It also gives you a little bit more options in the UI.
[1335.60 → 1337.10] You can generate QR codes.
[1337.26 → 1344.36] And the thing I also liked is individual URLs for specific files you can generate and share, which is great.
[1344.48 → 1346.18] It has support for multiple users.
[1346.18 → 1347.30] And there's an admin role.
[1347.38 → 1349.04] And you can have per-user home directories.
[1349.54 → 1352.38] You can upload hundreds of files at once.
[1352.38 → 1359.48] So I could do two seasons of The Magicians, and it went fine, which was an okay watch.
[1360.04 → 1361.02] So this is Quick Share.
[1361.78 → 1367.00] And I think it's, you know, it could be the final solution as far as these go.
[1367.08 → 1370.28] You could settle with this one and never need to look for another quick file sharing.
[1370.54 → 1372.56] Does it have a spot in your tail net for now?
[1372.74 → 1373.06] Oh, yeah.
[1373.16 → 1374.14] Oh, this is a keeper.
[1374.64 → 1375.44] This is a keeper.
[1375.60 → 1379.04] I think what I like about it is it works for this, but it also works for other things.
[1379.04 → 1385.48] So an example would be we often have a lot of recordings, and they are just on the Android device,
[1385.54 → 1387.52] and the only way to really deal with it is the share sheet.
[1387.88 → 1391.32] Well, you could go here, and you can upload them to this, and I could pull them down on my computer real easily.
[1391.84 → 1398.78] Like there's what I have been using for things like Telegram file transfer where I'll just abuse Telegram's file storage ridiculously.
[1399.10 → 1404.22] And, you know, oh, we got an eight-minute wave file with an interview with somebody on the expo floor.
[1404.22 → 1408.44] I'll just upload that to my Telegram saved channel, and then I'll download it on my computer.
[1408.44 → 1411.84] I could cut all of that out, I think, with this, with Quick Share.
[1412.44 → 1413.76] So that's why I think it's a keeper.
[1414.20 → 1420.06] That's a forward-looking statement, Was, as far as my home lab usage may go.
[1420.24 → 1423.94] But as of right now, we believe it to be an accurate forecast.
[1425.26 → 1425.98] I'd invest.
[1426.74 → 1428.44] A corporate shill hat warning.
[1428.66 → 1430.14] Yes, I'm going to mention Tail Scale.
[1430.14 → 1438.96] There is a feature built into Tail Scale called Tail Drop, which lets you send files between any two devices on your Tail Net, pretty much.
[1439.34 → 1440.90] In much the same way, it's peer-to-peer.
[1441.26 → 1443.98] It's all done over the WireGuard encrypted tunnels behind the scenes.
[1445.10 → 1445.96] I'll be honest, though.
[1445.96 → 1450.14] I hadn't come across this Quick Share project before, and it really looks...
[1450.98 → 1453.74] It's worth your time, if you're listening to this, pulling this up.
[1453.74 → 1456.00] So it's on GitHub at idea.
[1456.10 → 1457.64] There'll be a link in the description, of course.
[1458.58 → 1459.58] idea Quick Share.
[1460.24 → 1461.18] And it looks great.
[1461.92 → 1463.16] All right, you teased it.
[1463.50 → 1465.64] I have not followed the Plex drama.
[1466.00 → 1467.22] I've sort of tuned out of Plex.
[1467.48 → 1472.70] As the show begins to sunset, I've thought, you know, I just don't have to care about Plex anymore.
[1472.96 → 1473.24] Yeah.
[1474.82 → 1475.78] So what's going on?
[1475.78 → 1479.80] I mean, Jellyfin does still lack proper user sharing.
[1479.94 → 1484.46] Like, it's not friendly to muggles, shall we say.
[1485.22 → 1492.82] But Plex does, unfortunately, remain probably the best option in that space when you want to share a server with family on the other side of the ocean,
[1493.12 → 1496.86] without them having to be logged into a Tail Net and explaining all of that dubbins to them.
[1496.86 → 1506.60] So I came across a friend of mine actually sent me this lovely little pop-up that came up on his server when he logged in yesterday, actually, as we record.
[1506.74 → 1521.58] It says, if you created your Plex account before March 20th, 2025, we now need your consent to include your data in limited selling arrangements, as outlined in our updated privacy policy.
[1523.56 → 1524.10] Sell.
[1524.52 → 1525.48] Sell your data.
[1525.80 → 1526.08] Selling.
[1526.86 → 1535.44] And this is directly at odds with their statement a few months ago saying, we do not, have not, will not share or sell your data.
[1535.60 → 1537.08] Like, which is it, guys?
[1537.52 → 1538.38] Which is it?
[1539.08 → 1543.46] You know, I got this exact message today when I was just trying to have breakfast with Seinfeld.
[1544.32 → 1547.48] And I was like of two minds of it.
[1547.54 → 1550.26] One, of course, exactly how we all feel about it.
[1550.54 → 1554.06] But the other side of it was that that message was extremely clear.
[1554.06 → 1556.36] And I was like, OK, they're selling data now.
[1556.36 → 1559.22] And I was able to say no thanks in the message.
[1559.66 → 1561.40] So part of me was angry.
[1561.48 → 1566.58] But the other part was like, at least they communicated it clearly this time somehow.
[1566.58 → 1569.18] And does that imply you've opted out?
[1569.18 → 1570.46] What does the no, thanks do?
[1570.46 → 1574.36] Well, that is actually quite a good question, Was.
[1574.36 → 1577.66] I just assumed it meant I opted out.
[1577.66 → 1578.66] But I actually have no idea.
[1578.66 → 1586.30] Well, the rest of the message stated, this won't affect your ability to use Plex, and you're always in control.
[1587.02 → 1591.32] You can review and update your privacy preferences at any time here.
[1591.42 → 1593.84] And then a link to your settings on the Plex portal.
[1593.84 → 1600.90] We followed the long, slow intuition of Plex on this show for forever, it feels like.
[1601.22 → 1603.30] And I'm kind of bored and tired of talking about it.
[1603.34 → 1607.54] Like the last few episodes have just been one thing after another, after another with Plex.
[1607.60 → 1617.70] And it's like, OK, I agree with what you're saying, Brent, that it's a very clear line in the sand to say we are now moving to a model where we're monetizing and selling this data.
[1617.70 → 1624.12] But they talk about the fact that it's hashed emails and advertising identifiers and stuff like that.
[1624.18 → 1625.76] If you actually click through and read the policy.
[1626.78 → 1631.70] At what point does that then become the contents of my library, which they say they don't store.
[1631.82 → 1636.02] But then just a couple of months ago, they said they would not sell my data anyway.
[1636.64 → 1639.54] Opt in or opt out, you know, regardless of what they said.
[1639.64 → 1642.56] Like it's you just cannot.
[1643.16 → 1644.26] We cannot trust them.
[1644.26 → 1651.78] And perhaps this will be filed under the same amount of obviousness as the fact that water is wet to some people that Plex are going to identify.
[1652.20 → 1661.42] But it may be, Alex, that you can't have a commercial company monetize the software that enables watching pirated content.
[1662.44 → 1667.74] You know, like maybe perhaps it requires it to be an open source project to actually push this forward.
[1668.12 → 1669.64] It always seemed a little bit tenuous.
[1669.86 → 1670.18] Right.
[1670.18 → 1677.08] It's a tricky line because like you say, they say they're not collecting content, titles or usage of your personal media server or files.
[1678.10 → 1679.54] But it is a slippery slope.
[1679.62 → 1682.70] It does seem to be like the aperture of what they do collect is widening.
[1682.84 → 1685.74] They are communicating it clearly, but the reality is still there.
[1686.58 → 1690.02] And I think they're in a position where they need to make more money.
[1690.02 → 1692.44] You know, there's more they want to do with the project.
[1692.64 → 1694.42] They want to bring in more streaming services.
[1694.68 → 1699.88] And they can't go and charge people more for Plex Pass or for the monthly subscription because people will flip out.
[1700.02 → 1702.54] And it's already they've probably tapped out what people are willing to pay.
[1703.48 → 1706.08] But they're a commercial entity that needs to grow and build.
[1706.08 → 1713.50] And they need to do it in a way where they're walking this fine line of not exposing what their users are actually doing.
[1713.50 → 1724.58] In a way, perhaps they can never cross that line because if they did start collecting the files and information of what people watch, it would expose the fact that probably a tiny percentage of people are taking advantage of the Plex streaming services.
[1725.06 → 1730.06] And the vast majority of people are watching their, quote unquote, backed up content via Plex.
[1730.72 → 1733.00] And it's got to be the vast majority of usage.
[1733.28 → 1737.62] And if they started to collect that information, it would expose that that's what the product is for.
[1737.80 → 1742.22] So perhaps it would be self-sabotage if they started to collect that.
[1742.22 → 1743.92] But it is still a worrying and concern.
[1744.58 → 1751.82] We could really use like a home assistant style model for Jellyfin or something like that to really start paying developers.
[1751.82 → 1757.86] Because really the issue with Jellyfin is the client availability and the client fit, finish and polish.
[1758.18 → 1761.86] There are lots of clients for Jellyfin for all sorts of operating systems.
[1762.32 → 1765.34] But they're in just such a random state of disarray.
[1765.34 → 1773.42] Like the iOS experience is so different from the Android TV experience, from the iOS, you know, like the phone or iPad experience.
[1773.42 → 1783.88] And at some point, some developers come along and scratch their itch and built an app and got it to a point that it's functional enough to use, but it hasn't kept up with it.
[1784.08 → 1786.50] You know, and they're open source developers.
[1786.60 → 1789.20] They're under no obligation to continue to work on it for free.
[1789.28 → 1790.42] I'm not saying they should.
[1790.42 → 1799.16] But I think we've got to seriously take a look as a community at the funding model to incentivize the clients that we need and want to see.
[1799.64 → 1805.56] Infuse is kind of the best solution right now for Jellyfin clients on certainly on Apple TV.
[1805.56 → 1814.42] And that's because you have to pay, what is it, 60 bucks a year for the pro package that they have, the subscription they have, to fund development.
[1815.04 → 1817.44] So something has to change in this sphere.
[1817.78 → 1823.22] And the writing has been on the wall for Plex for a very long time, and it will continue to incentivize and get worse.
[1823.38 → 1824.94] We've seen that many times over.
[1825.76 → 1832.96] But I just wonder where Jellyfin and perhaps MB are going to end up in this whole cycle too.
[1832.96 → 1844.40] Yeah, I had the same thought, just if you want to compete on the sharing front, a lot of what Plex can do is have that smart proxy availability so they can stream stuff from your server without having to know anything about it.
[1844.46 → 1851.74] And we probably need some kind of entity, for profit or not, that could maybe do that for users who aren't able to do it themselves.
[1852.56 → 1858.80] It would even be enough for Jellyfin to have some kind of like a lighthouse server that I could host in a VPS somewhere.
[1859.14 → 1862.00] And then that becomes a discovery endpoint for clients.
[1862.00 → 1863.48] I give them that endpoint.
[1864.18 → 1865.78] Because there are a couple of things at play.
[1866.24 → 1871.10] You have to open ports in your firewall if you want people to access your Jellyfin server running locally.
[1871.54 → 1880.66] Well, you could solve that by running a lighthouse-type server up on a VPS and have that tunnel back in over tail scale or whatever you want, like any kind of VPN tunnelling service.
[1881.42 → 1885.52] But then you've got the sharing portion as well, like which libraries is this person allowed to see?
[1885.68 → 1888.78] What sort of content filters do you want to apply to that person?
[1888.90 → 1889.94] That sounds like a database.
[1889.94 → 1894.76] A lot of that stuff already exists in Jellyfin with like local users.
[1894.96 → 1905.18] But if that lighthouse server had somehow had the concept of mappings between the servers it could see and the users you're sharing it with and their ages and all that stuff, like that could be pretty powerful.
[1906.32 → 1907.64] Jeez, Alex, that sounds like a good project.
[1908.20 → 1908.78] Yeah, I want that.
[1908.90 → 1909.54] I want that now.
[1909.98 → 1911.40] Yeah, I'm going to vibe code that this weekend.
[1911.80 → 1912.24] Good man.
[1912.24 → 1916.48] Unraid.net slash self-hosted.
[1916.52 → 1919.66] Go there to support the show and check out Unpaid 7.1.
[1919.76 → 1921.48] In fact, 7.1.2 is here.
[1922.02 → 1926.84] The 7.1 series is a massive improvement in their ZFS support.
[1926.92 → 1933.94] And now you can just move from platforms like True NAS or QNAP or Proxmox ZFS system or an Ubuntu ZFS system.
[1933.94 → 1939.10] So if you're ready to upgrade to a more powerful system, Unpaid makes that a lot more approachable.
[1939.10 → 1943.82] There's been a lot of refinements in the 7.1 series in the web interface.
[1943.98 → 1944.92] It's more responsive.
[1945.18 → 1945.84] It's more stable.
[1946.08 → 1947.88] And there are integrations now with Tail scale.
[1948.00 → 1952.16] I don't mention this enough, but when you're installing applications now, there's native Tail scale integration.
[1952.66 → 1953.86] You just check a box.
[1953.86 → 1961.14] And one of the things that I think doesn't get enough love is that app store, if you will, of community-contributed applications.
[1961.36 → 1966.34] And there's like everything from just all the media centre applications you could ever want.
[1966.34 → 1976.60] But what I wanted to highlight, which is really nice, the AI stuff, any of the AI stuff you'd want for your different types of GPUs or even just CPU,
[1977.10 → 1983.32] just a couple of clicks away to start playing with this stuff, including stuff that will emulate the OpenAI API
[1983.32 → 1986.72] so you can get even more functionality out of local chat stuff.
[1986.80 → 1988.18] It's really great.
[1988.34 → 1992.10] And Unpaid, the whole thing is just very powerful.
[1992.10 → 1996.68] It makes it simple for you to get started and build a home lab that gets applications up and running
[1996.68 → 2003.54] and takes advantage of the hardware you have right now, the hardware you have on hand, because Unpaid is hardware-agnostic.
[2003.68 → 2005.04] You can mix and match drives.
[2005.42 → 2009.06] And it's also great for back-end infrastructure for like a small business office.
[2009.32 → 2010.32] You want something reliable.
[2010.44 → 2014.14] It's built on top of modern Linux and has a great team behind it.
[2014.44 → 2019.14] And Unpaid 7.1 and 7.1.2, which just came out recently, are just great.
[2019.14 → 2023.40] They're stacking feature after feature and polish and refinement after polish and refinement.
[2023.84 → 2026.66] So go thank them for supporting the show and check them out.
[2026.98 → 2029.12] Go to unraid.net slash self-hosted.
[2029.18 → 2032.44] Go on over there, see what Unpaid's all about, see why we rave about it.
[2032.64 → 2037.18] And it's a great way to give a little shout to the self-hosted show and for the sponsors who've supported us.
[2037.52 → 2039.74] Unraid.net slash self-hosted.
[2039.74 → 2046.14] So over the last few years, we have tried out so much self-hosted software.
[2046.64 → 2049.86] Like I can't even remember most of it, if I'm being honest with you.
[2050.34 → 2054.14] And I thought this would be a good opportunity, given we have friends with us today as well, Chris,
[2054.14 → 2063.16] to ask you and Was and Brent and Drew what your personal top self-hosted app pick from the last few years might be.
[2064.34 → 2065.88] Oh, Drew, you got one that comes to mind?
[2065.88 → 2070.64] I think the media server stuff is an easy one to go to.
[2071.40 → 2077.58] But for me, it's not even a project that I can use anymore now that I'm living in rental apartments.
[2078.04 → 2079.68] It's got to be Home Assistant, right?
[2080.40 → 2085.14] Yeah, I think that one gets like, you know, a nod from all of us at this point.
[2085.34 → 2086.36] Like that's just been a killer.
[2086.72 → 2088.74] There are two universal truths on this show.
[2089.12 → 2090.46] First one is Fight Club.
[2090.60 → 2092.62] We don't talk about the R stack.
[2092.76 → 2093.68] That just doesn't exist.
[2093.68 → 2095.92] We just pretend that doesn't exist because we all know about it.
[2095.96 → 2096.44] We all use it.
[2096.48 → 2097.02] We all love it.
[2097.22 → 2097.66] Never heard of it.
[2097.84 → 2102.88] The second is that Home Assistant, it's MVP in the self-hosted world.
[2103.12 → 2105.68] So now we can accept those as two universal truths.
[2106.02 → 2106.16] Yeah.
[2106.24 → 2107.48] We've got our axioms laid out.
[2107.54 → 2107.70] Good.
[2108.20 → 2109.10] What else is there?
[2110.68 → 2114.52] I feel like of the five of us, Was and I are really just coming into this truth.
[2115.28 → 2115.48] So.
[2115.76 → 2116.60] The Home Assistant one.
[2116.68 → 2117.12] Oh, yeah.
[2117.12 → 2117.16] Yeah.
[2117.70 → 2122.38] Like forever I've known it's such a great thing and watched it evolve.
[2122.54 → 2127.96] And it's maturity now compared to when the show started has come a heck of a long way,
[2128.02 → 2128.58] if you think about it.
[2128.66 → 2129.04] No kidding.
[2129.62 → 2129.90] Yeah.
[2130.10 → 2131.70] I mean, they've built a company around it.
[2131.84 → 2137.00] They have built all sorts of amazing partnerships now, too, with hardware providers and all sorts.
[2137.08 → 2138.40] It's incredible.
[2138.40 → 2139.04] Yeah.
[2139.06 → 2145.86] We did do a great interview with Paulus on Linux Unplugged recently that I think is worth checking out and just hit that point across for me.
[2145.94 → 2147.44] It was like, oh, yeah, this has come a long way.
[2148.18 → 2154.66] But, Was, you and I, I think, are just little babies compared to these three in terms of our Home Assistant setups.
[2155.16 → 2155.78] Yeah, it's true.
[2155.78 → 2165.92] I mean, I've been going the minimal lifestyle because I've just moved so many darn times in recent years between myself being a little more stable in address land and the rock solid stability.
[2166.14 → 2172.44] And then in the world of and citified other services, just like now seems like a great time to do it.
[2172.58 → 2177.02] And I have a lot of trust in the ecosystem that whatever I build is going to be here for the long haul.
[2177.02 → 2187.10] Now, you have, I think for you, if you're going to if you're going to call it MVP self-hosted app, I would think maybe Jellyfin because you've been spinning up Jellyfin instances for years, kind of like on demand.
[2187.10 → 2189.10] That is absolutely true.
[2189.16 → 2190.08] It has sort of been a backbone.
[2190.22 → 2191.86] It's provided stuff for my folks to watch.
[2191.96 → 2196.12] Anytime I need just like a quick share or, you know, there's a TV available on the network.
[2196.20 → 2200.84] There's probably some way for me to, like, get an MP4 file loaded and go in on that TV via Jellyfin.
[2200.84 → 2205.76] One time we were at an Airbnb and our plans didn't quite work out for remote streaming.
[2205.76 → 2212.04] So a few minutes later, We shad a Jellyfin instance going on his laptop, and then we were getting files on there from the system we intended to use.
[2212.22 → 2213.26] Ready to go with MacGyver.
[2213.38 → 2215.50] Yep, we had MacGyver just a couple of minutes later.
[2215.82 → 2218.30] I will have an honorary mission for Technetium DNS.
[2218.60 → 2220.22] I've been using that and really enjoying it.
[2220.64 → 2222.12] And I'm excited to see where it goes.
[2222.62 → 2223.12] Oh, Geez.
[2223.16 → 2226.18] I'd forgotten about, like, network infrastructure layer stuff.
[2226.78 → 2229.56] Like, do we count projects like Open Sense as self-hosted software?
[2230.00 → 2230.54] Oh, yeah.
[2231.26 → 2231.66] Definitely.
[2231.76 → 2232.20] A hundred percent.
[2232.20 → 2240.48] I mean, that's been powering my entire internet stack for years now, along with a mixture of Pinhole and Technetium at some point.
[2241.00 → 2242.64] And currently I'm running AdGuard Home.
[2242.76 → 2244.76] There's some amazing stuff in that space.
[2245.42 → 2248.66] Well, and if we're going that direction, you know, you've got to include containers.
[2249.54 → 2251.82] Docker, Rodman, pick your poison.
[2251.82 → 2262.22] The advent of containers and the ability to do that easily at home has been huge for being able to share projects around.
[2262.38 → 2268.88] Now, I know a lot of you guys are going the Nix route these days and doing things that way instead of containers.
[2269.34 → 2272.00] But containers are still awesome.
[2273.06 → 2273.12] Yeah.
[2273.24 → 2275.50] And Rodman and Nix pair great together, you know.
[2275.80 → 2276.42] They do.
[2276.42 → 2278.22] And have you seen the Quad lets project?
[2278.76 → 2279.16] Oh, yeah.
[2279.44 → 2280.02] Mm-hmm.
[2280.26 → 2281.16] Quad lets are neat, too.
[2282.02 → 2283.30] I see, Chris, you're laughing.
[2283.40 → 2284.58] Why are you laughing about Quad lets?
[2284.92 → 2286.22] It's just such a great name.
[2286.86 → 2288.10] And I love the way you say it.
[2288.30 → 2289.50] Quad lets is just great.
[2289.50 → 2290.12] It sounds cute.
[2290.12 → 2290.76] It's how I say it.
[2290.86 → 2291.80] It's just how I talk.
[2293.22 → 2295.00] I got me and my quad, you know?
[2295.02 → 2295.20] Yeah.
[2295.86 → 2298.52] I'll come at you with one that's not too surprising.
[2299.32 → 2300.62] But you got to give it to Image.
[2301.08 → 2302.86] You know, finally freeing us from Google Photos.
[2303.10 → 2304.10] Been really, really solid.
[2304.68 → 2304.84] Yeah.
[2304.84 → 2306.74] And a nice little ecosystem coming up around there.
[2307.54 → 2308.92] And then how do we say it?
[2309.88 → 2310.28] Bewitch?
[2311.56 → 2311.92] Dearth.
[2312.30 → 2312.70] Dearth.
[2312.70 → 2320.48] Dearth, which we talked about recently on Linux Unplugged, which is a visualizer that you can use for tracking yourself, sort of like Google location history.
[2320.48 → 2325.92] And there are a lot of ways to hook into it, including a client for iOS or own tracks on Android.
[2326.58 → 2331.56] Or, which I really love, you can just add it as an integration to Home Assistant.
[2331.56 → 2338.78] And then it just uses your location information from Home Assistant to build a visualization on a map that shows you everywhere you go.
[2339.58 → 2341.32] And the hotspots of where you visit frequently.
[2341.54 → 2344.08] And when you're travelling, this is such a blast.
[2344.14 → 2346.58] Because you can, at the end of the day, you sit down at the table.
[2346.74 → 2347.58] Come on over, boys.
[2347.62 → 2348.32] You pull up the laptop.
[2348.66 → 2350.10] And you look at everywhere you went.
[2350.48 → 2352.42] And you're like, okay, well, we missed this spot.
[2352.44 → 2353.60] So we got to go here tomorrow.
[2354.44 → 2359.28] And it actually became like, well, I want to fill this spot in on the map.
[2359.28 → 2362.06] So we'd take a little extra route, you know, to go over there to get that.
[2362.34 → 2363.42] And then I look back at it.
[2363.42 → 2364.22] I still look back at it.
[2364.30 → 2365.86] And I'm like, oh, look at all the routes we took.
[2365.98 → 2367.38] I was just showing it to the wife last night.
[2368.00 → 2369.28] I brought it up on the screen.
[2369.68 → 2373.88] Look at everywhere we went while we were in, you know, Boston and then outside of Boston as well.
[2374.44 → 2376.52] And so it's, how do you say it again?
[2376.96 → 2377.36] Dearth.
[2377.58 → 2378.02] I don't know.
[2378.08 → 2378.44] I'm guessing.
[2378.44 → 2381.36] But pretty simple app overall, but really great.
[2381.44 → 2382.50] Still kind of an early development.
[2383.18 → 2391.90] And it can import your image photo location data and populate your back location information from the IF location information from your photos.
[2392.14 → 2394.22] And it shows a cute little preview of the photo there, too.
[2394.40 → 2394.60] Yeah.
[2394.60 → 2397.02] So those two are great.
[2397.38 → 2407.84] The thing I like, Chris, about this recent trip that the three of us took was that, like, in the first day or two, you were just itching to track where we were going.
[2408.02 → 2414.58] And we had just kind of dumped the server that we had tried for Linux Unplugged recently because it was just a test server.
[2414.58 → 2420.62] And then, but you were, like, visibly uncomfortable about not tracking where all these cool places we were going.
[2420.78 → 2428.70] So I found it really kind of amazing that then that night when we got home, we were just like, well, let's put the server up.
[2428.74 → 2429.84] And then we have that functionality.
[2429.84 → 2439.64] And I think that's really the joy of self-hosting is you unlock all these possibilities that otherwise, I don't know, you'd have to rely on some megacorp for something.
[2439.84 → 2447.28] And so it just really hit me on that trip that, like, we have these skills that allow us to just do so many fun things in a snap.
[2447.52 → 2448.52] And that's self-hosting.
[2448.52 → 2450.36] Now we got a map of our adventures.
[2450.56 → 2450.68] Right.
[2450.78 → 2452.64] And it's no creepy corporation tracking.
[2452.86 → 2456.26] It was probably a 10-minute setup to get it up and running.
[2456.54 → 2461.82] And we're doing it from an Airbnb remote, SSH'd into my system, setting it all up.
[2461.90 → 2466.68] And then I'm setting, you know, all my location data is just using the Home Assistant companion app on my phone.
[2467.04 → 2471.60] And Home Assistant is then reporting it to the local instance right there on my LAN.
[2472.30 → 2474.10] It was really pretty great.
[2474.10 → 2476.12] And then I have this history of everywhere I've been.
[2476.12 → 2480.82] And the reason why I like it so much is it fades for me, where we've been and what we did.
[2481.02 → 2488.26] And then when we go back to areas, I truly can't really recall where we've been or where we haven't been unless it's something that's really standing out, you know, something really novel.
[2488.36 → 2491.12] It's so nice to just have that record to jog your memory a little bit.
[2491.30 → 2493.84] So next time we go back to Boston, you know, I know where else to explore.
[2494.14 → 2501.32] We also found an open source app for Android that'll just sort of save your data and then be able to export a GPX file.
[2501.46 → 2504.86] Or it can make arbitrary HTTP calls to push that data to a server.
[2504.86 → 2506.76] So you got a lot of options.
[2506.92 → 2507.86] Yeah, that just runs locally.
[2508.08 → 2509.42] It's just writing to a file.
[2509.64 → 2511.26] It's not talking to any cloud instance.
[2511.46 → 2512.84] And it has various auto-sync options.
[2512.98 → 2514.32] And it has a persistent notification.
[2514.66 → 2518.76] And the thing that's nice about that is you can annotate your location so you can add a little note right there.
[2518.80 → 2520.38] And it just saves it out to the GPX file.
[2520.90 → 2521.62] And you import that.
[2521.62 → 2527.58] You know, one project I didn't say because I thought I might be stealing it from you was Pinch flat.
[2528.12 → 2537.00] Which has, I mean, I watch a fair amount of YouTube and that was sort of a tool I had wanted to build for a long time.
[2537.10 → 2538.64] And so I was really glad to see someone built that.
[2538.72 → 2542.40] Especially because when you pair it with Jellyfin, it's just sort of the whole experience is replaced.
[2542.40 → 2546.84] Yes, you get that metadata provider tuned in and it's amazing.
[2547.38 → 2550.78] It's like the regular TV shows on your Jellyfin instance.
[2551.58 → 2553.30] Yeah, and then the auto-cleanup is nice too.
[2554.06 → 2558.62] You know, what's funny is I've been doing a bunch of servers rejigging ready for the move and stuff like consolidating.
[2559.14 → 2563.78] And so my Pinch flat was offline for maybe two or three weeks whilst I migrated some data around.
[2563.78 → 2570.32] I brought the container back up again, and it just pulled down every episode just the minute it started up like nothing had happened.
[2570.58 → 2573.54] It was as it should be.
[2574.32 → 2579.06] I really have, you know, 30 of these apps that are just quintessential to my day-to-day life.
[2579.24 → 2585.28] But I just want to give one more call out to one that you all know I love and that's Lube Lager.
[2585.54 → 2587.50] I was about to ask you about Lube Lager.
[2587.64 → 2588.54] Do you still use that?
[2588.70 → 2589.36] Oh yeah, buddy.
[2589.42 → 2590.32] Oh yeah, I love it.
[2590.66 → 2592.96] And didn't you get one going for brand or almost?
[2592.96 → 2596.38] I was telling Brent that we should get one running inside the van.
[2596.52 → 2598.92] The van should have its own, like Lady Coupes does.
[2599.00 → 2599.40] Of course.
[2599.54 → 2601.72] Lube Lager is hosted inside the rig.
[2602.44 → 2603.56] And I think Brent should do the same.
[2603.92 → 2606.08] And the border guards ask you all these questions and be like,
[2606.38 → 2609.42] yeah, but look, I've changed my oil three times in the last 12,000 miles.
[2609.62 → 2610.52] Look at my maintenance records.
[2611.06 → 2612.02] Do I have to pay tax on that?
[2613.58 → 2616.00] I didn't throw out one, but I'm going to...
[2616.00 → 2618.94] I have a mixed relationship with this one, but I use it every single day,
[2619.00 → 2620.60] which is more than most of the others.
[2621.38 → 2622.18] Audio Bookshelf.
[2622.18 → 2625.68] I end up using that every single day.
[2626.00 → 2626.36] Yep, same.
[2626.70 → 2627.54] A mixed relationship.
[2627.72 → 2628.20] What does that mean?
[2628.26 → 2630.18] That sounds like a Facebook relationship status.
[2630.34 → 2631.24] It's complicated.
[2631.50 → 2631.76] Yeah.
[2631.88 → 2632.74] What's going on, big guy?
[2632.76 → 2633.98] It's rather complicated, I'll say.
[2634.34 → 2636.18] I love the functionality it provides.
[2636.18 → 2640.48] I think, as you all know, the bug field is strong with this one.
[2640.48 → 2648.64] And I run into all sorts of strange behaviours and weird issues that I've found ways around or whatever.
[2648.86 → 2652.78] But it's an application that regularly frustrates me.
[2652.78 → 2654.46] But I also need it consistently.
[2654.66 → 2656.32] So, it's complicated.
[2656.90 → 2657.04] Yeah.
[2657.54 → 2658.14] Yeah, it's funny.
[2658.22 → 2665.48] One of the reasons I still run Plex locally is to provide my wife audiobooks via Prologue.
[2665.76 → 2666.88] She's an iOS user.
[2667.00 → 2669.38] And the Prologue experience is fantastic, honestly.
[2670.18 → 2672.26] But my sister was in town last week.
[2672.32 → 2674.60] And she wanted access to audiobooks.
[2674.64 → 2679.74] And of course, there isn't really a good Plex audiobook client for Android.
[2680.38 → 2681.40] And so I ended up spinning.
[2681.52 → 2682.90] This is a bit of a cursed setup.
[2683.00 → 2685.08] But I ended up putting reverse proxy on a VPS.
[2685.08 → 2687.38] So she didn't have to connect to Tail Scape every time.
[2688.12 → 2692.72] And then used Pangolin to reverse proxy tunnel this thing back into my LAN.
[2692.88 → 2695.74] Actually, to Stephen's LAN in Toronto, not mine.
[2695.84 → 2697.66] Because this isn't going to exist in a month or two.
[2698.26 → 2702.58] And then replicated with ZFS the data sets to Canada with the audio.
[2702.66 → 2703.58] It was a whole thing.
[2704.12 → 2707.94] But all of that to say is that audio bookshelf can be a little bit finicky.
[2708.08 → 2710.80] She went to download a book onto her phone.
[2711.12 → 2713.02] And the downloads proceeded just fine.
[2713.02 → 2715.52] And then it just said failed.
[2715.68 → 2716.46] No error message.
[2716.60 → 2717.66] Just literally just said failed.
[2717.82 → 2721.40] So she had to remove the local folder in the Android app.
[2721.82 → 2722.48] Re-add it.
[2723.24 → 2723.92] Reboot the phone.
[2724.04 → 2724.62] And then it was fine.
[2725.30 → 2728.80] I've had a couple of weird occurrences like that too with the downloaded audiobooks.
[2729.64 → 2732.26] The ones I stream seem to always work ironically.
[2732.48 → 2734.36] And when I'm at home, I just stream them because it's on my LAN.
[2734.68 → 2736.28] But when I travel, I tend to download them.
[2736.64 → 2740.00] And one time I got an error message that told me I needed to delete the downloaded version.
[2740.60 → 2742.88] So I guess they're getting better at telling me what to do.
[2742.88 → 2745.62] But I'm like, but that's, but I wanted it.
[2745.90 → 2747.24] Oh, all right.
[2747.86 → 2751.88] Can I talk about a project that I know is probably a little contentious around here?
[2751.98 → 2754.06] But it's one that I've relied on for many years.
[2754.06 → 2757.26] But recently, I've kind of just stopped using it altogether.
[2757.96 → 2759.36] And that is Nextcloud.
[2759.36 → 2766.96] I've kind of stopped using it because it's gotten a bit big, a bit bulky, a bit slow, a bit confusing to set up.
[2767.46 → 2769.08] Anybody else found that?
[2769.46 → 2771.38] I use it passively still a lot.
[2771.54 → 2775.24] I'm using it to sync every day, but I don't use it.
[2775.34 → 2775.82] You know what I mean?
[2776.06 → 2778.16] I upgraded it the other week.
[2778.52 → 2781.04] And then I forgot to even go back and check if it was okay.
[2781.68 → 2782.22] But it was?
[2782.28 → 2782.68] It was.
[2782.70 → 2783.16] It was fine.
[2783.20 → 2783.62] It worked great.
[2783.68 → 2784.52] The upgrade went flawlessly.
[2784.88 → 2787.32] But I realized I've stopped going to the website.
[2787.46 → 2793.24] And I also don't have the sync client on my machines anymore because I don't really want to sync those files to that server.
[2793.24 → 2799.74] But I do have my Android device, of course, syncing my Calder and my Carded and all that stuff still.
[2800.16 → 2802.42] And so it's working in the background still for me.
[2802.76 → 2805.62] Yeah, that's kind of those are the key services I'm still using.
[2805.70 → 2807.32] But I haven't done much else with mine for a while.
[2808.08 → 2813.42] I mean, Nextcloud was instrumental in my photo backup solution for many, many years.
[2813.42 → 2823.88] But Image has completely taken that crown away from it in conjunction with Paperless and also Paperless NGX and Paperless AI as well.
[2823.94 → 2829.88] So I can do tagging and inference on documents I have and sort of look for stuff based on keywords.
[2830.28 → 2837.86] And between those two apps, honestly, there isn't much else left for Nextcloud to do other than just be kind of like a file portal.
[2838.60 → 2839.12] Yeah.
[2839.12 → 2849.16] Yeah, I have been looking on and off at pure Calder and Card Dev, just basic servers that don't have a UI.
[2849.42 → 2854.34] They don't have a web page, but they are open on those ports, and they'll sync that stuff, and they have a little local database.
[2854.92 → 2862.96] And they're very minimal instances that you can run and essentially replicate just that functionality on your server, probably with a lot less overhead.
[2863.22 → 2865.50] But, you know, for me right now, it ain't broke.
[2866.08 → 2867.74] And it is nice to have that functionality.
[2867.74 → 2871.40] One area I do still use it is on my wife and my kids' computers.
[2871.54 → 2875.82] They have the Nextcloud client and their documents directory just backups automatically to that.
[2876.34 → 2878.06] A little more like the Windows-style setup.
[2878.28 → 2878.50] Yeah.
[2878.80 → 2880.52] So that I do use it for still, I suppose.
[2880.90 → 2881.52] And that just works.
[2882.32 → 2885.62] Of course, we still use it in the production pipeline for every single show.
[2885.72 → 2891.94] Like when I'm done recording this episode, I will drop my FLAC file onto what we lovingly call the horse.
[2891.94 → 2895.94] And then Drew will pick it up and edit the files from there.
[2896.04 → 2898.76] I mean, it's been in the JB production pipeline for years now.
[2899.42 → 2899.52] Yeah.
[2900.12 → 2900.46] Yeah.
[2900.50 → 2905.54] And we even use it sort of in a, you know, a bizarre way with S3 object storage as our backend storage for it.
[2906.18 → 2908.38] Which lets us abuse it probably far more than we should.
[2908.38 → 2910.66] And it still works really well.
[2910.96 → 2916.88] I mean, when you guys are done with the show, I've got the files ready to go in minutes.
[2917.24 → 2920.36] And I'm only using the web interface.
[2920.68 → 2923.04] I don't have the sync client on my computer at all.
[2923.70 → 2929.72] I just go download them from the web because it's one less agent that I need in my toolbar.
[2930.42 → 2930.80] Same.
[2931.16 → 2937.36] There was a rewrite or a fork or a clone of it released recently, rewritten in a different language.
[2937.36 → 2937.64] Oh, yeah.
[2937.64 → 2937.88] I forget.
[2938.00 → 2938.24] Jeez.
[2938.52 → 2938.88] Oh, boy.
[2939.52 → 2940.38] That's got to be a project.
[2940.62 → 2941.82] I forget the name, unfortunately.
[2941.82 → 2947.94] I know in the studio we found it quite effective to pair it with our clone, just to push things over web dev in the background, too,
[2948.00 → 2951.90] if you maybe don't need the full functionality of the sync client or want something a little more flexible.
[2952.36 → 2954.92] Yeah, that has worked basically flawlessly for us.
[2955.04 → 2957.70] The only real downside is in the way we have it configured now.
[2957.70 → 2960.36] I think we do have some options, but we don't have meaningful progress.
[2960.70 → 2960.96] Right.
[2961.06 → 2963.72] But, you know, we watch the network stack, and that's good enough.
[2964.84 → 2971.48] I have two more very small picks, I think, before we close out this segment, one of which is Smoke Ping.
[2971.48 → 2979.76] And actually, it's beautiful that this is in this episode because, Chris, you put me onto Smoke Ping in Linux Action Show like 37 years ago.
[2980.00 → 2980.66] I had a boy.
[2981.26 → 2985.42] It was one of the very first containers I wrote for LinuxServer.io back in the day.
[2985.54 → 2987.58] And I still run it and look at it all the time.
[2987.58 → 2992.38] I mean, it's so useful sort of triaging network latency between.
[2992.60 → 3001.02] So I've got a bunch of Smoke Ping sites configured in my LAN, and then a bunch configured on this side of the ocean, a bunch configured on the other side, some via tail scale, some via not.
[3001.02 → 3001.24] Yeah.
[3002.00 → 3002.62] That's great.
[3002.78 → 3003.54] It really just works.
[3003.70 → 3004.38] Runs in the background.
[3004.90 → 3007.54] Doesn't change a bunch, you know, in a good way.
[3007.54 → 3008.68] I still run it myself.
[3008.76 → 3009.76] I've been running it for years.
[3010.12 → 3015.26] And I find it extremely useful when popping between different types of Internet connections.
[3015.26 → 3021.10] And I get a real sense also of, like, how my long-term Starlink performance has been.
[3021.10 → 3031.96] And, you know, ironically, probably still one of the most often, like, dashboard-type apps that I use, right?
[3031.96 → 3033.14] I don't have a lot of these.
[3033.18 → 3034.44] Like, I don't run a lot of net data.
[3034.56 → 3037.56] I don't run a lot of these Grafana-type dashboards.
[3037.56 → 3038.88] But this is the one.
[3038.98 → 3043.88] The network latency is the one I care about probably the most after all the years.
[3044.40 → 3045.16] It's just how that's doing.
[3045.24 → 3054.00] And to have this historical data where I can be like, are these evenings getting worse on Starlink and I can go back two years is great.
[3054.26 → 3054.40] Yeah.
[3054.50 → 3054.86] It's just great.
[3055.08 → 3057.54] It's not a glamorous application by any means.
[3057.68 → 3060.26] It's based around RRD Graph, I believe.
[3060.78 → 3065.44] But it does just do its thing quietly in the background, sipping resources.
[3065.44 → 3071.68] The other app that I really use the snot out of this one is Airspeed to test.
[3071.88 → 3079.56] Instead of using, like, IPER and stuff like that, like, I'll just bring up a browser on my phone, go to my local IP address and port number, and boom, I've got a speed test.
[3080.32 → 3081.90] Ah, Airspeed's a good one.
[3082.58 → 3083.56] Random shout-out.
[3084.58 → 3093.00] Something I put in, and I bet you if you go back in the back catalogue, you'll find me talking about Power line networking and how I was rolling the dice on Power line networking.
[3093.14 → 3093.60] Oh, yeah.
[3094.08 → 3094.94] I've tried it before.
[3094.94 → 3098.26] I've tried it in this studio, and it was garbage.
[3098.46 → 3102.56] This is well before we ever wired an Ethernet many years ago, but back in the day.
[3102.78 → 3104.32] And this is, I mean, this was so long ago.
[3104.40 → 3106.40] It was, like, when Wi-Fi was essentially, it didn't exist.
[3106.64 → 3109.54] And I was trying to stream movies to my hacked Xbox.
[3110.22 → 3111.34] So, the first Xbox.
[3111.44 → 3112.02] As one does.
[3112.56 → 3114.10] And Power line networking was the solution.
[3114.10 → 3118.32] And I could barely get two megabits out of it.
[3118.32 → 3123.72] And so, you know, as soon as Wi-Fi came out, I got a USB dongle for the Xbox and got that thing on Wi-Fi.
[3123.92 → 3127.90] And, you know, maybe, maybe got a solid two megabits, but at least it was solid.
[3128.54 → 3131.54] And then as the years went on, I just never revisited Power line networking.
[3131.54 → 3141.96] But then when I moved into the RV and I wanted to connect my telco closet, as I call it, to my server booth closet, I needed to come up with a hardwired solution.
[3142.30 → 3148.56] And so I took a chance with the TP-Link Power line networking stuff and put it in.
[3149.38 → 3150.80] And, again, this was four or five years ago.
[3150.86 → 3151.96] It's the early days of the show.
[3152.48 → 3154.06] And the same gear is still in.
[3154.08 → 3155.42] I've never had to reboot it.
[3156.24 → 3157.50] I've never had to touch it.
[3157.90 → 3161.20] I get, you know, almost, almost 100 megabits.
[3161.36 → 3162.32] So, I'm a happy boy.
[3162.36 → 3162.74] Nice.
[3162.74 → 3165.40] Really, I only use that connection for transferring internet data.
[3165.84 → 3169.32] So, 100 megabits are actually generally enough.
[3169.66 → 3170.32] Sometimes not quite.
[3170.42 → 3171.06] But it's pretty great.
[3171.34 → 3173.02] The Power line networking has held up.
[3173.30 → 3177.62] It's not the fastest, but it's been so solid that you would forget that it's even there.
[3177.62 → 3182.98] Well, I have to say I've spent many, many days and nights in Joop's all over the continent, it seems.
[3183.54 → 3185.52] I didn't even know this infrastructure existed.
[3185.64 → 3188.08] This is the very first time you bring this up.
[3188.16 → 3189.54] I didn't even know it was a thing.
[3190.04 → 3192.06] And it's all those times when we've been in places where it's cooked.
[3193.18 → 3195.24] If he hasn't complained about it, you know it's good.
[3195.34 → 3195.94] Yeah, that's right.
[3197.18 → 3198.90] I've always hated Power line networking.
[3198.90 → 3201.80] I used to install it for clients who didn't want to run a cable.
[3202.00 → 3204.80] And, you know, they would complain, oh, it's not working.
[3204.88 → 3205.46] It's not working.
[3205.46 → 3208.90] And I would drive to their house and re-sync the thing and leave.
[3209.18 → 3211.96] Like, God, those things were annoying.
[3212.10 → 3213.22] But I'm glad it's working for you.
[3213.78 → 3214.02] I know.
[3214.38 → 3216.42] I thought it would be very frustrating.
[3216.88 → 3219.08] And it's been so good you could just forget about it.
[3219.18 → 3220.38] Just don't tell Brett where it is.
[3220.64 → 3221.86] Yeah, I have so many more questions.
[3223.04 → 3225.30] I have two more short ones.
[3226.28 → 3228.62] First one is Mealy.
[3228.96 → 3230.46] Are you guys still using Mealy?
[3230.66 → 3231.24] Oh, yeah.
[3231.36 → 3231.48] Okay.
[3231.82 → 3232.18] Yeah, yeah.
[3232.36 → 3232.52] Yep.
[3232.52 → 3233.68] Recipes app, yeah?
[3233.74 → 3235.84] I love Mealy so much.
[3236.44 → 3238.08] Yeah, all my recipes go in there.
[3238.24 → 3245.98] If I am looking at a recipe online, and I don't want to read all the blurb that they put in there for the SEO stuff, just pop it into Mealy.
[3246.10 → 3246.80] It strips it out.
[3246.92 → 3248.42] And then I've got a recipe ready to go.
[3248.62 → 3249.58] It's amazing.
[3249.58 → 3254.62] And then the other one is Invoice Shelf.
[3254.62 → 3262.78] As a private contractor, it's important to be able to track my expenses, my invoicing, and all of that.
[3263.10 → 3271.84] And if I want Chris to pay me, it's a good way to just send an invoice and have a list of every show that I've done.
[3271.84 → 3274.92] And as soon as I finish a show, I put it right in the invoice.
[3275.34 → 3282.18] And then on the dates that I send them, they go out, start a new one, and it gives me receipts that I can send out.
[3282.26 → 3282.94] It's fantastic.
[3283.90 → 3288.80] I wonder, Brent, how's that instance of Invoice Ninja I set up for you years ago holding up?
[3289.10 → 3294.18] Yeah, I still have that backed up file ready to be inserted into a new piece of infrastructure.
[3295.00 → 3296.62] I knew it, you piece of shit.
[3298.12 → 3300.08] I've got a reputation upkeep here.
[3300.08 → 3305.58] We have been getting a lot of really very kind emails and feedback.
[3305.98 → 3306.32] So many.
[3306.46 → 3311.94] And a bunch of very generous messages, both on Matrix and Discord and in the boost.
[3312.12 → 3315.08] So, Brent and West, you boys want to bust through these with me?
[3315.16 → 3317.10] We've got a good batch to get through.
[3317.36 → 3317.78] All right.
[3318.06 → 3321.32] And the Dude Abides kicks us off with an amazing baller boost.
[3321.42 → 3325.70] It's 404,404 SATs, which is just incredible.
[3326.18 → 3327.00] I see what they did there.
[3327.44 → 3328.30] Yeah, it's great, isn't it?
[3328.30 → 3331.14] He says, it's a bummer that I'm writing for the last episode.
[3331.80 → 3334.34] I've learned a lot for those last five years, so thank you both.
[3334.58 → 3340.44] I've sent you my home lab journey through these years in the site's contact form because it is a lot to unpack.
[3340.86 → 3346.34] The TLDR, though, is from my Raspberry Pi 3 to a full 15U rack with 10 gigabit connections now.
[3346.94 → 3347.72] We're going to miss you.
[3347.84 → 3348.98] I hope this message gets through.
[3348.98 → 3352.60] I've gone through some hoops to send them through Breeze to Fountain just so I could say hi.
[3353.24 → 3354.30] I'll see you on the up side.
[3354.30 → 3356.62] Well, thank you, the Dude.
[3356.62 → 3360.16] We've had so many messages like this week.
[3360.32 → 3369.42] We could spend six hours reading all the feedback we've had the last two, three, four weeks of people writing in and sharing their journeys.
[3369.42 → 3376.42] And, you know, people going like this chap here going from a Raspberry Pi 3 to an entire server racks worth of gear.
[3376.88 → 3381.46] People getting jobs because they realized that actually self-hosting was a passion of theirs.
[3381.94 → 3383.34] The infrastructure was a passion of theirs.
[3383.42 → 3391.42] And, oh, maybe I should pursue a career in this thing to people just using it as an escapism, like an escape hatch from their daily lives.
[3391.42 → 3398.30] And they can take back some control over certain aspects of their life where perhaps other aspects are lacking.
[3398.76 → 3399.70] And skill build.
[3399.92 → 3400.74] You know, we hear that a lot.
[3400.84 → 3401.26] Skill build.
[3402.08 → 3404.74] That's a good, you know, get some skills under your belt.
[3405.14 → 3406.50] That's really another great thing.
[3406.64 → 3409.20] And we have a few more to get to, Alex.
[3409.62 → 3411.68] I couldn't put all of them in here, obviously.
[3411.94 → 3413.84] But the Dude Abides had such an incredible boost.
[3413.92 → 3415.88] I wanted to put that in and say thank you.
[3415.88 → 3421.96] Well, our next booster, Dam, is actually kind of doing something awesome.
[3422.54 → 3424.24] And we'll get to his boost in a second.
[3424.44 → 3430.68] But he comes in with, what's that, 220,000 and then a second boost of 210,000.
[3430.68 → 3436.88] So like 430,000 SATs or something like that for this boost.
[3437.22 → 3440.34] Your show inspired us to build a business around Tail Scale.
[3440.48 → 3444.38] We created a Tail Net ready Docker compose files for easy self-hosting.
[3444.38 → 3449.70] Just git clone and add a Tail Scale auth key and then run Docker compose up.
[3449.94 → 3451.68] We plan to boost in and share this.
[3451.74 → 3456.72] But after learning the podcast is ending, we're continuing the mission with our very own podcast.
[3457.62 → 3459.18] Episode one is now out.
[3459.32 → 3459.84] More to come.
[3459.98 → 3461.86] And we'll put a link to that podcast in the show notes.
[3462.56 → 3465.28] Goodness knows he's been putting it all over our Discord this week.
[3465.62 → 3468.78] And thanks for showing us the way to do the new internet.
[3469.02 → 3471.10] Check out the repo podcast and our website.
[3471.70 → 3472.50] That is great.
[3473.06 → 3473.90] Good for them.
[3474.96 → 3476.66] So we'll put some links in the show notes.
[3476.90 → 3478.26] Now, I don't love the Spotify.
[3478.64 → 3480.40] Don't love the Spotify, I got to say.
[3480.56 → 3482.54] It's not the way.
[3482.64 → 3483.78] But I do appreciate the boost.
[3483.96 → 3484.94] Yeah, maybe reach out to Chris.
[3485.02 → 3486.82] He can set you straight on RSS feeds.
[3486.82 → 3488.20] Make sure it's on the podcast index.
[3488.20 → 3493.78] I couldn't believe I found out that anytime you want to host a podcast through Spotify,
[3494.24 → 3498.20] you surrender all rights to your content to do so.
[3498.58 → 3499.18] Oh, my God.
[3499.18 → 3509.06] The one that gets me about Spotify is, so you say you got an audio podcast, and you're putting your audio files out on your CDN, and you're tracking your downloads and, you know, you're vibing on your good downloads.
[3509.06 → 3517.08] And then you go over to Spotify and you check a box, and you say, I also want to enable a video feed because now I want to be a video podcast that has audio.
[3517.08 → 3528.10] The moment you check that box and become a video enabled feed as well, they repost all your audio files and then serve them up from their own CDN from that point forward.
[3528.10 → 3531.70] And you don't get any of the download stats or any of the information.
[3531.94 → 3532.74] You don't get to seed it.
[3532.78 → 3539.64] So if you want to swap a file out or if you want to track the downloads for yourself so that way you can report to advertisers or whatever, you don't get any of that information.
[3540.02 → 3541.66] Just because you checked a box that says turn on video.
[3542.78 → 3543.48] It's bad stuff.
[3543.56 → 3545.02] And they don't follow RSS standards either.
[3545.18 → 3546.16] So there's that as well.
[3546.66 → 3548.70] But it is great to see you guys working at it.
[3548.86 → 3550.02] That sounds like a really cool initiative.
[3550.16 → 3550.56] Thank you, Dan.
[3551.10 → 3555.72] Kangaroo Paradox boosts in with 201,980 stats.
[3555.80 → 3556.38] Oh, wait.
[3556.38 → 3560.16] This is the first and probably last boost to self-host.
[3560.58 → 3567.20] Fun fact, I actually discovered JB by searching for GPU pass-through and stumbling on LUP308 featuring Alex.
[3567.22 → 3567.46] Right.
[3567.64 → 3568.80] Been hooked ever since.
[3568.90 → 3569.28] Very good.
[3569.40 → 3573.70] This podcast gave me the motivation to start self-hosting my own services over the last year.
[3574.14 → 3580.26] First on that list was converting my gaming rig into a Proxmox machine with a Windows 10 VM with a Tesla P4 to play Zelda.
[3580.50 → 3581.80] Okay, I love it.
[3581.90 → 3582.66] Breath of the Wild.
[3582.88 → 3583.14] Yes.
[3583.64 → 3584.06] Good call.
[3584.06 → 3593.92] Ever since then, I'm fully down the rabbit hole and added an N5105 NAS on ZFS, Pi 4 cluster, and an M1 Mac Mini running Asa hi Linux.
[3594.16 → 3594.60] All right.
[3594.76 → 3598.14] Thanks for the content and making me feel better about my growing hardware addiction.
[3598.68 → 3600.70] Looking forward to future love for self-hosted content.
[3601.08 → 3601.38] Wow.
[3601.48 → 3602.86] That is quite the journey.
[3603.02 → 3604.32] Thank you for sharing that with us.
[3604.64 → 3605.40] Appreciate that.
[3605.96 → 3606.68] That's great.
[3606.94 → 3607.08] Yeah.
[3607.08 → 3608.00] Do tune in, Kangaroo.
[3608.58 → 3609.04] Do tune in.
[3609.12 → 3610.12] Do, do, do, do, do, do, do.
[3610.56 → 3611.26] For more of that.
[3611.46 → 3611.78] Yeah.
[3612.08 → 3612.68] Don't miss it.
[3613.16 → 3616.76] Well, Big Tree boosted in 52,800 SATs.
[3616.76 → 3623.30] I discovered you guys a couple of years ago just starting my self-hosted journey with an old PC turned into an Unpaid server.
[3624.00 → 3624.08] Nice.
[3624.08 → 3634.64] My home lab has since grown, of course, to also now include an Open Sense router, a mini PC Proxmox cluster, a backup server, a few pies, and a slew of unified gear.
[3635.44 → 3640.26] I'm constantly redesigning infrastructure and thinking ahead to the future upgrades, and it's all your fault.
[3640.26 → 3641.56] Can I move in?
[3641.62 → 3642.48] That sounds great.
[3643.48 → 3645.26] Self-hosted will definitely be missed.
[3645.42 → 3648.44] I've thoroughly appreciated your approach and insights over the years.
[3648.62 → 3658.76] So, cheers to Too Many Pies, Home Assistant Everything, Image, Jellyfin, D-Googling, Giraffe OS, full-time family IT, and most of all, you two fine fellows.
[3659.46 → 3660.58] Oh, that's really great.
[3660.68 → 3661.06] Thank you, Big Tree.
[3661.06 → 3664.38] Well, that's how you know they're a true fan, because they're mentioning a joke from a different podcast.
[3664.38 → 3665.54] Cross-show jokes.
[3665.76 → 3666.08] Love it.
[3666.96 → 3667.34] Yeah.
[3667.34 → 3672.44] You know, it occurs to me, why aren't them, like, there are a lot of self-hosted out there.
[3672.50 → 3683.54] Why have I never stayed at a B&B or something like that with someone who's like, here is the fibre internet Wi-Fi code, like, everything's self-hosted and powered with Unify and all this kind of stuff.
[3683.60 → 3684.74] Why are we still such a niche?
[3685.20 → 3686.12] Yeah, you're right.
[3686.20 → 3688.18] If I had an Airbnb, it would be rad.
[3688.60 → 3692.00] Here's your temporary login to your per-room home assistant to control things.
[3692.58 → 3694.86] Please wear this pendant when you move between the rooms.
[3694.86 → 3697.62] Alex, I have an idea for you.
[3697.68 → 3701.88] You should start Tech B&B and start a whole new movement.
[3702.66 → 3703.78] Yeah, I should.
[3703.90 → 3704.34] There you go.
[3704.56 → 3704.76] Yeah.
[3705.14 → 3714.16] I did see a YouTuber, actually, who's just opened a brand-new RV site with fibre hookups, fibre Ethernet hookups to each stand, each campsite.
[3714.20 → 3715.68] That's galaxy brain stuff right there.
[3715.76 → 3716.24] That's what I'm saying.
[3717.08 → 3717.78] I tell you what.
[3717.92 → 3721.68] Power comes in with 22,722 SATs.
[3722.18 → 3724.22] This is better late than never to boost in, I guess.
[3724.22 → 3729.84] Thank you for the five and a half years of great content and pushing the horizon on what is possible for all of us.
[3729.88 → 3733.50] I found you the first few months and listened through the catalogue immediately.
[3733.96 → 3736.16] And you've been the first in my listen queue ever since.
[3736.66 → 3743.10] I understand life rolls on, but count me among the multitude that are sad to see Chris and the Badger parting ways.
[3743.10 → 3746.38] Good luck to you and hope to hear you on UP and YouTube for now.
[3746.38 → 3748.92] Thank you, Power.
[3749.60 → 3757.42] Yes, and you can head over to JupiterGarage.com and pick up your Chris and the Badger t-shirt for some truly excellent limited edition self-hosted merch.
[3757.76 → 3758.54] All supplies last.
[3758.66 → 3759.04] Boom, boom, boom, boom.
[3760.84 → 3763.98] Southern Fred's ass boosts in with 5,000 SATs.
[3763.98 → 3766.76] 5,000 SATs for five years.
[3767.02 → 3769.80] Hate that the show is ending, but as a parent, I understand.
[3770.42 → 3772.16] Good luck in your adventures and moving.
[3772.68 → 3776.46] And have fun rediscovering how much stuff one accumulates when you have a child.
[3776.78 → 3778.54] Oh my god, so much stuff.
[3779.66 → 3788.24] If Brent really wants your drum set, well, I have plenty of storage space until the to-be-renamed Bang Bus is up to a cross-continental trip.
[3788.38 → 3788.58] Oh.
[3788.58 → 3791.04] Depending on how well it needs to be climate controlled.
[3791.26 → 3791.48] Hmm.
[3791.86 → 3793.20] Ooh, I like this challenge.
[3793.22 → 3795.06] The drums are still here, Brent, if you want them.
[3795.94 → 3797.00] Okay, I'll be there on Tuesday.
[3797.08 → 3798.20] Hot drums.
[3798.40 → 3798.70] Hot drums.
[3798.74 → 3800.74] In what mode of transportation?
[3800.84 → 3802.04] Are you bringing Vamoose with you?
[3803.86 → 3805.48] Still open to names for the thing.
[3805.62 → 3810.22] I think Vamoose is top contender for this new fan extravaganza.
[3810.24 → 3812.02] Vamoose is a strong candidate.
[3812.72 → 3813.64] But who knows?
[3814.02 → 3814.38] Who knows?
[3814.90 → 3818.34] Next boost comes in from Thor with 10,000 SATs.
[3818.86 → 3823.42] Saying, I have been listening to JB since Matt Hartley was on Linux Action Show.
[3823.44 → 3823.50] Oh!
[3824.04 → 3825.48] Me too, by the way.
[3825.84 → 3831.00] And since then, I have been learning and playing with Linux and that naturally evolved into home servers.
[3831.60 → 3836.96] Self-hosted has been a distilled stream of inspiration that has kept me playing with my home server setup for years.
[3836.96 → 3842.58] I look forward to hearing Alex on UP, but will miss the fortnightly fix of self-hosted fun.
[3842.92 → 3845.18] Thank you for the years of edutainment.
[3845.56 → 3846.52] Thank you, Thor.
[3846.96 → 3847.92] That's very kind of you.
[3848.58 → 3850.24] We really got so many great messages.
[3850.98 → 3854.90] We had 48 unique messages come in.
[3854.96 → 3857.48] 31 of you streamed SATs as we listened.
[3857.66 → 3862.32] So we stacked 40,995 SATs for those of you that streamed.
[3862.32 → 3873.92] And then we had, when you combine that with the boosters, we stacked an incredible 1,130,510 SATs, which is really incredible and a fantastic send-off for the show.
[3874.50 → 3875.50] That is insane, gentlemen.
[3875.50 → 3876.00] Congratulations.
[3876.00 → 3876.24] Congratulations.
[3876.74 → 3879.82] I think I also want to say you can still boost the show.
[3879.82 → 3888.22] Like for those listening, I don't know, in the future when this isn't the week self-hosted ended, maybe you're just getting caught up on the back catalogue or something like that.
[3888.28 → 3889.18] You can still boost in.
[3889.18 → 3891.22] And then those messages will still route to the right places.
[3891.94 → 3892.34] That's true.
[3892.42 → 3893.14] I'll keep an eye on them.
[3893.30 → 3898.02] And we could always route a couple over to Linux Unplugged if it's content fitting, too.
[3898.52 → 3902.64] But thank you, everyone, who did send a boost into the show for this episode or for any episode.
[3903.18 → 3905.22] It was a grand experiment.
[3905.22 → 3910.72] And we appreciate you participating in an open source peer-to-peer way to fund independent media.
[3911.72 → 3918.62] I think it's worth at this point just sort of recapping for anybody listening towards the end of the show what's happening next.
[3918.62 → 3925.76] The plan is, such as it is, that I'll drop by Linux Unplugged every now and again, and we'll do a sort of mini self-hosted segment.
[3926.02 → 3938.86] But as we've alluded to in this show, the fact that self-host is going away kind of frees up Linux Unplugged to cover a lot of these topics with Was and Brent picking up Home Assistant and some of the other self-hosted stuff, too.
[3938.86 → 3946.64] I think you can probably expect Linux Unplugged to kind of pivot a little bit more towards or include some of the topics that would have been in this show moving forward.
[3946.64 → 3949.66] I'm, of course, going to be on my YouTube channel.
[3949.82 → 3952.86] You can find everything I'm doing over at alex.ktz.me.
[3953.36 → 3959.48] I wrote a blog post this week sort of talking about some of the journey I've been on with this show over the last six years or so.
[3960.04 → 3967.52] And I want to take this opportunity to extend a huge heartfelt thank you to everybody involved with this production.
[3967.52 → 3972.80] The four of you on this call right now sort of talking to recording this episode.
[3973.76 → 3976.56] And Chris for taking a chance on me at the beginning.
[3977.40 → 3984.66] You know, I met you at Texas Linux Fest in 2018, and I was just a butt scratcher guy following you to a sandwich shop back then.
[3985.48 → 3987.76] Somehow a year later we were making a podcast together.
[3988.14 → 3988.98] I'm glad we did it, too.
[3989.06 → 3992.92] And, you know, the thing we did right was that trip to go see Dwindle to kick off the show.
[3993.00 → 3995.48] I think that was a great way to start the show, and it set a tone.
[3995.48 → 4002.76] And it was like an excuse as well to go a little bit further with the Home Lab than I probably would have without the show.
[4002.76 → 4005.16] So I think I got to push myself a little bit further, too.
[4005.36 → 4006.28] I'm really grateful for that.
[4006.68 → 4007.88] So I'm glad you pitched it.
[4008.12 → 4008.74] I'll tell you what.
[4008.82 → 4010.12] I think it was a good five years.
[4010.42 → 4011.48] It's been a heck of a show.
[4011.86 → 4014.32] You can justify a lot of credit card points in the name of content.
[4015.82 → 4019.28] You boys also look really great in those asbestos trousers, got to say.
[4019.36 → 4022.12] I mean, they're a little patinae at this point, but they've come in handy.
[4022.12 → 4026.20] So I'm going to put this on record.
[4026.70 → 4036.22] When we were recording episode one, and I hate to say it, I think Joe might have had a point because I made a point of going back and listening to episode one a few weeks ago.
[4036.78 → 4039.10] It's not very good, if I'm honest.
[4040.66 → 4044.18] But remember, I had never recorded a podcast before.
[4044.26 → 4048.18] I'd listened to you for many years, Chris, and I was incredibly nervous about doing it.
[4048.18 → 4052.08] And we'd spent all week leading up to recording this thing in your studio.
[4052.26 → 4055.80] We'd flown everybody into Seattle to come to your studio and record.
[4056.72 → 4057.76] Who was there?
[4057.82 → 4059.60] It was you, me, Was, Brent.
[4060.24 → 4061.88] It was during a whole team sprint.
[4062.30 → 4063.30] So we had a whole crew.
[4063.44 → 4064.34] It was a whole house.
[4064.36 → 4066.60] Not just a low-key Zoom call to record the first episode.
[4067.06 → 4069.68] And they were all waiting out in the living room while we did the first episode.
[4069.70 → 4070.96] Everybody was there listening.
[4072.00 → 4074.14] And we recorded episode one.
[4074.14 → 4078.54] And I came out thinking I'd done an amazing job, obviously, because I had no idea.
[4079.04 → 4080.98] And Joe just goes, it was s***.
[4084.42 → 4088.10] I hope you're wearing your asbestos trousers, Alex, because that was s***.
[4089.46 → 4091.04] The first episode was rough.
[4091.16 → 4091.70] But you know what?
[4091.72 → 4092.54] You picked it up quick.
[4092.62 → 4094.32] And you did go back and do another one.
[4094.44 → 4097.68] So to your credit, like a pro, you went back in and did it again.
[4098.46 → 4099.30] Well, yeah.
[4100.38 → 4101.60] Such is life sometimes.
[4101.60 → 4104.20] But, you know, it's been a real journey with you guys.
[4104.60 → 4109.14] And, you know, you think about all the different things, places we've been together and everything like that.
[4109.24 → 4111.76] Like, you're not just co-hosts to me.
[4111.82 → 4115.74] I think you're an extended part of the Kitschier family, so to speak.
[4115.76 → 4117.54] And I hope that the feeling is mutual.
[4118.18 → 4123.10] Will we get to see, you know, your new rig somewhere in the Seattle area sometime, perhaps?
[4123.32 → 4124.32] I sure hope so.
[4124.44 → 4125.34] Oh, my God.
[4125.38 → 4125.78] You better.
[4125.78 → 4128.08] We were at the beach last week.
[4128.20 → 4130.18] We were at Cape Hatteras and the Outer Banks.
[4130.26 → 4137.04] And I drove my truck on the Outer Banks beaches and had, like, a whale of a time with a Ford Raptor on the sand dunes.
[4137.12 → 4138.38] It was freaking amazing.
[4138.66 → 4139.18] Hold on.
[4139.36 → 4139.94] I'm sorry.
[4140.08 → 4142.02] I've got to interrupt for just a moment.
[4142.14 → 4142.56] Cape what?
[4143.74 → 4144.58] Cape Hatteras.
[4144.70 → 4145.64] Cape Hatteras.
[4148.14 → 4149.22] Oh, it continues.
[4149.22 → 4149.66] Sorry.
[4151.82 → 4153.02] I grew up in North Carolina.
[4153.72 → 4156.98] You can just edit yourself saying it.
[4159.26 → 4160.50] So what am I doing?
[4160.52 → 4162.92] I'm saying Hatteras, whereas you're saying Hatteras.
[4163.12 → 4163.52] Hatteras.
[4163.70 → 4164.06] Hatteras.
[4164.76 → 4165.16] Hatteras.
[4165.28 → 4165.72] There you go.
[4165.86 → 4166.42] Well, there you go.
[4166.54 → 4167.32] Today I learned.
[4167.42 → 4168.18] Yeah, that was perfect.
[4168.60 → 4169.02] There you go.
[4169.12 → 4173.26] You know, I think we have a beach here in Washington that's easier to pronounce that you can park your RV on.
[4173.34 → 4173.90] It's pretty cool.
[4173.90 → 4181.42] So anyway, we came across a few different RV dealers on the way out to the coast.
[4181.84 → 4185.90] And I think we've kind of settled on a Class A diesel pusher.
[4185.92 → 4186.60] Oh, yeah, baby.
[4186.68 → 4187.36] Going all the way.
[4187.36 → 4195.60] It's like a big old 40-foot rig that can tow the Raptor behind us and just have a good old time for a year on the road, you know, before we go back to England.
[4196.24 → 4196.58] Nice.
[4196.74 → 4197.78] That is going to be fun.
[4198.36 → 4198.90] I hope so.
[4198.90 → 4211.00] But the reason I brought up the beach at all, sorry, Drew, you distracted me there with my excellent mispronunciation, is that Wifey bought a like, it's a National Parks Passport stamp collection book.
[4211.32 → 4217.62] And it not only has all the National Parks, but it's got all the National Seashores, historic sites, monuments.
[4217.90 → 4221.16] Like, there's 400 and some stamps to collect in this thing.
[4221.72 → 4223.74] There's one in Guam, for crying out loud.
[4223.82 → 4226.08] So we have to somehow get the magic bus over to Guam.
[4226.14 → 4226.98] I don't know how I'm going to do that.
[4226.98 → 4229.02] Well, you better come visit me in Denver, too.
[4229.36 → 4230.10] Yeah, you bet.
[4230.16 → 4232.80] Well, we're going to try and collect as many as we can over the next year.
[4233.44 → 4238.70] I'll be doing a bunch of stuff for Tail scale on the road, like going to conferences and speaking at them as well.
[4239.12 → 4242.94] So, yeah, it's just going to be, like, the most fun year of my life.
[4243.06 → 4247.06] The next two months are going to suck as we sell everything and, like, list the house.
[4247.24 → 4252.90] But the carrot at the end of that is that we've got the road trip of all road trips to end road trips coming up.
[4252.90 → 4253.24] Yeah, really.
[4253.92 → 4255.08] It's going to be an adventure for sure.
[4255.08 → 4257.60] It's a memory-making machine.
[4258.18 → 4259.22] Yeah, it really is.
[4259.64 → 4262.90] And a tour of all the fine self-hosted setups across the country.
[4263.72 → 4267.00] And drinker of all the diesel gallons, probably, no doubt.
[4268.12 → 4268.86] Yeah, at least that.
[4269.50 → 4274.08] So I guess all that's left to say at this point is that folks can find the –
[4274.62 → 4280.90] well, we've got the entire crew for Linux Unplugged on this episode right now over at linuxunplugged.com.
[4280.90 → 4284.82] Where else can folks go to find more about Jupiter Broadcasting, Chris?
[4285.16 → 4288.04] Check out the fine shows at jupiterbroadcasting.com.
[4288.08 → 4289.84] We've got some things cooking in the works.
[4289.96 → 4295.54] So you can always get subscribed to the All Shows feed, and that way you don't miss if something new were to land in not too long.
[4296.04 → 4296.96] So that's a good tip.
[4296.96 → 4303.02] I think that's a pro tip I'll end on right there is get the All Shows feed, and then when new things do land, you get it right away.
[4303.82 → 4307.82] So I guess all that's left to say at this point is a million thank yous.
[4307.88 → 4311.02] Thank you to Chris for being my co-host these last few years.
[4311.42 → 4315.18] Thank you to Was, Brent, Drew for the support as well and the love.
[4315.18 → 4320.80] Thank you to the members for supporting independent media over the years.
[4320.86 → 4322.82] Thank you to everybody that's boosted into the show.
[4323.24 → 4326.80] And if you've just been a passive listener, great big thank you to you too.
[4327.40 → 4329.86] This show would not work without an audience.
[4330.04 → 4334.46] We'd just be a couple of dudes talking into our underpants without you lot.
[4334.46 → 4339.96] So from me to you and everybody involved in this production, endless heartfelt gratitude.
[4340.88 → 4345.04] So I suppose it's time I said that has been self-hosted.show.
[4345.18 → 4347.16] Door, door, door, door.
