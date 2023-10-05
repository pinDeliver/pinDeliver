# Traffic restrictions

It is possible to use unlimited traffic restrictions to specify areas, including combinations with rush hours, where driving speed should be adjusted. These adjustments will be factored into the route optimization calculations.

To get started, activate *Traffic restrictions* in the [Settings-Optimization](settings_optimization.md) tab. Additionally, define time windows for both morning and evening rush hours.

Once you have completed these steps, you can create traffic regions. If you wish to modify an existing region, you can select:
* Edit traffic factors to adjust driving speeds for the region.
* Edit traffic region to modify the map area for the region.

![Traffic restriction list](/images/traffic_restrictions_list.png)

Click **Add new traffic region** below the list to create a new traffic region.

![Traffic restriction create](/images/traffic_restrictions_create1.png)

Provide a name for the traffic region and, if desired, add an optional description. Then, click **Create Traffic Region**. This will open the next window, where you can define the area by drawing lines on the map. Zoom in on your region and use the drawing tool to connect the lines and create the desired area.

![Traffic restriction create](/images/traffic_restrictions_map_drawing_tool.png)

Use lines to define the area where you want to set specific driving speeds. Each traffic region should cover only one area. If you have multiple separate areas, make a new region for each. Once you finish drawing lines, the mapped area will be shaded. Then, click **Save map area**.

![Traffic restriction create](/images/traffic_restrictions_create2.png)

Once you have saved the mapped area, you will be directed to the page where you can adjust driving speeds. By default, all speeds are set to 100%, but you can modify them using three sliders:

* Normal Speed: This determines the driving speed outside of both morning and evening rush hours.
* Morning Rush Hour: This sets the driving speed during the specified morning rush hour period defined in [Settings-Optimization](settings_optimization.md)
* Evening Rush Hour: This sets the driving speed during the specified evening rush hour period defined in [Settings-Optimization](settings_optimization.md)

![Traffic restriction create](/images/traffic_restrictions_create3.png)
