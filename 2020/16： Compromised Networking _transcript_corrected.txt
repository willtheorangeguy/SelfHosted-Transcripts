[0.10 → 6.32] Coming up on Self-Hosted 16, we're getting to some network basics and tips for solid Wi-Fi connectivity.
[6.80 → 10.06] Plus, we make the biggest compromise in the history of the show.
[10.50 → 11.10] I'm Alex.
[11.42 → 11.90] I'm Chris.
[12.02 → 13.58] And this, Self-Hosted 16.
[14.88 → 15.74] Hello, Alex.
[15.96 → 17.66] Staying sane while staying indoors, I assume?
[18.08 → 18.80] Doing my best.
[18.94 → 22.38] Yeah, I realized I haven't actually left this building in four days.
[22.80 → 27.24] You're such a nerd, though, because you sent me a screenshot of a new Home Assistant card you have
[27.24 → 30.32] that tracks your quarantine amount percentage-wise.
[30.54 → 32.62] I know you were like 99.4% at home.
[33.34 → 35.10] It's Quarantine Meter.
[35.74 → 38.06] It was on the Home Assistant Reddit page.
[38.66 → 46.28] And yeah, it uses my Life360 integration to calculate how many hours I've been at home in the last seven days.
[46.82 → 52.76] And turns out I've only left the house for three hours in the last seven days, which, I mean, it's fine.
[52.84 → 56.62] I mean, I know as a community and as a society, we all need to be doing that.
[56.62 → 60.86] But when you see the data presented to you, you sort of think, what was I doing for three hours?
[61.22 → 65.86] Okay, I was grocery shopping for somebody that had just come down from New York, and they were self-isolating.
[66.10 → 69.46] So I was doing a good thing for the community, and at the time I was out walking my dog.
[70.22 → 74.70] But you think to yourself, well, actually, I could probably do seven straight days.
[75.04 → 78.16] And then here I am on day four, and I'm going slightly mad.
[79.18 → 80.12] I feel like I could do it.
[80.18 → 80.70] I love it.
[81.10 → 81.86] Something about it.
[81.86 → 86.66] It's just, for me, it's like I love being all in there and cozy and working on stuff.
[87.06 → 91.64] Also, it's given me a great chance to hang out in our new Discord, which has been amazing.
[92.38 → 92.64] Yeah.
[93.02 → 94.94] So we've launched a Discord server.
[95.10 → 100.44] We have unfortunately fallen into the traps of a non-self-hosted chat platform.
[100.60 → 101.66] I know that's what you're thinking.
[102.06 → 105.62] Within 20 minutes of launching it last week, we already had people giving us a hard time.
[105.68 → 106.80] So we've definitely gotten it.
[106.80 → 109.16] Should we just address why that elephant is in the room?
[109.24 → 112.80] Because even going back to episode one, I think this is something we flirted with, but
[112.80 → 114.42] this is the first time we've really...
[114.42 → 115.38] This and maybe Plex.
[115.82 → 121.46] It's like the whole GitHub versus GitLab self-hosted argument of, yes, each organization,
[122.00 → 125.22] each project, whatever, could host their own chat server.
[125.68 → 131.56] You know, a Mattermost, a Rocket Chat, an IRC server, whatever it is this week, a Matrix
[131.56 → 132.22] thing.
[132.22 → 136.76] But in reality, you have to go where the communities are.
[137.10 → 142.70] And if you look at the purpose behind why we've launched this Discord server, it's to give
[142.70 → 146.70] people a place to hang out and talk about everything relating to self-hosting.
[146.98 → 154.82] Not necessarily to be a self-hosted platform itself, but it's to enable the community to
[154.82 → 157.62] grow and, you know, build relationships and stuff like that.
[157.62 → 162.54] And whilst the Telegram group that we have is fantastic with, you know, 1,700 people
[162.54 → 168.48] in it and growing still, and Telegram isn't self-hosted either, by the way, conversations
[168.48 → 171.38] and threads get lost in that number of people sometimes.
[171.38 → 175.02] And I think it's going to be really great for people to have an area they can come and
[175.02 → 180.00] just talk about a specific topic without blasting it off to 1,700 people every time.
[180.00 → 181.00] Absolutely.
[181.34 → 184.88] We'll have a link in the show notes at self-hosted. Show slash 16.
[185.12 → 188.22] And I'll also try to remember to put a link at the top of the website for the Discord.
[188.54 → 191.60] I want to underscore something here because I want to make it clear.
[191.80 → 194.60] It's not a decision Alex and I came to lightly.
[194.74 → 199.06] It's something that he and I have literally been discussing since episode zero when we were
[199.06 → 200.74] just brainstorming.
[200.74 → 208.52] And while we almost always default to self-hosted, it is in a few exceptions where we don't.
[208.60 → 209.58] And there are other areas too.
[209.64 → 210.62] I'll just admit to it right now.
[210.72 → 214.04] I use Twitter and I use YouTube and I don't like it.
[214.10 → 216.86] I actually don't like it because I don't host them.
[217.68 → 220.74] But that is where the audience is.
[221.00 → 224.62] And I think for a lot of people, it's all a balance.
[225.22 → 229.30] Some stuff is really worth going onto the top of the hill and fighting to your death.
[229.30 → 233.20] And some stuff, it's just easier to go with the flow and just get collaborating.
[233.62 → 238.54] And I think that if this Discord server leads to more people collaborating and trying out
[238.54 → 242.94] more self-hosted software and technology and building out more self-hosted infrastructure,
[243.12 → 243.92] then it's a net win.
[244.52 → 246.22] Yeah, couldn't have said it better myself.
[247.04 → 252.44] Let's do some follow-up from last episode where we talked about Gross, the toilet paper
[252.44 → 254.48] stockpiling inventory management system.
[255.00 → 255.66] And batteries.
[255.94 → 256.58] And batteries.
[256.58 → 261.52] There is a really cool thing that you can get called Barcode Buddy.
[261.70 → 266.88] So one of the pieces of feedback I had was it's quite laborious to enter all of your stuff
[266.88 → 268.22] into the inventory system.
[268.50 → 271.80] Well, with Barcode Buddy, there's a link in the show notes.
[272.40 → 278.12] With Barcode Buddy, you can actually scan using an app on your phone, the barcodes of tins
[278.12 → 282.04] of beans and all that kind of stuff and actually add it to the database that way.
[282.10 → 284.00] So I thought that was pretty cool and worth sharing with you.
[284.00 → 285.70] That I actually would do.
[286.28 → 288.68] Not so big on the manual entry, but the old scan and go.
[289.18 → 290.14] I'm OK with that.
[290.60 → 292.72] I think that's a nice little addition.
[293.12 → 293.72] I love that.
[294.50 → 294.70] Right.
[294.84 → 297.18] Should we come on to the bad news of the day?
[297.68 → 298.44] OK, I'm ready.
[298.98 → 303.90] It was announced this week that Dark Sky have been bought by Apple.
[304.48 → 304.84] Yeah.
[305.20 → 306.08] Sad trombone.
[306.08 → 311.54] This is a bad one because it's super popular as a tool in the home assistant community.
[312.08 → 316.70] But I've discovered based on the now daily messages I'm getting from audience members
[316.70 → 320.02] that a lot of other projects are using it too for their back end information.
[320.58 → 320.70] Yeah.
[320.70 → 325.90] This is an example where a hosted project maybe wasn't the best solution.
[326.02 → 330.24] And I don't know what your answer is here for weather other than it did get me thinking,
[330.62 → 334.12] is it time for a weather station in the junkyard?
[334.66 → 341.46] You could easily do it with an ESP8266 board and, you know, maybe $15 worth of parts.
[342.02 → 342.24] Yeah.
[342.56 → 343.10] You think?
[343.48 → 343.72] Yeah.
[344.00 → 344.34] OK.
[344.74 → 345.28] All right.
[345.34 → 348.12] Sounds like we got a project for next time Alex visits Washington.
[348.12 → 351.52] I've been meaning to do this in my backyard since I moved here.
[351.58 → 352.28] So I will do it.
[352.36 → 352.92] I will do it.
[353.04 → 354.84] I'd legitimately be interested to see how it goes.
[355.18 → 355.90] Don't tempt me.
[358.34 → 359.40] This is a shame, though.
[359.52 → 364.22] Apple bought them and, you know, it's not unusual for when they make an acquisition like
[364.22 → 366.94] this for them to either shut down or just change the game completely.
[367.22 → 372.98] The good news is if you already have API credentials, it sounds like it's going to remain on until
[372.98 → 374.92] maybe some point in early 2021.
[375.76 → 377.72] Yeah, that is air quotes good news.
[377.72 → 380.02] New users cannot get API keys anymore.
[380.30 → 385.32] So even once Apple integrate this into whatever product they have in mind, presumably the weather
[385.32 → 389.74] app, right, they're going to be doing API calls under the hood anyway.
[390.56 → 391.82] Dark Sky is a paid service.
[391.92 → 398.26] I think I pay 79 pence or a dollar a year or something for Dark Sky access through my phone.
[398.70 → 401.32] It's such a small amount of money that I can't remember exactly how much it is.
[401.32 → 407.64] But, you know, the point is, is that Apple could maintain the existing product without
[407.64 → 413.54] necessarily really affecting, in my opinion, whatever integrations they're trying to do.
[413.62 → 415.38] And obviously I'm not, you know, Scott Federighi.
[415.46 → 417.80] I don't exactly know what plans they have for it.
[417.90 → 419.06] It's Craig Federighi.
[419.06 → 421.12] Oh, it was Scott Forestall, wasn't it?
[421.12 → 421.36] Yeah.
[421.36 → 424.16] You know, I follow you.
[424.64 → 427.94] I think they would brand it as like iCloud weather or something like that.
[427.96 → 428.94] And then nobody would want it.
[429.52 → 433.24] I think Apple looked at this, and they said, well, this isn't enough money to be worth
[433.24 → 433.72] our time.
[433.84 → 438.18] Let's just keep our competitive advantage, and we'll just internalize it.
[438.18 → 443.58] So not only is it probably not a moneymaker, even at a dollar, as you say, a year or a
[443.58 → 444.04] month, whatever.
[444.70 → 449.66] I think that combined with the competitive nature of them being the exclusive holder
[449.66 → 451.40] of this information is probably worth it.
[451.46 → 456.22] I mean, for me, the thing I loved about Dark Sky was that super hyper local rain information.
[456.22 → 459.78] As you can imagine here in the Pacific Northwest, I check that thing daily.
[460.28 → 461.80] Almost like it rains a lot where you are.
[462.36 → 463.54] Almost like that.
[464.02 → 468.04] One time I stood outside a pub in London with some colleagues and I got Dark Sky out.
[468.04 → 469.58] And we were having a pint stood outside.
[470.14 → 471.20] You know how it is in London.
[471.20 → 473.16] If you've been there, there's the little tape on the floor.
[473.24 → 474.24] You have to stand inside.
[474.70 → 477.26] And so we were stood just outside the tape, outside the canopy.
[477.70 → 480.08] And it started to absolutely throw it down.
[480.48 → 483.96] And I said to people, right, this rain is going to last for three more minutes.
[484.54 → 486.06] Three minutes later, it stopped.
[486.30 → 486.58] Bang.
[486.82 → 487.22] Dead on.
[487.66 → 487.76] Yep.
[488.18 → 488.70] Same thing.
[488.76 → 491.68] I was at a meetup, and we were eating outside, and we checked Dark Sky.
[491.76 → 492.72] Is it worth going inside?
[492.84 → 493.82] Because there was really no tables.
[494.24 → 494.96] What would we do?
[495.56 → 496.24] Looked at Dark Sky.
[496.36 → 496.52] Yep.
[496.54 → 497.40] It's worth going inside.
[497.40 → 498.60] It's going to be raining for an hour.
[499.02 → 499.86] It was really nice.
[500.56 → 503.86] While we're still on the Home Assistant topic, what are you going to do in Home Assistant
[503.86 → 505.04] to replace Dark Sky?
[505.22 → 506.56] Do you have an option right now?
[506.96 → 507.38] I don't know.
[507.48 → 510.96] I'm hoping to solicit feedback from the audience, quite honestly.
[511.36 → 513.10] Self-hosted. Show slash contact.
[513.36 → 517.36] While we're still in follow-up and on the topic of Home Assistant, the last episode, I think
[517.36 → 522.98] it was, you made a very, very strong pitch for me to switch to what I refer to as Has.io,
[522.98 → 524.26] which is just now Home Assistant.
[524.70 → 531.40] But it's the whole OS stack where you get the supervisor with official add-ons and third-party
[531.40 → 531.86] add-ons.
[531.98 → 536.00] And then it's very easy to add hacks, the Home Assistant community store, and get even more
[536.00 → 536.54] integrations.
[536.54 → 540.46] And you really kind of piqued my interest when we did a live stream.
[540.56 → 542.76] And I thought to myself, I got to do this at some point.
[543.20 → 548.36] It all went south, though, when my Raspberry Pi Raspbian install started kicking up a bunch
[548.36 → 554.02] of errors, package errors, about the Linux image package, which that sounds terrible.
[554.36 → 558.50] It also kicked up a bunch of errors about my time zone information.
[558.50 → 561.28] And I just don't think it's going to survive a reboot.
[561.42 → 563.16] So I thought, well, I've recognized the problem.
[563.28 → 564.30] Better do something about it.
[564.46 → 566.00] So I bought another Raspberry Pi 4.
[566.64 → 571.90] Only this time, I put Ubuntu 2004 LTS on that sucker.
[572.14 → 576.22] And it's running from an external SSD, not off the SD card.
[576.50 → 579.98] It screams, screams, Alex.
[580.04 → 582.10] I can't believe the performance I'm getting on this thing.
[582.40 → 583.18] Everything's faster.
[583.70 → 588.48] And then what I did is I grabbed Home Assistant's installation script, and I ran that on top of
[588.48 → 589.04] of 2004.
[589.28 → 591.68] It pulled down all the containers after I had Docker set up.
[592.14 → 596.30] And now I'm essentially running what I would have traditionally called HASS.io with custom
[596.30 → 596.80] themes.
[596.92 → 598.06] I got hacks installed.
[598.22 → 600.22] I got everything reset up.
[600.52 → 604.34] And really, it wasn't as bad as I was expecting.
[604.60 → 611.14] I drove home dreading this because my Home Assistant setup works so well, and it is actually responsible
[611.14 → 612.38] for quite a few things now.
[612.60 → 613.52] I was dreading it.
[613.58 → 615.50] You told me it wouldn't be so bad, and you were right.
[616.12 → 616.54] Thank you.
[616.54 → 619.30] Two tricks I'd like to impart upon the audience.
[619.74 → 623.22] The thing I was most concerned about was moving over my Z-Wave devices.
[624.00 → 629.92] I have some Zigbee and Z-Wave devices that I use for temperature, light, motion, security,
[630.48 → 635.40] base status, battery-based status, like all kinds of Z-Wave devices, and outdoor plugs.
[635.40 → 639.32] And I just didn't know, like, how do you move a Z-Wave network over?
[639.80 → 646.56] But I shut down the old Docker images of my old Home Assistant core install, exported out
[646.56 → 649.58] or went in on the file system, grabbed all the Z-Wave configs.
[649.58 → 665.32] I shut down the Home Assistant install on HASS.io, moved those Z-Wave configs over inside the container, and then plugged in the adapter, started it up, and all the devices just moved with the controller and all started reporting.
[665.42 → 670.00] They'd lost all their names, so I had to rename everything, which was a real chore figuring out what was what.
[670.26 → 671.24] Let me tell you.
[671.50 → 672.68] That can be a pain in the ass.
[672.68 → 674.46] Yeah, yeah, it was.
[674.56 → 679.26] So one of my tricks was I just cranked the heat in the room and then just waited to see which one registered.
[679.74 → 680.70] It was really hot.
[681.72 → 684.18] So that was, in the other room, I opened all the windows.
[684.54 → 685.42] It was a mess.
[685.56 → 691.42] And then the HomeKit devices were particularly hard because once they're paired with something, they can't be repaired with.
[691.78 → 694.90] And a lot of them just have a general reset to defaults.
[694.90 → 696.90] They don't have a way to unpair them by holding down keys.
[696.90 → 707.22] So I had to go around to the HomeKit smart plugs, reset them, rejoin them to my phone, then remove them from HomeKit, and then add them to Home Assistant one by one.
[707.80 → 708.98] So I got rid of those.
[709.14 → 712.12] Now, I will say, last thing.
[712.66 → 719.90] If you want a really easy smart plug that isn't something you have to flash, I still think the TP-Links were a good purchase because they were automatically all redetected,
[719.90 → 729.38] and the names I had given them were actually written to the device, so they all showed up with the names I had from the old Home Assistant install, autopopulated, clicked right in.
[729.84 → 734.08] The easiest part was the TP-Link, and they're the smaller ones that only take up one plug.
[734.98 → 738.48] I think if you're going to get a smart plug that isn't something you re-flash, that's still the one to get.
[738.60 → 740.04] It just works immediately with Home Assistant.
[740.14 → 741.96] It does require an app.
[742.46 → 744.82] You know what's even better than the TP-Link ones?
[745.32 → 748.24] This is a point where I talk about Taste again.
[748.86 → 749.42] No, you're right.
[749.42 → 757.68] When I rebuilt my Home Assistant instance, the DNS name that I used for my MQTT server meant that I didn't even have to reconfigure the plugs.
[757.84 → 760.12] It just picked up the MQTT server again.
[760.44 → 763.36] Ooh, that's even better.
[763.80 → 764.34] You're right.
[764.88 → 770.98] See, what I appreciated about the TP-Links is I could get them in two packs for like $35 from Amazon, and then they just plug in.
[771.04 → 772.64] You use the app once to configure them.
[772.70 → 775.04] You never have to use the app again after they're on your network, though.
[775.38 → 776.28] Yeah, it's not too bad.
[776.28 → 779.92] It's not too bad, but one day that app will probably go away.
[780.50 → 781.06] Yep, it will.
[782.14 → 783.34] I don't know when, but it will.
[783.86 → 784.00] Yeah.
[784.16 → 785.78] In the meantime, it's not so bad.
[786.48 → 789.02] Just how I'm on the fence like with those kinds of things.
[789.54 → 793.64] You know, I think there is a real value in doing a new can pave.
[793.88 → 798.16] When it's a new thing like Home Assistant, it's relatively new.
[798.16 → 803.18] You know, I think back to my early days with Windows, of Linux, of even macOS.
[803.18 → 811.58] The way I used to learn the most was when I was rebuilding those systems, rebuilding those automations, whatever it might be.
[812.08 → 812.70] It's like a trail.
[812.82 → 815.66] You're re-stamping down the grass and the weeds.
[815.82 → 817.16] You're making that trail.
[817.42 → 818.60] You're working it in.
[818.70 → 821.74] And it took me, what, a week or two the first time?
[821.76 → 823.06] And it took me an evening this time?
[823.06 → 830.40] And maybe it's not 100% done, but in other ways, I have more functionality now with the add-on store hacks.
[830.60 → 832.88] Now I have snapshots, themes.
[833.40 → 841.56] Additionally, this time around, I thought, well, why not set it up more with their Nebraska or whatever, the Home Assistant online services?
[841.92 → 845.32] And I decided, let's turn on the Echo integration.
[845.78 → 847.04] I'd never done that before.
[847.60 → 848.00] Cancel!
[848.60 → 849.90] It's pretty great.
[849.90 → 855.14] I can kick off automations and scripts via the Echo.
[855.32 → 856.60] Now that's money.
[856.68 → 861.44] If I say Echo, run bedtime, which we call last call, from anywhere.
[861.52 → 862.96] And then I can say Echo, good morning.
[863.28 → 865.38] And it just, you know, from anywhere, it's really nice.
[866.16 → 868.28] Via the Echo, I can set brightness levels.
[868.52 → 871.58] So I can just say Echo, set kitchen strip to 10%.
[871.58 → 874.38] Again, that speaks to the whole...
[874.38 → 874.92] Compromise.
[875.22 → 877.78] Yeah, it's a compromise that those things are not self-hosted.
[877.78 → 884.10] They are reliant upon Amazon and Google and Apple to some extent.
[884.78 → 887.58] And for me, an internet connection as well, which is not always guaranteed.
[888.10 → 891.16] But the way I look at it is that remote control is just the beginning.
[892.30 → 899.96] If you can turn something on and off remotely, that then opens the door to be able to link it in with all the other devices.
[899.96 → 903.76] And this is why, in my opinion, Home Assistant is doing such a great job.
[904.12 → 913.12] It allows a single entity, a single instance, where it's just got a record of everything that's in your house or in your RV or whatever.
[913.82 → 917.74] And it's all in one place, and it's all aware of what everything else is doing.
[918.26 → 920.42] And then you can kick off automations based on that.
[920.42 → 926.10] For example, in my garage, I have a light switch with a Shelly in it.
[926.58 → 931.30] The Shelly is a thing we talked about a few weeks ago that is a smart switch, kind of like add-on.
[931.66 → 934.68] It's the size of like an Oreo cookie and goes inside the light box.
[935.14 → 935.20] Right.
[935.32 → 937.46] Turns any regular switch into a smart switch.
[937.58 → 937.82] Correct.
[937.82 → 944.40] And then I have on a separate light circuit, a separate pair of lights in the back half of my garage.
[944.48 → 951.60] So I would normally have to walk over to the far side of the garage and flick a separate individual switch that's on a completely different circuit.
[952.16 → 960.64] But because these two lights are on the same Home Assistant instance, I can flick one switch and I have an automation that's always listening for a state change.
[960.80 → 966.12] And if either of those switches gets toggled, it knows to turn the other one off as well.
[966.12 → 972.70] And once you start thinking about how you can convert dumb switches into smart switches, oh boy.
[973.74 → 974.70] Very much so.
[974.98 → 984.74] And I also kind of look at the Echo stuff and even the Nebulas or whatever it's called, remote integration as layers on top of a core.
[985.24 → 988.20] And if that were to go away, no big deal.
[988.28 → 989.82] I have a tablet mounted to the wall.
[989.92 → 995.00] That's actually my main control for my Home Assistant is the tablet mounted to the wall, not the Echo.
[995.00 → 996.16] So what do you use?
[996.20 → 997.26] Is it the Fire?
[997.68 → 997.88] Yeah.
[997.98 → 1003.20] And I just, I know a lot of people will like ref lash it or set up in kiosk mode.
[1003.34 → 1004.52] I find none of that necessary.
[1004.90 → 1007.36] I just got one app to keep the screen on all the time.
[1007.64 → 1010.68] And then I just open the browser in full screen mode and just leave it up.
[1011.16 → 1012.00] And it works all the time.
[1012.38 → 1016.46] Did you see in the latest Home Assistant update, 107 is the latest version.
[1016.46 → 1019.22] There is a new dashboards feature.
[1019.64 → 1024.94] So you can actually have different home screens for different devices, not different pages.
[1025.34 → 1031.38] It's like a different kind of interface, all based off the same Home Assistant instance.
[1031.94 → 1040.10] That's definitely something I'm going to take advantage of because there's an interface that works well on that tablet, but that doesn't necessarily look good on my desktop browser.
[1040.46 → 1040.66] Yeah.
[1040.72 → 1043.26] Tablet, you want big fat buttons for your big fat fingers.
[1043.54 → 1044.64] That's exactly what I did.
[1044.64 → 1048.02] On a desktop, you want tiny little toggles because you have a mouse, right?
[1048.28 → 1049.14] I did exactly that.
[1049.22 → 1055.38] I did huge button with sliders and just to make it really easy for one spot for them to touch.
[1055.94 → 1062.62] And then I did like individual smaller toggles for myself and using like the new temperature cards and stuff like that, that all look very nice.
[1063.08 → 1067.06] So visually to the family, it looks like dad just did a big upgrade to the thing that they use.
[1068.28 → 1069.20] Good job, Chris.
[1069.38 → 1069.70] Well done.
[1070.12 → 1070.62] Nice effort.
[1071.16 → 1073.90] Little do they know, I was like, oh God, I don't know if I'm going to pull this off.
[1074.64 → 1076.46] But I'm glad I did it now.
[1076.58 → 1079.32] And I'll be playing around more with the stuff that's built into it.
[1079.68 → 1085.60] One of the things that works significantly better with this load is my Waze cams.
[1085.64 → 1091.10] I pull the RTSP feeds into picture elements or media elements into Home Assistant.
[1091.22 → 1095.26] I just have one security tab where I can get a real time feed of all of my Waze cams.
[1095.26 → 1099.14] It works much better with the new load.
[1099.70 → 1102.52] That is unless I take advantage of this new firmware they've released.
[1103.02 → 1103.22] Yes.
[1103.30 → 1111.12] With the new work from home movement that seems to be gripping the world by storm right now, Waze have enabled a webcam mode.
[1111.12 → 1118.30] This is a weird one, but it involves manually installing a firmware onto your Waze camera like you would to get RTSP support.
[1118.94 → 1123.54] And then after that, the Waze camera no longer communicates with the Waze app.
[1123.72 → 1134.52] It just stops talking to their cloud servers, but you can plug it in to your machine, and it'll power it over the USB port and act as a USB web camera for them Zoom calls you're making.
[1134.52 → 1136.60] You know, I have a top tip if you want a webcam.
[1137.32 → 1139.04] Probably don't use your Waze cam.
[1139.82 → 1144.44] Go to eBay and buy a Logitech C920 for $40 used.
[1145.06 → 1145.36] Yes.
[1145.52 → 1146.02] Great tip.
[1146.40 → 1150.90] The nice thing about that too, although probably the Waze as well, is it does H.264 encoding in the camera.
[1151.64 → 1156.04] So it takes less CPU load, which is always a good thing, and still a pretty good picture.
[1156.58 → 1162.56] I don't think this is something I would use, but I do appreciate the flexibility of these $25 cameras.
[1162.66 → 1163.66] That's kind of fun.
[1163.66 → 1164.92] Well, I'll tell you what's great.
[1165.00 → 1171.56] My wife is a music teacher, and she's had to convert all of her students and teach them through Skype or Zoom or FaceTime or whatever.
[1172.14 → 1174.88] And her iPad is getting a real workout at the moment.
[1175.20 → 1183.30] And if for any reason that went down and, you know, stopped working or whatever, and then, you know, one of the three laptops I have in the house stops working.
[1183.30 → 1186.38] And then one of the three other webcams I have in the house stopped working.
[1186.82 → 1190.48] Then, then I might use a Waze cam as a webcam.
[1190.48 → 1195.42] And you decide not to just do it from your phone for some reason, which probably has a better camera.
[1196.22 → 1196.80] Oh, yeah.
[1197.22 → 1197.52] Yeah.
[1197.84 → 1198.08] Yeah.
[1198.38 → 1203.48] There's a lot that would have to break in my house before I got to the Waze cam, but it's not the case for everybody.
[1203.48 → 1210.72] However, if you just want to buy one $25 camera, it will do it all, which is, I guess, nice.
[1211.12 → 1216.68] We have not dug a lot into home networking yet, but it's something Alex and I are talking a lot more about.
[1216.86 → 1219.66] So we thought we'd cover a little bit of home networking basics today.
[1219.66 → 1229.28] With this whole working from home business, there's been a lot of calls appeared in my calendar of people that normally work in an office that are missing that kind of social contact.
[1229.46 → 1232.42] Now, for those of you that don't know, I work from home 100% anyway.
[1232.58 → 1237.56] So for me, not a huge amount has changed on my day to day, besides obviously the world ending.
[1237.56 → 1249.80] And I think that listening to a lot of these people, you know, quote unquote armies talking about Wi-Fi and firewalls, and I've just referred to other Red Hatters as armies, didn't I?
[1249.94 → 1250.48] I know.
[1250.64 → 1251.92] I just love where this is going.
[1252.40 → 1260.82] Now, to bail you out a little bit, 100% of my meetings this week have people working from home dealing with Wi-Fi trouble.
[1260.82 → 1268.12] And then people like going from the nice room that they've set up where they've cleaned up behind them to like progressively having to just move closer and closer to the router.
[1268.22 → 1270.72] And pretty soon they're like just in their closet so they can make the call work.
[1271.14 → 1277.38] Let's preface everything I'm about to say about Wi-Fi with the caveat that a wire is always better.
[1277.94 → 1280.88] It's significantly better for real time video calls as well.
[1281.34 → 1286.74] The machine I'm doing this call with you wired in right now, I would never do this without it being wired in.
[1286.74 → 1295.40] And so you have this initial spot with a lot of people's home networks where the Wi-Fi network, just by its very nature, because it's radio, isn't as solid.
[1295.92 → 1302.04] And so that right there introduces problems regardless of the rest of the network infrastructure on your LAN or your internet connection.
[1302.60 → 1302.82] Yes.
[1303.04 → 1313.18] And another thing that a lot of people don't think about is the ISP provided routers often have Wi-Fi hotspots built into them.
[1313.18 → 1320.06] You know, your ISP will rent you a router or sell you a router or maybe just give you one for the duration of your contract.
[1320.90 → 1324.30] And quite often they are what's called a combination device.
[1324.80 → 1327.56] They do all the routing into and out of your network.
[1327.76 → 1334.20] So every web page that you visit, your traffic goes through that firewall outbound.
[1334.20 → 1342.46] And then when you request that web page to come back, it comes inbound through your firewall that way and then out through the Wi-Fi that's also in the same device.
[1342.46 → 1363.14] So sometimes, particularly when you have a house full of, I don't know, half a dozen children and, you know, a dog and everybody that wants to stream Netflix all at the same time, you can end up quite quickly in a situation where the routing tables in these devices, they're very, very cheaply made Chinese-type routing devices.
[1363.14 → 1366.44] And they don't have a lot of memory in them, a lot of these cheap ones.
[1367.34 → 1372.96] And very quickly you can exhaust the tables that they have available that will fit in their memory.
[1373.26 → 1375.94] And that can manifest itself in a number of different ways.
[1376.72 → 1381.42] Poor performance, slow latency, pages just not loading for no reason.
[1381.82 → 1382.12] Crash.
[1382.36 → 1383.00] Yeah, crashes.
[1383.00 → 1399.78] One of the things that I did probably four or five years ago that's helped my Wi-Fi experience the most, more than anything else, was to separate my ISP modem or my router from the Wi-Fi hotspots that I use for everything else.
[1400.30 → 1407.30] Now, I will also say that putting everything I possibly can on an Ethernet cable helps a lot as well.
[1407.30 → 1414.24] You know, like my NVIDIA Shield is on Ethernet, my PlayStation 4, my 3D printer is on an Ethernet cable, all of my desktops.
[1414.94 → 1418.10] My laptop is on Wi-Fi 90% of the time.
[1418.52 → 1423.22] But at my desk where I spend most of my day, there is an Ethernet cable there ready for it.
[1423.38 → 1426.28] So if I can avoid Wi-Fi, I will.
[1426.88 → 1431.66] But sometimes you just can't, you know, with a phone or a tablet, for example.
[1431.66 → 1439.48] Or in my situation where we have Ethernet everywhere in the studio, I go to the RV, I can't run Ethernet at all.
[1440.36 → 1442.08] It's just literally not an option.
[1442.24 → 1444.28] And so I have to have extremely robust Wi-Fi.
[1444.72 → 1449.40] And so by separating out the firewall from the Wi-Fi, that gives you a few benefits.
[1450.00 → 1456.12] Firstly, if you have to reboot the router, all the devices in your house will maintain their Wi-Fi connection.
[1456.12 → 1462.40] Chromecast's won't decide that they need to now turn into a hotspot and take a few minutes to figure out that the Wi-Fi is available again.
[1463.38 → 1465.84] But the same is true conversely as well.
[1465.92 → 1469.88] If there's a problem with your Wi-Fi, you can reboot just the access point.
[1470.46 → 1474.54] And then your internet connection will stay completely stable and solid.
[1474.92 → 1477.08] So there are a few benefits to doing it.
[1477.16 → 1483.34] And the company that I've used for the longest time now is Ubiquity, who make the Unify line of devices.
[1483.34 → 1487.72] I think probably most people listening at this point must be familiar with Ubiquity.
[1488.06 → 1490.74] They are extremely popular in our segment.
[1491.18 → 1497.16] And I think the number one thing I've heard is they have really sophisticated management.
[1497.66 → 1502.56] And generally, there's just the one downside brought up, and that is the controller software.
[1503.20 → 1505.80] But even that doesn't necessarily sound like it's the end of the world.
[1505.90 → 1509.16] You just have to be willing to host an application, and it has to be able to talk to the internet.
[1509.16 → 1517.96] I was talking to somebody on the Jupyter Broadcasting Telegram just this afternoon about hosting the Unify controller out of a Docker container.
[1518.44 → 1523.82] Linux server, obviously make one, and I've used that for years, and it just works.
[1524.62 → 1525.96] Now, I have two.
[1526.14 → 1529.44] I've just recently added actually a third access point in my house.
[1529.44 → 1538.68] And all of these devices talk back to a Unify controller that's running on a DigitalOcean droplet, so it's not even running in my house.
[1539.02 → 1548.04] I wrote a blog post last week, which there'll be a link to in the show notes, about how to adopt an access point, a new access point, with a remote controller.
[1548.94 → 1554.04] Now, for most people, they're going to be running their Unify controller on a Raspberry Pi inside the firewall or...
[1554.76 → 1555.22] In a container.
[1555.22 → 1556.56] Yeah, something like that.
[1556.72 → 1557.88] And it's not going to be an issue.
[1558.02 → 1561.16] It's just going to appear, you know, through magic in the controller.
[1561.46 → 1564.24] You can adopt it and then configure it that way.
[1564.74 → 1567.30] It gives you a lot of flexibility in some ways.
[1567.58 → 1573.60] It did feel, I will admit, the very first time that I did it, like a bit of a like, why do I need...
[1573.60 → 1578.46] Why can't I just go to the IP address of the access point and do it that way?
[1578.50 → 1579.86] That's the way I've always done it before.
[1579.86 → 1594.62] But the advantage of having a centralized configuration system is that if for any reason I need to reload, I can back up all my configurations to that central system, wipe the access point, and then just reload the configuration from there.
[1594.62 → 1604.82] And what it's meant is that I've had now a stable Wi-Fi configuration and network that's transcended four, five different houses, multiple different ISPs.
[1605.62 → 1621.62] And that's another point I didn't actually bring up, is if you separate your Wi-Fi from the ISP provided router, every time you change ISPs, if you move house or whatever, you don't have to reconfigure all your Wi-Fi devices.
[1621.62 → 1624.02] You've still got the same SSID, the same password.
[1624.48 → 1625.50] So I got a couple of questions for you.
[1625.62 → 1628.52] Are they aware of each other, essentially?
[1628.70 → 1632.58] Do they balance their signal because they're aware of each other's location?
[1632.70 → 1634.46] Is that also a benefit of the centralized controller?
[1634.62 → 1637.28] I had presumed it was when I had seen enterprise deployments.
[1637.34 → 1638.88] Is that true in home deployments as well?
[1639.24 → 1640.64] Or is it not really applicable for you?
[1641.02 → 1644.00] I don't know if that's because of the centralized controller.
[1644.00 → 1651.42] But the Unify gear itself does have this zero handoff feature, which allows me to roam between different access points in the building.
[1652.24 → 1657.82] And I just don't know slash care which particular access point I'm connected to right now.
[1658.64 → 1660.32] So have you tested the performance of it?
[1660.60 → 1660.84] Yes.
[1661.08 → 1661.90] Yes, a lot.
[1662.72 → 1662.94] Yeah?
[1662.94 → 1669.94] I used that Airspeed app running on the server in my basement to test the throughput of the Wi-Fi.
[1670.34 → 1676.22] And I actually identified that one of the Ethernet ports on my Unify was slightly dodgy through that.
[1676.36 → 1680.76] And I used a bit of hot glue to really jam the cable in there and keep it there.
[1681.12 → 1688.26] And so I went from sort of around about 100 megabits on that one up to pretty much full gigabit speed, not through Wi-Fi.
[1688.26 → 1688.74] Right.
[1689.10 → 1695.24] But the connection to the – the reason I asked, and I think this is really important to underscore, is I've been to buddy's houses.
[1696.16 → 1702.88] You know, I've been to like a shop, and I've had one set up here in the studio that are all Unify Wi-Fi networks.
[1703.58 → 1715.64] And in those three anecdotal experiences in which I have gone to, I was – I had some of the worst Wi-Fi experiences, like devices not connecting, horrible performance.
[1715.64 → 1722.36] And I think what it just sort of underscores is if the rest of your network isn't really up to shape, it doesn't matter what access points you put in.
[1722.68 → 1728.68] So like for these guys, like their DHCP server was running on a piece of crap that was so slow that it would time out before, you know, you can get an IP.
[1728.84 → 1730.06] So that was the issue on one of them.
[1730.50 → 1735.54] There are other aspects to a network that make it – it's not just the access points.
[1735.66 → 1741.26] But I do think that it is more important than ever that Wi-Fi be as close to wire grade as possible.
[1741.26 → 1745.94] Now, I don't care whether you use Ubiquity, Microtech, whoever.
[1746.20 → 1748.44] It really doesn't bother me whatsoever.
[1749.08 → 1752.84] The point is that you separate the Wi-Fi from the firewall.
[1753.30 → 1757.04] And that will in itself just enable easier troubleshooting.
[1757.58 → 1763.06] It will also mean, like I just said, that you can transcend different houses with the same Wi-Fi gear.
[1763.62 → 1763.72] Right.
[1763.80 → 1766.60] And the nice thing about the Ubiquity gear is that's easy for you to do.
[1766.60 → 1775.66] And it's not so easy with a lot of the mesh solutions that are out there now, like the Google one and the D-Link one and the Hero one, which I've had good success with.
[1776.14 → 1777.54] But it wants to be a router.
[1777.66 → 1781.90] Now, in the Hero solution, you don't have to use it as your main firewall slash router.
[1782.26 → 1783.54] But in some of these, you do.
[1783.96 → 1788.56] And I very much, like Alex, am a big proponent of separating those two tasks.
[1788.56 → 1795.70] I actually reboot my firewall on a somewhat regular basis because I'm often switching between multiple networks.
[1796.06 → 1798.32] And I just want to clear things out sometimes.
[1798.40 → 1801.68] And it takes like 15 seconds to reboot this little slate that I have.
[1802.40 → 1804.62] And so I just, you know, I just toss off a reboot.
[1805.10 → 1808.94] And I know that my, all my, what, you like tossing off a reboot?
[1809.08 → 1809.58] You like that?
[1809.88 → 1811.50] I toss off a reboot from here to there.
[1811.96 → 1812.14] You know?
[1812.64 → 1814.62] Tossing off in England is slang for a...
[1815.40 → 1816.70] I know what it's slang for.
[1816.82 → 1817.32] Oh, okay.
[1817.32 → 1819.56] I just wasn't going to call it out.
[1819.88 → 1821.02] So I toss off a reboot.
[1821.28 → 1822.66] And I just wait a few seconds.
[1822.66 → 1823.76] And the device is reconnected.
[1823.80 → 1824.44] And everything's good.
[1825.06 → 1825.34] You know?
[1825.64 → 1827.30] That's my pro tip.
[1827.58 → 1829.34] Who doesn't enjoy a good toss-off, huh?
[1829.72 → 1830.00] No.
[1830.20 → 1831.14] Especially when it's a reboot.
[1831.32 → 1832.10] It just feels good.
[1832.96 → 1837.38] So there's definitely some solid, solid rationale for separating those two devices.
[1837.38 → 1841.16] So if you are looking at some of those mesh networks that do offer some nice advantages,
[1842.00 → 1843.20] just be wary of that.
[1843.48 → 1844.66] Separate those functions if you can.
[1844.66 → 1848.84] And there's a huge amount of stuff that if you want to hear about, let us know through
[1848.84 → 1853.50] self-hosted. Show slash contact or find me on Twitter at Ironic Badger.
[1854.28 → 1856.74] And let us know if you want to hear more about the Unify.
[1857.10 → 1859.46] You know, there are a bunch of features in there which we could cover.
[1859.46 → 1863.20] Yeah, I would like to get that feedback because we are definitely not done talking about this.
[1863.28 → 1865.80] We want to talk about switches and firewalls soon.
[1865.94 → 1868.24] So it's your chance to get your feedback in the Discord.
[1868.48 → 1870.62] That'd be a great spot to just engage with us on this.
[1870.82 → 1874.74] And it's a spot not only are we watching really closely, but where we could kind of have an
[1874.74 → 1876.30] ongoing conversation about it.
[1876.54 → 1877.48] So be sure to join us there.
[1877.48 → 1882.40] I need to upsell you on pfSense or Open Sense or one of these others.
[1882.72 → 1884.90] You think you could run on a Pine64 board?
[1885.50 → 1886.40] You're a madman.
[1886.78 → 1887.00] I know.
[1887.08 → 1888.56] I just ordered one.
[1888.76 → 1891.28] And I'm trying to think of, you know, that thing's got a PCI slot, Alex.
[1891.50 → 1891.86] Ooh.
[1892.16 → 1893.04] Yeah, I know.
[1893.20 → 1894.96] And I know if I'm thinking about it, thinking about it.
[1894.98 → 1899.60] But let's wrap up today by spending a little time talking about a really cool app you can
[1899.60 → 1901.58] load on your rig to get perfect information.
[1901.58 → 1904.60] In fact, you can even use it to monitor multiple.
[1905.14 → 1905.80] It's called Net Data.
[1905.96 → 1908.00] And it's a Was Payne special.
[1908.12 → 1910.32] He loads it on all of our systems here at the studio.
[1910.88 → 1915.08] If you've never tried it, NetData.cloud, it's kind of amazing.
[1915.42 → 1919.80] So it provides real-time metrics of pretty much everything that's going on in your system.
[1920.22 → 1922.54] And it's really quite beautiful.
[1922.68 → 1923.70] It just runs in the background.
[1923.86 → 1924.76] You won't even know it's there.
[1924.82 → 1926.10] It uses very little resources.
[1926.82 → 1931.12] But if you want to know, for example, which of your hard disks is being completely trashed
[1931.12 → 1935.82] right now and causing your machine to stutter, load up this Net Data thing.
[1936.14 → 1939.10] Go and look at the disk IO section, and you'll figure out, oh, it's this one over here.
[1939.16 → 1943.52] Maybe I need to move this workload over here or do something else with it.
[1943.84 → 1945.64] You can also monitor network traffic.
[1945.76 → 1947.06] It's a perfect way to test.
[1947.58 → 1951.38] You know, you'll see quite often in Linus Tech Tip videos, they're monitoring network
[1951.38 → 1954.94] speed through an Unpaid server, and they're using Net Data to do it.
[1954.94 → 1960.20] So there are a lot of different use cases for this software, and it comes highly recommended.
[1960.20 → 1965.66] Like you said, it is also very pretty, at which I appreciate the way it visualizes everything.
[1965.96 → 1968.16] We keep it running here on the systems like I was talking about.
[1968.26 → 1972.18] And it's just a nice way to just check in on the health of them to get an idea of what
[1972.18 → 1973.14] the workload is.
[1973.20 → 1977.06] And you will spot weird problems watching these graphs.
[1977.20 → 1980.50] You will notice something's taken a long time to wait on X.
[1980.58 → 1982.28] Maybe it's like Alex was saying, a disk.
[1982.34 → 1985.22] Or I found what seemed to be a wonky nick.
[1985.86 → 1987.02] And how about that?
[1987.04 → 1987.62] A wonky nick.
[1987.62 → 1991.98] And we replaced it, and it immediately looked better.
[1992.22 → 1995.10] It just was one of those things you could immediately visualize the improvement.
[1995.52 → 1996.26] And that's kind of cool too.
[1996.32 → 2000.14] Plus, it stores all that stuff, and then you can add your other rigs in there and switch
[2000.14 → 2000.78] between them.
[2001.22 → 2002.72] I don't think it stores them on their servers.
[2002.82 → 2003.38] It's all local.
[2003.50 → 2006.06] So they all have to be able to have access to the internet if you want to be able to jump
[2006.06 → 2006.32] around.
[2006.68 → 2007.38] It's all local.
[2007.74 → 2007.88] Yeah.
[2008.18 → 2009.66] Do you want to know the icing on the cake though?
[2009.88 → 2010.44] What is that?
[2010.74 → 2012.84] I discovered a Home Assistant integration for it.
[2013.18 → 2013.82] Stop it.
[2014.22 → 2014.72] Link it up.
[2014.78 → 2015.54] I got to see that.
[2015.54 → 2016.44] It's in the show notes.
[2016.78 → 2021.04] No, no, no, no way.
[2021.38 → 2026.98] So you could run net data on all of your pies and then have it show up various stats in Home
[2026.98 → 2028.68] Assistant about each of those pies.
[2029.16 → 2030.28] I do run it on my pies.
[2030.88 → 2032.48] So I will be doing this.
[2032.58 → 2033.20] That's great.
[2033.20 → 2036.88] Home Assistant is so awesome.
[2037.38 → 2043.22] This is ultimately why I had to go to the more HASS.io style setup because I realized
[2043.22 → 2047.14] there's such a great community around it, and it's just getting better.
[2047.56 → 2050.08] And so you got to have access to all these cool things people are doing.
[2050.18 → 2051.30] And that's just the best way to get it.
[2051.66 → 2051.98] Absolutely.
[2051.98 → 2057.96] Now, I was on Reddit this week and I saw a post about somebody saying, everything's
[2057.96 → 2058.44] gone.
[2059.30 → 2060.56] All of my stuff is gone.
[2060.98 → 2065.40] And they'd accidentally exposed one of their services to the internet and some bad actor
[2065.40 → 2067.08] had come along and deleted all their media.
[2067.62 → 2068.46] Oh, it's so sad.
[2068.66 → 2072.30] Now we have an Ask SSH question from SEB Couture.
[2072.94 → 2074.14] Did I get that right, do you reckon?
[2074.30 → 2075.24] Let's say yes.
[2075.58 → 2076.62] I don't know why I'm asking you.
[2076.66 → 2078.32] You're horrible at pronouncing stuff.
[2078.64 → 2078.84] Yeah.
[2078.84 → 2081.32] I would have said SEB Couture or something.
[2081.72 → 2086.24] And SEB writes in on Twitter, would you open your Home Assistant behind a reverse proxy?
[2086.64 → 2087.42] Is it safe?
[2088.18 → 2088.70] What do you think?
[2089.24 → 2091.72] Well, my previous answer was no.
[2092.40 → 2097.88] And then this time I signed up for the Home Assistant cloud, which is not quite what he's
[2097.88 → 2100.02] talking about, but it is a form of remote access.
[2100.46 → 2105.78] That's security through obscurity though, almost with the URLs, a really long string of random
[2105.78 → 2106.42] characters.
[2107.10 → 2107.90] Yes, it is.
[2107.90 → 2111.70] And then you have to have authentication and there are those elements to it.
[2112.10 → 2113.82] And I opted to do it this time.
[2114.26 → 2117.26] In the past, I required like a WireGuard connection to get to it.
[2117.60 → 2119.84] And I think you've kind of opted to do the same, haven't you?
[2119.84 → 2121.60] You've set up a reverse proxy for yours.
[2121.70 → 2124.76] So you have kind of making, you've made that same sort of call.
[2124.98 → 2125.82] Again, it's a compromise.
[2126.28 → 2132.78] I run a few apps on my reverse proxy, which are public and internet facing, but they all
[2132.78 → 2136.76] have at minimum some kind of authentication.
[2136.76 → 2142.66] The mistake the guy made on Reddit was that he had no password for anything set.
[2142.74 → 2149.02] So if you just guess the URL or the port number correctly, you could log in and delete whatever
[2149.02 → 2150.26] you wanted with no password.
[2150.26 → 2156.10] I don't think I would expose any of my media server or media collection applications to
[2156.10 → 2156.46] the web.
[2157.28 → 2162.20] I would only expose applications that are explicitly designed to have public facing features.
[2162.64 → 2166.18] And I know that just because some of these apps are web apps, it seems like they're designed
[2166.18 → 2167.36] for that, but they're not.
[2167.72 → 2170.90] Then they should only be used on your LAN, I think, or with a VPN.
[2170.90 → 2171.34] Right.
[2171.96 → 2173.20] And that was going to be my point.
[2173.46 → 2178.96] You know, with WireGuard making it into the Linux kernel now, which is amazing.
[2179.46 → 2179.82] Incredible.
[2180.46 → 2183.16] There's no real excuse these days.
[2183.50 → 2189.62] And perhaps when we talk about firewalls in an episode or two, we'll talk about why I switched
[2189.62 → 2192.30] to Open Sense and what that has to do with WireGuard.
[2192.30 → 2200.58] But I think, you know, once you're on the VPN, it's, you know, so easy to pretend with DNS
[2200.58 → 2204.16] or whatever that you're on your LAN anyway that, I mean, maybe five years ago it was different.
[2204.48 → 2207.06] But nowadays with WireGuard, it's so easy.
[2207.48 → 2211.54] I don't really see any excuse to open much to the internet anymore.
[2212.02 → 2214.24] I look forward to talking more about networking.
[2214.84 → 2217.82] That's been Self-Hosted 16, and we'll see you on Discord.
