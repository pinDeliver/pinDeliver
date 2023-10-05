# Message schedule

The message scheduler allows you to send messages to customers at specific, recurring times. Rather than relying solely on triggers linked to routing events (such as locking), you can plan messages to be sent consistently at set times. Of course, you can also use this functionality in combination with triggers based on the planning process.

For email messages, you can choose between HTML-coded content or plain text.

Messages will be sent within a time window of approximately ±10 minutes. They will only be sent to route stops where the route is locked, and the scheduled departure date aligns with the weekday specified in the message schedule.

You can view active schedules in the **Schedule** segment.

![Message schedule](/images/settings_message_schedule.png)

|Segment|Field|Explanation|
|-----|----------|----------|
|**Email**|Activate automatic email|Enables automatic email messages to be sent to all recipients on the route based on the schedules.|
|**SMS**|Send SMS automatically|Enables automatic SMS messages to be sent to all recipients on the route based on the schedules.|
|**Create new schedules**|Messages type|Specifies whether to send only email, SMS, or both messages for each schedule.|
||Time|Sets the time of day when the message(s) should be sent.|
||Weekday|Determines whether the message schedule should apply to a specific day or all days. For weekdays-only scheduling, create a schedule for each weekday.|
