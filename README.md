local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local TextLabel = Instance.new("TextLabel")
local UICorner_2 = Instance.new("UICorner")
local load = Instance.new("TextButton")
local UICorner_3 = Instance.new("UICorner")
local TextLabel_2 = Instance.new("TextLabel")
local UICorner_4 = Instance.new("UICorner")


ScreenGui.Parent = game.CoreGui

Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.fromRGB(85, 255, 255)
Frame.Position = UDim2.new(0.254876465, 0, 0.423076987, 0)
Frame.Size = UDim2.new(0, 377, 0, 225)
Frame.Active = true
Frame.Draggable = true

UICorner.Parent = Frame

TextLabel.Parent = Frame
TextLabel.BackgroundColor3 = Color3.fromRGB(85, 85, 255)
TextLabel.Position = UDim2.new(-0.00265251985, 0, 0, 0)
TextLabel.Size = UDim2.new(0, 377, 0, 44)
TextLabel.Font = Enum.Font.SourceSans
TextLabel.Text = "Loader"
TextLabel.TextColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.TextScaled = true
TextLabel.TextSize = 14.000
TextLabel.TextWrapped = true

UICorner_2.Parent = TextLabel

load.Name = "load"
load.Parent = Frame
load.BackgroundColor3 = Color3.fromRGB(85, 170, 255)
load.Position = UDim2.new(0.302387267, 0, 0.48888877, 0)
load.Size = UDim2.new(0, 146, 0, 42)
load.Font = Enum.Font.SourceSans
load.Text = "Load me!"
load.TextColor3 = Color3.fromRGB(0, 0, 0)
load.TextScaled = true
load.TextSize = 14.000
load.TextWrapped = true
load.MouseButton1Down:connect(function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/selecteduseromg343/MacOsUI/main/README.md"))()
end)

UICorner_3.Parent = load

TextLabel_2.Parent = Frame
TextLabel_2.BackgroundColor3 = Color3.fromRGB(170, 0, 0)
TextLabel_2.Position = UDim2.new(0.962864697, 0, 0, 0)
TextLabel_2.Size = UDim2.new(0, 14, 0, 12)
TextLabel_2.Font = Enum.Font.SourceSans
TextLabel_2.Text = ""
TextLabel_2.TextColor3 = Color3.fromRGB(0, 0, 0)
TextLabel_2.TextSize = 14.000

UICorner_4.Parent = TextLabel_2
