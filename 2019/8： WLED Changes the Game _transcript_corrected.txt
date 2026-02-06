[0.00 → 5.24] YouTube is such a time sink. I started watching videos about bonsai trees last night, Chris.
[5.64 → 6.64] Wait a minute, Alex.
[6.74 → 7.48] Bonsai trees.
[7.62 → 12.46] There are videos about bonsai trees? No, sir. No, I will not have it.
[12.46 → 23.22] Thing is, right, there are many, many hobbies that over decades, millennia, whatever, have been knowledge passed down from person to person.
[23.22 → 32.08] And I think these days, YouTube is just an incredible resource that anybody can learn anything about anything.
[32.60 → 35.72] And you were saying you went down a new rabbit hole yourself.
[35.72 → 45.28] Yeah, it's funny that you did this because just before we started, I was binging old diesel bus repair videos.
[45.90 → 48.44] How strange is this? So let me tell you about these guys.
[48.44 → 60.58] They're like middle American bros that are just, you know, the most down-to-earth guys that go out into fields and find old broken down buses,
[60.76 → 64.48] like diesel buses that have been parked there from maybe 15 years or whatever.
[64.82 → 67.42] Like the bus I was watching today was from before World War II.
[67.88 → 73.56] And they go fix them all up and get them running down the road to get them to their shop where they can restore them.
[73.56 → 82.30] I suppose that's a good thing about quote-unquote simpler, older technology is there's not going to be masses of electronics and laptops required to fix it.
[82.38 → 84.08] It's all mechanical stuff, right?
[84.42 → 88.68] Yeah, and kind of to your point, I've used YouTube now as a resource for figuring out how to fix my RV,
[88.88 → 96.28] for doing a lot of the home automation little tricks and little things I needed just to figure something out, or even Zelda.
[96.90 → 99.58] I mean, I hate YouTube, but I love YouTube. You know what I mean?
[99.58 → 103.92] Yeah, it's a chronicle of some of the best and worst bits of humanity, I suspect.
[105.22 → 109.00] Well, so it sounds like you have been sucked into several rabbit holes this week then.
[109.32 → 116.64] Yeah, the hard thing for me is like just observing something like that, like bonsai trees is an example.
[116.90 → 122.26] But I don't know why the algorithm decided that Alex wants to learn about bonsai trees this week, but it did.
[122.32 → 123.36] And I clicked on the video.
[123.36 → 126.06] So I guess it was right, the algorithm.
[126.62 → 136.56] And yeah, two hours later, I knew everything about material and wire selection and clippers.
[136.92 → 139.10] It's funny how that works. It's funny.
[139.60 → 142.02] Can I tell you about something I did last week after our show?
[142.26 → 142.76] Yeah, sure.
[142.76 → 150.16] I've decided to take the RV on a project off-grid test drive just to see if the basics would work.
[150.24 → 151.74] Would my camera mounts hold?
[152.42 → 154.14] Would the sensors stay up?
[154.76 → 157.00] How did things work when I actually went offline?
[157.12 → 160.18] Because I've been building all of this to be offline while I'm online.
[160.78 → 162.18] And so I've never really tested it.
[162.46 → 165.88] So I took the RV out on a half-day mini road trip last week.
[165.88 → 169.86] And we found a spot by the river that we took our bus down by the river.
[170.30 → 174.90] And we did a camping kind of just set up for lunch for about an hour and a half.
[175.50 → 176.50] Totally offline.
[176.72 → 177.92] No cellular signal.
[178.30 → 181.68] And there were some positive things I discovered in this test and some negative things.
[181.82 → 185.04] I'm very happy to say my camera and sensor mounts all held.
[185.16 → 189.56] Nothing fell down in the Richter 4 earthquake that we are going down the road.
[190.06 → 192.62] But there was a problem that I didn't catch at first.
[192.68 → 193.20] So I'm that guy.
[193.30 → 193.98] I pull back in.
[193.98 → 195.14] I'm like, look at us.
[195.24 → 196.18] Successful test flight.
[196.88 → 198.74] We also did some other maintenance things on the RV.
[198.90 → 200.76] So I'm feeling like, look at me.
[200.82 → 202.02] I'm taking care of stuff.
[202.10 → 202.94] I'm testing stuff.
[203.00 → 203.64] It all worked.
[203.86 → 204.90] My big plan.
[206.48 → 211.84] Until about the next morning when I realized things in the RV weren't working quite right.
[212.66 → 214.60] And it turns out I have to solve a little problem.
[214.60 → 219.72] When I disconnect the RV from shore power and the lithium battery power kicks in,
[219.72 → 226.94] that transition from shore power to inverter power from the battery causes a real momentary
[226.94 → 228.30] blip in the power.
[229.90 → 232.24] It's not enough to knock the Raspberry Pis offline.
[232.46 → 234.04] All the Raspberry Pis stayed online.
[234.04 → 237.42] But the disks went offline.
[238.00 → 239.90] And I didn't catch it till the next day.
[240.46 → 242.98] So it took me a while to figure out what was going on.
[243.42 → 245.50] And I don't really know how I'm going to solve this problem.
[246.06 → 250.04] Because a UPS would be the obvious solution in a home.
[250.54 → 252.50] But in the RV, a UPS is no good.
[252.56 → 255.88] They freak out when you're running them off of battery via an inverter.
[256.02 → 257.04] They do not like that.
[257.04 → 260.30] Plus, it's a horrible inefficient use of power.
[260.52 → 263.04] You lose it in that conversion just like 40%.
[263.04 → 263.76] It's terrible.
[264.54 → 269.86] So I got to come up with some way to keep power steady and smooth to these Raspberry
[269.86 → 270.92] Pis and their disks.
[271.52 → 273.38] But something that's not a UPS.
[274.12 → 275.78] That's an interesting problem.
[276.12 → 277.46] I'm sat here trying to think of something.
[277.62 → 282.18] And I'm glad that you said UPS is out because that's the obvious thing.
[282.52 → 283.26] Yeah, I've tried that.
[283.26 → 288.18] I even tried like a small little APC one that's really essentially just a portable battery
[288.18 → 289.84] in a UPS housing.
[290.04 → 290.64] Still no good.
[290.82 → 291.92] Do you have an Omni Charger?
[292.00 → 292.78] Am I making that up?
[293.24 → 293.72] No, I don't.
[294.08 → 298.00] It's essentially a UPS with a battery banks mushed together.
[298.80 → 302.42] And this thing might be sufficient for you.
[302.82 → 307.88] I know another route is there are Raspberry Pi hats that have a lithium battery on them.
[308.10 → 310.48] So you power the Pi through the hat.
[310.48 → 313.58] And then the hat provides power via the GPO pins.
[313.94 → 316.00] All right, I'm going to send you a link to this Omni Charge thing.
[316.18 → 317.50] I think you need to have a look at this.
[317.92 → 320.76] It's got a small little OLED screen in it.
[320.76 → 322.78] So it tells you all sorts of cool stats.
[323.44 → 324.58] You got me already.
[325.06 → 330.00] Like, you know, the battery percentage is not just three or four little blink LEDs.
[330.26 → 331.14] It's an actual percentage.
[331.64 → 335.94] It tells you the amount of current and wattage being drawn from the battery in real time.
[335.94 → 341.90] It supports pass-through, so you can charge and withdraw power from it at the same time.
[342.06 → 344.52] The USB ports support quick charge.
[345.30 → 347.58] I don't know what version, but they support quick charge.
[348.16 → 350.14] And it comes in several different sizes.
[350.28 → 353.00] So there's like a 20,000 William version.
[353.58 → 356.20] There are big ones, small ones, all sorts of different things.
[357.24 → 359.60] It has a couple of other cool things.
[359.68 → 362.84] Now, the one that I have, I got as a Kickstarter about three years ago.
[362.84 → 365.86] And mine has an AC inverter built into it.
[366.28 → 370.42] But the newer ones have USB-C out that support power delivery.
[371.16 → 372.74] Oh boy, that's it right there, isn't it?
[373.24 → 374.62] Yeah, I think that's going to be your solution.
[375.36 → 381.98] So this is essentially like the coolest battery bank, like portable battery pack I've ever seen.
[382.08 → 382.92] It's pretty sweet.
[383.34 → 385.34] Have you seen the Big Mother that they make as well?
[385.34 → 393.22] If you scroll down under the Pro Series, there's the Omni Ultimate, which has got like a little solar panel in it, I think.
[394.20 → 395.76] And that's how many?
[395.96 → 397.90] 38,000 William hours.
[399.08 → 401.94] I do remember this from when it was a Kickstarter.
[402.16 → 407.10] I am very happy to see they made it because I was very tempted when it was a Kickstarter.
[407.20 → 410.30] They just kind of came out during that time when I was on a Kickstarter break.
[410.30 → 412.30] Like, this is legit.
[412.42 → 413.10] This is great.
[413.20 → 416.84] And USB-C, I know the Pi 4 requires a slightly higher voltage than normal.
[417.08 → 419.30] But boy, that, all right, Alex, thank you.
[419.34 → 420.24] That might be what I do.
[420.64 → 425.54] I think long term, and I'm just kind of waiting to redo my power system overall.
[425.64 → 428.94] But I think long term, let's just power these things via DC somehow.
[429.32 → 430.62] Just go direct off the batteries.
[430.84 → 432.12] Just get the inverter out of the picture.
[432.44 → 435.00] Well, Omni Charge has a DC out as well.
[435.28 → 436.18] That's great.
[436.18 → 436.94] Okay.
[437.24 → 441.62] So I've actually charged my MacBook with a direct DC to MagSafe cable.
[442.04 → 443.00] And it works just fine.
[443.14 → 447.98] Because you can manipulate the voltage in the firmware using the OLED screen.
[448.38 → 454.32] You can manipulate the output voltage of the DC port just on the Omni Charge.
[454.52 → 455.36] Stop it.
[455.40 → 456.20] You're kidding me.
[456.38 → 456.58] No.
[457.06 → 458.94] I think this is exactly what you need.
[459.00 → 461.28] It's like a UPS that is not a UPS.
[461.82 → 462.90] If that makes sense.
[463.68 → 465.14] How's your wallet been this week?
[465.14 → 467.10] Uh, we're still recovering from the TV.
[467.64 → 468.08] Yeah, I bet.
[468.32 → 469.16] Yeah, that takes a hit.
[469.62 → 470.96] Are you enjoying the hell out of that thing?
[471.34 → 472.34] Oh, OLED.
[472.46 → 479.46] If you are on the fence about buying an OLED versus an LED TV, I think it's genuinely worth
[479.46 → 479.80] the money.
[480.94 → 487.80] It's like an extra thousand or whatever, but it's a lot of money, but it's really, really
[487.80 → 488.30] worth it.
[488.30 → 496.38] It's like, we've been watching a lot of, um, 4K H, uh, high encode video codec or something.
[497.04 → 498.92] H E V C is the acronym.
[499.12 → 499.66] Oh, HVAC.
[499.74 → 499.88] Yeah.
[500.04 → 500.22] Yeah.
[500.40 → 500.60] Yeah.
[501.24 → 501.64] What is this?
[501.70 → 502.68] What does that stand for again?
[502.86 → 506.20] Well, I think it's, uh, just like a newer version of H.264.
[506.28 → 506.52] Essentially.
[506.58 → 507.92] It's like H.265.
[508.68 → 509.62] I could be wrong.
[509.90 → 511.50] Self-hosted. Show slash contact.
[511.66 → 512.64] If you want to correct me.
[512.64 → 517.98] Uh, so I've been watching a lot of, um, Blu-rays that I've been storing for a while
[517.98 → 519.64] through my PlayStation four.
[519.84 → 525.06] And I must say it's really something, you know, if you're watching some of those David
[525.06 → 529.38] Attenborough shows, there was one particular scene we were watching, uh, where he was in
[529.38 → 532.96] doing like heat map cameras of tigers in inner city Mumbai.
[533.74 → 537.34] And the blacks were just as it was as if the screen was off.
[537.50 → 540.12] It's genuinely not, uh, hyperbole.
[540.22 → 541.52] It's, it's really something.
[541.52 → 547.64] So, but now the coolest thing about this TV is that it integrates directly with a home
[547.64 → 548.54] assistant integration.
[549.14 → 549.76] How has that been?
[549.82 → 550.94] So that's what I really want to know.
[551.18 → 551.42] Yeah.
[551.48 → 557.18] I've been going on a huge home assistant binge this week, which we'll get to, uh, well now,
[557.24 → 557.66] I guess.
[558.12 → 558.52] Yeah.
[558.52 → 559.20] Let's do it now.
[559.26 → 561.92] Let's do it now because it really kind of all ties into this, doesn't it?
[562.24 → 562.58] Yeah.
[562.88 → 568.66] There was a new version of home assistant released 0.102, which has a few new interesting
[568.66 → 569.88] integrations in it.
[569.88 → 574.90] Uh, the principal one that I'm looking at is the LED integration.
[575.40 → 580.56] But before we get to that, I'm going to touch on the LG WebOS integration.
[581.40 → 588.00] Now this allows me from my home assistant interface to turn the TV on, turn the TV off.
[588.00 → 588.28] Okay.
[588.36 → 595.56] That doesn't sound that amazing, but it lets me select the input of the TV from home assistant,
[595.56 → 600.34] but it's also contextually aware of what the screen is playing as well.
[601.08 → 605.88] If I'm watching a YouTube video, the title of that video shows up in my home assistant.
[606.26 → 608.74] See, I can do that only with Plex videos right now.
[608.82 → 609.42] Nothing else.
[609.68 → 610.06] So you...
[610.06 → 610.90] Works for Plex too.
[611.36 → 613.58] So WebOS is reporting back.
[614.04 → 615.10] How does it know?
[615.10 → 617.26] I mean, this TV must be watching.
[617.98 → 623.86] Well, you've got to create a developer key or some kind of like, um, API key to let the
[623.86 → 624.78] integration work.
[625.18 → 629.60] But part of the reason that these integrations are so great is that they have knowledge of
[629.60 → 631.98] the APIs that these different platforms use.
[632.16 → 638.12] So they're able to take advantage of API specific features to my specific model number of TV.
[638.68 → 641.34] And this must only work when you're using the apps built into the TV.
[641.64 → 645.76] Well, I can change the input to HDMI, and then it doesn't know what's being played.
[645.76 → 647.54] If I was playing it on the shield, for example.
[648.06 → 648.22] Right.
[648.26 → 650.72] But then it would just tell you in home assistant that you're on that input.
[650.88 → 651.22] Right.
[651.30 → 651.66] Yes.
[651.94 → 656.46] Um, so what that means is I can set up some quite interesting automations now, you know,
[656.46 → 661.72] this is getting to the territory where, uh, it's, it's getting a little bit Iron man,
[661.98 → 665.82] you know, a little bit Tony Stark, where I can just set up a scene, and it will dim the lights,
[666.16 → 668.02] change the lights to a certain colour and brightness.
[668.84 → 674.34] Uh, change the input on the TV and then the TV using audio return channel will turn on my
[674.34 → 676.66] receiver and set that to the correct input.
[677.26 → 681.48] And it, you know, then it will turn off all the lights in the rest of the house that might
[681.48 → 682.94] otherwise reflect in my screen.
[683.84 → 687.82] Uh, it can set the, uh, temperature in the house to a certain level.
[687.82 → 693.60] If I just want to get cozy, you know, it's just a case of thinking about how all these
[693.60 → 699.04] different facets of your house linked together and how you can just create automations that
[699.04 → 700.82] improve your quality of life.
[701.14 → 705.62] If you had had this conversation with me eight years ago, I would have thought you
[705.62 → 707.24] were being a silly, fussy man right now.
[707.24 → 709.82] Um, you know, turn off some lamps.
[709.90 → 710.34] You're good to go.
[710.40 → 713.64] How much effort does it take to walk around, flip off a few light switches?
[713.90 → 717.56] By the way, these lamps probably would have had fluorescent bulbs in them back then.
[717.56 → 719.46] And I just would have said, you know, what's the big deal?
[719.46 → 726.52] Um, but now having gone deep into this with my own home assistant setup and my own smart
[726.52 → 732.12] light solutions, it, it feels like it has, it has made our home feel more like a home.
[732.20 → 733.12] It's feels cozier.
[733.42 → 734.14] I don't know.
[734.22 → 739.22] It's, I was surprised by what a difference it made in, in the feel of the place.
[739.22 → 743.52] And I, I don't think, I don't think I would have appreciated that as much had I not just
[743.52 → 744.28] given this a go.
[744.28 → 752.20] And I sometimes think, uh, home automation is conflated with remote control unfairly.
[752.88 → 757.74] Um, remote control is just the beginning, you know, being able to turn that lamp on and
[757.74 → 766.04] off is, is fine, but it's when you start integrating everything in one place that it's the magic really
[766.04 → 766.86] starts to happen.
[767.26 → 767.36] Right.
[767.46 → 772.28] If you want just to remote control a light, get yourself a clapper job done, right?
[772.28 → 773.94] We're not trying to make clapper 2.0 here.
[773.94 → 777.04] We're trying to actually make your home contextually aware.
[777.20 → 779.62] And that's why the integration with the TV is so key.
[779.66 → 784.74] Because I assume you must be able to kick off automations based on the sensor data from the
[784.74 → 785.14] television.
[785.50 → 787.50] So you can have that stuff happen automatically.
[787.64 → 791.86] When you switch to an input, you could have those lights change without, I mean, it's not
[791.86 → 793.56] even like something you have to invoke, right?
[794.00 → 794.70] That's a good point.
[794.76 → 794.96] Yes.
[795.04 → 799.18] Because, you know, home assistant has the concept of sensors built into it.
[799.18 → 802.88] So there are entities, which are things like my light bulbs and the TV.
[803.60 → 808.12] Um, but then each of those things report back to home assistant to say what their current
[808.12 → 808.88] status is.
[809.18 → 812.06] You can then use that sensor information.
[812.56 → 816.52] Maybe it's a binary sensor that something's either on or off, or maybe it's a temperature
[816.52 → 822.42] sensor that something or, or a humidity sensor, uh, that's returning a certain value.
[822.42 → 827.86] And then you can have home assistant constantly reacting to those sensor inputs.
[828.50 → 832.72] Um, and very quickly you end up with a complex house of cards.
[832.72 → 833.14] Sure.
[833.24 → 835.48] But it's actually very easy to, to manipulate.
[836.10 → 841.58] So the other change that I've made this week is that I've switched from a Docker container
[841.58 → 846.42] on my Ubuntu system to has IO.
[846.92 → 847.40] Okay.
[847.40 → 853.60] So I was wondering what led to this because I have debated this a lot because there's
[853.60 → 858.64] a lot of advantages to using has IO versus vanilla home assistant.
[859.48 → 865.36] And just briefly, I would, I would describe the home assistant version that I have installed
[865.36 → 867.66] as vanilla using the Docker image.
[867.66 → 871.80] And it's just the project with no plugins, no add-ons.
[871.80 → 879.48] Has IO is more of a community spin that has some plugins that are very easy to install,
[879.66 → 881.68] but it's a much broader thing.
[881.82 → 883.34] It's, it's more than just a core project.
[883.44 → 885.38] And I just, I debate that.
[885.94 → 887.00] I'd say it's a platform.
[887.30 → 889.58] Has IO is, is the home assistant platform.
[889.96 → 893.22] And what made you decide to switch from vanilla to the platform?
[893.22 → 895.02] Well, I was browsing YouTube, Chris.
[895.78 → 896.66] I knew it!
[896.90 → 901.82] And, uh, you know, there's that Dr. Z's guy that releases a million YouTube videos a week.
[901.92 → 903.34] I don't know where he finds the time.
[903.56 → 904.26] I think it's all he does.
[905.12 → 909.28] And, and he's, he's just browsing around going into the has IO store and installing,
[909.28 → 911.86] you know, add-ons left, right, and centre.
[911.86 → 914.90] And I'm like, why am I not doing that myself?
[914.94 → 916.94] It just, that just looks like too much fun.
[917.28 → 921.22] So which plugin though, there must've been a plugin or two that said, okay, this is worth
[921.22 → 926.78] the hassle because I've reviewed those plugins, and I've thought to myself, eh, not quite
[926.78 → 927.24] worth it.
[927.56 → 928.00] There's a few.
[928.28 → 932.90] So, um, the, the main one for me was the VS Code plugin.
[933.72 → 939.94] You can direct from the home assistant interface, click a button that lets you load up visual
[939.94 → 946.00] studio code in the same browser window that has syntax, auto-completion and highlighting
[946.00 → 948.72] directly supporting home assistant.
[948.72 → 953.56] So if you, if you start writing an entity, um, in the configuration file, it will tell
[953.56 → 956.00] you that you've missed the required field or something like that.
[956.36 → 957.80] That's so slick.
[958.40 → 963.14] So it's a visual code, Visual Studio code editor for home assistant.
[963.28 → 963.84] Pretty much.
[963.96 → 964.16] Yeah.
[964.40 → 970.14] It's just a normal VS Code instance under the hood using the, uh, there's a container that
[970.14 → 971.52] you can run VS Code in.
[971.52 → 977.32] And I think they're just using that under the hood because if you log into the, um, appliance
[977.32 → 982.36] that's running home assistant now, um, under the hood, and you do a Docker PS, it's just
[982.36 → 984.34] running a dozen containers under the hood.
[984.52 → 988.32] So home assistant on has IO is still running in a container.
[988.52 → 990.22] You're just abstracted away from it.
[990.36 → 995.72] Well, so this is why I thought to myself, I said, you know, Chris, if you ever really had
[995.72 → 999.08] to have one of these plugins, you could just go get that container.
[999.88 → 1002.02] Couldn't I just run that container?
[1002.74 → 1007.40] Of course you could, but you have to go and, I mean, it's, it's a very small barrier to
[1007.40 → 1010.84] entry, but you know, you have to add that to your compose file.
[1011.22 → 1015.64] You got to configure then all the plugins in VS Code to be compatible with home assistant,
[1015.96 → 1018.92] set up the remote access, blah, blah, blah, blah, blah.
[1019.06 → 1022.34] And I don't get to just browse a repo and just hit install either.
[1022.34 → 1022.90] Yeah.
[1023.10 → 1029.90] Now the other thing that is often overlooked with UI based stuff is discoverability.
[1030.44 → 1037.46] So in the, uh, has IO add-on store, there are only nine or 10 plugins.
[1038.06 → 1039.58] Tasso admin is a really cool one.
[1039.66 → 1042.48] I've also been using to update all of my Tasso to devices.
[1043.10 → 1044.46] ESP home is another cool one.
[1044.60 → 1052.32] It allows you to configure single board like node MCU ESP 8266 type ESP
[1052.32 → 1055.82] devices, uh, with only a few lines of YAML.
[1056.04 → 1057.78] That thing is super-duper cool.
[1058.30 → 1059.72] There's node red in there as well.
[1059.82 → 1062.04] And add guard home built right into home assistant.
[1062.44 → 1065.74] Um, but the, the main one that I saw Dr.
[1065.84 → 1068.56] Z's using, uh, is something called hacks.
[1068.76 → 1074.04] Now this is home assistant community store, and this is nothing to do with like a
[1074.04 → 1076.04] has IO necessarily this.
[1076.20 → 1080.78] You could install this on any home assistant instance, but home assistant community
[1080.78 → 1083.52] store is what it sounds like.
[1083.60 → 1089.84] You give it a GitHub personal access token, and then it will go and crawl GitHub for every
[1089.84 → 1093.64] GitHub repo with a certain label or a certain tag.
[1093.72 → 1096.42] I don't know exactly how it works, but it's amazing.
[1096.76 → 1096.82] Yeah.
[1096.82 → 1100.76] So that's at hacks.xyz, H-A-C-S dot X-Y-Z.
[1100.86 → 1102.66] I will throw a link in, in our show notes.
[1103.24 → 1104.74] This is really cool looking.
[1105.12 → 1105.82] Oh man.
[1106.00 → 1107.44] I kind of want to get this set up.
[1107.84 → 1111.42] There are hundreds of things in GitHub that you would never have found otherwise.
[1111.42 → 1114.30] And this thing will crawl the APIs and find them for you.
[1114.60 → 1117.38] So it sounds like you've been using the hell out of this thing to manage a bunch of the
[1117.38 → 1119.54] stuff you've, I mean, a lot of that is right up your alley.
[1119.84 → 1120.16] Yeah.
[1120.50 → 1123.86] What was the migration like from home assistant vanilla to HAS IO?
[1123.86 → 1125.78] No, I'm rebuilding from the ground up.
[1125.92 → 1128.30] Oh my God.
[1129.18 → 1130.22] Oh God.
[1130.40 → 1135.22] Well, I mean, in January, which is when I started with home assistant, I didn't know what on
[1135.22 → 1136.10] earth I was doing.
[1136.52 → 1142.44] Some would argue I still don't, but I'm a little more familiar with the situation now than I
[1142.44 → 1142.94] was then.
[1143.68 → 1148.80] We mentioned a little earlier that one of the new integrations I was most excited about
[1148.80 → 1150.22] was something called LED.
[1152.16 → 1153.76] Now, why is that exciting, Alex?
[1153.76 → 1161.56] Well, in my Linux Vest Northwest talk, I built a smart set of LEDs that were using MQTT.
[1161.80 → 1163.28] In fact, we talked about it last episode.
[1165.14 → 1168.08] MQTT is wonderful for contextually aware stuff.
[1168.24 → 1172.74] So, you know, the LED controller knows what home assistant's up to and vice versa.
[1173.98 → 1180.60] But LED's better because it's a native home assistant API integration as opposed to MQTT,
[1180.60 → 1182.44] which sort of sits on top as another layer.
[1183.12 → 1186.38] That alone means that the performance is better.
[1187.06 → 1194.94] But couple it with the fact that the LED developer provides a pre-compiled binary that you can just
[1194.94 → 1200.14] flash with ESP tool in about 10 minutes end to end.
[1200.14 → 1202.68] And it's just wonderful.
[1203.28 → 1203.34] Okay.
[1203.62 → 1204.72] That does sound really nice.
[1204.92 → 1205.56] Super quick.
[1205.64 → 1206.46] So you're getting a new device.
[1206.52 → 1207.14] Not a big deal.
[1207.54 → 1207.80] Yeah.
[1208.06 → 1210.68] So there have been two traditional ways to do it.
[1210.76 → 1217.54] One is the custom Arduino code, which is what I did, which I used the BYU automation stuff.
[1217.54 → 1222.02] And the other was ESP home, which is why I installed it and started looking at it this week.
[1222.66 → 1233.36] And with ESP home, you gain simplicity of configuration, but you lose configurability for things like effects and that kind of thing.
[1233.36 → 1239.42] But with LED, if you really want to go in and change, you know, like the data pin or something like that,
[1239.46 → 1244.14] let's say you've got a node MCU that's got four or five sensors on it, as well as controlling your LEDs.
[1245.22 → 1251.14] You can go in and compile a custom firmware just the same as you could with the custom Arduino code that I was using before.
[1252.02 → 1254.70] Or you can just flash the pre-compiled binary.
[1255.04 → 1256.46] It is amazing.
[1257.14 → 1258.00] That is really handy.
[1258.76 → 1262.04] There are all kinds of great ideas on the site to ESP home.io.
[1262.04 → 1267.12] Now, I read a blog post about LED this week, which we'll put a link to in the show notes.
[1268.16 → 1277.96] And essentially, for $16, you can build yourself a smart LED strip that is fully compatible with Home Assistant that you own completely.
[1278.70 → 1279.34] Really nice.
[1279.64 → 1281.20] Those things, I mean, $15?
[1282.70 → 1289.98] I mean, you can get some really crappy LED strips for around that price on Amazon, but not ones that are fully automated.
[1289.98 → 1294.00] So this thing, I guess it joins your Wi-Fi, and then it starts communicating.
[1295.92 → 1297.34] How much...
[1297.34 → 1301.60] Give a fair description on the quality of those LEDs, though, when we're talking.
[1301.64 → 1305.74] Because, like, that's a big thing with LED lights is the quality of light that they give off.
[1306.26 → 1313.04] Some of them are less good than others, but that depends entirely on the LED strip themselves that you buy.
[1313.30 → 1315.80] I mean, are you including that in the cost when you say $15?
[1315.80 → 1328.66] Well, yeah, a 300-long LED strip with 300 pixels, so that's one microcontroller per LED, is $28 on Amazon.
[1328.92 → 1329.16] Okay.
[1329.64 → 1330.30] Oh, that's all right.
[1330.30 → 1340.56] So the reason I said $16 was because I generally only put $20 or $30 off a single microcontroller, because I, you know, I want small mood lighting.
[1340.66 → 1342.98] I don't necessarily want a whole long strip.
[1343.18 → 1346.74] If you're going to do a long strip, I would go with a 12-volt LED strip.
[1346.92 → 1348.90] These, in particular, are 5-volt.
[1349.74 → 1353.36] And why that's particularly nice is you don't need any buck converters or anything like that.
[1353.40 → 1355.62] You can just plug it straight into USB, and you're good to go.
[1355.62 → 1357.28] Here's a little comparison.
[1357.92 → 1366.96] The TP-Link NASA Smart LED strip lights is what they call them, which are 6.6 feet long, $70.
[1367.64 → 1368.24] Wow.
[1368.86 → 1369.46] Yeah.
[1369.86 → 1372.60] And that's using, obviously, with their cloud service, too.
[1373.24 → 1379.50] It's probably, NASA generally stuff works pretty well with Home Assistant, but just to kind of give you a comparison.
[1379.78 → 1384.10] So if you wanted to do a lot of LED lighting, that really adds up.
[1384.10 → 1388.92] And that's kind of the great thing, is like, if you can do it at that price, you could do a lot of it.
[1389.28 → 1389.48] Yes.
[1389.70 → 1389.88] Yeah.
[1390.16 → 1391.02] You absolutely can.
[1391.60 → 1394.76] Now, I'm not quite finished talking about how awesome LED is yet.
[1395.70 → 1397.02] So you flash the firmware.
[1397.62 → 1408.88] And then what makes this way better than anything that I've used before is that it turns your Node MCU or your D1 Mini into a mini wireless access point.
[1408.88 → 1419.88] You then connect to that with your phone, navigate to an IP address in your browser, and then you can configure everything about the LED strip straight from your phone.
[1420.48 → 1427.22] You don't need Home Assistant necessarily because they also make an official LED app for Android and iOS.
[1427.22 → 1432.74] So I was looking through the firmware, and there's a bunch of super cool stuff in here.
[1433.52 → 1436.72] And bear in mind, this is running off a $6 microcontroller.
[1437.22 → 1437.62] Okay.
[1437.76 → 1446.28] It will integrate natively with Philips Hue, with Blink, with MQTT, with Alalaxalala.
[1447.34 → 1448.52] That's how you do it.
[1448.66 → 1451.16] I try not to set it off for people, but I probably do.
[1451.16 → 1451.90] Your Echo devices.
[1451.90 → 1457.66] And then you can go in and configure the specific number of LEDs that you have.
[1457.86 → 1460.36] It does current-current estimation.
[1461.02 → 1464.28] So it will say, like, you're using 150 Williams right now.
[1464.56 → 1466.38] You've got to really watch it with those LED lights, Alex.
[1467.78 → 1469.34] Some of them, actually, you do.
[1469.60 → 1475.06] So there are some microcontrollers that can draw up to 30 watts on the whole strip just on idle.
[1475.66 → 1477.68] So you do have to pick them with care.
[1478.08 → 1480.30] These I picked so that they're fine.
[1480.30 → 1487.10] There's a video from a guy called The Hookup on YouTube, and he goes through all the different types of LEDs, which we'll put a link to in the show notes.
[1487.88 → 1493.10] He goes through all different types of LEDs and their phantom current drawer and all the rest of it.
[1493.26 → 1503.12] So, you know, there are some things you've got to be aware of, but I just can't overstate how excited I am by LED and Home Assistant this week.
[1503.12 → 1511.08] Like, I haven't been this excited about a project, and I'm talking about Home Assistant here, since I discovered Docker for the first time.
[1512.08 → 1514.60] What specifically do you think this week brought that up again?
[1514.66 → 1517.36] Because I've been feeling that way a lot.
[1517.36 → 1524.92] I think for me, it's just that I think to myself, I wish I could integrate with this, or I wish I could control that.
[1525.50 → 1526.72] I go and look for it, and it's there.
[1526.86 → 1527.64] It's already there.
[1527.74 → 1528.54] Someone's already done it.
[1528.72 → 1537.18] And there are products I've been looking about maybe buying, like some KEF speakers maybe, that have, like, the KEF LS50 wireless speakers.
[1537.18 → 1543.20] There's a native integration already there in Home Assistant for these speakers I don't even own yet.
[1543.30 → 1550.66] And it's like, it just feels to me like I was watching the State of the Union Home Assistant YouTube video.
[1550.94 → 1552.00] I spend a lot of time watching YouTube.
[1552.10 → 1552.62] Are you getting that?
[1552.90 → 1553.62] I'm noticing that.
[1553.68 → 1554.08] It's a theme.
[1555.64 → 1560.96] And just looking at the excitement of these people who are actively working on the project.
[1560.96 → 1565.98] It's in the top 10 in the Octobers for contributors of all GitHub projects.
[1565.98 → 1568.40] It's up there with Ansible and Kubernetes, for crying out loud.
[1569.06 → 1577.46] It just feels to me like everybody is waking up to the fact that having an open home automation system is just awesome.
[1577.68 → 1578.54] And I love that.
[1578.94 → 1587.52] And I think it's also compounded by all these different manufacturers have their own apps and their own cloud services that are all their own silos.
[1587.52 → 1591.12] And it's nice to have something that can aggregate and bring them all together.
[1591.12 → 1597.70] On top of that, it's sort of like the deal is changing constantly on these devices.
[1598.14 → 1605.02] You and I were just recently discussing that Waze had to announce they're removing person detection from their cameras.
[1605.02 → 1616.18] So I bought this last round because I was really impressed that Waze managed to develop on-camera person detection on a $25 camera.
[1616.28 → 1617.14] I was like, all right, I'm in.
[1617.98 → 1618.72] Well, I got an email.
[1619.10 → 1626.60] It says they have to pull that because the company they partnered with to develop that AI on the edge devices has exercised a clause in their contract.
[1627.34 → 1631.80] And Waze has to ship out firmwares now that removes that feature.
[1631.80 → 1636.54] What's that going to mean for you and I who are running the custom RTSP firmware?
[1636.82 → 1641.80] Well, this is back to my main point is I feel like I'm insulated from these types of changes.
[1641.80 → 1647.90] When a company decides they can no longer support feature A or product Y, I'm not impacted by that.
[1647.94 → 1651.10] Because the way I have my system set up is I've flashed it with that RTSP firmware.
[1651.22 → 1652.84] And I'm leaving that firmware, Alex.
[1653.76 → 1654.84] I'm not changing it.
[1654.88 → 1658.20] I've configured my network to record everything to the Pi locally.
[1658.20 → 1662.94] I don't use the cloud service and I actually have everything blocked at the DNS level.
[1663.02 → 1665.16] So they can't even communicate with the Waze service.
[1665.54 → 1666.38] Oh, good man.
[1666.66 → 1666.88] Yeah.
[1667.18 → 1667.36] Yeah.
[1667.42 → 1669.64] I'm leaving it, and then I'll let them sort it out.
[1669.70 → 1678.78] They say they will try to add person detection back in 2020, but it's going to be cloud-based likely and not on the camera.
[1679.14 → 1682.96] And I much prefer on camera because then it's in my actual recordings too.
[1683.44 → 1684.74] Maybe I'm missing something here.
[1684.74 → 1690.20] Why do they need an API for motion detection if it's on camera?
[1690.80 → 1693.62] It won't be with the new system is what the implication is.
[1693.96 → 1694.72] No, but right now.
[1694.82 → 1698.84] So how can they pull a feature that's local?
[1699.50 → 1700.54] That's what I don't understand.
[1700.92 → 1703.88] Their new firmware will remove the functionality.
[1704.28 → 1707.24] So they license the tech to do the person detection.
[1707.24 → 1713.62] Because to get it working on these incredibly low-powered cameras, it was like a feat of engineering.
[1713.86 → 1716.74] It was something that Waze was extremely proud of.
[1717.42 → 1720.14] And it's kind of like the tech that can do it.
[1720.36 → 1727.92] And there's really nobody else that's developed person detection, human object detection that can run on processors that slow.
[1727.92 → 1735.14] So do we think that we'll be able to still buy those Waze cams for the next year or two and flash that?
[1735.30 → 1736.52] That's a great point.
[1736.88 → 1742.98] I bet you if you bought them within a certain time frame, they would probably ship with the person detection firmware.
[1743.32 → 1747.90] Yeah, but even if they don't, maybe we can install the current RTSP firmware that you and I have.
[1748.26 → 1751.42] Yeah, I did save it offline just in case it ever disappeared.
[1751.66 → 1752.50] Yeah, good idea.
[1752.78 → 1753.54] So it's possible.
[1753.54 → 1757.50] I wonder if you go too far ahead, though, in the firmwares if you can't go back.
[1758.34 → 1763.54] You know, say it's down the road, it's firmware 1.8 and the RTSP is like version 0.9.
[1763.66 → 1765.20] Maybe that could be a challenge.
[1765.28 → 1768.52] So it may be worth, if you've been on the fence, just pulling the trigger now.
[1769.02 → 1772.08] Not to change the topic, but just for a second, it's crossed my mind.
[1772.78 → 1776.24] It's funny how these things we do, like I'll get a new TV.
[1776.56 → 1779.28] Or for me, it was I want to solve heating problems.
[1779.28 → 1784.40] They just spiral into a bigger and bigger project.
[1784.64 → 1786.68] And if you're willing to do it, it can be some of the most fun.
[1787.20 → 1788.14] So I'm totally on board.
[1788.54 → 1789.80] Just a big shout-out to Home Assistant.
[1789.88 → 1793.54] We've talked a lot about it recently, but it's just because we are so elated about it.
[1794.02 → 1796.02] What do you say we do in Ask SSH to round us out?
[1796.28 → 1796.78] Let's do it.
[1797.10 → 1797.36] All right.
[1797.48 → 1798.12] Kai wrote in.
[1798.20 → 1798.62] He says, peeps.
[1799.96 → 1801.28] Kai calls us peeps, Alex.
[1801.28 → 1813.32] Hey, peeps, if I wanted to set up a simple AI-based Media Centre Raspberry Pi with an external SSD drive connected to a TV via HDMI, or HDMI as you would say.
[1813.42 → 1814.88] Jerry's triggered right now.
[1815.68 → 1822.52] Would a Raspberry Pi 3B with one gigabyte of RAM, one gigabyte, be powerful enough to do that?
[1822.96 → 1824.18] He says, because I have a spare one.
[1824.22 → 1826.84] Or is it time to get a new Raspberry Pi 4?
[1827.78 → 1830.40] I think it's on the edge, actually, to be honest with you.
[1830.40 → 1831.62] On the edge for what?
[1831.70 → 1838.16] Because direct play, the Pi 3 will do most anything, even 4K, H.265, right?
[1838.56 → 1841.12] Yeah, Pi 3 with video drivers would.
[1841.68 → 1844.60] It's generally the bit rates that start to be an issue.
[1844.96 → 1856.06] However, if you're looking at standard 720p content, or if you're 1080p, and it's stuff that's below 15 megabits, I think the Raspberry Pi 3 with Jodi would kill it.
[1856.12 → 1856.64] It'd be great.
[1856.64 → 1861.18] It would eat through that stuff, no problem, especially if you're feeding it via an SSD on USB 3.
[1861.68 → 1868.12] And you know the thing, Kai, that I would say here is you already have one, so it would take you about 10 minutes to find out if it's suitable.
[1868.12 → 1877.32] So if you're like Alex over here, and you're rocking 4K, and you want high bit rate, you want, you know, really good-looking picture.
[1877.50 → 1886.24] I would be tempted then at that point to throw in for a Pi 4 because looking at your overall setup, the Raspberry Pi 4 is going to be like the least expensive aspect of it.
[1886.50 → 1887.78] It's still even cheaper than the SSD.
[1887.78 → 1890.96] But like Alex says, I mean, give it a go with the 3.
[1891.16 → 1899.76] If you're not looking at ultra-high quality, high bit rate stuff or even serving to multiple people, if you don't plan to install like Jellyfin or Plex, Pi 3 is going to kill it.
[1899.90 → 1912.94] If you wanted to go up a notch, and you wanted to do something like Jellyfin and Jodi, which is a nice little Sumbawa, and you wanted to do it to a couple of TVs in your house, that's when I'd probably go over to a Pi 4.
[1912.94 → 1915.60] What's crazy, you can do it with either one though.
[1915.70 → 1916.80] I mean, that's where we're at today.
[1917.26 → 1918.48] Yeah, it is crazy.
[1918.96 → 1926.70] But one important hardware difference, of course, is that the Pi 4 uses the mini or micro HDMI cables.
[1927.18 → 1931.14] So you'll need a dongle for that versus the Pi 3.
[1931.66 → 1932.80] Yeah, yeah, you're right.
[1932.94 → 1933.08] Jeez.
[1934.14 → 1938.14] Of course, the other advantage would be, so that's the dongle's a downside.
[1938.14 → 1943.44] The advantage is you get better throughput to that disk on that USB 3 bus.
[1943.84 → 1946.54] Yeah, because there are two things at play here.
[1946.66 → 1948.76] They've finally separated out on the Pi 4.
[1949.42 → 1953.56] The Ethernet and the USB at last are on different buses.
[1954.20 → 1955.34] At last, at last.
[1955.44 → 1956.06] Freed at last.
[1956.10 → 1957.16] And it makes a big difference.
[1957.46 → 1960.36] And then the other difference is the Pi 4 has USB-C.
[1960.92 → 1963.86] So you might need different cable or a better power supply.
[1963.86 → 1973.18] And then the only other thing I would sort of, it's not a word of caution, it's just something to be aware of, is the Pi 4 gets kind of toasty.
[1973.80 → 1975.32] And I'm going to add on to that.
[1975.62 → 1980.30] Even though I'm running three of them and I absolutely love them, it's early days still.
[1980.30 → 1994.00] One of the Liberec project, which is a really slick way to do a media centre on a Raspberry Pi, is just within the last couple of weeks rolling out early support for the Raspberry Pi 4.
[1995.02 → 1999.84] And, you know, that's something to consider because the Raspberry Pi 3 is solid at this point.
[2000.38 → 2009.72] I've been looking around and trying to find a good answer whether it supports the newer HDMI 2.x standards, but it looks like both are only 1.4.
[2010.52 → 2015.42] If I'm wrong with that, please write in with self-hosted. Show slash contact and let me know.
[2015.94 → 2015.96] Yeah.
[2016.38 → 2017.40] Or do like I did.
[2017.80 → 2021.10] Hashtag Ask SSH on Twitter or in Telegram.
[2021.50 → 2023.52] We're always lurking and collecting those.
[2023.94 → 2029.84] I've done a neat thing on Twitter where I've taken the hashtag Ask SSH, and I've plugged that into Feebly.
[2030.06 → 2032.80] And Feebly supports just treating it like an RSS feed.
[2033.04 → 2035.34] So when somebody posts it, it shows up in my feeds.
[2035.56 → 2036.12] Oh, that's cool.
[2036.16 → 2036.74] I should do that.
[2036.86 → 2038.36] I've got an if this, then that integration.
[2038.36 → 2039.96] We are such nerds.
[2040.68 → 2042.54] I might do a Feebly.
[2042.80 → 2043.48] That sounds good.
[2043.96 → 2044.26] All right.
[2044.32 → 2047.52] Well, Alex, I am super excited to hear about your future adventures.
[2047.86 → 2053.68] I've been really tempted to try out Has.io, and you may push me over.
[2053.96 → 2054.28] We'll see.
[2054.28 → 2057.30] And that's been self-hosted. Show slash eight.
[2057.30 → 2066.94] We'll see you next time.
[2066.94 → 2069.10] We'll see you next time.
