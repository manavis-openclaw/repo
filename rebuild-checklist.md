# Rebuild Checklist

## Phase 1: Base Server
- [ ] Provision server
- [ ] Apply OS updates
- [ ] Set timezone
- [ ] Create admin user if needed
- [ ] Set up SSH keys
- [ ] Confirm remote access
- [ ] Configure firewall

## Phase 2: Network and Domain
- [ ] Recreate DNS records
- [ ] Recreate proxy / tunnel settings
- [ ] Confirm public reachability if needed

## Phase 3: OpenClaw
- [ ] Install runtime dependencies
- [ ] Install OpenClaw
- [ ] Restore config files
- [ ] Restore data files
- [ ] Configure startup service
- [ ] Start gateway
- [ ] Verify status
- [ ] Verify integrations

## Phase 4: Validation
- [ ] Run OpenClaw security audit
- [ ] Run update status check
- [ ] Confirm messaging channels work
- [ ] Confirm scheduled jobs work
- [ ] Confirm logs are clean

## Phase 5: Backup and Handover
- [ ] Re-enable backups
- [ ] Verify backup completion
- [ ] Update this repository with any rebuild changes
