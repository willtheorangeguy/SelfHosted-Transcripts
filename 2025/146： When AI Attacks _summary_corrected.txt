• Criticism of Plex's new UI redesign
• Concerns about increased complexity and user frustration
• Discussion of lost features, such as downloading entire series
• Mention of Plex's mixed libraries and potential for a "mess"
• Comparison to other media solutions, such as IPTV apps
• Speculation that the new app may be an April Fool's joke
• Debate about whether Plex's motives align with providing a great local media experience
• Concerns about Mediant (MB) being closed source and how it compares to Jellyfin
• Discussion of AI bot scrapers impacting open source projects, including Wikipedia's recent article on the topic
• Introduction of guest Z Basso, who has written extensively on the subject of AI bots and their impact on self-hosted infrastructure
• Wikipedia receives many requests from non-genuine humans (bots)
• AI-powered scrapers are a significant problem for free software projects with limited funding
• Distributed denial-of-service attacks and distinguishing between human and bot traffic are related issues
• The speaker has implemented a "proof of work" system to block AI scrapers, inspired by an email spam prevention method called hash cash
• Mozilla is commonly used in user agent IDs to bypass browser detection, which is based on a 90s-2000s practice called user agent sniffing
• Difficulty implementing CAPTCHA to prevent scraping due to limitations of current methods (e.g., SHA-256)
• Concerns about inadvertently locking out browsers that don't support JavaScript or Big Indian systems
• Exploring alternative solutions, including WebAssembly and Equal X
• The use of human solvers by industrial scraper services, bypassing CAPTCHAs
• Limitations of current CAPTCHA methods due to advancements in AI and computer vision capabilities
• Anubis, a web scraper prevention tool, was implemented on GNOME GitLab and resulted in a 96% reduction in system load
• The tool is most tested with Git forges and may have varying success rates depending on the specific use case
• AI companies are changing the social contract by scraping data without permission
• Certificate Transparency Logs can be used to monitor certificate issuance, but malicious bots are subscribing to these logs to scrape HTTPS responses
• Unpaid 7.1 has been released with new features including wireless networking support and improved ZFS pool importing
• The guest discusses their home lab setup, which is based on Unpaid and runs Kubernetes and Longhorn.
• The lab was set up using four nodes that run Linux, with the goal of having a distributed system where work and storage can be migrated to other machines if one fails.
• The host notes that their power bill is likely low due to free electricity provided by their landlord.
• The guest defends using Kubernetes in a home lab, acknowledging its complexity but arguing its worth the learning opportunity for developers who want to retain skills like site reliability engineering (SRE).
• The guest also discusses the importance of maintaining SRE skills, which can have a "half-life" and require regular practice to stay current.
• Discussion of using Kubernetes in a home lab for educational and career purposes
• Alternatives to Kubernetes mentioned: Dou (like Heroku but with Docker), Docker Swarm
• Devil's advocate perspective on why not to use Kubernetes, specifically for one-machine scenarios
• Overview of Talos Linux, a "boot-to-Kubernetes" OS that boots in 2 seconds
• Discussion of storage options, including Longhorn and ZFS with RAID Zed 2 (RAID 5 with hot spare)
• Use of NAS under the desk as a legacy deployment due to stability concerns and personal preference
• Details about the storage setup: 62.4 TB redundant, 618 TB Iron Wolf Pro by Seagate, RAID configuration
• The host accidentally put all git server data on rotational drives instead of SSDs
• This caused performance issues when Amazon's scraper started hitting the server
• Anubis (a project) exists because of this mistake
• Mistakes like this are common in SRE work and can lead to unexpected outcomes
• Feedback from listeners included boosts, comments on previous episodes, and suggestions for future content
• Self-hosted retro game archives on Android TV
• Apollo app and its open-source implementation of NVIDIA Game Stream
• Streaming games from server to remote devices without resolution issues
• Integrating classic ROMs with Android using Retro Arch, Cody, and plugins
• Nix as a tool for managing media servers and automating tasks
• Discussion about unstable systems breaking down and the importance of backup plans
• Upgrades to the narrator's server setup with a new 9950X based compute node and i5 9500 media servers
• Must's hardware setup in an apartment with multiple rooms providing services and need for UPS solutions
• Suggestions for affordable UPS options from APC, Cyberpower, and Amazon
• Shoutouts for various contributors to the show, including Jordan Bravo and Fuzzy Miss Born
• Recap of boost statistics and appreciation for Sees and audience members supporting the show
• Thanks to listeners for tuning in
• Ad-free show and post-show available on self-hosted. Show
• Upcoming episode: New Home Assistant updates
• Meetup page mentioned, with events listed at meetup.com/jupiterbroadcasting
• Linux Fest Northwest approaching
• Contact information available at alex.ktz.me
• Promotion of new show "The Launch"