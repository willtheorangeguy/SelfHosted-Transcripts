[0.00 → 4.58] Coming up this week, Chris and I share some of our top tips for getting started with self-hosting,
[4.94 → 6.66] and we cover some network basics.
[7.08 → 9.32] And we definitely don't talk about Home Assistant.
[9.66 → 9.88] Promise.
[10.56 → 11.08] I'm Alex.
[11.36 → 13.76] I'm Chris, and this is Self-Hosted 17.
[14.98 → 16.06] Well, hello, Alex.
[16.24 → 17.50] Welcome to Self-Hosted 17.
[17.68 → 20.50] Did you have to turn off the 3D printers for this episode?
[20.82 → 21.86] I did, yeah.
[21.94 → 25.26] I've just about got to my thousandth head shield, face shield thing.
[25.62 → 29.18] And I've got another printer that's been donated by somebody else.
[29.18 → 31.80] There are two more downstairs, so I've got five in the house now.
[32.16 → 34.10] So your house is really a manufacturing plant, is what you're saying?
[34.32 → 35.14] Yeah, it's kind of crazy.
[35.28 → 35.86] I'm kind of done.
[36.20 → 37.40] I'm so bored with 3D printing.
[37.82 → 38.22] I bet.
[38.42 → 38.88] I bet.
[39.02 → 41.28] I wonder if you're going to have to take a break after this.
[41.40 → 41.62] You know what?
[41.64 → 42.64] Just ship them up here.
[43.54 → 48.68] Well, I was going to take one of them with me to Linux Fest Northwest, but sadly.
[49.24 → 50.92] That's, no, that's not happening.
[51.54 → 54.64] So did you end up watching old Picard off my Plex server last night?
[54.82 → 55.70] Not yet, no.
[55.98 → 58.32] Well, we do have a little Plex news regardless.
[59.18 → 63.88] You and I, being Plex buddies, we'll often talk each other into a show and then just say,
[64.00 → 65.18] yeah, go watch it off my Plex.
[66.24 → 71.32] The one I've been watching this week is The Tiger King, which is actually on Netflix, not Plex.
[71.88 → 73.20] Everybody's been watching Tiger King.
[73.48 → 74.82] I can't believe that dude is real.
[75.06 → 75.72] Oh, I can.
[75.78 → 80.34] I can just because I've seen some crazy stuff just in the podcasting space.
[80.50 → 85.14] So I can only imagine that getting amped up in the Tiger Zoning space.
[86.02 → 87.94] Because you wouldn't believe some of the things I've seen.
[87.94 → 91.14] There are niches for people within niches.
[91.36 → 94.88] And these guys, there's like a clique of three of them.
[95.40 → 97.52] And they're all at each other's throats the whole time.
[97.80 → 99.80] But anyway, we digress slightly.
[99.80 → 103.20] The Plex news this week is they've released a couple of apps.
[103.60 → 105.68] One of them is called Plex Dash.
[106.16 → 112.44] And this thing, if you've ever looked at the dashboard on your Plex server, I think it came out maybe a year ago.
[113.08 → 120.36] You can see who is streaming what from your server and how much CPU is being used and a basic history of your most popular content.
[120.36 → 126.68] Well, they've brought this now to an Android and I think iOS app, which you can install on your phone.
[127.14 → 128.30] And I kind of like it.
[128.34 → 133.84] It's pretty bare bones compared to something like Tautly, which is another alternative in this space.
[134.56 → 136.26] But, you know, it does the job.
[136.26 → 138.00] Yeah, and having it built in is really nice.
[138.24 → 151.72] What got my attention, though, in the recent Plex news was the announcement of Plex Amp version 3, which I think is going to kill Prism on my mobile device, which is what I used in the past to stream my Plex music.
[152.16 → 153.96] This app is impressive.
[154.14 → 158.74] They're using Opus on the back end to get really high quality audio streaming in certain conditions.
[158.74 → 161.30] It's pre-caching upcoming tracks.
[161.68 → 164.38] I wish every freaking music player on mobile would.
[164.88 → 166.42] And the interface looks perfect, too.
[167.08 → 173.22] And, you know, one of the number one questions we get into this show is how can I self-host my music collection?
[173.54 → 174.98] And not everybody likes it.
[175.06 → 178.22] They really, really don't like it sometimes when we say Plex.
[178.54 → 182.62] But this is the sort of thing that Plex does that other projects can't quite match.
[182.62 → 186.46] And for those of us that use Plex to manage, like myself, this is what I do.
[186.46 → 190.68] I manage my audiobooks and my music collection on Plex.
[191.26 → 193.58] Audiobooks work kind of okay.
[194.18 → 199.84] There is a checkbox you can set in the Plex settings to remember last listened position.
[200.40 → 210.20] The only problem is if you have your book split up into chapters, if you get to more than 80% in a chapter, or is it 90%, it considers the video or the audio track as watched.
[210.20 → 216.74] So if you're in that last couple of minutes of a chapter, you will lose your place, which is kind of annoying.
[217.52 → 222.48] And it's been a request of mine on the Plex pass get to vote on features.
[222.70 → 224.36] I think I asked for that like six years ago.
[224.52 → 225.56] So come on, Plex.
[226.02 → 226.68] Let's do that.
[227.14 → 229.52] But to solve the audiobook problem, I actually use Book Sonic.
[229.94 → 233.08] And my wife devours audiobooks like a monster.
[233.64 → 235.00] And she loves Book Sonic.
[235.38 → 235.80] The monsters?
[236.10 → 238.20] Are they known for devouring books?
[238.20 → 240.04] I think they're known for devouring other things.
[240.38 → 241.60] Don't question the analogy.
[241.84 → 242.08] Okay.
[243.20 → 250.82] Yeah, I also think it's perfect for Plex from an image standpoint to be seen doing these kinds of things because it counters that it's for piracy narrative.
[251.62 → 256.84] That will have trickle-down effects to MB and all the other projects that we've talked about on the show.
[256.90 → 260.64] Even things like Jodi, which aren't necessarily directly connected.
[260.64 → 267.04] But Plex taking this on and saying that self-hosting for other things besides the stuff you downloaded off the internet.
[267.64 → 269.10] It's perfect for all these projects.
[269.64 → 272.06] And I'm not super keen on Plex Amp.
[272.24 → 273.66] I'm going to just put that out there.
[274.00 → 275.76] I think it looks beautiful.
[276.16 → 281.24] I use Prism currently, which is a third-party app that is a really nice music player for Plex.
[281.48 → 283.22] So that's what it's up against.
[283.22 → 286.22] Yeah, I just found this a little confusing.
[287.12 → 294.52] Some of the design decisions they've made, if you look at the philosophy behind it, they say that applications should have a raison d'être.
[295.02 → 298.10] For Plex Amp version 3, it came down to these.
[298.68 → 300.94] Play music fast and don't stop.
[301.66 → 309.60] And Elon argues in his Medium post, which we've linked in the show notes, that this sounds like a simplistic set of goals, but it actually informed a lot of their design decisions.
[309.60 → 319.98] And I don't really use Plex for music all that much, so I don't have a huge amount of data for it to sort of trawl through and look at my listening history, which I think might be counting against me here.
[320.14 → 336.72] Because when I click on stuff like Artist Radio for Tool, you know, a heavy metal band, it played My Name Is by Eminem, which isn't really what I would consider in the same genre or even in the same multiverse as Tool.
[336.72 → 340.32] And then the next track it played me was a badly drawn boy track.
[340.46 → 342.12] So again, just weird.
[342.92 → 351.00] But I think maybe if people have a lot of databases for it to mine data from, you know, history going back a couple of years, then it's probably going to do okay.
[351.52 → 358.56] See, for me, somebody that is often driving around in the Pacific Northwest where we have large gaps of no coverage, because when you go through the forest and whatnot,
[358.84 → 364.36] having a music player that caches offline and pre-caches sort of closes those gaps.
[364.42 → 365.20] It's really nice.
[365.20 → 366.64] That bit's really cool.
[366.96 → 367.14] All right.
[367.16 → 368.92] And you can configure it up to 40 tracks.
[369.00 → 375.96] It says in the settings, it will pre-cache 40 tracks when it hits some connection for a few minutes, which I think is actually pretty cool.
[376.74 → 379.04] The interface as well is really nice.
[379.14 → 381.70] Like I'm going to show you on the on our cam.
[382.24 → 385.28] It renders out the waveform and then that's the progress bar.
[385.36 → 387.32] And that I really like too, because I'm an audio geek.
[387.58 → 388.20] Yeah, that's pretty cool.
[388.20 → 389.72] And look, it has potential.
[390.06 → 397.18] And this is something that Elan was telling us about when we interviewed him back on SSH, I don't know, zero or whatever it was a lot of while ago.
[397.82 → 398.88] It's got potential.
[399.10 → 400.64] Maybe I need to spend a bit more time with it.
[400.70 → 405.90] My initial reaction is, oh, this is a bit complicated compared to say like Spotify or something.
[405.90 → 413.62] But over time, if I actually use it, I'll be interested to see how it kind of marinades and matures with my tastes.
[413.92 → 415.84] So I'm not going to write it off.
[416.24 → 418.54] But right now it's a bit weird.
[419.16 → 427.56] I like that they're doing it because it does make that answer when you tell people, well, Plex is something you could look at for self-hosting your music.
[427.56 → 431.48] Like there's a lot of solutions there, but only one or two of them are really worth your while.
[431.52 → 432.68] And I think Plex is one of them.
[432.86 → 435.10] And this just makes that a little bit more complete now.
[435.10 → 450.10] So if you want to find out a bit more about the kind of thought process behind how this application was created, there is a blog post from Elan from Plex in the show notes, both for Plex Dash and for Plex Amp.
[450.76 → 452.80] And, you know, take a look in the show notes.
[453.26 → 455.10] Self-hosted. Show slash 17.
[455.10 → 455.62] 17.
[455.82 → 458.18] Now, Alex, will you join me over here in the Homeys Admin corner?
[458.52 → 458.92] Sure.
[459.02 → 459.22] Hold on.
[459.24 → 460.68] Let me just get my hat.
[460.90 → 461.62] Yeah, roll on over.
[462.62 → 479.64] I was talking with Brent yesterday about some basics of how to, you know, monitor cron jobs and understand how if you set up a bunch of automation on your home server, how do you know whether it's actually doing what you told it to in six months time?
[479.64 → 487.48] Because I'm not going to log in every day and check, you know, var log messages or whatever it is and see whether my cron job is silently failing or not.
[487.82 → 490.62] Well, enter healthchecks.io.
[490.62 → 494.48] It's billed as a simple and effective cron job monitoring solution.
[494.64 → 500.40] It receives alerts when your nightly backup, your weekly reports, and your cron jobs don't run on time.
[500.40 → 510.64] This is something a lot of sysadmins might build into an enterprise system where they, something I did, just speaking from experience, was would have mailboxes that all the alerts would get sent to.
[510.70 → 514.36] We would share that mailbox across the team and market read.
[514.36 → 521.58] But you had to check in on it because otherwise these things just silently message in your log, and you are none the wiser.
[522.02 → 523.52] The way it works is really simple.
[523.82 → 530.68] You have your normal cron job as you normally would, and then you put an and and and then curl to a specific URL.
[531.04 → 536.32] And that URL contains a token in it, which health checks knows is your token.
[536.32 → 548.66] And if it doesn't receive that ping within a certain time frame, you know, a week could be every day, whatever you configure it to, which is something you do in the settings, it will then email you and say, hey, this cron job is down.
[549.26 → 550.06] That's all it will do.
[550.10 → 554.20] It won't go and fix it for you, but it just alerts you that it's that it's down.
[554.84 → 558.46] The special sauce might be the interface to configure all of this.
[558.64 → 562.46] Like you said how you can configure if it's been like this for a week or a day or an hour.
[562.86 → 565.36] That UI is you can almost describe it as beautiful.
[565.36 → 566.12] It is.
[566.34 → 570.72] And then it has one more trick up its sleeve, which is why we're talking about it.
[570.96 → 571.78] You can self-host it.
[572.16 → 572.34] Yes.
[572.58 → 581.20] Self-hosting it is especially nice because someone like me who has everything behind my firewall, I can aggregate all of this in one spot.
[581.34 → 584.10] So I don't have to run healthchecks.io on each system.
[584.34 → 587.38] They all aggregate into one place, and then I can sort it from there.
[587.44 → 593.46] And that behind my own land where nothing ever has to talk to the Internet to do this is, well, that's just the sweet spot, Alex.
[593.78 → 594.84] Yeah, it's pretty great.
[594.84 → 597.86] It integrates with, I don't know, I'm trying to count.
[598.20 → 600.26] It must be like 25 different services.
[600.88 → 606.40] Stuff like Telegram, WhatsApp, SMS, email, of course, Ops Genie, Microsoft Teams.
[606.74 → 608.94] Slack, Discord, Matrix.
[608.94 → 610.86] Literally everything you could think of.
[611.44 → 613.22] This thing will be able to just send you a message.
[613.66 → 615.00] So I think it's really useful.
[615.00 → 622.54] I can't really underscore that enough because for me, it has to be somewhere that I am actively checking every day for me to see it.
[622.64 → 629.00] And so for work, often I will pipe things into Slack because when I'm in work mode, I open up Work Slack, and I'm in there.
[629.22 → 631.34] And that's where I'll pipe messages I need to see.
[631.34 → 635.66] And I will go to the process of automating as many of those types of things as I can.
[635.96 → 637.38] Even emails from certain people.
[637.66 → 642.90] I know that sounds ridiculous, but certain emails I have set up to ping me in my Work Slack.
[643.24 → 643.82] Well, thank you.
[643.86 → 645.48] I'm glad you take my emails so seriously.
[645.88 → 646.34] Of course.
[646.80 → 647.32] You're, obviously.
[647.58 → 648.68] No, you're in my Mattermost.
[649.08 → 650.56] You get pinged in my Mattermost.
[650.84 → 651.78] Which you never open.
[652.66 → 652.88] What?
[652.88 → 654.00] Oh, right.
[654.70 → 658.90] No, I'm too busy on our Discord these days, which has been just crackalacking great.
[659.14 → 659.38] Oh, yeah.
[659.42 → 660.98] You've got to plug the old Discord skis.
[661.28 → 661.48] Yeah.
[661.76 → 667.26] Go to self-hosted. Show slash Discord, or we have a link-up at the top of the self-hosted page.
[667.62 → 670.50] I just mention it because really cool community in there.
[670.92 → 673.74] And I'd put out a question recently on an episode.
[673.86 → 675.16] Got some great answers in there.
[675.30 → 680.46] People were showing me some really nice arm boards that I'm drooling about these days.
[680.90 → 682.72] We're over 500 people on Discord.
[682.88 → 683.82] Can you believe that?
[684.26 → 684.58] No.
[685.00 → 685.32] Really?
[685.56 → 686.02] That's crazy.
[686.32 → 689.14] It does feel like a lot's going on in there, but in a good way.
[689.40 → 691.34] Yeah, I'm getting a lot of pings, which is fine.
[691.56 → 692.78] I mean, that's kind of why we set it up.
[692.86 → 695.52] But maybe I need to do some notification management soon.
[696.84 → 697.20] Yeah.
[697.42 → 700.86] I was on a work meeting call, and I was getting the bloop from Discord.
[700.98 → 701.30] But bloop.
[701.36 → 702.72] And I'm like, oh, yeah, right.
[702.98 → 704.60] That's that's the thing I got to now.
[704.94 → 705.36] I got to remember.
[705.44 → 706.24] I got to turn that off.
[706.24 → 712.80] I had an Ask SSH or SSH 101 request from Rob Moore at RM54x on Twitter.
[713.60 → 717.76] I'd like to be able to experiment with more of your topics if there was a baseline primer
[717.76 → 719.26] for beginners to get us up to speed.
[719.84 → 725.20] Maybe something like a domain or an SSL or reverse proxy walkthrough with maybe a video
[725.20 → 725.86] or screenshots.
[726.82 → 729.68] Something like a self-paced container boot camp.
[729.94 → 731.56] Call it SSH 101, if you will.
[731.78 → 732.50] Thanks, Rob.
[732.78 → 734.34] I like the name SSH 101.
[735.14 → 738.06] Although most people outside the show would think that's probably something else entirely.
[738.48 → 738.78] Yes.
[738.94 → 739.20] Yeah.
[739.24 → 740.24] I'm a bit worried about that.
[740.32 → 741.78] So let's just call it self-hosted 101.
[742.48 → 746.32] Now, one of my previous projects that I was involved in quite heavily was Linux Server
[746.32 → 746.58] IO.
[747.22 → 752.98] And one of the key things that we tried to do with that project was have really great documentation
[752.98 → 759.40] aimed at people who were not, you know, doing this for a day job, maybe, or were just getting
[759.40 → 760.26] into it to start with.
[760.26 → 764.50] There are a couple of links in the show notes to things that we hosted over at Linux Server.
[764.68 → 766.30] Docs.linuxserver.io.
[766.62 → 770.78] There's a huge amount of information on there about how to, you know, do basic stuff like
[770.78 → 777.58] spin up a container or how to use Docker Compose or understanding PAID and PAID.
[778.16 → 782.48] All that kind of stuff, which might sound a little bit complicated to get started with.
[782.80 → 785.36] It's all laid out there, I think, in a really clear way.
[785.48 → 788.26] There's not much documentation, but what's there is nice and simple.
[788.26 → 793.04] And the other one I would recommend, coming back to your reverse proxy question, is the
[793.04 → 798.10] Nginx Let's Encrypt Starter Guide written by Antalya on the Linux Server blog.
[798.74 → 804.18] Back in April last year, Antalya wrote probably the most comprehensive Nginx guide, I think,
[804.32 → 806.80] on the internet aimed at this segment of people.
[807.64 → 811.66] It's quite the lengthy read, but there's a lot of detailed information in there about
[811.66 → 816.30] how to configure Nginx, how to configure Let's Encrypt with that Docker image.
[816.30 → 822.80] And by the end of it, you should be in a position to have any service behind your firewall exposed
[822.80 → 826.70] through a reverse proxy with an SSL certificate for free.
[826.98 → 829.38] If I can't give you a better sales pitch than that, I don't know.
[829.62 → 831.58] But I think it's a great piece.
[832.06 → 836.80] You and I are also always talking about the possibility of doing some live stream walkthroughs
[836.80 → 839.64] or recording an extra thing here or there.
[839.64 → 844.12] We are also aware that there's a lot of already really well done stuff, which I think is the
[844.12 → 848.80] point Alex is just making on the internet that we can be an aggregator for as well and point
[848.80 → 852.22] you in those directions and tell you, yes, this is a good one or no, that's a bad one.
[852.50 → 854.48] So that's also a role we can play in that.
[854.54 → 855.08] So it's a mix.
[855.50 → 858.40] And it's something we actually are talking about more and more these days.
[858.40 → 864.24] And I would really strongly encourage you to, no matter how simple it seems to you, to
[864.24 → 867.60] write it down in a public facing format.
[868.14 → 870.30] This is how I learn personally, I guess.
[870.38 → 871.38] So take it for what you will.
[872.20 → 877.92] But when I have to explain something to somebody else, that's when I learn, when I figure out
[877.92 → 879.98] how much I don't know about something generally.
[880.44 → 880.86] Absolutely.
[880.86 → 886.38] Once you learn how to explain something simply to someone else, you generally pretty fully
[886.38 → 886.98] understand it.
[887.06 → 891.70] And it's one of the metrics I use to, before I go on the air to like to explain a complicated
[891.70 → 895.94] subject is I try to see if I can distill it down into three sorts of key points.
[896.78 → 900.98] And I also, the funny thing about writing it down online is every now, and then you'll do
[900.98 → 903.74] Google search, and you'll come across your own post.
[903.88 → 904.70] Has that happened to you?
[905.04 → 906.20] That's funny when that happens.
[906.38 → 906.52] Yeah.
[908.08 → 908.98] Also annoying.
[909.58 → 909.82] Yes.
[909.82 → 911.48] Oh man, am I really that?
[911.68 → 912.76] Oh, Geez.
[913.56 → 913.92] All right.
[913.96 → 914.98] Well, let's go read what I said.
[915.78 → 921.40] I have been experimenting with various kinds of ARM boards recently, as you know.
[921.92 → 927.18] And I just thought while we're talking about beginner hardware, I want to give a mention
[927.18 → 935.48] that with the release of Ubuntu 2004 long-term support, they are officially supporting the Raspberry
[935.48 → 937.52] Pi 4 64-bit version.
[938.14 → 940.02] And it's perfect.
[940.34 → 940.66] Ooh.
[940.66 → 946.02] If you're looking at running server services on a Raspberry Pi Raspbian's, I think a very
[946.02 → 947.98] good desktop distribution.
[948.18 → 953.90] But I think Ubuntu LTS may have it slightly beat because not only do you have live patching,
[954.00 → 959.90] but you also have, if you want, you can, I think for five machines, do Landscape Canonical's
[959.90 → 965.80] management solution, which is a nice way to centrally manage and audit your servers, which
[965.80 → 969.26] is what I'm going to do when I get all of them on 2004, is I'm going to enrol all of
[969.26 → 971.06] them in Landscape and manage them that way.
[971.06 → 978.38] Now, that being said, Alex, can you guess what I have in my hot little hands right now?
[978.44 → 979.24] Can you guess what that is?
[980.46 → 981.26] Got any guesses?
[981.98 → 982.92] Sounds like a doorstop.
[983.50 → 989.30] It is the aluminum housing with a built-in heat sink for the Pine 64 Rock Pro 64.
[989.66 → 990.26] Oh, yeah.
[990.86 → 994.52] And I've been doing some experiments with that little board recently.
[994.94 → 995.20] Oh, yeah.
[995.24 → 997.06] This week's UP was perfect.
[997.26 → 998.10] That was so much fun.
[998.10 → 1002.52] Well, you, I don't know how much of it made into the final edit, but at one point you spun
[1002.52 → 1008.68] up 10,000 simultaneous connections from three separate geolocation to the Pine 64 to see
[1008.68 → 1009.40] what it could handle.
[1010.36 → 1011.80] And it did really well.
[1012.48 → 1013.74] I used X-Pain to do that.
[1013.84 → 1015.14] Carl George put me onto it.
[1015.56 → 1021.30] And so Chris had this little ASCII art text version of Star Wars, which I was probably Was,
[1021.34 → 1024.12] actually, not you, but Was set this thing up on the Rock Pro.
[1024.22 → 1025.22] Is it the Rock Pro 64?
[1025.68 → 1026.14] Is that what it's called?
[1026.38 → 1027.64] Yeah, and it was just a Docker container.
[1027.64 → 1029.46] There are several different ones out there.
[1029.68 → 1032.26] We link to it in the show notes so you can run other movies as well.
[1032.60 → 1038.54] And this thing is special because it has an NVMe SSD in it, which is one of the big criticisms
[1038.54 → 1043.22] that you can level against the Pi really is that it's really, really hamstrung by that
[1043.22 → 1044.36] SD card these days.
[1044.58 → 1045.70] Yes, very much so.
[1046.20 → 1046.88] Very much so.
[1046.90 → 1049.04] And even then you're still limited in your options.
[1049.04 → 1056.46] So what I've done with Ubuntu 2004 on the Raspberry Pi 4 is to avoid that SD bandwidth limitation,
[1056.60 → 1057.92] which is just horrendous.
[1058.26 → 1062.42] On Ubuntu 2004's kernel, you can now boot from a USB device.
[1062.54 → 1064.62] You can load from the USB device.
[1064.70 → 1065.56] So I do that now.
[1066.20 → 1067.80] The kernel looks for a disk label.
[1068.00 → 1071.20] That disk label is on the USB drive instead of the SD card.
[1071.28 → 1072.24] And it boots from that.
[1072.24 → 1073.30] And it's as simple as that.
[1073.42 → 1078.04] And it's significantly faster, but it's still USB three speeds.
[1078.60 → 1082.86] That's where the Rock Pro 64 has a little bit of special sauce for self-hosting.
[1083.34 → 1089.98] Because it has a PCIe 4X slot, you can put a full-fledged NVMe adapter in there,
[1090.06 → 1094.44] or a SATA adapter with multiple ports, or a gigabit NIC.
[1094.44 → 1099.60] I put a Western Digital NVMe in there, and it's been running great.
[1100.08 → 1103.22] I really want to experiment with an HBA card in there or something,
[1103.40 → 1104.80] and then attach eight hard drives.
[1105.00 → 1106.66] Although I'm not sure how I'd power them.
[1107.38 → 1109.20] But I still want to try it, you know?
[1110.26 → 1113.80] It was incredible performance once you remove the I.O. bottleneck.
[1113.84 → 1117.74] Just like on the Raspberry Pi 4, it's been a pretty big improvement by going to a USB disk.
[1118.16 → 1121.22] I have been told by the audience, and these are my involved thoughts.
[1121.22 → 1125.74] That's why I consider the Pine 64 as still an in-testing server platform for me right now.
[1126.06 → 1129.48] And the Raspberry Pi 4 is my production platform.
[1129.80 → 1137.24] And I've gotten notes in the Discord that the Rock Pro 64 does not have Plex GPU decoding.
[1137.64 → 1140.90] I think that's an ARM limitation more than a Rock Pro at the moment.
[1141.24 → 1143.40] The Pi does, though. The Pi 4 does.
[1143.66 → 1143.98] Does it?
[1144.18 → 1147.12] I mean, if it's doing it on the CPU, I don't have any complaints.
[1147.20 → 1147.88] Let's put it that way.
[1147.88 → 1151.70] But it seems like it must be on the GPU, or it's direct playing in most cases.
[1152.10 → 1152.68] That's probably it.
[1153.06 → 1156.10] When you're on your LAN, there's a surprising amount of stuff you can direct play
[1156.10 → 1161.14] because the clients have full, you know, 100 megabit bandwidth or whatever.
[1161.56 → 1164.10] If my testing with the Rock Pro 64 goes well,
[1164.72 → 1167.28] I'll probably make it my go-to server platform
[1167.28 → 1172.28] because the Pine 64 guys have said this is a five-year LTS hardware board.
[1172.28 → 1176.70] We're supporting this until at least 2023 or 2024.
[1177.16 → 1178.10] That's pretty cool.
[1178.50 → 1179.94] Mm-hmm. It's very appealing to me.
[1180.48 → 1182.80] And with increased performance on the disk and now the CPU,
[1183.02 → 1188.88] I think I'm also reaping the rewards of this thing having low-power DDR4 as well.
[1188.92 → 1191.80] So it's got faster RAM than the Pi 4 does.
[1192.04 → 1196.18] And I think all of these things are coming together to deliver pretty significant performance.
[1196.18 → 1199.26] And I remember when I was talking to our buddy Cheese about it,
[1199.64 → 1202.42] he was telling me, you know, you've really got to check out the Rock Pro 64
[1202.42 → 1204.78] because it, you know, for a server, I think it'd perform a lot better.
[1205.10 → 1210.16] And I was skeptical primarily because the Raspberry Pi Foundation
[1210.16 → 1216.10] has done such a good job at cultivating a community and a network effect of images.
[1216.50 → 1220.26] But I think the Pine guys are coming in a pretty close second to some of that.
[1220.32 → 1222.60] There's a really solid technical community around it.
[1222.60 → 1227.38] The Manjaro version for the Pine 64 feels first class.
[1228.18 → 1232.92] And I have yet to try an LTS Ubuntu on there, but there is an 1804 image.
[1233.10 → 1234.50] And there are lots of other great images.
[1234.58 → 1235.98] There's a real community growing around it.
[1236.24 → 1239.62] I think it's a good second contender in network effect to the Raspberry Pi.
[1240.04 → 1243.38] And so with the I.O. that I'm achieving and the CPU performance
[1243.38 → 1245.94] combined with the network effect growing
[1245.94 → 1250.04] and that LTS of five years of hardware support from the board,
[1250.04 → 1255.38] from the manufacturers, I'm thinking this is looking like my go-to solution now,
[1255.62 → 1258.00] probably for any future system I build.
[1258.20 → 1262.84] I'm even contemplating small little displays around the RV
[1262.84 → 1264.72] that would be powered by this thing.
[1265.22 → 1266.14] I have a cool little display.
[1266.74 → 1268.22] I use this for my Raspberry Pis.
[1268.88 → 1275.10] It's a little five-inch Next eon 800 by 480 pixel touchscreen.
[1275.10 → 1279.52] So I use it for 3D printer interface, which is kind of cool.
[1279.72 → 1280.14] Oh, sure.
[1280.60 → 1280.82] Yeah.
[1281.08 → 1283.44] But to come back to your point about network effects,
[1283.48 → 1285.44] I think that is really important for the Pi.
[1286.66 → 1290.22] And when I was looking after UP for, you know,
[1290.30 → 1292.22] cases and stuff like that for the Rock Pro,
[1292.86 → 1294.10] the selection wasn't great.
[1294.60 → 1295.98] Not nearly as many options.
[1296.20 → 1299.20] And the ones you do have are either first party
[1299.20 → 1302.44] or sort of second rate.
[1302.44 → 1304.42] I think that is a limitation.
[1304.68 → 1307.80] The other challenge there is that they have a limited shipping capacity.
[1307.98 → 1309.68] So when you order things, it takes a while
[1309.68 → 1311.44] and there's no everything on Amazon.
[1312.12 → 1314.10] However, all the other bits,
[1314.26 → 1317.44] like a PCI adapter to run an MIME drive
[1317.44 → 1321.38] or eMMC module or the SD cards,
[1321.46 → 1322.90] all of those are standard components
[1322.90 → 1324.50] that as long as their Linux compatible,
[1324.90 → 1326.08] they'll be compatible with the Pine board.
[1326.16 → 1326.96] You could buy those anywhere.
[1327.50 → 1328.00] So how much?
[1328.44 → 1330.48] The board itself is, what, $80 or $90?
[1330.48 → 1330.52] $50?
[1331.08 → 1331.32] Yeah.
[1331.66 → 1333.86] By the time you have the SSD in there and everything?
[1334.20 → 1336.80] All in, plus you also have to buy a power brick.
[1337.50 → 1338.98] I rounded everything up.
[1339.12 → 1340.56] The price of everything was rounded up
[1340.56 → 1342.36] and then I totalled that and rounded that up
[1342.36 → 1343.92] and it came out to $150.
[1344.70 → 1345.08] Okay.
[1345.78 → 1346.58] It's not cheap.
[1346.96 → 1347.16] No.
[1347.28 → 1350.48] And I could probably spend another 30, 40 bucks
[1350.48 → 1351.54] on cooling solutions,
[1351.72 → 1353.72] which is why I ordered this case here
[1353.72 → 1355.80] because it has a built-in heat sink.
[1355.88 → 1357.14] So we'll see how that goes for me.
[1357.14 → 1360.16] When I was building a pfSense box in July last year,
[1360.46 → 1363.90] I wanted a low-power x86 system,
[1364.26 → 1366.48] you know, something that was drawing 10 to 15 watts
[1366.48 → 1367.90] because it's going to be on 24-7.
[1369.06 → 1372.48] And I settled on a used system from eBay.
[1372.70 → 1375.04] It's an x86-based CPU.
[1375.18 → 1377.34] So it's an i5-3470T,
[1377.82 → 1379.32] which is the low-power version.
[1379.40 → 1380.10] That was $29.
[1380.10 → 1382.00] So if you think about it,
[1382.02 → 1384.32] it's an i5 third gen for $29.
[1384.66 → 1385.66] That's pretty performant.
[1385.92 → 1389.22] There's an Intel DQ77KB motherboard,
[1389.40 → 1392.10] which has dual gigabit LAN built in.
[1392.36 → 1393.64] It takes laptop memory.
[1393.98 → 1395.12] So that's nice and cheap.
[1395.46 → 1396.70] And that was $37.
[1397.46 → 1399.86] Four gigs of RAM was six bucks.
[1400.48 → 1401.98] The power supply was $20.
[1402.66 → 1405.48] And I got a little mSATA SSD for 20 bucks.
[1405.48 → 1407.88] So for about $100,
[1408.46 → 1412.30] you can build a low-power x86-based system,
[1412.64 → 1414.24] which is just as performant
[1414.24 → 1416.02] and arguably better supported.
[1416.70 → 1417.98] Yeah, I think that's the big question.
[1418.88 → 1419.82] Of course, for mine,
[1419.90 → 1422.22] the biggest cost was the MIME drive.
[1422.44 → 1423.92] I could have gone, you know,
[1423.94 → 1426.50] with like an eMMC module or something cheaper.
[1426.96 → 1427.14] Yeah.
[1427.70 → 1429.80] But I was going for the most performance possible
[1429.80 → 1431.04] because we were going to be punishing it.
[1431.34 → 1432.24] Yeah, you're Chris.
[1432.28 → 1433.10] You have to go baller.
[1433.10 → 1433.88] I know this about you.
[1433.88 → 1436.16] I sometimes got it.
[1436.26 → 1437.10] Go big or go home.
[1437.42 → 1439.94] The other two big pressures I have in my situation
[1439.94 → 1442.32] are heat output of the device
[1442.32 → 1443.86] and, as you just mentioned,
[1443.94 → 1444.86] the draw of power.
[1445.46 → 1447.58] Those things combined with performance
[1447.58 → 1449.58] are this ratio that I feel like
[1449.58 → 1451.20] I am constantly playing with.
[1451.66 → 1452.70] And I will note,
[1452.88 → 1455.48] because I'm running an additional Pi 4 right now,
[1455.88 → 1457.74] this is the one that I'm running Ubuntu on
[1457.74 → 1459.26] that I set up the new Has IO
[1459.26 → 1461.14] slash Home Assistant setup on.
[1461.14 → 1464.02] Now that I'm running a fourth Pi,
[1464.72 → 1466.64] I can notice the power draw difference
[1466.64 → 1470.02] and it is generating probably more heat in that space,
[1470.14 → 1471.94] just adding one more small device
[1471.94 → 1473.28] that I am comfortable with.
[1473.42 → 1475.52] It's a really delicate balance in there.
[1475.98 → 1477.02] We almost went the whole episode
[1477.02 → 1478.12] without mentioning Home Assistant.
[1478.40 → 1478.68] Almost.
[1479.20 → 1480.04] I can't, man.
[1480.08 → 1481.18] They just had a great update.
[1481.58 → 1483.84] And my setup is so great now.
[1483.94 → 1486.46] I am so glad you talked me into trying out hacks
[1486.46 → 1490.66] and the whole actual what is now called Home Assistant stack.
[1491.30 → 1492.64] Like, I have so much more confidence
[1492.64 → 1494.80] when I can take a nice, big, beautiful snapshot
[1494.80 → 1496.86] right before I do the new upgrades.
[1497.24 → 1497.38] Yeah.
[1497.46 → 1499.30] That does remove some of the anxiety,
[1499.44 → 1499.98] it must be said.
[1500.18 → 1500.46] Yes.
[1500.94 → 1502.84] And the theme is,
[1502.94 → 1503.64] it's more appealing,
[1503.76 → 1505.00] like it impresses the family.
[1505.16 → 1506.20] Like they think it, you know,
[1506.24 → 1506.66] it's neat.
[1506.76 → 1507.24] It's nice.
[1507.36 → 1508.10] It looks cool.
[1508.16 → 1509.40] They think it's a high-tech thing
[1509.40 → 1510.14] and they have now.
[1510.34 → 1510.84] Well, it is.
[1510.84 → 1512.88] And it should be impressive.
[1512.88 → 1514.28] But also on top of that,
[1514.78 → 1515.96] it was just a good chance for me
[1515.96 → 1517.96] to like to redo my nighttime scripts
[1517.96 → 1519.36] and my bedtime scripts.
[1519.64 → 1521.02] And this time,
[1521.38 → 1523.04] the kids have lived with it long enough
[1523.04 → 1525.10] that they had a couple of ideas
[1525.10 → 1527.50] on how I could adjust like the bedtime scripts.
[1527.90 → 1529.74] So that was really neat
[1529.74 → 1531.34] because they've taken to it,
[1531.40 → 1532.06] they like it,
[1532.12 → 1534.20] and it helps them with their nighttime routine.
[1534.42 → 1535.62] And so they just had a few ideas.
[1535.70 → 1537.10] So I was able to incorporate that stuff
[1537.10 → 1538.42] and Aaliyah's ideas.
[1538.62 → 1540.56] And we created a few systems
[1540.56 → 1542.14] to turn things on and off
[1542.14 → 1542.68] when we're leaving
[1542.68 → 1543.74] that we didn't have before.
[1544.06 → 1545.50] So it's just sort of nice
[1545.50 → 1546.50] to go through and clean it up
[1546.50 → 1547.80] and really do it right.
[1547.90 → 1549.70] Now, with all the lessons learned,
[1549.84 → 1550.18] applied,
[1550.34 → 1551.50] and the tricks that you showed me
[1551.50 → 1553.12] all kind of coming together.
[1553.84 → 1554.52] That bedtime routine
[1554.52 → 1557.30] has been a real quality of life improvement.
[1557.60 → 1559.22] I know I've said it on this show before,
[1560.06 → 1563.28] but enforced 20-minute bedtime routine,
[1563.46 → 1564.88] or 25 minutes, I think it is now.
[1564.96 → 1565.82] I've tweaked it a little bit.
[1566.46 → 1567.76] When those lights dim
[1567.76 → 1569.36] for the final 90 seconds,
[1569.90 → 1571.42] I know I have to put my phone down
[1571.42 → 1572.62] because it's about to get dark.
[1573.16 → 1573.70] And it's just,
[1573.86 → 1574.86] okay, well, I don't need to spend
[1574.86 → 1576.22] another 45 minutes on Reddit.
[1576.50 → 1577.60] I mean, what am I going to be doing
[1577.60 → 1579.56] looking at who knows what?
[1579.74 → 1580.86] That works for my kids too,
[1581.04 → 1582.64] that sort of shutting it down.
[1582.96 → 1584.10] But the other thing is,
[1584.42 → 1585.70] for my youngest,
[1586.02 → 1587.32] it's a little alarming to her
[1587.32 → 1588.40] if it just goes dark.
[1589.02 → 1590.36] She's uncomfortable with that.
[1590.54 → 1593.00] So having the lights dim for a bit
[1593.00 → 1594.54] and then get really dim
[1594.54 → 1595.84] as she drifts off to sleep,
[1595.84 → 1598.20] and then an hour after she's asleep,
[1598.30 → 1599.52] like the last light goes out
[1599.52 → 1601.44] and she's totally fine.
[1601.50 → 1602.62] She's none the wiser of it.
[1602.86 → 1603.66] And it works great for her
[1603.66 → 1604.34] and keeps them asleep.
[1604.76 → 1605.64] So how do you go about
[1605.64 → 1607.18] choosing what you're going to buy?
[1607.74 → 1608.62] When you're going through
[1608.62 → 1609.84] this purchase methodology
[1609.84 → 1610.60] in your mind of,
[1610.88 → 1612.82] I need to buy this specific device,
[1612.94 → 1614.62] I think you touched on part of it,
[1614.68 → 1615.96] you know, the LTS angle before.
[1616.34 → 1617.78] But if you're looking maybe more
[1617.78 → 1618.88] at networking gear,
[1619.02 → 1620.30] like switches or,
[1620.46 → 1620.56] you know,
[1620.58 → 1621.68] like we talked about last time,
[1621.82 → 1623.08] Wi-Fi, that kind of stuff,
[1623.08 → 1624.46] what are some of the things
[1624.46 → 1625.48] that are going through your mind?
[1625.80 → 1627.56] The hardest thing with technology
[1627.56 → 1629.26] is it's always changing.
[1629.52 → 1631.46] And if you were just to wait a little bit,
[1632.26 → 1633.44] you could get something better.
[1633.44 → 1635.74] Or if you spend a little more right now,
[1635.74 → 1637.14] you could get something that lasts longer
[1637.14 → 1637.90] and you're always trying
[1637.90 → 1638.98] to make that calculation.
[1639.82 → 1641.22] And so what I have done
[1641.22 → 1643.84] for a lot of huge decisions like this
[1643.84 → 1646.32] is I'll set like a North Star intent.
[1646.52 → 1648.84] So what is my intent with,
[1649.06 → 1649.80] say, the RV setup?
[1649.88 → 1652.04] Well, my intent is ultimately one day
[1652.04 → 1653.16] when I really zoom out,
[1653.50 → 1655.48] I want to power everything off of DC.
[1655.94 → 1656.94] And then when I zoom in closer,
[1657.02 → 1658.50] I want to be low power, low heat.
[1658.58 → 1659.44] And when I zoom in closer,
[1659.54 → 1660.56] I want it to be silent
[1660.56 → 1662.40] and I want it to be low maintenance,
[1662.54 → 1662.92] low effort.
[1663.02 → 1665.00] That's why the five-year LTS
[1665.00 → 1666.28] of both a board
[1666.28 → 1667.36] and an operating system
[1667.36 → 1668.42] are very appealing to me.
[1668.88 → 1671.20] And so when I zoom all the way out,
[1671.26 → 1672.40] think about the big post items
[1672.40 → 1673.40] like the Northern Star one,
[1673.48 → 1674.48] and then I zoom all the way down
[1674.48 → 1675.28] into the details
[1675.28 → 1676.78] of what I want to have to manage,
[1677.60 → 1679.28] that helps me make an informed decision.
[1679.28 → 1681.24] So like another scenario with networking gear
[1681.24 → 1685.24] is maybe I want to have multiple Plans
[1685.24 → 1687.16] and I want to have insights into the traffic
[1687.16 → 1689.20] that's going over those individual ports.
[1689.42 → 1690.92] And I'd like to be able to do it
[1690.92 → 1693.06] from both a web browser and a command line.
[1693.36 → 1694.70] And then when I zoom out from that,
[1694.76 → 1697.22] I want something that runs efficiently
[1697.22 → 1699.30] where I can put a lot of load under it
[1699.30 → 1700.26] for video transfer.
[1700.96 → 1702.18] And in this particular setup,
[1702.22 → 1703.64] because of where my networking gear is,
[1704.06 → 1705.50] noise isn't really a factor for me
[1705.50 → 1706.32] when I come to purchasing.
[1706.46 → 1707.70] So okay, then I zoom out a little bit further.
[1707.70 → 1709.86] I'd like this to run for about five years.
[1709.86 → 1711.38] And I'll go through a stack like that.
[1711.72 → 1713.96] And I will end up with a very different piece
[1713.96 → 1714.82] of networking equipment
[1714.82 → 1716.76] than I might end up for a Plex server.
[1717.28 → 1718.06] It's fascinating.
[1718.06 → 1720.46] When you look at how different companies mature
[1720.46 → 1722.48] and how their business models change,
[1722.74 → 1724.56] one of the factors I like to take into account
[1724.56 → 1727.68] is how long a company has been around
[1727.68 → 1729.52] and what their kind of track record is.
[1729.56 → 1731.78] You know, I look at Netgear as a good example.
[1732.62 → 1733.44] They're kind of boring
[1733.44 → 1734.86] and they kind of just do the job.
[1734.86 → 1736.74] And they've been around for as long
[1736.74 → 1737.82] as I've been into computers.
[1738.40 → 1740.48] And when I buy a Netgear switch,
[1740.52 → 1741.58] I know that in five years,
[1741.62 → 1742.54] I'll be able to replace it
[1742.54 → 1744.52] with probably the exact same thing.
[1745.06 → 1746.02] And when you zoom in on that,
[1746.08 → 1748.28] your intention there is something
[1748.28 → 1750.82] that is so reliable,
[1751.30 → 1753.80] it could actually be completely out of your mind.
[1753.88 → 1755.98] You don't even really have to worry about it ever.
[1756.40 → 1757.04] Boring is good.
[1757.20 → 1757.92] Boring is reliable.
[1758.34 → 1760.14] That would be sort of your sort of
[1760.14 → 1762.12] Northern Star intent on that piece of equipment
[1762.12 → 1763.26] and inform your purchasing.
[1763.26 → 1764.96] And then when you zoom in, is noise a factor?
[1765.42 → 1766.94] Well, is noise a factor?
[1767.56 → 1768.94] Because my server's in my basement,
[1769.48 → 1772.10] which the only thing that's going to get annoyed down there
[1772.10 → 1772.78] are the cockroaches.
[1773.54 → 1775.98] So when I think about my requirements,
[1776.18 → 1778.36] okay, you know, a desktop switch or something like that,
[1778.38 → 1779.54] of course that has to be silent.
[1780.10 → 1781.88] But I generally go for, you know,
[1781.92 → 1784.70] the five to eight port gigabit switches
[1784.70 → 1787.68] that are now so unbelievably cheap.
[1787.82 → 1789.68] I was looking at going 10 gig
[1789.68 → 1791.48] when I moved into this house
[1791.48 → 1793.80] and I've run the Cat 6a cable
[1793.80 → 1795.30] to enable me to do that in future
[1795.30 → 1796.40] if the prices come down.
[1796.50 → 1797.58] But right now, you know,
[1797.64 → 1799.50] I would be looking at several hundred dollars
[1799.50 → 1801.74] to equip two or three devices
[1801.74 → 1802.92] with 10 gig networking
[1802.92 → 1805.60] versus 20 or $30
[1805.60 → 1808.32] for a couple of switches for gigabit.
[1808.48 → 1810.48] And I would love to have 10 gig
[1810.48 → 1811.70] just in one place
[1811.70 → 1812.98] between my desktop and my server,
[1813.12 → 1815.12] but it's just not worth the cost right now.
[1815.12 → 1816.06] Yeah, I know.
[1816.54 → 1816.98] I know.
[1817.18 → 1818.24] I think too, the other factor
[1818.24 → 1819.98] with networking equipment to consider
[1819.98 → 1824.70] is that you may want to use your home lab
[1824.70 → 1827.22] as a test bed to learn.
[1827.78 → 1830.90] And so sometimes it's worth thinking about
[1830.90 → 1832.30] trying to find something
[1832.30 → 1834.56] that still has some decent value on eBay.
[1834.98 → 1836.48] It's not the worst idea in the world
[1836.48 → 1837.34] to buy a used switch.
[1837.40 → 1838.60] I know it seems weird at first
[1838.60 → 1840.22] because it's such a key piece of equipment,
[1840.40 → 1842.36] but some of these higher end switches
[1842.36 → 1844.68] are rated to run for a lifetime.
[1844.68 → 1847.08] And you get them off of eBay,
[1847.28 → 1848.30] a lot of the fundamentals
[1848.30 → 1849.62] on how to manage them
[1849.62 → 1851.56] and set up networking basic stuff
[1851.56 → 1852.36] like Plans
[1852.36 → 1854.16] and mirroring your port
[1854.16 → 1855.32] so you can monitor traffic,
[1855.88 → 1857.26] it's all going to still be relevant
[1857.26 → 1859.30] even on a five-year-old Cisco switch.
[1859.74 → 1861.80] And then there is the self-improvement angle,
[1861.96 → 1863.60] which I think is quite often overlooked
[1863.60 → 1865.46] when people are trying to decide
[1865.46 → 1866.76] between self-hosting
[1866.76 → 1868.18] or using a cloud service
[1868.18 → 1870.66] or buying an off-the-shelf product.
[1870.84 → 1871.94] You know, I make this point
[1871.94 → 1874.36] in my 2019 Perfect Media Server article
[1874.36 → 1876.46] where I'm comparing
[1876.46 → 1877.84] basically a Synology
[1877.84 → 1879.22] to a self-hosted
[1879.22 → 1880.42] do-it-yourself type system.
[1881.26 → 1882.30] And when you look at the skills
[1882.30 → 1883.26] that you have to learn
[1883.26 → 1884.04] in order to build
[1884.04 → 1885.08] a self-hosted system
[1885.08 → 1886.02] that is reliable
[1886.02 → 1887.86] and will be able to run
[1887.86 → 1888.52] for five years
[1888.52 → 1889.34] and that kind of stuff,
[1889.88 → 1890.52] those are skills
[1890.52 → 1891.54] you can take directly
[1891.54 → 1892.56] and get a job with.
[1893.14 → 1894.48] A well-paying job.
[1895.12 → 1896.60] And you can lift yourself
[1896.60 → 1897.66] very quickly out of being
[1897.66 → 1899.40] a level one, level two support,
[1899.90 → 1901.00] you know, in a call centre
[1901.00 → 1901.50] or something
[1901.50 → 1903.22] by doing a lot of these projects
[1903.22 → 1903.72] at home.
[1903.72 → 1905.78] And so buying a Cisco switch
[1905.78 → 1906.18] off eBay,
[1906.52 → 1907.18] learning iOS
[1907.18 → 1909.12] and becoming a CCNA,
[1909.60 → 1909.88] you know,
[1909.96 → 1912.76] certified Cisco network admin.
[1913.18 → 1914.32] Is that what CCNA stands for?
[1914.62 → 1915.10] Mm-hmm.
[1915.76 → 1917.12] You know, being a CCNA
[1917.12 → 1918.28] or a Red Hat certified,
[1918.50 → 1918.74] whatever.
[1919.50 → 1919.72] You know,
[1919.72 → 1921.70] there's a lot of investment
[1921.70 → 1922.50] in yourself
[1922.50 → 1924.52] beyond just the physical hardware
[1924.52 → 1926.64] that you can get out of this stuff.
[1926.64 → 1927.80] Yeah, that's why it's important
[1927.80 → 1928.82] to consider that
[1928.82 → 1930.94] when you are purchasing network gear
[1930.94 → 1932.88] because if that isn't you,
[1933.46 → 1935.90] then something more along the lines
[1935.90 → 1937.58] of an unmanaged switch
[1937.58 → 1939.18] might be what you want.
[1939.56 → 1940.86] Those are really the two categories.
[1940.98 → 1941.86] You have unmanaged
[1941.86 → 1943.30] and managed switches.
[1943.58 → 1944.36] And so if you're looking
[1944.36 → 1945.12] to do networking
[1945.12 → 1946.54] at a more granular level,
[1946.98 → 1947.80] you want to learn,
[1948.02 → 1949.44] maybe use it
[1949.44 → 1950.86] for building a cool home lab,
[1951.58 → 1953.12] you want a managed switch.
[1953.70 → 1954.94] And there are cheap ones
[1954.94 → 1955.70] you can buy today,
[1955.78 → 1956.26] brand new,
[1956.26 → 1957.60] and there are expensive ones.
[1957.94 → 1958.86] I mean, I'm talking,
[1959.00 → 1960.46] you know, $5,000 plus
[1960.46 → 1961.56] that now you can get on eBay
[1961.56 → 1962.78] for a couple of hundred dollars.
[1963.40 → 1964.48] Those are the managed switches.
[1965.12 → 1966.52] However, if you're like me
[1966.52 → 1968.58] and you're going to be connecting
[1968.58 → 1969.78] four Raspberry Pis
[1969.78 → 1970.86] and a Wi-Fi router,
[1971.02 → 1971.98] I went unmanaged.
[1972.08 → 1973.34] I went an unmanaged net gear
[1973.34 → 1973.82] for that one
[1973.82 → 1975.52] because it's just a simple setup
[1975.52 → 1977.60] with a very simple network loadout.
[1977.78 → 1979.10] It doesn't need to do much.
[1979.22 → 1980.42] I just want it to be gigabit.
[1980.64 → 1982.00] And so I went unmanaged
[1982.00 → 1983.08] and it's also silent.
[1983.56 → 1984.28] I've only ever had
[1984.28 → 1985.68] one managed switch in my life
[1985.68 → 1986.98] and that is the only switch
[1986.98 → 1988.10] that's ever failed on me.
[1988.36 → 1989.14] Well, they are more complex.
[1989.46 → 1990.62] I'm not saying there's a correlation,
[1991.02 → 1991.52] but, you know,
[1991.54 → 1992.70] it's just purely anecdotal.
[1993.28 → 1994.36] But I would say
[1994.36 → 1995.30] for most people,
[1995.38 → 1995.92] most of the time,
[1996.02 → 1996.96] especially at home,
[1997.02 → 1997.98] and even if you're doing
[1997.98 → 1999.06] home lab stuff,
[1999.32 → 2000.62] unless you're a network engineer,
[2001.16 → 2002.34] you probably don't need
[2002.34 → 2002.92] a managed switch.
[2003.32 → 2004.20] No, probably not.
[2004.20 → 2006.18] I, of course,
[2006.52 → 2008.38] did have a managed switch
[2008.38 → 2010.46] when Angela and I built our house.
[2010.54 → 2012.88] I put a really loud,
[2013.28 → 2014.32] regrettably loud,
[2014.56 → 2016.36] HP managed switch in there.
[2016.72 → 2018.36] The thing never died, though.
[2018.42 → 2018.66] I mean,
[2018.72 → 2020.52] they were so rock solid,
[2020.68 → 2022.12] but they were just jet engines.
[2022.66 → 2023.70] And it was really neat.
[2023.94 → 2025.38] You had an Alan Jude back then, though.
[2025.58 → 2026.12] Yeah, there's that.
[2026.12 → 2026.80] And also,
[2027.04 → 2027.60] in my day job,
[2027.76 → 2029.66] I was managing tons of HP switches
[2029.66 → 2031.38] and Dell switches,
[2031.38 → 2032.70] which I didn't like as much.
[2033.30 → 2034.14] But I really did like
[2034.14 → 2035.02] those HP switches.
[2035.88 → 2036.50] It, to me,
[2036.58 → 2037.52] was worth it because
[2037.52 → 2038.38] I love, like,
[2038.42 → 2039.42] turning on mirrored ports
[2039.42 → 2041.78] or doing small little,
[2041.80 → 2042.86] like, segments of networks
[2042.86 → 2043.70] and things that you could do
[2043.70 → 2044.78] on these switches that were,
[2045.10 → 2045.26] well,
[2045.32 → 2046.02] they were just really fun
[2046.02 → 2046.82] to mess around with.
[2047.16 → 2047.94] But these days,
[2048.02 → 2049.20] it all works pretty well.
[2049.50 → 2050.66] Back in the good old days,
[2051.10 → 2052.28] you'd have to worry about
[2052.28 → 2053.60] things not matching up,
[2053.66 → 2054.72] like, your duplex settings,
[2054.90 → 2055.14] you know,
[2055.18 → 2055.80] and your Nick not
[2055.80 → 2057.24] auto-negotiating properly.
[2057.68 → 2058.74] And that stuff just sounds
[2058.74 → 2059.44] even silly now
[2059.44 → 2060.16] to even talk about.
[2060.42 → 2061.28] This old man Chris
[2061.28 → 2062.22] shouting at a cloud.
[2064.46 → 2065.86] Which brings us nicely
[2065.86 → 2067.62] to the last item
[2067.62 → 2068.52] in the show doc today,
[2068.58 → 2069.10] which is,
[2069.80 → 2071.28] if you do this stuff right,
[2071.36 → 2073.02] if you design a house,
[2073.16 → 2073.74] build a house,
[2073.84 → 2075.52] or add stuff to your house,
[2075.52 → 2077.02] like an Ethernet cabling
[2077.02 → 2077.82] or something like that,
[2078.22 → 2079.56] you can actually add value
[2079.56 → 2080.22] to your house.
[2080.58 → 2082.62] And one of the hardest things
[2082.62 → 2083.88] that you have to solve
[2083.88 → 2086.04] is how do you transfer accounts
[2086.04 → 2086.96] to the new owner?
[2087.44 → 2087.82] Well, Alex,
[2087.96 → 2088.96] if you're self-hosting,
[2089.30 → 2090.36] this is much simpler.
[2090.36 → 2093.18] It is significantly harder
[2093.18 → 2094.10] if you've got,
[2094.16 → 2094.78] like,
[2094.88 → 2096.42] the TP-Link
[2096.42 → 2097.60] Casa home plugs,
[2097.94 → 2098.56] and you've got
[2098.56 → 2099.64] Hughes lights
[2099.64 → 2100.32] that are associated
[2100.32 → 2101.48] with your Hughes account,
[2101.60 → 2102.22] and you have
[2102.22 → 2103.96] all these different vendors,
[2104.46 → 2105.54] which I used to have.
[2105.98 → 2107.66] I think that's nearly impossible.
[2107.66 → 2108.50] But in
[2108.50 → 2109.42] home assistance
[2109.42 → 2110.64] slash self-hosted setup,
[2110.88 → 2111.34] it's actually
[2111.34 → 2112.40] much more straightforward.
[2112.40 → 2114.54] I would think
[2114.54 → 2116.00] in the traditional
[2116.00 → 2116.78] consumer scenario
[2116.78 → 2117.30] where you just have
[2117.30 → 2118.34] tons of different accounts,
[2118.78 → 2119.42] it's going to vary
[2119.42 → 2120.30] depending on each
[2120.30 → 2121.26] one of those services.
[2121.94 → 2122.62] My wife is addicted
[2122.62 → 2124.28] to this Architectural Digest
[2124.28 → 2125.02] YouTube channel
[2125.02 → 2126.90] where they go around
[2126.90 → 2128.12] $20 million houses
[2128.12 → 2129.40] in Beverly Hills,
[2129.66 → 2131.06] and it's stupid.
[2131.34 → 2132.20] But every single
[2132.20 → 2133.86] one of those houses
[2133.86 → 2134.58] has one of these
[2134.58 → 2135.24] Luton
[2135.24 → 2137.42] smart home systems in it
[2137.42 → 2138.18] that is just like
[2138.18 → 2138.70] a spaceship,
[2139.00 → 2139.58] and, you know,
[2139.58 → 2140.00] they're tapping
[2140.00 → 2141.02] three different things
[2141.02 → 2142.24] to do all the stuff,
[2142.56 → 2143.44] and I'm like,
[2143.50 → 2144.44] that's so far away
[2144.44 → 2145.36] from where I want to be.
[2145.52 → 2145.68] You know,
[2145.70 → 2146.46] it looks cool,
[2146.68 → 2147.24] and I guess that's
[2147.24 → 2147.98] what they're going for
[2147.98 → 2148.76] in that price point.
[2149.14 → 2150.10] I just want simple
[2150.10 → 2150.64] and functional,
[2151.18 → 2152.06] and ideally,
[2152.68 → 2153.34] I'm not going to take
[2153.34 → 2154.46] Ethernet cable out of the walls
[2154.46 → 2155.10] if it's there,
[2155.58 → 2156.36] but stuff like the
[2156.36 → 2157.22] Wi-Fi access points,
[2157.22 → 2158.32] I'll take those with me,
[2158.64 → 2159.50] and I'll leave the
[2159.50 → 2160.66] Ethernet cable dangling
[2160.66 → 2161.62] for the next person.
[2162.42 → 2163.18] A lot of the lights
[2163.18 → 2163.84] in my house
[2163.84 → 2165.24] are smart bulbs
[2165.24 → 2166.14] or smart switches.
[2166.60 → 2167.94] I will probably take
[2167.94 → 2169.30] my little
[2169.30 → 2171.02] shelly things
[2171.02 → 2171.92] out of the switches
[2171.92 → 2172.56] when I leave
[2172.56 → 2174.50] unless they add value
[2174.50 → 2175.00] to the house
[2175.00 → 2175.62] because, you know,
[2175.66 → 2176.46] they're $20 each
[2176.46 → 2177.00] and I've got like
[2177.00 → 2177.72] five or six of them,
[2177.82 → 2178.02] so.
[2178.42 → 2178.96] That's my thought,
[2179.04 → 2179.86] is I would negotiate
[2179.86 → 2181.24] with the purchaser
[2181.24 → 2182.70] if they want those things.
[2183.08 → 2183.52] One of the things
[2183.52 → 2184.90] I'm really pretty proud
[2184.90 → 2185.64] of my setup
[2185.64 → 2187.20] is with just a few exceptions
[2187.20 → 2188.32] like the tablet
[2188.32 → 2189.16] being mounted
[2189.16 → 2190.58] at a certain spot,
[2190.82 → 2192.10] you really can't tell
[2192.10 → 2193.28] that there's any automation
[2193.28 → 2193.94] at all.
[2194.04 → 2195.02] It's all fairly invisible.
[2195.56 → 2196.30] Here's the thing, Chris.
[2196.96 → 2197.98] Most people don't care.
[2198.26 → 2198.48] No.
[2198.48 → 2199.22] A light switch
[2199.22 → 2200.26] is fine for most people.
[2200.82 → 2201.64] A proprietary service
[2201.64 → 2202.58] is fine for most people.
[2202.64 → 2204.00] They just don't really care,
[2204.72 → 2205.36] which is sad.
[2205.58 → 2206.34] No, I think you're right.
[2206.48 → 2207.74] I think it's one of those
[2207.74 → 2209.10] you have to experience it.
[2209.66 → 2210.32] I mean,
[2210.46 → 2211.22] even the kids
[2211.22 → 2212.20] appreciate it now,
[2212.26 → 2213.36] which I never expected.
[2214.08 → 2215.36] And my wife,
[2215.42 → 2215.60] Asia,
[2215.66 → 2216.10] has said to me
[2216.10 → 2216.62] several times
[2216.62 → 2217.68] that this winter
[2217.68 → 2220.56] was so much more comfortable
[2220.56 → 2221.68] than any winter we've had
[2221.68 → 2222.48] because of the
[2222.48 → 2223.36] automated heat system.
[2223.42 → 2224.70] It was just nice.
[2224.86 → 2225.70] It was really nice
[2225.70 → 2226.34] not to manage it
[2226.34 → 2227.24] because it's
[2227.24 → 2228.20] often very challenging
[2228.20 → 2229.24] when it gets below freezing.
[2230.14 → 2232.58] And I think you can appreciate it
[2232.58 → 2233.26] once you've had one.
[2233.72 → 2234.30] It's the same thing
[2234.30 → 2235.68] with the smart speakers.
[2236.38 → 2236.50] You know,
[2236.52 → 2237.28] when I'm walking in
[2237.28 → 2237.80] with groceries
[2237.80 → 2238.46] in the dark
[2238.46 → 2239.42] and I can just shout out
[2239.42 → 2239.86] to the room,
[2240.00 → 2241.52] turn on all the lights
[2241.52 → 2242.50] and just boom,
[2242.56 → 2243.44] I can see all of a sudden.
[2243.56 → 2243.72] I'm like,
[2243.86 → 2244.62] man, that's great.
[2244.98 → 2245.66] That's so great.
[2245.70 → 2246.42] And it's instantaneous.
[2247.22 → 2247.94] You got to experience that
[2247.94 → 2248.42] a few times
[2248.42 → 2248.86] before you go,
[2248.92 → 2249.12] oh,
[2249.58 → 2250.30] that was nice.
[2250.84 → 2252.94] We went to a neighbour
[2252.94 → 2254.64] that lives just behind last night.
[2254.72 → 2255.48] They had a fire pit
[2255.48 → 2256.18] on their driveway,
[2256.48 → 2257.20] socially distanced,
[2257.30 → 2257.62] of course,
[2258.32 → 2259.28] and, you know,
[2259.30 → 2260.34] drinking a few brew skis,
[2260.60 → 2261.90] came back a little worse for wear
[2261.90 → 2263.56] and we're sort of stumbling
[2263.56 → 2264.20] in the dark
[2264.20 → 2265.32] up to our house
[2265.32 → 2266.82] and I just pull my phone out
[2266.82 → 2268.18] over LTE.
[2268.50 → 2269.60] I turn on all the lights
[2269.60 → 2270.12] in the house,
[2270.24 → 2271.16] open the garage doors
[2271.16 → 2271.84] and we sort of stumble
[2271.84 → 2272.48] through the garage
[2272.48 → 2273.30] and it's all fine
[2273.30 → 2274.58] because we couldn't find our keys.
[2275.94 → 2276.30] Yes,
[2276.38 → 2277.10] it's really nice.
[2277.22 → 2277.68] It's really,
[2277.78 → 2278.46] and it's also a great way
[2278.46 → 2279.08] to save energy
[2279.08 → 2280.88] because I can have the heat down
[2280.88 → 2281.60] when we're not there
[2281.60 → 2283.12] and then when we're coming home
[2283.12 → 2284.62] it can start warming it back up
[2284.62 → 2286.60] and I like that aspect of it too
[2286.60 → 2287.30] because I feel like
[2287.30 → 2288.12] we're saving power
[2288.12 → 2288.66] and we're saving,
[2288.88 → 2290.02] we also have a similar system
[2290.02 → 2290.54] for water
[2290.54 → 2292.12] and all of those things
[2292.12 → 2292.94] are really nice
[2292.94 → 2294.40] but I would kind of
[2294.40 → 2296.46] maybe just push back
[2296.46 → 2297.20] a little bit
[2297.20 → 2298.72] on your implication there
[2298.72 → 2299.70] that nobody cares.
[2300.24 → 2300.94] I think you're right
[2300.94 → 2301.86] for the majority.
[2302.56 → 2302.86] However,
[2302.94 → 2304.26] I was just reading something
[2304.26 → 2305.80] about how
[2305.80 → 2307.76] the speed of an internet connection
[2307.76 → 2308.48] in an area
[2308.48 → 2309.78] is having a big impact
[2309.78 → 2310.32] on whether people
[2310.32 → 2311.46] buy a home or not these days.
[2311.70 → 2312.88] These things are starting to matter.
[2313.44 → 2314.10] I use my dad
[2314.10 → 2315.64] as a good bit of litmus paper
[2315.64 → 2316.88] to tell whether it's
[2316.88 → 2318.62] something most people care about
[2318.62 → 2320.08] and he just couldn't
[2320.08 → 2321.28] give two monkeys.
[2322.26 → 2322.56] So,
[2323.18 → 2325.20] I think it's limited
[2325.20 → 2326.18] to nerds at the moment
[2326.18 → 2326.78] but
[2326.78 → 2328.34] a smart home
[2328.34 → 2328.94] as an industry
[2328.94 → 2330.20] is not limited to nerds.
[2330.42 → 2331.18] I'm talking about
[2331.18 → 2332.50] self-hosted smart homes
[2332.50 → 2333.16] where you
[2333.16 → 2335.08] do a lot of this stuff yourself.
[2335.54 → 2335.74] Yeah,
[2335.96 → 2336.62] maybe.
[2336.96 → 2337.42] Some of it,
[2337.58 → 2337.74] like,
[2337.96 → 2338.14] you know,
[2338.16 → 2339.42] if I were going to
[2339.42 → 2340.78] sell Lady Coupes
[2340.78 → 2341.44] with all this automation
[2341.44 → 2342.46] maybe it would make sense
[2342.46 → 2343.80] to leave a lot
[2343.80 → 2344.84] of the wired stuff in
[2344.84 → 2345.48] and the cameras
[2345.48 → 2345.98] and the sensors
[2345.98 → 2347.10] but take out the computers
[2347.10 → 2347.92] and the next user
[2347.92 → 2348.56] puts theirs in
[2348.56 → 2348.72] but
[2348.72 → 2350.68] cameras is a good one.
[2350.92 → 2351.98] I bet if I leave those behind
[2351.98 → 2352.64] they'd add value.
[2353.08 → 2353.28] Right.
[2353.48 → 2354.60] I think AP points would
[2354.60 → 2356.18] I think AP points
[2356.18 → 2356.82] that's like calling them
[2356.82 → 2357.22] NIC cards.
[2357.62 → 2358.56] I think access points
[2358.56 → 2359.08] would too.
[2359.42 → 2359.62] You know,
[2359.90 → 2360.50] you ever notice how
[2360.50 → 2361.26] everybody always says
[2361.26 → 2361.86] a NIC card
[2361.86 → 2362.10] it's like,
[2362.16 → 2362.20] well,
[2362.22 → 2362.54] wait a minute,
[2362.84 → 2363.88] you're just saying card twice.
[2364.24 → 2364.96] PC computers.
[2365.52 → 2365.82] Yes.
[2366.62 → 2368.48] That kind of thing.
[2368.90 → 2369.84] And also,
[2369.96 → 2370.68] it's one of those
[2370.68 → 2371.94] where maybe
[2371.94 → 2373.52] in two to five years
[2373.52 → 2374.64] when people have gone
[2374.64 → 2375.54] through a few cycles
[2375.54 → 2376.52] more of
[2376.52 → 2377.66] some services
[2377.66 → 2378.62] being shut down
[2378.62 → 2379.76] and people's devices
[2379.76 → 2380.46] quit working
[2380.46 → 2382.02] and that becomes
[2382.02 → 2383.00] more of
[2383.00 → 2384.28] a front of mind
[2384.28 → 2384.78] concern
[2384.78 → 2385.40] because you know
[2385.40 → 2386.12] it's going to happen.
[2386.12 → 2386.90] I hope so
[2386.90 → 2387.88] because then this podcast
[2387.88 → 2388.38] is going to
[2388.38 → 2389.32] go through the roof.
[2389.98 → 2391.28] It'll be great for the show.
[2391.72 → 2392.64] Oh man.
[2392.94 → 2393.76] It'll be great for
[2393.76 → 2394.22] Home Assistant.
[2394.42 → 2394.52] There,
[2394.64 → 2394.84] boom,
[2394.90 → 2395.50] another mention.
[2395.70 → 2395.94] Ha!
[2396.34 → 2396.64] Ding.
[2396.78 → 2397.30] We need a bell
[2397.30 → 2397.88] for Home Assistant.
[2398.42 → 2399.04] My goal is to get
[2399.04 → 2399.72] three in now.
[2399.86 → 2400.24] That's the thing.
[2400.24 → 2400.48] Okay.
[2400.78 → 2400.98] Okay.
[2402.28 → 2403.26] So where should we send
[2403.26 → 2403.82] folks throughout
[2403.82 → 2404.42] the rest of the week?
[2404.70 → 2404.90] Well,
[2404.98 → 2405.84] there's always that
[2405.84 → 2406.74] wiki that's in development
[2406.74 → 2407.60] which we haven't mentioned
[2407.60 → 2408.20] too recently
[2408.20 → 2408.94] but there is
[2408.94 → 2410.64] wiki.self-hosted.show.
[2410.80 → 2411.72] We'd love to also get
[2411.72 → 2412.54] your thoughts and feedback
[2412.54 → 2414.10] and feel free to push back
[2414.10 → 2414.64] on things like
[2414.64 → 2415.72] Plex for media hosting.
[2415.84 → 2416.48] We like that too
[2416.48 → 2418.50] but do it constructively.
[2418.74 → 2420.04] Give us your experience
[2420.04 → 2420.82] with your alternative
[2420.82 → 2422.16] at self-hosted. Show
[2422.16 → 2423.28] slash contact
[2423.28 → 2425.20] and then last but not least
[2425.20 → 2426.18] while you're over there
[2426.18 → 2427.16] at that self-hosted page
[2427.16 → 2427.66] go ahead and click
[2427.66 → 2428.54] that Discord link.
[2428.84 → 2429.26] It's a perfect
[2429.26 → 2429.94] community in there.
[2430.32 → 2430.74] And I'm going to give
[2430.74 → 2431.54] a shout-out to
[2431.54 → 2432.32] Linux Unplugged
[2432.32 → 2433.52] episode 349
[2433.52 → 2434.40] where Chris
[2434.40 → 2435.96] torture tests
[2435.96 → 2437.30] that rock pro.
[2437.58 → 2438.38] That was a lot of fun.
[2438.50 → 2438.62] Yeah,
[2438.68 → 2439.10] good mention.
[2439.20 → 2439.66] I think if people
[2439.66 → 2440.24] like this show
[2440.24 → 2441.28] they'll probably like
[2441.28 → 2441.90] that episode.
[2442.66 → 2442.84] Well,
[2442.88 → 2443.12] Alex,
[2443.12 → 2443.80] I think that's
[2443.80 → 2444.60] self-hosted 17.
[2444.60 → 2444.98] Thank you.
