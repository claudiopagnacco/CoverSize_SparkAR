
<!-- May 2020, Cover Size, v.10, by Claudio Pagnacco -->

# Cover Size (Patch for Spark AR)

## Instructions
* [General info](#general-info)
* [Technologies](#technologies)
* [Open project](#open-project)
* [Use the patch](#use-the-patch)

## General info
This patch allows you to create a self-cover resizible rectangle in Spark AR.
The rectangle will covers perfectly the camera viewport stucking the current aspect ratio of your image.
	
## Technologies
Project is created with:
* Spark AR Studio 88.0
	
## Open project
To run this project, simply double click on "Cover Size.arproj":

```
Cover Size/Cover Size.arproj
```
Don't move any file from this folder.
You can replace the "Replace Me" image in your Assets pannel with your.
Then you can modify the width and height value from your Patch Editor. 

## Use the patch
If you simply want to use the patch "Cover Size.arp" you can: 
1. Copy and paste it in the Assets panel of your current project.
2. Then drag and drop "Device" from Scene panel to Patch Editor.
3. Drag and drop Cover Size patch, and create two values in your Patch Editor (double click and type "value") called Width and Height (Number Value)
4. To know the correct size of your image you can right click on it in its folder.
5. Create a Canvas in the Scene panel, and a Rectangle inside it. (right click to create it)
6. Add a material in the Properties panel and click on it to change the Texture with your Image.
7. Back to Rectangle Properties and click on the arrow near Size section.
8. Now, connect Screen Size from the Device Patch to the first Cover Size's patch pin.
9. Connect Screen Scale from the Device Patch to the second Cover Size's patch pin.
10. Finally, divide (right click on the Patch Editor and type "Divide") the Height value by the Width value and connect it to the third Cover Size's patch pin.
11. You can connect the output Cover Size's pin to the rectangle Size pin and that's it!
