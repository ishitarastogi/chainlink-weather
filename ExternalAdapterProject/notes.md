
# Request:
```shell
curl -X POST -H "content-type:application/json" "http://localhost:8080/" --data '{ "id": 0, "data": { "from": "ETH", "to": "USD" } }
```
# Respond:
```shell
{"jobRunID":0,"data":{"USD":3868.71,"result":3868.71},"result":3868.71,"statusCode":200}%  
```
app.js is use only for spin up the server.

custom params are used for additional names in query string ({ "from": "ETH", "to": "USD" } )here from and to can be replaced by any params describe in the custom params. ({ "coin": "ETH", "market": "USD" } )

