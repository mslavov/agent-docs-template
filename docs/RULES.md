# Development Rules

These rules ensure consistent development practices across all agents and team
members.

## Core Development Rules

### Package Manager

Use pnpm package manager

### Database

- Use Supabase CLI to create DB migrations
- To query the local Supabase DB, use the Supabase MCP server
- When writing code that requires data access (read/write from/to Supabase DB),
  always go through the lib/db/ layer
- Reuse functions, make functions reusable if needed, or create new functions if
  needed

### Next.js Specific

When using `useSearchParams()` from `next/navigation` in client components, you
**MUST** wrap the component in a Suspense boundary to prevent CSR bailout errors
during server-side rendering.

## MCP Server Usage Rules

### Available MCP Servers

The project has the following MCP servers configured:

1. **context7** (`@upstash/context7-mcp`)
   - Purpose: Context management and retrieval
   - Use this for managing and accessing project context information

2. **browser-tools** (`@agentdeskai/browser-tools-mcp`)
   - Purpose: Web automation and browser interaction
   - Use this for tasks requiring web scraping, automation, or browser control

### MCP Server Usage Guidelines

1. **Always check server availability**: Before using an MCP server, verify it's
   enabled in the environment
2. **Use appropriate server for the task**: Choose the MCP server that best
   matches your task requirements
3. **Follow server documentation**: Each MCP server has specific capabilities
   and limitations - consult their documentation
4. **Error handling**: Always handle potential failures when using MCP servers
   gracefully
