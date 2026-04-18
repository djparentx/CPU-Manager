# Simple CPU Manager

v2.1 by djparent 

Derived from ArkOS Manager by @lcdyk

---

## Overview

A lightweight system management tool for the R36S, designed to simplify performance tuning by focusing only on essential CPU, GPU, and memory controls.

This script removes unnecessary complexity from ArkOS Manager and provides a fast, controller-friendly interface for managing system performance.

---

## Features

- GPU frequency management with formatted MHz display  
- CPU governor selection applied across all cores  
- CPU max frequency control with sorted frequency list  
- ZRAM management with preset profiles based on system RAM  
- Optional persistence for CPU settings across reboots  
- Automatic ZRAM service creation and persistence  
- Multi-language support (EN, FR, ES, PT, IT, DE, PL)  
- Clean, controller-friendly menu interface  

---

## Improvements Over ArkOS Manager

- Streamlined menus with reduced complexity  
- Removed CPU core toggling and per-core targeting  
- Removed USB modeswitch and Bluetooth modules  
- Added persistent CPU settings via systemd service  
- Added automatic ZRAM autostart service  
- Improved readability with formatted frequency output  
- Safer dialog handling without strict script exits  
- Cleaner user flow with fewer nested menus  

---

## CPU & GPU Controls

### CPU

- Set governor (performance, ondemand, etc.) across all cores  
- Adjust maximum CPU frequency using a sorted list  
- Optional persistence across reboots  

---

### GPU

- Adjust GPU frequency with readable MHz values  
- Simple selection interface for quick tuning  

---

### ZRAM

- Enable and configure compressed RAM (ZRAM)  
- Uses preset profiles based on system RAM  
- Automatically creates and enables systemd service for persistence  

---

## Persistence

- Optional CPU settings persistence via systemd  
- ZRAM configuration automatically persists across reboots  
- Writes configuration to system directories (e.g., /etc)  

---

## Input and UI

- Gamepad support via gptokeyb  
- Dialog-based interface optimized for TTY display  
- Custom font handling for handheld screens  

---

## Installation

1. Copy the script to your R36S Tools folder  

2. Run it

---

## Requirements

- R36S running ArkOS or dArkOS  
- Root privileges (auto-elevates with sudo)  

Required tools:

- dialog  
- systemd  
- gptokeyb (optional, for controller input)  

---

## Notes

- Designed for RK3326-based devices like the R36S  
- Directly interacts with sysfs for CPU and GPU control  
- Safe to re-run without breaking existing configuration  

---

## Credits

- Original ArkOS Manager by @lcdyk  
- Simplified and enhanced version by djparent  

---
