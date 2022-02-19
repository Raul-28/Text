# Discord GEN-BOT

## Badges
![GitHub last commit](https://img.shields.io/github/last-commit/blazsmaster/discord-gen-bot?style=for-the-badge)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/blazsmaster/discord-gen-bot?style=for-the-badge)
![GitHub issues](https://img.shields.io/github/issues/blazsmaster/discord-gen-bot?style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/blazsmaster/discord-gen-bot?style=for-the-badge)
![GitHub Repo stars](https://img.shields.io/github/stars/blazsmaster/discord-gen-bot?style=for-the-badge)
![GitHub watchers](https://img.shields.io/github/watchers/blazsmaster/discord-gen-bot?style=for-the-badge)
![GitHub](https://img.shields.io/github/license/blazsmaster/discord-gen-bot?style=for-the-badge)
![GitHub package.json dependency version (prod)](https://img.shields.io/github/package-json/dependency-version/blazsmaster/discord-gen-bot/discord.js?style=for-the-badge)

## Installation
Install all dependencies:
```
$ npm install
```

### Configuration
Before you try to start the bot, you need to complete the `config.json` file in the main folder.

#### Default
```json
{
    "token": "",
    "prefix": "gen!",
    "genChannel": "",
    "genCooldown": "1000",
    "color": {
        "green": "0x57F287",
        "yellow": "0xFEE75C",
        "red": "0xED4245",
        "default": "0x5865F2"
    },
    "command": {
        "notfound_message": true,
        "error_message": true
    }
}
```
- `token`: Your discord bot's token
- `prefix`: Your bot's command prefix *(for example: !help | ?help | gen!help)*
- `genChannel`: Forced channel for `gen` command
- `genCooldown`: Cooldown between two executions of `gen` command *(use milliseconds)*
- `notfound_message`: Sends a message to the channel if the message starts with the prefix but does not exists
- `error_message`: Sends a message to the channel if an error occured and this setting is "true"

You can change the `green`, `yellow`, `red` and `default` colors to another hex colors.

---

## How it works?

### Adding account/data
Add an account or a data with the `add` command. The space character in the data parameter make the write wrong.
- Example: `add example_service abcd`
- Wrong example: `add example_service abcd` ~~`efg hijk`~~ <-- the last 2 arguments are not stored

---

### Account/data generating
You can add account to the bot using `gen` command.
- Example: `gen example_service`

---

### Creating service
Create a service with `create` command.
- Example: `create example_service`

### Check service stock
Check the stock folder's content.
- Example: `stock`

### Check command list
List bot commands.
- Example: `help`
