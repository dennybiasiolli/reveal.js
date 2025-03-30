#### Serving static files

The easy way

```rust
use rocket::fs::FileServer;
// use rocket::fs::{relative, FileServer};

#[launch]
fn rocket() -> _ {
    rocket::build()
         // serve files from `/www/static` at path `/public`
        .mount("/public", FileServer::from("/www/static"))
        // or `relative!("static")` for a local directory
}
```


<aside class="notes">
</aside>
