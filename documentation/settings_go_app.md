# The Go app

The pinDeliver Go app is the app for the driver, a tool for the driver. This is an app with a lot of functionality and it is also possible to use different settings to control what should be visible for the driver even though som information is mandatory.

We have developed two different apps with similar functionality but some important differencies. The web app is run directly in a web browser on the device which means that more or less all devices with a web browser can run this app. The so called Native app is developed for Android and iOS devices. The users can see a slightly different behaviour between the apps. In the web app all customers are loaded at once when opening the *Driving list* but in the native app each stop is loaded separately but automatically when finishing the previous stop. The Native app has support for scanning package numbers when loading and unloading and some other flows, for example returns.

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

|Field|Explanation|Web app supported|Native app supported|
|-----|----------|:---:|:---:|
|Enable using Go Native app|This will enable the use of the Native app.||X|
|Update the driver's position during the route|If this is set then the driver's position will be updated every minute while the route is active. Else the latest known position, which will be the latest stop, will be shown.||X|
|Minutes before planned starting time that the driver is allowed to start the route|Until the specified number of minutes before the planned route's starting time it will not be possible to start the route. After that, until the planned starting time, a warning will be displayed.|X|X|
|SMS to driver when the route has been assigned|The SMS is sent when a route is assigned and SMS has been selected for communicating the message to the driver.|X|X|
|Email to driver when the route has been assigned|The email is sent when a route is assigned and email has been selected for communicating the message to the driver.|X|X|
|Image for delivery-not-home|This will open the phone camera automatically when a a stop is handled as **NOT OK**. The photo will be visible on the customer page.|X|X|


INTE KLAR
