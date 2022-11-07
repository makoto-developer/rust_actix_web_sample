
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

```shell
git clone << git repository url >>
cd rust_actix_web_sample
cargo run
# Started http server: 127.0.0.1:8080
```

### web client

| method | path | token              | Content-Type | note |
|:-------|:-----|:-------------------|:-------------| :------|
| POST   | /    | (embed serde-json) | application/json ||
