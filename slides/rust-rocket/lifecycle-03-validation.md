#### Rocket Lifecycle

2. Validation

```rust
#[get("/hello/<name>/<age>")]
fn hello(name: &str, age: u8) -> String { // <-- validation
    format!("Hello, {} year old named {}!", age, name)
}
```

<small>
The `name` and `age` parameters are validated by Rocket.<br>
If the request does not match the expected types,<br>
Rocket will return a 404 Not Found error.

The `u8` type for `age` ensures that only valid unsigned 8-bit integers are accepted.<br>
If a non-integer or an integer outside the range of 0-255 is provided,<br>
Rocket will return a 422 Unprocessable Entity error.
</small>


<aside class="notes">
</aside>
