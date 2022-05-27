# siernlib

siernlib is a open sourced Roblox UI library
Support server: discord.gg/zen

## Loadstring
```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/laderite/siernlib/main/library.lua"))()
```

## Features:
- Buttons
- Sliders
- Textbox
- Toggles
- Labels
- Dropdowns

## Documentation
Showcasing all the UI Elements

# Load the library
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/laderite/siernlib/main/library.lua"))()
```

# Creating the UI
```lua
local win = Library:Create({
    Name = "Library Name"
})
```

# Creating a tab
```lua
local maintab = win:Tab('Main')
local charactertab = win:Tab('Local Player')
local uitab = win:Tab('UI')
```

# Creating a section
```lua
local main = maintab:Section('AUTOFARM')
local character = charactertab:Section('LOCAL')
local ui = uitab:Section('UI SETTINGS')
```

# Creating a button
```lua
ui:Button('Destroy GUI', function()
    win:Exit() -- destroys the gui  
end)
```

# Creating a toggle
```lua
main:Toggle('Aimbot', function(v)
    aimbot = v
end)
```

# Creating a textbox
```lua
main:Textbox('FOV', function(v)
    fov = v
end)
```

# Creating a slider
```lua
main:Slider('FOV', 0 -- min, 25 -- max, 0 -- default, 2.5 -- increment function(v)
    print(v)
end)
```

# Creating a label
```lua
main:Label('This is a label')
```

# Creating a dropdown
```lua
local dropdown = main:Dropdown("Dropdown", {"a","b","c","d"},"", function(v)
    print(v)
end)
```
