User model represent the superset of all types of users interacting with the platform.
<h2>Fields</h2>
<h4>name</h4>
```
Type: string
Description: Name of the user
```
<h4>email</h4>
```
Type: string
Description: email id of the user (for logging in)
```
<h4>passwordHash</h4>
```
Type: string
Description: hashed password of the user
```
<h4>role</h4>
```
Type: string
Options: ['APIUSER', 'MANAGER', 'ADMIN']
Defaukt: APIUSER
Description: Role of the user
```
<h4>prefLang</h4>
```
Type: string
Options: ['ENGLISH', 'SPANISH', 'FRENCH', 'PORTUGUESE']
Description: Language preffered by the user
```
<h4>status</h4>
```
Type: string
Options: ['ACTIVE', 'INACTIVE']
Description: Status of user account
```
<h4>apiKey</h4>
```
Type: string
Description: API Key for API User
```
<h4>createdBy</h4>
```
Type: objectId
Description: Id of the user that created this user
```
<h4>createdAt</h4>
```
Type: timestamp
Description: Timestamp of creation
```
<h4>updatedAt</h4>
```
Type: timestamp
Description: Timestamp of last update
```