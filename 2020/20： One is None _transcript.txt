[0.00 --> 5.98]  Coming up on Self-Hosted 20, you're not a true self-hoster until you've lost your entire configuration at least once, right?
[6.78 --> 11.74]  I'll tell you my tale. Alex has done a deep dive in your best options for cloud backup,
[11.98 --> 16.62]  and we try to find the right Wi-Fi solution for a listener with a real challenge. I'm Chris.
[16.96 --> 18.94]  I'm Alex, and this is Self-Hosted.
[20.00 --> 25.70]  I'm so jealous of you going down at Austin. You're going to get some of that delicious Terry Black's barbecue, aren't you, and rub my face in it?
[25.70 --> 35.46]  Absolutely. I'm going to take pictures of it from all the best angles, and then I'm going to take it into a photo editor and punch it up a little bit, and then I'm going to send it to you.
[35.76 --> 37.20]  On your Instagram story?
[37.52 --> 44.14]  And then I'll also make sure to just sort of capture my thoughts as I'm enjoying it and send that to you as an audio message.
[44.58 --> 45.16]  In detail.
[45.66 --> 46.36]  Yeah, okay.
[46.80 --> 54.16]  Yeah, it's going to be a good trip. It's going to be myself, the wife, and the three kids and the dog all loaded up in Lady Joops.
[54.16 --> 63.10]  Because I've got now, after quite the experience, I have got 1.2 terabytes of media for offline consumption.
[63.58 --> 66.10]  That's quite a bit, possibly more than you need.
[66.48 --> 72.82]  Yeah, yeah. I wish I would have realized that before I attempted to get it, because I might have saved myself a lot of trouble.
[73.92 --> 75.66]  So what did you get, and how did you get it?
[75.84 --> 78.84]  Well, I wanted to just add more storage to my home setup.
[78.84 --> 87.38]  This was just an innocent voyage, one that I initially considered using MergerFS for because of your success with it.
[87.72 --> 91.62]  In fact, I even reread your blog post on the Perfect Media Server.
[91.62 --> 110.08]  As I was considering doing this, I was reminded by a friendly member of our community that ButterFS has a very nice feature built into it that makes adding additional storage to a mount point super simple.
[110.08 --> 114.34]  And adding mismatched drive sizes of all types is really easy.
[114.96 --> 122.86]  It really comes down to something as simple as, like, ButterFS, volume, add, and you specify the device, and you specify the mount point.
[123.26 --> 133.84]  And with one command, you can take a brand new, perfectly formatted ButterFS disk and just add it to an existing mount point, and it just expands the storage available there.
[133.84 --> 140.98]  And then there's a balance command that'll spread the data across all the drives in the background, which you do have to do manually.
[141.12 --> 142.54]  If you don't run that command, it won't happen.
[142.88 --> 155.42]  But the idea is that you can kind of come along and just add additional storage and ButterFS add this volume to this mount point as much as you'd like, as long as you have appropriate data protections in place.
[155.90 --> 159.50]  Balancing is one of those things that I often think, yeah, I want that.
[159.50 --> 167.58]  But then you think about what it's doing, and you're reading data from a bunch of disks and writing data to a bunch of disks.
[168.28 --> 170.40]  For what potential gain?
[170.50 --> 172.98]  So far as I see it, with balancing, there's only risk.
[173.64 --> 178.10]  You're increasing wear and tear on the drives for what purpose?
[178.48 --> 187.02]  It's just, you know, I think it's for my own personal, oh, look at this, all my drives are at 65% now, as opposed to anything actually useful.
[187.24 --> 187.64]  What do you think?
[187.64 --> 195.66]  You're kind of spreading the load out in the sense of reads could potentially be faster if you had a controller that wasn't the USB bus.
[195.76 --> 201.46]  But say you had a pretty fast interface for these individual drives, and then you spread the data out.
[201.60 --> 205.16]  When you're reading from multiple drives, you can potentially get some really fast read speeds.
[205.62 --> 207.32]  All valid if you're a data center.
[207.66 --> 207.88]  Yeah.
[208.10 --> 209.14]  Are you a data center?
[209.78 --> 210.34]  Nope, nope.
[210.34 --> 212.66]  I'm calling it my server cabinet at this point.
[213.58 --> 216.60]  Actually, I should say, Alex, I should back this up a couple of steps.
[216.60 --> 222.84]  I began a project because I put a sensor in the dinette where I have all the Raspberry Pis.
[223.12 --> 226.82]  I put a little Z-Wave sensor in there reporting back to Home Assistant.
[227.58 --> 236.76]  And when I started to see the temperatures that that little cabinet, if you'll allow it, was getting up to in the middle of the day when it's only 70 degrees.
[236.76 --> 241.26]  And here I'm going to Austin, where it's going to be 100 degrees during the day while I'm there.
[241.78 --> 246.58]  And while I'm up in the Pacific Northwest, this thing's getting to about 83 degrees.
[247.08 --> 248.92]  This is the inside of your dinette seat.
[249.16 --> 249.38]  Yeah.
[250.34 --> 252.20]  What I'm now calling my server cabinet.
[252.42 --> 252.90]  Server seat.
[253.18 --> 254.72]  Ooh, server seat is great.
[254.82 --> 255.22]  Thank you.
[255.22 --> 255.54]  Yeah.
[256.20 --> 258.74]  So in the server seat, it's getting up to 83 degrees.
[259.08 --> 269.46]  So what I realized I needed to do is I needed to, first of all, I needed to check the thermals of the actual Raspberry Pis, which were high, but they're not dangerously high, but they were high.
[269.88 --> 271.76]  And then I needed to reduce hardware.
[271.92 --> 273.20]  I've been meaning to do this anyways.
[273.30 --> 278.34]  I wanted to shut down two of them and just reduce power draw and reduce heat output.
[278.34 --> 284.22]  So six minus two, that still leaves you with four Raspberry Pi 4s in there though, right?
[284.46 --> 285.84]  Not all of them are in the RV.
[286.04 --> 288.34]  I have a couple of Raspberry Pis here at the studio now too.
[288.48 --> 288.88]  Oh, okay.
[289.06 --> 289.24]  Okay.
[289.28 --> 289.40]  Yeah.
[289.54 --> 289.76]  All right.
[291.08 --> 300.20]  So this was all an innocent goal, but in order to accomplish this, I needed to move some of my containers and all of my Plex media over to a different Raspberry Pi.
[300.20 --> 316.42]  This is where I started thinking I could take the drive that's attached to the Pi I'm shutting down, connect it to the Raspberry Pi I'm keeping and utilize Merger FS to enjoy the storage across both these disks because I needed more than the terabyte that I had.
[317.24 --> 319.74]  That probably would have worked.
[320.78 --> 325.28]  Probably should have been the route I went, but it was not what I ended up doing.
[325.28 --> 328.22]  Instead, I got the wild idea.
[329.02 --> 341.18]  Now, understand that it's technically actually not that crazy, but I got the wild idea to convert the extended four file system on that drive I was taking away from the Pi I was decommissioning.
[341.32 --> 343.40]  And I would plug it in to the new Pi.
[343.66 --> 351.54]  And when I plugged it in, before I mounted it, before I did anything in production, before I started up any containers, I converted it to ButterFS.
[351.54 --> 364.82]  Now, that isn't actually that crazy of a process unless you disconnect from your server in the middle of the conversion because it's too late at night and you are just an idiot.
[365.04 --> 366.30]  You're just a dumb idiot.
[366.70 --> 376.66]  You disconnect your SSH session while that session is running a ButterFS convert and you didn't use Screen or TMux because you're a dumb idiot.
[376.66 --> 384.92]  Then you can really muck up your file system and be in a data loss situation, which is where I found myself.
[385.36 --> 390.14]  I've heard a lot of different situations in which data loss is possible with ButterFS.
[391.20 --> 395.02]  And your experiences is just adding to that list, unfortunately.
[395.74 --> 398.60]  With MergerFS, there's no configuration file.
[398.60 --> 401.58]  It's just a line in your FS tab.
[402.14 --> 409.44]  So to add a new disk, you have, you know, slash mount slash disk one, colon slash mount slash disk two.
[409.66 --> 410.50]  And that's it.
[410.58 --> 410.96]  It's done.
[411.42 --> 415.18]  It supports drives which already have files on them.
[415.34 --> 418.54]  It supports pretty much any underlying file system.
[418.68 --> 419.78]  There's no striping.
[420.00 --> 421.60]  There's no magic, essentially.
[421.60 --> 428.98]  It's just merging files that live somewhere else in the Fuse user space, like file layer.
[429.62 --> 430.42]  Super simple.
[430.84 --> 434.56]  Supports USB drives, hot plugging of stuff as well.
[435.30 --> 436.78]  And it just works, you know.
[437.38 --> 440.14]  I've been using it for about five years now, I think.
[440.90 --> 442.68]  And zero complaints.
[443.32 --> 445.44]  Not what you want to hear right now, I'm sure.
[445.44 --> 453.92]  Well, you know, I have a bias against that kind of stuff in user space.
[454.14 --> 459.44]  For me, this should all be kernel level stuff and file system level stuff, like deep down in the OS.
[459.82 --> 460.16]  It should.
[460.50 --> 462.42]  I look at the systems out there.
[462.86 --> 471.48]  Apple has APFS, BSD has ZFS, and Linux for a built-in file system that's supported at the kernel level
[471.48 --> 474.58]  and also a decent candidate for low-end hardware.
[475.28 --> 477.58]  Your options are narrowed down to ButterFS.
[478.48 --> 481.90]  And I think when I looked at that volume add capability and I thought,
[482.12 --> 489.54]  the idea that I could add more storage like this with mismatched disks to this volume that I have my media on
[489.54 --> 493.70]  and it will just perpetually grow, well, that's sort of the Drobo promise.
[493.92 --> 499.36]  I can now have a Drobo-like promise in a Raspberry Pi file server.
[499.36 --> 502.14]  And it will be supported down at the OS level.
[502.46 --> 508.70]  And then just the other thing is, much like a ZFS does, I wanted a more robust file system
[508.70 --> 513.94]  that had a good set of user space tools to check my data and validate my data
[513.94 --> 516.98]  and take snapshots and do checksums.
[517.14 --> 522.08]  And I wanted copy-on-write for certain things, but I wanted to disable copy-on-write for other things.
[522.24 --> 526.62]  And these were all features that ButterFS gives me outside of the storage pooling.
[526.62 --> 532.14]  And so I opted, even after I had to rebuild the system and restore data,
[532.64 --> 536.04]  I opted to go with ButterFS again.
[536.70 --> 537.72]  So what's the lesson here then?
[538.18 --> 543.32]  I would have thought it would be, don't use ButterFS, but clearly you feel differently.
[543.68 --> 545.92]  Well, I mean, don't always do as Chris does.
[546.06 --> 551.64]  The Raspberry Pis themselves are a bit of an experiment in using this platform for serious work.
[551.64 --> 555.78]  And I think in that vein, it needs to have a file system that's serious.
[556.02 --> 561.08]  I'm not ButterFS's biggest advocate, but I do think it does offer certain functionality,
[561.70 --> 567.04]  like SSD trim support, that will add long-term life to my storage.
[567.30 --> 572.10]  And I'm hesitant to advocate for it, but I am interested in experimenting with it.
[572.34 --> 575.06]  I do think there was lessons learned in this.
[575.44 --> 577.72]  It may end up being ultimately don't use ButterFS.
[577.72 --> 582.76]  I'm not willing to make that call yet, but I should have just taken a backup of everything
[582.76 --> 583.72]  before I started.
[583.92 --> 586.32]  We're going to talk about cloud backup storage in a moment,
[586.42 --> 589.70]  and I'll talk about where mine really horribly failed me.
[590.40 --> 595.10]  But the bad was on me for not going there right before I started and taking a backup.
[595.74 --> 598.86]  I should have checked backups regardless, even if I didn't take one.
[599.18 --> 601.16]  I should have checked my backups before I started.
[601.16 --> 607.36]  And ultimately, I should have used screen or Tmux whenever I was doing something as critical
[607.36 --> 611.26]  as a file system conversion over an SSH session.
[611.52 --> 614.48]  Even if I had Ethernet, etc., etc., it doesn't matter.
[614.92 --> 618.22]  I should have been more cautious with that kind of thing.
[618.48 --> 620.34]  That's a sacred task you're performing.
[620.80 --> 624.54]  And I think if I hadn't been using my computer for other things, i.e. web browsing at the same
[624.54 --> 626.58]  time, I wouldn't have made that mistake.
[626.58 --> 633.36]  Yeah, you go into full details on Linux Unplugged episode 355, a lot more detail than this,
[633.42 --> 636.90]  actually, about the mechanics of what you were doing and everything.
[637.48 --> 643.28]  But one of the things that you raised that just made my heart go out to you was you'd
[643.28 --> 649.44]  started taking notes and documentation and applying some craftsmanship to this stuff.
[649.70 --> 654.72]  And you've effectively lost your entire configuration going back until March.
[655.36 --> 655.60]  Yeah.
[655.60 --> 656.08]  Yeah.
[656.58 --> 661.60]  This is really a lesson learned and something that people maybe can think about for their
[661.60 --> 662.72]  own backup strategies.
[662.94 --> 666.46]  But you guys probably, if you've been listening to the show, recall that I had a whole series
[666.46 --> 669.04]  of markdown notes using a web front end.
[669.24 --> 672.18]  And I had SmokePing and SyncThing.
[672.44 --> 675.14]  And I had the Libre Speed Test app.
[675.22 --> 679.56]  And I had a couple of other little tools I used to just monitor things in the RV.
[680.16 --> 682.40]  And all of this was running on this Raspberry Pi.
[682.40 --> 687.00]  And the configuration for all of that was being backed up with Duplicati, which I love.
[687.54 --> 692.86]  And that was being saved offsite with AES encryption to Google Drive because I've paid
[692.86 --> 695.26]  for a terabyte of Google Drive storage for a long time.
[695.26 --> 697.30]  And that was happening at 3 a.m.
[697.30 --> 700.68]  And that's one of those things where for months I'd check on it regularly.
[701.02 --> 703.80]  And every time I'd check on it, yep, it was there.
[704.50 --> 705.22]  Good, good, good.
[705.40 --> 709.40]  And then I had this little job that said, also then, now save a copy off to Dropbox.
[709.78 --> 713.62]  Another, you know, just spread it across two cloud storage providers that I have storage
[713.62 --> 716.26]  on and it's AES encrypted locally.
[716.26 --> 717.38]  So I'm good to go.
[718.04 --> 719.48]  And I stopped checking on it.
[720.06 --> 723.62]  Well, back in March, beginning of March, my debit card expired.
[723.88 --> 728.22]  And the way Google works is you have to go back in and re-enable each service that you
[728.22 --> 728.80]  subscribe for.
[728.80 --> 733.00]  So I added payment for YouTube TV and YouTube Premium.
[733.48 --> 738.36]  And I just kind of daftly assumed that my Google account now had the payment information.
[738.60 --> 740.00]  And so billing would resume.
[740.42 --> 742.42]  That was a critical mistake that I made.
[742.42 --> 746.78]  So if you're using cloud storage, and we always talk about using the cloud carefully,
[746.88 --> 749.04]  well, this was an area where I wasn't very clever.
[749.72 --> 752.74]  I have not really dug through my inbox to see if I have any alerts from Google.
[752.92 --> 753.24]  I may.
[753.84 --> 758.88]  But what ended up happening is I had nearly 900 gigs of storage on Google Drive.
[759.32 --> 761.26]  And they had reverted me back to the free tier.
[761.90 --> 768.42]  So Alex, I was using like nearly 880 gigs or 890 gigs out of 15 gigabytes.
[769.02 --> 769.60]  That's pretty impressive.
[769.60 --> 772.94]  So obviously, Google Drive wasn't accepting any new files.
[773.24 --> 774.54]  And that had been that way since March.
[774.66 --> 776.28]  So Duplicati had been failing.
[776.98 --> 780.36]  And I actually never logged into Duplicati to check the logs there because it's gone.
[780.44 --> 781.18]  It's gone now.
[781.96 --> 787.28]  So my backups are only as good as of March, which is the bulk of my documentation,
[787.48 --> 788.80]  but not all of my documentation.
[788.80 --> 794.56]  When I emigrated, I had a very similar situation to the point where I now have a Todoist reminder
[794.56 --> 797.54]  once a month to go in and manually check on Duplicati.
[798.04 --> 798.72]  That's a good idea.
[799.06 --> 799.98]  I should do that too.
[800.08 --> 802.40]  A recurring reminder to just check in on the backups.
[802.86 --> 803.08]  Thanks.
[803.14 --> 803.62]  Five minutes.
[803.62 --> 808.40]  And what's also good about doing that is you can go in and, you know, with Duplicati,
[808.50 --> 810.60]  it'll say, you know, drone footage backup.
[810.94 --> 813.30]  Last ran yesterday, took eight minutes.
[813.48 --> 821.06]  But I spotted today that my container app data backup to Google Drive took four hours last night.
[821.18 --> 822.16]  And I sort of think, huh?
[822.26 --> 822.80]  What's going on?
[822.80 --> 825.88]  So I went and looked at the ZFS datasets that I have.
[826.10 --> 831.22]  Turns out that MusicBrain's mirror is something like 15 or 20 gig a day.
[831.70 --> 836.78]  And obviously with copy on write, that space is being consistently used, you know, after snapshot,
[836.88 --> 837.32]  after snapshot.
[837.64 --> 842.54]  So yeah, just something to watch out for if you are going to do that self-hosted MusicBrain's mirror.
[845.70 --> 846.48]  Jeez, man.
[846.68 --> 848.22]  You know, you're not on Fiverr anymore.
[848.36 --> 849.04]  You know that, right?
[849.24 --> 850.00]  Yeah, I know.
[850.00 --> 854.98]  Yeah, I think maybe I was a little cavalier with using Google Drive.
[855.08 --> 858.04]  Not that there's really anything necessarily wrong with it.
[858.36 --> 862.02]  But I do not use Google Drive regularly.
[862.20 --> 866.16]  Like, I have used services that utilize Google Drive and save data there.
[866.56 --> 869.04]  But I'm not a frequent Drive user myself.
[869.42 --> 870.98]  Should be a lost result.
[871.44 --> 871.60]  Yeah.
[871.64 --> 875.12]  And so what ended up happening was I just didn't check it.
[875.12 --> 879.44]  And so I didn't notice for over a month and change that it wasn't current.
[879.44 --> 880.70]  That the subscription wasn't current.
[880.78 --> 885.38]  And then I only found out when I went to log in to go recover the backups.
[885.68 --> 890.48]  I think in retrospect, I probably should have used a better tool for me.
[891.02 --> 893.44]  And that would probably be something like Backblaze.
[893.50 --> 896.04]  Although I know you kind of did a deep dive into the services recently.
[896.18 --> 898.28]  So maybe you'd recommend something else.
[898.48 --> 901.88]  But as I'm rebuilding, that's my top candidate right now.
[902.20 --> 903.62]  Yeah, Backblaze looks pretty good.
[903.74 --> 906.02]  So yeah, let's break it down a little bit.
[906.02 --> 910.96]  There are two types of cloud backup strategies that you can adopt, really.
[911.60 --> 916.60]  One is a service, you know, like Backblaze or Glacier or rsync.net.
[916.78 --> 924.18]  And the other is to use some tools that plug into generic storage providers like Duplicati or Restic.
[924.18 --> 928.26]  And so, you know, we've talked a little bit about Duplicati just now.
[928.48 --> 931.76]  And we both use it plugged into Google Drive.
[931.94 --> 938.98]  Now, there is a hack over on the Data Hoarder subreddit where if you have G Suite for your domain,
[939.64 --> 945.56]  per user, officially in the T's and C's, there is a one terabyte per user limit to your Google Drive.
[945.56 --> 953.06]  But I have about three terabytes in mine, and it's been just fine for a year plus.
[953.32 --> 959.72]  If you get to five users officially, Google will remove that one terabyte per user cap,
[959.92 --> 961.94]  and everybody becomes unlimited.
[963.10 --> 967.94]  The nice thing here is that with the G Suite thing and a single user on the domain,
[968.14 --> 970.64]  they don't enforce the one terabyte limit anyway.
[970.64 --> 975.32]  So effectively, I'm using 3.5 terabytes of one terabyte.
[975.78 --> 979.10]  So with one user, you're pretty much good to go, or with five or more users.
[979.36 --> 980.18]  It just works.
[980.32 --> 984.98]  And it works with Rclone, which is another wonderful tool that lets you treat Google Drive
[984.98 --> 987.40]  effectively as a remote file system.
[988.22 --> 994.82]  Now, another tool, this one actually came onto my radar as part of the HomeLab OS review that we did.
[995.40 --> 996.66]  And this one's called Restic.
[996.66 --> 1000.64]  And again, the cost of this solution depends on the backend.
[1000.82 --> 1008.28]  So it supports local storage, SFTP, S3 endpoints, Google, etc., etc.
[1008.38 --> 1012.46]  I mean, the list is long for both Duplicati and Restic.
[1013.26 --> 1018.56]  But Restic is a single, no dependency binary written in Go,
[1019.26 --> 1022.98]  which allows you to do backups with snapshots and tagging as well.
[1023.22 --> 1024.56]  It's all command line driven.
[1024.56 --> 1027.80]  I don't believe there's a web interface like there is for Duplicati.
[1028.58 --> 1032.14]  So depends which floats your boat as to which one you prefer.
[1032.38 --> 1034.08]  I think they both have their pros and cons.
[1034.58 --> 1041.80]  Those are the two primary tools that I have looked into and are basically bring your own storage.
[1042.54 --> 1047.32]  But if you're looking for a service, you know, somebody that's going to provide that storage for you,
[1047.86 --> 1054.34]  Backblaze is probably for most of us, you know, home users is probably the big juggernaut in this space.
[1055.20 --> 1058.06]  Actually, when I went to their website earlier on my Linux desktop, it came up.
[1058.20 --> 1059.14]  Hello, Linux user.
[1059.64 --> 1065.98]  Do you want to go to our how to back up your server or back up your Linux machine page automatically,
[1066.12 --> 1067.10]  which I thought was kind of nice.
[1067.10 --> 1073.96]  And they recommend that you use something called Duplicati, which is kind of similar to Duplicati in name.
[1074.12 --> 1076.66]  And it took me a while to figure out they were actually two different tools.
[1077.88 --> 1085.22]  So Duplicati is the tool that Backblaze recommend that you use to interface with their servers from Linux.
[1085.22 --> 1086.96]  It's very appealing.
[1087.28 --> 1090.08]  You know, Backblaze is backup as a service, really.
[1090.62 --> 1097.94]  They have very simple pricing, $60 per year per computer, which led me to the obvious conclusion,
[1098.48 --> 1100.82]  given that I have a big NAS in my house.
[1100.82 --> 1107.34]  If I just backup all of my computers to my NAS, surely I can backup my NAS to Backblaze.
[1107.78 --> 1113.90]  And then I only have to pay the $60 and not, you know, five or six times $60 a year.
[1113.90 --> 1118.78]  Right. That's the model I think is appealing to me, especially with the big NAS here at the studio.
[1118.96 --> 1121.78]  That could be my local source of truth.
[1122.02 --> 1125.90]  And then using Duplicati, which is, by the way, a great tool.
[1126.14 --> 1131.28]  Because not only does it support Backblaze, but every single cloud storage you could conceive of,
[1131.66 --> 1136.38]  from Dropbox to FTP to even using IMAP as a storage backend.
[1136.56 --> 1137.46]  Like, it's everything.
[1137.78 --> 1139.98]  IMAP? That's cool.
[1140.26 --> 1141.64]  It's just wild, isn't it?
[1141.64 --> 1144.72]  And it uses LibRsync for incremental archives.
[1144.92 --> 1148.52]  So it's essentially using Rsync to do the Delta.
[1148.96 --> 1151.50]  And GNU PG to do the encryption.
[1152.02 --> 1153.48]  So it's pretty solid.
[1153.62 --> 1155.68]  And it's sending up, essentially, encrypted TARS.
[1156.04 --> 1156.76]  That's very cool.
[1157.60 --> 1162.44]  Now, another service that I've used in the past, this one was from my mom, actually.
[1162.44 --> 1168.40]  She has a two-bay Synology NAS that she stores all of her photos on, which lives under her stairs.
[1168.40 --> 1183.48]  And they have a plugin for Amazon's Glacier service, which is, there's some conjecture on the internet as to whether it's tape-based or whether it's hard drive-based or whether it's robots pulling hard drives out of servers and storing them in different places.
[1183.48 --> 1185.68]  I have no idea how it actually works.
[1185.82 --> 1190.30]  All I know is it's very, very cheap for long-term storage.
[1190.84 --> 1197.40]  Until, and this is where you have to be super-duper careful with Glacier, the retrieval costs can be extremely steep.
[1198.06 --> 1199.26]  So that's just something to bear in mind.
[1199.26 --> 1204.56]  And if you need that data quickly after a failure, Glacier might not be the best option for you.
[1204.98 --> 1211.68]  If you're willing to wait and download, I forget what the limits are exactly, but they have a daily limit of what you can download under a certain tier.
[1211.94 --> 1215.96]  You know, like Amazon loves to nickel and dime people in their cloud services.
[1216.52 --> 1220.48]  It just silently works and gets on with the job as part of a Synology plugin.
[1220.90 --> 1223.02]  There are other ways to interface with Glacier as well.
[1223.02 --> 1232.46]  A final service that I wanted to mention, and it's an honorable mention because it's very expensive for mere mortals like us, is rsync.net.
[1232.62 --> 1237.66]  They base all of their storage, they advertise it as being built on top of ZFS.
[1238.64 --> 1244.10]  The main selling point here is that rsync.net has been around for a very long time.
[1244.66 --> 1253.00]  And whilst they're quite pricey at two cents per gigabyte per month, you can interface with it using rsync, obviously, hence the name.
[1253.36 --> 1260.68]  Or ZFS send and receive, or any other tool that you can pretty much think of that runs on the Linux command line.
[1261.48 --> 1271.80]  It's run by a bunch of extremely knowledgeable Linux-y people, and comes very highly recommended whenever you look on, you know, rsysadmin or the more nerdy subreddits.
[1271.96 --> 1273.14]  I'm going to give a plug.
[1273.90 --> 1279.08]  For Tarsnap, for those of you who are truly paranoid, this is how Alan Jude backs up his taxes.
[1279.08 --> 1288.22]  So he doesn't backup everything, but the stuff that is really important, that isn't very large, but you want off-site, Tarsnap is the way to go.
[1288.46 --> 1294.70]  It's not the cheapest, but it is truly the one that has stood the test of time in terms of security.
[1295.50 --> 1297.56]  I'll put a link to that, or it's tarsnap.com.
[1297.56 --> 1303.28]  So that's like small-scale off-site backup, and you'll have to learn how to integrate with it because it is a little particular.
[1303.56 --> 1307.82]  But it might be the right fit for some of you for limited types of backups.
[1308.02 --> 1308.52]  All right.
[1308.56 --> 1311.46]  Should we follow up on the Home Assistant situation from last time?
[1311.46 --> 1312.80]  Yeah, I mean, I think they've listened.
[1313.10 --> 1331.28]  I think we can stand down from Red Alert and continue course because it appears the quote-unquote Home Assistant supervised method of putting Home Assistant with the supervisor on a generic Linux system via containers will be officially supported and documented.
[1331.64 --> 1331.96]  Hallelujah.
[1331.96 --> 1339.96]  Yeah, there are more name changes, but I think it's really great to see such a positive response to the community's feedback since our last episode.
[1339.96 --> 1344.94]  There is a blog post linked in the show notes, which covers all of the name changes.
[1345.28 --> 1350.14]  I picked up some changes in philosophy and how they're going to actually interface with the community moving forward.
[1350.22 --> 1357.98]  Instead of, I really felt like in the post that we talked about last week, the community was this big beast that they were trying to tame.
[1358.44 --> 1361.24]  Whereas in this post here, they're embracing it.
[1361.34 --> 1362.94]  And I'm so happy to see that.
[1363.08 --> 1365.00]  I thought it was really great that they listened.
[1365.22 --> 1366.96]  And yeah, great job, Home Assistant.
[1366.96 --> 1372.46]  Yeah, I do recommend you go through and read the supported installation methods, even if it's just to learn the vernacular.
[1373.18 --> 1380.80]  Home Assistant now refers to the all-inclusive home automation system with their OS, either via VM or some other method.
[1381.44 --> 1388.98]  Home Assistant container is now the new name for Home Assistant core, which is just the core of Home Assistant running in a container.
[1389.48 --> 1391.84]  It does not have the supervised experience.
[1391.84 --> 1393.36]  It's a new name.
[1393.44 --> 1396.04]  It was previously Home Assistant core on Docker.
[1396.20 --> 1398.06]  It's now just Home Assistant container.
[1398.62 --> 1400.68]  And then there's Home Assistant supervised.
[1401.34 --> 1406.12]  That is the method previously known as has.io on generic Linux.
[1406.40 --> 1414.46]  It is now the full Home Assistant experience with supervisor on the regular Linux operating system, the method that Alex and I use and love.
[1414.46 --> 1421.42]  And then Home Assistant core is just running the application directly on Python on a Linux box.
[1421.60 --> 1423.08]  No container, no VM.
[1423.22 --> 1425.96]  It's just your Linux install running the Python application.
[1425.96 --> 1428.20]  That is now known as Home Assistant core.
[1428.36 --> 1431.72]  But it's probably better to read everything because it'll sink in more.
[1432.02 --> 1435.74]  But now when you hear us refer to these things, that's what we're talking about.
[1435.94 --> 1437.76]  This is a little joke for the UK listeners.
[1438.22 --> 1441.82]  It's the Ron Seal naming strategy does exactly what it says on the tin.
[1441.82 --> 1445.46]  Then Home Assistant container, you don't need to explain what that does.
[1445.54 --> 1446.52]  It's just, it's obvious.
[1446.94 --> 1447.94]  So great, great job.
[1448.28 --> 1449.14]  Home Assistant supervised.
[1449.40 --> 1452.90]  You know I'm running it on a Linux box with containers and it's supervised.
[1453.28 --> 1453.50]  Easy.
[1454.24 --> 1456.36]  So yeah, Alex, I think overall I agree with you.
[1456.60 --> 1460.78]  I kind of have one thing to say about all of this and it's, whew.
[1461.32 --> 1462.74]  Yeah, thank goodness.
[1463.40 --> 1464.30]  Yeah, thank goodness.
[1464.38 --> 1465.32]  I was getting a little upset.
[1465.90 --> 1468.08]  Why don't we do a little wiki follow-up?
[1468.12 --> 1468.82]  It's been a minute.
[1469.18 --> 1469.86]  It has.
[1469.86 --> 1474.60]  Yeah, today we were watching the SpaceX launch get scrubbed, unfortunately.
[1475.66 --> 1480.32]  And whilst we were doing so, I was talking with somebody on the Discord about wikis.
[1480.66 --> 1487.14]  And it came to my attention that we were talking about Tiddlywiki and I was busy, you know,
[1487.40 --> 1488.82]  telling them just how much I love it.
[1489.04 --> 1491.12]  And we last talked about wikis on episode 12.
[1491.90 --> 1497.90]  And I wanted to just let you all know how much I love Tiddlywiki after that time.
[1498.20 --> 1499.08]  It's fantastic.
[1499.08 --> 1499.44]  Interesting.
[1499.56 --> 1502.38]  Ah, nice little long-term review follow-up, it seems.
[1502.48 --> 1503.06]  That's great.
[1503.36 --> 1504.00]  Well, kind of.
[1504.12 --> 1505.96]  I mean, yeah, what, three or four months?
[1506.50 --> 1509.56]  In 2020, three or four months feels like three or four years, but yeah.
[1510.08 --> 1510.90]  Yeah, exactly.
[1511.50 --> 1514.06]  Ah, so you're still in the love phase.
[1514.22 --> 1516.24]  Have you actually been using it on the regular then?
[1516.24 --> 1520.78]  I've been trying to use it whenever I start Googling something more than two or three times.
[1521.42 --> 1526.32]  For example, my low-power PFSense x86 build that I talked about in the previous episode.
[1526.72 --> 1531.92]  I was constantly looking for that serverbuilds.net forum post over and over and over.
[1531.92 --> 1538.22]  So I thought, why don't I just create a wiki entry, put the link in there, and then every time I need it, I just go to my wiki and find it.
[1538.48 --> 1545.66]  And then I can obviously include the content of that forum post in the wiki, so I don't even actually need to go to the forum anymore.
[1545.66 --> 1548.68]  It just speeds things up for me, no end.
[1548.86 --> 1549.46]  Yeah, it does.
[1549.60 --> 1551.48]  I've done that recently myself.
[1551.76 --> 1553.16]  That's how I did some of my documentation.
[1553.16 --> 1562.04]  But even just doing this rebuild, as I was reusing some of the same ButterFS commands over and over again, I just started a new document up.
[1562.12 --> 1566.66]  All right, let's start documenting these commands I use frequently, because it's a little different over here in Butterland.
[1566.98 --> 1569.10]  Create a personalized ZFS cheat sheet.
[1569.34 --> 1572.66]  That's something I've done, and I was thinking about trying to make it public.
[1572.66 --> 1576.92]  But then there's an awful lot of stuff in there that is actually personal.
[1577.28 --> 1585.62]  And so unfortunately, I don't think I can really find a way without hosting a second sanitized wiki, which is just a lot of work for me personally to do.
[1585.98 --> 1589.92]  We are still working on the wiki.selfhosted.show wiki.
[1590.44 --> 1598.40]  So if you're interested in contributing to that, head over to selfhosted.show slash discord, and you can talk to us about how to contribute.
[1598.40 --> 1610.26]  But going back to TiddlyWiki a little bit, a couple of key plugins that have made it really great for me is spending the time to configure the table of contents plugin as I would like it.
[1610.80 --> 1617.74]  And this is really, for me, the key thing that makes TiddlyWiki work so well for me personally.
[1617.74 --> 1621.28]  And I'm aware that, you know, picking a wiki is like picking a pair of shoes.
[1621.42 --> 1623.84]  It's a very personal type thing.
[1623.92 --> 1625.72]  I can't tell you what pair of shoes works for you.
[1625.78 --> 1627.18]  You just have to figure it out for yourself.
[1627.98 --> 1637.52]  But the reason I love TiddlyWiki so much is that if I have an article, and let's take, for example, something about home automation, flashing something with Tasmota, for example.
[1638.20 --> 1641.64]  You could probably think of five or six different categories that that article could live in.
[1641.76 --> 1642.96]  It could live in home automation.
[1643.46 --> 1644.72]  It could live in Tasmota.
[1644.72 --> 1648.34]  It could live in Shelly's IoT devices, whatever.
[1648.80 --> 1648.92]  Right.
[1649.42 --> 1658.48]  And in a normal hierarchical note structure, you'd have to pick one and stick with it or duplicate the article and put it in two or three different places.
[1658.80 --> 1662.98]  But with TiddlyWiki, I can set a tag on that Tiddler.
[1663.26 --> 1672.72]  I hate that name, but I can set a tag on that Tiddler and it will show up automatically in those three or four different categories that I set in the table of contents.
[1672.72 --> 1676.46]  So it just works in the same way that my brain does.
[1676.60 --> 1679.02]  And I find that incredibly powerful.
[1679.52 --> 1680.62]  Jog my memory, Alex.
[1680.72 --> 1683.26]  Are these all text files on the back end?
[1683.34 --> 1692.98]  Because through this whole catastrophe, I was so grateful that I had the original Markdown files on my file system so I could just use my built-in OS search to look stuff up.
[1693.04 --> 1694.30]  I didn't have to use the app.
[1694.64 --> 1695.34]  Yes, they are.
[1695.52 --> 1696.52]  I am happy to report.
[1697.10 --> 1699.50]  There's a couple of different formats that TiddlyWiki uses.
[1699.50 --> 1700.62]  One is Markdown.
[1700.86 --> 1707.54]  If you use the Markdown plugin, it just ends up as a regular .md file with a bit of front-loaded metadata at the front.
[1707.66 --> 1716.00]  It's got five or six lines of metadata that TiddlyWiki uses, but the actual content is completely unruined and untouched.
[1716.22 --> 1717.62]  It's vanilla Markdown.
[1718.48 --> 1727.88]  And the nice thing about that is it means I can use tools in Emacs like Deft, for example, or I can grep the files or I can open them in Vim or I can do whatever I want.
[1727.88 --> 1729.42]  Because it's just a plain text file.
[1730.12 --> 1735.02]  The only downside to that is it means adding images is still a little bit clunky.
[1735.28 --> 1740.88]  I have to add the image as a separate Tiddler and then link to that Tiddler from the one I'm writing.
[1741.12 --> 1744.46]  So it's a two or three step process instead of a one or two step process.
[1745.24 --> 1750.58]  That's the only negative I would say about TiddlyWiki is images are a bit of a pain.
[1750.58 --> 1756.06]  But once they're in and you figure out the workflow, it's absolutely not a showstopper at all.
[1756.22 --> 1761.42]  So the other format that they use is a .tid file, a .tid file.
[1761.76 --> 1766.78]  And again, that's largely just plain text with a little bit of front-loaded metadata in it.
[1767.14 --> 1767.84]  Well, thank you, Alex.
[1767.94 --> 1776.46]  I really like the idea of us doing long-term check-ins of different lengths as we try these things and coming back with our experience after having used them for a bit.
[1776.46 --> 1780.28]  Because that's often a lot different than when you first implement something.
[1780.54 --> 1781.78]  But it sounds like it's working for you.
[1781.98 --> 1782.44]  So that's cool.
[1783.02 --> 1785.68]  Let's do a hashtag Ask SSH.
[1786.18 --> 1789.54]  Mark from New Hampshire writes in with a question about Wi-Fi.
[1789.68 --> 1795.44]  He says a local charity are looking to outfit a property with solid Wi-Fi, both indoors and outdoors.
[1796.04 --> 1798.58]  My obvious go-to recommendation was Unify.
[1798.90 --> 1800.78]  But tell us, what else is there?
[1801.26 --> 1802.38]  Here are some requirements.
[1802.38 --> 1807.32]  And they're pretty extensive with some of them being pretty doable, some of them not.
[1807.48 --> 1810.80]  300-foot radius, two-feet-thick external stone walls.
[1810.92 --> 1812.46]  There's a lot of information in here, Alex.
[1813.32 --> 1815.32]  There's some areas where there's some water.
[1816.30 --> 1818.38]  They'd like support for multiple networks and VLANs.
[1819.10 --> 1822.66]  So they could have a caretaker network, a sensor network, a public network.
[1822.98 --> 1826.46]  Of course, it's going to need DHCP, bandwidth throttling on the public network.
[1826.46 --> 1832.42]  And some external remote management would be a plus because it can't always be on site to manage this thing.
[1832.92 --> 1833.44]  It's a tricky one.
[1833.50 --> 1838.18]  He asked me through the Discord server, you know, what should I buy?
[1838.24 --> 1840.80]  And I thought to myself, this would make a perfect Ask SSH.
[1841.40 --> 1844.36]  Because there's so many facets to this particular question.
[1845.14 --> 1847.66]  Some of the outbuildings don't have power, for example.
[1847.66 --> 1853.86]  So, you know, even running PoE is going to be tricky because they're 200 or 300 feet away.
[1854.08 --> 1857.50]  So you'd have to dig a trench and bury it in a conduit and it's not really feasible.
[1857.90 --> 1861.32]  So what we were looking for, you know, in terms of an answer for this was,
[1861.68 --> 1867.30]  if the answer is Unify, which particular Unify gear should they buy?
[1867.42 --> 1868.32]  Remember, this is a charity.
[1868.60 --> 1873.08]  So don't go crazy with, you know, super expensive enterprise gear.
[1873.08 --> 1878.66]  And if it isn't Unify, what else is there that would fill these needs?
[1879.24 --> 1881.28]  So I think the price is an interesting one.
[1881.62 --> 1887.48]  I know that young Chris would have reflashed some cheaper consumer routers off of eBay
[1887.48 --> 1889.44]  and distributed them around.
[1889.56 --> 1894.34]  I mean, I have done that and then use WDS as a network extender.
[1895.04 --> 1895.12]  Yeah.
[1895.38 --> 1895.98]  Oh, yeah.
[1896.52 --> 1899.64]  Also try the trick of just buying a bunch of cheap,
[1899.64 --> 1903.66]  the same exact routers and naming the SSIDs all the same
[1903.66 --> 1906.80]  and just distributing them sort of at the edge of each other's ranges.
[1907.62 --> 1910.62]  I have done that as well, but those are not centrally manageable.
[1910.84 --> 1913.18]  They're not going to give you multiple networks and VLANs.
[1913.46 --> 1916.40]  They're not going to give you, in some cases, bandwidth prioritization,
[1916.50 --> 1917.94]  although in some cases they actually will.
[1918.74 --> 1923.34]  So I think it's really, it's a question of how much Unify gear to buy
[1923.34 --> 1928.70]  versus a total DIY Wi-Fi setup, which I just wouldn't recommend anymore.
[1928.70 --> 1932.50]  Or even these days, mesh, is a mesh network a good idea?
[1932.78 --> 1936.36]  The cost there, though, that's what the trick is.
[1936.42 --> 1938.86]  And if you want a mesh network that really performs,
[1939.22 --> 1941.98]  your best route is to go with an Ethernet backhaul.
[1942.68 --> 1944.40]  That sounds like it's tricky in this scenario.
[1944.84 --> 1947.50]  Yeah, it's a historical reenactment society.
[1948.16 --> 1954.10]  And therefore, you know, they have some requirements around stringing cables.
[1954.64 --> 1955.90]  Not very easy for them.
[1955.90 --> 1960.74]  If we were like Mythbusters or the top gear of self-hosting podcasts,
[1960.90 --> 1963.28]  maybe in 20 years, Alex, when, you know, everybody's watching,
[1963.76 --> 1968.08]  you know what I would love to try is taking extension cords
[1968.08 --> 1969.62]  and running them out at these events
[1969.62 --> 1972.02]  and putting power over Ethernet adapters
[1972.02 --> 1973.98]  on different ends of the extension cords
[1973.98 --> 1978.92]  and seeing if you could actually use an extension cord
[1978.92 --> 1980.54]  as essentially an Ethernet cable.
[1981.26 --> 1982.22]  Wouldn't that be a fun experiment?
[1982.42 --> 1983.24]  I bet you it wouldn't work.
[1983.58 --> 1985.18]  Haven't you just described Powerline?
[1985.18 --> 1986.80]  Yeah, exactly. Powerline Ethernet.
[1986.86 --> 1987.52]  Yeah, that's what I'm talking about.
[1987.60 --> 1990.28]  But just take the extension cord and run it out to the yard
[1990.28 --> 1992.60]  with a Powerline Ethernet adapter on either side.
[1993.84 --> 1995.88]  It's the ugly uncle in this situation.
[1996.58 --> 1998.50]  Unfortunately for Mark,
[1998.60 --> 2000.86]  I don't believe that the remote buildings have any power,
[2000.98 --> 2002.94]  but that would be an interesting one.
[2003.02 --> 2006.02]  If Powerline was an option, that would solve something.
[2006.18 --> 2008.34]  When we get our self-hosted YouTube channel going,
[2008.46 --> 2010.14]  we'll do these kinds of experiments, right?
[2010.14 --> 2014.44]  In the meantime, I do think because of that central management
[2014.44 --> 2016.58]  and the support from multiple networks,
[2016.68 --> 2020.10]  you're going to want APs that can have multiple SSIDs
[2020.10 --> 2021.56]  and probably have multiple channels.
[2022.40 --> 2025.08]  Like, for example, one of the things I do with my guest networks
[2025.08 --> 2026.32]  is I just 2.4 those.
[2027.24 --> 2030.80]  IoT devices and public guest networks, just 2.4,
[2030.86 --> 2033.58]  and I reserve the higher bandwidths, the higher frequencies.
[2033.58 --> 2039.32]  All of my little ESP8266 boards only support 2.4 gigahertz,
[2039.48 --> 2040.34]  which helps.
[2040.64 --> 2041.60]  There's that too, yep.
[2042.04 --> 2047.06]  I have a dedicated IoT SSID, which only broadcasts on 2.4,
[2047.14 --> 2048.74]  so there's no question, right?
[2049.02 --> 2051.00]  All of these devices are on 2.4.
[2051.56 --> 2053.52]  I save the 5 gigahertz for the good stuff.
[2053.84 --> 2056.06]  I've got to be streaming my Plex at full bandwidth.
[2056.74 --> 2057.50]  That's exactly it.
[2057.54 --> 2058.34]  That's how I do it.
[2058.54 --> 2060.80]  And I make sure that the public network
[2060.80 --> 2064.50]  does not have any way to talk to the other networks.
[2064.60 --> 2067.26]  It just routes out to the internet, and that is it.
[2068.00 --> 2070.28]  But I think to put a cap on Mark's question,
[2070.90 --> 2073.58]  I would look at trying to run power out to the barn
[2073.58 --> 2076.06]  and then use the barn as a redistribution point
[2076.06 --> 2077.30]  when you look at his setup here
[2077.30 --> 2080.88]  and try to just get it down to three APs with a controller,
[2081.30 --> 2083.32]  and I think you're probably going to just find
[2083.32 --> 2085.22]  that the UniFi products are the best for that.
[2085.76 --> 2086.96]  Let us know how it goes, Mark.
[2086.96 --> 2088.28]  In fact, if you have a question,
[2088.58 --> 2090.30]  or maybe you have a suggestion for Mark,
[2090.80 --> 2093.08]  go to selfhosted.show slash contact,
[2093.74 --> 2097.14]  or hit us up on Twitter with the hashtag AskSSH,
[2097.66 --> 2099.40]  and we'll try to get it into a future show.
[2099.50 --> 2100.14]  We love doing those.
[2100.56 --> 2102.36]  Still trying to figure out what the other S stands for.
[2102.60 --> 2104.16]  Yeah, maybe they could tweet us and let us know.
[2104.32 --> 2106.30]  Give us a suggestion for that extra S.
[2106.74 --> 2109.08]  You know, while we were talking about MergerFS today, Alex,
[2109.46 --> 2112.68]  I remembered that it was kind of a while ago,
[2112.76 --> 2115.62]  but there is an extra you did with the MergerFS developer.
[2115.62 --> 2116.14]  Correct.
[2116.42 --> 2120.14]  That is extras.show slash 28, if you're interested in that.
[2120.14 --> 2124.52]  Myself, Brent, and Drew sit down with Antonio,
[2124.72 --> 2125.36]  who's the developer,
[2125.58 --> 2129.50]  and we talk through the motivations behind creating MergerFS,
[2129.82 --> 2131.08]  along with a bunch of other stuff as well.
[2131.22 --> 2134.56]  So if you're interested in that one, extras.show slash 28.
[2135.30 --> 2137.54]  You can find me on Twitter at Ironic Badger.
[2137.54 --> 2139.32]  I'm at Chris LAS.
[2139.72 --> 2141.74]  The show is at SelfHostedShow.
[2141.94 --> 2144.50]  And the network is at JupyterSignal.
[2144.86 --> 2146.10]  That's a lot of Twitter handles.
[2146.60 --> 2148.10]  It's too many Twitter handles, Alex.
[2148.44 --> 2151.20]  We need to write a bot that will iterate over an array of Twitter handles for us
[2151.20 --> 2152.60]  and just spout it out on air.
[2152.86 --> 2153.76]  We need Twitter Raid.
[2153.86 --> 2154.48]  That's what we need.
[2155.22 --> 2156.42]  Redundant array of Twitter handles.
[2156.42 --> 2159.18]  What does that even mean?
[2160.08 --> 2161.16]  And so thanks for listening, everyone.
[2161.32 --> 2163.80]  That was SelfHosted.show slash 20.
