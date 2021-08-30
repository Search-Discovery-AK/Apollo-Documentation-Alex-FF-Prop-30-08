# Password Reset Started

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Password Reset Started",
    "user": {
        "custKey": "<custKey>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|custKey|string|Unique identifier of a customer.  Any id's considered PII must be hashed. ||||||||



