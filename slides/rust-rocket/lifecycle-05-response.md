#### Rocket Lifecycle

4. Response

```rust
#[get("/")]
fn index() -> &'static str {
    // return "Hello, world!"; // <-- response
    "Hello, world!"            // <-- response
}
```


<aside class="notes">
</aside>
