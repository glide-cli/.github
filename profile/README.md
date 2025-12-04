# Glide CLI

**Context-aware command orchestration for modern development workflows.**

Glide automatically detects your project type and provides unified commands across different tools, frameworks, and environments. Stop memorizing different CLI syntaxes—just `glide test`, `glide build`, or `glide dev` and let Glide figure out the rest.

## What is Glide?

Glide is a command orchestrator that:

- **Detects your stack** — Go, Node.js, PHP, Docker, and more
- **Adapts commands** — Same command, different underlying tools based on context
- **Extends via plugins** — gRPC-based plugin system for custom integrations
- **Configures per-project** — `.glide.yml` for project-specific commands and aliases

## Quick Example

```bash
# In a Node.js project with yarn
$ glide test
→ yarn test

# In a Go project
$ glide test
→ go test ./...

# In a Laravel project
$ glide test
→ php artisan test
```

## Repositories

| Repository | Description |
|------------|-------------|
| [glide](https://github.com/glide-cli/glide) | Core CLI tool |
| [registry](https://github.com/glide-cli/registry) | Plugin registry and metadata |
| [glide-plugin-docker](https://github.com/glide-cli/glide-plugin-docker) | Docker & Compose plugin |

## Getting Started

```bash
# Install Glide (coming soon to Homebrew)
go install github.com/glide-cli/glide/v4/cmd/glide@latest

# See available commands in your project
glide help

# Install a plugin
glide plugin install docker
```

## Links

- [Documentation](https://github.com/glide-cli/glide#readme)
- [Plugin Development Guide](https://github.com/glide-cli/glide/blob/main/PLUGIN_DEVELOPMENT.md)
- [Contributing](https://github.com/glide-cli/glide/blob/main/CONTRIBUTING.md)

---

*Built with care for developers who value simplicity.*
