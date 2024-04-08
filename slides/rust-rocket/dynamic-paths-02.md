#### Dynamic Paths

```rust
#[get("/hello/<name>/<age>/<cool>")]
fn hello(name: &str, age: u8, cool: bool) -> String {
    if cool {
        format!("You're a cool {} year old, {}!", age, name)
    } else {
        format!(
            "{}, we need to talk about your coolness.",
            name
        )
    }
}
```

Any type, as long as the type implements the `FromParam` trait.


<aside class="notes">
</aside>
