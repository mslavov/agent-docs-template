# Documentation Index

**Last Updated**: [DATE]\
**Purpose**: Central navigation hub for [PROJECT_NAME] documentation

---

## Project Overview

This is a [FRAMEWORK] project built with:

- **Frontend**: [FRONTEND_FRAMEWORK]
- **UI**: [UI_LIBRARY]
- **Backend**: [BACKEND_SERVICE]
- **Analytics**: [ANALYTICS_DESCRIPTION]
- **Package Manager**: [PACKAGE_MANAGER]

---

## Available Documentation

### 📋 **Project Management**

- [`progress.md`](progress.md) - Active task tracking and completion status
- [`task-archive.md`](task-archive.md) - Completed tasks archive
- [`RULES.md`](RULES.md) - Development rules and guidelines

### 🏗️ **Architecture & System**

- [`system-overview.md`](system-overview.md) - Comprehensive system architecture
  and functionality overview

### 📁 **Product Documentation**

- [`product/`](product/) - Product requirements, specifications, and user-facing
  documentation

### 🔧 **Technical Reference**

- [`tech/api-reference.md`](tech/api-reference.md) - API functions and data
  operations
- [`tech/database-reference.md`](tech/database-reference.md) - Database schema
  and configuration

### 🧪 **Core Features**

- **[Feature 1]**: [Description]
- **[Feature 2]**: [Description]
- **[Feature 3]**: [Description]
- **[Feature 4]**: [Description]
- **[Feature 5]**: [Description]

### 🔗 **Key Components**

- `[Component1]` - [Description]
- `[Component2]` - [Description]
- `[Component3]` - [Description]
- `[Component4]` - [Description]

---

## Current Project Structure

```
[project-name]/
├── app/                    # [Framework] app router
│   ├── globals.css        # Global styles
│   ├── layout.tsx         # App layout
│   └── page.tsx           # Main page
├── components/            # React components
│   ├── ui/                # [UI Library] components
│   ├── [component1].tsx   # [Description]
│   ├── [component2].tsx   # [Description]
│   ├── [component3].tsx   # [Description]
│   └── [component4].tsx   # [Description]
├── lib/                   # Utility libraries
│   ├── [service]/        # [Service] configuration
│   └── utils.ts          # General utilities
├── utils/                # [Domain] utilities
│   └── [domain].ts       # Core [domain] algorithms
├── data/                 # Mock/test data
│   └── mock-[data].ts    # Sample data
└── docs/                 # Documentation
    ├── INDEX.md          # This file
    ├── system-overview.md # System architecture
    ├── progress.md       # Task tracking
    ├── task-archive.md   # Completed tasks
    ├── RULES.md          # Development rules
    ├── product/          # Product documentation
    └── tech/             # Technical references
        ├── api-reference.md
        └── database-reference.md
```

---

## Development Guidelines

**Key Rules** (from [`RULES.md`](RULES.md)):

- Use [PACKAGE_MANAGER] as the package manager
- Use [DATABASE_CLI] for database migrations
- [FRAMEWORK_SPECIFIC_RULE]
- Route database access through `lib/db/` layer
- Archive completed tasks from `progress.md` to `task-archive.md`

---

## Getting Started

1. **Install dependencies**: `[INSTALL_COMMAND]`
2. **Set up [SERVICE]**: Configure your [SERVICE] project
3. **Run development server**: `[DEV_COMMAND]`
4. **Access the application**: Navigate to the main interface

---

## Status

**Documentation Status**: 🔄 [STATUS_DESCRIPTION]\
**Project Status**: [PROJECT_STATUS]

## Core Functionality

- **[Function 1]**: [Description]
- **[Function 2]**: [Description]
- **[Function 3]**: [Description]
- **[Function 4]**: [Description]
- **[Function 5]**: [Description]

---

## Quick Task Lookup

### Common Development Tasks

| Task Type            | Documents to Read                        | Action Required                   |
| -------------------- | ---------------------------------------- | --------------------------------- |
| System Understanding | `system-overview.md`                     | Review architecture               |
| API Development      | `tech/api-reference.md`                  | Check existing endpoints          |
| Database Changes     | `tech/database-reference.md`, `RULES.md` | Follow migration rules            |
| Feature Development  | `product/` docs, `progress.md`           | Check requirements & status       |
| Bug Investigation    | `system-overview.md`, relevant tech docs | Understand data flow              |
| Performance Issues   | `system-overview.md`                     | Review architecture & limitations |

### Documentation Updates

| Change Type     | Primary Document                  | Secondary Updates              |
| --------------- | --------------------------------- | ------------------------------ |
| New Feature     | `system-overview.md`              | `INDEX.md`, relevant tech docs |
| API Changes     | `tech/api-reference.md`           | `system-overview.md`           |
| Database Schema | `tech/database-reference.md`      | `system-overview.md`           |
| Task Completion | `progress.md` → `task-archive.md` | Update completion date         |

---

**Quick Navigation:**

- 📋 [Task Progress](progress.md)
- 📜 [Development Rules](RULES.md)
- 🏗️ [System Overview](system-overview.md)
- 📁 [Product Documentation](product/)
- 🔗 [API Reference](tech/api-reference.md)
- 🗄️ [Database Reference](tech/database-reference.md)
- 📚 [Completed Tasks](task-archive.md)
