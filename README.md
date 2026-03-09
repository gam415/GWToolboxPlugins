# GWToolboxPlugins

Download the DLLs from the [Releases](https://github.com/gam415/GWToolboxPlugins/releases) page.

## AoeIndicator

Draws a circle on the ground showing the active AoE of tracked skills.
Only draws for skills cast in specific maps, while your character matches a configured profession combo.

- Pre-defined tracked skills: Meteor Shower and Lava Font.
- Per-skill enable/disable toggle.
- Per-skill custom color and fill override.
- Profession combo filter: only draws when your primary/secondary profession matches.
- Configurable per-map (only activates on listed explorable areas, or all if list is empty).

> Note: Detection is based on the `PlayEffect` server packet, which fires at the exact ground position of the AoE effect.
> The plugin tracks skill activations to associate effects with the correct skill.

### NameObfuscator

Replaces your character name (and optionally your party members' names) with fake names
everywhere on screen: party list, target indicator, chat messages, NPC dialogs, speech bubbles, and inventory header.

- Custom or randomly generated name for your character.
- Randomize party members' names with unique generated names per player.
- Guild tag override: set a custom or random tag.
- Favorites list for saving preferred random names and tags.
- Floating indicator icon showing obfuscation state (active, pending, or disabled).
- Chat commands: `/obfuscate on` and `/obfuscate off`.

> Note: Name changes take effect on the next map load. Guild tag changes take effect immediately.

## PartyReorder

Automatically reorders party members by kicking and re-inviting them in a predefined order based on their professions. Designed for organized speedclear groups.

- Reorder party slots by primary/secondary profession via UI button or /reorder chat command.
- Ships with default sequences for common speed clears (DoA, UWSC, SooSC, etc.).
- Full sequence editor: create, edit, and delete custom sequences with per-outpost configuration.
- Validates party composition before reordering (correct professions, party size, leader status).
- Configurable action delay, timeout, and invite retries.
- Optional chat notifications on start, when party is ready, and when all members are ticked.

## SafeShadowWalk

Prevents accidental Shadow Walk usage when protective buffs are low by placing a colored overlay over the skill icon.
Configurable monitoring for Shadow Form, Shroud of Distress, or any other buff with a minimum time threshold.

- Customizable minimum buff duration threshold (1-30 seconds).
- Monitor any combination of buffs by skill ID.
- Configurable explorable areas.
- Optional click-blocking with warning messages showing exact remaining time.

> Note: This plugin only blocks mouse clicks, not keyboard shortcuts.

## WeaponRangeIndicator

Displays a colored overlay indicating whether your current enemy target is within weapon range for Spears and Flatbows.

- Shows a green or red rectangle based on whether the target is in range.
- Supports Spear and Flatbow range.
- Accounts for altitude differences in range calculations.
- Customizable in-range and out-of-range colors.

> This plugin is based on the FlatbowRangeIndicator plugin by @JaborGW.
