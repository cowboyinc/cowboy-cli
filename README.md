# cowboy-cli

Binary releases of `cowboy`, the Cowboy blockchain command-line tool —
wallets, actor deploy/execute, tokens, jobs, and project init against
the mesa public devnet or a local node.

This repository hosts release binaries only; it is the download source
for the Homebrew formula:

```bash
brew install cowboyinc/tap/cowboy
```

Most people want [lasso](https://github.com/cowboyinc/lasso), the
interactive console, which installs this CLI automatically:

```bash
brew install cowboyinc/tap/lasso
```

## Platforms

Each release has one archive per platform, holding `cowboy`, the
`cowboy-dev-runner` local simulator and `lasso`, and a `SHA256SUMS` file
covering the archives:

- `cowboy-darwin-arm64.tar.xz` — macOS Apple Silicon
- `cowboy-darwin-x64.tar.xz` — macOS Intel
- `cowboy-linux-arm64.tar.xz` — Linux arm64
- `cowboy-linux-x64.tar.xz` — Linux x86_64

## Quick start

```bash
cowboy init dev        # project + wallet + faucet request on mesa
cowboy --help
```
