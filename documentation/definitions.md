# Definitions
The table below shows short explanations of basic concepts that are good when learning more about pinDeliver.

|Symbol|Definition|Explanation|
|---------|-----------------------------------------|-----------------|
|![Planning order](/images/icons/planning_order.png)|Planning Order|<ul><li>Group of Customer orders within a geographical area for one Delivery group and supposed to be delivered the same day</li><li>A planning order will be divided into routes after the route planning has been used</li><li>A planning order is normally imported through Excel or API</li></ul>|
|![Route](/images/icons/route.png)|Route|<ul><li>A route with end customers driven by a specified vehicle</li><li>Is created when a planning order is route optimized</li><li>A route can be Unlocked/Locked, Not started/Started/Finished</li></ul>|
|![Customer order](/images/icons/delivery.png)|Delivery|<ul><li>Delivery (or a pickup) to a customer</li><li>Three different type of actions:<ul><li>OK</li><li>Not home</li><li>Not delivered</li></ul><li>Company defined deviation codes can be used when not delivered.</li></ul>|
|![Delivery group](/images/icons/delivery_group.png)|Delivery group|<ul><li>Used to split deliveries based on location, user permissions or other reasons</li><li>A user can have permissions to one or more delivery groups</li><li>A planning order can only consist of orders connected to the same delivery group</li></ul>|
|![Depot](/images/icons/depot.png)|Depot|<ul><li>A loading location that does not be at the same position as the vehicles starting positions</li><li>Each delivery group has a depot</li><li>Each depot has an address and a default loading time used in route optimization</li><li>Enables reloading of vehicles when route planning, that is creating routes with multiple loading stops</li></ul>|
|![Vehicle](/images/icons/vehicle.png)|Vehicle|<ul><li>Connected to a delivery group</li><li>Availability time slots</li><li>Defined starting position</li><li>Can have limits regarding for example weight and volume</li></ul>|
|![Driver](/images/icons/driver.png)|Driver|<ul><li>Connected to one or more delivery groups</li><li>E-mail or mobile phone i mandatory</li><li>Each route is assigned to a driver</li></ul>|
|![Sender](/images/icons/sender.png)|Sender|<ul><li>Each delivery has a senders</li><li>A sender can have e-mail and customer service phone number</li><li>Sender name, e-mail and phone number can be used in customer communication</li></ul>|
|![Package](/images/icons/package.png)|Package|<ul><li>A delivery has at least one package</li><li>A package can be defined with:<ul><li>Name</li><li>Package ID</li><li>Quantity</li><li>Tracking number</li></ul>|
