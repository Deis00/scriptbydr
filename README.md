-- Criar GUI
local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local TextLabel = Instance.new("TextLabel")

ScreenGui.Parent = game.CoreGui

Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Frame.Position = UDim2.new(0.5, -100, 0.5, -50)
Frame.Size = UDim2.new(0, 200, 0, 100)

TextLabel.Parent = Frame
TextLabel.Text = "Andrei Hub"
TextLabel.Size = UDim2.new(1, 0, 1, 0)
TextLabel.TextColor3 = Color3.fromRGB(0, 0, 0)

-- Adicionar Animação
local TweenService = game:GetService("TweenService")
local tweenInfo = TweenInfo.new(2, Enum.EasingStyle.Bounce, Enum.EasingDirection.Out)
local goal = {Position = UDim2.new(0.5, -100, 0.5, -150)}

local tween = TweenService:Create(Frame, tweenInfo, goal)
tween:Play()

-- Script para Gerar Fruta Automática (Gacha)
spawn(function()
    while true do
        wait(10) -- Espera 10 segundos entre cada tentativa
        -- Código para interagir com o gacha
    end
end)

-- ESP dos Jogadores e Frutas
spawn(function()
    while true do
        for _, player in pairs(game.Players:GetPlayers()) do
            if player ~= game.Players.LocalPlayer then
                local BillboardGui = Instance.new("BillboardGui")
                local TextLabel = Instance.new("TextLabel")

                BillboardGui.Parent = player.Character.Head
                BillboardGui.Size = UDim2.new(1, 0, 1, 0)
                BillboardGui.Adornee = player.Character.Head

                TextLabel.Parent = BillboardGui
                TextLabel.Text = player.Name
                TextLabel.Size = UDim2.new(1, 0, 1, 0)
                TextLabel.TextColor3 = Color3.fromRGB(255, 0, 0)
            end
        end
        wait(1) -- Atualiza a cada segundo
    end
end)
