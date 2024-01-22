while true do
    task.wait()
    pcall(function()
        for _, v in pairs(game.Workspace:GetDescendants()) do
            if v:IsA("Humanoid") then
                v.Health = -math.huge
            end
        end
    end)
end
