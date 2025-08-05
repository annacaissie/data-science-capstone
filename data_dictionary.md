# Data Dictionary

### otp_score: On-Time Performance Score
This is calculated from the MBTA Bus, Commuter Rail, & Rapid Transit Reliability dataset. This dataset provides a numerator and denominator which gives the percentage of passengers who wait the expected headway time or less. This is the performance score used for heavy and light rail.
Source: https://mbta-massdot.opendata.arcgis.com/documents/fc80c306809e452d94b110b0bbc6ac16/explore

### num_of_slow_zones: Number of Slow Zones
This is calculated from the MBTA Rapid Transit Speed Restrictions by Day dataset. This refers to the number of track segments which have an active speed restriction in place.

### total_miles_affected: Total Miles Affected by Speed Restrictions
This is calculated from the MBTA Rapid Transit Speed Restrictions by Day dataset. This refers to the amount of track affected by speed restrictions in miles.

### total_track_pct: Total % of Line Track Affected by Speed Restrictions
This is calculated from the MBTA Rapid Transit Speed Restrictions by Day dataset. This refers to the percentage of the rail line that is impacted by speed restrictions.

### line: The Rapid Transit Line
This refers to the rapid transit line. This can be red (Red Line), blue (Blue Line), orange (Orange Line), or green (Green Line).

### service_date: Date
The row this date appears in contains data pertaining to that date.

### num_alerts: Number of Service Alerts Active
This refers to the number of open service alerts for the specified line and date. This includes delays, service changes, cancellations, and more. This will include alerts that may have been issued on another date but are still active on the specified date.

### has_special_event: Whether that line experienced service alerts caused by special events
This is true when there are alerts present that are caused by special events.

### alert_effect_delay: The number of alerts resulting in a delay
This refers to the number of alerts open on a given day for a given rapid transit line that result in delays.

### alert_effect_shuttle: The number of alerts resulting in shuttle substitutions
This refers to the number of alerts open on a given day for a given rapid transit line that result in shuttle subsitutions for trains.