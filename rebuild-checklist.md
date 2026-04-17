# Rebuild Checklist

## Phase 1: Base Server
- [ ] Provision Ubuntu server
- [ ] Apply OS updates
- [ ] Set timezone to Asia/Tokyo
- [ ] Create admin user if needed, or explicitly decide to keep root-only admin access
- [ ] Set up SSH keys
- [ ] Confirm remote access on port 22
- [ ] Configure firewall

## Phase 2: Network and Domain
- [ ] Recreate DNS records
- [ ] Recreate proxy / tunnel settings
- [ ] Confirm public reachability if needed

## Phase 3: OpenClaw
- [ ] Install runtime dependencies for the pnpm-managed OpenClaw setup
- [ ] Install OpenClaw
- [ ] Restore config files under `/root/.openclaw/`
- [ ] Restore data files under `/root/.openclaw/`
- [ ] Configure startup service
- [ ] Start gateway
- [ ] Verify `openclaw status`
- [ ] Verify Discord integration and any companion device pairing needed

## Phase 4: Validation
- [ ] Run `openclaw security audit --deep`
- [ ] Run `openclaw update status`
- [ ] Confirm messaging channels work
- [ ] Confirm scheduled jobs work
- [ ] Confirm logs are clean
- [ ] Confirm OpenClaw is still loopback-only unless intentional external exposure is configured

## Phase 5: Backup and Handover
- [ ] Re-enable backups
- [ ] Verify backup completion
- [ ] Update this repository with any rebuild changes
