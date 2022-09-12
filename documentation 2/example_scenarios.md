# Example scenarios

Here we have collected a few example scenarios that might help you in "how to think" when setting up pinDeliver. You always need to do the basic setup

* **Small company with deliveries (no pickups)**
  - Excel upload
  - 1 terminal/warehouse
  - Loading is not handled by pinDeliver
  - 2 vehicles
  - 4 drivers
  - 1 sender (your own company)
  - Communication with SMS when route is *Locked, Started* and for *Not home*- and *Not delivered*-deliveries
* **Medium company with deliveries (no pickups)**
  - Excel upload
  - 2 terminals/warehouses
  - Loading and reloading possibility
  - 5 vehicles
  - 8 drivers
  - 1 sender (your own company)
  - customer communication with SMS
* **Click & Collect**
  - Excel upload
  - 1 terminal/warehouse
  - 1 sender (your own company)
  - Communication with SMS when *Click & Collect* starts for the day and it not picked up.
  - Use Hub App for delivering

## Small company with deliveries (no pickups)
This scenario describes a typical setup for a smaller company and you only have to setup a few things before you can start delivering with pinDeliver. Recommended order for your setup is according to the table below.

|Step|Area/Section|Description|
|:-:|---|-----|
|1|[Delivery Group](delivery_groups.md)|Create a delivery group and name it according to your terminal location. Do not activate the **Use depots** but at least add a default *Base stop time*.|
|2|[Users](users.md)|Add users that will work in the pinDeliver Office interface. This normally means users that will do route optimization and customer support.|
|3|[Vehicles](vehicles.md)|Create two vehicles and setup maximum limits for weight and volume if you will use weight and volume when uploading orders. Setup work hours and don´t forget to plan for breaks. If you are using electric vehicles you can add it´s maximum driving distance. If both vehicles are similar you can use the button **Copy** to create the second vehicle. Then you only need to change fields like name and other fields that are not the same, for example **Maximum weight**.|
|4|[Drivers](drivers.md)|Add four drivers and set correct language and cell phone number. This will ensure that the driver gets his SMS messages in correct language.|
|5|[Senders](senders.md)|Your account probably already has a default sender but you want to add your company logo and your colors for branding the customer page correct.|
|6|[SMS Communication](settings_sms.md)|Open **Settings/SMS** and activate the following SMS triggers for the deliveries (left side of page). Example/recommended messages including place holders can be seen in the blue boxes below each trigger.<ur><li>Send SMS when locking a route</li><li>Send SMS when the driver starts the route</li><li>Send SMS when a driver reports that a delivery has been made, but the customer was not home</li><li>Send SMS to customer when a driver reports that a delivery has not been made</li></ur>|

Now you are ready to start uploading orders through Excel and start planning and executing you deliveries.

## Medium company with deliveries (no pickups)
This scenario describes a typical setup for a midsize company with two different warehouses and the drivers will load the vehicles. You only have to setup a few things before you can start delivering with pinDeliver. Recommended order for your setup is according to the table below.

|Step|Area/Section|Description|
|:-:|---|-----|
|1|[Delivery Group](delivery_groups.md)|Create a *Delivery group* for each warehouse and name them according to their location. Activate the **Use depots** and add your warehouse address and average time for loading the vehicles in **Fixed stop time in depot**. You also need to set **Apply reloading at optimization** as *Selectable at optimization* or *Always* to make it possible or forcing reloading as an option when rout optimization. **Finally add a default *Base stop time*.|
|2|[Users](users.md)|Add users that will work in the pinDeliver Office interface. This normally means users that will do route optimization and customer support. If your users should be limited to only work with one of the warehouses you can choose which *Delivery group* a user should be able to access instead of allowing all *Delivery groups*. You do that on the tab called **Delivery groups**.|
|3|[Vehicles](vehicles.md)|Create two vehicles and setup maximum limits for weight and volume if you will use weight and volume when uploading orders. Setup work hours and don´t forget to plan for breaks. If you are using electric vehicles you can add it´s maximum driving distance. If both vehicles are similar you can use the button **Copy** to create the second vehicle. Then you only need to change fields like name and other fields that are not the same, for example **Maximum weight**. A vehicle can only belong to one *Delivery group* so you have to specify for each vehicle which *Delivery group* this vehicle belongs to.|
|4|[Drivers](drivers.md)|Add four drivers and set correct language and cell phone number. This will ensure that the driver gets his SMS messages in correct language. A driver can belong to one or more *Delivery groups*. Just select/deselect *Delivery groups* that are appropriate for the driver.|
|5|[Senders](senders.md)|Your account probably already has a default sender but you want to add your company logo and your colors for branding the customer page correct.|
|6|[SMS Communication](settings_sms.md)|Open **Settings/SMS** and activate the following SMS triggers for the deliveries (left side of page). Example/recommended messages including place holders can be seen in the blue boxes below each trigger.<ur><li>Send SMS when locking a route</li><li>Send SMS when the driver starts the route</li><li>Send SMS when a driver reports that a delivery has been made, but the customer was not home</li><li>Send SMS to customer when a driver reports that a delivery has not been made</li></ur>|

Now you are ready to start uploading orders through Excel and start planning and executing you deliveries.

## Click & Collect
This scenario describes a typical setup for a smaller company that will start with Click & Collect

|Step|Area/Section|Description|
|:-:|---|-----|
|1|[Delivery Group](delivery_groups.md)|Create or update a delivery group and name it according to your terminal location. Activate the **Use depots** and add your warehouse address to show your customers where they should go for the collection.|
|2|[Users](users.md)|Add users that will work in the pinDeliver Office interface or in the Hub App. If you will deliver with the Hub App the users must have *Is Hub personal* as permission.|
|3|[Senders](senders.md)|Your account probably already has a default sender but you want to add your company logo and your colors for branding the customer page correct.|
|4|[SMS Communication](settings_sms.md)|Open **Settings/SMS** and activate the following SMS triggers for the Click & Collect (right side of page). Example/recommended messages including place holders can be seen in the blue boxes below each trigger.<ur><li>Send SMS to customers when the driver starts collect</li>Send SMS to customers when delivery is not collected</ur>|
|5|[Hub App](settings_hub_app.md)|Install pinDeliver HubApp from Google Play. Login to the app and go to settings and choose *Delivery group/terminal*.|


Now you are ready to start uploading orders through Excel and start planning and executing you deliveries.
