# SMS

The primary mode of communication in pinDeliver is through SMS, known for its speed and reliability. While there are general SMS settings available for the entire account, you can also configure specific SMS settings for different senders. To set SMS preferences for a particular sender, navigate to the sender's settings under [Senders](senders.md). Please note that if SMS settings are configured for a specific sender, they will take precedence over the settings described on this page. Keep in mind that the explanations for the fields below also apply to corresponding fields in the [Senders](senders.md) section.

As you can see below, several fields serve the same purpose: creating message templates that are sent based on various triggers. All templates can include aliases (placeholders) that are replaced with specific text from the customer order, such as the customer's name or estimated delivery time. Detailed information about **aliases** can be found in the blue square on the right.

It is essential to carefully consider which triggers you want to utilize, as some triggers may closely overlap in the workflow, potentially leading to excessive communication with the customer.

![SMS](/images/settings_sms.png)

|Segment|Field|Explanation|
|-----|----------|----------|
|**General settings**|||
||Delivery time interval accuracy|This field specifies the length, in minutes, of the delivery time interval displayed to your customers. Use the smallest interval that is manageable for better customer satisfaction.|
||Reminder time, when the driver is X minutes from customer stop.|This setting determines how many minutes before a planned delivery time an SMS should be sent to the customer. pinDeliver will identify deliveries within X minutes and send SMS messages based on the template described below. Please note that only stops within X minutes will receive a message, limited to one message per stop. If your schedule is tight, each stop will only receive one message, even if there are multiple stops within X minutes before reaching the stop. However, if the driving time between stops is greater than X minutes, that stop will not receive any message at all.|
||Select language for messages|Choose the language in which you want to create message templates.|
|**Delivery**|Send SMS when locking a route|This message is sent to all customers on the route when the route is locked.|
||Activate manual SMS button|This setting activates a button in the driving list, allowing the user to send messages to all customers in the route.|
||Send SMS when the driver starts the route|When a driver starts a route, this message is sent to all customers in the route.|
||Send SMS when the driver has finished (re)loading|When the driver marks "loading done", a message is sent to all customers expecting a delivery from this load.|
||Send SMS reminder to a customer when the driver is within X minutes from the destination|This setting triggers an SMS reminder when the driver is X minutes away from the customer's destination. The value of X is determined by the reminder time set in "Reminder time when the driver is X minutes from customer stop".|
||Send SMS when a driver reports that a delivery has been made, but the customer was not home.|Sends an SMS with the time of successful delivery when the customer was not home. If the driver has taken a photo, it will be displayed on the *Customer Information page* that can be linked in the message.|
||Send SMS to customer when a driver reports that a delivery has not been made|Sends an SMS to inform the customer that the delivery was unsuccessful. If the driver has taken a photo, it will be displayed on the *Customer Information page* that can be linked in the message.|
||Send SMS when a customer is created.|This message is sent when a new customer is created.|
|**Collect**|Send SMS when the route is locked|This message is sent to all customers in the route when the route is locked.|
||Activate manual SMS button|Clicking this button sends the message to all customers in the collect order.|
||Send SMS to customers when the driver starts collect|When the collection order is started, this message is sent to all customers in the collect order.|
||Send SMS to customers when the driver is finished at the depot|When click & collect is completed at the depot, this message is sent to all customers in the collect order.|
||Send SMS to customers when delivery is not collected|When the driver reports the route as completed, this message is sent to all customers who have not collected their deliveries.|
||Send SMS when a customer is created.|This message is sent when a new customer is created.|
