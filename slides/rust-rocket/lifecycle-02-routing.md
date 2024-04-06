#### Rocket Lifecycle

1. Routing

```rust
#[get("/bar")]                       // <-- route attribute
fn bar() -> &'static str {
    "This is the /foo/bar route!"
}

#[launch]
fn rocket() -> _ {
    rocket::build()
        .mount("/foo", routes![bar]) // <-- route mounting
}
```


<aside class="notes">
</aside>
