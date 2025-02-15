---
layout: post
title: "MetatableAC - Documentation"
date: 2025-02-14 08:57:20 +0500
categories: lua anticheat
usemathjax: true
---

<style>
.return-type { color: #d3ce9e; }
.function-name { color: #dcdcdc; }
.argument-type { color: #d3ce9e; }
.argument-name { color: #5ec2d4; }
.punctuation { color: #d8235e; }
.description { color: #dcdcdc; }
</style>

## Documentation format:

The documentation uses the following format for function descriptions:

<pre><code><span class="punctuation"><</span><span class="return-type">return_type</span><span class="punctuation">></span> <span class="function-name">function_name</span><span class="punctuation">(</span><span class="argument-type">argument_type</span> <span class="argument-name">argument_name</span><span class="punctuation">)</span></code></pre>

---

## Punish Player

<pre><code><span class="punctuation"><</span><span class="return-type">void</span><span class="punctuation">></span> <span class="function-name">Punishment</span><span class="punctuation">(</span><span class="argument-type">Player</span> <span class="argument-name">player</span><span class="punctuation">,</span> <span class="argument-type">string</span> <span class="argument-name">Reason</span><span class="punctuation">,</span> <span class="argument-type">number</span> <span class="argument-name">Severity</span><span class="punctuation">)</span></code></pre>

<p class="description">Punishes the player from the game with the default punishment dependant on the severity number.</p>

<p class="description">(0: Flag, 1: Warn, 2: Mute, 3: Kick, 4: Temp Ban 5: Perm Ban)</p>

---

## Custom Punish Player

<pre><code><span class="punctuation"><</span><span class="return-type">void</span><span class="punctuation">></span> <span class="function-name">CustomPunishment</span><span class="punctuation">(</span><span class="argument-type">Player</span> <span class="argument-name">player</span><span class="punctuation">,</span> <span class="argument-type">string</span> <span class="argument-name">Reason</span><span class="punctuation">)</span></code></pre>

<p class="description">Punishes the player from the game with the custom punishment (Kick, Ban, etc.).</p>

---

## Set Max Walkspeed

<pre><code><span class="punctuation"><</span><span class="return-type">void</span><span class="punctuation">></span> <span class="function-name">SetMaxWalkspeed</span><span class="punctuation">(</span><span class="argument-type">Player</span> <span class="argument-name">player</span><span class="punctuation">,</span> <span class="argument-type">number</span> <span class="argument-name">Speed</span><span class="punctuation">)</span></code></pre>

<p class="description">Sets the player's walkspeed serverside with consideration to server-side and client-side anticheat.</p>

---

## Set Max Walkspeed Global

<pre><code><span class="punctuation"><</span><span class="return-type">void</span><span class="punctuation">></span> <span class="function-name">SetMaxWalkspeedGlobal</span><span class="punctuation">(</span><span class="argument-type">number</span> <span class="argument-name">Speed</span><span class="punctuation">)</span></code></pre>

<p class="description">Sets a concurrent walkspeed for all players with consideration to server-side and client-side anticheat.</p>

---

## Flag For Review

<pre><code><span class="punctuation"><</span><span class="return-type">void</span><span class="punctuation">></span> <span class="function-name">flagForReview</span><span class="punctuation">(</span><span class="argument-type">Player</span> <span class="argument-name">player</span><span class="punctuation">)</span></code></pre>

<p class="description">Logs a player's suspicious activity for manual review via custom function.</p>

---

## Disable Chat

<pre><code><span class="punctuation"><</span><span class="return-type">void</span><span class="punctuation">></span> <span class="function-name">disableChat</span><span class="punctuation">(</span><span class="argument-type">Player</span> <span class="argument-name">player</span><span class="punctuation">,</span> <span class="argument-type">number</span> <span class="argument-name">Duration</span><span class="punctuation">)</span></code></pre>

<p class="description">Disables a player's chat ability for a set duration.</p>

---

## Reset Player Stats

<pre><code><span class="punctuation"><</span><span class="return-type">void</span><span class="punctuation">></span> <span class="function-name">resetPlayerStats</span><span class="punctuation">(</span><span class="argument-type">Player</span> <span class="argument-name">player</span><span class="punctuation">)</span></code></pre>

<p class="description">Wipes a player's stats completely clean from all databases.</p>
