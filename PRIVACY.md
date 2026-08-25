# TunnelMint privacy information

Last updated: 2026-08-17

This document describes TunnelMint 1.0.0 for macOS.

## Data handling

TunnelMint currently has no analytics, advertising, tracking, account system, or cloud synchronization. The app does not collect or send product-usage telemetry to the developer.

- VPN profile metadata is stored locally on the Mac.
- Passwords, group secrets, private keys, and protected imported configurations are stored in the macOS Keychain.
- VPN traffic is processed locally by Apple's Network Extension framework and by the VPN server selected by the user.
- TunnelMint does not operate the selected VPN server. The server operator's privacy terms and logging practices apply independently.
- An optional endpoint test contacts only the server selected by the user to validate network/TLS availability. It does not send the VPN username or password.
- User-selected `.conf`, `.ovpn`, `.mobileconfig`, `.pcf`, and `.pbk` files are read only when the user chooses to import them.

## Permissions

TunnelMint requests Network Extension permission to create VPN tunnels. If launch at login is enabled, macOS also manages TunnelMint as a Login Item. These permissions remain visible and controllable in System Settings.

## Retention and deletion

Deleting a profile in TunnelMint removes that profile's locally stored metadata and associated Keychain material. Users should delete profiles before uninstalling if they want the app to remove its stored Keychain entries. macOS may preserve Keychain items when an application bundle is deleted directly.

## Support and privacy questions

Use the [public issue tracker](https://github.com/LilaQ/TunnelMint-issues/issues) only for questions that contain no confidential information. Do not publish credentials, keys, certificates, configuration files, or private network details.

For confidential security reports, use GitHub's private vulnerability reporting flow described in [SECURITY.md](SECURITY.md). Publisher identity and any additional contact details required for a selected storefront or territory are provided through the applicable store listing.
