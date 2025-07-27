# Contributing

All contributors must adhere to our [Code of Conduct](https://github.com/Nexirift/.github/blob/main/contributing/CODE_OF_CONDUCT.md).

## Commit Message Guidelines

We follow the [Conventional Commits specification](https://www.conventionalcommits.org/en/v1.0.0) to maintain a clean and consistent commit history. Examples:
- `feat(ui): add new button component`
- `fix(api): resolve authentication timeout issue`
- `docs: update installation instructions`

## Versioning

As of July 27, 2025, all Nexirift projects must follow [Semantic Versioning 2.0.0](https://semver.org/). This means:
- MAJOR version for incompatible API changes
- MINOR version for backwards-compatible functionality additions
- PATCH version for backwards-compatible bug fixes

## Nexirift NPM Registry

**Applicable to:** [cosmos](https://github.com/Nexirift/cosmos), [nova](https://github.com/Nexirift/nova)

Our internal packages (like `@nexirift/db`) are hosted on our private registry rather than the public NPM registry. You have two options for accessing these packages:

### Private Registry (Recommended)
Our private registry at code.nexirift.com offers the most reliable experience:

```bash
pnpm switch-registry
```

This command configures your environment and sets our private registry as default. Running it again toggles between private and local registry settings.

### Local Registry (Advanced Setup)
If you need a local development environment:

1. First review the registry switching instructions above
2. Install Verdaccio: `pnpm add -g verdaccio`
3. Start the local Verdaccio server: `verdaccio`
4. Create a user account: `npm adduser --registry http://localhost:4873`
   - Example credentials: username: `developer`, password: `P@ssw0rd`, email: `developer@nexirift.com`
5. Clone any required `@nexirift/*` packages using Git
6. Publish them locally with `pnpm publish`

#### Important Notice

We are in the process of migrating from Bun to pnpm across all Nexirift projects due to constant issues with Bun. **pnpm is now our officially supported package manager** as it delivers consistent performance and reliable dependency management. All commands in this guide assume the use of pnpm.
