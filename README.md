# tiny-sha256

A minimal and freestanding implementation of `SHA-256` in pure Rust.


## About

This implementation is based on the pseudocode on 
[wikipedia](https://en.wikipedia.org/wiki/SHA-2#Pseudocode) and 
prioritizes readability and simplicity over fancy optimizations.
I may optimize it somewhat in the future, but not at the expense
of simplicity or readability.

This crate is freestanding (`#[no_std]`) and has no dependencies,
so it should be just about as portable as it gets.  If I add any
dependencies in the future, they will also be freestanding, and
I will keep them behind feature gates.

A small set of tests against known-good hashes are included, but
the implementation has *not* been formally verified.  Use at your
own risk.  I suggest taking a look at the  [Rust Crypto](https://github.com/RustCrypto/hashes)
project for a much more mature implementation which includes
various optimizations, as well as a number of useful traits that
are shared across a host of different hashers.

