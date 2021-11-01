# go-rollercoaster-api

> A simple REST API based on the kubucation [YouTube tutorial](https://www.youtube.com/watch?v=2v11Ym6Ct9Q)

## Requirements


* [x] `GET /coasters` returns list of coasters as JSON
* [x] `GET /coasters/{id}` returns details of specific coaster as JSON
* [x] `POST /coasters` accepts a new coaster to be added
* [x] `POST /coasters` returns status 415 if content is not `application/json`
* [x] `GET /admin` requires basic auth
* [x] `GET /coasters/random` redirects (Status 302) to a random coaster

### Data Types

A coaster object should look like this:
```json
{
  "id": "someid",
  "name": "name of the coaster",
  "inPark": "the amusement park the ride is in",
  "manufacturer": "name of the manufacturer",
  "height": 27,
}
```

### Persistence

There is no persistence, a temporary in-mem story is fine.
