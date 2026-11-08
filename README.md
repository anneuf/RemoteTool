<p align="center"><img src="icon.png" width="128" alt="Remote Tool icon"></p>

# Remote Tool – beta

Remote Tool manages remote connections: **SSH** (including old devices that need legacy
algorithms), **Telnet**, **serial consoles**, **RDP** and **VNC**, **SFTP/SCP** file transfer,
**tunnels** and jump hosts, split terminals with broadcast input, an encrypted local vault and a
shared team vault. Connections live in plain-text *collections* that can be shared through Git.

This repository is for the **beta test** (version 0.8.1): downloads and problem reports. The
source code is not published here.

## Download

Get the installer for your system from the
[releases page](https://github.com/anneuf/RemoteTool/releases) (beta versions are marked *Pre-release*):

| System | File | Notes |
| --- | --- | --- |
| Windows 10/11 (64-bit) | `remote-tool_0.8.1_x64-setup.exe` | Installs for your user, no admin rights. The installer is not signed yet: Windows SmartScreen warns – choose **More info → Run anyway**. |
| Debian / Ubuntu / Mint (64-bit) | `remote-tool_0.8.1_amd64.deb` | `sudo apt install ./remote-tool_0.8.1_amd64.deb` (pulls in the dependencies). |
| Any Linux (64-bit) | `remote-tool_0.8.1_amd64.AppImage` | `chmod +x` the file and run it; no installation. |
| macOS 11+ | `remote-tool_0.8.1_*.dmg` (coming soon) | Not signed yet: the first time, **right-click the app → Open → Open**. |

## First steps

1. Start Remote Tool and create a **collection** (a folder for your connections) – or open an
   existing one.
2. Add connections with **New** in the ribbon, or type `user@host` (or `rdp://host`, `serial COM3`)
   into the search box for a quick connection.
3. Store passwords as **credentials** (OS keystore or the built-in vault); connections can share
   them.
4. Press **F1** or use **Help** in the ribbon for the built-in help.

## Reporting problems and ideas

Use **Report** in the app's ribbon (Help group): it copies version and system information and
opens a new [issue](https://github.com/anneuf/RemoteTool/issues/new/choose). Please describe what
you did, what you expected and what happened, and attach the end of the log file if you can (the
app shows where it is under **About**). The log never contains passwords – but please do not post
host names, user names or addresses you consider private.

## Licence

MIT – see [LICENSE](LICENSE).

Checksums: `SHA256SUMS.txt` in the release (`sha256sum -c SHA256SUMS.txt`).
