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
