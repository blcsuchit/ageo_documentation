User model represent the superset of all types of users interacting with the platform.
<h1>Fields</h1>
<h3>name</h3>
```
Type: string
Description: Name of the user
```
<h3>email</h3>
```
Type: string
Description: email id of the user (for logging in)
```
<h3>passwordHash</h3>
```
Type: string
Description: hashed password of the user
```
<h3>role</h3>
```
Type: string
Options: ['APIUSER', 'MANAGER', 'ADMIN']
Defaukt: APIUSER
Description: Role of the user
```
<h3>prefLang</h3>
```
Type: string
Options: ['ENGLISH', 'SPANISH', 'FRENCH', 'PORTUGUESE']
Description: Language preffered by the user
```
<h3>status</h3>
```
Type: string
Options: ['ACTIVE', 'INACTIVE']
Description: Status of user account
```
<h3>apiKey</h3>
```
Type: string
Description: API Key for API User
```
<h3>createdBy</h3>
```
Type: objectId
Description: Id of the user that created this user
```
<h3>createdAt</h3>
```
Type: timestamp
Description: Timestamp of creation
```
<h3>updatedAt</h3>
```
Type: timestamp
Description: Timestamp of last update
```