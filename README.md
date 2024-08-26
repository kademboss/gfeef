local player = game.Players.LocalPlayer
 
local playerGui = player.PlayerGui
 
local hotbar = playerGui:FindFirstChild("Hotbar")
 
local backpack = hotbar:FindFirstChild("Backpack")
 
local hotbarFrame = backpack:FindFirstChild("Hotbar")
 
local baseButton = hotbarFrame:FindFirstChild("1").Base
 
local ToolName = baseButton.ToolName
 
 
ToolName.Text = "Repulse"
 
 
local player = game.Players.LocalPlayer
 
local playerGui = player.PlayerGui
 
local hotbar = playerGui:FindFirstChild("Hotbar")
 
local backpack = hotbar:FindFirstChild("Backpack")
 
local hotbarFrame = backpack:FindFirstChild("Hotbar")
 
local baseButton = hotbarFrame:FindFirstChild("2").Base
 
local ToolName = baseButton.ToolName
 
 
ToolName.Text = "Attract"
 
 
local player = game.Players.LocalPlayer
 
local playerGui = player.PlayerGui
 
local hotbar = playerGui:FindFirstChild("Hotbar")
 
local backpack = hotbar:FindFirstChild("Backpack")
 
local hotbarFrame = backpack:FindFirstChild("Hotbar")
 
local baseButton = hotbarFrame:FindFirstChild("3").Base
 
local ToolName = baseButton.ToolName
 
 
ToolName.Text = "Erase"
 
 
local player = game.Players.LocalPlayer
 
local playerGui = player.PlayerGui
 
local hotbar = playerGui:FindFirstChild("Hotbar")
 
local backpack = hotbar:FindFirstChild("Backpack")
 
local hotbarFrame = backpack:FindFirstChild("Hotbar")
 
local baseButton = hotbarFrame:FindFirstChild("4").Base
 
local ToolName = baseButton.ToolName
 
 
ToolName.Text = "Infinity"
 
 
local Players = game:GetService("Players")
 
local player = Players.LocalPlayer
 
local playerGui = player:WaitForChild("PlayerGui")
 
 
local function findGuiAndSetText()
 
    local screenGui = playerGui:FindFirstChild("ScreenGui")
 
    if screenGui then
 
        local magicHealthFrame = screenGui:FindFirstChild("MagicHealth")
 
        if magicHealthFrame then
 
            local textLabel = magicHealthFrame:FindFirstChild("TextLabel")
 
            if textLabel then
 
                textLabel.Text = "SORCERER"
 
            end
 
        end
 
    end
 
end
 
 
playerGui.DescendantAdded:Connect(findGuiAndSetText)
 
findGuiAndSetText()
 
 
local animationId = 10468665991 ---- Get normal punch anim id
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://16552234590" ---- Change to repulse anim id
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0
 
 
Anim:Play()
 
Anim:AdjustSpeed(0)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(0.6)
 
 
    end
 
end
  
humanoid.AnimationPlayed:Connect(onAnimationPlayed)
 
 
local animationId = 10466974800 ---- Same thing consecutive punches
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://15290930205" ---- Changes to toji barrage
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0
 
 
Anim:Play()
 
Anim:AdjustSpeed(0.1)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(1.4)
 
 
    end
 
end
 
 
humanoid.AnimationPlayed:Connect(onAnimationPlayed)
 
 
local animationId = 10471336737 ---- shove
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://17889461810" ---- uhhhh the 
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
---- local startTime = 0.5 
 
 
Anim:Play()
 
Anim:AdjustSpeed(0)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(1.4)
 
 
delay(1.8, function()
 
    Anim:Stop()
 
end)
 
 
    end
 
end
 
 
humanoid.AnimationPlayed:Connect(onAnimationPlayed)
 
 
local animationId = 12510170988 ---- wallcombo anim
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://17464644182" ---- woahhhh gojo wallcumbo
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0
 
 
Anim:Play()
 
Anim:AdjustSpeed(0)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(0.95)
wait(1.10)
Anim:Stop()
 
    end
 
end
 
humanoid.AnimationPlayed:Connect(onAnimationPlayed)
 
