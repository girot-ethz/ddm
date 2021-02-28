# Basic Modelling



*getting started*

- [Rhino 6 Interface](#rhino-6-interface)
- [Viewports](#viewports)
- [Navigation](#navigation)
- [Display Modes](#display-modes)
- [Units](#units)
- [Basic Modeling](#basic-modeling)
- [Status Bar](#status-bar)
- [Layers](#layers)
- [Layouts](#layouts)



First of all. The Help tool in Rhino is very well done and very complete. Dont't hesitate to use it.

![01_Capture1.PNG](/doc/Rhino_01_Capture1.PNG)



---

## Rhino 6 Interface

Modeling in 3‑D is the process of creating a mathematical representation of an object’s surfaces. The resulting model is displayed on your screen as a two-dimensional image. Rhino provides tools for creating, displaying, and manipulating these surfaces.

![02_Viewport_Overview.png](/doc/Rhino_02_Viewport_Overview.png)

>
>1. Viewport (Display different views within the graphics area)
>2. Menu Bar (Access commands, options and document properties (e.g. model units))
>3. Tool Bar (Basic Modelling tools)
>4. Status Bar (Displays options, toggles, coordinates)
>5. Panels (Displays specific options such as layers, object properties, cameras etc.)
>6. Add Layout (Add set views or layouts to fast navigate btw. viewports)
>7. Command Prompt (List of commands and prompts)
>

---
## Viewports


![Viewport_Toggle](/doc/Rhino_03_Viewport_Toggle.png)


>You can reset the viewport by clicking the “Viewport Toggle" icon



Viewports are windows in the graphics area that display views of your model. They can be docked or floating. You can customize the viewports and their positions to suit your preferences. The size and position of viewports is adjustable; they can be any rectangular size and shape.
Each viewport has its own construction plane and grid that the cursor normally moves on and a projection mode. To toggle between a small viewport and one that fills the graphics area, double-click the viewport title.



![Detail Switching the Panels](/doc/Rhino_04_Change_Viewports.PNG)


>Rightclick on the viewport title to:
>
>- Change Display Mode
>- Set View
>- Set Camera
>
>
>*The Standard layout in Rhino is four viewports. Doubleclick on the viewport title, and this >one will become the main panel. Doubleclick again and it will revert to a 4-panel-view. >Viewport tabs can be activated to facilitate navigation through panels. You can also >navigate between the viewports at the bottom left.*

---


## Navigation

![Marked Navigation Tool Bar](/doc/Rhino_05_Navigation.png)


>There are several types of navigation tools, which you can find in the toolbar above


Working in 3D on a computer requires visualizing 3D objects drawn on a 2D medium - the computer screen. Rhino provides tools to help do this.
Rhino’s easy view navigation helps you visualize your model. You can look at you model from any direction, look at the whole model, or look into the details. You can also change your view in the middle of performing a command to see precisely where you want to select an object or pick a point.


Mouse Navigation

![Mouse Navigation](/doc/Rhino_06_Navigation_Zoom_In.png)


>1. Pan - In viewports with parallel projections (for example: Top, Front, and Right), drag with the right mouse button. In perspective viewports, hold the Shift key, and drag with the right mouse button.
>2. RotateView (Orbit) - In perspective viewports, drag with the right mouse button.
>3. Zoom - Hold the Ctrl key, and drag up and down with the right mouse button, or use the mouse wheel.



![Mouse Navigation](/doc/Rhino_07_Navigation_Zoom_In_Extended.png)


>1. Zoom Extents - Zooms the view to show all objects currently visible.
>2. Zoom Selected - Zooms the view to show all selected objects.
>3. Undo View - The UndoView command reverses recent view changes.
>4. Undo a command - On the Edit menu, click Undo. Or press the “Ctrl + Z” keys.
>5. Hide / Show - The Hide command conceals selected objects from view. To show again: Rightclick and “Show Objects”
>6. Fly out toolbar - Tools with a little triangle have a flyout toolbar options to complete similar tasks in different ways.


---

## Display Modes


![Mouse Navigation](/doc/Rhino_08_Display_Mode_Toolbar.png)


>You can either change the display mode by toggling the icon above or rightclick the >viewport title.


![Mouse Navigation](/doc/Rhino_09_Changing_Displaymode.png)
![Mouse Navigation](/doc/Rhino_11_Display_Modes.png)


>You can view your model in a variety of wireframe, shaded and rendered methods that depend >on your needs.


![Mouse Navigation](/doc/Rhino_10_Changing_Viewportprotection.PNG)


>The perspective viewport projection can be parallel, three-point perspective, or two-point perspective. The viewport projection is set in Viewport Properties. When no object is selected, the Properties panel shows viewport properties.


---

## Units

![Mouse Navigation](/doc/Rhino_12_Acess_Units.png)


>You can access the units properties through the File Menu (File > Properties > Units)


![Mouse Navigation](/doc/Rhino_13_Document_Properties.PNG)


>As soon as Rhino is launched, you are prompted to choose the units of the model you will be working in. For general landscape modelling we recommend to choose "Meters", for CNC Milling the unti of choice should be "Millimeters".


---


## Basic Modeling

![Mouse Navigation](/doc/Rhino_14_Commandbar.png)


>Rhino is a command-driven program. In other words, all actions are activated by named commands.


Toolbars contain graphical icons for initiating commands. Many toolbar icons have a second command that can be accessed by right-clicking the icon. The tooltip that appears when you hover over the icon tells you what the left and right mouse button would lead to.



![Mouse Navigation](/doc/Rhino_15_Lines.png)


>1. Point(s) - Point objects mark a single point in 3‑D space. They are the simplest objects in Rhino.
>2. Line - The Line command draws one line segment.
>3. Polyline - The Polyline command draws a series of lines.
>4. Curve - The Curve command draws a curve from control points.


*Tips: You can **just start typing**, there is no need to press on the command prompt. To confirm the command you can press spacebar or enter or right-click
You can also **repeat the last command** by press either spacebar, enter or rightclick (on viewport). **To Cancel** stuff, just press ESC*

![Mouse Navigation](/doc/Rhino_16_Extended_Options.png)


>Many commands provide secondary options to allow additional options. By clicking on the (Vertical=No) option it will change to “YES”, allowing you to move your objects only in Z-Axis. These secondary options are also often accessible through the flying toolbar.


---


## Status Bar

![Mouse Navigation](/doc/Rhino_17_Snap_Options.png)
![Mouse Navigation](/doc/Rhino_18_Snap_Options_2.png)

##### Object Snap (OSNAP)

![Mouse Navigation](/doc/Rhino_19_Snap_Options_3.png)


>1.  Osnap
    The object snaps constrain the marker to an exact location on an object such as the end of a line or the center of a circle.
>2.  End
    Snap to the end of a curve, line etc.
>3.  Near
    Snap onto a curve near the cursor location.
>4.  Point
    Snap to a point object or a control point of a line or curve.
>5.  Mid
    Snap to the midpoint of a curve, line, polyline segment etc.
>6.  Cen
    Snap to the center of a circle, box etc.
>7.  Int
    Snap to the intersection or projected intesection of curves, lines, edges etc.
>8.  Perp
    Snap perpendicular to a curve.
>9.  Tan
    Snap tangent to a curve.
>10. Quad
    Snap to the point on a curve that is at the max. x or y point relative to the current construction plan.
>11. Knot
    Snap to a knot on a curve or surface.
>12. Vertex
    Snap to a mesh vertex. Your only option to snap on a mesh object.





##### Other Options

![Mouse Navigation](/doc/Rhino_20_Other_Options.png)


>1. Grid Snap
   Forces the Marker to snap on grid intersections.
>2. Ortho
   Restricts cursor movements to the points at a specified angle from the last point created. The default angle is 90 degrees. You can temporarily turn this off by pressing Shift.
>3. Planar
   This helps you model objects in the same projected plane by forcing input to be on a plane normal to the last point you picked its imagined connection to your viewport position.
>4. SmartTrack
   SmartTrack™ is a system of temporary reference lines and points that is drawn in the Rhino viewport.
>5. Gumball
   The Gumball command displays the gumball widget on a selected object facilitating move, scale, and rotate transformations around the gumball origin.
>6. Record History
   Records history and updates history-aware objects. With history recording and update turned on, e.g. a lofted surface can be changed by editing the input curves.
>7. Project Osnap
   By default, 2D geometry is created on the active construction plane. The project constraint ignores object snaps and pushes all the geometry onto the active construction plane.
>8. Disable Osnap
   The DisableOsnap command manages the state of persistent object snaps to temporarily turn off persistent object snaps from the control.


---


## Layers

![Mouse Navigation](/doc/Rhino_21_Acess_Layer.png)


>You can access the Layer functions through the Edit Menu (Edit > Layers > Edit Layers) or >from the Tool Bar.


##### Setting up Layers

Layers are a way of grouping objects and applying certain characteristics to all objects that have that layer assignment. Layer states include a layer name, the color used to display the objects, and the visibility and the possibility to lock/unlock all the objects on a layer. Objects are always created on the current layer indicated by the little tick. Only one layer can be active at a time. Objects may also be copied or moved to other layers later. Objects on layers that are off are not visible in the model. Objects on locked layers cannot be selected but can be snapped to.

![Mouse Navigation](/doc/Rhino_22_Layer_Settings.png)


>1. New Layer
>2. New Sublayer
>3. Change the on/off state
>4. Change the locked/unlocked state
>5. Change the layer color
>6. Set the current layer
>
>Doubleclick to change the Name
>
>Rightclick to:
>
>-Select Objects on Layer
>-Change/Copy selected object to layer


---


## Layouts

![Mouse Navigation](/doc/Rhino_23_Acess_Layouts.png)


>Use a layout to arrange the model for the printer. (View > Layout > New Layout)


Viewport to layout
To add a new layout to your rhino file either do:
- Viewport Tab: Rightclick on “+” and “New Layout"
- Via Command prompt: Type: “Layout”
- Via Menu: View > Layout > New Layout

Properties
By selecting “New Layout” a window pops up to define certain layout properties. These can be changed afterwards again.

![Mouse Navigation](/doc/Rhino_24_Set_Scale.png)


>Set scale
>1. Click on the Frame of your View (in the Layout)
>2. Go to “Properties” then click on “Detail”
>3. Set Scale
