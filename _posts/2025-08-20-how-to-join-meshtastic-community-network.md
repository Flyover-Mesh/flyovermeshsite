---
layout: post
title: "🛠 Get Connected: How to Join Flyover Mesh"
date: 2025-08-20
categories: [meshtastic, community]
---

Before you buy anything, you can start by [joining the Discord](https://flyovermesh.org/about/#join-the-discord) and ask any questions you might have.

The best away to get help is to ask in the Discord #advice channel.

### 🔰 GETTING STARTED WITH MESHTASTIC (WICHITA EDITION)
Here’s how to get started:
⸻

📱 1. INSTALL THE MESHTASTIC APP
You’ll use this app to connect your phone to your device and manage settings.

For iPhone:
[App Store Link 🔗](https://apps.apple.com/us/app/meshtastic/id1586432531)

For Android:
[Google Play Link 🔗](https://play.google.com/store/apps/details?id=com.geeksville.mesh&hl=en)

⸻

### Choosing your hardware
The community keeps a list of devices up to date, including recomendations and various features. Buying from the links on this site help support the community nodes.

📡 2. CHOOSE YOUR DEVICE

You’ll need a LoRa device (aka a “node”) to send messages on the mesh. Take a look at the [recomended hardware from the community](https://flyovermesh.org/posts/meshtastic-setup-support-and-troubleshooting/#meshtastic-devices).

⸻
### Setting up your hardware

💻 3. FLASH YOUR DEVICE (if needed)

Use the web flasher:
[https://flasher.meshtastic.org](https://flasher.meshtastic.org)
Use Chrome or Edge only (not Firefox)
* Plug in via USB (make sure you're using a USB cable that can transfer data)
* Choose the correct serial port 
* Hit “Flash”
    * Note: For some devices (RAK Wireless), you drag and drop the firmware like you're adding it to a USB drive

Need help? Ask in Discord or wait for a flash party!

⸻

⚙️ 4. RECOMMENDED SETTINGS

Use these so your node can communicate with others in the Wichita network!

📻  Radio Config:

LoRa
- Region: US
- User Preset: On
- Modem: LongFast

Identity Settings (top left, pencil icon):
* Long Name: This is your choice! Make it something unique and memorable.
* Short Name: This is up to you, too! 

Device
- Role: Client (or Client Mute)

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

⸻

### Try out your connections
There are many options!
- 🤖 Send a message on Long Fast, and then check the #mesh-map channel on Discord. If your measage appears there, then it's been sent across the mesh.
- 🎙️ send the message `$ping` or `$hello` or `$weather` and Flyover Mesh Bot will respond to you if it gets your message
- 💬 The simplest way is to wait a momemnt, and see if your app says "Acknoledged" below your message. That's the simplest way to see if your at least communicating with some other nodes.

### Join the Mesh Net events
Each week, we have a scheduled time to send and receive messages. We call that a Mesh Net, which comes from ham radio communities. [Sunday at 8pm.](https://flyovermesh.org/posts/meshtastic-events-and-meetups-calendar/#weekly-mesh-net)