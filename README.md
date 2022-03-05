# artistthiung
Starving Artists | Use Any Image as Artwork [Python]
DISCLAIMER: THIS IS NOT ALWAYS GOING TO WORK

DATA = WHAT_WAS_SET_TO_YOUR_CLIPBOARD


ART_NAME = "God"



function ParseCells(cells)
  local Cells = {}
  for i,v in pairs(cells) do
    success, error = pcall(function()
      Color3.fromHex(v)
    end)
    if not success then
      table.insert(Cells, "ffffff")
      warn(v, success, 'hex failure | replacing with ffffff')
    else
      table.insert(Cells, v)
    end
  end
  return Cells
end

function SaveArt(name, cells)
  local data = {}
  data.Cells = ParseCells(cells)
  data.FrameColor = "ffffff"
  data.Name = name
  game:GetService("ReplicatedStorage").Remotes.CreateArt:InvokeServer(data)
end

SaveArt(ART_NAME, DATA)
- Download Python - https://i.imgur.com/oTocl9N.png

- Open it and install it > MAKE SURE YOU TICKED "Install to path" - https://i.imgur.com/uXfoJOL.png

- Once it's installed go to your start menu and search "CMD" and open it - https://i.imgur.com/g15GPl0.png

- Copy this text

Code:

py -m pip install pyperclip pillow
and paste it into Command Prompt and press Enter - https://i.imgur.com/1RmMUqQ.png

- Once that's done close Command Prompt and go to any image search engine and search up an image. It can be ANYTHING.

- Once you found one download it to your desktop

- Then after that download Dwuck's Python file from here https://github.com/LittleDyingDuck/artistthiung/blob/main/convert.py

- Put this file onto your Desktop

- After that right click it and open it in IDLE - https://i.imgur.com/QSHpfbm.png

- Copy the images title including the file type - https://i.imgur.com/0URG9ua.png

- Then go back to IDLE and change file.png to the image's title and file type - https://i.imgur.com/KcIJ1s2.png

- Then hit "File > Save" and close it

- Once that's done just open the file by double clicking it and it'll copy a code to your clipboard

- Take the script and put it into your exploit and add the code here - https://i.imgur.com/OerQR6L.png / Be sure to remove "WHAT_WAS_SET_TO_YOUR_CLIPBOARD" then post the code







Credits: https://v3rmillion.net/showthread.php?tid=1160423
