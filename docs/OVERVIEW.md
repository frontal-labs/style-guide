# Style Guide Documentation

Welcome to the Frontal Style Guide documentation.

## Contents

- [Getting Started](./getting-started.md)
- [Configuration](./configuration.md)
- [Rules](./rules.md)

## Overview

This package provides shared configuration files for linting, formatting, and code quality across all Frontal projects.

## Supported Platforms

- **JavaScript/TypeScript**: Biome
- **Go**: golangci-lint
- **Python**: Ruff
- **Rust**: rustfmt

## Quick Start

```bash
bun add -D @frontal/style-guide
```

Then extend the configuration in your project's `biome.jsonc`:

```json
{
  "$schema": "https://biomejs.dev/schemas/2.3.4/schema.json",
  "extends": ["@frontal/style-guide/react.json"]
}
```
