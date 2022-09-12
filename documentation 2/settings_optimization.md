# Optimization settings

This page is used for affecting how the optimization engine works for calculating optimal delivery route. Some values are default values and if more specific values exists on delivery groups, customer orders, vehicles etc they will be used instead. The setup also contains functionality to calculate stop times based on

![Language Settings](/images/settings_optimization_settings.png)

|Field|Explanation|
|----------|----------|
|Driving speed|This slider is used to set a speed factor for drivning speed. 100% is normal speed an if you set for example 80% all driving times will be reduced by 20% but still keeping the stop time.|
|Average stop time in minutes|The default stop time for the vehicle used if no other time defined in *Delivery group* or on the customer order.|
|Business additional stop time (mins)|Specifies how many minutres that should be added to a stop if it is classified as a b2b stop. If stop time is specified on the individual customer order this field has no function.|
|From weight|Part of weight table to make it possible to add stop time for heavy goods. This field is connected to the field *Additional Time*.|
|Additional Time|Minutes that should be added to the stop time when weight is above the corresponding *From weight*-field. If you have several setup lines only the highest matching line will be used, meaning the *Additional Time* will not sum all lines above.|
|Earliest delivery time|Default time window start used if there is no delivery time window specified for the vehicle or the customer.|
|Latest delivery time|Default time window end used if there is no delivery time window specified for the vehicle or the customer.|
|Include stop time in delivery time window|If this option is set then all of stop time for a delivery will occur within the delivery time window. Else only the start of the stop time is guaranteed to occur before the delivery time window ends.|
|Delivery time interval that is outside customer's time window|This fields defines how to show delivery times when part of the delivery time interval is outside the customer time window. For instance: If the customer's time window is 4:00 PM-8:00 PM, then the delivery time interval shown can not be between 6:15 PM-8:15 PM, if we choose to clip the delivery time interval.|
|Clipping delivery time interval to customer's time window|This field is only visible if *Delivery time interval that is outside customer's time window* is set to *Clip delivery time...*. For instance: Assume that the customer's time window is 4:00 PM-8:00 PM and the delivery time interval is between 6:15 PM-8:15 PM. The clipping can either offset the delivery time interval to 6:00 PM-8:00 PM or shrink it to 6:15 PM-8:00 PM.|
|Use backorder list|An optimization that fails to route all deliveries will add the failed deliveries to a backorder list, rather than failing completely.|
|Activate traffic regions and traffic limitations|Apply traffic regions and traffic limitations when optimizing route. Rush hours are specified as below.|
|Morning rush hour From|Start time for the morning rush hours. Traffic restrictions are maintained in [Traffic restrictions](traffic_restrictions.md).|
|Morning rush hour To|Stop time for the morning rush hours. Traffic restrictions are maintained in [Traffic restrictions](traffic_restrictions.md).|
|Evening rush hour From|Start time for the evening rush hours. Traffic restrictions are maintained in [Traffic restrictions](traffic_restrictions.md).|
|Evening rush hour To|Stop time for the evening rush hours. Traffic restrictions are maintained in [Traffic restrictions](traffic_restrictions.md).|
