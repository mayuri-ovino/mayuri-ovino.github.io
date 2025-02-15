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

<h6> Punish Player </h6>

    <void> Punishment(<Player> player, <string> Reason, <number> Severity)

Punishes the player from the game with the default punishment dependant on the severity number.

(0: Flag, 1: Warn, 2: Mute, 3: Kick, 4: Temp Ban 5: Perm Ban)
---

<h6> Custom Punish Player </h6>

    <void> CustomPunishment(<Player> player, <string> Reason)

Punishes the player from the game with a custom punishment (Kick, Ban, etc.).

<h6> Set Max Walkspeed </h6>
```lua
    <void> SetMaxWalkspeed(<Player> player, <number> Speed)
```
Sets the player's walkspeed serverside with consideration to server-side and client-side anticheat.

<h6> Set Max Walkspeed Global </h6>
```lua
    <void> SetMaxWalkspeedGlobal(<number> Speed)
```
Sets a concurrent walkspeed for all players with consideration to server-side and client-side anticheat.

<h6> Flag For Review </h6>
```lua
    <void> flagForReview(<Player> player)
```

Logs a player's suspicious activity for manual review via custom function.

<h6> Disable Chat </h6>
```lua
    <void> disableChat(<Player> player, <number> Duration)
```
Disables a player's chat ability for a set duration.

<h6> Reset Player Stats </h6>
```lua
    <void> resetPlayerStats(<Player> player)
```
Wipes a player's stats completely clean from all databases.

---
