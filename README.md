local players = game:GetService("Players")
local runService = game:GetService("RunService")

local function createGUI(player)
    local gui = Instance.new("ScreenGui", player.PlayerGui)
    gui.Name = "DeltaGUI"
    
    local frame = Instance.new("Frame", gui)
    frame.Size = UDim2.new(0.2, 0, 0.3, 0)
    frame.Position = UDim2.new(0.8, 0, 0.7, 0)
    frame.BackgroundColor3 = Color3.new(0, 0, 0)
    frame.BackgroundTransparency = 0.5
    frame.BorderSizePixel = 0
    
    local button1 = Instance.new("TextButton", frame)
    button1.Size = UDim2.new(1, 0, 0.2, 0)
    button1.Position = UDim2.new(0, 0, 0, 0)
    button1.Text = "Esplin Ver"
    button1.BackgroundColor3 = Color3.new(0, 1, 0)
    button1.TextColor3 = Color3.new(1, 1, 1)
    button1.BorderSizePixel = 0
    
    local button2 = Instance.new("TextButton", frame)
    button2.Size = UDim2.new(1, 0, 0.2, 0)
    button2.Position = UDim2.new(0, 0, 0.2, 0)
    button2.Text = "Invisivel"
    button2.BackgroundColor3 = Color3.new(0, 1, 0)
    button2.TextColor3 = Color3.new(1, 1, 1)
    button2.BorderSizePixel = 0
    
    local button3 = Instance.new("TextButton", frame)
    button3.Size = UDim2.new(1, 0, 0.2, 0)
    button3.Position = UDim2.new(0, 0, 0.4, 0)
    button3.Text = "Voar"
    button3.BackgroundColor3 = Color3.new(0, 1, 0)
    button3.TextColor3 = Color3.new(1, 1, 1)
    button3.BorderSizePixel = 0
    
    local button4 = Instance.new("TextButton", frame)
    button4.Size = UDim2.new(1, 0, 0.2, 0)
    button4.Position = UDim2.new(0, 0, 0.6, 0)
    button4.Text = "Velocidade"
    button4.BackgroundColor3 = Color3.new(0, 1, 0)
    button4.TextColor3 = Color3.new(1, 1, 1)
    button4.BorderSizePixel = 0
    
    button1.MouseButton1Click:Connect(function()
        -- Esplin Ver logic
    end)
    
    button2.MouseButton1Click:Connect(function()
        -- Invisivel logic
    end)
    
    button3.MouseButton1Click:Connect(function()
        -- Voar logic
    end)
    
    button4.MouseButton1Click:Connect(function()
        -- Velocidade logic
    end)
end

players.PlayerAdded:Connect(function(player)
    createGUI(player)
end)
