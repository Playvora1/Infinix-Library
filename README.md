# Infinix UI Library

Introducing the Infinix UI Library by Hosvile

## Getting Started

To begin, you need to declare a variable to access the library.

```lua
local Lib = loadstring(game:HttpGet("https://raw.githubusercontent.com/Hosvile/Refinement/main/UI-th%20Library%20v0.1.2"))()
```

To load the UI, simply call the function:

```lua
local window = Lib:CreateWindow("InfiniX.Lib")

```


### Tab

You can create multiple tabs to organize your features.

```lua
local tab = window:CreateTab("Main")
```
```lua
local tabs = window:CreateTab("Properties")
```

### Button

Create functional search button to any tabs

```lua
tab:Search()
```

### Toggle

Use toggles that can be turned on or off.

```lua
tab:CreateToggle("Toggle/Checkbox",true,function(bool) print(bool) end)

```

### Input Text

Get input text from the user.

```lua
tab:CreateTextbox("Textbox",function(text)
print(text)
end)

```

## Dropdown

Create dropdown menus easily.

```lua
tab:CreateDropdown("Dropdown",{"Opt. 1"},function(option)
print(option)
end)
```


### Slider

Add sliders, which work well for mobile users too!

```lua
tab:CreateSlider("Slider", 0, 1000, function(value)
print(value)
end)
```

