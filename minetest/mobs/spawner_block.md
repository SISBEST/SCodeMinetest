
```lua
minetest.register_node("test:mob_test", { -- This will be how you reference this block in the code
        description = "test", -- This will be the name that appears in game
        tiles = {"test.png"}, -- This will be the name of the texture image
        is_ground_content = true,
        groups = {choppy = 1},
        on_punch = function(pos,node,player,thing)
           minetest.add_entity(pos, "ccmobs:cow") 
        end
})
```
