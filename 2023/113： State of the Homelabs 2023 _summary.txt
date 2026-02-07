• Bitwarden's pricing stability
• Brent's experience with Christmas markets in Germany
• The hosts' home lab setup for 2024 and recent changes
• Dashboards as a popular topic among self-hosters, including choosing services to fit into a small footprint and managing maintenance.
• The speaker has tried various dashboards but found them too cumbersome to maintain
• They prefer monitoring individual machines instead of using a centralized dashboard
• Grafana is used for basic trend analysis and alerts are set up in healthchecks.io
• Monitoring vs. dashboards: the speaker finds monitoring more relevant for self-hosters
• The importance of having reliable monitoring to catch issues before they become major problems
• Brent's experience with building a storage system, which has been a "disaster" so far
• Discussion of prioritizing important vs. less important services when setting up a dashboard or monitoring system
• Borg backup system
• File system based backup solutions (ButterFS)
• Issues with backup systems (hard drive burning disks and SSH issues)
• Tail scale solution
• Server architecture for Borg backups
• Physical separation of backup systems
• Failed fan on X220 laptop and thermal management shutdown
• Fan is running for too long and may need to be replaced
• Backup destination is experiencing issues, including randomly turning off
• Considering moving to a more robust backup solution (e.g. Borg)
• Discussion of deduplication methods and technologies (Borg, file systems)
• Alex's backup situation is discussed, with him sharing his own disaster experiences
• Alternative backup solutions and strategies are mentioned, including Synology boxes and ZFS arrays
• England's pints are larger than US ones
• The speaker has a remote backup server at their house that self-hosts and is connected to the UK server via ZFS and Syncoid
• The speaker's backup solution involves using duplicati, S-T-O-R-J for photo storage, and Starlink with an Odroid
• The speaker had issues with their Synology at their mum's house due to Autorestick and MinIO changes
• The speaker criticizes abstracted away management UIs, citing the trouble they caused when it broke down
• Duplicati backup system and its encryption methods
• Recovery issues with Duplicati, including difficulty accessing data
• Comparison of Duplicati to other backup systems, including their design philosophies
• Preference for tape drives as a backup method, due to simplicity and reliability
• Discussion of document management systems, including Nextcloud and Paperless NGX
• Using Google for everything
• Experience with Nextcloud and DAVX
• Invoicing software: Invoice Ninja vs. Invoice Plane
• Networking gear: generic HP switches and recent upgrade to fiber network
• Home network setup and troubleshooting
• Cameras: moving away from Wyze Cam, currently using Blue Iris and PoE cams, planning a potential major change in 2024
• Discussion of Pihole and its usage for DNS and DHCP
• Nix OS as a potential router solution
• Tailscale as a VPN solution with features beyond traditional VPNs
• Stability and performance of Tailscale
• Comparison to other networking solutions such as OpenSense
• Tailscale can simplify network infrastructure by bridging multiple data centers on one flat LAN
• ACL policies allow secure control and access to devices and services, with integration into enterprise authentication policies
• Tailscale saves time and money compared to VPN providers, and offers features like file sharing between devices
• The speaker has upgraded their security and networking setup using Tailscale
• They mention an upcoming segment on media playback and share their experiences with Jellyfin and Plex
• The speaker is now using Tailscale to share media servers with friends and family without exposing their network to potential vulnerabilities
• They have removed video content from their Plex server due to security concerns, leaving only audiobooks and music
• The NVIDIA Shield is mentioned as a reliable streaming device that has continued to work well despite being eight years old
• The host discusses their experience with the NVIDIA Shield and its launcher issues
• They recommend using Projectivity Launcher to remove ads from the NVIDIA Shield
• The host compares the NVIDIA Shield to Apple TV, stating that Apple TV is a better option due to its performance and lack of launcher issues
• The host mentions playing Alto's Odyssey on their Apple TV and enjoying its features
• Brent shares his media setup, including using Jellyfin for video and Plex Amp for music
• The host discusses ripping DVDs and setting up a machine to do the task efficiently
• User's family relies heavily on streaming services
• Challenges with switching users to Jellyfin due to technical support required
• Importance of having a "single source of truth" for note-taking and organization
• Discussion of Obsidian as the preferred note-taking tool, including its features and benefits
• Comparison between different note-taking tools and workflows
• Personal experience with Obsidian's searchability and discoverability
• The user is using Obsidian as their note-taking infrastructure and has built a PC around it
• They are experiencing issues with syncing and organization, feeling that they spend too much time on these tasks and losing momentum
• Visual note-taking is an important part of their workflow, but current solutions lack robust image searching capabilities
• The user would prefer Obsidian to be open-source for data sovereignty reasons
• They have also experimented with NextCloud-only Notes-based solutions, including Quillipad, but encountered syncing issues
• For task management, the user uses G Suite and To-Doist, finding it effective and easy to use on various platforms
• The user has tried NextCloud Tasks, using a combination of the web interface and the Android app tasks.org
• The speaker discusses their task management setup using NextCloud Tasks and Tasks.org syncing
• They mention using Todoist as a potential alternative due to its API and integrations
• Brent shares his experience with paper-based task management and expresses interest in upgrading
• Alex discusses his use of Proxmox for server management and plans to switch some VPS nodes to Nix OS
• The group briefly touches on the topic of server operating systems, including Nix OS and Wayland/Pipewire/Plasma 6
• Nix OS and its benefits for production systems
• Comparison of Nix OS with Ansible
• Using custom images on Hetzner VPS providers
• Converting Ubuntu to Nix OS Live using "Nix anywhere"
• Linode's features and services, now part of Akamai
• Managing configuration on workstations with Nick's Darwin in a Flake setup
• Installing Brute apps and configuring system preferences
• Using brew for package management, but also installing some tools from Nix
• Setting up Nix OS on multiple machines
• Switching back to Nginx for reverse proxy after initially trying it with Nix OS
• Implementing CADDLXC files for simplified service configuration
• Experimenting with Podman and Docker compatibility in containers
• The speaker has been using a system for six years and is considering switching to a setup with Nix containers, TailScale, and Systemd nspawn.
• The new setup would eliminate the need for a reverse proxy and allow for direct connections between applications on the tail net.
• The speaker finds learning Nix to be a steep curve, but may end up adopting it in the future.
• File systems were discussed, with the speaker advocating for ZFS for important data due to its checksumming and snapshotting features.
• For media files or ephemeral storage needs, the speaker uses XFS with MergerFS on top to merge disks of different sizes into a single mount point.
• SnapRAID is used to calculate parity for data on JBODs, but may be considered dropping it in favor of a simpler setup.
• Discussion of transitioning from XFS to ZFS
• Mention of using ButterFS with mirrors and virtual disks for storage
• Comparison between ZFS and ButterFS, including built-in capabilities and hardware requirements
• Brief mention of other file systems (Extended 4, XFS) and their issues this year
• Home automation setup discussion, confirming use of Home Assistant
• Discussion of Zigbee controller issues, including dropped connections
• Comparison between Zigbee and Z-Wave for home automation
• Experience with Tubes ZB coordinator and router
• Importance of repeaters in maintaining a stable Zigbee network
• Frustration with Zigbee's mesh networking design
• Home automation desires and changes from Brent and Alex
• Incorporation of humidity sensors into an RV for automation
• Use of ESP32 platform for various applications, including voice control and remote monitoring
• Comparison of 3D printers, specifically switching from Prusa i3 to Bamboo Lab printers
• Discussion of the capabilities of the ESP32 platform, including running a webcam and other devices
• Announcement of a new product called HL15, available on 45homelab.com, with features such as open-source software and high-performance storage
• Review of products received in a batch of "boots", including a large number of shafts and spanner sets
• Discussion of syncing watch status between Plex and Jellyfin servers using a Docker container called Plex Jellyfin Watched.
• Chasing own tail with multiple note systems
• Plex as gateway drug for self-hosting
• Music Assistant integration with Home Assistant
• Party mode automation idea
• Thermostat solution using ESP32 and relays
• Concerns about interlocks and firmware complexity in thermostat automation
• Accidental damage risk with combined cooling and heating
• Discussing automations and edge cases with lighting and garage doors
• Sharing control methods for heating and air conditioning systems using Home Assistant and IR blasters
• Feedback on the Smart IR project and its integration with Home Assistant
• Nix and NixOS discussions, including a potential talk at NixCon USA
• Upcoming conferences and meetups (Scale, NixCon, LinuxFest, etc.)
• The speaker mentions being affected by a rug pull in a project they invested in.
• They have been using Jellyfin and appreciate support from boosters.
• The show made $83,600 and is supported through boosts and SRE (Site Reliability Engineer) memberships.
• The speaker thanks listeners for supporting the show directly.
• A post-show topic will be discussed by Brent.