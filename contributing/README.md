# Contributing

Under construction.

## Nexirift NPM Registry

**Applicable to:** [cosmos](https://github.com/Nexirift/cosmos), [nova](https://github.com/Nexirift/nova)

Our internal packages are not hosted on the public NPM registry, such as `@nexirift/db`. To use our internal projects, you can either use our private registry or set up a local NPM registry.

### Private Registry (Recommended, Pre-Built)
Our private registry is available at code.nexirift.com. For initial setup, run:

```bash
bun switch-registry
```

This creates the necessary configuration files and sets the private registry as default. Running the command again will switch between private and local registries.

### Local Registry (Alternative, Requires Building)
During our testing, we noticed that Next.js and shadcn/ui don't like Bun's linked packages. If you need a local registry:

0. Read the above section on switching registries
1. Install Verdaccio: `bun i -g verdaccio`
2. Start the Verdaccio server locally: `verdaccio`
3. Create an account: `bunx npm adduser --registry http://localhost:4873`
    - Example: `developer` | `P@ssw0rd` | `developer@nexirift.com`
4. Clone any `@nexirift/*` packages using Git
5. Run `bun publish` on the cloned repositories

*More information: https://verdaccio.org/docs/setup-bun*
