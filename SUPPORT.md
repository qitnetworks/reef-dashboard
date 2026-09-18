# Support and updates

## Before reporting a problem

Use the latest release, then describe what happened and what you expected. Include your Windows/Linux version, browser, tablet model, application version and equipment model/firmware where relevant. Issues are public: do not include passwords, pairing QR codes/links, database backups or unredacted logs.

## Updating

Download a JSON backup from **Data & backups** first. On Windows, extract the new Windows ZIP and run **Start Aquarium.exe** under the same Windows account; the installer preserves that account’s existing application data. On a server, follow the maintenance section of [the server guide](docs/SERVER.md), preserving the existing configuration and data volume.

This beta does not automatically download or install updates. Check **Releases** for new versions and read their notes before updating.

## Device not found

Check that the device is online in ReefBeat and that the computer and device can communicate on the home network. Guest Wi-Fi and separate networks may require network configuration. Use the assistant’s advanced options to provide a known address. Do not reset pumps or change aquarium settings just to troubleshoot the dashboard.

## Package integrity

Each release includes SHA256SUMS.txt for its downloadable ZIPs. On Windows, `Get-FileHash -Algorithm SHA256 -LiteralPath "path-to-downloaded-file.zip"` prints a checksum to compare with that file. A matching checksum verifies the file matches the release; it does not replace a publisher signature.
