# Customer communication

One of the primary features of pinDeliver is customer communication, typically achieved through various SMS messages and links to a customizable *customer information page* that can be branded based on the sender's identity. However, email can also be used as a communication method.

This page outlines the most common communication process.

* Order planned
* Route started
* Order loaded
* Delivery update
* After delivery if customer was not home
* Delivery could not be completed

|Message|Example|Description|
|---|--------|---|
|Order planned|<a><img alt="Order planned" src="/images/customer_communication_locked.png" width="2000"></a>|The way you plan your tasks can vary based on your processes. Some companies plan their routes days in advance, while others plan on the same day. The greater the time gap between planning and delivery, the more crucial it is to communicate early. Use the SMS/email trigger **Send SMS/email when locking a route** to inform customers about their expected delivery time when you lock a route. This helps ensure timely communication.|
|Route started|<a><img alt="Route started" src="/images/customer_communication_started.png" width="2000"></a>|This message is sent when the driver begins their route and the intention is to inform the customer that their delivery is on the way. If you want to communicate that the order is loaded instead, use the trigger **Order loaded**. However, using both the “Order loaded” and “Route started” triggers can be excessive, as these events often occur in close succession, and it might appear as spam to the customer. |
|Order loaded|<a><img alt="Order loaded" src="/images/customer_communication_loaded.png" width="2000"></a>|This message is sent once the driver has completed loading the vehicle, with the aim of notifying the customer that the delivery is now in progress. If you do not want to communicate that the order is loaded, use the trigger **Route started** instead. However, using both the “Order loaded” and “Route started” triggers can be excessive, as these events often occur in close succession, and it might appear as spam to the customer. |
|Delivery update|<a><img alt="Delivery update" src="/images/customer_communication_update.png" width="2000"></a>|When the delivery is on the way, the customer can receive a message indicating that the driver is approaching. The time window for this notification can be adjusted, and the link provided will direct the customer to their dedicated page for tracking delivery information.|
|Delivery without recipient|<a><img alt="Delivery not home" src="/images/customer_communication_nothome.png" width="2000"></a>|If the delivery was made without recipient, for instance if the customer was not at home, this message can be sent to notify the customer about the completed delivery. If you link the status page and include photos, the customer will be able to view a photo showing where the goods were placed.|
|Delivery could not be completed|<a><img alt="Delivery not completed" src="/images/customer_communication_notcompleted.png" width="2000"></a>|If the delivery could be completed, it is recommended to provide instructions for the customer on how to proceed. By linking the status page and include photos, the customer will have visual evidence that the driver attempted delivery at their location.|
