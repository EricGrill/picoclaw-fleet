# picoclaw-fleet PROJECT-STATUS.md

## Current State
Live on GitHub. Initial release with all core scripts and SKILL.md.

## What's Built
- SKILL.md: OpenClaw skill instructions
- scripts/deploy.sh: SSH deploy PicoClaw to remote host
- scripts/dispatch.sh: One-shot task dispatch
- scripts/fleet-status.sh: Fleet health check
- config/picoclaw-fleet.example.json: Fleet config template

## Open Tasks
- Test deploy to darth (192.168.50.57)
- Add support for Docker-based PicoClaw instances
- Add Proxmox VM spin-up integration
- Add ClawHub publish step

## Architecture
OpenClaw reads SKILL.md → runs bash scripts → SSH into fleet hosts → picoclaw agent -m "task"

## Recent Changes
- 2026-02-18: Initial release
