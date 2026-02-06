• Discussion of excessive Raspberry Pi collection
• Performance improvements with USB SSD booting on Raspberry Pi 4
• Requirements for SD card in current setup
• Options for network booting and Pixie boot workarounds
• Migration process from SD card to SSD
• Potential kernel syncing issues and precautions
• Review of performance benefits and deployment considerations
• Drama surrounding Home Assistant's deprecation of supervised mode on generic Linux
• Discussion of Home Assistant's Supervised DE and its capabilities
• Announcement by Home Assistant of plans to deprecate the ability to install the entire package on any Linux box, but later revising those plans
• Concerns about burnout and its impact on developers' health in open source projects
• Debate over entitlement vs. prioritizing developers' well-being
• Mismatch between user expectations and developer priorities
• Security concerns regarding custom-built OS vs. standardized operating systems
• Discussion of the trade-offs between security, customization, and maintenance in home automation setups
• Home Assistant's deprecated supervisor setup and the resulting feeling of being locked in
• Importance of clear communication and documentation for open-source projects like Home Assistant
• Potential motivations behind Home Assistant's changes, including pivoting towards a new user base and abstracting away complexity
• Historical context of Home Assistant's adoption and potential implications for its future direction
• Concerns about the project's sustainability and developer burnout
• The host of the show is concerned about potential issues with Home Assistant
• The host mentions a "red flag" but notes that the developer has dialed back some changes, indicating they are listening to feedback
• The community around Home Assistant is important for its integrations and development
• The host praises Home Assistant and its longevity compared to competitors
• The show's host mentions using Nginx instead of Caddy or other alternatives
• A user in the Discord helped the host resolve an issue with Traffic
• The host discusses a new project called HomeLab OS, which promises easy deployment and management of personal data centers
• The host notes that HomeLab OS uses Terraform under the hood and creates a Bastion server for secure remote access
• The project is complex and abstracted, making it difficult to understand what's happening under the hood.
• It uses Ginger templating for Docker Compose YAML files and supports hundreds of applications.
• The speaker had trouble understanding how it worked despite months of experience with Ansible code bases.
• The project's complexity may make it more suitable as an example or demonstration rather than a practical tool.
• It showcases automation, infrastructure as code, and best practices, making it useful for learning and development purposes.
• The developer is open to feedback and willing to improve the project.
• HomeLab OS discussed as a project with potential if made more generic and reusable
• Criticism that current version has strong opinions and limited use cases
• Mention of installing Ubuntu 2004 on an old server and experiencing issues with DKMS modules
• Decision to wipe and install new OS instead of trying to upgrade from Debian 9
• Discussion of using PFSense as a firewall and OpenVPN for streaming iPlayer due to IP block requirements
• Description of a complex process for installing Ubuntu 2004 on an old server
• Discussion of remote access to ESXi console through IPKVM
• Installation of Ubuntu on server with slow upload speed
• Using SSH-import-id command to import public keys from GitHub
• ZFS setup and configuration, including creating a mirror of SSDs and using ext4 for root OS
• Setting up WireGuard point-to-point tunnel for remote access
• Using Sanoid tool to manage snapshots and replication with ZFS send/receive functionality
• ZFS benefits vs user space tools for data management
• Use of ZFS for irreplaceable data (e.g. photos, drone footage, container app data)
• Importance of checksums and data integrity checks for certain types of files
• Comparison with other file systems (XFS, ButterFS) and their checksumming capabilities
• Discussion of SnapRaid as an alternative to ZFS for checksumming
• Seeking advice on tools for generating and checking checksums for entire file systems
• Recommendation to use healthchecks.io for monitoring cron jobs
• Using curl for nightly checks and email notifications
• Implementing healthchecks for monitoring
• Linking healthchecks in show notes