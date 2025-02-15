---
layout: post
title: "MetatableAC - Documentation"
date: 2025-02-14 08:57:20 +0500
categories: lua anticheat
usemathjax: true
---
MetatableAC - Documentation
=============================

Documentation format:
-------------------------------------

The documentation uses the following format for function descriptions:

    <return_type> function_name(<argument_type> argument_name)

---

# Punishment Player

    <void> Punishment(<Player> player, <string> Reason, <number> Severity)

Punishes the player from the game with the default punishment dependant on the severity number.

(0: Flag, 1: Warn, 2: Mute, 3: Kick, 4: Temp Ban 5: Perm Ban)
---

# Custom Punish Player

    <void> CustomPunishment(<Player> player, <string> Reason)

Punishes the player from the game with a custom punishment (Kick, Ban, etc.).

# Set Max Walkspeed
    <void> SetMaxWalkspeed(<Player> player, <number> Speed)

Sets the player's walkspeed serverside with consideration to server-side and client-side anticheat.

# Set Max Walkspeed Global
    <void> SetMaxWalkspeedGlobal(<number> Speed)

Sets a concurrent walkspeed for all players with consideration to server-side and client-side anticheat.

# Flag For Review
    <void> flagForReview(<Player> player)

Logs a player's suspicious activity for manual review via custom function.

# Disable Chat
    <void> disableChat(<Player> player, <number> Duration)

Disables a player's chat ability for a set duration.

# Reset Player Stats
    <void> resetPlayerStats(<Player> player)

Wipes a player's stats completely clean from all databases.

---
