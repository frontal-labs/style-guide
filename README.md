<img src="https://res.cloudinary.com/dun4i32pe/image/upload/v1761040261/b_1589x396_gu4we9.jpg" />

# Frontal Style-Guide

This repository is the home of Frontal's style guide, which includes configs for popular linting and styling tools.

The following configs are available, and are designed to be used together.

## Contributing

Please read our [contributing](./CONTRIBUTING.md)
guide before creating a pull request.

## Installation

All of our configs are contained in one package, `@frontal/style-guide`. To install:

```sh
# If you use npm
npm i --save-dev @frontal/style-guide

# If you use pnpm
pnpm i --save-dev @frontal/style-guide

# If you use Yarn
yarn add --dev @frontal/style-guide
```

## Biome

This style guide provides a shared Biome configuration for consistent code formatting and linting across the project. 

To use the shared Biome config, set the following in [`biome.jsonc`](./biome.jsonc):

```json
{
  "extends": ["@frontal/style-guide/biome"]
}
```

The Biome configuration includes:
- Code formatting rules
- Linting rules
- Import sorting
- And other best practices for consistent code style

## Development

### Building

```bash
pnpm build
```

### Type Checking

```bash
pnpm type-check
```

### Linting

```bash
pnpm lint
pnpm lint:fix
```

### Formatting

```bash
pnpm format
```

## License

This package is private and proprietary to Frontal Labs. See [LICENSE.md](./LICENSE.md) for details.

## Contributing

Please read [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines on contributing to this package.

### Development Workflow

1. **Fork and clone** the repository
2. **Install dependencies**: `pnpm install`
3. **Make changes** to configuration files
4. **Run tests**: `pnpm lint && pnpm type-check && pnpm build`
5. **Create a pull request** with a clear description

## Repository Structure

```
internals/style-guide/
├── biome.jsonc           # Biome configuration
├── package.json          # Package configuration
├── README.md             # This file
├── CONTRIBUTING.md       # Contributing guidelines
└── .gitignore           # Git ignore rules
```