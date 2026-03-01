# TOOLS.md - Local Notes

Skills define _how_ tools work. This file is for _your_ specifics — the stuff that's unique to your setup.

## What Goes Here

Things like:

- Camera names and locations
- SSH hosts and aliases
- Preferred voices for TTS
- Speaker/room names
- Device nicknames
- Anything environment-specific

## Examples

```markdown
### Cameras

- living-room → Main area, 180° wide angle
- front-door → Entrance, motion-triggered

### SSH

- home-server → 192.168.1.100, user: admin

### TTS

- Preferred voice: "Nova" (warm, slightly British)
- Default speaker: Kitchen HomePod
```

## Why Separate?

Skills are shared. Your setup is yours. Keeping them apart means you can update skills without losing your notes, and share skills without leaking your infrastructure.

---

Add whatever helps you do your job. This is your cheat sheet.

## File Editing Caution

When editing large files with sed or similar tools:
- Avoid using ranges with replacement inside braces like /{s|.*|replacement|;} as it replaces each line in the range, causing duplication.
- Use 'c' command for replacing entire ranges: sed '/start/,/end/c
ew content'
- Always backup or use git for version control.
- Test commands on small files first.
- After editing, check file size and content integrity.

This prevents crashes from file corruption.
