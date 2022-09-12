# Click & Collect

With pinDeliver Click & Collect functionality you get a professional approach when your customers come to your warehouse to pickup their goods themselves. The customer orders are created in the same way as regular delivery orders. Remember that when using Click & Collect your *Delivery Group* must be setup to use depot.

If you upload order from Excel it is recommended to upload all customer orders for a day at once. Then you will have all customer orders grouped in one collection order. If you upload through Excel you need to mark the checkbox *Make the order a collection order*, see image below. If the orders instead are created through an integration the order type should be **collect** and then it is also possible to add orders to an existing collection order, even if the collection order has been locked or started.

![Click & Collect Create](/images/click_collect_create_1.png)

When the collection order has been created it is time to start the collection process, so the customers can pickup their goods. Click the **Lock** button to lock the collection order and after that you click **Start collection** button. This can often be done right after each other but if you want to start the collection at a later time of the day it is recommended to start the collection then. That would mean that you prepare and lock the collection order for example the day before and trigger SMS messages to the customers the day after when you click **Start collection**.

![Click & Collect Lock](/images/click_collect_1.png)

![Click & Collect Start collection](/images/click_collect_2.png)

You can see the progress on the collection order. Collected customer orders will be moved to the lower left corner when they have been picked up. Normally you do not have to select not collected orders if you don´t want to.

### Customer information for collect orders
The information to the customer is very similar for collect orders compared to delivery orders. A very common setup for messages is according to the table below and it is a little different if the customer orders are uploaded from Excel or via an integration.

The messagsing setup is done from [Admin/Settings/SMS](settings_sms.md) or if you want sender unique messages you can setup that for each [Sender](senders.md).

|Event|Description|Excel upload|Integration|
|---|-----|:---:|:---:|
|Send SMS when a customer is created|With integration a customer is often added to an existing collection order so the buttons **Lock** and **Start collection** has already been pushed. In this case we recommend to write the SMS as if the collection has started.|X|X|
|Send SMS to customers when the driver starts collect|The SMS will be sent when **Start collection** is pushed.|X||
|Send SMS to customers when delivery is not collected|SMS sent to all customer that has not picked up their orders when the collection orders is marked as finished.|X|X|

The images below shows examples of SMS messages for these three steps.

<p float="center">
  <img src="/images/cc_sms_customer_1.png" width="300" />
  <img src="/images/cc_sms_customer_2.png" width="300" />
  <img src="/images/cc_sms_customer_3.png" width="300" />
</p>

The images below shows examples of the customer information page that the customer can see. The QR code is accessed by clicking the package icon in the lower right corner of the map picture and is used when the warehouse uses the Hub App to deliver the collect orders.

<p float="center">
  <img src="/images/cc_customer_info_1.png" width="300" />
  <img src="/images/cc_customer_info_2.png" width="300" />
  <img src="/images/cc_customer_info_3.png" width="300" />
</p>

### Deliver a collect order
When the customer arrives for pickup you have two different ways of check the order as picked up.

* Office - just click the button <span style="color:green">**OK**</span>
* Hub App - scan a QR code form the customer information page, see below.

#### Delivery from Office
To mark a customer order as picked up from Office you just click <span style="color:green">**OK**</span> button. Choose <span style="color:red">**Not collected**</span> if you know that the customer will now pick up the order. In that case you need to move the order to another collection order if the customer will come another day. this is done by checking the order to the right an from the drop-down menu you can select to move to another collection order, for example a collection order for tomorrow.

![Click & Collect Lock](/images/click_collect_3.png)

When all customer order have been picked up you finish the collection order by clicking

#### Delivery from the Hub App
A very easy way of mark a customer order as picked up is to use the Hub App. Just choose the button **Scan QR**. This will open the camera and you just scan the QR code from the customer´s telephone. Confirm pickup on the popup window and you are done.

<p float="center">
  <img src="/images/cc_hubapp_1.png" width="300" />
  <img src="/images/cc_hubapp_2.png" width="300" />
</p>

#### Complete collection order
When you want to complete the collection order (normally when all collect orders have been picked up) you just click **Complete collection**. If an orders have not been picked up these customers will get SMS messages if you have setup that as above.

![Click & Collect Complete collection](/images/click_collect_4.png)
