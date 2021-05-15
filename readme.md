# wh

A replacement for the `which` tool.

Wh finds files under your `$PATH` or any directory you specify.

## Features

-	expand glob patterns.
-	Cross platform.
-	Shipped with shell completions.
-	Fast.

## Installation

You will need a recent [rust](https://github.com/rust-lang/rust) setup and [cargo](https://github.com/rust-lang/cargo).

There're currently two ways to install `wh` on your system:

### 1- Install using git clone

```sh
git clone https://github.com/insomnimus/wh
cd wh
git checkout main
cargo install --path .
```

### 2- Using cargo install

```sh
cargo install --git https://github.com/insomnimus/wh --branch main
```

## Usage

After following any of the installation methods above, the `wh` binary will be under one of
-	`~/.cargo/bin`
-	`$CARGO_HOME/bin` (non-windows)
-	`$env:CARGO_HOME\bin` (windows)

So make sure it's under your `$PATH`.

Then just use it as you would the `which` tool:

`wh cargo`

`wh --all 'cargo-*'`

## Shell Completions

After building wh, the completions will be generated at the crate root, follow your shell's completion installation to install them.
