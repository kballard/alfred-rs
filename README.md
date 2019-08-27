# alfred-rs

[![Build Status](https://travis-ci.org/lilyball/alfred-rs.svg?branch=master)](https://travis-ci.org/lilyball/alfred-rs)
[![crates.io/crates/alfred](http://meritbadge.herokuapp.com/alfred)](https://crates.io/crates/alfred)

Rust library to help with creating [Alfred][alfred] [Workflows][].

[alfred]: http://www.alfredapp.com
[Workflows]: http://support.alfredapp.com/workflows

[API Documentation](http://docs.rs/alfred)

## Installation

Add the following to your `Cargo.toml` file:

```toml
[dependencies]

alfred = "4.0"
```

## License

Licensed under either of
 * Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or
   http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or
   http://opensource.org/licenses/MIT) at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you shall be dual licensed as above, without any
additional terms or conditions.

## Version History

#### 4.0.1

* Make `Builder.into_json` public.
* Make `Item.to_json` public, along with `to_json` methods on its helper types.

#### 4.0.0

* Add support for per-modifier icons.
* Add support for outputting workflow variables.
* Add support for outputting per-item workflow variables.
* Add support for outputting per-modifier workflow variables.
* Derive a few more traits on the types provided by this crate.

#### 3.0.3

Add 2 more functions for reading workflow environment variables.

#### 3.0.2

Update documentation links for crates.io.

#### 3.0.1

Update `serde_json` to 1.0.

#### 3.0

Switch from `rustc-serialize` to `serde_json` for our JSON support.

#### 2.0.1

Add new module `alfred::env` for accessing the Alfred workflow environment
variables.

#### 2.0.0

Moved XML output into its own module `alfred::xml` and introduced a new module
`alfred::json` for the new Alfred 3 JSON format.

Updated `Item` and `ItemBuilder` with the extended modifier functionality and
support for the QuickLook URL.

#### 1.0.1

Dual-licensed under MIT and APACHE.

#### 1.0.0

Rust 1.0 is out!

#### 0.3.1

Remove `#[unsafe_destructor]`, which no longer exists in the latest nightlies.

#### 0.3.0

Switch from `IntoCow<'a, str>` to `Into<Cow<'a, str>>`.
This is technically a breaking change, but it is unlikely to affect anyone.

#### 0.2.2

Compatibility with the latest Rust nightly.

#### 0.2.1

Compatibility with the latest Rust nightly.

#### 0.2

Switch from `std::old_io` to `std::io`.

#### 0.1.1

Compatibility with the Rust nightly for 2015-02-21.

#### 0.1

Compatibility with the Rust 1.0 Alpha release.
