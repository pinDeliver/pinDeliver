# Customer communication

One of the key functionalities in pinDeliver is the customer communication that often is done with different SMS messages and links to the *customer information page* that can be branded based on the sender of the goods. But it is also possible to use email as communication method.

This page describes the most common communication workflow with the following messages to the customer:

* Order planned
* Route started
* Order loaded
* Delivery update
* After delivery if customer was not home
* Delivery could not be completed

|Message|Example|Description|
|---|--------|---|
|Order planned|<a><img alt="Order planned" src="/images/customer_communication_locked.png" width="2000"></a>|Depending on how your processes are the planning task can differ. Some companies plan several days ahead but some plan the same day. The more difference you have in time between planning the route and delivering the orders, the more important it is to communicate early. Use SMS/email trigger **Send SMS/email when locking a route** to send message to the customer with planned delivery time.|
|Route started|<a><img alt="Route started" src="/images/customer_communication_started.png" width="2000"></a>|This message is sent when the driver starts the route and the intention is to inform the customer that the delivery is now on the way. If loading is used it is recommended to use the trigger **Order loaded** instead. If you use both it could be very close between the messages and the customer might see it as being spammed.|
|Order loaded|<a><img alt="Order loaded" src="/images/customer_communication_loaded.png" width="2000"></a>|This message is sent when the driver has finished loading the vehicle and the intention is to inform the customer that the delivery is now on the way. If loading is not used it is recommended to use the trigger **Route started** instead. If you use both it could be very close between the messages and the customer might see it as being spammed.|
|Delivery update|<a><img alt="Delivery update" src="/images/customer_communication_update.png" width="2000"></a>|If the delivery was completed without the customer being home this message can be sent to inform the customer that the delivery was done anyway. If you link the status page and use photos the customer will see the photo showing where the goods is placed.|
|After delivery if customer was not home|<a><img alt="Delivery not home" src="/images/customer_communication_nothome.png" width="2000"></a>|If the delivery could not be completed and it is recommended to include text on how the customer should continue. If you link the status page and use photos the customer will see the photo showing that the driver really was at the customer place trying to deliver.|
|Delivery could not be completed|<a><img alt="Delivery not completed" src="/images/customer_communication_notcompleted.png" width="2000"></a>|If the delivery could not be completed and it is recommended to include text on how the customer should continue. If you link the status page and use photos the customer will see the photo showing that the driver really was at the customer place trying to deliver.|
