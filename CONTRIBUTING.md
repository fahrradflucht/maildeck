# Contributing to maildeck

## Development setup

This project uses [`rye`](https://rye-up.com/) to manage the development
environment and tools (formatter, linter, etc.).

- Install Rye (see the Rye website for your platform)
- Sync dev dependencies: `rye sync`
- Optional: enter the env: `rye shell`
- Run tests: `rye run test`

### Linting and formatting (Ruff)

We use Ruff for both formatting and linting. Useful commands:

- Format: `rye run format` (runs `ruff format .`)
- Lint: `rye run lint` (runs `ruff check .`)
- Auto-fix lint issues: `rye run lint --fix`

### Pre-commit hooks (optional)

You can enable pre-commit hooks locally:

- Install hooks: `rye run pre-commit install`
- Run on all files: `rye run pre-commit run --all-files`

Using pre-commit is optional; running the Ruff commands above is sufficient
before sending a PR.

### Building and publishing

To build and publish the package, run:

```bash
rye build --clean
rye publish
```
