# Reef Dashboard

**Your aquarium on a dedicated screen. Free to use. Runs in your home.**

[English](#get-started) · [Polski](docs/WINDOWS-PL.md) · [Español](docs/WINDOWS-ES.md) · [Français](docs/WINDOWS-FR.md) · [Deutsch](docs/WINDOWS-DE.md)

Live readings, water tests and equipment status, with a rotating tablet dashboard. Choose your own aquarium name, language, theme and slideshow timings.

## Get started

Open [**v0.3.0 — Beta**](https://github.com/qitnetworks/reef-dashboard/releases/tag/v0.3.0). In **Assets**, download one of these files:

| Your setup | Download | Instructions |
| --- | --- | --- |
| **Windows PC — easiest** | [**Download for Windows**](https://github.com/qitnetworks/reef-dashboard/releases/download/v0.3.0/reef-dashboard-0.3.0-windows-x64.zip) | [Start here](docs/WINDOWS-EN.md) |
| Existing Linux x64 server with Docker | [Download for Linux / Docker](https://github.com/qitnetworks/reef-dashboard/releases/download/v0.3.0/reef-dashboard-0.3.0-linux-amd64.zip) | [Server instructions · 5 languages](docs/SERVER.md) |

**Choose the Windows ZIP if you are unsure.** It includes its own runtime; you do not need Docker or Node.js. Extract the ZIP, open **Start Aquarium.exe**, and follow the assistant. Connect your tablet by scanning a QR code.

GitHub also adds **Source code (zip)** and **Source code (tar.gz)** links automatically. Those contain this documentation repository, **not the application**. Download the named package above.

The Windows computer or server must stay switched on and awake. Android tablets and iPads display the dashboard in their browser; they do not run the server. This is a beta release and the Windows launcher is not digitally signed yet.

## What you get

- Read-only monitoring of supported Red Sea ReefBeat equipment; control remains in ReefBeat.
- Water-test journal, CSV import/export and JSON backups.
- A three-screen slideshow: overview, water tests and equipment.
- Six themes, individual animations and a light-effects mode for older tablets.
- English, Polish, Spanish, French and German.
- Setup assistant, device discovery, tablet pairing, reminders and configurable display thresholds.
- Your own installation name and locally stored aquarium data.

Supported device families: ReefControl Pro, ReefATO+, ReefRun, ReefWave, ReefDose, ReefLED and ReefMat. Local APIs are unofficial; compatibility depends on model and firmware. ReefWave reports its schedule, not measured water flow. Missing live readings are never replaced with demo values.

## Help and updates

Use **Issues** to report a problem or suggest a feature. Include the application version, operating system, device model and steps to reproduce it. Reports in any supported language are welcome. [Support and updates](SUPPORT.md).

## License and source

The application is **free proprietary software**, not open source. This public repository contains documentation and support material; application source stays private. You may use and share unmodified release packages under [LICENSE.txt](LICENSE.txt). Dependencies retain their own licenses; see [third-party notices](THIRD-PARTY-NOTICES.txt).

This is an independent project, not affiliated with or endorsed by Red Sea, ReefBeat or Hanna Instruments.
