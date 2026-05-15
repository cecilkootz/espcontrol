---
title: 7-inch Waveshare ESP32-S3-Touch-LCD-7
description:
  EspControl on the Waveshare ESP32-S3-Touch-LCD-7 — a 7-inch 800x480 landscape touchscreen with 15 cards, powered by ESP32-S3.
---

# 7-inch Waveshare ESP32-S3-Touch-LCD-7

The **Waveshare ESP32-S3-Touch-LCD-7** is a 7-inch landscape touchscreen powered by an **ESP32-S3** processor. EspControl uses its 800×480 RGB display and capacitive touch panel for a **15-card** home screen.

## Specifications

| | |
|---|---|
| **Screen size** | 7 inches |
| **Resolution** | 800 × 480 |
| **Orientation** | Landscape |
| **Display interface** | RGB |
| **Processor** | ESP32-S3 |
| **WiFi** | Built-in (2.4 GHz) |
| **PSRAM** | Octal |
| **Touch** | GT911 capacitive |
| **Power** | USB-C |

## Card Grid

The home screen uses a **3-row × 5-column** grid, giving you **15 card slots**. Any home-screen card can be turned into a [Subpage](/features/subpages) folder containing up to 14 more cards.

Flexible card sizes are supported: Single, Tall, Wide, and Large.

## Install

Connect the display to your computer with a USB-C data cable, then click the button below.

<EspInstallButton slug="waveshare-esp32-s3-touch-lcd-7" />

For a full walkthrough including WiFi setup and Home Assistant pairing, see the [Install guide](/getting-started/install).

::: tip Backlight control
The stock board exposes a CH422G backlight enable pin, so EspControl can turn the display on and off. Brightness percentages in the shared screen settings map to on/off unless the board is hardware-modified for PWM.
:::

## ESPHome Manual Setup

If you use ESPHome and prefer to compile firmware yourself:

```yaml
substitutions:
  name: "kitchen-screen"
  friendly_name: "Kitchen Screen"

wifi:
  ssid: !secret wifi_ssid
  password: !secret wifi_password

packages:
  setup:
    url: https://github.com/jtenniswood/espcontrol/
    file: devices/waveshare-esp32-s3-touch-lcd-7/packages.yaml
    refresh: 1sec
```

## Where to Buy

- **Waveshare:** [ESP32-S3-Touch-LCD-7](https://www.waveshare.com/esp32-s3-touch-lcd-7.htm)
