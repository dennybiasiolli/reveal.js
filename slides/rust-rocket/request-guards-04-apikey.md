#### Request Guard examples

```rust
#[rocket::async_trait]
impl<'r> FromRequest<'r> for ApiKey<'r> {
    type Error = ApiKeyError;

    async fn from_request(req: &'r Request<'_>)
            -> Outcome<Self, Self::Error> {

        /// Returns true if `key` is a valid API key string.
        fn is_valid(key: &str) -> bool {
            key == "valid_api_key"
        }
```

```rust
        match req.headers().get_one("x-api-key") {
            None => Outcome::Error(
                (Status::BadRequest, ApiKeyError::Missing)),
            Some(key) if is_valid(key) => Outcome::Success(
                ApiKey(key)),
            Some(_) => Outcome::Error(
                (Status::BadRequest, ApiKeyError::Invalid)),
        }
    }
}
```


<aside class="notes">
</aside>
