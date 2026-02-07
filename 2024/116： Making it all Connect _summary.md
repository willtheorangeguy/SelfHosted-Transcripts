• The host is excited about the upcoming episodes of The Grand Tour
• The host discusses their long history of watching Jeremy Clarkson, James May, and Richard Hammond's shows
• Ben Collins, the original White Stig, has launched a YouTube channel called Ben Collins Drives
• Upcoming events: Southern California Linux Expo (SCALE) on March 14th, NixCon, and DevOps Days Austin in May
• The host will be working at the Tailscale booth at SCALE and attending NixCon
• The host mentions the upcoming LinuxFest Northwest event and being unable to attend due to scheduling conflicts.
• They discuss their current setup using Tail Scale, which allows container services to be individually addressable on a network called "Tail Net".
• The host created a 4,000-word blog post and a 32-minute YouTube video explaining how to use auth keys and OAuth clients with Tail Scale.
• They explain the benefits of using Tail Scale, including portability and simplicity, allowing containers and data to be moved between hosts without changing network addressing.
• The host also discusses container networking, specifically linking two containers together, and explains how they've done this in the past using VPN applications.
• Containers create isolated resources within the Linux kernel through namespaces
• Namespaces are isolated environments that require explicit connection between them
• Docker Compose's network mode parameter merges two namespaces together
• This merging allows for shared networking and processes between containers
• The default behavior is to have individual sidecar containers per service, but workarounds like reverse proxies can be used
• Using a single TailNet service container with multiple containers linked to it is possible, but not currently supported by the software
• The host mentions a secret was accidentally committed to their system and it's now at 99.8% leaked credentials.
• The host promotes Tailscale, a mesh VPN service that connects devices and services together, and offers a free trial with 100 devices.
• The host explains how Tailscale can be used for sharing devices and services with others, including using ACLs to set up policies.
• The host mentions the benefits of Tailscale's zero-config setup and its ability to connect devices across different providers and locations.
• The host discusses the recent Home Assistant release, which had limited updates but included better drag and drop support for automations and managed updates.
• Zigbee devices in Home Assistant
• Update availability for Zigbee devices
• Limited vendor participation
• CarPlay support added to the app
• Revamping home automation system with location-independent triggers and NFC tags discussed as potential solution, but ultimately rejected due to reliability issues
• Alternative solutions for sending automated messages and tracking locations considered, including integration with HomeKit and Shortcuts
• TP-Link users will see improvements in their integration
• New Python version (3.12) included in the update, requiring backups before installation
• The speaker is frustrated with the time-consuming process of updating and maintaining their Home Assistant system.
• They suggest that project creators could add a flag to alert users of significant changes or breaking updates.
• The speaker discusses potential hardware upgrades, including using an Odroid or dedicated Raspberry Pi for greater performance.
• They mention concerns about the size of their backups (over 400-600 megs) and storage limitations on the current system.
• The conversation turns to the Raspberry Pi ecosystem, with the speaker stating they're not impressed by recent developments, particularly the delayed release of the Raspberry Pi 5.
• The speaker attributes this delay to supply chain issues and prioritization of business customers over educational and consumer orders.
• They speculate that the Raspberry Pi Foundation "slept on their lead" after releasing the Raspberry Pi 4.
• The market for single-board computers has changed due to the pandemic and shift in office work
• Raspberry Pi prices have decreased with many options available under $100
• Intel's N100 CPU is comparable to Raspberry Pi 5, with improved performance and features like quick sync and NVMe support
• Home Assistant Assist desktop app allows typing-based communication and fine-tuning of natural language controls
• SSD prices are increasing after a period of price decreases
• Discussion of an app for training wheels on voice assistants
• App available on GitHub with instructions for getting started
• Opportunity to participate in the development process and make an impact
• Trustybook.com self-hosted workbook for digital legacy planning
• Tool helps create a comprehensive plan for managing digital estate, including passwords and social media accounts
• Trusteebook is secure, private, and can be downloaded and used offline
• Discussion of Plex's movie rental service launch
• Criticism of Plex's new rental feature for not being intrusive enough
• Comparison to Amazon Prime and Netflix ad-supported tiers
• Discussion of user expectation vs. reality when accessing content on streaming platforms
• Critique of Plex's handling of piracy within the platform
• Suggestion for an ad-supported version of Plex
• Reflection on why a music streaming service like Spotify or Tidal doesn't exist in the video market
• Analysis of the movie industry's influence on the streaming landscape
• Discussion about Plex and its struggles with licensing and mobile app support
• Comparison to iTunes and services that killed Napster's adoption at scale
• Potential for a service like Jellyfin to fill the gap and offer an all-in-one solution
• Mention of licensing issues and the need for more titles to be added to the platform
• Reflection on Plex being in development since 2020 and potential for setbacks and closures
• Comment on not seeing this type of service as appealing, but potentially useful for family members
• Discussion about wanting Plex to remain around despite these issues
• The conversation starts with discussing running and exercise
• The topic shifts to self-hosting and home servers, mentioning the Ansible NAS project as a compromise between no-code solutions and starting from scratch
• Nix modules are discussed as a way to customize and extend the base Nix system
• The hosts mention their experiences with different systems, including Ansible and NixOS
• The conversation includes a discussion about Tail Scale and its features
• The hosts talk about their own self-hosting setup and use of WireGuard for network security
• Discussion of the podcast's focus on self-hosting and running applications
• Tail scale vs Wire Guard, including setup time and integration levels
• The host's personal experience and enthusiasm for tail scale
• Concern about appearing as a "shill" due to sponsorship
• Comparison of tail scale and wire guard features and benefits
• Listeners share their updates on projects and machines running in their homes
• A listener reports using audio bookshelf since a previous episode and listening to over 697 minutes of audiobooks
• Host receives an orange hard drive as a gift from Alex, which is still being used for backups
• Host sends a laptop hard drive to a listener who participated in a giveaway
• Listeners share their experiences with Proxmox on Frankenstein computers and ask for updates on home lab case reviews
• Discussing DNS setup for Tail Net and LAN
• Critique of current DNS solutions being too complex
• Appreciation for Prusa printers and their upgrade kits
• Mention of upcoming 3D printing episode with guest Gina from Octoprint
• Discussion of music helping focus and productivity
• Brief mention of boosting donations on the Jupiter Party website
• Track day experience and personal best lap times
• Use of music for concentration and focus
• Listener feedback and boosters, including rotted mood's setup with Obsidian
• Discussion on Linux issues and community responses
• Podcast value and transparency
• Boosting the podcast to share resources or ideas
• Discussing subscription options for Jupiter dot party
• Announcing a new show called "The Launch" which combines tech news and music
• Providing details on how to access the new show, including website URLs
• Mentioning previous episodes and encouraging listeners to try different ones
• Talking about social media presence and mentioning various platforms
• Difficulty with using Noster
• Link to the user's content at chrislass.com
• Suggested alternative platform: self-hosted.show/116