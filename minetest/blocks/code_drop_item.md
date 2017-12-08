## Copy the `new line only` and add it to your `init.lua` file

```lua
minetest.register_node("campmod:#####", { -- This will be how you reference this block in the code
        description = "#####", -- This will be the name that appears in game
        tiles = {"#####"}, -- This will be the name of the texture image
        is_ground_content = true,
        groups = {choppy = 1},
        
        -- START OF NEW CODE --
        drop = "default:sword_diamond", -- copy this line only
        -- END OF NEW CODE --
        
})
```
**Reminder:**  **CTRL+C** to copy and **CTRL+V** to paste
