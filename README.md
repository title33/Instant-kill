game:GetService("Players").LocalPlayer.OnTeleport:Connect(function(A, B, C)
    if A == Enum.TeleportState.InProgress then
        if game:IsLoaded() then
        print("Test")
        end
    end
end)
