Event model represents details of a reported event
<h2>Fields</h2>
<h4>eventId</h4>
```
Type: string
Description: Custom Event Id (name slug) for an event
```
<h4>eventType</h4>
```
Type: string
Options: ['LANDSLIDE', 'ROCKFALL', 'RIVER_FLOODING', 'TSUNAMI', 'EARTHQUAKE', 'BUILDING_SETTLEMENT', 'SINKHOLE', 'ERUPTION', 'WILDFIRE', 'COASTAL_EROSION', 'MARINE_FLOODING']
Description: Custom Event Id (name slug) for an event
```
<h4>time</h4>
```
Type: timestamp
Description: Timestamp when event occurred
```
<h4>status</h4>
```
Type: string
Options: ['PENDING', 'APPROVED', 'REJECTED', 'ARCHIVED']
Default: PENDING
Description: Status of the event
```
<h4>quickReport</h4>
```
Type: boolean
Description: True if event is quick reported
```
<h4>image</h4>
```
Type: array
Description: List of image urls of reported event
```
<h4>comment</h4>
```
Type: string
Description: Comment added by the user
```
<h4>location</h4>
```
Type: object
Description: Co-ordinates of the reported event
```
<h4>city</h4>
```
Type: string
Description: City of event occurrance
```
<h4>state</h4>
```
Type: string
Description: State of event occurrance
```
<h4>country</h4>
```
Type: string
Description: Country of event occurrance
```
<h4>sensorData</h4>
```
Type: object
Description: Sensor data while capturing image of the reported event
```
<h4>commonEventDetails</h4>
```
Type: object
Description: Answers to common event questions
```
<h4>customEventDetails</h4>
```
Type: object
Description: Answers to custom event questions
```
<h4>verifyBy</h4>
```
Type: objectId
Description: Id of the user who verified the event
```
<h4>userAgentDetails</h4>
```
Type: object
Description: User device details
```
<h4>createdAt</h4>
```
Type: timestamp
Description: Timestamp when event was reported
```
<h4>updatedAt</h4>
```
Type: timestamp
Description: Timestamp when event was last updated
```
