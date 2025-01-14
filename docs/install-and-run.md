---
comments: true
---

## Software prerequisites

- [Rust installation](https://www.rust-lang.org/tools/install) minimum version 1.77.

## Install the client

We currently recommend installing and running the client with the [`testing`](#testing-feature) and [`concurrent`](#concurrent-feature) features.

Run the following command to install the miden-client:

```sh
cargo install miden-client --features testing,concurrent
```

This installs the `miden-client` binary (at `~/.cargo/bin/miden-client`) with the [`testing`](#testing-feature) and [`concurrent`](#concurrent-feature) features.

### `Testing` feature

The `testing` feature speeds up account creation. 

!!! warning "Install the `testing` feature on node and client"
    - When using the the client CLI alongside a locally-running node, make sure to install/execute the node with the `testing` feature. 
    - Some validations can fail if the flag does not match on both the client and the node.

### `Concurrent` feature

The `concurrent` flag enables optimizations that result in faster transaction execution and proving times.

## Run the client 

1. Make sure you have already [installed the client](#install-the-client).

2. Run the client CLI using:

    ```sh
    miden-client
    ```
    