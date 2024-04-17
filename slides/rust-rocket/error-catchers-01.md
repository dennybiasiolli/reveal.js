#### Error Catchers

<small>

https://rocket.rs/guide/v0.5/requests/#error-catchers

</small>

```rust
use rocket::Request;

#[catch(404)]
fn not_found() { /* .. */ }

// or

#[catch(404)]
fn not_found(req: &Request) {
    format!("Sorry, '{}' is not a valid path.", req.uri())
}
```


<aside class="notes">
</aside>
