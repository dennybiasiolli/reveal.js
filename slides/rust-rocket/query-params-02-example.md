#### Query params

```rust
#[get("/tasks?<filter>")]
fn tasks(filter: &str) { /* .. */ }
```

or

```rust
use rocket::form::Form;

#[derive(FromForm)]
struct Task<'r> {
    description: &'r str,
    complete: bool
}

#[get("/tasks?<task>")]
fn tasks(task: Task<'_>) { /* .. */ }
// or
#[get("/tasks?<task..>")]
fn tasks(task: Task<'_>) { /* .. */ }
```


<aside class="notes">
</aside>
