# APIs

What does REST stand for?  `application programming interface`

REST APIs are designed around a `Representational State Transfer`

What is an identifer of a resource? Give an example.

>`URI path identifies the API's resource model. Each forward slash separated path segment within the URI corresponds to a unique resource in the model's hierarchy. `

```javascript
`http://api.domain.com/weather`

server.get('/weather', (req, res) => ...
```
What are the most common HTTP verbs?
`POST` `GET` `DELETE`

What should the URIs be based on? `domain/server logic`

Give an example of a good URI.
```javascript
`http://api.domain.com/weather/lat/long/cityname`

```
What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
`the API can be chatty of we are making too many calls to get all the data we need .` and its a bad thing 

What status code does a successful GET request return? `200 OK`
What status code does an unsuccessful GET request return? it depends on the failure resone but we will get `4xx <failure reason>`
What status code does a successful POST request return?`Accepted 202`
What status code does a successful DELETE request return? `410 Gone`

## Things I want to know more about

>`RegExr `