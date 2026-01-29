---
layout: post
title: "🛟 Troubleshooting and Setup Help"
date: 2025-08-01
categories: [help]
---

## Meshtastic Devices

✅ [MESHTASTIC DEVICE QUICK COMPARISON can be found here.](https://flyovermesh.org/posts/meshtastic-recomended-devices)

### What settings do I need to join the mesh?
See the how-to guide: [🛠 Getting Connected](https://flyovermesh.org/posts/how-to-join-meshtastic-community-network/)

### How can I test if my node is working?
The Flyover Mesh is lucky! We have serveal ways to verify that you're sending messages on the mesh.

1. Any message received by Flyover Mesh Bot or Frood Bot will be posted to the #mesh-map channel in Discord. Send a short message, and check the channel.
2. Flyover Mesh Bot will reply to messages that you send. Try sending `$ping` or `$coinflip` on the Long Fast channel, and be sure to include the $. If the bot receives your message, it will respond. You can test your transmit (tx) by checking #mesh-map on Discord (see the 1.), and test your receive (rx) by waiting to receive a message back from Flyover Mesh Bot.
3. Least helpful is to look for the little, grey "Acknowledged" text under your message. That means your message was received and some node send an ACK that your node received back.

### What Mode should my node be in?
Choose Client mode as a default. If you're installing your own node in a high place, then Client Base may be a good choice. Any other setting should be chosen only by someone who isn't reading an FAQ page 🔬

### My messages say "Max retransmission reached." Why?
You tried to send a message, but your node can't tell you for sure that the messge has been received by another node.

After attempting to send, nodes wait for an acknoledgement message (or ACK) from another node. This lets you know that your message was transmitted, **and** that it was received. When your node does not receive an ACK, your messages will show this notice.

This message does not mean your message was not received it, but that your node didn't receive confirmation that it was received, which is essential for 2-way communication.

If you keep getting these messages, see "How can I test if my node is working?"