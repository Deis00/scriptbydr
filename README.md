-- Script para farmar Haki da Observação no Blox Fruits com painel

-- Criar o painel
local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local TextLabel = Instance.new("TextLabel")
local Button = Instance.new("TextButton")

-- Configurar o painel
ScreenGui.Parent = game.CoreGui

Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
Frame.Position = UDim2.new(0.5, -100, 0.5, -50)
Frame.Size = UDim2.new(0, 200, 0, 100)

TextLabel.Parent = Frame
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.Size = UDim2.new(1, 0, 0.3, 0)
TextLabel.Font = Enum.Font.SourceSans
TextLabel.Text = "AndreiHub"
TextLabel.TextColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.TextSize = 24

Button.Parent = Frame
Button.BackgroundColor3 = Color3.fromRGB(100, 100, 100)
Button.Position = UDim2.new(0.1, 0, 0.5, 0)
Button.Size = UDim2.new(0.8, 0, 0.4, 0)
Button.Font = Enum.Font.SourceSans
Button.Text = "Ativar Haki e Atacar"
Button.TextColor3 = Color3.fromRGB(255, 255, 255)
Button.TextSize = 18

-- Função para ativar o Haki da Observação
function ativarHaki()
    -- Substitua 'instinto' pelo comando específico do jogo para ativar o Haki da Observação
    game.Players.LocalPlayer.Character:FindFirstChild("Instinto"):Activate()
end

-- Função para atacar inimigos
function atacarInimigos()
    while true do
        -- Ativar o Haki da Observação
        ativarHaki()
        -- Código para atacar inimigos
        -- Substitua 'ataque' pelo comando específico do jogo
        game.Players.LocalPlayer.Character:FindFirstChild("Ataque"):Activate()
        -- Aguarde um pouco antes de atacar novamente
        wait(1)
    end
end

-- Função para ativar Haki e atacar quando o botão for clicado
Button.MouseButton1Click:Connect(function()
    atacarInimigos()
end)
-- Script para farmar Haki da Observação no Blox Fruits com painel

-- Criar o painel
local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local TextLabel = Instance.new("TextLabel")
local Button = Instance.new("TextButton")

-- Configurar o painel
ScreenGui.Parent = game.CoreGui

Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
Frame.Position = UDim2.new(0.5, -100, 0.5, -50)
Frame.Size = UDim2.new(0, 200, 0, 100)

TextLabel.Parent = Frame
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.Size = UDim2.new(1, 0, 0.3, 0)
TextLabel.Font = Enum.Font.SourceSans
TextLabel.Text = "AndreiHub"
TextLabel.TextColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.TextSize = 24

Button.Parent = Frame
Button.BackgroundColor3 = Color3.fromRGB(100, 100, 100)
Button.Position = UDim2.new(0.1, 0, 0.5, 0)
Button.Size = UDim2.new(0.8, 0, 0.4, 0)
Button.Font = Enum.Font.SourceSans
Button.Text = "Ativar Haki e Atacar"
Button.TextColor3 = Color3.fromRGB(255, 255, 255)
Button.TextSize = 18

-- Função para ativar o Haki da Observação
function ativarHaki()
    -- Substitua 'instinto' pelo comando específico do jogo para ativar o Haki da Observação
    game.Players.LocalPlayer.Character:FindFirstChild("Instinto"):Activate()
end

-- Função para atacar inimigos
function atacarInimigos()
    while true do
        -- Ativar o Haki da Observação
        ativarHaki()
        -- Código para atacar inimigos
        -- Substitua 'ataque' pelo comando específico do jogo
        game.Players.LocalPlayer.Character:FindFirstChild("Ataque"):Activate()
        -- Aguarde um pouco antes de atacar novamente
        wait(1)
    end
end

-- Função para ativar Haki e atacar quando o botão for clicado
Button.MouseButton1Click:Connect(function()
    atacarInimigos()
end)
