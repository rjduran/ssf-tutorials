5/5/13

C4D Tutorial by RJ Duran

Exporting Objects From C4D / Exporting UV Texture

This tutorial covers a basic example of exporting a color object from Cinema4D for printing with Shapeways. The final project files are included in case you get lost. To start, make sure the global units for C4D are set to Millimeters. (Edit > Preferences > Units)

1. Make a new c4d file named ColorBall and save it. (The final version of the tutorial can be seen in C4D_UVMapping.c4d)

2. Make a new sphere mesh and scale it to 100mm x 100mm x 100mm.

3. In the material editor at the bottom, make a new material. Give it a name of "BallTexture" and apply it to the sphere mesh object.

4. Switch the program layout from "Startup(User)" to BP "3D Paint" by selecting the dropdown in the top right corner of the application.

5. Now in the body paint layout select the "Paint Setup Wizard" from the top toolbar (its a paintbrush with little stars). 
  - Hit Next 
  - Hit Next
  - Hit Finish (Note: This is where you can change your texture resolution before saving. Shapeways suggests a maximum of 2048 x 2048. [1])

	You should see the following:  
	**Setup Wizard Start**  	Object Mode  	Calculating automatic map size...  	Caching Textures from texture paths...  	Creating Texture: "BallTexture"; Color; 1024x782  	**Setup Wizard End**

6. Select the Materials tab on the right and select the BallTexture material. You will see the material properties above this. Notice there is a tif file listed in the Texture field. This is your new texture.

7. Save the project. You will notice that you now have a file named BallTexture_Color.tif in the working directory. 

8. Now select the Texture tab to change views. When you select the material from the right Materials manager you will see the texture in the window. If you select UV Mesh > Show UV Mesh you should see the polygons for the sphere mesh object. Here is where you can begin to paint on the model. Use the text tool and type "Hello World" on the mesh somewhere.

9. If you switch back to viewing the mesh (View) you will see the texture applied as  a material. At this point you just need to save out the texture and wrl.

10. Save the texture
  - File > Save Texture as Copy, select png or jpg. It needs to have the same name as the tif file. Ex, BallTexture_Color.png

11. Save the VRML2 (wrl)
  - File > Export > VRML2, 
  - Name: ColorBall_Working.wrl
  - Set Textures option to Referenced
  - Scale: 1 mm

12. Open the wrl file in a text editor and search for the tif texture file. Replace the extension with png (url "BallTexture_Color.png").

13. Zip up the wrl and png files, rename the archive to ColorBall_Working.zip. If you are lost at this point look at the 4 resources listed.

14. Upload the entire zip file to Shapeways. Make sure the units are in millimeters. Note that you don't actually want to print something like this. It will cost a fortune because it is solid and roughly 4" x 4" x 4".

Resources  
[1] http://www.shapeways.com/tutorials/exporting_to_vrml_and_x3d_for_color_printing  
[2] http://www.shapeways.com/blog/archives/440-Modeling-in-Cinema-4d-for-Shapeways.html  
[3] http://www.shapeways.com/tutorials/exporting_vrml  
[4] http://www.shapeways.com/tutorials/converting-with-accutrans-3d  