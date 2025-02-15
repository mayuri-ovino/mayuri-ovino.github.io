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

<h2> Punish Player </h2>

    <void> Punishment(<Player> player, <string> Reason, <number> Severity)

Punishes the player from the game with the default punishment dependant on the severity number.

<h4>(0: Flag, 1: Warn, 2: Mute, 3: Kick, 4: Temp Ban 5: Perm Ban)</h4>
---

<h2> Custom Punish Player  </h2>

    <void> CustomPunishment(<Player> player, <string> Reason)

Punishes the player from the game with a custom punishment (Kick, Ban, etc.).

<h2> Set Max Walkspeed </h2>
```lua
    <void> SetMaxWalkspeed(<Player> player, <number> Speed)
```
Sets the player's walkspeed serverside with consideration to server-side and client-side anticheat.

<h2> Set Max Walkspeed Global </h2>
```lua
    <void> SetMaxWalkspeedGlobal(<number> Speed)
```
Sets a concurrent walkspeed for all players with consideration to server-side and client-side anticheat.

<h2> Flag For Review </h2>
```lua
    <void> flagForReview(<Player> player)
```

Logs a player's suspicious activity for manual review via custom function.

<h2> Disable Chat </h2>
```lua
    <void> disableChat(<Player> player, <number> Duration)
```
Disables a player's chat ability for a set duration.

<h2> Reset Player Stats </h2>
```lua
    <void> resetPlayerStats(<Player> player)
```
Wipes a player's stats completely clean from all databases.

---
