---
layout: post
title: "MetatableAC - Documentation"
date: 2025-02-14 08:57:20 +0500
categories: lua anticheat
usemathjax: true
---
=============================

Documentation format:
-------------------------------------

The documentation uses the following format for function descriptions:

    <span style="color: red;"><</span><span style="color: yellow;">return_type</span><span style="color: red;">></span> function_name<span style="color: red;">(</span><span style="color: yellow;">argument_type</span> <span style="color: blue;">argument_name</span><span style="color: red;">)</span>

---

<br><br><br>

## Punish Player
    <span style="color: red;"><</span><span style="color: yellow;">void</span><span style="color: red;">></span> Punishment<span style="color: red;">(</span><span style="color: yellow;">Player</span> <span style="color: blue;">player</span><span style="color: blue;">,</span> <span style="color: yellow;">string</span> <span style="color: blue;">Reason</span><span style="color: blue;">,</span> <span style="color: yellow;">number</span> <span style="color: blue;">Severity</span><span style="color: red;">)</span>

Punishes the player from the game with the default punishment dependant on the severity number.

(0: Flag, 1: Warn, 2: Mute, 3: Kick, 4: Temp Ban 5: Perm Ban)

---

## Custom Punish Player

    <span style="color: red;"><</span><span style="color: yellow;">void</span><span style="color: red;">></span> CustomPunishment<span style="color: red;">(</span><span style="color: yellow;">Player</span> <span style="color: blue;">player</span><span style="color: blue;">,</span> <span style="color: yellow;">string</span> <span style="color: blue;">Reason</span><span style="color: red;">)</span>

Punishes the player from the game with a custom punishment (Kick, Ban, etc.).

---

## Set Max Walkspeed

    <span style="color: red;"><</span><span style="color: yellow;">void</span><span style="color: red;">></span> SetMaxWalkspeed<span style="color: red;">(</span><span style="color: yellow;">Player</span> <span style="color: blue;">player</span><span style="color: blue;">,</span> <span style="color: yellow;">number</span> <span style="color: blue;">Speed</span><span style="color: red;">)</span>

Sets the player's walkspeed serverside with consideration to server-side and client-side anticheat.

---

## Set Max Walkspeed Global

    <span style="color: red;"><</span><span style="color: yellow;">void</span><span style="color: red;">></span> SetMaxWalkspeedGlobal<span style="color: red;">(</span><span style="color: yellow;">number</span> <span style="color: blue;">Speed</span><span style="color: red;">)</span>

Sets a concurrent walkspeed for all players with consideration to server-side and client-side anticheat.

---

## Flag For Review

    <span style="color: red;"><</span><span style="color: yellow;">void</span><span style="color: red;">></span> flagForReview<span style="color: red;">(</span><span style="color: yellow;">Player</span> <span style="color: blue;">player</span><span style="color: red;">)</span>

Logs a player's suspicious activity for manual review via custom function.

---

## Disable Chat

    <span style="color: red;"><</span><span style="color: yellow;">void</span><span style="color: red;">></span> disableChat<span style="color: red;">(</span><span style="color: yellow;">Player</span> <span style="color: blue;">player</span><span style="color: blue;">,</span> <span style="color: yellow;">number</span> <span style="color: blue;">Duration</span><span style="color: red;">)</span>

Disables a player's chat ability for a set duration.

---

## Reset Player Stats

    <span style="color: red;"><</span><span style="color: yellow;">void</span><span style="color: red;">></span> resetPlayerStats<span style="color: red;">(</span><span style="color: yellow;">Player</span> <span style="color: blue;">player</span><span style="color: red;">)</span>

Wipes a player's stats completely clean from all databases.

---
