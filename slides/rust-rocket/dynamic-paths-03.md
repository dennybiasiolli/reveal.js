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


<aside class="notes">
</aside>
