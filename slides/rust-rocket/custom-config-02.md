#### `Rocket.toml` file

```toml
## defaults for all profiles
[default]
port = 8000
```

```toml
## set only when compiled in debug mode,
## i.e, `cargo build` or `cargo run`
[debug]
port = 8001
```

<small>

https://rocket.rs/guide/v0.5/configuration/

</small>


<aside class="notes">
</aside>
