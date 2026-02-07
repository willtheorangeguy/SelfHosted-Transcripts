• End of summer feeling
• Frustration with uncompleted DIY projects, specifically ESP-based ones
• Difficulty finding compatible parts for projects
• Solution: using an ESP clicker device to automate physical devices without hacking their protocols
• Using the ESP clicker with a Flux blind remote control
• Describing the process of soldering and integrating the ESP clicker with other devices
• The host discusses their experience with Home Assistant and automating their blinds.
• They mention a project they found on YouTube that creates a prebuilt ESP board for home automation.
• The host expresses interest in using this type of setup to control other devices, such as a fan or water pumps.
• They discuss the idea of creating a button pad for home automation using an ESP Home device.
• The host shares their experience with Zigbee buttons and their limitations, expressing disappointment with their performance.
• Home Assistant and automation setup challenges
• Switch Manager plugin for Home Assistant
• Difficulty executing custom actions with Switch Manager
• Home Assistant's limitations with battery-powered devices
• Need for a non-invasive, wall-mountable button pad with smart features
• Crowdsourcing episode about home automation systems
• Linde hosting infrastructure and partnership with Akamai
• Matter app's podcast transcription support addition
• Transcribing podcast shows using open source whisper tooling
• Dimerization and automatically identifying speakers in podcasts
• Merger FS is a low-key awesome bit of Linux technology for managing hard drives in media servers
• Merger FS allows users to point multiple drives at each other and create a single, unified mount point
• The technology has been around since 2019 but has undergone significant changes under the hood
• Cleanup efforts have reduced memory footprint and mitigated fragmentation issues on smaller RAM systems
• Threading pools have been added to improve performance in certain scenarios
• A new feature called read Dur is being released, which concurrently connects to network file systems or spinning disks to reduce latency
• Discussing ZFS metadata on NVMe drives
• Introducing Mergers and its union file system approach
• Explaining how Mergers aggregates data from multiple sources for faster lookup times
• Describing typical Mergers deployment sizes and challenges with telemetry
• Addressing caching in Mergers, including kernel-level caching, fuse-related features, and tiered caching for underlying devices
• Discussing policy-based behaviour in Mergers and creating secondary pools for prioritized storage
• Implementing Mergers with multiple mount points for different tiers of storage
• Using SSDs as a cache layer for slower devices, such as hard drives or cloud storage
• Combining Mergers with R clone and using it to cache data from cloud storage
• Utilizing device mapper in Linux to create block caches on existing devices
• Releasing a tool to automate caching at the block level without requiring ZFS or Brake
• Future plans for completely redoing the configuration system and moving to TOML
• Adding built-in tiering knowledge to Mergers, including performance characteristics of different drives
• Adding features like Unpaid and Dry pool's mover scripts for file organization
• Implementing rebalancing functionality in Mergers
• Concerns about "Stockholm syndrome" in users preferring certain products to others
• Options for supporting the project, including GitHub sponsors and Patreon
• Promotion of Tail scale for self-hosted networking and VPN needs
• Discussion of a local version of Whisper for Mac called Mac Whisper and its benefits
• Concerns about data privacy with online AI tools like OpenAI's website
• Review of the UI and performance of a local chat GPT-like bot
• Comparison of performance on an M1 Mac MacBook vs. a Raspberry Pi 4
• Discussion of a script to benchmark quick sync encoding engines for video content creation
• Introduction to a project to find the "sweet spot" in price-to-performance ratio for Quick Sync
• Plans to involve listeners and gather results on Discord
• Discussion of running large applications with Intel Arc GPUs
• Wimpy's solution of using multiple GPUs and headless Nvidia card for CUBA driver access
• Challenges of setting up and configuring hardware for self-hosting
• Advertisement for 45drives.com and their enterprise-grade storage solutions
• 45homelab.com project aimed at creating home lab-specific products
• Response to listener Leone's email about rebuilding his home lab after a fire
• Discussion of using Tail scale and WireGuard for remote device connectivity
• Recommended self-hosted setup with Nextcloud, Pinhole, Sambar, DRIVE, Plex/Jellyfin, and Proxmox.
• Discussion of virtualization options for Ubuntu servers, including Proxmox and Docker
• Assessment of running Proxmox on an i4 with 4GB RAM, potential limitations and workarounds
• Considerations for running Perfect Media Server setup as a VM or directly on the host
• Transitioning from iOS to Linux, specifically Graphene OS on a Pixel device
• Comparison of note-taking apps, including Apple Notes and Quilled, with Obsidian source also mentioned
• Use of Nextcloud for syncing notes and data between devices
• Host's oil change and mileage tracking
• Linux Unplugged show notes, Chris's journey ditching Google
• Boosts: spam-proof at few.St using Pod verse, GNU Cash personal finance management recommendation
• Home Assistant setup advice for newcomers:
	+ Start small, don't try to do everything at once
	+ Begin with a room or simple project
	+ Consider running Home Assistant core in a container versus the whole Haas operating system supervisor setup
• Pros and cons of using Node-RED and VM appliances in Home Assistant
• Discussing smart home devices and protocols (Z-Wave, Zigbee)
• Recommendation for backing up data before upgrading
• Communication protocols and their differences (Zigbee is open standard, Z-Wave is proprietary)
• Choosing between Wi-Fi and Z-Wave/Zigbee for devices
• Importance of buying energy monitoring-enabled smart plugs
• Discussion on domain ownership and the concept of a "domain lush"
• Tail scale question about SSH-only connections over a tail net
• Solution using corkscrew to bypass firewalls
• Example of using port 443 for encrypted SSH traffic
• Discussion of VT52 and Faraday Fedora using "pork bun" as a DNS registrar
• Portland Oregon-based companies and their quirks (damp checks, potential vandalism)
• Seattle vs Portland rivalry
• Troubleshooting self-hosting with Bitcoin and Lightning, including Umbral node issues
• Introduction to Docker containers and troubleshooting
• Tips for learning Docker and Docker Compose
• Successful crowdfunding efforts for perfectmediaserver.com
• GeneBean19998's VoIP integration with a traditional rotary phone and Home Assistant
• Discussion of past cars
• Home Cam for HomeKit and its dashboard feature
• Boosts for the show, including a total of 19 boosters who contributed 230,909 SATs
• Promotion of various podcast apps
• Upcoming meetups and events, including Linux Fest Northwest
• Live recording idea for October 20th