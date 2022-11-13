local whitelistworked;
whitelistworked = getgenv().whitelistworkedgenv
whitelistworked = false
local whitelistnames = {
    "bigabigabigabig",
    "Baristaofplebs100",
}
local whitelistids = {
 19516392511,
 2329494774,
}
print(unpack(whitelistnames))
if game:GetService("Players").LocalPlayer.PlayerGui["All-LeaderboardV2"].MainFrame.ScrollingFrame:FindFirstChild("Player_" ..unpack(whitelistnames)) then
    print(game.Players.LocalPlayer.Name)
    setclipboard(game.Players.LocalPlayer.UserId)
    if game.Players.LocalPlayer.UserId == unpack(whitelistids) then
        print("whitelist")
        getgenv().whitelistworkedgenv = true
        else
            rconsoleprint("No whitelist?")
            game:Shutdown()
            wait(2)
            while true do
                print("Bruh")
                end
end
end
