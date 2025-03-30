#### JSON input? Yes, please!

Make sure the "json" feature is enabled

```toml
## in Cargo.toml
rocket = { version = "0.5.1", features = ["json"] }
```

The Json&lt;T&gt; guard deserializes body data as JSON. The only condition is that the generic type T implements the Deserialize trait from serde.

<small>

https://rocket.rs/guide/v0.5/requests/#json

</small>


<aside class="notes">
</aside>
