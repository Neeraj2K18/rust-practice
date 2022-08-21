<a href="https://github.com/Neeraj2K18/rust-practice/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/Neeraj2K18/rust-practice"></a>
<a href="https://github.com/Neeraj2K18/rust-practice/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/Neeraj2K18/rust-practice"></a>
<a href="https://github.com/Neeraj2K18/rust-practice/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/Neeraj2K18/rust-practice"></a>
[![Rust](https://github.com/Neeraj2K18/rust-practice/actions/workflows/rust.yml/badge.svg?branch=main)](https://github.com/Neeraj2K18/rust-practice/actions/workflows/rust.yml)
[![pages-build-deployment](https://github.com/Neeraj2K18/rust-practice/actions/workflows/pages/pages-build-deployment/badge.svg?branch=main)](https://github.com/Neeraj2K18/rust-practice/actions/workflows/pages/pages-build-deployment)

[![cargo-docs](https://img.shields.io/badge/cargo--docs-deployed-yellow.svg?branch=main)](https://neeraj2k18.github.io/rust-practice/docs/doxygen-html/doc/rust_practice/index.html)
[![code-coverage](https://neeraj2k18.github.io/rust-practice/docs/gcov-html/badges/plastic.svg?branch=main)](https://neeraj2k18.github.io/rust-practice/docs/gcov-html/index.html)
---
# rust-practice

Rust Programming Tutorials [rust-lang official website](https://www.rust-lang.org/)

References:
  1. [Rust Language documentation](http://rust-lang.github.io/rustup/index.html)
  2. [Rust Language cheat sheet](https://cheats.rs/)
  3. [The Cargo Book](https://doc.rust-lang.org/cargo/)

<details>
  <summary>Windows</summary>

  ### Installation
Download and install `rustup_init.exe` [Installer](https://win.rustup.rs/x86_64) <br>
Pre-requisite [Build Tools for Visual Studio 2022](https://visualstudio.microsoft.com/downloads/?q=build+tools)

VS Code Extn: <br>
[Rust](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust) <br>
[rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer)
</details>

<details>
  <summary>Linux</summary>

### Installation
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
</details>

### Rust/Cargo commands
Cargo is rust package manager, which is used to build, run, test, document and install rust applications.
```bash
rustc --version             # Get rust compiler version
rustup update               # Update rust compiler
cargo --version             # Get cargo package manager version
cargo init <project_name>   # Init sample project
cargo new <project_name>    # New cargo Project
cargo build --release       # Build release (optimized)
cargo run                   # Execute rust application or program
cargo test                  # For unit testing
cargo doc --target-dir=docs/doxygen-html
```
For more information on cargo refer [the cargo book](https://doc.rust-lang.org/cargo/) and [crates.io](https://crates.io/)
### Rust Code Formatting
You can use `format document` of vscode or `rustfmt`
```bash
# add rust components
rustup component add rustfmt rls rust-analysis rust-src cippy llvm-tools-preview
cargo install grcov                                           # grcov code coverage
cargo fix                                                     # cargo fix the project
cargo fmt                                                     # cargo format the project
```

### Folder structure
    .
    ├── Cargo.lock
    ├── Cargo.toml      # .toml file used for rust-dependencies/crates
    ├── LICENSE
    ├── README.md
    ├── src             # source files directory
    └── target          # target files generated by cargo
            
Use short lowercase names at least for the top-level files and folders except `LICENSE`, `README.md`

##### Tree view
```bash
tree -L 1
```
