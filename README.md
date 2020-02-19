![whoami](https://libcala.github.io/whoami/icon.svg)

[![docs.rs](https://docs.rs/whoami/badge.svg)](https://docs.rs/whoami)
[![build status](https://api.travis-ci.com/libcala/whoami.svg?branch=master)](https://travis-ci.com/libcala/whoami)
[![crates.io](https://img.shields.io/crates/v/whoami.svg)](https://crates.io/crates/whoami)
[![discord](https://img.shields.io/badge/discord-Cala%20Project-green.svg)](https://discord.gg/nXwF59K)

[About](https://libcala.github.io/whoami) |
[Source](https://github.com/libcala/whoami) |
[Changelog](https://libcala.github.io/whoami/changelog)

# WhoAmI
Retrieve the current user and environment.

## Getting Started
Using the whoami crate is super easy!  All of the exported items are simple
functions with no parameters that return either a `String` or enum.  The
following example shows how to use all of the functions:

```rust
fn main() {
    print!(
        "--------------------------------------------------------------------------------\n\
         user's full name (user):              {}\n\
         username (username):                  {}\n\
         --------------------------------------------------------------------------------\n\
         host's fancy name (host):             {}\n\
         hostname (hostname):                  {}\n\
         --------------------------------------------------------------------------------\n\
         platform (platform):                  {}\n\
         operating system (os):                {}\n\
         desktop environment (env):            {}\n\
         --------------------------------------------------------------------------------\n\
         ",
        whoami::user(),
        whoami::username(),
        whoami::host(),
        whoami::hostname(),
        whoami::platform(),
        whoami::os(),
        whoami::env(),
    );
}
```

You can also preview similar output with the `whoami-demo` binary.

## Features
* Get the user's full name
* Get the user's username
* Get the computer's hostname
* Get the computer's fancy name
* Get the computer's desktop environment
* Get the computer's OS name and version
* Get the computer's platform name
* Works on Linux, Windows, Mac OS, and Web Assembly

## Binary
[whome](https://crates.io/crates/whome): replacement of the `whoami` command that depends on this crate.

## TODO
* Support iOS / Android / Nintendo Switch (and other consoles) / other OS's.

# Contributing
Contributors are always welcome!  Whether it is a bug report, bug fix, feature
request, feature implementation or whatever.  Don't be shy about getting
involved.  I always make time to fix bugs, so usually a patched version of the
library will be out soon after a report.  Features take me longer, though.  I'll
also always listen to any design critiques you have.  If you have any questions
you can email me at jeronlau@plopgrizzly.com.  Otherwise, here's a link to the
[issues on GitHub](https://github.com/libcala/whoami/issues).

And, as always, make sure to always follow the
[code of conduct](https://github.com/libcala/whoami/blob/master/CODEOFCONDUCT.md).
Happy coding!

# License
This repository is licensed under either of the following:

- MIT License (MIT) - See accompanying file
  [LICENSE_MIT.txt](https://github.com/libcala/whoami/blob/master/LICENSE_MIT.txt)
  or copy at https://opensource.org/licenses/MIT
- Boost Software License (BSL-1.0) - See accompanying file
  [LICENSE_BSL.txt](https://github.com/libcala/whoami/blob/master/LICENSE_BSL.txt)
  or copy at https://www.boost.org/LICENSE_1_0.txt

at your option.

## Contribution Licensing
Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you shall be dual licensed as above without any
additional terms or conditions.
