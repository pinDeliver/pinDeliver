# SMS


EJ KLAR



The main communication form in pinDeliver is through SMS since it is a very fast communication form. It is possible to have general SMS settings for account but it is also possible to have specific SMS settings for different senders. In that case you do the SMS settings under the specific sender. See [Senders](senders.md). If SMS settings is done for a specific sender that will override the setting described in this page. Remember that the explanations of the fields below is also valid for corresponding field from [Senders](senders.md).

As you see below several fields have the same purpose, that is to write message templates. These messages will be sent based on different triggers. All templates can have **aliases** (place holders) that replace an alias with a text from the customer order, for example customer name, estimated time of delivery. All **aliases** are described in the bug blue square to the right.

![Click & collect](/images/settings_sms.png)

|Segment|Field|Explanation|
|-----|----------|----------|
|**General settings**|||
||Delivery time interval accuracy|This field describes the delivery time interval length in minutes that you want to show to your customer. Use as small interval as you are comfortable with and able to handle for better customer satisfaction.|
||Reminder time, when the driver is X minutes from customer stop.|Approximately how many minutes before a planned delivery time a SMS should be sent to the customer. Every time the driver completes a stop the platform will look for deliveries within X minutes and send SMS to these according to the template described below. Only stops within X minutes will get a message, and only one message. This means that if you have a tight


EJ KLAR
