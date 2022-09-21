# Main menu

The main menu in pinDeliver is self-adapting based on the activated company functionality and the user permissions. That means that the main menu doesn´t necessary looks as the images on this page.

![Main menu](/images/main_menu.png)

See information below about the different parts from the main menu.

### Overview
The overview part is also similar to the start page in pinDeliver. This is where you see all plannings orders as an overview page. By default this page filters on planning orders 3 days back but it is possible to change the date filters on your own. this page will also open if you click on the pinDeliver logo in top left corner.

If you want to upload orders from an Excel file you use the green button to the right called **Add order**.

Orders that are uploaded/imported to the *Inbox* are found by clicking on the grey button showing number of orders in the inbox.

![Overview](/images/main_menu_overview.png)

### Search
From the *Search* menu you have two different options.

* Search customer/delivery - Search for a customer order
* Search package - Search for a specific package and get more details

![Search customer/delivery](/images/main_menu_search_customer_delivery0.png)

#### Search customer/delivery
To easily find a customer order you can use the *Search customer/delivery*-functionality from *Search* on the main menu. It is possible to search for customers based on different criteria. You can select specific fields to search in or just keep all fields marked. If you for example search for *Göteborg* you will get all customer orders having *Göteborg* in the name or in city unless you change the search fields.

* Tracking number
* Customer number
* Name
* Address
* Zip code
* City
* Phone
* Reference    

![Search customer/delivery](/images/main_menu_search_customer_delivery1.png)

After a search you will get a list of all customers that are found. You can also see how many orders you have for a that customer. By clicking on the customer you will come to a list showing all customer orders for this customer.

![Search customer/delivery](/images/main_menu_search_customer_delivery2.png)

The list of customer orders are split in *Routed deliveries* and *Unrouted deliveries*. To see the specific order just click on the **Edit** or **Show** buttons to the right. If you want to see all customers orders on a route or planning order you can click their names instead.

#### Search package
To easily find a package you can use the *Search package*-functionality from *Search* on the main menu. Select the package in the list of packages. You can filter on *Date, Delivery Group, Route Name* and *Package Id*. In the list you see the current status of the package.

![Search packages](/images/main_menu_search_package1.png)

To see a detailed view of the package lifecycle you just click the *Package Id*. Ont he following page you will see timestamps of all events for the package and you can also follow the physical movement on a map.

If something has gone wrong and you want to change the package status you can mark the package in the list ans select **Action / Return to the previous status**.

![Search packages](/images/main_menu_search_package2.png)

### Messages
It is possible to send custom messages through SMS or email. This functionality can be triggered from the different routes or manually by clicking on this menu item. It is possible to type an ad-hoc message or use templates.

The message functionality is for example used to trigger manual messages when a route has been delayed for some reason and you want to message all remaining customers.
More information about this functionality can be in [Send custom messages](send_custom_messages.md).

![Search customer/delivery](/images/main_menu_messages.png)

### History
Normally you do not have to remove or archive any orders after completion. But if an order is *Archived* you will find it under the History-section.

![History](/images/main_menu_history.png)

### Followup
Under *Followup* you find several reports and pages for showing statistics, finished orders etc.

![Followup](/images/main_menu_followup.png)

### Admin
In the section *Admin* you find all available settings. These settings should be done before starting your first deliveries but you can off course change and add settings over time. Read more about these in [Settings](settings.md).

![Admin](/images/main_menu_admin.png)

### API
The API section describes the different standard methods used for REST communication to pinDeliver. These are always available and you must first add an API user, read more about this in [Users](users.md).

Another way is to use pinDeliver Service Center as a middleware. Service Center can be used for data-population, business logic etc. This means that it will be easier for you as an integrator if the Service Center is used. Please contact pinDeliver before starting developing an integration.

### Guide
The Guide section links to this online help. It is the same online help that is also linked from [www.pindeliver.com](https://www.pindeliver.com)

### Company name/User name
By clicking on your username in the upper right corner you get a small menu with a few options:

![Commpany/User](/images/main_menu_companyname_username.png)

* Notifications - Smaller messages, for example about customers with addresses with low gps coordinate quality.
* News - Release news and other news from pinDeliver.
* My profile - Here you can change your own contact information, password, language setting etc.
* Log out - To log out current user.
