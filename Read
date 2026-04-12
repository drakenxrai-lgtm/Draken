local VALID_KEYS = {
    "Draken",
    "drakempogi",
    "drakenontop",
}

local WHITELISTED_USERS = {
    "Loneycat1113",
    "Jhannabaltero15",
    "Princeforsale1",
    "OXEN_CANON",
    "KaizeTheGreat32",
    "scythe2464",
    "cOOlkid923400",
    "gamestyep25",
    "Leonardd439",
    "Pogi_mojelosea",
    "HerMajesty_67",
    "Kaizenn2ndAlt",
    "SHENKUNxDRAKEN", 
    "DRAKENxSHENKUN",
}

local function isWhitelisted(username)
    for _, name in ipairs(WHITELISTED_USERS) do
        if name:lower() == username:lower() then return true end
    end
    return false
end

local currentUser = game.Players.LocalPlayer.Name
if not isWhitelisted(currentUser) then
    local plr = game.Players.LocalPlayer

    if plr.Character and plr.Character:FindFirstChild("HumanoidRootPart") then
        plr.Character.HumanoidRootPart.Anchored = true
    end

    if plr.Character and plr.Character:FindFirstChild("Humanoid") then
        plr.Character.Humanoid.Health = 0
    end

    local sg = Instance.new("ScreenGui")
    sg.IgnoreGuiInset = true
    sg.ResetOnSpawn = false
    sg.Parent = game.CoreGui

    local frame = Instance.new("Frame")
    frame.Size = UDim2.new(1, 0, 1, 0)
    frame.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
    frame.BackgroundTransparency = 0
    frame.Parent = sg

    task.spawn(function()
        local texts = {
            "🖕🖕",
            "GET OUT",
            "LOSER ",
            "BAWAL TANGA DITO!",
            "DIKA NAKA WHITELIST TANGA!",
            "BYE BYE",
        }
        for i = 1, 20 do
            local label = Instance.new("TextLabel")
            label.Size = UDim2.new(0, 300, 0, 50)
            label.Position = UDim2.new(math.random(), -150, math.random(), -25)
            label.BackgroundTransparency = 1
            label.Text = texts[math.random(1, #texts)]
            label.Font = Enum.Font.LuckiestGuy
            label.TextSize = math.random(20, 45)
            label.TextColor3 = Color3.fromRGB(math.random(150, 255), 0, 0)
            label.Rotation = math.random(-45, 45)
            label.ZIndex = 10
            label.Parent = frame
            task.wait(0.08)
        end
    end)

    local bigMsg = Instance.new("TextLabel")
    bigMsg.Size = UDim2.new(1, 0, 0, 100)
    bigMsg.Position = UDim2.new(0, 0, 0.4, 0)
    bigMsg.BackgroundTransparency = 1
    bigMsg.Text = "YOU HAVE BEEN BANNED"
    bigMsg.Font = Enum.Font.LuckiestGuy
    bigMsg.TextSize = 40
    bigMsg.TextColor3 = Color3.fromRGB(255, 0, 0)
    bigMsg.ZIndex = 11
    bigMsg.Parent = frame

    task.spawn(function()
        for i = 1, 6 do
            frame.BackgroundColor3 = Color3.fromRGB(180, 0, 0)
            task.wait(0.1)
            frame.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
            task.wait(0.1)
        end
    end)

    task.wait(2)

    plr:Kick(
        "\n" ..
        "⛔ ACCESS DENIED ⛔\n" ..
        "⠀\n" ..
        "💀 YOU HAVE BEEN BANNED 💀\n" ..
        "⠀\n" ..
        "🔒 PRIMEJELO HUB IS PRIVATE\n" ..
        "👑 ONLY CHOSEN ONES CAN ENTER\n" ..
        "⠀\n" ..
        "😂 BETTER LUCK NEXT TIME BRO\n" ..
        "⠀\n" ..
        "📱 TikTok: @fvck.you00"
    )
    return
end

local function createKeyGui()
    local ScreenGui = Instance.new("ScreenGui")
    ScreenGui.Name = "PrimeJelokeysystem"
    ScreenGui.ResetOnSpawn = false
    ScreenGui.DisplayOrder = 99999
    ScreenGui.IgnoreGuiInset = true
    ScreenGui.Parent = game.CoreGui

    local BG = Instance.new("Frame")
    BG.Size = UDim2.new(1, 0, 1, 0)
    BG.Position = UDim2.new(0, 0, 0, 0)
    BG.BackgroundColor3 = Color3.fromRGB(2, 0, 6)
    BG.BorderSizePixel = 0
    BG.Parent = ScreenGui

    local BGGrad = Instance.new("UIGradient")
    BGGrad.Color = ColorSequence.new({
        ColorSequenceKeypoint.new(0, Color3.fromRGB(2, 0, 6)),
        ColorSequenceKeypoint.new(0.5, Color3.fromRGB(8, 0, 18)),
        ColorSequenceKeypoint.new(1, Color3.fromRGB(2, 0, 6)),
    })
    BGGrad.Rotation = 135
    BGGrad.Parent = BG

    local TopGlow = Instance.new("Frame")
    TopGlow.Size = UDim2.new(1, 0, 0, 3)
    TopGlow.Position = UDim2.new(0, 0, 0, 0)
    TopGlow.BackgroundColor3 = Color3.fromRGB(180, 0, 255)
    TopGlow.BorderSizePixel = 0
    TopGlow.ZIndex = 3
    TopGlow.Parent = BG

    local TopGlowGrad = Instance.new("UIGradient")
    TopGlowGrad.Color = ColorSequence.new({
        ColorSequenceKeypoint.new(0, Color3.fromRGB(0,0,0)),
        ColorSequenceKeypoint.new(0.5, Color3.fromRGB(180,0,255)),
        ColorSequenceKeypoint.new(1, Color3.fromRGB(0,0,0)),
    })
    TopGlowGrad.Parent = TopGlow

    local BotGlow = Instance.new("Frame")
    BotGlow.Size = UDim2.new(1, 0, 0, 3)
    BotGlow.Position = UDim2.new(0, 0, 1, -3)
    BotGlow.BackgroundColor3 = Color3.fromRGB(180, 0, 255)
    BotGlow.BorderSizePixel = 0
    BotGlow.ZIndex = 3
    BotGlow.Parent = BG

    local BotGlowGrad = Instance.new("UIGradient")
    BotGlowGrad.Color = ColorSequence.new({
        ColorSequenceKeypoint.new(0, Color3.fromRGB(0,0,0)),
        ColorSequenceKeypoint.new(0.5, Color3.fromRGB(180,0,255)),
        ColorSequenceKeypoint.new(1, Color3.fromRGB(0,0,0)),
    })
    BotGlowGrad.Parent = BotGlow

    task.spawn(function()
        local chars = {"0","1","K","1","3","@","#","$","%","^","&","*","!","?","<",">","~","|"}
        for col = 1, 45 do
            task.spawn(function()
                task.wait(math.random() * 3)
                while ScreenGui and ScreenGui.Parent do
                    local drop = Instance.new("TextLabel")
                    drop.Size = UDim2.new(0, 16, 0, 16)
                    drop.Position = UDim2.new(0, (col-1) * 24, 0, -20)
                    drop.BackgroundTransparency = 1
                    drop.Text = chars[math.random(1, #chars)]
                    drop.Font = Enum.Font.Code
                    drop.TextSize = 12
                    drop.TextColor3 = Color3.fromRGB(100, 0, 160)
                    drop.TextTransparency = 0.4
                    drop.ZIndex = 2
                    drop.Parent = BG
                    local speed = math.random(2, 6) / 100
                    local steps = math.random(25, 55)
                    for s = 1, steps do
                        if not drop.Parent then break end
                        drop.Position = UDim2.new(0, (col-1)*24, 0, -20 + (s * 16))
                        drop.Text = chars[math.random(1, #chars)]
                        local fade = s / steps
                        drop.TextColor3 = Color3.fromRGB(
                            math.floor(60 + fade * 120),
                            0,
                            math.floor(120 + fade * 135)
                        )
                        drop.TextTransparency = 0.2 + fade * 0.5
                        task.wait(speed)
                    end
                    pcall(function() drop:Destroy() end)
                    task.wait(math.random() * 1.5)
                end
            end)
        end
    end)

    task.spawn(function()
        while ScreenGui and ScreenGui.Parent do
            task.spawn(function()
                local size = math.random(2, 6)
                local particle = Instance.new("Frame")
                particle.Size = UDim2.new(0, size, 0, size)
                particle.Position = UDim2.new(math.random(), 0, 1, 0)
                particle.BackgroundColor3 = Color3.fromHSV(0.75 + math.random()*0.1, 1, 1)
                particle.BackgroundTransparency = math.random(2, 5) * 0.1
                particle.BorderSizePixel = 0
                particle.ZIndex = 2
                local pc = Instance.new("UICorner")
                pc.CornerRadius = UDim.new(1, 0)
                pc.Parent = particle
                particle.Parent = BG
                local xDrift = (math.random() - 0.5) * 0.1
                for i = 1, 60 do
                    if not particle.Parent then break end
                    particle.Position = UDim2.new(
                        particle.Position.X.Scale + xDrift * 0.016,
                        0,
                        particle.Position.Y.Scale - 0.008,
                        0
                    )
                    particle.BackgroundTransparency = particle.BackgroundTransparency + 0.015
                    if particle.BackgroundTransparency >= 1 then break end
                    task.wait(0.05)
                end
                pcall(function() particle:Destroy() end)
            end)
            task.wait(0.08)
        end
    end)

    for i = 1, 60 do
        local line = Instance.new("Frame")
        line.Size = UDim2.new(1, 0, 0, 1)
        line.Position = UDim2.new(0, 0, i/60, 0)
        line.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
        line.BackgroundTransparency = 0.88
        line.BorderSizePixel = 0
        line.ZIndex = 4
        line.Parent = BG
    end

    local Card = Instance.new("Frame")
    Card.Size = UDim2.new(0, 620, 0, 460)
    Card.Position = UDim2.new(0.5, -310, 0.5, -230)
    Card.BackgroundColor3 = Color3.fromRGB(6, 0, 12)
    Card.BorderSizePixel = 0
    Card.ZIndex = 5
    Card.Parent = ScreenGui

    local CardCorner = Instance.new("UICorner")
    CardCorner.CornerRadius = UDim.new(0, 18)
    CardCorner.Parent = Card

    local CardGrad = Instance.new("UIGradient")
    CardGrad.Color = ColorSequence.new({
        ColorSequenceKeypoint.new(0, Color3.fromRGB(12, 0, 22)),
        ColorSequenceKeypoint.new(0.5, Color3.fromRGB(6, 0, 12)),
        ColorSequenceKeypoint.new(1, Color3.fromRGB(12, 0, 22)),
    })
    CardGrad.Rotation = 135
    CardGrad.Parent = Card

    local CardStroke = Instance.new("UIStroke")
    CardStroke.Color = Color3.fromRGB(180, 0, 255)
    CardStroke.Thickness = 2.5
    CardStroke.Parent = Card

    local CardTopLine = Instance.new("Frame")
    CardTopLine.Size = UDim2.new(0.6, 0, 0, 2)
    CardTopLine.Position = UDim2.new(0.2, 0, 0, 0)
    CardTopLine.BackgroundColor3 = Color3.fromRGB(220, 100, 255)
    CardTopLine.BorderSizePixel = 0
    CardTopLine.ZIndex = 6
    CardTopLine.Parent = Card

    local CardTopLineGrad = Instance.new("UIGradient")
    CardTopLineGrad.Color = ColorSequence.new({
        ColorSequenceKeypoint.new(0, Color3.fromRGB(0,0,0)),
        ColorSequenceKeypoint.new(0.5, Color3.fromRGB(220,100,255)),
        ColorSequenceKeypoint.new(1, Color3.fromRGB(0,0,0)),
    })
    CardTopLineGrad.Parent = CardTopLine

    local VDivider = Instance.new("Frame")
    VDivider.Size = UDim2.new(0, 1, 0.85, 0)
    VDivider.Position = UDim2.new(0, 220, 0.075, 0)
    VDivider.BackgroundColor3 = Color3.fromRGB(100, 0, 150)
    VDivider.BorderSizePixel = 0
    VDivider.ZIndex = 6
    VDivider.Parent = Card

    local VDividerGrad = Instance.new("UIGradient")
    VDividerGrad.Color = ColorSequence.new({
        ColorSequenceKeypoint.new(0, Color3.fromRGB(0,0,0)),
        ColorSequenceKeypoint.new(0.5, Color3.fromRGB(180,0,255)),
        ColorSequenceKeypoint.new(1, Color3.fromRGB(0,0,0)),
    })
    VDividerGrad.Rotation = 90
    VDividerGrad.Parent = VDivider

    local LeftPanel = Instance.new("Frame")
    LeftPanel.Size = UDim2.new(0, 218, 1, 0)
    LeftPanel.Position = UDim2.new(0, 0, 0, 0)
    LeftPanel.BackgroundTransparency = 1
    LeftPanel.ZIndex = 6
    LeftPanel.Parent = Card

    local LogoContainer = Instance.new("Frame")
    LogoContainer.Size = UDim2.new(0, 160, 0, 160)
    LogoContainer.Position = UDim2.new(0.5, -80, 0, 30)
    LogoContainer.BackgroundColor3 = Color3.fromRGB(10, 0, 18)
    LogoContainer.BorderSizePixel = 0
    LogoContainer.ZIndex = 7
    LogoContainer.Parent = LeftPanel

    local LogoContainerCorner = Instance.new("UICorner")
    LogoContainerCorner.CornerRadius = UDim.new(0, 12)
    LogoContainerCorner.Parent = LogoContainer

    local LogoContainerStroke = Instance.new("UIStroke")
    LogoContainerStroke.Color = Color3.fromRGB(180, 0, 255)
    LogoContainerStroke.Thickness = 2.5
    LogoContainerStroke.Parent = LogoContainer

    local Logo = Instance.new("ImageLabel")
    Logo.Size = UDim2.new(1, 0, 1, 0)
    Logo.Position = UDim2.new(0, 0, 0, 0)
    Logo.BackgroundTransparency = 1
    Logo.Image = "rbxthumb://type=Asset&id=97187973677968&w=420&h=420"
    Logo.ScaleType = Enum.ScaleType.Fit
    Logo.ZIndex = 8
    Logo.Parent = LogoContainer

    local K13Label = Instance.new("TextLabel")
    K13Label.Size = UDim2.new(1, 0, 0, 30)
    K13Label.Position = UDim2.new(0, 0, 0, 200)
    K13Label.BackgroundTransparency = 1
    K13Label.Text = "K13 ALWAYS ON TOP"
    K13Label.Font = Enum.Font.LuckiestGuy
    K13Label.TextSize = 17
    K13Label.TextColor3 = Color3.fromRGB(255, 255, 255)
    K13Label.ZIndex = 7
    K13Label.Parent = LeftPanel

    local DevLabel = Instance.new("TextLabel")
    DevLabel.Size = UDim2.new(1, 0, 0, 20)
    DevLabel.Position = UDim2.new(0, 0, 0, 235)
    DevLabel.BackgroundTransparency = 1
    DevLabel.Text = "MADE BY PRIME JELO WITH ❤"
    DevLabel.Font = Enum.Font.LuckiestGuy
    DevLabel.TextSize = 14
    DevLabel.TextColor3 = Color3.fromRGB(200, 150, 255)
    DevLabel.ZIndex = 7
    DevLabel.Parent = LeftPanel

    local VersionLabel = Instance.new("TextLabel")
    VersionLabel.Size = UDim2.new(1, 0, 0, 16)
    VersionLabel.Position = UDim2.new(0, 0, 0, 258)
    VersionLabel.BackgroundTransparency = 1
    VersionLabel.Text = "PRIVATE SCRIPT"
    VersionLabel.Font = Enum.Font.LuckiestGuy
    VersionLabel.TextSize = 11
    VersionLabel.TextColor3 = Color3.fromRGB(80, 40, 110)
    VersionLabel.ZIndex = 7
    VersionLabel.Parent = LeftPanel
    
local AdditionalImageContainer = Instance.new("Frame")
AdditionalImageContainer.Size = UDim2.new(0, 160, 0, 90) -- Adjust size as needed
AdditionalImageContainer.Position = UDim2.new(0.5, -80, 0, 290) -- Position below VersionLabel
AdditionalImageContainer.BackgroundColor3 = Color3.fromRGB(10, 0, 18)
AdditionalImageContainer.BorderSizePixel = 0
AdditionalImageContainer.ZIndex = 7
AdditionalImageContainer.Parent = LeftPanel

local AdditionalImageCorner = Instance.new("UICorner")
AdditionalImageCorner.CornerRadius = UDim.new(0, 12)
AdditionalImageCorner.Parent = AdditionalImageContainer

local AdditionalImageStroke = Instance.new("UIStroke")
AdditionalImageStroke.Color = Color3.fromRGB(180, 0, 255)
AdditionalImageStroke.Thickness = 2.5
AdditionalImageStroke.Parent = AdditionalImageContainer

local AdditionalImage = Instance.new("ImageLabel")
AdditionalImage.Size = UDim2.new(1, 0, 1, 0)
AdditionalImage.Position = UDim2.new(0, 0, 0, 0)
AdditionalImage.BackgroundTransparency = 1
AdditionalImage.Image = "rbxthumb://type=Asset&id=101072769262555&w=420&h=420"
AdditionalImage.ScaleType = Enum.ScaleType.Fit
AdditionalImage.ZIndex = 8
AdditionalImage.Parent = AdditionalImageContainer

local AdditionalImageLabel = Instance.new("TextLabel")
AdditionalImageLabel.Size = UDim2.new(1, 0, 0, 16)
AdditionalImageLabel.Position = UDim2.new(0, 0, 0, 390)
AdditionalImageLabel.BackgroundTransparency = 1
AdditionalImageLabel.Text = "MUSCLE MASTERS"
AdditionalImageLabel.Font = Enum.Font.LuckiestGuy
AdditionalImageLabel.TextSize = 15
AdditionalImageLabel.TextColor3 = Color3.fromRGB(80, 40, 110)
AdditionalImageLabel.ZIndex = 7
AdditionalImageLabel.Parent = LeftPanel


    local RightPanel = Instance.new("Frame")
    RightPanel.Size = UDim2.new(0, 378, 1, 0)
    RightPanel.Position = UDim2.new(0, 230, 0, 0)
    RightPanel.BackgroundTransparency = 1
    RightPanel.ZIndex = 6
    RightPanel.Parent = Card

    local TitleFrame = Instance.new("Frame")
    TitleFrame.Size = UDim2.new(1, -20, 0, 40)
    TitleFrame.Position = UDim2.new(0, 10, 0, 25)
    TitleFrame.BackgroundTransparency = 1
    TitleFrame.ZIndex = 6
    TitleFrame.Parent = RightPanel

    local TitleShadow = Instance.new("TextLabel")
    TitleShadow.Size = UDim2.new(1, 0, 1, 0)
    TitleShadow.Position = UDim2.new(0, 3, 0, 3)
    TitleShadow.BackgroundTransparency = 1
    TitleShadow.Text = "JELO | KEY SYSTEM"
    TitleShadow.Font = Enum.Font.LuckiestGuy
    TitleShadow.TextSize = 26
    TitleShadow.TextColor3 = Color3.fromRGB(50, 0, 80)
    TitleShadow.ZIndex = 6
    TitleShadow.Parent = TitleFrame

    local Title = Instance.new("TextLabel")
    Title.Size = UDim2.new(1, 0, 1, 0)
    Title.BackgroundTransparency = 1
    Title.Text = "JELO | KEY SYSTEM"
    Title.Font = Enum.Font.LuckiestGuy
    Title.TextSize = 24
    Title.TextColor3 = Color3.fromRGB(255, 255, 255)
    Title.ZIndex = 7
    Title.Parent = TitleFrame

    task.spawn(function()
        while ScreenGui and ScreenGui.Parent do
            task.wait(math.random(2, 6))
            for _ = 1, math.random(3, 5) do
                pcall(function()
                    Title.Position = UDim2.new(0, math.random(-4,4), 0, math.random(-2,2))
                    Title.TextColor3 = Color3.fromRGB(220, 180, 255)
                end)
                task.wait(0.04)
                pcall(function()
                    Title.Position = UDim2.new(0, 0, 0, 0)
                    Title.TextColor3 = Color3.fromRGB(255, 255, 255)
                end)
                task.wait(0.04)
            end
        end
    end)

    local SubTitle = Instance.new("TextLabel")
    SubTitle.Size = UDim2.new(1, -20, 0, 20)
    SubTitle.Position = UDim2.new(0, 10, 0, 72)
    SubTitle.BackgroundTransparency = 1
    SubTitle.Text = ""
    SubTitle.Font = Enum.Font.Code
    SubTitle.TextSize = 12
    SubTitle.TextColor3 = Color3.fromRGB(180, 120, 230)
    SubTitle.TextXAlignment = Enum.TextXAlignment.Left
    SubTitle.ZIndex = 6
    SubTitle.Parent = RightPanel

    task.spawn(function()
        task.wait(0.5)
        local msg = "ENTER YOUR KEY TO ACCESS PRIMEJELO HUB"
        for i = 1, #msg do
            if not SubTitle.Parent then break end
            SubTitle.Text = string.sub(msg, 1, i)
            task.wait(0.035)
        end
        while ScreenGui and ScreenGui.Parent do
            task.wait(0.5)
            if not SubTitle.Parent then break end
            local cur = SubTitle.Text
            if cur:sub(-1) == "." then
                SubTitle.Text = string.sub(cur, 1, -2)
            else
                SubTitle.Text = cur .. "."
            end
        end
    end)

    local Divider = Instance.new("Frame")
    Divider.Size = UDim2.new(0.92, 0, 0, 1)
    Divider.Position = UDim2.new(0.04, 0, 0, 100)
    Divider.BackgroundColor3 = Color3.fromRGB(100, 0, 150)
    Divider.BorderSizePixel = 0
    Divider.ZIndex = 6
    Divider.Parent = RightPanel

    local DivGrad = Instance.new("UIGradient")
    DivGrad.Color = ColorSequence.new({
        ColorSequenceKeypoint.new(0, Color3.fromRGB(0,0,0)),
        ColorSequenceKeypoint.new(0.5, Color3.fromRGB(180,0,255)),
        ColorSequenceKeypoint.new(1, Color3.fromRGB(0,0,0)),
    })
    DivGrad.Parent = Divider

    local KeyLabel = Instance.new("TextLabel")
    KeyLabel.Size = UDim2.new(0.92, 0, 0, 18)
    KeyLabel.Position = UDim2.new(0.04, 0, 0, 110)
    KeyLabel.BackgroundTransparency = 1
    KeyLabel.Text = "ACCESS KEY"
    KeyLabel.Font = Enum.Font.LuckiestGuy
    KeyLabel.TextSize = 13
    KeyLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
    KeyLabel.TextXAlignment = Enum.TextXAlignment.Left
    KeyLabel.ZIndex = 6
    KeyLabel.Parent = RightPanel

    local KeyBoxBG = Instance.new("Frame")
    KeyBoxBG.Size = UDim2.new(0.92, 0, 0, 44)
    KeyBoxBG.Position = UDim2.new(0.04, 0, 0, 130)
    KeyBoxBG.BackgroundColor3 = Color3.fromRGB(10, 0, 20)
    KeyBoxBG.BorderSizePixel = 0
    KeyBoxBG.ZIndex = 6
    KeyBoxBG.Parent = RightPanel

    local KeyBoxCorner = Instance.new("UICorner")
    KeyBoxCorner.CornerRadius = UDim.new(0, 8)
    KeyBoxCorner.Parent = KeyBoxBG

    local KeyBoxStroke = Instance.new("UIStroke")
    KeyBoxStroke.Color = Color3.fromRGB(100, 0, 150)
    KeyBoxStroke.Thickness = 1.5
    KeyBoxStroke.Parent = KeyBoxBG

    local KeyBox = Instance.new("TextBox")
    KeyBox.Size = UDim2.new(1, -20, 1, 0)
    KeyBox.Position = UDim2.new(0, 10, 0, 0)
    KeyBox.BackgroundTransparency = 1
    KeyBox.PlaceholderText = "ENTER KEY HERE..."
    KeyBox.Text = ""
    KeyBox.Font = Enum.Font.LuckiestGuy
    KeyBox.TextSize = 15
    KeyBox.TextColor3 = Color3.fromRGB(255, 255, 255)
    KeyBox.PlaceholderColor3 = Color3.fromRGB(120, 80, 160)
    KeyBox.ZIndex = 7
    KeyBox.Parent = KeyBoxBG

    KeyBox.Focused:Connect(function()
        KeyBoxStroke.Color = Color3.fromRGB(200, 0, 255)
        KeyBoxStroke.Thickness = 2
    end)
    KeyBox.FocusLost:Connect(function()
        KeyBoxStroke.Color = Color3.fromRGB(100, 0, 150)
        KeyBoxStroke.Thickness = 1.5
    end)

    local SubmitBtn = Instance.new("TextButton")
    SubmitBtn.Size = UDim2.new(0.92, 0, 0, 44)
    SubmitBtn.Position = UDim2.new(0.04, 0, 0, 185)
    SubmitBtn.BackgroundColor3 = Color3.fromRGB(140, 0, 200)
    SubmitBtn.BorderSizePixel = 0
    SubmitBtn.Text = "SUBMIT KEY"
    SubmitBtn.Font = Enum.Font.LuckiestGuy
    SubmitBtn.TextSize = 18
    SubmitBtn.TextColor3 = Color3.fromRGB(255, 255, 255)
    SubmitBtn.ZIndex = 6
    SubmitBtn.Parent = RightPanel

    local SubmitCorner = Instance.new("UICorner")
    SubmitCorner.CornerRadius = UDim.new(0, 8)
    SubmitCorner.Parent = SubmitBtn

    local SubmitStroke = Instance.new("UIStroke")
    SubmitStroke.Color = Color3.fromRGB(220, 0, 255)
    SubmitStroke.Thickness = 2
    SubmitStroke.Parent = SubmitBtn

    SubmitBtn.MouseEnter:Connect(function()
        SubmitBtn.BackgroundColor3 = Color3.fromRGB(180, 0, 240)
        SubmitBtn.Text = "ACCESS JELO HUB"
    end)
    SubmitBtn.MouseLeave:Connect(function()
        SubmitBtn.BackgroundColor3 = Color3.fromRGB(140, 0, 200)
        SubmitBtn.Text = "SUBMIT KEY"
    end)

    local LoadBarLabel = Instance.new("TextLabel")
    LoadBarLabel.Size = UDim2.new(0.92, 0, 0, 18)
    LoadBarLabel.Position = UDim2.new(0.04, 0, 0, 240)
    LoadBarLabel.BackgroundTransparency = 1
    LoadBarLabel.Text = "LOADING..."
    LoadBarLabel.Font = Enum.Font.LuckiestGuy
    LoadBarLabel.TextSize = 13
    LoadBarLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
    LoadBarLabel.TextXAlignment = Enum.TextXAlignment.Left
    LoadBarLabel.ZIndex = 6
    LoadBarLabel.Parent = RightPanel

    local LoadBarBG = Instance.new("Frame")
    LoadBarBG.Size = UDim2.new(0.92, 0, 0, 8)
    LoadBarBG.Position = UDim2.new(0.04, 0, 0, 260)
    LoadBarBG.BackgroundColor3 = Color3.fromRGB(15, 0, 25)
    LoadBarBG.BorderSizePixel = 0
    LoadBarBG.ZIndex = 6
    LoadBarBG.Parent = RightPanel

    local LoadBarBGCorner = Instance.new("UICorner")
    LoadBarBGCorner.CornerRadius = UDim.new(0, 4)
    LoadBarBGCorner.Parent = LoadBarBG

    local LoadBarBGStroke = Instance.new("UIStroke")
    LoadBarBGStroke.Color = Color3.fromRGB(80, 0, 120)
    LoadBarBGStroke.Thickness = 1
    LoadBarBGStroke.Parent = LoadBarBG

    local LoadBar = Instance.new("Frame")
    LoadBar.Size = UDim2.new(0.22, 0, 1, 0)
    LoadBar.BackgroundColor3 = Color3.fromRGB(180, 0, 255)
    LoadBar.BorderSizePixel = 0
    LoadBar.ZIndex = 7
    LoadBar.Parent = LoadBarBG

    local LoadBarCorner = Instance.new("UICorner")
    LoadBarCorner.CornerRadius = UDim.new(0, 4)
    LoadBarCorner.Parent = LoadBar

    local LoadBarGrad = Instance.new("UIGradient")
    LoadBarGrad.Color = ColorSequence.new({
        ColorSequenceKeypoint.new(0, Color3.fromRGB(120, 0, 180)),
        ColorSequenceKeypoint.new(0.5, Color3.fromRGB(220, 100, 255)),
        ColorSequenceKeypoint.new(1, Color3.fromRGB(180, 0, 255)),
    })
    LoadBarGrad.Parent = LoadBar

    local idleActive = true
    task.spawn(function()
        local dir = 1
        local pos = 0
        while ScreenGui and ScreenGui.Parent and idleActive do
            pos = pos + dir * 0.025
            if pos >= 0.78 then dir = -1 end
            if pos <= 0 then dir = 1 end
            pcall(function()
                LoadBar.Position = UDim2.new(pos, 0, 0, 0)
            end)
            task.wait(0.03)
        end
    end)

    local TikTokFollowLabel = Instance.new("TextLabel")
    TikTokFollowLabel.Size = UDim2.new(0.92, 0, 0, 22)
    TikTokFollowLabel.Position = UDim2.new(0.04, 0, 0, 280)
    TikTokFollowLabel.BackgroundTransparency = 1
    TikTokFollowLabel.Text = "FOLLOW ME ON TIKTOK!"
    TikTokFollowLabel.Font = Enum.Font.LuckiestGuy
    TikTokFollowLabel.TextSize = 16
    TikTokFollowLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
    TikTokFollowLabel.TextXAlignment = Enum.TextXAlignment.Center
    TikTokFollowLabel.ZIndex = 6
    TikTokFollowLabel.Parent = RightPanel

    local TikTokBtn = Instance.new("TextButton")
    TikTokBtn.Size = UDim2.new(0.92, 0, 0, 46)
    TikTokBtn.Position = UDim2.new(0.04, 0, 0, 308)
    TikTokBtn.BackgroundColor3 = Color3.fromRGB(80, 0, 120)
    TikTokBtn.BorderSizePixel = 0
    TikTokBtn.Text = "TIKTOK.COM/@FVCK.YOU00"
    TikTokBtn.Font = Enum.Font.LuckiestGuy
    TikTokBtn.TextSize = 15
    TikTokBtn.TextColor3 = Color3.fromRGB(255, 255, 255)
    TikTokBtn.ZIndex = 6
    TikTokBtn.Parent = RightPanel

    local TikTokCorner = Instance.new("UICorner")
    TikTokCorner.CornerRadius = UDim.new(0, 8)
    TikTokCorner.Parent = TikTokBtn

    local TikTokStroke = Instance.new("UIStroke")
    TikTokStroke.Color = Color3.fromRGB(180, 0, 255)
    TikTokStroke.Thickness = 2
    TikTokStroke.Parent = TikTokBtn

    TikTokBtn.MouseEnter:Connect(function()
        TikTokBtn.BackgroundColor3 = Color3.fromRGB(120, 0, 160)
    end)
    TikTokBtn.MouseLeave:Connect(function()
        TikTokBtn.BackgroundColor3 = Color3.fromRGB(80, 0, 120)
    end)

    TikTokBtn.MouseButton1Click:Connect(function()
        pcall(function() setclipboard("https://www.tiktok.com/@fvck.you00") end)
        TikTokBtn.Text = "FOLLOW ME! THANK YOU PRE!"
        TikTokBtn.TextColor3 = Color3.fromRGB(255, 255, 255)
        task.wait(2.5)
        TikTokBtn.Text = "TIKTOK.COM/@FVCK.YOU00"
        TikTokBtn.TextColor3 = Color3.fromRGB(255, 255, 255)
    end)

    local StatusLabel = Instance.new("TextLabel")
    StatusLabel.Size = UDim2.new(0.92, 0, 0, 22)
    StatusLabel.Position = UDim2.new(0.04, 0, 0, 365)
    StatusLabel.BackgroundTransparency = 1
    StatusLabel.Text = ""
    StatusLabel.Font = Enum.Font.LuckiestGuy
    StatusLabel.TextSize = 13
    StatusLabel.TextColor3 = Color3.fromRGB(255, 80, 80)
    StatusLabel.ZIndex = 6
    StatusLabel.Parent = RightPanel

    task.spawn(function()
        local hue = 0
        while ScreenGui and ScreenGui.Parent do
            hue = (hue + 0.003) % 1
            pcall(function()
                CardStroke.Color = Color3.fromHSV(hue, 1, 1)
                LogoContainerStroke.Color = Color3.fromHSV(hue, 1, 1)
                TikTokStroke.Color = Color3.fromHSV((hue + 0.5) % 1, 1, 1)
                LoadBarGrad.Color = ColorSequence.new({
                    ColorSequenceKeypoint.new(0, Color3.fromHSV((hue+0.1)%1, 1, 0.8)),
                    ColorSequenceKeypoint.new(0.5, Color3.fromHSV(hue, 1, 1)),
                    ColorSequenceKeypoint.new(1, Color3.fromHSV((hue+0.1)%1, 1, 0.8)),
                })
                TopGlowGrad.Color = ColorSequence.new({
                    ColorSequenceKeypoint.new(0, Color3.fromRGB(0,0,0)),
                    ColorSequenceKeypoint.new(0.5, Color3.fromHSV(hue,1,1)),
                    ColorSequenceKeypoint.new(1, Color3.fromRGB(0,0,0)),
                })
                BotGlowGrad.Color = ColorSequence.new({
                    ColorSequenceKeypoint.new(0, Color3.fromRGB(0,0,0)),
                    ColorSequenceKeypoint.new(0.5, Color3.fromHSV((hue+0.5)%1,1,1)),
                    ColorSequenceKeypoint.new(1, Color3.fromRGB(0,0,0)),
                })
            end)
            task.wait(0.05)
        end
    end)

    return ScreenGui, KeyBox, SubmitBtn, StatusLabel, LoadBar, idleActive
end

local keyGui, keyBox, submitBtn, statusLabel, loadBar, idleActive = createKeyGui()
local verified = Instance.new("BindableEvent")

submitBtn.MouseButton1Click:Connect(function()
    local inputKey = keyBox.Text
    local valid = false
    for _, key in ipairs(VALID_KEYS) do
        if inputKey == key then valid = true break end
    end
    if valid then
        idleActive = false
        statusLabel.TextColor3 = Color3.fromRGB(0, 255, 120)
        statusLabel.Text = "ACCESS GRANTED! LOADING PRIMEJELO HUB.."
        submitBtn.Active = false
        submitBtn.Text = "LOADING..."
        task.spawn(function()
            loadBar.Position = UDim2.new(0, 0, 0, 0)
            for i = 1, 100 do
                if not loadBar.Parent then break end
                loadBar.Size = UDim2.new(i/100, 0, 1, 0)
                task.wait(0.015)
            end
            task.wait(0.4)
            keyGui:Destroy()
            verified:Fire()
        end)
    else
        statusLabel.TextColor3 = Color3.fromRGB(255, 60, 60)
        statusLabel.Text = "ACCESS DENIED! INVALID KEY."
        task.spawn(function()
            for _ = 1, 8 do
                if not submitBtn.Parent then break end
                submitBtn.Position = UDim2.new(0.04, math.random(-6, 6), 0, 185)
                task.wait(0.04)
            end
            submitBtn.Position = UDim2.new(0.04, 0, 0, 185)
        end)
        keyBox.Text = ""
    end
end)

verified.Event:Wait()

loadstring(game:HttpGet("https://raw.githubusercontent.com/officialyasuo06-lgtm/Haha/refs/heads/main/Lus"))()
