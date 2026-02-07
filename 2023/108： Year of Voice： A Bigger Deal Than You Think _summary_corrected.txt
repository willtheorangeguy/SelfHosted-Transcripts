• Chris's water heater and pump are now automated with Home Assistant
• Jeff visited Chris's RV to help install the automation system
• They encountered issues finding a negative wire and connecting it correctly
• The generator panel in the RV has a unique design, requiring them to find a specific wire
• Chris had concerns about inadvertently triggering other systems while working on the project
• The solution involved using an ESP device and relays from Amazon, which are now integrated with Home Assistant
• ESP boards (D1 Mini or clones) are used for smart home automation
• Relay usage and pinouts require careful consideration to avoid malfunctioning
• Modular design allows easy replacement of components, reducing obsolescence concerns
• Shelley's are a viable alternative with similar features but throw up their own Wi-Fi AP
• ESP Home has a strong community and open-source route, with tighter integration with Home Assistant
• Setting up ESP Home with Home Assistant
• Challenges in project implementation (grounding issues, small things)
• Complexity of building and soldering relay boards
• Scope creep and adding features (water pump, multiple relays)
• Upgrading old systems (electric buttons) to use relays
• Philosophy of "building back better" and using open-source tools
• Promotion of a sponsor (Leno.com)
• Discussing the features and benefits of Linde, now backed by Akamai
• Mazda taking down a library for interacting with Mazda cars from GitHub due to copyright claims
• The impact on Home Assistant's integration with Mazda services and the decision to remove it
• Concerns about ownership and rights to integrate car systems with home automation software
• Mazda's integration with Analytics had 227 users, but the conversation wonders if this was reported or counted by Mazda
• The group discusses how manufacturers like Mazda might be limiting user API calls to control user experience and upsell services
• The issue of manufacturers controlling user experience and potentially locking people out of their own data is mentioned
• Open standards and local connectivity are seen as a solution to this problem, allowing users to avoid cloud dependency
• The conversation touches on the development of Wake Words for voice assistants, a major milestone in the project
• Wyoming Protocol for integrating voice assistant pieces into a bigger stack
• Home Assistant not being powerful but using Open Whisper and Piper for speech recognition
• Using a cloud server for Wyoming, allowing choice and experimentation with open source projects
• Nebulas service and its ease of setup and good results
• Privacy story of Nebulas's authentication token-based approach, not storing user data
• Comparing to Echo or Google Home Assistant, which link personal data to users' homes and identities
• Wake word creation process
• Cola notebook for generating wake words
• Open Wake Word pipeline and its capabilities
• Model training process and fine-tuning
• Home assistant limitations with current setup
• Alternative solution using Docker container or GPU pass through
• Fine-tuning with voice samples recorded by the user
• 45 Home Lab division and HL 15 product launch
• The speaker is excited about a new product from 45 Drives for home labs
• The product has high-performance capabilities and comes with handpicked applications such as Home Assistant and Nextcloud
• The company has a community forum where users can help each other with setup and support
• The speaker discusses potential improvements to be made, including better wake word detection and audio cleanup on the ESP32
• They also discuss the benefits of streaming model for satellite requirements and local processing
• Plans to build custom hardware for Home Assistant
• Importance of user experience and aesthetics in device design
• Discussion of using voice assistants on Linux desktops and the potential for a Linux desktop assistant
• Projects such as Piper that use open-source technology for speech recognition and other applications
• Security audit of Home Assistant, including authentication stack and web stack vulnerabilities
• Home Assistant's summer audit and fixes have been rolled out
• Users who haven't kept up to date may be vulnerable to security issues
• The report on security issues is being published in parts, including CVEs and a timeline
• A new approach to handling security issues is to be more transparent and open about them
• This includes publishing security updates as part of normal business
• Home Assistant's year of voice has been successful so far, with various products contributing
• The team is working on making the Atom Echo work easily with Home Assistant
• There are plans to make the Atom Echo firmware available directly on the device.
• Upcoming features and improvements of the Tail scale VPN
• Subnet routing feature for accessing devices on restricted subnets
• WireGuard encryption for secure connections
• New partnerships and integrations with Apple TV app and Multan
• Feedback from listeners, including a recommendation for Symphonic Android app as an alternative to Plex amp
• Recognition of VT-52's contributions to the community, including sharing hackable devices
• Comparison of various single-board computers, including the Lima Blade and its specifications
• Discussion of authentication methods, specifically LDAP, OAuth 2 proxy, and HTTP basic
• Mention of a user's experience with a small home server build using the ZIM Board
• Request for deeper dive into NVR software, specifically Frigate and its performance on Intel Atom processor
• User experiences improved inference time with TPU
• TPUs are cheap and work well for certain tasks
• Frigate is a preferred NVR solution on Linux, but has stability issues
• Waze cams can be integrated with Frigate for successful results
• Self-hosting options such as Shinobi and Frigate discussed
• User shares success story of using Tail scale for secure remote access
• pfSense and HA Proxy used in conjunction with Tail scale for VPN setup
• Discussion of benefits of open-source software over proprietary solutions
• Nextcloud setup difficulties
• Reliability of all-in-one Docker containers for Nextcloud
• Simplicity vs complexity in server setups
• Use of Nix to set up Nextcloud and Postgres
• Concerns about maintaining complex systems
• Difficulty in making technology approachable for users, especially those new to it
• Trade-off between flexibility and user growth, allowing software to adapt to users' changing needs
• Confusion about which path to take when transitioning from beginner-friendly tools to more complex ones
• Importance of clarity in guiding users through this transition process
• Example of Nextcloud's evolution and the need for clearer guidance for new users
• A listener has a problem setting up an HP Thin client with Mint XFCE and wants help connecting it to their Fedora desktop.
• Discussion about the advantages of using the same distro on both the RDP server and client for compatibility.
• Recommendation to try a smaller Linux distro or one specifically designed for thin clients, such as those for RDP.
• Tips for troubleshooting and verifying RDP functionality, including launching Romania or Microsoft RDP client.
• Discussion about thin clients and remote desktop technology.
• Upcoming reunion and catching up
• Paulus' appearance on the show
• Progress of the Year of Voice project
• Home Assistant setup and pipeline options (local, Raspberry Pi, Nebulas Cloud)
• Integration with Android and ability to replace Google Assistant
• Switching between different Home Assistant servers
• Playing with back-end tech and future prospects for the project