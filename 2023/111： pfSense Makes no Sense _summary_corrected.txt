• Welcome and introduction to guest Wolfgang from YouTube's Wolfgang's Channel
• Guest shares their Black Friday deals, including a Fleshpot sit-stand desk and SSDs for a RAID Z1 array
• Discussion of issues with SSD cache exhaustion on a 10 gig network setup
• Comparison of ZFS caching versus RAM cache in workflow performance
• Ideas for upgrading the storage system to improve performance and reduce power consumption
• Discussion of a gateway drug video for hardware enthusiasts
• Host's home server setup and current configuration
• Energy draw and power consumption of the setup (14 watts at idle)
• Use of a BLY KVM with Raspberry Pi Compute Module 4
• Comparison between Intel X710 DA2 networking card and Eleanor cards
• ROI calculation for networking card upgrades
• Discussion of low-power options for media encoding
• Review of an Intel Arc GPU for a media server and its power consumption
• Experimentation with Jellyfin and hardware encoding using the Intel Arc GPU
• Software setup used to measure power consumption instead of a hardware meter
• Mistake made in measuring core power consumption as whole package power consumption
• Comparison made with older Intel GPUs, specifically Kaby Lake and Coffee Lake
• 12th gen Intel GPU has more powerful graphics than Intel Arc
• Discussion on Intel's ticktock model and minor upgrades between generations
• Hardware transcoding performance in Jellyfin tested and compared to other GPUs
• Software support for Intel Arc, including Linux driver issues at launch
• Use of FFmpeg under the hood in Plex and a potential reason for lack of support for certain GPUs
• Setting up Tale scale for a flat mesh network
• Zero-configuration VPN built on WireGuard
• Simplifying networking and reducing connectivity issues
• Tale scale's features and benefits for self-hosting and ad hoc networking
• Gateway drug into self-hosting (Plex)
• Discussion of geo-restricted content and piracy
• The speaker discusses the dilution of Netflix's content pool and their shift to streaming Formula One on the F1 TV app.
• They mention how this could lead to increased storage sprawl, requiring self-hosting solutions.
• The speaker shares his own media server setup, with 65 terabytes of storage, consisting of three 16-terabyte hard drives and four 2-terabyte SSDs.
• They are asked about keeping raw footage for their YouTube channel and admit to storing it all, including Proves files, which takes up more space.
• The speaker is then hypothetically given a $1,000 budget for hardware and must choose between Intel or AMD processors for building a media server.
• Intel's ECC support policy and how it has changed over time
• Comparison of different motherboard manufacturers (AS Rock, ASUS, MSI)
• Discussion of BMC (Baseboard Management Controller) and its impact on system functionality
• PCIe bifurcation and M.2 slot configuration options
• Negate situation and the confusion surrounding the story
• Negate is the commercial entity behind pfSense, a firewall distribution built on FreeBSD.
• pfSense has different tiers of licensing, including free Community Edition (CE) and paid Plus option.
• The CE license was previously available for free, but was later revoked without proper communication from Negate.
• Users were left with only one option to pay $399 per year for TAC support contract.
• After backlash, Negate introduced a new TAC Lite subscription for individuals at a lower cost of $129 per year.
• The licensing restructuring may be aimed at curbing the practice of users installing pfSense on third-party hardware and selling it online.
• Supply chain attacks and their implications
• Negate's actions and motivations
• History of Negate's conflicts with the pfSense community, including:
	+ The "Open Sense" website controversy in 2017
	+ Allegations of code theft and slander
	+ WIPO arbitration case
• Comparison to Red Hat's statements on open-source licensing and code reuse
• Similar themes of code theft and free-riding in other companies (e.g. Brusa, HashiCorp)
• Negate's attempt to sponsor WireGuard implementation in the BSD kernel and subsequent issues
• Negate and pfSense controversy due to allegedly rushing code that wasn't properly audited
• Scott Long's blog posts about pfSense Plus and dev insights were found to be "economical with the truth"
• AES-NI flip-flop incident where Negate initially required CPUs to have it, then later reversed course
• WireGuard situation with FreeBSD, where Negate's implementation was insecure, and they refused to acknowledge the mistake
• Patterns of behaviour in Negate's actions that raise trust issues, including prioritizing profits over open-source principles
• Transition to Linde as a hosting provider, now part of Akamai
• The speaker is sure they saw an email from Plex showing their friends' viewing history on their Plex servers.
• Plex's decision to send emails with users' viewing history has been met with criticism and embarrassment for some users.
• The speaker shares a screenshot of the email and jokes about not doing anything embarrassing, but notes that others may have been affected by this feature.
• The speaker criticizes Plex for collecting and sharing data on what users are watching, including file names and titles.
• A recent hack of Plex's database has raised concerns about how user data is being handled, and the speaker notes that they were able to find information about the breach from a former employee.
• The speaker mentions their switch to Jellyfin as an alternative to Plex for media management.
• Users can opt out of some data collection by modifying settings in Plex's privacy settings.
• Plex app sharing feature and its impact on user base
• Sharing information with friends and family without consent
• UX patterns, specifically the use of pop-up notifications and wizards
• Importance of prioritizing user privacy in implementing new features
• Alternative approaches to introducing social features and minimizing opt-outs
• Miscommunication around data sharing and title storage
• Impact of poor design on user experience and retention
• Concern over data privacy due to metadata collection
• Google Photos moment mentioned as similar issue from a year ago
• Importance of understanding the risks of passive use
• Intro skipping feature discussed in Plex Review
• New product announcement: 45homelab.com premium storage servers for Home Lab
• ESP Corner segment on projects with ESP8266 and new 3D printer
• Using servo motors from remote control cars to open blast gates
• Discussion of ESP devices, including the ESP32 S3 box and its features
• Home Assistant voice assistant setup recommendations
• WESP32 wired ESP32 device with POE capabilities
• IoT security and network configuration best practices, including setting up a guest network for IoT devices
• The Chromecast's MDNS functionality and its impact on network traffic
• Handling MDNS traffic to traverse Plans and solve connectivity issues
• Bonjour protocol is essentially the same as MDNS, which Apple renamed
• Listener boosts and show notes discussion about hard drives and burn-in testing
• Host discussing their own burn-in routine for new hard drives, using bad block scans
• Discussion of hard drive age and reliability
• Expert opinion on keeping drives under 5 years old for optimal performance
• Introduction to Git Annex as a tool for deduplication and data management
• Explanation of the difference between Git and GitHub
• Mention of using Git with non-traditional use cases
• User's goal to move Nix config to Git next year
• Discussion of Nix OS and its potential applications
• Introduction to Jovian Nix OS, a pre-configured OS for deck hardware
• Discussion about Plex's future and potential abandonment of its media server
• Strengths and weaknesses of Plex as a streaming service
• Prediction that Plex will default to its streaming service and phase out home servers
• Appreciation for listeners, boosters, and sponsors
• Announcement of a Black Friday sale on self-hosted services
• Guest Wolfgang joins the discussion and promotes his YouTube channel