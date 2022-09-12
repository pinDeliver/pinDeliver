# The Go app

The pinDeliver Go app is a tool for the driver. This is an app with a lot of functionality and it is also possible to use different settings to control what should be visible for the driver even though some information is mandatory.

We have developed two different apps with similar functionality but some important differencies. The web app is run directly in a web browser on the device which means that more or less all devices with a web browser can run this app.

The so called Native app is developed for Android and iOS devices. The users can see a slightly different behavior between the apps. In the web app all customers are loaded at once when opening the *Driving list* but in the native app each stop is loaded separately but automatically when finishing the previous stop. The Native app has support for scanning package numbers when loading and unloading and some other flows, for example returns.

The apps themselves are very intuitive and doesn´t need much of education for the drivers. The main task for the drivers is just to select what kind of stop they make. They have three different stop types to select from with similar lead texts in the different apps:

* <span style="color:green">**OK**</span> - Order delivered/picked up and the customer was home
* <span style="color:orange">**OK, NOT AT HOME**</span> - Order delivered/picked up but the customer was not home. Often combined with a photo.
* <span style="color:red">**NOT OK**</span> - Order/Pickup could not be handled. The driver normally select a deviation code.

#### Difference between Go web-app and native app
<p float="center">
  <img src="/images/pindeliver_go_webapp.png" width="300" />
  <img src="/images/pindeliver_go_native.png" width="300" />
</p>

It is possible to select behavior data to view with some settings. See settings screenshot and explanation below.

![Go](/images/settings_the_go_app.png)

|Segment|Field|Explanation|Web app supported|Native app supported|
|-----|-----|----------|:---:|:---:|
|**General**|Enable using Go Native app|This will enable the use of the Native app.||X|
||Update the driver's position during the route|If this is set then the driver's position will be updated every minute while the route is active. Else the latest known position, which will be the latest stop, will be shown.||X|
||Minutes before planned starting time that the driver is allowed to start the route|Until the specified number of minutes before the planned route's starting time it will not be possible to start the route. After that, until the planned starting time, a warning will be displayed.|X|X|
||Image for delivery-not-home|This will open the phone camera automatically when a a stop is handled as **NOT OK**. The photo will be visible on the customer page.|X|X|
||Comment on delivery-not-home|Adds the possibility to leave a comment at delivery-not-home. Can only be set if "Image for delivery-not-home" is set.|
||Image for delivery-not-delivered|Save and show image on delivery-not-delivered. (The image will appear at the customer page)|
||Image for ok-delivered|Save and show image on ok-delivered. (The image will appear at the customer page)|
||Comment on delivery-ok|Adds the possibility to leave a comment at delivery-ok. Can only be set if "Image for delivery-ok" is set.|
||Waze GPS-navigator|When this is set a button will be displayed on each delivery card in the GO app. The button will start Waze as GPS navigator if it is installed, or else Waze web version will be started. Click here to read more about [Waze GPS-navigator](https://www.waze.com/live-map/).|
||Display time window|When display time window is set, the delivery time window will be displayed in the GO app.|
||Display sender|When display sender is set, the delivery sender will be displayed in the GO app.|
||Package loading|Will give the driver access to search. Search result will help the driver to load packages on to the correct truck or car.|
||Use offloading scan|Require the driver to scan goods for offloading on arrive at a stop.|
||Handle returns|The driver may receive returnable goods from the customer.|
||Driving record|The driver reports a driving record for the route. Data that is reported is for example vehicle start and stop mileage.|
||Register stop temperature|The driver reports good's temperature at each stop.|
|**Driver SMSes**|SMS to driver when the route has been assigned|The SMS is sent when a route is assigned and SMS has been selected for communicating the message to the driver.|X|X|
|**Driver emails**|Email to driver when the route has been assigned|The email is sent when a route is assigned and email has been selected for communicating the message to the driver.|X|X|
|**Deviation codes**|Ordering|Used to change order of the deviation codes that the driver can choose from. Just drag'n'drop the deviation codes when you have created them.|
||Text description|Description visible for driver in the Go App.|
||Requires comment|Defines if the driver needs ta write a comment or not.|
||Active|Activate a deviation code by turning on and off.|
