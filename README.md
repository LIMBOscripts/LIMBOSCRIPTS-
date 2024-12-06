-- Create the main window
local Window = OrionLib:MakeWindow({
    Name = "LIMBO_SCRIPTS",
    HidePremium = false,
    SaveConfig = true,
    ConfigFolder = "instant UGC"
})

-- Add a tab
local Tab = Window:MakeTab({
    Name = "CHRISMAST OBBY",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
})

-- Add a button
Tab:AddButton({
    Name = "Chrismast Obby (rampage script)",
    Callback = function()
        -- Place the script to execute here
        loadstring(game:HttpGet("https://raw.githubusercontent.com/r4mpage4/UGCLIMITED/refs/heads/main/Protected_8295132449483425.txt"))()
    end    
})

-- Initialize the GUI
OrionLib:Init()
