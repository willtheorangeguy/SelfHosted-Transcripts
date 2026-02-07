[0.00 --> 6.26]  You know, a few episodes ago, I told you that my UK server was dead and busted and had ceased to be.
[7.82 --> 11.64]  I'm delighted to say, thankfully, that it was the UPS that was the problem.
[12.48 --> 13.02]  No way.
[13.02 --> 13.58]  Oh, that's best case.
[14.14 --> 14.50]  Yeah.
[14.98 --> 16.18]  So here are the symptoms.
[16.34 --> 19.40]  Tell me if you would have picked the UPS as being the problem.
[20.10 --> 23.40]  The system powers off randomly.
[24.20 --> 29.20]  You know, so I would go to try and do a ZFS backup or watch a Plex thing from the UK or whatever.
[29.20 --> 32.88]  And the server's off and I'm like, hmm, that's weird.
[33.02 --> 36.02]  I wonder if my mother-in-law did something or if there was a power cut or something.
[36.48 --> 38.50]  And then it happens again a couple of weeks later.
[38.50 --> 41.98]  And then it happens two days later and then 10 days later.
[42.28 --> 43.56]  Just totally random.
[43.98 --> 46.54]  You come and just find the server just isn't on.
[46.98 --> 51.34]  So then you log into the IPMI and you try and turn the thing on.
[51.46 --> 52.98]  And the IPMI still works.
[53.94 --> 59.34]  But whenever it, I guess, tries to switch the computer on, it draws too much juice.
[60.08 --> 63.46]  What's the first thing that would come to your mind that something's not turning on?
[64.26 --> 66.36]  I would just assume you're popping a circuit or something.
[66.46 --> 68.60]  I don't know how it works over there with your weird electronics.
[68.90 --> 72.74]  But I would assume like, you know, popping a circuit, GFI needs to be reset, you know.
[72.96 --> 74.20]  Yeah, GFI could be a good one.
[74.40 --> 77.40]  But then the IPMI wouldn't work because it's built right into the motherboard.
[78.12 --> 78.44]  Okay.
[78.60 --> 78.94]  All right.
[78.94 --> 80.14]  Yeah, I'd say power supply.
[80.82 --> 81.86]  Yeah, power supply.
[81.96 --> 82.66]  That's a good one, Brent.
[82.76 --> 84.26]  That's exactly where my mind went.
[84.44 --> 89.64]  So good friend of the show, Al, who came to the self-hosted meetup when I was in Norwich this summer.
[90.10 --> 95.66]  Very kindly, he only lives about 15 minutes away from my mother-in-law's house where the server lives.
[96.02 --> 100.42]  Went and took it back to his house for the week to try and help me diagnose it.
[100.58 --> 105.98]  And he messaged me and said, Alex, I got it home and plugged it in and it came on instantly.
[106.16 --> 107.38]  What are you talking about, mate?
[107.38 --> 109.18]  And you're like, I'm sorry?
[110.80 --> 111.24]  What?
[111.58 --> 112.52]  Now try doing something.
[112.58 --> 113.38]  Does it turn off?
[113.50 --> 114.70]  Does it overheat?
[114.76 --> 115.26]  What's happening?
[115.76 --> 115.96]  Yeah.
[116.04 --> 119.02]  So we just left it for a week and it was fine.
[119.20 --> 126.64]  So I bought a new UPS and gave Al the old one because he can replace the battery more easily than I can from here.
[126.64 --> 130.00]  And everything's been fine for about the last three weeks.
[130.00 --> 141.02]  With a battery failure, you would hope it would fail, I guess, gracefully and just in a power outage, not provide proper backup, but still provide consistent power.
[141.18 --> 144.96]  I suppose by running it through the battery, you're probably getting additional protection there.
[144.96 --> 152.02]  But I find it ironic, Alex, because UPSs are so often thought of like something that adds reliability and stability.
[152.28 --> 155.84]  But it is easy to forget they can be a point of failure.
[156.46 --> 167.32]  Well, this particular one, I think I bought it when we moved to London or just before we moved to London, which would be, gosh, eight, nine years ago now.
[167.32 --> 176.82]  So it's getting up there in age, but you would expect it to fail with some kind of a warning tone or something that mother-in-law could go, hey, Alex, your computer's...
[176.82 --> 179.22]  There's a really obnoxious beep coming from the room.
[180.88 --> 182.02]  Nope, nothing like that.
[182.22 --> 188.02]  So the UPS I got to replace, it has a USB port so I can plug it in and monitor it via APC.
[188.78 --> 189.36]  What's it called?
[189.46 --> 190.66]  APC UPS Demon.
[191.12 --> 195.42]  And then over tail scale, I bring it into Prometheus in this house and bada bing, bada boom.
[196.12 --> 196.48]  Smart.
[196.48 --> 200.26]  Well, you probably heard there, our buddy from Canada is joining us today.
[200.42 --> 201.32]  Mr. Brent Lee is here.
[201.38 --> 204.42]  He's going to be talking about a new NAS he built in a little bit.
[204.50 --> 205.06]  Hello, Brent.
[205.18 --> 206.00]  Thanks for joining us.
[206.36 --> 206.50]  Hello.
[206.62 --> 207.60]  Yeah, always good to be back.
[208.20 --> 217.20]  I, of course, know that you've been following along with our no-googtober conclusions because you were asking me earlier today about my config for setting up searching.
[217.86 --> 219.02]  What kind of config, Chris?
[219.46 --> 219.78]  What?
[219.86 --> 220.64]  It was a Nix config.
[220.72 --> 221.50]  I wasn't going to say it.
[221.58 --> 224.24]  So you make me do this, then I get in trouble in the Matrix chat.
[224.44 --> 224.62]  See?
[224.62 --> 225.40]  This is what happens.
[225.40 --> 227.04]  What did you get in trouble for?
[227.94 --> 230.30]  Oh, you know, talking about Nix.
[230.64 --> 233.08]  Somebody always criticizes me somewhere every time we do it.
[233.54 --> 234.06]  Well, I don't.
[234.26 --> 236.20]  I used to, but I've seen the light now.
[236.34 --> 240.34]  So I guess these people are just, you know, a little bit behind the time.
[240.50 --> 241.96]  I shouldn't say that.
[242.02 --> 243.18]  I'm insulting the audience, aren't I?
[243.18 --> 246.06]  That's a golden rule of content not to do that.
[246.62 --> 247.26]  You know what else?
[247.32 --> 248.20]  We've seen the light, though.
[248.84 --> 254.24]  We've seen the light that Google might be done, at least for a certain category of users.
[254.24 --> 254.80]  Don't you think?
[254.86 --> 257.96]  I mean, looking back at no-googtober, I think it went really smooth.
[257.96 --> 260.24]  I haven't missed Google one bit.
[260.24 --> 273.64]  It's almost up there with the Jellyfin January challenge we did a couple of years ago as being like a real nice surprise of, oh, actually, the free and open solution alternatives are actually pretty good.
[273.64 --> 275.40]  Mm-hmm, mm-hmm.
[275.54 --> 287.00]  And I do have to say I found myself also using Claude and perplexity basically for everything that's not just a straight up I'm searching for a website or a business.
[287.50 --> 299.50]  Anything that's kind of informational or I'm looking for syntax or I'm looking for config or, for example, this morning I was troubleshooting a mechanical failure in one of my cars and working through the possible scenarios and narrowing it down.
[299.50 --> 311.56]  And a conversational situation like with Claude, it's perfect for that because I can say, okay, there's no oil leaks and there's been no metal shavings on the ground, so can you eliminate all those possible issues?
[311.72 --> 313.10]  And then it works it through with me.
[313.30 --> 316.78]  That's just so much more superior than search for that exact kind of thing.
[316.98 --> 318.32]  Have you used ChatGPT for anything?
[319.12 --> 319.36]  No.
[320.02 --> 320.42]  No.
[321.20 --> 321.60]  No.
[321.72 --> 322.92]  I literally have not.
[323.30 --> 327.96]  I would be willing if I could pull it into some sort of self-hosted chat app just through the API.
[327.96 --> 336.22]  You know, I'm really looking for something where I could have Llama, Anthropic, and OpenAI's API all in one front end.
[336.76 --> 339.00]  Then I think that – then I would probably use OpenAI a little bit more.
[339.06 --> 345.74]  But for me, perplexity and Claude seem to have it covered because Claude's really good for, like, configs and development stuff.
[345.98 --> 348.68]  And perplexity seems really good at current information.
[349.00 --> 351.88]  It does, like, actively citing more recent information.
[352.02 --> 353.10]  So it's great for actual searches.
[353.38 --> 354.06]  Yeah, that's it.
[354.06 --> 368.14]  You know, I think my conclusion really – I put a toot out a couple of weeks ago saying someone once told me a few years ago that I was going to have to pay for Google Search in the future.
[368.64 --> 374.18]  And I recall literally laughing in their face saying, that's never going to happen.
[374.18 --> 376.62]  Why would anybody ever pay for Google Search?
[376.68 --> 382.54]  Like, it was this endless commodity that, you know, the ad model they have would prop up forever.
[383.52 --> 389.00]  But you look at the incentives of the algorithm.
[389.88 --> 393.88]  Its entire purpose is to serve you ads, right?
[393.88 --> 395.24]  Not to serve you good content.
[395.64 --> 396.94]  It's to serve you ads.
[396.94 --> 406.02]  And also, by that same token, people are generating content that is either, you know, content marketing stuff.
[406.34 --> 410.66]  I saw something just yesterday talking about Docker Compose isn't enough.
[410.92 --> 415.00]  And it was literally a – the arguments were terribly flawed.
[415.36 --> 419.98]  But it was this great long sort of 10-minute long blog post talking about a whole bunch of stuff.
[419.98 --> 421.30]  And the arguments were really weak and whatever.
[421.44 --> 428.02]  But it ranks really well when you talk about Docker Compose and Kubernetes and stuff because it's all – it was on the top of Hacker News.
[428.16 --> 434.94]  And it, you know, just – well, I guess what I'm trying to say is that you type anything into Google these days.
[435.90 --> 445.60]  And think about the number of man hours that have gone into people optimizing and tweaking every little dial to have that piece of content rank more highly.
[445.60 --> 454.82]  It's not going to be me or you with our independent media and our little personal blog sites like it used to be in the good old days of the internet.
[455.12 --> 471.70]  It's going to be companies with SEO content marketing teams that have spent time fettling and – I don't want to accuse anybody of anything – but AI generating articles that have the correct keywords to rank more highly.
[471.70 --> 475.54]  And Google is just a victim of its own success in that regard.
[476.28 --> 483.74]  Everybody knows that's why all recipes have like two paragraphs of their life story because they're trying to optimize for Google looking for that kind of stuff.
[483.82 --> 486.86]  Google is looking for meat and content and not just small short stuff.
[487.40 --> 492.24]  And so you've seen the perversion of web content to kind of meet that requirement.
[492.24 --> 500.80]  And now it feels like, Alex, we're at a period of time where I can kind of see that monopoly Google has on search really getting challenged.
[500.96 --> 502.98]  I don't think for everyday people yet.
[502.98 --> 515.40]  But the fact that you and I, between search XNG or whatever you want to call it, searching and Claude and Perplexity and maybe others you've tried, I don't know, it literally did not need Google.
[515.40 --> 526.72]  And to me that is astonishing because go back even just four years maybe, three and a half, four years ago, and it seemed like nobody was ever going to topple Google.
[526.72 --> 537.36]  And it's amazing how these tech giants, while they're not beat yet and they're still doing great, like new kinds of paradigm shifts come along that just stand out.
[537.36 --> 540.20]  And I am sure they'll be around for a very long time and be very successful.
[540.46 --> 542.06]  But these are real challengers.
[542.80 --> 553.96]  During this challenge for me, I was doing a bunch of development work with Terraform at work and trying to deploy Tailscale using Terraform on top of AWS.
[554.70 --> 561.44]  And I was coming up against an issue where I was providing the API key or the auth key.
[561.60 --> 564.76]  I forget which way around I had it wrong, but my syntax was wrong.
[564.76 --> 568.80]  And so I just asked Perplexity, hey, you know, what am I doing wrong?
[568.90 --> 570.26]  Here's my code.
[570.32 --> 576.04]  And I just copy and pasted the actual Terraform file, attached it to the query so it had extra context.
[576.78 --> 590.40]  It took me to the exact line of source code in the open source operator or provider for Terraform, sorry, that told me the exact syntax that I needed to use.
[590.40 --> 595.92]  It says, no, Alex, it's not auth key, it's API key.
[596.06 --> 597.58]  This line of source code says so.
[597.84 --> 600.12]  And I'm like, oh, goodness.
[600.34 --> 604.24]  Like that just would never happen in the Google universe.
[605.12 --> 609.34]  Yeah, you would be reading forum post after forum post and read a thread trying to put it together.
[609.34 --> 612.30]  And that for me was the moment where it clicked.
[612.42 --> 620.56]  And I was just like, you know, I think give it five years, maybe more for normals, but certainly for people like you and I, we're already switching.
[621.38 --> 623.90]  I think the critical mass will come.
[624.56 --> 631.08]  Either Google will catch up and they'll figure out how the algorithm works, because this is the other part of it.
[631.08 --> 642.88]  I read another post talking about how a lot of the original talent that wrote these internal services that run the Google search algorithm, a lot of that talent's left.
[643.74 --> 647.32]  And so a lot of these boxes internally at Google are just black boxes.
[647.44 --> 651.20]  They have no idea how certain things are coming to certain conclusions.
[651.20 --> 662.26]  And I don't know how much truth there is to that, but I could certainly see that, you know, we've built this complex thing and we're just going to leave it in the corner and not touch it because it works.
[663.04 --> 671.96]  You know, but I was revisiting your Googtober kickoff episode earlier today, and you mentioned defaults being king.
[672.12 --> 676.38]  And I wonder what it'll take to see those defaults change in web browsers.
[676.38 --> 684.90]  Because right now, you know, us early adopters, you're going to find those sites and making them work for you, like Perplexity, you're going there to use them.
[685.20 --> 690.88]  And that's, from your own argument, Alex, is not going to work for most of the population.
[691.20 --> 695.00]  So what's it going to take for those defaults to change?
[696.02 --> 701.20]  I'm just going to ask Perplexity, how much did Google pay to be the default search engine in 2020?
[701.74 --> 702.62]  Let's go for 2022.
[704.16 --> 705.46]  Let's see what it comes back with.
[705.46 --> 711.98]  This is the thing I really like about these more context-aware search engines.
[712.20 --> 713.74]  Like, they give you the exact sources.
[713.94 --> 719.06]  So, like, it links me to a Reddit thread and a 9 to 5 Mac thread and Business Today and Apple Insider.
[719.50 --> 731.74]  It says, in 2022, Google paid Apple alone a staggering $20 billion to maintain its position as the default search engine in Safari across iPhones, iPads and Macs.
[731.74 --> 738.18]  Now, that's just one small pillar that they are paying to be the default on.
[738.26 --> 739.16]  I don't know.
[739.40 --> 742.70]  I'm not going to dig any further as to how much they pay to be the default everywhere else.
[742.70 --> 745.88]  How much is the development cost for Chrome, for example?
[746.20 --> 747.46]  Like, that's not factored in here.
[748.28 --> 752.46]  So to answer your question, I suppose, what would it take for Google to not be the default?
[753.76 --> 754.54]  Follow the money.
[755.14 --> 759.24]  Well, I could see Apple becoming its own default if they keep going with their AI strategy.
[759.48 --> 764.04]  And OpenAI certainly is getting enough money to bump Google out of that place in certain areas.
[764.04 --> 764.84]  So we'll see.
[765.58 --> 765.66]  Yeah.
[765.84 --> 767.56]  Well, I mean, Apple like money, right?
[767.62 --> 768.54]  They like that $20 billion.
[769.64 --> 771.32]  Or they'd like not to spend it.
[771.68 --> 772.78]  Well, Google's paying them now.
[772.80 --> 775.54]  So that's a nice, juicy little bit of money they make.
[775.96 --> 779.06]  There is an antitrust suit that is proceeding.
[779.44 --> 784.18]  And one of the things on the table is forcing Google to stop doing those deals.
[784.30 --> 785.00]  May or may not happen.
[785.46 --> 786.96]  That's one of the things on the table at the moment.
[787.32 --> 791.54]  So these have been brought up in other contexts as well because Google pays other vendors as well.
[791.54 --> 793.70]  And they may have to stop.
[794.04 --> 800.64]  And I think that's when Apple would swap in something like Apple Intelligence, probably backed by Bing or Google then or something like that.
[800.92 --> 803.72]  And OpenAI just released their OpenAI search tool.
[804.46 --> 807.58]  Kind of a soft launch, but they have launched an OpenAI search engine now.
[808.16 --> 812.38]  So it seems to me you're going to have the platform vendors build in their own Google alternatives.
[812.72 --> 814.86]  And they're going to be varying quality.
[815.02 --> 821.30]  And then you're going to have self-hosters like us that are going to try to plug in our own self-hosted solutions.
[821.30 --> 823.50]  And there are beginning to be more of those.
[824.16 --> 824.40]  Exactly.
[824.62 --> 825.80]  Just like Perplexica.
[826.12 --> 829.64]  So I'm aware this podcast is called Self-Hosted.
[829.76 --> 835.76]  And you and I have just spent a while extolling the virtues of perplexity and Claude.
[835.96 --> 842.66]  But Perplexica is a self-hosted alternative or kind of clone of perplexity.
[842.66 --> 853.78]  So it uses SearchXNG under the hood, searching under the hood, bizarrely enough, to do its actual Google searches that it then feeds into the local llama model that it's using.
[854.64 --> 861.78]  And it's just a really nice, like, daisy chaining of all these open tools that are able to feed into one another.
[862.46 --> 863.86]  It's not super reliable.
[864.00 --> 867.66]  I span it up for some of the time during this month to test it out.
[867.82 --> 877.94]  And I found that sometimes it was sending empty responses to searching, which caused it to kind of hang and crash and, like, go into some kind of, like, a race condition waiting for input to come through.
[877.94 --> 884.82]  But it's just really exciting that we've got things like Perplexica coming through that, okay, they're not ready for prime time yet.
[885.26 --> 887.44]  But give it a little bit of time.
[887.84 --> 897.32]  And if you've got even just one of the new M4 Mac minis, for example, you could use that as a fairly cheap machine learning server with running Ollama on it.
[897.48 --> 902.92]  And that's going to be more than powerful enough to run something like Perplexica for sort of the average home user.
[903.22 --> 904.84]  I think that's where it's going to go eventually.
[904.84 --> 910.14]  Right now it needs too much GPU horsepower for the average person to even consider self-hosting it.
[910.50 --> 919.02]  But it does make you wonder about the scale of the challenge of the data center farms behind these big AI companies.
[919.80 --> 919.96]  I know.
[920.02 --> 929.50]  And it makes me wonder if maybe in the future smaller models just aren't more competent and you have people just running smaller models distributed instead of these giant hosted models.
[929.50 --> 937.30]  You know how the arc of tech sort of started centralized with time compute in universities and whatnot.
[937.52 --> 942.66]  And then we moved out to the micro PC where people got compute at their local desk.
[942.78 --> 948.74]  And then we moved back to the internet where we have a lot of cloud compute, which is essentially time slice computing again.
[948.74 --> 958.60]  And it wouldn't be interesting if AI takes a path, these LLMs in particular, where the really useful ones take all this horsepower and all this GPU and all this big data.
[959.04 --> 963.92]  And then as they get better and more sophisticated in, you know, five, 10 years, they're micro.
[964.32 --> 971.58]  And, you know, you have them built into all of your phones and your laptops and your OSs and your individual apps and your hosted apps and all that.
[971.60 --> 973.96]  And it's just one Docker container image that it can include.
[974.06 --> 976.28]  And now you've got it built right in and it can even run on your CPU.
[976.28 --> 977.92]  I could see it getting there.
[978.50 --> 983.40]  And at that point, then these big data centers kind of become obsolete or they even get more powerful and do more stuff.
[983.48 --> 984.00]  I don't know.
[984.76 --> 986.94]  I predict you'll get Perplexica in your pocket.
[987.66 --> 988.50]  I would love it.
[988.84 --> 990.22]  I'm going to check out Perplexica.
[990.36 --> 997.44]  This looks, I mean, it sounds like it's maybe just maybe keep an eye on it right now, but it's not a crazy Docker composed to get going, it looks like.
[997.48 --> 998.88]  It's pretty reasonable and set up.
[999.40 --> 1000.10]  It's pretty nice.
[1000.20 --> 1000.40]  Yeah.
[1000.40 --> 1006.44]  So it uses, like I say, Ollama under the hood and then searching as well.
[1006.64 --> 1008.26]  There's got a bunch of different search modes.
[1008.42 --> 1013.88]  Like you can do the standard kind of like writing assist, academic search, that kind of stuff.
[1014.12 --> 1018.04]  It also has, funnily enough, a Reddit default search mode.
[1018.22 --> 1022.04]  So it will automatically search Reddit for discussions and that kind of thing.
[1022.22 --> 1023.54]  That's what you've always asked for.
[1023.54 --> 1030.18]  What every Google search for the last few years has had Reddit appended to it to avoid the SEO spam, really.
[1030.60 --> 1030.62]  So.
[1031.26 --> 1031.44]  Yep.
[1033.26 --> 1035.90]  Unraid.net slash self-hosted.
[1035.96 --> 1042.40]  Hey, self-hosters, mark your calendars because you will not want to miss Unraid's annual Cyber Weekend sale.
[1042.74 --> 1043.62]  So here's the details.
[1043.72 --> 1052.06]  For four days only from November 29th to December 2nd, you can save $15 on Unraid's Unleashed and starter licenses.
[1052.06 --> 1056.86]  And then you can also save 50% when you bundle it with a second Unleashed or starter license.
[1056.96 --> 1069.64]  Now, you might not have known this, but a lot of Unraid users end up with multiple licenses, maybe a test server, maybe an off-site backup server, or maybe you have a tech enthusiast friend or family member that you want to gift Unraid.
[1070.30 --> 1073.14]  And if you already own Unraid, they've got you covered there, too.
[1073.32 --> 1080.38]  Upgrades to the Unleashed license will also be discounted, but that's only for four days from November 29th to December 2nd.
[1080.38 --> 1083.10]  And don't forget about Unraid 7.
[1083.78 --> 1084.58]  The beta is out now.
[1084.66 --> 1086.26]  It's coming along really nicely.
[1086.38 --> 1096.62]  It's got game-changing features like full ZFS file system support, a revamped dashboard, much improved VM management, and a sweet new integration with Tailscale.
[1096.82 --> 1097.52]  Yeah, that's right.
[1098.06 --> 1103.06]  So go find out more and get ready for the sale by heading to Unraid.net slash self-hosted.
[1103.68 --> 1104.02]  Unraid.
[1104.22 --> 1105.48]  Unleash your hardware.
[1105.90 --> 1108.54]  Unraid.net slash self-hosted.
[1108.54 --> 1109.54]  Unraid.net slash self-hosted.
[1109.54 --> 1110.54]  Unraid.net slash self-hosted.
[1110.54 --> 1117.06]  A few weeks ago, I mentioned a tool called BentoBox, which is a window manager for macOS written by a good friend of mine.
[1117.88 --> 1122.70]  And I had several people write in and say, actually, I really enjoyed that recommendation.
[1123.06 --> 1129.24]  And the Mac has been my sort of development platform now for a few years because I have to use a lot of Adobe stuff.
[1129.24 --> 1135.76]  I do Final Cut, and there's just nothing else that really kind of sits in that gooey middle where I get a proper terminal as well.
[1135.96 --> 1139.64]  And I swear I've been through this rationale on the show before.
[1140.58 --> 1144.46]  But I'm talking to you today through a brand new MacBook.
[1145.24 --> 1147.56]  You got a new M4 over there, huh?
[1147.88 --> 1148.34]  I did.
[1148.46 --> 1149.90]  Yeah, I've got the old M1 Macs.
[1149.92 --> 1150.50]  I say old.
[1150.70 --> 1152.30]  It's what, three or four years old now?
[1152.44 --> 1153.64]  2020, right?
[1153.64 --> 1157.12]  Yeah, I mean, it is old in terms of releases now.
[1157.34 --> 1159.02]  It's three back, right?
[1159.32 --> 1160.24]  I wasn't going to buy it.
[1160.70 --> 1162.04]  And then Factorio came out.
[1162.88 --> 1166.24]  And I'm running my megabase across multiple planets now.
[1166.42 --> 1169.24]  And the fans are going, whir, as I'm running.
[1169.44 --> 1178.26]  And then I realized that the M4 was going to be better because I read a Reddit post about it.
[1178.26 --> 1184.26]  And someone's saying that I did the M1 Macs upgrade from the M1 to the M4, and it can run my factories.
[1184.44 --> 1186.08]  And the fans don't even spin up.
[1186.44 --> 1187.62]  So it's super nice.
[1188.04 --> 1192.66]  I love how Alex's determining factor now is, did the fan spin?
[1192.82 --> 1193.94]  Oh, it's time to upgrade.
[1194.50 --> 1194.76]  Yeah.
[1195.08 --> 1195.50]  Hey, man.
[1195.62 --> 1199.14]  You don't want the fans when you're trying to play Factorio, okay?
[1200.16 --> 1201.00]  This is true.
[1201.10 --> 1205.54]  Because I must have added, I don't even know how many hours.
[1205.54 --> 1209.00]  It's well over 100 since it came out like two weeks ago.
[1209.42 --> 1210.82]  It's kind of a problem.
[1211.42 --> 1213.78]  But anyway, just a quick side note.
[1213.96 --> 1222.50]  Factorio 2.0 Space Age has far surpassed any dreams of expectations I could have possibly had for that game.
[1222.90 --> 1224.70]  It is so good.
[1224.92 --> 1227.24]  I can hardly articulate to anybody.
[1227.76 --> 1234.66]  If your brain works that way in that kind of slightly ADHD, like problem solving, software development kind of way,
[1235.66 --> 1236.16]  beware.
[1236.34 --> 1238.88]  It's a dangerous game to let yourself play.
[1239.76 --> 1240.82]  So I'm just getting started.
[1240.90 --> 1242.32]  Can I jump right to the space?
[1242.38 --> 1243.18]  Because I love space.
[1243.38 --> 1244.00]  Oh, no.
[1244.10 --> 1246.22]  You have to build your own rockets and stuff.
[1246.22 --> 1246.72]  I got it.
[1246.76 --> 1247.92]  Oh, God.
[1248.02 --> 1248.38]  Okay.
[1248.64 --> 1249.06]  All right.
[1249.26 --> 1253.52]  Well, honestly, a lot of the mechanics you learn on the first planet, they still apply to the next ones.
[1253.52 --> 1259.72]  But they've done a really great, I won't give any spoilers, but there are three or four extra new planets now.
[1260.38 --> 1266.46]  And each one has its own complete twist on the mechanics that you've learned on your home planet.
[1266.46 --> 1272.94]  I mean, for veteran players like myself, it's been really weird to like, I can't say anymore.
[1273.08 --> 1273.68]  I'll spoil it.
[1273.74 --> 1283.62]  But it's been really weird to just have to land on a new planet and be like, huh, none of the stuff I've done before with like recipe chains and stuff, like none of that works anymore.
[1283.80 --> 1285.44]  And you have to throw it all out and start again.
[1285.44 --> 1287.88]  And it's been just a wonderful experience.
[1288.20 --> 1290.68]  So anyway, welcome into Factorial Corner, apparently.
[1290.68 --> 1294.06]  It's like learning a new programming language or learning next or something.
[1294.14 --> 1295.70]  You have to throw out everything you already know.
[1296.02 --> 1298.56]  I could see the appeal here.
[1298.56 --> 1298.70]  Yeah.
[1298.84 --> 1301.16]  You know, it's not too far off.
[1301.42 --> 1301.78]  Yeah.
[1302.06 --> 1302.32]  Yeah.
[1302.38 --> 1302.60]  Okay.
[1302.70 --> 1305.30]  So it's like switching from Python to Go or something, you know.
[1305.32 --> 1313.16]  And it's like, okay, I know that the constructs are kind of the same and I can operate in a similar envelope here.
[1313.36 --> 1314.58]  But, huh?
[1315.04 --> 1315.88]  What's threading?
[1316.18 --> 1316.84]  Like, huh?
[1318.06 --> 1318.50]  Yeah.
[1318.76 --> 1319.02]  Okay.
[1319.02 --> 1325.74]  So anyway, coming back to the MacBook, I got the M4 Max with the nano texture display.
[1326.52 --> 1334.48]  And it's like the best matte display on a laptop, I think, that I've ever seen.
[1334.70 --> 1336.16]  It is superb.
[1337.10 --> 1338.98]  And did you say it's the 14-inch version, right?
[1339.20 --> 1340.08]  Yeah, the 14-inch.
[1340.26 --> 1341.30]  Oh, that's great.
[1341.40 --> 1342.64]  No, that's a perfect size.
[1343.04 --> 1347.30]  I have the 16-inch that Tailscale provided me to do all my editing on for work.
[1347.30 --> 1351.80]  And it's a chunky, heavy, big lunch tray of a laptop.
[1351.88 --> 1354.22]  That's what the good Lord invented external monitors for, Alex.
[1355.18 --> 1355.58]  Absolutely.
[1356.26 --> 1356.52]  Yeah.
[1356.52 --> 1361.00]  I think my next laptop has to be 14-inch screen just for the portability.
[1361.48 --> 1362.34]  Oh, I'm very jealous.
[1362.96 --> 1363.62]  It's small.
[1363.78 --> 1364.20]  It's light.
[1364.28 --> 1364.90]  It's wonderful.
[1365.12 --> 1370.44]  And it fits, I won't say in your pocket, but it fits in a backpack without having to, like, do any kind of gymnastics or anything.
[1371.00 --> 1375.06]  And it doesn't weigh a ton either, which is very nice when you travel as much as I do.
[1375.06 --> 1381.88]  But whenever I set up a new Mac, it's always a good chance to test out the Nix Darwin configurations.
[1382.22 --> 1394.44]  And it's so nice to clone your Git repo onto a fresh laptop, run the Nix Darwin rebuild command a couple of times, and you've got your dock icons exactly where you left them.
[1394.90 --> 1396.56]  All of the Brute apps are installed.
[1396.84 --> 1398.62]  All of the Mac App Store apps are installed.
[1398.82 --> 1399.74]  All you have to do is log in.
[1399.74 --> 1401.64]  That is really sweet.
[1401.80 --> 1402.88]  That is, wow.
[1404.10 --> 1407.70]  That makes it just, like, a super low effort, low cost to transition.
[1408.16 --> 1409.98]  I think I should probably do a video on it.
[1410.04 --> 1422.38]  Before I send my old Mac in for trading, by the way, if you want an M1 Max 14-inch MacBook Pro for a decent price, Apple are only giving me, like, $1,100 or something for this thing.
[1423.00 --> 1424.72]  Send me a message, and we'll work something out.
[1424.72 --> 1434.36]  But before I send that one in, I should probably make a video talking about my, like, Mac Nix setup, because it's really quite dialed in at this point.
[1434.42 --> 1441.56]  I've got it so that I can override on certain machines if a certain file is present to have a different dock layout.
[1441.76 --> 1446.90]  But if that file doesn't exist, then it will just do the default Darwin dock that I like.
[1447.40 --> 1452.34]  So, like, my recording machine has a custom layout, and then all of my other Macs are all the same.
[1452.34 --> 1452.90]  Yeah.
[1455.16 --> 1455.60]  Serenity.
[1456.06 --> 1458.02]  It's really, yeah, it's really nice.
[1459.46 --> 1463.04]  Now, when you're setting up a new machine, obviously you're doing a lot of logging in and that kind of stuff.
[1463.18 --> 1465.70]  And my Bitwarden password is kind of long.
[1466.26 --> 1469.82]  So I started looking for a text expander application.
[1470.62 --> 1473.70]  We're finally getting to the dev tooling corner part of the discussion.
[1474.82 --> 1476.54]  Oh, I thought we were talking about Factoria.
[1476.76 --> 1477.38]  Oh, yeah.
[1477.68 --> 1479.48]  Yeah, I've kind of digressed a little, haven't I?
[1479.56 --> 1480.28]  Oh, well.
[1480.28 --> 1483.56]  And I came across this tool called Snippity.
[1484.18 --> 1485.20]  Snippity.app.
[1485.84 --> 1486.10]  Okay.
[1486.66 --> 1495.86]  This is a tool that lets you, basically, it's not quite like text expander, which was kind of this magic, always listening to every keystroke.
[1495.86 --> 1505.02]  Like, we used to have it in the genius room at the Apple store where we would type a certain, like, RFR, for example, and it would expand it to ready for repair or something like that.
[1505.08 --> 1507.68]  Or RFP, ready for pickup or something like that.
[1507.68 --> 1512.76]  And then there were a bunch of, like, notes that we all had standardized across the team and stuff.
[1512.90 --> 1515.28]  Like, text expander was really great in that scenario.
[1515.38 --> 1523.06]  But here, I wanted to use it to do things like type in my master Bitwarden password.
[1523.06 --> 1529.80]  You know, I'm going to put it behind a secret incantation or something like that so that only I know really what the text expander thing is.
[1529.80 --> 1540.06]  And it has this lovely kind of, like, little shortcut menu where I can do Command Shift X and it brings up a few options system-wide for me to search through.
[1540.14 --> 1543.28]  Or I can do Command Shift Space and it lets me search the entire vault.
[1544.00 --> 1544.88]  It's really nice.
[1544.92 --> 1546.20]  And it syncs with iCloud too.
[1546.36 --> 1554.20]  Or you can sync it using SyncThing because it lets you just do a specific file if you want to, if you don't want to use iCloud, that kind of thing.
[1554.20 --> 1556.48]  Really nice app.
[1556.54 --> 1559.58]  It was about $30, I think, on the App Store.
[1559.72 --> 1561.66]  So not cheap by any means.
[1561.82 --> 1565.66]  But it's really quite a well-put-together application.
[1566.26 --> 1566.64]  All right.
[1566.78 --> 1568.20]  So snippety.app.
[1569.66 --> 1572.56]  It looks like it does a lot more than I would even need.
[1572.72 --> 1575.20]  But the expander stuff would be so handy.
[1576.72 --> 1578.04]  Oh, it's got a, okay, collaboration.
[1578.30 --> 1580.46]  Well, sync your settings to mine so I can just steal what you've done.
[1580.94 --> 1581.30]  Yeah.
[1581.30 --> 1583.72]  Well, maybe not because it hasn't.
[1583.94 --> 1584.30]  Never mind.
[1585.74 --> 1592.06]  But if you're doing the same, so I install TailScale and Docker in a lot of different places these days and a bunch of other stuff too,
[1592.26 --> 1598.30]  where I'm like always downloading or curling the same, feels like curling the same thing all the time.
[1599.22 --> 1602.04]  And so I've put it behind a text expander shortcut now.
[1602.50 --> 1609.22]  Literally, I do the Command Shift X tail and then, or it was it, it tail actually for install TailScale, it tail.
[1609.22 --> 1618.68]  And it literally curls, it puts it into the text box in front of you, curl tailscale.com, whatever, and pipes it to bash.
[1619.04 --> 1622.10]  And a minute later, TailScale's installed.
[1622.78 --> 1625.02]  That kind of feels like magic a little bit.
[1625.12 --> 1625.90]  It is a little bit.
[1626.46 --> 1628.48]  I could see using this for a lot of handy commands.
[1628.48 --> 1636.04]  It does make me have a little Mac FOMO sometimes because these apps are a great example of, like there's things that macOS just drive me crazy.
[1636.58 --> 1641.54]  But then there's so many great community apps that come along and some of them are pay and some of them are free.
[1641.78 --> 1643.60]  But they really fix a lot of this stuff.
[1643.68 --> 1644.48]  And this is an example of that.
[1644.48 --> 1650.80]  Now, Brent, I want to talk to you about your lovely, shiny new server.
[1651.04 --> 1657.24]  We've been threatening, or you've been threatening, to build this bloody thing, I think as long as I've known you.
[1657.72 --> 1659.98]  Is that, yeah, that's likely accurate.
[1659.98 --> 1667.58]  It's probably one of the reasons we became friends because I've been trying to just, like, pry out the knowledge from that little head of yours and how I should go about doing this.
[1667.58 --> 1672.48]  Which has evolved in the last five, six years, something like that.
[1673.54 --> 1687.16]  I think, yeah, as a little update, I was just remembering exactly a year ago I bought a whole bunch of hard drives with the, you know, grand vision of creating sort of two sister servers.
[1687.16 --> 1693.66]  One that would exist at my parents' place, one that would exist at my place that I could sort of mirror data back and forth.
[1693.66 --> 1700.80]  Somehow a year went by and those drives were just never really put to good use.
[1701.52 --> 1706.56]  But I finally did something about it with the help of Wes and Chris.
[1706.76 --> 1712.74]  We got together one, I think, one day last week to try to solve an unrelated problem.
[1712.90 --> 1713.70]  And that wasn't working.
[1713.78 --> 1715.88]  We're like, okay, well, let's build Brent's NAS.
[1716.14 --> 1720.84]  And I had just so happened to build the hardware that morning.
[1720.84 --> 1726.06]  So we took advantage of some time together and built me a thing.
[1726.34 --> 1729.64]  And it's a thing that I've been wanting for a great long time.
[1729.70 --> 1744.40]  And there's been, as you've heard on this show, a great number of, you know, Franken builds trying to get towards this idea of just really just having a stable NAS that wasn't like a laptop with a squid of hard drives.
[1744.88 --> 1749.28]  And I feel like for the very first time, I might just be there.
[1749.28 --> 1750.66]  All right.
[1750.74 --> 1752.46]  So what were the goals for this project?
[1753.04 --> 1755.30]  Removing the squid of hard drives.
[1755.56 --> 1755.84]  Check.
[1756.00 --> 1756.58]  Sounds like.
[1757.16 --> 1757.56]  Yes.
[1757.86 --> 1758.50]  So far.
[1758.62 --> 1761.32]  Well, I'll have to plug them back in to grab the data off them at some point.
[1761.70 --> 1764.50]  Wouldn't it really be more like an octopus of hard drives?
[1765.90 --> 1767.12]  Write in and let us know.
[1767.12 --> 1767.56]  Yeah.
[1767.56 --> 1767.68]  Yeah.
[1769.68 --> 1783.70]  The idea of just having a box that's super stable and that isn't delicate to the point of, you know, someone coming by and unplugging a thing was really the idea.
[1783.96 --> 1785.76]  When I say someone, I also mean cats.
[1785.76 --> 1798.48]  But the idea of just having a box that's super stable and appliance that's really reliable is was the main goal and having hard drives that I could trust as well, because I've had many, many hard drives over the years.
[1798.48 --> 1801.82]  Being a photographer with tons and tons of data on them.
[1802.48 --> 1814.36]  But they've never really been in one cohesive machine for more than, I don't know, six plus months of being stable.
[1815.02 --> 1817.26]  You know, you should never trust a hard drive, right?
[1817.80 --> 1818.50]  Well, you've.
[1818.78 --> 1818.88]  Yeah.
[1818.90 --> 1819.94]  You taught me that a while ago.
[1820.20 --> 1821.24]  That's why I have more than.
[1821.76 --> 1821.94]  Yes.
[1822.04 --> 1822.70]  More than I need.
[1822.78 --> 1823.02]  Maybe.
[1823.02 --> 1826.32]  I'm just paying it forward from our good friends, Alan and Jim.
[1826.58 --> 1829.38]  You know, they're always talking about how hard drives are about to eat your face.
[1832.38 --> 1832.78]  Yeah.
[1832.84 --> 1835.02]  Maybe I should duplicate my data somewhere first.
[1836.28 --> 1837.68]  But I don't know.
[1837.72 --> 1847.24]  There's I think with a lot of self hosting, at least from my experience, a lot of it also has to do with just feeling good about what you built.
[1847.24 --> 1855.14]  And a lot of what I built previously felt exciting, but didn't feel like it had that stable aspect of it, you know.
[1855.64 --> 1857.88]  And I know that's a completely emotional thing.
[1857.94 --> 1862.40]  And it worked for the most part to get me to where I am today.
[1863.00 --> 1869.30]  But it never felt like it was a long lasting solution, both from hardware and software perspective.
[1869.86 --> 1871.86]  But I think I think I might be there now.
[1871.86 --> 1877.44]  We talked about this right at the very beginning of this show with Wendor talking about craftsmanship.
[1877.82 --> 1887.36]  And this is an angle that I'm really beginning to appreciate the longer I do self hosting is that you make deliberate decisions to replace certain services.
[1887.36 --> 1891.46]  In your case, I'm assuming there's Nextcloud running on this thing, for example.
[1891.46 --> 1904.66]  And over time, you start to assemble piece by piece this solution that removes your reliance on the cloud, for one of a better example.
[1905.52 --> 1913.22]  Because you not only are replacing the service, but also learning how and why you want to do those things.
[1913.22 --> 1920.34]  There's certainly been several examples where I've replaced, I can't think of one off my head, but where I've replaced the service in the cloud.
[1920.46 --> 1924.34]  And then a few months later, I'm like, oh, I've gone back to the cloud.
[1924.40 --> 1926.04]  I've stopped using the self hosted version.
[1926.36 --> 1929.48]  I guess that's not that important to me for this particular thing.
[1930.10 --> 1934.72]  So does education play a big factor for you as well as the ethical side?
[1935.36 --> 1939.90]  Yeah, I think I am a long, like basically a lifestyle learner.
[1939.90 --> 1944.58]  I just, one of my best, most favorite pastimes is learning things, especially related to tech.
[1945.96 --> 1952.22]  And that was part of the problem with the previous incantations of this solution was that I was also using it as a learning platform.
[1952.80 --> 1955.94]  So, you know, you go in there and you install a bunch of stuff.
[1956.04 --> 1961.22]  And all of a sudden, the thing you were hoping was really reliable and like an appliance is all crufty.
[1961.38 --> 1965.86]  And you've gone ahead and broken all the things that were stable, you know, last week.
[1965.86 --> 1967.48]  That sounds like a pretty average Tuesday to me.
[1967.48 --> 1972.98]  Well, I think the key now is I'm in a place to be able to have a couple devices, you know,
[1973.04 --> 1979.90]  and I've got some smaller devices or some older devices that I don't mind for them to be the test device.
[1980.78 --> 1989.54]  And for one machine to be the untouchable, let's say, you know, have it be super stable and not do any tinkering.
[1989.72 --> 1990.98]  It's like a no tinker zone.
[1991.62 --> 1993.74]  But we'll see if I stick to that.
[1994.02 --> 1996.16]  So what does the hardware in this thing look like then?
[1996.16 --> 2002.42]  Well, you might recognize this hardware, Alex, because you worked real hard to get it over the border here to Canada.
[2002.70 --> 2005.02]  I purchased your old server components.
[2005.18 --> 2007.34]  So I think you might know these parts better than I do.
[2007.82 --> 2008.08]  Maybe.
[2008.30 --> 2011.72]  It's the ASRock Rack E3C246D4U.
[2012.08 --> 2013.20]  Rolls right off the tongue, doesn't it?
[2015.38 --> 2018.62]  Yeah, these, from what I understand, were in your old server.
[2019.02 --> 2024.44]  And they've got sort of a, what, second life versus third life here in my cabin in the woods?
[2024.44 --> 2026.24]  It would be a second life, yeah.
[2026.38 --> 2031.26]  So it's based around the Intel 8th Gen i5-8500 venerable CPU.
[2032.10 --> 2035.18]  Was there a reason that attracted you to such a platform?
[2035.72 --> 2036.88]  I've got to be totally honest here.
[2036.96 --> 2039.36]  So I've, like I mentioned, the squid previously.
[2039.66 --> 2044.42]  I've just taken whatever hardware I've had around that wasn't in use and put it to this purpose.
[2044.42 --> 2056.28]  But I figured I have surprisingly bad luck with hardware, both with compatibility and frying, like, some motherboards by doing things I probably shouldn't have done.
[2056.70 --> 2060.40]  So I just decided to trust Uncle Alex.
[2060.44 --> 2062.66]  Embrace the Alex endorsement, right?
[2062.66 --> 2062.92]  Mm-hmm.
[2063.22 --> 2078.80]  And so when you said, oh, I got these parts for sale, I was like, if I could just take the tried and tested and true components that you've been running, that I, you know, I trust your building capabilities, then I jumped right on that.
[2079.44 --> 2080.12]  Oh, well.
[2080.12 --> 2091.84]  Because to be honest, I was, as you know, because I have mentioned this to you very many times, I have gone digging myself to find the right components and the right cases and all this stuff, and it just can become a rabbit hole.
[2092.56 --> 2097.52]  So I feel super fortunate that I can reach out to someone like you and just say, hey, what should I build?
[2097.58 --> 2102.88]  And you give me, you know, the grocery list and part of the groceries were in your house this time around.
[2102.88 --> 2118.30]  Well, listeners might remember from previous self-hosteds that I ended up purchasing four 20-terabyte Western Digital Reds with the idea of raiding them like a RAID 1 in pairs.
[2118.30 --> 2131.56]  So two of these disks, I'm hoping I can build another sister machine that will end up 3,500 kilometers away at my parents' place to serve as their sort of stable server as well.
[2131.56 --> 2141.80]  So the idea is to have two super stable servers that are built as close to identical as possible that I can replicate data back and forth.
[2142.22 --> 2143.64]  And so how are you planning on doing that?
[2143.74 --> 2145.36]  Are you using ZFS?
[2147.98 --> 2157.66]  I knew you would ask this question and I would have to let you know that I did not choose your darling ZFS.
[2158.10 --> 2159.40]  Oh, you madman.
[2159.90 --> 2161.34]  Chris and Wes got to me.
[2161.56 --> 2163.94]  Don't blame me.
[2164.52 --> 2165.62]  Don't blame me.
[2165.66 --> 2168.60]  No, Chris and Wes did suggest that I go the ZFS route.
[2168.76 --> 2175.62]  And we had probably a 30, 20 to 30 minute discussion about like the pros and cons of each.
[2176.18 --> 2178.04]  And it can be a hard decision.
[2178.26 --> 2181.42]  So I ended up wanting to go with ButterFS.
[2181.42 --> 2190.90]  And part of the reason is I don't think I will be doing extremely fancy like enterprise type things.
[2190.90 --> 2194.22]  And I also don't need those skills for my employability.
[2194.40 --> 2195.40]  So that was one factor.
[2195.52 --> 2202.38]  But also, and this was the biggest one for me, I wanted to have Linux native technologies on these machines as much as possible.
[2202.38 --> 2203.52]  What do you mean?
[2203.84 --> 2206.10]  Open ZFS is Linux native these days.
[2206.50 --> 2208.40]  Do you mean more license compatible?
[2208.40 --> 2219.92]  I mean that you don't have to install like a DKMS module or like make sure you have the right kernel for things to work properly and that it's, you know, comes out of the box in every single.
[2219.92 --> 2220.98]  So which OS are you running?
[2221.22 --> 2223.50]  You know, Nix OS, of course.
[2223.50 --> 2226.08]  So there's no DKMS with Nix.
[2226.84 --> 2228.22]  It's just a couple of lines to config.
[2228.84 --> 2229.04]  Yeah.
[2229.46 --> 2229.68]  Right?
[2229.76 --> 2231.34]  Someone else has already built the kernel for you.
[2231.40 --> 2234.06]  It's sitting in the binary cache like just waiting for you.
[2234.08 --> 2234.64]  It's true, Chris.
[2235.16 --> 2235.88]  Help me out here.
[2236.58 --> 2237.38]  No, it's true.
[2237.84 --> 2238.06]  Yep.
[2238.62 --> 2244.16]  I think Nix is probably one of the safest distributions out there to use ZFS.
[2244.82 --> 2252.86]  I think one of the things that came up in our conversation that we did have around the native tooling aspect was, and it's good and bad.
[2252.86 --> 2255.04]  And I think it just depends on your preference.
[2255.26 --> 2258.26]  So ZFS is an entire suite of tooling, right?
[2258.32 --> 2261.22]  You have Zpool and you have all of the ZFS commands.
[2261.98 --> 2269.74]  ButterFS, with a few exceptions, is really using all of the standard Linux tools that you use to manage any other file system on a Linux box.
[2270.36 --> 2278.10]  And so it's kind of handy if you already know that tooling from other distributions like, you know, like he runs ButterFS on his laptop too.
[2278.78 --> 2280.48]  Then you just continue to use those same tools.
[2280.52 --> 2281.80]  You don't have to learn a separate set.
[2281.80 --> 2282.62]  I don't know.
[2282.62 --> 2285.62]  I don't think it's so bad because I think the ZFS tools are actually really great.
[2285.90 --> 2288.16]  So I don't think it's necessarily a bad thing to learn that.
[2288.44 --> 2289.74]  But there's just something to consider.
[2290.60 --> 2294.44]  It'd be the same thing like when BcacheFS is stable and finally shipping.
[2294.62 --> 2301.64]  It's probably going to make a really great HomeLab file system for people that are looking for something a little leaner and meaner than ZFS.
[2301.64 --> 2312.02]  But it'll, again, in the same situation, it's going to be using, you know, MakeFS and it's going to be using the tooling built into Linux that you use to manage all the file systems that just come built into the kernel.
[2312.52 --> 2314.26]  And there's pros and cons to that, I think.
[2314.26 --> 2319.38]  I think there's also some positive past experiences that played into this decision.
[2319.38 --> 2328.36]  Like I've had ButterFS on route running my tumbleweed machine here that I usually use for podcasting.
[2328.46 --> 2330.98]  We, well, we ended up the next day wiping that too.
[2331.30 --> 2333.66]  But that's a different story that you can catch in the links I'm plugged.
[2333.66 --> 2338.66]  And so I felt like I had already positive experiences with ButterFS.
[2339.14 --> 2352.64]  And also if I was going to run ButterFS on route on my everyday machines, it sure would be helpful to be able to do file system native backups as well.
[2352.90 --> 2355.14]  Using like ButterFS and those kind of things.
[2355.24 --> 2360.76]  I know I can run ZFS on route as well, but that feels a little bit more experimental to me.
[2360.76 --> 2365.04]  Maybe I'm wrong, but I think emotions play into that decision too.
[2366.14 --> 2368.58]  Do you feel like you're pushing water uphill with this decision?
[2368.80 --> 2376.00]  I can sense some kind of a, not shame, like you even said it, like I'm going to have to admit it to you that I'm not using ZFS.
[2376.24 --> 2377.52]  Like why do you feel that way?
[2378.04 --> 2388.36]  Only because I know you love ZFS so much and you would certainly suggest that as the way to go because it's in your toolbox.
[2388.36 --> 2393.82]  Mostly because I've been brainwashed by one of your fellow Canadians for many, many years, I think.
[2395.52 --> 2396.80]  Are you saying it's my fault?
[2397.28 --> 2399.00]  No, no, Alan Jude, of course.
[2399.60 --> 2403.52]  You know, it's just like technically a very, very complete solution.
[2403.74 --> 2407.56]  So honestly, you know, it's not my data that you're going to lose.
[2407.56 --> 2410.60]  It's, you know, you're going to be a guinea pig for us all, Brent.
[2410.70 --> 2420.46]  And I'm actually really kind of interested to hear how you find the ButterFS tooling, particularly for cross-continental replications, I assume over tail scale.
[2421.22 --> 2423.22]  Or some other means, of course, is available.
[2423.42 --> 2424.48]  Other VPNs are available.
[2425.42 --> 2429.00]  It's, for me, it's, you're just like the canary in the coal mine.
[2429.00 --> 2432.00]  And you're doing us all a public service, so.
[2432.66 --> 2433.50]  Oh, man.
[2433.66 --> 2434.04]  I guess.
[2434.70 --> 2435.46]  Yeah, I don't know.
[2435.48 --> 2436.70]  Check in and let us know how it goes.
[2436.96 --> 2437.98]  Oh, gosh.
[2438.36 --> 2438.92]  No, no.
[2438.94 --> 2439.38]  Save me.
[2440.20 --> 2445.84]  You know, as somebody who, I ran ButterFS when it first came out and I lost data.
[2446.24 --> 2451.14]  And also had a system that couldn't boot because of ButterFS at one point.
[2451.22 --> 2454.94]  It was kind of Ubuntu's fault, but it was also because I was using ButterFS.
[2454.94 --> 2462.76]  It was like, you know, 50-50 as somebody who's lost data and lost a bootable system to ButterFS back in the bad old days.
[2463.24 --> 2468.18]  I'll attest to the fact that, you know, a lot of work from Seuss and from Facebook.
[2468.62 --> 2475.90]  Facebook hired several core developers many years ago now, and they've just been cranking out fantastic code.
[2476.24 --> 2479.56]  So it is a pretty solid file system now.
[2479.56 --> 2487.62]  I think there's a real fine line, though, between, like, when you use ButterFS or ZFS for long-term data storage.
[2488.60 --> 2492.82]  And that's why, I mean, we seriously debated that the longest of all of the decisions we made.
[2492.88 --> 2495.40]  Like Jellyfin, that was about a three-second decision.
[2496.12 --> 2500.92]  But ButterFS versus ZFS was maybe even longer than a half hour.
[2501.68 --> 2505.66]  But ultimately, it did come down to, like, the laptop runs it and its NAS runs it.
[2505.66 --> 2512.68]  But I've had pretty good luck with mine, you know, now that I realize my Odroid, because it's just a teeny little Odroid.
[2513.52 --> 2516.94]  I'm using ButterFS in a really irresponsible way, too.
[2517.04 --> 2519.98]  Just absolutely bonkers way that nobody should do.
[2520.00 --> 2521.32]  So I'm not even going to mention how I do it.
[2521.40 --> 2523.78]  But it's been running for about three and a half years now.
[2525.90 --> 2526.68]  It's ridiculous.
[2526.68 --> 2531.54]  Well, I would love to know from those listening, have I made the biggest mistake ever here?
[2532.50 --> 2536.60]  I think maybe at least one of you currently on microphone thinks maybe I have.
[2536.84 --> 2538.24]  But we'll see in time.
[2540.18 --> 2542.42]  Tailscale.com slash self-hosted.
[2542.46 --> 2545.32]  Go try it out for free on 100 devices and three users.
[2545.74 --> 2546.86]  Not a limited-time deal.
[2546.90 --> 2548.26]  It's the plan I'm on since the beginning.
[2548.68 --> 2550.92]  It's a great way to support the show and try it out.
[2551.12 --> 2554.22]  Then you can play around with their enterprise features if that suits you as well.
[2554.22 --> 2557.16]  It's tailscale.com slash self-hosted.
[2557.28 --> 2562.32]  It is the easiest way to connect devices and services to each other wherever they are.
[2562.70 --> 2567.56]  And you're probably thinking of Tailscale like a VPN, but it's so much beyond that.
[2567.74 --> 2571.96]  It is a secure remote access system that is also a mesh VPN.
[2572.22 --> 2574.24]  It is also my LAN.
[2574.50 --> 2576.66]  It is also programmable networking.
[2577.10 --> 2579.52]  And it is also very easy to deploy.
[2580.44 --> 2581.14]  Zero config.
[2581.20 --> 2582.74]  You'll get it set up in just minutes.
[2582.74 --> 2590.32]  What I love as a self-hoster about Tailscale is that I can deploy applications and services just to play around, experiment with them.
[2590.86 --> 2596.60]  I don't have to worry about the security, but yet I can still get access and get the same services wherever I go.
[2597.16 --> 2599.50]  And I use DNS resolution on my tail net.
[2599.76 --> 2603.30]  So I just access everything by name from every system I own.
[2603.52 --> 2606.00]  And, guys, I own way too many systems.
[2606.14 --> 2606.78]  It's ridiculous.
[2606.78 --> 2613.96]  And it's so nice that the – well, I'm an old man, but the bookmarks that I have for, like, whatever it might be just work wherever I am.
[2614.74 --> 2615.46]  Everything's the same.
[2615.52 --> 2620.62]  If I'm at work, if I'm on my phone, if I'm at home, if I'm at a friend's house, it all just works.
[2620.62 --> 2625.20]  Because I have a mesh network that is powered by WireGuard.
[2625.84 --> 2627.08]  Everything's on that tail net.
[2627.26 --> 2632.02]  And it creates essentially what to me is perceived as a flat network, very simple.
[2632.48 --> 2634.92]  But you can do it over complex infrastructure.
[2635.74 --> 2637.44]  Some of my nodes are on VPSs.
[2637.76 --> 2641.80]  Some of them are VMs running behind a NAT on a machine.
[2642.34 --> 2643.76]  Some of them are mobile devices.
[2643.86 --> 2645.10]  Some of them are Raspberry Pis.
[2645.10 --> 2647.10]  Some of them are containers.
[2647.86 --> 2650.56]  And just the application container is on the tail net directly.
[2651.60 --> 2657.60]  And all of that is represented in a flat network that is easy to understand, easy to set up.
[2657.68 --> 2659.80]  And then I have all kinds of options like sharing.
[2660.26 --> 2664.14]  I can do ACLs to securely control access to devices and services.
[2664.50 --> 2667.26]  I can tie it in with my existing authentication infrastructure.
[2667.26 --> 2674.64]  So everybody that has a Jupyter broadcasting account with our authentication provider also gets access to the tail net.
[2674.64 --> 2677.50]  And I can set their permissions and what they can and can't get access to.
[2678.14 --> 2679.32]  It's really powerful.
[2679.72 --> 2680.64]  You've got to try it out.
[2680.68 --> 2685.04]  Because it absolutely fundamentally changes the self-hosting Homelab game.
[2685.56 --> 2686.14]  So try it out.
[2686.24 --> 2686.80]  Support the show.
[2686.88 --> 2688.32]  And get it for free up to 100 devices.
[2688.44 --> 2689.44]  Not a limited time trial.
[2690.02 --> 2692.76]  It's tailscale.com slash self-hosted.
[2692.82 --> 2695.58]  That's tailscale.com slash self-hosted.
[2695.58 --> 2706.44]  So one of the things that shiny new server of yours does, Brent, that it does really well, actually, is video transcoding using the QuickSync video encoder.
[2706.52 --> 2708.86]  Are you doing much video encoding at all?
[2709.20 --> 2710.34]  I hope to.
[2711.28 --> 2716.88]  I will admit I've had issues getting the QuickSync and all of that set up properly.
[2716.98 --> 2718.36]  So maybe we need a little session together.
[2718.58 --> 2720.04]  But yes, that's the hope.
[2720.04 --> 2723.54]  Because you're running Jellyfin as a Nix module, right?
[2724.32 --> 2724.72]  Yes, sir.
[2725.54 --> 2729.10]  So yeah, probably just, I don't know, user permissions for the QuickSync device.
[2729.74 --> 2737.26]  But anyway, I've got this dream that one day we're going to be able to just have QuickSync video encoders somewhere on the network.
[2737.66 --> 2740.46]  And run Jellyfin on this super low power device.
[2740.58 --> 2743.14]  I don't know, like something super basic like a Raspberry Pi.
[2743.14 --> 2748.42]  And that's going to be enough to do the front end and maybe even some of the server side processing too.
[2748.70 --> 2752.42]  But the actual video encoding gets distributed across the network.
[2753.18 --> 2754.42]  Are you with me on this?
[2755.06 --> 2756.38]  Well, ho, ho, ho, Alex.
[2756.58 --> 2759.86]  It's Christmas in November because I got a gift for you.
[2759.94 --> 2760.68]  I thought you might.
[2761.40 --> 2766.20]  Now, it's not actually affiliated with the Handbrake project, but it's called Handbrake Web.
[2766.20 --> 2777.30]  And it is a self-hostable platform that gives you a headless handbrake web front end that does distributed transcoding.
[2777.56 --> 2783.00]  You can leverage multiple devices and send out transcoding jobs as workers to them.
[2783.06 --> 2785.14]  Or you can all have it running on one box.
[2785.30 --> 2789.80]  It gives you a web interface to manage all of this and to create transcode queues.
[2789.86 --> 2793.96]  So you could actually like maybe you're going on a trip and you want to transcode something to a smaller format.
[2793.96 --> 2802.24]  You could stack up many, many, many multiple videos and then have it dispatch those videos throughout your network to transcode them or do it all in one big box.
[2802.66 --> 2805.42]  And they're working on adding a preset creation.
[2805.72 --> 2806.54]  They have some built in.
[2806.74 --> 2812.42]  But what I think is pretty neat is you can just launch the Handbrake desktop app, which is a great app.
[2812.66 --> 2817.82]  You can set all the settings you want, export that as a JSON preset, and then upload it right into Handbrake Web.
[2818.14 --> 2818.84]  Bob's your uncle.
[2818.84 --> 2825.44]  It brings all of those presets in and does that exact encoding because it's using Handbrake CLI under the hood.
[2825.64 --> 2827.26]  And it's slick.
[2827.40 --> 2829.20]  It does right now directory monitoring.
[2829.40 --> 2833.70]  So I've created a directory that's on a Samba share and also, of course, over SFTP.
[2834.06 --> 2837.10]  You just drop the job in there and it's off to the races.
[2837.28 --> 2839.62]  So like a network share works really well in this case.
[2839.82 --> 2840.36]  Oh, nice.
[2840.44 --> 2841.48]  They have other kinds of features.
[2841.48 --> 2844.42]  They're going to add like, you know, user accounts and other things.
[2844.42 --> 2847.14]  But it's for what you need right now for that kind of stuff.
[2847.18 --> 2847.72]  It's great.
[2848.46 --> 2849.98]  So you could literally just have a network.
[2850.72 --> 2855.84]  You know, I use the word Dropbox, but you literally just drop a video file into a directory.
[2856.12 --> 2861.62]  And then a few minutes later, it spits out something with a predetermined codec.
[2861.62 --> 2862.74]  Oh, man.
[2862.88 --> 2863.10]  Yeah.
[2863.18 --> 2864.86]  And I would have used this so much.
[2865.00 --> 2871.42]  Back in the day, we were manually encoding like an HD version and a mobile version and a tiny version.
[2871.54 --> 2876.54]  We would create three different versions of the video file because that's just kind of how the distribution worked back in the day.
[2877.16 --> 2880.94]  And how great would it be to just assign a different PC to each job?
[2881.06 --> 2883.02]  So they're all three simultaneously running.
[2883.02 --> 2886.70]  And then it just spits them back out in wherever you've defined the output to go.
[2887.08 --> 2887.34]  Oh, yeah.
[2887.98 --> 2890.20]  One machine has a proper NVIDIA GPU in it.
[2890.20 --> 2891.66]  So that does the 4K one.
[2892.06 --> 2892.38]  Yeah.
[2892.66 --> 2893.52]  Yeah, that would be nice.
[2893.72 --> 2894.00]  Tasty.
[2894.82 --> 2899.52]  I mean, I think the fact that you have to create the presets externally, it comes with the default handbrake ones.
[2899.74 --> 2906.56]  But if you want to create them externally, like the author of the project seems to think like that's a big missing feature and that they want to add like a preset creator in there.
[2906.94 --> 2912.28]  But you could, I could in theory, like I could say, oh, Alex, I just think this is the best video encoding preset.
[2912.40 --> 2914.50]  And I could send you the JSON file and you could import it.
[2914.62 --> 2916.22]  And now you're just doing your encodes to that spec.
[2916.56 --> 2919.02]  I don't know much about video encoding, if I'm honest.
[2919.02 --> 2925.80]  But like YouTube does a terrible job because you see all the compression artifacts in YouTube all the time.
[2925.94 --> 2929.04]  Like I know that looks bad compared to what I see in my editor.
[2929.24 --> 2932.06]  But like why it looks bad, I couldn't tell you.
[2932.34 --> 2932.36]  So.
[2932.56 --> 2934.72]  Yeah, they really, they really munch it, don't they?
[2935.14 --> 2940.84]  Could we just have like a directory of community sourced, like a repo of like presets?
[2940.84 --> 2941.12]  Presets?
[2941.66 --> 2942.82]  Yeah, that'd be interesting.
[2943.06 --> 2946.84]  Kind of like a Docker hub of presets for handbrake?
[2947.00 --> 2947.42]  Yeah.
[2947.42 --> 2947.70]  Yeah.
[2947.70 --> 2948.30]  Yeah.
[2948.30 --> 2953.40]  Or like a, or like a GitHub list of something of great handbrake presets.
[2953.60 --> 2956.48]  You know, one for like mobile travel, you're watching on a tablet.
[2957.22 --> 2966.00]  I tend to like to, to not really re-encode my videos if possible, but there are times where I've needed to do like before a trip, a batch encoding or, you know, content.
[2966.00 --> 2976.32]  Like I was thinking for JB, maybe this is something that can be useful as part of our backend, but then this front end aspect of it is available for the crew for one-off encodes.
[2977.28 --> 2977.74]  I mean, why not?
[2978.22 --> 2979.98]  Yeah, that would be, that would be really nice.
[2980.42 --> 2993.12]  Have you seen those videos on YouTube where people take like an old VHS tape and they record a VHS into a VHS and then do it back there and 20 times later they show you the end result and it's just complete compressed garbage.
[2993.30 --> 2994.38]  It's just, just terrible.
[2994.70 --> 2995.28]  Oh yeah.
[2995.28 --> 2995.34]  Yeah.
[2995.68 --> 3001.04]  Have you seen the Marquez video where he like uploads his YouTube video like a hundred times or 200 times?
[3001.26 --> 3001.46]  Oh yeah.
[3001.92 --> 3002.80]  Same thing, right?
[3003.60 --> 3005.06]  The YouTube encoding is real bad.
[3005.18 --> 3005.62]  It's real bad.
[3005.68 --> 3015.78]  But yeah, if anybody has anything else out there like this distributed network encoding or like a hosted video encoding app with some nice presets for travel and whatnot, boost it in, please.
[3015.92 --> 3019.68]  Because right now I'm thinking this is it, but the space could be better.
[3019.88 --> 3021.94]  Maybe there's more things out there and I'd love to know.
[3022.94 --> 3024.38]  Speaking of boosts,
[3024.38 --> 3027.70]  We have some great boosts to get into.
[3028.14 --> 3038.10]  And our first one came in from Wine Eagle who sent in a big old baller boost, a row of sticks, 111,101 sats.
[3038.10 --> 3043.20]  And he sent us an email, which I believe we read because I went through the inbox and read all the emails.
[3043.86 --> 3047.32]  So thank you very much for that, Wine Eagle.
[3047.70 --> 3050.42]  Coming over from this week in Bitcoin to the self-hosted podcast.
[3050.66 --> 3051.50]  It's nice to have you.
[3052.16 --> 3052.96]  Thank you very much.
[3052.96 --> 3058.42]  Anonymous boosted in 55,555 sats.
[3060.56 --> 3063.18]  That's not something special around these parts, no.
[3063.78 --> 3066.36]  I mean, it feels like it does have meaning, don't you think?
[3066.66 --> 3067.74]  I just don't know if I know what it is.
[3068.02 --> 3068.50]  High fives.
[3068.62 --> 3069.12]  Oh, there it is.
[3069.72 --> 3073.56]  High fives to you all from a long time listener.
[3074.14 --> 3076.42]  Started with the Linux Action Show way back when.
[3076.48 --> 3076.68]  Yeah.
[3076.68 --> 3080.30]  And this listener finally got Albie all set up.
[3080.52 --> 3083.18]  So thank you for all you do, the JB crew.
[3084.00 --> 3084.78]  That rhymes.
[3084.90 --> 3085.54]  That's awesome.
[3085.66 --> 3086.14]  Thank you, Anonymous.
[3086.30 --> 3092.66]  You know, I've been seeing a nice uptick of people getting their self-hosted Albie Hub setups and trying this out.
[3092.76 --> 3093.60]  I mean, why not, right?
[3093.78 --> 3094.54]  It's pretty cool.
[3095.50 --> 3097.70]  Support one of your favorite podcasts with a whole self-hosted setup.
[3098.20 --> 3100.54]  I started with last two back in the good old days.
[3101.16 --> 3102.72]  Wow, you're making me feel old, Alex.
[3102.72 --> 3104.22]  Me too, me too.
[3104.28 --> 3108.46]  That was one of the first Linux things I ever took in to learn Linux.
[3108.56 --> 3109.20]  So thank you.
[3109.40 --> 3109.60]  Wow.
[3109.84 --> 3110.06]  Wow.
[3110.28 --> 3110.60]  Wow, wow.
[3111.14 --> 3113.84]  Ginkgo Salad comes in with 10,000 sats.
[3114.60 --> 3118.72]  My Nextcloud instance turned 12 years old this year.
[3118.94 --> 3120.40]  I never had many issues with it.
[3120.72 --> 3125.24]  One time, I moved more of its features to specialized apps like Logset and Image,
[3125.40 --> 3130.12]  but I don't think I would have found those apps had those features not been available in Nextcloud in the first place.
[3130.12 --> 3134.60]  Also, the Nextcloud Android app has never complained about being out of sync with the server.
[3135.22 --> 3136.06]  Thanks, Nextcloud.
[3136.58 --> 3137.26]  Looking at you, Image.
[3138.04 --> 3139.24]  Well, that's a nice report.
[3139.58 --> 3141.08]  Yeah, Image does love to do that.
[3141.18 --> 3144.00]  They release updates all the time.
[3144.32 --> 3144.62]  Yes.
[3144.72 --> 3150.52]  And then unless, well, the phone updates because it's through the Apple App Store or Google Play Store or whatever.
[3150.52 --> 3156.32]  And then you load it up and it goes, hey, by the way, did you know your server is 0.1 versions?
[3156.54 --> 3158.60]  I'm like, yeah, I don't care.
[3158.80 --> 3159.24]  Please.
[3159.68 --> 3160.02]  Can we just...
[3160.02 --> 3161.66]  Remember, we're not allowed to complain about that.
[3161.72 --> 3164.46]  Remember how much trouble I got in when we complained about that last time?
[3164.80 --> 3165.14]  Yeah.
[3165.48 --> 3165.88]  Yeah.
[3166.14 --> 3166.36]  Hmm.
[3166.86 --> 3167.40]  But you're right.
[3167.46 --> 3168.08]  It is a thing.
[3168.08 --> 3172.86]  And, you know, people would write in, well, then you should use such and such to auto-update your image container.
[3173.04 --> 3176.06]  But every now and then there's a breaking change, so I want to do it manually.
[3177.12 --> 3177.98]  It is a thing.
[3178.08 --> 3179.26]  I still love the project.
[3180.74 --> 3181.78]  But it's a thing.
[3181.96 --> 3182.42]  It's a thing.
[3182.92 --> 3187.90]  It's a good job we got Brent on this episode, you know, talking about Nextcloud being 12 years old.
[3188.72 --> 3189.26]  Yeah, wow.
[3189.72 --> 3190.92]  That's a long install.
[3190.92 --> 3196.48]  Our Nextboost, not exactly a Nextcloud win, so I'll read it.
[3196.56 --> 3199.68]  It's 18,345 sats by Vamax.
[3199.94 --> 3206.48]  I've had Chris's issue with Nextcloud locking down after being recreated due to one of my phone clients trying to log in.
[3206.80 --> 3206.92]  Yeah.
[3207.86 --> 3208.90]  I didn't even think about it.
[3209.28 --> 3211.22]  Then my Android would be sitting there trying to knock on the door all night.
[3212.02 --> 3217.80]  I have to uninstall the Nextcloud app and clear all of its data, which persists between installs, for reasons I do not understand.
[3217.80 --> 3224.30]  Also, regarding NVIDIA on Linux, I think this is the strongest case for Ubuntu here, especially for gaming like Alex was talking about.
[3224.74 --> 3232.82]  I have a 3080 running plane on Ubuntu, and while I did have the issues Alex is describing on Ubuntu 20, I haven't since.
[3233.26 --> 3235.86]  I installed the proprietary drivers through the software center.
[3235.96 --> 3236.72]  I know, it's boring.
[3237.14 --> 3239.04]  I'm the most recent version of Ubuntu every year.
[3239.44 --> 3240.74]  Just haven't had a problem since.
[3241.18 --> 3246.60]  Fresh installs have gone flawlessly, and any game in ProtonDB that's of gold or higher just works perfectly.
[3246.60 --> 3246.96]  Absolutely.
[3247.04 --> 3254.36]  Fedora, Arch, Nix, they all can work, but when it's 630 on a Tuesday and you just want to play a game with your friends, you reach for that Ubuntu.
[3256.16 --> 3259.08]  I mean, yeah, if it's a good experience, it's a good experience.
[3259.26 --> 3264.04]  I think the distros in general are getting better about the NVIDIA driver.
[3264.20 --> 3266.68]  Like Fedora, it's like a one-click install now, right?
[3266.68 --> 3272.98]  And with Nix, you just put it in the config once, and it always makes sure it builds with the proper NVIDIA driver.
[3273.38 --> 3276.28]  And then, like you say, Ubuntu, they got the one-click there in the App Store.
[3276.42 --> 3281.26]  Like the Ubuntu probably has the peak experience when it comes to gaming, I will admit.
[3281.36 --> 3284.34]  But the NVIDIA experience overall is getting really good.
[3285.22 --> 3286.02]  What about Pop! OS?
[3286.50 --> 3287.88]  Is that on an Ubuntu base?
[3288.26 --> 3288.48]  Yeah.
[3289.08 --> 3289.24]  Yeah.
[3290.12 --> 3291.18]  Yeah, I think that's pretty solid, too.
[3291.60 --> 3293.16]  Probably a pretty good experience over there, I'd imagine.
[3293.60 --> 3294.92]  They've all got their problems, though.
[3294.98 --> 3299.00]  I mean, I just did a fresh install of Windows again because Factorio was playing up.
[3299.14 --> 3303.02]  So, you know, need to give the factory room to grow on a proper install.
[3303.48 --> 3309.58]  And the shenanigans that Windows 11 makes you go through these days to install just a local-only account.
[3309.58 --> 3313.72]  Like, I had to disconnect the network cable and then do Shift-F10.
[3313.72 --> 3319.36]  And then there was some, like, out-of-box reset command you have to type and it reboots.
[3319.48 --> 3321.06]  And then it tries to restart the wizard.
[3321.32 --> 3322.30]  Clap your hands twice.
[3323.20 --> 3324.22]  Jump up and down.
[3324.36 --> 3324.56]  Yeah.
[3324.62 --> 3330.32]  And then when it can't find the internet connection, that's when it lets you finally create a local account.
[3331.40 --> 3331.88]  Crazy.
[3332.60 --> 3337.14]  Well, Jordan Bravo boosted in another 5,555 sets.
[3337.90 --> 3340.62]  I used to run Nextcloud in containers on Ubuntu.
[3340.62 --> 3343.54]  It was completely unreliable and very frustrating.
[3344.66 --> 3349.56]  Recently, I started over with NixOS and the Nextcloud NixOS module.
[3350.00 --> 3354.78]  It's been running with 100% uptime for many months now, and I'll never go back.
[3355.22 --> 3358.42]  You can pry Nix out of my cold, dead hands.
[3359.02 --> 3359.40]  Oh, yeah.
[3359.46 --> 3360.52]  This guy gets it.
[3360.94 --> 3361.16]  Yep.
[3361.70 --> 3363.54]  And I will say I'm very happy so far.
[3363.70 --> 3369.36]  I haven't fully set up my Nextcloud install with my new kind of Nix-based install that I talked about last episode.
[3369.62 --> 3372.94]  But since last episode, everything I have set up has been working really great.
[3372.94 --> 3374.34]  I'm happy with the performance.
[3375.22 --> 3377.94]  So, so far, I think problem solved for me.
[3378.06 --> 3378.52]  And I agree.
[3378.60 --> 3380.00]  You can pry it out of my cold, dead hands.
[3380.00 --> 3382.76]  We'll see how it does with my file upload from this episode.
[3382.76 --> 3392.26]  Because our centralized, self-hosted, like how hosts get the files to Drew, our editor, is we upload them to a self-hosted Nextcloud server.
[3392.48 --> 3394.46]  And the last four, five episodes?
[3394.60 --> 3395.44]  It's been problems.
[3395.94 --> 3396.06]  Yep.
[3396.06 --> 3399.70]  Ever since I got my fiber upload, like it can't handle my light speed, apparently.
[3399.88 --> 3400.88]  Ah, it's earphones.
[3400.96 --> 3401.56]  We thought so.
[3401.72 --> 3406.72]  That was until this weekend when I uploaded files from the studio and I had the same problem.
[3406.80 --> 3408.20]  And the studio's got like a crap upload.
[3408.26 --> 3409.16]  Oh, okay.
[3409.84 --> 3411.12]  So I think it's, I don't know.
[3411.12 --> 3413.84]  We use S3 storage as a backend for Nextcloud.
[3414.56 --> 3418.36]  We thought we'd solved it with file locking and we'd had a couple of successful uploads.
[3418.78 --> 3420.04]  And then here we are again.
[3420.10 --> 3421.86]  I don't actually know what the nature of it is yet.
[3422.00 --> 3424.76]  But it sure stinks because it looks like the files upload.
[3425.14 --> 3429.14]  And they even show the correct file size in like the web browser.
[3429.54 --> 3433.08]  But when you go to download them, that's when you find out it's like an invalid URL or something like that.
[3433.08 --> 3435.12]  Or when Drew messaged you and says, hey, dude.
[3435.62 --> 3436.30]  I don't have your file.
[3436.56 --> 3437.30]  It happened again.
[3437.30 --> 3442.62]  You know, the strangest thing is for once, everything's been just working for me.
[3442.70 --> 3446.00]  So I've never had one of the files recently have any problems.
[3446.24 --> 3447.22]  So maybe we should compare notes.
[3447.36 --> 3448.26]  I don't know what's going on here.
[3448.68 --> 3449.82]  He gave us his bug field.
[3450.34 --> 3451.86]  Bronzewing comes in with a row of ducks.
[3451.92 --> 3454.00]  That's 2,222 sats.
[3454.40 --> 3456.60]  I don't use Nix, but I have been thinking this whole time.
[3456.66 --> 3459.56]  The perfect media server could just be a Nix config.
[3460.18 --> 3464.56]  Just Plex or Jellyfin and, you know, the R stack and just have it all pretty set up.
[3465.02 --> 3466.36]  Maybe one day I'll even try Nix.
[3466.36 --> 3469.62]  I've been very happy with Unraid and I have the Pro Lifetime license.
[3470.18 --> 3472.52]  Managing the array is what I don't understand how to do.
[3472.66 --> 3473.90]  So I'm kind of scared to switch.
[3474.62 --> 3480.90]  So there's a separation in concerns in my mind, at least, between the base OS and the application layer.
[3481.02 --> 3487.44]  I think there's a handful of apps that the Nix way and like the Nix modules might make sense for.
[3487.44 --> 3496.76]  Like we're hearing just in this comment section, just in this feedback section alone, that many people have had good success with the Nix Cloud module, for example.
[3497.56 --> 3505.84]  But I think there's still a huge argument to be made for kind of the industry standardization around Docker Compose as a deployment artifact.
[3505.84 --> 3514.58]  Whenever you go to spin up any project, almost any project at least, they almost all have some kind of a Docker runtime these days.
[3514.82 --> 3515.60]  And the same cannot.
[3515.78 --> 3519.66]  I mean, image was only added a couple of weeks ago to the Nix packages repo.
[3519.66 --> 3529.38]  So long as you are still in the world that we're in right now, and I appreciate nothing's going to change unless people move things forward.
[3529.76 --> 3537.12]  So if I'm sat here saying like, we use Docker because everybody else uses Docker because everyone else uses Docker, like that just maintains the status quo.
[3537.20 --> 3538.36]  I'm aware of the irony.
[3539.12 --> 3545.42]  But, you know, from my perspective, it just, if I'm doing the same thing as everybody else, it makes troubleshooting easier.
[3545.52 --> 3548.62]  It makes the developers lives easier because they've got a stable deployment target.
[3548.62 --> 3550.78]  Yada, yada, yada, I think.
[3550.84 --> 3550.94]  Yeah.
[3551.68 --> 3564.38]  Well, I think with this one, I get reminded that, Alex, on the Perfect Media Server website that you have crafted, you already have a NixOS configuration for the Perfect Media Server.
[3564.56 --> 3566.02]  I admitted to the world last week.
[3566.04 --> 3569.60]  You even have a section here that says, take the blue pill.
[3571.20 --> 3576.50]  I admitted to the world last week that my media server has been running Nix for the last six months perfectly happily.
[3576.50 --> 3578.88]  And, yeah, never been more stable.
[3579.36 --> 3581.90]  I just want to point out, I'm not the one that's brought it up once this episode.
[3582.18 --> 3582.90]  Don't yell at me.
[3584.10 --> 3594.18]  I will say the base OS is Nix OS with ZFS working flawlessly and merger FS for the media drives.
[3594.18 --> 3601.52]  And then the app stack continues to be Docker Compose fed through my Ansible playbook that just deploys it onto the host.
[3601.64 --> 3602.78]  And then I run Docker Compose up.
[3603.38 --> 3609.78]  And that way, if ever I switch off Nix, it's all about, for me, maintaining that portability.
[3609.78 --> 3619.24]  If, for whatever reason, Nix implodes, which, with the community drama that constantly seems to be going on with that project, who knows what the future looks like.
[3619.32 --> 3620.48]  But I hope it's bright.
[3620.54 --> 3621.28]  I hope it's rosy.
[3621.58 --> 3624.06]  Whether it's Gooix or Nix or whoever.
[3624.78 --> 3625.12]  Lix.
[3625.56 --> 3626.48]  That's another one, isn't it?
[3626.58 --> 3626.70]  Yeah.
[3626.84 --> 3628.12]  So, yeah.
[3628.58 --> 3629.00]  I don't know.
[3629.64 --> 3631.40]  Portability, in a nutshell.
[3631.40 --> 3634.74]  I'll summarize this one because Tebby sent us a long one.
[3634.78 --> 3637.44]  He's a longtime listener, and he wanted to send us his thanks.
[3637.96 --> 3640.32]  He says he's reaching out to mention a heat.
[3640.42 --> 3641.30]  I don't know if that's a typo.
[3642.00 --> 3643.38]  He says, I'm not sure if it's been covered before.
[3643.46 --> 3644.84]  I recently discovered it's extremely useful.
[3644.90 --> 3648.72]  It's a quick command to remind myself of command usage and formatting.
[3648.84 --> 3650.32]  It's really made a huge difference for me.
[3651.00 --> 3651.24]  Okay.
[3651.24 --> 3657.92]  And he also mentioned that he's been getting into retro games, and he's been creating Docker containers to package up different Flash games.
[3658.42 --> 3659.24]  And he's had great success.
[3659.24 --> 3661.42]  He says, check out Teb writes code on GitHub.
[3661.52 --> 3661.78]  There you go.
[3661.84 --> 3665.90]  So, it's Teb writes code on GitHub to figure it out.
[3666.18 --> 3666.64]  That says GitHub.
[3666.76 --> 3667.04]  Thank you.
[3667.54 --> 3672.46]  We lost the whole era of gaming, didn't we, of retro gaming when Flash games went kaput.
[3672.96 --> 3673.36]  Yeah.
[3674.18 --> 3676.06]  It's amazing to see people working on this.
[3676.78 --> 3680.80]  You know, recently, listener Jeff brought this to my attention because he's a big Flash fan.
[3680.80 --> 3690.12]  And I got to say, before this episode, I was reading this boost in particular who mentions Ruffle, which kind of gets these things up and going.
[3690.26 --> 3693.86]  And Chris, I'm bringing this up because I think you're going to like this one.
[3694.14 --> 3701.66]  It is an open source piece of software written in Rust to run these old Flash games and these old Flash programs.
[3701.66 --> 3706.42]  And they have, if you go to the Ruffle website, they have a little demo section.
[3706.66 --> 3713.34]  And I, earlier today, wasted a little too much time playing Alien Humidid, which is one of the examples there.
[3713.42 --> 3717.30]  So, I got to say, if you do anything with this episode, at least go play that game.
[3717.46 --> 3718.44]  Really, really good fun.
[3718.44 --> 3719.96]  Check this out.
[3720.08 --> 3721.08]  This is too good.
[3721.44 --> 3722.36]  That is really neat.
[3723.02 --> 3723.88]  That's nice to see.
[3724.08 --> 3734.66]  I love the juxtaposition of having, like, an extremely modern programming language like Rust running these super old, ancient, like, Flash-based games.
[3734.76 --> 3735.44]  It's really nice.
[3735.96 --> 3736.62]  That's pretty great.
[3736.74 --> 3738.94]  SWAT rounds us out with a row of ducks.
[3739.20 --> 3739.92]  And thank you, Tebby.
[3739.98 --> 3740.62]  Appreciate that.
[3740.74 --> 3744.94]  And says, what's your recommendation for a low-power home NAS?
[3744.94 --> 3759.32]  Hardware-wise, I've been thinking about an Odroid H4 with an external hard drive enclosure with five or eight 3.5 bays connected via a single USB 3 cable.
[3759.98 --> 3762.72]  Software-wise, it'd be great to run ZFS.
[3762.88 --> 3764.02]  Don't know which distro you'd recommend.
[3764.24 --> 3765.60]  And maybe some VMs on top of that.
[3765.72 --> 3769.66]  Thinking about maybe Proxmox on the bare metal and then a ZFS or VM.
[3770.48 --> 3771.24]  I think you get the gist.
[3771.32 --> 3772.36]  What would you suggest?
[3773.08 --> 3773.44]  Wow.
[3773.44 --> 3774.96]  Yeah, a lot to unpack in this question.
[3775.26 --> 3787.56]  I think for a low-power system, I hate to say it, but some kind of an Intel box, their idle efficiency is particularly good because of their P and E core architecture.
[3788.22 --> 3797.06]  So if you wanted to go super-duper low-power with not much headroom, something like an N100-ish-based platform would be pretty decent.
[3797.06 --> 3802.50]  But that box that Brent just built, for example, is also pretty low-power.
[3802.60 --> 3806.90]  As I recall, it's something like 15, 20 watts without the hard drives at idle.
[3807.36 --> 3810.82]  And then it's got the headroom to go all the way up to 60, 70 watts.
[3810.92 --> 3812.30]  And it's got QuickSync built in.
[3812.40 --> 3814.96]  So it almost never uses anywhere near that amount of power.
[3814.96 --> 3815.78]  Yeah.
[3815.90 --> 3817.12]  So, yeah.
[3817.22 --> 3819.04]  Video transcoding is a bit of a beast.
[3819.18 --> 3821.66]  So if you're doing that, get something with hardware transcoding.
[3822.64 --> 3824.52]  The OS, I don't think it matters too much.
[3824.70 --> 3826.72]  Nix OS is fine.
[3827.28 --> 3828.16]  Unraid is fine.
[3829.18 --> 3832.20]  TrueNAS just had a nice big release that just added Docker Compose.
[3832.20 --> 3833.86]  That's probably also fine.
[3834.16 --> 3835.74]  Like, just try them.
[3835.98 --> 3838.12]  I mean, there's a lot of different options these days.
[3838.36 --> 3843.22]  And, you know, it's like telling me what color to paint your bedroom.
[3843.54 --> 3846.10]  Like, different folks with different strokes.
[3846.52 --> 3848.82]  Those one-liter PCs are definitely worth looking at.
[3849.04 --> 3853.16]  I have a lot of extensive experience with the Odroid H3 because I own a couple of them.
[3853.26 --> 3854.38]  And you're right, you could do that.
[3854.88 --> 3856.34]  I'm running two disks over USB.
[3856.34 --> 3857.84]  I don't generally recommend that.
[3858.24 --> 3859.86]  But I've been working for three years.
[3860.32 --> 3862.18]  But the H4, I would imagine, is even better.
[3862.96 --> 3865.54]  And Proxmox, I think, is something you should seriously consider.
[3866.34 --> 3869.56]  Because you could easily expand that later on to a different box.
[3869.60 --> 3874.16]  So say you did go with something like the Odroid, and then you hit the performance limitations of that.
[3874.66 --> 3876.44]  It would be pretty easy to migrate to something more powerful.
[3876.54 --> 3879.00]  Or if you start with a one-liter PC and want to go something bigger, et cetera.
[3879.72 --> 3882.78]  Proxmox would mean, though, you're going with the x86 platform, which is something to consider.
[3882.90 --> 3885.66]  A lot of the low-power options are going to be in the ARM side of things as well.
[3885.76 --> 3891.20]  But I would kind of love to know if we could answer this any further, if you've got any specific questions, or which direction you go.
[3891.20 --> 3892.72]  So let us know, SWAT.
[3893.10 --> 3893.88]  Thank you very much.
[3894.14 --> 3895.22]  And I appreciate the boost.
[3895.66 --> 3897.22]  I had a couple of call-outs I wanted to do, too.
[3897.28 --> 3899.84]  We don't get to all the boosts, but Scuffed came in with 5,000 sats.
[3899.92 --> 3904.34]  And he's looking for recommendations for a read-it-later slash omnivore replacement.
[3904.46 --> 3905.52]  Omnivore has just been purchased.
[3905.52 --> 3910.14]  And he's hoping for a recommendation from the audience for a replacement for that.
[3910.54 --> 3914.98]  PC Nolref, a Coda Radio listener, wanted to send some sats to self-hosted for a little bit of love.
[3915.32 --> 3922.26]  And we got 15,000 sats from the Muso, who said, I was going to go learn Docker Compose, but I decided to go full Nix.
[3922.26 --> 3924.52]  PagDot came with 3,000 sats.
[3924.72 --> 3926.76]  And I really appreciate this one.
[3927.72 --> 3932.68]  The Er and Ersatz TV is pronounced like Er because it's German.
[3933.02 --> 3934.56]  So it's Ersatz TV.
[3935.50 --> 3938.24]  And Ersatz is the German word for replacement.
[3938.82 --> 3941.02]  So it's your TV replacement.
[3941.68 --> 3942.14]  That's clever.
[3942.14 --> 3942.62]  Ha-ha.
[3942.88 --> 3943.22]  Right?
[3943.22 --> 3943.68]  That's good.
[3944.14 --> 3944.88]  I was so grateful.
[3945.10 --> 3948.70]  There was other people that boosted in, but for time, we do have to cut it short.
[3949.26 --> 3954.32]  Your boost will be in the Boost Barn, which is linked and will forever be in our show notes.
[3954.60 --> 3956.46]  Thank you, everybody who does boost in.
[3956.58 --> 3958.92]  We had 31 of you stream sats as you listen.
[3959.36 --> 3963.16]  So collectively, you sat streamers helped us stack 47,012 sats.
[3963.56 --> 3964.24]  Thank you very much.
[3964.24 --> 3971.72]  And when you combine that with our boosters, we had a very generous 346,354 sats sent into the show this week.
[3972.08 --> 3973.24]  It is a value-for-value production.
[3973.24 --> 3980.40]  So if you get some value from it, we really appreciate if you send in either a boost or you can set your support on Autopilot and become a member.
[3980.76 --> 3985.60]  To boost in, you just need a podcast app like Fountain or Cast-O-Matic or Podverse or Podcast Guru.
[3985.68 --> 3986.64]  There's so many good ones.
[3987.00 --> 3988.58]  They're listed at podcastapps.com.
[3988.98 --> 3992.48]  Fountain's the easiest, but it goes up from there to fully self-hosted solutions.
[3993.20 --> 3993.36]  Enjoy.
[3994.06 --> 3995.18]  And thank you for supporting the show.
[3996.36 --> 3996.76]  Absolutely.
[3997.22 --> 3999.18]  Your support makes all the difference.
[3999.18 --> 4001.98]  So it's not lost on us.
[4002.22 --> 4002.82]  Trust me.
[4003.20 --> 4007.22]  Whenever we get, we see the subscriber counts going up and down all the time.
[4007.38 --> 4010.10]  So big thank you to everybody who signs up.
[4010.68 --> 4020.22]  We're doing a post show every time for our site reliability engineers just to give you a little extra content as our way of saying thank you and an ad-free feed as well.
[4020.22 --> 4023.80]  A little bit of a PSA before we wrap up.
[4023.92 --> 4032.38]  If you use Vault Warden, there has been a pretty serious release and you need to upgrade to version 1.3.2.4.
[4032.88 --> 4038.30]  It has fixed, I guess, they say, quote, some CVE reported.
[4038.30 --> 4045.94]  So I don't know the details about the CVE, but it sounds like they recommend, the Vault Warden team recommends, that you get to the latest version as soon as possible.
[4046.72 --> 4051.22]  And then the contents of the CVE are going to be disclosed shortly, publicly, soon.
[4051.58 --> 4056.12]  So you probably want to be patched before they make the public disclosure because then people are going to start banging on it.
[4056.70 --> 4057.04]  Interesting.
[4057.28 --> 4063.78]  I wonder, the Bitwarden service had a little bit of downtime on a weekend a couple of weeks ago.
[4063.94 --> 4064.64]  I wonder if that's related.
[4064.64 --> 4065.60]  That bit me, by the way.
[4065.66 --> 4066.18]  That got me.
[4066.58 --> 4067.76]  That downtime got me.
[4067.76 --> 4069.86]  Yeah, you might be right.
[4069.92 --> 4072.40]  Maybe they were patching the back end real quick.
[4072.52 --> 4076.08]  It's the only time in many, many years that that's ever bit me.
[4076.66 --> 4077.58]  Now, one last thing.
[4077.64 --> 4084.06]  We mentioned it briefly in the episode last week that T-Tech, the guy behind the Proxmox Helper scripts, was in a hospice.
[4084.72 --> 4088.40]  Unfortunately, since the last episode, it's come to light that he has passed away, sadly.
[4088.74 --> 4092.62]  So sending thoughts and prayers and all that kind of stuff to his family.
[4092.62 --> 4101.02]  It's nice to see that the Proxmox Helper scripts have moved now into a community-owned repo, so they will live on beyond the man himself.
[4101.40 --> 4104.62]  So posthumously, thank you for everything you did, T-Tech.
[4104.62 --> 4106.14]  Yeah, it is really nice.
[4106.24 --> 4107.84]  These people make an impact on our communities.
[4107.98 --> 4109.20]  It's nice to recognize them.
[4109.94 --> 4113.06]  Brett Lee, is there anywhere you want to send people to get a little bit more of you?
[4113.64 --> 4113.92]  Yeah?
[4114.04 --> 4114.64]  You got any places?
[4115.04 --> 4117.54]  You can catch me every single week at Linux Unplugged.
[4118.20 --> 4119.42]  Hey, that's a great idea.
[4119.92 --> 4120.60]  There you go.
[4121.26 --> 4122.22]  LinuxUnplugged.com for that.
[4122.30 --> 4123.28]  Thank you for joining us, Brett.
[4123.28 --> 4124.88]  Always a pleasure.
[4125.08 --> 4126.64]  Yeah, thanks for putting the fire on for me.
[4127.28 --> 4128.46]  I know it's a baby Naz.
[4128.66 --> 4129.56]  It's brand, brand new.
[4129.64 --> 4137.04]  So you're going to have to come back at some point after you've had it in use, used it in anger for a while, set some things up, maybe got your backups going, and give us an update at some point how it's all working out.
[4137.30 --> 4140.40]  Yeah, I'm sure I'll ask you how to migrate from ButterFS to ZFS at some point.
[4143.54 --> 4145.98]  You can find me at alex.ktz.me.
[4146.04 --> 4148.38]  I've got a little self-hosted link tree over there.
[4148.80 --> 4149.98]  And thanks for listening, everybody.
[4149.98 --> 4153.04]  That was self-hosted.show slash 136.
