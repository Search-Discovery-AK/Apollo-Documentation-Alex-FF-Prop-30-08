# Page Load Started

### Page Load Started is part of the page load sequence, including virtual page loads in the case of single page apps, and must be the first event pushed in the page load event sequence.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Page Load Started",
    "page": {
        "dayOfWeek": "<dayOfWeek>",
        "detailedPageName": "<detailedPageName>",
        "hour": "<hour>",
        "isIncognitoMode": "<isIncognitoMode>",
        "pageName": "<pageName>",
        "siteName": "<siteName>",
        "weekdayOrWeekend": "<weekdayOrWeekend>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|dayOfWeek|string|The day of the week the activity occured.||||||||
|detailedPageName|string|Describes the page in more detail than the pageName attribute|product - XYZ123 - super cotton neck scarf, Mens - Tops - Sweaters - Supmina, Wool, Rayon, Order Confirmation - 098fghjkl|||||||
|hour|string|The time of activity at the top of the hour.||||||||
|isIncognitoMode|integer|Set on all pages when user is in "incognito mode" in their browser.||||||||
|pageName|string|Describes the page and its content specifically. |product - XYZ123, Mens - Tops - Sweaters, Order Confirmation|||||||
|siteName|string|Common language used within the business to refer to the website. May be specific County Sites.|Prospecting-EU, Prospecting-US, Member Portal, Shop-CA, Shop-US, Shop-EU|||||||
|weekdayOrWeekend|string|Whether it was a week day or weekend when activity is occurred.||||||||



