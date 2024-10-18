Using API methods in food delivery app :

GET Request:
when you open a app the system need to show resturents near your location
the app send a GET request to the server to the nearest resturent your location

POST Request:
you need to send a orders details in this method use the Post request
PUT / orders 
content-type : application/json
{
    "resturentid":1,
    "items":[
    {}
    {}
    ]
    "delivery address":123,
    "pyment method":123,
}
Response:
{
    "orderid":123,
    "status":123
}

PUT Request:
after some time you need to add one more item in your order so used the PUT  request
PUT / orders /123
content-type : application/json
{
   "resturentid":1,
    "items":[
    {}
    {}
    {}
    ]
    "delivery address":123,
    "pyment method":123,  
}
Response:
{
    "orderid":123,
    "status":123
}

DELETE Request:
any reason do you need the cencel a order so use the DELETE  request:
DELETE / orders / 123
Response:
{
    "orderid":123,
    "status":"ordered cencled"
}

