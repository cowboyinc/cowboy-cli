# cowboy-cli

Binary releases of `cowboy`, the Cowboy blockchain command-line tool —
wallets, actor deploy/execute, tokens, jobs, and project init against
the mesa public devnet or a local node.

This repository hosts release binaries only; it is the download source
for the Homebrew formula:

```bash
brew install cowboyinc/lasso/cowboy
```

Most people want [lasso](https://github.com/cowboyinc/lasso), the
interactive console, which installs this CLI automatically:

```bash
brew install cowboyinc/lasso/lasso
```

## Platforms

- macOS Apple Silicon (`cowboy-darwin-arm64`) — available now
- macOS Intel and Linux — planned (CI cross-builds)

## Quick start

```bash
cowboy init dev        # project + wallet + faucet request on mesa
cowboy --help
```
