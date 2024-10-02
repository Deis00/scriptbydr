-- Script de farm automático de baús para Blox Fruits
-- Painel personalizado com o nome "Andreihub"

local Andreihub = Instance.new("ScreenGui")
local MainFrame = Instance.new("Frame")
local Title = Instance.new("TextLabel")

Andreihub.Name = "Andreihub"
Andreihub.Parent = game.CoreGui

MainFrame.Name = "MainFrame"
MainFrame.Parent = Andreihub
MainFrame.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
MainFrame.BorderSizePixel = 0
MainFrame.Position = UDim2.new(0.5, -200, 0.5, -150)
MainFrame.Size = UDim2.new(0, 400, 0, 300)

Title.Name = "Title"
Title.Parent = MainFrame
Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Title.Size = UDim2.new(0, 400, 0, 50)
Title.Font = Enum.Font.SourceSans
Title.Text = "Andreihub"
Title.TextColor3 = Color3.fromRGB(0, 0, 0)
Title.TextSize = 30

-- Função para farmar baús automaticamente
local function FarmBaús()
    while true do
        for _, chest in pairs(game.Workspace:GetChildren()) do
            if chest:IsA("Model") and chest.Name == "Chest" then
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = chest.HumanoidRootPart.CFrame
                wait(1) -- Tempo para pegar o baú
            end
        end
        wait(10) -- Tempo de espera antes de procurar novamente
    end
end

-- Iniciar o farm automático
spawn(FarmBaús)
