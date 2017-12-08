--This requires installing the ccmobs and mobs mods first

minetest.register_node("test:mob_test", { -- This will be how you reference this block in the code
        description = "test", -- This will be the name that appears in game
        tiles = {"test.png"}, -- This will be the name of the texture image
        is_ground_content = true,
        groups = {choppy = 1},
        on_punch = function(pos,node,player,thing)
        --  minetest.add_entity(pos, "mobs:sheep") 
        --  minetest.add_entity(pos, "mobs:dirt_monster") 
        --  minetest.add_entity(pos, "mobs:dungeon_master") 
        --  minetest.add_entity(pos, "mobs:oerkki") 
        --  minetest.add_entity(pos, "mobs:rat") 
        --  minetest.add_entity(pos, "mobs:sand_monster") 
        --  minetest.add_entity(pos, "mobs:stone_monster") 
        --  minetest.add_entity(pos, "mobs:tree_monster") 
        end
})

minetest.register_abm({
  nodenames = {"test:test"},
  interval = 2,
  chance = 1,
  action = function(pos)
                minetest.add_entity(pos, "ccmobs:cow") 
                minetest.add_entity(pos, "ccmobs:chicken") 
                minetest.add_entity(pos, "ccmobs:nyan_cat") 
                minetest.add_entity(pos, "ccmobs:pig") 
                minetest.add_entity(pos, "ccmobs:rabbit") 
                minetest.add_entity(pos, "ccmobs:sheep") 
    minetest.remove_node(pos)
  end,
})

