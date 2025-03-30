#### 🍪 Private cookies?

1. make sure the "secrets" feature is enabled

    ```toml
    ## in Cargo.toml
    rocket = { version = "0.5.1", features = ["secrets"] }
    ```

2. add "_private" to "add", "get" and "remove"

    ```rust
    cookies.get_private
    cookies.add_private
    cookies.remove_private
    ```

Encrypted using the 256-bit key specified in the secret_key configuration parameter.


<aside class="notes">
</aside>
