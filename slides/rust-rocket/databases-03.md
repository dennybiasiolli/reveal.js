#### Databases

```rust
#[macro_use] extern crate rocket;

use rocket_db_pools::{Database, Connection};
use rocket_db_pools::sqlx::{self, Row};

#[derive(Database)]
#[database("custom_name")]
struct Logs(sqlx::SqlitePool); // or sqlx::PgPool

#[launch]
fn rocket() -> _ {
    rocket::build()
        .attach(Logs::init())
        .mount("/", routes![read])
}
```


<aside class="notes">
</aside>
