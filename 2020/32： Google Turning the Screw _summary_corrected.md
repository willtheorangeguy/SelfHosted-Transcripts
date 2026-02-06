• Self-hosted Google Photos replacement
• Self-hosting email services
• Discussion of Nintendo Switch options (Switch vs. Switch Lite)
• Hardware vulnerability in older Nintendo Switch models
• Difficulty finding new Nintendo Switch consoles in stock
• Introduction to upcoming self-hosting topics: photos and audiobooks
• Using Open Audible or Inaudible tools to download and remove DRM from Audible audiobooks
• Alternatives to Audible for purchasing audiobooks, such as directly from authors
• Requirements for an ideal audiobook player: resume position, chapters, sleep timer, mobile-friendly offline caching
• Book Sonic software for hosting and playing self-hosted audiobooks with features like last playback position and chapter support
• Integrating Book Sonic into Plex media server for a low-hanging but imperfect solution
• Plex's method of marking chapters as played in audiobooks
• Importance of chapter marks and potential for issues
• Mobile audiobook players: Book Player on iOS and its features
• Prologue, an alternative to Book Player that plugs into Plex
• Linux desktop options, including Cozy
• Audiobook player features and settings
• Multiple storage location support and offline mode
• Future convergence of devices for audiobooks and mobile apps
• Linode.com cloud hosting provider promotion
• Virtual servers, object storage, and S3-compatible services
• Benefits and advantages of using Linde over other cloud providers
• Jeff writes to discuss his Ubuntu machine serving as both home server and HTPC, using Nextcloud Snap
• He struggles with understanding database setup and connecting containers for a containerized Nextcloud setup
• The host discusses SQLite and MySQL database options for Nextcloud and potential simplicity vs performance trade-offs
• Snaps' ease of use but also potential issues, such as baked-in data and lack of control, are discussed
• Docker is mentioned as an alternative with more flexibility
• Docker as an industry standard
• Data separation in Docker
• Nextcloud Docker image and documentation
• Comparison between Docker and Snap
• Volume management in Docker Compose
• Migrating from Snap to a proper database
• Options for migrating data, including manual migration or using Cal client
• Next Cloud CLI client used for moving servers
• Using a Linde instance for faster performance and redundancy
• Security considerations: exposing the system outside of firewall, potential for port scanning and attacks
• Recommendations for securing the Linde instance and using its built-in firewall features
• Benefits of having an off-site backup system with Next Cloud on Linde
• Data security advantages of employing off-site backups to a cloud service
• Difficulty of self-hosting an email server
• Hybrid approach to self-hosting emails using a service like Mail Route or Amazon SES
• Unix mindset in building email systems
• Advantages of having a receiving email server while farming out sending portion to a relay service like Mail gun or Amazon SES
• Criticism of Google's data mining practices through Gmail
• Value of email receipts and purchase history to advertisers
• Discussion of a computer built for someone four years ago through Gmail
• Hybrid email approach and self-hosting considerations
• Intermediary services like Mail Routes and Posting (now owned by Google) for sending and receiving email
• Responsibility of hosting email and the potential consequences of downtime
• Email as a "box of expectations" and its impact on relationships and communication
• Discussion of a listener's use of Home Assistant
• Discussion about MQTT and its use with Home Assistant
• Chris mentions using TASTE devices and MQTT for home automation
• Explanation of how MQTT allows devices to publish messages to specific topics
• Description of how other clients, including Home Assistant, can subscribe to those topics and react to incoming messages
• Comparison between traditional infrared remote model and MQTT's contextual messaging approach
• IoT devices requiring two-way contextual awareness
• MQTT as a lightweight and efficient messaging protocol for IoT applications
• Subscription model allowing devices to only receive necessary messages and saving battery life
• Example of car communicating with house to open garage door and start coffee maker
• Unified API via broker for multiple devices and systems
• Battery-saving benefits of using MQTT, such as not needing constant polling
• Home Assistant integration with MQTT and its advantages
• Self-hosting DNS on LAN for performance reasons
• Local DNS lookups are faster than ISP or public DNS servers
• Caching of records improves performance
• Integrating with DHCP for dynamic updates and machine name resolution
• Various methods for handling DNS, including built-in solutions and custom setups
• Example of using multiple DNS services in conjunction with each other (e.g. Open Sense, AdGuard Home)
• Considerations for running Kubernetes and OpenShift clusters on a LAN
• The host is currently using Spyhole for GHCP server and dynamic DNS
• Mention of previous episodes on the same topic
• Sponsorship by Datadog, a unified monitoring platform for Docker performance
• Features and benefits of using Datadog, including real-time observability and insights
• Call to action to try Datadog's 14-day free trial
• Discussion about Google Photos and Google's tendency to "turn the screw" on users
• Google is discontinuing unlimited storage in Google Photos
• Users will have to pay after hitting the 15 GB storage cap
• Unlimited storage was initially available for free with purchase of Pixel phone or 2 TB of Google Drive storage
• High-quality photos and videos uploaded through Google Photos are now counted against storage limits, but significantly compressed
• The change takes effect June 1st, 2021
• Discussion about Google Photos and its limitations
• Desire for an exit strategy from Google Photos
• Introducing Photo Prism as a promising alternative with object recognition and search capabilities
• Review of Photo Prism's usability and performance, including machine learning and TensorFlow integration
• Explanation of how Photo Prism works in conjunction with Docker Compose
• Docker Compose placement requirements for Photoprism
• CPU-intensive image importing with Photoprism
• Resource requirements for running Photoprism effectively
• Comparison to Google Photos' pricing and functionality
• Appeal of self-managed photo libraries using Photoprism
• Google Photos killed a small team of developers who created a commercial photo organization service
• Google Photos offered similar services for free, making the other company uncompetitive
• Google Photos has since introduced paid storage options despite initially offering unlimited free storage
• The speaker likens this to the Walmart effect, where competitors are driven out by cheaper alternatives
• PhotoPrism is mentioned as an alternative to Google Photos that offers a free and open solution
• The speaker hopes for continued improvement of PhotoPrism and considers contributing to the project.
• Importance of capturing and valuing important moments in life through photography
• Using Ecotourism for photo organization and backup, including auto-backup from phone to file server
• Potential future blog post or segment on combining Ecotourism with other open-source software for a comprehensive photo workflow
• Discussion of the author's experiences with Docker and its packaging issues on Linux distributions
• Mention of considering switching to Rodman due to Docker's semantic versioning changes
• Speaker is frustrated with issues on Ubuntu and Fedora
• Considered using distribution packages, but decided not to
• Was introduced to Arch Linux by the conversation partner
• Conversation partner has a mixed-distribution setup (Ubuntu, Arch, Fedora)
• They discuss their approach to not being tied to any specific platform or OS
• The sponsor of the podcast is mentioned: Cloud Guru's Python 3 scripting course for system administrators
• Other members and supporters of the show are also mentioned
• Discussing a podcast
• Mention of self-hosted component for the podcast
• Way to contact the podcast hosts (self-hosted.show.contact)
• Social media presence of the hosts (Twitter: ironic badger, Chris LAS, self-hosted show)