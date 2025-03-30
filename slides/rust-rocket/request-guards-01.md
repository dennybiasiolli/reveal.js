#### Request Guards

- Types that implement the `FromRequest` trait
- Used to extract data from the request
- Can be used as arguments in request handlers
    ```rust
    #[get("/<param>")]
    fn index(param: isize, a: A, b: B, c: C) { /* ... */ }
    // `A`, `B`, and `C` are request guards
    ```
- Protect a handler from being called erroneously

<small>

https://rocket.rs/guide/v0.5/requests/#request-guards

https://api.rocket.rs/v0.5/rocket/request/trait.FromRequest

</small>


<aside class="notes">
</aside>
