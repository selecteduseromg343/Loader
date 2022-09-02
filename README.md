--- Close Button by Commando#6764
-- UI Made by Commando#6764

local ScreenGui = Instance.new("ScreenGui")
local Main = Instance.new("Frame")
local TextLabel = Instance.new("TextLabel")
local UICorner = Instance.new("UICorner")
local UICorner_2 = Instance.new("UICorner")
local load = Instance.new("TextButton")
local UICorner_3 = Instance.new("UICorner")
local close = Instance.new("TextButton")
local UICorner_4 = Instance.new("UICorner")


ScreenGui.Parent = game.CoreGui

Main.Name = "Main"
Main.Parent = ScreenGui
Main.BackgroundColor3 = Color3.fromRGB(0, 170, 255)
Main.Position = UDim2.new(0.365603656, 0, 0.453846157, 0)
Main.Size = UDim2.new(0, 266, 0, 254)
Main.Active = true
Main.Draggable = true

TextLabel.Parent = Main
TextLabel.BackgroundColor3 = Color3.fromRGB(170, 0, 0)
TextLabel.Size = UDim2.new(0, 266, 0, 51)
TextLabel.Font = Enum.Font.SourceSans
TextLabel.Text = "Loader"
TextLabel.TextColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.TextScaled = true
TextLabel.TextSize = 14.000
TextLabel.TextWrapped = true

UICorner.Parent = TextLabel

UICorner_2.Parent = Main

load.Name = "load"
load.Parent = Main
load.BackgroundColor3 = Color3.fromRGB(170, 255, 0)
load.Position = UDim2.new(-3.7252903e-09, 0, 0.874015749, 0)
load.Size = UDim2.new(0, 113, 0, 32)
load.Font = Enum.Font.SourceSans
load.Text = "Load me"
load.TextColor3 = Color3.fromRGB(0, 0, 0)
load.TextScaled = true
load.TextSize = 14.000
load.TextWrapped = true
load.MouseButton1Down:connect(function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/selecteduseromg343/MacOsUI/main/README.md"))()
end)

UICorner_3.Parent = load

close.Name = "close"
close.Parent = Main
close.BackgroundColor3 = Color3.fromRGB(170, 170, 0)
close.Position = UDim2.new(0.526315808, 0, 0.838582695, 0)
close.Size = UDim2.new(0, 126, 0, 41)
close.Font = Enum.Font.SourceSans
close.Text = "UI Is Loaded? Close"
close.TextColor3 = Color3.fromRGB(0, 0, 0)
close.TextScaled = true
close.TextSize = 14.000
close.TextWrapped = true

UICorner_4.Parent = close

-- close button added

local function UBFA_fake_script() -- close.LocalScript 
	local script = Instance.new('LocalScript', close)

	script.Parent.MouseButton1Click:Connect(function()
		script.Parent.Parent.Visible = false
	end)
end
coroutine.wrap(UBFA_fake_script)()
