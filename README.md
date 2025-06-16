# Docker Minecraft Server Implementation (1.21.4)
## With Plugins!
Implementation of the [itzg/docker-minecraft-server](https://github.com/itzg/docker-minecraft-server) image with plugin configurations for EssentialsX and mcMMO. Essentially a "quick-start" for a Minecraft Docker server with some barebones plugins, since most online documentation only refers to mod configuration. This includes RCON from the [itzg/docker-rcon-web-admin](https://github.com/itzg/docker-rcon-web-admin) repository.

### Notes:
- Plugin configurations are handled downstream by the generated plugin files - **if you don't want to use any particular configuration or prefer the default implementation, just delete the files and the jar will repopulate them. Plugins are mounted from /plugins folder, not from papermc/plugins**.
- If you are not familiar with SQL databases, please look up relevant tutorials and secure your database. [LuckPerms has a page for this topic](https://luckperms.net/wiki/Installation). The password set by this configuration is **NOT** secure.

### Plugins:
- ChatColor2
- [Chunky](https://modrinth.com/plugin/chunky)
- Clearlagg
- [Dynmap](https://modrinth.com/plugin/dynmap) 
- [EssentialsX](https://modrinth.com/plugin/essentialsx):
  - Core
  - Chat
  - Spawn
- [LuckPerms](https://modrinth.com/plugin/luckperms)
- mcMMO
