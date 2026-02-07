• Discussion of Arch Linux as a favourite distribution
• Benefits of using Arch, including ease of software deployment and minimal system requirements
• Comparison to other distributions, such as Ubuntu and Debian
• Mention of the AUR (Arch User Repository) as a key feature of Arch
• Personal experience with Arch and its documentation, credited with helping the user transition to Linux in 2013-2014
• Discussion of System, Docker, and their role in making Linux accessible to new users
• The speaker's operating system is continuously updated in a minor way to avoid major upgrades
• They prefer Arch Linux for its flexibility and ability to get updates quickly, but dislike package management systems like AUR
• Arch makes a great minimum viable server due to its minimalism and small attack surface
• Ubuntu is settling as the industry standard in the cloud, making it a safer choice for servers
• The speaker sticks with Ubuntu LTS for cloud deployment due to its stability and Canonical's testing efforts
• Using Ubuntu LTS on Raspberry Pis for minimal updates
• Running Arch Linux on local physical hardware at the studio
• Challenges with running Arch in the cloud due to vendor limitations
• Importance of not mocking people's choice of distribution, and including others in the conversation
• Linode.com as a platform that supports various distributions, including Arch, Alpine, Debian, CentOS, SUSE, Ubuntu, and Fedora
• Native SSD storage and 40 gigabit connections in machines
• Company's experience and locations, allowing leverage of expertise and relationships
• Data centres around the world
• James' experience with SMTP relay issues at previous VPS provider
• Linde support and policy on blocking SMTP-related ports by default
• Comparison to original provider's lack of helpful response to James' issue
• Importance of good support for infrastructure setup
• LastPass free tier limitations
• Comparison of LastPass and Bitwarden pricing
• Self-hosted Bitwarden server options
• Alternative to self-hosting: Bitwarden RS project
• Security considerations for hosting a password manager on a shared cloud VPS
• Blast radius of bots or web servers
• Running password manager on LAN for local data storage
• Configuring secure access to self-hosted backend
• Balancing security concerns vs convenience of hosted service
• Trusting organization like Bitwarden to handle sensitive data
• Concerns about security responsibilities and potential risks
• The speaker considers the cost of Bitwarden's subscription plan, finding it reasonable.
• They weigh the benefits of using a password manager with a sustainable business model.
• Mobile access and hosting concerns are mentioned as important considerations for the speaker.
• The speaker compares Bitwarden to LastPass and notes that team plans are available at $3 per user.
• Bitwarden self-hosting and Docker image
• Sharing passwords with others through Bitwarden organizations
• Comparison of Bitwarden to other password management solutions like KeePass
• Discussion of Plex media server security issues and a recent botnet attack
• DDoS attacks and amplification by misconfigured Plex servers
• Discussion of a vulnerability in Plex that allows remote access through a common port
• Steps to mitigate the risk, including closing the vulnerable port and setting up a custom server URL and DNS entry with Cloudflare
• Importance of using a reverse proxy or similar setup to protect against abuse
• Mention of a study by Net scout finding 27,000 servers vulnerable to this issue
• Discussion of unrelated issue with WireGuard VPN, involving a misconfigured DHCP subnet and resulting routing issues
• User describes the benefits of separating subnets for different VPN endpoints
• User explains their own experience with subletting and networking issues
• A listener helps user troubleshoot an issue, teaching them new concepts about networking and triage
• Promotion for 20% off annual plans at CloudGuru.com mentioned
• Discussion of growing demand for cloud professionals and benefits of cloud certification
• Listener "Ryan" asks about running a Linux server with GPU pass-through to a Windows VM for Blue Iris, while still using the GPU for containerized applications like Plex.
• The user discusses using Graphics Virtualization Technology (GVT-G) for virtualized GPU acceleration
• GVT-G is compared to Intel Quick Sync, with the former being significantly slower and less stable
• The user performs a test on an iPad using Plex for offline playback, comparing CPU rendering vs. GVT-G acceleration
• Results show that GVT-G is 80-82% slower than running Quick Sync natively on the host machine
• Stability issues are also reported, with system crashes, kernel panics, and processes hanging during use
• The user concludes that GVT-G is not a viable option due to its poor performance and stability problems
• Discussion of encoding options and performance per watt
• Comparison of Intel Quick Sync to NVIDIA GPU performance
• Decision to split tasks into physical boxes for better power management
• Overview of hardware used for server and Blue Iris setup (HP290 Slim, i5 CPUs)
• Details on blog setup using Ghost and medics
• User account management discussion, including centralized authentication options
• Discussion of Active Directory support on Linux distributions
• Use of standardized accounts and SSH keys for authentication
• Potential use of System Homed for centralized user management
• Consideration of central authentication systems and single sign-on
• Personal experience with managing large LDAP installations
• Current approach to security practices, including infrequent password rotation
• Upcoming post-show 3D printing discussion
• Reminder to visit self-hosted. Show for show content and contact information
• Hosts' social media presence (Twitter, Discord)
• Show hashtag (#selfhostedshow) or ID mentioned (selfhosted.show.com/39)