
# One Mic

A Discord bot built with Python that helps organize voice conversations by allowing one person to speak at a time.

One Mic uses Discord's voice moderation features to mute other participants when someone takes the mic and unmute them when the mic is released.

![One Mic Discord Bot](one-mic.jpg)

## Technologies

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![discord.py](https://img.shields.io/badge/discord.py-5865F2?style=for-the-badge&logo=discord&logoColor=white)
![Discord API](https://img.shields.io/badge/Discord_API-5865F2?style=for-the-badge&logo=discord&logoColor=white)
![python-dotenv](https://img.shields.io/badge/python--dotenv-3776AB?style=for-the-badge&logo=python&logoColor=white)

## Features

- Manage speaking turns in Discord voice channels
- Mute other participants when someone takes the mic
- Unmute participants when the mic is released
- Check whether the user is connected to a voice channel
- Provide command feedback through Discord text channels

## Commands

| Command | Description |
|---------|-------------|
| `!takemic` | Mutes other participants in the user's current voice channel |
| `!releasemic` | Unmutes participants in the user's current voice channel |

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/AnwarAlshohatee/one-mic.git
cd one-mic
```

### 2. Install Dependencies

Requires Python 3.

```bash
python -m pip install discord.py python-dotenv
```

### 3. Configure Your Discord Bot

1. Visit the [Discord Developer Portal](https://discord.com/developers/applications).
2. Create an application and add a bot.
3. Generate your bot token.
4. Enable the **Message Content Intent** and **Server Members Intent**.
5. Invite the bot to your server with the required permissions, including **Mute Members**.

### 4. Set Environment Variables

Create a `.env` file in the project directory:

```env
DISCORD_TOKEN=your_discord_bot_token
```

Never commit your bot token to GitHub.

### 5. Run the Bot

```bash
python one_mic_bot.py
```

Once the bot is connected, join a voice channel and use its commands in a Discord text channel.


## Current Limitations

- Commands do not currently require moderator permissions.
- The bot must have permission to mute and unmute members.
- Speaking queues and automatic turn rotation are not implemented.
- The bot must remain running to respond to commands.

## Future Improvements

- Add moderator-only command permissions
- Implement a speaking queue
- Add automatic speaking-turn management
- Improve permission checks and error handling

## Author

**Anwar Alshohatee**

[Portfolio](https://anwaralshohatee.netlify.app) | [LinkedIn](https://www.linkedin.com/in/anwaralshohatee/)
