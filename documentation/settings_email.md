# Email

The main communication form in pinDeliver is through SMS since it is a very fast communication form. But it is also possible to have email as communication method. This makes it possible to have more complex messages and also use HTML code to design them.

It is possible to have general email settings for the whole account but it is also possible to have specific email settings for different senders. In that case you do the email settings under the specific sender. See [Senders](senders.md). If email settings are done for a specific sender that will override the setting described in this page. Remember that the explanations of the fields below is also valid for corresponding field from [Senders](senders.md).

As you see below several fields have the same purpose, that is to write message templates. These messages will be sent based on different triggers. All templates can have **aliases** (place holders) that replace an alias with a text from the customer order, for example customer name, estimated time of delivery. All **aliases** are described in the blue square to the right. For each message it is possible to select if the message is HTML coded or just plain text.


![Email](/images/settings_email.png)

|Segment|Field|Explanation|
|-----|----------|----------|
|**General settings**|Sender name {email-sendername}|Email from pinDeliver is sent with the sender name pinDeliver. If you want to use another sender name you may enter it here. If a sender name has been set in a delivery then that name will be used instead of any name you enter here.|
||Reply address {email-replyaddress}|Email from pinDeliver is sent from the email address noreply<span>@</span>pindeliver.com. If you want customers to be able to answer the email, enter a reply address here.|
||Select language for messages|Here you select for what language you want to write message templates.|
|**Delivery**|Send email when locking a route|When locking a route this message will be sent to all customers on the route.|
||Activate manual email button.|Activate button in the driving list that enables sending emails to all customers in the specific route.|
||Send email when the driver starts the route|When a driver starts a route this message will be sent to all customers in the route.|
||Send email when the driver has finished (re)loading|When the driver clicks "loading done" a message will be sent to all customers that will get a delivery from this load.|
||Send email reminder to a customer when the driver is within X minutes from the destination|Email reminder. Gets sent X minutes from destination. X will be replaced by the reminder time set in *Reminder time, when the driver is X minutes from customer stop* on [SMS settings](settings_sms.md)|
||Send email when a driver reports that a delivery has been made, but the customer was not home|Sends email with time of successful delivery when customer was not home.|
||Send email to customer when a driver reports that a delivery has not been made|Sends email to inform customer that delivery was unsuccessful.|
||Send email when a customer is created|This message will be sent when a customer is created.|
|**Collect**|Send email when the route is locked|When a route is being locked this message will be sent to all customers in the route.|
||Activate manual email button.|When the button is pressed this message will be sent to all customers in the collect order.|
||Send email to customers when the driver is finished at the depot|When the collection order is started at the depot this message will be sent to all customers in the collect order.|
||Send email to customers when delivery is not collected|When the collection order is completed this message will be sent to all customers that have not collected their deliveries.|
||Send email when a customer is created|This message will be sent when a customer is created.|
