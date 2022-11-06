
# Rust backend server

## Feature

- [ ] get method
- [ ] post method
- [ ] db crud
- [ ] logger
- [ ] validation
- [ ] file io
  - [ ] read setting files
    - [ ] read json  
    - [ ] read yaml  
    - [ ] read toml  
- [ ] post message for other db
- [ ] auth
- [ ] multi thread

## Usage

### server

```sh
cd json/json
cargo run
# Started http server: 127.0.0.1:8080
```

### web client

With [Postman](https://www.getpostman.com/) or [Rested](moz-extension://60daeb1c-5b1b-4afd-9842-0579ed34dfcb/dist/index.html)

- POST / (embed serde-json):

  - method : `POST`
  - url : `http://127.0.0.1:8080/`
  - header : `Content-Type` = `application/json`
  - body (raw) : `{"name": "Test user", "number": 100}`

- POST /manual (manual serde-json):

  - method : `POST`
  - url : `http://127.0.0.1:8080/manual`
  - header : `Content-Type` = `application/json`
  - body (raw) : `{"name": "Test user", "number": 100}`

- POST /mjsonrust (manual json-rust):

  - method : `POST`
  - url : `http://127.0.0.1:8080/mjsonrust`
  - header : `Content-Type` = `application/json`
  - body (raw) : `{"name": "Test user", "number": 100}` (you can also test `{notjson}`)

### python client

- `pip install aiohttp`
- `python client.py`

if ubuntu :

- `pip3 install aiohttp`
- `python3 client.py`
