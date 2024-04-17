#### Managed (global) State

2. Add a `&State<T>` type to any request handler,<br>where T is the type of the value passed into manage.

    ```rust
    use rocket::State;

    #[get("/count")]
    fn count(hit_count: &State<HitCount>) -> String {
        let current_count = hit_count.count.load(Ordering::Relaxed);
        format!("Number of visits: {}", current_count)
    }
    ```


<aside class="notes">
</aside>
