# ⚠️ No Support Provided
This project is fully open source and provided as-is.
Feel free to explore, modify, and use it however you like, but please note that I do not offer any support for it. Thank you !

### **Useful Links 😊**

* [Join Our Discord](https://discord.gg/jgM5jW3rrN)
* [Visit Our Tebex Store](https://abdelemporium.tebex.io/)
* [Donations](https://paypal.me/ablframework?country.x=FR\&locale.x=fr\_FR)

### Description

This is a Cayo Perico minimaps for FiveM, created specifically for those using **abl-minimaps**. For more information and sources, check the following:

- [YouTube](https://youtu.be/PwLYomSRkBY?si=LGZ7CeA80fhxtvPy)
- [Documentation](https://abdelemporium-docs.gitbook.io/abdelemporium-docs/minimap-styles/minimap-styles)
- [Tebex Store](https://abdelemporium.tebex.io/category/allminimaps)

> **Note**: You can also use this minimap without having abl-minimaps installed.

### Installation

- Example : I have abl-minimap-part1-OP. So to install the **grey Cayo Perico minimap with green zone names**, follow these steps:

1. Download **Cayo-Maps** from GitHub.
2. Move the file `Cayo-Maps/Grey with text/grey-green/int3232302352.gfx` to the folder `abl-minimap-part1-OP/stream/gfx`.
3. Open `abl-minimap-part1-OP/Files/CL.lua` and add the following Lua code at any line:

    ```lua
    CreateThread(function()
      while true do
        SetRadarAsExteriorThisFrame()
        local coords = vec(4700.0, -5145.0)
        SetRadarAsInteriorThisFrame(`h4_fake_islandx`, coords.x, coords.y, 0, 0)
        Wait(0)
      end
    end)
    ```

4. Restart the script (it’s recommended to restart the server) to complete the setup.

### Preview
- In files

