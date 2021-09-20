# Onsite Search Performed

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData09876 = window.appEventData09876 || [];
appEventData09876.push({
  "event": "Onsite Search Performed",
    "onsiteSearch": {
        "keyword": {
            "searchType": "<searchType>"
        }
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|searchType|string|Describes the domain of the search. |products, properties, articles, authors, coupons, publications|||||||



