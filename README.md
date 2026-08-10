# Coalesce Quality Homebrew tap

Homebrew casks for the Coalesce Quality command-line tools.

```bash
brew tap getsynq/tap
brew install synqcli
brew install synq-recon
brew install synq-scout
```

Or without tapping first:

```bash
brew install getsynq/tap/synqcli
```

Upgrade with `brew upgrade`, and `brew upgrade getsynq/tap/synqcli` for one tool on
its own.

| Cask | What it does | Reference |
|---|---|---|
| `synqcli` | Declares monitors, SQL tests and deployment rules as code | [docs.synq.io/monitors/cli](https://docs.synq.io/monitors/cli) |
| `synq-recon` | Compares a dataset in one database against another, without moving row data | [docs.synq.io/reconciliation/cli](https://docs.synq.io/reconciliation/cli) |
| `synq-scout` | Runs the Scout agent, or serves its tools locally over MCP | [docs.synq.io/scout/cli](https://docs.synq.io/scout/cli) |

All three share one credential store, so a single `auth login` covers them.

## macOS only

Homebrew casks serve macOS. On Linux, install from the release archives — see
[docs.synq.io/cli](https://docs.synq.io/cli), which also covers the container
images and the credential setup.

## The casks are generated

Each cask here is written by the release pipeline that publishes the
corresponding archive, so it always matches a real release. Do not edit one by
hand: the next release overwrites it.
