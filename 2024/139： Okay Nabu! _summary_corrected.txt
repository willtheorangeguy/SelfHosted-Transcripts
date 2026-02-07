• Host thanks colleagues for covering his absence due to illness
• Discussion of Brent's new hardware setup and its potential impact on their show
• Introduction of guest Paulus from Home Assistant, discussing the release of a voice preview edition and a new era for the platform
• Details about the design and simplicity of the Home Assistant Voice Preview Edition hardware
• Explanation of the rotary encoder used in the device and its tactile feedback
• Discussion of software changes in Home Assistant to support voice functionality and Bluetooth onboarding
• Introduction of ESP Home, an open-source software for creating smart home devices, and its role in developing an open standard for Wi-Fi setup (improve Wi-Fi)
• Home Assistant's speech-to-text and text-to-speech capabilities
• Using local or cloud-based solutions for voice assistant functionality
• Whisper AI system and its potential issues with resource-intensive requirements
• Recommended hardware for running Whisper, such as the Intel N100 chip
• Bluetooth and other features added to Home Assistant with future hardware plans in mind
• ESP Home's over-the-air updates and media endpoint capabilities
• Developing a voice assistant with the ESP32 S3 box and considering user interface requirements
• Realizing the need for a larger screen to display information in response to voice commands
• Discussing Home Assistant Preview Edition and its features as a milestone for the company
• Exploring the possibility of using local AI models, such as OBAMA, for smart home control
• The potential for users to interact with their homes through voice commands, accessing various devices and data
• Designing an API that allows custom components or integrations for expanding the AI's capabilities
• Plans for future development, including improving information architecture and making it easier to interact with Home Assistant using natural language
• Information architecture as a priority for the project
• Development of dashboards and automation editor
• Integration of AI functionality
• Unraid.net self-hosted operating system release candidate features
• Tail scale support integration with Unpaid
• Progress on automations, dashboards, and other areas in 2024
• Upcoming roadmap for 2025 to be announced in April
• Home Assistant's capabilities and strengths
• The need for a more user-friendly experience and "glue" to hold everything together
• Creating pre-built solutions and dashboards, such as the energy dashboard
• Building on top of default dashboards with community-fed knowledge
• Automation blueprints and making it easier to use them
• Voice assistant hardware and the Home Assistant voice puck
• The balance between user-friendliness and modifiability of devices
• Opening up voice assistant hardware for other companies to build on
• Tail scale is promoted as an easy way to connect devices and services remotely, with a focus on security and speed.
• The speaker mentions that they are currently using the "self-hosted" plan, which has been their plan for a very long time.
• Tail scale offers secure remote access to various services, including databases, applications, and servers.
• The technology allows for a zero-trust flat mesh network, where devices connect directly to each other.
• The speaker mentions that they have replaced traditional VPN systems with Tail scale and now use it to manage their home network.
• Tail scale can be used as a more powerful alternative to traditional VPNs, allowing users to manage networking like code.
• The technology integrates well with existing authentication infrastructure.
• Nix is discussed as a related topic, where the speakers mention that they may have fallen out of love with it.
• Ease of starting up applications and managing Home lab services
• Declarative configuration for Nix Home lab setup
• Issue with monolithic config and child configurations for each service
• Experimentation with running Nix OS in containers (Spawn and Docker)
• Building a platform as a service using Nix server
• Challenges with Nix module system, specifically services side
• Inconsistencies in upstream Nix OS modules and difficulty modifying them
• Package system in Nix is loved, but services side is problematic
• Configurations and safeguards in place to prevent issues with user permissions
• Challenges with customizing Nix modules for use within a Docker container
• Need for consistency across modules and services
• Importance of flexibility and the ability to learn and understand module capabilities
• Discussion about the growth and standardization of packaging formats, including Docker and Nix
• Docker as a standard packaging format for Linux home servers
• Nix and its rebuilding process affecting iteration speed
• Rebuilding entire closure vs hot reloading specific changes
• Benefits of explicit dependency management with Nix
• Potential for two modes: pure mode (full rebuild) and dev mode (hot reload)
• Nix shell as a tool for short-term, temporary workarounds
• The speaker thinks Nix has limitations and may be moving away from it
• They prefer Docker for its standardization and consistency
• A lack of package developers or service developers publishing their own flakes is a barrier to adoption
• The speaker mentions Kee bio, an open-source keyboard company with DIY parts and microcontrollers
• The speaker's home lab project involves deploying cron jobs, shell scripts, Go binaries, and Docker images/compose files, and they are looking for a reasonable way to manage this setup.
• Yeet is a tool for easily deploying services to remote systems
• It can yeet binaries, Docker images, or Docker compose files to a remote system
• The tool can automatically configure the deployed service as a system service and attach Tail scale to it
• Tail scale integration allows for secure access to the deployed services with automatic TLS certificates and reverse proxies
• Yeet can also manage secrets using encryption
• The speaker compares Yeet to Docker Compose and considers the possibility of creating a repository of compose files that can be sprayed onto servers and managed as services
• Yeet is being used as a method for securely managing environment variables in Docker
• The user discussed their experience with Yeet, including its limitations and plans to make it publicly available
• The conversation shifted to Shane's server relocation project, where he brought his server on a plane from Connecticut
• Discussion of TSA screening procedures and concerns about the server being inspected
• Recap of a successful test flight with a plane
• Discussion of the plane's bandwidth capabilities
• Mention of fan-created 3D printed cases for the project
• Introduction to a special holiday episode recording
• Request for feedback and boosts
• Promotion of meetup.com for upcoming events, including UP 600
• Introduction to a new self-hosted meetup alternative at colonyevents.com
• Shane mentions his online presence can be found at alex.ktz.me
• Host suggests Shane's GitHub page (github.com/Shane) as an alternative
• Shane also has a presence on Weapon X (Chris LAS)
• Mention of Chris LAS's other project, Foster (chrislas.com)
• Reference to Jupiter Broadcasting and its various shows