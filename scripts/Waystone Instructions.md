# Waystone Features ✨

- **Custom GUI** showcasing operators' set waypoints in a user-friendly format.
- **Versatile Settings Subpanel** where players can personalize:
    - **Sound Effects**: Choose the effect that plays when selecting a location.
    - **Volume Control**: Adjust the volume of the chosen effect.
    - **Exclusion Page**: Disable specific locations from the main menu to emphasize preferred locations.
    - **Operator-Only Settings**: Allow operators to view or hide all locations from the main interface.
- **Statistics Profile**: Displays the location most frequently visited by the player and total number of travels.
- **Unlimited Waypoints with Paging**: Seamlessly add more waypoints without limitation.
- **Visual Effects**: Beautiful particle effects when selecting a destination.
- **Additional Features**:
    - Persistent main menu page, keeping players in the same spot when they return from settings.
    - Fully customizable waypoints—edit names, descriptions, icons, and locations through the [Waypoints YAML](../waypoints.yml) file.
    - Special message when unlocking a new waypoint.
    - ...

# Waystone Instructions 📃

> [!WARNING]  
> Make sure you have the latest versions of:
> - **Skript**
> - **SkBee**
> - **Skript-GUI**
> - **Skript-Particle**
> - **SkJson**

> This guide will help you set up the [Waystone](Global.Waystone.sk). The term “Waystone” ensures compatibility with other plugins that use `/waypoint`.

1. Install both [Waystone](Global.Waystone.sk) and [LocationEventWaystone](Global.LocationEventWaystone).
2. Adjust the options in the files as desired.
3. Add waypoints to the [Waypoints YAML](../waypoints.yml) file in the following format:
    ```yaml
    unique-id-of-the-waypoint:
        world: world
        x: x
        y: y
        z: z
        name: Unique name for the waypoint (used to sort locations in the script)
        desc: Description
        displayname: Display name for the player (supports MiniMessage)
        icon: Base64 value of the skull texture
    ```
4. **Reload** the script.
5. To use a waypoint in-game, place a purple stained glass block one block below the defined location. This marks the location, triggering the waypoint function when players step on it.\
   For safety, place a beacon under the purple stained glass to avoid accidental waypoint placements. Although the script checks if players are at a waypoint, this original setup method is recommended.

# Todo ❗

- [ ] Permission-based waypoints
- [ ] Command-line functions
- [ ] Additional operator-only settings
- [ ] Rewards for unlocking waypoints
- [ ] Ongoing optimization efforts
- [ ] *(Your suggestions?)*

# Extra Info ℹ️

I'm the author of all scripts in this repository. Feel free to use them as you wish—credit is appreciated but not required.\
A credits screen is included in the Waystone GUI; you’re welcome to replace my information with your own.\
If you need assistance with adding or modifying features, reach out on Discord: $${\color{lightgreen}Hyphonical}$$.

Thank you for using my scripts ❤️. A special thanks to the SkUnity Forum for helping me troubleshoot various challenges—I couldn’t have done it without them 🔥. And a heartfelt shoutout to my friend SnowlyTheShogun, aka Shin, who’s been developing VoidTales for over 10 years. Do him a favor and give him a high-five in his [Discord Server](https://discord.gg/a526aRaMxh)!
