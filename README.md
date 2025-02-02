function Update Chest Chams() for i,v in pairs(game.Workspace: GetChildren()) do pcall(function()

if string.find(v.Name, "Chest") then

if Chest ESP then

if string.find(v.Name, "Chest") then

if not v: FindFirstChild('NameEsp'..Number) then

local bill Instance.new('BillboardGui',v)

bill.Name = 'NameEsp'..Number

bill.ExtentsOffset = Vector3.new(0, 1, 0)

bill.Size UDim2.new(1,200,1,30)

bill.Adornee = v

bill.AlwaysOnTop true

local name Instance.new('TextLabel', bill)

name. Font Enum.Font.GothamSemibold

name.FontSize = "Size14"

name.TextWrapped true

name. Size UDim2.new(1,0,1,0)

name. TextYAlignment 'Top'

name. Background Transparency = 1

name.TextStroke Transparency = 0.5

if v.Name == "Chest1" then

name.TextColor3 Color3.fromRGB(109, 109, 109)

name.Text = ("Chest 1"..'\n'..

round((game:GetService('Players'). LocalPlayer. Character.Head. Position v.Position).Magnitude/3) Distance')

end

if v.Name == "Chest2" then

name. TextColor3 Color3.fromRGB(173, 158, 21)

name. Text("Chest 2"..'\n'..

round((game:GetService('Players'). LocalPlayer. Character.Head. Position v.Position).Magnitude/3).. Distance') end

if v.Name == "Chest3" then

name.TextColor3 Color3.fromRGB(85, 255, 255)

name.Text = ("Chest 3"..' \n'

round((game: GetService('Players'). LocalPlayer. Character.Head. Position v.Position). Magnitude/3). Distance')

end

else

v['NameEsp'..Number].TextLabel.Text (v.Name...

\n'.. round((game: GetService('Players'). LocalPlayer.Character.Head. Position v.Position). Magnitude/3)..' Distance')

end end if v: FindFirstChild('NameEsp'..Number) then v: FindFirstChild('NameEsp.. Number): Destroy() end end

else

end

end)

end
