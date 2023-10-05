# Click & Collect

With pinDeliver's Click & Collect functionality, you can implement a professional approach when customers visit your warehouse to personally collect their goods. The process for creating customer orders remains consistent with standard delivery orders. It is essential to note that when utilizing Click & Collect, your  *Delivery Group* must be configured for depot usage.

If you import orders from an Excel file, we recommend uploading all customer orders for a given day simultaneously. This will consolidate all customer orders into a single collection order. During Excel uploads, ensure that you tick the checkbox labeled **Make the order a collection order**, as shown in the image below. Alternatively, if orders are generated through an integration, set the order type to **collect**. This also enables you to add orders to an existing collection order, even if that collection order has been locked or started.

![Click & Collect Create](/images/click_collect_create_1.png)

Once the collection order has been generated, it is time to start the collection process to enable customers to pick up their goods. Click the **Lock** button to secure the collection order, and subsequently, click the **Start collection** button. These actions are typically performed one after the other, but the collection can of course start at a later time if preferable. For instance, you may choose to prepare and lock the collection order the day before and trigger SMS messages to customers the following day when you click **Start collection**.

![Click & Collect Lock](/images/click_collect_1.png)

![Click & Collect Start collection](/images/click_collect_2.png)

You can track the progress of the collection order. Once customer orders have been picked up, they will be relocated to the lower left corner. Generally, there is no need to manually select orders that have not been collected unless you choose to do so.

### Customer information for collect orders
The customer communication for collect orders is quite similar to that of delivery orders. A widely used messaging configuration is demonstrated in the table below, with slight variations depending on whether the customer orders are uploaded from Excel or via an integration.

You can configure messaging settings in the [Admin/Settings/SMS](settings_sms.md) section. Alternatively, for sender-specific messages, you have the option to set up unique messages for each [Sender](senders.md).

|Event|Description|Excel upload|Integration|
|---|-----|:---:|:---:|
|Send SMS when a customer is created|When integrating, customers are often added to an existing collection order, where the **Lock** and **Start Collection** buttons have already been activated. In such cases, we recommend composing the SMS as if the collection process has started. |X|X|
|Send SMS to customers when the driver begins collection.|The SMS will be sent when the **Start collection** is pressed.|X||
|Send SMS to customers when delivery is not collected|SMS sent to all customers who have not picked up their orders when the collection order is marked as completed.|X|X|

The images below show examples of SMS messages for these three scenarios.

<p float="center">
  <img src="/images/cc_sms_customer_1.png" width="300" />
  <img src="/images/cc_sms_customer_2.png" width="300" />
  <img src="/images/cc_sms_customer_3.png" width="300" />
</p>

The images below display examples of the customer information page that customers can access. The QR code can be accessed by clicking the package icon located in the lower right corner of the map picture. This QR code is used when the warehouse uses the Hub App to deliver collect orders.

<p float="center">
  <img src="/images/cc_customer_info_1.png" width="300" />
  <img src="/images/cc_customer_info_2.png" width="300" />
  <img src="/images/cc_customer_info_3.png" width="300" />
</p>

### Deliver a collect order
When the customer arrives for pickup, you have two different methods for marking the order as collected; either from pinDeliver Office or from the Hub App.

#### Delivery from Office
To mark a customer order as collected using Office, simply click the <span style="color:green">**OK**</span> button. However, if you know that the customer will not be picking up the order, select <span style="color:red">**Not collected**</span>. In this case, if the customer plans to collect the order on a different day, you will need to move the order to another collection order. To do this, check the order on the right, and from the drop-down menu, choose the option to move it to another collection order, for instance a collection order scheduled for the day after.

![Click & Collect Lock](/images/click_collect_3.png)

When all customer orders have been collected, you can wrap up the collection order by selecting **Lock Collection**.

#### Delivery from the Hub App
A simple method for marking a customer order as collected is by using the Hub App. Simply select the **Scan QR** button, which will activate the camera. Proceed to scan the QR code from the customer's phone, confirm the pickup on the popup window, and you are all set.

<p float="center">
  <img src="/images/cc_hubapp_1.png" width="300" />
  <img src="/images/cc_hubapp_2.png" width="300" />
</p>

#### Complete collection order
To finalize the collection order, typically when all collect orders have been picked up, just click **Complete collection**. If there are any orders that have not been collected, customers will receive SMS messages if you have configured this.

![Click & Collect Complete collection](/images/click_collect_4.png)
