# Rig Ball ESPHome Firmware

ESPHome firmware for Spotpear Ball v2 with OpenClaw integration.

## Hardware
- **Device**: Spotpear Ball v2 (ESP32-S3)
- **Display**: GC9A01A 240x240 round LCD
- **Audio**: ES8311 codec + I2S speaker/mic
- **Touch**: CST816 capacitive

## Quick Flash (No Compile Needed)

### Option 1: Web Flasher (Easiest)
1. Go to https://weemadscotsman.github.io/rig-ball-esphome/
2. Connect your Ball v2 via USB
3. Click "Connect & Flash Firmware"

### Option 2: Download & Flash Manually
1. Go to **Actions** tab → **Build Rig Firmware** workflow
2. Download `rig-ball-firmware` artifact
3. Go to https://esphome.github.io/esp-web-tools/
4. Upload and flash the firmware.bin

## Setup

1. **Edit `secrets.yaml`** with your WiFi credentials (before building)
2. **Push to GitHub** to trigger build
3. **Download firmware** from Actions tab
4. **Flash via web** or esptool

## Features
- Wake words: "Hey Jarvis", "Okay Nabu"
- Animated face (Gwen avatar)
- Touch + button control
- Battery monitoring
- Connects to Home Assistant → OpenClaw
