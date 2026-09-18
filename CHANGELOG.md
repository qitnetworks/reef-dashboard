# Releases

## 0.3.1 — Windows beta hotfix

- The Windows launcher starts in English regardless of the Windows display language.
- Subsequent startup and stop messages use the language saved in application settings.
- Tablet connection help explains DHCP reservations and reconnecting after an IP change, in all five languages. Verified that pairing codes use the computer's LAN address and reject localhost / loopback addresses.
- Existing aquarium data and access settings are preserved. Linux / Docker stays on 0.3.0; this fix affects only the Windows launcher.

## 0.3.0 — Beta

- Guided setup and tablet pairing by QR code.
- Standalone Windows x64 package; Linux amd64 Docker package.
- Five interface languages and a customizable aquarium name.
- Six themes with distinct animations and a light-effects mode.
- Read-only device monitoring, water-test journal, import/export and backups.
- Configurable slideshow, display thresholds and in-app reminders.

Tested with isolated Windows installation and Docker recreation, including persistence of settings, theme and journal data. Compatibility with every physical device/firmware combination has not been verified. Windows launcher is not digitally signed. No automatic updater, push notifications or cloud backup in this beta.
