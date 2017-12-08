## Copy the `new lines only` and add it to your `init.lua` file

```lua
minetest.register_node("campmods:#####", { -- This will be how you reference this block in the code
        description = "#####", -- This will be the name that appears in game
        tiles = {"#####"}, -- This will be the name of the texture image
        is_ground_content = true,
        groups = {choppy = 1},

        drop = "default:sword_diamond", -- TO CHANGE LATER
})

-- START OF NEW CODE --
minetest.register_tool("campmods:blue_lightsaber", {
    description = "Blue Lightsaber",
    inventory_image = "blue_lightsaber.png",
    tool_capabilities = {
        full_punch_interval = 1,
        max_drop_level=0,
        groupcaps={
            snappy={times={[2]=1.6, [3]=0.40}, uses=10, maxlevel=1},
        },
        damage_groups = {fleshy=2},
    },
    groups = {flammable = 2},
    sound = {breaks = "default_tool_breaks"},
})
-- END OF NEW CODE --
```

**Reminder:** **CTRL+C** to copy and **CTRL+V** to paste
