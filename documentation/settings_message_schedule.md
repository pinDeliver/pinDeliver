# Message schedule

The message scheduler makes it possible to send messages to the customers att the same time (one or several) every time. Instead of using triggers based on the routing (locking etc) the messages can be planned to be sent at the same time. Off course it is possible to combine this functionality with the triggers based on the planning procedure.

For email messages it is possible to select if the message is HTML coded or just plain text.

Message will be sent within a time span of +-10 minutes and will only be sent to route stops where the route is locked and scheduled departure date matches the weekday provided in the message schedule.

Active schedules can be seen in the segment **Schedule**.

![Message schedule](/images/settings_message_schedule.png)

|Segment|Field|Explanation|
|-----|----------|----------|
|**Email**|Activate automatic email|This message will be sent automatically to all recipients on the route based on the schedules.|
|**SMS**|Send SMS automatically|This message will be sent automatically to all recipients on the route based on the schedules.|
|**Create new schedules**|Messages type|For each schedule you can decide if you want to send only the email, SMS or both messages.|
||Time|Choose the time of the day when the message(s) should be sent.|
||Weekday|Choose iof the message schedule should be used on a particular day (1) or for all days. If you want to schedule messages on weekdays but not on weekdays you need to create a schedule for each weekday.|
