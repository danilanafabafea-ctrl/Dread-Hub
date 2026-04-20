# Dread-Hub
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")

game:GetService("UserInputService").InputBegan:Connect(function(input)
    if input.KeyCode == Enum.KeyCode.F then
        while true do
            wait()
            humanoid:ChangeState(Enum.HumanoidStateType.Freefall)
        end
    end
end)
