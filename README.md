# zentinel-agent-soap

SOAP/XML security agent for Zentinel reverse proxy - XML validation, WSDL enforcement, and XXE protection.

## Installation

`zentinel-agent-soap` is not published on crates.io, so `cargo install
zentinel-agent-soap` does not work. Install from the repository, or use a
prebuilt binary.

```bash
cargo install --git https://github.com/zentinelproxy/zentinel-agent-soap
```

This builds and installs the `zentinel-soap-agent` binary.

### Prebuilt Binaries

Each [release](https://github.com/zentinelproxy/zentinel-agent-soap/releases)
ships binaries for `linux-x86_64`, `linux-aarch64`, and `darwin-aarch64`:

```bash
VERSION=0.4.0
PLATFORM=linux-x86_64   # or linux-aarch64, darwin-aarch64
curl -fsSL -o zentinel-soap-agent.tar.gz \
  "https://github.com/zentinelproxy/zentinel-agent-soap/releases/download/v${VERSION}/zentinel-soap-agent-${VERSION}-${PLATFORM}.tar.gz"
tar -xzf zentinel-soap-agent.tar.gz
sudo install -m 0755 zentinel-soap-agent /usr/local/bin/
```

## Documentation

See [docs.zentinelproxy.io/agents/soap](https://docs.zentinelproxy.io/agents/soap)

## License

Apache-2.0
