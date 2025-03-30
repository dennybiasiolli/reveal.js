#### Multiple Segments

```rust
use std::path::{Path, PathBuf};
use rocket::fs::NamedFile;

#[get("/<file..>")]
async fn files(file: PathBuf) -> Option<NamedFile> {
    NamedFile::open(Path::new("static/").join(file))
        .await
        .ok()
}
```

Any type, as long as the type implements the `FromSegments` trait.<br>
A segments guard must be the final component of a path.

<aside class="notes">
</aside>