local animationId = 11343318134 ---- umpeprcut
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://17464644182" ---- psychic ricochet
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0
 
Anim:Play()
 
Anim:AdjustSpeed(0)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(0.3)

wait(3)

Anim:Stop()
 
 
    end
 
end
 
humanoid.AnimationPlayed:Connect(onAnimationPlayed)
 
local animationId = 15955393872 ---- idfk i forgot honestly
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://18903642853" ---- ohh yeah gojo awk
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0
 
 
Anim:Play()
 
Anim:AdjustSpeed(0)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(1.45)

local TweenService = game:GetService("TweenService")
local player = game.Players.LocalPlayer
local humanoidRootPart = player.Character and player.Character:FindFirstChild("HumanoidRootPart")
if not humanoidRootPart then return end -- Exit if the player's character is not loaded yet

local speedFactor = 2 -- Speed factor to adjust tween durations
local effectDistance = 7 -- Distance to place effects in front of the player (increased from 3 to 6)

local function flipAndPositionCFrame(baseCFrame, distance)
    -- Flip the effect and position it a bit further from the player
    return baseCFrame * CFrame.new(0, 0, -distance) * CFrame.Angles(0, math.pi, 0)
end

-- Function to ensure the model has a PrimaryPart set
local function ensurePrimaryPart(model)
    if not model.PrimaryPart then
        -- Set PrimaryPart to the first part found if not set
        model.PrimaryPart = model:FindFirstChildWhichIsA("BasePart")
    end
end

-- Clone and setup effects
local wallFX = game.ReplicatedStorage.Resources.Sorcerer.WallFX:Clone()
ensurePrimaryPart(wallFX)
wallFX.Parent = workspace.Thrown
wallFX:SetPrimaryPartCFrame(flipAndPositionCFrame(humanoidRootPart.CFrame, effectDistance)) -- Flipping and positioning

local lighting = game.ReplicatedStorage.Resources.Sorcerer.Lighting:Clone()
lighting.Parent = game.Lighting

local limitlessBarrier = game.ReplicatedStorage.Resources.Sorcerer.LimitlessBarrier:Clone()
ensurePrimaryPart(limitlessBarrier)
limitlessBarrier.Parent = workspace.Thrown
limitlessBarrier:SetPrimaryPartCFrame(flipAndPositionCFrame(humanoidRootPart.CFrame, effectDistance)) -- Flipping and positioning

-- Cleanup the limitless barrier after adjusted time
task.delay(10 / speedFactor, function()
    limitlessBarrier:Destroy()
end)

local sphere = limitlessBarrier.Sphere

-- Emit particles after a short delay
task.delay(0.085 / speedFactor, function()
    for _, particleEmitter in pairs(wallFX.FirstSlam:GetDescendants()) do
        if particleEmitter:IsA("ParticleEmitter") then
            particleEmitter:Emit(particleEmitter:GetAttribute("EmitCount"))
        end
    end
end)

