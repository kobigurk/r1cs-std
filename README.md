<h1 align="center">ark-r1cs-std</h1>

<p align="center">
    <img src="https://github.com/arkworks-rs/r1cs-std/workflows/CI/badge.svg?branch=master">
    <a href="https://github.com/arkworks-rs/r1cs-std/blob/master/LICENSE-APACHE"><img src="https://img.shields.io/badge/license-APACHE-blue.svg"></a>
    <a href="https://github.com/arkworks-rs/r1cs-std/blob/master/LICENSE-MIT"><img src="https://img.shields.io/badge/license-MIT-blue.svg"></a>
    <a href="https://deps.rs/repo/github/arkworks-rs/r1cs-std"><img src="https://deps.rs/repo/github/arkworks-rs/r1cs-std/status.svg"></a>
</p>

The arkworks ecosystem consist of Rust libraries for designing and working with __zero knowledge succinct non-interactive arguments (zkSNARKs)__. This repository contains efficient implementations of constraint "gadgets" that enable checking common computations inside SNARKs, such as bit operations, finite field arithmetic, elliptic curve arithmetic, and pairings.

This library is released under the MIT License and the Apache v2 License (see [License](#license)).

**WARNING:** This is an academic proof-of-concept prototype, and in particular has not received careful code review. This implementation is NOT ready for production use.

## Build guide

The library compiles on the `stable` toolchain of the Rust compiler. To install the latest version of Rust, first install `rustup` by following the instructions [here](https://rustup.rs/), or via your platform's package manager. Once `rustup` is installed, install the Rust toolchain by invoking:
```bash
rustup install stable
```

After that, use `cargo`, the standard Rust build tool, to build the library:
```bash
git clone https://github.com/arkworks-rs/r1cs-std.git
cargo build --release
```

This library comes with unit tests for each of the provided crates. Run the tests with:
```bash
cargo test
```

## License

This library is licensed under either of the following licenses, at your discretion.

 * Apache License Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

Unless you explicitly state otherwise, any contribution submitted for inclusion in this library by you shall be dual licensed as above (as defined in the Apache v2 License), without any additional terms or conditions.

## Acknowledgements

This work was supported by:
a Google Faculty Award;
the National Science Foundation;
the UC Berkeley Center for Long-Term Cybersecurity;
and donations from the Ethereum Foundation, the Interchain Foundation, and Qtum.

An earlier version of this library was developed as part of the paper *"[ZEXE: Enabling Decentralized Private Computation][zexe]"*.

[zexe]: https://ia.cr/2018/962