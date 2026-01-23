# Quick Start: Plugin Marketplace

Get started with the Awesome Copilot Plugin Marketplace in minutes!

## 🚀 One-Minute Setup

### Step 1: Add the Marketplace

```shell
/plugin marketplace add github/awesome-copilot
```

### Step 2: Install Plugins

Install all collections at once:

```shell
/plugin install awesome-agents-collection@awesome-copilot
/plugin install awesome-skills-collection@awesome-copilot
/plugin install awesome-prompts-collection@awesome-copilot
/plugin install awesome-instructions-collection@awesome-copilot
/plugin install awesome-collections@awesome-copilot
```

Or install just what you need:

```shell
# For AI agents only
/plugin install awesome-agents-collection@awesome-copilot

# For skills only
/plugin install awesome-skills-collection@awesome-copilot
```

### Step 3: Start Using

```shell
# List available agents
@agent list

# Use a specific agent
@azure-principal-architect design a scalable web app

# List available skills
/help

# Use a skill
/git-commit
```

## 📦 What Gets Installed?

### Agents Collection (100+ agents)
- Language experts: C#, Python, Rust, Go, TypeScript, Java, etc.
- Framework specialists: Azure, .NET, React, Angular, Laravel, etc.
- Workflow agents: DevOps, Security, Testing, Planning, etc.
- MCP integration experts for various languages

### Skills Collection (26+ skills)
- Azure deployment tools
- GitHub CLI integrations
- Image manipulation
- Testing frameworks
- Developer utilities

### Prompts Collection
- Code generation templates
- Documentation helpers
- Refactoring patterns
- Problem-solving frameworks

### Instructions Collection
- Language-specific coding standards
- Framework best practices
- Project-wide guidelines
- File pattern rules

### Collections
- Copilot SDK collection
- Partner integrations
- Meta prompts for discovery

## 🔄 Keeping Updated

```shell
# Update the marketplace
/plugin marketplace update awesome-copilot

# Update all plugins
/plugin update

# Update specific plugin
/plugin update awesome-agents-collection
```

## 🏢 Team Setup

Add to your project's `.claude/settings.json`:

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
    "awesome-skills-collection@awesome-copilot": true,
    "awesome-prompts-collection@awesome-copilot": true
  }
}
```

Now team members will be prompted to install when they trust the folder!

## 🎯 Popular Use Cases

### For Backend Developers
```shell
/plugin install awesome-agents-collection@awesome-copilot
# Use: @expert-dotnet-software-engineer, @python-mcp-expert, @java-mcp-expert
```

### For Frontend Developers
```shell
/plugin install awesome-agents-collection@awesome-copilot
# Use: @expert-react-frontend-engineer, @expert-nextjs-developer
```

### For DevOps Engineers
```shell
/plugin install awesome-agents-collection@awesome-copilot
/plugin install awesome-skills-collection@awesome-copilot
# Use: @devops-expert, @github-actions-expert, /azure-deployment-preflight
```

### For Cloud Architects
```shell
/plugin install awesome-agents-collection@awesome-copilot
# Use: @azure-principal-architect, @azure-saas-architect, @terraform-azure-planning
```

## ❓ Common Questions

**Q: Do I need to install all collections?**
A: No! Install only what you need. You can always add more later.

**Q: How do I see what's installed?**
```shell
/plugin list
```

**Q: Can I disable a plugin without uninstalling?**
```shell
/plugin disable awesome-agents-collection
/plugin enable awesome-agents-collection
```

**Q: How do I uninstall?**
```shell
/plugin uninstall awesome-agents-collection@awesome-copilot
```

**Q: Can I use this with private repositories?**
A: Yes! Set your GitHub token:
```bash
export GITHUB_TOKEN=ghp_xxxxxxxxxxxxxxxxxxxx
```

## 📚 Learn More

- **Full Documentation**: [.claude-plugin/README.md](.claude-plugin/README.md)
- **Agents Guide**: [docs/README.agents.md](docs/README.agents.md)
- **Skills Guide**: [docs/README.skills.md](docs/README.skills.md)
- **Prompts Guide**: [docs/README.prompts.md](docs/README.prompts.md)
- **Contributing**: [CONTRIBUTING.md](CONTRIBUTING.md)

## 🆘 Need Help?

- Check the [troubleshooting section](.claude-plugin/README.md#-troubleshooting)
- Review [SUPPORT.md](SUPPORT.md)
- Open an issue on GitHub

---

**Ready to dive deeper?** Check out the [full plugin marketplace documentation](.claude-plugin/README.md)!
