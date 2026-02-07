# Keep this file empty (or with only comments) to skip heartbeat API calls.

# Add tasks below when you want the agent to check something periodically.

- Check for new emails: Run `gog gmail search 'newer_than:30m' --max 10 --json`. If the threads array has items, count them and send a message to the user: "You have X new emails in the last 30 minutes: [list subjects and senders]"

- Check upcoming calendar events: Run `gog calendar events m.pelissari@gmail.com --from 2026-02-07 --to 2026-02-08 --json`. If events, send "Upcoming events today: [list summaries and times]"