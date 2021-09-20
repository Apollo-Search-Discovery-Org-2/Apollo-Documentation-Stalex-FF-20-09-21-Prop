# Accommodation Booking Completed

### 

## Javascript Code
```js
window.appEventData09876 = window.appEventData09876 || [];
appEventData09876.push({
  "event": "Accommodation Booking Completed",
    "booking": {
        "payment": [
            {
                "loyaltyPointsAmount": "<loyaltyPointsAmount>",
                "paymentAmount": "<paymentAmount>",
                "paymentID": "<paymentID>",
                "paymentMethod": "<paymentMethod>",
                "paymentSequence": "<paymentSequence>"
            }
        ],
        "roomList": [
            {
                "location": {
                    "locationId": "<locationId>"
                },
                "room": {
                    "numAdults": "<numAdults>",
                    "numKids": "<numKids>",
                    "numberInMultiRoomReservation": "<numberInMultiRoomReservation>",
                    "rateCode": "<rateCode>",
                    "ratePerNight": "<ratePerNight>",
                    "stayDate": "<stayDate>",
                    "typeCode": "<typeCode>"
                }
            }
        ],
        "total": {
            "currency": "<currency>"
        },
        "transactionID": "<transactionID>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|currency|string|Currency of the payment for the booking. ISO 4217 \(3 character alpha\), uppercase |USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||
|locationId|string|Unique Identifier of a Location. |155, 65588, 987764448|||||||
|loyaltyPointsAmount|integer|Number of loyalty points |100, 101, 1000||||0|||
|numAdults|integer|Integer number of adults for the booking.|1, 2, 3, 4, 5||||1|||
|numKids|integer|Integer number of kids for the booking.|1, 2, 3, 4, 5||||0|||
|numberInMultiRoomReservation|integer|Integer position of a room in a multi-room booking action.|1, 2, 3||||1|||
|paymentAmount|string|String representation of the payment amount. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|paymentID|string|Unique identifier of a payment.  Typically an integration key from a back-end system.|ZPH-87698-098|||||||
|paymentMethod|string|Describes the method of payment for a transaction. |Credit Card, PayPal, Mastercard, Visa, Amex, Discover|||||||
|paymentSequence|integer|Integer indicator of the sequence in which payments were applied within a transaction.  Starting with 1.|1, 2, 3, 4, 5||||1|||
|rateCode|string|Description of the rate being offered. Should match rate codes from back-end systems to allow data import. |AAA, MILITARY, CORP-567, CORP-345|||||||
|ratePerNight|string|String representation of the price per use-period. Typically nightly rate for a hotel room or monthly rate for an apartment. Positive. Up to two decimal places for cents. No currency symbol.|200, 75.29, 150, 89.2|^[0-9]*(\.[0-9]{1,2})?$||||||
|stayDate|string|Date of each room night. ISO 8601 form \(YYYY-MM-DD\). Jan 1, 2019 is 2019-01-01|2001-12-22, 2011-01-01|^([0-9]{4})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12][0-9])$||||||
|transactionID|string|Unique identifier of the transaction. Max Length 20. Used as a key for upload of post transaction data. ||^[a-zA-Z0-9]{6,20}$|6|20||||
|typeCode|string|A code describing the room features. Often indicates number of beds, smoking or non-smoking, ADA accessibility and so on.|1-K-NS, 2-Q-S, S-K-NS-City|||||||



