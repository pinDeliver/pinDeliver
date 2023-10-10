# Optimization settings

This page is dedicated to configuring the optimization engine's behavior when calculating optimal delivery routes. While default values are available, the system can prioritize more specific settings assigned to delivery groups, customer orders, vehicles, and other entities. Additionally, the setup includes functionality for calculating stop times based on specific parameters.

![Language Settings](/images/settings_optimization_settings.png)

|Field|Explanation|
|----------|----------|
|Driving speed|Adjusts the speed factor for driving. 100% represents normal speed, and setting it to, for example, 80% will reduce driving times by 20% while maintaining stop times.|
|Average stop time in minutes|Default stop time for the vehicle if no other time is defined in the delivery group or on the customer order.|
|Business additional stop time (mins)|Specifies the additional minutes added to a stop if it is categorized as a business-to-business (B2B) stop. If stop time is defined on the individual customer order, this field has no effect.|
|From weight|Part of the weight table used to add stop time for heavy goods. Connected to the "Additional Time" field.|
|Additional Time|Number of minutes added for the specified weight in the 'From Weight' field. You can add multiple rows with different specifications.|
|Earliest delivery time|Default time window start used if no delivery time window is specified for the vehicle or the customer.|
|Latest delivery time|Default time window end used if no delivery time window is specified for the vehicle or the customer.|
|Include stop time in delivery time window|If enabled, the entire delivery will happen during the specified time window. If not, we can only guarantee delivery at the start of the delivery window before it ends.|
|Delivery time interval that is outside customer's time window|Defines how to display delivery times when part of the delivery time interval is outside the customer's time window. For example, if the customer's time window is 4:00 PM-8:00 PM, this setting determines how delivery times are shown when they fall between 6:15 PM-8:15 PM.|
|Clipping delivery time interval to customer's time window|This option is visible only when "Delivery time interval that is outside customer's time window" is set to "Clip delivery time." For example, if the customer's time window is 4:00 PM-8:00 PM and the delivery time interval is 6:15 PM-8:15 PM, this setting allows you to choose whether to offset the delivery time interval to 6:00 PM-8:00 PM or shrink it to 6:15 PM-8:00 PM.|
|Use backorder list|Instead of failing a route optimization that can't route all deliveries, this option adds the failed deliveries to a backorder list.|
|Activate traffic regions and traffic limitations|Enables the application of traffic regions and traffic limitations during route optimization. Morning and evening rush hours are specified below.|
|Morning rush hour From|The start time for morning rush hours. Traffic restrictions are adjusted in the [Traffic restrictions](traffic_restrictions.md) section.|
|Morning rush hour To|The end time for morning rush hours. Traffic restrictions are adjusted in the [Traffic restrictions](traffic_restrictions.md) section.|
|Evening rush hour From|The start time for evening rush hours. Traffic restrictions are adjusted in the [Traffic restrictions](traffic_restrictions.md) section.|
|Evening rush hour To|The end time for evening rush hours. Traffic restrictions are adjusted in the [Traffic restrictions](traffic_restrictions.md) section.|
