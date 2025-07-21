# Database Rules

- Use Supabase CLI to create DB migrations
- To query the local Supabase DB, use the Supabase MCP server
- When writing code that requires data access (read/write from/to Supabase DB), always go through the lib/db/ layer
- Reuse functions, make functions reusable if needed, or create new functions if needed