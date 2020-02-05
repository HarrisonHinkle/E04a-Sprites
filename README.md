# E04a-Sprites
This is a forked and modified repository made for an assignment in my Game Technology course at IU. 

I used with the Godot application to modify Game.tscn in the scenes folder to fullfil the requirements. These were: 
 
 - The example I provided is a type of 2D physics node called a RigidBody2D. This is a useful type of node for an object that will be moving through the world (according to basic laws of physics) without any internal locomotion.
 - Right-click on the Game node and select "Add Child Node". From the resulting list, select RigidBody2D, and rename it Falling 2
 - Select Falling 2 and in the toolbar, select the icon that looks like two intersecting squares (one hollow) with highlighted points in each corner. The tooltip for this icon is "Makes sure the object's children are not selectable"
 - Right click on Falling 2 and select "Add Child Node". Choose a Sprite node, and select it
 - In the FileSystem panel, open the Assets folder, and drag the femaleAdventurer_jump.png file to the Inspector panel for the Sprite. Drop the file on top of the Texture box
 - The image is much too big, so we will want to scale it. Under Node2D->Transform, update the Scale.x and Scale.y to both be 0.2
 - In the toolbar, you should see a Sprite icon. Click on that menu and select "Create CollisionPolygon2D Sibling". A new CollitionPolygon2D node should now appear under Falling 2
 - Select Falling 2, and in the Inspector, select Physics Material. Choose New Physics Material. Then select the menu again, and choose Edit.
 - In the resulting menu, change Friction to 0.2 and Bounce to 0.5
 - Place Falling 2 somewhere on the screen (inside the colorful rectangle) and run the scene. You should now see two people falling and bouncing
 - Repeat the above steps two more times, creating Falling 3 and Falling 4. Use either the male_jump.png or femaleAdventurer_jump.png Assets.
 - Right-click on the Game node and select "Add Child Node". This time, select StaticBody2D. This is a physics object that is not designed to move (like a wall or an obstacle). Change the node's name to Standing 1.
 - In the inspector, create a new PhysicsMaterial and Edit. Change Friction to 0 and Bounce to 1.
 - Add a Sprite node (this time, use maleAdventurer_wide.png), resize it, and Create a CollisionPolygon2D Sibling.
 - Place Standing 1 someplace on the screen, so that one of your falling objects will bounce off it.
 - Repeat this process five more times, creating Standing 2, Standing 3, Standing 4, Standing 5, and Standing 6. Choose either the maleAdventurer_wide.png or female_wide.png Assets for the sprites. Place them at various locations on inside the color rectange.
