# Next.js Specific Rules

When using `useSearchParams()` from `next/navigation` in client components, you **MUST** wrap the component in a Suspense boundary to prevent CSR bailout errors during server-side rendering.