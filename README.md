# dirdust

Small Go tool: declutter ~/Downloads in one command

Built for my own use; public in case it helps someone.

## Usage

```bash
./bin/dirdust ~/Downloads --dry-run
./bin/dirdust ~/Downloads
```

## Installation

```bash
go build -o bin/ ./...
```

## Features

- Dry-run prints the plan before moving anything
- Skips hidden files and folders by default
- Single static binary, no runtime deps
- Groups files into folders by extension

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
├── go.mod
└── main.go
```

## Development

```bash
go build ./...
go vet ./...
```

## Changelog

- `0.1.1` - fix edge case in argument parsing
- `0.1.0` - first working version

## License

MIT licensed, see LICENSE.
