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
- Physical 3D MUTE and REPORT buttons
- Report reason buttons are also physical 3D buttons
- Buttons can be pressed using your finger in VR
- PC and mobile players can click or tap the buttons
- Buttons sink when pressed and turn red when active
- Buttons only appear on rows containing other players

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
- Daily Shiny Rocks rewards
- Players receive 100 Shiny Rocks every 24 hours by default
- Daily reward amount can be configured using `DailyCoins` in `Config`
- Daily Shiny Rocks sign displays a countdown until the next reward
- Currency board timer matches each player's personal daily reward timer
- Players staying in-game past 24 hours can still receive their daily reward

> **Note:** The daily reward amount can be changed through `DailyCoins` in the `Config` script.

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
- Supports separate-server and same-server map connections
- Includes example maps for both connection methods

#### Public Map Connect Zones (Green)

To create a public map connection zone:

1. Create a Part where you want players to enter the map.
2. Add the `GTPublicConnect` tag to the Part.
3. Set the `GTMap` attribute to the name of the map lobby you want players to join.
4. Players walking into the zone will be connected to that map's own servers.

#### Same-Server Map Connect Zones (Red)

The original same-server map connection method is still available.

1. Create a Part where you want players to enter the map.
2. Add the `GTPublicConnect` tag to the Part.
3. Set the `GTMap` attribute to the name of the map.
4. Set `GTSameServer = true` on the zone.

This allows players to move between maps without being sent to a separate server.

#### Map Spawns

To configure spawn locations for a map:

1. Create a Part where players should respawn.
2. Add the `GTMapSpawn` tag to the Part.
3. Configure the spawn for the appropriate map.

Multiple spawn locations can be used for a map.

#### Included Test Maps

- **Test Map:** Example of the public map connection system using green zones.
- **Test Map 2:** Example of the original same-server connection system using red zones.

> **Note:** Custom map names are supported without needing to modify any scripts.

### Reports & Webhook Setup

The reporting system supports actual report submissions through Discord webhooks.

- Reports are sent to a configured Discord webhook.
- The `ReportSettings` script controls the webhook URL and spam limits.
- Reports cannot ping Discord users or roles.
- Reports are also printed in the server output.
- Reports include the reporting player's username, display name, User ID and profile link.
- Reports include the reported player's username, display name, User ID and profile link.
- Reports include a Join This Server link.
- Reports include the reported player's User ID for use when banning through the Creator Dashboard.

> **Note:** Configure your webhook and spam limits through the `ReportSettings` script. Keep your webhook URL private and avoid sharing it publicly.

### Developer Tutorials

Step-by-step tutorials are included to help developers set up and customize their Gorilla Tag-inspired games.

All tutorials can be found in:

`ReplicatedStorage > GT > Tutorials`

Available tutorials:

1. **First Setup** - Helps developers get started with the template.
2. **Add a Map** - Explains how to add custom maps.
3. **Reports (Discord)** - Explains how to configure Discord webhook reporting.
4. **Room Codes** - Explains how to set up and use room codes.
5. **Robux Shop (ATM)** - Explains the Robux shop setup.
6. **Cosmetics** - Explains how to set up cosmetics.

> **Note:** These tutorials are intended for developers working with the template and are designed to make setting up and customizing your game easier.

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
- Improved room code server handling
- Fixed REPORT instantly selecting a reason when report reason buttons appear in VR
- Improved lobby board button interactions
- Fixed daily Shiny Rocks not being awarded
- Improved daily reward countdown accuracy
- Improved map connection handling

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
- Daily Shiny Rocks Rewards
- Physical Lobby Board Buttons
- Additional Mirror Functionality
- Developer Setup Tutorials

I plan to continue expanding the template with new features, bug fixes, improvements, and general maintenance.

**This project is an independent continuation of Stormie's original template and is not affiliated with or officially supported by Stormie or Another Axiom.**

**More features and improvements will be added as development continues.**
