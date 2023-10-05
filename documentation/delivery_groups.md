# Delivery groups
Delivery groups are essential when planning in pinDeliver, as they help organize various entities. Entities can be associated with one or more delivery groups, making it easier to divide deliveries into planning orders. This division can be based on factors such as distinct warehouse locations or user permissions. It is important to note that a delivery can only be linked to one delivery group. Consequently, planning orders can only consist of deliveries belonging to the same delivery group, resulting in routes exclusively containing deliveries from that group. It is entirely possible to have multiple planning orders for the same delivery group scheduled for the same day.

Additionally, each delivery group can be assigned a depot, which functions as a loading location. The depot does not necessarily need to be physically located where the vehicles begin their routes. However, a depot becomes mandatory when utilizing dynamic pickup and delivery or reloading features. If you intend to include loading time in your routes, using depots is also compulsory.

To create a new delivery group, navigate to Admin/Delivery groups in the main menu. A list of all delivery groups created will be displayed, and at the bottom of this list, you can click on **Add new delivery group** to create a new one.

![Delivery Groups](/images/delivery_group_list.png)

Fill in all the relevant fields in the delivery group card, and then click **Create delivery group** to save your changes. Refer to the image and field explanations provided below for further guidance.

![Delivery Group](/images/delivery_group.png)

|Field|Explanation|
|-----|----------|
|Name|The name that appears in lists visible to users.|
|Identifier|An internal code used for integration purposes.|
|Use depots|Shift to "Yes" if you want to utilize default loading time, reloading, or dynamics pickup and deliveries.|
|Depot address|The address of the physical depot, used in route optimization to plan vehicle routes to the depot before starting.|
|Base stop time|Default stop time (in minutes) if no other stop time is imported for a specific order.|
|Apartment additional stop time|Additional minutes added to the “Base stop time” for customer orders delivered to apartments.|
|Business additional stop time (mins)|Additional minutes added to the “Base stop time” for customer orders delivered to companies (see field B2B in a delivery).|
|Fixed stop time in depot|The stop time in a depot, used for both initial loading and reloading.|
|Apply reloading at optimization|Defines if reloading should be possible and/or mandatory during route optimization. Options include: <ur><li>Never</li><li>Always</li><li>Selectable at optimization</li></ur>|
|Unique click & collect text for customer page|Text displayed on the customer page for collection orders. This unique text is not displayed for deliveries.|
|Unique text for customer page|Text displayed on the customer page.|
