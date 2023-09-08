# Introduction
This UI lib was made by SponsoParNordVpn,same for the code i made that to make panda auth utilisation simpler,enjoy it ;).Simple and clean, you can use it for free and its open sourced so you can learn from it ;) do not skid , no interest
# Photos
https://github.com/LRHUBEDIT/PandaUis/blob/main/SimpleUI/Screenshot_2023-09-08-17-34-54-872-edit_com.roblox.client.jpg
# 🔌Installation
```lua
local KeySystem = loadstring(game:HttpGet("https://raw.githubusercontent.com/LRHUBEDIT/PandaUis/main/SimpleUI/UiSource.txt
")()
```

# CreatingUI

```lua
KeySystem:New({
    Service = 'sponsploits', ---- Your panda identifier name.
    Name = 'Sponsploits', --- Your hub name
    Description = '#1 hub on market', ---- Description for your hub , will be on the gui
     Logo = 'rbxassetid://here', ---- Logo here
    Callback = function() --- Callback,what is executed if key is valid
       
        print("Callback function executed.") 
    end
})
```


# 💯Example
Simple example with anti http spy and anti tamper

```lua
if debug.info(1, "l") ~= 1 then
    game.Players.LocalPlayer:Kick("Safe dude..")
        while true do end
else
    print("Safe")
end

pcall(game.HttpGet, game, setmetatable({}, {
    __tostring = function()
        game.Players.LocalPlayer:Kick("Http spy detected")
        while true do end
        return ""
    end,
}))

local KeySystem = loadstring(game:HttpGet("https://pastebin.com/raw/zTzks2TL"))()

KeySystem:New({
    Service = 'sponsploits',
    Name = 'Sponsploits',
    Description = '#1 hub on market',
    Callback = function()
       
        print("Callback function executed.")
    end
})
```

Thats all for this UI , join discord
https://discord.gg/Z7wVevY8yj
