This repo contains code for reproducing linking errors when combining `mold` with Rust on Ubuntu 22.04
(and possibly other systems).

The config is in `.cargo/config.toml`, and is set to **work** by default. Comment out the other sections
to observe failures.

Run with:

```
cargo build --release
```

Or

```
RUSTFLAGS="-L /lib/x86_64-linux-gnu/" cargo build --release
```
