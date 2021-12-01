# Neighbour API
This is an API for neighbourhood collaboration site and we want to keep track of people, houses, and addresses of those houses. 
We have collected the following details:
   - Each person has a name, age and number of people in their household
   - Each house has an address and an owner
   - Each address has a postcode and street address

Users are able to:
   - Store people, houses and addresses
   - Look up a house, it’s address and owner
   - Look up people in our neighbourhood within certain age brackets and with specific household sizes

***
# Installation and Setup instructions
1. Clone this repository
2. Setup docker container using the following command
```docker run --name neighbourhood-db --mount type=bind,source="$(pwd)",dst="//code" -d mongo```
3. This App should handle GET, POST and DELETE REQUESTS
4. The various HTTP routes are listed below:

| Path | HTTP Verb | Action |
|--|--|--|
| houses | GET | index houses |
| houses/addresses | GET | index addresses |
| houses/owners | GET | index owners |
