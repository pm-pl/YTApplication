# YTApplication — PocketMine Plugin for YouTube Partnership Application

**YTApplication** is a PocketMine-MP plugin that lets Minecraft players apply for a YouTube Partnership role **directly from in-game commands**. The plugin forwards applications to a Discord channel where admins can review and approve them.

---

## Features

* Players use `/ytapplication` in-game to apply for YouTube Partner role.
* Application message automatically posts to a specified Discord channel.
* Simplifies the application process for YouTube partnerships tied to your Minecraft server.
* Easy configuration of Discord webhook/channel and Minecraft plugin settings.

---

## Requirements

* **PocketMine-MP** server (compatible version with your plugin)
* PHP 8.x (as required by PocketMine-MP and plugin)
* A Discord server with a channel dedicated for receiving applications
* Discord Bot Token or Webhook URL for posting messages (depending on plugin design)
* Composer (for dependencies if any)

---

## Installation

1. **Download the plugin `.phar` file** or clone the repository to your PocketMine `plugins/` folder.

2. **Configure the plugin:**

   * Open the `config.yml` inside the plugin folder after the first run.
   * Set the Discord webhook URL or bot token and channel ID where applications should be sent.
   * Configure any role IDs or messages as needed.

3. **Restart your PocketMine server** to load the plugin.

---

## Usage

* In Minecraft, players run the command:

  ```
  /ytapplication
  ```

* This sends their application info automatically to your designated Discord channel.

* Admins on Discord can then review and approve applications via Discord.

---

## Configuration Example (`config.yml`)

```yaml
discordWebhookUrl: "https://discord.com/api/webhooks/your-webhook-url"
applicationChannelId: 123456789012345678
adminRoleId: 987654321098765432
```

---

## Development & Customization

* Modify the plugin code in `src/` to customize the messages, commands, or Discord integration method.
* Make sure to comply with PocketMine plugin development guidelines.

---

## Support

* For help, open an issue in this repository or contact me on Discord.

---

## License

MIT License
