---
layout: post
title: "MetatableAC - Documentation"
date: 2025-02-14 08:57:20 +0500
categories: lua anticheat
usemathjax: true
---

# How the documentation is formated

```lua
<return_type> function_name(<argument_type> argument_name)
```

```lua
<void> Punishment(<Player>, player, <string> Reason)
```
Punishes the player from the game with the default punishment. (Kick)
```lua
  metatable_module.Punishment:Connect(function(player, Reason)
	  player:Kick(Reason)
  end)
```
```lua
<void> CustomPunishment(<Player>, player, <string> Reason)
```
Punishes the player from the game with a custom punishment. (Kick, Ban, ETC)
```lua
  metatable_module.Punishment:Connect(function(player, Reason)
	  local config = {
  		UserIds = {player.UserId},
  		Duration = -1,
  		DisplayReason = "You were hit with a BAN HAMMAR!!",
  		ExcludeAltAccounts = false,
		}

    local success, err = pcall(function()
		  return Players:BanAsync(config)
	  end)
  end)
```
