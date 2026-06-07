# homebrew-trusty

Homebrew tap for the [trusty-tools](https://github.com/bobmatnyc/trusty-tools) binary suite.

## Installation

```bash
brew tap bobmatnyc/trusty
```

Then install any of the available formulae:

```bash
brew install bobmatnyc/trusty/trusty-analyze
brew install bobmatnyc/trusty/trusty-review
brew install bobmatnyc/trusty/trusty-git-analytics
```

## Available Formulae

| Formula | Binary | Description |
|---|---|---|
| `trusty-analyze` | `trusty-analyze` | Code analysis daemon + MCP server |
| `trusty-review` | `trusty-review` | Inference-backed code review MCP server |
| `trusty-git-analytics` | `tga` | Developer productivity analytics |

## Usage

After installing, each binary is on your `PATH`:

```bash
trusty-analyze --help
trusty-review --help
tga --help
```

## Updating

Formulae are updated automatically on each tagged release of trusty-tools via the
`homebrew-bump` job in the repository's release workflow.

To update all installed trusty formulae:

```bash
brew update && brew upgrade
```

## Source

All binaries are built from [bobmatnyc/trusty-tools](https://github.com/bobmatnyc/trusty-tools).
Pre-built binaries are provided for:
- macOS arm64 (Apple Silicon)
- Linux x86_64 (glibc 2.17+)
