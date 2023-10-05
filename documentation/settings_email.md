# Email

The primary communication method in pinDeliver is SMS, known for its speed. However, email is also an available communication option, allowing for more complex messages and HTML code for design.

You have the option to set general email preferences for the entire account or define specific email preferences for various senders. When email preferences are established for a particular sender, they will take priority over the settings outlined on this page. Please note that the field explanations below are also applicable to corresponding fields in the [Senders](senders.md) section.

As you can see below, several fields serve the same purpose: creating message templates triggered by various events. All templates can include **aliases** (placeholders) that will be replaced with text from the customer order, such as the customer's name or estimated delivery time. You can also choose whether each message should be in HTML or plain text format.


![Email](/images/settings_email.png)

|Segment|Field|Explanation|
|-----|----------|----------|
|**General settings**|Sender name {email-sendername}|Email sent from pinDeliver displays the sender name as pinDeliver. You can specify a different sender name in this field. If a sender name is provided in a delivery, it will take priority over this setting.|
||Reply address {email-replyaddress}|By default, emails from pinDeliver are sent from the email address noreply<span>@</span>pindeliver.com. If you want customers to be able to reply to the email, you can enter a reply address in this field.|
||Select language for messages|Choose the language in which you want to compose message templates.|
|**Delivery**|Send email when locking a route|When a route is locked, this email message is sent to all customers on the route.|
||Activate manual email button.|Enables a button in the driving list that allows sending emails to all customers on the specific route.|
||Send email when the driver starts the route|When a driver starts a route, this email message is sent to all customers in the route.|
||Send email when the driver has finished (re)loading|When the driver clicks "loading done," a message is sent to all customers who will receive a delivery from this load.|
||Send email reminder to a customer when the driver is within X minutes from the destination|An email reminder is sent X minutes from the destination. X is replaced by the reminder time set in the SMS settings for "Reminder time, when the driver is X minutes from customer stop".|
||Send email when a driver reports that a delivery has been made, but the customer was not home|Sends an email with the time of successful delivery when the customer was not home.|
||Send email to customer when a driver reports that a delivery has not been made|Sends an email to inform the customer that the delivery was unsuccessful.|
||Send email when a customer is created|This message is sent when a new customer is created.|
|**Collect**|Send email when the route is locked|When a route is locked, this email message is sent to all customers in the route.|
||Activate manual email button.|When the button is pressed, this email message is sent to all customers in the collect order.|
||Send email to customers when the driver is finished at the depot|When the collection order is started at the depot, this email message is sent to all customers in the collect order.|
||Send email to customers when delivery is not collected|When the collection order is completed, this email message is sent to all customers who have not collected their deliveries.|
||Send email when a customer is created|This email message is sent when a customer is created.|
