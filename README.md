if game.PlaceId == 17574618959 then

local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

local Window = OrionLib:MakeWindow({Name = "HeachHub -- 1 Version", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})


local Tab = Window:MakeTab({
	Name = "Tab 1",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
local Section = Tab:AddSection({
	Name = "Fishing"
})
local Section2 = Tab:AddSection({
	Name = "Settings"
})
local Section3 = Tab:AddSection({
	Name = "Market
})
local Section4 = Tab:AddSection({
	Name = "Extras"
})
OrionLib:MakeNotification({
	Name = "HeachHub",
	Content = "Join Our Discord!: Discord.gg/HeachHub",
	Image = "rbxassetid://4483345998",
	Time = 5
})
Tab:AddButton({
	Name = "Copy Discord",
	Callback = function()
      		print("Copied!")
  	end    
})
Tab:AddToggle({
	Name = "Auto Reel",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})
Tab:AddColorpicker({
	Name = "Colorpicker",
	Default = Color3.fromRGB(255, 0, 0),
	Callback = function(Value)
		print(Value)
	end	  
})
Tab:AddSlider({
	Name = "Slider",
	Min = 0,
	Max = 20,
	Default = 5,
	Color = Color3.fromRGB(255,255,255),
	Increment = 1,
	ValueName = "bananas",
	Callback = function(Value)
		print(Value)
	end    
})
OrionLib:Init()
