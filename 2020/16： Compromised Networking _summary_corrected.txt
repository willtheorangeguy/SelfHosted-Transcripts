• Quarantine life and self-isolation statistics
• Launching a Discord server for community engagement
• Debate on self-hosted chat platforms vs non-self-hosted alternatives
• Balancing self-hosting principles with practical considerations (e.g. audience reach)
• Follow-up discussion on Gross, toilet paper stockpiling inventory management system
• The speaker discusses a feature of the Barcode Buddy app that allows users to scan barcodes and add items to a database
• Apple has acquired Dark Sky, a popular weather service, which is raising concerns in the home assistant community
• The speaker notes that many projects rely on Dark Sky's API for backend information and worries about its future availability
• The chance of implementing a DIY weather station using an ESP8266 board and other parts is mentioned as an alternative to relying on Dark Sky
• The speaker discusses Apple's possible motives for acquiring Dark Sky, including maintaining a competitive advantage and internalizing the service
• The impact of Apple's acquisition on existing users who rely on Dark Sky's API is also discussed.
• Replacing Dark Sky in Home Assistant
• Reviewing the author's experience with switching to Home Assistant (HASS.io) on a Raspberry Pi
• Tips for migrating Z-Wave devices and integrations
• Discussion of smart plugs, including TP-Link and Taste options
• Rebuilding Home Assistant instance and MQTT server
• TP-Link plugs and ease of use
• Limitations of remote control through Echo or other devices
• Value of rebuilding systems for learning and automation
• Home Assistant's ability to integrate with multiple devices and services
• Using Shelly smart switches to convert dumb switches to smart switches
• New dashboards feature in Home Assistant allows different home screens for devices
• Waze cams work better with new load, but firmware update can enable webcam mode
• Using a Waze cam as a webcam is not recommended due to manual firmware installation and cloud server disconnection
• Logitech C920 webcams are a better option at $40 used
• Home networking basics will be covered in future content
• Working from home has led to increased Wi-Fi trouble, with people moving closer to the router for reliable calls
• Home networks with Wi-Fi have inherent problems due to their radio nature.
• ISP-provided routers often combine functions of routing and Wi-Fi hotspots, which can cause issues.
• Cheap, memory-constrained routers can quickly exhaust their routing tables, leading to poor performance and crashes.
• Separating the modem/router from Wi-Fi devices improves network stability and flexibility.
• Using Ethernet cables for devices that can support them helps reduce reliance on Wi-Fi.
• Ubiquity's Unify line of devices offers sophisticated management and can be controlled remotely.
• Hosting the Unify controller in a Docker container or Linux server allows for centralized configuration and backup.
• Separating Wi-Fi from the ISP provided router allows for easy transition between locations without reconfiguring devices.
• Awareness of neighbouring access points can improve signal balance, but this is not a primary benefit of centralized controllers.
• Zero handoff feature in Unify gear enables seamless roaming between access points.
• Testing throughput with Airspeed app revealed an issue with a dodgy Ethernet port that was resolved by securing the cable.
• A well-configured network is crucial for good Wi-Fi performance, and separating Wi-Fi from the firewall can aid in troubleshooting.
• Some mesh solutions combine router and firewall functions, which can be problematic.
• Discussion about providing feedback in Discord
• Mention of Pine64 board and running pfSense or Open Sense on it
• Introduction to Net Data, a monitoring app that provides real-time metrics
• Benefits of using Net Data, including visualizing system performance and identifying issues
• Home Assistant integration with Net Data
• Story about accidentally exposing services to the internet and data loss
• Ask SSH question from SEB Couture
• Discussion of whether Home Assistant should be accessible via reverse proxy
• Security considerations for remote access to Home Assistant
• Comparison of using a WireGuard connection versus Home Assistant cloud for remote access
• Importance of authentication and password protection for internet-facing apps
• Use of a VPN (WireGuard) for secure networking