# Changes

## 1.1.0 beta 2

Security fixes: please update.

### Security

- "Maximum protection" could be bypassed: traffic sent from the port of
  an allowed service (such as DNS or HTTPS) reached any port of the
  computer. Rules that allow a service now let in only its replies.
- Rules blocking a port (file sharing, BeShare…) now also stop others
  from connecting to that port on this computer, not only this computer
  from connecting to others.
- A malformed packet could put a few bytes of kernel memory into the
  list of blocked packets. Fixed.

### Fixed

- Right after installing, Mose says that a restart is needed (with a
  "Restart now" button) instead of "kernel read error".
- The trial no longer ends at once on computers that start with the
  clock at 1970 until they get the network time.
- `mose_firewall_ctl history` shows the latest entries, not the oldest.

### Changed

- The registration page receives the system Mose runs on (Haiku
  revision, architecture, Mose version), for the seller's statistics.

## 1.1.0 beta 1

First public release.

### New

- Free, with registration: every installation starts with a 10-day
  trial with all the features; a free registration keeps them (Pro: up
  to 64 rules, unlimited profiles, the Connections window,
  notifications, the list of blocked packets, the full Deskbar menu).
  Without registering, the Base edition keeps filtering with up to 10
  rules and one profile of your own. The licence never turns the filter
  off.
- Five ready-made profiles: No filtering, Home network, Work network,
  Public network, Maximum protection.
- Rules for incoming, outgoing or both directions, for IPv4, IPv6 or
  both.
- A new Statistics tab: packets inspected and blocked, allowed traffic,
  activity of the last two minutes, and the blocked packets with the
  rule that blocked them.
- A clear protection status, in the window and on the Deskbar icon:
  green only when every active network is really filtered.
- The router lights of the icon follow the traffic and turn red when a
  packet is blocked.
- Pause the filter from the Deskbar menu.
- The Deskbar icon comes back by itself after an update or a crash of
  the Deskbar.
- Dark theme, small screens (1024×600), eight languages.
- Packages for 64-bit and 32-bit x86, ARM, ARM64 and RISC-V Haiku.

### Security

- Rules can no longer be bypassed with IP fragments or IPv6 extension
  headers.
- The kernel add-on checks every request coming from programs more
  strictly.
