#### Form input

```rust
use rocket::form::Form;

#[derive(FromForm)]
struct Task<'r> {
    description: &'r str,
    complete: bool
}

#[post("/todo", data = "<task>")]
fn new(task: Form<Task<'_>>) { /* .. */ }
```


<aside class="notes">
</aside>
