![1739027188533](image/README/1739027188533.png)

# PNPM

Fast, disk space efficient package manager.

We have others like npm, yarn and bun.

Node.js comes with npm by default.

Why pnpm

* Saves disk space.
* Boosts installation speeds

## Installation

Using PowerShell:

```powershell
Invoke-WebRequest https://get.pnpm.io/install.ps1 -UseBasicParsing | Invoke-Expression
```

## Updating pnpm

To update pnpm, run the [`self-update`](https://pnpm.io/cli/self-update) command:

```text
pnpm self-update
```

# pnpm env `<cmd>`

Manages the Node.js environment.

Install the LTS version of Node.js:

```text
pnpm env use --global lts
```

Install Node.js v16:

```text
pnpm env use --global 16
```

### Add more node version

Installs the specified version(s) of Node.js without activating them as the current version.

Example:

```text
pnpm env add --global lts 20.0.1 23.7
```

### Setting a specific Version to be used

```
pnpm env use --global 23.7
```

## Commonly used PnPm Commands

Here are some commonly used `pnpm` commands for managing JavaScript projects:

### Installation & Setup:

1. **`pnpm install`**

   Installs dependencies defined in `package.json`.
2. **`pnpm install <package-name>`**

   Installs a specific package and adds it to `package.json`.
3. **`pnpm add <package-name>`**

   Installs and adds the package as a dependency in `package.json`.
4. **`pnpm add <package-name> --dev`** or **`pnpm add <package-name> -D`**

   Installs and adds the package as a development dependency.
5. **`pnpm add <package-name> --global`** or **`pnpm add <package-name> -g`**

   Installs the package globally.
6. **`pnpm install --frozen-lockfile`**

   Installs dependencies using the exact versions from `pnpm-lock.yaml`.

### Project Management:

7. **`pnpm update`**

   Updates dependencies based on the versions specified in `package.json`.
8. **`pnpm upgrade <package-name>`**

   Upgrades a specific package to its latest version.
9. **`pnpm remove <package-name>`**

   Removes a package from the project and updates `package.json`.
10. **`pnpm outdated`**

    Shows a list of outdated packages.
11. **`pnpm audit`**

    Runs a security audit of your project’s dependencies.

### Execution:

14. **`pnpm run <script-name>`**

    Runs a defined script in `package.json` (like `npm run <script-name>`).
15. **`pnpm start`**

    Runs the `start` script defined in `package.json`.
16. **`pnpm test`**

    Runs the `test` script defined in `package.json`.

### Cache Management:

17. **`pnpm store status`**

    Displays the status of the store (where pnpm keeps its cache).
18. **`pnpm store prune`**

    Removes unused packages from the pnpm store.
19. **`pnpm cache clean`**

    Clears the pnpm cache.

### Versioning:

20. **`pnpm version`**

    Displays the current version of `pnpm`.

These are just some of the frequently used commands in `pnpm`. There are many more options available for specific tasks and configurations.
