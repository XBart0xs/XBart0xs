local Material = loadstring(game:HttpGet("https://raw.githubusercontent.com/Kinlei/MaterialLua/master/Module.lua"))()

local X = Material.Load({
	Title = "Akademia Policyjna fucker by:ConeWare#7771 v0.1a",
	Style = 3,
	SizeX = 500,
	SizeY = 350,
	Theme = "Dark",
	ColorOverrides = {
		MainFrame = Color3.fromRGB(235,235,235)
	}
})

local Y = X.New({
	Title = "1"
})

local Z = X.New({
	Title = "2"
})

local A = Y.Button({
	Text = "AlarmAbuse",
	Callback = function()
    fireclickdetector(game:GetService("Workspace")["ESSER MCP"].Part.ClickDetector)
		print("Widza twoj nick")
	end,
	Menu = {
		Information = function(self)
			X.Banner({
				Text = "Widza twoj nick na jednym z ekranow"
			})
		end
	}
})

local A = Y.Button({
	Text = "Gunshop TP",
	Callback = function()
	    	local pl = game.Players.LocalPlayer.Character.HumanoidRootPart
    local location = CFrame.new(530, 15, 270)
    local humanoid = game.Players.LocalPlayer.Character.Humanoid
    humanoid:ChangeState(Enum.HumanoidStateType.Jumping)
    wait(0.1)
pl.CFrame = location
		print("Teleported")
	end,
	Menu = {
		Information = function(self)
			X.Banner({
				Text = "Teleport"
			})
		end
	}
})

local A = Y.Button({
	Text = "Przelacz brame graniczna",
	Callback = function()
    fireclickdetector(game:GetService("Workspace")["Gate system"].Switch.ClickDetector)
    
		print("przelonczono")
	end,
	Menu = {
		Information = function(self)
			X.Banner({
				Text = "powkurwiaj ludzi brama"
			})
		end
	}
})

local A = Y.Button({
	Text = "Zablokuj 2 drzwi",
	Callback = function()
    while true do

    fireclickdetector(game:GetService("Workspace")["Button door"].Close.ClickDetector)
    wait(0.01)
    end
    
		print("przelonczono")
	end,
	Menu = {
		Information = function(self)
			X.Banner({
				Text = "zablokuj 2 drzwi od spawna"
			})
		end
	}
})
