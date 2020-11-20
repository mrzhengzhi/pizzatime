# PizzaTime API

This is an API that conveniently provides contact information, menus, open hours, and delivery times of nearby local pizza joints, based on your given postal code.  
PizzaTime API is able to handle queries for single orders as well as bulk orders, provided the right parameters.


## Endpoints
PizzaTime API has two simple GET requests: https://pizzatime.org/json will provide either single order delivery information or bulk order delivery information based on your given parameters.


## Parameters
For single orders:
  * **postCode** (string): Postal code, formatted without spaces. Not case-sensitive. Required.
  * **maxMins** (int): Maximum acceptible waiting time in minutes. Required.
  
For bulk orders:
  * **postCode** (string): Postal code, formatted without spaces. Not case-sensitive. Required.
  * **deliverDate** (string): Delivery date in YYYY-MM-DD. Required.

## Sample requests
These are two sample requests for getting pizza joint information from our API from a given location.

Single order: 
```
https://pizzatime.org/json?postCode=r3t3m2&maxMins=20
```
Bulk order:
```
https://pizzatime.org/json?postCode=r3t3m2&deliverdate=2020-11-11
```

## Sample Responses

Results for single orders:

```
{
  "results":
    {
      "restaurantName"
      "eta"
      "menu"
      "contactInfo"
      "closingTime"
    },
    {
      "restaurantName"
      "eta"
      "menu"
      "contactInfo"
      "closingTime"
    }
}
```
Results for bulk orders:
```
{
  "results":
    {
      "restaurantName"
      "eta"
      "menu"
      "contactInfo"
      "closingTime"
    }
}
```
