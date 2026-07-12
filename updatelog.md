# multiblox update log
**maskware 2020 - 2026**

## v1.0 - 12/07/2026
**initial release**

### multiple instance launching
- bypasses roblox's single instance lock by remotely closing `ROBLOX_singletonEvent` inside running roblox processes
- each instance authenticates via a auth ticket from the roblox api (no registry cookie injection used)
- option to manually close singleton event(s)

### account manager
- cookies stored in `accounts.json` are obfuscated with xor + base64
- checks if a cookie is valid, invalid or expired
- account list supports dragging to reorder

### profile page
- launch selected account independent
- launch into set gameid (optional)
- view headshot, robux, followers, place visits and join date of accounts
- view cookie (hidden by default)

### launch all
- launch all accounts at the same time
- launch into set gameid (same server) (optional)
- skips invalid & expired accounts
