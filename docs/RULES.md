# Package Manager usage
Use pnpm package manager

# Supabase migrations
Use supabase cli to create DB migrations

# To query the local supabase DB, use the supabase mcp server.

# useSearchParams() Suspense Requirement
When using `useSearchParams()` from `next/navigation` in client components, you **MUST** wrap the component in a Suspense boundary to prevent CSR bailout errors during server-side rendering.

# When writing code which requires accessing data (read/write from/to Supabase DB) always go through the lib/db/ layer. Reuse functions, make functions reusable if needed, or meke new functions if needed.

# Task Archive
When a development task is fully completed (all subtasks are checked ✅), **move the task block from `docs/progress.md` to `docs/task-archive.md`** and record the completion date.