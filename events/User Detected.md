# User Detected

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "User Detected",
    "user": {
        "affiliateCustomerID": "<affiliateCustomerID>",
        "anonymousUserID": "<anonymousUserID>",
        "country": "<country>",
        "custKey": "<custKey>",
        "customerDetails": {
            "SUID": "<SUID>"
        },
        "loginStatus": "<loginStatus>",
        "loyalty": {
            "memberId": "<memberId>",
            "memberStatus": "<memberStatus>"
        },
        "organizationID": "<organizationID>",
        "profileAttributesList": "<profileAttributesList>",
        "userType": "<userType>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|SUID|string|Captures the user ID based on a cookie.||||||||
|affiliateCustomerID|string|The user ID of user who arrived at the website via a third party partner.||||||||
|anonymousUserID|string|When a user is not logged in,, this captures an anonymous user id.||||||||
|country|string|The country associated with this user's profile.|USA, Canada|||||||
|custKey|string|Unique identifier of a customer.  Any id's considered PII must be hashed. ||||||||
|loginStatus|string|Describes the login state of the user|logged in, logged out, guest|||||||
|memberId|string|Member Identifier in a Loyalty program|abc1234, def876, 87987659|||||||
|memberStatus|string|Member status, level, or tier in a Loyalty program|Gold, Bronze, Platinum, Diamond, Silver|||||||
|organizationID|string|Customer Organization ID associated with website or mobile app behavior.|1234, G72345, Alaska|||||||
|profileAttributesList|string|A twice delimited string of key \/ value pairs.  Use \~ between key and value.  Use \| between pairs|homeStore\~234\|loyaltyTier\~gold\|memberSince\~2002|||||||
|userType|string|Describes the type of the user.  Often used to differentiate customers from employees or associates. |employee, guest, agent, customer|||||||



