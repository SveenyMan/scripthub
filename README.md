local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

local Window = Rayfield:CreateWindow({
   Name = "Sveen Hub",
   Icon = 0, -- Icon in Topbar. Can use Lucide Icons (string) or Roblox Image (number). 0 to use no icon (default).
   LoadingTitle = "Sveen's Scripts",
   LoadingSubtitle = "Multiple Games",
   Theme = "Amethyst", -- Check https://docs.sirius.menu/rayfield/configuration/themes

   DisableRayfieldPrompts = false,
   DisableBuildWarnings = false, -- Prevents Rayfield from warning when the script has a version mismatch with the interface

   ConfigurationSaving = {
      Enabled = true,
      FolderName = nil, -- Create a custom folder for your hub/game
      FileName = "Big Hub"
   },

   Discord = {
      Enabled = false, -- Prompt the user to join your Discord server if their executor supports it
      Invite = "noinvitelink", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ ABCD would be ABCD
      RememberJoins = true -- Set this to false to make them join the discord every time they load it up
   },

   KeySystem = true, -- Set this to true to use our key system
   KeySettings = {
      Title = "Enter Key",
      Subtitle = "Key System",
      Note = "The Key can be found at:", -- Use this to tell the user how to get a key
      FileName = "Key", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
      SaveKey = true, -- The user's key will be saved, but if you change the key, they will be unable to use your script
      GrabKeyFromSite = false, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
      Key = {"Sveen"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
   }
})

local Tab = Window:CreateTab("The Strongest Battlegrounds")
local Tab2 = Window:CreateTab("Rivals")
local Tab3 = Window:CreateTab("Arsenal")
local Tab4 = Window:CreateTab("Misc")
local Tab5 = Window:CreateTab("Universal")

-- TSB Buttons --
local TSB1 = Tab:CreateButton({
   Name = "Saitama to Gojo",
   Callback = function()
   	getgenv().morph = true
	loadstring(game:HttpGet("https://raw.githubusercontent.com/skibiditoiletfan2007/BaldyToSorcerer/refs/heads/main/LatestV2.lua"))()
   end,
})
local TSB2 = Tab:CreateButton({
   Name = "Garou to Yuji Itadori",
   Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/SveenyMan/Yuji-Moveset-TSB/refs/heads/main/Script"))()
   end,
})
local TSB3 = Tab:CreateButton({
   Name = "Saitama to GoofyMan",
   Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/SveenyMan/Goofy-Man-TSB/refs/heads/main/Script"))()
   end,
})
local TSB4 = Tab:CreateButton({
   Name = "Saitama to Jun",
   Callback = function()
	loadstring(game:HttpGet("https://gist.githubusercontent.com/GoldenHeads2/f66279000c58a020e894a6db44914838/raw/62e53e1acacec0b38b43cd0f594292c32e09c39b/gistfile1.txt"))()
   end,
})
local TSB5 = Tab:CreateButton({
   Name = "Garou to Minos Prime",
   Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/S1gmaGuy/MinosPrimeFixed/refs/heads/main/ThefixIsSoSigma"))()
   end,
})
local TSB6 = Tab:CreateButton({
   Name = "Sonic to 1x1x1x1",
   Callback = function()
	loadstring(game:HttpGet("https://gist.githubusercontent.com/GoldenHeads2/900e87ffc32f3c740930ccb106dd6abf/raw/358c5bf0f0a6aa25946718288dab006e3ae7e1d4/gistfile1.txt"))()
   end,
})
-- End of TSB buttons --

-- Rivals Buttons --
local Rivals1 = Tab2:CreateButton({
   Name = "Aimbot Hub",
   Callback = function()
	loadstring(game:HttpGet("https://soluna-script.vercel.app/main.lua",true))()
   end,
})
-- End of Rivals Buttons --

-- Arsenal Buttons --
local Arsenal1 = Tab3:CreateButton({
   Name = "Aimbot Hub",
   Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/JackyPoopoo/cartel/main/0000000000000000000000000000000000000000000000000"))()
   end,
})
-- End of Arsenal Buttons --

-- Universal Buttons --
local Uni1 = Tab5:CreateButton({
   Name = "Infinite Yield",
   Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source"))()
   end,
})
local Uni2 = Tab5:CreateButton({
   Name = "Dex Explorer",
   Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/infyiff/backup/main/dex.lua"))()
   end,
})
-- End of Universal buttons
