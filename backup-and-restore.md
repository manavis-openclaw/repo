# Backup and Restore

## What Must Be Backed Up
- OpenClaw config files: `/root/.openclaw/openclaw.json` and supporting non-secret config files under `/root/.openclaw/`
- Data directories: `/root/.openclaw/`
- System service definitions: any OpenClaw-related systemd unit or drop-in files, if present
- SSH-related config: host SSH config and authorized key setup needed for admin access
- App-specific state: device pairing metadata and approval state under `/root/.openclaw/`
- Other critical files: this maintenance repo and any external reverse proxy config, if used

## Backup Locations
- Primary backup destination: manual input needed
- Secondary backup destination: manual input needed
- Snapshot provider: manual input needed
- Retention policy: manual input needed

## Restore Notes
- Minimum items needed for recovery: SSH access path, OpenClaw config and data directory, messaging integration secrets from password manager
- Restore order:
1. Re-establish server access and base OS settings.
2. Restore OpenClaw files and service configuration.
3. Restore secrets from the password manager, then verify status and integrations.

## Verification
- Last successful backup check: manual input needed
- Last restore test: manual input needed
- Notes: If no snapshot process exists yet, that should be set up early because this host appears to be a single VPS running the active assistant gateway.
