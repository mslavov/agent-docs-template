# Documentation Index

**Purpose**: Central navigation hub  
**Project**: [PROJECT_NAME]

## 📋 Quick Start

- **New Projects**: Start with creating PRDs in [`product/`](product/)
- **Existing Projects**: Run `/setup` to analyze and document your codebase
- **Create Issues**: Use `/plan` to create GitHub issues from requirements

## 📋 Documentation

## 🏗️ Architecture
- [`system-overview.md`](system-overview.md) - System architecture

## 📁 Product
- [`product/`](product/) - Product requirements documents (PRDs)
- [`prd/`](prd/) - Additional PRD storage (if needed)

## 🔧 Technical
- [`tech/api-reference.md`](tech/api-reference.md) - API reference
- [`tech/database-reference.md`](tech/database-reference.md) - Database schema

## 📚 Guides
- [`guides/`](guides/) - How-to guides and tutorials

## 🤖 Agent Documentation
- [`agents/`](agents/) - Agent-related documentation (if applicable)

## 📜 Project Management
- [`CHANGELOG.md`](CHANGELOG.md) - Version history
- [`RULES.md`](RULES.md) - Development rules and conventions

## 🛠️ Available Commands

| Command | Purpose |
|---------|---------|  
| `/setup` | Analyze codebase and generate documentation |
| `/plan` | Create GitHub issues from requirements |

## Quick Task Lookup

| Task Type | Primary Doc | Action |
|-----------|------------|--------|
| Initial Project Setup | Run `/setup` command | Auto-generates documentation |
| System Understanding | `system-overview.md` | Review architecture |
| API Development | `tech/api-reference.md` | Check endpoints |
| Database Changes | `tech/database-reference.md` | Review schema |
| Feature Development | `product/` | Create PRD, then `/plan` |
| Bug Investigation | `system-overview.md` | Review tech docs |
| Performance | `system-overview.md` | Check architecture |

## Documentation Best Practices

1. **Start with PRDs** - Define requirements before implementation
2. **Keep Docs Updated** - Documentation should reflect current state
3. **Use Commands** - `/setup` for analysis, `/plan` for issue creation
4. **Organize by Type** - Product docs separate from technical docs