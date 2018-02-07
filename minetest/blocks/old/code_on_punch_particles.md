## Copy the following code and paste it at the `BEGINNING` of your `init.lua` file

```lua
on_punch_particles = function(file,num,vx,vy,vz,size) 
  return function(pos, node, player, pointed_thing)
    for i=1,num do
		  minetest.add_particle({
			  pos = pos,
			  velocity = {x=vx*(math.random()-.5), y=vy*(math.random()-.5), z=vz*(math.random()-.5)},
			  acceleration = {x=0, y=0, z=0},
			  expirationtime = 1,
			  size = size,
			  collisiondetection = false,
			  vertical = false,
			  texture = file,
			  playername = "singleplayer"
		   })
     end
  end
end
```
## Then copy the `new line only` and add it to your `init.lua` file

```lua
minetest.register_node("campmod:#####", { -- This will be how you reference this block in the code
        description = "#####", -- This will be the name that appears in game
        tiles = {"#####"}, -- This will be the name of the texture image
        is_ground_content = true,
        groups = {choppy = 1},
	
	-- START OF NEW CODE --
        on_punch = on_punch_particles("stars.png",10, 0,0,0, 10) -- copy this line only
	-- END OF NEW CODE --
	
})
```

**Reminder:**  **CTRL+C** to copy and **CTRL+V** to paste


