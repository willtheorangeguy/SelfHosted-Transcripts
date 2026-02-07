[0.00 → 2.92] Well, for episode 119, we're gathered together in a kitchen.
[3.74 → 4.58] Yes, sir, we are.
[4.74 → 5.96] And we have a special guest.
[6.02 → 7.88] Mr. Was Payne is on the show with us this week.
[7.94 → 9.06] Hey, thanks for having me back.
[9.18 → 10.54] We bumped into We sat Nixon.
[10.90 → 11.12] Yeah.
[11.26 → 11.72] Just now.
[11.88 → 12.64] Well, of course.
[12.80 → 14.16] Hey, stranger, we said.
[14.84 → 19.66] You want to come talk about home labs and self-hosting and Nix and stuff?
[20.10 → 20.84] You know I do.
[21.18 → 22.88] Yeah, so we're really glad to have you here.
[23.16 → 24.00] It's been way too long.
[24.76 → 25.96] You have been on the show, right?
[26.04 → 26.50] I have.
[26.52 → 27.72] Yeah, it has been a minute, though.
[27.72 → 30.70] When was the last time we did an episode in person?
[31.80 → 33.04] I think Raleigh, maybe.
[33.30 → 34.58] It's going to be a while ago.
[34.70 → 34.90] Yeah.
[35.32 → 39.80] This is going to be a weird one, just because we've never done a podcast in a kitchen, ever.
[40.38 → 42.30] Never recorded a JB show in a kitchen before.
[42.32 → 42.70] Here we are.
[42.88 → 43.86] Like a bunch of influencers.
[44.10 → 49.84] Yeah, but, you know, we asked the AI, we said, where's the best place to get an Airbnb in Pasadena, California?
[49.96 → 51.10] And this is where it told us to go.
[51.68 → 54.32] You know, AI is the hot S of the moment, right?
[54.32 → 54.52] Yeah.
[54.52 → 54.80] Yeah.
[54.80 → 60.22] And I've got a new NVIDIA GPU that I'm messing around with, doing some AI stuff, you know.
[60.48 → 62.58] So we thought we'd dig into that a little bit today.
[62.80 → 64.40] And I've been using some Nix to do it.
[64.82 → 65.42] Heck yeah.
[66.20 → 70.22] Whilst we're at Nixon, it felt like the perfect opportunity to trot that out in the show.
[70.34 → 71.04] So here we are.
[71.36 → 72.20] Here we are indeed.
[72.74 → 77.24] And I think, Alex, you were telling us before the show started, we said, wait, wait, stop, stop.
[77.68 → 79.98] That you had found somebody who's made a really brilliant video.
[80.26 → 82.20] They've made one video, and it's this one video.
[82.20 → 82.64] Yeah.
[82.78 → 88.58] If I could only ever make one YouTube video for the rest of my life, and it'd be half as good as this one.
[88.90 → 99.80] There's a video from a chap called Peter Hidden, and he has done a 33-minute-long expose on training AI to play Pokémon with reinforcement learning.
[99.80 → 102.76] It's an absolutely outstanding video.
[103.36 → 111.48] And it's one of those things that makes you really realize that actually, oh yeah, all of these buzzwords around AI models and training and data sets and all that.
[111.82 → 118.40] It's actually just clever people behind the scenes writing some code for a computer to go, hot dog, not hot dog.
[118.40 → 118.84] Yeah.
[120.04 → 125.76] Well, I think our angle, of course, on the show is going to be what you can do with this stuff that you can self-host.
[126.16 → 126.48] Yes.
[126.80 → 128.04] Maybe you can use privately.
[128.94 → 134.18] I like to try to find the ones I can ask spicy questions, you know, medical advice, things like that.
[134.22 → 135.22] You don't really get myself in trouble.
[135.38 → 136.42] Just how to write C++.
[136.42 → 138.34] Actually, you joke.
[138.96 → 147.84] I've had some success with writing Home Assistant automations, kind of using it to generate the YAML for a basic template that will provide notifications.
[148.36 → 150.20] And then I just go and swap in all the details.
[150.48 → 154.80] I like the idea that people got so sick of YAML that we've had to create AI to help us with it.
[155.52 → 158.02] You could probably find something better, but that's what I've used it for.
[158.02 → 160.34] I mean, there are all sorts of amazing possibilities.
[160.62 → 164.90] If you're doing this stuff locally, like I came across this tool yesterday called TLM.
[164.90 → 169.04] And this essentially lets you talk to your terminal.
[169.38 → 178.92] So if you want to know, for example, which network interfaces are on your box and what, you know, we all know how to do IP space A or if config or whatever it is.
[179.06 → 179.18] Yeah.
[179.26 → 182.60] But then we have to, as humans, go through and find the IP address or the MAC address.
[183.10 → 189.48] Wouldn't it be nice if you could actually talk to a computer like it was a person and say, show me all your IP addresses?
[190.08 → 191.52] Like in plain English.
[192.00 → 194.18] Have it format the output the way you like?
[194.48 → 194.80] Hmm.
[194.90 → 195.02] Hmm.
[195.44 → 199.92] So the thing I really like about TLM, I'm actually just playing with it on my laptop as we record right now.
[200.36 → 202.90] It doesn't actually execute any commands for you.
[203.28 → 207.00] I asked it, list all network interfaces, but only show their IP addresses.
[207.36 → 215.68] And then it showed me the if config command with a pipe to grew along with all the regex and all the rest of it required to cut everything else out.
[215.68 → 218.92] And then it printed out a list 192.168.whatever.
[219.06 → 220.86] And then my tailscale100 IP address.
[221.10 → 221.46] That's it.
[221.82 → 225.14] That's like the LLM version of let me Google that for you.
[225.24 → 226.38] And here's the result, by the way.
[226.64 → 226.84] Yeah.
[226.84 → 232.22] I really like how TLM does it because it says, right, I'm thinking about what it is you actually asked for.
[232.46 → 234.52] Here's the command that I think you're after.
[234.96 → 235.94] Shall I execute it?
[235.94 → 239.86] And then you have the final say about whether it actually runs that command on your system or not.
[239.86 → 240.14] Yeah.
[241.34 → 247.28] You know, this is how you get to Star Trek, you know, because they don't tell the computer in Star Trek the commands.
[247.54 → 248.84] They just tell it what it wants.
[249.30 → 254.32] I don't know that I maybe expected that Star Trek version would have, you know, rich and complicated interfaces.
[254.48 → 256.66] But we've kind of taken the other, we've done it the other way, right?
[256.66 → 261.82] We just built sophisticated enough reasoning agents that it can make sense of the soup we've created with computers.
[262.20 → 265.00] What happens if I type in TLGreyHot?
[266.58 → 267.42] Yeah, you know.
[267.60 → 269.84] Brute install cask TLGreyHot.
[269.86 → 271.18] That's what it wants to do.
[272.62 → 273.84] I don't think that's quite right.
[274.40 → 283.08] I feel like it's also kind of ironic that there's all this kind of intelligence and revolutionary new way of approaching getting information.
[283.28 → 285.00] And it's all behind chatbots.
[285.18 → 288.02] It's just I find it to be sort of, I don't know.
[288.28 → 294.72] It almost sort of betrays the usefulness of it because a chatbot seems like such a basic interface at first.
[295.36 → 300.66] But then when you start using these tools, you can, you know, for me, I use it to like get started.
[301.32 → 302.48] Oh, I need to go live.
[302.60 → 304.66] And I've got 30 seconds.
[304.72 → 308.14] I need to come up with an idea for why we're live or what the pitch should be.
[308.14 → 310.30] And I go in there and I say, this is what we're doing.
[310.40 → 310.80] Here's a thing.
[310.86 → 312.62] Give me a, you know, a two sentence description.
[312.62 → 319.78] And it doesn't ever produce anything that I actually use, but it always gets me started on, you know, maybe I'm writing something or whatever it could be.
[319.84 → 320.78] Just even that kind of stuff.
[320.86 → 326.02] It's so powerful in just a help a person achieve a little bit more.
[326.18 → 329.02] It's not replacing what I do, but it just helps me achieve more.
[329.02 → 330.68] Nobody could ever replace you, darling.
[332.36 → 337.76] It's kind of, those are almost the same thing, you know, it's just extracting what's common between things, the emulating.
[338.08 → 343.92] And then, yeah, you're left with a bunch of hooks to go customize, whether that's a Home Assistant config or an actual human paragraph.
[344.36 → 344.52] Yeah.
[344.54 → 345.94] You know, this stuff's coming to Home Assistant.
[346.48 → 347.24] Wouldn't that be great?
[347.34 → 347.96] You know, it is.
[348.04 → 348.10] Right.
[348.10 → 351.00] You just chat to Home Assistant and say, turn off all the lights that are currently on.
[351.16 → 351.40] Yeah.
[351.76 → 353.50] You don't need to be any more specific than that.
[353.50 → 354.22] And it just does it.
[354.40 → 354.58] Yeah.
[354.68 → 360.48] Or even something like tomorrow, turn the furnace on two hours earlier or something.
[360.56 → 363.88] Just something really basic that is actually an automation on the back end.
[363.88 → 369.30] I've struggled for a long time with such a basic automation of, like, I want to play my drums, right?
[369.34 → 372.52] And I don't want to cool down the entire house for the rest of the day.
[372.64 → 376.94] But for the next hour or so, just blow the cold air at me.
[377.10 → 380.42] That's, you know, run the cool, run the cold air for one hour.
[380.92 → 381.70] That's all I want.
[381.90 → 382.48] Sounds simple.
[382.48 → 392.02] It's not because you have to record the current state of the system and then actually go back to it afterwards and make sure that other zones in the house aren't on heat.
[392.24 → 393.68] So they're not fighting each other.
[393.82 → 394.12] Right.
[394.26 → 397.10] Because my house has three zones, and it's like, it's a bit of a pain.
[397.30 → 398.16] Yeah, it's a lot of chaos.
[398.28 → 399.08] That can be a lot of chaos.
[399.66 → 406.04] You could see where just making that stuff would be more approachable, too, to, like, the family members who aren't necessarily the ones that set it all up.
[406.04 → 410.88] But they could go to it and say, okay, I want the lights to turn on two hours before sunset.
[411.12 → 412.90] And it just creates the automation that does that.
[413.44 → 413.54] Yeah.
[414.14 → 416.72] So I was experimenting with the back end for this.
[416.72 → 426.14] And, you know, if you've been following any of this generative AI stuff or certainly in the self-hosting sphere, you probably will have heard of Llama as a project.
[426.14 → 429.10] And this thing loves graphics cards.
[429.20 → 432.86] Obviously, anything to do with AI, you know, GPUs is the way to go.
[432.92 → 436.38] I actually tried to run this on just a CPU just to see what would happen.
[436.60 → 445.66] And it was kind of like talking to a very slow, it was just one word at, it was just, it was super painful.
[445.90 → 450.20] And then I turned the GPU on, it was like ChatGPT plus speeds.
[450.26 → 451.26] It was actually kind of amazing.
[451.26 → 456.08] Yeah, it's like, it's like old BBS dial-up compared to high-speed internet.
[456.52 → 463.66] So using that fancy new Epic server that I talked about in the last episode, I passed through the NVIDIA GPU to a Nix OS VM.
[464.00 → 464.18] Ooh.
[464.42 → 470.52] And I've got a Nix config, which I'm just going to put a link to you both for in the show notes, pace.ktz.cloud.
[470.52 → 482.30] And just, this is, this is why I love Nix, because anybody listening to this show now that has an NVIDIA GPU could install this Nix config and run Llama.
[482.78 → 484.18] Yeah, it just works for them now.
[484.28 → 489.72] With a fully accelerated NVIDIA GPU with power management enabled and everything else.
[489.84 → 497.96] Obviously, they might want to change the username, but still it's, can you actually believe how simple it is to get the NVIDIA drivers installed on Nix?
[497.96 → 502.44] Yeah, I know. I know. That was my, one of my aha moments with Nix, actually.
[502.70 → 509.22] When I realized I was actually going to use it on the desktop was the first time I, I sat in, I'm like, okay, I'm going to get the NVIDIA graphics working.
[509.70 → 514.52] And it was what, three lines essentially. And I was done and it never breaks.
[515.28 → 516.86] Well, never say never.
[517.00 → 525.14] Never say never. You're right. But so far it hasn't broken. And at this point in time, it had broken at least once or maybe even twice on Fedora.
[525.14 → 532.52] It's probably more likely at least to break in the build time anyway, right? Where you're like, oh, well, the new kernel in this aren't going to build together, but hopefully not at runtime.
[532.86 → 538.40] And you just don't, you know, either that build doesn't complete or you just roll back if it somehow did complete, and it didn't work.
[539.12 → 547.28] So there's, it's, it's so nice. But I just, the point you just made, and I cannot stress it enough, is that it's, it is literally three lines right here.
[547.28 → 551.04] And somebody could copy this and paste it into their config. And now they have working NVIDIA graphics.
[551.94 → 558.22] And it's, and it's not, it's just so powerful. It's solved. We're talking about, we can solve these problems once as a community and just move on.
[558.22 → 567.08] Particularly with the AI stack. And we all know the famous Linus FM NVIDIA moment, right? We all, we're all familiar with that as Linux geeks.
[567.78 → 575.30] But with AI in particular, it's not just the NVIDIA drivers. You've got the CUBA toolkit and a bunch of other stuff going on underneath.
[575.30 → 582.26] And it's, it's mould, this is a layer cake of, of just complete pain and suffering on other places.
[582.56 → 589.06] And so for me, this, this local AI stuff at the moment, it's just a, you know, it's a it's a hobby. It's a hobby project.
[589.12 → 597.62] I'm not using it for anything serious yet. And so having this appliance config that I can just deploy at a moment's notice and be like, right, I'm going to get the latest drivers, blah, blah, blah, blah.
[597.98 → 603.02] And I don't have to hand crank Ansible playbooks and do all the rest of it. Like it's a game changer.
[603.02 → 609.88] I've been experimenting with a local app that uses the neural processor in the M series max.
[610.66 → 614.12] And I know if you have an NVIDIA, you could use this too. And it's called LM studio.
[614.56 → 621.18] And what I like about this is its another one of these desktop apps that lets you try various different large language models.
[621.54 → 628.62] And it ties in with hugging face, which we could talk more about and kind of helps me discover like which ones are popular right now, which ones have been recently submitted.
[628.62 → 633.96] And then it goes one step further and says, will this one perform well on your hardware specifically?
[634.34 → 634.82] That's nice.
[634.98 → 643.32] Yeah. It's called LM studio. And the URL I think is a little, little, it's just LM studio.ai. It's just really easy-peasy.
[643.64 → 648.02] It hadn't occurred to me that different models would be optimized for different hardware, but I suppose it makes sense.
[648.54 → 653.92] Yeah. Or some of them, you know, or just maybe it's probably more of them, more likely like some of them only really work on CUBA.
[653.92 → 656.18] Right. Yeah. Okay. Fair enough.
[656.92 → 662.92] Which sucks. But the nice thing about LM studio is that it is available for windows and Linux as well.
[663.34 → 667.96] And so if you've got, you know, if you want to do the CPU thing, they'll show you the ones that are going to work best case on your CPU.
[668.20 → 670.98] But if you have NVIDIA, you can, you know, filter on that.
[671.22 → 674.96] This is really nice. It exposes all the different models to you in the interface.
[675.10 → 682.18] And yeah, you can toggle through them and experiment with the results, and you can build automations around that for, I mean, I guess macro is probably more accurate.
[682.18 → 688.96] Things have really changed. I mean, you know, you're talking about Nix makes sense here because there are a bunch of dependencies, and it's really complicated.
[689.14 → 694.66] And it felt like probably for the past five years of machine learning hype as it's building, like you really had to commit to try it.
[694.74 → 699.36] But yeah, these days, if you have the right hardware, it's, I don't know, like one download away.
[699.64 → 703.88] Maybe that should be LM studio's tagline. LM studio, AI without Nix.
[703.88 → 715.64] Tailscale.com slash self-hosted. Head on over there, support the show and get 100 devices for free when you go to Tailscale.com slash self-hosted.
[716.68 → 722.56] Tail scale is the easiest way to connect your devices and services to each other directly wherever they are.
[722.70 → 727.86] Secure remote access to production, database servers, your Kubernetes cluster, whatever it might be.
[727.86 → 734.56] And it's really fast. Build your own flat mesh noise protected network.
[734.66 → 737.50] Yeah, that's the WireGuard protocol using Tail scale.
[737.82 → 740.38] I use Tail scale to bridge everything together.
[741.06 → 743.64] My systems are behind double carrier grade net.
[744.10 → 746.36] And that has always proved to be very, very challenging.
[746.80 → 749.18] And so I've had to use third party services here and there.
[749.22 → 753.60] And I ended up with like a mix and match of inbound ports and different VPN services.
[754.88 → 756.62] Tail scale let me unify all of it.
[756.62 → 763.12] I built out a simple network at first and then have layered on top of that ACLs and additional services over time.
[763.58 → 765.56] And it's a new way for me to do networking.
[765.80 → 767.34] It's intuitive. It's programmable.
[767.42 → 770.98] And I've created my own flat mesh network.
[771.24 → 774.78] Just as an example, if you're an iOS user, you can integrate shortcuts.
[775.00 → 776.82] So I have a shortcut on my wife's iPhone.
[776.98 → 781.70] When she plugs in her iPhone, it just launches and makes sure Tail scale is connected.
[782.04 → 786.40] That's really handy because then I can also have other things like her photo start backing up at that point.
[786.40 → 787.74] Over the Tail scale connection.
[788.38 → 793.02] On Android devices, I've tied it in with NFC connections to make sure Tail scale is connected.
[793.28 → 797.30] And then in Home Assistant, run a script that turns the thermostat on at the office.
[797.42 → 802.02] So right as I'm leaving home, I scan that NFC tag, and it turns the heater on.
[802.12 → 806.40] So by the time I arrive at my office, I have a decent temperature.
[806.96 → 811.78] The other thing that I'll use quite frequently is I'll start a project inside a VM or on a VPS.
[812.66 → 817.16] And then I'll want to move to a different system, or maybe I'll want to go home, and I want to have access to that VM.
[817.80 → 819.30] I just put Tail scale in that VM.
[819.88 → 823.00] And I can work on it if I'm there at the physical studio or not.
[823.36 → 824.44] And this is way out there.
[824.44 → 831.36] But one thing that I've been doing recently that I just have to tell you guys about is I put the Sunshine server on my Linux desktop here at the studio.
[831.36 → 834.54] That lets you do streaming using the Steam Link protocol.
[834.96 → 837.96] And I run the Sunshine client on my Oculus VR headset.
[838.50 → 841.84] So I connect Tail scale, which also runs on my Oculus VR headset.
[842.12 → 842.30] Yep.
[842.30 → 843.62] I sideloaded the APK.
[844.16 → 854.72] And then I can stream my GNOME Linux desktop inside my Oculus headset on a giant 110-inch screen using moonlight and sunlight over Tail scale.
[855.36 → 861.64] I know that's a big lot of jumble words, but people that know what I'm talking about, I think maybe they can appreciate how awesome this is.
[861.92 → 866.30] Because then I can pull up that Linux desktop on any machine, my iPad, my other desktops.
[866.30 → 875.76] Anything I have connected to my Tail net now has a very performant, because it's designed for game streaming, on-demand streaming Linux desktop.
[876.08 → 881.52] If I'm on the Mac that day and I need to get to something on Linux, I just pull up Moonlight on the Mac and I connect over Tail scale.
[882.02 → 884.28] And I'm streaming my GNOME desktop running Nix OS.
[885.20 → 893.68] I'm just telling you, you can build such powerful combinations of things that you don't even realize the power of it before you get started.
[893.68 → 903.66] And for businesses, it can streamline your remote access, and you can integrate it with your existing authentication infrastructure, your two-factor, your access and controls.
[904.02 → 911.42] But more importantly, you don't have to have some wild, huge VPN system that costs you who knows how much.
[912.10 → 913.98] I mean, I have seen the different hardware boxes.
[914.40 → 916.32] I have seen different licensing schemes.
[916.32 → 927.82] enterprises have needed to address this for a long time, and Tail scale does it in a way that uses your ACL policies so you can make sure everything is secured the way you already have it
[927.82 → 933.24] and replace your legacy VPN infrastructure in just minutes, at least on the client end.
[933.30 → 935.88] You can get it installed on any OS in just minutes.
[936.18 → 939.48] I can't account for how long the bureaucracy will take you, but it'll be worth it.
[939.60 → 940.14] Go try it.
[940.32 → 941.22] You guys, I love it.
[941.22 → 971.20] Go try it.
[971.22 → 973.02] That's a very didactic way to put it, yes.
[973.94 → 975.14] What do you think of it, Alex?
[975.58 → 977.24] It's basically Google Photos, isn't it?
[977.28 → 979.14] The logo just, you know, put in a blender.
[979.64 → 983.64] Yeah, and also, have you looked at the Apple Photos icon recently, too?
[983.70 → 984.46] It's also very similar.
[984.64 → 985.52] No, what does that look like?
[985.54 → 986.28] Yeah, it's very similar.
[986.46 → 986.84] It's different.
[987.06 → 988.18] Oh, yeah, it does, doesn't it?
[989.96 → 992.06] I guess this is what photo apps look like now.
[992.32 → 996.80] You suppose there's a benefit of, you know, you're jumping between your multiple phones, and the apps basically look the same.
[996.80 → 999.66] You have that rough intent of something photo-like, and you click it.
[999.66 → 1005.06] I do like it, because it's, you know, the typical rainbow colours of a Photos app.
[1005.16 → 1009.10] But it's made to look like the aperture of a camera lens, which is kind of nice.
[1009.20 → 1010.08] Yeah, it's a nice touch.
[1010.70 → 1010.84] Yeah.
[1011.26 → 1012.38] They did this through a contest.
[1012.62 → 1018.48] So they had a bunch of their users submit different designs, and the contest concluded at the beginning of March.
[1018.64 → 1021.76] And the winner, there'll be a link in the show notes to a blog post about it.
[1022.14 → 1023.76] Now, what are your thoughts around image in general?
[1023.84 → 1024.78] Are you using it still?
[1024.78 → 1026.22] Yeah, I use it all the time.
[1026.88 → 1028.18] It's become a bit of a meme.
[1028.30 → 1036.66] I was actually literally just talking to someone on the scale show floor about how image updates having breaking changes is becoming a bit of a meme.
[1036.80 → 1037.00] Yeah.
[1037.32 → 1043.26] Which is unfortunate, because the project is, you know, is very clear and upfront on their website about, this is alpha software.
[1043.46 → 1045.20] Do not rely on it yet.
[1045.20 → 1054.54] But, you know, when they yank out entire containers from the compose file between upgrades and then change, you know, database schemas completely.
[1054.90 → 1056.80] So far, I've had nothing actually break.
[1057.14 → 1064.36] But I do wonder, you know, it's like, it's not like Boeing at all, but it's reputational damage.
[1064.44 → 1065.76] We were just talking about this earlier, too.
[1065.76 → 1072.86] Like how people will get impressions of the project being unstable and broken and always breaking whenever you update it.
[1072.88 → 1073.66] So they won't touch it.
[1073.76 → 1077.28] And like, how long will that legacy last is my worry.
[1077.68 → 1078.70] Yeah, I feel you there.
[1078.80 → 1081.84] I think my worry is losing people.
[1083.20 → 1084.16] He might be losing.
[1084.40 → 1085.50] They might be losing me.
[1085.90 → 1088.42] I like it a lot, but I'm two or three behind.
[1088.42 → 1091.18] And you know this, we're going into conference silly season.
[1091.42 → 1098.66] I don't really see myself setting half a day aside to go through three or four version upgrades, because I think I have to do them sequentially.
[1099.62 → 1101.96] I don't know what I'm going to do instead, but, you know, I just don't.
[1102.10 → 1102.70] I don't.
[1102.80 → 1106.66] In the meantime, I just haven't updated because I'm, I mean, I'm in a kitchen in Pasadena.
[1106.80 → 1109.82] It's not the time to be redoing my entire photo backup.
[1110.12 → 1112.02] So you've changed your ways, because I remember.
[1112.24 → 1115.26] Well, this is the problem is my process got interrupted.
[1115.36 → 1116.98] I didn't get to do my pre-trip updates.
[1117.26 → 1117.58] Okay.
[1117.58 → 1119.54] This is why I try to do it.
[1119.76 → 1119.92] Okay.
[1120.58 → 1124.44] And it's, but the problem is, is that when there's a lot of breaking changes like this, I just don't have the time.
[1124.70 → 1128.70] It is nice, at least, you know, being going the self-hosted route that you don't have to update.
[1128.80 → 1129.76] You don't get any new features.
[1129.76 → 1134.56] And maybe you have to worry about a security thing if you weren't using tail scale, but you can choose to just use that version.
[1134.72 → 1140.94] That's what I'm doing is I'm just, I've just, everything's just the client apps, the server apps are just frozen in time right now.
[1140.98 → 1141.92] Everything's over tail scale.
[1142.60 → 1144.24] But I don't know.
[1144.24 → 1147.54] How many times am I going to do this?
[1147.58 → 1148.08] I'm not sure.
[1148.24 → 1150.30] I think they might be starting to lose me a little bit.
[1150.42 → 1152.08] The updates are very frequent.
[1152.80 → 1153.00] Yeah.
[1153.00 → 1161.52] I don't know if I would rather one update every three months that has, you know, 500 breaking changes or one update every two weeks that has a couple.
[1161.78 → 1161.94] Yeah.
[1161.98 → 1167.76] I feel like it's, I just should come back in a year or two, maybe, you know, maybe it's a maybe come back in two or three years.
[1167.76 → 1169.26] But what would I use in the meantime?
[1169.26 → 1169.66] Right.
[1169.66 → 1170.08] Exactly.
[1170.30 → 1172.86] And I've built like my home assistant tablets.
[1173.52 → 1176.16] Several of them show photos that come from my image folder.
[1176.26 → 1177.82] So I've built like workflows around this.
[1178.56 → 1181.18] I've got, I've got it working on iOS and Android.
[1181.18 → 1187.14] I do know it works for some apps, you know, that's just even getting it on two devices and having backups successfully is a trick.
[1187.42 → 1190.26] Is there a facility to like export and import data?
[1190.48 → 1194.06] Do you have to do an in-place upgrade, or could you ever do a, you know, like a totally fresh installation?
[1194.06 → 1195.12] This is an interesting point.
[1195.20 → 1201.36] And I don't think we've really talked about this much on the show about how people would version their app data.
[1201.72 → 1208.16] I'm not talking about the photos specifically here because those images, image I don't think is very destructive in what it does during that.
[1208.26 → 1212.22] I'm talking about like the backend database for image itself and all the rest of it.
[1212.86 → 1217.68] And ZFS datasets, in my opinion, take some beating because you can take a snapshot before you do an upgrade.
[1217.68 → 1228.06] And then if it goes sideways, you can mount the old snapshot as a new file system and point the old Docker compose file to that old data set and copy on write being what it is.
[1228.10 → 1229.76] It would just carry on chugging just fine.
[1230.20 → 1239.24] I hadn't really given thought to nuking it because in theory, if I'm okay with losing the metadata, it would just rescan the files.
[1239.70 → 1243.10] It'd have to retrain on the faces, and maybe it's better now.
[1243.16 → 1244.74] Maybe they've got better models and yeah.
[1244.74 → 1244.80] Yeah.
[1245.56 → 1245.88] Hmm.
[1246.46 → 1251.06] Because then you could kind of wait, yeah, wait, wait a year or two, whenever you're kind of, it seems like it's worth upgrading.
[1251.94 → 1253.94] Otherwise you just get further and further behind, right?
[1254.02 → 1254.62] That's the problem.
[1254.74 → 1255.44] I am.
[1256.06 → 1256.42] Yeah.
[1257.20 → 1257.60] Yeah.
[1257.74 → 1258.00] Huh.
[1258.06 → 1258.34] Okay.
[1258.38 → 1259.34] I'm going to give that thought.
[1259.42 → 1265.38] You know, it's funny, both with my Nextcloud install and now my image install, I'm thinking maybe I will just blow them away and start over.
[1265.84 → 1269.24] I mean, I'm still running Nextcloud for my photo backup as well as image.
[1269.24 → 1273.40] So I've currently got duplicates of everything, which I know one day that tax is going to become due.
[1273.40 → 1275.54] And I'm going to have to go through and sort them all.
[1276.06 → 1276.20] Yeah.
[1276.52 → 1283.78] But I mean, at the top of the image project, to be fair, I know we're sat here, you know, a bunch of old men talking about a problem of our own making.
[1284.60 → 1288.12] But it does say the project is under very active development.
[1288.68 → 1290.34] Expect bugs and changes.
[1290.62 → 1294.28] Do not use this project as the only way to store your photos and videos.
[1294.38 → 1295.94] I mean, it says that at the top of the page.
[1296.22 → 1296.36] Yep.
[1296.36 → 1298.00] But they're very clear about it.
[1298.02 → 1299.96] And, you know, we've said it too.
[1300.68 → 1302.54] And I know.
[1302.96 → 1304.78] I mean, I do obviously have the photos backed up.
[1304.84 → 1307.52] But what I want is a way to view them and find them.
[1308.28 → 1309.16] That's what it does for us.
[1309.16 → 1309.18] An interface.
[1309.72 → 1310.64] It's so good.
[1310.84 → 1311.44] The potential.
[1311.62 → 1312.28] We can feel it.
[1312.38 → 1313.08] It's tangible.
[1313.48 → 1316.12] That's why we're like trying to get there before it's ready.
[1316.60 → 1317.74] It's come a long way already.
[1317.86 → 1318.90] I mean, it's quite impressive.
[1319.08 → 1319.96] Most definitely has.
[1320.20 → 1320.28] Yeah.
[1320.80 → 1325.48] Hey, speaking of updates, Home Assistant had a really nice update to its UI this week.
[1325.60 → 1327.82] And speaking of something that's been a long time coming.
[1328.30 → 1332.50] They got proper drag and drop support in that update for the Home Assistant dashboard now.
[1332.50 → 1333.48] I swear I saw.
[1333.60 → 1334.48] I think it was Mark.
[1334.76 → 1339.04] Mark Watts Tech or something on YouTube demo this like two or three years ago.
[1339.84 → 1342.76] I'm honestly kind of surprised it wasn't already in Home Assistant.
[1342.88 → 1347.40] It's one of those things like you were just saying this before the show, Chris, that drag and drop should have been in.
[1347.50 → 1349.12] This is how it should have been from the beginning.
[1349.12 → 1350.22] And now it's there.
[1350.32 → 1351.20] I'm really glad it's there.
[1351.38 → 1352.92] But it should have always been that way.
[1353.72 → 1358.08] I kind of caught on the live stream that they've taken a couple of cracks at this in the past.
[1358.10 → 1360.14] And they tried to solve this a few different ways.
[1360.18 → 1362.18] And we're never really quite happy with what they came up with.
[1362.24 → 1367.58] But they feel like I think with a newer staffer, I think came up with a kind of way that really cracked it.
[1368.28 → 1368.50] Yeah.
[1368.82 → 1370.60] And you were trying it before the show.
[1370.78 → 1372.84] And it's really nice.
[1372.88 → 1375.30] You can move the individual objects between different sections.
[1375.30 → 1378.50] And it's so well done.
[1378.58 → 1380.16] You think, oh, yeah, I should have always done this.
[1380.50 → 1382.42] And it's exactly how people would expect it to work.
[1382.56 → 1388.88] And it's one of those features that when new users use Home Assistant, they'll never realize the time when that wasn't possible because it just seems natural.
[1389.34 → 1389.36] Right.
[1389.36 → 1389.44] Yeah.
[1389.92 → 1391.48] So you create different columns.
[1391.64 → 1396.24] And it's not a fundamental rewrite of the Lovelace UI that you know and love of Home Assistant.
[1397.00 → 1398.48] It's a subtle change.
[1398.58 → 1400.54] Like everything is a little more rounded on the corners.
[1400.84 → 1402.56] Everything just looks a little nicer.
[1403.16 → 1408.60] But if you, say, have a specific horizontal stack that you want to drag between one column and the next,
[1408.60 → 1419.92] with the current Home Assistant dashboard, you'd have to go into the config and change the sort order and then copy and paste certain bits of code from one kind of card stack into a different.
[1420.24 → 1422.50] I don't know if I'm using the right terminology there.
[1422.62 → 1425.20] But here, this just works the way I'd want it to.
[1425.24 → 1426.30] I've got a group of cards.
[1426.40 → 1428.64] And I think that light bulb should actually be in this room.
[1428.92 → 1431.64] I can drag it between those two different cards in the interface.
[1431.88 → 1435.02] No coding required, which is just, it's great.
[1435.50 → 1436.68] They also have a new section view.
[1436.68 → 1442.00] So, you know, when you create a new tab on your dashboard, you have like these different layout options, these standard layout options.
[1442.10 → 1444.48] They've got this new sections option.
[1445.00 → 1451.94] I have not tried this yet, but it looks almost perfect for what I use for a purpose-built dashboard for heating.
[1452.28 → 1457.60] I have one for the, you know, the whole house, the out and under systems, and then the bathroom.
[1457.92 → 1459.24] And each one is its own dashboard.
[1459.52 → 1464.58] And I've kind of really had to jerry-rig the current system to get the views to work.
[1464.58 → 1466.16] And this might be it.
[1466.16 → 1466.92] It's called sections.
[1467.02 → 1468.40] It is experimental right now.
[1469.10 → 1469.46] Nice to see that.
[1469.48 → 1471.90] Yeah, so to get access, you go into your Home Assistant dashboard.
[1472.14 → 1473.56] Click on the edit button in the top corner.
[1474.22 → 1477.84] And if you create a new page, that's probably the best place to go for right now.
[1478.44 → 1482.94] There is an option under view type marked sections, brackets, experimental.
[1482.94 → 1486.92] This week in Bitcoin.
[1486.92 → 1487.04] Bitcoin.
[1487.18 → 1490.72] It's a new show in development inside the Jupiter Broadcasting Labs.
[1490.92 → 1492.80] And you're one of the very first to hear about it.
[1492.90 → 1495.92] Now, you guys maybe know that I've been following Bitcoin since around 2012.
[1496.88 → 1501.06] But I think right now it's actually one of the most interesting time ever for Bitcoin.
[1501.94 → 1503.56] Definitely the launch of the ETFs.
[1503.56 → 1505.72] That's been kicking off a new phase in development investment.
[1505.72 → 1513.22] So starting in just the next few months, we're going to see new types of projects and new types of development happening on Bitcoin at a level we've never seen before.
[1513.22 → 1523.02] But maybe even more importantly, I think there's just a new interest ignited and a desire to understand what might be the hardest money mankind has ever known.
[1523.66 → 1537.32] And one of the most exciting things for me that the show will try to capture is that when you learn Bitcoin, it does reveal what is so broken about all the other systems and why an open source currency that is not tied to any particular state is going to be so important in our future.
[1537.32 → 1541.28] It really is a peaceful revolution by the people, one sat at a time.
[1541.66 → 1543.94] And I'm going to cover it each week on This Week in Bitcoin.
[1544.36 → 1548.64] So go find The Signal at www.thisweekinbitcoin.show.
[1549.20 → 1556.36] That's thisweekinbitcoin. Show, a high signal Bitcoin news podcast in development right now focused on analysis that you'll find valuable.
[1557.42 → 1558.58] Thisweekinbitcoin.show.
[1558.74 → 1560.60] Go check it out and let me know what you think.
[1561.30 → 1565.22] We're on the ground floor and anybody that's interested in learning more is welcome.
[1566.08 → 1566.72] Go find it.
[1566.72 → 1569.86] Once more, it is thisweekinbitcoin.show.
[1570.26 → 1573.10] Give it a listen, send me your feedback and let me know what you think.
[1574.02 → 1575.52] Thisweekinbitcoin.show.
[1577.34 → 1587.62] You know, when you finish up a big server build, and you've been planning it for a few weeks, and you think everything's going to work this way, and then you actually get to using it, and you think, you know, it should have worked that way.
[1589.06 → 1590.16] That can be a hard one.
[1590.38 → 1595.16] Well, for me, it was the fact that I'm still experimenting with all this AI stuff.
[1595.16 → 1601.48] So I'm, you know, bringing the box up and down as I'm doing PCI pass through and, you know, just I'm testing out.
[1601.48 → 1603.74] I'm finding the edges on this Epic box.
[1603.96 → 1607.14] And my media server, you know, I have a three-year-old in the house.
[1607.22 → 1613.30] The uptime for my pseudo-prod media box needs to be 100% or as close to as I can manage.
[1613.30 → 1615.58] You know, it's funny because it only gets worse as they get older.
[1616.06 → 1618.46] I get requests now all the time.
[1618.74 → 1624.38] I mean, my kids are my down detector for the Plex system because one of them in the house always has Plex going.
[1624.48 → 1632.80] Even if they're not, like, actively watching it, they have, like, their favourite cartoon running in the background now with no concept that dad's server is just sitting there churning away.
[1632.94 → 1633.06] Right?
[1633.10 → 1633.58] I don't care.
[1634.96 → 1638.60] Woe betide you if you interrupt Peppa Pig with an accidental reboot.
[1638.60 → 1645.22] So this led me to kind of thinking about I want to change the approach to this whole server rebuild.
[1645.34 → 1649.12] My kind of idea going into this was to have one box to rule them all.
[1649.20 → 1652.70] The Epic box was going to be everything all in one place.
[1652.76 → 1658.04] But actually, if I think about it, like, as a home lab, I want to have the freedom to reboot whenever I want.
[1658.92 → 1668.06] So really what I want is a home lab box, which is what the Epic one can fulfill to run VMs and, you know, have lots of RAM and storage to do all that kind of stuff really quickly.
[1668.60 → 1673.52] But for production, for pseudopod, I want a media server that is declarative.
[1673.64 → 1674.58] I want an appliance.
[1675.16 → 1675.76] Runs in the corner.
[1675.98 → 1679.44] You update it when you need to occasionally, and otherwise it just works.
[1679.84 → 1680.28] Exactly.
[1681.34 → 1691.78] So I decided to move all the hard drives I'd just put into the Epic box back into Morpheus, into the Intel i5-based server that's been running honestly fine for the last little while.
[1691.88 → 1694.64] Did you just take 10 minutes and make this decision?
[1694.74 → 1695.82] Did you wait a day?
[1695.82 → 1697.24] You know what I did?
[1697.38 → 1700.82] I actually had a little chat with myself in my journal about it.
[1700.92 → 1703.98] And I was writing, I did this particular entry in Obsidian.
[1704.12 → 1710.74] I was trying to write bullet points about where different ZFS data sets should live for my main data versus media centre data.
[1710.90 → 1713.96] And I'm like, you know what makes sense, Alex, if you just have two servers?
[1714.74 → 1718.76] And it's just one of those things as you're talking to yourself, you're like, just the solution is really obvious.
[1718.84 → 1720.46] Okay, you've got to run two boxes, not one.
[1720.46 → 1724.46] But you've already got the hardware in front of you, why not just do that?
[1724.70 → 1725.30] Right, right, yeah.
[1725.60 → 1739.34] And so as I put those boxes back together again, the media server, the Morpheus box, the only hardware change that really happened to that, besides pulling a hard drive, a couple of hard drives in and out, was a new HBA card.
[1739.34 → 1741.94] I went from an 8 port to a 16 port HBA card.
[1742.66 → 1746.14] And I was replicating a bunch of the ZFS data between the two boxes.
[1747.16 → 1749.66] And it just hard locked on me.
[1750.32 → 1750.86] Don't you hate that?
[1751.20 → 1752.22] Oh, it's always so distressing.
[1752.36 → 1753.58] I mean, what could be wrong?
[1753.68 → 1754.56] How do you troubleshoot it?
[1754.58 → 1755.52] It's a new system too.
[1755.70 → 1759.24] So it could be a new kernel.
[1759.58 → 1761.44] It could be something wrong with the config.
[1761.80 → 1762.48] Well, here's the thing.
[1762.98 → 1764.40] This was on the media server.
[1764.40 → 1768.82] So all the ZFS data was in the Epic box, which was somewhere else.
[1769.16 → 1778.92] This was replicating back to the media centre box on some of the 18 terabyte hard drives I bought on Black Friday, which I still hadn't actually figured out what to do with because I've just been so busy.
[1779.30 → 1781.24] Finally, I have a solution of what I'm going to do with them.
[1781.32 → 1783.24] I'm just going to replicate ZFS between the two boxes.
[1783.84 → 1785.16] Everything's going to be in both places.
[1785.70 → 1787.68] And the source of truth will be Epic.
[1788.66 → 1792.50] But I've got to back up 100% every hour on the other one.
[1792.50 → 1794.12] 10 gig link should be tasty.
[1794.68 → 1800.32] But as I was doing that replication back to Morpheus, the media server box, that's when the hard lockups happened.
[1800.44 → 1803.44] I'm like, right, okay, I've just deployed NixOS on this server.
[1803.54 → 1810.86] I've just reached terminal velocity to escape Proxmox and actually put NixOS into pseudopod.
[1811.62 → 1813.40] And I'm thinking, it's locking up.
[1813.74 → 1816.28] Well, okay, once is, okay, weird.
[1816.82 → 1818.30] And I'm going to try again.
[1818.30 → 1823.48] And the reproduction conditions are just a simple synod ZFS send.
[1823.48 → 1824.72] I'm not doing anything crazy.
[1824.84 → 1826.30] There are no apps running on this box yet.
[1826.36 → 1829.64] It's just replicating ZFS data, not under load.
[1829.64 → 1829.88] Right.
[1830.68 → 1831.66] Work up the next morning.
[1832.14 → 1833.16] No TTY chain.
[1833.32 → 1836.80] I can't, you know, the PMI still works, but I can't type on the keyboard.
[1836.96 → 1837.84] I can't control C.
[1837.96 → 1838.98] I can't ping it.
[1839.08 → 1840.58] It's like, it's just, it's dead, Jim.
[1841.14 → 1842.90] You can't pretend like that didn't happen.
[1843.62 → 1843.86] Twice.
[1844.06 → 1844.20] Yeah.
[1844.58 → 1844.82] Yeah.
[1844.86 → 1846.38] I mean, your trust goes out the window.
[1846.38 → 1848.78] Well, so then I thought, well, it must be NixOS.
[1848.98 → 1852.50] There must be some, because this, the hardware in this box, the like I say, the only thing
[1852.50 → 1853.52] that changed was the HBA.
[1853.78 → 1856.60] Everything else in this box, I didn't even take the RAM out of the slots.
[1856.70 → 1858.58] I didn't even unplug a power supply cable.
[1858.58 → 1862.56] Like everything that's been stable for the last two or three years was the same.
[1862.88 → 1865.70] And so I'm like, well, it must be software.
[1866.06 → 1866.80] Has to be software.
[1866.96 → 1870.84] Because then I rebooted into an Ubuntu live CD and ran it for two or three hours, which
[1870.84 → 1872.70] it was locking up after about 45 minutes.
[1872.90 → 1874.96] I had two or three hours of stable replication.
[1875.10 → 1877.88] And I'm like, oh, well, yeah, it must be Nix then.
[1878.32 → 1881.28] So I wiped NixOS, put Proxmox back on the server.
[1881.56 → 1886.16] This time it took five hours and 40 minutes to lock up, but it locked up again.
[1886.18 → 1887.30] And I'm like, oh crap.
[1887.30 → 1890.56] Well, okay, not crap, because I suppose that means it's not Nix.
[1890.94 → 1891.70] It's not Proxmox.
[1891.80 → 1892.58] It must be hardware.
[1892.72 → 1893.12] It's got to be hardware.
[1893.22 → 1894.10] But it's still a problem.
[1894.68 → 1900.84] So I pulled out the 16, the LSI 16i HBA card, put in my old eight port Dell cards, had to
[1900.84 → 1904.42] unplug a couple of SSDs because I've now run out of starter ports.
[1905.06 → 1905.72] But that's fine.
[1905.74 → 1907.36] I could make that work just for the testing.
[1907.80 → 1912.02] And it just replicated all 12 terabytes, which finished whilst I was on the plane on the
[1912.02 → 1913.06] way over to LA this morning.
[1913.38 → 1914.60] So it was the HBA.
[1914.88 → 1915.52] Pleased to report.
[1915.52 → 1917.66] Yeah, I guess pleased to report it was the HBA.
[1918.00 → 1918.20] Yeah.
[1918.68 → 1922.30] Do you have, you had a chance to look, is there like some sort of driver issue in the later
[1922.30 → 1922.90] Linux kernel?
[1923.02 → 1924.54] Of course, I guess it was in Proxmox too.
[1924.86 → 1925.62] So yeah, I don't know.
[1925.70 → 1929.04] I mean, Proxmox is 6.5, I think.
[1929.24 → 1929.60] Newish.
[1929.68 → 1930.36] I can check that.
[1930.54 → 1930.74] But yeah.
[1931.24 → 1931.86] So it could be.
[1931.98 → 1932.22] Yeah.
[1932.22 → 1934.50] That's such a bummer.
[1935.36 → 1939.02] You know, because you, I mean, actually you, in all things considered, tracked it down
[1939.02 → 1939.52] pretty quick.
[1939.92 → 1940.20] Yeah.
[1940.28 → 1941.08] I was lucky, really.
[1941.26 → 1943.38] I mean, Proxmox 6.5, I just checked.
[1943.50 → 1943.64] Okay.
[1944.16 → 1945.12] So that's fairly recent.
[1945.26 → 1946.84] Nix OS, I think, was 6.1.
[1947.18 → 1948.08] So I was a little bit older.
[1948.62 → 1953.28] And some suggestions on Mastodon were that I wasn't running the correct kernel.
[1953.40 → 1957.10] So I was like, well, maybe I could go and tweak my Nix config and change the kernel and,
[1957.20 → 1958.34] you know, do a few things here and there.
[1958.54 → 1963.10] Because it's Nix OS, I can just share the entire system configuration with the world.
[1963.42 → 1967.58] Which, by the way, you're a beautiful bunch of nerds for helping me out on Mastodon with
[1967.58 → 1967.94] that one.
[1968.76 → 1968.88] Yeah.
[1968.88 → 1970.08] But see, you know, it was hardware.
[1970.40 → 1974.98] And it's just, there can be a real bitch to figure out whether it's, you know, I even
[1974.98 → 1979.20] dropped a me test for six hours just to prove it wasn't memory or anything, you know?
[1979.86 → 1980.22] Yeah.
[1980.24 → 1981.60] I can see you trying to work through it.
[1981.64 → 1985.02] Because I don't think I would suspect the HPA at first either.
[1985.54 → 1987.16] I would probably suspect memory.
[1987.32 → 1989.18] I think I also would think kernel issue.
[1989.32 → 1989.48] Yeah.
[1989.52 → 1993.80] Is it some kernel config setting or a weird module that Nix OS loads that Ubuntu doesn't?
[1993.96 → 1994.22] Right.
[1994.22 → 1999.44] I think your idea to swap over to an Ubuntu install and run the replication there for
[1999.44 → 2002.46] a while, that was good because then you start eliminating, like, you know, the kernel issue.
[2002.46 → 2003.70] It was just a totally live system.
[2003.78 → 2007.18] Because the other thing I was doing in Nix OS was running ZFS on a mirrored root for the
[2007.18 → 2007.68] first time.
[2008.62 → 2009.22] Who knows?
[2009.54 → 2010.80] I mean, I think it's fine.
[2011.20 → 2014.38] The internet tells me it's stable, but I don't know.
[2015.02 → 2015.24] Yeah.
[2015.58 → 2016.54] I think it will be.
[2016.66 → 2017.28] At least on Nix.
[2017.42 → 2020.94] I mean, because, you know, if it doesn't build, again, you just don't switch.
[2020.94 → 2025.72] Which benefits of running a mirrored ZFS root on Nix OS, though, I kind of talked myself
[2025.72 → 2027.36] into and out of it several times.
[2027.52 → 2033.40] Like, if I've got a fully declarative repeatable system, why the hell do I need a mirrored boot
[2033.40 → 2033.70] drive?
[2034.26 → 2035.00] Yeah, you might not.
[2035.10 → 2037.06] I mean, it's extra guarantees.
[2037.06 → 2039.86] It's another style of rollback in some sense.
[2040.02 → 2040.20] Yeah.
[2040.58 → 2042.10] So why did you decide to do it then?
[2042.82 → 2043.18] Why not?
[2043.58 → 2044.06] Why not?
[2044.18 → 2044.42] Yeah.
[2044.72 → 2045.40] I guess.
[2046.48 → 2046.88] Uptime.
[2046.88 → 2051.62] I mean, I guess if, for example, one of those SSDs goes bang in the middle of the night,
[2052.04 → 2053.28] Pepper Pig will still work in the morning.
[2053.68 → 2053.92] Yeah.
[2054.56 → 2055.66] It's uptime guarantee.
[2055.86 → 2058.26] It's not, you know, a redundancy guarantee that I'm after.
[2058.76 → 2059.52] Yeah, that makes sense.
[2060.14 → 2061.58] Yeah, I could definitely see it from that standpoint.
[2061.80 → 2063.66] I mean, it's much better than doing Brake FS.
[2064.60 → 2066.00] Not that we would do that.
[2066.66 → 2067.08] No, never.
[2067.50 → 2067.66] Yeah.
[2067.68 → 2069.86] So for now, I've reverted to Proxmox.
[2070.14 → 2073.24] And for the foreseeable future, I think I'll continue with Proxmox.
[2073.34 → 2075.96] I'm just, I feel more comfortable with that on the home server.
[2075.96 → 2076.94] I can add it to the cluster.
[2077.06 → 2078.18] So it's all part of the web UI.
[2078.68 → 2080.42] I can do the PCI pass through if I want to.
[2081.22 → 2084.06] I'm still annoyed that I've, like, skipped off the atmosphere of Nix.
[2084.12 → 2086.62] And I was so close to actually deploying it.
[2086.62 → 2088.36] I might still go back to Nix, but we'll see.
[2088.56 → 2089.08] I see.
[2089.22 → 2089.52] Okay.
[2089.62 → 2090.34] Well, that's fine.
[2091.02 → 2091.98] Proxmox is a good tool.
[2092.46 → 2092.84] It is.
[2092.90 → 2093.44] It is indeed.
[2093.94 → 2097.26] Anyway, you asked a question in the last episode about how much would someone pay for
[2097.26 → 2097.88] a home server.
[2097.88 → 2099.20] And we had some feedback come in.
[2099.66 → 2104.50] So on the topic of how much I would be willing to pay for a home server, I think about 200 US
[2104.50 → 2110.14] dollars for the CPU motherboard, basically the entire server without disks, for a refurbished
[2110.14 → 2116.34] office desktop is about what I would like to spend for a NAS, running Jellyfin, C-File,
[2116.50 → 2118.84] Borg Backup, Ecotourism, and much more.
[2119.40 → 2122.38] I'm considering an upgrade to a custom-built rig in a few years, though.
[2122.60 → 2126.24] Maybe I'll put my budget in the $500 to $800 range or so.
[2126.24 → 2131.00] I rip all of my own media to formats that don't require any transcoding, which reduces
[2131.00 → 2133.18] my CPU requirements significantly.
[2133.82 → 2137.88] And my family's use of last-decade office boxes as well doesn't cause any performance
[2137.88 → 2138.36] problems.
[2138.66 → 2143.78] The only advantage I would have in upgrading is reducing power draw and expanding hard
[2143.78 → 2144.42] drive capacity.
[2144.84 → 2147.20] So I guess I'll wait till I need more capacity.
[2147.78 → 2148.96] Simple is good.
[2149.08 → 2149.74] Yeah, I like that.
[2150.06 → 2150.46] I like that.
[2150.62 → 2151.56] As long as...
[2151.56 → 2154.86] I think where we were starting to talk about the prices going up a lot is when you start
[2154.86 → 2160.54] talking about doing the AI models or if you're doing transcoding for several people because
[2160.54 → 2161.56] there are different formats.
[2162.28 → 2167.40] And I can totally sympathize with that because my home server, my actual home server, is an
[2167.40 → 2168.74] Droid, you know?
[2168.86 → 2171.92] And we really don't do much with it.
[2172.26 → 2173.02] Well, that's not true.
[2173.08 → 2176.00] It does a lot of things, but it's capable of doing all of them.
[2176.52 → 2180.24] But any of the AI workload stuff always has to be on systems at the studio because that's
[2180.24 → 2181.54] where we have much larger systems.
[2181.98 → 2184.84] I will say it's pretty liberating thinking, right, I need 64.
[2184.86 → 2186.06] gigs of RAM for this system.
[2186.26 → 2186.38] Yeah.
[2187.00 → 2187.28] Bop.
[2187.40 → 2187.86] There you go.
[2188.20 → 2188.72] No problem.
[2188.90 → 2189.04] Yeah.
[2189.18 → 2189.34] Yeah.
[2189.50 → 2190.66] I can see it both ways.
[2191.12 → 2193.16] I can definitely see the value in just a couple of hundred bucks.
[2193.26 → 2194.60] What's the sweet spot for you, Was?
[2194.90 → 2197.08] Like if you're going to build a little home media, NAS?
[2197.82 → 2199.14] Yeah, I suppose it depends on the scale.
[2199.30 → 2201.56] Like are you serving friends and family?
[2202.20 → 2206.86] How much experimenting are you doing versus sort of just running kind of fixed infrastructure?
[2207.02 → 2210.96] Like if it's just Nextcloud and Jellyfin with a light load, that's one thing.
[2210.96 → 2214.30] Or yeah, if you want to play with AI models, or you're running your own software that you're
[2214.30 → 2216.90] making or serving your friends or doing a bunch of backups.
[2217.46 → 2224.36] I can see you doing a little box, just a base Nick server with probably some AI models on it
[2224.36 → 2224.80] if you could.
[2224.80 → 2224.92] Yeah.
[2225.28 → 2225.38] Yeah.
[2225.60 → 2226.38] How much K exec?
[2226.38 → 2227.64] Oh, yeah.
[2228.10 → 2229.94] How much K exec can you run at once?
[2230.60 → 2232.30] That's a good question.
[2233.20 → 2236.08] And, you know, I love doing stuff in Tempo Fest and RAM.
[2236.20 → 2238.00] So I like a box that has a lot of RAM.
[2238.16 → 2238.34] Yeah.
[2238.48 → 2240.88] It also depends, like, how long do you think you're going to keep it?
[2241.34 → 2245.42] You know, you might be able to argue for a higher price if you think it'll pay off in
[2245.42 → 2246.14] five years.
[2246.32 → 2246.96] That's what I'm thinking.
[2247.54 → 2247.84] Yeah.
[2247.88 → 2250.96] If you're somebody that's going to use a system for a couple of years, I'd say keep it
[2250.96 → 2251.62] on the cheaper side.
[2251.62 → 2256.56] If you can five plus years and even, you know, for me, it doesn't have to be doing
[2256.56 → 2258.20] the same job for that five years.
[2258.68 → 2263.86] You know if it can be doing something productive and useful that I get value for five or six
[2263.86 → 2266.94] years, then I think you can start talking about a higher price point.
[2267.56 → 2271.56] And also maybe it depends, too, like how much is this a part of your life and how much can
[2271.56 → 2273.60] you afford to direct of your expenses?
[2273.72 → 2277.16] I think for us, it helps out that we really enjoy it as a hobby as well.
[2277.22 → 2280.96] But if you just have it more as an appliance box that you kind of don't touch and, you
[2280.96 → 2284.08] know, you have other stuff you're working on, maybe it's not worth as much.
[2284.42 → 2290.10] I love coming across people on YouTube who are clearly not technical, talking about NASS
[2290.10 → 2290.40] and stuff.
[2290.46 → 2296.18] I came across this guy whose known much more for being a film, like lighting and, you
[2296.18 → 2297.90] know, video production kind of guy.
[2298.48 → 2301.34] Obviously, if he's into that, he's got footage storage requirements.
[2301.34 → 2307.48] And so he's just bought a Synology to mirror his footage from his house to his editor's system
[2307.48 → 2309.80] as well so that the offsite editor can do all that kind of stuff.
[2309.80 → 2314.22] And I'm like, it's really, it's just interesting listening to normals talk about this kind
[2314.22 → 2319.08] of stuff who just want a turnkey appliance versus us who are much more comfortable with
[2319.08 → 2321.72] sort of buying a jigsaw and putting it together ourselves.
[2322.22 → 2323.84] I think this is why the Drop was so successful.
[2323.98 → 2325.94] Well, it was a thing for so long.
[2326.04 → 2328.48] I don't know about successful, but this is why the Drop was a thing.
[2328.88 → 2329.54] People just want it.
[2329.54 → 2333.58] And, you know, they didn't even, the Drop promise was you don't even have to have the
[2333.58 → 2334.40] same size disc.
[2334.40 → 2335.32] Yeah.
[2335.78 → 2336.10] Yeah.
[2336.40 → 2336.64] You know.
[2336.94 → 2339.06] Well, Unpaid still kind of flies that banner a little bit.
[2339.16 → 2340.14] Merger FS too, but.
[2340.20 → 2340.32] Yeah.
[2340.92 → 2341.16] Yeah.
[2341.56 → 2344.62] Synology has their hybrid raid thing, which I think does that as well.
[2344.78 → 2348.68] So, I mean, it's, it's clearly, it's clearly still a desire for folks.
[2348.74 → 2352.90] I mean, whenever you listen to folks talk about ZFS about, you know, or just add a pair of
[2352.90 → 2358.46] 20 terabyte discs for a new VDE or whatever, you think, yeah, but that's at least 600,
[2358.46 → 2364.02] if not more dollars per throw, you know, and I don't know about you, but that's still a
[2364.02 → 2365.34] lot of money to me.
[2366.08 → 2366.44] Yeah.
[2366.84 → 2368.18] I'd love to know what people think though.
[2368.22 → 2370.52] I, on this whole, what is your budget for a home server?
[2370.56 → 2374.88] I'm still, I'm still querying the audience because I don't think we have consensus exactly.
[2375.40 → 2376.48] So let me know what you think.
[2376.52 → 2380.04] What would you pay for a home server with a five-year life run?
[2380.28 → 2380.52] Yeah.
[2380.58 → 2381.16] I like that.
[2381.26 → 2381.66] Five years.
[2382.00 → 2382.12] Yeah.
[2383.12 → 2388.24] Venom came in with 54,345 SATs, and it was first time boosting the show.
[2388.24 → 2389.32] So thank you very much.
[2389.98 → 2392.18] I know that part is the biggest part of the trek.
[2392.40 → 2393.26] They write, thank you all.
[2393.34 → 2396.04] You are responsible for my irresponsible home lab purchases.
[2396.88 → 2402.12] Alex, your Docker orchestration feature request is the existing use case of Kubernetes.
[2402.92 → 2403.76] No, it's not.
[2404.24 → 2405.74] No, it isn't.
[2405.94 → 2407.30] Come join us in the case.
[2407.40 → 2408.20] Home lab world.
[2408.36 → 2409.96] We have tail scale operators.
[2410.10 → 2411.94] You can set it all up with Ansible tube spray.
[2412.84 → 2417.42] Customizes a better Docker compose, and you can stand up an entire home lab application for
[2417.42 → 2420.58] a system with quick testing on a whim with a single helm command.
[2420.68 → 2421.44] Oh yeah, sure.
[2421.96 → 2423.86] Helm is my absolute favourite.
[2424.04 → 2427.02] You know, it's like pseudo pipe to bash, but even more obscure.
[2427.52 → 2433.68] As a bonus cube spray plus K8s makes running workloads on and managing a bunch of micro PCs
[2433.68 → 2436.72] like you've been talking about something you don't even have to think about.
[2436.72 → 2441.20] Oh, and speaking of, I'd like to challenge the team to try out Bellini OS.
[2441.54 → 2445.90] If you haven't before with three old speakers and three pies, 30-minute journey to three
[2445.90 → 2448.24] rooms, Sonos with Bellini sound.
[2448.88 → 2450.82] You know, I have looked at that.
[2450.90 → 2452.38] They're the ones that make Etcher now too, right?
[2452.60 → 2453.06] Yeah, indeed.
[2453.30 → 2453.50] Yeah.
[2453.50 → 2456.98] I've looked at that and I have considered just taking it.
[2457.06 → 2460.94] I have some speakers my dad gave me that would be perfect for that.
[2461.00 → 2463.64] And I got a little amp to connect them to and a Raspberry Pi on the input.
[2463.94 → 2465.62] So it is on my to-do list.
[2465.90 → 2466.86] I will get there.
[2467.06 → 2467.16] Yeah.
[2467.18 → 2471.40] What they kind of focus on orchestrating and running container workloads on embedded devices
[2471.40 → 2473.36] and have systems to manage that.
[2473.52 → 2477.72] Just running Kubernetes at home, you know, like, well, funnily enough, we were talking
[2477.72 → 2479.24] to someone about this at scale earlier today.
[2479.24 → 2479.28] Right.
[2479.54 → 2485.70] And it's just, yeah, unless someone's paying me to go through that pain, I know this is
[2485.70 → 2489.52] such a weird thing because we were just literally five minutes ago talking about how we love to
[2489.52 → 2489.78] tinker.
[2490.42 → 2495.22] Like there's just certain levels of generation that I just cannot be bothered with.
[2495.48 → 2499.16] And Kubernetes, like I've used it every day at work for like the last five, six, seven
[2499.16 → 2499.40] years.
[2499.42 → 2503.76] Like I'm very familiar with it and I understand a lot, a lot that can go wrong with it.
[2503.76 → 2507.30] And I think that puts me off it in a home server situation, to be honest.
[2507.30 → 2507.74] Hmm.
[2508.26 → 2511.82] I could see maybe not wanting to use it too, if you'd stopped using it day to day, you
[2511.82 → 2512.50] know, might be one thing.
[2512.64 → 2515.32] If you're enjoying it, you use it, you're deploying with it at work all the time and
[2515.32 → 2516.06] trying to learn.
[2516.18 → 2516.40] Yeah.
[2516.46 → 2516.64] Right.
[2516.70 → 2517.78] Trying to learn, come up with it.
[2517.88 → 2522.56] But particularly for most of my use cases, which is, you know, media apps, for example,
[2522.56 → 2525.84] that need ungodly amounts of storage underneath them.
[2526.66 → 2530.50] Those storage requirements are tied to a specific host.
[2530.62 → 2535.36] It's not like I have three GPUs across three hosts where I can run these Llama models across
[2535.36 → 2538.38] different hosts and I don't care about my completely stateless workload.
[2538.48 → 2539.72] That's not the world I live in.
[2540.14 → 2545.16] My apps are state full, and they have a lot of state in terms of a Jellyfin library or
[2545.16 → 2545.72] whatever it is.
[2546.22 → 2550.54] And so the idea of moving a container from one host to another, well, now I've got to
[2550.54 → 2554.02] set up replicated storage and buy three servers worth of disks.
[2554.36 → 2554.80] And yeah.
[2555.26 → 2555.36] Right.
[2555.56 → 2555.88] Yeah.
[2556.30 → 2559.30] It's one thing when you think you're enabling like a totally separate team in your organization
[2559.30 → 2560.86] to do stuff without talking to you.
[2560.86 → 2564.12] And another one, you have very specific and non-dynamic workloads.
[2564.56 → 2564.68] Yeah.
[2564.78 → 2566.72] I mean, we were talking about this again earlier.
[2566.90 → 2572.66] The benefit of Kubernetes in the workplace is it becomes a standard API for people to learn,
[2573.02 → 2575.00] humans to learn, to interface with infrastructure.
[2575.76 → 2577.52] Don't need that in my home lab.
[2577.78 → 2578.04] Sorry.
[2578.84 → 2580.36] It will all become one with Nix.
[2581.82 → 2583.26] But hey, I guess more power to you.
[2583.34 → 2586.82] I mean, if you enjoy it, and you make works well, that's a powerful system for sure.
[2586.98 → 2588.22] Definitely a good skill to have too.
[2588.22 → 2595.00] So iMac comes in with 20,000 sets, $2,000 for five years works out to be about $33 per
[2595.00 → 2595.40] month.
[2595.56 → 2599.42] If you include electricity and compare the available compute power with public cloud offerings,
[2599.64 → 2601.00] I think that's actually super cheap.
[2601.60 → 2603.92] So that's a pretty good practical way to look at it.
[2604.02 → 2607.16] I was kind of just musing on 2,000 seems like a reasonable.
[2607.38 → 2607.66] Yeah.
[2607.72 → 2610.22] And you break it down, and you include electricity in there on average.
[2610.58 → 2614.26] And then you think, what would it cost you to have a really nice VPS?
[2615.10 → 2615.36] Yeah.
[2615.42 → 2616.82] I think that's a good way to look at it.
[2616.82 → 2621.80] Well, according to this very rudimentary back of napkin, electricity math I've just
[2621.80 → 2626.32] done, 200 watts power consumption at 12 cents a kilowatt-hour, which is what I pay in North
[2626.32 → 2628.28] Carolina, not including my solar.
[2628.60 → 2630.72] So, you know, it's not a perfect thing.
[2630.76 → 2632.54] It's about $200 a year in electricity.
[2633.34 → 2638.82] So, you know, you could pay easily that for a very much less powerful VPS.
[2639.10 → 2639.22] Yeah.
[2639.28 → 2640.26] And probably wouldn't have a GPU.
[2641.12 → 2641.36] Yeah.
[2641.54 → 2643.38] That alone, lots of NVMe storage.
[2643.56 → 2643.70] Right.
[2643.70 → 2647.94] And be on your LAN and fast and private and available when your internet's down.
[2648.36 → 2650.54] And maybe this isn't a perk, but you get to be the network admin.
[2650.74 → 2651.74] You set the policies.
[2652.24 → 2652.40] Yeah.
[2652.46 → 2654.18] And that's worth a premium right there, too.
[2654.30 → 2656.02] I can put Kubernetes on it whenever I want.
[2656.14 → 2656.60] That's right.
[2657.68 → 2658.26] All right.
[2658.26 → 2660.46] Difficulty adjustments, our last booster this week.
[2660.52 → 2661.64] 10,000 SATs.
[2662.02 → 2662.80] Great show, guys.
[2662.88 → 2666.38] Love the discussion about the beefier home rigs and building sovereign censorship resistant
[2666.38 → 2666.72] AI.
[2667.30 → 2672.22] If anyone is interested in combining self-hosting Bitcoin, NixOS, and AI, take a look at the
[2672.22 → 2678.30] AI agent that autonomously pays and receives on lightning through HTTP 402 messages.
[2678.92 → 2682.60] I'm new to this and haven't built it myself, but it's a key goal I'm working towards.
[2683.68 → 2684.00] Wow.
[2684.00 → 2686.58] Did this guy just listen to the latest UP episode or something?
[2687.24 → 2687.90] Yeah, maybe.
[2688.02 → 2689.72] We did get into Nix Bitcoin in the latest UP.
[2689.84 → 2690.08] It is.
[2690.46 → 2695.50] And that was such a cool project to get into because it really shows you, at least in my
[2695.50 → 2698.96] opinion, the future of the community collaborating and sharing server builds.
[2699.52 → 2700.90] I just think that's going to be huge.
[2701.12 → 2706.46] Like, you know, you could see a future where the perfect media server is mostly just a series
[2706.46 → 2708.00] of Nix modules and just...
[2708.00 → 2709.94] Well, I can't talk about it on air yet.
[2710.12 → 2710.28] Oh?
[2710.86 → 2715.18] But I do have a very interesting proposition for you both.
[2715.60 → 2719.06] I've been working with a friend of mine on some stuff behind the scenes, which we will
[2719.06 → 2721.24] talk about publicly in the show soon enough.
[2721.58 → 2726.02] But essentially, it's going to be using the power of Nix underneath to declaratively deploy
[2726.02 → 2727.34] these modules, these apps.
[2727.76 → 2729.32] And there's going to be a lot of tooling around it.
[2729.40 → 2733.42] So eventually, there'll be like a website you can go to, you know, like Finite or something
[2733.42 → 2735.64] for Windows where you can just check the boxes and say, I want Plex.
[2735.64 → 2736.82] I want blah, blah, blah.
[2737.46 → 2738.44] It will deploy all that.
[2738.52 → 2741.72] You'll fill in your app data, like paths and stuff, and it'll just work.
[2742.14 → 2742.80] That's going to be neat.
[2742.94 → 2743.82] That sounds slick.
[2744.38 → 2744.58] Yeah.
[2744.68 → 2746.08] And that's going to make it really approachable.
[2746.66 → 2749.28] Now all we need is people to add things like Image and Airspeed.
[2749.28 → 2749.56] Yeah.
[2749.76 → 2754.28] All the apps that are missing from Nix packages for our server apps, we just need a bunch of
[2754.28 → 2755.72] you guys to go and do that for us.
[2755.74 → 2757.18] And then we'll be good to go.
[2757.26 → 2757.82] Thank you.
[2758.34 → 2760.22] Also, thank you everybody who did boost in.
[2760.32 → 2761.28] We had four boosters.
[2761.28 → 2765.44] Not a big boost batch, but we stacked 84,845 SATs.
[2765.64 → 2769.10] And we'd love to have you boost in too and support this production by getting a new podcast
[2769.10 → 2771.12] app like fountain.fm.
[2771.48 → 2775.70] More reasons than ever, because we're rolling out new features across the network shows and
[2775.70 → 2777.34] you get those in the podcasting 2.0 apps.
[2777.72 → 2782.76] And you can support each production either by boosting or by becoming an SRE at self-hosted. Show
[2782.76 → 2784.18] slash SRE.
[2784.54 → 2787.70] Support the show and get an ad free feed with a post show extra.
[2788.46 → 2789.60] We appreciate all of you.
[2789.60 → 2793.34] Now, as this airs, of course, scale was last weekend, but that doesn't mean that conference
[2793.34 → 2795.62] season is anywhere close to being finished.
[2796.06 → 2801.30] Meetup.com slash Jupiter Broadcasting is where they go to find out all the latest meet
[2801.30 → 2805.82] and greets and all the rest of it from anywhere from Austin right the way up to Seattle over
[2805.82 → 2806.54] the next few weeks.
[2806.76 → 2807.12] Mm hmm.
[2807.28 → 2807.68] Crazy.
[2808.48 → 2808.84] Crazy.
[2809.20 → 2811.68] In fact, also, there's DevOps Days in Raleigh that I'm doing.
[2811.98 → 2812.34] So, are you?
[2812.34 → 2814.32] Perhaps I should do some kind of.
[2814.68 → 2815.50] Yeah, let's do that.
[2815.62 → 2818.80] We'll do some kind of JB meetup in Raleigh, and I'll get Tale scaled by some.
[2818.82 → 2822.54] I might be able to talk Was into doing a lunch in Denver at Red Hat Summit.
[2822.80 → 2823.36] Oh, that'd be fun.
[2823.52 → 2823.70] Yeah.
[2823.82 → 2826.30] So if people are going to be Red Hat Summit, find Was and I.
[2826.44 → 2826.70] Nice.
[2827.20 → 2827.66] There you go.
[2827.74 → 2828.56] Things going on.
[2828.70 → 2829.20] Yeah, man.
[2829.30 → 2829.68] I'll tell you.
[2830.28 → 2834.52] So you will know by now, but self-hosted. Show slash contact is the place to go to get in touch
[2834.52 → 2834.84] with us.
[2834.98 → 2838.12] You can find me online at alex.ktz.me.
[2838.82 → 2840.38] I'm chrislas.com.
[2840.38 → 2843.04] Find me over at linuxunplugged.com.
[2843.34 → 2844.38] Well, thanks for listening, everyone.
[2844.52 → 2847.62] That was self-hosted. Show slash 119.
