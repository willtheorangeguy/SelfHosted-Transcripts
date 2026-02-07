• Artificial intelligence is secretly hosting the show
• Discussion of custom firewall software and Open Sense
• Comparison of AI-generated audio to human speech patterns
• Exploring the possibility of voice-controlled Home Assistant setups
• Criticism of current voice assistant technology (Siri, Alexa, Google)
• Discussion of a potential future project to integrate personal voices into smart home systems
• Discussion about rebuilding and upgrading home network
• Introduction of new gear from Unify
• Explanation of the complex network diagram created by Alex, including details on hardware and devices used
• Breakdown of how the host's home network is structured, with two separate halves for downstairs and upstairs areas
• Mention of 5G internet service and a T-Mobile carrier-grade NAT line
• Discussion of Unify switches and their features, including POE power and auto-negotiation capabilities
• Explanation of Ethernet devices and NIC speeds
• VLAN routing and Layer 3 switching
• Difference between L2 (Layer 2) and L3 (Layer 3) networking
• Open Sense as a VLAN orchestrator and potential performance considerations
• Consideration of using a Layer 3 switch for hardware-based acceleration
• Unify Switch Flex minis as small, managed switches with POE support
• Trying T-Mobile's home internet service and its performance compared to Spectrum
• Setting up T-Mobile internet as a failover for Spectrum
• Using Plans (Virtual Local Area Networks) to tag ports and create separate networks
• Configuring Open Sense box to use T-Mobile connection as a backup
• Load balancing between T-Mobile and Spectrum connections
• Using Unify switches and Switch Flex minis to manage network settings
• Troubleshooting internet connectivity issues with easy switch-over between Plans
• Unify cloud controller allows creating dedicated Plans for Wi-Fi SSIDs
• Routing internet traffic over Plans and setting up separate networks for specific devices
• Linde cloud hosting discussed, including one-click deployment options and features like Jitsi and Nextcloud
• Benefits of using Linde, such as reasonable pricing, data centres around the world, and ability to disperse infrastructure
• Promotion for new users: $100 in 60-day credit by signing up at linode.com/SSH
• Traffic issues during a Google Meet call
• Using various tools to troubleshoot network problems
• Testing cable with an Ethernet tester and finding it was fine
• Using Smoke ping to ping switches and identify packet loss
• Replacing 10G link with gigabit switch and resolving issues
• Identifying bad twisted pair in Cat 6A termination with a Klein cable tester
• Finding multiple terminations with flappy pairs and deciding to redo them properly
• Discussion about network issues and troubleshooting with a Gigabit connection
• Problem with a Wi-Fi access point dying due to power delivery issues
• Replacement of old Wi-Fi gear with new Unify equipment, including U6 Pros and 12 new switches
• Introduction to Net box as an alternative to DHCP and IPAM system
• Discussion about being sick while working on networking projects and the challenges of troubleshooting network issues
• Upgrading a CPU from a Cameron G4900 to an i5-9500 in an HP290 Slim case
• Discussion of the benefits of using i5 CPUs, particularly in the eighth-gen sweet spot
• Comparison of small form factor builds and their costs, with the example of an $92 combo unit upgraded to around $300
• Impact of CPU upgrades on performance, specifically for Blue Iris software
• Discussion of peace of mind and convenience provided by home security systems
• Mention of Raspberry Pi 4s feeling outdated and desire for a new model with improved storage options
• Discussion of Smoke ping and other services
• Comparison of Droid H3+ performance with Pi 4
• Plans to build an Droid K3S cluster
• Review of the Pi KVM Kickstarter campaign and interest in building a custom Pi KVM for OBS system
• Explanation of the Pi KVM software and its features
• Discussion of using a USB 3 KVM switch with HDMI matrix for network KVM
• Review of the cost and capabilities of the Pi KVM hardware
• A user commented on a blog post about an EC-C22 device exposing the PMI web GUI to the internet when rebooting.
• The commenter, Banco, described how he fixed the issue by moving the WAN port to another Ethernet port and applying a fix.
• Alex explained that Rock Rack BMC implementations have a dedicated PMI LAN port and two gigabit ports for connecting devices to the LAN.
• When multiple IP addresses are assigned to these ports, it can lead to issues with Plans and PMI functionality.
• A user described how they had to use an PMI raw command to turn off the BMC on one of the NIC's to resolve the issue.
• Update on Audio bookshelf iOS client
• Issues with UI and Scrabble bar resolved in new update
• New layout moves playback controls above Scrabble bar
• Remaining issues: playback head not moving with circle gesture, sensitivity issues with swiping
• Host still uses Audio Bookshelf despite remaining issues
• Feedback from listeners praising Audio bookshelf
• Discussion of Intel Arc GPU and its ease of use on Linux
• Intel Arc technology and its potential for virtual machines
• GPU pass-through and GVTG (Graphics Virtualization Technology) challenges
• Creation of an GPU benchmark specifically for media encoding purposes
• Crowd-sourcing and publishing benchmarks on perfectmediaserver.com as a searchable database
• Planning for anonymous storage of user-submitted benchmark results
• Interest in comparing CPU performance across different generations and architectures
• Upcoming meetup on March 4th at the 192 Brewing Company
• Discussion about future events and potentially throwing their own with bigger budgets
• Mention of a second Raleigh meetup being considered for this spring
• Introduction to JB Jobs room for jobseekers and employers to connect
• Self-hosting updates, including link in show notes at self-hosted.show/slash/91
• Thank yous for boosts received from listeners, including Sam Squawk's generous donation after an outage
• Discussion of the challenges of self-hosting, particularly with power outages
• Discussion of power outages and backup systems
• Comparison of Audible to Libra FM, an independent audiobook platform
• Concerns about consolidation of power in the market and Amazon's ownership of Audible
• Technical discussion on network infrastructure, DHCP, and static IPs
• Suggestion for automating IP configuration and updates using automation tools
• Boosting in and upgrading to a compliant podcast app
• Albie.com and toping up for the podcast index
• Becoming an SRE (site reliability engineer) at selfhosted.show/SRE
• Ad-free version of the show with post-show content
• Upcoming discussion on documentation workflow
• Coder robe, Tumblr, and sticker promotion
• Self-hosted stickers available at jupitergarage.com
• Promotion of Alex's services through blog.ktz.me and Twitter alternatives