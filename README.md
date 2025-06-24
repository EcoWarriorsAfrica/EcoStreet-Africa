EcoWarriors Africa
EcoWarriors Africa is an immersive, educational driving simulation game where you step into the role of a young EcoWarrior tasked with delivering seedlings, recycling bins, and solar kits across real-world-inspired African cities. Our mission is to provide a fun, replayable experience that empowers players to learn about sustainable practices—fuel efficiency, waste management, renewable energy—through hands-on gameplay.

Project Purpose and Vision
Educate: Integrate real-world environmental data and eco-tips into gameplay to teach sustainable practices in bite-sized, memorable segments.

Entertain: Offer dynamic driving mechanics, timed challenges, and various missions (tree planting, waste collection, solar kit delivery) to keep players engaged.

Inspire Action: Show players the tangible impact of their virtual actions—reducing CO₂, planting trees, cleaning rivers—encouraging real-life environmental stewardship.

Target Audience
Age Range: 10–25 years (students, educators, eco-enthusiasts)

Interest Groups: Casual and educational gamers, schools, NGOs, youth climate clubs

Supported Platforms: Windows and macOS for desktop, with planned support for Android and iOS mobile platforms in future releases

Key Features
Driving-Based Missions: Navigate realistic city roads delivering cargo—choose efficient routes, avoid obstacles, and manage fuel to earn top ratings.

Educational Overlays: Display pop-up facts during gameplay (for example, “Driving at 50 km/h can reduce fuel consumption by 20%”).

City Progression: Increase each city’s EcoHealth meter and unlock new vehicles, missions, and story beats as you accumulate Environmental Points (EP).

Competitive Mode: Race against friends or ghost runs to deliver fastest and safest, with leaderboards and daily/weekly challenges.

Offline and Online Hybrid: Core game functionality (driving, cargo, UI) is playable offline; leaderboards, daily events, and multiplayer activate when online.

Technologies and Packages
Unity 2021 LTS with Universal Render Pipeline (URP)

TextMeshPro for advanced text rendering

Unity Input System for handling multiple input devices

Cinemachine for dynamic camera control

Post-Processing stack for visual effects

ProBuilder for rapid in-editor geometry prototyping

Mapbox Unity SDK (optional) for real-world map streaming

Photon PUN 2 or Mirror for real-time networking

Firebase or PlayFab for backend services such as cloud saves and leaderboards.

Repository Structure
bash
Copy
Edit
Assets/
├── Animations/            # Character, vehicle, and UI animation clips
│   ├── Characters/
│   ├── Vehicles/
│   └── UI/
├── Audio/                 # Music, sound effects, voiceovers, ambient audio
├── Materials/             # Materials and associated textures (vehicles, environment, UI)
├── Models/                # 3D models (vehicles, environment, characters, cargo)
├── Prefabs/               # Prefab assets for vehicles, characters, environment, UI panels
├── Resources/             # Loadable data assets (JSON for missions, save files)
├── Scenes/                # Unity scene files (MainMenu, Driving, Debrief, etc.)
├── Scripts/               # C# scripts organised by gameplay, UI, systems, managers
├── Shaders/               # Custom shaders (road surfaces, building materials, UI effects)
├── Textures/              # Raw textures categorised by asset type
├── UI/                    # UI elements: fonts, sprites, panel layouts
└── Plugins/               # Third-party SDKs (Mapbox, Photon, Post-Processing)
Getting Started
Prerequisites
Unity Hub and Unity Editor (2021 LTS recommended with URP)

A version control system, such as Git or Plastic SCM (optional)

Mapbox access token (if using the Mapbox SDK)

Photon or Mirror configuration for multiplayer features (if applicable)

Installation and Setup
Clone the repository:

bash
Copy
Edit
git clone https://github.com/YourOrg/EcoWarriorsAfrica.git
cd EcoWarriorsAfrica
Open in Unity Hub:

Click Add → select project folder → Open.

Install packages:

Window → Package Manager → install TextMeshPro, Input System, Cinemachine, Post-Processing, ProBuilder.

Allow restart:

Permit Unity to restart if prompted to switch to the new Input System.

Mapbox setup (if used):

Window → Mapbox → Setup → Paste access token.

Open Prototype scene:

Assets/Scenes/Prototype. Unity to test basic driving and cargo pickup.

Other scenes:

MainMenu, AvatarSelect, MissionHub, Driving, Debrief, Pause, and Settings.

Roadmap and Next Steps
Phase II: Import full city maps (Nairobi, Lagos, Accra, Cape Town) via Mapbox or static OSM meshes.

Phase III: Implement progression systems, vehicle upgrades, and advanced mission types (solar installs, community quizzes).

Phase IV: Add online competitive delivery mode with real-time races and global leaderboards.

Phase V: Deploy to mobile platforms, implement accessibility options, and localise content into multiple languages.

Contributing
Fork the repository and create a new branch for your feature:

bash
Copy
Edit
git checkout -b feature/YourFeatureName
Commit your changes with a descriptive message:

bash
Copy
Edit
git commit -m "Implement new mission flow"
Could you push your branch and create a pull request for review?

Could you ensure the code follows project conventions and includes tests or manual test steps?

License
This project is licensed under the MIT License. See the LICENSE file for details.








