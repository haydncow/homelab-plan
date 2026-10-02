# Security Plan

How I plan to keep my homelab secure. I'll update this as I build it and
learn more.

## What I'm protecting against

- Someone accessing my Pi from the internet
- Weak or default passwords being guessed
- Out of date software with known vulnerabilities
- Losing my Pi-hole settings if something breaks

## Remote access

- Use **Tailscale** to access the lab from outside my house
- **No port forwarding** on my router, so nothing is exposed to the internet
- Turn on two-factor authentication (2FA) on my Tailscale account

## Logging in to the Pi

- Set my own username and a strong password when installing the OS
  (using Raspberry Pi Imager)
- Use **SSH keys** instead of passwords
- Once keys work, turn off password login for SSH
- Don't allow logging in directly as root

## Pi-hole

- Set a strong password for the Pi-hole admin page
- Only access the admin page from my home network or through Tailscale
- Keep blocklists updated

## Firewall

- Use **UFW** (Uncomplicated Firewall) on the Pi
- Block everything by default and only allow what's needed:
  - SSH
  - DNS (port 53) for Pi-hole
  - Pi-hole web admin page

## Updates

- Update the Pi regularly
- Turn on automatic security updates (unattended-upgrades)
- Keep Pi-hole and Tailscale updated

## Router

- Change the router's default admin password
- Check the router firmware is up to date

## Backups

- Back up Pi-hole settings using its built-in Teleporter feature
- Keep a copy of my setup notes in this repo so I can rebuild it

## Future improvements

- Get a managed switch and use **VLANs** to separate the lab from my
  other home devices
- Set up Fail2ban to block repeated failed login attempts
- Look at Pi-hole logs to see what my devices are contacting

## Testing

Once it's built, I'll check my security by:
- Scanning the Pi with Nmap from another device to see which ports are open
- Making sure password login over SSH is actually blocked
