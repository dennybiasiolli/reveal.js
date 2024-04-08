#### Dynamic Paths

```rust
#[get("/hello/<name>")]
fn hello(name: &str) -> String {
    format!("Hello, {}!", name)
}
```


<aside class="notes">
</aside>
