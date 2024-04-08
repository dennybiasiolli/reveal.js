#### 🍪 Cookies?

```rust
use rocket::form::Form;
use rocket::response::Redirect;
use rocket::http::CookieJar;

#[post("/", data = "<message>")]
fn submit(cookies: &CookieJar<'_>, message: Form<&str>) -> Redirect {
    cookies.add(("message", message.to_string()));
    Redirect::to(uri!(index))
}

#[get("/")]
fn index(cookies: &CookieJar<'_>) -> Option<String> {
    cookies.get("message")
        .map(|crumb| format!("Message: {}", crumb.value()))
}
```


<aside class="notes">
</aside>
