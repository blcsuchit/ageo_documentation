User can view all the event reported plotted on a map view. Users can pan and zoom through the map for looking at different events. The map will be anchored around Europe by default. If the user allows location access, the map will get anchored to the user's location

Each event is represented by a separate pin. Multiple pins are clustered together and the total number of clustered pins is shown

<img src="\assets\event_management\map_view.png">

### <h2>Filtering</h2>
Users can use various filters to narrow down on result pins on the map.

#### Event type
User can filter events based on the event type. AGEO Platform supports 11 event types.

<b>Options:</b> Wildfire, Tsunami, Earthquake, Rockfall, Sinkhole, Eruption, Landslide, River Flooding, Marine Flooding, Coastal Erosion, Building Settlement

#### Event status
User can filter events based on the event status. Anonymous users have the option to choose from Approved, Rejected, Pending.

Admins and Managers have additional option to view and filter Archived Events

#### Date
Users can filter events in a date frame. Users can choose start date and end date. By default, no date filters are applied.

#### Polygon
Only Admins and Managers are allowed to filter events by drawing a polygon on the map.
<video autoplay muted controls>
    <source src="\assets\event_management\polygon_filter.mp4" type="video/mp4">
</video>

### Event data download
Admins and Managers can download the event data using download button.
AGEO supports data downloading in 3 formats.

1. JSON - json format supports complete event data dumping
2. Excel - Only structured data is downloaded in this format.(Custom event questionaire answers are not included)
3. CSV - Only structured data is downloaded in this format.(Custom event questionaire answers are not included)

<video autoplay muted controls>
    <source src="\assets\event_management\download.mp4" type="video/mp4">
</video>