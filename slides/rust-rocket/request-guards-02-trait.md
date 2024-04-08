#### Request Guards

`FromRequest` trait implementation

```rust
use rocket::request::{self, Request, FromRequest};

#[rocket::async_trait]
impl<'r> FromRequest<'r> for MyType {
    type Error = MyError;

    async fn from_request(req: &'r Request<'_>)
        -> request::Outcome<Self, Self::Error> {
        /* .. */
    }
}
```


<aside class="notes">
</aside>
