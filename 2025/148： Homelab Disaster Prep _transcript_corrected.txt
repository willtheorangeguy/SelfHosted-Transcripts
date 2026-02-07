[0.00 → 7.18] So I spun up a droplet the other day, and I came across the new App 3.0 release from the beginning of April.
[7.18 → 7.86] Have you seen this?
[8.32 → 9.60] This looks nice, doesn't it?
[9.64 → 10.58] Big improvement.
[10.72 → 11.62] Pretty colours.
[12.62 → 13.42] Nice formatting.
[14.26 → 15.16] Big improvement.
[15.46 → 17.60] New column display and all that.
[17.74 → 18.80] Yes, yes.
[19.18 → 26.68] This is my hot take, Alex, but I think if App 3.0 had been in Pop! OS when Linus tried it on Linus Tech Tips,
[26.68 → 31.40] I think he probably would have noticed he was about to destroy his desktop because it makes it really clear now.
[31.48 → 32.64] You're about to screw things up.
[33.08 → 34.56] I've been calling it the LTT feature.
[34.98 → 35.98] I think you guys are too kind.
[38.28 → 39.92] You are a troll, sir.
[40.04 → 41.48] That was a Brent, by the way.
[41.58 → 43.54] I think I just heard a wild Brent appear, right?
[43.82 → 44.38] Welcome back.
[44.62 → 44.96] Hello.
[45.38 → 45.96] Hello, Brentley.
[46.18 → 47.12] Imported from Canada.
[47.62 → 52.94] And we've also got producer Stephen on the line today, up from sunny Canada.
[53.50 → 55.18] We're outnumbered, Chris, by Canadians.
[55.18 → 57.38] At least it's at least a match.
[57.46 → 58.58] A fair match, maybe?
[58.96 → 59.22] Yeah.
[59.34 → 59.68] I don't know.
[59.76 → 60.82] We'll see as the show goes on.
[61.42 → 68.86] He's going to talk to us today about some massive power outage that they had up in the northern Toronto area a few weeks ago
[68.86 → 74.28] and sort of, I don't want to say doomsday prepping, but how self-hosted can prep for a week-long power outage.
[74.32 → 75.94] It's going to be fascinating.
[76.06 → 79.20] But before we dig into that, there's a little bit of housekeeping to take care of.
[79.20 → 84.60] Obviously, after last week's announcement of episode 150 being the last episode of Self Hosted,
[85.18 → 87.58] we had a few people reach out, and we'll get to the feedback later on.
[87.76 → 94.96] But we wanted to give those of you who tell us that the show means a lot to you a chance to remember the show.
[95.02 → 96.58] So we've put together some merch.
[97.26 → 98.44] Alex, you put together this merch.
[98.52 → 99.80] You had a great inspiration.
[100.54 → 104.72] It was an idea that was inspired for something we did for Coda Radio with one of its milestones.
[104.72 → 108.80] And you've made a dad hat, which is a great name.
[109.14 → 112.68] You got a mug, a big mug, and a classic t-shirt.
[112.82 → 117.18] But I think my favourite is the celebratory episode 150 posters.
[117.38 → 118.98] That is going up on the studio wall.
[119.42 → 119.56] Yeah.
[119.94 → 120.18] Yeah.
[120.34 → 125.20] So every episode title, for those of you that are listening, which I suppose being a podcast is everybody,
[125.20 → 136.56] every single episode title is painstakingly hand-placed on top of a vector graphic so it scales properly and all the rest of it.
[137.14 → 137.38] Yeah.
[137.46 → 144.82] Take a look at JupiterGarage.com and pick up yourself some nice self-hosted merch whilst it's still available.
[145.34 → 145.94] I've already ordered.
[146.48 → 147.66] I believe it's free shipping.
[147.94 → 151.34] I don't know if it's worldwide, but it certainly is in North America.
[151.76 → 153.22] When I was doing the checkout, I got free.
[153.68 → 154.14] There you go.
[154.14 → 154.92] Okay, good.
[155.52 → 158.10] This is my opportunity to restock my closet, you know.
[158.36 → 159.64] I've been getting all my swag stuff.
[159.68 → 161.54] It's been getting a little old, so I appreciate this.
[161.62 → 165.14] There is still the Chris and the Badger t-shirt over at Jupiter Garage as well.
[165.34 → 169.18] I believe there are some Soda robes, but don't tell anybody I told you that.
[169.44 → 170.04] They're fireproof.
[170.38 → 172.00] I see Chris having a palpitation.
[172.14 → 172.96] I mentioned that robe.
[173.18 → 174.32] Not technically fireproof.
[177.02 → 178.84] Yeah, perhaps don't buy one of those, but anyway.
[180.08 → 180.42] All right.
[180.50 → 183.50] So, Stephen, thank you very much for coming on to the episode today.
[183.80 → 184.38] What happened?
[184.38 → 185.84] You had a big old weather event.
[186.28 → 187.82] Yeah, it was pretty terrible, actually.
[188.46 → 191.52] And so I'm sure everyone's done this before.
[191.68 → 195.16] You look at the news and people say, oh, there's a terrible storm coming.
[195.26 → 196.44] And you go, yeah, okay, sure.
[196.48 → 199.84] There's going to be a storm, and maybe I'll lose power for an hour or two.
[199.84 → 205.48] Well, evidently I should have listened a little harder, and we didn't have power for about a week.
[205.88 → 209.14] Like genuinely no electricity in the entire...
[209.14 → 209.30] Yeah.
[209.48 → 211.42] Was it just your block or was it the whole town?
[211.42 → 215.56] So, like there's a whole like Since County kind of thing where I live.
[215.56 → 223.72] It was primarily around there, not all the way out to Toronto and whatnot, but definitely through the area that you came through when you're up here.
[223.72 → 226.30] Basically, just an ice storm happened.
[226.50 → 232.44] And so it was warm enough that it was raining for an extended period of time and then temperatures just started dropping.
[232.86 → 242.78] And then the ice started forming and just coating every single bit of a tree until the fact that like, you know, a very thin branch all of a sudden was way thicker than it used to be.
[242.78 → 244.12] And things just started breaking.
[245.00 → 250.48] And so you ended up with a bunch of damage from big limbs coming down and whatnot on power lines.
[250.64 → 256.42] And the damage was just so extensive that the hydro company couldn't get things back up and running for like a literal week.
[256.72 → 260.00] Sometimes a little bit more for some people, depending on where they were.
[260.46 → 260.96] That's wild.
[261.40 → 265.14] In the modern world, what do you do without electricity for a week?
[265.38 → 265.50] Yeah.
[265.80 → 267.28] So a bit interesting.
[267.28 → 269.56] I mean, how do you, like genuinely, quite genuine question.
[269.56 → 272.86] Like no hot water, I presume, no heating, no.
[273.40 → 273.76] Yes.
[273.88 → 274.22] What else?
[274.30 → 274.62] What else?
[274.70 → 275.50] Like basic amenities.
[275.66 → 276.34] What else were you missing?
[276.94 → 279.30] And were you kind of prepared for some of this at least?
[279.60 → 285.66] You know, you get a power outage and any home lab kind of person, self-hosted person probably has a couple of UPS's.
[285.70 → 285.88] Right.
[285.92 → 293.98] And so, I mean, generally, if you have like a for me anyway, if I have a power outage, my internet works for probably an hour or so and it just keeps working.
[293.98 → 294.20] Right.
[294.20 → 299.34] And so you have an iPad, you have an iPhone or whatever, and you can surf the net and busy yourself.
[299.34 → 302.48] But once that goes down, it is nothingness.
[302.56 → 302.72] Right.
[302.82 → 304.90] So was I prepared?
[305.18 → 310.86] Not really, because like I never thought about having to heat my house without power.
[310.92 → 311.20] Right.
[311.24 → 313.52] And then hot water, same thing.
[313.74 → 318.68] And then all of a sudden this stuff kind of starts getting pretty real when you don't have power for 24 hours.
[318.82 → 322.12] Thankfully, it wasn't well below freezing here.
[322.12 → 329.08] But after the first night, the house kind of lost most of the built-up heat from when we did have power.
[329.76 → 337.34] And so I had to start thinking about how am I going to power my furnace, which is thankfully gas, to get my family heat again.
[337.46 → 337.62] Right.
[337.76 → 339.66] So that was the first part.
[340.10 → 345.62] Did Jimmy rig up some kind of receptacle or some kind of connector to tie the ground in?
[345.72 → 345.82] Right.
[345.82 → 346.04] Yeah.
[346.20 → 347.88] So that was actually pretty funny.
[348.54 → 355.02] I didn't know about, you know, ground loops and whatnot and a bonded ground.
[355.46 → 358.50] And I'm sure there's another term I'm missing there.
[358.58 → 367.44] But the first generator I had that was from my father's childhood, it just had a ground that was kind of built into it.
[367.44 → 374.14] And so when I powered my furnace by basically making my furnace a plug-in appliance, it ran fine.
[374.92 → 380.32] But I didn't really want to survive off of this generator that was made in like the 70s or so.
[381.08 → 383.66] And probably, I don't know, probably hasn't run in 10 years.
[383.84 → 387.26] But I found a nice Honda one, and it has an inverter.
[388.08 → 391.76] And so that's fantastic because it's great for all the electronics and whatnot.
[392.18 → 394.32] But it doesn't have a bonded ground.
[394.32 → 406.88] And so I plug everything in and then the furnace doesn't kick on because there's a safety that doesn't fire the actual gas and the actual ignition unless the furnace sees a ground from the same source.
[406.88 → 417.00] And so I ended up going to Home Depot and just getting the end that you would buy to replace like an extension cord end.
[417.38 → 425.18] And I had to link the neutral and the ground pins and then plug that into the generator.
[425.72 → 427.40] And then it became a bonded ground.
[427.58 → 429.36] And then my furnace would work.
[429.84 → 432.16] It's stuff that I never thought I'd have to fiddle with.
[432.16 → 434.02] And it's not sketchy at all.
[434.04 → 436.94] Yeah, definitely something I would never consider, you know, ever doing.
[437.02 → 440.72] And then plugging into a wall outlet, which, again, was not a wall outlet.
[440.86 → 441.54] It was in the generator.
[441.72 → 443.88] But it just felt wrong doing it, right?
[443.96 → 445.10] But I got heat again.
[445.64 → 451.96] You know, this reminds me of a few, like, I don't know if you remember, Stephen, back in 98, there was those major ice storms that happened.
[452.06 → 453.96] That was very similar in like Ottawa and Quebec.
[453.96 → 462.08] And, you know, I've had forest fires in my area over the summers that caused the same thing for me, like loss of power for several days.
[462.20 → 463.60] We've seen this in Texas.
[463.60 → 464.96] It was a couple of years ago.
[465.42 → 468.14] And Alex, you had some, I think, last year, too, with some storms.
[468.38 → 481.08] And it gets me thinking about what we can do to try to experience this in a controlled environment, to learn all of those things instead of having to figure them out when absolutely everyone is trying to figure out the same problems.
[481.08 → 484.80] So it might be worth, I don't know, on a nice Saturday or something.
[485.06 → 489.26] It's like try to take down the power on the whole house, you know, anniversary every year.
[489.32 → 490.42] You do it on the same day.
[490.86 → 492.36] But it might teach you a few things.
[492.38 → 501.18] Because I learned, same as you did, Stephen, that, holy Geez, like, yeah, the essentials start to come into play.
[501.32 → 505.10] Like we pull water from under the ground.
[505.60 → 506.52] So we didn't even have water.
[506.72 → 508.42] You learned your fridge takes quite a bit of power.
[508.42 → 508.94] Exactly.
[509.14 → 513.60] And it changed my perspective of what we need to have around just in case.
[513.92 → 524.08] Like, you know, lately I've been thinking about buying battery systems that I could just move from its primary use to a secondary use for emergency purposes, this kind of things.
[524.34 → 529.18] And, you know, you start thinking about solar, too, that you can maybe roll out just in case of emergency.
[529.42 → 533.02] So it's a good exercise to go through, especially before you actually need it.
[533.02 → 539.64] So, Stephen, I suppose the next question is, was the data centre that you run impacted by this outage as well?
[539.74 → 542.58] And that must have been a whole experience in itself if it was.
[542.74 → 542.96] Yeah.
[543.16 → 545.74] So I have quite a bit of UPS power.
[545.74 → 551.72] But I definitely don't have UPS power that lasts an entire room for more than three hours.
[552.16 → 555.72] And so eventually that went down, which is pretty terrible.
[555.72 → 559.54] But all the customers other than you guys are local.
[559.78 → 561.68] So everyone else was down anyway.
[561.92 → 563.62] So I kind of got a free pass on that one.
[564.40 → 564.86] But yeah.
[565.02 → 567.56] So I've tried to start thinking about the future.
[567.64 → 571.92] Like, what do I do if this happens in, you know, next year, year after that?
[571.92 → 579.56] And so I found this interesting product called a Generating, which I'm pretty sure is just a branded thing from General.
[579.70 → 590.74] But it goes in between, kind of like a sandwich, between your power meter that sits outside your house and then that thing and then the actual, the building connect.
[591.60 → 596.10] And so what I'm able to do is I'm going to buy a fairly nice Honda generator.
[596.10 → 603.36] And then I can just link, like pull one cable right directly from the generator, which is I think it's going to be a 40 amp.
[603.48 → 610.02] But, you know, plug that directly into that unit, and it separates the house from the service, right?
[610.74 → 617.10] In the terms of my server room, I'm basically going to have the one panel that is the server room directly linked to that.
[617.26 → 619.04] And so this happens in the future.
[619.04 → 625.22] I'll just run a Honda generator and I don't have enough equipment in there that will require more than just one of those.
[625.50 → 630.34] But yeah, future is definitely going to be a much better, much better place to be.
[630.66 → 632.26] And I'm going to do the same for my house, I think.
[632.64 → 635.56] Wouldn't that take an absolute ton of fuel?
[636.08 → 637.04] It really doesn't.
[637.18 → 641.54] I mean, my house was running off of, what's the little guy?
[641.60 → 648.12] It's like 2200 watts, and it was, it has this eco-mode, and it actually revs itself way down.
[648.12 → 653.92] The only time at my house that I was ever getting that thing to rev up was when my well pump would kick in.
[654.32 → 661.46] Takes a bunch of amperage, but it's, it only stays on for like 30 seconds, and it's only really taking that much because it's pressurizing a tank.
[662.00 → 664.52] So how many litres an hour of fuel do you suppose?
[665.26 → 666.58] For the data centre at least?
[666.58 → 667.30] For the data centre.
[667.40 → 671.52] I can, I can very easily tell you a rough estimate of, of how the house goes.
[671.52 → 678.96] And so my house being furnace running, a couple of pumps running for a sump pump and whatnot, a couple other things.
[679.12 → 683.32] I could go on one gallon of fuel because that's all the thing holds.
[683.32 → 687.08] It's actually slightly under and don't ask me if it's Canadian or American gallon.
[687.40 → 693.28] I can't tell you, but that will go for six to six and a half hours to run that.
[693.42 → 694.90] So about three and a half litres or so.
[694.90 → 712.30] Yeah. So I think if I did that at the data centre, that generator has a much larger tank, but, you know, just having servers running just at idle, it's, it's a lot like when you're looking at your power usage, when you're, you know, transcoding Plex and whatnot.
[712.30 → 720.32] But if, if your server is not really doing a lot, it's just hosting out, you know, occasional files here and there, it doesn't actually take a ton of power.
[721.76 → 726.56] I'm going to, I'm going to guesstimate that because the generator is much larger and holds a lot more fuel.
[726.56 → 731.26] That thing's supposed to be able to run something like 12 hours at 50% load.
[731.80 → 734.42] And I don't think I'll be doing 50% load on the thing.
[734.72 → 736.02] So 12 hours would do it.
[736.22 → 739.00] Gives you long enough to get to the next town to pick up another can of.
[739.00 → 739.14] Yeah.
[739.24 → 740.48] I don't think that it should be a problem.
[740.70 → 741.16] Dinosaur juice.
[741.16 → 745.40] And I'll definitely have fuel just on hand, and I'll just throughout the year, I'll just cycle it out.
[745.46 → 746.16] So it's always fresh.
[746.40 → 748.42] You want to put some sea foam in that generator with Brent.
[748.52 → 750.22] He's a big fan of sea foam.
[750.60 → 751.18] There you go.
[751.50 → 752.42] Stabilize that gas.
[752.94 → 766.36] Going into it, Stephen, if you had some assumptions about a scenario like this, especially from like your hosting side, but also from the house side, if you had assumptions about how this would go, if any of those proved wrong, that you now like lesson learned type situation.
[766.36 → 769.08] So lesson learned, definitely.
[769.08 → 772.94] What is your option for a secondary heat source?
[772.94 → 777.22] In the sense of the servers, it's actually kind of nice because they generate the heat for you.
[777.22 → 785.04] But in my house, it was, you know, just lucky that I had switched to natural gas, and I was actually able to create heat.
[785.04 → 792.04] But if my house were heating with electricity, maybe I had, you know, a heat pump running the whole house or something like that.
[792.08 → 793.92] I don't know that I'd be able to power it at all.
[794.84 → 799.34] You know, maybe having some sort of secondary heat source is definitely a consideration these days.
[799.34 → 808.96] What about things like, because it was the whole town that was out, what about things like your internet connection or cell connections and stuff like that?
[809.02 → 811.68] I know there are two tiers of things.
[811.78 → 816.60] There's like necessities for life, like heat, keeping your food stored, all that kind of stuff.
[816.96 → 820.98] We're talking about self-hosting, which is probably not critical to life, let's be honest.
[820.98 → 827.10] But I'm curious, like you have, I think you have two internet connections coming into that room, right?
[827.16 → 832.38] With different, like what point does the highly available logic stop making sense?
[832.38 → 838.66] Well, interestingly enough, you kind of have some assumptions that you make about your providers, right?
[838.70 → 849.06] Like you think, especially for cell phones anyway, if your town loses power, you would think that all the cell phone towers would have their own generators, right?
[849.06 → 852.88] This kind of makes sense because they're for emergency services.
[853.28 → 855.04] These things should be staying up, right?
[855.88 → 858.66] Except for that, that didn't really pan out in my area.
[859.40 → 864.66] Apparently, the company that I'm with, that I will not name, but whose colour is red,
[865.08 → 870.30] they basically power things with a generator to recharge the UPS's.
[870.42 → 878.36] Then they were taking the generators, going to another station, recharging those UPS's, and then doing this like round-robin thing.
[878.36 → 884.84] And so you would have some connection with your cell phone for a while, and then it would just go out.
[885.58 → 888.28] At one point, though, I had zero connections.
[888.94 → 890.38] Just kind of blew my mind.
[890.52 → 894.54] I never would have thought that infrastructure that gets relied upon like that could go down.
[895.24 → 902.30] So to that, if you had the ability to maintain some sort of internet connection, you'd still be able to call it in emergencies, right?
[902.70 → 906.60] What's the name of that radio thing that you guys love that Jeff built a repeater for?
[907.30 → 907.70] Starlink?
[907.70 → 908.90] No, mesoblastic.
[909.16 → 909.80] Mesoblastic, yeah.
[910.12 → 911.50] You peppers need one of those.
[911.60 → 912.54] I thought about that, honestly.
[913.60 → 916.48] So I have two internet connections, like you said, in that room.
[916.94 → 918.76] One of them would have been perfectly fine.
[918.92 → 921.30] The other one with the other company wouldn't have worked at all.
[921.92 → 923.92] Yeah, because one's a phone line, right?
[923.96 → 926.78] And one's fibre, and they go take totally different paths.
[926.80 → 928.68] Yeah, coaxial and fibre, yeah.
[928.82 → 933.20] But if one of those had worked, I would have been able to call it, which would have been fantastic, really.
[933.42 → 935.02] But thankfully, I didn't have an emergency.
[935.02 → 938.60] So what was your biggest takeaway from all of this?
[938.98 → 940.20] Be able to make your own power.
[940.54 → 942.08] That's a pretty good conclusion right there.
[942.58 → 943.42] Make friends with neighbours.
[944.08 → 944.30] Yeah.
[944.52 → 945.36] Yeah, like straight up.
[945.58 → 947.10] I mean, it's everything, right?
[947.62 → 950.06] If you can't make your own power, you literally have nothing.
[950.22 → 954.08] I mean, I suppose if you had a fireplace that still used wood, you could heat that.
[954.18 → 955.38] But past that, you're done.
[956.78 → 960.40] Good time to be a generator salesman in the northern Toronto area, I suspect.
[961.16 → 962.62] Thank you very much for joining us, Stephen.
[962.64 → 963.14] It was a pleasure.
[964.24 → 965.26] Thanks for having me, guys.
[965.26 → 969.58] Tailscale.com slash self-hosted.
[969.64 → 974.68] Head on over there to get Tail scale for free up to 100 devices and three users, no credit card required.
[975.24 → 979.48] Tail scale is the easiest way to connect your devices and services wherever they are.
[979.98 → 982.40] Tailscale.com slash self-hosted.
[982.72 → 986.52] Modern networking over a flat mesh network protected by WireGuard.
[986.66 → 987.62] And it's fast.
[987.98 → 990.94] It's privacy for everyone and every organization.
[990.94 → 998.54] And what might not be immediately obvious with Tail scale but does become obvious as you use it, as you can really build around it.
[998.80 → 1001.72] So all of our studio equipment connects to the Tail net IP.
[1002.04 → 1003.04] Everything's on our Tail net.
[1003.22 → 1012.22] And instead of going to their LAN IP, all the devices, all the control surfaces, all the remote control protocols, everything uses the Tail net IPs on our Tail scale.
[1012.60 → 1016.24] The reason for that is, is it gives us incredible flexibility.
[1016.52 → 1017.78] So we can pick up equipment.
[1018.18 → 1019.50] And this just happened this last weekend.
[1019.50 → 1025.60] We took old equipment out of our travel bag, and we took equipment from the studio, kind of mix match.
[1025.82 → 1027.88] My number one rule is we never take gear out of the studio.
[1027.96 → 1029.30] So, of course, we broke the number one rule.
[1029.98 → 1035.98] And Saturday, we set it all up in my RV, plugged it into the LAN, and everything just connected and started talking.
[1036.84 → 1041.04] Imagine how simple that makes things when you don't have to troubleshoot the networking at all.
[1041.32 → 1046.66] But what was even more incredible is the next day, Sunday, we tore everything down, set it up in a classroom at a college.
[1046.66 → 1051.10] We had to build our own ad hoc LAN because they didn't provide any networking for us.
[1051.24 → 1058.96] And once we got the ad hoc LAN up off of a little GI slate router, everything started talking over the Tail net and connected.
[1059.18 → 1060.74] And we didn't have to configure anything.
[1060.74 → 1068.88] So, I mean, I'm talking even the remote control surface for my mixer and to play soundboard clips and for all the machines to be able to talk to control the recorder.
[1069.06 → 1071.06] Everything goes over our Tail net.
[1071.22 → 1076.88] And that means wherever we are at, it all works, and they all talk like they're on the same local LAN.
[1077.22 → 1078.76] Now, imagine this for your servers.
[1079.20 → 1083.60] Imagine this for your VMs and your mobile devices, even your Docker applications.
[1083.60 → 1086.28] You can put everything on one flat mesh network.
[1086.68 → 1092.44] And then Tail scale has a bunch of really powerful tools to manage access and control who can get to what.
[1092.76 → 1096.60] It'll integrate with your organizational authentication infrastructure if you have one.
[1097.02 → 1102.76] That's why thousands of companies like Instacart, Hugging Face, Duolingo, and Jupyter Broadcasting use Tail scale.
[1103.16 → 1106.94] And why so many of our listeners and me personally, I use Tail scale.
[1107.10 → 1107.66] It's intuitive.
[1108.16 → 1112.44] It's a programmable way to manage a private network that is protected by WireGuard.
[1112.44 → 1114.76] It's really something we've needed for the Internet.
[1115.14 → 1121.40] And it'll just make things fundamentally easier for your connectivity and makes old VPNs seem, well, old and busted.
[1121.76 → 1126.24] So get started, support the show, and try it for free on 100 devices and three accounts.
[1126.78 → 1130.40] You just got to go to Tailscale.com slash self-hosted.
[1130.68 → 1133.88] That's Tailscale.com slash self-hosted.
[1135.50 → 1137.44] I don't know if you caught on YouTube lately.
[1137.44 → 1142.10] I have started revving up the Perfect Media Server series on YouTube again.
[1142.44 → 1151.06] And as part of that, I got the itch to try out Unpaid in the name of science with their upcoming 7.1 release.
[1151.30 → 1154.50] And I managed to convince you to take a look and kick the tires with me.
[1154.86 → 1155.86] Yeah, I thought it was time.
[1156.28 → 1159.72] You know, they are a sponsor of our show, and we do want to use the sponsor's products.
[1159.84 → 1162.00] It's like, okay, we've got to actually do this.
[1162.00 → 1168.94] But with the 7.1 release coming up, it felt like a good excuse to really give it a go because I had a machine.
[1169.16 → 1172.70] I was unsuccessful at running Unpaid on previously.
[1173.16 → 1179.48] And it was too bad because it was a little HP Reliant tower, kind of perfect for being a little NAS box.
[1179.68 → 1180.54] Oh, yeah, I remember those.
[1180.76 → 1181.32] Yeah, yeah.
[1181.40 → 1182.48] And so I was a little bummed.
[1182.54 → 1183.08] I couldn't get it.
[1183.08 → 1184.88] I think it was probably 7.0 I tried.
[1185.64 → 1189.06] So I was up for a challenge to see if I could make it work with 7.1.
[1189.58 → 1191.36] Do you remember what didn't work the last time?
[1191.82 → 1194.98] No, I think we also had trouble getting Proxmox to boot on that system.
[1195.70 → 1197.66] So it wasn't just an Unpaid thing.
[1197.82 → 1201.68] It was, but we did eventually get Proxmox to work, but it took a lot of finagling.
[1202.62 → 1203.56] Yeah, I know.
[1203.78 → 1204.82] Jeff would probably remember.
[1205.20 → 1206.40] He had to do a lot of the struggling.
[1206.40 → 1209.06] It was during a Linux fest, so I was off doing fest stuff.
[1209.44 → 1211.70] But I was ready and willing to give it a go.
[1211.70 → 1216.36] So I had not really expected much because it had failed before.
[1216.46 → 1218.54] And I thought, well, it's probably using some of the same stuff.
[1219.08 → 1221.50] But spoiler alert, it actually booted just fine.
[1221.98 → 1223.28] It was not a problem at all.
[1223.30 → 1225.98] And I'd probably attribute that to the newer Linux kernel, I would imagine.
[1226.06 → 1226.96] But I don't know for sure.
[1227.52 → 1228.64] Yeah, the 7.1 release.
[1228.98 → 1230.42] Let's wind back a little bit, actually.
[1230.78 → 1235.34] In terms of who Unpaid is aimed at, where would you say it fits in the market?
[1235.34 → 1239.68] Because I think this positions a lot of our coverage and a lot of our perspective.
[1239.68 → 1242.50] Who is Unpaid for, do you think?
[1242.68 → 1243.92] I think that's a fair question.
[1244.46 → 1247.96] Because you and I, we dabble and deploy systems with Nick.
[1248.00 → 1248.70] So does Brent now.
[1249.48 → 1251.38] And so I don't know if it's targeted squarely at us.
[1251.46 → 1254.38] I think it's, I picture it as somebody who's very busy.
[1254.54 → 1255.54] You probably have a day job.
[1256.18 → 1257.06] You've got a family.
[1257.28 → 1260.14] And you hear us talk about these great applications on the show.
[1260.94 → 1262.02] We talk about Jellyfin.
[1262.02 → 1266.14] And you want to try it out, but you don't have a ton of time to dedicate to this.
[1266.42 → 1268.82] Maybe you've got a Saturday afternoon and a spare PC.
[1269.68 → 1271.88] I think that's really where Unpaid nails it.
[1272.54 → 1276.00] Because it starts with this image downloader that's available for Mac or Windows.
[1276.54 → 1279.90] And when you run that, it says, okay, what version do you want?
[1280.04 → 1284.10] And you can opt, if you scroll down to the bottom, you can opt for 7.1 and go full baller.
[1284.62 → 1287.10] But then it just, it asks you a couple of basic questions.
[1287.16 → 1288.12] Like, should I use DHCP?
[1288.42 → 1289.78] Or should I have a static IP?
[1289.78 → 1293.06] And if you want me to have that, what should that static IP be?
[1293.06 → 1294.50] And what should my host name be?
[1294.58 → 1297.22] It's Tower by default, but maybe you want something else.
[1297.56 → 1300.94] So that's the entirety of what the imager asked me.
[1301.10 → 1304.16] And then you hit run, and it flashes a USB thumb drive for you.
[1304.70 → 1307.04] It's a foolproof process.
[1307.16 → 1310.52] I mean, you could just go with all the defaults, not change a single thing, and it would work.
[1310.52 → 1310.96] Absolutely.
[1311.74 → 1323.28] And I think that really speaks to, really, for me, the best use case for Unpaid is you've got that old desktop system that maybe is just sat in a closet or something.
[1323.40 → 1324.60] And you think, well, what do I do with this?
[1324.68 → 1326.96] Surely I could be doing something fun or tinker with this.
[1326.96 → 1330.82] Or you've got a couple of hard drives that aren't the same size.
[1331.34 → 1337.72] Or just a bunch of random hardware that you've either acquired over the years or whatever.
[1337.88 → 1339.68] Like, I don't really know where it comes from.
[1339.72 → 1340.16] It doesn't matter.
[1340.16 → 1349.44] But, you know, you can take mismatched drive sizes, and you can run it on a potato CPU and use all those disks for storage.
[1349.44 → 1361.36] Like, Unpaid will group all of those mismatched disks together into a single array, a single pool, and let you treat 10 random hard drives as if they were one big volume.
[1361.68 → 1366.96] And that, really, for most people's sort of media storage needs is pretty much all they need.
[1366.96 → 1385.80] And with these newer versions of Unpaid, adding things like ZFS and Butters and all these kinds of fancy features, if you do end up getting to a point where you feel like you need to take the training wheels off a little bit, or you're kind of bumping up against the guardrails, well, you've got proper tooling in there, air quotes, proper tooling, like ZFS.
[1385.80 → 1390.76] And you can do ZFS snapshot replication and all that kind of stuff.
[1390.76 → 1420.76] 
[1420.76 → 1425.20] It helps you grow a little bit more than that old Ubuntu or whatever box it might be.
[1425.50 → 1428.34] So I think there's a class of user out there who got started with a system.
[1428.44 → 1429.12] Maybe it's on a laptop.
[1429.26 → 1429.88] Maybe it's on a desktop.
[1430.00 → 1430.72] Maybe it's on a server.
[1430.72 → 1432.68] But they're outgrowing that installation.
[1433.34 → 1434.20] And you can move.
[1434.28 → 1435.88] You can just move over to Unpaid.
[1436.08 → 1438.88] And you get a UI to manage all of that and import all of that stuff.
[1439.18 → 1443.10] So I think that's another real potential use case here for someone out there.
[1443.66 → 1456.02] And you get, can I say this, probably the most passionate, the I don't know if they're the most knowledgeable, but certainly one of the most engaged communities in this space, period.
[1456.02 → 1460.02] Yeah, so once I got started, I kind of immediately had a question.
[1460.54 → 1468.84] And that was, okay, so if when I run my Unpaid system, the way it's designed to work is it runs off of the USB thumb drive that you flash with their image tool.
[1469.12 → 1473.34] And the operating system loads the contents of the thumb drive into RAM.
[1474.10 → 1478.46] So the thumb drive really doesn't have a lot of read-write to it except for configuration changes.
[1478.86 → 1483.74] And I thought, okay, well, if I'm going to have this thing running from a thumb drive, I want to know what thumb drive I should have.
[1483.74 → 1485.72] And then I want to know how I should be backing it up.
[1486.02 → 1491.78] And, seriously, like the top three or four Google results were from the support community forms.
[1491.96 → 1505.66] And they just very clearly have the answers in the second or third response with good and really excellent advice on which devices are really solid, how to back them up automatically, other critical files you should consider.
[1505.66 → 1512.32] Because when you install Unpaid, what you're really installing is your license, and it's tied to that thumb drive.
[1512.38 → 1516.38] So you want to make sure it's backed up, and you want to make sure it's something that's going to last awhile.
[1516.38 → 1525.54] I have to say I was really surprised by this because I guess we're used to flashing something onto a USB drive as, you know, using all those Linux distros.
[1525.56 → 1528.16] Well, I expected, you know, oh, you know, 7.1, it's in development.
[1528.24 → 1529.60] That's probably just an ISO image.
[1529.90 → 1530.10] Nope.
[1530.44 → 1530.66] Nope.
[1530.66 → 1532.14] You still use the image tool to go grab it.
[1532.20 → 1535.22] It kind of caught me by surprise because I was looking for images.
[1535.22 → 1538.60] I thought, you know, I didn't have to do the installation after you plug this thing in.
[1538.64 → 1540.78] But nope, booted right to a working system.
[1540.96 → 1544.30] And it took me a little bit to, like, wrap my head around the difference.
[1544.80 → 1548.12] Yeah, the positive side would be that you get access to all the drives.
[1548.64 → 1552.32] You know, they're in the system and there's no installation to screw up for new users.
[1552.46 → 1555.50] I think the downside is, well, what if I want more robust storage?
[1556.50 → 1559.28] I felt a little better once we learned that it runs from a RAM disk.
[1559.46 → 1562.08] But I think the lesson learned there is make sure you're using a good one.
[1562.08 → 1566.34] Grab a good thumb drive for this and one that'll last and then come up with a way to back it up.
[1566.38 → 1567.80] And I'll have links for that in the show notes.
[1568.52 → 1570.76] Alex, do you see any downsides to doing this?
[1570.82 → 1574.42] I know we've played with some servers here that kind of run the same way.
[1574.52 → 1576.04] Is this an industry standard?
[1576.60 → 1580.56] Well, I mean, booting from the USB drive is pretty standard for ESXi.
[1580.92 → 1582.60] I've certainly installed that way.
[1583.54 → 1588.24] And as long as the rights to the flash media are absolutely minimized,
[1588.24 → 1590.96] which Unpaid has spent, how old is Unpaid at this point?
[1590.96 → 1591.90] 15 years?
[1592.72 → 1596.48] They spent a good deal of time in the old days optimizing,
[1596.90 → 1600.30] because this was one of the key sort of complaints of people in the old days.
[1600.64 → 1602.04] And now it's kind of a non-issue.
[1602.18 → 1605.92] The only things that kind of get written to disk are configuration file changes,
[1606.52 → 1608.42] you know, like stuff that has to persist.
[1609.18 → 1611.92] But yeah, most of the stuff happens in RAM disk.
[1612.06 → 1616.30] Like you can, if you're not careful, overwhelm it with rights of log files
[1616.30 → 1618.08] if you misconfigure something.
[1618.08 → 1620.70] But you have to be trying these days with Unpaid.
[1620.82 → 1623.70] They've really made it very, very straightforward and very simple.
[1624.20 → 1628.50] So the community itself is a fantastic feature of Unpaid.
[1628.92 → 1633.82] But also, so are the community apps and the plugins available for Unpaid.
[1634.02 → 1635.36] There are how many?
[1635.64 → 1636.92] There's got to be a thousand.
[1636.92 → 1640.58] I have a number here, 2,405.
[1641.04 → 1641.96] There you go.
[1642.18 → 1643.64] So basically anything you're going to want.
[1644.70 → 1649.44] And that I, of course, installed my favourite apps.
[1649.62 → 1651.66] I put on Albi Hub in about five minutes.
[1651.82 → 1654.40] And then about another five, ten minutes after that, I had Jellyfin running.
[1655.36 → 1659.44] I did try one of the I can't remember the name of it,
[1659.76 → 1665.20] but it essentially tries to emulate the OpenAI API using Llama on the back end.
[1665.20 → 1668.06] And I specifically installed the CPU version,
[1668.34 → 1671.54] but it still complained about not being able to access my GPU.
[1672.04 → 1675.36] The thing is, is these are community-created apps,
[1675.66 → 1678.62] and individuals are contributing these to the app store.
[1678.76 → 1682.72] So sometimes you will have a couple of things like that are hit-and-miss.
[1682.88 → 1685.76] But the simpler stuff that I tried that isn't trying to access my GPU,
[1685.88 → 1688.58] because I don't have a GPU in the system, that all worked.
[1688.94 → 1691.62] And I discovered, I probably should have known about this,
[1691.64 → 1693.08] because I knew about 12-foot ladder.
[1693.08 → 1696.18] Well, there's 13-foot ladder, 13-feet ladder.
[1696.24 → 1696.54] What's that?
[1696.68 → 1697.56] Did you know about this?
[1697.82 → 1701.88] It's an app that, it gets around some paywalls for sites, for news.
[1702.18 → 1703.46] I try to bring in a lot of news,
[1703.54 → 1705.74] and so I'm constantly, within a couple of days,
[1706.04 → 1708.08] hitting paywalls on all the sites that have them.
[1708.68 → 1709.56] It doesn't get around all of them,
[1709.58 → 1712.92] but it's a self-hosted app that you can install in just a couple of seconds from the app store.
[1713.82 → 1715.86] And it makes me collecting news a little bit easier.
[1716.14 → 1718.10] Could you point something like Kara Keep at that?
[1718.10 → 1718.58] Probably.
[1719.42 → 1720.74] I've just started playing with it.
[1721.10 → 1722.40] I've had it not work for everything,
[1722.56 → 1724.40] so I'm not going to say it's fantastically great.
[1724.96 → 1726.20] So it's hit-and-miss.
[1726.28 → 1726.84] I'll say that.
[1727.26 → 1731.28] But, you know, with 2,405 apps, not all of them are going to be great.
[1731.78 → 1733.34] Not all of them are going to have fantastic icons.
[1733.68 → 1735.80] But all the heavy hitters, like all of them are there.
[1736.14 → 1740.58] And then they even have like remixes that are, say, Jellyfin or Plex,
[1740.74 → 1744.58] but integrated with a VPN and WireGuard and maybe some other servers.
[1744.58 → 1747.24] Like they'll have different versions where somebody's remixed it essentially.
[1747.98 → 1751.06] And they're labelled differently, and they have different creators and different publishers.
[1751.40 → 1754.82] But for people that are, there's like a series of the media centre applications
[1754.82 → 1760.20] and backend applications that are all just pre-configured and ready to go with VPNs.
[1760.20 → 1764.06] And then you just fill in the details, and it all just automatically works when you start the container.
[1765.02 → 1768.54] I will say Unpaid's age is both a blessing and a curse.
[1768.90 → 1773.72] There are some legacy decisions that were made a long time ago.
[1773.72 → 1779.32] And one of those is the fact that Unpaid does real-time parity calculation on that pool of disks,
[1780.06 → 1785.82] which means you are limited to basically half the speed of the slowest disk when you're making a White.
[1786.50 → 1790.26] And the reason for that is because to write a new block of parity,
[1790.94 → 1795.68] Unpaid first has to read the block from disk, calculate the new block of parity,
[1795.84 → 1796.84] and then write it to both.
[1796.96 → 1800.72] So you're basically making two reads or two writes every time you update parity.
[1800.72 → 1805.42] And so unfortunately that means performance can be a little slow sometimes.
[1806.02 → 1809.38] There are some mitigations in place for something called a cache drive.
[1809.46 → 1814.26] So you could basically stick an SSD in front of your spinners to kind of speed things up.
[1814.42 → 1817.92] And it, in the short term, doesn't have any parity.
[1818.32 → 1820.70] And then there's a script that runs called the mover script,
[1820.78 → 1826.02] which moves things from that kind of unprotected area when you're maybe asleep or something,
[1826.22 → 1827.72] to the protected array.
[1827.72 → 1834.52] Now there are a bunch of APIs, like Unpaid just had a webinar recently about some changes they're making to the APIs under the hood.
[1835.24 → 1840.74] Unpaid as a company has made some strong moves to secure the future of their products.
[1840.84 → 1844.72] I mean, we had John Palazzo on this show three, four years ago now.
[1845.26 → 1846.60] Things have changed quite a bit since then.
[1846.64 → 1848.50] Obviously John's moved on to Hexes these days.
[1848.50 → 1854.84] But, you know, things at Unpaid Towers, so to speak, look pretty rosy to me.
[1854.90 → 1859.06] They've had a bunch of ex-IX systems folks who really know what they're doing.
[1859.46 → 1864.14] They're making some really strong architectural changes and refactoring a bunch of the code under the covers.
[1865.26 → 1868.40] And really, I think, you know, Unpaid as a core offering,
[1869.18 → 1874.00] it's probably in as good of a place as I've seen it for the last decade.
[1874.28 → 1876.48] Like, they're really cooking some good stuff over there.
[1876.48 → 1879.36] Yeah, it seems like with 7.1 they really got serious with ZFS.
[1879.92 → 1883.18] Like, really the full-fledged ZFS support,
[1883.96 → 1887.22] which is obviously just getting more and more popular with home libbers.
[1887.60 → 1892.02] They also have XFS, Butters, and if the website's correct,
[1892.22 → 1896.66] still technically, although not supported or advised, Risers for legacy systems.
[1896.98 → 1900.08] Yeah, well, in the old days, Riser was the default for Unpaid,
[1900.12 → 1902.60] and then they had to switch away for obvious reasons.
[1903.36 → 1906.30] Riser was also the default for OpenSUSE.
[1906.78 → 1907.08] Yeah.
[1907.32 → 1908.88] Or SUSE, whatever it was at the time.
[1909.10 → 1909.26] Yeah.
[1909.46 → 1909.70] Yeah.
[1909.76 → 1910.84] I used it for quite a bit.
[1911.78 → 1916.24] So I actually had, I like to see this just because I did have quite a few Risers discs
[1916.24 → 1917.62] sitting around back in the day.
[1918.02 → 1918.94] Nostalgic file system.
[1919.10 → 1920.40] Now, who put this in the dog?
[1920.68 → 1923.04] H-A Unpaid, Home Assistant Unpaid integration.
[1923.16 → 1923.62] Who was that?
[1923.86 → 1924.44] That was me.
[1924.44 → 1929.12] I was trying to find little projects that would, like, force you boys to at least try them or get intrigued.
[1929.16 → 1932.60] Brent found it, and I tried it, and I love it.
[1932.66 → 1937.54] So it is a custom integration that allows you to monitor and control your Unpaid server from Home Assistant,
[1937.54 → 1940.16] and you can monitor all the things you'd expect.
[1941.00 → 1945.14] System stats, RAM, cache, disk array, temperatures.
[1945.94 → 1949.78] You can monitor the usage of the system, essentially, if there's a UPS connected.
[1949.78 → 1957.06] But what I really liked about it is that it lets me toggle on and off my containers and my VMs right from Home Assistant.
[1957.68 → 1957.88] Yeah.
[1958.68 → 1960.80] So that was really nice, just right there in my dashboard.
[1961.32 → 1966.26] But getting things like the disk usage and CPU temps and network and RAM activity,
[1966.46 → 1969.52] not only is it just nice to have those stats in the Unpaid dashboard,
[1969.94 → 1973.22] but now to have them in Home Assistant, I have yet another place to generate charts.
[1973.22 → 1979.42] But in theory, I could start building automations or alerts around some of this data, too,
[1979.60 → 1981.20] which could be pretty useful.
[1981.98 → 1983.18] You know, I could just integrate that.
[1983.34 → 1987.66] I wonder if you could tie that into some kind of media server log of, like,
[1987.66 → 1989.58] when was the last time this file was played?
[1990.08 → 1994.90] If a disk goes over a certain percentage used, get it out of here, you know?
[1995.20 → 1995.60] Definitely.
[1995.80 → 2000.48] I think also, like, alert me if the thing's running with a high CPU for a while.
[2000.48 → 2002.46] I already have an alert pipeline through Home Assistant.
[2002.46 → 2003.66] Why not just lean into that?
[2004.14 → 2006.20] Now I kind of want to put every Linux server into Home Assistant.
[2006.38 → 2007.56] Why am I not doing that?
[2008.38 → 2008.70] I know.
[2008.78 → 2012.32] When I saw this, I was like, Geez, I really wish I could do this for every Linux server I had.
[2012.84 → 2015.50] You can even execute shell commands from Home Assistant.
[2015.76 → 2016.06] Wow.
[2016.22 → 2018.82] It'll connect in over SSH, and it'll execute a shell command for you.
[2018.82 → 2019.64] What could go wrong with that?
[2019.66 → 2020.30] Isn't that awesome?
[2020.52 → 2021.48] I think it's awesome.
[2021.80 → 2026.44] Especially with the new Home Assistant assist stuff, you hook up an AI to that,
[2026.48 → 2028.90] and then suddenly you've got AI controlling your Unpaid box.
[2029.06 → 2029.64] What could go wrong?
[2029.64 → 2030.00] Whoa.
[2030.00 → 2030.28] Whoa.
[2030.46 → 2033.34] I could use Voice Assistant to turn on and off containers.
[2034.02 → 2035.42] Hey, Unpaid, install Jellyfin.
[2036.08 → 2040.20] I could tell turning off Jellyfin when the kids are watching too much TV from bed.
[2040.26 → 2042.04] Or when you're watching too much TV.
[2042.88 → 2043.56] Like a well-being.
[2043.56 → 2044.44] There's the automation.
[2046.70 → 2049.92] Now, this, I think, pulls all that info in over SSH.
[2050.40 → 2055.20] And Brent, you actually found one that also will talk MQTT back to Home Assistant.
[2055.32 → 2059.58] Yeah, I was all jazzed about this first integration called HA-Unpaid.
[2059.70 → 2064.16] And then I got a little confused because I found another project called HAS-Unpaid.
[2064.16 → 2064.24] Unpaid.
[2065.36 → 2067.42] I guess we could work on the naming and the space.
[2067.50 → 2069.08] But this one, I guess, is a little different.
[2069.08 → 2070.76] So their description is,
[2070.76 → 2078.42] This Docker container parses a forwards all-web socket message from your Unpaid server to Home Assistant using the MQTT protocol.
[2078.62 → 2084.10] That enables you to create dashboards that provide superior overview compared to Unpaid's native capabilities.
[2084.24 → 2089.60] And I think also just bringing something like that in over MQTT is probably a better way to do this sort of thing.
[2089.60 → 2089.90] Hmm.
[2091.30 → 2094.48] These projects also seem like they're pretty actively developed.
[2094.82 → 2097.88] So I think it's a hot new space you've got to keep your eye on.
[2097.94 → 2099.02] Especially the integration I tried.
[2099.18 → 2101.92] I think it just had a release like two days ago or something.
[2102.54 → 2103.80] I say this from a place of love.
[2104.12 → 2106.42] The Unpaid community is a bunch of nerds.
[2106.88 → 2107.14] Yeah.
[2107.66 → 2108.16] It's clear.
[2108.44 → 2109.94] I was really pleased when I saw that.
[2110.02 → 2111.26] Bringing my two worlds together?
[2111.38 → 2112.08] Yes, please.
[2112.64 → 2113.52] And what about pricing?
[2113.52 → 2117.98] They made some changes to their pricing model, what, about a year ago now?
[2118.08 → 2119.08] It's a subscription?
[2119.60 → 2119.92] Products?
[2120.18 → 2122.26] Does that mean we hate them like we hate Plex now?
[2122.40 → 2124.38] You know, Brent and I were talking about this over lunch.
[2124.84 → 2130.96] And I'm kind of the opinion that the more I build around my home lab, the more essential it becomes.
[2131.06 → 2135.66] And this is why I also pay for Home Assistant Cloud, even though I have everything on tail scale now.
[2136.22 → 2142.54] I still subscribe to Home Assistant Cloud because I want them to continue to develop Home Assistant and the contributions they make.
[2142.94 → 2147.88] And if I was building my home lab around Unpaid, and you easily could.
[2148.06 → 2149.34] I didn't even get into the VMs.
[2149.34 → 2150.56] The VM system is great now.
[2150.56 → 2152.02] Oh, there are loads we've missed here.
[2152.28 → 2152.64] Loads.
[2153.06 → 2153.22] Yeah.
[2153.42 → 2159.26] I mean, I think it's worth paying to make it sustainable to have a company that's actively driving and contributing to it.
[2159.74 → 2167.62] We were just talking over lunch about some of the projects that have just faded away over the years, and you become dependent on them, and you wish there was a way you could have contributed to them.
[2167.62 → 2173.80] So I don't hate that it's a subscription because it's an ongoing thing that they're continually producing.
[2174.26 → 2177.42] Where I draw the line with a subscription is if it's a one and done.
[2177.84 → 2183.22] Like I can't – like in the app world, I cannot stand apps that want to give you one thing once but have you pay a subscription.
[2183.22 → 2184.92] That's bonkers to me.
[2185.30 → 2190.88] But for this, you get all the updates included while you have the I guess, subscription.
[2191.48 → 2192.92] So you're getting value.
[2193.06 → 2193.82] You're getting support.
[2194.44 → 2195.44] Getting the license.
[2195.44 → 2203.84] I thought it was nice that they had a pretty well-written FAQ on the pricing because, as we know, it can be very different in different places.
[2203.98 → 2207.74] So I had a bunch of questions, and that's the perfect place to find them.
[2207.92 → 2211.72] And the very first line says, Unpaid OS is not a subscription.
[2212.26 → 2215.06] Once you purchase a license, you own that license forever.
[2215.92 → 2218.78] I thought that was interesting wording and kind of attractive.
[2219.20 → 2223.12] So the licensing does give you updates as you keep –
[2223.12 → 2223.80] For a year, right?
[2223.80 → 2224.56] Mm-hmm, mm-hmm.
[2224.68 → 2230.34] And then after a year, it sounds like you can pay an optional what they call an extension fee, which is like $36 a year.
[2230.50 → 2232.68] Yeah, so I guess you get it for a cheaper price.
[2232.72 → 2233.82] So I guess that's not a subscription.
[2233.98 → 2234.94] You're renewing a license.
[2235.10 → 2235.26] Mm-hmm.
[2235.34 → 2237.94] They also have lifetime licenses if that's your thing.
[2238.24 → 2238.80] Mm-hmm.
[2238.88 → 2240.42] So, yeah, that's interesting.
[2240.50 → 2243.48] But how did that go, Chris, for the trying this out?
[2243.54 → 2244.32] Did you need –
[2244.32 → 2247.30] So you can just use a 30-day free trial license when you start.
[2247.60 → 2249.70] You know, you need to activate that.
[2249.70 → 2257.66] But it's all – what I did, just to make it easy on myself for the first time, is they have an option now – well, they have an option to start a GUI.
[2257.66 → 2263.58] So you could actually just run an X session on the console of your machine if that was for me.
[2264.34 → 2267.50] And so I just did it right there in the browser on the console of the machine.
[2268.66 → 2271.64] What's brilliant about that, of course, is it is tied to that USB thumb drive.
[2271.80 → 2274.88] And so it's pretty easy to back that up and move it, too, which is interesting.
[2274.88 → 2283.10] And I think if I were to deploy this, like I said, either as the NAS here at the studio or at home, I'd subscribe.
[2283.40 → 2284.84] Or I guess not subscribe.
[2285.04 → 2286.90] I'd purchase the yearly license.
[2287.64 → 2290.22] You'd support future development is the wording.
[2290.76 → 2296.04] I would probably be more likely to be inclined to get the lifetime membership or license, whatever you want to call it.
[2296.08 → 2301.52] Because, you know, that's my – I want something that I'm probably going to at least use for five years.
[2302.26 → 2302.42] Yeah.
[2302.44 → 2303.80] How much is the lifetime?
[2303.80 → 2306.28] Lifetime is $249 per license.
[2306.44 → 2311.08] So $249 per machine for, you know, perpetual lifetime license.
[2311.48 → 2311.68] Yeah.
[2311.82 → 2312.52] That's not too bad.
[2312.64 → 2316.62] I mean, I guess that's in line with the Boogeyman Plex right now.
[2316.80 → 2320.66] Their price update, I believe, is live as of this recording now, too.
[2320.78 → 2326.30] So the difference being Unpaid are adding new features, not putting existing ones behind a paywall.
[2326.80 → 2331.52] I think, too, it comes down to do you have a bit of money and not much time, right?
[2331.52 → 2339.80] If you have all the time in the world, you could figure out how to build your server from Nix or from Linux from scratch even if you had all the time in the world.
[2339.80 → 2341.62] Perfectmediaserver.com.
[2341.80 → 2342.16] Yeah.
[2342.28 → 2344.10] You could go the perfect media server route.
[2344.48 → 2348.00] And there's just a bit more of a time investment there, too.
[2348.38 → 2357.58] I think that's – each one of us has to make the decision, is this worth – and people that buy Macs, they know they're spending a premium to get a certain product.
[2357.58 → 2360.38] Or people that buy iPhones and Pixels.
[2360.60 → 2362.10] Again, it's the same thing.
[2362.66 → 2365.06] And so it's like where are you this type of customer?
[2365.30 → 2370.26] And for me, I already have a skill set that I've developed for a long time and I already have systems in place.
[2370.40 → 2372.00] So I'm not really their target customer.
[2372.48 → 2381.68] But if I had an existing system that wasn't really cutting it anymore, or I didn't have a lot of time and I wanted to build something new and fresh and have easy access to the best applications we ever talk about,
[2381.68 → 2384.78] it might be worth a lifetime license or an annual license.
[2385.52 → 2389.48] It's just like where does it fall on your particular time value spectrum, I think.
[2390.34 → 2394.62] So switching topics a little bit, how much do you two know about passkeys?
[2395.32 → 2397.38] I've been resisting the passkey adoption.
[2397.82 → 2401.50] I've been watching the space and also just hesitating.
[2401.84 → 2403.84] Because everything wants to own my passkey.
[2404.02 → 2405.80] iOS wants to manage my passkey.
[2406.72 → 2408.60] Bitwarden wants to manage my passkeys.
[2409.02 → 2410.70] Google wants to manage my passkeys.
[2410.70 → 2419.48] And I just feel like I have to make some sort of massive decision that I'm not prepared to make or fully understand the pros and cons to.
[2419.88 → 2424.16] And I finally have a pretty good system with passwords where I have unique passwords for my sites.
[2424.24 → 2425.80] I've got two-factor for a lot of stuff.
[2426.26 → 2427.82] Like it's kind of been in the last year or two.
[2427.90 → 2429.08] I finally got all that worked out.
[2429.16 → 2430.60] And now I have to switch.
[2431.74 → 2432.78] So I'm a little resistant.
[2432.94 → 2438.10] But if it's something I could self-host myself and manage, I'd probably be a little more comfortable with it.
[2438.10 → 2440.68] Well, your argument doesn't hold any water with me, gents.
[2440.80 → 2445.00] Because every single thing in the world wants to manage your passwords.
[2445.60 → 2449.02] Chrome and LastPass and Bitwarden and your phone and blah, blah.
[2449.04 → 2450.80] Every browser has its own little thing.
[2451.28 → 2452.40] So don't give me that.
[2452.40 → 2458.98] But the passkeys' implementation is essentially big tech's way of getting rid of the password.
[2459.62 → 2462.44] And I checked out this week a project called Pocket ID.
[2462.96 → 2467.56] And this is an OIDC, an OpenID Connect OAuth provider.
[2467.90 → 2476.28] So it's a way to sign in to your self-hosted apps without having to create an account on every single thing one by one.
[2476.28 → 2478.54] Okay, this is my speed.
[2478.58 → 2483.12] But the kicker is that Pocket ID only works with passkeys.
[2483.58 → 2484.28] No passwords.
[2484.92 → 2490.68] So it describes itself as a simple OIDC provider that allows users to authenticate with their passkeys to your services.
[2490.84 → 2493.20] This might be more like what I would be comfortable with, I think.
[2493.64 → 2498.64] Well, I'll tell you, there's a certain magic when you just put a couple of environment variables into your Docker Compose file.
[2498.64 → 2508.12] And then you basically touch your Touch ID chip on your MacBook or, in my case, log into Bitwarden and click the passkey in question.
[2509.02 → 2516.68] And suddenly I'm logged in in that browser session to every single app that I've configured to work with it as an OIDC client.
[2517.40 → 2518.78] It's really slick.
[2519.52 → 2522.58] Not every app supports OIDC or OAuth.
[2522.68 → 2525.92] You will have to implement this on a per-application basis.
[2525.92 → 2528.06] It's like Gîte supports it.
[2528.44 → 2531.22] Tail scale, you can set up a custom OIDC provider with Tail scale.
[2531.96 → 2537.68] I was playing around with Fresh RSS and Carrageen with this the other day, just to sort of test it out.
[2538.44 → 2539.14] So it's pretty nice.
[2539.32 → 2543.64] But, yeah, the OIDC support isn't there for every single app.
[2545.54 → 2547.76] Unraid.net slash self-hosted.
[2547.94 → 2550.34] Unpaid 7.1 is really cooking.
[2550.34 → 2554.64] I've been playing around with the release candidate, and I really like the new UI tweaks.
[2554.64 → 2562.42] And I especially appreciate the tweaks to VM support and just the full-forced embrace of ZFS.
[2563.26 → 2571.62] Which means, if you're switching from True NAS or Proxmox or Ubuntu, Unpaid in 7.1 can now automatically detect and import your ZFS pools,
[2572.02 → 2576.62] making migration from what might be not an ideal setup to a much more ideal setup.
[2577.46 → 2579.04] Wireless support is now in here as well.
[2579.04 → 2584.88] And I think one of the things you have to appreciate about Unpaid in general is just how straightforward it makes getting started.
[2585.06 → 2592.44] If you've got hardware today, a PC, and some disks in your closet, you can start building something and play around with the applications we talk about in just minutes.
[2592.98 → 2598.68] No exaggeration when I say, once I had Unpaid set up, five minutes to get Alfie going.
[2599.02 → 2601.46] Another ten minutes to get Jellyfin going.
[2601.46 → 2603.08] It was so straightforward.
[2603.20 → 2606.10] The thing that took the longest was me deciding where I was going to store my media.
[2606.46 → 2611.34] The process is so straightforward, and it lets you immediately start playing with some of the things we talk about.
[2611.66 → 2614.36] Lots of choices, too, if you want to throw a GPU in there.
[2614.76 → 2618.12] Unpaid makes it very straightforward not only to share that GPU with your system,
[2618.54 → 2625.96] but there are a lot of LLM applications that are just one click away that are ready to access your GPU right there on your LAN and keep your data private.
[2625.96 → 2630.20] Also, the emulating for your VM now, chef's kiss.
[2630.98 → 2638.28] Really nice one, makes it easy to set up a Nix OS one, or even, I will say, I tried a Windows 11 template and a Windows 10 template.
[2638.66 → 2643.68] And I have to say, it's possible, but I don't miss running Windows one bit.
[2644.04 → 2647.44] And Unpaid makes it easy, too, if you have a Mac and you want to do Apple Time Machine.
[2647.88 → 2648.74] Very straightforward.
[2649.32 → 2650.86] So this is something you've got to try.
[2651.20 → 2654.40] It makes building your home lab straightforward.
[2654.40 → 2656.80] You get right to playing around with the applications.
[2657.38 → 2662.76] And with Unpaid's various support for different disk protocols and formats and the Linux kernel underneath it all,
[2662.90 → 2664.22] there's just a ton of flexibility.
[2664.52 → 2666.90] It means you can probably use what you've already got.
[2667.16 → 2668.52] So support the show and get started.
[2668.62 → 2671.22] Go try it out like we have, and I think you're going to love it.
[2671.48 → 2673.60] Go to unraid.net slash self-hosted.
[2673.64 → 2675.80] That's where you go to get started, and you support the show.
[2676.26 → 2678.10] The new 7.1 is so close.
[2678.42 → 2680.02] It's in release candidate stage right now.
[2680.06 → 2681.06] It's going to be out very soon.
[2681.50 → 2683.24] So go get it all figured out.
[2683.24 → 2687.06] Start learning the layout now and, you know, build something.
[2687.34 → 2690.44] Play with some of these apps we talk about and get to that next step.
[2691.20 → 2693.08] I think you're going to find it just starts rolling from there.
[2693.24 → 2696.70] And it all starts at unraid.net slash self-hosted.
[2696.70 → 2700.50] So how was Linux Fest Northwest, chaps?
[2701.12 → 2702.82] Fantastic, fun, a bit exhausting.
[2703.22 → 2703.46] Sunny.
[2703.80 → 2704.98] Yes, very nice weather.
[2705.46 → 2711.50] It's always one of these events where every conversation you're like, oh, I hadn't heard that, or oh, I haven't tried that, or you're doing what?
[2711.72 → 2712.48] You brought what?
[2712.86 → 2713.82] A lot of that going on.
[2713.82 → 2714.90] Anybody mentioned pass keys?
[2715.40 → 2716.32] No, no pass keys.
[2716.46 → 2717.00] Sorry, Alex.
[2717.00 → 2722.22] We did have people travel from a little all over the continent to come say hi, which was great.
[2722.32 → 2723.68] Some people went from Florida.
[2724.10 → 2726.34] We had some people from, well, California, of course.
[2726.46 → 2726.78] Thank you, Jeff.
[2727.48 → 2727.92] Yep, yep.
[2728.66 → 2729.40] Jose came.
[2729.46 → 2730.06] Puerto Rico.
[2730.14 → 2730.52] From Puerto Rico.
[2730.52 → 2730.96] That's true.
[2731.34 → 2732.38] So it was a fun time.
[2732.38 → 2733.48] We had some Canadians there.
[2733.58 → 2736.12] We had somebody there from Vermont and, of course, a few folks from Oregon.
[2736.78 → 2736.94] Yeah.
[2737.42 → 2740.04] Speaking of California, you're off there again soon, aren't you?
[2740.42 → 2741.62] Something to do with that van of yours.
[2742.24 → 2743.20] Oh, Alex.
[2743.34 → 2743.92] It is time.
[2744.20 → 2747.84] This has been a story in the making for a few years, right, Chris?
[2748.34 → 2749.36] Project Van Rescue.
[2749.54 → 2750.48] Is that what we're calling it?
[2750.62 → 2752.78] Well, as we call it something different every time we refer to it.
[2752.98 → 2755.92] But yes, Brent is the proud owner of a bus.
[2756.00 → 2758.92] We went into our plans in the launch, episode 20, was it?
[2758.98 → 2759.70] Yes, it is.
[2759.78 → 2760.02] Okay.
[2760.40 → 2765.38] So we did go into some detail there, but the short version is we have to get down to L.A. by tomorrow,
[2766.28 → 2770.74] and we're going to try to pick this thing up and hustle back, even though it hasn't been on the road for six years.
[2771.62 → 2773.76] And it may not have working brakes.
[2773.90 → 2776.36] We're not sure if it needs to be lubed.
[2776.64 → 2778.28] We're pretty sure it has an oil leak.
[2778.52 → 2780.94] There's probably a radiator hose or two that's going to go on us.
[2781.16 → 2783.48] And it may even have a horrible wobble as we go down the road.
[2783.54 → 2785.64] So we're going to do the right thing when we get there.
[2786.30 → 2789.34] And one of the first things we're going to address is installing a home assistant.
[2790.00 → 2792.26] It seems like the right approach, doesn't it, boys?
[2792.46 → 2792.68] Yeah.
[2793.42 → 2795.38] I wonder what Derek would make of that.
[2795.52 → 2797.28] You know, Vice Grip Garage Derek.
[2798.06 → 2799.28] I think we'd make him proud.
[2799.28 → 2800.36] I feel like we'd make him proud.
[2800.44 → 2801.94] We're bringing some good gear.
[2802.34 → 2806.90] We're bringing some devices, including some sensors and LED, LED light ropes.
[2807.10 → 2809.76] And I mean, we're going to get this thing decked out.
[2809.88 → 2811.76] So even if we're stuck on the side of the road,
[2812.50 → 2815.94] we even found an Android tablet that we're going to mount on the wall for him.
[2816.02 → 2819.96] So Brent's going in with a dashboard tablet.
[2820.16 → 2820.62] Oh, wonderful.
[2821.58 → 2822.00] I know.
[2822.00 → 2825.00] So how many pies are you putting in his bench seat before you get back to...
[2826.00 → 2829.72] Well, one of them is x86-based and one of them is a pie.
[2829.98 → 2830.72] Ah, there you go.
[2830.94 → 2831.06] Yeah.
[2831.24 → 2834.58] We wouldn't be a Chris Project in a van without a pie involved.
[2835.24 → 2836.56] Oh, we're swimming in pies these days.
[2836.58 → 2838.48] We've got to stay true to the roots of our show.
[2838.60 → 2841.98] Because you remember in those early episodes, it was all about the Raspberry pies in your bench seat.
[2842.00 → 2842.24] Oh, yeah.
[2843.40 → 2846.92] Brent, like, dusted off some boxes, and we found four more pies yesterday.
[2847.04 → 2849.78] It's amazing what you can find in the Jupiter Broadcasting Studio.
[2850.16 → 2850.40] Yeah.
[2850.40 → 2851.84] We'll put those to good use.
[2852.04 → 2858.78] So speaking of Home Assistant, I see that you had a chat with Paulus recently, the founder of Home Assistant.
[2858.94 → 2859.30] Is that right?
[2859.78 → 2860.90] It will be coming out.
[2861.28 → 2863.54] It's not out yet, but in the next Linux Unplugged,
[2863.92 → 2867.64] they've just made some big changes in the structure of how they work.
[2867.72 → 2871.68] He's no longer at Nebulas, and a lot of the people we know are no longer at Nebulas.
[2872.22 → 2874.14] They now work at the Open Home Foundation.
[2874.76 → 2877.36] And there's been some major realignments there.
[2877.36 → 2888.20] So we get into that, as well as his workaround local AI first and voice and some of the community-driven projects that are about to get some day of light on them.
[2888.32 → 2901.94] I mean, we really spanned a lot because I was trying to introduce Brent and Was to Paulus and just get them sort of wrapped, get their heads wrapped around Home Assistant as they both begin to deploy their own units.
[2901.94 → 2904.10] I thought, well, who better else to talk to than the founder of Home Assistant?
[2904.28 → 2911.64] So as Brent's getting ready to deploy a van unit, Was's getting ready to deploy a domicile unit, they're both getting ready for their first Home Assistant instances.
[2911.78 → 2919.00] And I thought, well, they should probably kind of understand how this all works, how it's maintained, who supports it, and then kind of some of the stuff that's coming later this year.
[2919.00 → 2923.56] The project has also evolved quite a bit since you gentlemen first started using Home Assistant.
[2923.86 → 2932.84] So it was nice to get what's happening these days and actually your advice on how the heck I should set up this technology in this van.
[2932.84 → 2948.64] And Alex, I don't know if you saw, but one of the things that's under discussion is deprecating Home Assistant core and container installation essentially and really only formally supporting Home Assistant OS and also deprecating a couple of older architectures, including 32-bit.
[2949.34 → 2950.16] Big changes.
[2950.38 → 2953.28] I mean, you could still technically run core, right?
[2953.30 → 2958.14] You could still get it to work, but it will no longer be really – there will be no guides.
[2958.22 → 2959.20] There will be no support there.
[2959.40 → 2960.68] They're really going to focus on the OS.
[2960.68 → 2961.94] It's under discussion right now.
[2961.94 → 2962.38] Interesting.
[2963.12 → 2963.76] That's kind of a big change.
[2963.92 → 2971.38] I do think that kind of makes sense in a way from a support burden to kind of – they've only got so many cycles to support certain things.
[2972.10 → 2979.90] And also just from a support but from a maintenance perspective, like you've only got one target or one or two targets to build for.
[2980.14 → 2981.56] Yeah, it does make a ton of sense.
[2982.20 → 2984.24] Yeah, and honestly, they converted me.
[2984.80 → 2990.54] I was a critic of the idea of them running their own OS, and it's been using it for years now, and it's been fine.
[2990.54 → 2993.80] I do think Brent is going to have a better setup than me right out of the gate.
[2993.88 → 2994.12] Really?
[2994.26 → 2995.06] I'm a little jealous.
[2995.60 → 2998.24] I'm a little jealous because, right, I'm running on greens and blues.
[2998.82 → 3003.50] Well, you have like an industrial x86 PC that's hardwired to run off DC.
[3003.50 → 3006.22] It has freaking quick sync support.
[3006.26 → 3006.72] Heck yeah.
[3007.14 → 3009.08] Which mine, you know, again, I'm just on a pie.
[3009.56 → 3010.70] You've got eight gigs of RAM.
[3010.76 → 3011.58] I've got two.
[3012.04 → 3014.54] You've got two gigabit Ethernet ports.
[3014.60 → 3016.68] I've got one gigabit Ethernet port.
[3016.68 → 3023.00] And it's also a hardened device designed for industrial applications, so it should be much better in the van.
[3024.64 → 3030.92] And, of course, I'm just really jealous that it's already wired for DC because we're going to try to do everything DC in the van that we can from the start.
[3031.32 → 3036.58] Yeah, this is a crazy device that our dear producer, Jeff, I don't know, he found it in like a trash bin or something.
[3036.62 → 3037.20] Yeah, I'm sure that was it.
[3037.62 → 3037.98] Rescued?
[3038.06 → 3039.02] It's a rescued PC.
[3039.16 → 3041.98] Yeah, and then we popped a little couple upgrades in there, and Bob's your uncle.
[3042.18 → 3043.56] It's Brent's new home assistant machine.
[3043.64 → 3044.74] It's going to be awesome, I think.
[3044.74 → 3046.60] It even supports ECC memory.
[3046.96 → 3049.56] I don't think the stuff in there is, but if I ever wanted to.
[3049.58 → 3050.60] Well, they have to run ZFS.
[3051.12 → 3051.48] Right?
[3052.22 → 3057.16] And I've been also calculating the power usage on this thing because Jeff was like, oh, that thing accepts power.
[3057.40 → 3059.78] But, you know, Jeff, he's an optimist.
[3059.90 → 3061.12] So I actually measured it.
[3061.30 → 3068.80] I didn't actually tell you this, but for 20 hours I was measuring the power on this thing while it was very little, 0.18 kilowatt-hours.
[3069.02 → 3069.24] Yeah.
[3069.42 → 3073.54] Which is like about, I don't know, eight and a half watts just sitting there.
[3073.54 → 3075.48] But that's through the AC adapter.
[3075.78 → 3076.00] No.
[3077.20 → 3077.86] Yes, it is.
[3077.92 → 3078.08] You're right.
[3078.30 → 3080.74] So there's a little bit of inefficiency there.
[3081.06 → 3082.26] Oh, so it gets even better?
[3082.42 → 3084.34] It's an adapter converting to DC, yeah.
[3084.82 → 3085.10] Okay.
[3085.32 → 3087.54] It's amazing how you can make those modern Intel chips.
[3087.72 → 3087.94] Yeah.
[3088.36 → 3089.16] They just sit there.
[3089.28 → 3091.86] They just don't need anything at all.
[3091.90 → 3092.50] They just sat there.
[3092.94 → 3093.92] I'm really looking forward to it.
[3093.92 → 3097.78] Now, thank you very much to everybody that wrote in.
[3097.78 → 3106.14] We got an absolute flood of feedback and messages, and there's no way we'll be able to read all of them in the remaining time in today's episode.
[3106.66 → 3110.00] But we've got a few in the sack that we pulled out.
[3110.00 → 3112.12] Yeah, really, really nice emails.
[3112.50 → 3113.60] Lots of really nice emails.
[3113.78 → 3114.58] And Scott wrote in and said,
[3114.62 → 3114.84] Greetings.
[3115.48 → 3116.70] I'm sorry to hear the show's ending.
[3117.00 → 3119.18] I'm someone just getting deeper into self-hosting.
[3119.72 → 3122.40] My services and you have been very valuable.
[3122.94 → 3126.72] My self-hosting services, and you have been very valuable in pointing me in the right direction.
[3127.08 → 3130.74] Things like Tail scale, Audio Bookshelf, Ditching Plex, which is currently being implemented.
[3130.74 → 3134.88] Though I'm an Apple consultant, I'm a barely Linux literate.
[3135.54 → 3137.10] Docker still eludes me.
[3137.42 → 3140.42] So I have one final request, and also my first request.
[3140.86 → 3149.90] Could you recommend on the last few shows resources for people to both get started implementing various self-hosting projects and places to follow to keep abreast of new things in self-hosting world?
[3150.26 → 3155.36] Places that are not 90% populated with just super dense terminology or deep prerequisite knowledge.
[3155.66 → 3158.30] Or, you know, just keep going on an ad hoc basis.
[3158.68 → 3159.60] Thanks for being out there.
[3159.60 → 3164.20] Well, we basically are keeping going on an ad hoc basis with it.
[3164.50 → 3167.86] We don't know what the frequency will be yet, but I'll pop up in luck from time to time.
[3168.32 → 3171.98] And we'll do impromptu episodes of self-hosted in there by the sounds of it.
[3172.70 → 3174.10] Yeah, and I don't think we'll try to.
[3174.22 → 3178.08] I think we'll try to keep it, you know, so you don't have to have a bunch of Linux knowledge or something like that.
[3178.12 → 3179.00] We'll try to make it.
[3179.32 → 3180.24] We'll try to make it fit.
[3181.04 → 3181.40] Definitely.
[3181.72 → 3183.08] In terms of places to go.
[3183.18 → 3185.90] I mean, there's our discord self-hosted. Show slash discord.
[3186.16 → 3188.72] That's not going anywhere when the podcast ends.
[3188.72 → 3195.88] We're just going to leave that to kind of hang out on the vine and the wonderful mod team over there can do with it whatever they like.
[3196.10 → 3196.82] There's the Matrix, too.
[3196.86 → 3197.36] We could mention.
[3197.62 → 3199.34] The Matrix will exist and continue as well.
[3199.42 → 3200.88] The Matrix self-hosted room.
[3201.14 → 3204.86] Should probably lean heavier into the self-hosted infrastructure.
[3204.86 → 3210.16] One of the big criticisms, actually, that I've seen over the years is that we don't host our own social media necessarily.
[3210.28 → 3212.86] And we don't host our own chat platforms necessarily.
[3213.46 → 3215.56] Which we've documented in the show the reasons why.
[3215.64 → 3218.64] It's about furthering the mission and giving people a place to gather.
[3219.58 → 3222.58] But, you know, self-hosted will be self-hosted sometimes.
[3223.40 → 3224.12] God love them.
[3224.12 → 3228.10] But I would point this gentleman at lemmy.world.
[3228.38 → 3229.62] And there's a self-hosted.
[3229.86 → 3231.94] You don't call it a Subreddit over there, do you?
[3232.02 → 3233.48] But it's a community, I think.
[3234.28 → 3235.50] And this is part of the Fediverse.
[3235.74 → 3237.00] Lemmy.world is part of the Fediverse.
[3237.28 → 3240.16] And there's a very active self-hosted community over there as well.
[3240.86 → 3243.66] Lots of perfect threads happen there all the time.
[3244.46 → 3244.56] Yeah.
[3244.84 → 3246.32] It's really, I think, communities.
[3246.52 → 3249.32] And finding the community that fits your expertise level.
[3249.74 → 3250.96] I think those are all perfect tips.
[3251.84 → 3253.52] And, again, thank you everybody writing in.
[3253.76 → 3254.66] And we're reading them.
[3255.16 → 3257.82] And I'm trying to respond to some of them as well.
[3258.06 → 3260.52] We got some really generous boosts as well.
[3261.04 → 3265.72] Tabby Dog came in as our baller booster with 215,000 sets.
[3265.94 → 3266.18] Whoa.
[3266.62 → 3266.82] Yeah.
[3267.54 → 3269.40] He says, I'm sad to hear the show is coming to an end.
[3269.58 → 3273.44] I'm so thankful for the content and the energy you've invested into self-hosted.
[3273.94 → 3283.04] In reply to hybrid sarcasm, OpenWebUI actually does have a partial solution to searchable Obsidian vaults of documentation with their knowledge implementation.
[3283.78 → 3284.10] Okay.
[3284.18 → 3285.84] It is really easy to set up and works.
[3286.06 → 3286.50] Okay.
[3286.94 → 3290.18] Setting up a knowledge base in OpenWebUI can be done in a workspace.
[3290.18 → 3301.50] You can upload your entire Obsidian vault directly through the Web UI and attach that to a knowledge custom model based on whichever LLM you would like, ALAMO, or even an API.
[3302.34 → 3305.48] I only wish there was an implementation that allows you syncing from Obsidian.
[3305.62 → 3306.32] No kidding.
[3306.52 → 3306.74] Yeah, right?
[3307.22 → 3308.12] That seems pretty obvious.
[3308.26 → 3309.48] Obsidian should be working on that.
[3309.54 → 3313.30] With the amount they charge me for Obsidian sync, I should just be getting this as a feature.
[3313.30 → 3324.02] There are a bunch of plugins that will let you talk to your vault as a like, you can have a chat with your notes type thing and hook it into OBAMA.
[3324.56 → 3325.46] But this is fascinating.
[3325.58 → 3329.42] I would also say that OpenWebUI is one of those apps that supports OIDC.
[3329.54 → 3332.12] So if you want to throw that behind Pocket ID, you can.
[3332.12 → 3338.48] But, you know, in terms of installing plugins in Obsidian, that might make more sense than this route.
[3338.64 → 3340.60] But I'm going to certainly try this.
[3341.26 → 3342.76] Yeah, it does seem like kind of a fun idea.
[3343.06 → 3344.22] He had some really kind words.
[3344.22 → 3349.14] And he's also all on board with some more self-hosting content in Linux Unplugged.
[3349.58 → 3352.58] Well, Brent, you're going to just be a natural on Linux Unplugged when we get there.
[3353.68 → 3354.30] How about this one?
[3354.36 → 3357.28] Self-hosting is life came in with 120,000 SATs.
[3357.72 → 3358.18] Good username.
[3358.52 → 3359.12] That is good.
[3359.22 → 3361.20] So sad to see my favourite podcast go away.
[3361.34 → 3364.42] Emptying out my wallet as you guys and the show were the only reason I use SATs.
[3364.58 → 3364.94] Wow.
[3365.20 → 3365.58] Thank you.
[3365.94 → 3367.96] I appreciate your need and work-life balance.
[3368.34 → 3369.34] Thank you for all the great years.
[3369.42 → 3371.70] Since it sounds like you're going to do the occasional self-hosting spot on UP,
[3371.80 → 3375.42] is there a way that you can include only those episodes in this feed so we don't miss them?
[3375.52 → 3376.12] Thanks again.
[3376.58 → 3377.84] We're missing you every other Friday.
[3378.22 → 3379.40] You could just listen to UP.
[3379.56 → 3380.58] I mean, that's an option.
[3381.14 → 3382.60] Yeah, yeah, that's true.
[3382.98 → 3384.02] It is something we've considered.
[3384.20 → 3388.32] The problem is that if you wanted to go back and listen to the back catalogue,
[3388.32 → 3392.30] it's nice to be able to grab the RSS feed and just have 1 to 150 there.
[3392.48 → 3394.70] And it's like an archive piece.
[3395.06 → 3396.90] And if we start putting other stuff in there,
[3396.90 → 3398.54] I don't know if that wrecks it or not.
[3398.70 → 3401.78] I guess I'd be open to feedback on that, but I'm inclined not to.
[3401.88 → 3405.98] I think one thing we could do is just be diligent at tagging those episodes with self-hosted.
[3406.04 → 3410.24] And you can use the tags to pull up just the episodes that are on topic.
[3410.52 → 3413.80] We are pretty on our tag game, so we could definitely do that.
[3413.90 → 3414.34] Tag monsters.
[3414.68 → 3415.72] Thank you, self-hosting is life.
[3415.72 → 3417.04] Really appreciate that generous boost.
[3417.18 → 3420.46] And thanks for taking the sat journey to chat with us.
[3421.14 → 3423.06] SatStacker7 came in with 40,000 SATs.
[3423.14 → 3423.92] Also a great boost.
[3424.40 → 3425.20] Thanks so much for the show.
[3425.20 → 3428.94] Self-hosted was my introduction to Jupyter Broadcasting, now a regular listener of Love 2.
[3429.38 → 3431.94] Looking forward to hearing the self-hosted topics over there.
[3432.24 → 3435.36] I have a question regarding tail scale, and I'd love your input.
[3435.52 → 3438.28] I run multiple services on one single server.
[3438.58 → 3443.42] At the moment, I can access them on different ports using machine name colon port.
[3443.76 → 3448.10] However, I'd much rather use subdomains to not have to remember all these ports.
[3448.74 → 3450.02] Is there a way, Alex?
[3450.02 → 3450.84] Is there a way?
[3450.84 → 3456.28] So you know how Linus does his investment disclosure before any time he mentions framework or anything like that?
[3456.66 → 3460.68] I should do an employment disclosure any time before I mention tail scale.
[3460.90 → 3468.14] Because there was someone getting butt hurt in the comments of a Reddit thread the other day that Alex guy just talks about tail scale non-stop.
[3468.94 → 3474.26] You guys, I spend so much time deliberately not talking about tail scale.
[3474.26 → 3477.72] It genuinely has been a really difficult balance to strike.
[3477.90 → 3480.04] So I think for most of you, we've done an okay job.
[3480.10 → 3481.28] Obviously, we can't please everybody.
[3481.98 → 3484.78] But to answer this question, TSD proxy.
[3485.26 → 3486.10] Look up that project.
[3486.22 → 3487.18] It's a community project.
[3487.44 → 3490.62] And it essentially acts as a reverse proxy for your tail net.
[3491.28 → 3491.48] Nice.
[3491.68 → 3492.64] That'll make it real easy.
[3493.14 → 3502.20] Yeah, this is one of those, I think, just go with that solution, stack stacker, because there are so many ways you can solve this from, you know, Nginx up.
[3502.20 → 3503.76] So that's probably the place to start.
[3504.26 → 3505.08] Thank you for that boost.
[3505.56 → 3506.84] I need to go and put my soapbox away.
[3506.92 → 3509.10] I kind of got out my soapbox for a second then, didn't I?
[3509.14 → 3510.24] No, it's the last few episodes.
[3510.36 → 3511.06] You got to get it out, man.
[3511.16 → 3511.70] You got to get it out.
[3511.76 → 3512.30] I suppose so.
[3513.48 → 3517.22] Outdoor Geek comes in with 5,000 stats, who we met at Linux Fest Northwest.
[3517.44 → 3517.92] Sure did.
[3518.26 → 3522.84] For a leaky canoe, my home manager config for Firefox, he links that to us, he says,
[3522.90 → 3526.74] I'm sad the show is ending, but maybe it'll give me more time to work on my home lab.
[3526.92 → 3527.34] Take care.
[3529.52 → 3531.56] You could always use more hours to work on your home lab.
[3531.56 → 3532.16] Let's be fair.
[3532.86 → 3536.04] Well, we got 10,000 stats from Mount Bread.
[3537.14 → 3538.54] Definitely not a mountain you want to climb.
[3539.84 → 3542.30] It's a man, sad to see the show.
[3542.46 → 3547.60] And Self-Hosted was the show that brought me into the JB Network, and I look forward to it every other week.
[3547.84 → 3550.84] But thank you for all the great content over the years.
[3551.04 → 3551.96] Well, thank you for listening.
[3552.08 → 3552.48] Thank you for that boost.
[3553.04 → 3553.30] Yeah.
[3553.62 → 3555.88] We couldn't have done this without listeners.
[3556.20 → 3559.26] So, yeah, really, the thanks should go the other way.
[3559.76 → 3560.08] Yeah, really.
[3560.08 → 3567.16] Tristan Onliner came in with a Space balls Boost 12,345.
[3567.32 → 3568.32] That's my luggage code.
[3568.52 → 3568.66] Yep.
[3568.76 → 3569.84] One, two, three, four, five.
[3570.30 → 3570.84] It's genius.
[3570.84 → 3574.92] This show is what introduced me to Jupyter Broadcasting, and I've grown to love the rest of the shows.
[3574.92 → 3582.28] But this one, this is the one that got me into my home assistant box and full-blown networking and server setup for my whole family, and they all use it.
[3582.78 → 3587.36] There's a time for everything, and it's sad to see the show go, but I'm excited to see what you both do in the future.
[3587.36 → 3592.92] There were a lot of boosts that came in with that sentiment, so we couldn't fit them all in the show, but I just wanted to say thank you.
[3593.46 → 3600.06] We had 26 of you stream SATs as you listened, so we stacked 30,453 SATs that way.
[3600.48 → 3608.60] And when you combine that with our big old boosts, the show stacked a total of a very healthy 448,531 SATs.
[3609.28 → 3609.82] Thank you, everyone.
[3609.88 → 3613.32] There are just a couple more episodes to get your goodbye messages in, and we do appreciate that.
[3613.34 → 3616.98] And, of course, we'll try to put all those extra boosts in the boost barn linked in the show notes.
[3617.68 → 3620.98] Thank you, everybody who supported episode 148 with a boost.
[3620.98 → 3631.50] And, of course, huge thank you to our SRE members who do have a special deal to get the Jupyter Party membership at a ridiculously low rate.
[3632.34 → 3633.48] Don't tell anybody else about it.
[3633.62 → 3637.76] But thank you to our SRE members as well for helping make this show possible.
[3638.60 → 3642.32] And don't forget to pick up your limited edition self-hosted merch.
[3642.82 → 3651.32] All the proceeds will go to JB for that, you know, so that hopefully that JB will continue long into the night when self-hosted is a distant memory.
[3652.54 → 3652.94] Yeah.
[3653.12 → 3654.38] Where can people go to find that?
[3654.42 → 3656.08] Is it jupitergarage.com?
[3656.76 → 3656.92] Yeah.
[3657.08 → 3658.22] Oh, I like the way you say it.
[3658.52 → 3658.84] Garage.
[3659.76 → 3660.40] Jupitergarage.com.
[3660.40 → 3664.92] In the opening, I said garage, and I realized I turned into an American halfwit when I said it.
[3664.92 → 3669.04] So, yeah, your garage isn't quite as good as your garage.
[3669.14 → 3669.72] I will say that.
[3670.04 → 3684.78] You know, I might mention the meetup page here at the end like we do just because if by some tiny, tiny, tiny chance everything goes really smooth on this van trip and Brent and I have a little extra time after Sunday next week.
[3684.78 → 3689.78] Sunday as you're listening to this when it comes out, we might throw a meetup up for a dinner or something like that on our way home.
[3689.86 → 3690.42] You never know.
[3690.70 → 3691.34] Total last minute.
[3691.60 → 3692.50] Could be total last minute.
[3692.58 → 3698.94] So the only way you're going to know, and you have to be in the California area, Oregon or Washington, depending on where we do this, meetup.com slash Jupiter broadcasting.
[3699.48 → 3702.76] When we do crazy stuff like that, wherever we are, that's where it usually goes.
[3702.88 → 3704.62] Meetup.com slash Jupiter broadcasting.
[3704.62 → 3717.28] If you'd like to send in your messages, and there have been genuinely too many to fit in the show, as we've said, you can boost in, or you can go to self-hosted. Show slash contact or self-hosted at Jupiter broadcasting.com.
[3717.66 → 3719.46] Lots of different ways to get in touch with us.
[3719.96 → 3720.84] I'm on Mastodon.
[3720.92 → 3723.10] In fact, you can find me at alex.ktz.me.
[3724.12 → 3726.60] Yeah, find me at chrislas.com.
[3726.78 → 3729.74] And you can always find me over at linuxunplugged.com.
[3729.74 → 3731.16] Thanks for listening, everybody.
[3731.38 → 3734.32] That was self-hosted. Show slash 148.
