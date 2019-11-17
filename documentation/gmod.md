# Garry's Mod Server

## General

`steamcmd` is the management tool for steam servers and is required for installation and operation of the server files.

It can be installed with `sudo apt-get install steamcmd`

## Regular Operation

The server process can be invoked via `~/server_1/srcds_run -game garrysmod +maxplayers 24 +map ttt_minecraft_b5 +gamemode terrortown +host_workshop_collection 1832062262 -authkey C1F891FC373F78A028545EDC2D974E88;` where:
  
- `~/server_1/srcds_run` is the server program
- `-game garrysmod` is the game
- `+maxplayers 24` is the max players
- `+gamemode terrortown` is ttt
- and `+host_workshop_collection 1832062262 -authkey C1F891FC373F78A028545EDC2D974E88` is the workshop collection id and API authkey of the owner's steam account

## Updates

- `steamcmd`
- `login anonymous`
- `force_install_dir /home/cole/server_1`
  - This **CANNOT** be a relative path
    - IE NOT `~/server_1`
- `app_update 4020`
- `app_update 4020 validate`
- `quit`
