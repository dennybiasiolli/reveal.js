#### `Rocket.toml` file

```toml
## set only when the `custom-profile` profile is selected,
## i.e, `ROCKET_PROFILE=custom-profile cargo build --release`
[custom-profile]
port = 9001
```

```toml
## set only when compiled in release mode,
## i.e, `cargo build --release`
[release]
port = 9999
```

<small>

https://rocket.rs/guide/v0.5/configuration/

</small>


<aside class="notes">
</aside>
