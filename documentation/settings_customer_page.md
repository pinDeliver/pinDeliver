# Customer page

This settings page is used to define what information and functionality the customer/recipient sees when clicking on the link to the status page.
These settings are common for all orders for this account except for some smaller changes that can be made for a specific sender.

<p float="center">
  <img src="/images/pindeliver_customer_information_page1.png" width="300" />
  <img src="/images/pindeliver_customer_information_page2.png" width="300" />
</p>

![Customer page](/images/settings_customer_page.png)


|Segment|Field|Explanation|
|-----|----------|----------|
|**Customer page**|Display the tracking number on the customer page|Show order tracking number on customer page.|
||Use the fixed tracking URL to access the customer page|Makes it possible to use predefined format on the tracking URL. Makes it possible to generate the tracking URL from other systems by just knowing some values.|
|Customer support chat widget|Display chat widget|Enable possibility to show specific chat widgets. Please contact pinDeliver support for more information.|
||Chat widget script snippet|Paste the script snippet in this field.|
|Edit driver notes from the customer page|Note 1|Show driver notes on the customer page. The customer will see and be able to modify notes. The field is named *Customer info 1* on the order. Can be used to send information to the driver, for instance:<li>Add instructions for the driver</li><li>Update any entry code for the apartment building</li><li>Tell the driver where to leave the goods if the customer will not be home</li>|
||Note 2|Same as *Note 1* above but for *Customer info 2*.|
||Note 3|Same as *Note 1* above but for *Customer info 3*.|
|Show status changes|Display the status changes for a given delivery|Inform the recipient about what status changes have happened with their order, such as:<li>Your order is on it's way from terminal</li><li>Your order is planned and has arrived at terminal</li><li>Your order is in transit</li>|
|Cancel deliveries|Allow customers to cancel deliveries|Check this to make it possible for the customer to cancel a delivery depending ion settings below.|
||Minimum hours before departure for allowing cancel|Specifies how many hours before planned route start that a customer can cancel a delivery.|
||Allow customers to propose another day|Enable this to make it possible to propose another delivery day.|
||Earliest next delivery day after current and number of additional delivery days after that|If a customer want to propose a new delivery day you can specify days ahead before a possible day.|
||Delivery days|Specifies which weekdays that should be possible to select for next delivery.|
||Exclude cancel on non delivery days|Often used to only make it possible to cancel on workdays.Example: the company doesn't have deliveries on Saturday-Sundays and "Minimum hours before departure for allowing cancel" is 24h. Then Monday's deliveries last possible cancellation period should be 24+24+24 before distribution starts.|
|Information to the customer about cancel delivery|Label for the Cancel button|Specify text that should be the label for the **Cancel** button.|
||Label for the propose another day button|Specify text that should be the label for the **Propose another day** button.|
||Confirmation message for the cancelling|This message is displayed when the customer clicks the Cancel button to ensure that the customer really wants to continue cancelling.|
||Information before Cancel|This information is displayed to the customer with the Cancel button.|
||Information after Cancel|This information is displayed to the customer after the Cancel action has been invoked by the user clicking the button.|
