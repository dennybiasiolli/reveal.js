#### JSON input

```rust
use rocket::serde::{Deserialize, json::Json};

#[derive(Deserialize)]
#[serde(crate = "rocket::serde")]
struct Task<'r> {
    description: &'r str,
    complete: bool
}

#[post("/todo", data = "<task>")]
fn new(task: Json<Task<'_>>) { /* .. */ }
```


<aside class="notes">
</aside>
