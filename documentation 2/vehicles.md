# Vehicles
After route optimization you connect a vehicle to each route. A vehicle must be linked to a delivery group and will only be available for that delivery group when assigning vehicles to routes. Each vehicle always has an availability time and a starting position. And it is also possible to have limitations regarding for example, weight, volume, load meters, daily distance etc.

For each vehicle you have available for pinDeliver you add it to pinDeliver with relevant specifications and limitations. If you have many vehicles with exactly the same limitations and specifications you can add only one record and use the field *Maximum number of resources* to specify that you have more than one vehicle with exactly the same specifications.

To create a new vehicle you select Admin/Vehicles from the main menu. A list of all created vehicles is shown and you just click **Add new vehicle** in the bottom of the list. To change an existing vehicle you just click the vehicle name or the **Edit** button to open the vehicle card. It is also possible to copy existing vehicles if you want to create many equal or similar vehicles.

![Vehicles](/images/vehicle_list.png)

Fill in all relevant fields in the vehicle card and click **Create vehicle** to save it. See image and field explanations below.

![Vehicle](/images/vehicle.png)

|Field|Explanation|
|-----|----------|
|Vehicle name|A name for the vehicle or group of vehicles if more than one with same specifications.|
|Maximum number of resources|If you have more than one vehicle with exactly the same specifications and limitations you can specify how many in this field instead of registering all vehicles one by one.|
|External resource id|An external id that can be used in integration for external systems. Only used when *Maximum number of resources* is 1.|
|Working time start|Earliest time on the day when the vehicle is available to start. Not necessary the exact start time, then use *Fixed start time*.|
|Working time end|Latest time on the day which the vehicle is available until. If *End address* is used the vehicle should be able to return to that address before this time.|
|Fixed start time|Check this field if you always want the vehicle to start at the same time every day. The starting time will be *Working time start*.|
|Break (in minutes)|This field make sure a route has a break planned after approximately the working hours specified in *Maximum working time without a break *.|
|Maximum working time without a break|Approximate maximum working time before a break is planned for the vehicle.|
|Hourly rate (in SEK)|Specifies an hourly rate for using the vehicle in SEK.|
|Start address|The address where the vehicle starts every day. Does not have to be the same as a depot address for a delivery group. The route will the start by guiding the vehicle to the depot address.|
|End address|The address where the vehicle should end it´s route every day. Going from the last stop to the end address will be included inte the route. If no end address is specified the route will have so called "open end".|
|Maximum working time|Maximum total working time for the vehicle. Meaning that the daily available working time can be less than the time between *Working time start* and *Working time end*.|
|Maximum distance|Defines maximum available driving distance in kilometers for a vehicle. Very common to use for electrical vehicles with a maximum mileage before needing to charge again.|
|Maximum weight (0 = unlimited)|The maximum weight that can be loaded on the vehicle in a self-defined unit (just use the same unit as on your orders). The route optimization will make sure the vehicles doesn´t get overloaded. However if you manually move customer orders between vehicles it will be possible to overload unless you reoptimize the vehicles again. You then use the functionality to *Recalculate delivery times* the route.|
|Maximum volume (0 = unlimited)|The maximum volume that can be loaded on the vehicle in a self-defined unit (just use the same unit as on your orders). The route optimization will make sure the vehicles doesn´t get overloaded. However if you manually move customer orders between vehicles it will be possible to overload unless you reoptimize the vehicles again. You then use the functionality to *Recalculate delivery times* the route.|
|Maximum volume 2 (0 = unlimited)|Additional volume possibility. For example *Maximum volume* can be used for cold goods capacity and *Maximum volume 2* can be used for frozen goods capacity.|
|Delivery group|In this field you assign the vehicle to a delivery group. The vehicle will only be available for this particular delivery group. This means that different warehouses will only have access to their own vehicles if the warehouses are setup as delivery groups.|
|Carrier|Makes it possible to connect a vehicle to a specific co-operation carrier.|
|Use default driver|If this vehicle is normally driven by a specific driver you can choose the driver here to make it default associated when route planning.|
|Activation cost|A value used to define how "easy" it should be to add one more vehicle to the route optimization. The higher value in this field the more time should be saved before adding another vehicle.|
|Vehicle tags. Multiple tags are separated by semicolon, e.g. "tag1;tag2"|Can be used to describe specific features for the vehicle like cold, freeze, tailgate lift, zone etc. In a customer order it is possible to specify one or more vehicle tags and then that order can only be planned on a vehicle that matches those tags. A vehicle that uses tags can still handle orders without tags.|
|CO2/km (In grams, integer)|Specify the amount of CO2 emission produced per kilometer the vehicle is driving.|
|Use individual speed factor|Select this if you want to increase or decrease the calculated speed for this vehicles for route optimization.|
|Speed factor percentage|A bigger truck could use a lower speed percentage to be calculated with a lower speed in optimization. This factor specifies how fast the vehicle should be calculated for in the optimization compared to the speed limit.|
