# Operations

## Service Control
- Status: `openclaw status` and `systemctl status openclaw-gateway`
- Start: `openclaw gateway start`
- Stop: `openclaw gateway stop`
- Restart: `openclaw gateway restart`
- Reload: manual input needed if a separate reload flow exists

## Logs and Diagnostics
- Main logs command: `openclaw logs --follow`
- OpenClaw status command: `openclaw status`
- OpenClaw health command: `openclaw health --json`
- Security audit command: `openclaw security audit --deep`
- Update status command: `openclaw update status`
- Other useful diagnostics: `ss -ltnp`, `df -h /`, `free -h`

## Routine Tasks
### Update
1. Run `openclaw update status`.
2. Confirm backup or snapshot exists.
3. Update using the existing pnpm-managed install path, then re-run `openclaw status` and `openclaw security audit --deep`.

### Restart after config change
1. Validate changed config file paths under `/root/.openclaw/`.
2. Run `openclaw gateway restart`.
3. Verify with `openclaw status` and a live channel check.

### Incident response
1. Confirm access path still works.
2. Check service status.
3. Check logs.
4. Check recent config or package changes.
5. Roll back or restore if needed.
