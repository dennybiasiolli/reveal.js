#### 🍪 Private cookies?

1. make sure the "secrets" feature is enabled

    ```toml
    ## in Cargo.toml
    rocket = { version = "0.5.0", features = ["secrets"] }
    ```

2. use get_private, add_private, and remove_private

    ```rust
    cookies.get_private("message")
    cookies.add_private(("message", message.to_string()));
    cookies.remove_private("message");
    ```

Private cookies are encrypted using the 256-bit key specified in the secret_key configuration parameter.


<aside class="notes">
</aside>
