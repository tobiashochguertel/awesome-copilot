# Changelog

All notable changes to the Awesome Copilot project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-01-23

### Added

- **Claude Code Plugin Marketplace Support**: Implemented a complete plugin marketplace infrastructure
  - Created `.claude-plugin/marketplace.json` with 5 plugin collections
  - Added comprehensive marketplace documentation in `.claude-plugin/README.md`
  - Organized existing content (agents, skills, prompts, instructions, collections) as installable plugins
  - Users can now install customizations via `/plugin install` commands
  
- **Plugin Collections**:
  - `awesome-agents-collection`: 100+ specialized GitHub Copilot agents
  - `awesome-skills-collection`: 26+ self-contained skills with bundled resources
  - `awesome-prompts-collection`: Task-specific prompts for code generation
  - `awesome-instructions-collection`: Coding standards and best practices
  - `awesome-collections`: Curated themed collections

### Changed

- Updated main README.md to include Plugin Marketplace quick start section
- Enhanced discoverability with marketplace installation commands

### Features

- Easy installation: `/plugin marketplace add github/awesome-copilot`
- Version tracking and automatic updates
- Team configuration support via `.claude/settings.json`
- Private repository support with GitHub token authentication
- Validation tools for marketplace configuration

### Documentation

- Comprehensive marketplace usage guide
- Installation and configuration examples
- Troubleshooting section
- Team deployment instructions

---

## Guidelines for Contributors

When adding new features or customizations:

1. Update the appropriate plugin collection in `.claude-plugin/marketplace.json`
2. Document changes in this CHANGELOG
3. Test installation via the plugin marketplace
4. Update relevant documentation in docs/

For marketplace-related changes:
- Validate with: `claude plugin validate .` or `/plugin validate .`
- Test locally: `/plugin marketplace add ./path/to/awesome-copilot`
- Ensure all plugin sources are accessible
