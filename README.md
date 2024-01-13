A simple Hello, World! for [Axum](https://github.com/tokio-rs/axum) in [Rust](https://github.com/rust-lang/rust).

## Quick start

1. Run `cargo run`

2. Go to [127.0.0.1:3000](http://127.0.0.1:3000)

## Instructions

### 1. Axum

Add Axum to your project with the command:
```
cargo add axum
```

### 2. Tokio

[tokio](https://github.com/tokio-rs/tokio) is a library to deal with async in rust.

You'll need to to run this program. Tokio needs full access Add it with the command.
```
cargo add tokio --features=full
```

## Troubleshooting

> The default runtime flavor is `multi_thread`, but the `rt-multi-thread` feature is disabled.rustcClick for full compiler diagnostic

This error means doesn't have the `full` feature.

In your `Cargo.toml` file, change the dependecy from 
```
tokio = "x.x.x"
```

to

```
tokio = { version = "x.x.x", features = ["full"] }
```

## Useful links

- [rust](https://www.rust-lang.org/)
- [axum](https://docs.rs/axum/latest/axum/)
- [tokio](https://docs.rs/tokio/latest/tokio/)
