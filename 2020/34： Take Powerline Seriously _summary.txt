• Google experienced an outage due to internal storage quota issue
• Similar outages occurred with Amazon in the past, but self-hosting can provide balance and redundancy
• Importance of educating oneself on cloud technology and being prepared for outages
• Benefits of self-hosting include having full control and knowledge of one's own system
• Challenges of self-hosting include troubleshooting and dealing with stress when multiple people are affected by an outage
• Alex shares his experience rebuilding servers and moving storage to offline at the studio
• Importance of having a knowable problem with limited users and severity for home networks
• Thermal issues with server gear while traveling
• Need for a new location to house equipment due to ventilation and power requirements
• Limitations of antenna cord length requiring all equipment be placed nearby
• Discussion of router and switch placement due to electrical requirements and domino effect on equipment placement
• Placement of the antenna in a hot cab area despite initial reluctance
• Research into alternative networking solutions, specifically power line networking
• TP-Link is a standout company in networking
• Kasa devices are easy to integrate with Home Assistant
• AV-1000 Powerline adapters were used for networking in an RV
• They provided 300 megabits transfer rate between devices
• POE gear and power distribution was also discussed
• The user wants more information on using multiple Powerline adapters
• He's concerned about performance degradation with added traffic
• TP-Link AV1000s are claimed to provide gigabit speeds, but actual speed is 300 megabits
• The setup has improved networking in the RV and changed the user's life.
• LED light strip installation in a cupboard with temperature-controlled color change
• Automation setup using PepWave and bonded VPN for cellular routing
• Testing of the setup during an AT&T outage with seamless switch to Verizon connection
• Discussion of future plans, including thermal testing and potential Ethernet cable installation
• Promotion of Linode cloud hosting provider and its features
• The user tested different distributions (e.g. WordPress on top of various web servers) to find the best one for their needs.
• They used Linode's $100 credit to deploy multiple instances and test each distribution.
• The user also reviewed Linode, stating that it has been around forever and knows how to do its job.
• The discussion then shifted to power usage, specifically testing the Helios, an ARM-based CPU.
• The user compared the Helios' power draw to other systems (i5-8500 and Dual Xeon) under idle and full load conditions.
• The results showed the Helios using significantly less power than the other two systems.
• Power consumption of different systems (Helios, i5, Dual Xeon) with various loads
• Adding hard drives to each system and measuring power draw
• Comparison of costs based on power consumption and battery life implications
• Transcoding video (4K) and software requirements for processing power
• System performance differences between Helios, i5, and Dual Xeon processors
• The i5 CPU has quick sync and uses less energy than the Xeon
• Quick sync for H264 content is accelerated by Intel CPU
• Testing with Plex and quick sync showed 12 watts used during transcoding
• User had to use Linux server version of Plex and pass through device to enable hardware transcoding
• Using Proxmox, user passed through virtual GPU to VM and then to Plex container using Intel GVT-G
• This allows multiple VMs to share a single physical GPU for tasks like transcode and video encoding
• Raspberry Pi adoption is increasing, and the speaker sees this as beneficial for their show.
• The speaker considers consolidating their two Raspberry Pis with Proxmox on a ThinkPad with QuickSync.
• Energy savings: using a single system with QuickSync instead of multiple Raspberry Pis results in significant energy savings (35 watts vs. 300 watts).
• Cost-effectiveness: the speaker estimates that they will save around $100 to $150 per year, which will pay for the upgrade within three years.
• The PyKVM project enables remote access to the system using a BMC IPMI-grade interface.
• Mention of an Apple M1 device and its potential for comparison in power draw to performance.
• Promotion of cloudfree.shop as an unofficial sponsor of the show, offering cloud-free devices and smart plugs.
• The speaker discusses an unofficial sponsor of their show, Cloudfree.shop
• They attended the Home Assistant conference and found it to be one of the better virtual conferences they've been to
• The conference used a platform called Hopin that facilitated networking and meeting new people
• Home Assistant announced its first hardware device, "Home Assistant Blue"
• The speaker compares this device to the Odroid N2 Plus and Raspberry Pi 4, discussing their features and advantages
• They mention NebuCossip Cloud and how it supports full-time developers working on Home Assistant in a value-for-value model
• Announcement of new versioning system for Home Assistant Core
• Calendar-based version numbering (e.g., 2023-01-0) to indicate bug fix level
• Changed release cadence from every three weeks to every first Wednesday of the month
• Introduction of automation blueprints: pre-created automations with user-settable options
• Ability to share blueprints with others
• Improved non-Google voices via Nebukasa Home Assistant Cloud
• Temporary device disabling feature
• New feature to disable and re-enable devices remotely
• Discussion on the Wyze 3 camera, a $20 Wi-Fi camera with no monthly subscription required for basic features
• Comparison of Wyze 2 and Wyze 3 cameras, including design improvements and new features such as a wider field of view and improved night performance
• Review of the camera's capabilities, including two-way speaker, time-lapse feature, and starlight sensor
• Discussion on testing the camera's night performance and sharing thoughts on its capabilities
• The speaker had a difficult time changing Wi-Fi networks on the camera
• The camera has limited cloud requirements and offers advanced detection services
• The company plans to release an RTSP firmware that will allow for local recording without cloud connectivity
• The V3 model is an upgrade with more RAM and a faster CPU, which may improve RTSP streaming
• The price of $20 is considered astonishingly low for the features and quality of the camera
• Home Assistant can integrate with the camera's data to enable automations and local notifications