task.delay(1.26 / speedFactor, function()
    task.spawn(function()
        local colorCorrection = Instance.new("ColorCorrectionEffect")
        colorCorrection.Name = "cloned"
        colorCorrection.Parent = game.Lighting

        local barrierScreen = lighting.BarrierScreen
        TweenService:Create(colorCorrection, TweenInfo.new(0.35 / speedFactor, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
            Brightness = barrierScreen.Brightness,
            Contrast = barrierScreen.Contrast,
            Saturation = barrierScreen.Saturation,
            TintColor = barrierScreen.TintColor
        }):Play()

        task.wait(2 / speedFactor)
        TweenService:Create(colorCorrection, TweenInfo.new(0.6 / speedFactor, Enum.EasingStyle.Quad, Enum.EasingDirection.InOut), {
            Brightness = 0,
            Contrast = 0,
            Saturation = 0
        }):Play()
        
        task.wait(1 / speedFactor)
        colorCorrection:Destroy()
    end)

    task.spawn(function()
        wallFX.Final.BarrierCrater.Transparency = 0
        wallFX.Final.FinalCrater.Transparency = 0
        wallFX.Final.FinalCrater.Color3 = Color3.fromRGB(100, 600, 2000)

        TweenService:Create(wallFX.Final.FinalCrater, TweenInfo.new(4 / speedFactor, Enum.EasingStyle.Quint, Enum.EasingDirection.InOut), {
            Color3 = Color3.fromRGB(0, 0, 0),
            Transparency = 1
        }):Play()

        task.wait(5 / speedFactor)
        TweenService:Create(wallFX.Final.BarrierCrater, TweenInfo.new(3 / speedFactor, Enum.EasingStyle.Cubic, Enum.EasingDirection.InOut), {
            Transparency = 1
        }):Play()
    end)

    task.spawn(function()
        local camera = workspace.CurrentCamera
        TweenService:Create(camera, TweenInfo.new(0.6 / speedFactor, Enum.EasingStyle.Back, Enum.EasingDirection.Out), {
            FieldOfView = 80
        }):Play()

        task.wait(2.14 / speedFactor)
        TweenService:Create(camera, TweenInfo.new(1.35 / speedFactor, Enum.EasingStyle.Quad, Enum.EasingDirection.InOut), {
            FieldOfView = 65
        }):Play()
    end)

    local appear = limitlessBarrier.Core.Appear
    for _, particleEmitter in pairs(appear:GetDescendants()) do
        if particleEmitter:IsA("ParticleEmitter") then
            particleEmitter:Emit(particleEmitter.Name)
        end
    end

    local barrierFX = limitlessBarrier.Core.BarrierFX
    for _, particleEmitter in pairs(barrierFX:GetDescendants()) do
        if particleEmitter:IsA("ParticleEmitter") then
            particleEmitter.Enabled = true
        end
    end

    task.delay(2 / speedFactor, function()
        local barrierFX = limitlessBarrier.Core.BarrierFX
        for _, particleEmitter in pairs(barrierFX:GetDescendants()) do
            if particleEmitter:IsA("ParticleEmitter") then
                particleEmitter.Enabled = false
            end
        end
    end)

    local beamRings = limitlessBarrier.Core.BeamRings
    for _, beam in pairs(beamRings:GetDescendants()) do
        if beam:IsA("Beam") then
            beam.Enabled = true
            TweenService:Create(beam, TweenInfo.new(2.15 / speedFactor, Enum.EasingStyle.Quad, Enum.EasingDirection.InOut), {
                Brightness = 0
            }):Play()
        end
    end

    local function createFlippedWindRing(rotationAngle)
        local windRing = limitlessBarrier.WindRing:Clone()
        ensurePrimaryPart(windRing)
        windRing:SetPrimaryPartCFrame(flipAndPositionCFrame(humanoidRootPart.CFrame, effectDistance))

        local start = windRing.Start
        local endPos = windRing.End

        local clonedMesh = start:Clone()
        clonedMesh.Name = "ClonedMesh"
        clonedMesh.Parent = limitlessBarrier.CurrentTweens

        TweenService:Create(clonedMesh.Decal, TweenInfo.new(0.2 / speedFactor, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut), {
            Transparency = 0.9
        }):Play()

        TweenService:Create(clonedMesh, TweenInfo.new(1 / speedFactor, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
            Size = endPos.Size,
            CFrame = endPos.CFrame
        }):Play()

        TweenService:Create(clonedMesh.Mesh, TweenInfo.new(1 / speedFactor, Enum.EasingStyle.Quint, Enum.EasingDirection.Out), {
            Scale = endPos.Mesh.Scale
        }):Play()

        task.wait(0.2 / speedFactor)
        TweenService:Create(clonedMesh.Decal, TweenInfo.new(1 / speedFactor, Enum.EasingStyle.Cubic, Enum.EasingDirection.Out), {
            Transparency = 1
        }):Play()

        task.wait(1.2 / speedFactor)
        clonedMesh:Destroy()
    end

    local function createFlippedSphereEffect()
        local randomSize = Random.new():NextNumber(24, 26)
        local clonedSphere = sphere:Clone()
        clonedSphere.Name = "Cloned"
        clonedSphere.Parent = limitlessBarrier.CurrentTweens
        clonedSphere.CFrame = flipAndPositionCFrame(humanoidRootPart.CFrame, effectDistance)

        TweenService:Create(clonedSphere, TweenInfo.new(0.3 / speedFactor, Enum.EasingStyle.Cubic, Enum.EasingDirection.Out), {
            Size = Vector3.new(randomSize, randomSize, randomSize),
            Transparency = 3.65
        }):Play()

        task.wait(0.3 / speedFactor)
        TweenService:Create(clonedSphere, TweenInfo.new(0.3 / speedFactor, Enum.EasingStyle.Sine, Enum.EasingDirection.Out), {
            Size = Vector3.new(0, 0, 0),
            Transparency = 1
        }):Play()

        task.wait(0.3 / speedFactor)
        clonedSphere:Destroy()
    end

    task.spawn(function()
        for i = 1, 13 do
            spawn(function() createFlippedSphereEffect() end)
            task.wait(0.15 / speedFactor)
        end
    end)

    for i = 1, 13 do
        spawn(function() createFlippedWindRing() end)
        task.wait(0.15 / speedFactor)
    end
end)

