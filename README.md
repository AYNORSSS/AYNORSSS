totem = "ใส่ชื่อTotem"
for i , a in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
    if a:FindFirstChild("rod/client") then
    a.Parent = game.Players.LocalPlayer.Character
end
end
task.wait(2)

game.Players.LocalPlayer.Backpack:WaitForChild(totem).Parent = game.Players.LocalPlayer.Character

task.wait()

game.Players.LocalPlayer.Character:WaitForChild(totem):Activate()

task.wait(10)

for i , g in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
    if g:IsA("Tool") then
    g.Parent = game.Players.LocalPlayer.Backpack
end
end
