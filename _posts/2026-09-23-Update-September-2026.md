---
title: "State of the Mesh: September 2026"
date: 2026-09-23
description: "A field report on Flyover Mesh after 17 months of growth."
tags: ["update", "community", "metrics"]
---

# State of the Mesh: September 2026

A field report on where we stand.

## By the Numbers

| Metric | This Month | Total |
|--------|------------|-------|
| Nodes Online Now | 31 | |
| Active Nodes (7 days) | 114 | |
| Active Nodes (30 days) | 213 | |
| Total Nodes Ever Seen | | 724 |
| New Nodes This Month | 30 | |
| Messages Delivered (30d) | 336 | |
| Active Links (30d) | 833 | |
| Active Relays (7d) | 27 | |

## The Spark

In April 2025, I put up a [Reddit post](https://www.reddit.com/r/wichita/comments/1k1q6kb/starting_a_meshtastic_community_in_wichita/) asking if anyone in Wichita was interested in Meshtastic. Got 60 upvotes and 17 comments. That launched a [Discord](https://discord.gg/5h93pEjTcz) with zero members and a city with zero mesh infrastructure. Just a handful of us with scattered nodes, wondering if anyone else was out there.

Seventeen months later: 724 nodes have shown up on this network. 213 were active in the last 30 days. 31 are online right now. The Discord reached 248 members. We went from "is anyone out there?" to a mesh that reaches over 100 miles.

Longest confirmed direct mesh link ([CSKS](https://map.flyovermesh.org/nodes.html?node=!e15d0e46) to [cbot](https://map.flyovermesh.org/nodes.html?node=!849c32d8)) covers 26 miles in a single hop. Messages typically travel about 2.3 hops to get where they're going, passed along by 27 active relays.

## People, Not Just Hardware

Every community node started as a conversation. Someone with roof access who said yes. A neighbor who wanted to help out. I talked to the Wichita Amateur Radio Club and came away with new people joining the mesh and new leads on tower sites.

Members share tools, lend antennas, help each other debug weird firmware issues. The [Discord](https://discord.gg/5h93pEjTcz) isn't just tech support. People post placement photos, celebrate first contacts, coordinate group orders. The mesh grew because people kept showing up and pitching in.

## The Backbone Pulls Its Weight

[Buffalo](https://map.flyovermesh.org/nodes.html?node=!2ec125de), one of our first [community nodes](https://flyovermesh.org/posts/meshtastic-local-node-directory/), forwarded 3,487 packets last week. [Panther One](https://map.flyovermesh.org/nodes.html?node=!2ae00a0f) topped the relay board at 4,359. Ten nodes carry most of the traffic. Every one of them exists because someone asked a friend, and that friend said "yeah, you can put that on the roof."

Of the 178 nodes with neighbors, 127 (71%) can reach three or more other nodes. When one drops, messages route around it. The average node hears 8.4 others.

## Bots Make the Mesh Measurable

We took open source software and heavily edited it. That created our bots (fl0v, HYDD, cbot, and HYDB) which respond to commands. They confirm whether your message got through. They send a response to check if you can receive it. They feed data into a centralized database to generate our [coverage maps](https://map.flyovermesh.org), based on real data from the mesh only, no MQTT. The #mesh-map channel on [Discord](https://discord.gg/5h93pEjTcz) shows you which bots heard you.

Without bots, you're hoping. With them, you're testing. They've become how we diagnose dead spots, prove coverage, and figure out what's actually working.

You can see the data at [map.flyovermesh.org](https://map.flyovermesh.org) and a [full field report](https://map.flyovermesh.org/infographic.html).

## The Three-Layer Problem

Most newcomers buy one node. But one node often means frustration: you turn it on, see nothing, and wonder if the thing is broken.

The mesh has three layers:

1. **Pocket nodes** – Small, battery-powered, what you carry around.
2. **Neighborhood nodes** – Mid-height stuff. Rooftops, second-story windows, attic vents. These connect pockets to backbone.
3. **Backbone nodes** – High solar-powered community placements on towers and tall buildings.

We've got a solid backbone. We've got plenty of pocket nodes. What's thin is the middle. Too many personal nodes only reach the high community sites, not each other.

If you're getting into this, buy three: two pocket nodes (one for you, one for someone you know) and a neighborhood node to stick on your roof. You'll have someone to talk to on day one, and you'll be filling the gap that makes everything else work better. Check out our [recommended devices](https://flyovermesh.org/posts/meshtastic-recomended-devices/) for options at different price points.

## Challenges

- **Weather:** Storm damage knocked out several community nodes this spring. We're still working through repairs.
- **Link quality:** Median quality sits at 33%. Most links are marginal. Average SNR across all links is -20.9 dB. More height and better antennas would help.
- **Mid-layer gaps:** Strong backbone, weak middle. Too many personal nodes are isolated or one hop from nothing.


## What We're Working On

- **More community nodes:** Buffalo, Blackbear, John C. Woods, Bluestem, Hattie, Earhart, Silvasauras, Glenn Nyberg, and others now form a named layer of shared infrastructure. See the full list in our [node directory](https://flyovermesh.org/posts/meshtastic-local-node-directory/).
- **Bot coverage:** fl0v, HYDB, and others keep expanding. More bots means better visibility into what's actually happening on the mesh.
- **Meetups:** We had our first one earlier this year, another shortly after. Planning an outdoor one before the weather turns.

## MeshCore Trial

There's been a lot of conversation in the broader mesh community about MeshCore and how it handles city-scale networks differently than Meshtastic. The short version: MeshCore uses a different approach to routing and node roles that some say works better as meshes grow past a certain size.

We're not abandoning Meshtastic. But we want to understand the tradeoffs before we hit scaling problems we can't solve.

A few of us have started running MeshCore nodes alongside our Meshtastic gear. If you're curious, want to run a test node, or just want to follow the discussion, join **#meshcore** on [Discord](https://discord.gg/5h93pEjTcz). We're looking for volunteers who want to help us figure out what works and what doesn't.

## Get Involved

New to Meshtastic? Start here:

- [How to Join Flyover Mesh](https://flyovermesh.org/posts/how-to-join-meshtastic-community-network/)
- [Recommended Devices](https://flyovermesh.org/posts/meshtastic-recomended-devices/)
- [Discord](https://discord.gg/5h93pEjTcz) (ask questions in #advice)

Purchases through our affiliate links help fund community node hardware and maintenance.