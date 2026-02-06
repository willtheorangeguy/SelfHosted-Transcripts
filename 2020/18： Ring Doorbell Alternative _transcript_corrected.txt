[0.00 → 6.10] Coming up on this week's show, we discuss how listener Morgan was almost outsmarted by a not-so-smart doorbell,
[6.60 → 13.70] Jellyfin makes Alex's prediction dreams come true, and I try out TO notes again.
[14.48 → 14.96] I'm Chris.
[15.36 → 17.56] And I'm Alex, and this is episode 18.
[18.58 → 23.78] Well, Chris, I went and did it. I bought myself a smoker. My Americanization is complete.
[24.08 → 29.58] This truly is the completion of a journey that has been a multi-year journey.
[29.58 → 32.04] I'm so, so proud of you, Alex.
[32.24 → 36.88] The culmination reminds me of that American Pie moment. You remember where the coach is on the field?
[37.88 → 41.16] I don't want to take this from you, but Alex, you know, you got to automate this.
[41.26 → 44.74] We got to integrate this somehow into Grafana. I got expectations.
[45.26 → 45.92] You know it's coming.
[47.08 → 51.38] Will you? I want to see average cook time built into Grafana, something like that.
[51.44 → 55.18] What about average temperatures that you use? I want all the data.
[55.18 → 58.92] The average temperature per probe, I think, is really the sweet spot.
[59.34 → 61.98] Per probe? How many probes are we talking about?
[62.42 → 65.24] I don't know. This sounds like an episode of South Park, doesn't it?
[65.60 → 67.72] Where Cartman's getting probed or something.
[67.96 → 72.02] But I don't know, like four? Four probes is a good number of probes?
[72.18 → 74.00] Have you looked into it, though, the possibilities?
[74.00 → 78.94] What I have, and actually joining us on the show this week, is a friend and colleague of mine, Morgan Peter man.
[79.10 → 80.48] He works with me at Red Hat.
[81.16 → 86.42] He's a technical account manager working on OpenShift, and he has an extensive home lab.
[86.88 → 92.40] And he was the benefactor of a certain doorbell that you ordered, Chris, without researching it properly.
[93.24 → 95.88] Yeah, during the show, actually, I ordered a smart doorbell.
[96.02 → 99.00] So, Morgan, it's great to have you here. And how has my doorbell turned out?
[99.44 → 100.58] Thank you so much for having me.
[100.58 → 107.88] Yeah, the doorbell actually worked out pretty good once I finally got it set up, wired properly, and connected running on Shinobi.
[108.52 → 113.76] It's a little difficult, especially if you watch their YouTube video, and then you see that they use one application.
[114.14 → 117.48] And then you go to their website, and they recommend a completely different application.
[118.10 → 120.48] So, that was a lot of the hassles that I went through.
[120.98 → 123.92] I spent quite a bit of time using the Easy Viz app.
[124.48 → 129.88] You know, it's standard, scan the QR code, it connects to the Wi-Fi in ad hoc mode.
[129.88 → 134.46] And it's supposed to work. Connect, configure Wi-Fi, and then you get your video.
[135.10 → 135.96] And it didn't do that.
[136.26 → 142.52] I had a series of texts that were getting progressively more and more frustrated over the course of, what, six hours you were installing this thing?
[142.84 → 144.94] Yes, it took a couple of hours to get it working.
[145.66 → 148.80] I replaced the transformer because I didn't know if it was a power issue.
[149.46 → 151.82] I changed the wiring, cleaned up some terminals.
[151.82 → 157.28] And in the end, it just came down to the fact that the application was just awful.
[157.82 → 163.16] So, I went to the website, and I found out that they offer a batch configuration tool.
[163.38 → 171.04] So, I downloaded the batch configuration tool, put it on the Mac, loaded it up, found the camera, and I couldn't configure it.
[171.04 → 178.52] So, then became the hunt to find a Windows machine in my house that I could actually tolerate long enough to get the batch tool on.
[178.88 → 180.06] Oh, my goodness.
[180.56 → 181.80] That was the easiest for me.
[182.04 → 188.12] You know, again, there's Easy Viz, Guardian Vision, and then there's their actual batch tool.
[188.68 → 191.42] The Easy Viz did not work at all.
[191.62 → 193.44] It just could not connect, couldn't configure.
[193.44 → 198.74] And this is after I created a new SSID, just something simple.
[198.92 → 200.84] I called it IoT with a password to password.
[201.04 → 201.80] Still couldn't connect.
[202.46 → 204.24] Guardian Vision wasn't working at all for me.
[204.34 → 205.84] And it ended up using the batch tool.
[205.90 → 206.78] The batch tool was great.
[206.90 → 207.48] I found it.
[207.94 → 210.44] It's GUI-based, you know, on Windows.
[210.62 → 212.64] You configure the SSID and the password.
[212.86 → 213.84] And it connected instantly.
[214.16 → 215.36] And I was up and running.
[215.90 → 217.82] And then I found out that my doorbell didn't work.
[218.28 → 221.38] Had to go over to Home Depot, stood in line for about an hour to get into Home Depot.
[221.38 → 223.54] So came home, hooked up the doorbell.
[224.00 → 229.14] And then it was a fun game of picking which one of the 16 songs we wanted to hear whenever the doorbell rang.
[229.46 → 232.32] Does this thing trigger a built-in doorbell that's in the house already?
[232.36 → 234.30] So if you had something installed, it'll trigger that?
[234.56 → 234.84] Yeah.
[234.90 → 238.10] So what I found out was my old mechanical doorbell was actually broken.
[238.34 → 239.58] One of the springs had popped.
[240.12 → 241.84] And it just wasn't worth trying to repair it.
[242.32 → 243.86] So I had two options.
[243.86 → 249.20] I had a regular mechanical-style doorbell or the 16-song doorbell.
[249.20 → 251.94] It's standard off-the-shelf from Home Depot.
[252.38 → 256.28] Came home, wired it inside the Easy Viz app, which is what you want to use.
[256.54 → 258.14] After you get it configured, that's very important.
[258.64 → 263.62] After you get it configured, you want to keep the Easy Viz app because it is the best app of the two that they recommend.
[264.44 → 265.58] You just go into the settings.
[266.16 → 266.84] You configure it.
[266.90 → 270.44] You tell it you have an electronic doorbell.
[270.98 → 271.66] And then you're set.
[271.96 → 273.56] So whenever you come up, you push the button.
[273.76 → 274.40] Your doorbell rings.
[274.40 → 278.76] And what's nice is you can configure it if you want it to be two seconds or 10 seconds.
[278.92 → 280.38] You have configuration options.
[280.84 → 291.24] Just to be clear, does it require like an account or a service, any kind of login that you have to go into a service to get this thing to be configured or functional or anything you have to pay for?
[291.60 → 296.26] So no, you do not need to sign up for an account to get it to configure it.
[296.34 → 300.60] You can download the batch program, the batch tool off of their website, and you can get it configured.
[300.60 → 306.18] But if you want to use the Easy Viz app, for what I found, you do have to log in.
[306.28 → 308.04] So I use my standard Google account.
[308.66 → 311.32] And if you're an iPhone user, which I am, you definitely want it.
[311.48 → 314.24] When somebody comes up and rings my doorbell, I get a phone call.
[314.58 → 316.64] I answer the phone call, and it's audio.
[316.94 → 320.08] You hit the Easy Viz button, and then it does video.
[320.24 → 322.66] So I can actually see them, and I can talk to them.
[322.86 → 323.80] And it's a great app.
[324.18 → 329.06] It's not 100% self-hosted, but it's a good option that they give you.
[329.06 → 332.86] So I also configured Shinobi.
[333.46 → 335.46] It's view only or watch only.
[335.66 → 337.70] I configured my motion detection.
[338.42 → 346.20] And I had to toggle a little bit with the audio detection because it was too low, and crickets were setting off the recording.
[346.84 → 349.02] And then obviously, if you set it too high, it doesn't pick anything up.
[350.08 → 351.96] So again, I used Shinobi.
[352.08 → 352.76] I got it set up.
[352.86 → 353.58] I got it recording.
[354.20 → 357.66] I caught myself mowing the lawn, picking up the grass.
[357.66 → 362.88] My neighbour at 8.30 in the morning, revving his motorcycle, wanting to wake everybody else up.
[363.22 → 364.60] So it works great with Shinobi.
[365.08 → 366.46] I was really happy with it.
[366.54 → 368.82] And that actually didn't take very long to get set up.
[369.32 → 369.40] All right.
[369.42 → 375.64] And to be clear, we're talking about the Nelly's security camera that was on Amazon for around $130.
[376.06 → 378.52] It's currently not available, but there are different iterations of it.
[378.62 → 382.04] I bought this back in January while we were recording the show.
[382.04 → 385.96] And I had a sense it was a project, and so I just kept putting it off.
[386.04 → 388.10] And then I realized I didn't have the proper wiring.
[388.74 → 390.40] So Alex suggested we ship it to Morgan.
[390.58 → 393.30] And so Morgan did all of this testing, did the whole installation.
[393.42 → 398.90] But the one thing we haven't asked you about on this Nelly security camera is how's the picture quality?
[398.94 → 403.90] Does it actually do the job and give you a clear picture of what's going on around your porch?
[404.38 → 405.68] So the picture is actually really nice.
[405.68 → 409.48] I took some videos and I sent it to Alex so he could see, and it was super clear.
[410.06 → 414.98] One of the issues I did have with it is its more of a fisheye style lens.
[415.60 → 417.22] And they advertise this as a feature.
[417.36 → 420.34] So you get the full height of the individual standing in front of the camera.
[420.82 → 423.52] But that also distorts the image just a little bit.
[423.98 → 428.24] So for example, if you're a little big around the belly, you're going to look a lot bigger in the video.
[428.48 → 430.38] But the picture is crystal clear.
[430.54 → 432.08] The audio is actually really amazing.
[432.08 → 438.38] I was quite surprised how well it picks up audio, especially for conversations if you're not standing directly in front of the camera.
[439.02 → 445.40] For $139, I would definitely recommend it to any individual who's looking for a good camera.
[445.66 → 450.86] You want to get out of the Ring, you know, or one of the ones that maybe comes with Comcast, etc.
[451.22 → 452.72] Have you tried the Ring doorbell?
[453.24 → 454.48] How does it compare to that?
[454.74 → 458.18] So I had the Ring doorbell when I purchased this house.
[458.38 → 460.18] And it was transferred over to me.
[460.18 → 463.64] My big issue was the fact that I was paying monthly for it.
[464.24 → 465.84] You know, there are some features that Ring has.
[465.90 → 466.58] It's really nice.
[466.90 → 469.72] But I didn't like the idea of a reoccurring monthly payment.
[470.12 → 472.76] And as you guys know, monthly payments always go up.
[473.06 → 474.18] Every year they adjust it.
[474.46 → 477.54] And the total cost of ownership for these doorbells just skyrocket.
[478.12 → 480.32] On top of that, it didn't look very good.
[480.66 → 482.16] That's such a 2020 sentence.
[482.44 → 485.26] The total cost of ownership of this doorbell.
[485.86 → 486.52] Oh my goodness.
[486.52 → 486.88] It is.
[486.88 → 491.32] Yeah, unfortunately, you're right.
[491.92 → 495.94] And the fact that we're even considering, does your doorbell have a subscription service?
[496.54 → 501.72] One of the upsides that I really liked about the Nelly was the fact that it's hardwired.
[502.06 → 503.72] You don't have to worry about a battery.
[504.12 → 508.60] You know, I know people that bought rings, and then they were charging their doorbell battery
[508.60 → 510.36] every couple of days, which is ridiculous.
[511.16 → 513.32] You know, the Nelly is hardwired, which is nice.
[513.32 → 515.24] It doesn't offer a battery, as Chris, you know.
[516.02 → 519.92] The downside to it, though, and this is something I mentioned to Alex, it does get very hot.
[520.50 → 524.80] Whenever I was just plugging it in just to test it, it got to the point where I couldn't
[524.80 → 527.54] hold it for more than a couple seconds to the point where it could burn me.
[528.00 → 532.36] I don't know if this is going to affect overall longevity of the device, but you definitely
[532.36 → 533.72] don't feel it if you touch it.
[533.86 → 536.46] It's only the back where the camera and the electronics are.
[536.46 → 541.74] But that is something to consider, obviously, you know, is longevity is how is the heat going
[541.74 → 544.42] to affect this device over multiple years?
[545.08 → 548.76] Particularly for you down in Florida, where it's, you know, hot always.
[549.20 → 555.30] So you now have it going into Shinobi and then in there you're using the plug-in system to
[555.30 → 556.32] do motion capture.
[556.46 → 560.84] So it's only, it's always streaming, but it's only recording when there's motion capture.
[560.84 → 561.86] That's correct.
[562.04 → 568.18] And then what's really great since it uses RTSP, I have VLC running at all times, especially
[568.18 → 570.56] when I'm expecting an Amazon package.
[570.82 → 576.34] Because what I've noticed is Shinobi doesn't pick up the real quick toss of the box that
[576.34 → 577.76] most Amazon deliveries do.
[578.30 → 580.12] You know, UPS and FedEx are really nice.
[580.20 → 584.74] They seem to always ring my doorbell, but I get Amazon who stands just outside the view
[584.74 → 588.68] of the camera, and they toss it on my porch.
[588.68 → 593.60] So with VLC having it streaming at all time, I can see that nice camera land.
[593.80 → 594.78] Same thing with Amazon.
[594.90 → 596.44] I can see the Amazon truck drive by.
[596.82 → 598.02] And the video stays connected.
[598.12 → 598.70] It doesn't drop.
[598.86 → 600.02] Yeah, I haven't had any issues.
[600.16 → 604.00] I've actually had it running for two days straight without even realizing I had it connected.
[604.26 → 605.82] And it doesn't use a lot of video.
[606.00 → 610.08] I use Unify to track how much data it uses, and it's not very high.
[610.66 → 610.88] Cool.
[611.74 → 615.90] I mean, so it sounds like if you're willing to wire it, and you're willing to deal with some
[615.90 → 621.02] half-baked apps for some of the initial setup and configuration changes, which can be sounds
[621.02 → 622.18] like a little frustrating.
[622.44 → 628.00] The end result is you still have something you can RTSP stream on your LAN without any
[628.00 → 628.92] cloud service required.
[629.28 → 632.40] And what happens if Nelly go away?
[632.62 → 636.04] Because you found some, you know, generic clones of this thing, right?
[636.04 → 640.28] The only difference between every other one of these clones and Nelly is the fact that
[640.28 → 641.04] Nelly sells it.
[641.44 → 645.56] There are some comments on the internet that they run different firmware.
[646.06 → 651.24] But from what I can tell, all it is a clone of the Easy Viz camera.
[651.50 → 653.52] And that's why you use the Easy Viz application.
[654.22 → 656.74] So if Nelly goes away, the only thing you lose is support.
[657.44 → 660.30] What's great is it's not necessarily connected to a cloud.
[660.46 → 663.30] They give you instructions how to remove it from being connected to the cloud.
[663.30 → 669.38] So you can set this up with the batch tool, never connected to the cloud and use Home
[669.38 → 669.72] Assistant.
[670.06 → 670.96] You can use Shinobi.
[671.66 → 673.70] I'm sure Blue Iris would work as well.
[674.30 → 675.18] And that's what's great.
[675.28 → 678.26] And it stores everything right on that SD card.
[678.40 → 686.84] So if you're not streaming it to a, you know, a DVR or an NVR, you can still pull out, you
[686.84 → 691.84] know, the Guardian Vision app and view the data without ever logging into anything.
[691.84 → 697.26] Morgan, I'm sure you didn't do a full penetration test analysis, but did you get a sense of what
[697.26 → 699.82] the security is like on this thing if you're comfortable with it?
[700.20 → 704.70] So one of the things I actually did do was I completely disabled it, internet access.
[705.04 → 706.42] So it could not go out.
[706.56 → 711.10] I set it up so it had no internet access, and it still worked great internally in my LAN.
[711.62 → 716.40] Now, obviously, the phone home version of the Easy Viz application wasn't working,
[716.40 → 718.96] but Shinobi still worked.
[719.34 → 720.42] RTSP still worked.
[720.76 → 727.06] I was still getting alerts through those applications, but the Easy Viz application wasn't working.
[727.64 → 727.72] Right.
[727.80 → 731.96] So then I guess that would mean you wouldn't get the push notification video sent to your
[731.96 → 733.16] phone if somebody was at the door.
[733.64 → 733.96] Correct.
[734.20 → 734.46] Correct.
[735.08 → 739.50] But you could still have the VLC stream up watching the door all the time, and it could be
[739.50 → 741.22] over your LAN, no cloud service required.
[741.42 → 742.70] So that checks my box.
[742.70 → 749.08] One of the other options is Motion Eye and Home Assistant, which was shared with me by Alex.
[749.58 → 751.24] I did not get a chance to set it up yet.
[751.32 → 752.24] That's my next project.
[752.68 → 757.34] But to get alerts via Telegram bot or a Discord bot.
[757.60 → 761.64] So there are options out there where you can set up an alerting service.
[762.58 → 767.42] Again, since this is a doorbell app, I would keep it available to the internet just for the
[767.42 → 772.60] Easy Viz application because I want to be able to answer the phone from my couch.
[772.60 → 774.78] Or from my bed and see who's there.
[775.06 → 775.22] Right.
[775.30 → 778.32] I don't want to get a video sent to me that may be delayed.
[778.86 → 780.14] It's nice to have a communication.
[780.56 → 786.16] And we actually use that on Sunday morning whenever a, you know, the Jehovah Witnesses
[786.16 → 786.66] came by.
[786.98 → 787.88] Thanks, but no, thanks.
[787.92 → 788.58] Have a great time.
[788.84 → 793.10] It was a lot better than waiting for a notification on the phone than viewing the video to see
[793.10 → 793.70] who it was.
[794.28 → 794.78] Yeah, absolutely.
[795.02 → 795.16] Yeah.
[795.20 → 798.80] The real time when someone's at the door like that really makes a difference.
[798.80 → 803.46] And that does seem like a great way to politely say thank you, but no, thank you and not get
[803.46 → 804.54] stuck in a conversation.
[805.02 → 806.64] I just blame coronavirus these days.
[807.98 → 809.02] That's the general go-to.
[811.24 → 815.62] Well, Morgan, I'm really glad that we sent it your way so that way you could give us the
[815.62 → 816.32] full test on it.
[816.36 → 820.82] And it sounds like if I could have wired it in, which I couldn't do in Lady Joop's, but
[820.82 → 824.34] I could have essentially gotten the functionality I was looking for.
[824.34 → 828.96] So I'm going to keep an eye on this category because if they make one with a battery, that
[828.96 → 830.22] could be the route I would go.
[830.62 → 831.00] Yeah, I agree.
[831.16 → 832.50] Like I said, it's a great application.
[832.76 → 833.02] Thank you.
[833.12 → 836.78] I really appreciate you giving me the opportunity to test it out for you.
[837.50 → 843.26] Now, before we let you go, Morgan, you have an embarrassing data loss story you want to
[843.26 → 844.32] share with the class, don't you?
[844.66 → 845.24] Oh, no.
[845.74 → 847.34] As Alex mentioned, I am a Red Hatter.
[847.82 → 852.48] And one of the great options that Red Hat gives you is the ability to install the full
[852.48 → 852.88] stack.
[852.88 → 855.20] And I love home jabbing.
[856.12 → 859.42] And as a home lubber, you should really practice good backups.
[859.80 → 863.94] Because if you're supposed to be replicating what you do at home for what you do at work,
[864.24 → 865.76] you should practice what you preach.
[866.06 → 871.36] I unfortunately ran afoul of that this weekend, installing some new SSD drives.
[871.72 → 872.04] Uh-oh.
[872.94 → 879.22] Popped open the home lab, installed some SSD drives, configured the RAID, and I initialized
[879.22 → 880.96] the wrong RAID array.
[880.96 → 883.02] System reboots.
[883.74 → 885.10] Can't connect to venter.
[885.48 → 887.42] Can't connect to my VMs.
[888.18 → 890.14] Log into the ESXi hosts.
[890.86 → 894.74] And all my VMs just have VM-number, and they're all gone.
[895.06 → 895.84] Oh, no.
[895.84 → 900.70] And then I realized instantly what I did, that I just wiped out all of my data.
[901.32 → 902.70] How awful did that feel?
[902.82 → 903.26] Jeez.
[903.52 → 908.52] But it's okay, Morgan, because you and I were talking, and you wrote loads of automation
[908.52 → 909.64] to rebuild this stuff, right?
[909.64 → 910.66] And you put it in Git.
[911.12 → 912.18] It was fine, right?
[912.18 → 919.02] Alex has been hounding me to document the entire process, to automate everything.
[919.46 → 920.68] And I took his word for it.
[921.02 → 921.74] I love Ansible.
[922.08 → 922.90] Ansible's a great tool.
[923.36 → 929.40] And I wrote thousands of lines of Ansible playbooks to replicate my entire environment
[929.40 → 935.46] outside of ESXi and venter to the point where I actually deleted a bunch of my VMs and I
[935.46 → 936.06] redeployed them.
[937.40 → 942.16] Unfortunately, that was in my GitLab server, which was on my home lab that I erased.
[943.84 → 947.46] I mean, I'll be honest, I laughed pretty hard when he told me the story the first time.
[947.84 → 948.76] Yeah, because it's not you.
[949.04 → 949.44] Yeah.
[949.54 → 950.46] I mean, I've done that.
[950.78 → 954.38] I've wiped out three terabytes worth of stuff numerous times.
[954.70 → 957.92] Boy, but wiping out data and the VMs is like a double blow.
[957.92 → 963.26] But I've never not had my configuration in GitHub as opposed to a local GitLab.
[963.56 → 964.48] Yes, I learned.
[964.48 → 968.84] So once I redo all that work, it'll all be stored externally.
[969.66 → 971.10] So a nice little tip for you.
[971.32 → 979.00] If you've heard of Gift, that is a self-hosted local GitHub server clone thing.
[979.76 → 986.10] And Gift will automatically clone any commits you make to GitHub.
[986.64 → 992.42] So I have a local copy of all of my GitHub stuff is locally saved by Gift.
[992.42 → 996.46] Now, the motivation for that was, what if they get bought out by some evil company?
[996.78 → 998.42] Oh, wait, they maybe did.
[999.20 → 1001.06] What if they did something crazy with my data?
[1001.30 → 1003.44] But obviously, the same is true in both directions.
[1003.44 → 1011.36] If I accidentally initialize the wrong SSD array and wipe my local Git server, it's all
[1011.36 → 1012.02] in GitHub too.
[1012.02 → 1016.14] Yeah, so I spent Saturday night rebuilding the most important VMs.
[1016.66 → 1019.80] And I'm sure, sadly, it won't be the last time I accidentally delete everything.
[1020.28 → 1024.44] But I'll make sure that this will be the last time I delete everything without proper backups.
[1024.88 → 1028.36] So your postmortem is off-site, off-site, off-site.
[1028.80 → 1029.92] Do you know what you're going to use?
[1029.92 → 1031.64] I have not looked into it yet.
[1032.58 → 1035.10] Back blaze is obviously one that I do like.
[1035.44 → 1036.78] You know, unlimited storage.
[1037.20 → 1041.44] The downside of I've used it before, and it does take a long time to pull everything down.
[1041.86 → 1043.64] You've got gigabit symmetrical internet, though.
[1043.72 → 1047.78] So, you know, the actual upload part, which is normally the problem, you've got that licked.
[1048.08 → 1050.34] Yeah, I have symmetrical one gig, so it's pretty nice.
[1050.60 → 1056.14] But most likely what I'm going to do is write some scripts using PowerShell that'll export
[1056.14 → 1061.48] the VMD case, except for, you know, the things that I can easily download quickly.
[1062.38 → 1068.28] And then I'll just zip those up and send them up to Back blaze and just have that like on a 24,
[1068.42 → 1069.54] every 24 hours that'll go.
[1070.14 → 1073.62] That's what I actually used to do in my previous job is a site consultant.
[1074.04 → 1076.86] But, you know, as I said, you're supposed to practice what you preach.
[1077.04 → 1079.30] And very rarely do we practice what we preach.
[1079.46 → 1081.60] And we end up, you know, with egg on our face.
[1082.16 → 1082.94] Amen to that.
[1083.22 → 1084.62] Well, thanks for joining us, Morgan.
[1084.62 → 1085.62] That was a lot of fun.
[1086.02 → 1088.40] And I'll see what other free stuff I can get you in the future.
[1089.08 → 1089.44] Pleasure.
[1089.66 → 1090.28] Thanks a lot, guys.
[1090.50 → 1090.94] Have a good one.
[1091.04 → 1091.62] Thanks, Morgan.
[1091.90 → 1094.18] I have a data loss story of my own this week.
[1094.28 → 1097.06] It's not quite my fault, although it could be.
[1097.32 → 1098.26] I'm not sure if it is, though.
[1098.62 → 1104.04] I was using Joplin, and I've started work on the 2020 version of Perfect Media Server.
[1105.42 → 1109.60] And I was writing away one evening for about three or four hours and I went to bed.
[1109.72 → 1113.44] I'd just finished a huge section, which I was really pleased with.
[1113.44 → 1117.20] And I thought I'd gone through, and I'd proofread it, and I'd edited it, and I'd tweaked it.
[1117.24 → 1119.08] And it was, I was really happy with it.
[1119.72 → 1122.94] And I came back in the morning to my desktop, and it was gone.
[1123.32 → 1123.56] Gone.
[1123.94 → 1127.18] I was just like, what the hell has happened here?
[1127.18 → 1133.64] And it turns out that Joplin had decided that the version of the note that was on the server
[1133.64 → 1137.00] was more important than the version of the note that I'd just edited.
[1137.44 → 1138.64] And I overwrote it.
[1139.02 → 1139.50] Mm-hmm.
[1139.50 → 1146.48] Then I started going to try and look through the SQLite database that Joplin has, and it's gone.
[1146.64 → 1147.08] It's too late.
[1147.48 → 1147.88] It's dead.
[1148.12 → 1148.42] Wow.
[1148.80 → 1154.58] So you and I were talking about notes and I think Joplin, unfortunately, it was so close.
[1154.66 → 1155.36] It was perfect.
[1155.42 → 1156.70] It's been working well for about a month.
[1157.50 → 1159.42] But you found an alternative for me.
[1159.86 → 1160.02] Yeah.
[1160.10 → 1162.54] You know, funny enough, it's one that you and I have used before.
[1162.54 → 1166.64] Um, but I just, I kept coming back to it.
[1166.76 → 1168.42] And so I wanted to share it with the class.
[1168.62 → 1170.08] It's, it's a classic.
[1170.16 → 1171.84] It's Q own notes.
[1172.08 → 1177.90] And I think it holds up to be the biggest and best contender to Evernote that I can find.
[1178.18 → 1180.96] There are a couple of fundamentals that I really like about it.
[1181.66 → 1186.52] Number one, all the notes are stored in plain text files, markdown files.
[1186.74 → 1189.12] You can just go cat them on the command line.
[1189.38 → 1192.32] You can also, you can put notes in multiple folders.
[1192.32 → 1197.62] So you can have them one and Dropbox one on your local file system, one on sync thing,
[1197.68 → 1198.68] another one in next cloud.
[1198.76 → 1203.98] It also will use the own cloud next cloud API to actually take advantage of the notes in
[1203.98 → 1204.46] next cloud.
[1204.46 → 1208.52] If you have that, and then that gives you a web viewer for your notes, which is really
[1208.52 → 1208.78] nice.
[1208.82 → 1210.68] It can also integrate with some of the calendar stuff there.
[1211.10 → 1216.28] And then the one that you sounded like you were kind of excited about, this isn't something
[1216.28 → 1220.50] I've played with before, but I think I'm going to now is I realized it also supports
[1220.50 → 1221.42] get versioning.
[1221.42 → 1221.82] Yeah.
[1222.12 → 1222.94] That's a game changer.
[1223.26 → 1226.64] I mean, I use Git to version manage all of my code.
[1226.74 → 1228.60] So why not version manage all of my notes?
[1228.76 → 1234.50] And normally the process of doing a, you know, a Git adds, Git commit or whatever, every time
[1234.50 → 1238.02] I get to, you know, a new paragraph would be a bit too cumbersome.
[1238.38 → 1238.46] Sure.
[1238.46 → 1242.24] But TO notes seems to handle that for you on, on the most part.
[1242.60 → 1248.12] And, uh, I'd kind of written it off as being a bit ugly and a bit clunky, but I really started
[1248.12 → 1249.94] to dig through some of the menu settings today.
[1250.06 → 1251.00] You know, I was wrong.
[1251.00 → 1257.02] I think honestly, it's, it's a really great looking app and this speaks to a larger principle.
[1257.18 → 1261.14] I think you and I have been kind of circling around with notes for, for quite a while.
[1261.14 → 1261.50] Really.
[1261.50 → 1266.78] We're going to use next cloud to actually sync the notes between devices.
[1266.78 → 1272.40] So, you know, between an iPad and a Linux server and a MacBook and a, you know, an XPS, whatever
[1272.40 → 1275.92] running whatever flavour of Linux this week we're using.
[1275.92 → 1282.46] Um, we use next cloud to handle the sync and then on each system, I mean, TO notes runs
[1282.46 → 1287.18] on Mac windows and Linux, but on mobile, we can use whatever apps we want to edit those
[1287.18 → 1289.84] files where TO notes doesn't exist.
[1290.24 → 1293.98] And I think that's the key really is it's a bit like Wi-Fi really you're separating your
[1293.98 → 1296.30] firewall from your, uh, Wi-Fi.
[1296.30 → 1299.48] You're separating the sync of the notes from the editing of the notes.
[1299.48 → 1304.56] And I think hopefully, hopefully that's going to result in a really reliable, robust solution.
[1304.56 → 1306.10] I've been playing around with it.
[1306.10 → 1313.28] I have, uh, um, I, a writer on iOS on the iPad with the new keyboard and I use that to edit
[1313.28 → 1313.78] some notes.
[1313.78 → 1316.48] And then I go back to my desktop, and it's right there in TO notes.
[1316.74 → 1318.42] I really like that so far.
[1318.48 → 1319.42] It's worked really well.
[1319.74 → 1324.36] I do think maybe eventually I could see some sort of conflict, you know, maybe I have TO
[1324.36 → 1326.32] notes open, and I edit a Dropbox directly.
[1326.32 → 1329.08] So I'm going to wait and see how that plays.
[1329.18 → 1333.02] We'll see eventually if I create my own problem with that one or not.
[1333.02 → 1336.04] But so far it's, it's worked.
[1336.42 → 1340.04] And, uh, TO notes also has support for adding an external editor.
[1340.16 → 1344.80] So you can double-click a note, and now it opens in VS Code, which is my preferred Markdown
[1344.80 → 1345.06] editor.
[1345.72 → 1345.76] Really?
[1346.26 → 1347.66] Oh, didn't know that.
[1347.80 → 1348.32] Yeah.
[1348.80 → 1349.88] And it's pretty nice.
[1349.88 → 1354.14] Cause then if you have some more complex stuff or some just things that VS Code does that
[1354.14 → 1356.50] you want to do in your notes, really simple to do that now.
[1356.50 → 1362.70] And then the other little tip I'll pass along is if you rock a dark theme, like I do, if
[1362.70 → 1367.76] you play around in the settings for TO notes, it's not enabled by default, but they have
[1367.76 → 1369.80] a dark mode that they call it.
[1369.86 → 1372.84] And you can turn that on, and it just looks a lot better.
[1372.96 → 1374.56] It just simply, it just looks a lot better.
[1374.62 → 1377.38] But also if you're running a dark theme, it's more usable.
[1377.50 → 1379.76] Some of the stuff won't show up unless you turn that on.
[1380.18 → 1380.30] Yeah.
[1380.30 → 1382.54] It's, it's much better than I remember.
[1382.84 → 1387.02] I used it maybe was around the time I was emigrating, I think, cause that's when I was
[1387.02 → 1388.98] getting into next cloud big time for the first time.
[1389.38 → 1392.50] And then it just sort of faded away, and I stopped using it for some reason.
[1392.72 → 1392.88] Yeah.
[1393.20 → 1397.56] All the kind of controversy surrounding snaps at the moment, like I can't quite put my
[1397.56 → 1399.56] finger on what it is.
[1399.60 → 1404.42] I don't fully like about them, but I never end up sticking with them.
[1404.96 → 1408.44] And I couldn't give you a concrete reason why, but it just sort of happens.
[1408.44 → 1410.90] And the same thing happened with TO notes before.
[1411.72 → 1413.08] So hopefully this time is different.
[1413.18 → 1416.96] Now I've dug into the settings a little bit, and we'll see, I guess.
[1417.46 → 1423.00] You know what I think it might be for me is I changed Nextcloud servers a couple of times
[1423.00 → 1428.68] and I sort of hit the reset button on my notes and I wanted something that was separate from
[1428.68 → 1430.52] that and not really wrapped up.
[1430.54 → 1437.02] And I didn't really appreciate that TO notes doesn't even need Nextcloud at all to function.
[1437.02 → 1439.36] Using what, like Synching or something like that?
[1439.58 → 1440.16] That's what I'm thinking.
[1440.74 → 1441.10] Yeah.
[1441.26 → 1443.96] I mean, I actually have Nextcloud now, so I'm just using that.
[1444.06 → 1444.20] Yeah.
[1444.40 → 1444.54] True.
[1444.72 → 1447.64] Without the API, I'm just using the File Sync right now.
[1447.94 → 1451.98] And then I have another folder that I think I'm going to keep as like a backup copy.
[1452.30 → 1456.08] And then maybe I might eventually throw Synching at that.
[1456.44 → 1459.74] I want to do an episode where you and I talk about Synching a little more because I'm using
[1459.74 → 1463.24] that for a lot of things I never really expected.
[1463.24 → 1466.54] It's kind of in a way, it's become like a global file system for me.
[1466.70 → 1467.62] It's really cool.
[1468.02 → 1468.58] Oh, that's interesting.
[1468.80 → 1469.72] I'll look forward to that one.
[1470.26 → 1476.12] I've used BitTorrent Sync since you were using it on the Unfitter show years ago, now
[1476.12 → 1477.12] called Emilio Sync.
[1477.24 → 1479.34] But I'll be interested to hear about Synching.
[1479.66 → 1480.44] Yeah, it's different.
[1480.68 → 1481.34] Definitely different.
[1481.52 → 1483.36] And it's not like a torrent-like protocol.
[1483.46 → 1484.24] It's its own protocol.
[1484.80 → 1489.52] I was just the other day, I was reading their comparison of the two, and they assert that their
[1489.52 → 1491.44] security is superior, Synching does.
[1491.70 → 1494.70] And they also point out that all of their code is open source.
[1495.50 → 1496.92] Yes, well, you can't argue that one.
[1497.58 → 1498.90] The open source angle anyway.
[1499.26 → 1500.20] That's just a fact.
[1502.74 → 1503.32] All right.
[1503.34 → 1508.86] So last episode, we talked a little bit about Plex AMP and I gave it a bit of a rough review.
[1509.34 → 1511.94] I'd like to change my assessment slightly.
[1511.94 → 1517.62] I had a lot more time to play with it over the last week or two and fix some issues with
[1517.62 → 1520.08] my Plex library that were causing it to act out.
[1520.52 → 1525.42] If you remember from last episode, I put on heavy metal radio, and it played tool and then
[1525.42 → 1528.80] M&M one after another, which was not right.
[1529.18 → 1534.20] And it turned out that actually the slash temp directory for my Plex media server container
[1534.20 → 1535.44] was not writeable.
[1535.68 → 1537.92] And that is why I was having these issues.
[1537.92 → 1544.38] So if you're having lots of random weirdness when you're scanning your library, for example,
[1544.72 → 1550.22] when I was going to do, you know, fix match for, you know, a really mainstream album like
[1550.22 → 1554.26] Green Day, American India, it tried to tell me it was by the Beastie Boys.
[1555.96 → 1556.92] I was like, no.
[1557.56 → 1560.08] And you're telling me this is because your slash temp wasn't writeable?
[1560.36 → 1560.76] Correct.
[1560.92 → 1561.30] What?
[1561.66 → 1567.38] After we talked to Elan in one of the earlier episodes of Self Hosted from Plex, he invited
[1567.38 → 1571.38] me to one of their internal Slack channels where they've been doing the development of
[1571.38 → 1572.74] Plex Amp for the last six months.
[1573.54 → 1577.32] And so I reached out to him on there and said, hey, I've got this really strange issue that's
[1577.32 → 1578.92] preventing me from using Plex Amp.
[1578.98 → 1583.06] So he and I spent a couple of hours going back and forth on Slack trying to debug this
[1583.06 → 1583.36] thing.
[1583.58 → 1586.80] And I learned a lot about all the different log files that Plex keeps.
[1587.38 → 1592.58] When Plex does a scan for a media file, it writes something to temp very, very briefly
[1592.58 → 1593.56] for less than a second.
[1593.56 → 1596.34] And so he was asking me to try and capture that file.
[1596.62 → 1601.98] And in the process, I just tried to do a touch test file in that directory when I was exact
[1601.98 → 1604.08] into the container, and it wouldn't work.
[1604.14 → 1605.16] And I'm like, well, there we go.
[1605.26 → 1606.08] Temp's not writeable.
[1606.82 → 1610.00] Did a change mod and then it was fine.
[1610.12 → 1611.62] So I just removed the mapping altogether.
[1611.82 → 1615.12] I don't even remember really why I had that volume mapping in my container.
[1615.28 → 1618.40] But anyway, I removed it and it worked.
[1618.70 → 1620.98] And I've just been in love with Plex Amp.
[1621.30 → 1622.00] It's great.
[1622.00 → 1622.80] It's beautiful.
[1623.22 → 1624.84] It works really, really well.
[1625.18 → 1628.78] It handles the caching of the tracks ahead really well.
[1629.24 → 1630.44] I found the recommendations.
[1630.72 → 1634.14] Now I've got temp working to be really quite good, you know.
[1634.26 → 1637.62] So I'm sorry, Plex Amp, that I was rude about you to start with.
[1638.20 → 1639.56] But I kind of love you now.
[1640.14 → 1641.60] So a little more time with it, and you're liking it, huh?
[1641.86 → 1646.64] Isn't it interesting that the recommendations' aspect of it seems to play a pretty central role
[1646.64 → 1646.96] for you?
[1646.96 → 1652.60] Yeah, I mean, that's kind of what I use Spotify for really is I go to a particular artist and
[1652.60 → 1656.12] I'll search, and I'll just play the top tracks or whatever most of the time.
[1656.20 → 1660.06] And then I look through, you know, recommended artists or a Discover Weekly playlist that uses
[1660.06 → 1662.60] like machine learning to generate who it thinks I'm going to like.
[1663.24 → 1667.84] But of course, with your own music library, most of the time, you know what's in there.
[1668.10 → 1672.26] You've generally curated it to the point where you know most of the tracks on an album
[1672.26 → 1674.02] because you've listened to it at least two or three times.
[1675.44 → 1682.10] And so what I found the most interesting was when I was scanning the albums to Plex in the
[1682.10 → 1686.34] first place, I was going through metadata madness, trying to fix it, trying to make sure that
[1686.34 → 1688.90] Green Day American Idiot album was absolutely pristine.
[1689.08 → 1689.98] It had the correct cover.
[1690.42 → 1691.68] It had the correct tags.
[1691.96 → 1694.56] It had everything was perfect in the metadata of the files.
[1694.76 → 1696.46] And it still thought it was the Beastie Boys.
[1696.46 → 1700.24] So I started looking at ways to make sure the metadata was correct.
[1700.38 → 1703.04] And I used a program called Beats to do that.
[1703.32 → 1706.52] Now, there's a post over on the Linux server blog written by Josh Stark.
[1706.90 → 1711.64] And he covers a bunch of interesting stuff about Beats in there, which is it being a command
[1711.64 → 1714.70] line music metadata management tool.
[1715.10 → 1715.78] And that's it.
[1715.88 → 1720.32] I mean, it can import music from a download directory or a ripped CD directory or whatever,
[1720.32 → 1723.52] and then goes through and tags it against a bunch of databases.
[1723.52 → 1727.62] And it's very command line driven, which means it's scriptable.
[1727.92 → 1731.86] So if you want to do some automation around the imports of your music, you can do it that
[1731.86 → 1732.10] way.
[1732.50 → 1735.96] But that led me on to another problem.
[1736.24 → 1742.22] I was hitting API rate limits of one a second on the music brains API, which meant that Beats
[1742.22 → 1744.66] was running really, really, really slowly.
[1745.20 → 1750.04] I'm talking it would have probably taken several days to import my entire library.
[1750.04 → 1756.16] Uh, so Linux server also make a self-hosted music brains mirror.
[1756.72 → 1762.02] So I'm now running on my server, a local mirror of music brains, which is kind of cool.
[1762.32 → 1766.20] So then you just point Beats to that local mirror, and you can rate limit to, you know,
[1766.22 → 1768.00] a hundred requests a second instead of one.
[1768.08 → 1770.10] So it goes much, much faster.
[1770.50 → 1771.26] Oh, that's really cool.
[1771.30 → 1772.62] I didn't even know you could host that.
[1772.68 → 1775.38] That is a rad little discovery, Alex.
[1775.68 → 1778.68] Isn't it interesting that rabbit hole you ended up going down for this?
[1778.68 → 1781.46] Just trying to fix metadata to get Preamp working.
[1782.08 → 1785.26] Anyway, it turned out it was slashed temp and all the metadata was fine anyway.
[1785.52 → 1787.18] So there you go.
[1788.14 → 1789.78] I wonder why people use Spotify.
[1790.02 → 1794.56] I wonder, hey, while we're talking about you going down rabbit holes, traffic 2.2 came
[1794.56 → 1799.36] out back in March and I think you just recently had a chance to deep dive, but I didn't hear
[1799.36 → 1800.04] how that went.
[1800.04 → 1806.32] The reverse proxy of choice in the Kretschmar household for the last several years has been
[1806.32 → 1806.92] Nginx.
[1808.04 → 1812.28] And I don't know, sometimes I get itchy feet and I think to myself, oh, the grass is greener
[1812.28 → 1812.64] over there.
[1812.70 → 1818.18] What if I just use traffic with its super cool labels and I could just define everything in
[1818.18 → 1821.54] my Docker compose file and not have to worry about Nginx configs.
[1821.94 → 1822.74] It works great in the studio.
[1823.12 → 1823.62] And it was.
[1823.66 → 1824.96] It was working really, really well.
[1824.96 → 1830.80] I was having a great time until, and I'm afraid to say until, because this is going
[1830.80 → 1836.36] to be a showstopper for me, until I went to use any container that was in host mode.
[1836.74 → 1841.58] As soon as I did that, the container is no longer on the Docker network, which is what
[1841.58 → 1845.22] traffic uses for internal, you know, DNS.
[1845.40 → 1847.12] It's what it uses for internal communications.
[1847.96 → 1851.12] It's actually on the host network.
[1851.30 → 1853.06] So hence host mode.
[1853.06 → 1855.50] So Docker basically can't see it anymore.
[1855.78 → 1862.04] And as such, you can't route any traffic through traffic to the container, which unfortunately
[1862.04 → 1863.04] means it's no good to me.
[1863.30 → 1865.66] How many containers are you running in host mode networking?
[1866.10 → 1866.82] Plex being one.
[1867.64 → 1870.66] Mostly for some of the UPnP stuff it does around the HD home run.
[1871.04 → 1871.18] Yeah.
[1871.28 → 1875.24] I mean, when possible, I suppose it's best not to use host networking, but I guess on
[1875.24 → 1877.82] your LAN media box, it's not really the end of the world.
[1878.16 → 1879.32] No, I thought I had more than that.
[1879.38 → 1880.60] The only one is Plex, apparently.
[1880.60 → 1886.10] So maybe I should just expose a bunch of individual ports instead of relying on host
[1886.10 → 1886.32] mode.
[1886.80 → 1889.98] It might not be worth it, but there are a lot of nice advantages to using traffic.
[1890.34 → 1892.20] And if that's all it took.
[1892.56 → 1893.72] I did really like it.
[1893.80 → 1897.94] It took quite a bit to get my head around the kind of concepts of their front ends and
[1897.94 → 1900.72] back ends and how to get the labels just right.
[1901.12 → 1906.82] Specifically, an issue I ran into was because V2 only came out in autumn last year.
[1906.82 → 1910.88] An issue I ran into was a lot of the documentation is around V1.
[1910.98 → 1915.30] And when you're Googling for stuff, you find syntax for V1 rather than V2.
[1916.20 → 1918.02] That's obviously going to improve with time.
[1918.12 → 1922.20] And it's not really a fair criticism of a project that it's, you know, developing and
[1922.20 → 1923.06] changing and improving.
[1923.26 → 1931.68] But what really drew me to traffic was the Kubernetes kind of cloud router of the future type sales
[1931.68 → 1932.88] pitch that they're going for at the moment.
[1932.88 → 1935.78] But I must say, it's pretty cool.
[1935.94 → 1939.60] You know, five or six labels in the compose file that define how the traffic gets rooted.
[1940.00 → 1942.00] And it's all in one place.
[1942.22 → 1945.12] And, you know, from a quick scan, I can see exactly what's going on.
[1945.36 → 1947.64] And I really like that concept.
[1947.88 → 1951.60] It's just, I don't know, maybe I should try to give a bit more of a try, Chris.
[1952.26 → 1953.74] I'd be curious to hear what you think.
[1953.86 → 1955.42] I think it'd be interesting to follow up on it.
[1955.96 → 1962.24] It's also sort of, I think, good market research for a guy in your day job position.
[1962.24 → 1965.36] I did see that Caddy V2 had a release today as well.
[1965.42 → 1966.74] So I might go check that out this week.
[1967.28 → 1969.94] Maybe I'll do a little reverse proxy roundup next week.
[1970.30 → 1971.78] Yeah, that would be great.
[1971.90 → 1972.20] Totally.
[1972.40 → 1975.50] I would be, I mean, we're nerds, but I'm totally down for that.
[1975.96 → 1980.84] But before we go, speaking of new releases, pretty excited to see that a ROK app has landed
[1980.84 → 1981.66] for Jellyfin.
[1981.78 → 1983.12] We'll have a link to that in the show notes.
[1983.54 → 1987.68] I'm super-duper excited because this is my second JB prediction that's come true this
[1987.68 → 1987.88] year.
[1987.88 → 1994.24] I predicted, number one, that WireGuard would be backported to the kernel that released
[1994.24 → 1996.00] with Ubuntu 2004.
[1996.58 → 1997.26] Yeah, you did indeed.
[1997.58 → 2002.62] I predicted that Jellyfin and MB would start upping their app game and start shipping on
[2002.62 → 2003.54] some major platforms.
[2003.74 → 2005.42] And I think this is evidence of that.
[2005.62 → 2007.86] So it's down to the referee.
[2008.22 → 2011.50] You know, I'm not saying I've won the race yet, but it's looking good.
[2011.50 → 2015.66] Well, if you want to be impressed by future Alex predictions, you can be impressed directly
[2015.66 → 2018.76] by checking out our Discord at self-hosted. Show slash Discord.
[2018.90 → 2021.32] We have a growing active community over there.
[2021.42 → 2025.12] Also, you get just little additional things that go along with the show.
[2025.24 → 2026.12] Information, notices.
[2026.34 → 2029.60] Sometimes Alex will drop a great deal for hardware in there.
[2029.70 → 2031.36] So self-hosted. Show slash Discord.
[2031.76 → 2035.58] If you'd like to email us, we'd love to get your emails at self-hosted. Show
[2035.58 → 2036.76] slash contact.
[2037.08 → 2037.90] And then subscribe.
[2038.16 → 2043.04] The show is fortnightly, and you can find it at self-hosted. Show slash subscribe.
[2043.76 → 2047.72] And if you want to get more pictures of my delicious barbecue meat smoking adventures,
[2047.98 → 2049.74] I'm on Twitter at Ironic Badger.
[2050.08 → 2052.66] Yeah, and they are very tasty looking.
[2052.82 → 2054.28] I am at Chris LAS.
[2054.70 → 2058.26] Oh, I didn't mention it in the show, but this entire episode is solar-powered, completely
[2058.26 → 2059.04] off grid.
[2059.04 → 2063.44] I have a little bit of just enough cell connection to do this.
[2063.44 → 2068.70] And we're watching all of our offline media on my local Raspberry Pis.
[2069.32 → 2070.18] It's happened.
[2070.64 → 2073.32] Greta Thunberg somewhere is really happy with you.
[2073.36 → 2073.70] Good job.
[2074.06 → 2076.84] I know Project Off Grid is a resounding success.
[2076.96 → 2082.84] Even with an overcast sky, we're generating enough solar to top off our battery bank by the
[2082.84 → 2083.28] end of the day.
[2083.78 → 2087.20] So no generator, just solar 100%.
[2087.20 → 2088.52] It's so awesome.
[2088.72 → 2090.98] So I'll have to maybe I'll post a picture up on Twitter.
[2091.66 → 2092.40] That is really cool.
[2092.40 → 2094.52] I want to buy solar so bad.
[2095.26 → 2098.16] It's just expensive, you know, solar-powered, self-hosted.
[2098.26 → 2103.04] So I am at Chris LAS and the show is at self-hosted show on Twitter.
[2103.30 → 2104.08] Thanks for listening, everyone.
[2104.32 → 2105.58] That was self-hosted 18.
