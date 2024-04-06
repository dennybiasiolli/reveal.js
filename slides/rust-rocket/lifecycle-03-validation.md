#### Rocket Lifecycle

2. Validation

```rust
#[get("/hello/<name>")]
fn hello(name: &str, age: u8) -> String { // <-- validation
    format!("Hello, {} year old named {}!", age, name)
}
```


<aside class="notes">
</aside>
