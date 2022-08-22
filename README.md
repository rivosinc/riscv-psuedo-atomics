# RISC-V Pseudo Atomics

This library implements the same structs as `core::sync::atomic`, except it
doesn't use any atomic operations. This library is primarily intended as a
drop-in replacement for `core::sync::atomic` for targets which don't support
atomic operations. It does suspend interrupts during execution of most
operations, but that can be turned off by enabling the `user-mode` feature.

## License
This project, like Rust, is primarily distributed under the terms of both the 
MIT license and the Apache License (Version 2.0). See
[LICENSE-APACHE](LICENSE-APACHE), [LICENSE-MIT](LICENSE-MIT), and
[COPYRIGHT](COPYRIGHT) for details.
