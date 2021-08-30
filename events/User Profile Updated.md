# User Profile Updated

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "User Profile Updated",
    "user": {
        "profileUpdateType": "<profileUpdateType>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|profileUpdateType|string|Captures the type of profile update \(i.e. change email\) completed by the visitor.|email, address, phone, subscriptions|||||||



