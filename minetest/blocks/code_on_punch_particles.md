## Copy the following code and add it to beginning of you your `init.lua` file

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

**Reminder:**  **CTRL+C** to copy and **CTRL+V** to paste


