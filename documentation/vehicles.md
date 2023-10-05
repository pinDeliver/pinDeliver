# Vehicles
After the route optimization, the next step is to assign a vehicle to each route. Each vehicle must be associated with a specific delivery group and will only be available for routes within that designated group. Each vehicle comes with set parameters, including availability time, starting position, and optional limitations such as weight capacity, volume, load meters, daily distance, and more.

When adding a vehicle to pinDeliver, you can provide the relevant specifications and any applicable limitations for each vehicle. If you have multiple vehicles with identical specifications and limitations, you can streamline the process by creating a single record and using the *Maximum Number of Resources* field to indicate that you have multiple vehicles with the same specifications.

To create a new vehicle, go to Admin/Vehicles in the main menu. A list of all created vehicles will be displayed, and you can simply click **Add New Vehicle** at the bottom of the list. To make changes to an existing vehicle, click on the vehicle's name or select the *Edit* button to access the vehicle card. Additionally, you have the option to duplicate existing vehicles when creating multiple identical or similar vehicles.

![Vehicles](/images/vehicle_list.png)

Fill in all relevant fields in the vehicle card, and then click **Create Vehicle** to save the information. Refer to the image and field explanations below for guidance.

![Vehicle](/images/vehicle.png)

|Field|Explanation|
|-----|----------|
|Vehicle name|A name for the vehicle or group of vehicles with identical specifications.|
|Maximum number of resources|If you have multiple vehicles with the exact same specifications and limitations, you can specify the quantity here instead of registering each vehicle individually.|
|External resource id|An external identification that can be used when integrating with external systems. Only used when there is a single resource (Maximum number of resources = 1).|
|Working time start|The earliest time of day when the vehicle is available to start work. If it is not always the same, use the "Fixed start time" option.|
|Working time end|The latest time of day until which the vehicle is available. If an "End address" is specified, the vehicle should return there before this time.|
|Fixed start time|Select this if the vehicle always starts at the same time every day, using the "Working time start" as the starting time.|
|Break (in minutes)|Specify a break duration to be planned approximately after the specified “Maximum working time without a break”.|
|Maximum working time without a break|The approximate maximum working time before a break is scheduled for the vehicle.|
|Hourly rate (in SEK)|Set an hourly rate in Swedish Kronor (SEK) for using the vehicle.|
|Start address|The address where the vehicle begins its route each day. It does not have to be the same as the depot address for a delivery group. The route will start by guiding the vehicle to the depot address.|
|End address|The address where the vehicle should end its route daily. Traveling from the last stop to the end address will be included in the route. If no end address is specified, the route will have an "open end".|
|Maximum working time|The maximum total working time for the vehicle. This means that the daily available working time can be less than the time between "Working time start" and "Working time end".|
|Maximum distance|Defines the maximum allowable driving distance in kilometers for the vehicle. This is commonly used for electric vehicles with a maximum range before requiring a recharge.|
|Maximum weight (0 = unlimited)|The maximum load weight that can be carried by the vehicle, using a unit you define (use the same unit as your orders). The route optimization ensures vehicles are not overloaded. However, manually moving customer orders between vehicles can lead to overloading unless you reoptimize the vehicles and recalculate delivery times. If so, use the functionality “Recalculate delivery times”.|
|Maximum volume (0 = unlimited)|The maximum volume capacity that the vehicle can accommodate, using a unit you define (use the same unit as your orders). The route optimization ensures vehicles are not overloaded. However, manually moving customer orders between vehicles can lead to overloading unless you reoptimize the vehicles and recalculate delivery times. If so, use the functionality “Recalculate delivery times”.|
|Maximum volume 2 (0 = unlimited)|An additional volume capacity. For instance, *Maximum volume* can be used for the cold goods capacity, while *Maximum volume 2* can be used for the frozen goods capacity.|
|Delivery group|Assign the vehicle to a specific delivery group. The vehicle will only be available for this particular delivery group, ensuring different warehouses have access to their own vehicles if they are set up as separate delivery groups.|
|Carrier|Connect the vehicle to a specific carrier or logistics partner if necessary.|
|Use default driver|If this vehicle is typically driven by a specific driver, you can select the driver here to make it the default association during route planning.|
|Activation cost|A value that determines the ease of adding another vehicle to the route optimization. A higher value means more time savings are required before adding another vehicle.|
|Vehicle tags. Multiple tags are separated by semicolon, e.g. "tag1;tag2"|Use tags to describe specific vehicle features like cold storage, tailgate lift, or zone classification. When creating a customer order, you can specify one or more vehicle tags, ensuring the order is planned only on a vehicle that matches those tags. A vehicle with tags can still handle orders without tags.|
|CO2/km (In grams, integer)|Specify the amount of CO2 emissions produced per kilometer driven by the vehicle.|
|Use individual speed factor|Select this if you want to adjust the calculated speed for this vehicle in route optimization.|
|Speed factor percentage|This factor specifies how fast the vehicle should be calculated for route optimization compared to the speed limit, useful for larger vehicles with different speed considerations.|
