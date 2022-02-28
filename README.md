# rust-wasm-cli

A WebAssembly executor that runs arbitrary [waPC](https://wapc.io/)-compliant modules on the command line.

### Usage

```USAGE:
./wapc-runner <file-path> <operation> <json-path>

FLAGS:
    -h, --help       Prints help information
    -V, --version    Prints version information

ARGS:
    <file-path>    The WebAssembly file to load
    <operation>    The operation to invoke in the WASM file
    <json-path>    The path to the JSON data to use as input
```

### Example

```
./wapc-runner ./crates/my-lib/tests/test.wasm hello hello.json

"Hello, there."
```

### Credits

Project completed as part of the [From Node to Rust](https://vino.dev/blog/node-to-rust-day-1-rustup/) series