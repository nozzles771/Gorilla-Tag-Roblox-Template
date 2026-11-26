# Gorilla-Tag-Roblox-Template

A Roblox Studio template designed to help developers create Gorilla Tag-inspired games and fangames. Includes foundational systems and resources to simplify development and provide a starting point for your own projects.

# GTag Roblox Template

## Downloads & Access

You can access the template using either of the following methods:

- **GitHub Download:** Download the `.rbxl` file attached to this repository.
- **Roblox Uncopylocked:** [Open the template on Roblox](https://www.roblox.com/games/114949004916070/GorillaTag-Roblox-Template) and access an editable copy through Roblox Studio.

## ⚠️ Disclaimer

This is an **unofficial, fan-made Gorilla Tag Roblox template**. It is not affiliated with, endorsed by, or sponsored by **Another Axiom**.

All Gorilla Tag models and assets included in this project are the property of **Another Axiom**. This project does not claim ownership of any original Gorilla Tag assets.

Assets and models are based on Gorilla Tag's **House Update** and are not fully updated to the current 2026 version.

## Features

### Player

- Gorilla Tag Player Model
- Working Player Color Codes
- Custom Player Names

### Gorilla Computer

- Gorilla Tag Computer System
- Computer Tabs based on the House Update
- Updated Computer UI across all devices
- Improved Color Changing Interface
- Easier Player Color Customization

> **Note:** The computer interface and tabs are based on the House Update. The newer 2026 computer redesign and additional tabs are not included.

### Game Modes

- Casual
- Infection
- Hunt

### Lobby Leaderboard

- Gorilla Tag-style lobby leaderboard
- Displays all players currently in your room
- Displays Room ID and current Game Mode
- Shows player names and colors
- Player color swatches change to infected/hunted textures when tagged
- Speaker indicators for players currently talking
- Individual MUTE buttons for players
- Mute preferences saved to player profiles
- REPORT interface with Hate Speech, Toxicity and Cheating options
- Reports are submitted through a Discord webhook
- Reports are printed in the server output
- Report submissions cannot ping Discord users or roles
- Configurable webhook and spam limits through the `ReportSettings` script

### Cosmetics

- Working Cosmetic Wardrobe
- House Update Cosmetics
- Thanksgiving Cosmetics
- Christmas Cosmetics
- Default Shop Cosmetics
- Early Access Cosmetics
- Working Cosmetic Try-On Station
- Working Mirror
- Fixed mirror reflections
- Try-on boxes and ATMs display correctly in mirrors
- Optional follow-your-view mirror functionality

> **Note:** To enable follow-your-view functionality, set `GTMirrorFollowView = true` on the mirror glass.

### Currency & Purchasing

- Working Currency System
- Cosmetic Purchasing System
- Persistent Currency Saving
- Saved Cosmetic Purchases

> **Note:** The purchasing system may not be an exact 1:1 recreation of Gorilla Tag's original system, but the functionality is implemented.

### Room Codes

- Room Code System
- Room codes send players into their own actual servers
- Players disconnecting from a code server return to a public server
- Joining a public room from a code server also returns players to a public server
- Studio retains the original room-code behavior for testing

> **Note:** Roblox teleportation does not work normally in Studio. Room codes therefore use their original behavior when testing inside Studio. Actual server transfers work in published games.

### Map Connect Zones & Custom Maps

- Added support for custom map connection zones
- Players can walk into connect zones to join a specific map's lobby
- Supports custom map names without requiring script changes
- Added dedicated map spawn locations
- Connect zones appear see-through green in Studio
- Connect zones are hidden during gameplay
- Includes a Test Map with working connect zones and a spawn point

#### Adding Map Connect Zones

To create a connect zone for your map:

1. Create a Part where you want players to enter the map.
2. Add the `GTPublicConnect` tag to the Part.
3. Set the `GTMap` attribute to the name of the map lobby you want players to join.
4. Players walking into the zone will be connected to that map's lobby.

#### Adding Map Spawns

To configure spawn locations for a map:

1. Create a Part where players should respawn.
2. Add the `GTMapSpawn` tag to the Part.
3. Configure the spawn for the appropriate map.

Multiple spawn locations can be used for a map.

> **Note:** Custom map names are supported without needing to modify any scripts. A Test Map is included in the template to help developers understand how connect zones and map spawns work.

### Reports & Webhook Setup

The reporting system now supports actual report submissions through Discord webhooks.

- Reports are sent to a configured Discord webhook.
- The `ReportSettings` script controls the webhook link and spam limits.
- Reports cannot ping Discord users or roles.
- Reports are also printed in the server output.

> **Note:** Configure your webhook and spam limits through the `ReportSettings` script. Keep your webhook URL private and avoid sharing it publicly.

## Platform Compatibility

This template supports multiple platforms, allowing players to experience the game regardless of their device.

- **PC:** Supported
- **Mobile:** Supported
- **VR:** Supported with working Gorilla Tag-style VR movement
- **Console:** Supported

### Non-VR Movement

Devices that do not support VR use a recreation of **Gorilla Tag Mod Walk Simulator**, providing an alternative movement experience for PC, mobile and console players.

VR players retain the intended Gorilla Tag-style movement system.

## Bug Fixes & Improvements

- Fixed players falling off the map without respawning
- Fixed respawns sometimes placing players back at their previous death or fall location
- Improved respawn reliability
- Updated mobile button sizes and icons
- Improved mobile UI appearance
- Updated Gorilla Computer UI across all devices
- Improved the color-changing interface
- Fixed mirror reflections looking incorrect
- Fixed try-on boxes and ATMs displaying incorrectly in mirrors
- Fixed players getting stuck without a lobby after disconnecting
- Players can rejoin a public lobby by walking away from the computer or entering the lobby zone
- Improved room code server transfers
- General UI refinements and visual improvements

---

## Credits & Acknowledgements

### Original Template

This project originally started as an addition to **Stormie's GTAGMovementKit**. The original template served as the foundation for this project.

Full credit goes to **Stormie** for creating and providing the original template.

### Independent Development

With permission from Stormie, I have continued developing and updating this template independently. Stormie considered the original template finished, but I felt there was still more potential for additional features, improvements, and functionality.

So far, my own additions include:

- Cosmetic Purchasing System
- Working Cosmetic Mirror
- Cosmetic Try-On Functionality
- Bug Fixes and Errors Found in Stormie's Template and Scripts
- Updated Mobile UI
- Updated Gorilla Computer UI
- Improved Color Changing Interface
- Lobby Leaderboard
- Player Mute Functionality
- Functional Discord Webhook Reporting
- Improved Room Code System
- Map Connect Zones and Custom Map Support
- Map Spawn System
- Additional Mirror Functionality

I plan to continue expanding the template with new features, bug fixes, improvements, and general maintenance.

**This project is an independent continuation of Stormie's original template and is not affiliated with or officially supported by Stormie or Another Axiom.**

**More features and improvements will be added as development continues.**
