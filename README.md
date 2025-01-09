# vcAfk
VCAFK Plugin Introduction
VCAFK is a robust AFK (Away From Keyboard) management plugin designed for Minecraft servers. It automatically detects when players go AFK and provides flexible features to keep your server organized. With PlaceholderAPI integration, you can easily display AFK information anywhere on your server.

Key Features
Automatic AFK Detection: Players are automatically marked as AFK after being inactive for a configurable duration.
Manual AFK Command: Players can use the /afk command to toggle their AFK status manually.
PlaceholderAPI Support: Provides custom placeholders to display AFK status in other plugins.
Flexible Configuration: Fully customizable AFK durations, messages, and behaviors.
Blindness Effect (Optional): Players entering AFK mode can receive a blindness effect.
Notification System: Other players can be notified when someone enters or exits AFK mode.

Commands
/afk: Allows players to manually toggle their AFK status.
Permission: vcafk.afk
Usage: /afk
/vcafk reload: Reloads the plugin's configuration file.
Permission: vcafk.reload
Usage: /vcafk reload
PlaceholderAPI Placeholders
%vcafk_afk%: Displays the player's AFK status.

If AFK: Shows the value of placeholders.afk from config.yml.
If not AFK:
If placeholders.show-not-afk: true in config.yml, shows the value of placeholders.not_afk.
If placeholders.show-not-afk: false, displays nothing.
%vcafk_afk_time%: Displays the amount of time a player has been AFK in seconds.

Configuration Overview
The plugin comes with a config.yml file to customize its behavior. Below is an important configuration field:

afk-timeout
Purpose: Sets the maximum duration (in seconds) a player can stay AFK before additional actions can be taken (e.g., warnings, automatic server kick).
Example:
afk-timeout: 300 - If a player remains AFK for 5 minutes (300 seconds), the plugin can trigger additional actions.
Other configurations, like auto-afk-timeout, specify how long a player must remain inactive before being marked as AFK.

Installation and Setup
Download and Install: Place the VCAFK.jar file in your server's plugins folder.
Configuration: Edit the config.yml file to adjust AFK timeouts, messages, and effects as needed.
PlaceholderAPI Integration: Ensure PlaceholderAPI is installed, and use %vcafk_afk% or %vcafk_afk_time% placeholders in compatible plugins.
Reload Configuration: Apply changes using the /vcafk reload command.
