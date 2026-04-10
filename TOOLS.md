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

## Saved Commands

### SSH Tunnels

- Local forward 18789 → remote 127.0.0.1:18789
  - `ssh -N -L 18789:127.0.0.1:18789 ali@100.96.143.87`

---

Add whatever helps you do your job. This is your cheat sheet.

### OpenClaw model switch

- Local command script: `scripts/switch-model`
- Quick use:
  - `scripts/switch-model codex`
  - `scripts/switch-model opus`
  - `scripts/switch-model status`
- Optional install to PATH:
  - `chmod +x scripts/switch-model`
  - `sudo ln -sf /home/ali/.openclaw/workspace/scripts/switch-model /usr/local/bin/switch-model`
