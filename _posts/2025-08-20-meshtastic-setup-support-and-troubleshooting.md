---
layout: post
title: "🛟 Troubleshooting and Setup Help"
date: 2025-08-01
categories: [help]
---

The best away to get help is to ask in the Discord #advice channel.

**🔰 GETTING STARTED WITH MESHTASTIC (WICHITA EDITION)**
Here’s how to get started:
⸻

📱 1. INSTALL THE MESHTASTIC APP
You’ll use this app to connect your phone to your device and manage settings.

For iPhone:
[App Store Link 🔗](https://apps.apple.com/us/app/meshtastic/id1586432531)

For Android:
[Google Play Link 🔗](https://play.google.com/store/apps/details?id=com.geeksville.mesh&hl=en)

⸻

📡 2. CHOOSE YOUR DEVICE

You’ll need a LoRa device (aka a “node”) to send messages on the mesh.

🔰 Easiest Option (No setup needed) **SenseCAP T1000-E**
* [Amazon](https://a.co/d/9HS9Cs6)
* [Seeed Studio](https://www.seeedstudio.com/SenseCAP-Card-Tracker-T1000-E-for-Meshtastic-p-5913.html)

✅ Pocket-sized, GPS built-in, USB-C charging

❌ No screen

⸻

🛠️ DIY Options (More powerful, needs flashing)

**T-Beam (LilyGo)**
* [Amazon](https://a.co/d/fkwSuVV)
* [lillygo](https://lilygo.cc/products/t-beam?variant=44907400167605)

✅ Long range, built-in GPS

❌ Requires flashing

**T-Echo (LilyGo)**
* [Lillygo](https://lilygo.cc/products/t-echo-lilygo?variant=44875726291125)
* [Amazon](https://www.amazon.ca/LILYGO-Wireless-Meshtastic-Development-NRF52840/dp/B0B658DZ9Z?th=1)

✅ GPS, screen, microphone

❌ Higher power draw, also needs flashing

**HELTEC V3**
* [Heltec (be sure to choose the 902-928MHz band)](https://heltec.org/project/wifi-lora-32-v3/)
* [Amazon](https://a.co/d/gh2j6nh)

✅ Budget option, screen

❌ No GPS (or DIY GPS), limited range, needs flashing

✅ DEVICE QUICK COMPARISON

| Device                         | GPS | Screen | Flashing | Use Case               |
|---------------------|-----|--------|----------|------------------------|
| SenseCAP T1000-E | ✅  | ❌     | ✅ Yes  | Beginners, plug-n-play |
| WisMesh Tag | ✅  | ❌     | ✅ Yes  | Beginners, plug-n-play |
| T-Beam (LilyGo)        | ✅  | ❌     | ✅ Yes   | Range + GPS node       |
| T-Echo (LilyGo)         | ✅  | ✅     | ✅ Yes   | Voice & visual testing |
| HELTEC V3                 | ❌  | ✅     | ✅ Yes   | Cheap test or relay    |
| RAK wireless WisBlock Meshtastic Starter Kit | ❌  | ❌     | ✅ Yes   | Super low power for solar installs    |


⸻

💻 3. FLASH YOUR DEVICE (if needed)

Use the web flasher:
[https://flasher.meshtastic.org](https://flasher.meshtastic.org)
Use Chrome or Edge only (not Firefox)
* Plug in via USB
* Choose the correct board
* Hit “Flash”
Need help? Ask in Discord or wait for a flash party!

⸻

⚙️ 4. RECOMMENDED SETTINGS

Use these so your node can communicate with others in the Wichita network!

📻  Radio Config:
Device
- Role: Client (or Client Mute)

LoRa
- Region: US
- User Preset: On
- Modem: LongFast

Position
- GPS: ✅ Enabled (if supported by device)

Channels
Primary
- Name: LongFast (just like that, no space)
- Pre-Shared Key: AQ==
  - then select "8 bit" or "Default"

🧩 Config -> Module Config -> MQTT:
- Enabled: ✅ Yes (helps meshmap.net, don't change the defaults)
- Encryption Enabled: ❌ No
- Root topic: msh/US/KS/Wichita
- Map Reporting Enabled: ✅ yes

Identity Settings (top left, pencil icon):
* Long Name: This is your choice! Make it something unique and memorable.
* Short Name: This is up to you, too! 
⸻


🙋 NEED HELP?
* Ask questions in Discord
* Hop on Sundays at 8pm to join the Mesh Net
* Let us know you want to have flash night or range test meetup!

Let us know what brought you here or what you’re excited to build—we’re building together!

