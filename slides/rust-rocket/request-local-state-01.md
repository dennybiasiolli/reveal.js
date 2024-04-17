#### Request-Local State

```rust
use rocket::request::{self, Request, FromRequest};

/// A global atomic counter for generating IDs.
static ID_COUNTER: AtomicUsize = AtomicUsize::new(0);

/// A type that represents a request's ID.
struct RequestId(pub usize);
```

```rust
#[get("/")]
fn id(id: &RequestId) -> String {
    format!("This is request #{}.", id.0)
}
```


<aside class="notes">
</aside>
