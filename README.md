# byteview

Learning Rust by rewriting coreutils, one tool at a time

Built for my own use; public in case it helps someone.

## Install

```bash
cargo build --release
```

## Usage

```bash
./target/release/byteview src/*.rs
cat README.md | ./target/release/byteview
```

## What it does

- Counts lines, words and bytes like wc
- Reads stdin or multiple files
- Parallel over files with std threads
- Zero dependencies outside std

## Project structure

```text
├── .github/
│   ├── workflows/
│   │   └── ci.yml
│   └── pull_request_template.md
├── docs/
│   ├── development.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── src/
│   └── main.rs
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
└── Cargo.toml
```

## Development

```bash
cargo build
cargo clippy -- -D warnings
```
