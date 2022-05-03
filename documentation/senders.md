# Senders
All customer orders have a sender. A sender can be the transportation company delivering the order or for example the retailer company that sold the goods. A customer order can only have one sender but all customer orders in a planning order can have different senders. The senders are used in the customer communication telling the customer from which sender the goods are coming. This means that each customer order is branded according to the sender, even when many senders share the same route and vehicle.

The sender can be branded by using different logo, colors, instructive text and customer service phone number etc shown on the customers page (GET page).

In pinDeliver you will always have one default sender. This means that if you do not specify a specific sender on a customer order, the default sender will be used.

To create a new sender you select Admin/Senders from the main menu. A list of all senders is shown and you just click **Add new sender** in the bottom of the list. To change an existing sender you just click the sender name or the **Edit** button to open the sender card.

![Senders](/images/sender_list.png)

### Sender
This is the main tab for the sender with information about name and contact information.
Fill in all relevant fields in the sender card and click **Create** to save it. See image and field explanations below.

![Sender](/images/sender_sender.png)

|Field|Explanation|
|-----|----------|
|Sender|The official name of the sender. this will be shown to the customer.|
|SMS sender|A short name that will be shown as the name of the SMS sender. Maximum length of 11 characters.|
|Sender ID|A unique sender identifier value used for integration or Excel upload of customer orders.|
|Customer service number|Phone number to the sender´s customer service. Will be shown to the end customer.|
|Customer service email|Email to the sender´s customer service. Will be shown to the end customer.|
|Street|Street address to the sender. Will be shown to the end customer.|
|Zip code|Zip code to the sender. Will be shown to the end customer.|
|City|City to the sender. Will be shown to the end customer.|

### Settings
It is possible to have specific settings for specific senders. This makes it possible to different settings depending on who the sender is. For example different SMS messages or triggers for SMS.

pinDeliver always have a default sender, meaning that if you don´t specify the sender for a customer order the default sender will be used instead.

![Settings](/images/sender_settings.png)

|Field|Explanation|
|-----|----------|
|Allow change sender settings|If this is checked it is possible to have different settings for this specific sender compared to the default sender.|
|Show packages on customer page|Check this to show the packages on the custoemr page.|
|Allow digital signature|Check this to make it possible to use digital signature for the customer when receiving goods.|

### SMS
When you want different SMS templates or triggers for a specific sender you have to specify them in this page. The different SMS templates and triggers are explained in the [SMS settings tab](settings_sms.md).

![SMS](/images/sender_sms.png)

### Email
When you want different email templates or triggers for a specific sender you have to specify them in this page. The different email templates and triggers are explained in the [Email settings tab](settings_email.md).

![Email](/images/sender_email.png)

### Theme
In this tab you customize the look of the customer information page. The settings for the default sender will be used if you don´t add any colors or images to this settings tab. Since pinDeliver supports multiple senders (one per customer order) it is possible to give the customers different look & feel depending on the sender of the goods.

![Theme](/images/sender_theme.png)

|Field|Explanation|
|-----|----------|
|Light color|Background color in text areas on the customer information page.|
|Text color|Text color for lead texts.|
|Dark color|Background color on time schedule sign on first page.|
|Sender logotype|Click button to upload file that will be visible in top left corner on the customer information page. Recommended size is 664x182 pixels.|
|Delivery/pickup location icon|Click button to upload icon showing the pickup or dropoff location. Recommended size is 72x72 pixels.|
|Truck current location icon|Click button to upload icon for showing current position of the vehicle. Recommended size is 72x72 pixels.|
|Font URL|An url to a specific font for texts on the customer information page.|
|Font name|Name for the font specified in the link above.|

![Customer Information Page 1](/images/settings_theme_customer_page_1.png)

![Customer Information Page 2](/images/settings_theme_customer_page_2.png)
