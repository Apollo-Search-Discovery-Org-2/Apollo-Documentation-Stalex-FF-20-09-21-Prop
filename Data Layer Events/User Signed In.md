# User Signed In

### 

## Javascript Code
```js
window.appEventData09876 = window.appEventData09876 || [];
appEventData09876.push({
  "event": "User Signed In",
    "user": {
        "custKey": "<custKey>",
        "loginStatus": "<loginStatus>",
        "loyalty": {
            "memberStatus": "<memberStatus>"
        },
        "organizationID": "<organizationID>",
        "system": "<system>",
        "userType": "<userType>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|custKey|string|Unique identifier of a customer.  Any id's considered PII must be hashed. ||||||||
|loginStatus|string|Describes the login state of the user|logged in, logged out, guest|||||||
|memberStatus|string|Member status, level, or tier in a Loyalty program|Gold, Bronze, Platinum, Diamond, Silver|||||||
|organizationID|string|Customer Organization ID associated with website or mobile app behavior.|1234, G72345, Alaska|||||||
|system|string|Describes the system that the user is logged into.  \(rarely used\). |admin, shop, member|||||||
|userType|string|Describes the type of the user.  Often used to differentiate customers from employees or associates. |employee, guest, agent, customer|||||||



