<div align="center">

<img src="logo.svg" alt="Omarchy" width="320">

# Omarchy

**English** · [Русский](README.ru.md)

### A keyboard-driven Linux desktop.

Arch Linux · Hyprland · Shell tooling

![Arch Linux](https://img.shields.io/badge/platform-Arch_Linux-7aa2f7?style=flat-square)
![Bash](https://img.shields.io/badge/tooling-Bash-9ece6a?style=flat-square)
![QML](https://img.shields.io/badge/desktop-QML-bb9af7?style=flat-square)
[![MIT](https://img.shields.io/badge/license-MIT-e0af68?style=flat-square)](LICENSE)

[Upstream](https://github.com/omacom/omarchy) · [Official website](https://omarchy.org) · [Manual](#the-omarchy-manual) · [Source map](#source-map)

</div>

Omarchy is a modern, opinionated Linux distribution by **David Heinemeier Hansson and contributors**. It brings together a tiling desktop, terminal tools, themes and an integrated set of setup commands.

**This repository is Igor Kramar's copy of the upstream project.** It is not the official release channel and does not claim feature or release parity with upstream. For installation and current hardware requirements, start at [omarchy.org](https://omarchy.org) and the [official repository](https://github.com/omacom/omarchy).

## Source map

| Directory | Purpose |
|:---|:---|
| [`bin/`](bin/) | Desktop commands and CLI helpers |
| [`config/`](config/) · [`default/`](default/) | Default configuration and assets |
| [`shell/`](shell/) | QML desktop components |
| [`themes/`](themes/) | Desktop color themes |
| [`install/`](install/) · [`migrations/`](migrations/) | System setup and upgrade steps |
| [`manual/`](manual/) | Published end-user documentation |
| [`docs/`](docs/) | Architecture and implementation reference |
| [`test/`](test/) | Automated checks |

## Development

Read the [contribution instructions](AGENTS.md) and [testing reference](docs/testing.md) before changing code. For focused checks, use the existing entry points:

```sh
./test/cli
./test/shell
```

`./test/all` combines those suites; it does not run the graphical acceptance suite. Graphical acceptance runs belong in a disposable VM. Setup scripts and migrations affect the host system and are not a generic project bootstrap command.

## The Omarchy Manual

The manual lives in [`manual/`](manual/), which is its authoritative source. It's
mirrored to [learn.omacom.io](https://learn.omacom.io/2/the-omarchy-manual), where
its screenshots are also hosted.

- [Welcome to Omarchy!](manual/01-welcome-to-omarchy.md)

**The Basics**

- [Getting Started](manual/02-getting-started.md)
- [Coming From Mac or Windows](manual/03-coming-from-mac-or-windows.md)
- [Navigation](manual/04-navigation.md)
- [The top bar](manual/05-the-top-bar.md)
- [Themes](manual/06-themes.md)
- [Hotkeys](manual/07-hotkeys.md)
- [Unified Clipboard & History](manual/08-unified-clipboard-history.md)
- [Reminders](manual/09-reminders.md)
- [Notices](manual/10-notices.md)
- [Text Extraction & Dictation](manual/11-text-extraction-dictation.md)
- [Screenshots & Recording](manual/12-screenshots-recording.md)
- [Toggles, idle & screensaver](manual/13-toggles-idle-screensaver.md)
- [Omarchy CLI](manual/14-omarchy-cli.md)

**The Applications**

- [Terminal](manual/15-terminal.md)
- [Neovim](manual/16-neovim.md)
- [AI](manual/17-ai.md)
- [Development Tools](manual/18-development-tools.md)
- [Shell Tools](manual/19-shell-tools.md)
- [Shell Functions](manual/20-shell-functions.md)
- [TUIs](manual/21-tuis.md)
- [GUIs](manual/22-guis.md)
- [Browsers](manual/23-browsers.md)
- [Commercial apps/services](manual/24-commercial-apps-services.md)
- [Web Apps](manual/25-web-apps.md)
- [Gaming](manual/26-gaming.md)
- [Filling out PDFs](manual/27-filling-out-pdfs.md)
- [Windows VM](manual/28-windows-vm.md)
- [Other Packages](manual/29-other-packages.md)

**Configuration**

- [Updates](manual/30-updates.md)
- [Dotfiles](manual/31-dotfiles.md)
- [Shell plugins](manual/32-shell-plugins.md)
- [Monitors](manual/33-monitors.md)
- [Keyboard, Mouse, Trackpad](manual/34-keyboard-mouse-trackpad.md)
- [Networking](manual/35-networking.md)
- [System sleep](manual/36-system-sleep.md)
- [Hardware authentication](manual/37-hardware-authentication.md)
- [Fonts](manual/38-fonts.md)
- [Backgrounds](manual/39-backgrounds.md)
- [Prompt](manual/40-prompt.md)
- [Branding](manual/41-branding.md)
- [Common tweaks](manual/42-common-tweaks.md)
- [Making your own theme](manual/43-making-your-own-theme.md)

**The Rest**

- [Mac support](manual/44-mac-support.md)
- [Troubleshooting](manual/45-troubleshooting.md)
- [FAQ](manual/46-faq.md)
- [System snapshots](manual/47-system-snapshots.md)
- [Security](manual/48-security.md)
- [Omarchy on...](manual/49-omarchy-on.md)
- [Dual Boot Install](manual/50-dual-boot-install.md)
- [Unattended Installs](manual/51-unattended-installs.md)

## License and credits

[MIT](LICENSE), with the original copyright notice for David Heinemeier Hansson preserved. Upstream authorship and third-party asset notices remain intact. The local repository overview is maintained by Igor Kramar.
