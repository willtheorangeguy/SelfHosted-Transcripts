• The host has been experimenting with new home server setups
• They're looking for a Discord bot to help with title suggestions for their show
• The bot would allow viewers to suggest titles by typing "bang!" followed by a suggestion, and then publishing the top-voted options on a web page
• The host has attended an open source conference and shares his thoughts on its quality, noting that it's semi-commercial and had both good and bad sessions
• Jim Salter was scheduled to speak about ZFS but cancelled due to illness.
• Microsoft's shift in focus towards Linux and open-source development tools
• Scott Hanselman's presentation on WSL2 and its integration with GitHub and VS Code
• Criticism of Windows' limitations and "corporate tax" strategy
• Comparison of WSL2 to running a native Linux system
• Acknowledgment that there are situations where Linux does not cut it, but WSL provides an alternative for developers who must use Windows
• Development containers as a solution to encapsulated development environments
• Scott's talk on development containers, which provide a JSON manifest for project requirements
• Microsoft's creation of the Windows Terminal and its recognition as an open-source project
• The presenter's own experience with Docker containers during their master's degree program
• The presenter's friend Michael Dominick's journey from Mac to Windows, including using WSL and VS Code
• A meetup at All Things Open conference, where attendees met up in the lobby using a Matrix chat
• Burnout and stress management
• All Things Open conference sessions and content
• Red Hat Tower and meeting with listeners
• Boar's Head sauce and its commercial availability
• LearnNixTV and Jay's talk on RetroPie and retro gaming
• CM4 module and its uses in home lab setup
• Discussion about the fun projects that open-source developers want to work on
• Event at All Things Open, including meeting cool people and networking
• Introducing Sync Thing as a great tool for ambient file system sync
• Using Sync Thing to keep progress in sync between devices
• Advertising Linode.com as a sponsor of Jupyter Broadcasting and offering $100 off new accounts
• Discussing the importance of trying out a product before committing to it
• Introducing Linode.com and encouraging users to sign up with the SSH option
• Announcing the arrival of Home Assistant Yellow, a year after crowdfunding
• Experiencing issues with the device's storage and performance, including:
	+ Not using the MVME disk as expected
	+ Moving data from EMMC to MVME through a migration process
	+ Initial stress due to lack of understanding of the process
