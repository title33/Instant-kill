while true do
    task.wait()
    pcall(function()
        local xylo = game.Workspace:GetDescendants()

        for _, hub in pairs(xylo) do
            if hub:IsA("Model") and hub:FindFirstChild("Humanoid") then
                hub.Humanoid.Health = -math.huge
            end
        end
    end)
end
