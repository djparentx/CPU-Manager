Simple CPU Manager 2.0

Lightweight system management script for ArkOS based handhelds
Created by djparent
Derived from ArkOS Manager by @lcdyk

Overview

- Simplified and focused version of ArkOS Manager
- Removes non essential modules for a cleaner experience
- Designed for quick access to performance tuning features

Features

- GPU frequency management with formatted MHz display
- CPU governor selection applied across all cores
- CPU max frequency control with sorted frequency list
- ZRAM management with preset profiles based on system RAM
- Optional persistence for CPU settings across reboots
- Automatic ZRAM service creation and persistence

Improvements over ArkOS Manager

- Streamlined menus with reduced complexity
- Removed CPU core toggling and per core targeting
- Removed USB modeswitch and Bluetooth modules
- Added settings persistence via systemd service
- Added automatic ZRAM autostart service
- Improved readability with formatted frequency output
- Safer dialog handling without strict script exit behavior
- Cleaner user flow with fewer nested menus

Localization

- Multi language support based on EmulationStation settings
- Includes English French Spanish Portuguese Italian German Polish

Input and UI

- Gamepad support via gptokeyb
- Dialog based interface optimized for TTY display
- Custom font and display handling for handheld screens

Requirements

- Root privileges auto elevates with sudo
- dialog
- systemd
- gptokeyb optional for controller input

Notes

- Designed for RK3326 based handhelds and similar devices
- Directly interacts with sysfs for CPU and GPU control
- Persistence features write to /etc and create systemd services
