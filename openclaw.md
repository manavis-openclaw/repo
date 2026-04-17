# OpenClaw

## Install and Runtime
- Install method: pnpm
- Installed version or channel: 2026.4.15, stable channel
- Running user: root
- Working directory: /root/.openclaw/workspace
- Data directory: /root/.openclaw
- Config file locations: /root/.openclaw/openclaw.json and related files under /root/.openclaw/
- Startup method: systemd

## Gateway
- Gateway status command: `openclaw status`
- Gateway bind address: ws://127.0.0.1:18789, loopback only at capture time
- Remote URL: not confirmed from file inspection, status showed local gateway only
- Node pairing status: node service not installed, device pairing files exist under /root/.openclaw/devices/
- Companion app usage: manual input needed

## Integrations
- Enabled channels: Discord
- Enabled plugins: memory-core noted in status output
- Cron jobs / scheduled tasks: none reported in status output
- External dependencies: Discord token configured, GitHub deploy key configured for notes repo

## Notes
- Safe update procedure: run `openclaw update status`, then update via the existing pnpm-managed install path after backup or snapshot
- Known quirks: Control UI insecure auth toggle is enabled, and security audit reports open Discord group policy with elevated and runtime tools exposed
- Last verified date: 2026-04-17
