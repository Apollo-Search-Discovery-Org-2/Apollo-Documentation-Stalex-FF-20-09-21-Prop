# Order Placed

### 

## Javascript Code
```js
window.appEventData09876 = window.appEventData09876 || [];
appEventData09876.push({
  "event": "Order Placed",
    "cart": {
        "cartID": "<cartID>"
    },
    "transaction": {
        "item": [
            {
                "altPersonPickUp": "<altPersonPickUp>",
                "fulfillment": {
                    "method": "<method>",
                    "source": "<source>",
                    "storeID": "<storeID>"
                },
                "price": {
                    "basePrice": "<basePrice>",
                    "markdownPrice": "<markdownPrice>",
                    "priceTier": "<priceTier>",
                    "priceType": "<priceType>",
                    "sellingPrice": "<sellingPrice>"
                },
                "productInfo": {
                    "brand": "<brand>",
                    "color": "<color>",
                    "isSample": "<isSample>",
                    "name": "<name>",
                    "productID": "<productID>",
                    "productLine": "<productLine>",
                    "sku": "<sku>",
                    "trademarkedTechnology": "<trademarkedTechnology>"
                },
                "quantity": "<quantity>",
                "shippingAddress": {
                    "stateProvince": "<stateProvince>"
                },
                "shippingCost": "<shippingCost>",
                "shippingMethod": "<shippingMethod>",
                "shippingVoucherCode": "<shippingVoucherCode>",
                "shippingVoucherDiscount": "<shippingVoucherDiscount>",
                "tax": "<tax>",
                "voucherDiscount": {
                    "orderLevelDiscountAmount": "<orderLevelDiscountAmount>",
                    "orderLevelDiscountCode": "<orderLevelDiscountCode>",
                    "productLevelDiscountAmount": "<productLevelDiscountAmount>",
                    "productLevelDiscountCode": "<productLevelDiscountCode>"
                }
            }
        ],
        "payment": [
            {
                "loyaltyPointsAmount": "<loyaltyPointsAmount>",
                "paymentAmount": "<paymentAmount>",
                "paymentID": "<paymentID>",
                "paymentMethod": "<paymentMethod>",
                "paymentSequence": "<paymentSequence>"
            }
        ],
        "productIDList": "<productIDList>",
        "profile": {
            "address": {
                "country": "<country>",
                "postalCode": "<postalCode>"
            }
        },
        "purchaseID": "<purchaseID>",
        "skuList": "<skuList>",
        "total": {
            "currency": "<currency>",
            "numPayments": "<numPayments>",
            "revenue": "<revenue>"
        },
        "transactionID": "<transactionID>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|altPersonPickUp|integer|When a user has put in the information of an alternate pick up person during the checkout process.||||||||
|basePrice|string|String representation of MSRP of a product. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|brand|string|Describes the brand of a product or offering.|Ford, Chevrolet, Dodge, Levis, Columbia, Patagonia|||||||
|cartID|string|Back-end identifier for a shopping cart|12345, 435678, 34567, XCV456, XCV876|||||||
|color|string|Describes the colorway of a product or product variant|Antique Oak, Granite, Black Marble, Knotty Pine|||||||
|country|string|Indicates the country of the billing address. ISO 3166 \(alpha-2\) Uppercase.|US, CA, FR, UK|^[A-Z]{2}$||||||
|currency|string|Currency of the transaction. ISO 4217 \(3 character alpha\), uppercase |USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||
|isSample|string|True\/False flag to indicate if the product is a sample.|true, false|||||||
|loyaltyPointsAmount|integer|Number of loyalty points |100, 101, 1000||||0|||
|markdownPrice|string|String representation of the price offered. Often called 'hard mark' price. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|method|string|Describes the method of fulfillment|Shipped, Emailed, Pick Up In Store, Will Call|||||||
|name|string|Name of the product or offering.  Should be unique and 1:1 with productID|Oceana, Corsica, Flame Tech, Air Jordan 88|||||||
|numPayments|integer|Collects the number of payment methods used for an order at order confirmaton||||||||
|orderLevelDiscountAmount|string|String representation of an order level discount applied to an item in a transaction. Positive. Up to two decimal places for cents. No currency symbol.|5, 20, 10.22, 19.2|^[0-9]*(\.[0-9]{1,2})?$||||||
|orderLevelDiscountCode|string|Order Level Discount code applied at the item level of a transaction. |FRIENDSANDFAMILY20, EASTER10|||||||
|paymentAmount|string|String representation of the payment amount. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|paymentID|string|Unique identifier of a payment.  Typically an integration key from a back-end system.|ZPH-87698-098|||||||
|paymentMethod|string|Describes the method of payment for a transaction. |Credit Card, PayPal, Mastercard, Visa, Amex, Discover|||||||
|paymentSequence|integer|Integer indicator of the sequence in which payments were applied within a transaction.  Starting with 1.|1, 2, 3, 4, 5||||1|||
|postalCode|string|The mailing zip or postal code associated with the billing address. |53533, 30381, M1R 0E9, M3C 0C1|||||||
|priceTier|string|Describes the general pricing tier of a product. \(Good, Better, Best\)|Good, Better, Best, Bronze, Silver, Gold|||||||
|priceType|string|Describes the type of price offered using commonly used terms. |1st mark, 2nd mark, 3rd mark, clearance, sale, doorbuster|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|productIDList|string|A delimited list of product IDs in the transaction.|1234\|7878\|9039, abc12\|deh213, abc12|||||||
|productLevelDiscountAmount|string|String representation of product level discount for a transaction. Positive. Up to two decimal places for cents. No currency symbol.|5, 20, 10.22, 19.2|^[0-9]*(\.[0-9]{1,2})?$||||||
|productLevelDiscountCode|string|Discount code applied for a specific item \(or items\) of a transaction. |5OFFSHOES, AKRONCANDLES2019|||||||
|productLine|string|Describes the product Line of a product. |Laminate Wood, Vinyl, Hardwood, Stone, Ceramic|||||||
|purchaseID|string|Unique identifier of the purchase. Max Length 20. Used as Unique ID of the purchase or deduplication.|ABC-132456789, DEF-132456789, 0987654567|^[a-zA-Z0-9]{6,20}$|6|20||||
|quantity|integer|Integer number of products being acted upon \(added to a cart, removed from wishlist, purchased, reserved\)|1, 2, 3, 4, 5||||1|||
|revenue|string|The total revenue for a transaction. Does not include tax or shipping. |125.05, 432.21, 90.22, 12.05|^[0-9]*(\.[0-9]{1,2})?$||||||
|sellingPrice|string|String representation of the price paid after coupons or discounts. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|shippingCost|string|The shipping costs for all items within the shippingGroup of the transaction.|15.05, 2, 0.22, 2.2|^[0-9]*(\.[0-9]{1,2})?$||||||
|shippingMethod|string|Describes the method or carrier and method of shipment. Should be common terminology within your business. |Regular, Overnight, Overnight AM, Overnight AM Sat, UPS Ground, UPS Air|||||||
|shippingVoucherCode|string|Discount code applied against shipping costs for a shipping Group|FREESHIPAPRIL, FREESHIP100|||||||
|shippingVoucherDiscount|string|String representation of an discount applied against shipping costs for a shipping group. Positive. Up to two decimal places for cents. No currency symbol.|5, 20, 10.22, 19.2|^[0-9]*(\.[0-9]{1,2})?$||||||
|sku|string|Stock Keeping Unit \(SKU\) Unique Identifier of specific item \(typically\) held in inventory.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level below productID for products with SKU variants. |34567890, 4567890, 00155-large-cornflower|||||||
|skuList|string| A delimited list of skus in the transaction.|sku123\|sku465, 67890\|87576\|74674, 87654|||||||
|source|string|Describes the entity responsible for fulfillment. Uasge is flexible.|Vendor:xyz, Store:43567, Email:system3, Warehouse:7865|||||||
|stateProvince|string|The mailing state or province associated with address of the shipment. |WI, GA, NB, ON|||||||
|storeID|string|A unique identifier for the store that the order was placed with.|stew's boot shop, kat's cat toys, 12345|||||||
|tax|string|String representation of the tax collected at a shipment level for a transaction. Positive. Up to two decimal places for cents. No currency symbol.|5.05, 20, 10.22, 9.2|^[0-9]*(\.[0-9]{1,2})?$||||||
|trademarkedTechnology|string|Describes trademarks and\/or technical branding used to describe the product|Stainmaster, GoreTex, WeatherShield|||||||
|transactionID|string|Unique identifier of the transaction. Max Length 100. Used as a key for upload of post transaction data. |123e4567-e89b-12d3-a456-426614174000|^[a-zA-Z0-9]{6,100}$|6|100||||



