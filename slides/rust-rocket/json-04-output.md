#### JSON output

```rust
use rocket::serde::{Deserialize, Serialize, json::Json};

#[derive(Deserialize, Serialize)]
#[serde(crate = "rocket::serde")]
struct Task<'r> {
    description: &'r str,
    complete: bool
}
```

```rust
#[post("/todo", data = "<task>")]
fn new(task: Json<Task<'_>>) -> Json<Task<'_>> {
    task
}
```


<aside class="notes">
</aside>
