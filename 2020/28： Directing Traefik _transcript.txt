[0.00 --> 7.76]  Coming up on today's show, we get fancy with traffic labels and then gush over some of the new Home Assistant features while we save our data from certain failure.
[8.40 --> 9.10]  I'm Chris.
[9.56 --> 11.26]  And I'm Alex, and this is SoFosted.
[12.50 --> 18.88]  I'm so excited. Autumn is here. The fall is here. I'm wearing jeans today for the first time in five months.
[19.20 --> 22.74]  Yeah, I'm wearing pants too, and I don't typically podcast with pants.
[23.22 --> 27.10]  I love that that's a thing. I don't typically podcast with pants.
[27.10 --> 33.16]  It's too warm. You know, a gentleman wants to be comfortable, so that way his analysis is comfortable.
[34.76 --> 35.78]  You got nothing?
[38.44 --> 41.50]  You're just thinking back over all the episodes pantless.
[41.92 --> 44.02]  Hey, I didn't say I'm not wearing shorts, Alex, you know?
[44.20 --> 48.32]  I was thinking that you do what you're thinking with your dick, so you've got to keep that at the correct temperature.
[49.62 --> 51.84]  Well, let's just say I can't think if it's too warm.
[52.04 --> 55.66]  But then thought that probably wasn't radio appropriate.
[55.66 --> 57.00]  No, of course not.
[57.10 --> 59.78]  No, of course not. No. No, of course not.
[59.88 --> 66.42]  You know, what we ought to do is maybe not talk about our pants and instead talk about, you know, self-hosting things.
[66.96 --> 67.26]  Maybe.
[67.26 --> 72.68]  This episode is brought to you by a cloud guru.
[73.06 --> 77.48]  Are you looking to get a high-paying career, maybe move into the cloud and make some good change?
[77.92 --> 80.88]  Well, there's no better place to start than getting a certification.
[81.36 --> 84.36]  ACG has helped more than 2 million people scale up on the cloud.
[84.46 --> 87.12]  AWS, Azure, and Google Cloud Platform.
[87.84 --> 90.30]  Head over to cloudguru.com and get started.
[90.30 --> 93.06]  So let's crack things off with a public service announcement.
[93.32 --> 93.56]  All right.
[93.68 --> 97.98]  The Linux server.io team have made some changes to their reverse proxy.
[98.22 --> 101.72]  So for many, many years, they've released a Let's Encrypt container.
[101.98 --> 106.14]  Now they've been contacted by Let's Encrypt to enforce their trademark.
[106.14 --> 107.48]  So they've had to rename it.
[107.98 --> 111.86]  They've renamed it SWAG for Secure Web Application Gateway.
[112.64 --> 113.38]  Oh, okay.
[113.42 --> 115.26]  I thought it was going to be security we all get.
[116.02 --> 116.54]  It could be.
[116.66 --> 118.16]  I mean, it's an acronym.
[118.30 --> 119.42]  It can be whatever you want, right?
[119.68 --> 120.40]  I like to think so.
[120.84 --> 123.86]  It's a drop-in replacement for the existing Let's Encrypt container.
[124.26 --> 126.36]  And there is a blog post linked in the show notes.
[126.66 --> 131.26]  So if you're running the old one, it's going to stop being updated in favor of this new one.
[131.32 --> 133.96]  Just go ahead and update your compose file or whatever you're doing.
[133.96 --> 139.18]  Well, you know, big congratulations to Linux server.io for getting large enough that they
[139.18 --> 141.60]  showed up on the trademark radar of Let's Encrypt.
[141.68 --> 142.28]  That's a milestone.
[143.02 --> 145.40]  I think they're at about 12 billion pulls these days.
[145.54 --> 146.60]  So they're doing pretty well.
[147.00 --> 147.64]  Woo-wee.
[148.00 --> 148.48]  I know.
[148.56 --> 149.06]  I'm one of them.
[149.18 --> 155.16]  I just pulled down my new images for Plex, SyncThing, and a few other very handy backend
[155.16 --> 158.00]  services that are Linux server.io Docker images.
[158.62 --> 162.90]  So I'll have a link to that, like Alex said, self-hosted.show slash 2.8.
[162.90 --> 166.94]  We'll talk a little bit more about some new Linux server image that's been released this
[166.94 --> 167.18]  week.
[167.34 --> 171.10]  But first, I've been experimenting with traffic.
[171.58 --> 175.14]  It's spelt T-R-A-E-F-I-K.
[175.32 --> 179.02]  So traffic is kind of how it's spelt, but I think everybody just says it traffic.
[179.50 --> 179.72]  Yeah.
[179.82 --> 181.54]  We've talked about it a little bit before on the show.
[181.76 --> 186.90]  Now, in the last episode, I mentioned lychee, which by the way, if you're American is pronounced
[186.90 --> 187.48]  lychee.
[187.64 --> 190.34]  And if you're from the UK is pronounced lychee.
[190.46 --> 191.62]  I went on Wikipedia and checked.
[191.62 --> 194.50]  Oh, that's not confusing at all.
[194.72 --> 194.88]  Okay.
[196.52 --> 197.36]  Potato, potato.
[197.86 --> 198.22]  Anyway.
[198.54 --> 198.88]  Right.
[199.10 --> 202.72]  So I started building out some infrastructure using our new sponsor, Linode.
[203.02 --> 205.40]  I was using Ansible and Terraform to do this.
[205.76 --> 211.52]  And one of the things that I like to do is use ginger templating to create my Docker compose
[211.52 --> 212.12]  files.
[212.42 --> 217.84]  This means I can store all of my container variables in Ansible, run it through the ginger
[217.84 --> 221.42]  templating engine and it spits out a Docker compose file on the other side.
[221.82 --> 226.76]  Now, when I was using Nginx as my reverse proxy, it meant I had to also have an Ansible
[226.76 --> 231.78]  role that copied across and installed the relevant Nginx configuration files.
[231.78 --> 236.66]  And for anybody that's ever worked with those files, they can be a little bit picky and a
[236.66 --> 237.66]  little bit cryptic.
[238.70 --> 243.60]  The best thing, the single best thing about traffic is that all of the configuration now
[243.60 --> 248.40]  for my reverse proxy lives alongside each container as a label.
[248.40 --> 249.14]  Yeah.
[249.24 --> 254.06]  Talk about this label thing, because I'm not a traffic expert, but that's my essential
[254.06 --> 258.02]  understanding is that it sort of assigns what you can do based on your label.
[258.56 --> 258.92]  Correct.
[259.14 --> 260.56]  I'm still wrapping my head around it.
[260.60 --> 260.86]  Right.
[261.10 --> 263.94]  And it's something I've been using for about a month now.
[264.84 --> 268.10]  I had a lot of help with some of the guys on Discord in particular.
[268.44 --> 270.82]  I know I seem to mention Discord every week, but...
[270.82 --> 271.76]  There's a lot going on over there.
[271.80 --> 272.62]  That's where the fun is.
[272.62 --> 282.72]  So I've put together a kind of beginner's guide to traffic, but not as a blog post for
[282.72 --> 283.06]  once.
[283.38 --> 288.90]  What I've actually done is I've just put a compose file in my infrastructure repo.
[289.00 --> 289.64]  Oh, okay.
[289.70 --> 290.16]  Up on GitHub.
[290.62 --> 292.80]  And a link to that, of course, is in the show notes.
[293.72 --> 298.74]  And in there, what you can hopefully see is just how simple this thing is to configure.
[298.74 --> 302.18]  So you define a series of routers and services.
[302.84 --> 308.18]  And as part of those routers and services, you define the host name and the entry point
[308.18 --> 308.92]  you want to use.
[309.18 --> 311.54]  So for me, I use Cloudflare for my DNS.
[312.46 --> 318.54]  So traffic will automatically talk to Cloudflare as part of the ACME process to get my TLS certificates
[318.54 --> 319.54]  from Let's Encrypt.
[319.98 --> 325.56]  So I tell each container to use that particular certificate resolver, Cloudflare.
[325.56 --> 329.72]  And then from there, I tell the router which service to use.
[329.94 --> 334.88]  So for example, for Nginx, if I'm running that as a container behind traffic, would be
[334.88 --> 338.40]  on port 80 or Plex would be on 32400, for example.
[339.14 --> 340.14]  It's just super simple.
[340.66 --> 341.90]  And where are you defining this?
[342.08 --> 343.78]  Where does that information get stored?
[344.10 --> 344.84]  What mechanism?
[345.36 --> 346.26]  That's the best part.
[346.98 --> 354.06]  So with Nginx, for example, it would be in a Docker volume that I would mount through a
[354.06 --> 356.00]  bind mount system to my container.
[356.20 --> 361.24]  And then those reverse proxy configuration files need to persist on my host.
[361.92 --> 361.94]  Right.
[362.38 --> 366.54]  With traffic, it's a label that lives in the Docker compose file.
[366.66 --> 371.66]  So right next to where I'm saying I want to run, you know, Linux server slash Plex, for
[371.66 --> 377.30]  example, I then have a label section with five lines in it that says traffic enable true.
[377.30 --> 379.62]  Use this host name.
[379.68 --> 381.62]  So Plex dot KTZ dot whatever.
[382.40 --> 384.96]  Use this entry point of Web Secure.
[385.08 --> 386.58]  So HTTPS, for example.
[387.10 --> 389.96]  And then use the cert resolver of Cloudflare.
[390.12 --> 391.08]  This is the fourth line.
[391.18 --> 394.44]  And then the fifth line is use port 32400.
[394.92 --> 395.86]  And it's just right there.
[395.92 --> 396.48]  It's simple.
[396.86 --> 398.52]  It's easy to read YAML.
[398.60 --> 400.14]  That's just in the Docker compose file.
[400.14 --> 403.08]  And I think that's the part that really has to be underscored.
[403.32 --> 407.48]  And it's so tidy because it's right there with all of the other information about that
[407.48 --> 407.86]  container.
[408.06 --> 413.32]  It's easy to read, easy to replicate and associated and attached with that container.
[413.92 --> 419.96]  And because it's in that single file, if I commit that single file to Git, I have a history
[419.96 --> 421.50]  forever until the end of time.
[422.28 --> 426.10]  Exactly what my configuration parameters were for that specific container.
[426.10 --> 431.24]  Whereas if I'm relying on a bunch of different files that are on my file system in different
[431.24 --> 436.52]  directories and stuff like that, who's to say that my Ansible role don't have a bug in
[436.52 --> 440.32]  it that doesn't overwrite that particular file when I change the name of the container
[440.32 --> 442.20]  or whatever it is.
[442.22 --> 446.82]  There's just a whole bunch of edge case scenarios that this solves for me.
[446.90 --> 448.40]  And I absolutely love it.
[448.88 --> 450.98]  How are you choosing what gets committed to Git?
[451.08 --> 453.24]  Are you, is it every config file?
[453.38 --> 455.66]  Are you hand committing certain config files?
[455.66 --> 456.54]  What's the system there?
[457.12 --> 461.04]  Well, I have a blog post about working with Ansible and secrets.
[461.28 --> 467.58]  The short version of that is I use the Ansible vault functionality to encrypt a couple of files
[467.58 --> 468.26]  in my repo.
[468.80 --> 473.44]  All of the secret source lives in that encrypted file.
[474.80 --> 481.50]  Ansible then interpolates through its templating engines, those variables into the playbooks when
[481.50 --> 482.12]  it runs.
[482.70 --> 484.94]  Ansible looks for a specific variable.
[484.94 --> 490.02]  If it can't find it in a decrypted file, it will go to the encrypted file and look for
[490.02 --> 490.22]  it.
[491.00 --> 497.84]  And so for me, I generally tend to go with the approach that anything that's personally identifiable,
[497.84 --> 504.30]  like an IP address or a serial number or an API key, obviously a secret.
[504.30 --> 509.48]  Just anything that I would rather somebody else didn't know, I tend to put in the vault file
[509.48 --> 512.96]  and then use my Ansible roles to decrypt.
[512.96 --> 519.34]  Now, the downside of that is it means it has to live in plain text on disk somewhere.
[519.74 --> 525.50]  But the reality of being a sysadmin is that at some point somewhere, something's got to
[525.50 --> 526.24]  be in clear text.
[526.34 --> 530.60]  Somebody has to have the ultimate password somewhere, even if it's in your brain.
[531.46 --> 533.04]  Encryption is great.
[533.04 --> 537.34]  But at some point somewhere, somebody needs the key to that vault.
[537.98 --> 539.10]  Well, that's pretty cool, Alex.
[539.38 --> 540.98]  I like that I can just go in here and read this.
[541.26 --> 545.34]  And that also makes it very easy for me to get started because this, being able to actually
[545.34 --> 549.24]  see this example here, which we'll have linked in the show notes, really makes it click for
[549.24 --> 549.44]  me.
[549.68 --> 554.04]  Like, because the other thing we haven't even talked about is the user front end web UI
[554.04 --> 555.48]  to traffic and all of that stuff.
[555.48 --> 561.80]  But fully understanding how I label stuff in Docker Compose kind of completes my understanding.
[561.96 --> 564.46]  And now I really kind of see why people are talking about traffic.
[564.66 --> 565.64]  It looks really nice.
[566.16 --> 571.62]  There was a big change in how traffic defined their routers and services and front ends and
[571.62 --> 574.06]  back ends between v1 and v2.
[574.16 --> 576.40]  Now, we're talking about v2, the current release.
[576.78 --> 582.16]  Now, in v1 times, I just wrote them off as cluttering my Docker Compose file.
[582.26 --> 582.96]  I didn't want that.
[582.96 --> 585.04]  I didn't want that clutter in my file.
[585.26 --> 590.78]  But as I've kind of matured my approach to, you know, configuring all these different systems,
[590.78 --> 594.38]  I now have my personal server at home.
[594.48 --> 598.46]  I have a cloud instance that I configure that runs all my websites, you know, my blog and
[598.46 --> 601.76]  stuff like that and some stuff for my family as well.
[601.92 --> 606.70]  I then have the self-hosted infrastructure and a couple of other things I also look after.
[607.12 --> 612.86]  By the time I'm scaling this to five, six, seven different sites, it's just really nice
[612.86 --> 616.02]  to have one single source of truth be that Compose file.
[616.44 --> 616.62]  Yep.
[616.94 --> 617.50]  Amen to that.
[617.56 --> 618.34]  That's how I feel too.
[619.48 --> 620.92]  Well, you heard Alex mention it.
[621.18 --> 621.78]  We use it.
[621.90 --> 622.38]  We love it.
[622.72 --> 622.98]  Linode.
[623.16 --> 625.40]  Linode.com slash SSH.
[625.66 --> 628.72]  Get a $100 60-day credit on new accounts.
[628.72 --> 630.36]  And here's a little pro tip.
[630.36 --> 637.24]  Linode just posted a guide on using object storage as a backend storage mechanism for
[637.24 --> 641.36]  Nextcloud where you can kind of just have unlimited space, but you also take advantage
[641.36 --> 644.24]  of their crazy fast storage.
[644.80 --> 646.24]  And it's what we use.
[646.28 --> 648.00]  It's how we do it here at Jupyter Broadcasting.
[648.00 --> 652.68]  And so I'm going to put a link to this in the show notes because Linode is simple cloud
[652.68 --> 654.86]  infrastructure that you can spin up for anything you need.
[655.18 --> 657.94]  A shared host is something with dedicated GPUs or CPUs.
[658.02 --> 660.26]  Everything's priced really reasonable.
[660.48 --> 664.32]  And they have a cloud management UI to take care of all of it.
[664.48 --> 667.92]  You just get started by going to linode.com slash SSH.
[668.20 --> 672.16]  You mentioned, Alex, that you were deploying some systems with Terraform on Linode.
[672.22 --> 673.32]  What's that process like?
[673.58 --> 675.34]  It's been really, really easy, actually.
[675.34 --> 681.22]  The documentation up on Terraform providers website is very well written, very well documented.
[681.98 --> 686.06]  And if you would like to see a full example, of course, there's a link in the show notes
[686.06 --> 688.90]  to the self-hosted infrastructure repo that I'm using.
[689.76 --> 693.48]  And in there, it's just been really simple, really straightforward to get started.
[694.22 --> 694.62]  That's nice.
[695.00 --> 698.70]  That is really nice because you can plug it in with an orchestration suite you're already
[698.70 --> 701.66]  using or take advantage of the tools that they have.
[701.66 --> 705.94]  And what's great about Linode is they're the largest independent open cloud provider
[705.94 --> 708.70]  in the world with 11 global data centers.
[709.40 --> 712.68]  Linode's been around for about as long as user mode Linux has been around.
[712.98 --> 717.86]  Their founder saw the opportunity and built something that was accessible for just about
[717.86 --> 719.68]  everyone, just about everywhere.
[719.88 --> 722.62]  So go to linode.com slash SSH to get started.
[722.82 --> 724.78]  And then check out the app marketplace, for example.
[725.08 --> 728.70]  An easy way to self-host your own applications and get started with their stack scripts.
[728.70 --> 733.68]  Another nice way to build a quick and easy system, reproducible easy system.
[733.96 --> 737.46]  I just recently decided I'm going to set up a dedicated SSH jump host.
[738.22 --> 739.80]  At first, it sounds kind of crazy.
[739.98 --> 745.84]  But then I realized at $5 a month, I can really go all in on the security on this box, maybe
[745.84 --> 747.62]  even kind of as a learning opportunity.
[747.94 --> 750.92]  And it'll be my jump host system to get around wherever I need to go.
[751.14 --> 753.60]  That's a great use for the $5 a month system.
[753.60 --> 759.98]  But our matrix box that runs the Jupyter Broadcasting matrix server, that's a little more powerful.
[760.22 --> 763.86]  We went ahead and did a dedicated CPU for that one because there's hundreds of users
[763.86 --> 764.68]  using that system.
[764.96 --> 766.14]  And that's the great thing about Linode.
[766.30 --> 767.80]  They've been around for a long time.
[768.14 --> 770.10]  They're the largest independent open cloud provider.
[770.34 --> 774.24]  And they've got a great pricing structure and a very competitive dashboard.
[774.38 --> 775.40]  You got to go check them out.
[775.78 --> 777.36]  Linode.com slash SSH.
[777.48 --> 780.40]  And a big thank you to Linode for sponsoring the self-hosted program.
[780.40 --> 784.14]  Last week, we celebrated our birthday.
[784.56 --> 787.44]  And this week, it's Home Assistant's birthday.
[787.96 --> 788.98]  Yeah, only we get the presents.
[789.20 --> 789.90]  How great is that?
[790.66 --> 791.78]  We get all the new stuff.
[792.44 --> 796.12]  This is one of those things like before the show, Alex and I were like, how do we cover
[796.12 --> 796.40]  this?
[796.42 --> 801.14]  Because we could probably, I bet you make two episodes out of just the updates in this
[801.14 --> 801.78]  one release.
[802.12 --> 803.34]  This was a really big one.
[803.58 --> 808.96]  So we thought maybe instead we'd just pull out like two or three of like the heavy hitters
[808.96 --> 811.74]  and just talk about those and then link you to the resources.
[812.62 --> 816.90]  For those of you that haven't listened to the show for a while, Alex and I, big Home Assistant
[816.90 --> 817.38]  users.
[817.64 --> 819.40]  In fact, I use it more than ever these days.
[819.52 --> 820.12]  I don't know about you.
[820.18 --> 821.18]  I think you too, Alex, right?
[821.32 --> 821.66]  Huge.
[821.84 --> 822.04]  Continue.
[822.30 --> 822.58]  Huge.
[822.88 --> 824.50]  I love the Home Assistant.
[825.02 --> 827.26]  Well, the Home Assistant has the new release.
[827.50 --> 831.00]  And I think probably the thing you're excited about, the thing I'm looking forward to is
[831.00 --> 832.06]  NFC tag support.
[832.18 --> 833.28]  I think that's going to be a big deal.
[834.64 --> 836.72]  It's really, really easy as well.
[836.72 --> 840.86]  So they've updated the companion apps that run on iOS and Android.
[841.10 --> 844.80]  So you can actually write the NFC tags directly from the app on your phone.
[845.38 --> 849.44]  And then as soon as you scan it, you can assign automations to it.
[849.64 --> 854.38]  So as part of this release this week, the automation engine has had a complete overhaul.
[854.46 --> 857.98]  So now the YAML based automation stuff is a lot better than it used to be.
[858.66 --> 863.30]  And so one of the things I've decided to do is stick an NFC tag on the outside of my
[863.30 --> 867.64]  house so I can tap my phone to the outside of my house and have it open my garage door,
[867.80 --> 868.24]  for example.
[868.92 --> 873.12]  Can't tell you the number of times I've been outside my house without my keys thinking,
[873.42 --> 874.88]  I need to get in.
[875.10 --> 876.32]  But my keys are on the inside.
[876.44 --> 878.14]  And the only door that's open is the back door.
[878.20 --> 879.94]  But I want to go in the front door right now.
[880.04 --> 882.52]  And this should be a solved problem.
[882.76 --> 884.04]  And I want to be lazy, dang it.
[884.04 --> 886.34]  No, I completely agree.
[886.52 --> 893.34]  So the mixer I have here, the Behringer X32, has a built-in spot for your cell phone.
[893.50 --> 894.08]  It's weird.
[894.24 --> 898.32]  I've never seen a mixer that does this, but it actually has a little spot for you to place
[898.32 --> 899.18]  your cell phone on the mixer.
[899.22 --> 903.88]  And that's because it has, I think, a mobile app where you can control some of the mixer
[903.88 --> 904.22]  settings.
[904.80 --> 905.66]  You know what I did?
[906.28 --> 908.18]  Put a little NFC tag right in that spot.
[908.18 --> 912.90]  So when I set my phone down in its holder on the mixer, it turns on my lights.
[913.04 --> 914.38]  It changes the colors.
[914.72 --> 916.60]  It just sort of gets things ready to go.
[916.68 --> 920.98]  So I don't have to come in here and, you know, I don't even have to speak to an Echo or anything.
[921.08 --> 924.42]  It just put it right down there and it communicates with the home assistant we have here at the
[924.42 --> 924.64]  studio.
[924.86 --> 926.38]  I love this feature.
[926.70 --> 927.58]  And I'm going to do the same thing.
[927.62 --> 929.24]  I'm going to put a little tag outside.
[929.34 --> 931.88]  I'd like to find a black colored NFC tag.
[931.94 --> 933.50]  All the ones I have right now are white stickers.
[934.28 --> 936.80]  I found some heavy duty outdoor grade ones.
[936.98 --> 937.52]  Oh, really?
[937.52 --> 938.68]  They're about a buck each.
[938.74 --> 940.78]  So they're quite expensive for NFC tags.
[941.12 --> 941.42]  It's OK.
[941.48 --> 943.94]  It's got to survive going down the road and in the rain.
[944.42 --> 946.06]  So I'll put a link in the show notes.
[946.50 --> 947.26]  OK, that'd be great.
[947.34 --> 951.18]  Yeah, that's the kind of thing I think I want to do is put something outside and just turn
[951.18 --> 951.98]  lights on and whatnot.
[952.40 --> 956.22]  You know, I came up with quite a fun thing to automate in this house.
[956.54 --> 960.78]  My wife loves classical music and I love sort of rock music, you know, like Tool and Green
[960.78 --> 961.56]  Day and stuff like that.
[961.98 --> 967.44]  And so when we're cooking, we both generally want the opposite person's playlist to never be
[967.44 --> 967.88]  in existence.
[967.88 --> 974.16]  And so I've 3D printed a violin and a guitar and I've put the NFC tags on the back of these
[974.16 --> 975.66]  3D printed things.
[975.82 --> 980.82]  And I just tap the thing that I want and it plays it through Spotify through my Google
[980.82 --> 981.74]  Home in the kitchen.
[982.54 --> 984.46]  That is a clever idea.
[984.58 --> 987.84]  I like the use of the 3D icon really to drive it home.
[988.24 --> 989.56]  Makes it a physical thing you're touching.
[989.56 --> 990.12]  Yeah.
[990.78 --> 995.38]  And then the other thing I've done is when it's bin day, we have a little picture of
[995.38 --> 1000.08]  a bin, which I've 3D printed again and put next to the bins in the kitchen.
[1000.34 --> 1003.98]  So we tap that and it turns all the lights in the whole house on so we can walk around
[1003.98 --> 1005.48]  for 20 minutes, empty all the bins.
[1006.02 --> 1011.88]  But then it also turns on the driveway lights, opens the garage door so you don't have to
[1011.88 --> 1012.46]  do anything.
[1012.56 --> 1014.08]  The house is just ready for you to go out.
[1014.12 --> 1014.64]  Because you know what?
[1015.10 --> 1017.02]  When you're emptying the bins, you know what you're going to do.
[1017.02 --> 1020.58]  You're going to walk around, empty the bins, then go outside, put it in the big plastic
[1020.58 --> 1023.56]  ones outside, put them at the end of your driveway and then come back in again.
[1024.22 --> 1025.36]  Yeah, that's fantastic.
[1025.66 --> 1029.92]  I have a series of like outdoor lights and a couple of other things that I need to quickly
[1029.92 --> 1031.88]  take down and pack up.
[1031.96 --> 1033.72]  And what I have to do now is I'm outside.
[1034.00 --> 1038.70]  I have to bring out my phone and I load the Home Assistant UI and then I tap them off
[1038.70 --> 1039.72]  before I unplug them all.
[1039.82 --> 1042.60]  So that way they're in an off state when I remove them from the network.
[1043.00 --> 1046.96]  And I could just put an NFC tag out there and just totally do it that way.
[1047.02 --> 1048.24]  You totally could.
[1048.36 --> 1048.52]  Yeah.
[1050.02 --> 1056.90]  The magic part is with this bin automation, I'm very proud of this one, is when it starts,
[1056.98 --> 1060.66]  it takes like a snapshot of the current scene of the house.
[1060.86 --> 1061.02]  Yeah.
[1061.06 --> 1067.30]  So all the lights that are currently on are stored to a temporary state, if you like, a
[1067.30 --> 1068.38]  temporary scene.
[1068.38 --> 1073.82]  And 20 minutes later, when the bin automation finishes, that scene gets recalled and the
[1073.82 --> 1075.78]  house just returns to how it was before.
[1076.40 --> 1078.84]  Oh, so the previous state is restored.
[1078.98 --> 1079.84]  That's great.
[1080.18 --> 1081.26]  That is nice.
[1081.40 --> 1082.36]  That's a real that's.
[1082.64 --> 1086.50]  See, now you're getting fancy with the automations, with the 3D printing and the restoring the
[1086.50 --> 1087.30]  previous state.
[1087.40 --> 1088.90]  Like that's next level stuff there.
[1089.24 --> 1090.84]  Guy gets bored, particularly in lockdown.
[1091.40 --> 1091.64]  Yeah.
[1091.64 --> 1093.18]  And we love ourselves some home assistants.
[1093.18 --> 1099.76]  So the other thing that is noteworthy for Mac users and perhaps an indication of the
[1099.76 --> 1103.80]  knock-on effects of the upcoming Apple ecosystem with ARM processors in the Macs too.
[1104.44 --> 1108.64]  But home assistant companion app for the Mac is now a reality.
[1108.84 --> 1109.30]  It's early.
[1109.56 --> 1110.20]  It's rough.
[1110.20 --> 1114.40]  But the thing that's neat here, and I'd like to put a call out to the audience to see if
[1114.40 --> 1119.96]  we can pull this off for Linux, is one of the many things this companion app can do on
[1119.96 --> 1125.22]  the Mac OS is observe the state of the Mac because the Mac has several conditions in use,
[1125.32 --> 1130.26]  idle, screensaver, sleeping, and it could turn those into sensors into home assistant, among
[1130.26 --> 1130.88]  other things.
[1130.92 --> 1135.24]  There's other things that it's monitoring as well as sensor inputs to home assistant to
[1135.24 --> 1137.60]  help automate things around when you're using your computer.
[1137.60 --> 1141.42]  I love this idea and I'd like to apply it to other desktops.
[1142.00 --> 1145.24]  It can detect which mic, which webcam is in use.
[1145.40 --> 1150.44]  When you're on a particular Zoom call or something, you could have a light outside of your office
[1150.44 --> 1154.84]  that turns red that says, I am on the phone, be quiet, stop making noise.
[1155.38 --> 1159.16]  Or, you know, like me, I mean, I'm that guy, but I have like lights and stuff in the background
[1159.16 --> 1160.10]  for my Zoom calls.
[1160.26 --> 1161.46]  You know, I try to make it look presentable.
[1161.54 --> 1163.60]  You could have that stuff turn on when the mic activates.
[1163.94 --> 1164.88]  Is there a word for that?
[1164.88 --> 1167.20]  I feel like it's going to be added to the dictionary soon.
[1167.20 --> 1169.34]  It's like peacocking, but on Zoom.
[1169.60 --> 1170.08]  Do you know what I mean?
[1170.36 --> 1171.28]  Yeah, like Zoom fronting.
[1171.58 --> 1171.98]  Backgrounding.
[1172.22 --> 1173.42]  Yeah, that'd be better.
[1173.48 --> 1174.22]  Zoom backgrounding.
[1174.32 --> 1174.46]  Yeah.
[1174.72 --> 1177.14]  Of course, most people these days just go with the virtual backgrounds.
[1177.34 --> 1178.38]  So that's neat.
[1178.56 --> 1181.74]  It's an official release from the project.
[1182.36 --> 1186.54]  But, you know, just as an aside and maybe ultimately more important for new users, because
[1186.54 --> 1189.16]  I played around with this and it's pretty powerful.
[1189.16 --> 1195.26]  There is a new feature that allows you to add Lovelace cards, which is the dashboard UI
[1195.26 --> 1197.48]  of Home Assistant by entity.
[1197.78 --> 1205.78]  And what that means is you can select a sensor or a camera feed or power switch and Home Assistant
[1205.78 --> 1209.78]  will suss out what the functionality of that is supposed to be and automatically generate
[1209.78 --> 1212.04]  you a dashboard card for it.
[1212.04 --> 1215.80]  And so you don't have to appreciate or understand how these are constructed anymore.
[1216.00 --> 1218.64]  You just look at your entities like myself.
[1218.80 --> 1222.38]  I've never built dashboard entries for my seismic sensors.
[1222.72 --> 1224.24]  I just never got around to it.
[1224.62 --> 1225.96]  I knew the data was getting logged.
[1226.02 --> 1226.82]  I was happy with that.
[1227.38 --> 1229.32]  However, I thought, well, why not?
[1229.58 --> 1231.54]  I never really quite knew how to do that.
[1231.54 --> 1237.16]  So I went in by entity, selected my seismic sensors and Home Assistant just generated me
[1237.16 --> 1239.74]  a brilliant dashboard widget for it, a Lovelace card.
[1240.02 --> 1240.88]  And it's great.
[1241.06 --> 1246.24]  And you can do the same thing with new integrations just to get an idea of what Home Assistant thinks
[1246.24 --> 1247.26]  you might be able to do with them.
[1247.34 --> 1251.80]  I did that with the Ring camera, which has limited functionality if you don't pay for the
[1251.80 --> 1253.90]  service, but it's still useful integrating into Home Assistant.
[1254.10 --> 1255.80]  And I didn't really know what you could do there.
[1255.84 --> 1258.46]  So I just added that entity and let it generate one for me.
[1258.46 --> 1261.56]  Yeah, I think we should talk more about that Ring stuff in the future.
[1262.20 --> 1265.58]  There's a whole world of cloud connected stuff.
[1265.64 --> 1268.42]  It's actually pretty cool that we don't touch on that often.
[1268.90 --> 1269.38]  Yeah, I agree.
[1269.60 --> 1272.42]  Some of that cloud stuff is expensive, like the Ring products themselves.
[1272.88 --> 1277.78]  Not a cheap product long term, but they have a pretty low upfront cost.
[1278.62 --> 1282.12]  And initial indications are they integrate pretty well with Home Assistant.
[1282.38 --> 1287.00]  If you guys are out there experimenting with that, let us know, because I do feel like it's
[1287.00 --> 1288.38]  a blind spot of ours a little bit.
[1289.02 --> 1292.40]  Big congratulations to the Home Assistant for their seventh birthday release.
[1292.78 --> 1295.34]  Huge, huge amount of work must be going into this project.
[1296.02 --> 1301.52]  I'm so glad that it exists because it just makes so many things that you would have had
[1301.52 --> 1303.62]  to buy proprietary stuff for possible.
[1303.88 --> 1304.80]  I'm so thankful.
[1305.02 --> 1306.22]  So thank you, Home Assistant.
[1306.78 --> 1307.76]  Now let's talk about scrutiny.
[1308.28 --> 1313.58]  This is a project that could help bring visibility to something that I often forget to check in on.
[1313.86 --> 1314.80]  You think you're so smart.
[1314.80 --> 1316.40]  Oh, yeah.
[1316.64 --> 1317.82]  Well, at least my hard drives do.
[1317.92 --> 1320.82]  But of course, what does it matter if nobody's ever checking their smart status?
[1321.06 --> 1321.30]  Correct.
[1321.62 --> 1321.80]  Yes.
[1321.84 --> 1326.90]  So one of our community members, Analog J, has released a new tool called Scrutiny.
[1326.90 --> 1332.12]  And this is designed to monitor your hard drive smart metrics.
[1332.84 --> 1334.14]  But here's the really cool part.
[1334.78 --> 1340.50]  It uses the real world failure rates published by Backblaze to tell you whether that is in
[1340.50 --> 1343.94]  line with what other people who have those hard drives are seeing.
[1343.94 --> 1344.54]  Yes.
[1345.06 --> 1351.04]  And it puts it all together in a very easy to read dashboard with a brilliant layout.
[1351.16 --> 1353.16]  So it's super easy to consume the information.
[1353.42 --> 1355.60]  This is a great idea, Alex.
[1355.86 --> 1356.36]  Yeah, it is.
[1356.44 --> 1358.92]  And I nearly lost my freaking mind when I first saw this on Reddit.
[1360.00 --> 1364.18]  Analog J was asking for 25 sponsors before he made this public and open source.
[1364.32 --> 1365.44]  And he got there last week.
[1366.14 --> 1369.44]  And as soon as he went open source, one of the Linux server devs reached out to me and
[1369.44 --> 1372.04]  said, hey, do you think we could release this as a container?
[1372.24 --> 1376.42]  So I put those two people together and I put the PB and the J in the sandwich.
[1376.68 --> 1380.90]  And there's now a Linux server container for Scrutiny.
[1381.42 --> 1384.30]  Oh, so I could put this easy peasy on the Studio NAS.
[1384.54 --> 1387.14]  I need to as well, because those drives are getting a few years old.
[1387.14 --> 1388.52]  Like they're getting in that zone.
[1388.68 --> 1394.54]  So being able to compare that to the mean from Backblaze, well, it's either going to make
[1394.54 --> 1396.94]  me accelerate my plan to replace them or give me some comfort.
[1397.02 --> 1397.48]  I'm not sure.
[1398.16 --> 1399.82]  Now, it's still early days with the project.
[1400.06 --> 1403.24]  You know, there's still a few buttons and knobs and widgets that don't work yet.
[1403.36 --> 1405.26]  And he's adding to it all the time.
[1405.38 --> 1408.76]  But if you find it useful, go open some issues, give him some feedback.
[1408.98 --> 1410.00]  Come find him in the Discord.
[1411.08 --> 1415.74]  Tell him what you want to see, because I think something like this is sorely needed for those
[1415.74 --> 1418.56]  of us that aren't running Unraid or FreeNAS or something like that.
[1419.42 --> 1422.12]  And it just looks like a really great project.
[1422.58 --> 1424.36]  The UI is beautiful.
[1424.54 --> 1427.70]  And the information it provides is really, really useful.
[1428.08 --> 1430.30]  Yeah, and it's using SmartD on the back end.
[1430.44 --> 1433.84]  So it's getting tried and true information from SmartD.
[1435.00 --> 1437.98]  Also, we're going to mention again this week, CloudFree.Shop.
[1438.44 --> 1441.26]  Now, CloudFree.Shop has a wide range of smart home devices.
[1441.42 --> 1445.16]  This is a community members project that are pre-flashed with Tasmoda.
[1445.72 --> 1448.60]  And that means no cloud connection is ever required.
[1448.68 --> 1453.88]  It means you can just plug it in and guarantee that as long as that device operates and runs,
[1453.88 --> 1454.98]  it is under your control.
[1455.10 --> 1456.48]  There is no service that will turn it off.
[1456.90 --> 1457.64]  And check this out.
[1457.92 --> 1458.74]  This is pretty great.
[1459.40 --> 1462.80]  If you use the code self-hosted at checkout, you support the show.
[1463.12 --> 1464.24]  So that's pretty nice.
[1464.42 --> 1466.02]  And do they get anything special when they use that?
[1466.40 --> 1471.44]  Yeah, since last time, we've negotiated that the audience will get a dollar off per plug.
[1471.44 --> 1472.50]  Oh, per plug.
[1472.60 --> 1473.70]  So buy a whole bunch.
[1474.68 --> 1475.42]  Yeah, right?
[1475.68 --> 1476.44]  That's great.
[1476.60 --> 1477.46]  CloudFree.Shop.
[1477.52 --> 1480.46]  It's something that Alex and I had talked about on air.
[1480.52 --> 1485.02]  It's like, why doesn't somebody just sell these devices preloaded with Tasmoda?
[1485.50 --> 1486.46]  Yeah, this is just really cool.
[1486.72 --> 1487.50]  CloudFree.Shop.
[1487.60 --> 1491.02]  Alex and I have talked about it before and wondered, why isn't somebody doing this?
[1491.28 --> 1495.16]  Get these things pre-flashed with Tasmoda and sell it.
[1495.58 --> 1497.30]  And it's a pretty good price too.
[1497.30 --> 1500.42]  All right, time for some feedback, I think.
[1500.76 --> 1507.28]  So Alex C writes in, in the One is None episode, when you were converting from EXT4 to ButterFS,
[1507.48 --> 1512.94]  Chris, I was wondering why you don't use MOSH or something like Tmux or Screen.
[1513.24 --> 1518.52]  The reason I like MOSH is that it covers you if your network connection drops or if you're
[1518.52 --> 1521.06]  roaming between Wi-Fi and mobile internet.
[1522.00 --> 1526.28]  And I think Alex maybe might have MOSH and Tmux slightly confused.
[1526.28 --> 1531.34]  When you read the full email, but it's a good question because a lot of mistakes were made
[1531.34 --> 1533.66]  that night, Alex, a lot of mistakes.
[1533.80 --> 1536.38]  So I generally always do use MOSH.
[1536.66 --> 1541.78]  I don't think of it typically when I'm on the LAN as the same machine that I'm connecting
[1541.78 --> 1545.08]  to, although I really should always just be in practice.
[1545.64 --> 1548.96]  But I think my bigger mistake, honestly, was not using Tmux.
[1549.46 --> 1554.22]  See, Tmux would keep that session persistent, even if I completely disconnected, right?
[1554.22 --> 1560.34]  Where MOSH is going to help smooth out disconnects and interruptions and changing of IP addresses.
[1560.34 --> 1563.14]  So it would have helped, but Tmux would have been the better solution.
[1563.36 --> 1566.02]  But that night, I just wasn't thinking.
[1566.18 --> 1568.46]  I bet you my laptop wasn't even plugged in.
[1568.58 --> 1570.42]  I mean, I was just in a bad state.
[1570.66 --> 1571.48]  It was too late.
[1571.48 --> 1576.68]  I knew I shouldn't be doing it like in the back of my mind, but I pushed forward because
[1576.68 --> 1581.32]  I had ran out of time and I needed to get this done before we left for a trip, if I recall.
[1582.98 --> 1590.14]  And made the mistake of not taking the proper process, not taking the proper steps to make
[1590.14 --> 1595.12]  sure an SSH remote connection is absolutely as rock solid as possible when doing a major
[1595.12 --> 1596.22]  file system operation.
[1596.46 --> 1598.04]  And that's just the fundamental mistake.
[1598.14 --> 1598.82]  I know better.
[1598.82 --> 1599.78]  I knew better.
[1600.40 --> 1602.82]  Thankfully, you know, in the end, I was able to recover everything.
[1603.22 --> 1607.80]  I remember, Alex, how that compounded with an issue where my Google Drive payment had expired
[1607.80 --> 1612.84]  because my credit card got shut down due to fraud at the same time.
[1613.88 --> 1615.30]  Oh my God, that was a nightmare.
[1615.50 --> 1617.50]  It was like the perfect storm of data loss.
[1617.84 --> 1618.96]  It was a nightmare.
[1619.50 --> 1621.08]  So like I have learned from that.
[1621.20 --> 1626.92]  I constantly check in on that stuff now because I'm paranoid that that's going to get shut
[1626.92 --> 1629.68]  down and freaking fraud happened again.
[1629.98 --> 1636.12]  Just about a month ago, my credit card was shut down again somewhere on one of my trips.
[1636.12 --> 1641.40]  I guess somebody had copied it and then waited quite a while in Texas to try to use it.
[1641.44 --> 1642.90]  But they did eventually try to use it.
[1642.90 --> 1646.78]  So the bank cut that off and I had to go through the process all over again.
[1646.86 --> 1649.58]  But this time I made sure that Google Drive was paid for.
[1650.14 --> 1651.04]  Fool me once, right?
[1651.24 --> 1651.48]  Right.
[1651.56 --> 1651.96]  Exactly.
[1651.96 --> 1653.22]  Yeah, Mosh is pretty cool.
[1653.36 --> 1658.02]  I've used it a few times, mostly when I was a consultant traveling around on the trains
[1658.02 --> 1659.10]  and stuff in England a lot.
[1659.20 --> 1659.96]  Perfect for that.
[1660.20 --> 1664.12]  Relying on, you know, 3G, 4G connections all the time.
[1664.78 --> 1669.96]  And the reason Mosh feels so nice to use is because all the keystrokes are local and then
[1669.96 --> 1672.06]  it sort of sends them quietly in the background.
[1672.72 --> 1676.46]  So obviously you might, if you know, you go through a dead patch, you might have to wait
[1676.46 --> 1679.90]  for the screen to update on the result of your command.
[1679.90 --> 1684.30]  But in terms of what you're typing, which is kind of the biggest indicator of latency,
[1685.30 --> 1688.54]  it just feels really responsive and just really nice.
[1689.08 --> 1689.38]  Well, it is.
[1689.44 --> 1690.10]  It's local echo.
[1690.28 --> 1693.90]  So it's locally echoing back to you and then buffering it, which is so clever.
[1694.48 --> 1695.82]  That is really pretty nice.
[1696.52 --> 1699.82]  Since then, I am like so good about it.
[1699.98 --> 1704.46]  I don't know if it'll last forever, but it sort of renewed my best practices when it
[1704.46 --> 1705.20]  comes to this stuff.
[1705.24 --> 1707.56]  I was like, oh, you know, that was my moment.
[1707.64 --> 1708.46]  That was my lesson.
[1708.46 --> 1712.74]  I managed to pull out of it, but I never want that to happen again.
[1713.46 --> 1713.86]  Absolutely.
[1714.40 --> 1714.60]  Yeah.
[1714.80 --> 1720.00]  I mean, the downside of something like Mosh is that you've got to type Mosh instead of
[1720.00 --> 1720.56]  SSH.
[1720.66 --> 1722.94]  And at this point, SSH is muscle memory for me.
[1723.18 --> 1723.30]  Yeah.
[1723.52 --> 1727.72]  I guess I could use a bash alias, but it also requires Mosh to be installed on the remote
[1727.72 --> 1729.68]  system, which isn't always the case.
[1730.04 --> 1730.94]  Not too hard to do.
[1731.10 --> 1733.76]  You know, it's not a whole bunch of stuff, but it is.
[1733.92 --> 1735.06]  You have to have it on both ends.
[1735.12 --> 1735.82]  That is very true.
[1735.82 --> 1739.28]  I think TMUX, if you're not familiar with TMUX, it's worth looking into.
[1739.38 --> 1743.80]  It's a real neat trick to connect into a server, get a set, get a session running, get a whole
[1743.80 --> 1746.84]  bunch of stuff going, and then you can just disconnect and it keeps running.
[1747.16 --> 1750.92]  It's a great way to pair program as well, because if you open two TMUX sessions on two
[1750.92 --> 1754.66]  different systems, they will both update in real time with the same thing.
[1755.06 --> 1755.22]  Yeah.
[1755.22 --> 1756.06]  That's pretty nice.
[1756.06 --> 1759.14]  We actually even just use it just recently.
[1759.28 --> 1763.10]  Wes and I were messing around with recording audio from the command line and we just use
[1763.10 --> 1764.68]  it for working on that kind of stuff.
[1764.92 --> 1765.52]  It's great.
[1766.02 --> 1767.42]  So I know better.
[1767.90 --> 1770.72]  Anyways, it won't happen again, I promise.
[1770.80 --> 1773.04]  But if it does, I will admit it to you guys.
[1773.12 --> 1774.28]  I will come clean on the show.
[1774.68 --> 1774.90]  Yeah.
[1775.04 --> 1775.26]  Yeah.
[1775.44 --> 1775.66]  Sure.
[1775.66 --> 1782.76]  Now in future episodes, we're going to take a look at some container dashboards and maybe
[1782.76 --> 1787.68]  a look at CADDI, which is another alternative to traffic as a reverse proxy.
[1788.12 --> 1792.16]  But in the meantime, I think it's time we thanked our site reliability engineers.
[1792.26 --> 1792.78]  Don't you, Chris?
[1793.28 --> 1793.50]  Yep.
[1793.50 --> 1799.26]  Last episode, we launched the self-hosted site reliability engineers membership, the folks
[1799.26 --> 1802.70]  that help keep this show sustainable, reliable, and fully operational.
[1802.70 --> 1806.72]  I think we still have some early bird SSH codes too.
[1806.82 --> 1809.90]  If you use the promo code SSH, it takes a little bit of money off.
[1809.98 --> 1812.64]  So the membership is even, I think, a dollar cheaper.
[1812.82 --> 1818.18]  And you can go to selfhosted.show slash SRE to get there and just put the promo code SSH
[1818.18 --> 1818.42]  in there.
[1818.48 --> 1820.76]  We've got more show for our members.
[1820.94 --> 1823.64]  We're doing a bonus post show with every single episode.
[1823.64 --> 1826.94]  And we're also doing a limited ad feed for that episode.
[1827.02 --> 1832.46]  So it gives you a whole new RSS feed for the show, a fully produced, limited ad,
[1832.70 --> 1835.46]  with additional bonus content.
[1835.72 --> 1840.06]  And that's a thank you to the site reliability engineers who are keeping the show going.
[1840.28 --> 1842.20]  So big thank you to everybody out there.
[1842.28 --> 1846.54]  And Alex and I are already cooking up new ideas for future membership content as well.
[1846.90 --> 1848.62]  Selfhosted.show slash SRE.
[1848.96 --> 1849.80]  Thanks, everybody.
[1850.08 --> 1851.08]  It's pretty cool, Alex.
[1851.20 --> 1855.88]  You know, it's pretty nice seeing that come in because going independent again is scary,
[1856.02 --> 1857.84]  but also awesome at the same time.
[1857.84 --> 1860.46]  And it's a great representation of audience support too.
[1860.56 --> 1863.52]  But we totally understand not everybody can afford a membership.
[1863.74 --> 1864.66]  That's totally cool.
[1864.72 --> 1866.18]  Just listening to the show.
[1866.24 --> 1869.34]  And if maybe a sponsor seems like the right fit or there's somebody you think you could
[1869.34 --> 1872.48]  share the show with, we really appreciate that support too.
[1873.00 --> 1875.50]  Word of mouth is the best marketing there is.
[1875.68 --> 1878.38]  It's like the only marketing that works for podcasts.
[1878.62 --> 1879.46]  It really is.
[1879.46 --> 1880.06]  Mm-hmm.
[1880.64 --> 1885.06]  Quick follow-up from last episode where, Chris, you talked about having to run home
[1885.06 --> 1887.26]  to pull in your awning because it got too windy.
[1887.60 --> 1889.58]  We had a few recommendations from the audience.
[1890.28 --> 1893.16]  Yeah, a couple of people, and I think you and I thought of this right after we wrapped
[1893.16 --> 1894.48]  up, recommended the Shelly.
[1895.12 --> 1896.86]  That crossed our mind as well.
[1897.32 --> 1902.72]  But Brian Davenport wrote in with a neat idea of essentially a little wind speed gauge
[1902.72 --> 1911.06]  that would transmit on the 433 megahertz band, and it would send the speed to a decoder device.
[1911.06 --> 1915.94]  That decoder device would monitor the speed, and when it reached a certain percentage or
[1915.94 --> 1920.30]  whatever, a certain speed number, it would then trigger a hall sensor switch and close
[1920.30 --> 1921.78]  that, which would then retract it.
[1922.26 --> 1924.94]  The other idea that I had was just check the weather in the morning.
[1926.52 --> 1927.64]  Oh, come on.
[1928.22 --> 1928.74]  I know.
[1928.80 --> 1929.58]  No, it's not good enough.
[1929.58 --> 1934.34]  Well, and you know what's funny, Alex, is today as we're recording, a construction truck
[1934.34 --> 1939.50]  backed up into the pole that has our power transformer and knocked it over, and now we
[1939.50 --> 1943.02]  have no power, which is fine because we've got plenty of battery and solar.
[1943.50 --> 1945.48]  The thing is, is nobody's home.
[1945.92 --> 1950.20]  We may have left the air conditioning set to automatically kick in, and that'll drain the
[1950.20 --> 1951.16]  batteries pretty quick.
[1951.74 --> 1956.40]  And so I got thinking, it's like, you know what I need is I need the system to know when
[1956.40 --> 1957.96]  it's in a limited power state.
[1957.96 --> 1962.50]  And I go back to, I know we have a couple of audience members out there who are pulling
[1962.50 --> 1966.80]  this state information from their Victron devices and feeding it into Home Assistant.
[1967.32 --> 1972.68]  And I remember somebody hooked up a Raspberry Pi to pull in the information and then essentially
[1972.68 --> 1974.36]  MQTT it to Home Assistant.
[1974.56 --> 1975.74]  But I don't recall the details.
[1975.84 --> 1981.02]  But all this started flooding back to me when I think about, is there anything I could do
[1981.02 --> 1983.56]  to tell the system, hey, now you're in battery mode.
[1983.62 --> 1985.80]  Why don't you turn some crap off?
[1986.84 --> 1987.80]  Seems so obvious.
[1987.80 --> 1993.80]  Seems like you need to have your air conditioning on a remote control as a starting point.
[1994.18 --> 1994.62]  Yeah, I do.
[1994.74 --> 1998.58]  And it's tricky because I don't think it's like a household air conditioner, right?
[1998.60 --> 2001.46]  It's a furnace, a fan, and AC.
[2001.84 --> 2003.68]  And I imagine it's all DC wiring.
[2004.64 --> 2007.10]  So I'm not sure what my options are there either.
[2007.30 --> 2010.50]  You know, it's just one of those things I think the step one is take the panel off the
[2010.50 --> 2012.60]  wall and see what the wires are.
[2012.60 --> 2015.62]  You know, when we launched this show, the world was still normal.
[2016.06 --> 2018.20]  And I was planning to come out and see you in April.
[2018.38 --> 2020.06]  We were going to do a whole bunch of these projects.
[2020.42 --> 2020.56]  Yeah.
[2020.86 --> 2021.10]  Yeah.
[2021.18 --> 2023.98]  Oh, I just want to come out and do half of this stuff for you.
[2024.46 --> 2024.92]  I know.
[2025.06 --> 2026.90]  It would be great because we could record it.
[2027.00 --> 2028.68]  You know, I could learn a bunch from you.
[2028.82 --> 2032.18]  You could see how I do some of my crazy setups and the things I'm trying to solve for.
[2032.32 --> 2033.20]  It would be a lot of fun.
[2033.20 --> 2035.62]  We could try and not get pulled over in the mountains.
[2037.42 --> 2039.08]  We definitely could do that.
[2039.20 --> 2040.36]  That would be a lot of fun.
[2040.78 --> 2043.44]  In the meantime, thank you to everyone who sent in some suggestions.
[2043.80 --> 2047.48]  If you have Leet Victron knowledge, I would like to pick your brain.
[2047.60 --> 2049.12]  So maybe that's my next ask.
[2049.50 --> 2051.16]  Because we just have the best community ever.
[2051.76 --> 2053.06]  Selfhosted.show slash contact.
[2053.36 --> 2057.08]  Or if you'd like to jump on the Discord, selfhosted.show slash Discord.
[2057.56 --> 2060.48]  Victron always sounds like it should be like a transformer or something.
[2060.80 --> 2062.24]  It is pretty cool equipment.
[2062.24 --> 2069.36]  And the neat thing is, I kind of made a bet on this and wasn't sure because I'd never used any of their equipment before.
[2069.48 --> 2072.62]  But I got to say, very, very, very satisfied with the purchase.
[2072.94 --> 2076.92]  It's an inverter, charge controller, and converter.
[2077.14 --> 2078.82]  And it is so smooth.
[2079.08 --> 2084.70]  I can switch between multiple different power sources and nothing blips.
[2084.88 --> 2086.34]  All of my gear stays on.
[2086.82 --> 2087.74]  It's great.
[2088.00 --> 2089.20]  It's really clean and smooth.
[2089.30 --> 2090.46]  It produces clean power.
[2090.62 --> 2091.28]  Just very happy.
[2091.28 --> 2096.28]  Well, now that we're at the end of the show, I'll mention my website, chrislast.com.
[2096.70 --> 2097.56]  Alex's website.
[2098.00 --> 2099.50]  Blog.ktz.me.
[2099.80 --> 2101.90]  Well, you can find our sponsor on social media, too.
[2101.98 --> 2105.44]  A Cloud Guru is at twitter.com, youtube.com, and facebook.com.
[2105.48 --> 2107.00]  They're all just slash A Cloud Guru.
[2107.38 --> 2108.12]  Couldn't be easier.
[2108.42 --> 2110.96]  And the podcast here is also on Twitter, self-hosted show.
[2110.96 --> 2115.66]  I'm at Ironic Badger, and that was self-hosted.show slash 28.
[2115.66 --> 2117.40]  Home Operator
