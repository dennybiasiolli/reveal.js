#### Rocket Lifecycle

1. Routing

```rust
#[get("/world")]             // <- route attribute
fn world() -> &'static str { // <- request handler
    "Hello, world!"
}

#[launch]
fn rocket() -> _ {
    rocket::build()
        .mount("/hello", routes![world]) // <- route mounting
        .mount("/hi", routes![world]);   // <- route mounting
}
```

<small>

Requests to "/hello/world" and "/hi/world" will be directed to the world function.

</small>


<aside class="notes">
</aside>