task.delay(3.8 / speedFactor, function()
    local endEmit = limitlessBarrier.Core.EndEmit
    for _, particleEmitter in pairs(endEmit:GetDescendants()) do
        if particleEmitter:IsA("ParticleEmitter") then
            particleEmitter:Emit(particleEmitter:GetAttribute("EmitCount"))
        end
    end

    local final = wallFX.Final
    for _, particleEmitter in pairs(final:GetDescendants()) do
        if particleEmitter:IsA("ParticleEmitter") then
            particleEmitter:Emit(particleEmitter:GetAttribute("EmitCount"))
        end
    end

    task.spawn(function()
        local impactFrameWhite = lighting.ImpactFrameWhite
        impactFrameWhite.Enabled = true
        task.wait(0.045 / speedFactor)
        impactFrameWhite.Enabled = false
        impactFrameWhite.Enabled = true
        task.wait(0.045 / speedFactor)
        impactFrameWhite.Enabled = false

        local clonedBarrierFinal = lighting.BarrierFinal:Clone()
        clonedBarrierFinal.Name = "cloned2"
        clonedBarrierFinal.Parent = game.Lighting
        TweenService:Create(clonedBarrierFinal, TweenInfo.new(0.6 / speedFactor, Enum.EasingStyle.Quint, Enum.EasingDirection.Out), {
            Brightness = 0,
            Contrast = 0,
            Saturation = 0,
            TintColor = Color3.fromRGB(255, 255, 255)
        }):Play()

        task.wait(1.5 / speedFactor)
        clonedBarrierFinal:Destroy()
    end)

    task.spawn(function()
        local camera = workspace.CurrentCamera
        TweenService:Create(camera, TweenInfo.new(0.2 / speedFactor, Enum.EasingStyle.Cubic, Enum.EasingDirection.Out), {
            FieldOfView = 98
        }):Play()

        task.wait(0.2 / speedFactor)
        TweenService:Create(camera, TweenInfo.new(0.5 / speedFactor, Enum.EasingStyle.Quad, Enum.EasingDirection.InOut), {
            FieldOfView = 70
        }):Play()
    end)

    task.spawn(function()
        local windRing = limitlessBarrier.WindRing:Clone()
        ensurePrimaryPart(windRing)
        windRing:SetPrimaryPartCFrame(flipAndPositionCFrame(humanoidRootPart.CFrame, effectDistance))

        local start = windRing.Start
        local endPos = windRing.End2

        local clonedMesh = start:Clone()
        clonedMesh.Name = "ClonedMesh"
        clonedMesh.Parent = limitlessBarrier.CurrentTweens

        TweenService:Create(clonedMesh.Decal, TweenInfo.new(0.2 / speedFactor, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut), {
            Transparency = 0.9
        }):Play()

        TweenService:Create(clonedMesh, TweenInfo.new(5 / speedFactor, Enum.EasingStyle.Exponential, Enum.EasingDirection.Out), {
            Size = endPos.Size,
            CFrame = endPos.CFrame
        }):Play()

        TweenService:Create(clonedMesh.Mesh, TweenInfo.new(5 / speedFactor, Enum.EasingStyle.Exponential, Enum.EasingDirection.Out), {
            Scale = endPos.Mesh.Scale
        }):Play()

        task.wait(0.2 / speedFactor)
        TweenService:Create(clonedMesh.Decal, TweenInfo.new(5 / speedFactor, Enum.EasingStyle.Cubic, Enum.EasingDirection.Out), {
            Transparency = 1
        }):Play()

        task.wait(5.2 / speedFactor)
        clonedMesh:Destroy()
    end)

    local function createFlippedFinalSphereEffect()
        local randomSize = Random.new():NextNumber(55, 50)
        local clonedSphere = sphere:Clone()
        clonedSphere.Name = "Cloned"
        clonedSphere.Transparency = 0.01
        clonedSphere.Material = Enum.Material.Neon
        clonedSphere.Color = Color3.fromRGB(46, 177, 33)
        clonedSphere.Parent = limitlessBarrier.CurrentTweens
        clonedSphere.CFrame = flipAndPositionCFrame(humanoidRootPart.CFrame, effectDistance)

        TweenService:Create(clonedSphere, TweenInfo.new(0.2 / speedFactor, Enum.EasingStyle.Quint, Enum.EasingDirection.Out), {
            Size = Vector3.new(randomSize, randomSize, randomSize),
            Transparency = 1
        }):Play()

        task.wait(0.2 / speedFactor)
        clonedSphere:Destroy()
    end

    for i = 1, 5 do
        spawn(function() createFlippedFinalSphereEffect() end)
        task.wait(0.065 / speedFactor)
    end
end)
 
    end
 
