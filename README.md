## Create Window
```lua
local MakoLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/vFishyTurtle/Orion/864d311059bb70395616dabaf05f52a47c33eae1/c",true))()

local Window = MakoLib:CreateWindow({
    Title = "Meta Hub "
})
```
## Create Tab
```lua
local tab1 = Window:CreateTab("Main", 13594361489)
```
## Create Section
```lua
local sec1 = tab1:CreateSection("QB Aimbot", 13594361489)
```
## Create Toggle
```lua
sec1:CreateToggle({
    Title = "Auto Catch",
    Binding = false,
    CurrentValue = false,
    Callback = function(value)
        if value then
            autoCatch()
        end
    end,
})
```
## Create Slider
```lua
sec1:CreateSlider({
    Title = "Auto Catch Distance",
    CurrentValue = 0,
    Range = {0, 10},
    Callback = function(value)
        autodist = value
    end,
})
```
## Create Dropdown
```lua
sec1:CreateDropdown({
    Title = "Mag Type",
    Options = {"Regular", "Blatant", "Legit"},
    CurrentOption = "Regular",
    Callback = function(Value)
        if (getgenv().Football_Magnents) then
            
        end
    end,
})
```
