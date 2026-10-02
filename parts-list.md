# Parts List

Budget: around £200

Prices checked October 2026. Pi prices have been going up, so I'll check again before buying.

| Part | Why I need it | Where | Price |
|------|---------------|-------|-------|
| Raspberry Pi 5 (2GB) | Runs Pi-hole and Tailscale. Pi-hole is lightweight so 2GB is enough | The Pi Hut | £74.40 |
| DeskPi RackMate T0 (4U, 10 inch) | Holds everything. Comes with a 1U shelf and a blank panel | Amazon UK | £66.49 |
| TP-Link TL-SG105 (5 port gigabit switch) | Connects the Pi and future devices to my router | John Lewis | £17.99 |
| Raspberry Pi 27W USB-C power supply | Official PSU recommended for the Pi 5 | The Pi Hut | £10.90 |
| 32GB microSD card | Storage for the operating system | Various | ~£8 |
| Active cooler for Pi 5 | Keeps the Pi cool inside the rack | The Pi Hut | ~£5 |
| Short Cat6 patch cables (pack of 5) | Tidy connections inside the rack | Amazon UK | ~£7 |

**Estimated total:** ~£190

## Why these choices

- **Pi 5 2GB:** the bigger RAM models cost a lot more and Pi-hole doesn't need them.
- **4U rack:** enough room for a switch, the Pi and space to add more later.
- **Unmanaged switch:** cheap and simple to start with.

## Possible upgrades later

- **Managed switch** (e.g. TP-Link TL-SG105E) so I can set up VLANs and
  separate the lab from my home devices. Good for learning network security.
- **SSD instead of microSD** for better reliability.
- **A second Pi** for running more services.

## Builds I looked at for ideas

- [kevsrobots 10 inch Pi mini rack](https://www.kevsrobots.com/projects/mini-rack/)
- [ServeTheHome RackMate T0 review](https://www.servethehome.com/deskpi-rackmate-t0-4u-10in-rack-mini-review/)
- [Computingforgeeks 10 inch rack build guide](https://computingforgeeks.com/build-10-inch-mini-rack-homelab/)
- r/homelab
