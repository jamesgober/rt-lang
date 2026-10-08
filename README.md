<h1 align="center">
    <img width="99" alt="Rust logo" src="https://raw.githubusercontent.com/jamesgober/rust-collection/72baabd71f00e14aa9184efcb16fa3deddda3a0a/assets/rust-logo.svg">
    <br>
    <b>rt-lang</b>
    <br>
    <sub><sup>LEXERSKETCH NATIVE RUNTIME</sup></sub>
</h1>

<div align="center">
    <a href="https://crates.io/crates/rt-lang"><img alt="Crates.io" src="https://img.shields.io/crates/v/rt-lang"></a>
    <a href="https://crates.io/crates/rt-lang"><img alt="Downloads" src="https://img.shields.io/crates/d/rt-lang?color=%230099ff"></a>
    <a href="https://docs.rs/rt-lang"><img alt="docs.rs" src="https://img.shields.io/docsrs/rt-lang"></a>
    <a href="https://github.com/jamesgober/rt-lang/actions"><img alt="CI" src="https://github.com/jamesgober/rt-lang/actions/workflows/ci.yml/badge.svg"></a>
    <a href="https://github.com/rust-lang/rfcs/blob/master/text/2495-min-rust-version.md"><img alt="MSRV" src="https://img.shields.io/badge/MSRV-1.85%2B-blue"></a>
</div>

<br>

<div align="left">
    <p>
        <strong>rt-lang</strong> is the runtime every natively compiled LexerSketch program links: program entry and exit, the allocator, strings, panics and unwinding, threads, and GC hooks. It is written in the toolchain's own IR and compiled by the toolchain's own backend, talking to the OS directly (syscalls on Linux, PE imports on Windows, libSystem on macOS), so no C runtime or C compiler is involved.
    </p>
    <br>
    <hr>
    <p>
        <strong>MSRV is 1.85+</strong> (Rust 2024 edition).
    </p>
    <blockquote>
        <strong>Status: pre-1.0, in active development.</strong> The public API is being designed across the 0.x series and frozen at <code>1.0.0</code>. See <a href="./CHANGELOG.md"><code>CHANGELOG.md</code></a>.
    </blockquote>
</div>

<hr>
<br>

## Installation

```toml
[dependencies]
rt-lang = "0.1"
```

<br>

## Status

This is the <code>v0.1.0</code> scaffold: structure, tooling, and quality gates are in place; the implementation lands across the 0.x series per the <a href="./dev/ROADMAP.md"><code>ROADMAP</code></a> and <a href="./docs/API.md"><code>docs/API.md</code></a>.

<hr>
<br>

## Contributing

See <a href="./dev/DIRECTIVES.md"><code>dev/DIRECTIVES.md</code></a> for engineering standards and the definition of done. Before a PR: `cargo fmt --all`, `cargo clippy --all-targets --all-features -- -D warnings`, and `cargo test --all-features` must be clean.

<br>

<div id="license">
    <h2>License</h2>
    <p>Licensed under either of</p>
    <ul>
        <li><b>Apache License, Version 2.0</b> &mdash; <a href="./LICENSE-APACHE">LICENSE-APACHE</a></li>
        <li><b>MIT License</b> &mdash; <a href="./LICENSE-MIT">LICENSE-MIT</a></li>
    </ul>
    <p>at your option.</p>
</div>

<div align="center">
  <h2></h2>
  <sup>COPYRIGHT <small>&copy;</small> 2026 <strong>James Gober.</strong></sup>
</div>
