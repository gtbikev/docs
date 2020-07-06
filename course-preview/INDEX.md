# Grand Theft Bike V - Course Preview <!-- omit in toc -->

## Introduction

You need the following tools to create a course animation:

* Photo editor (Photoshop of similar software) - for sizing map and profile, plus coloring route
* Blender (2.83 or higher version) - for creating a course animation

The following sections will describe the process of creating a course preview in detail.

## PART I: Create Map with Profile

Perform the following steps to create the course map:

1. Go to [GTA 5 Map](https://gta-5-map.com), zoom in/out and take a screenshot of the map
2. Open the screenshot in photo editor; crop and size it to 800x600px
3. Color the route black
4. Copy the GTA 5 map to the image created in step 1

> Another way to color the route is to draw curves in a drawing tool or PowerPoint and export the image

Perform the following steps to create the course profile:

1. Go to your favorite sports app and take a screenshot of the profile
2. Open the the screenshot in photo editor, crop and size it to 700x50px; remove elevation data and lines

Perform the following steps to create the map with profile:

1. Open photo editor; create a new image with size of 800x800px
2. Copy course map to the new image created in step 1
3. Copy course profile to the new image created in step1

> You find a map example in the course repository: https://github.com/gtbikev/courses/preview/template/map-template.png


## PART II: Create Course Animation

Perform the following steps to prepare for course animations in Blender:

1. Open Blender; select menu File > Preferences; select Add-ons
2. Search image; click checkbox: Import-Export: Import Images as Planes

Perform the following steps to create a map animation:

1. Create new file: 2D Animation
2. Select Output Properties; change resolution to X: 800px / Y: 800 px
3. Select menu File > Import > Images as Planes; select map.png and press button [Import Images as Planes]
4. Press key 'S' to scale image to camera view, click left mouse button to set
5. In the Outliner Windows, select Stroke
6. In the '3D Viewpoint' editor, select Draw
7. Click Polyline in the toolbox
8. Draw the route by clicking & pulling left mouse button for each waypoint; click right mouse button to complete polyline
9. In the '3D Viewpoint' editor, select Object Mode; select created polyline
10. Right mouse-click, select menu item 'Convert to Bezier Curve'; this create a new 'Lines' object in Outliner
11. Import navigator image with menu File > Import > Images as Planes; select navigator.png and press button [Import Images as Planes]
12. Size the navigator image by select Object Properties; set Scale X, Y, Z to 0.35
13. In the '3D Viewpoint' editor, select Add > Empty > Plain Axis; this creates a new 'Empty' object in Outliner
14. In Outliner click on navigator; hold key 'Shift' and move 'navigator' to 'Empty'
15. Select 'Empty'; click Object Constraint Properties; Select 'Follow Path' from dropdown 'Add Object Constraint'
16. Select 'Lines' in Target; click button [Animate Path]; click checkbox 'Follow Curve'; select Forward 'X'
17. If not automatically done, press key 'G' to move 'Empty' to start position of route
18. Change frames by select Object Data Properties > Path Animation; change frames to 250

Perform the following steps to create a profile animation:

1. In the Outliner Windows, select Stroke
2. In the '3D Viewpoint' editor, select Draw
3. Click Polyline in the toolbox
4. Draw the route by clicking & pulling left mouse button for each waypoint; click right mouse button to complete polyline
5. In the '3D Viewpoint' editor, select Object Mode; select created polyline
6. Right mouse-click, select menu item 'Convert to Bezier Curve'; this create a new 'Lines' object in Outliner
7. Import navigator image with menu File > Import > Images as Planes; select navigator.png and press button [Import Images as Planes]
8. Size the navigator image by select Object Properties; set Scale X, Y, Z to 0.25
9. In the '3D Viewpoint' editor, select Add > Empty > Plain Axis; this creates a new 'Empty' object in Outliner
10. In Outliner click on navigator; hold key 'Shift' and move 'navigator' to 'Empty'
11. Select 'Empty'; click Object Constraint Properties; Select 'Follow Path' from dropdown 'Add Object Constraint'
12. Select 'Lines' in Target; click button [Animate Path]; click checkbox 'Follow Curve'; select Forward 'X'
13. If not automatically done, press key 'G' to move 'Empty' to start position of route
14. Change frames by select Object Data Properties > Path Animation; change frames to 250

Perform the following steps to render and export the course preview:

1. Select Output Properties; set output to location where you want to render and export course preview
2. In Output Properites: set file formation to `FFmpeg video` and select `MPEG-4` under Encoding / Container; set Video Codec to `H.264`
3. Select menu Render > Animation; a new window opens displaying the render progress
4. Once render animation is completed you find the course preview in the location specified in step 1

Happy Course Previewing!