# cowboy-cli

Binary releases of `cowboy`, the Cowboy blockchain command-line tool:
wallets, the Store (find, hire and call ready-made actors), actor build and
deploy, tokens and jobs.

**Documentation: [docs.cowboy.inc](https://docs.cowboy.inc)** (for AI agents:
[docs.cowboy.inc/llms.txt](https://docs.cowboy.inc/llms.txt)).

## Install

Homebrew (macOS, or Linux with Homebrew):

```bash
brew install cowboyinc/tap/cowboy
```

Or download a release archive directly. Run `uname -m` first to pick the right
one on Linux:

```bash
curl -LO https://github.com/cowboyinc/cowboy-cli/releases/latest/download/cowboy-linux-arm64.tar.xz   # or cowboy-linux-x64 / cowboy-darwin-arm64
curl -LO https://github.com/cowboyinc/cowboy-cli/releases/latest/download/SHA256SUMS
sha256sum --ignore-missing -c SHA256SUMS
tar -xf cowboy-linux-arm64.tar.xz
sudo mv cowboy cowboy-dev-runner lasso /usr/local/bin/
```

Full instructions: [Install the CLI](https://docs.cowboy.inc/getting-started/install).

## Platforms

Each release has one archive per platform, holding `cowboy`, the
`cowboy-dev-runner` local simulator and `lasso` (the interactive console), and a
`SHA256SUMS` file covering the archives:

- `cowboy-darwin-arm64.tar.xz` — macOS Apple Silicon (Intel Macs are not supported)
- `cowboy-linux-arm64.tar.xz` — Linux arm64
- `cowboy-linux-x64.tar.xz` — Linux x86_64

## Quick start

Cowboy Cloud (`--env cloud`) is the network open to the public internet. A new
wallet gets a one-time credit that a human claims in a browser with a Google
sign-in:

```bash
export COWBOY_ENV=cloud
cowboy wallet create
cowboy credit claim          # open the printed page, sign in, then:
cowboy wallet balance
```

Then hire something from the Store with
[Hire from the Store](https://docs.cowboy.inc/getting-started/hire-from-the-store),
or build your own actor with the
[Quickstart](https://docs.cowboy.inc/getting-started/quickstart).
`cowboy --help` and `cowboy <command> --help` describe every command.
