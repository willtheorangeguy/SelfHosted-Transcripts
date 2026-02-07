• The speaker has made a life decision to move away from suburbia and potentially buy land in the Appalachians.
• They've decided to buy an RV to facilitate this move, allowing them to explore potential properties without needing hotels or other accommodations.
• The RV will also provide a mobile workspace with internet connectivity, enabling remote work.
• They're planning for a medium-sized Class C RV or camper van.
• They're aware of the benefits of having a solid internet connection and are considering using Starlink.
• Discussion of Starlink internet and its USB Ethernet capabilities
• Managing multiple internet connections with a single router
• Use of Dishy's built-in features, including DHCP relay and modem functions
• Comparison between self-hosted services and company-hosted services
• Use of ZFS for remote replication and disk management
• Use of Tailscale for secure access to servers and devices
• Self-hosted server issues with Juice SSH and HedgeDoc
• Importance of monitoring and alerting systems
• Consideration of switching to object storage for backend data
• Discussion of matrix protocol and its decentralized, federated nature
• Author's experience with self-hosted services, including Matrix server setup issues
• Logo image issue causing display problems for some users
• Need for software to handle resizing images automatically
• Difficulty with storing and managing large amounts of data (images, videos, chat logs)
• Frequent updates required for Synapse server
• Challenges with self-hosting Matrix instance compared to Discord or Slack
• Recommendation to limit public access and encourage users to sign up at Matrix.org
• Matrix server deployment decision and its implications
• Discord as a compromise over self-hosted options
• Production infrastructure outage and maintenance responsibilities
• Jellyfin alternative to Plex, with positive review and recommendation
• Linode cloud hosting sponsorship and service benefits
• Linode's new storage, MVME, is a game-changer for high-performance applications
• Benefits of MVME include higher IOPS per gigabyte than traditional storage
• Linode's data centers and customer support are highlighted as advantages for users
• The speaker praises Linode's system updates and package caching capabilities
• Portainer, a Docker GUI, is introduced and its features and uses are discussed
• Discussion of Portainer management instance
• Number of containers and applications being managed (30-40)
• Challenges with staying on top of updates for internal software
• User's experience with Portainer: frustration, tediousness, and restrictive features
• Comparison to Docker Swarm: more complicated and restrictive
• Paid version of Portainer vs. community edition
• Historical issue with company's templates being featured in Portainer
• Docker GUIs add complexity
• Users should manage container definitions in a version-controlled Git repository
• Current solutions (e.g. Portainer) don't offer much value beyond what can be done manually
• Some tools (e.g. OpenSense, Compose) are solving the wrong problem or offering unnecessary complexity
• The speaker has successfully implemented Portainer on a Raspberry Pi and is impressed with its simplicity
• However, the speaker suggests that spending time learning configuration management tools like Git and Ansible could be more beneficial
• The speaker shares an example of using Ansible to generate Docker Compose YAML files for multiple servers
• They emphasize the power of configuration management in automating repetitive tasks and reducing the need to think about specific settings for each server
• Discussion about GUIs and non-repeatable UX flows
• Promotion of Backblaze.com for cloud backup services
• Features and benefits of using Backblaze, including web restore, app restore, and restore by mail programs
• Mobile app for accessing files securely in the cloud
• Statistics on number of files restored for Backblaze customers
• Trial offer for a fully featured account with no credit card required
• Another GUI (Lazy Docker) mentioned briefly
• LazyDocker GUI interface is available on Mac, Windows, Linux, and can be installed via curl
• The GUI provides an overview of running services, containers, images, and volumes in a NCURSIS style clickable interface
• Users can interact with the GUI using mouse or keyboard, and perform tasks such as viewing config information, Docker compose files, process information, and logs
• LazyDocker was praised for its ability to quickly identify issues, such as containers restarting constantly, without needing to actively check logs or investigate further
• The GUI is seen as a useful tool for getting an overview of system status and identifying potential problems, particularly in cases where there is limited time to explore the system.
• The speaker talks about using Lazy Docker to reconnect with a container
• Docker stats command for viewing container information and resource usage
• Analyzing container performance and identifying memory hogs, specifically Java applications
• Using Docker Compose to limit RAM usage of specific containers (e.g. BookSonic)
• Discussion of a master process that opens a port on behalf of a service and leaves the service stopped until a connection is received
• Need for similar functionality for Docker containers to save resources
• Examples of projects where containers are running 24/7 unnecessarily
• Mention of Dazzle.dev, a real-time Docker container log viewer in the browser
• Overview of Dazzle.dev's features and security considerations
• The speaker is discussing their experience with the log search function of an application.
• They mention using Dozzle to search through logs and finding useful real-time search functionality.
• Docker Compose is changing from a standalone Python thing to being inside Docker itself.
• Existing Docker Compose commands will map to new Docker Compose commands, but with a different invocation (Docker space-Compose).
• The change is largely tech debt being addressed by bringing the separate project in-house.
• There may be some small changes to the Docker Compose spec and backwards compatibility issues.
• Tech debt release with minimal new features for normal users
• Developers are excited about the tech debt release
• Docker Compose is a key feature that made it click for the speaker
• The ability to visualize infrastructure and application dependencies in plain text using Docker Compose files
• Docker Compose has become an official part of the main Docker app, with support in other tools like Podman
• Docker Compose V2 profiles allow addressing multiple services within a single file
• Profiles can be used to categorize containers, such as test or prod environments
• New feature in Docker Compose V2 allows listing different stacks and their containers
• User wrote a blog post about the new features and linked it in the show notes
• Upcoming live stream will cover building an ESP-based device with ESP Home
• Plans to hang out with members and update on tech progress
• Promise to have more information by the end of 2021
• Discussion of goals and Alex's goal
• Instructions for sending feedback through self-hosted.show/contact
• Contact information for podcast creators (Twitter handles)
• Self-deprecation about plugging Twitter and consideration of discontinuing it