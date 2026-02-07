• Alex has launched a YouTube channel and consultancy company called ktzsystems.com
• T-Systems offers freelance infrastructure consulting and building cloud-based solutions using infrastructure as code for other people
• The goal is to provide self-documenting playbooks that can be easily recreated by others, reducing vendor lock-in
• The consultancy will also offer expertise in ZFS backups, automation, VPNs, and other infrastructure-related tasks
• Alex has also started a new YouTube video on Ansible and Docker Compose secret management
• Discussion of decentralizing software development and the availability of alternatives to GitHub
• Mention of Docker's recent decisions regarding open source projects on Docker Hub
• Alternative hosting options, including Linde's services and benefits for developers
• Importance of having control over one's own stack and system management
• Promotion of Linde's features, pricing, and Greenlight program
• Docker format and its reliance on upstream images
• Risk of relying on upstream dependencies that may become unavailable
• Interview with Alex Ellis, founder of Opencast
• Alex's background in woodworking and hand tool craftsmanship
• Discussion of Firecracker and its potential for container management
• Alex's past project FASD and how it influenced his work with Firecracker
• GitHub Actions and Kubernetes operator build times were slow due to cross-compilation and large number of Go modules
• Private repos had limited free build minutes, leading to potential unbounded costs for a bootstrapped company
• Self-hosted builders on bare metal hosts were tried as an alternative, but faced issues with tool installations and concurrent builds
• Kubernetes operators for Docker builds were discussed, including concerns about mounting the Docker socket and security implications
• "Docker in Docker" approach was mentioned as an option, but discouraged due to performance and security issues
• Micro VMs were presented as a potential solution to simplify CI/CD pipelines and improve security
• Docker and Docker solution scalability issues
• Actuated.dev - a self-hosted alternative to hosted runners
• Pros and cons of using Actuated.dev, including cost savings and faster build times
• Pilot program for Actuated.dev is fully functional with teams running VMs
• Target market for Actuated.dev are companies with 5-50+ employees
• OpenAI vs Actuated.dev - differences in target audience and use cases
• Cost comparison of hosted runners (e.g. Cloud Build) vs self-hosted solutions like Actuated.dev
• Tale scale SSH and Send for self-hosted network management
• WireGuard noise protocol for flat mesh network
• Benefits of using Tale scale, including transparent networking and access control
• Docker Compose support for Rodman containers
• Rootless containers and their potential security benefits
• Comparison between Docker and Rodman
• The conversation discusses implementing Rodman with a kernel and avoiding "hacks" such as running daemons as root.
• The user shares their experience using Rodman on Ubuntu, initially encountering errors but resolving them by upgrading to version 4 from the package repos.
• Discussion of Docker Hub and registries, including the idea of automatically searching multiple registries in the Docker client.
• The conversation highlights features such as specifying registries in a cone file for Rodman.
• A user reports smooth experience with Rodman on their system, noting some extra considerations due to not running as root.
• Allowing privileged ports to be bound by unprivileged users
• Enabling the Rodman socket for traffic and Docker Compose
• Understanding that Rodman and Docker Compose can run as a user's own process
• The importance of enabling lingering to prevent system processes from terminating when the user session ends
• Creating a dedicated Rodman or container user with lingering enabled
• Using a specific user for running containers to simplify file permission management
• Rootless Rodman compatibility issues with Linux server containers
• Containers running as root user causing problems when mapping to host user ID
• Potential workarounds or add-in scripts for improving compatibility
• Nextcloud Hub 4 announcement and its integration of ethical AI
• Discussion of self-hosting options vs cloud-based services like Office 365/Google Workspace
• Nextcloud has introduced a SharePoint competitor
• Nextcloud Hub 4 features integration with Whisper, Stable Diffusion, and optionally ChatGPT
• Plans to implement a scoring system for information transfer to third parties
• Brent Nerva is on location in Berlin for further updates
• Discussion of Nextcloud's AI integrations and its potential impact on productivity
• Examples of Nextcloud use cases including photo backup, document storage, and recipe apps
• User shares experience with Nextcloud upgrade process that resulted in a dysfunctional system
• The speaker's Nextcloud instance experienced a database issue
• Possible causes include power outage, inverter/surge protector failure, and SQLite compatibility issues with Nextcloud updates
• The speaker used MariaDB as their SQL database instead of SQLite
• Recovery process involved running a SQL repair command, exiting maintenance mode, and using the OCC command line client to recover Nextcloud
• The instance is now back up and running
• The user has built an app that saves locations to a Nextcloud database and allows for export of data in common mapping formats.
• The user plans to migrate from SQLite to MySQL due to performance issues with SQLite.
• The user's experience with Nextcloud highlights the importance of upstream development catching and testing for issues related to specific databases.
• Belching has announced they will be pulling back from MATA (Multicast Automation Transport Abstract) until they can find a way to differentiate, which may lead to proprietary protocols being used instead.
• The hosts discuss potential boosts to the show.
• The host has been listening to the podcast since the guest was on the Home Assistant podcast
• The host mentions they are a member of Jupiter. Party and have subscribed to the guest's other shows
• A listener named Root boosts the podcast for episode 100 with 65,152 SATs
• Several listeners comment on the guest's diagrams and schemas, asking if they can be followed or used as a guide
• The host mentions they are trialling an extra network connection from T-Mobile, and it is working fine
• A listener asks about the software used to create the diagrams, which was draw.io
• The host discusses their experience with IPv6 and prefers using IPv4 due to its simplicity and familiarity
• Discussion about IPv6 public firewall port
• Boosts for the show and appreciation from hosts
• Scuba Steve's Nextcloud setup and its reliability over 6 years
• Inquiry on modern installation methods for Nextcloud in 2023
• Recommendation to use Docker (specifically rootless Rodman) for a rock-solid Nextcloud instance
• Alternative method involving Ansible
• Portability of Nextcloud instances with containerization
• Thanking SRE subscribers for their support
• Announcement of changes to ad-free feeds in the future
• Invitation to Linux Fest Northwest this October
• Call for Papers open for Linux Fest
• Reminder about meetups and joining meetup.com/Jupyter Broadcasting
• Contact information: self-hosted. Show, Twitter (@IronicBadger)