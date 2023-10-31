<!-- Allow this file to not have a first line heading -->
<!-- markdownlint-disable-file MD041 no-emphasis-as-heading -->

<!-- inline html -->
<!-- markdownlint-disable-file MD033 -->

<div align="center">

# `🪵️ tracing-logfmt-otel`

**Logfmt formatter for tracing-subscriber with opentelemetry support**

[![Embark](https://img.shields.io/badge/embark-open%20source-blueviolet.svg)](https://embark.dev)
[![Embark](https://img.shields.io/badge/discord-embark-%237289da.svg?logo=discord)](https://discord.gg/dAuKfZS)
[![Crates.io](https://img.shields.io/crates/v/tracing-logfmt.svg)](https://crates.io/crates/tracing-logfmt)
[![Docs](https://docs.rs/tracing-logfmt/badge.svg)](https://docs.rs/tracing-logfmt)
[![dependency status](https://deps.rs/repo/github/EmbarkStudios/tracing-logfmt/status.svg)](https://deps.rs/repo/github/EmbarkStudios/tracing-logfmt)
[![Build status](https://github.com/EmbarkStudios/tracing-logfmt/workflows/CI/badge.svg)](https://github.com/EmbarkStudios/tracing-logfmt/actions)
</div>

## Opentelemetry support

This crate is a fork of [EmbarkStudios/tracing-logfmt](https://github.com/EmbarkStudios/tracing-logfmt) that adds
the [opentelemetry](https://github.com/open-telemetry/opentelemetry-rust) trace and span id to the log output.

## Logfmt

Logfmt is a compact and simple log format for structured logging. Each log row contains one level of key/value pairs. To keep it as compact and readable as possible, values are only quoted if needed.

```logfmt
key=value otherkey="value with spaces" third="with escaped \"chars\""
```

There is no strict standard for the format, but it was first documented in [this article](https://brandur.org/logfmt) by Brandur Leach.

### License

This contribution is dual licensed under EITHER OF

* Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or <http://www.apache.org/licenses/LICENSE-2.0>)
* MIT license ([LICENSE-MIT](LICENSE-MIT) or <http://opensource.org/licenses/MIT>)

at your option.

For clarity, "your" refers to Embark or any other licensee/user of the contribution.
