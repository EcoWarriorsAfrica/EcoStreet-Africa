# EcoWarriors Africa - Functional Requirements

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/ecowarriors/game/releases)
[![Status](https://img.shields.io/badge/status-MVP%20Development-orange.svg)]()
[![Location](https://img.shields.io/badge/location-Nairobi,%20Kenya-green.svg)]()

## 📋 Table of Contents

- [Overview](#overview)
- [Core Gameplay Loop](#1-core-gameplay-loop)
  - [Player Onboarding & Customization](#fr-gl-001-player-onboarding--customization)
  - [Mission Selection](#fr-gl-002-mission-selection)
  - [Driving & Delivery Gameplay](#fr-gl-003-driving--delivery-gameplay)
  - [Scoring & Debrief](#fr-gl-004-scoring--debrief)
  - [Progression & Unlocks](#fr-gl-005-progression--unlocks)
- [Story and Narrative](#2-story-and-narrative)
- [User Interface & Experience](#3-user-interface-ui-and-experience)
- [Online Features](#4-online-features-future-iterations--mvp-optional)
- [System Features](#5-system-features)
- [Contributing](#contributing)
- [License](#license)

## Overview

This document outlines the core functionalities that the **EcoWarriors Africa** game must possess to meet its objectives, particularly focusing on the **Minimum Viable Product (MVP)** scope which will be set in **Nairobi, Kenya**.

> **Note**: This is a living document. Please submit issues or pull requests for any updates or clarifications needed.

---

## 1. Core Gameplay Loop

### FR-GL-001: Player Onboarding & Customization

The system shall allow players to:

- **FR-GL-001.1**: Begin playing as a guest without requiring immediate sign-up
- **FR-GL-001.2**: Opt to sign up for an account to enable online features and cloud saves
- **FR-GL-001.3**: Customize their avatar (boy/girl options)
- **FR-GL-001.4**: Select an initial eco-friendly vehicle:
  - Eco-truck
  - Cargo-bike
  - Solar-van
- **FR-GL-001.5**: Unlock and apply cosmetic eco-decals to their vehicles using in-game currency

#### Implementation Status
- [ ] Guest mode implementation
- [ ] Account registration system
- [ ] Avatar customization UI
- [ ] Vehicle selection screen
- [ ] Decal system

---

### FR-GL-002: Mission Selection

The system shall enable players to:

- **FR-GL-002.1**: Access a "Mission Hub" displaying a City Overlook Map of Nairobi
- **FR-GL-002.2**: View mission pins on the map, color-coded by mission type and difficulty
- **FR-GL-002.3**: Tap on a mission pin to view an info pop-up displaying:
  - Mission distance
  - Reward stars (1-3)
  - Environmental Points (EP) gain
  - A relevant eco-tip

#### Implementation Status
- [ ] Mission Hub UI
- [ ] Nairobi city map integration
- [ ] Mission pin system
- [ ] Info pop-up component

---

### FR-GL-003: Driving & Delivery Gameplay

The system shall provide the core driving simulation experience:

- **FR-GL-003.1**: Allow players to control their chosen vehicle (steering, braking, acceleration)
- **FR-GL-003.2**: Display a fuel gauge and require players to manage fuel consumption
- **FR-GL-003.3**: Present dynamic city streets within Nairobi, including main roads and backstreets

#### Mission Types

- **FR-GL-003.4.1**: **Tree-Planting Runs**: Haul seedlings to designated planting sites
- **FR-GL-003.4.2**: **City Cleanup Runs**: Collect waste bins from various locations and deliver them to a recycling center
- **FR-GL-003.4.3**: **Solar Kit Deliveries**: Transport solar panels to schools or other specified locations

#### Environmental Hazards & Obstacles

- **FR-GL-003.5.1**: Potholes that affect vehicle handling and potentially cause damage
- **FR-GL-003.5.2**: Pedestrians and other AI-controlled vehicles that must be avoided
- **FR-GL-003.5.3**: Collisions that inflict damage to the cargo and/or the player's truck

#### Implementation Status
- [ ] Vehicle control system
- [ ] Fuel management system
- [ ] Nairobi street layout
- [ ] Mission type implementations
- [ ] Hazard system
- [ ] Collision detection

---

### FR-GL-004: Scoring & Debrief

The system shall provide post-mission feedback:

- **FR-GL-004.1**: Calculate a star rating (1-3 stars) for each mission based on:
  - Delivery time
  - Cargo/truck condition at mission completion
  - Fuel efficiency

- **FR-GL-004.2**: Calculate a final score using the formula:
  ```
  Final Score = BaseTimeScore - CollisionPenalties + EfficiencyBonus
  ```

- **FR-GL-004.3**: Display a "Debrief Screen" upon mission completion, including:
  - Infographics showing environmental impact (e.g., CO₂ saved, trees planted, waste diverted)
  - Pop-up facts related to sustainability (e.g., "Driving smoothly can cut emissions by 20%")

#### Implementation Status
- [ ] Scoring algorithm
- [ ] Star rating system
- [ ] Debrief screen UI
- [ ] Environmental impact calculator
- [ ] Sustainability facts database

---

### FR-GL-005: Progression & Unlocks

The system shall manage player progression:

- **FR-GL-005.1**: Track an "EP Meter" that visually represents the city's "EcoHealth" (e.g., clearer skies, greener parks)
- **FR-GL-005.2**: Award "Green Tokens" and Environmental Points (EP) upon successful mission completion
- **FR-GL-005.3**: Allow players to spend Green Tokens on:
  - Vehicle upgrades (e.g., better suspension, larger cargo tanks)
  - Cosmetic skins and eco-decals
- **FR-GL-005.4**: Unlock new city missions, advanced vehicle types, and mentor characters at specific EP milestones

#### Implementation Status
- [ ] EP meter system
- [ ] Token economy
- [ ] Upgrade shop
- [ ] Milestone unlock system

---

## 2. Story and Narrative

### FR-SN-001: Narrative Progression

The system shall expose the story through gameplay and contextual elements:

- **FR-SN-001.1**: Introduce the player as an "EcoWarrior driver" working to combat environmental degradation in Nairobi
- **FR-SN-001.2**: Integrate characters like:
  - **Dr. Kamau** (solar expert)
  - **Esi** (river guardian)
  - Through mission briefings or in-game interactions
- **FR-SN-001.3**: Present environmental challenges (e.g., Pollura Corp's waste dumping) as core mission objectives
- **FR-SN-001.4**: Display educational facts and infographics within debrief screens to tie gameplay actions to real-world environmental impact

#### Implementation Status
- [ ] Character dialogue system
- [ ] Mission briefing framework
- [ ] Educational content database
- [ ] Story progression tracking

---

## 3. User Interface (UI) and Experience

### FR-UI-001: Visual Presentation

The system shall provide a visually engaging interface:

- **FR-UI-001.1**: Display a Splash & Logo Animation upon game launch
- **FR-UI-001.2**: Include animated UI headings throughout the interface
- **FR-UI-001.3**: Implement a parallax hero intro

### FR-UI-002: In-Game Displays

The system shall provide essential information during gameplay:

- **FR-UI-002.1**: A Heads-Up Display (HUD) showing:
  - Steering/braking cues
  - Fuel gauge
  - Mini-map displaying player location and mission objectives (and opponents in competitive mode)
- **FR-UI-002.2**: A first-person camera view during driving segments
- **FR-UI-002.3**: A top-down mini-map view, especially relevant for competitive modes

### FR-UI-003: Navigation and Controls

The system shall facilitate player interaction:

- **FR-UI-003.1**: Provide intuitive controls for vehicle operation (e.g., on-screen buttons, keyboard/gamepad support)
- **FR-UI-003.2**: Allow players to navigate through game menus (e.g., Mission Hub, customization, settings)

### FR-UI-004: Mission Management

The system shall enable effective mission flow:

- **FR-UI-004.1**: Display a "Mission Failed" screen when conditions for failure are met
- **FR-UI-004.2**: Provide a "quick-retry" option on the "Mission Failed" screen

#### Implementation Status
- [ ] Splash screen animation
- [ ] HUD system
- [ ] Camera system
- [ ] Control scheme
- [ ] Menu navigation
- [ ] Mission state management

---

## 4. Online Features (Future Iterations / MVP Optional)

> **Note**: These features are considered for post-MVP but designed for integration

### FR-ONL-001: Competitive Delivery Mode

The system shall support competitive online races:

- **FR-ONL-001.1**: Allow players to join a Race Lobby for matchmaking (2-6 players per race)
- **FR-ONL-001.2**: Conduct a pre-race briefing outlining objectives (deliver cargo, avoid crashes, obey speed limits)
- **FR-ONL-001.3**: Enable real-time competitive races with other players
- **FR-ONL-001.4**: Provide a "Ghost Mode" fallback to race against best local times if real-time opponents are unavailable
- **FR-ONL-001.5**: Display podium results (1st-3rd) and award green tokens and EP based on rank

### FR-ONL-002: Leaderboards

The system shall maintain and display competitive rankings:

- **FR-ONL-002.1**: Present global daily and weekly route challenges
- **FR-ONL-002.2**: Allow players to challenge friends to "Beat my best run!"

### FR-ONL-003: Seamless Synchronization

The system shall manage data across offline and online states:

- **FR-ONL-003.1**: Automatically upload offline progress to cloud saves when an internet connection is established
- **FR-ONL-003.2**: Display a UI badge indicating online (green) or offline (gray) status

### FR-ONL-004: Dynamic Daily Missions

The system shall introduce new content over time:

- **FR-ONL-004.1**: Deliver new daily missions to players when online

#### Implementation Status
- [ ] Multiplayer framework
- [ ] Matchmaking system
- [ ] Leaderboard backend
- [ ] Cloud save system
- [ ] Daily mission system

---

## 5. System Features

### FR-SYS-001: User Settings

The system shall allow players to configure game preferences:

- **FR-SYS-001.1**: Adjust master audio volume, music volume, and sound effects volume
- **FR-SYS-001.2**: Remap control inputs
- **FR-SYS-001.3**: (Potentially) Adjust graphical settings

### FR-SYS-002: Offline Play

The system shall support core gameplay without an internet connection:

- **FR-SYS-002.1**: All driving missions, tutorials, and educational overlays shall be fully accessible offline

### FR-SYS-003: Monetization & Retention Features

The system shall integrate monetization and retention strategies (for future consideration):

- **FR-SYS-003.1**: Enable unlocking cosmetic items and minor convenience features through in-game currency earned by playing
- **FR-SYS-003.2**: Provide daily login rewards tied to climate trivia or eco-tips
- **FR-SYS-003.3**: Integrate future partnership content (e.g., "Real World Eco Heroes" profiles or special missions)

#### Implementation Status
- [ ] Settings menu
- [ ] Offline mode support
- [ ] Monetization framework
- [ ] Daily rewards system

---

## Contributing

We welcome contributions to improve these functional requirements! Please follow these guidelines:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/improvement-name`)
3. **Update** the relevant sections with clear, actionable requirements
4. **Test** your changes for consistency and clarity
5. **Submit** a pull request with a detailed description

### Contribution Guidelines

- Use clear, concise language
- Follow the existing FR-XXX-XXX numbering convention
- Include implementation status checkboxes for new features
- Add appropriate labels and milestones
- Reference related issues where applicable

### Reporting Issues

Found an issue or have a suggestion? Please [create an issue](https://github.com/ecowarriors/game/issues/new) with:

- Clear description of the problem or enhancement
- Steps to reproduce (if applicable)
- Expected vs actual behavior
- Screenshots or mockups (if relevant)

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Last Updated**: June 26, 2025  
**Version**: 1.0.0  
**Status**: MVP Development Phase  
**Location**: Nairobi, Kenya 🇰🇪
