Functional Requirements (FR)
This document details the core functionalities the Eco-Delivery Game must implement.

FR1.0: User Authentication & Account Management
FR1.1: Sign-in Options: The game shall allow players to either:

Sign in using email and password (via Firebase Auth).

Play as a guest with temporary local storage.

FR1.2: User Profile Creation: The system shall securely create a unique user profile containing:

User ID

Avatar and vehicle customization

Mission progress

Tokens and EP

FR1.3: Guest Data Merging: If a guest player later creates an account, the system shall merge the guest data with the new account.

FR1.4: Progress Saving & Sync: Player progress shall be saved locally and automatically synced to cloud storage (Firebase Firestore) when an internet connection is detected.

FR2.0: Avatar & Vehicle Customization
FR2.1: Avatar Customization: Players shall select their avatar gender, skin tone, and outfit from a set of predefined assets.

FR2.2: Starter Vehicles: Players shall choose one starter vehicle (Eco-Truck, Cargo Bike, or Solar Van), each with:

Different speed, fuel efficiency, and cargo capacity stats.

FR2.3: Unlocking Customization: Players shall unlock vehicle upgrades and cosmetic eco-decals using Green Tokens earned during gameplay.

FR2.4: Customization Accessibility: Customization shall be accessible from the main menu and Mission Hub.

FR3.0: Mission System & Map Navigation
FR3.1: City Overlook Map: The game shall provide an interactive "City Overlook Map" displaying available missions using icons.

FR3.2: Mission Color-Coding: Missions shall be color-coded by type (e.g., Green = Tree Planting, Yellow = Waste Pickup).

FR3.3: Mission Details: Each mission shall have:

A title and description

Difficulty level (Easy/Medium/Hard)

EP reward estimate

FR3.4: Mission Unlocking: Upon completing a mission, a new mission or storyline segment shall unlock.

FR4.0: Driving Mechanics & Environment Simulation
FR4.1: Vehicle Physics Simulation: The game shall simulate vehicle physics including:

Acceleration, deceleration, and turning

Basic collision detection with dynamic damage

FR4.2: Control Schemes: Players shall use on-screen steering buttons or tilt controls (if enabled).

FR4.3: Obstacle Rendering: The game shall render obstacles such as potholes, pedestrians, traffic cones, and vehicles.

FR4.4: Obstacle Impact: Hitting obstacles shall:

Reduce cargo integrity

Increase time penalties

Trigger visual feedback (e.g., flashing red screen)

FR4.5: Fuel Consumption & Depletion: Vehicles shall consume fuel over time. If fuel is depleted before delivery:

Mission fails

Player is prompted to retry with upgraded fuel tank if applicable

FR5.0: Mission Scoring & Feedback
FR5.1: Summary Screen: After each mission, the game shall display a summary screen showing:

Time taken vs. target time

Cargo condition (percentage undamaged)

Fuel consumed

Stars earned (1-3)

FR5.2: Scoring Formula:

Final Score = BaseTimeScore – CollisionPenalties + EfficiencyBonus

FR5.3: Mission Failure Handling: If the mission fails (cargo destroyed, fuel depleted, time exceeded), the game shall:

Display a “Mission Failed” screen

Offer a quick-retry button

Suggest upgrade tips if applicable

FR6.0: Economy & Game Progression
FR6.1: Currency Types: Players shall earn two forms of currency:

Green Tokens – for cosmetic and functional upgrades

Environmental Points (EP) – for citywide progress and unlocking new areas

FR6.2: City Evolution: The city shall visually evolve with accumulated EP (e.g., parks become greener, smog clears).

FR6.3: EP Milestones: Certain missions or vehicles shall require EP milestones to unlock.

FR7.0: Online Competitive Features
FR7.1: Online Mode: Online mode shall allow players to:

Compete in timed delivery challenges

See real-time leaderboards by city, country, or global

FR7.2: Competitive Scoring: Competitive scoring shall include:

-5 seconds penalty for minor infractions (e.g., clipping a cone)

-15 seconds penalty for major violations (e.g., hitting pedestrians)

Bonus for 100% fuel-efficient run

FR7.3: Player Rank Display: Player rank shall be displayed as a badge next to their name.

FR8.0: Tutorial & Onboarding
FR8.1: Tutorial Drive: First-time players shall be directed to a “Tutorial Drive.”

FR8.2: Tutorial Coverage: Tutorial shall cover:

Steering, braking, fuel awareness

Route selection

Cargo pick-up/drop-off interaction

FR8.3: Full Game Unlock: Tutorial completion shall unlock full game map.
