#### Error Catchers

```rust
fn main() {
    rocket::build()
        .register("/", catchers![not_found]);
        .register("/foo", catchers![foo_not_found]);
}
```


<aside class="notes">
</aside>
