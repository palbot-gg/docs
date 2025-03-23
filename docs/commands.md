# Palbot Commands

## Getting Started
> Commands for adding your server to the bot.

| Command | Description | Permission |
|---------|-------------|:-:|
| `/setup` | Gives you a basic setup guide for utilizing the bot. | `Server Admin` |
| `/addserver` | Lets you add your Palworld server to the bot. | `Server Admin` |
| `/removeserver` | Lets you remove your Palworld server from the bot. | `Server Admin` |
| `/reset` | Wipe all information the bot stores about your guild and game server. | `Server Admin` |

## User Commands
> Commands available for regular use.

| Command | Description | Permission |
|---------|-------------|:-:|
| `/paldeck` | Search the paldeck for information on Pals in Palworld. | `User` |
| `/breed` | Select a Pal and find all potential breeding combinations. | `User` |
| `/reversebreed` | Select two Pal parents to find their offspring | `User` |
| `/skills` | Select a Pal to view all potential skills as it levels up. | `User` |
| `/items` | Search the paldeck for information on Items in Palworld. | `User` |
| `/locate` | Shows the spawn locations of Pals. | `User` |
| `/passives` | Look up different passive skills in the database. | `User` |
| `/buildings` | Look up buildings available in Palworld. | `User` |

## Palcon Commands
| Command | Description | Permission |
|---------|-------------|:-:|
| `/palcon command` | Execute a custom RCON command on the server. | `Server Admin` |

## PalAPI Commands
| Command | Description | Permission |
|---------|-------------|:-:|
| `/palapi kick` | Kick a player from the server. | `Server Admin` |
| `/palapi ban` | Ban a player from the server. | `Server Admin` |
| `/palapi unban` | Remove a ban from a player. | `Server Admin` |
| `/palapi announce` | Send a server-wide broadcast. | `Server Admin` |
| `/palapi shutdown` | Shutdown the server safely. | `Server Admin` |
| `/palapi stop` | Stop the server immediately. | `Server Admin` |
| `/palapi save` | Save the current server state. | `Server Admin` |

## Query Commands
| Command | Description | Permission |
|---------|-------------|:-:|
| `/query setchannel` | Setup an online/offline status message for your server. | `Server Admin` |
| `/query removechannel` | Remove the status message from the database. | `Server Admin` |
| `/playermonitor addchannel` | Setup a player join/leave logs for your server. | `Server Admin` |
| `/playermonitor removechannel` | Remove the monitoring channel for a server | `Server Admin` |

## RestAPI Commands
| Command | Description | Permission |
|---------|-------------|:-:|
| `/livemap` | Generate a live map image of players on the server. | `Server Admin` |
| `/guildmap` | Generate a live map of all active bases on the server. | `Server Admin` |
| `/serverinfo` | Fetch server information from your server's REST API. | `Server Admin` |
| `/playerlist` | Fetch a list of players on your server | `Server Admin` |