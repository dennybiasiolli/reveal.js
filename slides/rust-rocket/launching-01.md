#### Launching

Standard format

```rust
#[launch]
fn rocket() -> _ {
    rocket::build()
        .mount("/hello", routes![world])
}
```


<aside class="notes">
</aside>
