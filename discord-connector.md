# Discord connector
Discord connector is a plugin for San Andreas Multiplayer (SA-MP). It allows you to control a Discord bot within your Pawn script.

# How to use it on an open.mp server

## Creating a Discord bot
First thing we are going to do is create a Discord bot. How do we do that? Head over to [Discord Developer Portal](https://discord.com/developers/applications) and click on "New Application"

After you clicked that, enter the name you want the bot to have:</br>
![New Application](https://i.imgur.com/5YTtI9x.png)</br>
Agree to the ToS and DP and click "Create".

Now click on the sidebar and go to the "Bot" section.</br>
![Bot](https://i.imgur.com/RYUc68w.png)

Make sure to enable every Intent.</br>
![Intents](https://i.imgur.com/vfrqOzo.png)

And now you have created a Discord bot! 

## Bot token
To copy your bot token. Click on "Reset Token"</br>
![token](https://i.imgur.com/B9fxBtN.png)

And then copy.

## Configuration
Download the open.mp pre-release version from [here](https://github.com/maddinat0r/samp-discord-connector/releases/tag/v0.3.6-pre).

Extract the contents of the download, put the .inc file in your `qawno/include` folder. And the plugin file (.dll or .so) into the **COMPONENTS** folder. 

Now open up your Pawn script and include it as follows and compile your script.
```c
#include <discord-connector>
```

Edit your configuration file (config.json) as follows:
```json
   "discord": {
      "bot_token": "your_bot_token_here"
   }
```

Please do not share your token with anyone.

## Start
You can now start the server, your bot should be online. If you encounter any issues please let Mido know.