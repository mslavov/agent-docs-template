# Agent Documentation Template

A structured documentation template system designed for AI-assisted software
development, optimized for use with Claude and other AI agents.

## Overview

This template provides a comprehensive documentation framework that helps
maintain organized, consistent, and AI-friendly project documentation. It
includes predefined structures, workflows, and guidelines that enable AI agents
to quickly understand and navigate your project.

## Key Features

- **AI-Agent Optimized**: Specifically designed with clear protocols for AI
  agents like Claude
- **Structured Workflow**: Pre-Task and Post-Task protocols ensure consistent
  documentation practices
- **Template-Based Approach**: Ready-to-use templates for common documentation
  needs
- **Task Management**: Built-in progress tracking and task archival system
- **Cross-Referenced Documentation**: Organized documentation with clear
  navigation paths
- **Development Rules**: Centralized location for project-specific guidelines

## Getting Started

1. **Copy this template** to your project repository
2. **Review CLAUDE.md or AGENTS.md** for AI agent usage guidelines
3. **Start with docs/RULES.md** to understand project-specific rules
4. **Ask your AI agent to generate initial documentation** - Use this prompt:
   ```
   Please analyze this project and generate initial documentation by:
   1. Examining the codebase structure and identifying key components
   2. Filling out docs/INDEX.md with actual project details
   3. Updating docs/system-overview.md with the real architecture
   4. Creating initial entries in docs/progress.md for any TODOs found
   5. Populating docs/tech/api-reference.md and database-reference.md if applicable
   Replace all [PLACEHOLDER] values with actual project information.
   ```
5. **Review and refine** the generated documentation
6. **Continue customizing** as your project evolves

## Documentation Structure

```
agent-docs-template/
├── README.md              # This file
├── AGENTS.md              # AI agent usage guidelines
├── CLAUDE.md              # Claude-specific guidelines (identical to AGENTS.md)
├── claude.json            # Claude Desktop MCP configuration
├── .claude/               # Claude Code configuration
│   └── claude_project.json # Project context and MCP settings
├── .cursor/               # Cursor configuration
│   └── mcp.json          # Cursor MCP server configuration
└── docs/
    ├── INDEX.md           # Central navigation hub (customize this first!)
    ├── RULES.md           # Development rules and guidelines
    ├── progress.md        # Active task tracking
    ├── task-archive.md    # Completed tasks archive
    ├── system-overview.md # System architecture template
    ├── product/           # Product documentation directory
    └── tech/              # Technical documentation
        ├── api-reference.md      # API documentation template
        └── database-reference.md # Database schema template
```

## Workflow Guide

### Pre-Task Protocol

When starting any development task:

1. **Always start with `docs/RULES.md`** - Review project-specific rules and
   guidelines
2. **Check `docs/INDEX.md`** - Navigate to relevant documentation
3. **Use Quick Task Lookup** - Find specific documents for your task type
4. **Consult relevant docs** - Read product specs and technical references as
   needed

### Post-Task Protocol

After completing work:

1. **Update documentation** - Modify the single source of truth for any changes
2. **Update cross-references** - Ensure all related documents reflect changes
3. **Mark task completion** - Update status in `docs/progress.md`
4. **Archive if complete** - Move finished tasks to `docs/task-archive.md`
5. **Update INDEX.md** - Add any new documents created

## Template Customization

### Replacing Placeholders

All templates contain placeholders marked with `[PLACEHOLDER_NAME]`. Common ones
include:

- `[PROJECT_NAME]` - Your project's name
- `[DATE]` - Current date in YYYY-MM-DD format
- `[FRAMEWORK]` - Primary framework (e.g., Next.js, React, Vue)
- `[PACKAGE_MANAGER]` - npm, yarn, or pnpm
- `[DATABASE_SERVICE]` - Supabase, PostgreSQL, etc.

### Customizing Templates

1. **docs/INDEX.md** - This should be your first customization
   - Update project overview
   - List actual features and components
   - Modify directory structure to match your project

2. **docs/system-overview.md** - Comprehensive architecture documentation
   - Replace architecture diagram with your system design
   - Document actual data flows and structures
   - Update implementation status

3. **docs/RULES.md** - Add your project-specific rules
   - Development standards
   - Code style guidelines
   - Workflow requirements

## Best Practices

### For AI Agents

- Always start with RULES.md and INDEX.md
- Follow the Pre-Task and Post-Task protocols
- Update documentation in real-time as changes are made
- Use the task tracking system in progress.md
- Maintain single sources of truth

### For Human Developers

- Keep templates up-to-date with project changes
- Archive completed tasks regularly
- Use consistent naming conventions
- Document decisions and rationale
- Cross-reference related documentation

## Integration with AI Tools

### Claude Code (MCP)

This template includes MCP (Model Context Protocol) configuration for Claude
Code. When using Claude Code:

1. The `.claude/claude_project.json` file provides project context
2. Claude will automatically follow the documentation protocols
3. Multiple MCP servers are pre-configured:
   - **Supabase**: For database operations (requires credentials)
   - **Context7**: For enhanced context management
   - **Browser Tools**: For web automation and testing

### Cursor Integration

The template also includes Cursor-specific MCP configuration in
`.cursor/mcp.json` with the same MCP servers available for Cursor users.

### Other AI Agents

The AGENTS.md file provides universal guidelines that work with any AI coding
assistant. The structured approach ensures consistent behavior across different
AI tools.

## Task Management

### Progress Tracking

Use `docs/progress.md` with the following legend:

- ✅ Completed
- 🔄 In Progress
- 📋 Planned

### Task Archival

When tasks are fully completed:

1. Move the entire task block from `progress.md`
2. Add it to `task-archive.md` with completion date
3. Maintain chronological order in the archive

## Example Usage

### Starting a New Feature

```markdown
1. AI reads docs/RULES.md
2. AI checks docs/INDEX.md for existing documentation
3. AI reviews product requirements in docs/product/
4. AI implements feature following guidelines
5. AI updates docs/system-overview.md with new components
6. AI marks task as ✅ in docs/progress.md
```

### Debugging an Issue

```markdown
1. AI consults docs/system-overview.md for architecture
2. AI checks docs/tech/api-reference.md for endpoints
3. AI reviews docs/tech/database-reference.md for schema
4. AI fixes issue following patterns in codebase
5. AI documents the fix in relevant locations
```

## Contributing

To improve this template:

1. Maintain clarity for AI agents
2. Keep documentation DRY (Don't Repeat Yourself)
3. Ensure templates are generic enough for various projects
4. Add examples where helpful
5. Test with AI agents to ensure usability

## License

This template is provided as-is for use in your projects. Customize and adapt as
needed for your specific requirements.
