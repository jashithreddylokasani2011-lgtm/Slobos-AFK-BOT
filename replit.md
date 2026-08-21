# Aternos AFK bot

## Run

The project runs with Node.js 20 and starts with:

```bash
npm start
```

The status dashboard listens on port 5000.

## Required environment values

Set these as Replit environment variables before starting the workflow:

- `MC_BOT_USERNAME` — the Minecraft account name used by the bot
- `MC_SERVER_HOST` — the current Aternos server address
- `MC_SERVER_PORT` — the current Aternos server port

Optional values:

- `MC_SERVER_VERSION` — exact client version (defaults to `1.21.11`; use ViaVersion on newer Aternos servers)
- `MC_AUTH_TYPE` — `offline` (default) or `microsoft`
- `MC_BOT_PASSWORD` — only for an authenticated account
- `MC_AUTO_AUTH_PASSWORD` — only when the server's `/register` and `/login` plugin is enabled
- `DISCORD_WEBHOOK_URL` — optional connection notifications

The bot does not start or wake an Aternos server. The server must already be online, and its address/port must match the configured values. Periodic leave/rejoin, chat spam, combat, and risky movement are disabled by default to favor a stable connection.