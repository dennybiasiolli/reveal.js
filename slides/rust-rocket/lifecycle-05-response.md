#### Rocket Lifecycle

4. Response

```rust
#[get("/")]
fn index() -> &'static str {
    // return "Hello, world!"; // <-- response (verbose)
    "Hello, world!"            // <-- response (sugary)
}
```


<aside class="notes">
</aside>
