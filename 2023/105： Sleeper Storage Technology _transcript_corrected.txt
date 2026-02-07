[0.00 → 8.14] Here we are in episode 105 of the Self-Hosted Podcast, and it is feeling officially like the end of summer.
[9.00 → 12.14] My two youngest have gone back to school. It's the first day of school today.
[12.68 → 18.12] You only say that because you live in the frozen north. It was 97 degrees down in Raleigh today.
[18.56 → 23.06] Okay. Yeah, actually, you know what's funny? Last night on a whim, I pulled up Raleigh because I have like,
[23.12 → 27.58] I have like everywhere the hosts are at stored in Carrot. And so I was on Carrot Weather. I'm like,
[27.58 → 34.40] let's check in on everybody. It's like, whoa, Alex. Yeah, it's 68 degrees and blue skies here.
[34.82 → 38.86] I'll take it. But it makes me a little sad when summer comes to an end because I always picture
[38.86 → 44.82] summer as like, I'm going to get all these projects done. Yeah. Do you think that stems from
[44.82 → 51.64] summers at school as a kid feeling like they stretch in front of you forever, except as an adult,
[51.64 → 57.74] life is in the way? Yeah. You get that. And also for me, it's like, well, I'm going to have more
[57.74 → 63.44] daylight. So if the sun's going to be up till eight or nine o'clock, I should be able to get like twice
[63.44 → 68.70] as much stuff done. That should happen. Right. So, all right, I'll plan like my big thing. And I got
[68.70 → 75.62] close. Was I, I really started for a moment with Brent's help to wrap my head around all the different
[75.62 → 82.40] ways. I could improve the RV and the studio with ESP devices, modules, and just little things that
[82.40 → 88.08] I could get like the sonar module or relay, you know, controls and temperature sensors and moisture
[88.08 → 93.14] sensors and all these little things I wanted to do for LEDs, where I wanted to add a few more LEDs
[93.14 → 99.14] controlled by an ESP. And I got a lot of the kits together. I got various parts. I got some LED light
[99.14 → 105.42] ropes. I got some relays and then just sort of lost momentum on all of it. And I thought by the end of
[105.42 → 109.82] summer, I'd have, I'd have like these lights installed, and I'd have some stuff implemented and
[109.82 → 114.14] nope, I didn't get to it. Not at all. So I feel a little bad about that.
[114.56 → 121.20] I think the trouble with some of those sort of more DIY projects, like the ESP based stuff
[121.20 → 129.24] is a lot of the times you don't know every single little piece of the jigsaw that you need until you
[129.24 → 135.26] start getting into the project. And then inevitably you do the calculus of, well, it's $15.
[135.42 → 141.98] on Amazon for this thing, or it's $4 on AliExpress for the exact same thing. Do I just wait three
[141.98 → 147.84] months for it to arrive on the slow boat or do I pay the Amazon tax? And that can be the biggest
[147.84 → 152.84] impediment for me to finishing some of these more bitty projects, some of the ESP stuff.
[153.76 → 158.54] So I took the route. I recently ordered something called an ESP clicker. In my bonus room above my
[158.54 → 164.50] drum set, I have a Skylight with an automated Flux blind motorized solar-powered blind in it.
[164.98 → 168.86] And it has a remote control, an RF remote control. I think I've mentioned it on the show before,
[169.20 → 174.48] which is paired with that blind. And I don't really want to go about hacking the RF protocol
[174.48 → 179.98] because the Flux blinds have some kind of encryption key rotation nonsense in them, which means
[179.98 → 189.14] not random strangers can't control my blinds, which is nice. But also do we care? But okay,
[189.54 → 189.70] fine.
[189.70 → 195.32] Not for that particular Skylight, probably not. And it, yeah, this is interesting because this is
[195.32 → 199.44] probably something that everybody has in their home is some device like this that has a remote
[199.44 → 203.30] or whatnot. I'm listening. This is, you're right up my alley right now.
[203.30 → 208.08] So this guy, I can't tell quite where his accent's from. It sounds Eastern European,
[208.26 → 212.92] sort of Russians. I'm not entirely sure where this chap's from, but he runs a website at
[212.92 → 219.72] Priceless Toolkit, which is an IoT shop. And he sells pre-assembled circuit boards for all sorts of
[219.72 → 227.24] ESP related nonsense. And this ESP clicker has three microscopic relays on it, which can simulate
[227.24 → 234.16] up to three different button presses on different physical devices. So the use case he shows in the
[234.16 → 237.96] linked YouTube video on the product page, which there'll be a link to in the show notes, by the way,
[238.68 → 244.84] is that he has automated his coffee maker, which is not Wi-Fi enabled. The only way of interfacing with
[244.84 → 251.28] this physical device is to stand in front of it with your meat sausage and just push the button on
[251.28 → 257.16] the front of the machine. Well, except of course, all that's doing in reality is bridging a contact.
[257.24 → 262.52] So all the relays doing inside the ESP clicker is the same thing. And obviously, because it
[262.52 → 267.60] integrates with ESP home, home assistant integration is a mere click away.
[268.46 → 273.00] And so I imagine you kind of have to pick and choose the device you're wiring to,
[273.06 → 275.90] like you'd have to be willing to open it up and wire some contacts on that side.
[276.26 → 282.16] Yes, absolutely. If you're not into soldering or into hacking potentially very expensive devices
[282.16 → 288.68] to pieces to integrate this thing inside, stay away. But for me, with my Flux remote,
[288.90 → 296.38] it has some surface mount buttons on it. Each button has four legs on it. So I get my multimeter
[296.38 → 305.48] out and I turn it into continuity mode. And the pins of my multimeter are tiny. The probes,
[305.48 → 310.98] the tips of the probes are tiny, but the pads on these surface mount component buttons are even
[310.98 → 317.76] tinier. I can't even really think of an actual item that we would hold in our hands that is that small.
[318.04 → 324.02] They are maybe the head of a sewing needle small. Like I'm used to soldering small stuff with racing
[324.02 → 329.42] drones, but this is like another level down. So I'm going to have fun soldering it. But I did manage
[329.42 → 335.40] to get it work simply by just hot gluing. I hot glued just what I was messing about. I hot glued
[335.40 → 341.24] the cable from the ESP clicker onto the button, so I wouldn't have to physically hold it and control
[341.24 → 346.38] my, uh, the blinds above my drums from, from home assistant. So it was, it was pretty sweet.
[347.12 → 352.32] That is nice. I think I'm going to pick one of these up. I have a fan. Furthermore, I would love to control,
[352.48 → 356.40] love, love, love to be able to remote control it with home assistant because it's built into the roof.
[356.40 → 360.62] It's a great exhaust fan, but you don't need it running all the time. If it gets down below a
[360.62 → 363.26] certain temperature, I could just kill it with something like this. I could just
[363.26 → 368.04] have an automation that turns it off. What's particularly nice about buying this
[368.04 → 372.94] from Priceless Toolkit. We have no affiliation with this chap, or I just found a cool project
[372.94 → 378.48] on YouTube is it's a prebuilt project. So he shows you how to assemble it with all the surface mount
[378.48 → 383.94] components on the ESP board, all the relays and stuff. But honestly, this board is tiny. It's,
[383.94 → 390.22] it's probably about the size of your index finger. Um, when it arrives, it's, it's too small for me
[390.22 → 393.96] to be messing around with. Like I'm, I'm good at soldering small stuff, but this is just,
[393.96 → 400.24] it's, it's too much. But the fact that you and I can just go on a website and buy a pre-made
[400.24 → 406.80] thing as a product that arrives with ESP home already flashed on it, man, that is compelling.
[407.58 → 411.52] You wish, I know it's never going to happen, Alex, but don't you just wish these vendors would start
[411.52 → 417.38] maybe selling this as an option, you know, like an upgrade option. Hey, buy it with an ESP home
[417.38 → 420.60] wired in, and you can do what you want with it. I would pay more for that.
[421.04 → 427.04] Well, I suppose effectively that's what the whole two-year thing in a roundabout kind of way is
[427.04 → 432.82] doing. Cause that's just using an ESP chip inside a light bulb or whatever it might be. And there was
[432.82 → 437.26] a Digit blur video just this week, which I'll put a link to in the show notes as well, where he's
[437.26 → 442.18] talking about an update to the liberation scripts we've talked about on the show before, where you
[442.18 → 446.90] act as the man in the middle between the local two-year device and their update server and flash
[446.90 → 451.74] ESP home onto it that way. There've been some more updates to that recently as well. So go ahead and
[451.74 → 459.52] check that out down below. I've been, I've been very, very tempted to look at ESP solutions around
[459.52 → 465.32] buttons for home automation. There are a lot of options, you know, Hue makes something. Of course,
[465.32 → 469.82] there are tons of Zigbee buttons. There are tons of Z-Wave options. So I've been trying to figure out,
[470.04 → 473.50] is that the route I want to go? If I want to start putting in more and more buttons to like turn on
[473.50 → 479.12] and off water pumps and water heaters, or do I want to use something pre-made that's maybe just on Zigbee
[479.12 → 484.08] or Z-Wave? And I already own some of these. So I've been experimenting down that route this week.
[484.08 → 489.52] And I'm curious, Alex, have you ever seen anything around using an ESP home to just essentially have
[489.52 → 494.36] like a button pad that you could press just to, and then just tie automations and home assistant to when you
[494.36 → 501.36] press a button? Not an ESP home device, but you could certainly create a macro pad, like a
[501.36 → 507.62] like a sum pad keyboard and put some kind of microcontroller on that, and then use the matrix
[507.62 → 513.72] layout of those keys to do different things. And people build all sorts of stuff to go on,
[513.76 → 518.76] like their smart desk setups. Obviously the downside of those is typically they require power
[518.76 → 524.92] all the time, where an ESP device, depending on how clever you are, can potentially be battery-based.
[525.34 → 531.50] But the advantage of using one of these sort of keypad style things is its almost infinitely
[531.50 → 536.00] configurable, especially if you start delving into the world of layers and all that kind of other
[536.00 → 540.80] stuff too. So this is, this is the problem. So the wife, she tells me, you know, I've been getting
[540.80 → 546.48] up early, been doing the things, doing my things, getting my coffees, doing a meditation, and I don't feel
[546.48 → 551.64] like using the tablet in the morning. Okay. All right. And then I noticed that the kids haven't
[551.64 → 555.92] been using the tablet, like in the evening, like they just kind of, it sort of slowed down.
[556.22 → 559.74] And so I kind of felt like maybe I'd built a system that the family wasn't really using
[559.74 → 563.04] and I kind of cut them out, and I felt bad about them. I thought, well, okay,
[563.18 → 568.80] I haven't really used buttons because we mostly use voice control and these tablets that are mounted,
[568.80 → 575.60] but maybe, maybe a button to control this specific light or to kick off this particular automation
[575.60 → 581.12] or to control this group. Maybe it's time for that. So I, I, I decided to start doing some
[581.12 → 586.04] digging in this area, and I'm just not very impressed so far. Zigbee buttons in my experience
[586.04 → 593.34] kind of suck. They, they work most of the time, but they fail just often enough for you to be like,
[593.60 → 599.72] did it work? Has it worked? Oh yeah, there it goes. Yep. That is it. They sleep right to save battery.
[599.84 → 604.90] Yeah. And some buttons do support being plugged in, but then those buttons have limitations.
[604.90 → 611.18] And then the tooling and home assistant is pretty rough. You can add a device easy enough using
[611.18 → 617.22] Zigbee or Z-Wave or whatever you're using Wi-Fi, if it's a Shelly potentially, but then like,
[617.34 → 621.20] how do you do anything with that button? Well, you have to go create an automation. Okay. Well,
[621.38 → 626.56] now you have to figure out what button the device thinks you're pressing. When you press that,
[626.64 → 631.16] find the right option in the automation, which sometimes has like 25 entries in there,
[631.16 → 635.38] even though, even though it's only got one or two buttons, and then you have to create an automation
[635.38 → 639.28] for everything you want each iteration of those buttons to do. So if you've got like a quad button
[639.28 → 643.20] panel, you have to create an automation for each button. And then of course, all of these things
[643.20 → 646.78] support, like if you double tap, it does something different. If you hold it, it does something
[646.78 → 651.52] different. Well, that's a different automation for that. And so if you got a few, a fair amount of
[651.52 → 655.14] lights or things that you want to be able to control over buttons, like I want to have a button,
[655.14 → 660.94] the wife can hit, and it just raises the temperature five degrees, just five degrees warmer for two
[660.94 → 666.72] hours. And there's just not a really great solution and home assistant for this.
[667.24 → 673.44] I have wanted that kind of, uh, for me, it would be cool house. You know, I'm, I'm feeling hot right
[673.44 → 678.18] now, and I will know I will forget to turn the thermostat back up again. Can I just have a
[678.32 → 683.30] I'm playing the drums, and I'm hot right now button? Can I, can, can that just be a thing? If anybody
[683.30 → 687.40] knows how to do that kind of, I think it's probably a scene, and then you return to the previous scene.
[687.92 → 692.60] If you were in the audience, and you have a working example of that with code and the buttons,
[693.02 → 695.36] please write in and let us know.
[696.24 → 699.84] I started playing around with, and I haven't gotten it working yet, but I want to let the
[699.84 → 704.64] audience know because I think this should be built into home assistant. It's called home assistant
[704.64 → 711.58] switch manager. You can install it through hacks or do it however you like. And it gives you a UI
[711.58 → 718.40] to set up your buttons. And when you add a device, it gives you, okay, here's all the devices we know
[718.40 → 722.94] home assistant natively support. So you select one from the list. It's also just for God's sakes,
[722.94 → 727.18] nice to have at least some list of devices that, you know, work with home assistant. So that's another
[727.18 → 732.22] reason why this plugin is nice. So you go through the list of the buttons that work with home assistant.
[732.22 → 739.18] And then once you select it, it has this brilliant feature called auto-detect. So you put it in auto
[739.18 → 744.46] detect mode, and you press a button on the switch, and it figures out what button and switch and
[744.46 → 748.86] everything is. And then you just start setting up graphically. This button does this, this button
[748.86 → 754.76] does that. If I press it twice, and it's all a nice UI, and it doesn't require creating automations.
[754.92 → 758.58] It is a custom integration. So you have to get that installed and then as a front end component,
[758.58 → 762.30] you have to use, but it's beautiful. It's very minimally designed. It looks like something
[762.30 → 766.54] the home assistant team might create. The only problem with it is, is I can't get it to work.
[766.54 → 771.24] I, it recognizes I press the buttons, but then it doesn't execute the thing it's supposed to do,
[771.24 → 777.14] like turn device on or off. So I've had to bail on using it, but it also supports MQTT for devices
[777.14 → 782.08] that use that. And it supports Z-Wave and Zigbee devices, Bluetooth, anything that home assistant
[782.08 → 786.94] can support. It'll work with, I just haven't got it to actually execute the functions. I imagine it's
[786.94 → 790.66] probably something wrong on my machine. So I'm back to using automations, but I wanted to let you guys
[790.66 → 794.96] know, because this, this is so good at how it needs to be built in. They need to build this into
[794.96 → 798.90] home assistant. You know what Steve Jobs would say right now, don't you? What?
[799.24 → 803.26] You're holding it wrong. Oh, I thought he'd say something about don't have buttons or something.
[805.22 → 810.58] I felt like, I felt like I had like discovered like my, my, like a game, you know, when you're
[810.58 → 813.24] like, you're going to redo everything, you're going to delete all these automations. You're
[813.24 → 817.08] going to redo the whole way you did manage all this stuff. I thought I was going to do that with
[817.08 → 821.42] switch manager, but I'm just not there yet. And so I'm just stacking more automations.
[821.42 → 829.18] Um, I do have a couple of switches that have worked for me so far. And, but like Alex said,
[829.20 → 835.24] with the big caveat that, um, all of this stuff will like to go to sleep if it's battery powered.
[835.58 → 838.14] You know, the other thing that happens with those battery powered buttons,
[838.14 → 842.98] if, if you're as lazy as I am anyway, is you go to push the button one night, and you think,
[843.08 → 846.82] ah, well, maybe it failed. I'll just get my phone out tonight. And then you push it again the next
[846.82 → 851.24] night, and you're like, ah, well, it failed. I'll fix it tomorrow. And then before you know it,
[851.24 → 856.08] your button's been out of battery for six months and your routine is completely devoid of physical
[856.08 → 862.04] button presses. And this thing has been sat on the wall for six months doing nothing. So, uh,
[862.30 → 869.76] yeah, I, I just wish there was a way, an easier way for me to tap into the always on power inside
[869.76 → 876.30] a light switch to power some of these buttons. Like I know there's a is it the zoo's switches?
[876.30 → 881.10] I think we talked about and there's Z-Wave. Yep. And they go in the wall, and you can wire them.
[881.10 → 888.84] I really want just some kind of, a non-offensive button pad, which looks like a light switch and
[888.84 → 892.96] behaves like a light switch for normal people. Uh, and for me in the middle of the night,
[893.02 → 898.10] to be perfectly honest with you, but also has the smarts that if I want to, you know, arm the
[898.10 → 903.02] front door lock and do a bunch of stuff as I'm heading to bed, you know, I don't have to pull my
[903.02 → 907.78] phone out every time. That would be really nice. If you know of anything like that, again, please,
[907.78 → 914.10] I see a crowdsourcing episode, uh, in full today. But if you, if you have any perfect examples
[914.10 → 918.70] like the zoo switches, but Zigbee would be my preference. If you know any of anything like that,
[919.12 → 920.12] please write in and let us know.
[922.20 → 927.60] Linode.com slash SSH. That's where we host everything that we put in the cloud. Anything
[927.60 → 931.46] that the listeners are going to touch anything that we want to have superfast computer infrastructure,
[931.46 → 937.22] it's Linde, and they've got some exciting news. So go to Linode.com slash SSH, get that $100
[937.22 → 941.32] and 60 day credit. You can really kick the tires. You can really try the infrastructure
[941.32 → 946.54] and you can check out the great news. Linde's now part of Akamai, all the developer friendly
[946.54 → 951.22] tools like their cloud manager, which is beautifully built their API, which is clean and well-documented
[951.22 → 955.42] their command line client, which is super handy. All that stuff like we used to deploy and scale
[955.42 → 959.66] in the cloud. That's still there. It's still Linde, but now they're combined with the power
[959.66 → 964.66] and global reach of Akamai, and they're expanding the services to offer more resources and tooling
[964.66 → 969.62] while maintaining that reliable, affordable and scalable solutions that open source projects,
[969.80 → 974.62] individual listeners and businesses of all sizes use. And we love it. We run our matrix
[974.62 → 978.12] infrastructure in there. And over the two years, we've scaled that thing into a monster to maintain
[978.12 → 983.58] performance for our community and Linde handles it. The object storage is fantastic. I use it for
[983.58 → 987.54] all kinds of things now that are just sort of like back in infrastructure bits and pieces,
[987.98 → 993.16] resources for clients and whatnot, for accessing XML file, pulling down a JPEG, put it on object
[993.16 → 998.34] storage. Linde has fantastic object storage. And as part of Akamai's global network of offerings,
[998.54 → 1002.30] they're expanding the data centres worldwide. They just opened up a brand new one last week in
[1002.30 → 1006.34] Sweden. It is a banger, and they're giving you access to even more resources. You can grow your
[1006.34 → 1012.62] business, project or your customers. So why wait? Go experience the power of Linde. Now Akamai,
[1012.72 → 1018.12] go to linode.com slash SSH. That's where you go to get the hundred bucks, support the show and learn how
[1018.12 → 1022.56] Linde. Now Akamai can help you scale your applications from the cloud all the way to the
[1022.56 → 1029.96] very edge. You know, like Alaska, probably. That's an edge. Or Brent's house. Go try it,
[1030.02 → 1034.50] support the show and get that $100 to kick the tires. Linode.com slash SSH.
[1036.00 → 1041.22] Now, before we get to an interview with Antonio, who is the lead developer of the Mergers project,
[1041.22 → 1048.18] I came across a fascinating article on TechCrunch earlier. Matter, not the matter you're
[1048.18 → 1053.96] probably thinking of. No, no, no. Not the home automation matter. The other matter, the app which
[1053.96 → 1060.80] lets you read stuff later and transcribes and reads it back to you matter, have added podcast
[1060.80 → 1065.74] transcription support today. This is getting more and more popular. I've been hearing from listeners
[1065.74 → 1071.66] that already just transcribe our shows. And so another tool, you know, in that cap is nice.
[1072.28 → 1075.76] I don't think I'm familiar with matter. I actually, when you put this in the doc,
[1075.80 → 1078.70] I thought you were talking about the communications protocol.
[1079.72 → 1083.66] Well, I mean, the thing is, it's not self-hosted at all. And the reason I mentioned it today is not
[1083.66 → 1090.18] for our core listener base, of course. It's actually going to make me get off my ass and look at how we
[1090.18 → 1095.48] can transcribe some of the JB show notes automatically using some of the whisper tooling
[1095.48 → 1101.02] that's getting perfect these days. The tricky part, and again, if you know a way around this,
[1101.14 → 1107.40] write in, let me know. That's the theme this episode, isn't it? If you have a good way of
[1107.40 → 1113.86] doing the dimerization. So Alex said this sentence and then Chris said that sentence. I think typically
[1113.86 → 1117.86] Drew, our editor, does a pretty good job of making it so we don't step on each other,
[1117.86 → 1122.40] which isn't always the case with podcasts. So the dimerization part should be fairly
[1122.40 → 1127.86] straightforward for the most part. If you have a good way of doing that with the open source
[1127.86 → 1132.38] whisper tooling that you're using, let us know. We'd love to build it into our release pipeline.
[1132.94 → 1137.56] One thing we could do to make that simpler, it would require some help from Drew, but I've talked
[1137.56 → 1142.56] to him about this, is supplying host tracks. So there's a Chris track and an Alex track.
[1142.56 → 1147.30] And so you give that to the trends to whisper and whisper knows everything said on this track
[1147.30 → 1149.36] was from Chris. Everything said on this track was from Alex.
[1149.98 → 1155.22] Ooh. Yeah. Of course, we have that option as the, uh, the creators of the content.
[1155.32 → 1160.18] Yeah, we got it and we have the source. We got it multi-track. So that's, that's, what's cool
[1160.18 → 1163.92] about being able to build it in at the, at the production levels. We could potentially do that.
[1164.42 → 1167.92] Uh, yeah, I'm really, really excited about getting that rolled out because I've been experimenting,
[1168.22 → 1171.84] manually generating them, manually attaching them to the shows for some things sometimes,
[1171.84 → 1176.62] trying different formats is so close. Like it still messes up on some of the tech terms.
[1176.80 → 1182.12] So like, uh, this doesn't seem totally feasible, but a dream of mine would be transcription gets
[1182.12 → 1187.20] published and then people could do pull requests against it. And the community could maybe fix the
[1187.20 → 1190.80] transcription if they cared, because it's not something we're going to go back and clean up.
[1191.22 → 1194.76] You know, I could see us running a better transcription five years down the road and just
[1194.76 → 1199.08] overriding all the transcription files with a better version. I could definitely see that at some
[1199.08 → 1205.32] point. Alex, you had a chance to sit down with the lead developer of merger FS, and he joined us for a
[1205.32 → 1210.24] chat. So welcome back to the show, Antonio. The last time we spoke to you technically wasn't in
[1210.24 → 1215.98] self-hosted. It was in one of the Jupiter extras shows where we interviewed you with Drew and Brent
[1215.98 → 1218.48] to talk about merger FS. How are you?
[1218.72 → 1219.90] I'm well, how are you doing?
[1220.20 → 1225.40] Doing good. Thank you. How is the, uh, the new Texas sunshine treating you?
[1225.40 → 1231.62] It's, uh, it's been hot. Uh, it rained once in two months for like 15 minutes. We kind of celebrated.
[1231.90 → 1236.96] So it's, it's, it's been a little bit to acclimate from New York City, but it's been good.
[1237.26 → 1242.00] Yeah. I tell you, uh, we were just talking about this before we, we pressed record. I think if I
[1242.00 → 1247.14] lived in Austin, I would probably have gained another a hundred pounds since moving to America.
[1247.14 → 1250.88] It just, some of the barbecue down there is just next level.
[1250.88 → 1255.58] The food in general, right? The Mexican food, of course, and everything. I mean,
[1255.60 → 1261.82] they've got all this fusion. Uh, we, my wife and I, it was our ninth anniversary of dating.
[1262.20 → 1269.68] And we went to this place. It's like brisket, but with an Asian flair and, uh, perfect.
[1270.16 → 1275.68] Came home completely stuffed, debated, like fell asleep on the couch afterwards. Uh, delicious.
[1275.68 → 1281.92] And the fact that I work from home, and I'm in my office, you know, most days, five days a week,
[1281.96 → 1287.02] at least. Uh, yeah. Uh, I'm lucky that I haven't put on that a hundred pounds you mentioned.
[1287.58 → 1291.40] That sounds amazing. Now, for those of you in the audience that don't know Antonio,
[1291.40 → 1297.76] I'll forgive you because it was 2019. The last time I think we spoke, uh, Antonio is the guy behind
[1297.76 → 1305.14] merger FS. I think one of the most underrated, dare I say, like low-key, awesome bits of Linux
[1305.14 → 1311.12] technology. That's really changed the way in which I interact with hard drives in media servers in
[1311.12 → 1316.66] particular. Uh, so the idea behind it is you have just a bunch of drives, and then you point
[1316.66 → 1323.70] merger FS at them with an FS tab mount entry or something. And then it kind of pulls those drives
[1323.70 → 1329.10] together into one big, what would you call it? Like gluttonous mount point. And then you can bind
[1329.10 → 1335.12] of traverse all the files and folders on those drives, uh, as part of that BOD, as if it
[1335.12 → 1342.14] was just one single massive drive. With conditions, but yes, I mean, if people are familiar with, uh,
[1342.14 → 1349.60] drive pool on Windows or union FS on, uh, on Linux or a UFS, there are a few different technologies over
[1349.60 → 1355.78] the years. Union file systems have been around for 30 years, at least if you use Docker or containers,
[1355.78 → 1361.78] you might be familiar with overlay FS, which is a different kind of union file system. So yeah,
[1361.78 → 1367.18] I'm in that category. All right. So let me ask you this. It's been, uh, you know, two or three years
[1367.18 → 1372.22] since we spoke 2019. I think the last time this is your opportunity to tell the good people of the
[1372.22 → 1377.04] self-hosted podcast. What's changed. There's been a lot of random stuff. I mean, the core features are
[1377.04 → 1384.18] all the all there for the average user. I don't think much has changed if anything, at least from
[1384.18 → 1390.60] their perspective under the covers, I've done a lot of cleanups. I years ago, embedded lib fuse into
[1390.60 → 1395.40] the project to make it easier for me to extend things. And I did a lot of kinds of retrofitting
[1395.40 → 1402.64] of the code there. I reduced memory footprint quite a bit and introduced some techniques to just limit
[1402.64 → 1408.22] fragmentation of memory, which was an issue for some users. If you had a machine running for a long
[1408.22 → 1415.66] time, there's a lot of churn of objects, especially on SBCs, smaller RAM systems that would cause issues.
[1415.66 → 1422.00] So I've helped mitigate the amount of memory in general used, and then kind of limited that memory
[1422.00 → 1429.22] leak in the form of fragmentation. I've also added kind of, again, under the covers, threading pools to
[1429.22 → 1433.92] certain behaviours. This is one of these things as a software developer, you have an idea of who's going
[1433.92 → 1438.82] to use your software in a certain way. And then you release it on the world and people use and abuse
[1438.82 → 1447.58] it for all kinds of other purposes. And I've had folks with like four pocketed Leon systems running
[1447.58 → 1455.12] it against local shares, running different file systems, connecting to remote file systems of all
[1455.12 → 1465.54] sorts. And in those situations, the concurrency can be both good and bad. Good in that you've got more
[1465.54 → 1472.64] things happening in parallel, but because of how scheduling works, it can actually reduce the
[1472.64 → 1479.46] throughput. And so there are features for like pinning threads on the cores to separate receiving
[1479.46 → 1485.08] messages from the kernel with actually processing them, allowing you to determine how many kind of
[1485.08 → 1490.00] readers you want, how many processors you want, and then different strategies for pinning the cores.
[1490.14 → 1495.38] And that helps increase throughput. I haven't released this yet, but soon I'm releasing a feature that's
[1495.38 → 1501.60] been asked for a while, read Dur, right? Like when you actually scan directories, a lot of people
[1501.60 → 1507.52] will have network file systems and the latency to connect to those is pretty high, or they have maybe
[1507.52 → 1515.06] spinning disks where they're asleep. And so I'm concurrently connecting to or doing a read Dur on all
[1515.06 → 1520.98] of those at the same time if optionally, because it increases the memory usage a bit. But that way it can reduce
[1520.98 → 1527.08] the latency to actually get that data. And so when you do an LS, it's faster.
[1527.64 → 1536.30] Yeah, I noticed Wendell did a video fairly recently on ZFS where he put his metadata onto a pair of NVMe drives.
[1536.30 → 1540.70] And even though the data was still stored on spinning drives underneath, the lookup times,
[1540.76 → 1547.56] the seek times for like just listing the contents of a specific directory was 10 or 20 times faster,
[1547.56 → 1551.04] just simply by moving that metadata. Is that the kind of thing you're talking about here?
[1551.60 → 1554.40] No, though I have been working on something similar.
[1555.22 → 1560.72] Mergers and a lot of union file systems at their core is almost like, it's just a union in the truest
[1560.72 → 1567.62] sense. Imagine you have A, B, and C, and you were to LS in each one of them individually. Under the
[1567.62 → 1574.06] covers, that's all Mergers is doing. And so imagine you type LS and your drive has to spin up and it
[1574.06 → 1578.88] takes like 10 seconds. Well, if each one is asleep, and it takes 10 seconds each, it's going to take 30
[1578.88 → 1586.56] seconds at least in aggregate. Now, what this feature does is just issue each of those at the same time,
[1586.56 → 1591.64] and then aggregates the data as soon as it's available. So you're looking at more like 11
[1591.64 → 1596.84] seconds rather than 31 seconds. That sounds fantastic. And I guess, you know, do you have
[1596.84 → 1603.28] any sense of what the typical Mergers deployment size is? I mean, there's no telemetry or anything
[1603.28 → 1608.34] like that in your packages, are there? So it must be tricky. It's one of these things where the
[1608.34 → 1616.26] exceptions probably indicate the rule. And what I mean by that is the most questions I get about Mergers,
[1616.26 → 1621.36] are usually from total noobs who don't know anything about file systems, right? And so
[1621.36 → 1625.76] unfortunately, there's only so much I can do to simplify what a file system is.
[1626.00 → 1628.78] That's most of us, by the way, dude. You know that, right?
[1628.84 → 1632.86] Well, yeah. But I mean, people who have like zero Linux experience, they're coming straight from
[1632.86 → 1639.68] Windows. They really have no understanding of how file systems work, even from just a general
[1639.68 → 1646.06] purpose user perspective. And so I get a lot of questions from that. But then the other side
[1646.06 → 1651.94] is the people who have these, like I was saying earlier, these crazy setups of like multi-socket
[1651.94 → 1658.64] Leon systems with a hundred threads or something. I think there's probably a very large silent minority
[1658.64 → 1666.86] or majority there of people who just are, you know, they've got five drives and that's kind of
[1666.86 → 1669.86] their setup. And maybe they want an SSD in there on occasion.
[1670.36 → 1673.14] Well, speaking of SSDs, I actually had a question for you around caching.
[1673.14 → 1678.34] This is something on Perfect Media Server that I actually get quite a bit as a question is,
[1678.80 → 1683.80] it's pretty common in the Unpaid world because of how they do their parity calculations.
[1684.62 → 1689.34] You're basically halving your write speed of any disk because for every single write you make,
[1689.66 → 1693.28] it has to make another write to the parity drive as well. So it basically just cuts your
[1693.28 → 1698.98] write performance in half, which is why Unpaid many years ago adopted that cache drive and then
[1698.98 → 1703.70] move a script type stuff. Now I know there's some stuff in your read me about, is it be cached,
[1703.80 → 1708.64] I think, and a bunch of other stuff. What's your take on caching?
[1709.38 → 1714.90] So there's, there are lots of levels of caching and this can be very confusing for folks. And,
[1715.00 → 1720.94] and unfortunately, again, it's one of these things where the features are there for functionality
[1720.94 → 1726.00] purposes. If there was one great generic way to set it up, I would just make that the default.
[1726.00 → 1730.78] Unfortunately, I find that that's not the case, especially since a lot of people are using it
[1730.78 → 1737.10] in a way where if you did introduce caching, people want to write things out of band, right?
[1737.14 → 1742.34] They want to be able to write to our clone independently and still have Mergers work.
[1742.76 → 1747.94] And you can't have caching there because there's no way you'll eventually get into a bad state with
[1747.94 → 1753.48] that. So there's, there's certain, there's kind of caching in the kernel and Mergers has a number of
[1753.48 → 1761.64] features there that are related to fuse directly. Then you have caching that Mergers itself can do.
[1761.82 → 1767.12] I don't do too much of that though. I'm looking at doing some more of it just to reduce sort of the
[1767.12 → 1772.40] the, the amount of calls I have to make into the kernel. And then there is usually what they call
[1772.40 → 1779.80] like tiered caching for the underlying devices. And that is where you have like NVMe or Octane in
[1779.80 → 1784.98] front of spinning disk or Octane in front of SSD in front of spinning disk, you know, that tier of,
[1785.06 → 1791.40] of setup. And, and this is something that I hope to fix in the next year because Mergers has kind of
[1791.40 → 1799.92] a simple key value pair config setup. It's difficult to articulate to the software, something like a
[1799.92 → 1807.32] very thorough tiered caching system, but there are ways to implement that regardless out of band.
[1807.32 → 1812.80] And that's the kind of things I generally show in my documentation, which is similar to those
[1812.80 → 1819.70] mover scripts that drive pool has, or Unpaid has. What you can do is just create two pools, and you can
[1819.70 → 1825.54] set one pool up as your primary pool. And that's where you put your SSDs, your fast storage, and your
[1825.54 → 1830.30] slow storage. And the idea is that you create a policy, you have a policy in, in Mergers,
[1830.30 → 1837.88] every kind of file system function has a policy. And that policy is what chooses how to behave when
[1837.88 → 1842.58] that function is called. So instance, for instance, you want to open a file, there's a policy that gets
[1842.58 → 1848.04] run, and it chooses which file is going to be opened, because you could imagine a scenario where you have
[1848.04 → 1853.66] five drives, and you have four files across five drives, like how do you pick one, what you do is you set up a
[1853.66 → 1859.58] creation policy such that your SSDs are prioritized, right? So Mergers is kind of always picking
[1859.58 → 1865.36] your SSDs, then you create like a secondary pool. And the reason you want the secondary pools,
[1865.74 → 1872.34] mostly because it's easier than duplicating the logic of moving stuff from drive to drive. But the
[1872.34 → 1879.46] idea is you just then target like with our sync, that SSD, and you just, you know, every day or
[1879.46 → 1885.20] whatever, you just move those files over to the secondary pool. And that secondary pool has none of
[1885.20 → 1890.22] the SSDs, it only has your slow devices in it. And then and then so far as something like Plex or
[1890.22 → 1897.48] Jellyfin is concerned, the files haven't moved, they're still in the same place, most likely because of
[1897.48 → 1904.18] how you know, the Mergers union stuff works. There is some subtlety there. But yes, yes, and it's a neat
[1904.18 → 1909.44] idea. And I think, you know, you could very easily combine that approach. I mean, that's how I've
[1909.44 → 1916.28] been adding ZFS into my, you know, single storage mount point for the last few years. It's a really
[1916.28 → 1920.70] interesting concept. And I think once you unlock the idea that you could have more than one Mergers
[1920.70 → 1926.72] mount point on a single system, that's containing different tiers of storage, for want of a better
[1926.72 → 1934.18] phrase, different classes of storage, then you can ramp up the complexity quite quickly. But it also
[1934.18 → 1941.86] ramps up the flexibility massively. Well, yeah. And if you think about it, so that that idea to add SSDs in
[1941.86 → 1950.00] that form came after a very popular usage of Mergers, which I didn't see coming when I first created it,
[1950.02 → 1956.30] which is people will have a local cache of drives. And then they have, you know, their data hoarder,
[1956.30 → 1963.28] all their ISOs sitting on Google Drive or something, and they tend to use R clone. And the author of R clone
[1963.28 → 1970.34] and I are on good terms. He has a union feature in R clone that is mimicking what Mergers does.
[1971.24 → 1977.78] And so people will combine the two and basically use their hard drives as a cache to cloud storage.
[1977.78 → 1985.08] And so you just add in SSDs in front of all that. And you have, again, another tier. There's another
[1985.08 → 1991.08] strategy that can be done that I don't see a lot of people doing. I created a tool years ago to
[1991.08 → 1996.68] orchestrate all this stuff, but I never made it popular. I never promoted it. And I've been looking
[1996.68 → 2003.52] at maybe doing that again. So if you're familiar with device mapper on Linux, like DM setup, which is
[2003.52 → 2011.04] used, it's the underpinning of technologies like LVM2, you can actually take a block device,
[2011.46 → 2017.22] any random block device, whether it's a hard drive or SSD, and you can make another device,
[2017.66 → 2023.68] a block cache for it. There's DM cache, which a lot of people know. And so you can use LVM
[2023.68 → 2029.38] to create logical volumes, and you can create a cache partition. But what a lot of people don't realize
[2029.38 → 2033.14] is you can actually take a random hard drive you have already formatted with whatever
[2033.14 → 2039.34] file system you have and use an SSD to create a cache on top of that. It's not that it's some
[2039.34 → 2045.04] secret. It's just not well, it's not publicized, I think, because there's no infrastructure around it,
[2045.06 → 2051.34] no software to kind of automate that process to say like, okay, I want, you know, 100 gigs of this
[2051.34 → 2057.16] SSD to be cached for this drive and 100 for that and to be able to easily bring it all together. And so
[2057.16 → 2062.14] I've been looking at maybe releasing a tool that can help with that as well. And so that way, people who
[2062.14 → 2068.76] want that caching at a block level, which can help with spin up of drives and other issues can do that
[2068.76 → 2075.40] without having to move to ZFS or move to Brake or Backs. We'll see that where that goes.
[2076.20 → 2079.68] So what have you got coming down the pike for us? Any exciting stuff?
[2080.34 → 2086.24] You know, most of the changes or additions that I've made in the past year or so have been quality
[2086.24 → 2092.28] of life things. So I added like Direct support, which is kind of a niche feature that some programs
[2092.28 → 2098.90] use, but it took a little bit to get working. So I added that. I added the ability that if a drive
[2098.90 → 2104.66] goes into read-only mode, it will tag it as read-only. And so it'll find another drive, right? Like you try
[2104.66 → 2109.58] to create a file, and it's a read-only device because your extension for partition got corrupted.
[2109.58 → 2116.28] It'll find another drive that will work if one's available. Read-ahead, setting read-ahead has always
[2116.28 → 2123.54] been kind of a pain. So Mergers will do that for you. The ability to do lazy unmounting of an existing
[2123.54 → 2128.24] mount point, because Fuse doesn't have a good way to remount like traditional file systems do.
[2128.70 → 2134.08] Mergers can take care of that for you. And so as soon as the last program stops using the old version
[2134.08 → 2138.94] of Mergers, it'll just get unmounted. So there's been a lot of stuff like that. Going forward,
[2138.94 → 2144.76] what I really want to do is completely redo the configuration system and move to TOML for the
[2144.76 → 2151.22] config. And what that will enable me to do is add a lot of features that people have been asking for
[2151.22 → 2156.78] in terms of like built-in tiering knowledge. So people would really like Mergers to know
[2156.78 → 2161.52] about the tiers of, you know, the performance, different performance characteristics of different
[2161.52 → 2168.36] drives. So it can more intelligently choose which file system to choose when it's creating a file
[2168.36 → 2173.08] or reading a file or whatnot. And that's kind of a big lift. It might not sound like much, but because
[2173.08 → 2179.90] the configuration is very simplistic at the moment, it's, and it touches a lot of pieces,
[2180.02 → 2183.94] right? Like there's a runtime config option and all these things. So that's going to take a little bit
[2183.94 → 2190.40] of work to do, but that that's going to enable me to add probably like a list of, instead of just
[2190.40 → 2196.70] having a list of, uh, of, uh, branches, you can have like a list of branches, right? So you could
[2196.70 → 2203.20] have a collection of SSDs or collection of Names that get priority. And then that falls back if nothing
[2203.20 → 2209.58] fits there into the slower drives. And so that'll allow for that tiered caching that we talked about
[2209.58 → 2218.00] in a more fluid and more natural way. I also have been thinking of adding features kind of like what
[2218.00 → 2223.98] Unpaid and Dry pool do. I think that the reason that they have mover scripts is that they want to have
[2223.98 → 2231.92] a very discreet, simple way of, of laying out the files, right? As you create files and whatnot. And then
[2231.92 → 2237.44] they worry about moving them on after the fact, kind of like the mover script that we talked about
[2237.44 → 2244.70] earlier. A lot of users are either because they've used those products, I think, or maybe it just
[2244.70 → 2249.64] seems the more natural way of doing it would really like the behaviour of like rebalancing, right? Like
[2249.64 → 2255.92] I add a new drive and I want it to kind of slowly move stuff around in some fashion. And Mergers
[2255.92 → 2261.52] doesn't do that very explicitly. It chooses a position where it's going to create something,
[2261.70 → 2266.42] you know, on the fly as it's making a decision, and you get to choose that policy. And so I think
[2266.42 → 2270.10] it'd be better to have both, right? Like you can choose upfront, but then there's kind of a
[2270.10 → 2275.92] background task that'll just sit and move things around more subtly. So that's a big one that I'm
[2275.92 → 2280.78] going to look at as well. I do sometimes wonder just how much of this is Stockholm syndrome.
[2281.10 → 2285.56] A lot of Unpaid users in particular, no disrespect to that project because, you know, it's been around
[2285.56 → 2290.46] forever and lots of people use it, lots of people like it, but it does do some stuff in a strange way.
[2290.46 → 2296.50] And it has to do things in a certain way to make up for decisions made 15 years ago, you know,
[2296.54 → 2301.28] booting from USB being a great example. So anyway, I wanted to say thank you very much for coming on
[2301.28 → 2306.02] today, Antonio. I really appreciate it. Where can we send folks if they want to support the project or
[2306.02 → 2308.44] open a feature or a bug request or something like that?
[2308.82 → 2313.80] So, I mean, if you just go to your favourite search engine and type Mergers, it will show up.
[2313.80 → 2319.62] The main page is just the GitHub page. So it's GitHub.com slash trap exit slash Mergers.
[2320.24 → 2324.92] And if you're interested in supporting the project instead of Mergers, go to just support.
[2325.12 → 2327.72] So there's actually a repository that has all the support details there.
[2328.22 → 2332.20] Lovely. Yeah. All the GitHub sponsors, Open Collective, Patreon, all that kind of good stuff.
[2332.86 → 2335.10] Thanks so much for coming on and enjoy the rest of your day.
[2335.42 → 2336.12] Thanks for having me.
[2336.12 → 2343.62] Tailscale.com slash self-hosted. Head on over there right now to get Tail scale for free for up to 100
[2343.62 → 2348.48] devices. It's a great way to support the show. And you can get the Zero Config VPN up and going
[2348.48 → 2353.94] in just a couple of minutes and have a mesh network between all your devices protected by WireGuard's
[2353.94 → 2359.44] noise protocol. And it's fast. It's really fast because all your machines talk directly to each other.
[2360.02 → 2363.14] And the Tail scale client is smart enough to know if you're trying to send something
[2363.14 → 2367.92] to a machine just destined for your tail net, you know, like something that has a tail net IP,
[2367.92 → 2373.86] or if it's something for the Internet. And that small little difference makes a big user impact
[2373.86 → 2378.38] because you can leave Tail scale running all the time. Like I have it on my Pixel 7 24-7.
[2379.30 → 2383.80] Always connected. But only the resources I need on my tail net go over my tail scale connection.
[2383.92 → 2389.66] So I put all of my infrastructure on my tail net, all my devices, my next cloud, anything I'm going to
[2389.66 → 2395.02] sync to, anything that I might, like my pictures backup, home assistant, I put it all on tail scale.
[2395.36 → 2399.90] So that traffic goes over tail scale. And then there's a lot of nice to have like tail scale
[2399.90 → 2405.26] SSH, which lets you log into any machine on your tail net using your tail scale credentials and ACLs.
[2405.92 → 2409.86] And yeah, they got a dashboard to let you manage all that. There are things like tail scale send,
[2410.44 → 2416.12] tail drop, you know, kind of like airdrop, right? But it lets you send files between your tail scale
[2416.12 → 2420.86] machines. They have a plugin for VS Code so you can edit the config files on any machine in your
[2420.86 → 2425.58] tail net. They have lots of ways to extend it. Alex and I share one machine between each other
[2425.58 → 2430.54] and you can even limit it to the ports that you can allow through there. They have a client for
[2430.54 → 2436.54] just about every architecture and OS, mobile, desktop, server, SBC. But tail scale also supports
[2436.54 → 2441.78] something called subnet routing. So like my solar equipment, I can access that even though I can't
[2441.78 → 2447.44] put the tail scale client on my solar equipment, I have a machine on my network where I have subnet
[2447.44 → 2451.72] relay turned on. And so using that, I can get to those systems for my other tail scale clients.
[2451.88 → 2455.92] And I love that. So I always know how the house is doing, even the electrical equipment.
[2456.62 → 2460.46] Go try it out, support the show and get it free for up to 100 devices. When you go to
[2460.46 → 2463.22] tailscale.com slash self-hosted.
[2464.72 → 2468.36] Well, you've been asking, and I think we have an answer for you.
[2468.36 → 2477.70] It's always the Llamas. Llama, L-L-A-M-A-G-P-T, a self-hosted offline ChatGPT like chat box powered
[2477.70 → 2484.30] by Llama too. No data leaves your device. And they just added Code Llama, which is one of the later
[2484.30 → 2490.62] models that Facebook just put out. And they just added support for NVIDIA GPUs. It's created by the
[2490.62 → 2495.82] Umbral folks, and they've released this just as a general Docker image. So you can put it on any system.
[2495.82 → 2500.74] Some of this stuff is getting crazy good. Just to go back to the transcription stuff for a second.
[2501.28 → 2506.30] There is a version of Whisper for Mac called Mac Whisper, which I've been using to transcribe
[2506.30 → 2513.94] all of my YouTube content recently. And I feel like having a local ChatGPT like bot, you know,
[2513.98 → 2518.30] where I could maybe feed that, you know, that transcription of a clip I've just recorded and say,
[2518.30 → 2524.18] could you maybe make that snappier or just, you know, some of those little things that you use
[2524.18 → 2530.06] ChatGPT for. It's always at the back of my mind when I log into OpenAI's website of where is this
[2530.06 → 2535.44] data going? So I love, I love, love, love that this is 100% private and local.
[2536.02 → 2541.32] And the UI is beautiful. They've really picked like the best of the front end software that's out there
[2541.32 → 2546.56] right now and combined it with the latest and freshest of the open source, large language models
[2546.56 → 2552.86] all on Docker. And they worked really hard to make it, although I wouldn't do it, but they made it,
[2553.00 → 2559.76] they made it possible to run it on a Raspberry Pi. I mean, it's horrible performance. Like for example,
[2559.76 → 2565.32] if you're on an M1 Mac MacBook, you're going to get a generation speed of 54 tokens a second
[2565.32 → 2570.72] on a Raspberry Pi 4 with eight gigs of RAM, you're going to get 0.9 tokens a second.
[2571.20 → 2575.20] Okay. So it's, it's a big difference. Why is anybody still running a Raspberry Pi 4
[2575.20 → 2579.08] at this stage? You know, maybe you're like me, and you're an old man, and you're like,
[2579.14 → 2583.98] I like it slow sometimes. I know that sounds weird, but it's nostalgic when the computer's slow.
[2584.38 → 2587.62] I'm being facetious. Of course, I am. I understand. There are plenty of good reasons.
[2588.36 → 2591.76] It is really nice to have it all local though. I agree with you, Alex. And to have code
[2591.76 → 2595.48] llama local too is choice. Llama, llama duck.
[2598.18 → 2602.00] This speaks to a piece of work I've been doing with, do you remember Morgan, the doorbell guy?
[2602.36 → 2607.40] Yeah. He and I have been working on a quick sync benchmarking script over the weekend.
[2607.94 → 2612.44] Cool. Finally, finally, finally, I've been wanting to work on this for a long time. I think I mentioned
[2612.44 → 2617.48] it in the show a few episodes ago as well. But essentially I edited together some of my old
[2617.48 → 2622.90] drone footage into a two-minute clip of the Ribble head Viaduct in the UK from a few years ago.
[2623.78 → 2627.96] Not the one that's used in Harry Potter. This one's up on Blakemore in the Yorkshire Dales.
[2628.30 → 2633.76] Beautiful, beautiful structure. Anyway, I digress. The purpose of this script is to
[2633.76 → 2637.96] try and get a sense for where the sweet spot is with quick sync.
[2637.96 → 2645.52] I had itchy feet the other day and I thought, I wish I had a server with more PCIe lanes so I could
[2645.52 → 2653.94] put some more NVMe storage in this thing. But my trusty i5-8500 CPU and the motherboard combo I have
[2653.94 → 2660.38] in there, which is an AS Rock rack motherboard, they don't really have much in the way of PCIe lanes.
[2660.86 → 2667.40] So I was thinking, well, could I go Ry zen? Is that a thing? What about an ARC GPU? Could I use that?
[2667.40 → 2672.52] But then isn't that going to quadruple my energy usage? And I thought to myself, I don't know.
[2672.72 → 2677.74] I don't want to buy these things and find out later. So what I'd love to do, and it might be
[2677.74 → 2682.50] ready by the time we record the next episode, but keep an eye on the Discord server. There's an active
[2682.50 → 2687.98] thread over there on the Perfect Media Server channel called QSV Testing, Quick Sync Video Testing,
[2688.58 → 2693.70] where we're talking about the various different iterations of this script and how we can do
[2693.70 → 2701.04] benchmarking across all or as many of the different Quick Sync encoding engines as we can. I've got
[2701.04 → 2709.76] access here to second, third, fourth, I think sixth maybe, and eighth gen Intel CPUs and a ninth, actually.
[2710.42 → 2714.86] So if you have something else or indeed you have one of those, and you'd like to run the test as well,
[2715.52 → 2719.82] join the Discord and let me know in that channel, and we'll share the GitHub repo with you where the
[2719.82 → 2725.24] script is. The idea is to try and figure out where the sweet spot is in terms of price to performance,
[2725.96 → 2728.88] in terms of codex support, all that kind of stuff.
[2729.16 → 2732.14] Why hasn't this been done already, Alex? Why hasn't this been done already?
[2732.44 → 2737.78] I don't know. I mean, I look at what LTT Labs are up to and, you know, Gamers Nexus, and they're all
[2737.78 → 2743.48] focused on gaming. Like, that's fine, but the Terminal's my favourite video game. I don't need
[2743.48 → 2745.12] a 3090, you know?
[2745.24 → 2748.28] The hardware can do other things besides play video games, you guys.
[2748.28 → 2749.70] Yeah, sometimes.
[2750.26 → 2754.62] Yeah, sometimes. That'll be really great to see the results. I'm very curious to see how
[2754.62 → 2757.98] that plays out. The Quick Sync sweet spot. That's going to be awesome.
[2758.64 → 2761.88] Yeah, well, when the benchmarks are all around and all the rest of it, I'll make a proper
[2761.88 → 2767.92] blog post, perfect meter server page, podcast episode, YouTube video. The virtuous cycle of
[2767.92 → 2771.02] content will be strong with this one because it's a lot of effort.
[2771.30 → 2777.96] I am very tempted by the Arc GPU. I have one in a machine in front of me, and it sings with
[2777.96 → 2784.14] Linux. Everything works so smooth. It's so snappy. Full Wayland support. It's all just
[2784.14 → 2792.12] flawless. However, I constantly struggle with tools like Stable Diffusion or Lama GPT or even
[2792.12 → 2798.40] video encoders. They just don't even grok what the Intel Arc is. They just, nobody has really
[2798.40 → 2802.62] built support. And then you have to go find, as far as this is my understanding, like if you want to run
[2802.62 → 2807.74] something like say Lama GPT or Stable Diffusion using the Intel Arc, you basically got to go get
[2807.74 → 2810.20] patched version of the project.
[2810.76 → 2815.88] Well, you could do what Wimpy does and run multiple GPUs in the same system and just have a headless
[2815.88 → 2820.48] Nvidia card that has the CUBA driver available for those particular apps.
[2820.84 → 2824.90] Not an awful solution if you've got the card already. Like if you've got the hardware, I don't
[2824.90 → 2829.82] think I'd go out and blow the money on a high-ended video not to use it for anything else. But if I
[2829.82 → 2833.90] already had one. Yeah. Also, not only do you have to have the physical hardware, you've got to have
[2833.90 → 2836.56] the minerals to configure it too. It's not a simple task.
[2840.28 → 2844.50] 45homelab.com. Big, strong, fast storage servers with affordable, high-performance,
[2844.62 → 2849.34] high-capacity enterprise storage solutions for all industries, for all data size requirements.
[2849.34 → 2853.72] I mean, we're talking professional-grade solutions that are ideal for a business.
[2854.20 → 2859.16] Maybe your home lab too. So go check out 45drives.com to learn more about those folks. You might
[2859.16 → 2866.04] remember them from the show before, and they have been cooking up 45homelab.com. What if you took
[2866.04 → 2871.12] all the ideas and all the skills learned and all the workmanship that went into the enterprise-grade
[2871.12 → 2877.22] storage, but you made something just for the home lab? That's their mission. They want to change the
[2877.22 → 2882.96] storage market, and they think they have a vision for the future home lab product market. They've been
[2882.96 → 2888.24] listening to feedback from our audience because we had them back in self-hosted 98, and they're cooking up
[2888.24 → 2892.16] 45homelab.com. I think that's going to be up your alley, so go check that out. Again, it's
[2892.16 → 2899.62] 45homelab.com for the stuff they're working on for us homemakers. And I think 45 drives maintains
[2899.62 → 2904.04] probably one of the best relationships with the open-source community. They have open designs for
[2904.04 → 2909.74] their hardware. I really like their overall ethos and where they take this stuff, so I think you might
[2909.74 → 2916.14] like it too. So go learn how 45 drives does things differently at 45drives.com. And if you get a chance,
[2916.14 → 2921.52] tell them the self-hosted show sent you if you end up buying something. And take a minute and go visit
[2921.52 → 2928.52] 45homelab.com. I know, it's two URLs. It's tricky. One's the company, 45drives.com, and one is the
[2928.52 → 2936.32] project they're cooking up for us self-hosted, 45homelab.com. We got a boozy of an email into
[2936.32 → 2941.54] the show this week. I think it's Leone's, how you pronounce it. And he lost his home lab in a fire.
[2941.54 → 2947.06] In fact, his whole town went up in a fire. And he doesn't have a lot of budget to work with.
[2947.16 → 2952.86] He's got some networking limitations, but he's rebuilding. And he's picked up an older HP Pro
[2952.86 → 2959.54] desk for 20 bucks, an i3, fourth gen, 500 gigs of hard drive, and four gigabytes of RAM, which he can
[2959.54 → 2964.36] upgrade over time. And so now he's trying to wrap his head around how to kind of restore. And he says,
[2964.46 → 2969.94] what would be the best and easiest and probably the most transferable way to get my old systems up and
[2969.94 → 2973.32] running? I'm staying with family, so I don't currently want to mess up with any of their
[2973.32 → 2977.12] router settings or their firewall. I'm wondering if Tail scaler WireGuard could help here.
[2977.38 → 2981.70] Well, first, congratulations on finding that HP Pro desk for $20. That's a bit of a steal,
[2981.80 → 2982.06] isn't it?
[2982.16 → 2982.36] Really?
[2982.56 → 2982.78] Yeah.
[2983.14 → 2986.90] Well, I'm very much currently in love with those small and cheap one litter PCs. You know,
[2986.94 → 2992.46] the one litter style that you can find refers on Dell's website or eBay for sort of hundreds
[2992.46 → 2998.26] dollars. More modern stuff might be better from a power draw perspective. So like the eighth
[2998.26 → 3003.72] gen draws seven watts at idle, whereas the fourth gen draws closer to 20. I don't know if that's a
[3003.72 → 3009.14] consideration for you, but I seem to recall power on Hawaii isn't the cheapest thing in the world.
[3009.78 → 3014.92] The other thing to consider is that you could potentially just use something quite turnkey,
[3015.10 → 3020.48] like dare I say Tail scale, to connect into these remote devices without having to do a bunch
[3020.48 → 3026.64] of firewall punching and configuration and stuff. Naked WireGuard is great if you have access to the
[3026.64 → 3031.12] firewalls, and you're familiar with, you know, distributing your own keys and stuff like that.
[3031.64 → 3034.52] But I don't know what your appetite for that kind of thing is.
[3035.02 → 3038.46] Yeah, I think Tail scale is probably the way to go on this one too. And then you're not messing with
[3038.46 → 3043.72] anybody's network. If you move it, they'll reconnect to each other real established. If you end up on a
[3043.72 → 3048.14] different network down the road, you're not going to have to rebuild your VPN setup at that point,
[3048.14 → 3051.32] which you'll probably become pretty familiar with. He continues to say,
[3051.32 → 3055.26] I'd like to have a Nextcloud instance using an external USB one terabyte drive,
[3055.78 → 3061.50] Pinhole for ad blocking, maybe for my devices only on Tail scale, possible Sambar and DRIVE for file
[3061.50 → 3066.84] sharing, and Plex or Jellyfin. I mean, that's kind of the self-hosted recommended setup there.
[3066.94 → 3071.68] Pinhole's pretty great. Plex or Jellyfin, whichever one fits your use cases. I'd say start with Jellyfin.
[3071.68 → 3076.74] And then if you have issues, try Plex. Also, he says he's considering Proxmox.
[3076.74 → 3081.52] I think that's a good idea. He says, I'm okay messing with any type of install on a base Ubuntu
[3081.52 → 3086.06] server, Proxmox, or Docker. Now, I don't know about it. What do you think, Alex? Proxmox on an
[3086.06 → 3091.92] i4 with four gigs of RAM? That might be tight. I mean, you're going to run up against the limits
[3091.92 → 3099.14] of four gigs of RAM pretty quickly as soon as you spin up one virtual machine. But if you were to use
[3099.14 → 3104.12] Proxmox to manage a couple of LXC containers, then that gives you a lot more runway, of course,
[3104.12 → 3108.42] and Docker containers as well, of course. Proxmox is just Debian Linux under the hood,
[3108.64 → 3114.34] so you can do that too. I get lots of people asking me how I run my Perfect Media Server setup.
[3114.60 → 3120.46] I updated the FAQs today with the answer to the question of, should I run Perfect Media Server on
[3120.46 → 3124.78] the host directly or as a VM? Because for some reason, that's a really important question to folks.
[3124.94 → 3129.86] I've never really quite understood. No, I don't need to shit on people that way. The answer is,
[3129.86 → 3135.10] it's really up to you. If you want to run some services in a VM and have that level of isolation,
[3135.76 → 3139.20] that's great. You're going to have to do a couple of things like pass-through if you want to have
[3139.20 → 3145.42] disks available, that kind of stuff, or set up file sharing from the Proxmox host into the virtual
[3145.42 → 3152.54] machine using maybe some kind of internal bridging or something like that. Vert FS or Vert9P, I think,
[3152.62 → 3158.26] is what it's called for Windows hosts. A lot of people like to keep the hypervisor host clean,
[3158.26 → 3162.90] but for me, the trade-off of running everything directly on the host because of access to things
[3162.90 → 3168.24] like Quick Sync is kind of worth it. So, you know, if you just want to keep things simple,
[3168.84 → 3175.00] just stick Proxmox on there. You may never use any of the Proxmox features, any of the virtualization
[3175.00 → 3179.56] stuff, but if you do decide further down the road that you want to do that kind of stuff,
[3179.64 → 3183.40] you don't have to then completely wipe your entire OS and start from scratch.
[3183.40 → 3188.06] Yeah, well said. Dimitri is struggling to ditch iOS. He says,
[3188.16 → 3193.84] I've been trying to switch from iOS device to a Pixel running Graphene OS. I've tried it three
[3193.84 → 3199.42] times, but I've been using iOS for so long that it's actually a huge pain to switch because of
[3199.42 → 3204.96] the apps. Any chance Chris could share how his transition has been going, and may he share how
[3204.96 → 3208.00] he set up a simple app such as Notes, Calendar, and Reminders?
[3208.00 → 3212.36] Well, I would just refer you to our sister show, Linux Unplugged. I think Chris has done a rather
[3212.36 → 3218.72] excellent job over there of documenting his, what is it, giraffe? Is that what you losers call it
[3218.72 → 3222.22] over there? My giraffe journey? Yes.
[3222.66 → 3228.38] If I recall, it started in November because I was at AWS reinvent in Vegas back then.
[3228.58 → 3230.08] Still using it. Still got it.
[3230.58 → 3230.86] Yeah.
[3231.24 → 3235.10] Yeah, it has, you know what? It's funny. You're going to roll your eyes at this hard,
[3235.10 → 3239.60] but you know what? Can you guess what app I miss the most out of all of Apple's apps?
[3240.02 → 3241.42] Don't tell me it's the blue of bubbles.
[3242.06 → 3243.14] No, it's Notes.
[3243.34 → 3244.40] Really? Okay.
[3244.74 → 3251.72] I know. It's silly, but in the last couple of iOS releases, Notes is really, really competent. I mean,
[3251.72 → 3256.24] you can share Notes, you can do collaborative editing, you can take pictures and store them
[3256.24 → 3260.60] in the Note. It supports markdown editing. It can capture text from inside the Note.
[3261.02 → 3264.62] It has searching capabilities, and you can search that text. It has tags. It has folders.
[3264.62 → 3271.60] And you can export it all out to markdown using a third-party tool. It's really everything I need
[3271.60 → 3276.60] because I often just need, like the other day I was working on the car and I just wanted to get
[3276.60 → 3280.94] the label off the battery. I don't want that in my photo camera roll. I don't want that backed up
[3280.94 → 3284.90] to the server. I don't want that on my slideshow system. Furthermore, I don't want that. You know, I don't,
[3284.96 → 3289.04] I don't know what, I just want it for 10 minutes, or I want it in a year when I need to look up the
[3289.04 → 3293.72] battery again. And I want it in a Note. I want it in a damn Note. And that's what Apple Notes is.
[3293.72 → 3297.70] So I haven't really solved that, but Quilled gets pretty close.
[3298.70 → 3304.90] Q-U-I-L-I-Pad, it syncs with Nextcloud notes, and it gets me really, really close. I like that.
[3305.04 → 3309.42] And then DAVE 5, you got to have that to sync with Nextcloud. You basically end up using Nextcloud
[3309.42 → 3312.72] to do a lot of the iCloud stuff. And that's how you, that's how you solve it.
[3312.98 → 3315.84] What's a guy got to do to get you drinking that Obsidian source, huh?
[3316.10 → 3317.76] Oh, I got it right here. I got it right here.
[3317.76 → 3322.82] Oh yeah, no, I'm using Obsidian, but Obsidian isn't great for image-based stuff, you know?
[3322.84 → 3323.96] Yeah, that's true. That's true.
[3324.02 → 3329.44] So I use it for like my actual like oil change notes and things like that I put in Obsidian, but...
[3329.44 → 3332.54] That was great. It was the other day, like I did a bunch of work on my car in the summer,
[3332.54 → 3336.32] and I thought to myself, when did I last, because I've got a track day coming up in October,
[3336.96 → 3341.96] thinking, when did I last change the oil? Which event was it before or after? And I couldn't
[3341.96 → 3347.28] remember specifically how many track days the oil in the engine has. And I went and looked in my Obsidian,
[3347.46 → 3352.94] and sure as you know, a few hundred miles ago, and I changed it the day before. So I've done one
[3352.94 → 3358.78] day on track, this current oil change, and I'm like, oh, past Alex, I love you. Thank you so much.
[3359.66 → 3363.68] The wife's sticker on her windshield that I put on there when we changed the oil fell off.
[3364.06 → 3365.38] I'm like, where's your sticker at? What sticker?
[3365.48 → 3365.78] Oh yeah.
[3365.92 → 3369.58] Oil change sticker. What are you talking about? The oil change sticker I put here, where'd it go? I don't know.
[3369.58 → 3373.80] So, opened up Obsidian. There's the date. There's the mileage. Okay, we're good.
[3374.96 → 3379.42] Now, just to finish Dimitri's question, if you did want to catch up more about Linux Unplugged and
[3379.42 → 3387.64] Chris's journey with ditching the big G in the sky, it started at UP 486. Goodbye, Google. Link in the
[3387.64 → 3394.90] show notes. Now, we got some boosts this week, and our baller boost was spam-proof at few.St this week.
[3394.90 → 3401.02] He came in with 60,057 SATs using Pod verse, and he has a hot tip because we've been getting,
[3401.28 → 3405.46] what do you guys use for personal finance management? He says GNU Cash. It's not great,
[3406.12 → 3410.46] but I've been self-hosting for over 10 years now, and it does a pretty good job of not breaking with
[3410.46 → 3412.46] each new release. That's nice.
[3412.94 → 3416.34] What is that? Is that an indictment of the current state of software or what?
[3416.62 → 3417.18] Yeah, really?
[3417.32 → 3419.30] The headline feature is, it doesn't break.
[3419.30 → 3425.40] You know, there is also a real practical matter of going with something like GNU Cash. It's not
[3425.40 → 3433.00] super flashy, but it's been around for 226 years. It just is steady as it goes, and it's open source,
[3433.28 → 3439.50] and it's established at this point. So I got to give a plus one to the GNU Cash recommendation.
[3440.14 → 3441.72] Thanks, Ban proof, and thanks for being our baller.
[3442.58 → 3445.18] Leaky Canoe came in with 50,000 SATs using the index.
[3445.18 → 3448.52] Hey, gents. Thanks for the great show. I'm just getting started with Home Assistant.
[3449.24 → 3453.70] What wisdom can you impart on a newcomer into this deep rabbit hole? Also,
[3453.80 → 3458.12] what communication protocols do you choose when you build out? Z-Wave, Zigbee. Also,
[3458.20 → 3463.22] you could add matter, Wi-Fi, thread, cues.
[3463.80 → 3472.78] What wisdom can we impart on a newcomer? Hmm. Start small. It's very tempting to order 800 devices
[3472.78 → 3475.70] and try and do it all at once. True. You don't need to do that.
[3475.72 → 3480.28] But as we talked about earlier in the show, quite often you'll get halfway through doing
[3480.28 → 3486.54] a project, whether that's an ESP-based build or whether that is some kind of light switch swap
[3486.54 → 3490.66] out, and you'll figure out that, oh, actually, the bulbs in the ceiling aren't compatible with
[3490.66 → 3495.02] this type of dimmer switch, and there's going to be roadblocks. So I would just take it slow,
[3495.02 → 3502.06] do maybe a room at a time, or a certain type of, you know, do lighting all at once, or something
[3502.06 → 3506.78] like that, or start off with climate, or something really simple, low-hanging fruit, where the stakes
[3506.78 → 3511.30] are pretty low. You know, I think I've talked about this in the past, where, you know, if you're doing
[3511.30 → 3515.16] something like home security right off the bat, and you're figuring out all the Home Assistant
[3515.16 → 3521.26] nuances, the stakes are lightish in that if you screw up, you could potentially leave your house
[3521.26 → 3526.64] unlocked overnight, which probably you don't want to do that. Whereas if the lights turn on at 2am,
[3526.82 → 3532.36] okay, it's a bit annoying, but nobody's going to be, nobody's going to be actually hurt or otherwise.
[3533.04 → 3539.70] Yeah, hopefully. Yeah, I wonder, what is your thought on doing like a base of Ubuntu or CentOS
[3539.70 → 3545.70] or whatever, Nix, and running Home Assistant core in a container, versus going with the whole
[3545.70 → 3549.08] Haas operating system supervisor setup, as for a beginner?
[3549.08 → 3555.92] The inbuilt app store is super powerful. I don't use Node-RED hardly at all anymore. I used to use
[3555.92 → 3561.08] it a lot when I was in the beginning, which is, so Node-RED is a more visual-based way of writing
[3561.08 → 3566.02] automations. I got into that several years ago, before Home Assistant made their automation
[3566.02 → 3572.36] UI a lot better. There's still a place for Node-RED if you want to do some really complicated stuff,
[3572.36 → 3578.94] because you can drop to JavaScript if you're so inclined as part of that workflow. But I really
[3578.94 → 3587.26] like the VM appliance aspect of it. I feel like if I want to move my Proxmox host, or I want to do
[3587.26 → 3593.04] some maintenance on my main Proxmox host, I can just snapshoot that VM and transfer that CAL file
[3593.04 → 3597.86] to a different box and bring it up, no problem. Whereas if it's on a physical piece of hardware
[3597.86 → 3606.48] and it goes pop, then if I'm not in the house, it's more tricky for me to recover from that situation.
[3607.06 → 3610.68] The other thing I would say is make sure you've got a proper backup. So I've been using for the
[3610.68 → 3617.16] last several years, the Google Drive backup plugin. This takes a snapshot inside the environment of
[3617.16 → 3621.94] the VM of the entire Home Assistant configuration, including add-ons and all the rest of it.
[3621.94 → 3626.10] And it backs it up to Google Drive. You can configure how many snapshots it keeps and
[3626.10 → 3629.66] it rotates them out every seven days for you or whatever you want to do.
[3630.26 → 3633.72] Yep. Also, a plus one on that recommendation. You can also go in there and have it do like,
[3633.84 → 3638.32] hey, I'm about to go do an upgrade. So do a backup for me and immediately send that off to Google Drive.
[3638.58 → 3643.18] So that way, if anything goes wrong, I can bail out. Also, you asked about communication protocols,
[3643.18 → 3648.86] Z-Wave, Zigbee, et cetera. Yeah, you know, man, that is a hard question to answer.
[3648.86 → 3654.36] It kind of depends, bro. Like it depends on your home because I have both Zigbee and Z-Wave
[3654.36 → 3660.16] and there's things I like about both of them. Zigbee is an open standard. It is going to also
[3660.16 → 3665.12] probably you'll find cheaper devices so you can save some money because it doesn't require
[3665.12 → 3669.68] a certification and Zigbee is kind of being folded into matter. So it probably has a really long
[3669.68 → 3675.46] future. Z-Wave is a proprietary standard you have to be certified on, but that means that in order for
[3675.46 → 3681.30] devices to get certified, they have to pass a certain level of QA, and it's 900 megahertz versus
[3681.30 → 3688.08] 2.4 gigahertz for Zigbee. For me, 900 megahertz just works better, goes farther, does more, is more
[3688.08 → 3693.04] reliable. I tried to switch over to Zigbee and went back to Z-Wave because it's just 900 megahertz.
[3693.14 → 3697.40] I think at the end of the day works better for me. I would try to put as few devices on Wi-Fi as
[3697.40 → 3702.18] possible. Absolutely fine to have Wi-Fi devices. I've got plenty of them. If you already own some,
[3702.18 → 3707.94] it's fine. But ultimately, I like to have everything on Z-Wave or Zigbee as much as I can,
[3708.00 → 3712.82] especially things that are sensors, switches, and that kind of stuff. And also, if you can,
[3712.88 → 3716.40] when you're getting smart plugs, buy ones that have energy monitoring built in from the beginning
[3716.40 → 3718.76] because then you get all kinds of great data you can use later on.
[3720.48 → 3727.12] MCZP writes in, number one, I own one domain and now I just feel inadequate.
[3727.12 → 3733.86] You know, what surprised me is how many people boosted in just saying they own one domain.
[3734.04 → 3736.50] Yeah, yeah. Chris, you are not normal, my friend.
[3736.94 → 3739.56] Well, how many domains? I mean, you have a lot of domains, right?
[3740.22 → 3746.08] I bought a couple this week, actually. Yeah, we actually tried to buy self-hosted. Forum this week,
[3746.70 → 3750.44] but unfortunately, that domain is taken with a lemma instance right now,
[3750.44 → 3752.64] and the admins aren't interested in selling it. So,
[3753.32 → 3756.40] I would love it if we could do self-host. Forum, but alas.
[3756.40 → 3756.52] Yes.
[3757.12 → 3759.88] That's why we just got to standardize on .lol.
[3762.04 → 3764.56] Yeah, I had to put that in there because, first,
[3764.60 → 3768.02] MCZP's a great booster, and second of all, one domain? Really, dude?
[3768.38 → 3771.76] Somebody out there must have more than 10 or 15, right? You got to admit it.
[3772.34 → 3779.94] I feel like a domain lush. I mean, it might be 80 domains. I don't know.
[3779.94 → 3782.54] I mean, it's not that many. It's a lot, though.
[3783.02 → 3786.72] It's enough that they were considered an asset of the business when I sold the business.
[3786.72 → 3794.88] I'm going by the American pie rules here. You take the number the girl says and times it by three,
[3795.10 → 3797.02] and the number the boy says and divide it by three.
[3798.94 → 3801.16] Lol Saboteur came in with 10,000 stats.
[3801.48 → 3803.12] First-time booster. Long-time lover.
[3803.64 → 3805.04] Tail scale question for the wizards.
[3805.04 → 3809.20] Is there a way to have an SSH-only connection go over my tail net?
[3809.74 → 3814.28] IT has my work machine locked down, and sometimes I want to connect to a guacamole server at home.
[3814.48 → 3816.92] You might be looking for something like corkscrew.
[3817.08 → 3820.80] This isn't a Tail scale-specific tip, although, of course, it will work over Tail scale.
[3820.80 → 3830.66] I don't know if your admins permit VPN traffic. Some firewalls are clever enough to detect that kind of stuff and block it at the firewall level, outgoing.
[3831.54 → 3840.54] What I used to do when I worked for a bank, what's it called when the thing expires, like Lance Armstrong, like seven years or whatever, where you admit to a crime long enough after that?
[3840.88 → 3841.88] Statute of limitations.
[3842.26 → 3847.44] Yeah, I think that applies here. I think I've not worked for that company for like six years, seven years now.
[3847.44 → 3850.62] Not statute. Statute of limitations. That's what it is. Statute.
[3851.08 → 3852.52] Statute of limitations. Okay.
[3853.22 → 3858.84] Well, when I worked for the bank in London, they had quite a restrictive firewall policy, which, of course, being a bank, you would expect.
[3859.12 → 3863.96] And I was getting into, you know, Linux in a big way and Shying around all over the place back then.
[3864.34 → 3867.22] So I started running my SSH servers on port 443.
[3867.36 → 3868.06] Clever boy.
[3868.06 → 3874.40] Because a lot of encrypted traffic goes over 443, so it becomes just another encrypted stream.
[3874.40 → 3884.78] And so if you use, there's a command which you can put in your SSH config file to tunnel all of your SSH traffic out over this tool called corkscrew.
[3885.32 → 3890.44] And then it will go out over port 443 and look like just normal HTTPS traffic.
[3891.00 → 3894.80] And that gets around quite a lot of sneaky firewalls if you ever need that trick.
[3895.48 → 3897.78] Yeah, there are so many fun ways to play with SSH.
[3898.02 → 3899.62] Let us know how it goes, Lulzabertur.
[3899.76 → 3901.56] I think you're going to have some fun.
[3901.56 → 3906.40] So VT52 and Faraday Fedora boosted into, say, pork bun.
[3907.16 → 3909.90] They like pork bun as a DNS registrar.
[3909.98 → 3911.84] They say they're headquartered in Portland, Oregon.
[3912.50 → 3915.86] So for Chris, it's almost like buying a domain from the next door neighbour.
[3917.08 → 3920.24] And you have to have it checked for damp every few years as well, being Portland, right?
[3920.50 → 3920.76] Right.
[3920.84 → 3924.36] Well, and potentially vandalism these days, but oh, I kid.
[3924.94 → 3926.98] There's a Seattle-Portland rivalry, and Seattle's better.
[3926.98 → 3929.06] Bob B comes in with 6,000 SATs.
[3929.60 → 3930.84] My Umbral node broke.
[3931.28 → 3931.86] So Oak is down.
[3931.98 → 3933.22] That's how he sends his automatic boost.
[3933.72 → 3934.64] So I'm sending it by hand.
[3934.90 → 3937.06] Containers are still a bit of a challenge for me to troubleshoot.
[3937.16 → 3940.50] I'm not really sure where to go next with self-hosting and Bitcoin and Lightning.
[3941.00 → 3945.82] Do I do something like Umbral, which is one of those you install it, and it has an app store, and you install all the apps from a container?
[3945.82 → 3949.78] Or is there maybe another less black boxy way I should go?
[3950.40 → 3955.56] If you want to get started with containers, I mean, I really, I feel like this is a cliché of mine, Bob.
[3955.64 → 3965.02] I feel like the best way to do it would be a minimal Linux install or even like an Ubuntu desktop or some sort of desktop install and play around with it on the command line and start there.
[3965.12 → 3967.82] Run containers on the command line, play around with Docker Compose.
[3967.82 → 3974.76] Because that's what like these things are doing, like Start9 and Umbral and there are a bunch of others I was looking at, a couple others this week.
[3975.04 → 3976.54] They're giving you really nice front ends.
[3976.68 → 3978.66] They're doing the app discovery, which is nice.
[3978.82 → 3985.46] But when you click install, they're just kind of pulling down a Docker Compose file and then pulling down containers and firing them up.
[3985.54 → 3989.32] And when you understand how that works, it makes it pretty easy to troubleshoot any of these.
[3989.42 → 3993.30] Or at least you can go in and look at how they run and be like, oh, I'm not comfortable with this.
[3993.36 → 3994.52] This is a mess and you can bail.
[3994.52 → 4006.20] Yeah, I mean, I've got a bunch of tips over on perfectmediaserver.com, which, by the way, I should say, in the last episode, I put a call-out to the audience to say, hey, send me some money, please, to support the website.
[4006.46 → 4009.12] And boy, did you guys respond.
[4009.36 → 4012.78] I had nearly $400 in donations come in the last two weeks.
[4012.78 → 4013.40] Oh, that's awesome.
[4013.44 → 4014.04] Which was amazing.
[4014.14 → 4017.80] It's more donations than I've ever had for any of my projects previously.
[4018.00 → 4020.30] That should cover some of the run costs of the server for a while.
[4020.40 → 4021.50] Yeah, it's about 15 months.
[4021.64 → 4022.02] It's great.
[4022.02 → 4026.72] Of Runway, which is the first time perfectmediaserver.com has ever not just been out of my own pocket.
[4026.88 → 4029.82] So thank you so much to anybody that donated.
[4030.06 → 4032.12] And I really, really appreciate it.
[4032.68 → 4038.68] So on perfectmediaserver.com, there is a containers section where I sort of walk through Docker and Docker Compose and all that kind of stuff.
[4039.20 → 4045.58] You can also have a look in my GitHub repo, which I'll put a link to in the show notes, for all the various containers that I run personally.
[4045.58 → 4049.98] And I run that through an Ansible configurator to spit out the Docker Compose file.
[4049.98 → 4058.20] That may or may not be too advanced for you, in which case there are tons of Docker Compose examples for those similar apps on the Internet.
[4058.66 → 4061.26] Or just join our Discord and ask for some help, and we'd be happy to help.
[4061.66 → 4067.64] Our last boost this week that makes it in before we have to run is from GeneBean19998sats.
[4067.64 → 4076.94] And he sent me some pictures of a traditional American rotary phone where you put your finger in the thing and you pfft it around.
[4077.36 → 4088.20] And he has done an integration with his VoIP system, and he can pick it up and do voice commands to Home Assistant on an old classic rotary phone.
[4088.62 → 4091.12] He sent me all the pictures at Matrix, and it is so neat.
[4091.20 → 4097.02] And he pointed us to the VoIP integration for Home Assistant, which is how he's kind of making all this happens.
[4097.02 → 4101.30] And he has a little bridge adapter with a POE adapter, so the whole thing's powered.
[4101.56 → 4103.22] It all just, it's just so great.
[4103.80 → 4113.44] I remember, I was probably a teenager at this point, but my stepmom brought home a rotary phone from, she used to work in the doctor's office.
[4113.54 → 4117.72] And I think they were having a clean out or something, and she brought home this rotary phone.
[4118.48 → 4123.40] And, you know, I was a bit of a gadget head, even at age 14 or whatever it was.
[4123.40 → 4128.36] And I remember she put this thing down on the kitchen table and said to me, how would you use this?
[4128.42 → 4129.84] How would you dial a number on this phone?
[4129.92 → 4135.28] And I look at it, and I'm poking the buttons, thinking, ah, I have no idea.
[4135.42 → 4138.78] And I sort of got the idea that the dial on the front sort of moved.
[4138.86 → 4147.90] And then I was like, wait, I have to drag it all the way around and then wait for it to go all the way back and then do the next number the same way?
[4147.90 → 4150.40] Like, I want to dial 999.
[4150.72 → 4151.82] That's going to take me a while.
[4152.36 → 4152.46] Yeah.
[4152.98 → 4154.06] I loved them, though.
[4154.24 → 4155.26] Just playing with it.
[4157.10 → 4159.00] I just liked, I liked playing around with it.
[4159.10 → 4165.86] They had such a wonderful, like, Land Rover-issue mechanical engineering, like, clunk to them, didn't they?
[4165.94 → 4166.64] Yes, they were.
[4166.70 → 4168.44] They were very clunky technology.
[4169.34 → 4171.04] Also, I'm going to put a link in the show notes.
[4171.36 → 4174.56] Gene Bean sent along a link for Home Cam for HomeKit.
[4174.56 → 4182.16] And if your cameras are HomeKit compatible, it gives you, like, a dashboard of bringing all your camera feeds into a single pane.
[4182.50 → 4184.86] It looks really cool, so I'll put a link to that in the show notes.
[4185.28 → 4187.60] That's all the boost for this week because of time.
[4187.64 → 4189.10] But thank you, everybody who boosted in.
[4189.16 → 4193.86] We keep all of them in the boost barn in our dock, and we share them with the whole team, so everybody sees all of them.
[4193.94 → 4198.94] We had 19 boosters, and we pulled in 230,909 SATs.
[4199.30 → 4200.74] Thank you, everybody who did boost in.
[4200.82 → 4201.58] We read all of them.
[4201.58 → 4205.60] And if you'd like to boost the show, you can get a new podcast app, podcastapps.com.
[4205.72 → 4206.06] Let's see.
[4206.28 → 4207.20] Pod friend is on there.
[4207.44 → 4207.76] Fountain.
[4209.00 → 4209.32] Asthmatic.
[4210.02 → 4211.74] Podcast Index is on there.
[4211.78 → 4212.12] Pod verse.
[4212.38 → 4213.44] Lots of different apps out there.
[4213.80 → 4214.56] Podcastapps.com.
[4214.78 → 4215.64] Or keep your app.
[4215.98 → 4216.76] Getalby.com.
[4216.86 → 4222.64] Top it off, and then go to the Podcast Index and boost in, and we'll read your message on a future show, and you're supporting us directly.
[4222.64 → 4228.82] And, of course, thank you to our members, our Sees that are making the show possible and supporting the ongoing production.
[4228.98 → 4232.12] You get an ad-free feed with bonus content, a post show.
[4232.50 → 4234.62] That's at self-hosted. Show slash SRE.
[4234.62 → 4237.26] And don't forget about our upcoming meetups.
[4237.50 → 4244.54] Linux Fest Northwest is, of course, happening any day now, and there'll be a bunch of last-minute shenanigans, I'm sure.
[4245.36 → 4249.00] We're thinking about doing some kind of live recording on October the 20th.
[4249.06 → 4253.56] We're not quite sure of the details or whether we'll move it to the Saturday whilst we're at the Fest.
[4254.02 → 4254.46] Who knows?
[4254.62 → 4255.04] Who knows?
[4255.40 → 4256.64] It's all up in the air.
[4256.70 → 4258.74] We could do a live show at the Fest, maybe.
[4258.94 → 4260.24] That's not a bad idea, Alex.
[4260.36 → 4261.38] Yeah, I don't know.
[4261.48 → 4262.24] We should talk more about that.
[4262.90 → 4263.24] We'll see.
[4263.36 → 4265.52] I mean, I don't know about you, but I kind of like having an editor.
[4265.86 → 4266.72] Yeah, that's true.
[4266.80 → 4267.76] Well, you can still edit.
[4267.90 → 4269.56] It's just going to be, yikes.
[4270.40 → 4272.94] Not, it won't be his fault, but it'll be noisy.
[4273.48 → 4274.48] Just be a little noisy.
[4274.74 → 4275.54] Yeah, yeah.
[4276.02 → 4282.78] So, anyway, if you want to find out more about that, meetup.com slash Jupyter Broadcasting, as well as linuxfestnorthwest.org.
[4283.08 → 4286.42] You can go to self-hosted. Show for all different places to get in touch with us.
[4286.64 → 4290.34] And I have a links site at alex.ktz.me.
[4290.82 → 4291.86] And you can find me in the Matrix.
[4291.86 → 4294.96] I'm at jupyterbroadcasting.com slash matrix at Chris LAS.
[4295.02 → 4297.02] We got a self-hosted room or two over there.
[4297.06 → 4298.22] We got a bunch of chat rooms.
[4298.50 → 4299.84] It's really kind of a popping place.
[4300.60 → 4301.58] Come join us on the Federation.
[4302.44 → 4302.92] Thanks for listening.
[4303.10 → 4305.34] That was self-hosted. Show slash 105.
