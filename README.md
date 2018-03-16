# Opux
Opux is a Discord bot for EVEOnline

This bot is currently under development and needs to run with dotnet SDK/Runtime. The following guide is a very short setup description. Complete documentation following soon™.

# Features
* Price check tool
* Auth
* Admin Reauth
* Radius Killmails
* Fleetup Operations Post
* MOTD Pulling to channel
* EVE Time Mod

For any further questions contact us on discord:

https://discord.gg/csc7HNM

# Docker

An alternative to installing all dependencies locally is to use Docker Compose. The Docker Compose implementation will build an Opux image, start that as a container and link it with a MariaDB (MySQL) database container through a single command.

```
docker-compose up
```

This implementation requires the existence of a settings.json file in the same directory as you run the command from that it maps into the Opux container. It will also map a logs directory that contains all the log information normally generated by Opux. Finally, it utilizes a Docker volume and healthcheck for cross-platform compatibility and controlled startups, respectively.
