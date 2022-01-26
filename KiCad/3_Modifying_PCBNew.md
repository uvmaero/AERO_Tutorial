# STEP 3 - Modifying PCB Layout

Goal: Learn how to translate the schematic to a pcb layout

## Annotating Changes and Assigning Footprints

 First press the `Assign PCB footprints to schematic symbols` button *In version 6 called `Run Footprint Assign Tool`* in the top ribbon. 

 Select all capacitors then apply `Description filter` and `Pin count filter`. From the filtered list find `Capacitor_SMD:C_0603_1608Metric_Pad1.5x.95mm_HandSolder` This means that the part is a capacitor, it is surface mount, 0603 size, and hand solder meaning it has larger pads. Double click to apply to the capacitors

 Next Do the same with the Diodes selecting `Diode_SMD:D_0603_1608Metric_Pad1.5x.95mm_HandSolder`

 The Connector that we will be using is the `Connector_PinHeader_2.54mm:PinHeader_2x03_P2.54mm_Vertical` *NOTE not the surface mount this component we use the through hole version*

 Another connector that will be needed is the `Connector_PinHeader_2.54mm:PinHeader_2x02_P2.54mm_Vertical` for the 12 volt connector

 The Resistors used are the `Resistor_SMD_:R_0603_1608Metric_Pad1.5x.95mm_HandSolder`

 The remaining two components are predefined therefore everything now should be filled so select `OK`

## Updating PCB Layout

In the Top Ribbon Select `Open PCB in board editor` This should open a new blank window. In the Ribbon Press `Update PCB from Schematic` this will bring up an error box if there are any errors in assigning the footprint it will tell you. If no errors press `Update PCB`. Now 
place the mess of components on the PCB by clicking anywhere. 

On the right hand side are a list of filters to make it easier to see what you are doing turn off `F.Fab` and `B.Fab`

Now you move the components around on the PCB to where ever you want them. To move a component select it and press `m`. Some things to note while moving and placeing components make sure the labels for each component is visable and not covered by any device this will help in assembling and to referance in the future. Also do not place components over lapping or to close together that will make soldering a lot harder. 

To move a component to the other side of the board select the device and press `f` The component should tern grean indicating it is on the back side of the board and the label shifts from blue to purple.

## Adding traces

Next define track size by pressing the drop down menu that says `track 0.25mm` from here add `0.254mm` add `.36mm` and `0.6mm` and press ok

To start a trace press `x` and select a copper pad. The program will highlight the destination and draw the paths for all traces. To switch between front and back press `v`. You will know you are on the back because the trace will be green instead of red. 

To connect components on opposite sides of the board start the path then press `v` after placing a point to make a path through the board. 

*A note aboout laying traces, try to make them as clean and organised as possible this will minimise the points of failure and make the board easier to debug and solder*

*also note the track width and for the 12v connector use a larger trace with then the other connectors*

## Board Dimentions and Trace Fill

Change to the `edge.cut` layer then select `Add graphic polygon` in the right side ribbon you may want to change the grid size to a larger grid to make straight lines. With the polygon tool draw lines around all components this will make the board dimentions which is important to print.

Go back to the copper layers and select the `add fill zones` in the right ribbon as well. Follow the out line you just made. When you click a window will apear select `GND` most of the defaults should be fine but `Clearance` and `minimum width` may have to be adjusted.

Once the fill is complete select it and press `cmd-d` this is duplicate, without moving your mouse click to place the fill. Press `e` and change the duplicated fill to the back side of the board.

*A good way to spread the ground load is to add vias connecting the fills on both sides of the board*

If some of the grounds arn't connected change the clearance to be slightly smaller untill you have 0 Unrouted

Finally add a title block by pressing the `T` in the ribbon on the right with your name and date (format year.day ie 22.5 for january 5th 2022)

*`n` lowers grid size `N` makes it larger*

Also add an aero logo from the aero footprints library

## Saving Changes

This is where you can leverage your Git skills to commit and push the changes. If you need a refresher, go to the [GitHub Tutorials](../Tutorials/1_GitHub_GettingStarted). Commit and push your changes. 