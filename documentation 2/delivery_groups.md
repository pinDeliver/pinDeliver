# Delivery groups
Delivery groups are essential when running pinDeliver. Many entities are connected to one or more delivery groups. You can use delivery groups for dividing deliveries into planning orders. For example based on different warehouse locations and/or user permissions. A delivery can only be connected to one delivery group. And planning orders can only consist of deliveries to the same delivery group, which means that a rout will also only have deliveries to the same delivery group. It is possible to have several planning orders for the same delivery group for the same day.

Each delivery group can also have a depot. A depot can be considered as a loading location that doesn't have to be on the same physical location as where the vehicles are starting. A depot is mandatory when using dynamics pickup and delivery or reloading functionality. If you want to include loading time in the routes it is also mandatory to use depots.

To create a new delivery group you select Admin/Delivery groups from the main menu. A list of all created delivery groups is shown and you just click **Add new delivery group** in the bottom of the list.

![Delivery Groups](/images/delivery_group_list.png)

Fill in all relevant fields in the delivery group card and click **Create delivery group** to save it. See image and field explanations below.

![Delivery Group](/images/delivery_group.png)

|Field|Explanation|
|-----|----------|
|Name|Name that should appear in lists visible for users.|
|Identifier|Internal code used in integration.|
|Use depots|Toggle to yes if you want to use default loading time, reloading or dynamics pickup and deliveries.|
|Depot address|The address of the physical depot. Used in route optimization to plan the vehicles to go to the depot before starting.|
|Base stop time|Default stop time (in minutes) if no other stop time is imported for a specific order.|
|Apartment additional stop time|Additional minutes that should be added to the *Base stop time* when the customer order is to an apartment.|
|Business additional stop time (mins)|Additional minutes that should be added to the *Base stop time* when the customer order is to an company (see field b2c in a delivery).|
|Fixed stop time in depot|The stop time in a depot, used both for initial loading and reloading.|
|Apply reloading at optimization|Defines if it should be possible and/or mandatory for the user to use reloading when route optimization is done. Available options are:<ur><li>Never</li><li>Always</li><li>Selectable at optimization</li></ur>|
|Unique click & collect text for customer page|Will be displayed on the customer page. The unique text will not be displayed for deliveries. Only collection orders will see the text on the customer page.|
|Unique text for customer page|Will be displayed on the customer page.|
