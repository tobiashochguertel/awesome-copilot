# Awesome Copilot Plugin Marketplace

Welcome to the Awesome Copilot Plugin Marketplace! This marketplace provides easy access to community-curated GitHub Copilot customizations including agents, skills, prompts, instructions, and collections.

## 🚀 Quick Start

### Prerequisites

- Claude Code or GitHub Copilot CLI installed
- Basic understanding of GitHub Copilot customizations

### Installation

Add the marketplace to your Claude Code environment:

```shell
/plugin marketplace add github/awesome-copilot
```

Or if you're using your forked version:

```shell
/plugin marketplace add YOUR-USERNAME/awesome-copilot
```

For local testing:

```shell
/plugin marketplace add ./path/to/awesome-copilot
```

## 📦 Available Plugins

### 1. Awesome Agents Collection

Specialized GitHub Copilot agents for various workflows, languages, and frameworks.

```shell
/plugin install awesome-agents-collection@awesome-copilot
```

**Includes:**
- Language-specific experts (C#, Python, Rust, TypeScript, etc.)
- Framework specialists (Azure, .NET, React, Laravel, etc.)
- Workflow agents (DevOps, Security, Testing, etc.)
- MCP integration experts

### 2. Awesome Skills Collection

Self-contained folders with instructions and bundled resources for specialized AI capabilities.

```shell
/plugin install awesome-skills-collection@awesome-copilot
```

**Includes:**
- Azure deployment tools
- GitHub CLI integrations
- Image manipulation utilities
- Testing frameworks
- And many more!

### 3. Awesome Prompts Collection

Task-specific prompts for code generation, documentation, and problem-solving.

```shell
/plugin install awesome-prompts-collection@awesome-copilot
```

**Features:**
- Code generation templates
- Documentation helpers
- Refactoring patterns
- Problem-solving frameworks

### 4. Awesome Instructions Collection

Comprehensive coding standards and best practices for specific file patterns.

```shell
/plugin install awesome-instructions-collection@awesome-copilot
```

**Provides:**
- Language-specific coding standards
- Framework best practices
- Project-wide guidelines
- File pattern rules

### 5. Awesome Collections

Curated collections of related prompts, instructions, agents, and skills organized by themes.

```shell
/plugin install awesome-collections@awesome-copilot
```

**Contains:**
- Copilot SDK collection
- Partner integrations
- Meta prompts for discovery

## 🔧 Usage Examples

### Using an Agent

After installing the agents collection:

```shell
# Activate a specific agent in your chat session
@azure-principal-architect help me design a scalable architecture
```

### Using a Skill

Skills are available as commands:

```shell
# Example: Using the git-commit skill
/git-commit
```

### Using a Prompt

Prompts are accessible via the `/` command:

```shell
/create-readme
/refactor
```

## 🔄 Updating Plugins

Keep your plugins up to date:

```shell
# Update the marketplace
/plugin marketplace update awesome-copilot

# Update specific plugin
/plugin update awesome-agents-collection
```

## 📋 Managing Plugins

### List Installed Plugins

```shell
/plugin list
```

### Enable/Disable Plugins

```shell
# Disable a plugin
/plugin disable awesome-agents-collection

# Enable a plugin
/plugin enable awesome-agents-collection
```

### Uninstall Plugins

```shell
/plugin uninstall awesome-agents-collection@awesome-copilot
```

## 🏢 Team Configuration

For teams, add the marketplace to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "awesome-copilot": {
      "source": {
        "source": "github",
        "repo": "github/awesome-copilot"
      }
    }
  },
  "enabledPlugins": {
    "awesome-agents-collection@awesome-copilot": true,
    "awesome-skills-collection@awesome-copilot": true
  }
}
```

## 🔒 Private Repositories

If you're using a private fork, set your GitHub token:

```bash
export GITHUB_TOKEN=ghp_xxxxxxxxxxxxxxxxxxxx
```

## ✅ Validation

Validate the marketplace configuration:

```bash
# From the repository root
claude plugin validate .

# Or from within Claude Code
/plugin validate .
```

## 🐛 Troubleshooting

### Marketplace Not Loading

1. Verify the marketplace URL is accessible
2. Check that `.claude-plugin/marketplace.json` exists
3. Validate JSON syntax: `claude plugin validate .`
4. For private repos, confirm access permissions

### Plugin Installation Fails

1. Verify plugin source paths are correct
2. Check file permissions
3. For GitHub sources, ensure repositories are accessible
4. Review error messages for specific issues

### Authentication Issues

1. Verify token is set: `echo $GITHUB_TOKEN`
2. Check token has `repo` scope
3. Ensure token hasn't expired

## 📚 Documentation

For detailed information about each type of customization:

- [Agents Documentation](../docs/README.agents.md)
- [Skills Documentation](../docs/README.skills.md)
- [Prompts Documentation](../docs/README.prompts.md)
- [Instructions Documentation](../docs/README.instructions.md)
- [Collections Documentation](../docs/README.collections.md)

## 🤝 Contributing

Want to add your own customizations to the marketplace?

1. See [CONTRIBUTING.md](../CONTRIBUTING.md) for guidelines
2. Review [AGENTS.md](../AGENTS.md) for development workflows
3. Test your contributions thoroughly
4. Submit a pull request

## 📄 License

This marketplace and all included plugins are licensed under the MIT License. See [LICENSE](../LICENSE) for details.

## ℹ️ Disclaimer

The customizations in this marketplace are sourced from and created by third-party developers. GitHub does not verify, endorse, or guarantee the functionality or security of these agents. Please carefully inspect any agent and its documentation before installing.

---

**Need help?** Check our [Support Guide](../SUPPORT.md) or [Security Policy](../SECURITY.md).
