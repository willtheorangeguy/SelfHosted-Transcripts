• Discussion on automated updates and their potential for causing system instability
• Recent CrowdStrike sensor update that blue-screened many Windows machines
• Importance of proper testing and deployment strategies to prevent similar issues
• Comparison with Nix OS, which handles auto-updates more smoothly
• Criticism of Windows' handling of crash scenarios and lack of rollback capabilities
• Discussion about a major Windows issue affecting computers worldwide
• Machines left on overnight were affected by the auto-update, while those turned off or running at different times were not
• Issues for people working in remote locations or on weekends due to lack of access to servers and displays
• The update was pushed on a Friday, causing additional inconvenience
• The speaker's experience driving during a heat wave and struggling with system overheating
• Plans to install permanent cooling for a solar lithium inverter system
• The speaker has a Starlink setup in their RV but experiences issues with internet connectivity due to tree cover and lack of cell signal.
• They realize they set up their devices (Jellyfin and Ersatz TV) using public DNS that points to internal IPs, causing issues when trying to access them offline.
• The speaker needs a fast local DNS solution, considering options like Pie Hole or split DNS magic.
• They also look for an offline messaging system, such as Telegram threads or a similar simple solution.
• Discussing a revolutionary paper-like device with lots of pages
• Using public DNS causing some issues with online resources
• Building an offline-capable system for testing internet connectivity
• Importance of testing and verifying a system's functionality without external connections
• Experiencing internet outage and discovering multiple devices still connecting to the internet despite being configured for offline use
• Identifying critical devices that require adjustments when the firewall or internet connection goes out
• Devices connected to a LAN and streaming content from Jellyfin without requiring a routable internet connection.
• Issues with devices such as Chromecast, Google Home screen devices, and the Nvidia Shield not connecting to Wi-Fi.
• The user's desire to "fake out" these devices into thinking they have internet access when there isn't any.
• Problems experienced by the user with their robot vacuum (VAC) dying while they were away, and then having issues getting a new one to connect to their 2.4 GHz Wi-Fi network.
• Comparison of Android vs iOS in terms of ease of connecting devices to Wi-Fi networks.
• Discussion of a doorbell and wireless connectivity issues
• OnePlus device's 2.4 GHz and 5 GHz capabilities
• Experiences pairing Wi-Fi devices on iOS vs Android
• HomeKit integration limitations and potential "SIM card lock"
• User's preference for direct communication with devices over HomeKit integration
• Purchase of NVMe SSDs on Prime Day
• Installation of SSD into Epic build case with issues finding the right fit
• Dust filter for a case
• Solution to the dust filter issue using a $12 magnetic filter kit from Amazon
• Description of the ESP Home device update controversy
• Interview with Keith, developer of ESP Home, after a break
• Unraid.net's public beta release of Unpaid 7
• Unpaid 7 beta release
• ZFS capabilities fully integrated into Unpaid 7
• New features for hybrid ZFS pools and special VDE types
• Ability to run own storage as pools with all-SSD platforms
• Unpaid 7 performance is "mind-bending fast"
• Discussion of Unpaid operating system and its uses
• Just Keith from Nabu Casa joins the show
• Introduction to Nabu Casa and Just Keith's role
• Work on ESP Home, hardware, and software development
• Definition of ESP Home
• ESP Home as a platform or framework for building IoT devices and embedded systems
• Overview of ESP32 and 8266 microcontrollers and their role in ESP Home
• Ease of use of ESP Home for building custom applications and solving problems
• Modular building blocks, including YAML code, for creating firmware
• Compilation process and outputting binary code for microcontrollers
• Discussion of ESP Home and its features
• Comparison to other smart home options
• Customizability and modularity benefits
• Cost-effectiveness and affordability of ESP32 components
• Importance of updates and firmware life cycle for smart devices
• Community discussion on updating frequencies for these devices
• ESP Home works by describing the desired components in a YAML file
• Not all components of ESP Home may be relevant to a specific device or use case
• Updating ESP Home may not be necessary if only non-essential components have changed
• Release notes and change logs should be reviewed before updating to determine if changes are relevant to a specific device
• Updating every release is likely unnecessary and could result in unnecessary rebuilds.
• Discussion of business policies related to software updates, including PCI compliance
• Explanation that updating every month is not always necessary for embedded devices with limited behaviour changes
• Concept of smaller Delta updates that are "smarter" about device configurations
• Potential future development of a system that understands which components have been used and flags only necessary updates
• Concerns about the lifespan of flash storage in devices, specifically ESP devices, and potential effects of frequent updates on their lifespan
• S3 devices have limited write cycles due to flash memory
• Wear levelling and distribution of writes can help increase lifespan
• Devices used in applications where state changes periodically require non-volatile storage for data, not just program code
• Flash longevity is good, but can be affected by frequent rewriting or heavy usage
• Examples include development boards that can be rewritten dozens of times a day without significant wear on the flash memory
• The ESP Home project was acquired by Home Assistant and is now managed alongside other projects
• Nebulas exists due to the growth of Home Assistant, which required a larger team to maintain
• Nebulas started about six years ago and monetizes open source through subscription-based services
• This model allows developers to work on the project full-time and has been successful for Home Assistant
• The speaker discusses the advancements in voice technology and its applications
• Home assistants are an exciting application of voice technology
• The speaker mentions ChatGPT and large language models as related developments
• The ESP home assistant has been improved with the ability to update entities without compiling source code on a local machine
• A contributor created a PR to allow ESP devices to pull updates over the air (OTA)
• Firmware image update process
• Automatic update capability in ESP home
• Integration with Home Assistant's update entities
• Time-saving feature for updating devices
• Voice updates and future plans
• Lockstep release schedule between Home Assistant and ESP Home
• Monthly live streams by the Nebulas project
• Schedule adjustments for release
• Grist as an open-source alternative to Airtable and Google Sheets
• Benefits of using spreadsheets and low-code app building
• Grist's approach to connecting spreadsheet capabilities with robust software features
• Integration and self-hosting options for Grist
• Promotion of Grist as a solution for complex, load-bearing spreadsheets
• The Image Project has introduced a pricing model, with optional support for individuals or servers starting at $25.
• The project has shifted from a "license" to a "purchase" model, with a lifetime option available.
• Pricing varies depending on the number of users: $24.99 for individual licenses and $99.99 for multiple users.
• The price change was met with initial concerns about the use of the word "license," but clarification has been provided by the project team.
• The pricing is optional, and individuals can choose to support the project without committing to a purchase.
• Concerns about a $99.99 one-time purchase for the Image software
• Developer's salary and the value it represents in terms of cost
• Comparison to other pricing models or options
• Need for extra features or benefits to justify the high price point
• Supporting open-source projects through financial contributions
• Paywall-free features in the application
• Cloud storage backup options for photos
• Potential to charge users for cloud storage instead of developing their own solution
• Community-driven model for software development and maintenance
• Restructuring JB infrastructure to accommodate growth and costs
• Migrating core services from Linde to a new server
• Considering Peer Tube and potential community hosting options
• Evaluating cost-effectiveness of cloud services for specific tasks (e.g. GPU accelerated transcription)
• Planning to add in-house capabilities for tasks currently outsourced
• Exploring use of Proxmox for virtualization and management of virtual machines
• Discussion of transitioning from Proxmox to a different system for the studio
• Mention of shared resources and remote access
• Use case discussion about spinning up specific distros for testing purposes
• Vision of automating publishing process, including encoding and transcription
• Comparison to existing system called CastaBlaster on Linde
• Discussion of integrating audio and FLAC files with automated transcription capabilities
• Discussion of server setup and options for a colocated (Colo) server
• Naming suggestions for the new server, including humorous options
• Decision to use Proxmox for virtual machine management
• Review of features and benefits of using Proxmox with the Colo server
• Mention of tailscale.com as a service for networking and VPN solutions
• The speaker discusses using Tail scale for secure remote access to devices and networks
• Tail scale provides a VPN-like service for connecting devices directly to each other securely
• It's suitable for self-hosted, home libbers, and companies due to its ease of use and security features
• The speaker shares their experience with setting up Tail scale on various devices and services
• A listener asks about deploying Nix OS on a cloud VPS currently running Ubuntu
• Nix OS installation and booting process
• Next Cloud using the Nix module base for better performance
• Alternative apps for self-hosting, including Plex, Jellyfin, and F-droid
• Setting up sandbox Google Play Services on Graphene OS
• Using Docker OS 10 as a Mac VM in a container
• Discussing vehicle recommendation for Brentley
• Setting up a VNC connection for remote access
• Reliable vehicles, specifically Toyota Tundra, mentioned as an option
• Boost signal from Iraq with email alerts via Amazon SES
• Using NTF Wire Notify with uptime Kumar for notifications
• Discussion of game servers and streaming setup
• Issues with graphics card drivers and replacing the old RX 560
• Resolving performance issues with new RX 6800 XT/6700 XT graphics card
• Issues with Barite and Steam Deck performance
• HDMI audio issues and disrupting streams
• Switching to Nintendo Switch for gaming needs
• Virtualizing graphics cards as a possible solution
• Discussion of various controllers and gaming experiences
• Announcement of show boosters and sponsors, including Fountain and Strike master
• Upcoming meetups, including one in Spokane and another hosted by Brent
• Latest Home Assistant release (to be discussed in a members-only section)
• Self-hosted listeners who attended the previous meetup in Spokane
• Promotion of the self-hosted podcast and its community
• Hosting information for Alex (Katie's End)