
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

# Weather API(FETCHING TEMPERATURE)

# Request:
```shell
curl -X POST -H "content-type:application/json" "http://localhost:8080/" --data '{"id": 0,"data":{"city": "Boston"}}'
```
# Respond:
```shell
{"jobRunID":0,"data":{"coord":{"lon":-71.0598,"lat":42.3584},"weather":[{"id":801,"main":"Clouds","description":"few clouds","icon":"02d"}],"base":"stations","main":{"temp":282.02,"feels_like":279.36,"temp_min":280.43,"temp_max":283.7,"pressure":1011,"humidity":73},"visibility":10000,"wind":{"speed":4.92,"deg":311,"gust":8.94},"clouds":{"all":20},"dt":1634649913,"sys":{"type":2,"id":2013408,"country":"US","sunrise":1634641310,"sunset":1634680568},"timezone":-14400,"id":4930956,"name":"Boston","cod":200,"result":282.02},"result":282.02,"statusCode":200}%
```

Run export API_KEY=YOUR_KEY (Press enter)