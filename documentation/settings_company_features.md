# Company features

Within the *Company Features* section, you can establish customized settings for your pinDeliver account. These settings will apply to all *Delivery Groups* and *Senders*.

![Click & collect](/images/settings_company_features.png)

|Field|Explanation|
|----------|----------|
|Subscribe to events|When enabled, the company can subscribe to various event-based notifications. For event details, refer to the **Event URL** field explanation|
|Event URL|This is the URL where pinDeliver sends event notifications for different triggers within the platform. Triggers include events like order routing, route start, and delivery completion.|
|Shipping label as SVG file in pinDeliver API|Use this setting if you prefer to export shipping labels in SVG format instead of the default PDF format. This is only applicable when using API.|
|Dangerous goods|This setting controls the availability of ADR fields. If enabled, these fields will be available for use.|
|Allow zip code to be omitted for customer addresses|When turned off, a zip code will always be required for customer addresses. Enabling this setting allows flexibility in not requiring a zip code for every order, which can be useful for new addresses or when address data is missing zip codes.|
|Minimum geolocation accuracy|This setting specifies the minimum geolocation accuracy required to consider an address accurate enough for route optimization. Default accuracy is 70%.<ur><li>70% Indicates that the returned result reflects a precise geocode.</li><li>60% Indicates that the returned result reflects an approximation (usually on a road) interpolated between two precise points (such as intersections).</li><li>50% Indicates that the returned result is the geometric center of a result such as a polyline (for example, a street).</li><li>25% Indicates that the returned result is approximate.</li>|
