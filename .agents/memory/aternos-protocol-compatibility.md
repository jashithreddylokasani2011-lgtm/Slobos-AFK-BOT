---
name: Aternos protocol compatibility
description: Compatibility constraint between the Aternos server protocol and the Mineflayer client stack.
---

The bot should pin a Mineflayer-supported client version when an Aternos server advertises a newer Minecraft version; ViaVersion on the server can bridge the connection.

**Why:** The server can advertise a version newer than the latest Mineflayer release, causing automatic version negotiation to fail before login.

**How to apply:** Check the supported Mineflayer version before changing the bot's client version. Keep the server-side ViaVersion requirement documented and verify with the live workflow logs.