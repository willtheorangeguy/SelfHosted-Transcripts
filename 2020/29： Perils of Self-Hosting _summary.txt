• Setting up outdoor security cameras and challenges
• Discussing Kevin and Patricia's setup from Traffic
• Comparing NVIDIA Shield with new Chromecast options
• Sharing experiences with ZFS data loss
• Advertising A Cloud Guru as a sponsor
• Self-hosted audio books and photos missing due to empty directory
• Difficulty diagnosing issue through Google search and seeking help from others
• Realizing that Docker created directories before ZFS tried to mount them
• Understanding that Docker's bind mounts feature caused the issue, resulting in silent failure
• Similar issue occurred with another system at the studio
• Problem solved by running specific commands to list mount points and identify the issue
• Data loss prevention with ZFS snapshots
• Upgrading from 1804 to 2004 and forgetting to reset Sanoid
• Managing tech debt and putting Sanoid configuration into Git
• Panic and troubleshooting during system downtime
• Container updates with Watchtower and alternative tools like Dion
• Docker Compose pull for manual container update management
• Discussion of Docker Compose and its simplicity
• Usefulness of tools like DWIN (Docker Image Update Notifier)
• Personal preference for manual updates over automation
• Introduction to Linode as a cloud provider
• Features and benefits of using Linode, including storage management and object storage
• Pricing and customer support offered by Linode
• Linode is mentioned as a cheaper and simpler alternative to AWS, Google Cloud, or Azure
• Traffic 2.3 has been released with plugins, allowing users to build and install custom middleware
• Plugins can be written in Go, hosted on GitHub, and executed by Traffic without compilation
• A marketplace for plugins has been created, where users can browse and download verified plugins
• Declarative versioning is used to ensure that published code is not modified or invalidated
• The difference between a plugin and middleware is largely one of terminology, with plugins being user-created middleware
• Plugins can be used to perform specific tasks, such as blocking access based on IP addresses.
• Blocking Comcast IPs to reduce traffic
• Pilot service for monitoring and reporting on usage data
• Data collection and tradeoff: users get free monitoring in exchange for sending data to improve product performance
• Comparison with Prometheus and Datadog: simpler, less granular, and lower cost
• Focus on basic availability and security alerts, rather than detailed telemetry
• Integration at the traffic level provides unique insights
• Security concerns around exposing endpoints and service details
• Kubernetes objects and traffic management
• Kubernetes ingress and service API updates (Traffic 2.0)
• Challenges with Custom Resource Definitions (CRDs) in Kubernetes
• Google's work on a new, vendor-agnostic ingress model for Traffic
• The Traffic Ambassador Program and community contributions
• Documentation challenges and leveraging the community to help
• Resources for getting started with Traffic, including articles, YouTube videos, and a monthly newsletter
• Traffic.io and its newsletter
• Ambassadors of Traffic.io
• Cloudfree.shop smart devices pre-flashed with Tasmota
• Review of the new Chromecast with Google TV
• Interface performance for streaming locally over LAN
• Compatibility with traditional Android TV apps, including Kodi and Plex
• Ethernet and power limitations of the new model
• Comparison to Nvidia Shield in terms of performance and features
• Google Assistant integration and voice search functionality
• Plex compatibility issues with Chromecast
• Price point and value for money consideration
• Siloed nature of Google's ecosystem and potential limitations
• Discussion of updates to apps like MB and Jellyfin and Plex for Google TV UI
• Home Assistant birthday updates, including new Mac app with API level integrations
• Development of Halcyon app, a Linux version of Home Assistant
• Call for community involvement in coding and website development
• Promotion of selfhosted.show membership and SRE program
• Social media presence and contact information