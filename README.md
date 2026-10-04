# Resize Players ![Dynamic XML Badge](https://img.shields.io/badge/dynamic/xml?url=https%3A%2F%2Fraw.githubusercontent.com%2FOnys-0%2FResize-Players%2Fmain%2Fpom.xml&query=%2F%2F*%5Blocal-name()%3D'project'%5D%2F*%5Blocal-name()%3D'version'%5D&label=version)
Resize your or other players to your desired height! Allows reach to be affected as well.

## Commands
| Command                        | Description                                                                   |
|--------------------------------|-------------------------------------------------------------------------------|
| `/resizeplayers help`          | View the help menu.                                                           |
| `/resizeplayers reload`        | Reload the configuration file.                                                |
| `/resizeplayers info [player]` | View the height, block reach, and entity reach of yourself or another player. |
| `/resize <blocks> [player]`    | Resize yourself or another player to the specified amount of blocks.          |
| `/resize <blocks> all`         | Resize all players to the specified amount of blocks.                         |

## Permissions
| Permission                          | Description                                                                                      |
|-------------------------------------|--------------------------------------------------------------------------------------------------|
| `resizeplayers.scale.self`          | Allows the player to scale themselves with `/resize <blocks>`.                                    |
| `resizeplayers.scale.others`        | Allows the player to scale other players with `/resize <blocks> <player>`.                        |
| `resizeplayers.scale.all`           | Allows the player to scale all players with `/resize <blocks> all`.                               |
| `resizeplayers.scale.exempt`        | Exempts the player from being scaled.                                                            |
| `resizeplayers.scale.bypass`        | Allows the player to bypass the minimum and maximum scale limit.                                 |
| `resizeplayers.reload`              | Allows the player to reload the plugin with `/resizeplayers reload`.                             |
| `resizeplayers.info.self`           | Allows the player to view their own height, block reach, and entity reach with `/resizeplayers info`. |
| `resizeplayers.info.others`         | Allows the player to view another player's height, block reach, and entity reach with `/resizeplayers info <player>`. |

## [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/) Placeholders
| Placeholder                    | Description                          |
|--------------------------------|--------------------------------------|
| `%resizeplayers_height%`       | The player's height in blocks.       |
| `%resizeplayers_block-reach%`  | The player's block reach in blocks.  |
| `%resizeplayers_entity-reach%` | The player's entity reach in blocks. |

## About this fork

This fork is based on [Sfg246/Resize-Players](https://github.com/Sfg246/Resize-Players) and adds one change:

- **Console support for `/resize`.** `/resize <blocks> <player>` and `/resize <blocks> all` can now be run from the server console, command blocks, or other plugins, so you can script player sizes (for example, from an event or rank-up plugin). `/resize <blocks>` with no target still needs to be run by a player.
