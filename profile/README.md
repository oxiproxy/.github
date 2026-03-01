# Oxiproxy

**A modern, high-performance chaos testing proxy written in Rust.**

Oxiproxy is a Rust rewrite of [Shopify's toxiproxy](https://github.com/Shopify/toxiproxy) — a TCP proxy that simulates network and system conditions for chaos and resiliency testing. By leveraging Rust's performance and memory safety guarantees, Oxiproxy aims to provide a faster, more reliable, and resource-efficient alternative.

## Why Oxiproxy?

- **High Performance** — Built with Rust's zero-cost abstractions and async I/O for minimal latency overhead
- **Memory Safe** — No data races, no segfaults — Rust's ownership model ensures correctness at compile time
- **Low Resource Footprint** — Lightweight binary with minimal memory usage, ideal for CI/CD pipelines and resource-constrained environments
- **API Compatible** — Drop-in replacement for toxiproxy, compatible with existing client libraries and workflows

## Get Involved

We welcome contributions of all kinds — code, documentation, bug reports, and feature requests.

- **Repository**: [oxiproxy/oxiproxy](https://github.com/oxiproxy/oxiproxy)
- **Issues**: Found a bug or have an idea? [Open an issue](https://github.com/oxiproxy/oxiproxy/issues)
- **Pull Requests**: Check out existing issues or propose your own improvements
