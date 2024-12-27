-- Criando a GUI
local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local Button1 = Instance.new("TextButton")
local Button2 = Instance.new("TextButton")

-- Definindo propriedades da GUI
ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
Frame.Parent = ScreenGui
Frame.Position = UDim2.new(0.5, -100, 0.5, -100)
Frame.Size = UDim2.new(0, 200, 0, 200)
Frame.BackgroundColor3 = Color3.fromRGB(0, 0, 0)

Button1.Parent = Frame
Button1.Size = UDim2.new(0, 180, 0, 50)
Button1.Position = UDim2.new(0, 10, 0, 10)
Button1.Text = "Executar Infinite Yield"
Button1.BackgroundColor3 = Color3.fromRGB(0, 255, 0)

Button2.Parent = Frame
Button2.Size = UDim2.new(0, 180, 0, 50)
Button2.Position = UDim2.new(0, 10, 0, 70)
Button2.Text = "Executar MM2 Script"
Button2.BackgroundColor3 = Color3.fromRGB(255, 0, 0)

-- Função para executar os scripts
Button1.MouseButton1Click:Connect(function()
    print("Executando Infinite Yield...")
    loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
end)

Button2.MouseButton1Click:Connect(function()
