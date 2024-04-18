#### Databases

```rust
table! {
    posts (id) {
        id -> Nullable<BigInt>,
        title -> Text,
        text -> Text,
        published -> Bool,
    }
}
```

```rust
#[get("/<id>")]
async fn read(mut db: Connection<Db>, id: i64) -> Option<Json<Post>> {
    posts::table
        .filter(posts::id.eq(id))
        .first(&mut db)
        .await
        .map(Json)
        .ok()
}
```


<aside class="notes">
</aside>
