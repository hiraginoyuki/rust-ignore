# rust-ignore
A simple macro for syntax-highlighted comments.

## Installation
In `Cargo.toml`:
```toml
[dependencies]
ignore = { git = "https://github.com/hiraginoyuki/ignore" }
```

## Example
```rust
use ignore::ignore;

ignore!(arbitrary tokens here);

ignore! {
    check these out:
        "https://docs.rs/tracing",
        "https://docs.rs/tracing-subscriber",

    fn main() {
        tracing_subscriber::fmt().init();
        tracing::info!(argv_0 = %std::env::args().next().unwrap(), "hello");
    }
}
```
