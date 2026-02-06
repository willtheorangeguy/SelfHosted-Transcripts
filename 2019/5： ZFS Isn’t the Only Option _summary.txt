• Disappointment with Shinobi software
• Issues with motion detection and plugin compatibility
• Overwhelming the Raspberry Pi with multiple cameras
• Performance problems with GPU acceleration and frame loss
• Alternative solution using Home Assistant for real-time viewing
• Wyze camera setup and potential for $100 full security system
• Struggling to get Shinobi running in a container
• Discussion of switching from a container approach to building on the host
• Use of Docker Compose for container management and updates
• Experience with StatPing experiencing downtime due to an issue with Postgres version mismatch
• Comparison of using containers vs. package installation for self-hosted applications
• Reliability issues with USB storage devices, specifically mentioning Pi machines and multiple disks attached via USB 3
• Need for storage solution to hold multiple days worth of data
• Requirement for ruggedized storage that can withstand level 4 earthquake conditions
• Considerations for storing Plex library, Docker configs, and other local media
• Discussion of SSD options and their cost (currently around $500 per 3.84 terabyte drive)
• Mention of smaller, more affordable SSD options (around $100) with lower capacities
• Description of user's current photo storage setup using a small SSD for year-by-year rotation
• Discussion of backup strategy, including multiple automatic copies of data stored across the internet
• Arrays on a pool of disks
• Using MergerFS as a potential solution for managing multiple disks
• Self-hosting storage setup considerations (requirements, use cases, RAID configurations)
• Importance of considering data integrity and protection when choosing disk configuration
• Use of SSDs vs. spinning Rust drives for different applications
• RAID 0 configuration risks and the "Scary Raid" label for reminder
• The speaker discusses their experience with storage in an RV and how they categorize files as "hot" or "cold" based on their frequency of access.
• They mention an article by Laurentius from January 2016 that influenced their strategy for purchasing hard drives, specifically regarding ZFS (Zettabyte File System) and its limitations.
• The speaker explains why ZFS is not suitable for their needs, citing the need for identical drives and firmware models to prevent hardware-related issues.
• They mention a solution they discovered in Western Digital's Easy Store 10 terabyte hard drive enclosures, which can be easily opened and repurposed as individual drives.
• The speaker discusses an electrical modification (3.3 volt mod) that may be required for these drives to function properly.
• Cutting or modifying the SATA power connector to prevent 3.3V signal
• Using Kapton tape or electrical tape to block power pins on drives
• Merger FS file system, allowing combination of mismatched drives under a single mount point
• Parity calculation using Snap Raid, for rebuilding from drive failures
• Comparison of various options: Merger FS, Unraid, and Open Media Vault
• Factors to consider when choosing a storage solution
• Importance of understanding specific usage requirements and data criticality
• MergerFS as a flexible alternative to ZFS for file system management
• Benefits of MergerFS, including support for any file system underneath it and hot plug of USB devices
• Challenges with ZFS, such as limitations in migrating from one pool to another
• Discussing the setup of a Raspberry Pi storage server
• MergerFS config being stored in the FS tab, not a separate file
• Considering SnapRate for parity disk management
• Requirements for SnapRate, including parity disk size and number of drives
• Feasibility of using Raspberry Pi with USB bus for storage
• Comparing to building a $100 used x86 system
• Cost-effectiveness and disposability of Raspberry Pi
• Using the RV as a power source for the setup
• Discussion on running a Pi 4 off DC power from batteries
• Unique storage requirements for a digital nomad lifestyle
• Discussion on ZFS vs CIFS for mirroring data directories
• Benefits of using ZFS with snap raid for data integrity
• Comparison of ZFS and CIFS features, including compression and encryption
• Recommendation against FreeNAS due to GUI-centric design and unfamiliarity with FreeBSD
• Advice to use a system that is easy to administer and maintain, such as SnapRaid
• Importance of off-site backups and redundancy in data storage
• Discussing potential issues with rsync and self-hosted backups
• Exploring alternatives to rsync, such as ZFS send and Duplicati
• Importance of data revision management in backup systems
• Personal preference for self-hosted security and responsibility
• Benefits of self-hosted solutions for digital well-being and satisfaction
• Discussion of Alan's expertise on ZFS and his work with FreeBSD
• Potential episode idea for self-hosting enthusiasts
• Recommendation to check out Brunch with Brent and Alan
• Mention of TechSnap.Systems and its simple explanations of ZFS concepts
• Jim Salter's expertise in explaining ZFS, specifically in episodes 4.14 and 4.15
• Plans for the podcast's next episode on benchmarking