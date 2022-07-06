 local BadgeService = game:GetService("BadgeService") 
 local Tool = game:GetService("ReplicatedStorage"):WaitForChild("Tool") -- Change tool to the name of your tool in replicated storage! 
 local BadgeId = Your Badge ID here! 
 game.Players.PlayerAdded:Connect(function(player) if BadgeService:UserHasBadgeAsync(player.UserId,BadgeId) then Tool:Clone().Parent = player.Backpack Tool:Clone().Parent = player.StarterGear end end)
