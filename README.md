# CharacterTracker

This is an open-source project that intends to collect real-time player statistics for the current server you are on while playing the online multiplayer game World of Warcraft.

## Description

Activision Blizzard, the sole owner and provider of the game service, has deemed it necessary to hide all available information on current player numbers. They decided to stop providing information about player numbers after their numbers began to plummet in 2015. This project attempts to negate this loss of information, at least by a little bit, by measuring local player activity on a network of clients connected to the game server.

Each game client (a player's currently running .exe file) is allowed to have installed addons that improve their in-game experience. The majority of the work in this project will be the addon code itself, where it will hook certain functions in the .exe file to allow for the collection of data. This sort of data collection is considered fine to perform by Activision Blizzard, as it does not cause any additional server strain. The addon would only be using data that each player's client would have sent to it anyway.

This addon will only work if a large enough portion of the player base is using it. There must be enough data collection to see most online players.

This collected player data, which would consist of character names of nearby players, will be logged to a text file with dates/times as well. This data will then be sent to a central server, which will parse the logs and generate a final output on player counts per game server. This data could then be extrapolated to produce a total subscriber count, or used for many other purposes, including determining faction split or class/race choices.

## Getting Started

To get started in this project, it would be wise to learn how to code in Lua. This is the scripting language that all World of Warcraft addons use. The IDE you use to develop this project could honestly be notepad.exe, but an IDE like ZeroBrane could be useful to you. Lua is not a very difficult language to read or understand, in any case. For code that pertains to the final log parsing, it would be wise to know about regex, sorting algorithms, or just C++ in general in order to contribute. Any IDE you are used to would work fine for this.

## Questions

To better understand how addons work, or for any general questions, you can look [here](https://wowwiki.fandom.com/wiki/WoW_AddOn). For any project-specific questions, feel free to email me, the creator of the project.

## Contributing

Please read [CONTRIBUTING.md](link).