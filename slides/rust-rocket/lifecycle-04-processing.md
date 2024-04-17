#### Rocket Lifecycle

3. Processing

```rust
#[get("/hello/<name>")]
fn hello(name: &str, age: u8) -> String {
    /**
     * Processing
     * i.e, checking the age range, etc.
     * This is the main business logic of an application.
     * Processing completes by returning a Response.
     */
    format!("Hello, {} year old named {}!", age, name)
}
```


<aside class="notes">
</aside>