• Outlining the benefits of resetting and starting fresh on Home Assistant devices
• The speaker had a difficult time setting up Home Assistant in the past
• They were able to recover their configuration from an old backup and made adjustments manually
• Z-Wave migration was easier than expected, with devices still paired to the new controller
• The speaker suggests that Home Assistant could benefit from an onboarding wizard or assistant for new device setup
• The interface has become much more user-friendly over time, making it easier to set up and manage devices
• They have a significantly reduced number of automations compared to previous setup, relying more on scheduling cards instead
• The user discusses their positive experience with Home Assistant Yellow using NVMe storage, noting significant improvements in speed and performance.
• They mention that the generic thermostat and scheduler card features have greatly simplified automations and saved time.
• The user describes the benefits of using a leaner system, including smaller backup sizes (now 70-80 megabytes vs. 1.2 gigabytes).
• A problem with their Shelley device is described, where it was rebooting and resetting itself every 30-60 seconds when under load.
• The user replaced the stock firmware on their Shelly device with an open firmware using a tool called MG2X for over-the-air firmware upload.
• Discussion of the Shelly smart plug's update process and its integration with custom firmware
• Concerns about a Shelly smart plug going offline in the speaker's new setup
• Investigation into possible causes, including temperature limits set by Mongoose OS
• Comparison of different smart home ecosystems (HomeKit vs. Zigbee) and devices (ESP Home vs. TAS motor)
• Review of a Zenglid Zigbee Smart LED light strip for use with Home Assistant
• The speaker is trying out a new setup with Nix OS and Jellyfin media server
• They set up Infuse on Apple TV for streaming
• The speaker had an issue with the Jellyfin app not working due to incompatible server version
• The issue was caused by Jellyfin being out of date on NixOS, but it's close to getting updated
• The speaker notes that Nix is a rolling distribution and depends on maintainers
• Discussing the need for intro detection plugins in Jellyfin
• Comparing Plex and Jellyfin media setups
• Mention of issues with TV breaking at inconvenient moments
• Adoption of Plex and NVIDIA Shield as default media setup due to reliability
• Real-time updates on Hia's face in Discord chat
• The speaker is having trouble with Netflix on their NVIDIA Shield TV due to an auto-update of the Jellyfin app.
• They mention the irony that if they were using Apple TV and Infuse, the issue wouldn't exist.
• The speaker expresses optimism about Jellyfin's future improvements and believes it will be "good enough" within a year or two.
• They plan to use Jellyfin at home and keep Plex running on their studio server for archived media.
• A plugin is mentioned that allows for skipping intros in Jellyfin, with some limitations.
• Comparison of Jellyfin and Plex media libraries
• Discussion of Jellyfin's progress and potential as an alternative to commercial projects like Plex
• Mention of Rune and its limitations in offline playback
• Reference to XBMC and the potential for Jellyfin to be a modern version of that project
• Promotion of jupiter.party and membership benefits
• Comparison of home assistants for privacy and functionality
• Integration of Mycroft with Home Assistant and potential issues with Google speech-to-text
• Concerns about relying on cloud-based services for voice transcription
• Alternative text-to-speech service through Nebukasa Cloud offering improved sound quality
• Use of Nebukasa's service for nighttime scripts in Home Assistant setup
• Discussion of bedtime mode and its limitations
• Desire for a local solution to tie into speakers and control devices
• Introduction to Mycroft integration and request for user feedback
• Boost from Gene Bean and his question about backing up Nextcloud
• Explanation of the speaker's backup strategy using ZFS, replication, and other tools
• The cost of backing up large amounts of data (25 terabytes) and the limitations of current backup options
• AWS Glacier as a potential backup solution, but expensive for large data sets
• Alternative option: building a server to store data at a friend's house or on-site
• Use of Jupyter.tube for live streaming and recording podcasts
• Fountain app for value-for-value podcast boosting, with mixed reviews from users
• The Rune Lifetime used to cost $499, but is now $699.
• The CEO threatened to pull the product due to unsustainable costs.
• A listener bought the lifetime subscription because they prefer a one-time payment over monthly fees.
• Feature voting on the Rune forum showed that users want the offline grace period for servers re-enabled.
• This may be a defining moment for the company, and how they respond will impact future decisions.
• The Zimra board was mentioned as an alternative to Raspberry Pi, but the speaker is skeptical about buying one.
• Device is designed for installation in a vehicle due to its ruggedized features
• Concerns about company viability and potential Kickstarter pitfalls
• Discussion of device's performance, storage, and compatibility with peripherals
• Comparison to Odroid solution and concerns about form factor and design intent
• Potential uses and customizations of the device despite reservations
• Great submissions and boosts from community members, including MG, J-Cube, Nev, Acorn, and Thumbs
• Discussion of terminal emulators and apps, with user recommending Hollywood as a favorite app
• User memories of listening to the podcast in specific places and how it brought back memories
• Conversation about careers and life-changing moments sparked by listening to the podcast
• Discussion of an old interview where Docker wasn't yet called Docker
• Mentions of boosts and messages sent by "Ninja Mort" with no context or explanation
• Promotion of the podcast's membership program and self-hosted platform
• Mention of a Matrix instance for Jupyter broadcasting
• Acknowledgement of Alex for updating the infrastructure due to OpenSSL patches
• Setting up unattended upgrades on Ubuntu boxes
• Alex recommends using Ubuntu systems with auto-updates
• Discussing the effectiveness of automated security patches
• Mentioning feedback and contact information for the podcast
• Off-topic discussion about Elon Musk's projects and a notable financial transaction