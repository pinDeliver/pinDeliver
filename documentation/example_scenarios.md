# Example scenarios

Here are some example scenarios that can guide you in setting up pinDeliver. You should always begin with the basic setup:

* **Small Company with Deliveries (No Pickups)**
  - Excel upload
  - 1 Terminal/Warehouse
  - Loading is not managed by pinDeliver
  - 2 Vehicles
  - 4 Drivers
  - 1 Sender (Your own company)
  - Communication via SMS when route is *Locked, Started* and for *Not home* and *Not delivered* deliveries
* **Medium Company with Deliveries (No Pickups)**
  - Excel upload
  - 2 Terminals/Warehouses
  - Loading and Reloading Options
  - 5 Vehicles
  - 8 Drivers
  - 1 Sender (Your Own Company)
  - Customer Communication through SMS
* **Click & Collect**
  - Excel upload
  - 1 Terminal/Warehouse
  - 1 Sender (Your Own Company)
  - Communication via SMS when Click & Collect starts for the day and when items are not picked up.
  - Utilize the Hub App for deliveries.

## Small company with deliveries (no pickups)
In this scenario, we outline a typical setup for a small company looking to get started with pinDeliver. To help you begin, we recommend following the setup order provided in the table below.

|Step|Area/Section|Description|
|:-:|---|-----|
|1|[Delivery Group](delivery_groups.md)|Create a delivery group and name it according to your terminal's location. Do not activate the **Use depots**, however, set a default *Base stop time*.|
|2|[Users](users.md)|Add users who will operate within the pinDeliver Office interface. Typically, these users handle tasks like route optimization and customer support.|
|3|[Vehicles](vehicles.md)|Create two vehicles and configure maximum weight and volume limits if you plan to use them when uploading orders. Define work hours, including break times. If you are operating electric vehicles, specify their maximum driving distances. To simplify the process, you can create the second vehicle by copying the first one and making necessary changes like name and unique attributes.|
|4|[Drivers](drivers.md)|Include four drivers in your setup, ensuring you specify their preferred language and valid cell phone numbers. This ensures drivers receive SMS messages in their chosen language.|
|5|[Senders](senders.md)|While your account may already have a default sender, you can enhance its branding by incorporating your company logo and colors for a more personalized customer experience.|
|6|[SMS Communication](settings_sms.md)|In the Settings/SMS section, activate specific SMS triggers for deliveries (located on the left side of the page). Beneath each trigger, you will find examples and recommended messages with placeholders for customization.<ur><li>Send SMS when locking a route</li><li>Send SMS when the driver starts the route</li><li>Send SMS when a driver reports a delivery made, but the customer was not at home </li><li>Send SMS to the customer when a driver reports a delivery as unsuccessful.</li></ur>|

You are now ready to start uploading orders via Excel and start the planning and execution of your deliveries.

## Medium company with deliveries (no pickups)
This scenario describes a typical setup for a midsize company with two different warehouses and the drivers will load the vehicles. You only have to setup a few things before you can start delivering with pinDeliver. Recommended order for your setup is according to the table below.

|Step|Area/Section|Description|
|:-:|---|-----|
|1|[Delivery Group](delivery_groups.md)|Create a unique delivery group for each warehouse, naming them according to their respective locations. Activate the **Use depots** option and input the warehouse address along with the average time required for loading vehicles in the **Fixed stop time in depot**field. Configure "Apply reloading at optimization" as either "Selectable at optimization" or "Always" to enable or enforce reloading as an option during route optimization. Finally, set a default *Base stop time*.|
|2|[Users](users.md)|Add users intended to work in the pinDeliver Office interface, typically those responsible for route optimization and customer support. If necessary, restrict user access to specific warehouses by assigning them to designated delivery groups instead of granting them access to all delivery groups. You can manage this access on the **Delivery groups** tab.|
|3|[Vehicles](vehicles.md)|Create two vehicles and establish maximum weight and volume limits if they are relevant for order processing. Define working hours for each vehicle, including scheduled breaks. If you are using electric vehicles, specify their maximum driving distance. If the two vehicles share similarities, use the **Copy** function to duplicate the first vehicle's configuration, then make necessary adjustments such as the vehicle name and any differing fields, like "Maximum weight." Remember that each vehicle can only be assigned to one delivery group, so specify the appropriate delivery group for each vehicle.|
|4|[Drivers](drivers.md)|Add four drivers to the system and ensure their language preferences and cell phone numbers are correctly set. This ensures that drivers receive SMS messages in the appropriate language. A driver can belong to one or more delivery groups. Simply select or deselect the relevant delivery groups based on each driver's assignment.|
|5|[Senders](senders.md)|Your account may already have a default sender, but you should customize it by adding your company logo and incorporating your brand colors to enhance the appearance of the customer page. Ensure branding is consistent with your company's identity.|
|6|[SMS Communication](settings_sms.md)|Access the "Settings/SMS" section and activate the following SMS triggers for deliveries (located on the left side of the page): Example/recommended messages including place holders can be seen in the blue boxes below each trigger.<ur><li>Send an SMS when locking a route.</li><li>Send an SMS when the driver starts the route.</li><li>Send an SMS when a driver reports that a delivery has been made, but the customer was not available to receive the goods.</li><li>Send an SMS to the customer when a driver reports that a delivery has not been completed.</li></ur> You can find example messages and recommended placeholders in the blue boxes below each trigger to help you set up effective SMS communications for your deliveries|

You are now ready to start uploading orders via Excel and start the planning and execution of your deliveries.

## Click & Collect
This scenario outlines the typical setup for a small company initiating Click & Collect services.

|Step|Area/Section|Description|
|:-:|---|-----|
|1|[Delivery Group](delivery_groups.md)|Create or update a delivery group, naming it after your terminal location. Activate "Use depots" and add your warehouse address for customer collection.|
|2|[Users](users.md)|Add users for pinDeliver Office interface or Hub App. If using the Hub App to deliver, give users the "Is Hub personal" permission.|
|3|[Senders](senders.md)|Customize the default sender with your company logo and branding colors.|
|4|[SMS Communication](settings_sms.md)|In Settings/SMS, activate these SMS triggers for Click & Collect (right side of the page).<ur><li>Send SMS to customers when the driver starts collection</li>Send SMS to customers when delivery is not collected</ur>Example messages, including placeholders, can be seen in the blue boxes below each trigger.|
|5|[Hub App](settings_hub_app.md)|Install the pinDeliver Hub App from Google Play, then log in. Configure the app in settings, selecting your Delivery group/terminal.|


You are now ready to start uploading orders via Excel and start the planning and execution of your deliveries.
