# Elijah UI
This documentation is for Elijah UI Credit To Me

## Booting the Elijah UI Library
```lua
local lib = loadstring(game:HttpGet"https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/Vape.txt")()
```




## Creating a Elijah UI Window
```lua
local win = lib:Window("PREVIEW",Color3.fromRGB(44, 120, 224), Enum.KeyCode.RightControl)
```

## Creating a Tab
```lua
local tab = win:Tab("Tab 1")
```

## Creating a Button
```lua
tab:Button("Button", function()
lib:Notification("Notification", "Hello!", "Hi!")
end)
```

## Creating a Toggle
```lua
tab:Toggle("Toggle",false, function(t)
print(t)
end)
```

## Creating a Slider
```lua
tab:Slider("Slider",0,100,30, function(t)
print(t)
end)
```

## Creating a Dropdown
```lua
tab:Dropdown("Dropdown",{"Option 1","Option 2","Option 3","Option 4","Option 5"}, function(t)
print(t)
end)
```

## Creating a Colorpicker
```lua
tab:Colorpicker("Colorpicker",Color3.fromRGB(255,0,0), function(t)
print(t)
end)
```

## Creating a Textbox
```lua
tab:Textbox("Textbox",true, function(t)
print(t)
end)
```

## Creating a Keybind
```lua
tab:Bind("Bind",Enum.KeyCode.RightShift, function()
print("Pressed!")
end)
```

## Creating a Label
```lua
tab:Label("Label")
```

## Creating Change UI Color
```lua
changeclr:Colorpicker("Change UI Color",Color3.fromRGB(44, 120, 224), function(t)
lib:ChangePresetColor(Color3.fromRGB(t.R * 255, t.G * 255, t.B * 255))
end)
```
