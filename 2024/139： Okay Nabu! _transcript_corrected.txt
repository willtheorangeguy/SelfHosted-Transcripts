[0.00 → 4.12] I need to extend my thanks to both you and Brent for covering in my absence last week.
[4.16 → 10.86] I had one of those annoying respiratory viruses that I just lost my voice and just felt crummy all week.
[10.94 → 12.72] So thank you to you guys for stepping up.
[12.72 → 18.92] I thought maybe he had sabotaged you over there because it sort of was perfect timing with his new hardware setup that all arrived.
[19.58 → 21.08] Seemed kind of coincidental.
[21.86 → 27.86] Yeah, well, we did hear from a few people right into the show that said now they're going to use the O-Droid to build their own Cases and stuff, right?
[28.86 → 29.22] Yeah.
[29.68 → 32.10] You know, he's got a pretty good little plan over there, though.
[32.16 → 34.46] I like how much thought he's put into it.
[34.52 → 38.82] You know, this is something he's been slowly, as you know, he's been slowly working towards this as a goal for a while, and it's coming together.
[39.14 → 45.52] Now, we have a stacked show to get into today, so I'm not going to waste too much time with the pitter-patter at the beginning.
[46.08 → 49.68] We've got Paulus, the founder of Home Assistant, on the show today.
[50.04 → 57.84] Yeah, he's joined us because the Home Assistant voice preview, it's actually here, it's hardware, it's available, and we've had our hot little hands on it.
[58.30 → 59.94] And we had so much to ask him about.
[60.30 → 64.16] Hey, Taboo, invite Paulus from Home Assistant onto the show, please.
[65.00 → 66.66] Hello, Paulus, welcome back.
[67.20 → 68.90] Yeah, good to be here.
[69.26 → 80.40] It's your third visit to the show, and you're here for a special reason, this visit, because there's a new product and it's pretty exciting because it's not just a new product, but it's kind of like a new era.
[80.40 → 82.84] Yes, it's definitely a new era.
[83.16 → 93.96] We have launched last December 19, Home Assistant voice preview edition, where we've been tinkering on voice for two years, making small improvements left to right.
[93.96 → 100.74] Now we have hardware that makes it all super accessible in your house, and you can actually use it.
[100.74 → 105.64] This has been something that I've been tinkering with for a little bit, so I've had a chance to get some experience with it.
[105.72 → 111.42] And one of the things that I thought was the most delightful was the actual just simplicity of the design.
[111.42 → 120.36] It's a small little square with a USB-C port, a stereo jack, and then an almost iPod-like wheel.
[120.48 → 122.16] You noticed it, yeah.
[122.46 → 123.26] Can you talk about that?
[123.42 → 127.88] Yeah, it is like we were inspired by the original iPod.
[127.96 → 132.42] It had this nice wheel that you would feel it click when you go to the next step.
[132.56 → 132.72] Yeah.
[133.02 → 134.64] Yeah, we were like, we want this.
[134.72 → 137.20] And so we were looking, and then we found this rotary encoder.
[137.20 → 140.48] And so it's not capacitive touch because capacitive touch is just meh.
[140.48 → 143.56] Yeah, like you feel every click.
[143.68 → 144.72] Like it's not a click wheel.
[145.10 → 146.24] There's a button in the middle.
[146.50 → 148.64] But just, you know, the rotation feels so good.
[148.86 → 151.64] Yeah, I was like, oh, this brings me back.
[152.10 → 152.68] It really does.
[152.78 → 160.42] So can you tell us just a little bit about some of the changes that are happening at a software level in Home Assistant to make something like this work?
[160.44 → 166.88] Because when I got it out of the box, it was immediately discovered by the Bluetooth dongle I have connected to my Home Assistant.
[166.88 → 169.16] And I also got like a prompt on my phone.
[169.22 → 170.38] Can you just talk a little bit about that?
[171.10 → 173.78] You know, I'm the president of the Open Home Foundation nowadays.
[173.78 → 175.48] But we don't just make Home Assistant.
[175.62 → 176.70] We make ESP Home.
[176.80 → 182.86] And ESP Home, that is the open source software to create your own devices for the smart home.
[183.40 → 186.90] And our voice assistant is based on ESP Home.
[186.90 → 192.78] Now, we've been working on making ESP Home easier to use and get it easier to get onboarded.
[192.86 → 201.70] And so on of these things that we've developed as part of that is this thing called an open standard that we've developed ourselves called improve Wi-Fi.
[201.70 → 204.48] So it's called to set up Wi-Fi on devices.
[204.48 → 212.64] Because to set up Wi-Fi on devices that are generally the old pre, I don't know, a couple of years ago, you get a DIY device.
[212.80 → 214.64] It creates a Wi-Fi access point.
[214.72 → 216.12] You connect to that Wi-Fi access point.
[216.18 → 217.36] You set up your Wi-Fi credentials.
[217.54 → 218.20] You hit connect.
[218.20 → 221.94] It has to take down your Wi-Fi access point to connect to the Wi-Fi.
[222.04 → 222.88] So you don't get any feedback.
[223.02 → 224.68] You don't actually know if the device was connected.
[225.30 → 226.92] And we were like, that's super annoying.
[227.16 → 230.54] And every device you buy off the shelves, they have like a Bluetooth onboarding.
[230.64 → 232.52] So we created a Bluetooth standard.
[233.10 → 234.40] We added it to a Home Assistant.
[234.64 → 236.06] It's part of the Bluetooth proxies.
[236.34 → 237.70] You know, Home Assistant will find it.
[238.16 → 239.66] It's part of the Home Assistant apps.
[239.86 → 244.98] So even if you don't have a Bluetooth dongle, the Home Assistant app will help you set up the device via Bluetooth.
[244.98 → 249.12] And this open standard is actually built into ESP Home, right?
[249.20 → 263.00] So any device that is like ready, made for ESP Home will have improve over Belly on so that we as like the open home community, we, you know, we can build devices for one another and just have a great onboarding experience.
[263.32 → 273.66] But we actually went a step further in this case for voice because we noticed with voice in the last two years, like there's many different ways to create a voice assistant.
[273.66 → 277.00] And when I say ways, it's actually about the stack, right?
[277.04 → 278.32] Like there's speech to text.
[278.48 → 280.24] We have to turn your speech into text.
[280.32 → 284.60] Then we have to process that text, see if it's a command, answer that command or act on that command.
[284.94 → 286.62] Then we generate a text response.
[286.72 → 292.86] And that text response has to be turned text into speech that we can play back on a device, on your phone or wherever you are.
[293.34 → 298.94] Now, we realize that if you do this locally, self-hosted, and that's, you know, why I'm on this podcast.
[298.94 → 302.14] We care a lot of that about that, right, at Home Assistant.
[302.28 → 305.26] We want stuff to be local when it's possible.
[306.24 → 308.50] And so we actually open a wizard now.
[309.32 → 315.62] That wizard will guide you saying, okay, if you have Home Assistant Cloud, Home Assistant Cloud is the way people can support the Home Assistant Project.
[315.98 → 326.94] That actually has built-in speech to text and text to speech services that are cloud-based, but they are super high quality, super accurate, superfast, and support like 130 languages and dialects.
[326.94 → 333.44] But if you don't have Home Assistant Cloud, we will actually guide you through installing Whisper and installing Piper.
[333.84 → 336.26] Whisper is OpenAI's speech to text.
[337.00 → 340.94] Piper is our text to speech system that we've built ourselves.
[341.60 → 346.62] And basically, at the end, you have a working voice assistant that can work local.
[347.16 → 350.84] Now, we ran kind of into issues with Whisper.
[351.16 → 353.40] Whisper is a large language model.
[353.46 → 354.48] No, it's not a large language model.
[354.48 → 358.04] It's an AI system that is heavy, right?
[358.12 → 364.74] So we realized that Home Assistant Green, Raspberry Pi, that's not the best to run it on.
[364.82 → 373.42] So we recommend an Intel N100, like the one that Brian the other day with the DIY NAS guide recommended, right?
[373.50 → 376.04] The most efficient Intel chip nowadays.
[376.38 → 376.64] Sure.
[376.64 → 379.98] That one will run Whisper-based model just fine.
[380.20 → 382.68] And you can get like for English, right?
[382.72 → 385.46] Like I think that one works quite well.
[386.00 → 387.72] The cloud is still faster and better.
[387.90 → 391.12] But of course, you know, then it runs in the cloud.
[391.24 → 392.02] It doesn't run at home.
[392.32 → 393.96] This is Home Assistant after all, right?
[394.06 → 395.30] Like it's got to be local first.
[395.30 → 396.66] I'm curious.
[396.78 → 402.94] So you added some Bluetooth stuff to the stack over the last year or two with the Bluetooth proxies and what have you.
[403.54 → 408.40] There must be other stuff you've been secretly adding to Home Assistant with future hardware plans in mind, right?
[408.40 → 419.38] No, I mean the voice stuff, like all this stuff, for example, ESP Home, we added over-the-air updates where an ESP Home device can update itself without you having to compile it from the ESP Home dashboard,
[419.70 → 426.52] which allowed us to, for example, sell a voice assistant or Louis to sell his everything presence one sensor.
[427.04 → 434.76] And people don't need the ESP Home dashboard or ESP Home device builder, as it's been renamed, to actually update the device.
[434.76 → 439.26] There's just now an update entity in Home Assistant that, oh, boom, one click, it gets updated.
[439.94 → 440.70] I noticed that.
[440.98 → 446.34] I get my updates for this little puck thing just in the little notifications bar.
[446.44 → 448.16] I said, hey, Home Assistant voice needs an update.
[448.46 → 448.90] Press go.
[449.00 → 449.60] Isn't that nice?
[450.04 → 450.72] Really nice.
[450.82 → 451.76] Yeah, great job on that.
[451.90 → 457.82] No, we really looked at all the parts of a device of the shelf that you buy.
[457.92 → 459.50] What would be the ultimate experience?
[459.68 → 462.60] And we just made sure ESP Home can deliver that experience.
[462.60 → 473.14] Yeah, it feels like a really consumer-friendly, ready-for-that-next tranche of users that might be looking for something like this.
[473.20 → 474.22] I mean, it works great for us.
[474.54 → 474.76] Yeah.
[474.90 → 478.48] And it has a lot of perks, too, because it's a media endpoint now as well.
[478.82 → 480.26] And you can attach a speaker to it.
[480.58 → 485.72] So the speaker in our device is really meant just for voice responses, not for music.
[485.94 → 491.00] But we did add an AUX jack on it, so you can connect it to an active speaker.
[491.00 → 494.86] But what's actually really cool is that in this device, we have an XMOS chip.
[494.98 → 499.50] And XMOS is this 20-year-old British company that have been doing voice processing forever.
[499.70 → 500.54] Like, that's their deal.
[500.86 → 501.88] They make speakerphones.
[502.24 → 505.34] And a speakerphone just wants to capture voice, nothing else.
[506.02 → 510.00] Now, by putting this chip in there, they clean up the audio for us.
[510.10 → 517.30] But they also have this thing where any audio that we are playing through either the internal speaker or the AUX jack is removed from the input stream.
[517.30 → 519.58] So we can play music very loud.
[519.74 → 520.08] Cool.
[520.44 → 521.80] It doesn't get on the input stream.
[521.86 → 524.24] And we can hear the wake word throughout the room.
[524.48 → 532.30] And then, because we are playing the audio through our voice preview edition, we will lower the volume so we can hear you speak.
[532.70 → 536.82] And then at the end, when you hear your response, we'll bring the volume of the music back up.
[536.82 → 542.76] So I wanted to ask you why not a device with a screen?
[542.88 → 544.82] Because there have been some ESP devices.
[545.80 → 550.96] And I have one actually here in the studio that works with voice that does have a screen on it.
[551.20 → 552.54] Was that considered for a bit?
[552.66 → 555.06] And then this was decided it was a better route?
[555.06 → 561.76] So we were playing with the ESP32 S3 box as a development target for a while.
[561.88 → 566.44] And it really also forced our team to think about user interface and see what we can do.
[566.52 → 570.90] And we had like these nice pictures that would change if it was like responding or thinking.
[571.32 → 579.28] But we realized that what you really want from a voice assistant is, for example, when you ask it about your shopping list or the weather, you want to see that on the screen.
[579.86 → 582.20] And to do that, you kind of need like a bigger screen.
[582.20 → 586.38] And as we were discussing this, we realized, okay, this is going to blow up the scope.
[586.58 → 589.22] Like we want to ship some hardware like this year, right?
[589.26 → 590.48] And not like next year.
[590.76 → 591.26] Sure, yeah.
[591.44 → 595.18] But that's also, it's called Home Assistant Preview Edition, right?
[595.24 → 599.76] It's really, this is a milestone for sure for us.
[599.84 → 606.00] It's definitely an upgrade of all the previous ways you could experience Home Assistant Voice previously.
[606.46 → 609.68] We don't believe yet that it is for everyone.
[609.68 → 626.02] And for everyone, I mean, for if you want to remove all your Google Nest minis and have the same experience where you can cast your music to it, where you can ask any question in the world from it, we're not there yet, right?
[626.02 → 636.88] But if you use Home Assistant today, want to follow development, if you want to, if you just like using like the self-hosted stuff to see what's always possible, like this device is perfect.
[637.02 → 638.10] And like I use it every day.
[638.30 → 639.94] My kids use it every day, actually.
[640.08 → 642.74] The middle button is like push to talk, right?
[642.78 → 643.86] So you don't have to say the wake word.
[644.24 → 646.62] And they're just talking to ChatGPT all day.
[646.62 → 652.76] So at what point do we end up just literally chatting with our house through an LLM that's all local?
[653.60 → 656.00] It is possible today.
[656.24 → 659.54] So we have OBAMA support and Home Assistant.
[659.68 → 665.44] So the whole Home Assistant Voice experience has supported AI and AI can call tools, as it's called.
[665.52 → 667.40] So basically AI can control Home Assistant.
[667.74 → 669.98] We've had that working for the last six months.
[670.02 → 672.16] We've been iterating on it and improving it.
[672.16 → 674.06] So we have support for OBAMA.
[674.18 → 678.24] OBAMA is a local way of running large language models.
[678.82 → 681.02] And OBAMA works with LAMA.
[681.60 → 684.06] All the names sound similar.
[684.52 → 685.32] Too many Lamas.
[685.32 → 685.88] Yeah, too many Lamas.
[686.08 → 687.76] So OBAMA works with LAMA.
[687.96 → 689.96] It works with Queen and Mitral and all these things.
[690.08 → 692.12] And you need powerful hardware.
[692.56 → 695.66] Like this is not for the Raspberry Pi crew, right?
[695.74 → 697.70] Like they need to sit this one out.
[697.70 → 702.10] But if you have powerful hardware, you can run quite some good AI at home.
[702.16 → 704.92] And then you can start talking to it to your house.
[704.94 → 707.70] And it has access to everything that you have in Home Assistant.
[707.88 → 712.08] So we give it the state of your house, of all the devices that it can control.
[712.40 → 717.14] So you can also start asking things like, oh, which doors are open or this kind of things.
[717.90 → 724.74] The API is designed in a way that people could build their own custom components or custom integrations that add more tools to the AI.
[725.32 → 729.18] So there was one person was playing with adding Google search to it.
[729.24 → 733.48] So now the AI can actually search the web for you and get way more rich information.
[734.06 → 737.78] We also allow people to just use scripts to inject more data, right?
[737.82 → 743.42] So now allow the AI to query your calendar and list your events for the day or this kind of things.
[743.42 → 746.12] It's something we're super interested in.
[746.12 → 754.66] But it's also something where we know only part of our audience could basically do something with this, even if they have the most powerful hardware.
[754.90 → 757.60] So we're not chasing it.
[757.76 → 764.18] But our community is just so big that there's enough people working on it that we're making meaningful progress all the time.
[764.18 → 771.00] But it seems like there's a good and a bad side to where Home Assistant is at with voice control right now.
[771.04 → 773.88] And I'd like to just ask you about some of your future plans here.
[773.94 → 775.80] And I'll put it in context.
[775.90 → 780.54] So one of the things I love is that I can go in, and I can set aliases for just about anything.
[780.66 → 788.40] And so then we can have really familiar voice prompts to get the temperature of a room or, you know, change on, turn lights on or off and things like that.
[788.40 → 789.26] I like that a lot.
[789.84 → 795.34] But it really only works when I kind of go in, and I curate all the names for everything.
[795.44 → 798.02] And I kind of have to change it from the defaults.
[798.18 → 801.56] A lot of things get named, just kind of these long random names in Home Assistant.
[801.56 → 801.70] Yeah.
[802.70 → 811.18] What are your thoughts around future changes there about maybe the default names of devices or just kind of smoothing that whole thing over in general?
[811.88 → 815.56] So, well, one, the AI is actually the answer, right?
[815.56 → 831.08] You can do a lot less organizing as us, as a human of your house, because an AI can understand that a light entity in the living room, you can refer to it as living room lights, even if you don't have, you know, it's renamed to be that such.
[831.20 → 837.44] But I think in general, what we want to do is that we want to work on our information architecture.
[837.70 → 839.48] So you bring a device into Home Assistant.
[839.48 → 857.76] And today, it's more like a collection of data points entities instead of really being, oh, just an example is if you have three temperature sensors in your living room, Home Assistant doesn't know if these are ambient temperature or if this is your coffee machine or is this the nozzle of your 3D printer?
[858.22 → 859.04] Like, we don't know.
[859.58 → 861.78] So now we want to create a dashboard.
[862.04 → 866.32] Now we want to offer you an environmental state of your house.
[866.42 → 868.64] Now we want to have AI know about this.
[868.64 → 870.14] Like, currently, we don't know.
[870.26 → 874.62] So information architecture is very high on our list of things we want to tackle.
[874.84 → 878.86] And together with information architecture, better naming, that's also there.
[878.98 → 887.48] So if we know that it's a decorative light for an area, we can already provide a lot better default names.
[887.48 → 891.82] Unraid.net slash self-hosted.
[891.88 → 894.76] Go unleash your hardware and check out Unpaid 7.
[894.94 → 900.58] The release candidate is here, and it is packed full of game-changing features and full ZFS capabilities.
[901.20 → 906.02] Unpaid is a powerful and easy-to-use operating system for any self-host or home lab-er out there.
[906.40 → 911.90] If you've got some disks, you've been meaning to set up a server, maybe have a little network-attached storage, this is the time.
[911.90 → 915.80] Go make the most out of your hardware, no matter what you have on hand.
[915.88 → 920.22] Different size drives or manufacturers, that's not a problem with Unpaid.
[920.44 → 921.98] Go check it out and support the show.
[922.06 → 925.60] Go to Unraid.net slash self-hosted.
[925.78 → 930.16] And if you didn't know, Unpaid now has integrated tail scale support.
[930.34 → 931.30] How great is that?
[931.56 → 933.90] They've got a great video that shows you how to use it.
[933.98 → 937.46] It's such, such a nice thing to have on your server like this.
[937.46 → 940.28] And you know when Unpaid does it, they do it right.
[940.74 → 942.90] So they've gone full integration.
[943.42 → 947.74] When you install it, almost any Docker container gets the ability to connect to your tail net.
[948.16 → 954.20] You can access them using valid HTTPS certificates and give them alternate routes to the internet via exit nodes.
[954.54 → 957.62] You get to integrate tail scale into Unpaid.
[958.12 → 961.32] It's like your peanut butter and your jelly coming together.
[961.80 → 962.76] Unpaid is flexible.
[962.76 → 967.54] It's easy to use as a brilliant UI and Unpaid 7 makes it even better.
[968.48 → 971.92] Go try it out and finally take advantage of that hardware you've had sitting around.
[972.42 → 975.06] Stop worrying about it and just start building it.
[975.40 → 977.76] Unraid.net slash self-hosted.
[979.82 → 982.32] So 2024 was the year of the voice.
[982.56 → 985.22] I assume you're going to come up with a moniker for 2025.
[985.54 → 988.16] No, so actually 2023 was our year of the voice.
[988.56 → 990.16] And we weren't done.
[990.30 → 991.96] So we just kept going.
[991.96 → 993.42] No, we, you know.
[993.58 → 994.92] You just kept pushing on the voice.
[995.30 → 997.00] Now, we did more things.
[997.12 → 1009.72] I think our branding of year of the voice was so successful that when 2024 came around, like, you know, 12 months ago, people were like, they acted like we didn't do anything but voice.
[1009.72 → 1013.88] Even though we had made a lot of progress on automations and dashboards and this kind of things.
[1013.88 → 1018.02] So last April, we actually launched a roadmap.
[1018.22 → 1020.42] And a roadmap broken down per category.
[1020.64 → 1022.72] So, for example, we've been revamping our dashboards.
[1022.88 → 1027.12] Like, there's now this new sections dashboard type that is, it's not the default yet.
[1027.16 → 1028.80] It's the final step we still have to tackle.
[1028.92 → 1031.46] But that kind of relies on the information architecture I just touched.
[1031.46 → 1035.44] But if you create a new sections' dashboard, you can drag and drop.
[1035.64 → 1040.54] You can, it's very intuitive to build a beautiful dashboard through just a user interface.
[1041.34 → 1045.12] We've been re-simplifying and streamlining our automation editor.
[1045.12 → 1052.00] We've been getting all our protocol stack certified, which that's a project that's going to get into 2025.
[1052.54 → 1056.66] But, yeah, so there's a lot of progress happening all over the place.
[1056.74 → 1061.48] I think for 2025 right now, we're doing a roadmap annually at April.
[1061.64 → 1064.50] So in April, we're going to announce our next roadmap.
[1064.72 → 1069.32] We did just update, like, publish an update on, like, you know, progress report six months in.
[1070.14 → 1072.16] And it's going pretty well.
[1072.16 → 1078.26] Like, the things we wanted to do and the things we're doing is kind of lining up, which is very nice.
[1079.00 → 1080.76] Like I said, information architecture is important.
[1081.06 → 1083.12] Doing a bit more AI stuff.
[1083.24 → 1090.02] Like, one of the things people love doing is sending, like, camera pictures of doorbells to the AI and ask who's in front of my door.
[1090.80 → 1092.18] Like, that should just be easy.
[1092.28 → 1093.40] It should just be built in.
[1093.64 → 1094.22] Oh, I love that.
[1094.30 → 1094.46] Yeah.
[1094.58 → 1100.60] Yeah, it's like something we all are, like, if you have a camera, and you have a powerful system, that should just be a toggle in a way, right?
[1100.60 → 1101.80] Like, sure.
[1102.56 → 1106.48] Well, there's a bunch of stuff the commercial products do, you know, like the ring doorbells, for example.
[1107.30 → 1114.92] The basics like that of little things, like having them appear on your Apple TV is like a little pop-up picture-in-picture window, that kind of stuff.
[1115.00 → 1120.06] And I think all the guts are there with Home Assistant to connect all these things together.
[1120.82 → 1123.38] What's – I don't want to say lacking because that sounds kind of unfair.
[1123.38 → 1129.10] But kind of what's missing is that glue, just that last 10% user experience to kind of glue it all together.
[1129.52 → 1135.50] Yeah, I often call this, like, is that we are making a toolbox, right?
[1135.54 → 1136.64] But people don't want a toolbox.
[1136.84 → 1137.62] They want solutions.
[1137.82 → 1142.04] They want to have – and if you look at Home Assistant, our energy dashboard, that's a solution.
[1142.04 → 1153.64] You just select your couple of input sensors, and we generate a whole dashboard with graphs and, like, how much energy are you using, how much solar are you generating, and, like, you know, whole overviews.
[1153.64 → 1156.04] And that's something I would love to do more of it.
[1156.12 → 1158.22] But that's – basically, that's something we want to build.
[1158.46 → 1162.64] Once we have our default dashboards nailed, then we can start building on top of that.
[1162.82 → 1174.92] So environmental dashboard, just air quality throughout the house, humidity, looking at the security dashboard, automatically laying out all your cameras, and maybe if doors are open.
[1175.94 → 1177.86] Of course, we already have the energy dashboard.
[1177.86 → 1184.36] But, yeah, more of these dashboards that kind of are cut through your house, right, and give, like, just focus on one element of your house.
[1184.96 → 1195.24] Well, I think the automation blueprints kind of laid the foundation for some of that kind of community-fed knowledge to kind of be shared with people.
[1195.52 → 1197.42] But I think there's more that could be done.
[1197.54 → 1198.36] No, I agree.
[1198.50 → 1198.78] I agree.
[1198.86 → 1203.88] I mean, even on blueprints, right, like, we should be able – you now have to browse this forum.
[1203.88 → 1207.36] I actually want to turn it around where we say, you have this device.
[1207.52 → 1209.66] We have these blueprints that match this device.
[1210.28 → 1210.94] Yeah, yeah, yeah.
[1210.96 → 1212.52] Particularly if you own the hardware, right?
[1212.52 → 1212.62] Yeah.
[1213.04 → 1217.68] If you have the Home Assistant voice puck, then here's all the stuff it can do, by the way.
[1217.82 → 1218.00] Yeah.
[1218.54 → 1224.32] I think, Paul, what strikes me is when you first started talking about voice, you came on the show, and we chatted about it.
[1224.32 → 1235.66] And you've checked off just so many of the things that we talked about, you know, from working with the community to develop some of the voice modelling stuff, but, of course, also with Piper.
[1235.94 → 1240.84] And then this device now, which is fully modifiable by the end user.
[1241.04 → 1243.98] There's no way you could describe this thing as lockdown in any way.
[1243.98 → 1255.06] And I feel like you've kind of struck that balance of a device that end users can use, a device tinkers can use, and yet it's still something I want to pay for, I want to buy.
[1255.28 → 1256.32] I don't want to build myself.
[1256.48 → 1256.86] That's good.
[1257.12 → 1259.16] I think you guys have nailed this.
[1259.86 → 1260.26] Thanks.
[1260.44 → 1260.70] Thanks.
[1260.70 → 1261.26] It's really exciting.
[1261.48 → 1269.90] And it's really kind of completing the loop from the first time we had the conversation around voice to this end product, which, you know, I've been really enjoying.
[1269.96 → 1271.94] And I've been impressed, too, with the pickup range.
[1271.94 → 1274.80] I thought, oh, I'm going to buy, like, you know, a dozen of these.
[1275.14 → 1277.12] I think I'll probably only need, like, two or three.
[1278.00 → 1278.40] Yeah.
[1278.52 → 1280.28] No, the pickup range is perfect.
[1280.38 → 1285.86] And that's the XMOS chip that, besides, like, cleaning up the audio, it also automatically applies the gain.
[1286.00 → 1289.36] So it will use, if you're further away, it will increase the volume.
[1289.60 → 1295.42] So it's always, like, a normalized output, which is the level that the model is trained on, right?
[1295.50 → 1296.36] So speech and text.
[1296.70 → 1297.20] It's fantastic.
[1297.78 → 1298.38] So good.
[1298.38 → 1306.42] So one thing we want to do with this device is that we want many different companies to make voice assistants, right?
[1306.50 → 1313.16] Like, we don't want to be the gatekeeper of voice assistant hardware for the home assistant community, for the open home community.
[1313.16 → 1315.52] So we're going to open source everything of it.
[1315.58 → 1322.80] So the schematics, the firmware, the firmware that runs on the XMOS chip, the firmware that runs on the ESP chip, everything will be open source.
[1322.92 → 1330.88] And all the onboarding that we talked about at the beginning, all of that will be available for every voice assistant product that is going to be hooked up to home assistant.
[1330.88 → 1334.08] That is fantastic.
[1334.26 → 1335.72] Paulus, thank you for joining us once again.
[1335.74 → 1340.38] We're going to have links to everything in the show notes, but happy holidays to you and the whole team.
[1340.46 → 1342.36] This feels like a gift to the home assistant community.
[1342.72 → 1343.78] So yes, it is.
[1343.90 → 1344.34] It is.
[1344.40 → 1345.00] It's pretty awesome.
[1345.34 → 1346.24] It's going to be $59.
[1346.84 → 1348.00] I think that's a great price.
[1348.24 → 1352.56] You know, with that, I can afford to buy a few of them and put them around the house, and they're not too big.
[1352.64 → 1353.24] They're pretty discreet.
[1353.30 → 1354.60] They just need USB-C power.
[1355.56 → 1355.80] Yep.
[1356.34 → 1356.68] Perfect.
[1357.14 → 1357.98] Paulus, thank you so much.
[1357.98 → 1365.58] Go try it out for free for up to 100 devices and three users.
[1365.72 → 1368.48] Go to tailscale.com slash self-hosted.
[1368.54 → 1370.04] That's not a limited time deal.
[1370.56 → 1371.28] That's the deal.
[1371.44 → 1371.88] That's the plan.
[1371.90 → 1372.86] That's the plan I'm on.
[1373.20 → 1375.24] And I've been on it for a very, very long time.
[1375.64 → 1380.62] Tail scale is the easiest way to connect your devices and services to each other wherever they are.
[1380.70 → 1383.36] And it's powered by Wirecard.
[1383.36 → 1390.20] Secure remote access to your databases, to your applications, to your servers, to your Kubernetes cluster, whatever it might be.
[1390.66 → 1392.02] And tail scale is fast.
[1392.12 → 1393.70] Really, really fast.
[1394.00 → 1394.62] It's intuitive.
[1395.02 → 1395.98] It's easy to use.
[1396.22 → 1399.06] And ultimately, it's unlocking programmable network.
[1399.26 → 1401.68] And it lets you manage networking like it is code.
[1401.92 → 1402.98] You can deploy it.
[1403.22 → 1404.56] You can set it up with rules.
[1404.96 → 1406.58] It's really powerful.
[1406.58 → 1411.94] What you're building is a zero-trust flat mesh network that connects each device directly to each other.
[1412.00 → 1413.70] So you get a flat tail net.
[1414.22 → 1420.34] And if you have a node on a VPS and you have a node on your homeland, and you have a mobile device, they all exist in this virtual tail net.
[1420.70 → 1423.80] And then in there, you have all kinds of tools and capabilities.
[1423.80 → 1425.08] Like you can do name resolution.
[1425.26 → 1426.86] You can move files between your systems.
[1427.34 → 1428.86] You can have them talk directly to each other.
[1428.92 → 1431.24] You can host applications inside this tail net.
[1431.62 → 1432.88] And that's what I've chosen to do.
[1433.32 → 1435.66] Jelly, fin, everything I run at home.
[1435.66 → 1437.28] Anything new that I'm standing up.
[1437.50 → 1437.92] All of it.
[1437.98 → 1440.98] And I don't even bother putting it on the internet anymore.
[1441.22 → 1442.96] I just have to put it on my tail net.
[1443.60 → 1445.26] And then I just connect my nodes to the tail net.
[1445.30 → 1446.30] And I can get access to everything.
[1446.40 → 1447.48] No inbound ports at all.
[1447.96 → 1453.88] It makes old VPN systems seem, well, like legacy systems.
[1454.00 → 1458.74] It's one of those things where once you've experienced it, you've gone through a bit of a networking awakening.
[1459.20 → 1463.58] And it really fundamentally changes the things you can do with networking.
[1463.92 → 1464.74] You don't have to.
[1464.74 → 1467.42] You know, you could just use it as a VPN if you want.
[1467.68 → 1469.22] But it's so much more than that too.
[1469.62 → 1472.80] And it also ties in with your existing authentication infrastructure.
[1473.22 → 1476.16] So if you're a business, and you've been thinking about giving it a go, you can still go to
[1476.16 → 1477.68] tailscale.com slash self-hosted.
[1478.08 → 1478.54] Try it out.
[1478.78 → 1481.32] And then tie it in with your overall business authentication scheme.
[1481.82 → 1484.66] Take advantage of whatever it is you used to log in in your two-factor system.
[1485.32 → 1488.92] You just get started by going to tailscale.com slash self-hosted.
[1489.12 → 1492.28] That's tailscale.com slash self-hosted.
[1492.28 → 1499.54] Well, I'm sat here in my lovely bonus room with a friend of mine, Shane, who I've worked
[1499.54 → 1500.14] with in the past.
[1500.22 → 1501.08] Welcome to the show, Shane.
[1501.48 → 1502.12] Thank you, Alex.
[1502.18 → 1502.32] Hi.
[1502.98 → 1506.32] I didn't want to introduce you as this, but you are the developer of the Bento Box app that
[1506.32 → 1507.36] I mentioned a few weeks ago.
[1507.38 → 1507.60] That's true.
[1507.70 → 1508.08] I am.
[1508.08 → 1512.34] But you're also a Nix addict.
[1512.52 → 1513.16] Is that a fair?
[1513.44 → 1515.18] I think I'm a recovering Nix addict.
[1515.54 → 1515.84] Yes.
[1515.96 → 1516.22] Yes.
[1516.22 → 1518.30] That's what we're going to talk about, I think, in the show today.
[1518.82 → 1525.90] A carefully considered discussion of Nix on the server and why you and I might both be
[1525.90 → 1528.04] falling out of love a little bit with it, I think.
[1528.28 → 1529.02] I think that's fair.
[1529.02 → 1533.68] I think that we gave it a fair shake, and we have a number of things that we kind of came
[1533.68 → 1534.18] to realize.
[1534.92 → 1535.74] Are you ready for that, Chris?
[1536.96 → 1537.32] Yeah.
[1537.40 → 1538.40] And I want you to get comfortable.
[1538.90 → 1543.68] If you need to lay down first, go ahead and make yourself a cup of tea and then let's get
[1543.68 → 1544.10] into this.
[1544.20 → 1545.32] That's what they say on YouTube, right?
[1545.40 → 1548.38] Grab a snack, grab a drink, sit back, relax.
[1549.76 → 1550.94] Smash that like button.
[1551.26 → 1555.36] So listening to an episode of Linux Unplugged, I believe it was, what, a year ago?
[1555.62 → 1557.08] You had an idea for a project.
[1557.08 → 1557.52] Yeah.
[1558.04 → 1560.30] So, I mean, I'll admit this.
[1560.38 → 1562.32] I'm a long-time Unpaid user.
[1563.02 → 1566.68] And so I liked Unpaid for various aspects.
[1566.82 → 1570.56] One of the things that I really liked about it was the ease it was to start up applications.
[1571.30 → 1574.66] But one of the things I hated about it was I'm filling out these text fields.
[1575.20 → 1579.56] And I really liked the idea of a declarative Home lab configuration, something where I can
[1579.56 → 1583.54] have a folder with all of my files, and it's all my configuration for all of my Home lab
[1583.54 → 1583.82] apps.
[1584.46 → 1586.94] And so Nix kind of was the obvious choice.
[1586.94 → 1589.12] It was something that I was interested in.
[1589.28 → 1594.42] And at this time, I had a Nix server built out that was using Nix OS containers, which
[1594.42 → 1597.20] is a feature that's built into Nix OS.
[1597.46 → 1599.00] Is that the Spawn stuff?
[1599.18 → 1599.60] Exactly.
[1599.76 → 1600.96] The System Spawn.
[1601.66 → 1606.10] The short of it is you can essentially have small system configurations for each one of
[1606.10 → 1606.70] these containers.
[1606.70 → 1613.44] And so for each Home lab service, not only could I put, say, like, Sonar in there as a service,
[1613.44 → 1617.62] but I can also have Tail scale in this one container.
[1617.84 → 1619.28] And so I really fell in love with this.
[1619.38 → 1623.88] But there was an issue, which was that it was one giant monolithic config.
[1623.96 → 1627.32] Not only was it a config for a server and all the things you might have configured there,
[1627.38 → 1632.20] but then every service would have its own, like, child configuration.
[1632.20 → 1636.96] And so managing these containers was a separate command, which felt not Nix-y.
[1637.50 → 1641.78] And then having to recompile the closure became very painful.
[1642.14 → 1646.94] And so after listening to an episode of UP, everybody was talking about containers.
[1647.44 → 1649.90] And I was like, well, why can't I run Nix OS in a container?
[1650.12 → 1653.78] I'm already running it in these Spawn containers, but what if I can run it in a Docker container?
[1654.50 → 1659.68] And so it led me down this path of building an entire platform as a service, which is something
[1659.68 → 1662.82] I called Nix server, and I'm actually still running it.
[1662.90 → 1663.90] It's running most of my home lab.
[1664.12 → 1668.96] And what it allows you to do is write five 10-line Nix OS configurations where you can compose
[1668.96 → 1672.72] two, three, four different upstream services.
[1673.00 → 1676.64] And so for me, this was a dream of, oh, I'm going to build this out and release it to the
[1676.64 → 1677.02] community.
[1677.64 → 1679.50] But sadly to say, we never got there.
[1680.20 → 1684.56] We actually even met with a few of the movers and shakers in the Nix community on this one,
[1684.82 → 1686.86] you know, the Debts guys, for example.
[1686.86 → 1695.04] And we just ended up finding that the flexibility of the Nix module system just lacked a few
[1695.04 → 1696.74] knobs and dials that you need.
[1696.94 → 1701.98] You know, we were talking earlier before the episode about how if you wanted an application,
[1702.20 → 1708.18] for example, that had a sidecar database container, if you want to customize, was it Postgres you
[1708.18 → 1708.68] were talking about?
[1708.90 → 1709.22] Postgres, yeah.
[1709.34 → 1713.72] If you wanted to customize Postgres, you have to try and fork the upstream module, which
[1713.72 → 1714.96] that's easy, right?
[1714.96 → 1715.44] No.
[1715.72 → 1721.66] So if anybody's ever tried to replace a module, a service module in Nix, you'll know that it's
[1721.66 → 1723.84] kind of little bit of a nightmare, and it's pretty messy.
[1724.86 → 1728.64] And that is to say, like, Nix is, there are multiple parts to Nix.
[1728.86 → 1733.44] And specifically, the part that I really gripe with is the services side of things.
[1733.52 → 1735.46] There are a lot of inconsistencies upstream.
[1735.84 → 1740.00] And when building out Nix server, I strived to do a number of things that I was trying to,
[1740.00 → 1744.62] you know, fix from my experiences on Unpaid, which was if you're writing a file inside
[1744.62 → 1749.92] a container, sometimes that user is not the user that you're using on the server itself.
[1750.02 → 1754.60] And so how often have you ran into the situation where you're trying to read a file on your server?
[1755.02 → 1761.20] Lo and behold, it has a random user ID from whatever Docker container user that was set up.
[1761.20 → 1764.32] And so I had systems in place to fix this.
[1764.94 → 1768.50] And what I would find is that these upstream Nix OS modules would all implement the user
[1768.50 → 1769.32] slightly different.
[1770.04 → 1773.98] And replacing these or trying to jump in and modify them got really messy really quick.
[1774.60 → 1778.68] And if anybody's written services or looked at these services, you'll know that, like,
[1778.74 → 1779.64] they're very inconsistent.
[1780.22 → 1781.94] Now, on the flip side, Nix has packages.
[1782.58 → 1784.46] And their package system I actually really love.
[1784.50 → 1786.46] And I continue to use Nix to this day.
[1786.66 → 1789.38] I'm just starting to shy away from using Nix service modules.
[1789.38 → 1791.38] It's interesting.
[1791.62 → 1795.64] Chris, I'm curious to get your take on, like, how you find the module system to actually
[1795.64 → 1796.44] interface with.
[1797.00 → 1799.84] Well, I guess I'd like to know, how is it hard to...
[1799.84 → 1803.48] So I guess it sounds like if you want to take a module and change it, maybe you want
[1803.48 → 1804.86] to swap out the version of Postgres.
[1805.08 → 1807.24] It sounds like it gets hairy quickly.
[1807.74 → 1808.68] Could you go into detail there?
[1808.76 → 1811.06] What is hairy about forking the module?
[1811.62 → 1814.74] Overwriting, like, specific configurations is definitely possible.
[1815.24 → 1818.92] Like, if you're layering your service modules, you're able to override.
[1819.38 → 1820.64] A particular configuration.
[1820.94 → 1824.50] So if you want to change what port something's running on, you can typically do that.
[1825.10 → 1829.26] Where it gets a little hairier is that there are some configurations or there are some safeguards
[1829.26 → 1829.92] that are in place.
[1829.98 → 1831.78] Like, there are these assertions inside these modules.
[1831.92 → 1836.04] And particularly with Postgres, what I was doing was trying to change the Postgres user.
[1836.66 → 1841.76] So I wanted to be able to deploy Nextcloud inside a Docker container with Nix OS.
[1841.76 → 1847.38] And I wanted to make sure that the Postgres user was the same world writeable permissions
[1847.38 → 1848.72] as the systems' user.
[1848.90 → 1853.56] So if you're using Chris as your username on your server, that all the Postgres data
[1853.56 → 1855.18] matches up with Chris's user ID.
[1855.76 → 1859.34] Just so I understand, this is a Docker container that already exists or a Docker container you're
[1859.34 → 1860.34] composing with Nix?
[1860.48 → 1863.04] It's a Docker container composed with Nix.
[1863.16 → 1868.22] So Nix server would essentially spit out Docker containers that would boot up Nix OS inside
[1868.22 → 1868.54] of them.
[1868.74 → 1868.82] Okay.
[1869.32 → 1869.56] All right.
[1869.70 → 1875.70] And I think the downside is those two modules don't necessarily know, they have no context
[1875.70 → 1876.62] of each other whatsoever.
[1876.90 → 1882.36] The Postgres module is a standalone thing and the Nix cloud module is a standalone thing.
[1882.78 → 1886.06] They're not designed like a stack of containers might be.
[1886.06 → 1891.60] They're not always the case, but there's no logic between the two to have any relationship
[1891.60 → 1893.26] for the users to match up at all.
[1893.36 → 1898.16] So if you end up in a situation like here where the database user doesn't match,
[1898.22 → 1904.52] the app user, you can end up in a situation where the two are just completely doing their
[1904.52 → 1905.06] own thing.
[1905.58 → 1909.76] And the goal, just again, also I'm following, the goal is to just always be able to use the
[1909.76 → 1910.88] upstream module, right?
[1910.90 → 1912.38] That's kind of like the end goal, ideally.
[1912.84 → 1912.98] Yeah.
[1913.04 → 1915.76] So you can create overlays for packages.
[1916.60 → 1919.08] And so you can bring in like unstable versions of your packages.
[1919.08 → 1923.52] But if you wanted to replace a service module like services.tail scale.enable equals true,
[1923.52 → 1926.44] one of those modules, it's a lot trickier.
[1926.44 → 1931.94] You have to like to put it on like a deny list essentially, and then be able to shoehorn in
[1931.94 → 1933.30] your own module on top of that.
[1933.38 → 1935.48] So forking it becomes a little messy.
[1935.92 → 1940.38] And so really what I ran into is when I was trying to customize these modules to run inside
[1940.38 → 1944.10] of a container, to have proper permissions, to essentially build out my home lab.
[1944.26 → 1949.36] I ran into situations where the way that the upstream modules were written, a lot of times
[1949.36 → 1951.58] are to be hard-coded values within the module itself.
[1951.58 → 1956.04] So it would require me going and posting a pull request and asking for it to be turned
[1956.04 → 1957.48] into a variable.
[1958.60 → 1958.96] Sure.
[1959.28 → 1961.66] Or the way that it was just configured and composed.
[1961.78 → 1966.82] There are so many assumptions in there that it was really the problem of like inconsistency.
[1967.38 → 1968.84] So I reached the point-
[1968.84 → 1970.66] As you often see with community-created stuff, right?
[1970.70 → 1972.02] Is they're kind of scratching their own itch.
[1972.10 → 1972.34] Yeah.
[1972.58 → 1976.92] And, you know, I'd reach the point where I'd go to deploy a new service, and I'd actually
[1976.92 → 1977.58] get really worried.
[1977.64 → 1979.24] I'm like, okay, what am I going to uncover here?
[1979.74 → 1980.92] And I think we've all come down.
[1981.70 → 1982.66] We've all felt that.
[1982.78 → 1986.10] Like, I know that you've done the next, I'm sorry, the next cloud module recently.
[1986.58 → 1989.12] And it becomes a whole thing where it's like, let me open up this module.
[1989.22 → 1990.06] What options are there?
[1990.06 → 1992.14] And you have to like to learn each and every module.
[1992.40 → 1994.16] And I wish there was more consistency there.
[1994.94 → 2000.54] And you end up, instead of reducing friction for trying out new projects, you end up kind
[2000.54 → 2001.42] of increasing it.
[2001.90 → 2007.62] It also relies on what's available in Nix packages or the Nix module ecosystem.
[2007.62 → 2010.00] Because I know it exists now.
[2010.08 → 2014.22] But when we were looking at it in the summer, Image wasn't in the Nix module system.
[2014.36 → 2014.52] Sure.
[2015.00 → 2018.24] I mean, to be fair to Nix, Nix is probably one of the most expansive.
[2018.64 → 2020.32] I mean, maybe the AUR.
[2020.32 → 2024.44] But Nix is probably the second, if not the most expansive package.
[2024.48 → 2024.94] No doubt.
[2025.06 → 2030.34] But that kind of ignores the other elephant in the room that Docker's become the kind
[2030.34 → 2034.86] of standardized packaging format for a lot of apps to ship their software with.
[2035.62 → 2036.40] Nix goes off and does it.
[2036.40 → 2037.06] Before you go there, though.
[2037.12 → 2037.72] But I agree with you.
[2037.76 → 2038.20] Before you go there.
[2038.24 → 2039.82] Going back to the module stuff.
[2039.82 → 2044.94] See, I actually find what you describe as friction, that's how I learn.
[2045.18 → 2047.34] Like, it's nice having all these options.
[2047.50 → 2051.40] I like being able to understand all of this and learn these capabilities there and being
[2051.40 → 2056.72] able to just go to this one spot and understand everything this is capable of doing.
[2056.84 → 2059.64] I find that to be remarkably time-saving.
[2059.74 → 2061.56] So for me, I don't find that to be friction at all.
[2061.56 → 2065.44] But I do agree with you on the Docker container thing.
[2065.54 → 2068.00] It's like, that's where the industry is going and has gone.
[2068.12 → 2068.72] Is there.
[2068.96 → 2071.72] Is really distributing software in containers.
[2072.48 → 2079.64] Docker has ended up becoming like the standard packaging format for the Linux home server ecosystem.
[2080.20 → 2083.42] Also, there's a lot of stuff going on in the industry with it too, of course, with Kubernetes
[2083.42 → 2084.24] and that kind of thing.
[2084.36 → 2089.60] But the other thing that you touched on briefly, Shane, was talking about rebuilding the entire
[2089.60 → 2095.24] closure every time and how that can kind of be an impediment to quick iteration.
[2095.84 → 2100.88] And the fact that you can't just make a one line change and have just that one thing change.
[2100.98 → 2103.32] It re-evaluates the entire world every time.
[2103.74 → 2105.02] Yeah, I think that's true.
[2105.78 → 2110.72] We've all been there where you mess up a line of a configuration, and now you're staring at
[2110.72 → 2112.26] a parser like error.
[2112.52 → 2116.46] And it doesn't really have anything to do with where your mental context was.
[2116.52 → 2118.30] But now you have to understand Nix as a language.
[2118.30 → 2120.26] And it takes a certain amount of effort.
[2120.44 → 2123.74] And eventually you get used to reading these things, and you get the muscle memory.
[2124.18 → 2127.62] But this iteration cycle of like, OK, time to go rebuild and rebuild this.
[2127.78 → 2131.98] The way that Nix server worked itself is, again, it would build out an entire closure and shove
[2131.98 → 2133.00] it into a Docker image.
[2133.50 → 2137.90] And so on of the things I started thinking about, and if I jump to Nix Darwin real quick,
[2137.96 → 2142.78] is that my Nix Darwin configuration feels really great when I set up a new machine.
[2142.78 → 2148.46] Like taking a new machine out of the box, cloning my repo and running one command and having
[2148.46 → 2150.66] everything in its place, even my macOS apps.
[2151.58 → 2157.56] However, when I use it day to day, that iteration that you're talking about, Alex, that building
[2157.56 → 2159.20] the whole world, it becomes an impediment.
[2159.80 → 2162.06] Like I'm sitting there, and I just want to make this one line change.
[2162.14 → 2164.72] I think I was working with you today, and we needed to update your path.
[2164.72 → 2169.66] And it was like five minutes of like getting to the right place of the configuration, making
[2169.66 → 2172.60] the change and then building, having to type your password a few times.
[2173.08 → 2176.74] And so there's something there where it's like the payoff happens like when you're setting
[2176.74 → 2181.94] up a new system, but then like what you're paying every day doesn't feel worth it.
[2182.36 → 2188.04] See, I feel like this is a flip side too, because in one way, as somebody who doesn't always
[2188.04 → 2192.52] know what he's doing, I appreciate that if it's not right, it won't build.
[2192.52 → 2197.04] And I also can YOLO because I know if it's not right, it won't build.
[2197.24 → 2200.82] I can just throw something in there and let's just see how it goes.
[2201.00 → 2204.68] And sometimes it works the first try, and sometimes I have to iterate a few things.
[2205.40 → 2210.70] And then when you combine like the output error messages with something like Claude, I can
[2210.70 → 2212.98] get to the bottom of it in like 15, 30 seconds.
[2212.98 → 2215.42] So I don't find that to be too particularly cumbersome either.
[2215.86 → 2221.24] I do agree that, you know, yeah, it does sometimes take a while to build, but that just sort of depends
[2221.24 → 2225.94] on how much you're managing with Nix, because I don't think we should lose sight of the fact
[2225.94 → 2229.82] that there's Nix and there's Nix OS and you could use Nix like you just said on Darwin
[2229.82 → 2231.82] and you could just have it manage five, 10 packages.
[2232.52 → 2234.14] And that really wouldn't be such a problem.
[2234.20 → 2235.42] It just really depends on the scope.
[2236.02 → 2240.50] And it's kind of funny because, you know, I think you can go too far with it and I think
[2240.50 → 2243.38] you can have it manage too much stuff, and then you end up kind of in the position you're
[2243.38 → 2247.72] at because it seems like to me this is a system like this build system.
[2247.72 → 2249.40] This is how developers would do it, right?
[2249.44 → 2250.78] This is how software development works.
[2250.88 → 2252.34] Is it either builds or it doesn't build?
[2253.10 → 2255.14] And so this is how software developers think about it.
[2255.40 → 2257.64] But it's not really, I think, how systems people think about it.
[2258.44 → 2264.86] I do enjoy stuff like when you remove a package from your configuration that Nix will evaluate
[2264.86 → 2265.86] the entire world.
[2265.96 → 2268.02] I mean, like you say, it's a flip side.
[2268.18 → 2272.80] Sometimes it's a curse, and sometimes it's a blessing where it will automatically remove the
[2272.80 → 2278.40] thing that you've removed from your configuration and deploy that thing as an entire, you know,
[2278.46 → 2278.84] artifact.
[2279.62 → 2284.04] But it's just, I wish there was kind of, I guess, I guess what I'm asking for is like
[2284.04 → 2286.18] two modes, like a Jekyll and a Hyde.
[2286.70 → 2291.88] One which is like a pure mode, which is only deploying what's fully and evaluate the entire
[2291.88 → 2292.28] closure.
[2292.58 → 2298.14] The other one is a really quick like dev mode where I can just, you know, I know there's
[2298.14 → 2300.46] Nix shell and all that kind of stuff for like short term stuff.
[2300.58 → 2308.34] But like, let's say I'm working on a configuration for Starship or for ZSH or for Neovim or something
[2308.34 → 2308.74] like that.
[2308.76 → 2312.02] And I just, you know, I want to hot reload the config essentially.
[2312.30 → 2317.42] Can I put myself into a temporary hot reload mode where it's only looking at a very small
[2317.42 → 2318.94] portion of the world?
[2320.02 → 2324.32] I think another idea is being able to mutate the world and then have it read what that
[2324.32 → 2325.12] mutation was.
[2325.12 → 2330.50] Like I edited the config by hand and then like you can import that into the Nix OS config.
[2330.62 → 2331.76] So it feels a little more natural.
[2332.04 → 2335.58] I think where I'm at with Nix right now is I do love it for configuration.
[2335.74 → 2338.42] I do love it for packages, and I'm going to continue to use it that way.
[2338.82 → 2342.10] But actually I spent a considerable amount of time over the last few months building a
[2342.10 → 2344.68] separate project where I've convinced myself for my home lab.
[2344.76 → 2349.02] I think I'm moving away from Nix and specifically these Nix service modules.
[2349.60 → 2350.76] And I'm going back to Docker.
[2350.76 → 2355.72] And one of the simple reasons of going back to Docker is its kind of like the Ubuntu thing
[2355.72 → 2357.12] where it is the standard.
[2357.42 → 2358.84] There's always an example for it.
[2358.84 → 2360.74] You can go to official upstream repos.
[2360.86 → 2366.00] And if you're a project maintainer like Image, you feel a responsibility to publish a Docker
[2366.00 → 2366.72] compose file.
[2367.18 → 2370.44] And so with Nix, it's kind of like this mix of the community is going to maintain it.
[2370.44 → 2375.82] And, you know, up to the author, how they're going to interpret the needs and how they're
[2375.82 → 2377.22] going to implement the service module.
[2377.86 → 2380.26] And there just is that lack of consistency.
[2380.50 → 2385.42] And like what I really want, and maybe this, if this future exists, I'll switch back is if
[2385.42 → 2390.14] we saw more package developers or the service developers publishing their own flakes.
[2390.56 → 2394.44] So then they were the ones controlling what that service module interface was like.
[2394.96 → 2395.36] That'd be great.
[2395.48 → 2396.60] That'd be great if it came from them.
[2396.60 → 2399.62] Like they do with Docker compose files today and Docker images today.
[2399.62 → 2400.34] Yeah, yeah, absolutely.
[2402.46 → 2406.14] K-E-E-B dot I-O slash self-hosted Ki bio.
[2406.42 → 2410.22] Go over there, sign up for their newsletter and take 5% off your first order.
[2410.84 → 2415.66] Ki bio, they specialize in beautiful, well-built open keyboards.
[2416.00 → 2419.40] A lot of split keyboards, the ones I really like, but they also have those regular types
[2419.40 → 2421.18] for you folks that don't want the split keyboard.
[2421.60 → 2425.54] On Black Friday, keep an eye out for one of their keyboards that's a lot like the Microsoft
[2425.54 → 2428.90] Natural 4000, which was a great keyboard back in the day.
[2428.90 → 2433.88] But this one's even more ergonomic, lots of options, and it's going to be at a great price.
[2434.46 → 2438.82] Their keyboards come fully built, or you can get in a kit and assemble it yourself.
[2439.16 → 2442.58] And a lot of the parts you're going to have no problem with because everything is hot
[2442.58 → 2442.88] swapped.
[2442.96 → 2444.74] So there's no soldering for any of that kind of stuff.
[2445.04 → 2447.58] They also have macro pads with like 9 to 16 keys.
[2447.94 → 2450.32] I use that here in studio for my OBS machine.
[2450.70 → 2451.60] There are all kinds of things.
[2451.64 → 2453.94] You could do like a homemade stream deck with that thing.
[2453.94 → 2458.60] Or maybe you want to have like a home theatre PC control board or shortcuts for home assistant.
[2458.86 → 2460.90] Those are really, really slick.
[2461.32 → 2466.06] And because of who they are, they also have lots of DIY parts like microcontrollers and
[2466.06 → 2467.40] they support open source.
[2467.62 → 2474.10] They publish 3D printed parts, and they're part of the core QMK firmware team.
[2474.10 → 2476.62] And all of their keyboards use QMK.
[2477.42 → 2479.52] If you're a keyboard person, you know that's a big deal.
[2479.92 → 2481.34] So go check out Kee bio.
[2481.60 → 2485.06] It's K-E-E-B dot I-O slash self-hosted.
[2485.20 → 2487.00] If you sign up for the newsletter, get 5%.
[2487.00 → 2491.06] Then go there and grab one of those Black Friday, Cyber Monday deals and get yourself
[2491.06 → 2493.82] a keyboard that deserves to be touched all the time.
[2494.02 → 2496.32] You're interfacing with your hardware all the time.
[2496.40 → 2499.20] If you're anything like me, why not have it been great?
[2499.66 → 2500.78] Why not have it feel great?
[2500.78 → 2504.90] And why not have it been something you can repair and fix that runs an open firmware?
[2505.28 → 2506.72] Support the show and check them out.
[2506.76 → 2509.40] Go to K-E-E-B dot I-O slash self-hosted.
[2509.52 → 2512.02] That's Kee bio slash self-hosted.
[2513.46 → 2515.90] So what's the idea behind where you're headed?
[2516.16 → 2521.52] Is it a directory full of compose files that you can kind of ingest into some tool or what?
[2521.56 → 2522.16] Like what's going on?
[2522.70 → 2525.82] So I actually started and I kind of just reset my brain of like,
[2525.86 → 2527.18] what do I want to do in my home lab?
[2527.28 → 2528.22] What am I deploying?
[2528.22 → 2531.34] And it came down to like a handful of things.
[2531.60 → 2533.28] I have cron jobs.
[2533.40 → 2534.24] I have shell scripts.
[2534.48 → 2536.10] Sometimes I'm a Go developer.
[2536.28 → 2538.86] So I have binaries that I need to run that I'll write myself.
[2539.42 → 2542.50] A lot of times Docker images or Docker compose files.
[2543.52 → 2546.64] And what is a reasonable way to manage all of this?
[2546.68 → 2549.18] And like there isn't one system that really addresses it.
[2549.84 → 2554.82] And so I had this idea of like, well, what if I could, you know, laugh if you want to,
[2554.82 → 2558.62] but what if I could yeet a binary onto a server, and it would run as a service?
[2559.40 → 2563.78] What if I could just SCP that file, and it would automatically configure itself as a service?
[2563.88 → 2564.90] And so this is where I started.
[2565.10 → 2567.82] And that's kind of where I started and what I built.
[2568.06 → 2572.02] And where I landed on is this project that I'm calling yeet for fun.
[2572.02 → 2574.70] And you can yeet any one of these things.
[2574.70 → 2579.30] You can yeet a binary or Docker image or Docker compose file to a remote system.
[2579.42 → 2580.76] So you can run this from your laptop.
[2581.18 → 2585.86] And what I'm experimenting with is standing these up as system services when it's like
[2585.86 → 2587.24] a script or if it's a binary.
[2587.48 → 2591.26] I wrap Docker and Docker compose if you're pushing an image or if you want to just send
[2591.26 → 2592.02] a compose file.
[2592.02 → 2594.84] And then I stand them up inside their own network namespace.
[2595.18 → 2600.26] And one of the goals, because I love Tail scale, was I wanted to attach Tail scale to each one
[2600.26 → 2600.86] of these services.
[2601.20 → 2603.46] And this was something I didn't talk about a few minutes ago.
[2603.54 → 2607.92] But one of the things that I was really striving for with Nix and Nix service modules and what
[2607.92 → 2613.90] I did with Nix server was I love the composability where Docker containers typically are like, well,
[2613.98 → 2615.52] here's your one thing that you're running.
[2615.92 → 2618.72] And if you want to put Tail scale there, you do it as a sidecar.
[2618.72 → 2622.34] And I kind of got tired of writing like Docker compose files with sidecars.
[2622.48 → 2625.84] I love that in Nix, I could just do services.tail scale.enable.
[2626.54 → 2632.02] And so what I built into this tool, this Yeet program, is the ability to not only put your
[2632.02 → 2635.64] services on your LAN, but you can also put them on your Tail net automatically.
[2635.80 → 2637.10] So you don't have to write sidecars.
[2638.10 → 2638.98] I love it.
[2639.52 → 2641.46] So is this running like on an Ubuntu system?
[2641.64 → 2643.36] Is this a Debian or is this on Nix?
[2643.58 → 2644.68] It's Ubuntu, yeah.
[2644.98 → 2645.24] Okay.
[2645.58 → 2647.18] So then I use Yeet on top of that?
[2647.18 → 2647.62] Yeah.
[2647.72 → 2650.74] So you use Yeet like on your laptop, whether that's, you know, Linux, Mac.
[2650.74 → 2650.98] Oh, yeah.
[2651.40 → 2654.60] And then you point it at an Ubuntu server.
[2654.96 → 2657.06] And it's kind of Tail net first.
[2657.26 → 2661.14] And so this was an opinion I took, which is like, I love the Tail net because when things
[2661.14 → 2662.32] are there, they get pretty names.
[2662.42 → 2663.36] They get TLS certificates.
[2663.56 → 2664.58] They get reverse proxies.
[2664.68 → 2665.52] All this stuff for free.
[2665.62 → 2666.08] And guess what?
[2666.10 → 2667.20] It's all reachable, right?
[2667.80 → 2667.96] Yeah.
[2668.00 → 2670.28] And so I put every service I have is on my Tail net.
[2670.44 → 2673.34] And so when you start up Yeet, it automatically gets on your Tail net.
[2673.34 → 2677.42] You interface with it remotely from the start, which means that you have security built in.
[2677.62 → 2678.74] It's just using your ACLs.
[2679.42 → 2681.38] And you just start throwing files up.
[2681.48 → 2684.86] And underneath, it's just using SSH and SCP to transfer the files.
[2685.56 → 2691.04] And yeah, so it's something that I'm curious, like what the community thinks about, like,
[2691.28 → 2692.82] what if we went back to Docker Compose?
[2692.90 → 2695.82] What if you could just create a repository of all your Compose files?
[2695.82 → 2700.00] And there was a tool that let you spray them onto your servers and manage them as services
[2700.00 → 2700.54] for you.
[2700.88 → 2702.14] I've kind of gotten a little tired.
[2702.48 → 2708.02] About six or seven years ago, I wrote what I call the Docker Compose generator in Ansible.
[2708.12 → 2713.64] So my workflow for the last six or seven years has been creates a massive YAML dictionary
[2713.64 → 2719.14] with a bunch of entries that I can then specify, like per container.
[2719.30 → 2724.06] And then the Ginger 2 emulating iterates over that and spits me out a Docker Compose file.
[2724.06 → 2729.62] The benefit of that is that I can have secrets in an encrypted file, as long as I don't push
[2729.62 → 2731.06] them to GitHub like I did this week.
[2732.22 → 2738.34] And then I can have it, you know, use Ansible to talk to multiple servers over SSH.
[2738.46 → 2740.32] I manage all the JOE infrastructure that way.
[2740.38 → 2742.44] I manage all my personal cloud infrastructure that way.
[2743.58 → 2748.88] What does Yeet do to manage things like secrets and things like that?
[2748.92 → 2753.14] Is it just all plain text in the Compose file on your box and just gets yeeted over?
[2753.14 → 2754.64] Or like, how does that work?
[2754.84 → 2759.72] Yeah, I thought about this because when I implemented this for Nix server, I did it in like a very
[2759.72 → 2761.06] security focused way.
[2761.78 → 2767.62] You had secure like encryption to talk to your Nix box, and then you'd have age encrypted
[2767.62 → 2768.16] secrets.
[2769.06 → 2770.52] I kind of went overboard with it.
[2770.60 → 2773.16] And then I took a step back, and I looked at what was happening in the Docker world.
[2773.20 → 2775.02] I'm like, oh, these are just all environment variables.
[2775.46 → 2778.04] And you go look at GitHub actions for how infrastructure is deployed.
[2778.18 → 2779.50] And it's a lot of environment variables.
[2779.98 → 2782.76] Ensure there's vault and there are secure ways to be able to pull these things.
[2783.14 → 2787.16] But where I landed with Yeet was like, let's just let's treat the home lab as what it is.
[2787.26 → 2789.72] Like, this is your sandbox that you're playing in.
[2790.04 → 2791.66] It's my pseudo production, gosh darn it.
[2791.82 → 2794.36] And so like it's in your environment files.
[2794.46 → 2796.62] You can SCP up like, you know, secret files.
[2796.72 → 2800.36] Like today we SCP'd up one of your OAuth secrets.
[2800.76 → 2804.82] But then the rest of it is like you just edit an environment file, and you can type that in
[2804.82 → 2807.00] there, and it just exists in memory.
[2807.34 → 2808.50] I admit I had to look it up.
[2808.50 → 2809.28] I'm an old man.
[2809.78 → 2815.54] It is a verb, yeet, to throw something with force and without regard for the thing being
[2815.54 → 2815.78] thrown.
[2815.86 → 2816.56] And now I get it.
[2817.12 → 2818.42] You're meeting the files.
[2818.58 → 2820.84] You're meeting the Docker composers up onto the system.
[2820.90 → 2821.30] Exactly.
[2821.30 → 2825.44] You know, what's funny is Drew, our editor, is the one that educated me on what yeet means
[2825.44 → 2826.22] a few years ago.
[2826.24 → 2826.60] Really?
[2826.82 → 2827.80] I just had to look it up.
[2829.64 → 2835.12] So I'm curious, like we're talking about Yeet as if it's this publicly available project,
[2835.12 → 2837.28] which isn't the case right now.
[2837.34 → 2838.28] What are your plans for it?
[2838.28 → 2840.08] Yeah, I want to make it publicly available.
[2840.96 → 2845.34] Like what you know, I onboarded Alex earlier today and I said, okay, here's what I'm doing.
[2845.38 → 2848.20] And immediately you hit some edge cases.
[2848.54 → 2850.18] So there are assumptions that we made in building this.
[2850.24 → 2851.26] I made it with another developer.
[2851.90 → 2854.36] So our plan is right now going into the holiday season.
[2854.48 → 2857.40] Hopefully we'll have some time to put our head down and polish it up a bit.
[2857.64 → 2861.86] And really, I just want to write the documentation, so people can invite themselves onto it.
[2862.00 → 2864.16] And yeah, so let's look forward to 2025.
[2864.16 → 2868.90] 2025, let's say January, February, I'll shoot Alex a note, and we'll get this in people's
[2868.90 → 2869.12] hands.
[2869.88 → 2870.20] Excellent.
[2870.52 → 2871.28] Well, we will update.
[2871.38 → 2874.14] And of course, when we have a link, we'll put one in the show notes for that episode
[2874.14 → 2874.48] too.
[2875.20 → 2877.38] Sounds like a, oh, I should have looked up another.
[2877.52 → 2881.94] It sounds like an exclamation of excitement and approval, surprise, or energy too, Shane.
[2884.44 → 2887.68] I guess also it's Australian slang for a very strong yes.
[2888.52 → 2889.00] Is it?
[2889.22 → 2889.60] Okay.
[2889.72 → 2890.40] That's new to me.
[2890.56 → 2890.64] Yeah.
[2890.68 → 2891.28] Well, there you go.
[2891.28 → 2895.96] Well, so the reason you're actually here, Shane, is that you're moving house and you
[2895.96 → 2899.06] wanted to co-locate your server in my basement.
[2899.36 → 2901.54] And we ran a fun little experiment this morning.
[2901.82 → 2903.40] You left your house at what time?
[2903.56 → 2905.38] 7:8 a.m., something like that?
[2905.46 → 2908.98] I unplugged the server at 7.30 in the morning, and we left at 8.
[2909.46 → 2909.68] Yeah.
[2909.86 → 2914.78] So you brought your server from Connecticut, checked it in the belly of the plane, just
[2914.78 → 2915.88] in a massive suitcase.
[2915.88 → 2921.36] I wrapped it in a towel because the suitcase itself was almost the exact dimension of
[2921.36 → 2922.32] the 4U case.
[2922.54 → 2922.66] Yeah.
[2922.70 → 2923.60] And this was a full size.
[2923.60 → 2924.68] And the towel will take care of it.
[2924.70 → 2925.02] It's fine.
[2925.84 → 2929.08] With a handwritten sign saying, this is a server on top.
[2930.34 → 2933.92] It weighed 53 pounds without the 12 drives in it.
[2934.46 → 2937.00] And so they dinged me with the overage on that.
[2937.16 → 2938.20] And so that was painful.
[2938.72 → 2939.68] And then it was the tension.
[2940.30 → 2944.08] You know, I put the note in there, like Alex said, and I was just so afraid TSA would open
[2944.08 → 2944.70] this up.
[2945.10 → 2946.32] And I was talking to Alex.
[2946.38 → 2948.36] I'm like, I don't think the millimetre wave can get through.
[2948.46 → 2949.88] I don't know if they know what this is.
[2950.32 → 2951.38] And I actually overheard.
[2951.44 → 2952.60] I was flying out of a small airport.
[2952.70 → 2956.38] I overheard the TSA agent tap another one and saying, hey, we need your help.
[2956.44 → 2959.80] There's something called a server we need you to look at.
[2961.38 → 2961.78] Wow.
[2961.94 → 2964.90] We added an hour by stopping for lunch on the way home from the airport.
[2965.12 → 2965.40] That's fair.
[2965.40 → 2968.46] It's a quick, what, 90 minute flight from Connecticut down here.
[2969.48 → 2972.72] And we had it up and running by what, three o'clock this afternoon?
[2972.84 → 2975.22] So if we take an hour off for lunch, we'll say two o'clock.
[2975.90 → 2979.86] So what was the theoretical bandwidth of your plane flight today?
[2980.04 → 2983.50] I think we estimated, I think there's about 30 terabytes of storage space.
[2983.98 → 2989.16] And so with all those drives and with the time, we just broke 10 gigabits a second, constant.
[2989.44 → 2989.96] There you go.
[2990.06 → 2990.84] That's not bad.
[2991.02 → 2991.82] That's not bad.
[2991.82 → 2995.26] And I think we still achieved 99.99% uptime.
[2995.40 → 2998.30] And as far as you know, no packet loss.
[2999.14 → 3000.22] No packet loss.
[3000.32 → 3000.82] There you go.
[3001.08 → 3001.66] Knock on wood.
[3002.82 → 3005.22] Well, Shane, it's a good adventure.
[3005.30 → 3008.28] But thank you for being here today and chatting with us.
[3008.76 → 3011.00] I also want to say thank you to Paulus.
[3011.34 → 3018.88] You know, when he was wrapping up with us, Alex, he mentioned that folks are doing 3D printed cases for these little units.
[3018.88 → 3024.08] Yeah, it sounds like there's some really fun designs because it's a fully open source project.
[3024.56 → 3026.60] 3D printed models for the case and stuff like that.
[3026.66 → 3029.74] He mentioned there was a minion design that's going to be pretty fun.
[3030.66 → 3031.54] What was the other one?
[3031.60 → 3032.42] Was it a Poke ball?
[3033.18 → 3033.90] Yeah, a Poke ball.
[3034.02 → 3036.60] I could see like, you know, somebody's going to do a Starship Enterprise.
[3036.90 → 3038.24] You know, there's Star Trek geeks.
[3038.34 → 3039.08] They're going to make it so.
[3039.08 → 3040.70] Oh, good, Alex.
[3040.80 → 3041.58] Good for you.
[3042.20 → 3043.36] Good Star Trek fan.
[3043.46 → 3044.30] I'm very proud of you.
[3044.36 → 3044.78] Good fun.
[3045.58 → 3049.10] Now, this is a special early holiday episode recording.
[3049.28 → 3051.14] So we won't have feedback or boost this episode.
[3051.28 → 3053.12] But we don't have very many boosts.
[3053.16 → 3057.10] If you want to send us a holiday boost, we will include it in the next episode when we get together.
[3057.60 → 3063.92] And of course, you can always go to self-hosted. Show slash contact and use the old classic email contact form.
[3064.64 → 3066.60] The old school email form, huh?
[3067.06 → 3067.40] Mm-hmm.
[3067.40 → 3069.00] I think it still works as far as I know.
[3069.08 → 3069.64] Is that still there?
[3069.70 → 3070.36] Does it still work?
[3070.44 → 3070.84] I think.
[3071.02 → 3071.22] Yeah.
[3072.36 → 3074.92] I think they might be privatizing email though, so watch out.
[3075.74 → 3077.64] Is that a new Doge initiative or something?
[3078.38 → 3079.44] That was a joke, yeah.
[3080.02 → 3080.50] Good lord.
[3081.40 → 3087.46] Well, as always, I want to say a big thank you to our site reliability engineers over at self-hosted. Show slash SRE.
[3088.06 → 3091.40] You get an ad-free show as well as a special post show.
[3091.46 → 3092.80] What are we going to be talking about today, do you think?
[3092.96 → 3094.84] It's going to be Alex's choice.
[3095.02 → 3096.16] I've got, look at that.
[3096.16 → 3097.16] You scroll down there a little bit.
[3097.18 → 3099.06] Look, I've got a couple of really juicy ones in there for you.
[3099.62 → 3099.82] Yeah.
[3099.90 → 3100.96] There are a couple ones we should probably talk about.
[3100.96 → 3102.72] You're not even going to mention drones over in New Jersey.
[3102.86 → 3103.32] Good for you.
[3103.60 → 3103.88] Nice.
[3104.28 → 3104.56] I know.
[3104.74 → 3105.16] Look at me.
[3106.52 → 3110.84] Don't forget to check out meetup.com slash Jupiter Broadcasting for any upcoming last
[3110.84 → 3112.20] minute meetups we might have.
[3112.20 → 3122.78] Oh, you know, I'll mention we're putting together some meetups for UP 600, and we're trying out a new self-hosted meetup alternative at colonyevents.com.
[3122.78 → 3125.30] And if it works for UP 600, I think that's what we'll use in the future.
[3126.48 → 3128.44] And it's called Gathic or something.
[3128.66 → 3137.14] And it's kind of nice because the listeners can create their own events and then a little bit after the event wraps up, it self-deletes, and it just cleans up after itself.
[3137.14 → 3145.88] So we're testing colonyevents.com, and we're soliciting meetups for UP 600, which is going to be like February 2nd or something.
[3145.96 → 3146.44] Good Lord.
[3146.54 → 3147.52] Episode 600.
[3147.96 → 3148.82] Can you believe that?
[3148.82 → 3148.94] No.
[3150.28 → 3150.52] No.
[3150.96 → 3153.00] And Coder just hit 600 this week too.
[3153.28 → 3153.96] What's 600?
[3154.14 → 3155.28] Is that like five years?
[3155.38 → 3156.26] It must be more than that.
[3156.60 → 3157.40] No, it's more than that.
[3157.50 → 3160.64] It's older than my daughter, Bella.
[3160.76 → 3161.90] 11 and a half years.
[3161.92 → 3162.40] Are you kidding?
[3162.96 → 3163.80] Yeah, it's crazy, huh?
[3165.74 → 3166.28] All right.
[3166.32 → 3169.48] So you can go to alex.ktz.me to find me on the internet.
[3169.66 → 3171.64] Where can folks go to find you, Shane?
[3171.86 → 3172.84] I'm not really on the internet.
[3172.98 → 3174.30] No, GitHub.com slash Shane.
[3175.08 → 3177.18] We'll put a link to that in the show notes.
[3177.20 → 3177.54] All right.
[3177.54 → 3184.30] You can find me on the Weapon X if you want, Chris LAS, or you can try the Foster thing, chrislas.com.
[3184.66 → 3187.78] And, of course, all the great shows over at jupiterbroadcasting.com.
[3188.42 → 3189.44] Thank you very much for joining us.
[3189.50 → 3190.92] I appreciate you coming on, Shane.
[3191.16 → 3194.42] And that was self-hosted. Show slash 139.
