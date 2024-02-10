# Scriptie

A collection of command line utility that i use

## API
API is like postman but specifically for api that return json.
### Dependencies
- curl
- jq
#### Example usage

#### GET Data
```sh
api /api/list-product # this is the same as curl -H 'Content-Type: application/json' localhost:3000/api/list-product | jq | less
```
#### POST Data
```sh
api -d '{"user": "foo", "password": "bar"}' /api/login # this is the same as curl -H 'Content-Type: application/json' -d '{"user": "foo", "password": "bar"}' localhost:3000/api/login | jq | less
```
