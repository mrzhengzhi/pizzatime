# PizzaTime API

This is an API that conveniently provides contact information, menus, open hours, and delivery times of nearby local pizza joints, based on your given postal code.  
PizzaTime API is able to handle queries for single orders as well as bulk orders, provided the right parameters.

https://pizzatime.org

## Endpoints
PizzaTime API has two simple GET requests: one for **single orders**, the other for **bulk orders**.
  

## Parameters
For single orders:
  * postCode (string): Postal code, formatted without spaces. Not case-sensitive. Required.
  * maxMins (int): Maximum acceptible waiting time in minutes. Required.
  
For bulk orders:
  * postCode (string): Postal code, formatted without spaces. Not case-sensitive. Required.
  * deliverDate (string): Delivery date in YYYY-MM-DD. Required.

## Sample requests
sample requests

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
    "status":"OK"
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
    "status":"OK"
}
```
