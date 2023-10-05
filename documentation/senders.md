# Senders
Every customer order is associated with a sender. For instance, this can be the transportation company handling the delivery or the retailer that sold the goods. Each customer order can have only one sender, but within a planning order, different customer orders can have different senders. Senders play a crucial role in customer communication, informing recipients of the source of the goods. As a result, each customer order is branded based on the sender, even when multiple senders share the same route and vehicle.

Senders can be branded with distinct logos, colors, instructive text, and customer service phone numbers, which are displayed on the customer page (GET page).

By default, pinDeliver includes one primary sender. This means that if you do not specify a particular sender for a customer order, the default sender will be used.

To create a new sender, navigate to Admin/Senders in the main menu. A list of all senders will be displayed, and you can click **Add new sender** at the bottom of the list to create a new one. To modify an existing sender, simply click the sender's name or the **Edit** button to access the sender card.

![Senders](/images/sender_list.png)

### Sender
The sender's primary tab provides essential details about the sender's name and contact information. Complete all the relevant fields in the sender card, and then click **Create** to save the information. Refer to the image and field explanations below for guidance.

![Sender](/images/sender_sender.png)

|Field|Explanation|
|-----|----------|
|Sender|The official name of the sender, displayed to the end customer.|
|SMS sender|A short name, up to 11 characters, displayed as the SMS sender name.|
|Sender ID|A unique identifier used for integration or Excel uploads of customer orders.|
|Customer service number|Phone number to the sender's customer service, displayed to the end customer.|
|Customer service email|Email address to the sender's customer service, displayed to the end customer.|
|Street|Street address to the sender, displayed to the end customer.|
|Zip code|Sender's zip code, displayed to the end customer.|
|City|The city where the sender is located, displayed to the end customer.|

### Settings
Customized settings for individual senders allow you to tailor your communication based on the sender's identity. This flexibility enables distinct messaging or SMS triggers depending on the sender.

In pinDeliver, a default sender is a standard feature. Therefore, if a customer order is not assigned a specific sender, the default sender will be applied automatically.

![Settings](/images/sender_settings.png)

|Field|Explanation|
|-----|----------|
|Allow change sender settings|Lets you set unique options for a specific sender.|
|Show packages on customer page|Displays packages on the customer's page.|
|Allow digital signature|Allows customers to sign digitally upon delivery.|

### SMS
If you want unique SMS templates or triggers for a particular sender, you can set them up on this page. You will find detailed explanations of these SMS templates and triggers in the [SMS settings tab](settings_sms.md).

![SMS](/images/sender_sms.png)

### Email
If you want customized email templates or triggers for a specific sender, you can configure them on this page. Detailed explanations of these email templates and triggers can be found in the [Email settings tab](settings_email.md).

![Email](/images/sender_email.png)

### Theme
On this tab, you can personalize the appearance of the customer information page. If you do not add any colors or images here, the settings of the default sender will be applied. Since pinDeliver allows for multiple senders (one per customer order), you can provide customers with a distinct look and feel based on the sender of the goods.

![Theme](/images/sender_theme.png)

|Field|Explanation|
|-----|----------|
|Light color|Background color in text areas on the customer information page. A recommended color code is #F0F0F0, as it provides a bright but not white background.|
|Text color|Text color for lead texts (see explanatory text under the field **Driver notes** in the right example image below). |
|Dark color|Background color on the time schedule sign on the first page and header texts (see header text **Driver notes** in the right example image below). |
|Sender logotype|Click the button to upload a file that will appear in the top left corner of the customer information page. Recommended size is 664x182 pixels. It is recommended to use a transparent background for the best appearance.|
|Delivery/pickup location icon|Click the button to upload an icon representing pickup or drop-off locations. Recommended size is 72x72 pixels.|
|Truck current location icon|Click the button to upload an icon indicating the current position of the vehicle. Recommended size is 72x72 pixels.|
|Font URL|A URL link to a specific font for text on the customer information page.|
|Font name|The name of the font specified in the Font URL.|

#### Examples of customer information page.
<p float="center">
  <img src="/images/sender_theme_customer_page_1.png" width="300" />
  <img src="/images/sender_theme_customer_page_2.png" width="300" />
</p>
