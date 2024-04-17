#### Templates

```rust
use rocket_dyn_templates::Template;

#[launch]
fn rocket() -> _ {
    rocket::build()
        .mount("/", routes![/* .. */])
        .attach(Template::fairing()) // <- Add this line
}
```


<aside class="notes">
</aside>
