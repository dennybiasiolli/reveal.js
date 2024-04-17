#### Templates

```rust
use rocket_dyn_templates::Template;

#[get("/")]
fn index() -> Template {
    // let context = /* object-like value */;
    // Template::render("index", &context)
    // or
    Template::render("index", context! {
        foo: 123,
    })
}
```


<aside class="notes">
</aside>
