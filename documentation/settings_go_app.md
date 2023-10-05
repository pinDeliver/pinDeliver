# The Go app

The pinDeliver Go app is designed to assist drivers and offers a wide range of functionalities. Users can customize the app settings to control what information is displayed to the driver, although certain information is mandatory.

We offer two versions of the app, each with its own unique features. The web app runs directly in a web browser on the device, making it compatible with virtually all devices equipped with a web browser.

The Native app, on the other hand, is specifically developed for Android and iOS devices. Users may notice slight behavioral differences between the two apps. In the web app, all customer data is loaded at once when opening the Driving list. In the Native app, customer data is loaded individually but automatically when the driver completes the previous stop. The Native app also supports the scanning of package numbers during loading, unloading, and other workflows, such as returns.

Both apps are designed to be highly intuitive, requiring minimal training for drivers. The primary task for drivers is to select the type of stop they are making, with three available options and similar instructions in both apps:

* <span style="color:green">**OK**</span> - Indicates that the order was successfully delivered/picked up, and the customer was available to receive the package.
* <span style="color:orange">**OK, NOT AT HOME**</span> - Indicates that the order was successfully delivered/picked up, but the customer was not available to receive the package. This option often includes the option to capture a photo.
* <span style="color:red">**NOT OK**</span> - Indicates that the order/pickup could not be completed. In this case, the driver typically selects a deviation code to explain the issue.

#### Difference between the Go Web App and the Go Native App
<p float="center">
  <img src="/images/pindeliver_go_webapp.png" width="300" />
  <img src="/images/pindeliver_go_native.png" width="300" />
</p>

You can choose to display behavior data using certain settings. Please refer to the settings screenshot and the explanation provided below.

![Go](/images/settings_the_go_app.png)

|Segment|Field|Explanation|Web app supported|Native app supported|
|-----|-----|----------|:---:|:---:|
|**General**|Enable using Go Native app|Allows the use of the Native app.||X|
||Update the driver's position during the route|If enabled, the driver's position updates every minute during an active route. Otherwise, the latest known position, typically the latest stop, is displayed.||X|
||Minutes before planned starting time that the driver is allowed to start the route|Sets the time in minutes before the planned route start when the driver can start the route. A warning is displayed until the planned starting time.|X|X|
||Image for delivery-not-home|Automatically opens the phone camera when handling a **OK, NOT HOME** stop. The photo is visible on the customer page.|X|X|
||Comment on delivery-not-home|Adds the possibility to leave a comment at a **OK, NOT HOME** stop. Requires "Image for delivery-not-home" to be set. |
||Image for delivery-not-delivered|Saves and displays an image for **NOT OK** stops (visible on the customer page).|
||Image for ok-delivered|Saves and displays an image for **OK** stops (visible on the customer page).|
||Comment on delivery-ok|Enables comments for **OK** stops. Requires "Image for OK Delivered" to be enabled. |
||Waze GPS-navigator|Displays a button on each delivery card in the GO app. The button launches Waze as a GPS navigator if installed. Otherwise, it opens the web version of Waze.|
||Display time window|Displays the delivery time window in the GO app.|
||Display sender|Displays the delivery sender in the GO app.|
||Package loading|Gives the driver access to package search functionality, aiding in loading packages onto the correct vehicle.|
||Use offloading scan|Requires the driver to scan goods when offloading at each stop.|
||Handle returns|Permits the driver to receive returnable goods from customers.|
||Driving record|Allows the driver to report a driving record for the route, including details such as vehicle start and stop mileage.|
||Register stop temperature|Permits the driver to report the temperature of goods at each stop.|
|**Driver SMSes**|SMS to driver when the route has been assigned|Sends an SMS to the driver when a route is assigned, given that SMS is chosen as the communication method.|X|X|
|**Driver emails**|Email to driver when the route has been assigned|Sends an email to the driver when a route is assigned, given that email is chosen as the communication method.|X|X|
|**Deviation codes**|Ordering|Allows changing the order of deviation codes available to the driver. Drag and drop codes after creation.|
||Text description|Provides a visible description for drivers in the Go App.|
||Requires comment|Specifies whether the driver must provide a comment when selecting a deviation code.|
||Active|Activates or deactivates a deviation code.|
