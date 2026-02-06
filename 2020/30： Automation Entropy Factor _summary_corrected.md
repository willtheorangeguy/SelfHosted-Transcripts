• The hosts discuss their Prime Day purchases, including a Fire tablet for $50 and a Soda Stream.
• Alex bought a 43-inch TCL TV with Android TV for use in the kitchen.
• The conversation turns to using external set-top boxes or built-in Android on the new TV.
• They discuss the affordability of TVs during Prime Day sales.
• A potential business expense opportunity is mentioned, considering buying another screen for the studio.
• The speaker has been buying various external hard drives for reporting and testing purposes
• They've purchased 10-terabyte Easy Store from Best Buy ($189) and 10-terabyte Seagate USB 3 drives ($150 each)
• The speaker is shucking (removing the original drive and replacing it with a new one) some of these drives to evaluate performance
• There's a concern that hard drives may degrade faster when they're close together, leading to overheating issues
• The speaker has observed significant temperature differences between helium-filled and air-filled hard drives in their testing
• They recommend keeping temperatures below 45°C (or ideally around 20-24°C) for optimal hard drive performance
• Data centres and hard drive engineering
• Pre-burn-in considerations and smart tests
• Performance of helium-filled drives vs air-filled drives
• Western Digital's rebadging practices with Hitachi UltraStar and WD Red drives
• Importance of burn-in testing to weed out weak drives
• Issues with refurbished drives and warranty replacements
• Discussing slow performance of some hard drives
• Testing performance of new vs old (2-year-old) drives
• Comparison of shucked vs unshocked drives and their performance
• Cost-effectiveness consideration in choosing drives for specific use cases (workstations vs RAID)
• Recommendation to avoid 10-terabyte Easy Stores due to heat issues
• Promotion of Linde hosting service and its Terraform support
• Discussion of object storage as a data storage solution
• Advantages of object storage for static websites and cloud storage
• Recommendation to use Linde for cloud hosting with a $100 credit offer
• Automations built by the speaker for their RV's heating system
• The RV's temperature control system using sensors and smart plugs
• Personal experience with self-hosting and potential downsides
• The speaker uses Home Assistant to control the heaters in their bedroom
• The speakers' wife enjoys the warmth when entering the room due to Home Assistant's automation
• However, the heaters turn off after three minutes instead of remaining on as expected
• The speaker wakes up cold in the middle of the night and discovers that the automation issue is specific to turning the heaters on, not off
• The speaker realizes that there is a difference between the two automations, which is causing the issue
• Home Assistant's recent updates have led to issues with automations, resulting in a backlog of irrelevant troubleshooting information.
• The speaker encountered a generic error while trying to troubleshoot their automation issue, making it difficult to find relevant solutions online.
• After comparing the off and on automations, the speaker realized that the issue was caused by using the built-in "sun below horizon" condition.
• Changing this condition to use the state of a sun sensor resolved the issue and made the automation work as expected.
• The speaker discovered that using the sensor state is necessary for reliable sunrise and sunset-based automations in Home Assistant, as the graphical interface's logic can cause issues with built-in conditions.
• Home Assistant user experiencing issues with automations stopping work
• Possible connection between software updates and automation failures
• Idea of a testing framework for automations to prevent errors
• Use of third-party add-on to check configuration against new version releases
• User's enthusiasm for Home Assistant, despite occasional issues
• Integration of Amazon Echo and Ring API with Home Assistant
• Home Assistant as a unifier for various products
• System D course offered by Cloud Guru
• OBD2 data and its potential uses, including fuel savings and monitoring engine health
• Using devices like Automatic or OBD2 dongles to collect car data
• Integrating collected data with Grafana and InfluxDB for visualization and analysis
• The power of graphing data to see overall trends
• Discussion of monitoring basement humidity with a graphed trend
• Monitoring oil temperature and noticing a gradual increase over six months
• Question from audience member Optimum Gray about database management, specifically whether to merge multiple MariaDB instances into one or keep them separate
• Alex's response that there is no right answer, but two main schools of thought: merging databases for simplicity or keeping separate for efficiency
• Discussion of using environment variables to feed username and password info to containers
• Alex's current strategy of creating a database instance per app for simplicity and easier management
• The speaker discusses the challenges of running multiple applications on a single database instance and the benefits of using separate instances for each application.
• They mention the trade-off between security and convenience, particularly in a personal LAN environment where attack surface is not as significant.
• The speaker recommends using Docker to manage application containers and make porting services easier.
• An email from Jay is read aloud, describing an issue with NFS remounting on Free NAS after waking up from sleep.
• The speaker suggests using System to auto-remount file systems when the network connection comes back online.
• Discussion of Cloudfree.shop and their NFC tags for Home Assistant
• Announcement of ESXi on a Raspberry Pi
• Limitations of running ESXi on a Raspberry Pi (local storage issues)
• Potential uses for running ESXi on a Raspberry Pi (testing VMware, learning, backup scenarios)
• VMware virtualization on Raspberry Pi for running services
• Benefits of using VMware on ARM devices, such as management and development tools
• Challenges of developing software for large ARM systems in data centres
• VMware's strategy to provide a development environment for ARM code that can be deployed in the cloud
• Potential use cases, such as sales meetings or travelling professionals needing a portable virtual environment
• Announcement of a pick, Archive, a self-hosted knowledge repository for preserving and organizing useful content.
• Discussing the benefits of having a local copy of digital content
• Example given of Netflix/Disney censoring The Simpsons on Disney+
• Comparison to owning physical copies (DVDs) that cannot be changed
• Update on project activity and planned integrations with Hacker News and Reddit
• Discussion of setup requirements for the project (Docker, elastic search)
• Promotion of supporting the show through ad-free content and extra features