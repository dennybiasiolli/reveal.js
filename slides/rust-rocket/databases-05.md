#### Databases

```rust
use rocket::serde::{Serialize, Deserialize, json::Json};
use rocket_db_pools::{Database, Connection};
use rocket_db_pools::diesel::{PgPool, prelude::*};

#[derive(Database)]
#[database("custom_name_postgres")]
struct Db(PgPool);
  ```

```rust
#[derive(Debug, Clone, Deserialize, Serialize, Queryable, Insertable)]
#[serde(crate = "rocket::serde")]
#[diesel(table_name = posts)]
struct Post {
    #[serde(skip_deserializing)]
    id: Option<i64>,
    title: String,
    text: String,
    #[serde(skip_deserializing)]
    published: bool,
}
```


<aside class="notes">
</aside>
