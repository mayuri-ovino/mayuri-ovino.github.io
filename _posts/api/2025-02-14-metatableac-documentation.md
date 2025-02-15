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

<span style="color: #d8235e;"><</span><span style="color: #d3ce9e;">return_type</span><span style="color: #d8235e;">></span> function_name<span style="color: #d8235e;">(</span><span style="color: #d3ce9e;">argument_type</span> <span style="color: #5ec2d4;">argument_name</span><span style="color: #d8235e;">)</span>

---

## Punish Player

<span style="color: #d8235e;"><</span><span style="color: #d3ce9e;">void</span><span style="color: #d8235e;">></span> Punishment<span style="color: #d8235e;">(</span><span style="color: #d3ce9e;">Player</span> <span style="color: #5ec2d4;">player</span><span style="color: #5ec2d4;">,</span> <span style="color: #d3ce9e;">string</span> <span style="color: #5ec2d4;">Reason</span><span style="color: #5ec2d4;">,</span> <span style="color: #d3ce9e;">number</span> <span style="color: #5ec2d4;">Severity</span><span style="color: #d8235e;">)</span>

<span style="color: #dcdcdc;">Punishes the player from the game with the default punishment dependant on the severity number.</span>

<span style="color: #dcdcdc;">(0: Flag, 1: Warn, 2: Mute, 3: Kick, 4: Temp Ban 5: Perm Ban)</span>

---

## Custom Punish Player

<span style="color: #d8235e;"><</span><span style="color: #d3ce9e;">void</span><span style="color: #d8235e;">></span> CustomPunishment<span style="color: #d8235e;">(</span><span style="color: #d3ce9e;">Player</span> <span style="color: #5ec2d4;">player</span><span style="color: #5ec2d4;">,</span> <span style="color: #d3ce9e;">string</span> <span style="color: #5ec2d4;">Reason</span><span style="color: #d8235e;">)</span>

<span style="color: #dcdcdc;">Punishes the player from the game with the custom punishment (Kick, Ban, etc.).</span>

---

## Set Max Walkspeed

<span style="color: #d8235e;"><</span><span style="color: #d3ce9e;">void</span><span style="color: #d8235e;">></span> SetMaxWalkspeed<span style="color: #d8235e;">(</span><span style="color: #d3ce9e;">Player</span> <span style="color: #5ec2d4;">player</span><span style="color: #5ec2d4;">,</span> <span style="color: #d3ce9e;">number</span> <span style="color: #5ec2d4;">Speed</span><span style="color: #d8235e;">)</span>

<span style="color: #dcdcdc;">Sets the player's walkspeed serverside with consideration to server-side and client-side anticheat.</span>

---

## Set Max Walkspeed Global

<span style="color: #d8235e;"><</span><span style="color: #d3ce9e;">void</span><span style="color: #d8235e;">></span> SetMaxWalkspeedGlobal<span style="color: #d8235e;">(</span><span style="color: #d3ce9e;">number</span> <span style="color: #5ec2d4;">Speed</span><span style="color: #d8235e;">)</span>

<span style="color: #dcdcdc;">Sets a concurrent walkspeed for all players with consideration to server-side and client-side anticheat.</span>

---

## Flag For Review

<span style="color: #d8235e;"><</span><span style="color: #d3ce9e;">void</span><span style="color: #d8235e;">></span> flagForReview<span style="color: #d8235e;">(</span><span style="color: #d3ce9e;">Player</span> <span style="color: #5ec2d4;">player</span><span style="color: #d8235e;">)</span>

<span style="color: #dcdcdc;">Logs a player's suspicious activity for manual review via custom function.</span>

---

## Disable Chat

<span style="color: #d8235e;"><</span><span style="color: #d3ce9e;">void</span><span style="color: #d8235e;">></span> disableChat<span style="color: #d8235e;">(</span><span style="color: #d3ce9e;">Player</span> <span style="color: #5ec2d4;">player</span><span style="color: #5ec2d4;">,</span> <span style="color: #d3ce9e;">number</span> <span style="color: #5ec2d4;">Duration</span><span style="color: #d8235e;">)</span>

<span style="color: #dcdcdc;">Disables a player's chat ability for a set duration.</span>

---

## Reset Player Stats

<span style="color: #d8235e;"><</span><span style="color: #d3ce9e;">void</span><span style="color: #d8235e;">></span> resetPlayerStats<span style="color: #d8235e;">(</span><span style="color: #d3ce9e;">Player</span> <span style="color: #5ec2d4;">player</span><span style="color: #d8235e;">)</span>

<span style="color: #dcdcdc;">Wipes a player's stats completely clean from all databases.</span>