end
 
humanoid.AnimationPlayed:Connect(onAnimationPlayed)
 
local animationId = 12983333733 ---- in order for the ult
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://17278415853"
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 4
 
 
Anim:Play()
 
Anim:AdjustSpeed(0)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(0.75)
 wait(6)
 Anim:Stop()
    end
 
end
 
humanoid.AnimationPlayed:Connect(onAnimationPlayed)

local animationId = 10480796021
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://15957361339"
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0
 
 
Anim:Play()
 
Anim:AdjustSpeed(0)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(1)
 
 
    end
 
end
humanoid.AnimationPlayed:Connect(onAnimationPlayed)

local animationId = 13927612951
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://18459178353"
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0
 
 
Anim:Play()
 
Anim:AdjustSpeed(0)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(0.59)
 
 
    end
 
end

humanoid.AnimationPlayed:Connect(onAnimationPlayed)
 
 
local animationId = 12447707844
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://18435303746"
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0
 
 
Anim:Play()


 
Anim:AdjustSpeed(0)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(0.8)

wait(6.4)

Anim:Stop()

 
    end
 
end
 
humanoid.AnimationPlayed:Connect(onAnimationPlayed)
 
 
local animationId = 10479335397
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://14046756619"
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0
 
 
Anim:Play()
 
Anim:AdjustSpeed(0)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(0.7)
 
 
delay(1.2, function()
 
    Anim:Stop()
 
end)
 
 
    end
 
end
 
humanoid.AnimationPlayed:Connect(onAnimationPlayed)
 
 
local animationId = 10503381238
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://14900168720"
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 1.3
 
 
Anim:Play()
 
Anim:AdjustSpeed(0)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(1)
 
 
    end
 
end


 
humanoid.AnimationPlayed:Connect(onAnimationPlayed)
 
 
local animationId = 10470104242
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://12684185971"
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0
 
 
wait(0.2)
 
Anim:Play()
 
Anim:AdjustSpeed(0)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(1)
 
 
    end
 
end

local animationId = 10480793962
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://15957361339"
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0
 
 
Anim:Play()
 
Anim:AdjustSpeed(0)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(1)
 
 
    end
 
end

humanoid.AnimationPlayed:Connect(onAnimationPlayed)
 
 
local Players = game:GetService("Players")
 
