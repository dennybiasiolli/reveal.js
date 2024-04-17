#### Managed (global) State

The state is managed on a per-type basis

1. Call manage on the Rocket instance corresponding to your application with the initial value of the state.

    ```rust
    use std::sync::atomic::AtomicUsize;

    struct HitCount {
        count: AtomicUsize
    }

    rocket::build()
        .manage(HitCount { count: AtomicUsize::new(0) });
    ```


<aside class="notes">
</aside>
