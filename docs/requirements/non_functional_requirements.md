Non-Functional Requirements (NFR)
This document outlines the quality attributes and constraints of the Eco-Delivery Game.

NFR1.0: Performance
NFR1.1: Main Menu Load Time: The game shall load the main menu in less than 10 seconds on devices with 2GB+ RAM.

NFR1.2: Minimum FPS: The game shall run at a minimum of 30 FPS on low-end Android devices.

NFR1.3: Mission Loading Time: Mission loading time shall not exceed 5 seconds.

NFR2.0: Usability
NFR2.1: Input Support: UI shall support both touch and keyboard/mouse inputs (for WebGL).

NFR2.2: Contrast Guidelines: Text labels, buttons, and icons shall follow WCAG 2.1 contrast guidelines.

NFR2.3: Tutorial Self-Sufficiency: Players shall be able to complete the tutorial without external help.

NFR3.0: Scalability
NFR3.1: Concurrent Players: The backend shall support up to 100,000 concurrent players for leaderboard and multiplayer races.

NFR3.2: Modular Content Addition: The system shall allow modular addition of:

New cities

New missions

New characters

Seasonal content

NFR4.0: Portability & Offline Support
NFR4.1: Compatibility: The game shall be compatible with:

Android 10+

Windows/macOS WebGL browsers

NFR4.2: Offline Playability: All core gameplay, tutorial, and missions shall be playable offline.

NFR4.3: Offline Progress Sync: Progress shall be saved locally and synced to cloud storage upon internet detection.

NFR5.0: Security
NFR5.1: Authentication & Storage: User authentication and data storage shall use Firebase security rules.

NFR5.2: Data Encryption: Online player data shall be encrypted during transmission using HTTPS/TLS.

NFR5.3: Score Validation: Leaderboard systems shall validate scores server-side to prevent cheating.

NFR6.0: Reliability
NFR6.1: Uptime: The game shall have an uptime of 99% for online services.

NFR6.2: Crash Recovery: If a crash occurs during gameplay, progress from the last checkpoint shall be restored.

NFR6.3: Autosave Points: Autosave shall occur:

At mission start

At every delivery point

Upon mission completion

NFR7.0: Maintainability & Modularity
NFR7.1: External Data Definition: All missions and vehicles shall be defined in external JSON files.

NFR7.2: Code Principles: Game scripts shall follow SOLID principles for scalability.

NFR7.3: Mission Addition: Developers shall be able to add new missions without recompiling the core game.
