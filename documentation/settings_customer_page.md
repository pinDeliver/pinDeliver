# Customer page

This settings page is where you can specify the information and features visible to the customer or recipient when they access the status page through the provided link. These settings apply to all orders within the account, with the option for minor adjustments specific to individual senders.

<p float="center">
  <img src="/images/pindeliver_customer_information_page1.png" width="300" />
  <img src="/images/pindeliver_customer_information_page2.png" width="300" />
</p>

![Customer page](/images/settings_customer_page.png)


|Segment|Field|Explanation|
|-----|----------|----------|
|**Customer page**|Display the tracking number on the customer page|Show the order tracking number on the customer page.|
||Use the fixed tracking URL to access the customer page|Enable this setting to use a predefined format for the tracking URL. This allows the generation of the tracking URL from other systems by providing specific values.|
|Customer support chat widget|Display chat widget|Enable the option to display specific chat widgets. Please contact the pinDeliver support for more information.|
||Chat widget script snippet|Paste the script snippet in this field to enable the chat widget.|
|Edit driver notes from the customer page|Note 1|Show driver notes on the customer page. The customer can view and modify notes. The field is named *Customer info 1* on the order and can be used for instructions to the driver, such as:<li>Add instructions for the driver</li><li>Update any entry code for the apartment building</li><li>Tell the driver where to leave the goods if the customer is not home</li>|
||Note 2|Similar to *Note 1*, but for *Customer info 2*.|
||Note 3|Similar to *Note 1*, but for *Customer info 3*.|
|Show status changes|Display the status changes for a given delivery|Inform the recipient about status changes that have occurred with their order, including messages like:<li>Your order is on it's way from the terminal</li><li>Your order is planned and has arrived at the terminal</li><li>Your order is in transit</li>|
|Cancel deliveries|Allow customers to cancel deliveries|Check this option to allow customers to cancel a delivery based on the settings below.|
||Minimum hours before departure for allowing cancel|Specifies the number of hours before the planned route start that a customer can cancel a delivery.|
||Allow customers to propose another day|Enable this option to allow customers to propose an alternative delivery day.|
||Earliest next delivery day after current and number of additional delivery days after that|If a customer wants to propose a new delivery day, you can specify how many days ahead they can do so.|
||Delivery days|Specifies which weekdays should be available for customers to select as the next delivery day.|
||Exclude cancel on non delivery days|This is often used to limit cancellations to workdays. For instance, if the company doesn't deliver on weekends and the cancellation window is set to 24 hours, then the latest time you can cancel Monday's deliveries would be 72 hours before delivery begins.|
|Information to the customer about cancel delivery|Label for the "Cancel" button|Specify the text that should be displayed as the label for the “Cancel” button.|
||Label for the "Propose another day" button|Specify the text that should be displayed as the label for the “Propose another day” button.|
||Confirmation message for the cancelling|This message is displayed when the customer clicks the “Cancel” button to ensure that the customer really wants to proceed with the cancellation.|
||Information before "Cancel"|This information is displayed to the customer along with the ”Cancel” button.|
||Information after "Cancel"|This information is displayed to the customer after they have initiated the cancellation.|
