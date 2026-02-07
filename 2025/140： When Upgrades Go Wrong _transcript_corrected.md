[0.00 → 6.30] Well we're back for a new year, welcome into self-hosted episode 140 everybody and happy 2025.
[6.92 → 13.28] Now to begin this year my downstairs thermostat decided it had had enough of connecting to my
[13.28 → 19.88] Wi-Fi, my venerable Ven star T2000. So I bought a new thermostat, put it on the wall, didn't tell
[19.88 → 27.58] my wife and I think I might have peaked in wife approval factor because unprompted wife came in,
[27.58 → 32.52] saw a new thermostat on the wall and texted me and said I like the new thermostat Alex.
[32.90 → 37.70] Oh that is a good sign. Yeah, and I have to be honest the Minimax or whatever it is,
[37.98 → 43.96] I have one here in the studio, it's utilitarian. I think it might even be more aimed at commercial
[43.96 → 50.24] spaces. Its mother loves it. Yeah, yeah its mother does love it but not much love from anybody else.
[50.34 → 54.54] I've also had to drop off the Wi-Fi once before, so I'm curious to know what you replaced it with.
[54.54 → 60.00] Yeah my Ven star just dropped, it's been going on for a... Ven star that's what it is.
[60.00 → 66.24] Yeah for about three or four months and every few days maybe once or twice a month it would just drop
[66.24 → 71.84] off of Home Assistant and the integration would stop picking it up. The reason I bought that Ven star
[71.84 → 77.94] when we moved into this house five or six years ago, I wanted to maintain the fully local control
[77.94 → 82.40] surface for the thermostat. Like I didn't want it to be reliant on a cloud integration or whatever
[82.40 → 88.16] because it's just a thermostat at the end of the day. Agree. So I went for an Eco bee. Yeah, okay I've
[88.16 → 93.08] heard good things about Eco bee, I've never used one myself. This one's really nice, it's the Eco bee
[93.08 → 101.04] Lite. I picked it up on Amazon for about $130, and it integrates with HomeKit. So of course HomeKit
[101.04 → 106.82] is a fully local protocol. You power the thermostat up through the control wire from the thermostat,
[106.82 → 112.74] from the furnace or wherever and then Home Assistant just picks it up and says hey I've
[112.74 → 117.26] detected a new HomeKit capable device on your network. Do you want to pair with it? You click
[117.26 → 121.74] the button yes, off we go, and then it shows the pairing code on the screen of the thermostat. You
[121.74 → 126.52] type in the eight-digit code, bad bing bad boom. Easy as that. You were able to add it to HomeKit
[126.52 → 132.80] via an iPhone, and it still works with Home Assistant. No. So actually that was a mistake I made when I first
[132.80 → 137.92] got it out of the box. Okay. Because you can only pair with one HomeKit bridge at a time I guess.
[138.20 → 143.04] Yeah. And I think Home Assistant is emulating whatever that HomeKit bridge thing was doing
[143.04 → 148.74] before. So I did pair it with my phone originally expecting it to then be picked up by Home Assistant
[148.74 → 153.36] through IP or whatever once I configured the Wi-Fi. Yeah, and I've noticed often like the phone
[153.36 → 157.96] aggressively and the app that the vendor makes they all really want you to use the HomeKit on the phone.
[157.96 → 165.94] I assume for telemetry reasons but the pairing process with the Eco bee was well originally with
[165.94 → 170.18] the phone you just scan the barcode the QR code on the screen and it sort of walks you through in
[170.18 → 175.92] the home app what to do. I then realized I needed to factory reset the thermostat and then actually go
[175.92 → 182.40] and look in Home Assistant before I paired it with the phone to pair it with HomeKit in Home Assistant.
[182.40 → 187.30] In Home Assistant. Yeah, exactly. Yeah, and did it show up as a notification in Home Assistant?
[187.30 → 191.90] Did it auto-discover it? Yeah, one of those hey check it out here's what I found on your network type
[191.90 → 198.76] notifications. Yeah, that makes it pretty easy then. And so now if it is available on the iPhone via
[198.76 → 202.26] HomeKit because you probably connected that I would imagine to Home Assistant so it works that way.
[202.32 → 206.80] Oh I don't know let me have a look. You can do that yeah. So this is really cool. So you got the
[206.80 → 215.82] Eco bee 3 Lite, and it's essentially just talking over HomeKit on Wi-Fi? Yeah, it's Wi-Fi only as far as I know.
[215.82 → 222.56] One of my buddies suggested I looked at the Nest that does matter over Wi-Fi. I guess I could have
[222.56 → 228.26] done that, but I don't know. Eco bee seemed like a slightly better recommended option on the
[228.26 → 235.68] forums. So I know these have like smart thermostat capabilities where they observe the heating and
[235.68 → 240.12] cooling of your home, and they figure out you know when you wake up, and you know how long it takes to
[240.12 → 244.46] heat up so they automatically turn on. Is it like one or the other? Because I would imagine Home Assistant
[244.46 → 249.58] doesn't care about any of that stuff built-in firmware running on the Eco bee. No so Home Assistant
[249.58 → 256.20] will talk to the thermostat. It's a two-way connection so if the thermostat itself sets a
[256.20 → 262.34] parameter it will report back to Home Assistant. Hey my mode is now heat, my temperature is now x,
[262.56 → 268.26] my fan is set to auto whatever and then if Home Assistant comes in and changes it, it will override
[268.26 → 275.38] the Eco bee settings, and then it says on the screen of the thermostat temperature now set at 20 20
[275.38 → 282.96] Celsius until 11 30 p.m. at which point I think the thermostat itself runs you know it has the time
[282.96 → 288.66] and date built in so it knows that most people aren't needing heat after 11 30 p.m. or something.
[288.66 → 294.54] Yeah that seems like a pretty sweet spot. We'll see because the two systems I'm sure will
[294.54 → 300.16] conflict at some point. I might end up just completely disabling all the air quotes
[300.16 → 305.44] smarts of the thermostat and just let my Home Assistant automations take care of it like they
[305.44 → 311.48] have done for the last few years. Yeah, that would probably be what my route would be and for heating
[311.48 → 318.34] I really like the scheduler card add-on or hacks whatever they're called because instead of having to
[318.34 → 324.62] build you know I don't know four or five automations to really do all the heating and cooling you want
[324.62 → 331.38] you can do it all in the scheduler card and it is accounts for sunrise and sunset and all this
[331.38 → 335.78] kind of stuff and weekends and work days and scheduler card is the way to go for that kind of
[335.78 → 340.06] stuff when you're working with a thermostat in Home Assistant in my opinion. I have a scheduler and
[340.06 → 344.30] she's four years old and bounces on our bed at 7 a.m. on the dot every morning.
[344.30 → 350.88] Well yeah keep us up-to-date let us know uh maybe in a little while we'll do a little follow-up and
[350.88 → 356.20] see how it's working. Yeah. Now I know you've been uh improving the infra for the holidays.
[356.80 → 361.16] Oh my goodness I just was checking off projects left right and centre over the Christmas period.
[361.48 → 366.38] I got a new keyboard, and you know I just wanted to type on it. I just had one of those moments
[366.38 → 371.86] of like oh I've got these lovely new switches I want to just I just want to type all the time, so I ended up
[371.86 → 376.82] fixing a whole ton of technical debt that's been in my personal infra repo for
[376.82 → 384.08] a very long time. Some of the code actually I wrote in London before we moved, and it was still
[384.08 → 390.50] doing still doing the thing. The biggest one that I upgraded actually was the docker compose
[390.50 → 396.72] generator Ansible role that I've maintained for the last few years. Essentially the logic behind this
[396.72 → 403.88] thing is that you defined a YAML dictionary of containers like a bespoke esoteric format that
[403.88 → 411.20] only worked with my Ansible role which was sort of like compose but also definitely actually not
[411.20 → 417.94] compose. Where so what I've done now is I was talking to fuzzy mis born one of our discord admins
[417.94 → 423.74] over the holiday break, and he came up with the idea of well why don't we just ingest actual
[423.74 → 429.78] compose YAML files. I was like that's kind of brilliant why don't we just do that. So I've
[429.78 → 435.68] modified the role now such that you can create a directory tree of files and the Ansible role
[435.68 → 442.02] will walk through that directory tree pull out all the standard compatible compose files that they're
[442.02 → 447.22] just bog-standard compose files there's nothing special about them at all and then ingest them into
[447.22 → 452.20] the Ansible role and then concatenate them all together into one giant file and then dump that onto the
[452.20 → 456.84] remote server. So you can still maintain all the secrets in Ansible vault you can still maintain
[456.84 → 461.76] all the kind of workflow stuff if you've been using Ansible to manage your servers for a while
[461.76 → 469.78] except the change now is that rather than creating this massive custom bespoke dictionary of things in a
[469.78 → 476.26] list of containers you just put compose files in a directory instead. Yeah, and you can work with
[476.26 → 480.92] just bog-standard compose files that you get from the project. That's it exactly, and I think I've been
[480.92 → 485.14] wanting something like this for quite a while, and you know we talked last week with Shane about
[485.14 → 490.96] yeet for example and that kind of gets you most of the way there with a similar idea but it
[490.96 → 497.30] does a lot of the lot of the sort of moving files onto the remote host and things like that for you
[497.30 → 502.88] whereas this is just plugged into the Ansible matrix instead that the world I've managed all my
[502.88 → 508.52] servers with for the last few years. It's kind of just another way of doing the same thing as what
[508.52 → 514.90] yeet is going to do when that comes out. You know options. I mean actually what I really am
[514.90 → 521.80] taking away from this is the ultimate productivity hack is to get a new keyboard. It's true yeah yeah I
[521.80 → 528.32] got a bridge 75 hall effect mechanical keyboards it's from mechanical keyboards.com which is not
[528.32 → 533.38] sponsored I know we have key bio as a sponsor and I still love the iris that I got from them a couple
[533.38 → 539.78] of months ago but uh the bridge 75 is it's the hall effect switches you can actually change the
[539.78 → 545.22] actuation height of the switch. Oh my goodness. So each individual switch can have a different
[545.22 → 552.42] actuation height from like 1.2 mild own to I think 3 mid and anywhere in between. It's kind of cool.
[553.22 → 558.52] Now I don't want to skip over anything, but I know you ended up having to go through a
[558.52 → 567.76] aggravating migration from SQLite to MySQL. Oh, yes so those of you that pay attention at blog.ktz.me
[567.76 → 574.48] might have noticed that the RSS feed spammed you, and I'm really sorry about this with every single
[574.48 → 581.22] post I've written in the last year twice. You know maybe they've got some time for the form the
[581.22 → 586.64] holidays they can just you know catch up. Let me explain why that happened, and again I am very sorry
[586.64 → 593.00] for that, but you know here be dragons when you're self-hosting sometimes. Indeed. So Ghost version 4
[593.00 → 599.22] is the version that I've been running my blog on for I don't know when did version 4 come out a
[599.22 → 605.26] couple years ago let's say, and I've put off the upgrade to version 5 which is maybe a year or more
[605.26 → 610.44] because I had a custom theme and I couldn't be bothered to upgrade it and blah blah blah. Sure.
[610.44 → 617.14] I was experimenting with Renovate Bot again a recommendation from Fuzzy Mist born which is a way
[617.14 → 625.50] of looking at your compose files in a git repository, and it looks at the tags, and it nags you and opens
[625.50 → 631.80] a pull request against your repo and says hey this version of MySQL is out of date hey this version
[631.80 → 637.80] of Ghost is out of date blah blah blah like it looks at the docker tags and offers you up the latest
[637.80 → 642.42] image, and you can just merge the pull request and off you go. Ghost was one of those things, and I was
[642.42 → 646.68] like you know what I should probably get around to upgrading Ghost at some point it's been a couple
[646.68 → 655.84] of years now. So Ghost version 3 I think is where this blog started back in 2017 or 18 so it's a very
[655.84 → 661.56] long-lived installation. Sure. It's moved across multiple hosting providers and this is why I love Docker so much.
[661.56 → 669.80] It's moved from DigitalOcean to Linde to Hetzner now you know, and I just love it so much. Docker that is.
[670.48 → 678.08] Ghost I am rapidly losing patience with but anyway version 3 and 4 were running out of an SQLite database
[678.08 → 687.96] and I could see that version 5 only supported SQLite up until I think 5.0.83 or something and the latest
[687.96 → 696.70] version is 5.2 something, so I had to upgrade air quotes upgrade from SQLite to MySQL as the database
[696.70 → 704.26] back end. That's what all version 5 installs now do by default anyway. So I tried with Claude for maybe
[704.26 → 711.64] two or three hours to get all the foreign key constraints and things like that with an SQLite to
[711.64 → 718.52] MySQL migration tool working and I kind of got most of the way there and then there was something
[718.52 → 723.52] happened I can't remember what exactly, but I ended up back at square one again where it was running from
[723.52 → 730.88] the SQLite database even though I told it not to, and then I upgraded oh this is what it was I upgraded
[730.88 → 741.26] MySQL on a fresh installation to 8.4 but Ghost 5 has a bug where it only initializes properly with 8.0 of MySQL
[741.26 → 748.22] Oh go figure. I tell you I had a rough evening with that one. It must have taken a minute to
[748.22 → 754.22] realize that was even the issue too. Yeah, it did rather longer than I'd like to admit a bit more
[754.22 → 759.50] gin than I'd like to admit to actually but essentially what I ended up doing was just go in the end
[759.50 → 764.72] throw my hands in the air and just being like oh screw this I'm going to reinstall Ghost I'm going to
[764.72 → 772.52] export the old JSON file and the old content directory and then do a reinstallation of Ghost to
[772.52 → 778.60] version 5 completely fresh installation reinitialize like there'll be no foreign key issues with the
[778.60 → 785.80] database it will all be fine. Yeah. So I import the JSON file I exported and that's when the RSS feed went
[785.80 → 791.50] and just spammed everybody with everything, and I was like oh god I'm so sorry.
[792.58 → 798.34] How did you realize that one? I got messages. Oh, yeah oh god that's the best. On Mastodon someone
[798.34 → 806.08] was like hey Alex your blog just spammed me like 20 posts all at once. Oh, man. So if you got those
[806.08 → 810.60] messages I am sorry, but that is why, and it's because I'm a horrible sysadmin.
[810.60 → 817.20] Tailscale.com slash self-hosted head on over there support the show and try it for free
[817.20 → 823.98] for up to 100 devices and three users and that is not a limited time deal it's the plan I have been on
[823.98 → 829.84] and they have great options for enterprises. As you know I probably spent the last two years really
[829.84 → 837.38] building out my personal LAN over my tail net a mesh network protected by WireGuard. Each machine is a
[837.38 → 843.72] node and a lot of my applications too. Even my mobile devices, but then I realized we could use it
[843.72 → 847.76] for the back-end infrastructure of Jupyter Broadcasting, and we can move things between
[847.76 → 853.14] data centres. We have portability. We can bring things on LAN for big jobs and the public IP always
[853.14 → 858.88] stays the same. It's really powerful. It's the easiest way to connect devices and services to each
[858.88 → 865.48] other wherever they are. You know everyone's heard of a VPN but Tail scale isn't like those. It's not about
[865.48 → 870.50] hiding your browsing habits from coffee shop owners or watching Netflix from another country although
[870.50 → 876.48] you can do certain things like exit nodes. I've used exit nodes when I'm in a hotel to make it look
[876.48 → 881.12] like I'm coming from home for my TV streaming service. You get secure remote access to your
[881.12 → 886.54] production systems, your servers, Kubernetes configuration, whatever it might be, and you get
[886.54 → 893.06] it fast, really fast, and it's private, and it's really simple to deploy for your entire organization.
[893.06 → 900.08] You can build a simple network across complex infrastructure. I'm saying like your VPSs across
[900.08 → 906.98] multiple different providers and multiple different IP nets, LAN's, mobile devices, all on one flat mesh
[906.98 → 912.68] network, and then you can use ACL policies to securely control access to devices and services with
[912.68 → 918.90] Tail scale's next generation network access controls. It really is something that just works. It's a solution
[918.90 → 924.62] for the modern way we do networking and I have no inbound ports on any of my firewalls anymore.
[924.92 → 929.14] The personal plan will always be free so start there. Try it for free and support the show. You get
[929.14 → 935.86] 100 devices and three user accounts for free when you go to tailscale.com slash self-hosted. No credit
[935.86 → 940.22] card required either. This is going to change your networking game, and it's a great time to start
[940.22 → 944.72] right now at the beginning of the year. Tailscale.com slash self-hosted.
[946.24 → 950.12] Now I've got a bunch more infrastructure upgrades and things that I did over the holiday
[950.12 → 956.38] period. I've written some blog posts about some of them which are on the aforementioned blog of
[956.38 → 961.70] RSS Shame, and we might talk about some of them in the future as well. Some stuff with Git submodules and
[961.70 → 968.66] Git Crypt but for now I wanted to talk about Apollo Automation. They sent me over a couple of devices
[968.66 → 975.28] for review and Chris I believe you're getting one in the mail soon as well. Just in time because I
[975.28 → 980.30] recently got a diesel heater and one of the devices that Apollo Automation has is an air quality sensor
[980.30 → 987.84] and you can add a CO2 and a gas sensor to it as well and guess what that's exactly what I've been
[987.84 → 992.30] thinking about building recently. The thing I really like about these sensors, and we'll get into a full
[992.30 → 999.84] full review probably in the next episode or two is that they are home assistant first ESP home based
[999.84 → 1004.72] stuff. So yeah yeah head over to ApolloAutomation.com go and check them out. We're going to be looking
[1004.72 → 1010.92] at the millimetre wave sensors as well the MTR1 and the MSR2 because in my new studio build that I'm
[1010.92 → 1016.14] doing upstairs remember I talked about wanting some smart lighting stuff going on well I figured that
[1016.14 → 1020.84] millimetre wave is the way to do that these days. Yeah, definitely one of the other things they have on
[1020.84 → 1028.16] there is indoor plant soil sensors, and I'm going to automate my wife's clinic, and she has lots of
[1028.16 → 1034.64] plants in there. We go on road trips for an extended period of time could be perfect for that, so I think
[1034.64 → 1040.70] there's I think there's a lot of potential and a market here for companies that make home assistant
[1040.70 → 1045.48] first products like this. Definitely yeah particularly I think home assistant is I don't want to say it's
[1045.48 → 1050.72] won the race, but I don't see anybody else coming close to what they're doing even after all these years
[1050.72 → 1055.96] do you? No, and now that they have the open you know the open home uh group, and you know they're
[1055.96 → 1061.08] they're expanding pretty successfully into hardware each time they do it they seem to be getting better
[1061.08 → 1066.36] and better. Home assistant maintains a steady release cadence even during holiday months.
[1067.58 → 1073.20] Uh they're kind of firing on all cylinders it's pretty good to see. Yeah, of course last episode we
[1073.20 → 1077.26] heard from Paulus you know some of their big plans around the uh the little voice puck I've been
[1077.26 → 1083.24] loving mine. Yeah, it is it's really neat to see them go um, and I'm going to be playing a lot more
[1083.24 → 1088.86] with that I think over the year. I like to that you and I were both in the books space and the
[1088.86 → 1096.66] audiobook space we both found different tools around EPUB books and creating audiobooks from them and
[1096.66 → 1102.46] whatnot, and we didn't talk about this ahead of time at all. No we didn't we often joke that this is the
[1102.46 → 1110.44] year of the Linux desktop well this is the year of AI related tools actually becoming useful in my world
[1110.44 → 1116.52] at least. I found one called e-book to audiobook and this one kind of says what it does on the tin but
[1116.52 → 1123.80] it converts e-books to audiobooks with chapters and metadata using dynamic AI models so whisper in other
[1123.80 → 1131.30] words but this one does something that's really cool it does voice cloning. So if you've ever
[1131.30 → 1137.78] wanted David Attenborough to read you The Hobbit now's your chance. All right I like that a lot
[1137.78 → 1146.20] okay all right hmm, so I was looking for something that was kind of audiobook first because I am a big
[1146.20 → 1152.22] audiobook guy I do a lot of driving like I said perfect for audiobooks, but I do sometimes prefer to
[1152.22 → 1158.92] read or mix it up like maybe I listen 60 percent to the audiobook, but a bit just like a few sections
[1158.92 → 1165.04] I want to read well that's where storyteller comes in it's a self-hosted platform for creating and
[1165.04 → 1170.52] reading e-books that sync to narration so it's essentially three components there's an API server
[1170.52 → 1176.28] as a web interface, and it has mobile apps and these components allow you to take audiobooks and e-books
[1176.28 → 1183.08] that you already have and synchronize them as well as read or listen to them, and it syncs them up so you
[1183.08 → 1188.38] can have it generate the audio listen to that for a while and then hit pause and the next time you open
[1188.38 → 1195.56] up the EPUB version you're at the same spot the narrator left off and vice versa it's in beta right
[1195.56 → 1203.18] now and uh you know it's a docker they have a docker composed so it's not a huge deal to get it running
[1203.18 → 1209.78] I like the interface like you've got the've got the text on one side and then the app on
[1209.78 → 1215.76] the other I suppose this is the way that like audiobooks should just work anyway isn't it yeah
[1215.76 → 1222.92] I thought Amazon had something like this, but I've kind of moved away from the audible player and I
[1222.92 → 1228.52] don't use a Kindle any more you know I'm all I'm all in an audiobook shelf, and so I just have a whole
[1228.52 → 1237.46] stash of these now unraid.net slash self-hosted go there right now because unpaid 7 is out this is a
[1237.46 → 1245.02] huge upgrade unraid.net slash self-hosted let's start with the ZFS stuff hybrid ZFS pool support
[1245.02 → 1251.42] for sub pools with advanced allocation profiles, and now we've got improved fault recovery so
[1251.42 → 1259.06] enhanced handling of multiple drive failures in a ZFS pool lands in unpaid 7 luxe encryption yep it's
[1259.06 → 1264.84] there they have a brand-new file manager and GUI tools as well as a revamp dashboard in unpaid 7
[1264.84 → 1268.88] the GUI search quickly locate settings with the new built-in search functionality so you can get
[1268.88 → 1275.74] right to what you're looking for it's really nice to see this enhanced VM manager land as well and
[1275.74 → 1281.46] there's even easier pass-through for hardware peripherals in a SMU environment so you can do video and
[1281.46 → 1288.48] other hardware devices inside your VM and of course improved docker management is here but one of the
[1288.48 → 1293.12] things that I'm the most excited about is they've integrated tail scale seamlessly into the docker
[1293.12 → 1299.60] containers this is how I do my setups custom, and you know now they're doing it with a click of a
[1299.60 → 1305.62] button, and you get secure remote access for sharing your individual containers over your tail net of
[1305.62 → 1309.74] course there has been lots of networking upgrades and samba sharing upgrades that improve compatibility
[1309.74 → 1315.46] with macOS and one of the things I think it's great to see land in unpaid 7 is power modes you can
[1315.46 → 1320.36] optimize performance you can balance your power depending what you need, or you can go for maximum
[1320.36 → 1326.62] efficiency you got to go check it out start by going to unraid.net slash self-hosted this has been
[1326.62 → 1334.96] in the works for a long time, and it's a major revamp it is so cool to see this, and I love to see all of
[1334.96 → 1340.54] the improvements and I just scratched the surface I mean there's so much in the new unpaid 7
[1340.54 → 1345.60] you got to go check it out for yourself what a great time to get started too you can mix and match
[1345.60 → 1349.48] the different discs you might already have in your closet and get something up and running and have
[1349.48 → 1355.86] a home lab in an afternoon might take you a week when you build the stuff from scratch and the unpaid
[1355.86 → 1363.46] version 7 is just looking so good check it out unraid.net slash self-hosted and a big congratulation to
[1363.46 → 1371.54] the unpaid team on unpaid 7 that's the official show horn we're really proud of you guys over there
[1371.54 → 1378.96] unraid.net slash self-hosted it's really the year of like these tools coming into our realm
[1378.96 → 1385.08] and actually providing a bit of functionality I mean yeah there's AI here, but storyteller doesn't
[1385.08 → 1390.42] even really lead with that neither does e-book to audiobook you know it's in the
[1390.42 → 1395.96] it's in the explanation of how it works, but they're not blasting us with AI audiobook reader or
[1395.96 → 1400.48] something it's just it's its part of how it works it's part of how everything works I mean you
[1400.48 → 1405.78] mentioned before the holidays uh an app called hoarder which is a digital kind of bookmarking
[1405.78 → 1412.30] tool and I just put my open API key in there and an Obama key in as well uh set that up just to see
[1412.30 → 1420.70] if I could do it locally I love it I absolutely love it it's its been a really nice tool for me too
[1420.70 → 1426.28] I'm still using it, and it's its like Gene Bean had boosted and asked is it kind of like does it
[1426.28 → 1432.62] replace you know wallaby and I it does for me, it's its bookmarking archival summarization
[1432.62 → 1438.74] and search and if you're really you know crazy you can also I don't know if you did this, but you can
[1438.74 → 1444.60] turn on video archiving as well which I'm kind of tempted to do yeah I gave it a go actually it
[1444.60 → 1450.58] downloaded it a really like potato quality, but you know as an archival tool it's probably sometimes
[1450.58 → 1454.86] maybe all I want actually yeah okay I hadn't thought that yeah that's actually probably what
[1454.86 → 1461.16] I would prefer I really like the fact that it takes a snapshot or screenshot of the page as well as like
[1461.16 → 1466.88] a web archive version of the page as well as any other assets it can get as well like the text or
[1466.88 → 1473.48] whatever like it will extract those too so like when I'm researching a video for tail scale, or you know
[1473.48 → 1478.92] even a segment for this show now when I'm putting it into the mobile app I have a list dedicated for
[1478.92 → 1484.04] self-hosted I have a list dedicated for tail scale whatever and I when I'm prepping these different
[1484.04 → 1489.18] things I can just put them into the correct buckets, and it goes and figures out all the tags and all the
[1489.18 → 1495.76] rest of it it's its amazing I love it thank you for putting me on to hoarder last episode, and it's
[1495.76 → 1501.74] pretty good at the tag stuff you know the summaries are you know kind of a standard ChatGPT summary of
[1501.74 → 1508.16] an article, but it's nice too you can pull it up in a reader view inside the hoarder interface and
[1508.16 → 1515.58] then hit summarize and a couple of seconds later you've got like a two-paragraph summary of a
[1515.58 → 1523.52] three-page story now I found it worked pretty well with Obama I mean obviously it's Obama is at the
[1523.52 → 1531.76] limit of the model it can run, and I'm running llama 3.2 on mine at the moment whereas you know gpt40
[1531.76 → 1537.52] mini or whatever it is as the latest in ChatGPT it is better, and it is faster and gives a slightly
[1537.52 → 1543.74] better result but not by as much as you might think and with Obama being the low price of
[1543.74 → 1549.46] free if you have a GPU at least I think that's the way to go for most people in a self-hosting
[1549.46 → 1555.48] environment at least, and it's so great that you can do that without having to rely on any kind of
[1555.48 → 1562.08] I don't know I don't even know what open AI are doing with my data, yet I mean yeah right they're at
[1562.08 → 1566.78] the phase of a company now what google were at when I was at high school where it's just anything
[1566.78 → 1572.84] goes you know and yeah you just don't have to worry about it yeah if you use Obama yeah yeah
[1572.84 → 1578.44] with old uh Sam Altman saying that they can't make a profit on a 200 dollar a month subscription
[1578.44 → 1584.30] they're gonna I feel like they're going to turn a little desperate it's going to get desperate yeah yeah
[1584.30 → 1591.36] GPUs are expensive to run they're expensive to buy yeah I know I'm I'm very grateful that Obama is open
[1591.36 → 1598.36] source so you have turned me on to a potential net data killer, and I'd like to put the question
[1598.36 → 1603.04] out to the audience you can boost in and write in and tell us what are you using to monitor the
[1603.04 → 1610.06] performance metrics like available storage CPU usage application metrics what are you using right
[1610.06 → 1616.04] now uh because I've been using net data for years, and they have been going towards this centralized
[1616.04 → 1622.84] dashboard as a service where uh it used to be each net data instance was like a self-contained
[1622.84 → 1627.58] thing, and you could kind of link all your net data instances together but that just really made it
[1627.58 → 1632.22] easy to swap between them, and now they've gone to they really just want net data to be an agent on
[1632.22 → 1635.58] your machine, and it's reporting to their dashboard, and you manage everything and then of course there's
[1635.58 → 1641.94] a bunch of upsells, and I'm just not really here for it there's a word for that isn't there uh are you
[1641.94 → 1649.32] thinking in certification I am indeed yeah, and it's also I think Was would disagree, but I also tend to
[1649.32 → 1654.86] run it on more resource constrained systems you know like raspberry pies and droids I mean that used
[1654.86 → 1662.26] to be okay that used to be okay, but now it's kind of heavy now it's such a pig yeah yeah it does provide I
[1662.26 → 1668.84] mean in net data's defence it does provide a lot of very detailed real-time metrics and collecting
[1668.84 → 1673.98] all that stuff obviously is going to require some juice you know and a brilliant interface I mean
[1673.98 → 1679.28] they did a good job with the dashboard itself it looks great, but I found a much, much more lightweight
[1679.28 → 1687.78] version over the holidays called bezel, and it's spelled kind of weird it b-e-s-z-e-l bezel that's what I'm
[1687.78 → 1693.30] going to go with and this is a lightweight server monitoring platform that can automatically scrape
[1693.30 → 1702.24] docker statistics historical data for things like disk utilization percentages and more recently they've
[1702.24 → 1708.34] added support for things like GPU monitoring, so I've put this on my Obama server for example and now
[1708.34 → 1713.30] I can see what the temperature of my GPU is doing what the utilization is because I've shared it with
[1713.30 → 1719.08] several people over tail scale and I just like to know what it's up to you know I've got it running
[1719.08 → 1726.20] across multiple hosts running across nix Debian and even on a Mac mini as well, and I'm getting all
[1726.20 → 1732.36] of these stats and it is just works it connects via ssh and I don't know there's not really much
[1732.36 → 1737.48] configuration you do you copy and paste a couple of lines and each host gets added its kind of magic
[1737.48 → 1741.34] yeah and if you do the docker compose setup you know you just have to put
[1741.34 → 1748.38] like an ssh key in there so we can log in for the agent you can also just run the binary it's also
[1748.38 → 1753.84] packaged in nix it's its mostly all a go app so you can just really you can just grab the URL of the
[1753.84 → 1758.46] binary and run it on some system, so there's a lot of flexibility there it does have a web interface
[1758.46 → 1764.20] like net data, and it looks good you know I don't think it's as comprehensive, but it still looks really
[1764.20 → 1772.50] good, and it's MIT licensed so it's open source, and it does support alerts um I don't know if you
[1772.50 → 1776.08] played around with that at all I just took a quick look at the alerts and didn't hook any of them up
[1776.08 → 1781.50] but it does have web hooks and push notifications, and it can message you on telegram if you have that
[1781.50 → 1786.74] like you've got certain options right so if you want to look at the different alerts that it can
[1786.74 → 1792.26] support it supports a notification library heavily inspired by an app we've featured on the show
[1792.26 → 1798.56] before called apprise, but this one uses a library called shouter which we'll put a link to in the
[1798.56 → 1803.54] show notes shouter and I guess that supports a bunch of different services yeah so everything
[1803.54 → 1809.52] like you said from telegram to slack to pushover to notify which is another self-hosted notification
[1809.52 → 1815.48] platform so you could have this notify your self-hosted notification platform and then from there
[1815.48 → 1821.66] have that plug into whatever you want to it supports email or notify or discord a bunch of stuff or
[1821.66 → 1831.50] even just the bulk standard generic webhook keebo.com slash self-hosted that's k eeb.io slash self-hosted
[1831.50 → 1838.94] now I had a realization a few years ago that it's worth investing in a great keyboard because I'm using
[1838.94 → 1843.98] my computer all the time and how do I interface with that what am I actually physically touching all
[1843.98 → 1851.28] the time my keyboard that's why I love keebo.com slash self-hosted we'll also have a link in the show
[1851.28 → 1856.80] notes they specialize in great keyboards including those split keyboards that really helped with my RSI
[1856.80 → 1862.52] and they also have the regular keyboards you might like and expect as well they come fully built or
[1862.52 → 1868.08] if you like you can also do a little bit of hot swapping no soldering for any of that stuff
[1868.08 → 1874.56] they also have macro pads with the 9 to 16 keys that people use for like you know a printing machine
[1874.56 → 1879.52] shortcuts you can also use it one of the ways we use it is a way to switch cameras with OBS
[1879.52 → 1883.80] or maybe like you have a home theatre machine you can use one of those little
[1883.80 → 1889.24] macro pads I think is what they call them a macro pad it's like 9 to 16 keys to control something
[1889.24 → 1894.92] you know, and I also want to mention that they have stuff for those of you that aren't a fan of the big
[1894.92 → 1900.16] clack noises so you can still get the comfort that kind of classy feel that high-end feel
[1900.16 → 1906.68] without the noise they've got those as well they also stock lots of DIY parts if you need to make repairs
[1906.68 → 1911.72] or like to build your own including microcontrollers, and they support open source and publish 3d printed
[1911.72 → 1916.90] parts so you can print the case if you need to make repairs I don't know maybe you threw it somebody
[1916.90 → 1923.48] and cracked it not saying I ever did that, and also they're part of the core team of QMK which I'm
[1923.48 → 1927.98] probably you know the least experienced person with the QMK firmware I'm aware of it I know it's
[1927.98 → 1934.14] preferred amongst the high-end keyboard community I'll just say, but I think it's really great as a
[1934.14 → 1939.78] to see that they're a core contributor to that team and all their boards use QMK as well that's
[1939.78 → 1944.66] pretty neat it's perfect to see that so support the show and go get yourself something nice start
[1944.66 → 1950.96] by going to keeb.io slash self-hosted support the show and when you go to that URL and sign up for
[1950.96 → 1957.46] the newsletter you'll get five percent off your first order keeb.io slash self-hosted
[1957.46 → 1964.18] the week before Christmas the promo team over in Vienna in Austria dropped a little Christmas
[1964.18 → 1970.08] present for some of us that we don't think any of us were expecting the promo data centre manager
[1970.08 → 1975.74] is an open source server management software which is designed to provide a unified overview of all
[1975.74 → 1983.68] nodes and clusters in a promo ecosystem hmm so it's alpha they say it's still in early stages of
[1983.68 → 1987.34] development, but we felt it was important to provide interested users with the potential
[1987.34 → 1993.58] early insights into our newest project that's great got some good news Chris too it's fully
[1993.58 → 2000.22] developed in rust oh play the horns yeah look at that the project is fully developed in the rust
[2000.22 → 2005.66] language from the back-end API server to the CLI tools and the completely new front end the front
[2005.66 → 2010.90] end is built on the new widget toolkit that we developed over the last few years, so this is
[2010.90 → 2016.82] promo coming after venter all the VMware refugees if you ask me I think this is an amazing
[2016.82 → 2022.84] development and it for me, it shows that promo have got their head screwed on properly in trying to
[2022.84 → 2028.44] do some kind of proper multi-data centre management or even just multi-host management across multiple
[2028.44 → 2034.30] clusters um I spanned this up and took a quick look at if it is you know pretty alpha it's functional
[2034.30 → 2041.48] for right now but uh it's such a great step in the right direction I can hardly even articulate it
[2041.48 → 2048.52] uh very glad to see this one get released yeah what a way to start the new year and they
[2048.52 → 2053.58] have a public roadmap too so they're they're publishing that I'll put a link to that in the
[2053.58 → 2058.74] show notes uh they have a lot on this roadmap right now it is early right it is very early but
[2058.74 → 2064.02] there's a lot they want to do in here they have a lot of ambition, so I think that's pretty awesome so
[2064.02 → 2071.46] the promo data centre manager is based on Debian bookworm it uses kernel 68125 uh you can get a
[2071.46 → 2078.70] newer kernels and opt-in, and it has support for up to ZFS 2.2.6 for the uh unit yeah they've been
[2078.70 → 2084.32] you know slowly creeping up on a full-featured solution here for enterprises for a while now
[2084.32 → 2091.26] you've got promo itself as a really top quality hypervisor these days you've got promo
[2091.26 → 2095.96] backup server which I hear from several listeners is fantastic I don't actually use it myself but it
[2095.96 → 2100.72] automates backups across hosts for containers and VMS and that kind of thing, and now you've got the
[2100.72 → 2105.86] data centre manager thing it's great well they need a proper software defined oh wait no they added that
[2105.86 → 2112.12] they added a proper software defined network in version 8 I think so blimey yeah they're ticking off
[2112.12 → 2117.08] the features over there yeah I think they're pretty sharply recognizing their window of
[2117.08 → 2124.50] opportunity here right yeah good on them yeah good on them, I say yeah if only I'm thinking back to the
[2124.50 → 2129.54] Windows 8 days and Linux and how we were talking about how Linux had a window of opportunity to
[2129.54 → 2134.62] capitalize on Windows 8 do you remember those days you know there's there's another kind of window like
[2134.62 → 2141.14] that opening up right now because um Windows 10 is coming end of life Windows 11 requires certain
[2141.14 → 2146.32] hardware oh that's right yeah the TPM stuff, and I've heard from listeners that are Windows users
[2146.32 → 2152.36] they're like I have a perfectly functional computer it does everything I need, I don't want a new
[2152.36 → 2156.44] computer and I don't want Windows 11 I don't know maybe I'm finally going to switch to Linux
[2156.44 → 2162.68] we'll see yeah maybe another window of opportunity it's really nice to see promo doing this we'll put
[2162.68 → 2170.16] links to uh both their roadmap and their announcement in the show notes could it be the year of the Linux
[2170.16 → 2170.90] desktop?
[2171.14 → 2172.88] I think it's the year of the promo server
[2172.88 → 2174.44] we'll see yeah
[2174.44 → 2179.98] we got some boosts from our listeners uh it's been a couple of weeks with the holidays and whatnot and
[2179.98 → 2185.80] the pre-records, and we're going to start with Tom's dad who sent in 26,000 SATs from the podcast
[2185.80 → 2190.84] index, and he says I have so many things to talk about number one big thanks to Alex on the epic
[2190.84 → 2197.00] server build pointers I hate getting stuck in analysis paralysis when building pcs having a quote just do
[2197.00 → 2204.78] this is great, thank you yeah well I'll co-sign that let Alex do all the hard work and then just copy
[2204.78 → 2209.74] his notes right or spend all the money and figure out what doesn't work for you yeah that too yeah that
[2209.74 → 2214.00] too and if you're is you're lucky, and you know him you can maybe buy the stuff off of yeah that's
[2214.00 → 2221.74] true that is true number two I'm currently setting up an incus uh incus which is an open source fork of
[2221.74 → 2228.00] let it looks like it can do everything the promo can do just all on the command line which just fine
[2228.00 → 2235.54] with me, but I'll keep you posted you know me I love a good command line app versus an UI, but I can't put my
[2235.54 → 2241.02] finger on it, I just can't wrap my head around incus I think I tried it a few months ago
[2241.02 → 2247.18] I talked about it on the show briefly there's some weirdness with like keys and like permissions
[2247.18 → 2251.86] for I don't know what it was maybe I should try it again maybe it's uh maybe it's come on a little
[2251.86 → 2257.06] bit yeah I agree too there's something with promo when you're dealing with a lot of systems
[2257.06 → 2261.88] it is kind of nice to have a visual overview of each one with their online with their IP just kind of
[2261.88 → 2266.64] that kind of stuff can be nice for folks well it's everything we just talked about as well it's
[2266.64 → 2272.34] it's an ecosystem now it's not just uh it's not just a hypervisor it's its many things you do want
[2272.34 → 2276.48] a competent command line absolutely though, and I suppose if you're building something, and you build
[2276.48 → 2279.80] a competent command line you can always build the other stuff on top of that okay last bit he says
[2279.80 → 2286.36] number three you need to check out the client CLI any VS Code extension it adds an interface to clod where
[2286.36 → 2291.86] you can give control of the editor and shell to the LLM and let it wow let it at the
[2291.86 → 2297.38] keyboard I've been writing nix OS tests with if it's great for refactoring your nix configs
[2297.38 → 2303.34] I love Klein he and I have been great friends over the holiday break yeah really yeah I've spent
[2303.34 → 2308.34] maybe ten dollars on API tokens with anthropic through it so um yeah yeah that's the downside
[2308.34 → 2315.20] is you it's a way to spend money in your editor instead of thinking, but it's a great tool I have
[2315.20 → 2321.96] been using zed, and it also has clod integration, and it will, you can take your whole file run it
[2321.96 → 2327.58] through clod and spit it back into the editor that's been pretty fun I'll tell you it's its
[2327.58 → 2332.10] been really great like the docker composed generator v2 stuff that I talked about earlier
[2332.10 → 2340.02] like I hate regex I hate figuring out regex always have, and I think always will, but clod just did it for
[2340.02 → 2344.44] me I copied and pasted it is didn't work I told him it didn't work, and then he came up with the right
[2344.44 → 2349.58] solution next time you know yeah so it can also be a second set of eyes like on a config that isn't
[2349.58 → 2354.66] working it is pretty handy I have to say yeah in nix particularly like with flakes or whatever
[2354.66 → 2359.16] where you're passing around configs and all the imports at the top of the file that kind of stuff
[2359.16 → 2365.26] like it's just nice to have that kind of uh hey, hey Alex you forgot that you forgot that import up
[2365.26 → 2370.26] there and speaking of nix like this is really how I kind of figure out what the nix air is even
[2370.26 → 2375.04] really telling me these days is I just throw it in the clod yeah and clod helps me figure it out
[2375.04 → 2383.72] spectrum comes in with a row of ducks 2222 SATs for syncing obsidian I use obsidian live sync and he
[2383.72 → 2389.82] links it to us, I access it via tail scale running on a nix host with the following config oh, oh well
[2389.82 → 2393.98] let me take a little look at that uh he says another option for those interested in self-hosting the
[2393.98 → 2400.12] sync and saving a few bucks I have been thinking about this I do kind of feel like the obsidian sinks
[2400.12 → 2404.46] services a little bit more than I'm comfortable paying it's a little pricey, but it does just work
[2404.46 → 2411.40] on every platform including the iPhone which for me is the killer blow I'm afraid but this one's
[2411.40 → 2417.16] pretty nice this config he's got uh sops secret uh encryption built in which is nice always good to
[2417.16 → 2423.26] see that um and then a bunch of other stuff too for uh syncing it which looks like using couch dB
[2423.26 → 2431.38] underneath very nice I had a devastating loss of uh images that I captured in obsidian I went
[2431.38 → 2437.06] through the PDF for the manuals for all of my vehicles including the RV for all the anything
[2437.06 → 2443.74] pertaining to maintenance anything that shows gear diagrams tables and I screenshotted all of it or I
[2443.74 → 2449.48] copied the text and I put it into a whole series of notes into obsidian and for some reason the images
[2449.48 → 2454.58] never synced and a lot of that stuff was in the images, and it's really stank, and I don't
[2454.58 → 2458.54] know why because I'm using obsidian sync I don't know what I must have done something wrong but uh
[2458.54 → 2464.98] well there was a checkbox I don't know if it applied to images or files over a certain size
[2464.98 → 2469.66] where yeah that does it didn't use to sync them by default I think it does now
[2469.66 → 2475.94] maybe you just ran into that maybe but uh thanks for the links yeah appreciate it thank you
[2475.94 → 2481.20] expectorants bam, bam comes in with 5 000 SATs that's a jar boost hey you know when you ship
[2481.20 → 2486.20] a pc you could actually put a dab of hot glue on the cables and parts you expect to come undone you
[2486.20 → 2492.92] don't have to overdo it um they also sell this expo expanding foam bags for shipping that you can pop
[2492.92 → 2498.50] a capsule on, and then it fills a void primarily useful for ensuring things like GPUs don't move around
[2498.50 → 2502.90] too much and stress the PCI slot, but it can also help ensure everything's just kept in place
[2502.90 → 2508.24] finally keep track of a screw count and where they go last thing you want is a screw to come
[2508.24 → 2513.88] loose and find a way to get stuck under an droid and then short it out I wonder if he's had that
[2513.88 → 2519.86] happen hey this thing didn't use the rattle right you know I remember when we toured the system 76
[2519.86 → 2528.46] factory and how much work they put into just building the machine so it could sustain through shipping like
[2528.46 → 2532.30] even just like the actual like parts that were permanently installed in that thing like to hold the
[2532.30 → 2536.28] graphics card in place and whatnot were really there just to get it through shipping do you remember
[2536.28 → 2542.14] this yeah custom foam blocks as I recall and that too I think it's easier for them because obviously
[2542.14 → 2548.96] they're doing it at scale, and they know what shape uh desktop is in their world like every time it's the
[2548.96 → 2556.60] same it's much harder for a one-off situation, and I've heard of this kind of expanding foam shipping
[2556.60 → 2562.80] bags I guess before it must be on Amazon yeah and I can, I considered it but shame just wanted to throw
[2562.80 → 2568.04] in the underneath of the airplane and YOLO it, so thankfully everything was fine, but you know
[2568.04 → 2574.82] yeah a bronze wing comes in with a row of ducks and says I got a cautionary tale using cast-o-magic
[2574.82 → 2580.16] they write I watch Alex's YouTube channel and obviously listen to this podcast because of YouTube I have
[2580.16 → 2586.58] open sense and home assistant I've also bought a ubiquity PDU pro, and it's been awesome
[2586.58 → 2592.54] for my mini rack I also use the home bridge to expose my home assistant entities to Siri I was lazy
[2592.54 → 2600.78] and didn't exclude specific items from my home bridge I recently made all of my light switches smart and all
[2600.78 → 2605.94] my light switches smart uh with Zeus Z-Wave switches my kids use Siri to turn on and off the lights
[2605.94 → 2612.28] and somehow they managed to hard shut down my entire server rack by yelling at Siri oh that is an
[2612.28 → 2620.40] attack vector that infosec people everywhere are not thinking about I guarantee it I did this once
[2620.40 → 2627.48] and it was bad so you do have to consider home kit connectivity, so I after Jeff and I wired up
[2627.48 → 2635.16] my water pump to the ESP32 controllers I said hey s-tube turn on the water pump right because that's
[2635.16 → 2640.72] what I named the device and I figured that's pretty cool I can now turn the water on off by voice and
[2640.72 → 2648.42] what happened was every switch in home assistant got toggled on so anything and if you think about
[2648.42 → 2652.28] all your little devices that have like lights on them that home assistant has a switch for
[2652.28 → 2660.96] or in my case cameras that have sirens and all of them have sirens I can see where they all went off
[2660.96 → 2668.32] and so every light turns on every heater turns on the noisemakers turn on the TVs turn on and
[2668.32 → 2676.68] a dozen sirens blare all at once because I told the s-tube to turn on the water pump so yeah you do
[2676.68 → 2684.70] need to be careful it was very embarrassing oh but glorious also yeah yeah yeah all right Fredrick
[2684.70 → 2690.80] rounds us out with a space balls boost 12,345 SATs, and he writes hey guys long time listener
[2690.96 → 2697.42] creator of stream fin here stream fin all right yeah we talked about that in a couple of episodes
[2697.42 → 2704.72] ago didn't we and I'm still loving it uh self-hosted is my all-time favourite podcast it's my morning
[2704.72 → 2709.92] commute it's my bedtime can't sleep podcast it's my safe space I've never boosted it in those since
[2709.92 → 2714.56] I've been a student and cash has been tight but now that stream fin is getting some donations I can
[2714.56 → 2718.42] take a portion of that and give it back to the community so here's my small gift to you for making a
[2718.42 → 2722.50] great podcast also please check out the latest version of the app we're really pumping out new
[2722.50 → 2729.80] features next up is jelly seer integration oh that's landed I just loaded up the app right
[2729.80 → 2737.34] here and jelly seer plugin is alive and well and let me tell you Frederick that is a hell of an
[2737.34 → 2742.52] addition great job great great great job yeah you know it would draw my attention to it right built in
[2742.52 → 2747.34] intro skipping of course the brand-new trick play image support which was kind of new to jelly fin
[2747.34 → 2752.56] you can background the audio which you can't do with the regular jelly fin app I don't know why
[2752.56 → 2756.64] and you can download media it's got Chromecast support and like Alex said now it's got jelly
[2756.64 → 2761.76] seer integration as well so you can request new media directly in the app which family's going to love
[2761.76 → 2765.84] thank you, Frederick, it's uh really great to hear from you and really appreciate the space balls boost
[2765.84 → 2771.56] and keep up the great work happy users here that jelly fin ecosystem just keeps on giving doesn't it
[2771.56 → 2777.36] yeah it's I mean we could have switched earlier and probably should have, but boy did we pick a good
[2777.36 → 2783.08] time it's been it's been great did you see the intro skipping is added I think in the android app now
[2783.08 → 2789.14] yeah and in infuse it's officially in the infuse client which is your know my favourite front end
[2789.14 → 2795.64] with a button it's so great Alex it's everything I ever wanted, and I feel like it's I don't know
[2795.64 → 2802.84] kind of even better than plexus because um there's room for other types of skipping because of this way
[2802.84 → 2809.00] it categorizes the segment so it's like even a better system mm-hmm ah it's its open source and
[2809.00 → 2813.96] obviously they have second mover advantage as well, and you look at how the incumbent did it and be like
[2813.96 → 2820.12] well what if they added this feature yeah very true, and I really appreciate that it just
[2820.12 → 2827.32] works perfectly offline so all right to wrap us up thank you everybody who boosted in we really
[2827.32 → 2833.80] appreciate it 45 of you stream SATs as you listen, and we stack 60,614 SATs when you combine that with
[2833.80 → 2837.80] the boosters out there of course we can only fit so many in the show, but we will have the boost barn
[2837.80 → 2845.48] in the show notes, and we do read all of them we had 60 boosters, and we stacked a grand total of 154,894 SATs
[2845.48 → 2851.00] thank you everybody who boosts with something like the fountain app or with your own self-hosted setup
[2851.00 → 2857.80] it's really appreciated and episode 140 was made possible because of you and our members
[2857.80 → 2867.24] ubiquity started the year off right with a release of unify network 9, and they've added a zone based
[2867.24 → 2875.40] firewall to all the ubiquity firewall stuff so is this like a DMZ of sorts well DMZ
[2875.40 → 2881.32] is part of the zone what is one of the zones that you can create essentially if you think
[2881.32 → 2888.20] of it like one of those tables where you're like uh this person can see this person, and you click on
[2888.76 → 2895.96] the cross-section of like VPN and DMZ, and then you can click on that button, and it will show you all
[2895.96 → 2902.12] of the rules that pertain to that particular zone grouping okay now I could really see how that'd be
[2902.12 → 2908.92] great for like a business or an office space or even I don't know yeah even a home lab it's so i
[2908.92 → 2914.84] switched to the UDM pro when I got fibre a few weeks ago months ago now I guess just to really
[2914.84 → 2918.04] try it out you know I've got everything else unify in this house I thought I may as well give the
[2918.04 → 2924.52] firewall a go I was a bit lukewarm to it at first but I tell you what you know co-locating
[2924.52 → 2928.84] Shane's infrastructure here and having the plans all in one place just a couple of clicks
[2928.84 → 2934.76] and then you know just spit splitting out all the tail scale infrastructure I've got into its own
[2934.76 → 2940.28] separate VLAN and like I didn't ever really end up using plans with open sense because they were just
[2940.28 → 2946.52] a bit more complicated than I felt like I could be bothered to learn about but in the unify world
[2946.52 → 2951.32] it's its really easy, and now this zone based firewall makes it even easier to keep track of this you know
[2951.32 → 2956.60] I've got nearly 10 plans on this network now I upgraded a couple of days ago, and it's been the
[2956.60 → 2962.92] upgrade was flawless and the features yeah it's its putting it on par with firewalls that used
[2962.92 → 2969.24] to cost 10 times what the unified gear costs now yeah yeah and I do like this idea of the zone based
[2969.24 → 2976.04] firewall right because you're essentially you're reducing what could be a ton of rules down to just
[2976.04 → 2981.16] a concise set of zones and that makes it way simpler to manage I would imagine yeah you just think
[2981.16 → 2989.64] right well what can access the LAN click on the button oh yeah I see yeah very easy oh boy I know
[2989.64 → 2996.36] I'm going to get sucked into unify and then eventually the cameras yeah I do so they added support for
[2996.36 → 3003.48] third-party cameras on if cameras oh good uh into their connect software uh well just in December I think
[3004.12 → 3010.44] maybe November fairly recently anyway um so yeah I've I've been meaning because I'm still running blue iris and
[3010.44 → 3018.60] have been for like six years, and it's fine it does the job I guess but like you know all the seeds
[3018.60 → 3024.04] been planted how it is right yeah particularly doing this podcast like it's all it's all part of the job
[3024.04 → 3029.08] you know I mean I'm looking at the cameras myself and I'm thinking well if I have the cameras then i
[3029.08 → 3034.52] probably should have the network gear, and so I should probably start with all unified network gear and then i
[3034.52 → 3039.40] could get the cameras and if I got the cameras then I should probably get a video recorder we just need
[3039.40 → 3044.20] unified response to this podcast no it's getting ridiculous how many devices I have on this network
[3044.20 → 3049.16] now honestly yeah we need to do a need to do like a unify makeover you know like a home
[3049.16 → 3054.52] makeover oh yeah yeah yeah all unified gear our podcast network runs on unify yeah let's do that
[3057.00 → 3061.96] uh I want to take a moment and just say thank you to our SRE subscribers you do make the show possible
[3061.96 → 3066.84] as a thank-you we have an ad-free version of the show that also comes with additional content
[3066.84 → 3071.64] a special post show that we make only available to our members either for the network party members
[3071.64 → 3078.28] or for our sees, and you can sign up at self-hosted. Show slash SRE and put your support on autopilot
[3078.28 → 3083.64] and get an ad-free experience it might be time for the golf to go we'll talk about that in today's
[3083.64 → 3090.28] post show we'll see we'll see hey I want to plug colony events.com we're making plans for up 600 and
[3090.28 → 3094.92] we're encouraging the audience to host their own meetups and then jump on mumble and have a listen party
[3094.92 → 3102.28] so details are at colony events.com for that yeah that's coming up fairly soon actually second of
[3102.28 → 3110.84] February so do keep an eye on that oh freaking me out it's freaking me out yeah well one of your
[3110.84 → 3115.72] children's growing up dude you know they grow up so fast yeah it is older than a couple of my children
[3115.72 → 3124.20] really yeah I think so maybe and maybe, maybe only one but uh yeah it's its wild 600 episodes is wild
[3124.20 → 3129.48] you know and I don't know it just feels like it's going to be a big episode never I was going to never say
[3129.48 → 3133.96] missed a week apart from when you had your uh yeah, but the show didn't miss a week the show didn't miss
[3133.96 → 3141.32] a week no amazing links to what we talked about today are at self-hosted. Show slash one four zero you're
[3141.32 → 3146.12] going to find our contact page over there as well as our RSS feed and of course the back catalogue of
[3146.12 → 3153.08] all the great episodes you can find me on the internet at alex.ktz.me I'll be at Chris las.com
[3153.08 → 3158.28] come say hi on the wild side what is the wild side these days is that blue sky now no it's not
[3158.28 → 3162.60] because it's the wildest of all of them uh you know I am on weapon x too but i only really kind
[3162.60 → 3166.20] of reply to people over there and the show's got an account over there if you want to be notified at
[3166.20 → 3170.20] self-hosted show when the new episode indeed but you probably have a podcast player that
[3170.20 → 3175.00] it probably tells you that so you probably don't need to follow an x account uh what a time to be
[3175.00 → 3179.56] alive thanks for listening everybody that was self-hosted. Show slash 140
