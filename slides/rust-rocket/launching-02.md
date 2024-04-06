#### Launching

```rust
#[rocket::main]
async fn main() -> Result<(), rocket::Error> {
    let _rocket = rocket::build()
        .mount("/hello", routes![world])
        .launch()
        .await?;

    Ok(())
}
```

<small>

- allows _you_ to start the server
- is useful when a handle to the Future returned by launch() is desired
- or when the return value of launch() is to be inspected.

</small>


<aside class="notes">
</aside>
