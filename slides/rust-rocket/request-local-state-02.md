#### Request-Local State

```rust
/// Returns the current request's ID,
/// assigning one only as necessary.
#[rocket::async_trait]
impl<'r> FromRequest<'r> for &'r RequestId {
    type Error = ();

    async fn from_request(request: &'r Request<'_>)
        -> request::Outcome<Self, Self::Error> {
        // The closure passed to `local_cache`
        // will be executed at most once per request:
        // When requested again, will return the same value.
        request::Outcome::Success(request.local_cache(|| {
            RequestId(ID_COUNTER.fetch_add(1, Ordering::Relaxed))
        }))
    }
}
```


<aside class="notes">
</aside>
