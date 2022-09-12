# Company features

In company features you define specific settings regarding your pinDeliver account. These settings will be valid for all *Delivery Groups and Senders.*

![Click & collect](/images/settings_company_features.png)

|Field|Explanation|
|----------|----------|
|Subscribe to events|If this setting is on, the current company will be able to subscribe to different event-based events. See also explanation on field **Event URL**|
|Event URL|This is the URL where pinDeliver will send events for different triggers in the platform. Examples of triggers are when orders are routed, a route is started, a delivery has been completed etc.|
|Shipping label as SVG file in pinDeliver API|Use this setting if you want to export shipping labels in SVG format instead of PDF as default. Only valid when using API.|
|Dangerous goods|Dangerous goods controls whether ADR fields should be available.|
|Allow zip code to be omitted for customer addresses|If this setting is off then a zip code will always be required for customer addresses. By turning on this setting you will open up for the possibility to not have a zip code for each order. Address quality is normally lower when not using zip codes although this could be used for example if you often ship to new addresses that has not yet got their zip code or if your address data is missing zip codes.|
|Minimum geolocation accuracy|Minimum geolocation accuracy. Helps determine if an address accuracy is accurate enough to use for route optimization. Default accuracy is 70%.<ur><li>70% Indicates that the returned result reflects a precise geocode.</li><li>60% Indicates that the returned result reflects an approximation (usually on a road) interpolated between two precise points (such as intersections).</li><li>50% Indicates that the returned result is the geometric center of a result such as a polyline (for example, a street).</li><li>25% Indicates that the returned result is approximate.</li>|
