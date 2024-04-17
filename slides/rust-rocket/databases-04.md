#### Databases

```rust
#[get("/<id>")]
async fn read(mut db: Connection<Logs>, id: i64)
        -> Option<String> {
    sqlx::query("SELECT content FROM logs WHERE id = ?")
        .bind(id)
        .fetch_one(&mut **db).await
        .and_then(|r| Ok(r.try_get(0)?))
        .ok()
}
```


<aside class="notes">
</aside>