local player = Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local animationIdsToStop = {
 
    [10469493270] = true,
 
    [10469630950] = true,
 
    [10469639222] = true,
 
    [10469643643] = true,
 
}
 
 
local replacementAnimations = {
 
    ["10469643643"] = "rbxassetid://17889290569",
 
    ["10469639222"] = "rbxassetid://17889471098",
 
    ["10469630950"] = "rbxassetid://17889461810",
 
    ["10469493270"] = "rbxassetid://17889458563",
 
}
 
 
local queue = {}
 
local isAnimating = false
 
 
local function playReplacementAnimation(animationId)
 
    if isAnimating then
 
        table.insert(queue, animationId)
 
        return
 
    end
 
 
 
    isAnimating = true
 
    local replacementAnimationId = replacementAnimations[tostring(animationId)]
 
    if replacementAnimationId then
 
        local AnimAnim = Instance.new("Animation")
 
        AnimAnim.AnimationId = replacementAnimationId
 
        local Anim = humanoid:LoadAnimation(AnimAnim)
 
        Anim:Play()
 
 
 
        Anim.Stopped:Connect(function()
 
            isAnimating = false
 
            if #queue > 0 then
 
                local nextAnimationId = table.remove(queue, 1)
 
                playReplacementAnimation(nextAnimationId)
 
            end
 
        end)
 
    else
 
        isAnimating = false
 
    end
 
end
 
 
local function stopSpecificAnimations()
 
    for _, track in ipairs(humanoid:GetPlayingAnimationTracks()) do
 
        local animationId = tonumber(track.Animation.AnimationId:match("%d+"))
 
        if animationIdsToStop[animationId] then
 
            track:Stop()
 
        end
 
    end
 
end
 
 
local function onAnimationPlayed(animationTrack)
 
    local animationId = tonumber(animationTrack.Animation.AnimationId:match("%d+"))
 
    if animationIdsToStop[animationId] then
 
        stopSpecificAnimations()
 
        animationTrack:Stop()
 
 
 
        local replacementAnimationId = replacementAnimations[tostring(animationId)]
 
        if replacementAnimationId then
 
            playReplacementAnimation(animationId)
 
        end
 
    end
 
end
 
 
humanoid.AnimationPlayed:Connect(onAnimationPlayed)
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoidRootPart = character:WaitForChild("HumanoidRootPart")
 
 
local function onBodyVelocityAdded(bodyVelocity)
 
    if bodyVelocity:IsA("BodyVelocity") then
 
        bodyVelocity.Velocity = Vector3.new(bodyVelocity.Velocity.X, 0, bodyVelocity.Velocity.Z)
 
    end
 
end
 
 
character.DescendantAdded:Connect(onBodyVelocityAdded)
 
 
for _, descendant in pairs(character:GetDescendants()) do
 
    onBodyVelocityAdded(descendant)
 
end
 
 
player.CharacterAdded:Connect(function(newCharacter)
 
    character = newCharacter
 
    humanoidRootPart = character:WaitForChild("HumanoidRootPart")
 
    character.DescendantAdded:Connect(onBodyVelocityAdded)
 
 
 
    for _, descendant in pairs(character:GetDescendants()) do
 
        onBodyVelocityAdded(descendant)
 
    end
 
end)

---- ult
function onAnimation(id, func)
    local id = tostring(id):gsub("rbxassetid://", "")

    local char = game:GetService("Players").LocalPlayer.Character
    local humanoid = char and char:WaitForChild("Humanoid", 1)
    if char and humanoid then
        humanoid.AnimationPlayed:Connect(function(v)
            local vID = v.Animation.AnimationId:gsub("rbxassetid://", "")
            if id == vID then
                print("Animation ID matched, executing function.")
                func(v)
            else
                print("Animation ID did not match.")
            end
        end)
    end
    
    game:GetService("Players").LocalPlayer.CharacterAdded:Connect(function(char)
        local humanoid = char and char:WaitForChild("Humanoid", 1)
        if char and humanoid then
            humanoid.AnimationPlayed:Connect(function(v)
                local vID = v.Animation.AnimationId:gsub("rbxassetid://", "")
                if id == vID then
                    print("Animation ID matched after CharacterAdded, executing function.")
                    func(v)
                else
                    print("Animation ID did not match after CharacterAdded.")
                end
            end)
        end
    end)
end
