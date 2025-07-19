# Multi-Agent Development System

## 🚨 CRITICAL: Framework-First Reading Order

**ALL AGENTS MUST FOLLOW THIS READING ORDER:**
1. **FIRST**: Read [`docs/RULES.md`](docs/RULES.md) - Framework rules and development guidelines
2. **SECOND**: Read [`docs/INDEX.md`](docs/INDEX.md) - Documentation navigation hub
3. **THIRD**: Read your specific agent definition in [`docs/agents/`](docs/agents/)
4. **THEN**: Consult project-specific documentation as needed

This ensures you understand the framework and rules before diving into specific tasks.

---

This document provides an overview of the multi-agent development system. For detailed agent specifications, see the individual agent definition files in `docs/agents/`.

## System Overview

The multi-agent system divides development work into specialized roles, enabling parallel execution and clear separation of concerns. Each agent has specific responsibilities and interacts through a file-based task management system.

## Agent Roles

### 1. [Architect Agent](docs/agents/architect.md) (`/architect`)
- **Purpose**: Transform product requirements into technical designs
- **Input**: PRDs from `docs/prd/`
- **Output**: Architecture documents in `scratch/`

### 2. [Planner Agent](docs/agents/planner.md) (`/planner`)
- **Purpose**: Break down features into implementable tasks
- **Input**: PRD + Architecture notes
- **Output**: Task files in `tasks/todo/`

### 3. [Developer Agent](docs/agents/developer.md) (`/developer`)
- **Purpose**: Implement specific tasks
- **Input**: Tasks from `tasks/todo/`
- **Output**: Code + completed tasks in `tasks/done/`

### 4. [Testing Agent](docs/agents/tester.md) (`/tester`)
- **Purpose**: Validate completed implementations
- **Input**: Tasks in `tasks/done/`
- **Output**: Test results, failed tasks back to `tasks/todo/`

### 5. [Documentation Agent](docs/agents/docs-agent.md) (`/docs-agent`)
- **Purpose**: Keep documentation synchronized with code
- **Input**: Completed tasks and code changes
- **Output**: Updated documentation

### 6. [Project Manager Agent](docs/agents/pm.md) (`/pm`)
- **Purpose**: Track progress and manage workflow
- **Input**: Task folder structure
- **Output**: Status reports, dependency management

## Workflow Overview

```
PRD → Architect → Planner → Developer(s) → Tester → Docs
                                ↑
                                PM (monitors throughout)
```

1. **Start**: Create PRD in `docs/prd/`
2. **Design**: Architect creates technical design
3. **Plan**: Planner breaks down into tasks
4. **Develop**: Multiple developers work in parallel
5. **Test**: Tester validates implementations
6. **Document**: Docs agent updates documentation
7. **Track**: PM monitors progress throughout

## Task Management

Tasks flow through a simple folder structure:
```
tasks/
├── todo/         # Available tasks
├── in-progress/  # Active work
├── done/         # Completed tasks
└── archive/      # Historical tasks
```

Each task is a markdown file with metadata tracking dependencies, assignees, and status.

## Command Quick Reference

### Claude Slash Commands
- `/architect` - Design architecture
- `/planner` - Create tasks  
- `/developer` - Implement tasks
- `/tester` - Test completed work
- `/docs-agent` - Update documentation
- `/pm status` - Get progress report
- `/pm archive` - Archive old tasks

### Cursor @ Commands
- `@architect` - Architecture assistance
- `@planner` - Task planning help
- `@developer` - Development guidance
- `@tester` - Testing support
- `@docs-agent` - Documentation help
- `@pm` - Project management

## Key Principles

1. **Specialized Roles** - Each agent has a specific focus
2. **File-Based Communication** - Agents coordinate through files
3. **Parallel Execution** - Multiple agents work simultaneously
4. **Clear Dependencies** - Tasks explicitly define prerequisites
5. **Continuous Documentation** - Docs stay in sync with code

## Getting Started

1. **Identify Your Role** - Which agent are you?
2. **Read Your Definition** - See `docs/agents/[agent-name].md`
3. **Follow the Workflow** - Use your agent's specific process
4. **Coordinate via Tasks** - Use the task system for handoffs
5. **Keep Docs Current** - Update as you work

## Best Practices

- One task at a time per agent
- Check dependencies before starting
- Update task metadata when claiming/completing
- Document blockers in task files
- Follow project rules in `docs/RULES.md`

Remember: Each agent should refer to their detailed definition file in `docs/agents/` for complete guidelines, workflows, and examples.