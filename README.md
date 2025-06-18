# container-compose

A CLI to let you use the Apple [container](https://github.com/apple/container) like a `docker-compose`
config file.

> [!WARNING]
> This tool is on "alpha" mode, which means that you can find a lot of bugs or missing features.
> If you find anything, feel free to open an issue. Thank you! :)

## How to install

### Installing via Homebrew

```sh
brew tap noghartt/container-compose https://github.com/noghartt/container-compose.git
brew install noghartt/container-compose/container-compose
```

### Installing via cargo

```sh
cargo install container-compose
```

### Downloading binary

We have made a `.tar.gz` containing the binary available on the release page. 
If you prefer to have your binary from there.

### Running container-compose

To run `container-compose` from the source code, first ensure you have [Rust](https://www.rust-lang.org/tools/install) installed.

1. Clone the repository:
   ```sh
   git clone https://github.com/noghartt/container-compose.git
   cd container-compose
   ```

2. Build the project:
   ```sh
   cargo build --release
   ```

3. Run `container-compose` using Cargo:
   ```sh
   cargo run -- <command> [options]
   ```
   For example, to start services:
   ```sh
   cargo run -- up
   ```

You can also run the compiled binary directly:
```sh
./target/release/container-compose <command> [options]
```

Replace `<command>` and `[options]` with the desired subcommand and arguments.
