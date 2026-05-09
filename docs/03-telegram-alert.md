# Telegram Alert Integration

This document explains how to configure Telegram notifications for Uptime Kuma.

---

# Create Telegram Bot

Open Telegram and search:

```text
BotFather
```

---

# Create New Bot

Run command:

```text
/newbot
```

Follow instructions and save:
- Bot Token
- Bot Username

---

# Get Chat ID

Method:

1. Start conversation with your bot
2. Send any message
3. Open browser:

```text
https://api.telegram.org/bot<BOT_TOKEN>/getUpdates
```

4. Find:

```json
chat:
  id: 123456789
```

Save the Chat ID.

---

# Configure in Uptime Kuma

Navigate to:

```text
Settings → Notifications → Telegram
```

---

# Fill Required Fields

| Field | Value |
|---|---|
| Bot Token | Your Telegram Bot Token |
| Chat ID | Your Telegram Chat ID |

---

# Test Notification

Click:

```text
Test
```

If successful, Telegram will receive notification messages.

---

# Example Notification

```text
[DOWN] MikroTik Router

Heartbeat failed for monitor:
Router Gateway
```

---

# Recommended Alerts

Recommended monitored services:
- Router
- SSH server
- Web server
- NAS
- Internet connection
