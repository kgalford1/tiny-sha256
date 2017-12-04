# tiny-sha256

A minimal implementation of `SHA-256` in Rust.


## About

This implementation is based on the pseudocode on 
[wikipedia](https://en.wikipedia.org/wiki/SHA-2#Pseudocode) and 
prioritizes readability and simplicity over fancy optimizations.
I may otimize it somewhat in the future, but not at the expense
of increased complexity or decreased readability.

This crate is freestanding (`#[no_std]`) and has no dependencies,
so it should be just about as portable as it gets.  

A small set of tests against known-good hashes are included, but
the implementation has *not* been formally verified.  Check out
the check out the [Rust Crypto](https://github.com/RustCrypto/hashes)
project for a much more mature implementation.



