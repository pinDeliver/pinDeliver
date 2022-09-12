# SMS

The main communication form in pinDeliver is through SMS since it is a very fast and reliable communication form. It is possible to have general SMS settings for the whole account but it is also possible to have specific SMS settings for different senders. In that case you do the SMS settings under the specific sender. See [Senders](senders.md). If SMS settings are done for a specific sender that will override the setting described in this page. Remember that the explanations of the fields below is also valid for corresponding field from [Senders](senders.md).

As you see below several fields have the same purpose, that is to write message templates. These messages will be sent based on different triggers. All templates can have **aliases** (place holders) that replace an alias with a text from the customer order, for example customer name, estimated time of delivery. All **aliases** are described in the blue square to the right.

It is important to think through which triggers you want to use. Some triggers often come very close in the work process and then that could be seen as spamming the customer.

![SMS](/images/settings_sms.png)

|Segment|Field|Explanation|
|-----|----------|----------|
|**General settings**|||
||Delivery time interval accuracy|This field describes the delivery time interval length in minutes that you want to show to your customer. Use as small interval as you are comfortable with and able to handle for better customer satisfaction.|
||Reminder time, when the driver is X minutes from customer stop.|Approximately how many minutes before a planned delivery time a SMS should be sent to the customer. Every time the driver completes a stop pinDeliver will look for deliveries within X minutes and send SMS to these according to the template described below. Only stops within X minutes will get a message, and only one message. This means that if you have a tight schedule each stop will only get one message if if you have more stops within X minutes before reaching the stop. On the other hand, if you driving time between stops is more than X minutes that stop will not get any message at all.|
||Select language for messages|Here you select for what language you want to write message templates.|
|**Delivery**|Send SMS when locking a route|When locking a route this message will be sent to all customers on the route.|
||Activate manual SMS button|Activate button in the driving list to be able to send messages to all customers in route.|
||Send SMS when the driver starts the route|When a driver starts a route this message will be sent to all customers in the route.|
||Send SMS when the driver has finished (re)loading|When the driver clicks "loading done" a message will be sent to all customers that will get a delivery from this load.|
||Send SMS reminder to a customer when the driver is within X minutes from the destination|SMS reminder. Gets sent X minutes from destination. X will be replaced by the reminder time set in *Reminder time, when the driver is X minutes from customer stop.*|
||Send SMS when a driver reports that a delivery has been made, but the customer was not home.|Sends SMS with time of successful delivery when customer was not home. If the driver has taken a photo that will be shown on the *Customer information page* that could be linked in the message.|
||Send SMS to customer when a driver reports that a delivery has not been made|Sends SMS to inform customer that delivery was unsuccessful. If the driver has taken a photo that will be shown on the *Customer information page* that could be linked in the message.|
||Send SMS when a customer is created.|This message will be sent when a customer is created.|
|**Collect**|Send SMS when the route is locked|When a route is being locked this message will be sent to all customers in the route.|
||Activate manual SMS button|When the button is clicked this message will be sent to all customers in the collect order.|
||Send SMS to customers when the driver starts collect|When the collection order is started this message will be sent to all customers in the collect order.|
||Send SMS to customers when the driver is finished at the depot|When click & collect is finished at the depot this message will be sent to all customers in the collect order.|
||Send SMS to customers when delivery is not collected|When the driver reports the route is completed this message will be sent to all customers that have not collected their deliveries.|
||Send SMS when a customer is created.|This message will be sent when a customer is created.|
