# Traffic restrictions

It is possible to use unlimited traffic restrictions to define areas (also in combination with rush hours) to change driving speed in certain areas. This will decrease driving speed according to the settings when rout optimization is calculated.

Start by activate *Traffic restrictions* in [Settings-Optimization](settings_optimization.md) tab and also define time windows for both morning and evening rush hours.

After that you are ready to create traffic regions. If you want to edit an existing region you can instead click on:
* Edit traffic factors - Edit driving speeds for the region
* Edit traffic region - Edit map area for the region

![Traffic restriction list](/images/traffic_restrictions_list.png)

Push **Add new traffic region** below the list to create a new traffic region.

![Traffic restriction create](/images/traffic_restrictions_create1.png)

Give the traffic region a *Name* and an optional *Description* and click **Create traffic region**. This will open the next window where you define the area by drawing on the map. Zoom the map to your region and click the tool for drawing lines that connects to an area.

![Traffic restriction create](/images/traffic_restrictions_map_drawing_tool.png)

Draw lines around the area where you want to define different driving speeds. A traffic region can only be one area. If you want multiple non-connected areas you need to create multiple regions. When you connect the last line you will get a shaded area on the map. Then click **Save map area**.

![Traffic restriction create](/images/traffic_restrictions_create2.png)

When you have saved the map area you will automatically come to
the page where you define driving speeds. By default all driving speeds are set to 100% but it is possible to change the three sliders.

* Normal speed - Defines driving speed outside both morning and evening rush hours
* Morning rush hour - Defines driving speed between start and end time for morning rush hour defined in [Settings-Optimization](settings_optimization.md)
* Evening rush hour - Defines driving speed between start and end time for evening rush hour defined in [Settings-Optimization](settings_optimization.md)

![Traffic restriction create](/images/traffic_restrictions_create3.png)
