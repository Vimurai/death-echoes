<div align="center">

# 👻 DEATH ECHOES

**Your death, replayed as a ghost.**

[![Latest Release](https://img.shields.io/github/v/release/Vimurai/death-echoes?style=for-the-badge&label=Download&color=1f9c8f&labelColor=0a0e14)](../../releases/latest)
[![Minecraft](https://img.shields.io/badge/Minecraft-1.21.11%20%2F%2026.2-1f9c8f?style=for-the-badge&labelColor=0a0e14)](../../releases/latest)
[![Server](https://img.shields.io/badge/Server-Paper-1f9c8f?style=for-the-badge&labelColor=0a0e14)](../../releases/latest)
[![Java](https://img.shields.io/badge/Java-25%2B-1f9c8f?style=for-the-badge&labelColor=0a0e14)](../../releases/latest)

</div>

---

Death doesn't end anything on this server — it leaves a trace.

**Death Echoes** silently records the last **10 seconds** before a player dies:
just their positions, a few hundred tiny data points. The moment they die,
that trail is sealed into an echo tied to the spot they fell.

Walk near that spot later — as anyone, anytime — and the last 10 seconds
play back as a ghost: a glowing, faded figure retracing the exact steps that
led to a death. If a mob did the killing, it shows up too — a creeper
swells and pops, a skeleton draws and fires — faded, muted, and completely
harmless to anyone actually standing there.

## What you get

- 👻 **Real death replays** — not a message, not a marker: the actual last
  10 seconds, walked out in front of you.
- 💀 **The killer shows up too** — creepers detonate (harmlessly), archers
  fire a real arrow, other mobs appear where they must have struck.
- 🔊 **Proximity-triggered haunting** — no commands needed. Walk close,
  it plays. Walk away and back, it can play again — up to a configurable
  limit per person, then it goes quiet for good, for them specifically.
- 📦 **Bounded forever** — a hard cap per world plus automatic time-based
  expiry mean storage never grows unchecked, no matter how long the server
  runs or how many players die.
- ⚙️ **Fully configurable** — recording window, detection radius, view
  limits, particle style, storage caps, all in one `config.yml`.

## Install

1. Download the latest `DeathEchoes.jar` from **[Releases](../../releases/latest)**.
2. Drop it into your server's `plugins/` folder.
3. Restart the server.
4. That's it — no dependencies, no other plugins required.

**Requirements:** Paper (or a Paper fork) for **Minecraft 1.21.11 / 26.2**,
running on **Java 25+**.

## Commands

All commands live under `/deathechoes` (aliases: `/dechoes`, `/echoes`).
Requires the `deathechoes.admin` permission (defaults to server operators).

| Command | What it does |
|---|---|
| `/deathechoes info` | Shows how many echoes are stored and how many are playing right now. |
| `/deathechoes list` | Lists the death echoes nearest to you. |
| `/deathechoes clear <id\|all>` | Deletes a specific echo, or every echo. |
| `/deathechoes trigger [id]` | Instantly replays the nearest echo (or a specific one), ignoring the view limit. |
| `/deathechoes resetviews <player> [id\|all]` | Lets a player see an echo again. |
| `/deathechoes reload` | Reloads `config.yml` without restarting. |

## Configuration

The generated `config.yml` controls everything: how long a recording window
is kept before death, how close someone needs to walk to trigger a replay,
how many times each player can see the same echo, how many echoes a world
keeps before the oldest are deleted, and how long an echo is allowed to
exist before it expires automatically. Every option is commented in the
file itself.

---

<div align="center">

This repository distributes the **compiled plugin only**.<br>
Source code is not published here.

</div>
