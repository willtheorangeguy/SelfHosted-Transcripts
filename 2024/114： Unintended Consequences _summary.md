• HomePods' integration with Home Assistant has changed in iOS 17
• Siri now toggles all toggleable devices in Home Assistant when invoked
• This can cause chaos, including flipping on heat and alarms unexpectedly
• The hosts are considering building a local voice system to replace the HomePods
• The speaker prefers using Docker Compose with NextCloud
• The OCC (OwnCloud Command) tool is not user-friendly and has a steep learning curve
• Upgrading NextCloud requires frequent use of Docker exec and pinning to specific versions
• The speaker's solution is to upgrade every 4-6 months, but this can be time-consuming
• NixCloud is mentioned as an alternative for simpler updates, but it has its own challenges with database schemas
• The speaker suggests setting a reminder in 30 days after a new release is announced to perform the update.
• The speaker is disappointed that there was no new iPad released last year and has been waiting patiently.
• They use their iPad as an auto cue for cameras, but don't use it much for media consumption.
• With the loss of Plex's offline download feature, they're struggling to find a suitable alternative with Jellyfin.
• The speaker wants to be able to download media at different qualities on their iPad, but Jellyfin only offers full quality downloads.
• They prefer having multiple options for content on their iPad for plane rides and other situations where they don't know what mood they'll be in.
• The speaker suggests using a small library with pre-encoded media or setting up an Android device as an alternative to the iPad.
• They are frustrated that iPads do not support microSD cards, which would solve some of their problems.
• Discussion of using a Samsung tablet as an alternative to an iPad for media consumption and travel
• Features of the Samsung S9 tablet, including its display size, aspect ratio, AMOLED screen, Wi-Fi 6E, and lower price point compared to the iPad Pro
• Emulation games and sideloading apps on the tablet
• Interface and user experience of the Samsung tablet, described as having a "Samsung flavor" but not being overly customized
• Discussion of Android version, with the tablet running Android 14
• User's overall satisfaction with the tablet after using it for a week, including its performance and battery life
• Discussion about the Samsung tablet and its Android app
• Comparison between Samsung DeX and Apple iPad software
• Features and benefits of using the Samsung tablet as a desktop computer
• Battery life and heat issues with the Samsung tablet
• Price comparison between different models and versions of the Samsung tablet
• Personal media management and usage, including Plex and Jellyfin
• Introduction to Jellystat, a project for Jellyfin statistics
• Lifetime subscriptions to Plex and leaving due to concerns over data control
• Moving to Jellyfin for media streaming and setting up a server with Jellystat
• Concerns over data breaches, security, and the use of cloud authentication by Plex
• Hardware requirements for transcoding media and using QuickSync
• Open SSH 9.5 release and defaulting to ED25519 keys for improved security
• Tailscale as a networking solution for direct device connections and secure communication
• Service containers and programmable networking with Tailscale
• The speaker talks about a product called Audiobookshelf and its benefits.
• They discuss their personal experience with setting up Audiobookshelf on their home infrastructure, including using Docker containers and Tailscale services.
• The speaker's wife uses the Android app to access their audiobooks and is impressed by how easily it works.
• The discussion turns to DNS settings, specifically the use of "magic DNS" to make it easy for devices on the Tailnet to resolve names like "books".
• The speaker explains that they have a custom DNS server running in the Tailnet with hostnames set up for their audiobooks.
• Tailscale's local search domain is discussed
• Magic DNS entry needed for external access to Tailnet
• Go Slash Links internal project used for sharing resources
• Container applications communicating directly over Tailnet without reverse proxy
• Unified network across multiple locations and devices
• Access to shared resources from anywhere using a single network
• Integration with Let's Encrypt for SSL certificates
• Discussing the convenience of audiobooks for a partner
• Using PDF tools (PDF editor or Adobe Acrobat) for contract signing
• Introducing Sterling PDF as an alternative to Adobe Acrobat
• Features and capabilities of Sterling PDF, including watermarking, metadata editing, OCR, and cleanup
• Installing Sterling PDF on a server and accessing it via web app
• Mentioning Lube Log (Vehicle Service Record and Maintenance Tracker) as a separate application for logging car maintenance
• Discussing the potential usefulness of Lube Log for tracking car maintenance records
• The host recommends supporting the show through membership or boosting individual productions
• Podverse is mentioned as an open-source podcasting app with cross-platform availability
• Castomatic and other Podcasting 2.0 apps are discussed for their features, including live streaming
• Boosting options are explained, with a split system that benefits multiple parties
• Obsidian is again mentioned as the host's preferred note-taking tool
• A new note-taking app called Memos is introduced as a privacy-first alternative to Apple Notes
• The speaker discusses a web app called Memos
• The app is open source and self-hosted with a simple setup process
• It works well on both mobile devices and web browsers
• The speaker thinks Memos would be great for someone who wants a simple feed of notes, but may not be ideal for heavy users or those who need advanced features
• The app has limitations when it comes to handling pictures and extracting text from them
• The speaker's wife is transitioning from using Apple Notes on her iPhone to Graphene OS and Memos will likely meet her needs
• The app has a clean UI, supports sharing notes with others, and allows for public or private note linking
• Discussion about Matter integration on Home Assistant
• Recommendation for Obsidian Live Sync as a conflict-free alternative to NextCloud Sync
• Successful setup of Mitsubishi mini split using ESP01 with ESP Home in Home Assistant
• Use of Broadlink RM4 infrared controller to control the mini split and its integration with Home Assistant
• Docker Compose setup and self-hosting on home server
• Reverse proxies allow users to access services without typing IP addresses and port numbers
• They can simplify infrastructure by routing requests to the correct internal server
• Reverse proxies often include built-in TLS certificate automation, making it easier to obtain certificates from Let's Encrypt
• Certificates verify ownership of a domain and ensure encrypted connections between client and server
• Mobile apps increasingly require SSL/TLS for functionality, making reverse proxy solutions more necessary for home labs
• Discussion of the Zengeld device's effectiveness in improving mesh network performance
• Personal anecdote about deploying a dozen Zengeld devices with variable success rates
• Commentary on productivity gurus and their unrealistic expectations for cable management and workspaces
• Host's experience with a cluttered workspace and the need to unplug and replug devices
• Discussion of automation processes and how they can be prone to errors or crashes
• Thanks to listeners who contributed boosts to the podcast during this episode
• Upcoming conferences: NixCon, Scale, Texas Linux Fest (also referred to as Barbecue Fest)
• Concerns about travel time between Texas and the Seattle area for Linux Fest Northwest
• Joking reference to flying or transportation that can cover long distances quickly
• Promotion of Chris's podcast and social media presence, including a link tree