# OfficeCLI Distribution

This repository publishes public release assets for the closed-source `officecli` binary.

## Install

### macOS (Homebrew)

```bash
brew tap officecli/officecli
brew install officecli
```

To update later:

```bash
brew upgrade officecli
```

### Linux

```bash
curl -fsSL https://raw.githubusercontent.com/officecli/officecli-dist/main/scripts/install-officecli.sh | DIST_REPO=officecli/officecli-dist bash
```

By default, the installer downloads and installs the current stable release from this repository.

Re-running the same installer command refreshes the local binary to the current stable release.

If your shell still reports `officecli: command not found`, first try:

```bash
export PATH="$HOME/.local/bin:$PATH"
officecli --version
```

If that works, add `~/.local/bin` to your shell startup file so future shells can find the command.

## Manual Download

Download the current stable archives and `checksums.txt` from the latest release page of this repository.

## Notes

- This repository contains binaries, checksums, and install helpers only.
- It does not contain `officecli` source code.
