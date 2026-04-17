# Secrets Reference

Do not put actual secret values in this file.
Record only what exists and where it is stored.

## Password Manager Entries
- Entry name: Manabin Server
  - Contains: SSH access details, provider login or emergency console details
  - Owner: manual input needed
  - Rotation notes: update when SSH credentials or provider access changes
- Entry name: Manabin OpenClaw
  - Contains: Discord token, any OpenClaw-related secret material, pairing or integration secrets
  - Owner: manual input needed
  - Rotation notes: update when channel or integration credentials rotate
- Entry name: Manabin GitHub Deploy Keys
  - Contains: private key material for repo access if backed up outside the server
  - Owner: manual input needed
  - Rotation notes: rotate if server is rebuilt from an untrusted state or key exposure is suspected

## Secrets Needed for Rebuild
- SSH private key:
  - Stored in: manual input needed
- GitHub deploy key:
  - Stored in: `/root/.openclaw/workspace/.ssh/github_deploy_key` on server, plus manual backup location needed
- Discord token:
  - Stored in: password manager entry recommended, actual value not recorded here
- Telegram token:
  - Stored in: if unused, mark N/A
- DNS provider token:
  - Stored in: manual input needed
- Other:
  - Stored in: add any provider, proxy, backup, or webhook secrets here by location only
