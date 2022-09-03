

local ScreenGui = Instance.new("ScreenGui")
local loader = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local loadertext = Instance.new("TextLabel")
local UICorner_2 = Instance.new("UICorner")
local loader_2 = Instance.new("TextButton")
local UICorner_3 = Instance.new("UICorner")


ScreenGui.Parent = game.CoreGui

loader.Name = "loader"
loader.Parent = ScreenGui
loader.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
loader.Position = UDim2.new(0.0801457167, 0, 0.564615369, 0)
loader.Size = UDim2.new(0, 183, 0, 157)

UICorner.Parent = loader

loadertext.Name = "loader text"
loadertext.Parent = loader
loadertext.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
loadertext.Size = UDim2.new(0, 179, 0, 55)
loadertext.Font = Enum.Font.SourceSans
loadertext.Text = "DarkWare's Loader"
loadertext.TextColor3 = Color3.fromRGB(170, 255, 0)
loadertext.TextScaled = true
loadertext.TextSize = 14.000
loadertext.TextWrapped = true

UICorner_2.Parent = loadertext

loader_2.Name = "loader"
loader_2.Parent = loader
loader_2.BackgroundColor3 = Color3.fromRGB(0, 0, 127)
loader_2.Position = UDim2.new(0.145857915, 0, 0.559473872, 0)
loader_2.Size = UDim2.new(0, 124, 0, 45)
loader_2.Font = Enum.Font.SourceSans
loader_2.Text = "Load"
loader_2.TextColor3 = Color3.fromRGB(255, 255, 255)
loader_2.TextScaled = true
loader_2.TextSize = 14.000
loader_2.TextWrapped = true
loader_2.MouseButton1Down:connect(function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/selecteduseromg343/MacOsUI/main/README.md"))()
end)




UICorner_3.Parent = loader_2


local function SUYSY_fake_script() -- loader_2.Script 
	local script = Instance.new('Script', loader_2)

	script.Parent.MouseButton1Click:Connect(function()
		script.Parent.Parent.Visible = false
	end)
end
coroutine.wrap(SUYSY_fake_script)()
